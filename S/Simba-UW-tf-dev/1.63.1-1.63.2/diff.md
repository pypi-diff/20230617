# Comparing `tmp/Simba-UW-tf-dev-1.63.1.tar.gz` & `tmp/Simba-UW-tf-dev-1.63.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.63.1.tar", last modified: Thu Jun 15 20:11:18 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.63.2.tar", last modified: Sat Jun 17 19:11:47 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.63.1.tar` & `Simba-UW-tf-dev-1.63.2.tar`

### file list

```diff
@@ -1,548 +1,559 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.63.1/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-23 15:42:32.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5814 2023-06-15 20:06:37.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.63.1/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.63.1/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.63.1/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.63.1/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    35431 2023-06-13 17:24:57.000000 Simba-UW-tf-dev-1.63.1/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.63.1/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.63.1/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20688 2023-06-11 20:18:17.000000 Simba-UW-tf-dev-1.63.1/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.63.1/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26931 2023-05-24 17:01:48.000000 Simba-UW-tf-dev-1.63.1/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.63.1/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.63.1/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.63.1/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.63.1/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.1/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.1/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.1/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9846 2023-06-06 18:27:30.000000 Simba-UW-tf-dev-1.63.1/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.1/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.63.1/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.63.1/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.1/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.63.1/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10287 2023-06-06 17:50:12.000000 Simba-UW-tf-dev-1.63.1/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.63.1/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.1/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.63.1/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.63.1/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.63.1/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.63.1/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.1/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.1/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.63.1/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-07 20:28:11.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/shap_log_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/shap_log_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    30764 2023-06-13 17:23:34.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/read_files_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.63.1/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.63.1/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43029 2023-06-05 17:40:09.000000 Simba-UW-tf-dev-1.63.1/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    38224 2023-06-15 15:41:52.000000 Simba-UW-tf-dev-1.63.1/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.63.1/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.63.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.63.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.63.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.63.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.63.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.63.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.63.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    37135 2023-06-02 12:12:15.000000 Simba-UW-tf-dev-1.63.1/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.63.1/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     9145 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.63.1/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    73254 2023-06-07 20:39:22.000000 Simba-UW-tf-dev-1.63.1/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.63.1/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10759 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.63.1/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.1/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    18001 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.63.1/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.63.1/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18559 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.63.1/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.63.1/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.63.1/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.63.1/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.63.1/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.1/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.1/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.1/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.1/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.63.1/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.1/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.63.1/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    21017 2023-06-05 18:05:35.000000 Simba-UW-tf-dev-1.63.1/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.63.1/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7396 2023-06-01 13:09:55.000000 Simba-UW-tf-dev-1.63.1/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.63.1/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    43061 2023-05-25 14:56:03.000000 Simba-UW-tf-dev-1.63.1/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     8585 2023-06-05 17:07:45.000000 Simba-UW-tf-dev-1.63.1/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.63.1/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.63.1/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    19250 2023-06-13 13:46:20.000000 Simba-UW-tf-dev-1.63.1/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.63.1/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.63.1/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.63.1/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.63.1/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5618 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.63.1/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     6774 2023-06-15 19:18:29.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    14029 2023-06-04 11:55:47.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7661 2023-06-15 20:00:19.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/pose_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.1/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.63.1/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.63.1/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16285 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.63.1/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.63.1/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12938 2023-05-23 20:14:45.000000 Simba-UW-tf-dev-1.63.1/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.63.1/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.63.1/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.63.1/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.63.1/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.63.1/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.63.1/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.63.1/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.63.1/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.63.1/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    20086 2023-06-05 20:43:28.000000 Simba-UW-tf-dev-1.63.1/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.63.1/simba/model/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.63.1/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.63.1/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.63.1/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.63.1/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20174 2023-06-12 15:28:58.000000 Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)     2290 2023-06-12 16:21:03.000000 Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11474 2023-06-12 19:37:22.000000 Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.63.1/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.63.1/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.63.1/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.63.1/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.63.1/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.63.1/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.63.1/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.63.1/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.63.1/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.1/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.63.1/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    45563 2023-06-09 13:51:45.000000 Simba-UW-tf-dev-1.63.1/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.63.1/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.63.1/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.63.1/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.63.1/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.63.1/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.63.1/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.63.1/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.63.1/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.63.1/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.63.1/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.63.1/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.63.1/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    65762 2023-06-10 19:40:55.000000 Simba-UW-tf-dev-1.63.1/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.63.1/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.63.1/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.63.1/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.63.1/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.63.1/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.63.1/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.63.1/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.63.1/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.1/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    20220 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)       12 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.63.1/LICENSE.md
--rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.63.1/pyproject.toml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/tests/
--rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.63.1/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.63.1/tests/test_distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.63.1/tests/test_interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)    12374 2023-06-07 20:44:17.000000 Simba-UW-tf-dev-1.63.1/tests/test_train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     2470 2023-06-12 20:51:29.000000 Simba-UW-tf-dev-1.63.1/tests/test_pose_importers.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.1/tests/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.63.1/tests/test_feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-12 20:53:51.000000 Simba-UW-tf-dev-1.63.1/tests/test_pose_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     1774 2023-06-13 19:27:04.000000 Simba-UW-tf-dev-1.63.1/tests/test_utils_data.py
--rw-r--r--   0 simon      (501) staff       (20)     8984 2023-06-07 20:11:11.000000 Simba-UW-tf-dev-1.63.1/tests/test_config_reader_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.63.1/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.63.1/tests/test_visualize_directing_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.63.1/tests/test_featurizers.py
--rw-r--r--   0 simon      (501) staff       (20)     8736 2023-06-13 13:49:50.000000 Simba-UW-tf-dev-1.63.1/tests/test_video_processors.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/tests/data/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.1/tests/data/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/two_c57/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/two_c57/video_processing/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/two_c57/video_processing/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/two_c57/video_processing/test_imgs/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/two_c57/video_processing/test_imgs/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/two_c57/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/two_c57/models/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/two_c57/models/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/two_c57/expected_animal_bp_dict/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/two_c57/expected_animal_bp_dict/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/mouse_open_field/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/mouse_open_field/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/zebrafish/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/zebrafish/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/zebrafish/models/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/zebrafish/models/generated_models/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/zebrafish/models/generated_models/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/zebrafish/models/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/zebrafish/models/validations/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/zebrafish/models/validations/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/zebrafish/project_folder/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/zebrafish/project_folder/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/zebrafish/project_folder/videos/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/zebrafish/project_folder/videos/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/zebrafish/project_folder/logs/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/zebrafish/project_folder/logs/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/zebrafish/project_folder/logs/measures/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/zebrafish/project_folder/logs/measures/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/zebrafish/feature_file/
--rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/zebrafish/feature_file/__init__.py
--rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.63.1/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
--rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.63.1/tests/test_thirdparty_appenders.py
--rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.63.1/tests/test_validation_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     4463 2023-06-12 18:41:18.000000 Simba-UW-tf-dev-1.63.1/tests/test_roi_tools.py
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.63.1/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.63.1/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-06-15 20:10:47.000000 Simba-UW-tf-dev-1.63.1/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-15 20:11:18.000000 Simba-UW-tf-dev-1.63.1/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.2/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5814 2023-06-15 20:06:37.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.63.2/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.63.2/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.63.2/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.63.2/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    35431 2023-06-13 17:24:57.000000 Simba-UW-tf-dev-1.63.2/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.63.2/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.2/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20688 2023-06-11 20:18:17.000000 Simba-UW-tf-dev-1.63.2/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.63.2/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26931 2023-05-24 17:01:48.000000 Simba-UW-tf-dev-1.63.2/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.63.2/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.63.2/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.63.2/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.63.2/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.2/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.2/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.2/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9846 2023-06-06 18:27:30.000000 Simba-UW-tf-dev-1.63.2/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.2/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.63.2/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.63.2/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.2/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.63.2/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10287 2023-06-06 17:50:12.000000 Simba-UW-tf-dev-1.63.2/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.63.2/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.2/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.2/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.63.2/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.63.2/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.63.2/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.2/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.2/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-06-17 19:01:05.000000 Simba-UW-tf-dev-1.63.2/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-07 20:28:11.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/shap_log_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/shap_log_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    30764 2023-06-13 17:23:34.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/read_files_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.63.2/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.2/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43029 2023-06-05 17:40:09.000000 Simba-UW-tf-dev-1.63.2/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    38224 2023-06-15 15:41:52.000000 Simba-UW-tf-dev-1.63.2/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.63.2/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.63.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.63.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.63.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.63.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.63.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.63.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.63.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    37135 2023-06-02 12:12:15.000000 Simba-UW-tf-dev-1.63.2/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.63.2/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     9145 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.63.2/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    73254 2023-06-07 20:39:22.000000 Simba-UW-tf-dev-1.63.2/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.63.2/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10759 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.63.2/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.2/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.2/simba/third_party_label_appenders/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    18001 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.63.2/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.63.2/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18559 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.63.2/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.63.2/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.63.2/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.63.2/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:37.000000 Simba-UW-tf-dev-1.63.2/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.2/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.2/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.2/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.2/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.63.2/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.2/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.63.2/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    21105 2023-06-17 18:47:23.000000 Simba-UW-tf-dev-1.63.2/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-17 19:01:05.000000 Simba-UW-tf-dev-1.63.2/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7497 2023-06-17 18:47:23.000000 Simba-UW-tf-dev-1.63.2/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.63.2/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    43061 2023-05-25 14:56:03.000000 Simba-UW-tf-dev-1.63.2/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     9338 2023-06-17 18:35:53.000000 Simba-UW-tf-dev-1.63.2/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.63.2/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.63.2/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    19250 2023-06-13 13:46:20.000000 Simba-UW-tf-dev-1.63.2/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.63.2/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/st/
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-06-16 17:26:25.000000 Simba-UW-tf-dev-1.63.2/simba/st/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 13:55:39.000000 Simba-UW-tf-dev-1.63.2/simba/st/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2105 2023-06-16 19:56:36.000000 Simba-UW-tf-dev-1.63.2/simba/st/select_groups_pg.py
+-rw-r--r--   0 simon      (501) staff       (20)     2245 2023-06-17 15:40:08.000000 Simba-UW-tf-dev-1.63.2/simba/st/aggregate_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     1485 2023-06-16 18:20:31.000000 Simba-UW-tf-dev-1.63.2/simba/st/app.py
+-rw-r--r--   0 simon      (501) staff       (20)      249 2023-06-16 18:20:19.000000 Simba-UW-tf-dev-1.63.2/simba/st/welcome_page.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.63.2/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.63.2/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.2/simba/pose_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.63.2/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5618 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.63.2/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     6774 2023-06-15 19:18:29.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    14029 2023-06-04 11:55:47.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7661 2023-06-15 20:00:19.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/pose_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.2/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/dash_app/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 12:50:41.000000 Simba-UW-tf-dev-1.63.2/simba/dash_app/plotly_dash.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.63.2/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.2/simba/data_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.63.2/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16285 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.63.2/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.63.2/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12938 2023-05-23 20:14:45.000000 Simba-UW-tf-dev-1.63.2/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.63.2/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.63.2/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.63.2/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.63.2/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.63.2/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.63.2/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.63.2/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.63.2/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.63.2/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    20086 2023-06-05 20:43:28.000000 Simba-UW-tf-dev-1.63.2/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:37.000000 Simba-UW-tf-dev-1.63.2/simba/model/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.63.2/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.63.2/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.63.2/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.2/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20174 2023-06-12 15:28:58.000000 Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)     2290 2023-06-12 16:21:03.000000 Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11474 2023-06-12 19:37:22.000000 Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.63.2/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.63.2/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.63.2/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.63.2/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:37.000000 Simba-UW-tf-dev-1.63.2/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.63.2/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.63.2/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.63.2/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.63.2/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.2/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.63.2/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    45563 2023-06-09 13:51:45.000000 Simba-UW-tf-dev-1.63.2/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.2/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.63.2/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.63.2/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.63.2/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.63.2/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.63.2/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.63.2/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.63.2/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.63.2/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:37.000000 Simba-UW-tf-dev-1.63.2/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.63.2/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.63.2/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    66084 2023-06-17 19:01:00.000000 Simba-UW-tf-dev-1.63.2/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-15 21:18:05.000000 Simba-UW-tf-dev-1.63.2/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-06-17 18:48:05.000000 Simba-UW-tf-dev-1.63.2/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.63.2/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.63.2/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.63.2/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.63.2/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.63.2/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.63.2/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.2/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    20500 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       12 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-06-17 19:11:46.000000 Simba-UW-tf-dev-1.63.2/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.63.2/LICENSE.md
+-rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.63.2/pyproject.toml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.63.2/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.63.2/tests/test_distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.63.2/tests/test_interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)    12374 2023-06-07 20:44:17.000000 Simba-UW-tf-dev-1.63.2/tests/test_train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     2470 2023-06-12 20:51:29.000000 Simba-UW-tf-dev-1.63.2/tests/test_pose_importers.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.2/tests/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.63.2/tests/test_feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-12 20:53:51.000000 Simba-UW-tf-dev-1.63.2/tests/test_pose_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1774 2023-06-13 19:27:04.000000 Simba-UW-tf-dev-1.63.2/tests/test_utils_data.py
+-rw-r--r--   0 simon      (501) staff       (20)     8984 2023-06-07 20:11:11.000000 Simba-UW-tf-dev-1.63.2/tests/test_config_reader_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.63.2/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.63.2/tests/test_visualize_directing_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.63.2/tests/test_featurizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     8736 2023-06-13 13:49:50.000000 Simba-UW-tf-dev-1.63.2/tests/test_video_processors.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/tests/data/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.2/tests/data/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/two_c57/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/two_c57/video_processing/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/two_c57/video_processing/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/two_c57/video_processing/test_imgs/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/two_c57/video_processing/test_imgs/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/two_c57/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/two_c57/models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/two_c57/models/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/two_c57/expected_animal_bp_dict/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/two_c57/expected_animal_bp_dict/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/mouse_open_field/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/mouse_open_field/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/zebrafish/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/zebrafish/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/zebrafish/models/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/zebrafish/models/generated_models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/zebrafish/models/generated_models/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/zebrafish/models/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/zebrafish/models/validations/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/zebrafish/models/validations/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/zebrafish/project_folder/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/zebrafish/project_folder/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/zebrafish/project_folder/videos/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/zebrafish/project_folder/videos/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/zebrafish/project_folder/logs/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/zebrafish/project_folder/logs/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/zebrafish/project_folder/logs/measures/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/zebrafish/project_folder/logs/measures/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/zebrafish/feature_file/
+-rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/zebrafish/feature_file/__init__.py
+-rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.63.2/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
+-rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.63.2/tests/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.63.2/tests/test_validation_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     4463 2023-06-12 18:41:18.000000 Simba-UW-tf-dev-1.63.2/tests/test_roi_tools.py
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.63.2/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.63.2/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-06-17 19:11:37.000000 Simba-UW-tf-dev-1.63.2/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-17 19:11:47.000000 Simba-UW-tf-dev-1.63.2/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.63.1/PKG-INFO` & `Simba-UW-tf-dev-1.63.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.63.1
+Version: 1.63.2
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/ui/.DS_Store`

 * *Files 6% similar despite different names*

```diff
@@ -253,23 +253,23 @@
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 000c 0000 000b  ................
 00001010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00001030: 0000 0000 e125 0000 000b 005f 005f 0070  .....%....._._.p
+00001030: 0000 0001 c1a1 0000 000b 005f 005f 0070  ..........._._.p
 00001040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00001050: 6d6f 4444 626c 6f62 0000 0008 cf7e c4bf  moDDblob.....~..
-00001060: 2d17 c541 0000 000b 005f 005f 0070 0079  -..A....._._.p.y
+00001050: 6d6f 4444 626c 6f62 0000 0008 bcee b1bf  moDDblob........
+00001060: 1b1f c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 00001070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00001080: 6444 626c 6f62 0000 0008 cf7e c4bf 2d17  dDblob.....~..-.
+00001080: 6444 626c 6f62 0000 0008 bcee b1bf 1b1f  dDblob..........
 00001090: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000010a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000010b0: 636f 6d70 0000 0000 0001 1000 0000 0007  comp............
+000010b0: 636f 6d70 0000 0000 0002 2000 0000 0007  comp...... .....
 000010c0: 0070 006f 0070 005f 0075 0070 0073 6277  .p.o.p._.u.p.sbw
 000010d0: 7370 626c 6f62 0000 00ca 6270 6c69 7374  spblob....bplist
 000010e0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 000010f0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 00001100: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
 00001110: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
 00001120: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
@@ -278,15 +278,15 @@
 00001150: 6261 7208 0809 0809 5f10 197b 7b33 3534  bar....._..{{354
 00001160: 2c20 3132 347d 2c20 7b31 3037 362c 2036  , 124}, {1076, 6
 00001170: 3231 7d7d 0908 1725 313d 4960 6d79 7a7b  21}}...%1=I`myz{
 00001180: 7c7d 7e9a 0000 0000 0000 0101 0000 0000  |}~.............
 00001190: 0000 000f 0000 0000 0000 0000 0000 0000  ................
 000011a0: 0000 009b 0000 0007 0070 006f 0070 005f  .........p.o.p._
 000011b0: 0075 0070 0073 6c67 3153 636f 6d70 0000  .u.p.slg1Scomp..
-000011c0: 0000 0007 4a53 0000 0007 0070 006f 0070  ....JS.....p.o.p
+000011c0: 0000 000a 7f9b 0000 0007 0070 006f 0070  ...........p.o.p
 000011d0: 005f 0075 0070 0073 6c73 7643 626c 6f62  ._.u.p.slsvCblob
 000011e0: 0000 02b8 6270 6c69 7374 3030 da01 0203  ....bplist00....
 000011f0: 0405 0607 0809 0a0b 0c0d 1848 4948 4a0c  ...........HIHJ.
 00001200: 4c5f 1012 7669 6577 4f70 7469 6f6e 7356  L_..viewOptionsV
 00001210: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
 00001220: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
 00001230: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
@@ -369,20 +369,20 @@
 00001700: 7b01 7c01 7e01 8701 8801 8a01 8b01 8d01  {.|.~...........
 00001710: 9601 9701 9901 9a01 9c01 a501 a601 a801  ................
 00001720: a901 ab01 b401 b501 b801 b901 bb01 bc01  ................
 00001730: c501 ce01 db01 dc00 0000 0000 0002 0100  ................
 00001740: 0000 0000 0000 4c00 0000 0000 0000 0000  ......L.........
 00001750: 0000 0000 0001 e500 0000 0700 7000 6f00  ............p.o.
 00001760: 7000 5f00 7500 7000 736d 6f44 4462 6c6f  p._.u.p.smoDDblo
-00001770: 6200 0000 08cd a621 2ed8 13c5 4100 0000  b......!....A...
+00001770: 6200 0000 08f5 31c6 66d3 1dc5 4100 0000  b.....1.f...A...
 00001780: 0700 7000 6f00 7000 5f00 7500 7000 736d  ..p.o.p._.u.p.sm
-00001790: 6f64 4462 6c6f 6200 0000 08cd a621 2ed8  odDblob......!..
-000017a0: 13c5 4100 0000 0700 7000 6f00 7000 5f00  ..A.....p.o.p._.
+00001790: 6f64 4462 6c6f 6200 0000 08f5 31c6 66d3  odDblob.....1.f.
+000017a0: 1dc5 4100 0000 0700 7000 6f00 7000 5f00  ..A.....p.o.p._.
 000017b0: 7500 7000 7370 6831 5363 6f6d 7000 0000  u.p.sph1Scomp...
-000017c0: 0000 09f0 0000 0000 0700 7000 6f00 7000  ..........p.o.p.
+000017c0: 0000 0e70 0000 0000 0700 7000 6f00 7000  ...p......p.o.p.
 000017d0: 5f00 7500 7000 7376 5372 6e6c 6f6e 6700  _.u.p.svSrnlong.
 000017e0: 0000 0100 0000 0000 0000 0000 0000 0000  ................
 000017f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001800: 0000 0000 0000 0003 0000 0000 0000 180b  ................
 00001810: 0000 0045 0000 100b 0000 0000 0000 0000  ...E............
 00001820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -497,17 +497,17 @@
 00001f00: 7b01 7c01 7e01 8701 8801 8a01 8b01 8d01  {.|.~...........
 00001f10: 9601 9701 9901 9a01 9c01 a501 a601 a801  ................
 00001f20: a901 ab01 b401 b501 b801 b901 bb01 bc01  ................
 00001f30: c501 ce01 db01 dc00 0000 0000 0002 0100  ................
 00001f40: 0000 0000 0000 4c00 0000 0000 0000 0000  ......L.........
 00001f50: 0000 0000 0001 e500 0000 0700 7000 6f00  ............p.o.
 00001f60: 7000 5f00 7500 7000 736d 6f44 4462 6c6f  p._.u.p.smoDDblo
-00001f70: 6200 0000 08cd a621 2ed8 13c5 4100 0000  b......!....A...
+00001f70: 6200 0000 08f5 31c6 66d3 1dc5 4100 0000  b.....1.f...A...
 00001f80: 0700 7000 6f00 7000 5f00 7500 7000 736d  ..p.o.p._.u.p.sm
-00001f90: 6f64 4462 6c6f 6200 0000 08cd a621 2ed8  odDblob......!..
-00001fa0: 13c5 4100 0000 0700 7000 6f00 7000 5f00  ..A.....p.o.p._.
+00001f90: 6f64 4462 6c6f 6200 0000 08f5 31c6 66d3  odDblob.....1.f.
+00001fa0: 1dc5 4100 0000 0700 7000 6f00 7000 5f00  ..A.....p.o.p._.
 00001fb0: 7500 7000 7370 6831 5363 6f6d 7000 0000  u.p.sph1Scomp...
-00001fc0: 0000 09f0 0000 0000 0700 7000 6f00 7000  ..........p.o.p.
+00001fc0: 0000 0e70 0000 0000 0700 7000 6f00 7000  ...p......p.o.p.
 00001fd0: 5f00 7500 7000 7376 5372 6e6c 6f6e 6700  _.u.p.svSrnlong.
 00001fe0: 0000 0100 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/roi_tools/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 0003 1e4f 0000 000b 005f 005f 0070  .....O....._._.p
+00000130: 0000 0003 66d1 0000 000b 005f 005f 0070  ....f......_._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 2c3b b6f1  moDDblob....,;..
-00000160: cc0c c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 e267 c4c2  moDDblob.....g..
+00000160: 1b1f c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 2c3b b6f1 cc0c  dDblob....,;....
+00000180: 6444 626c 6f62 0000 0008 e267 c4c2 1b1f  dDblob.....g....
 00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 000001b0: 636f 6d70 0000 0000 0004 7000 0000 0000  comp......p.....
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.63.2/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/labelling/.DS_Store`

 * *Files 3% similar despite different names*

```diff
@@ -44,23 +44,23 @@
 000002b0: 0062 0065 006c 006c 0069 006e 0067 002f  .b.e.l.l.i.n.g./
 000002c0: 0000 000b 005f 005f 0069 006e 0069 0074  ....._._.i.n.i.t
 000002d0: 005f 005f 002e 0070 0079 7074 624e 7573  ._._...p.yptbNus
 000002e0: 7472 0000 000b 005f 005f 0069 006e 0069  tr....._._.i.n.i
 000002f0: 0074 005f 005f 002e 0070 0079 0000 000b  .t._._...p.y....
 00000300: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000310: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000320: 0000 0000 a57a 0000 000b 005f 005f 0070  .....z....._._.p
+00000320: 0000 0001 3c13 0000 000b 005f 005f 0070  ....<......_._.p
 00000330: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000340: 6d6f 4444 626c 6f62 0000 0008 b5e2 07c3  moDDblob........
-00000350: 530f c541 0000 000b 005f 005f 0070 0079  S..A....._._.p.y
+00000340: 6d6f 4444 626c 6f62 0000 0008 8eb9 d848  moDDblob.......H
+00000350: af1d c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 00000360: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000370: 6444 626c 6f62 0000 0008 b5e2 07c3 530f  dDblob........S.
+00000370: 6444 626c 6f62 0000 0008 8eb9 d848 af1d  dDblob.......H..
 00000380: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 00000390: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000003a0: 636f 6d70 0000 0000 0000 c000 0000 0000  comp............
+000003a0: 636f 6d70 0000 0000 0001 7000 0000 0000  comp......p.....
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.1/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.63.2/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.63.2/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.63.2/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.63.2/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.63.2/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.63.2/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.63.2/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.63.2/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.63.2/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.63.2/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.63.2/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.63.2/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.63.2/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.63.2/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.63.2/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.63.2/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.63.2/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.63.2/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.63.2/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.63.2/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.63.2/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.63.2/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.63.2/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/.DS_Store`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 2800 0000 0800  ....Bud1..(.....
 00000010: 0000 2800 0000 300c 0000 100c 0000 400c  ..(...0.......@.
 00000020: 0000 500c 0000 0000 0000 0000 0000 0800  ..P.............
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 000a 0000 0002 0000 00b6  ................
+00000040: 0000 0000 0000 000a 0000 0002 0000 00ba  ................
 00000050: 0000 000c 0000 1000 0078 0069 006e 0073  .........x.i.n.s
 00000060: 6c73 7670 0000 0000 0000 0000 0000 0000  lsvp............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -764,15 +764,15 @@
 00002fb0: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
 00002fc0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
 00002fd0: 0809 5f10 187b 7b32 302c 2032 3336 7d2c  .._..{{20, 236},
 00002fe0: 207b 3130 3736 2c20 3632 317d 7d09 0817   {1076, 621}}...
 00002ff0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
 00003000: 0000 0001 0000 0000 0000 0010 0000 0005  ................
 00003010: 0075 0074 0069 006c 0073 6c67 3153 636f  .u.t.i.l.slg1Sco
-00003020: 6d70 0000 0000 0004 6873 0000 0005 0075  mp......hs.....u
+00003020: 6d70 0000 0000 0006 78bc 0000 0005 0075  mp......x......u
 00003030: 0074 0069 006c 0073 6c73 7643 626c 6f62  .t.i.l.slsvCblob
 00003040: 0000 0297 6270 6c69 7374 3030 d801 0203  ....bplist00....
 00003050: 0405 0607 0809 0a0b 1949 4a0a 4c5f 1012  .........IJ.L_..
 00003060: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
 00003070: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
 00003080: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
 00003090: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
@@ -848,20 +848,20 @@
 000034f0: 3b01 3c01 4501 4701 4801 4a01 4b01 5401  ;.<.E.G.H.J.K.T.
 00003500: 5601 5701 5901 5a01 6301 6501 6601 6801  V.W.Y.Z.c.e.f.h.
 00003510: 6901 7201 7401 7501 7701 7801 8101 8301  i.r.t.u.w.x.....
 00003520: 8401 8701 8801 9101 9201 9301 9401 9d01  ................
 00003530: a201 a300 0000 0000 0002 0100 0000 0000  ................
 00003540: 0000 4900 0000 0000 0000 0000 0000 0000  ..I.............
 00003550: 0001 ac00 0000 0500 7500 7400 6900 6c00  ........u.t.i.l.
-00003560: 736d 6f44 4462 6c6f 6200 0000 083a 1e5a  smoDDblob....:.Z
-00003570: 5655 1cc5 4100 0000 0500 7500 7400 6900  VU..A.....u.t.i.
-00003580: 6c00 736d 6f64 4462 6c6f 6200 0000 083a  l.smodDblob....:
-00003590: 1e5a 5655 1cc5 4100 0000 0500 7500 7400  .ZVU..A.....u.t.
+00003560: 736d 6f44 4462 6c6f 6200 0000 08c6 a590  smoDDblob.......
+00003570: 9d1b 1fc5 4100 0000 0500 7500 7400 6900  ....A.....u.t.i.
+00003580: 6c00 736d 6f64 4462 6c6f 6200 0000 08c6  l.smodDblob.....
+00003590: a590 9d1b 1fc5 4100 0000 0500 7500 7400  ......A.....u.t.
 000035a0: 6900 6c00 7370 6831 5363 6f6d 7000 0000  i.l.sph1Scomp...
-000035b0: 0000 0530 0000 0000 0500 7500 7400 6900  ...0......u.t.i.
+000035b0: 0000 07b0 0000 0000 0500 7500 7400 6900  ..........u.t.i.
 000035c0: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
 000035d0: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
 000035e0: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
 000035f0: 7200 7362 7773 7062 6c6f 6200 0000 c962  r.sbwspblob....b
 00003600: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
 00003610: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
 00003620: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
@@ -876,15 +876,15 @@
 000036b0: 0000 0000 0000 000f 0000 0000 0000 0000  ................
 000036c0: 0000 0000 0000 009a 0000 0010 0076 0069  .............v.i
 000036d0: 0064 0065 006f 005f 0070 0072 006f 0063  .d.e.o._.p.r.o.c
 000036e0: 0065 0073 0073 006f 0072 0073 6473 636c  .e.s.s.o.r.sdscl
 000036f0: 626f 6f6c 0000 0000 1000 7600 6900 6400  bool......v.i.d.
 00003700: 6500 6f00 5f00 7000 7200 6f00 6300 6500  e.o._.p.r.o.c.e.
 00003710: 7300 7300 6f00 7200 736c 6731 5363 6f6d  s.s.o.r.slg1Scom
-00003720: 7000 0000 0000 0333 0b00 0000 1000 7600  p......3......v.
+00003720: 7000 0000 0000 0472 6400 0000 1000 7600  p......rd.....v.
 00003730: 6900 6400 6500 6f00 5f00 7000 7200 6f00  i.d.e.o._.p.r.o.
 00003740: 6300 6500 7300 7300 6f00 7200 736c 7376  c.e.s.s.o.r.slsv
 00003750: 4362 6c6f 6200 0002 9762 706c 6973 7430  Cblob....bplist0
 00003760: 30d8 0102 0304 0506 0708 090a 0b19 494a  0.............IJ
 00003770: 0a4c 5869 636f 6e53 697a 655f 100f 7368  .LXiconSize_..sh
 00003780: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
 00003790: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
@@ -964,23 +964,23 @@
 00003c30: 0161 016a 016b 016d 016e 0170 0179 017a  .a.j.k.m.n.p.y.z
 00003c40: 017c 017d 017f 0188 0189 018c 018d 018f  .|.}............
 00003c50: 0198 0199 019a 019c 019d 01a6 01ab 0000  ................
 00003c60: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
 00003c70: 0000 0000 0000 0000 0000 0000 01ac 0000  ................
 00003c80: 0010 0076 0069 0064 0065 006f 005f 0070  ...v.i.d.e.o._.p
 00003c90: 0072 006f 0063 0065 0073 0073 006f 0072  .r.o.c.e.s.s.o.r
-00003ca0: 0073 6d6f 4444 626c 6f62 0000 0008 85b8  .smoDDblob......
-00003cb0: 5eee cc0c c541 0000 0010 0076 0069 0064  ^....A.....v.i.d
+00003ca0: 0073 6d6f 4444 626c 6f62 0000 0008 c1a2  .smoDDblob......
+00003cb0: e9f8 b219 c541 0000 0010 0076 0069 0064  .....A.....v.i.d
 00003cc0: 0065 006f 005f 0070 0072 006f 0063 0065  .e.o._.p.r.o.c.e
 00003cd0: 0073 0073 006f 0072 0073 6d6f 6444 626c  .s.s.o.r.smodDbl
-00003ce0: 6f62 0000 0008 85b8 5eee cc0c c541 0000  ob......^....A..
+00003ce0: 6f62 0000 0008 c1a2 e9f8 b219 c541 0000  ob...........A..
 00003cf0: 0010 0076 0069 0064 0065 006f 005f 0070  ...v.i.d.e.o._.p
 00003d00: 0072 006f 0063 0065 0073 0073 006f 0072  .r.o.c.e.s.s.o.r
-00003d10: 0073 7068 3153 636f 6d70 0000 0000 0003  .sph1Scomp......
-00003d20: f000 0000 0010 0076 0069 0064 0065 006f  .......v.i.d.e.o
+00003d10: 0073 7068 3153 636f 6d70 0000 0000 0005  .sph1Scomp......
+00003d20: 8000 0000 0010 0076 0069 0064 0065 006f  .......v.i.d.e.o
 00003d30: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
 00003d40: 006f 0072 0073 7653 726e 6c6f 6e67 0000  .o.r.svSrnlong..
 00003d50: 0001 0000 0000 0000 0000 0000 0000 0000  ................
 00003d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1034,231 +1034,231 @@
 00004090: 006d 0062 0061 005f 0064 0065 0076 002f  .m.b.a._.d.e.v./
 000040a0: 0073 0069 006d 0062 0061 002f 0000 000b  .s.i.m.b.a./....
 000040b0: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
 000040c0: 002e 0070 0079 7074 624e 7573 7472 0000  ...p.yptbNustr..
 000040d0: 000b 005f 005f 0069 006e 0069 0074 005f  ..._._.i.n.i.t._
 000040e0: 005f 002e 0070 0079 0000 000b 005f 005f  ._...p.y....._._
 000040f0: 0070 0079 0063 0061 0063 0068 0065 005f  .p.y.c.a.c.h.e._
-00004100: 005f 6c67 3153 636f 6d70 0000 0000 0000  ._lg1Scomp......
-00004110: c933 0000 000b 005f 005f 0070 0079 0063  .3....._._.p.y.c
+00004100: 005f 6c67 3153 636f 6d70 0000 0000 0001  ._lg1Scomp......
+00004110: 95ea 0000 000b 005f 005f 0070 0079 0063  ......._._.p.y.c
 00004120: 0061 0063 0068 0065 005f 005f 6d6f 4444  .a.c.h.e._._moDD
-00004130: 626c 6f62 0000 0008 68ff 13ac ef0f c541  blob....h......A
+00004130: 626c 6f62 0000 0008 170e b937 1d1f c541  blob.......7...A
 00004140: 0000 000b 005f 005f 0070 0079 0063 0061  ....._._.p.y.c.a
 00004150: 0063 0068 0065 005f 005f 6d6f 6444 626c  .c.h.e._._modDbl
-00004160: 6f62 0000 0008 68ff 13ac ef0f c541 0000  ob....h......A..
+00004160: 6f62 0000 0008 13a7 42bc 1b1f c541 0000  ob......B....A..
 00004170: 000b 005f 005f 0070 0079 0063 0061 0063  ..._._.p.y.c.a.c
 00004180: 0068 0065 005f 005f 7068 3153 636f 6d70  .h.e._._ph1Scomp
-00004190: 0000 0000 0000 e000 0000 0006 0061 0073  .............a.s
+00004190: 0000 0000 0001 c000 0000 0006 0061 0073  .............a.s
 000041a0: 0073 0065 0074 0073 6277 7370 626c 6f62  .s.e.t.sbwspblob
-000041b0: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
-000041c0: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
-000041d0: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
-000041e0: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
-000041f0: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
-00004200: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
-00004210: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
-00004220: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
-00004230: 0809 5f10 187b 7b33 3335 2c20 3139 387d  .._..{{335, 198}
-00004240: 2c20 7b39 3237 2c20 3536 387d 7d09 0817  , {927, 568}}...
-00004250: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
-00004260: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-00004270: 0000 0000 0000 0000 0000 0000 9a00 0000  ................
-00004280: 0600 6100 7300 7300 6500 7400 736c 6731  ..a.s.s.e.t.slg1
-00004290: 5363 6f6d 7000 0000 0000 7ddb 9300 0000  Scomp.....}.....
-000042a0: 0600 6100 7300 7300 6500 7400 736c 7376  ..a.s.s.e.t.slsv
-000042b0: 4362 6c6f 6200 0002 b062 706c 6973 7430  Cblob....bplist0
-000042c0: 30da 0102 0304 0506 0708 090a 0b0c 0d1a  0...............
-000042d0: 4849 484a 0c4c 5869 636f 6e53 697a 655f  HIHJ.LXiconSize_
-000042e0: 100f 7368 6f77 4963 6f6e 5072 6576 6965  ..showIconPrevie
-000042f0: 7757 636f 6c75 6d6e 735f 1011 6361 6c63  wWcolumns_..calc
-00004300: 756c 6174 6541 6c6c 5369 7a65 735f 100f  ulateAllSizes_..
-00004310: 7363 726f 6c6c 506f 7369 7469 6f6e 5958  scrollPositionYX
-00004320: 7465 7874 5369 7a65 5f10 0f73 6372 6f6c  textSize_..scrol
-00004330: 6c50 6f73 6974 696f 6e58 5a73 6f72 7443  lPositionXZsortC
-00004340: 6f6c 756d 6e5f 1010 7573 6552 656c 6174  olumn_..useRelat
-00004350: 6976 6544 6174 6573 5f10 1276 6965 774f  iveDates_..viewO
-00004360: 7074 696f 6e73 5665 7273 696f 6e23 4030  ptionsVersion#@0
-00004370: 0000 0000 0000 09ab 0e17 1c21 252a 2f34  ...........!%*/4
-00004380: 393e 43d4 0f10 1112 1314 0c0c 5a69 6465  9>C.........Zide
-00004390: 6e74 6966 6965 7255 7769 6474 6859 6173  ntifierUwidthYas
-000043a0: 6365 6e64 696e 6757 7669 7369 626c 6554  cendingWvisibleT
-000043b0: 6e61 6d65 1101 c709 09d4 0f10 1112 1819  name............
-000043c0: 1a1a 5875 6269 7175 6974 7910 2308 08d4  ..Xubiquity.#...
-000043d0: 0f10 1112 1d1e 1a0c 5c64 6174 654d 6f64  ........\dateMod
-000043e0: 6966 6965 6410 b508 09d4 0f10 1112 221e  ified.........".
-000043f0: 1a1a 5b64 6174 6543 7265 6174 6564 0808  ..[dateCreated..
-00004400: d40f 1011 1226 271a 0c54 7369 7a65 1061  .....&'..Tsize.a
-00004410: 0809 d40f 1011 122b 2c0c 0c54 6b69 6e64  .......+,..Tkind
-00004420: 1073 0909 d40f 1011 1230 310c 1a55 6c61  .s.......01..Ula
-00004430: 6265 6c10 6409 08d4 0f10 1112 3536 0c1a  bel.d.......56..
-00004440: 5776 6572 7369 6f6e 104b 0908 d40f 1011  Wversion.K......
-00004450: 123a 3b0c 1a58 636f 6d6d 656e 7473 1101  .:;..Xcomments..
-00004460: 2c09 08d4 0f10 1112 3f40 1a1a 5e64 6174  ,.......?@..^dat
-00004470: 654c 6173 744f 7065 6e65 6410 c808 08d4  eLastOpened.....
-00004480: 0f10 1112 441e 1a1a 5964 6174 6541 6464  ....D...YdateAdd
-00004490: 6564 0808 0823 0000 0000 0000 0000 2340  ed...#........#@
-000044a0: 2800 0000 0000 0054 6e61 6d65 0910 0100  (......Tname....
-000044b0: 0800 1d00 2600 3800 4000 5400 6600 6f00  ....&.8.@.T.f.o.
-000044c0: 8100 8c00 9f00 b400 bd00 be00 ca00 d300  ................
-000044d0: de00 e400 ee00 f600 fb00 fe00 ff01 0001  ................
-000044e0: 0901 1201 1401 1501 1601 1f01 2c01 2e01  ............,...
-000044f0: 2f01 3001 3901 4501 4601 4701 5001 5501  /.0.9.E.F.G.P.U.
-00004500: 5701 5801 5901 6201 6701 6901 6a01 6b01  W.X.Y.b.g.i.j.k.
-00004510: 7401 7a01 7c01 7d01 7e01 8701 8f01 9101  t.z.|.}.~.......
-00004520: 9201 9301 9c01 a501 a801 a901 aa01 b301  ................
-00004530: c201 c401 c501 c601 cf01 d901 da01 db01  ................
-00004540: dc01 e501 ee01 f301 f400 0000 0000 0002  ................
-00004550: 0100 0000 0000 0000 4d00 0000 0000 0000  ........M.......
-00004560: 0000 0000 0000 0001 f600 0000 0600 6100  ..............a.
-00004570: 7300 7300 6500 7400 736c 7376 7062 6c6f  s.s.e.t.slsvpblo
-00004580: 6200 0002 9562 706c 6973 7430 30da 0102  b....bplist00...
-00004590: 0304 0506 0708 090a 0b0c 0d1c 4849 484a  ............HIHJ
-000045a0: 0c29 5869 636f 6e53 697a 655f 100f 7368  .)XiconSize_..sh
-000045b0: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
-000045c0: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
-000045d0: 6541 6c6c 5369 7a65 735f 100f 7363 726f  eAllSizes_..scro
-000045e0: 6c6c 506f 7369 7469 6f6e 5958 7465 7874  llPositionYXtext
-000045f0: 5369 7a65 5f10 0f73 6372 6f6c 6c50 6f73  Size_..scrollPos
-00004600: 6974 696f 6e58 5a73 6f72 7443 6f6c 756d  itionXZsortColum
-00004610: 6e5f 1010 7573 6552 656c 6174 6976 6544  n_..useRelativeD
-00004620: 6174 6573 5f10 1276 6965 774f 7074 696f  ates_..viewOptio
-00004630: 6e73 5665 7273 696f 6e23 4030 0000 0000  nsVersion#@0....
-00004640: 0000 09d9 0e0f 1011 1213 1415 1617 2025  .............. %
-00004650: 2a2e 3338 3d42 5863 6f6d 6d65 6e74 735e  *.38=BXcomments^
-00004660: 6461 7465 4c61 7374 4f70 656e 6564 5c64  dateLastOpened\d
-00004670: 6174 654d 6f64 6966 6965 645b 6461 7465  ateModified[date
-00004680: 4372 6561 7465 6454 7369 7a65 556c 6162  CreatedTsizeUlab
-00004690: 656c 546b 696e 6457 7665 7273 696f 6e54  elTkindWversionT
-000046a0: 6e61 6d65 d418 191a 1b1c 1d0c 1f57 7669  name.........Wvi
-000046b0: 7369 626c 6555 7769 6474 6859 6173 6365  sibleUwidthYasce
-000046c0: 6e64 696e 6755 696e 6465 7808 1101 2c09  ndingUindex...,.
-000046d0: 1007 d418 191a 1b1c 221c 2408 10c8 0810  ........".$.....
-000046e0: 08d4 1819 1a1b 0c27 1c29 0910 b508 1001  .......'.)......
-000046f0: d418 191a 1b1c 271c 2d08 0810 02d4 1819  ......'.-.......
-00004700: 1a1b 0c30 1c32 0910 6108 1003 d418 191a  ...0.2..a.......
-00004710: 1b1c 350c 3708 1064 0910 05d4 1819 1a1b  ..5.7..d........
-00004720: 0c3a 0c3c 0910 7309 1004 d418 191a 1b1c  .:.<..s.........
-00004730: 3f0c 4108 104b 0910 06d4 1819 1a1b 0c44  ?.A..K.........D
-00004740: 0c46 0911 01c7 0910 0008 2300 0000 0000  .F........#.....
-00004750: 0000 0023 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
-00004760: 6509 0008 001d 0026 0038 0040 0054 0066  e......&.8.@.T.f
-00004770: 006f 0081 008c 009f 00b4 00bd 00be 00d1  .o..............
-00004780: 00da 00e9 00f6 0102 0107 010d 0112 011a  ................
-00004790: 011f 0128 0130 0136 0140 0146 0147 014a  ...(.0.6.@.F.G.J
-000047a0: 014b 014d 0156 0157 0159 015a 015c 0165  .K.M.V.W.Y.Z.\.e
-000047b0: 0166 0168 0169 016b 0174 0175 0176 0178  .f.h.i.k.t.u.v.x
-000047c0: 0181 0182 0184 0185 0187 0190 0191 0193  ................
-000047d0: 0194 0196 019f 01a0 01a2 01a3 01a5 01ae  ................
-000047e0: 01af 01b1 01b2 01b4 01bd 01be 01c1 01c2  ................
-000047f0: 01c4 01c5 01ce 01d7 01dc 0000 0000 0000  ................
-00004800: 0201 0000 0000 0000 004c 0000 0000 0000  .........L......
-00004810: 0000 0000 0000 0000 01dd 0000 0006 0061  ...............a
-00004820: 0073 0073 0065 0074 0073 6d6f 4444 626c  .s.s.e.t.smoDDbl
-00004830: 6f62 0000 0008 cf95 8ce8 d0e1 c441 0000  ob...........A..
-00004840: 0006 0061 0073 0073 0065 0074 0073 6d6f  ...a.s.s.e.t.smo
-00004850: 6444 626c 6f62 0000 0008 cf95 8ce8 d0e1  dDblob..........
-00004860: c441 0000 0006 0061 0073 0073 0065 0074  .A.....a.s.s.e.t
-00004870: 0073 7068 3153 636f 6d70 0000 0000 0081  .sph1Scomp......
-00004880: a000 0000 0006 0061 0073 0073 0065 0074  .......a.s.s.e.t
-00004890: 0073 7653 726e 6c6f 6e67 0000 0001 0000  .svSrnlong......
-000048a0: 000c 0062 006c 006f 0062 005f 0073 0074  ...b.l.o.b._.s.t
-000048b0: 006f 0072 0061 0067 0065 6277 7370 626c  .o.r.a.g.ebwspbl
-000048c0: 6f62 0000 00c9 6270 6c69 7374 3030 d701  ob....bplist00..
-000048d0: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
-000048e0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-000048f0: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
-00004900: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
-00004910: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
-00004920: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00004930: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00004940: 0809 0809 5f10 187b 7b33 3335 2c20 3139  ...._..{{335, 19
-00004950: 387d 2c20 7b39 3237 2c20 3536 387d 7d09  8}, {927, 568}}.
-00004960: 0817 2531 3d49 606d 797a 7b7c 7d7e 9900  ..%1=I`myz{|}~..
-00004970: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
-00004980: 0000 0000 0000 0000 0000 0000 0000 9a00  ................
-00004990: 0000 0c00 6200 6c00 6f00 6200 5f00 7300  ....b.l.o.b._.s.
-000049a0: 7400 6f00 7200 6100 6700 656c 6731 5363  t.o.r.a.g.elg1Sc
-000049b0: 6f6d 7000 0000 0000 0018 0400 0000 0c00  omp.............
-000049c0: 6200 6c00 6f00 6200 5f00 7300 7400 6f00  b.l.o.b._.s.t.o.
-000049d0: 7200 6100 6700 656d 6f44 4462 6c6f 6200  r.a.g.emoDDblob.
-000049e0: 0000 083f 3c3f 74e2 ddc4 4100 0000 0c00  ...?<?t...A.....
-000049f0: 6200 6c00 6f00 6200 5f00 7300 7400 6f00  b.l.o.b._.s.t.o.
-00004a00: 7200 6100 6700 656d 6f64 4462 6c6f 6200  r.a.g.emodDblob.
-00004a10: 0000 083f 3c3f 74e2 ddc4 4100 0000 0c00  ...?<?t...A.....
-00004a20: 6200 6c00 6f00 6200 5f00 7300 7400 6f00  b.l.o.b._.s.t.o.
-00004a30: 7200 6100 6700 6570 6831 5363 6f6d 7000  r.a.g.eph1Scomp.
-00004a40: 0000 0000 0020 0000 0000 0c00 6200 6c00  ..... ......b.l.
-00004a50: 6f00 6200 5f00 7300 7400 6f00 7200 6100  o.b._.s.t.o.r.a.
-00004a60: 6700 6576 5372 6e6c 6f6e 6700 0000 0100  g.evSrnlong.....
-00004a70: 0000 1200 6200 6f00 7500 6e00 6400 6900  ....b.o.u.n.d.i.
-00004a80: 6e00 6700 5f00 6200 6f00 7800 5f00 7400  n.g._.b.o.x._.t.
-00004a90: 6f00 6f00 6c00 7362 7773 7062 6c6f 6200  o.o.l.sbwspblob.
-00004aa0: 0000 ca62 706c 6973 7430 30d7 0102 0304  ...bplist00.....
-00004ab0: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
-00004ac0: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
-00004ad0: 6862 6172 5b53 686f 7754 6f6f 6c62 6172  hbar[ShowToolbar
-00004ae0: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
-00004af0: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
-00004b00: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
-00004b10: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
-00004b20: 095f 1019 7b7b 3335 342c 2031 3234 7d2c  ._..{{354, 124},
-00004b30: 207b 3130 3736 2c20 3632 317d 7d09 0817   {1076, 621}}...
-00004b40: 2531 3d49 606d 797a 7b7c 7d7e 9a00 0000  %1=I`myz{|}~....
-00004b50: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-00004b60: 0000 0000 0000 0000 0000 0000 9b00 0000  ................
-00004b70: 1200 6200 6f00 7500 6e00 6400 6900 6e00  ..b.o.u.n.d.i.n.
-00004b80: 6700 5f00 6200 6f00 7800 5f00 7400 6f00  g._.b.o.x._.t.o.
-00004b90: 6f00 6c00 7364 7363 6c62 6f6f 6c00 0000  o.l.sdsclbool...
-00004ba0: 0012 0062 006f 0075 006e 0064 0069 006e  ...b.o.u.n.d.i.n
-00004bb0: 0067 005f 0062 006f 0078 005f 0074 006f  .g._.b.o.x._.t.o
-00004bc0: 006f 006c 0073 6c67 3153 636f 6d70 0000  .o.l.slg1Scomp..
-00004bd0: 0000 0001 9d60 0000 0012 0062 006f 0075  .....`.....b.o.u
-00004be0: 006e 0064 0069 006e 0067 005f 0062 006f  .n.d.i.n.g._.b.o
-00004bf0: 0078 005f 0074 006f 006f 006c 0073 6c73  .x._.t.o.o.l.sls
-00004c00: 7643 626c 6f62 0000 0279 6270 6c69 7374  vCblob...ybplist
-00004c10: 3030 d801 0203 0405 0607 0809 0a0b 1646  00.............F
-00004c20: 4748 0a5f 1012 7669 6577 4f70 7469 6f6e  GH._..viewOption
-00004c30: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
-00004c40: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
-00004c50: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
-00004c60: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
-00004c70: 736f 7274 436f 6c75 6d6e 5869 636f 6e53  sortColumnXiconS
-00004c80: 697a 655f 1010 7573 6552 656c 6174 6976  ize_..useRelativ
-00004c90: 6544 6174 6573 1001 09ab 0c15 1a1f 2328  eDates........#(
-00004ca0: 2d32 373c 41d4 0d0e 0f10 0a12 0a14 5776  -27<A.........Wv
-00004cb0: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
-00004cc0: 656e 6469 6e67 5a69 6465 6e74 6966 6965  endingZidentifie
-00004cd0: 7209 1101 c709 546e 616d 65d4 0d0e 0f10  r.....Tname.....
-00004ce0: 1617 1619 0810 2308 5875 6269 7175 6974  ......#.Xubiquit
-00004cf0: 79d4 0d0e 0f10 0a1c 161e 0910 b508 5c64  y.............\d
-00004d00: 6174 654d 6f64 6966 6965 64d4 0d0e 0f10  ateModified.....
-00004d10: 161c 1622 0808 5b64 6174 6543 7265 6174  ..."..[dateCreat
-00004d20: 6564 d40d 0e0f 100a 2516 2709 1061 0854  ed......%.'..a.T
-00004d30: 7369 7a65 d40d 0e0f 100a 2a0a 2c09 1073  size......*.,..s
-00004d40: 0954 6b69 6e64 d40d 0e0f 1016 2f0a 3108  .Tkind....../.1.
-00004d50: 1064 0955 6c61 6265 6cd4 0d0e 0f10 1634  .d.Ulabel......4
-00004d60: 0a36 0810 4b09 5776 6572 7369 6f6e d40d  .6..K.Wversion..
-00004d70: 0e0f 1016 390a 3b08 1101 2c09 5863 6f6d  ....9.;...,.Xcom
-00004d80: 6d65 6e74 73d4 0d0e 0f10 163e 1640 0810  ments......>.@..
-00004d90: c808 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
-00004da0: 64d4 0d0e 0f10 161c 1644 0808 5964 6174  d........D..Ydat
-00004db0: 6541 6464 6564 0823 4028 0000 0000 0000  eAdded.#@(......
-00004dc0: 546e 616d 6523 4030 0000 0000 0000 0900  Tname#@0........
-00004dd0: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
-00004de0: 7900 8c00 8e00 8f00 9b00 a400 ac00 b200  y...............
-00004df0: bc00 c700 c800 cb00 cc00 d100 da00 db00  ................
-00004e00: dd00 de00 e700 f000 f100 f300 f401 0101  ................
-00004e10: 0a01 0b01 0c01 1801 2101 2201 2401 2501  ........!.".$.%.
-00004e20: 2a01 3301 3401 3601 3701 3c01 4501 4601  *.3.4.6.7.<.E.F.
-00004e30: 4801 4901 4f01 5801 5901 5b01 5c01 6401  H.I.O.X.Y.[.\.d.
-00004e40: 6d01 6e01 7101 7201 7b01 8401 8501 8701  m.n.q.r.{.......
-00004e50: 8801 9701 a001 a101 a201 ac01 ad01 b601  ................
-00004e60: bb01 c400 0000 0000 0002 0100 0000 0000  ................
-00004e70: 0000 4a00 0000 0000 0000 0000 0000 0000  ..J.............
-00004e80: 0001 c500 0000 0000 0000 0000 0000 0000  ................
+000041b0: 0000 00b8 6270 6c69 7374 3030 d601 0203  ....bplist00....
+000041c0: 0405 0607 0807 080b 085d 5368 6f77 5374  .........]ShowSt
+000041d0: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
+000041e0: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
+000041f0: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
+00004200: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
+00004210: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
+00004220: 0908 095f 1018 7b7b 3637 302c 2033 3939  ..._..{{670, 399
+00004230: 7d2c 207b 3737 302c 2034 3336 7d7d 0908  }, {770, 436}}..
+00004240: 1523 2f3b 525f 6b6c 6d6e 6f8a 0000 0000  .#/;R_klmno.....
+00004250: 0000 0101 0000 0000 0000 000d 0000 0000  ................
+00004260: 0000 0000 0000 0000 0000 008b 0000 0006  ................
+00004270: 0061 0073 0073 0065 0074 0073 6c67 3153  .a.s.s.e.t.slg1S
+00004280: 636f 6d70 0000 0000 007d db93 0000 0006  comp.....}......
+00004290: 0061 0073 0073 0065 0074 0073 6c73 7643  .a.s.s.e.t.slsvC
+000042a0: 626c 6f62 0000 02b0 6270 6c69 7374 3030  blob....bplist00
+000042b0: da01 0203 0405 0607 0809 0a0b 0c0d 1a48  ...............H
+000042c0: 4948 4a0c 4c58 6963 6f6e 5369 7a65 5f10  IHJ.LXiconSize_.
+000042d0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+000042e0: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+000042f0: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
+00004300: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
+00004310: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
+00004320: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
+00004330: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
+00004340: 7665 4461 7465 735f 1012 7669 6577 4f70  veDates_..viewOp
+00004350: 7469 6f6e 7356 6572 7369 6f6e 2340 3000  tionsVersion#@0.
+00004360: 0000 0000 0009 ab0e 171c 2125 2a2f 3439  ..........!%*/49
+00004370: 3e43 d40f 1011 1213 140c 0c5a 6964 656e  >C.........Ziden
+00004380: 7469 6669 6572 5577 6964 7468 5961 7363  tifierUwidthYasc
+00004390: 656e 6469 6e67 5776 6973 6962 6c65 546e  endingWvisibleTn
+000043a0: 616d 6511 01c7 0909 d40f 1011 1218 191a  ame.............
+000043b0: 1a58 7562 6971 7569 7479 1023 0808 d40f  .Xubiquity.#....
+000043c0: 1011 121d 1e1a 0c5c 6461 7465 4d6f 6469  .......\dateModi
+000043d0: 6669 6564 10b5 0809 d40f 1011 1222 1e1a  fied........."..
+000043e0: 1a5b 6461 7465 4372 6561 7465 6408 08d4  .[dateCreated...
+000043f0: 0f10 1112 2627 1a0c 5473 697a 6510 6108  ....&'..Tsize.a.
+00004400: 09d4 0f10 1112 2b2c 0c0c 546b 696e 6410  ......+,..Tkind.
+00004410: 7309 09d4 0f10 1112 3031 0c1a 556c 6162  s.......01..Ulab
+00004420: 656c 1064 0908 d40f 1011 1235 360c 1a57  el.d.......56..W
+00004430: 7665 7273 696f 6e10 4b09 08d4 0f10 1112  version.K.......
+00004440: 3a3b 0c1a 5863 6f6d 6d65 6e74 7311 012c  :;..Xcomments..,
+00004450: 0908 d40f 1011 123f 401a 1a5e 6461 7465  .......?@..^date
+00004460: 4c61 7374 4f70 656e 6564 10c8 0808 d40f  LastOpened......
+00004470: 1011 1244 1e1a 1a59 6461 7465 4164 6465  ...D...YdateAdde
+00004480: 6408 0808 2300 0000 0000 0000 0023 4028  d...#........#@(
+00004490: 0000 0000 0000 546e 616d 6509 1001 0008  ......Tname.....
+000044a0: 001d 0026 0038 0040 0054 0066 006f 0081  ...&.8.@.T.f.o..
+000044b0: 008c 009f 00b4 00bd 00be 00ca 00d3 00de  ................
+000044c0: 00e4 00ee 00f6 00fb 00fe 00ff 0100 0109  ................
+000044d0: 0112 0114 0115 0116 011f 012c 012e 012f  ...........,.../
+000044e0: 0130 0139 0145 0146 0147 0150 0155 0157  .0.9.E.F.G.P.U.W
+000044f0: 0158 0159 0162 0167 0169 016a 016b 0174  .X.Y.b.g.i.j.k.t
+00004500: 017a 017c 017d 017e 0187 018f 0191 0192  .z.|.}.~........
+00004510: 0193 019c 01a5 01a8 01a9 01aa 01b3 01c2  ................
+00004520: 01c4 01c5 01c6 01cf 01d9 01da 01db 01dc  ................
+00004530: 01e5 01ee 01f3 01f4 0000 0000 0000 0201  ................
+00004540: 0000 0000 0000 004d 0000 0000 0000 0000  .......M........
+00004550: 0000 0000 0000 01f6 0000 0006 0061 0073  .............a.s
+00004560: 0073 0065 0074 0073 6c73 7670 626c 6f62  .s.e.t.slsvpblob
+00004570: 0000 0295 6270 6c69 7374 3030 da01 0203  ....bplist00....
+00004580: 0405 0607 0809 0a0b 0c0d 1c48 4948 4a0c  ...........HIHJ.
+00004590: 2958 6963 6f6e 5369 7a65 5f10 0f73 686f  )XiconSize_..sho
+000045a0: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
+000045b0: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
+000045c0: 416c 6c53 697a 6573 5f10 0f73 6372 6f6c  AllSizes_..scrol
+000045d0: 6c50 6f73 6974 696f 6e59 5874 6578 7453  lPositionYXtextS
+000045e0: 697a 655f 100f 7363 726f 6c6c 506f 7369  ize_..scrollPosi
+000045f0: 7469 6f6e 585a 736f 7274 436f 6c75 6d6e  tionXZsortColumn
+00004600: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+00004610: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
+00004620: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
+00004630: 0009 d90e 0f10 1112 1314 1516 1720 252a  ............. %*
+00004640: 2e33 383d 4258 636f 6d6d 656e 7473 5e64  .38=BXcomments^d
+00004650: 6174 654c 6173 744f 7065 6e65 645c 6461  ateLastOpened\da
+00004660: 7465 4d6f 6469 6669 6564 5b64 6174 6543  teModified[dateC
+00004670: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
+00004680: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
+00004690: 616d 65d4 1819 1a1b 1c1d 0c1f 5776 6973  ame.........Wvis
+000046a0: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
+000046b0: 6469 6e67 5569 6e64 6578 0811 012c 0910  dingUindex...,..
+000046c0: 07d4 1819 1a1b 1c22 1c24 0810 c808 1008  .......".$......
+000046d0: d418 191a 1b0c 271c 2909 10b5 0810 01d4  ......'.).......
+000046e0: 1819 1a1b 1c27 1c2d 0808 1002 d418 191a  .....'.-........
+000046f0: 1b0c 301c 3209 1061 0810 03d4 1819 1a1b  ..0.2..a........
+00004700: 1c35 0c37 0810 6409 1005 d418 191a 1b0c  .5.7..d.........
+00004710: 3a0c 3c09 1073 0910 04d4 1819 1a1b 1c3f  :.<..s.........?
+00004720: 0c41 0810 4b09 1006 d418 191a 1b0c 440c  .A..K.........D.
+00004730: 4609 1101 c709 1000 0823 0000 0000 0000  F........#......
+00004740: 0000 2340 2800 0000 0000 0054 6e61 6d65  ..#@(......Tname
+00004750: 0900 0800 1d00 2600 3800 4000 5400 6600  ......&.8.@.T.f.
+00004760: 6f00 8100 8c00 9f00 b400 bd00 be00 d100  o...............
+00004770: da00 e900 f601 0201 0701 0d01 1201 1a01  ................
+00004780: 1f01 2801 3001 3601 4001 4601 4701 4a01  ..(.0.6.@.F.G.J.
+00004790: 4b01 4d01 5601 5701 5901 5a01 5c01 6501  K.M.V.W.Y.Z.\.e.
+000047a0: 6601 6801 6901 6b01 7401 7501 7601 7801  f.h.i.k.t.u.v.x.
+000047b0: 8101 8201 8401 8501 8701 9001 9101 9301  ................
+000047c0: 9401 9601 9f01 a001 a201 a301 a501 ae01  ................
+000047d0: af01 b101 b201 b401 bd01 be01 c101 c201  ................
+000047e0: c401 c501 ce01 d701 dc00 0000 0000 0002  ................
+000047f0: 0100 0000 0000 0000 4c00 0000 0000 0000  ........L.......
+00004800: 0000 0000 0000 0001 dd00 0000 0600 6100  ..............a.
+00004810: 7300 7300 6500 7400 736d 6f44 4462 6c6f  s.s.e.t.smoDDblo
+00004820: 6200 0000 08cf 958c e8d0 e1c4 4100 0000  b...........A...
+00004830: 0600 6100 7300 7300 6500 7400 736d 6f64  ..a.s.s.e.t.smod
+00004840: 4462 6c6f 6200 0000 08cf 958c e8d0 e1c4  Dblob...........
+00004850: 4100 0000 0600 6100 7300 7300 6500 7400  A.....a.s.s.e.t.
+00004860: 7370 6831 5363 6f6d 7000 0000 0000 81a0  sph1Scomp.......
+00004870: 0000 0000 0600 6100 7300 7300 6500 7400  ......a.s.s.e.t.
+00004880: 7376 5372 6e6c 6f6e 6700 0000 0100 0000  svSrnlong.......
+00004890: 0c00 6200 6c00 6f00 6200 5f00 7300 7400  ..b.l.o.b._.s.t.
+000048a0: 6f00 7200 6100 6700 6562 7773 7062 6c6f  o.r.a.g.ebwspblo
+000048b0: 6200 0000 c962 706c 6973 7430 30d7 0102  b....bplist00...
+000048c0: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
+000048d0: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
+000048e0: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
+000048f0: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
+00004900: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
+00004910: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
+00004920: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
+00004930: 0908 095f 1018 7b7b 3333 352c 2031 3938  ..._..{{335, 198
+00004940: 7d2c 207b 3932 372c 2035 3638 7d7d 0908  }, {927, 568}}..
+00004950: 1725 313d 4960 6d79 7a7b 7c7d 7e99 0000  .%1=I`myz{|}~...
+00004960: 0000 0000 0101 0000 0000 0000 000f 0000  ................
+00004970: 0000 0000 0000 0000 0000 0000 009a 0000  ................
+00004980: 000c 0062 006c 006f 0062 005f 0073 0074  ...b.l.o.b._.s.t
+00004990: 006f 0072 0061 0067 0065 6c67 3153 636f  .o.r.a.g.elg1Sco
+000049a0: 6d70 0000 0000 0000 1804 0000 000c 0062  mp.............b
+000049b0: 006c 006f 0062 005f 0073 0074 006f 0072  .l.o.b._.s.t.o.r
+000049c0: 0061 0067 0065 6d6f 4444 626c 6f62 0000  .a.g.emoDDblob..
+000049d0: 0008 3f3c 3f74 e2dd c441 0000 000c 0062  ..?<?t...A.....b
+000049e0: 006c 006f 0062 005f 0073 0074 006f 0072  .l.o.b._.s.t.o.r
+000049f0: 0061 0067 0065 6d6f 6444 626c 6f62 0000  .a.g.emodDblob..
+00004a00: 0008 3f3c 3f74 e2dd c441 0000 000c 0062  ..?<?t...A.....b
+00004a10: 006c 006f 0062 005f 0073 0074 006f 0072  .l.o.b._.s.t.o.r
+00004a20: 0061 0067 0065 7068 3153 636f 6d70 0000  .a.g.eph1Scomp..
+00004a30: 0000 0000 2000 0000 000c 0062 006c 006f  .... ......b.l.o
+00004a40: 0062 005f 0073 0074 006f 0072 0061 0067  .b._.s.t.o.r.a.g
+00004a50: 0065 7653 726e 6c6f 6e67 0000 0001 0000  .evSrnlong......
+00004a60: 0012 0062 006f 0075 006e 0064 0069 006e  ...b.o.u.n.d.i.n
+00004a70: 0067 005f 0062 006f 0078 005f 0074 006f  .g._.b.o.x._.t.o
+00004a80: 006f 006c 0073 6277 7370 626c 6f62 0000  .o.l.sbwspblob..
+00004a90: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
+00004aa0: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
+00004ab0: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
+00004ac0: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
+00004ad0: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
+00004ae0: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
+00004af0: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
+00004b00: 5368 6f77 5369 6465 6261 7208 0809 0809  ShowSidebar.....
+00004b10: 5f10 197b 7b33 3534 2c20 3132 347d 2c20  _..{{354, 124}, 
+00004b20: 7b31 3037 362c 2036 3231 7d7d 0908 1725  {1076, 621}}...%
+00004b30: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
+00004b40: 0000 0101 0000 0000 0000 000f 0000 0000  ................
+00004b50: 0000 0000 0000 0000 0000 009b 0000 0012  ................
+00004b60: 0062 006f 0075 006e 0064 0069 006e 0067  .b.o.u.n.d.i.n.g
+00004b70: 005f 0062 006f 0078 005f 0074 006f 006f  ._.b.o.x._.t.o.o
+00004b80: 006c 0073 6473 636c 626f 6f6c 0000 0000  .l.sdsclbool....
+00004b90: 1200 6200 6f00 7500 6e00 6400 6900 6e00  ..b.o.u.n.d.i.n.
+00004ba0: 6700 5f00 6200 6f00 7800 5f00 7400 6f00  g._.b.o.x._.t.o.
+00004bb0: 6f00 6c00 736c 6731 5363 6f6d 7000 0000  o.l.slg1Scomp...
+00004bc0: 0000 0244 4800 0000 1200 6200 6f00 7500  ...DH.....b.o.u.
+00004bd0: 6e00 6400 6900 6e00 6700 5f00 6200 6f00  n.d.i.n.g._.b.o.
+00004be0: 7800 5f00 7400 6f00 6f00 6c00 736c 7376  x._.t.o.o.l.slsv
+00004bf0: 4362 6c6f 6200 0002 7962 706c 6973 7430  Cblob...ybplist0
+00004c00: 30d8 0102 0304 0506 0708 090a 0b16 4647  0.............FG
+00004c10: 480a 5f10 1276 6965 774f 7074 696f 6e73  H._..viewOptions
+00004c20: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
+00004c30: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
+00004c40: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
+00004c50: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
+00004c60: 6f72 7443 6f6c 756d 6e58 6963 6f6e 5369  ortColumnXiconSi
+00004c70: 7a65 5f10 1075 7365 5265 6c61 7469 7665  ze_..useRelative
+00004c80: 4461 7465 7310 0109 ab0c 151a 1f23 282d  Dates........#(-
+00004c90: 3237 3c41 d40d 0e0f 100a 120a 1457 7669  27<A.........Wvi
+00004ca0: 7369 626c 6555 7769 6474 6859 6173 6365  sibleUwidthYasce
+00004cb0: 6e64 696e 675a 6964 656e 7469 6669 6572  ndingZidentifier
+00004cc0: 0911 01c7 0954 6e61 6d65 d40d 0e0f 1016  .....Tname......
+00004cd0: 1716 1908 1023 0858 7562 6971 7569 7479  .....#.Xubiquity
+00004ce0: d40d 0e0f 100a 1c16 1e09 10b5 085c 6461  .............\da
+00004cf0: 7465 4d6f 6469 6669 6564 d40d 0e0f 1016  teModified......
+00004d00: 1c16 2208 085b 6461 7465 4372 6561 7465  .."..[dateCreate
+00004d10: 64d4 0d0e 0f10 0a25 1627 0910 6108 5473  d......%.'..a.Ts
+00004d20: 697a 65d4 0d0e 0f10 0a2a 0a2c 0910 7309  ize......*.,..s.
+00004d30: 546b 696e 64d4 0d0e 0f10 162f 0a31 0810  Tkind....../.1..
+00004d40: 6409 556c 6162 656c d40d 0e0f 1016 340a  d.Ulabel......4.
+00004d50: 3608 104b 0957 7665 7273 696f 6ed4 0d0e  6..K.Wversion...
+00004d60: 0f10 1639 0a3b 0811 012c 0958 636f 6d6d  ...9.;...,.Xcomm
+00004d70: 656e 7473 d40d 0e0f 1016 3e16 4008 10c8  ents......>.@...
+00004d80: 085e 6461 7465 4c61 7374 4f70 656e 6564  .^dateLastOpened
+00004d90: d40d 0e0f 1016 1c16 4408 0859 6461 7465  ........D..Ydate
+00004da0: 4164 6465 6408 2340 2800 0000 0000 0054  Added.#@(......T
+00004db0: 6e61 6d65 2340 3000 0000 0000 0009 0008  name#@0.........
+00004dc0: 0019 002e 0040 0048 005c 0065 0070 0079  .....@.H.\.e.p.y
+00004dd0: 008c 008e 008f 009b 00a4 00ac 00b2 00bc  ................
+00004de0: 00c7 00c8 00cb 00cc 00d1 00da 00db 00dd  ................
+00004df0: 00de 00e7 00f0 00f1 00f3 00f4 0101 010a  ................
+00004e00: 010b 010c 0118 0121 0122 0124 0125 012a  .......!.".$.%.*
+00004e10: 0133 0134 0136 0137 013c 0145 0146 0148  .3.4.6.7.<.E.F.H
+00004e20: 0149 014f 0158 0159 015b 015c 0164 016d  .I.O.X.Y.[.\.d.m
+00004e30: 016e 0171 0172 017b 0184 0185 0187 0188  .n.q.r.{........
+00004e40: 0197 01a0 01a1 01a2 01ac 01ad 01b6 01bb  ................
+00004e50: 01c4 0000 0000 0000 0201 0000 0000 0000  ................
+00004e60: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
+00004e70: 01c5 0000 0000 0000 0000 0000 0000 0000  ................
+00004e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1285,15 +1285,15 @@
 00005040: 1799 b1f1 cc0c c541 0000 0012 0062 006f  .......A.....b.o
 00005050: 0075 006e 0064 0069 006e 0067 005f 0062  .u.n.d.i.n.g._.b
 00005060: 006f 0078 005f 0074 006f 006f 006c 0073  .o.x._.t.o.o.l.s
 00005070: 6d6f 6444 626c 6f62 0000 0008 1799 b1f1  modDblob........
 00005080: cc0c c541 0000 0012 0062 006f 0075 006e  ...A.....b.o.u.n
 00005090: 0064 0069 006e 0067 005f 0062 006f 0078  .d.i.n.g._.b.o.x
 000050a0: 005f 0074 006f 006f 006c 0073 7068 3153  ._.t.o.o.l.sph1S
-000050b0: 636f 6d70 0000 0000 0001 f000 0000 0012  comp............
+000050b0: 636f 6d70 0000 0000 0002 c000 0000 0012  comp............
 000050c0: 0062 006f 0075 006e 0064 0069 006e 0067  .b.o.u.n.d.i.n.g
 000050d0: 005f 0062 006f 0078 005f 0074 006f 006f  ._.b.o.x._.t.o.o
 000050e0: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
 000050f0: 0000 000f 0063 0075 0065 005f 006c 0069  .....c.u.e._.l.i
 00005100: 0067 0068 0074 005f 0074 006f 006f 006c  .g.h.t._.t.o.o.l
 00005110: 0073 6277 7370 626c 6f62 0000 00c9 6270  .sbwspblob....bp
 00005120: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
@@ -1310,25 +1310,25 @@
 000051d0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
 000051e0: 0000 0000 0000 9a00 0000 0f00 6300 7500  ............c.u.
 000051f0: 6500 5f00 6c00 6900 6700 6800 7400 5f00  e._.l.i.g.h.t._.
 00005200: 7400 6f00 6f00 6c00 7364 7363 6c62 6f6f  t.o.o.l.sdsclboo
 00005210: 6c00 0000 000f 0063 0075 0065 005f 006c  l......c.u.e._.l
 00005220: 0069 0067 0068 0074 005f 0074 006f 006f  .i.g.h.t._.t.o.o
 00005230: 006c 0073 6c67 3153 636f 6d70 0000 0000  .l.slg1Scomp....
-00005240: 0001 da29 0000 000f 0063 0075 0065 005f  ...).....c.u.e._
+00005240: 0002 98a5 0000 000f 0063 0075 0065 005f  .........c.u.e._
 00005250: 006c 0069 0067 0068 0074 005f 0074 006f  .l.i.g.h.t._.t.o
 00005260: 006f 006c 0073 6d6f 4444 626c 6f62 0000  .o.l.smoDDblob..
 00005270: 0008 00ae d77f cc0c c541 0000 000f 0063  .........A.....c
 00005280: 0075 0065 005f 006c 0069 0067 0068 0074  .u.e._.l.i.g.h.t
 00005290: 005f 0074 006f 006f 006c 0073 6d6f 6444  ._.t.o.o.l.smodD
 000052a0: 626c 6f62 0000 0008 00ae d77f cc0c c541  blob...........A
 000052b0: 0000 000f 0063 0075 0065 005f 006c 0069  .....c.u.e._.l.i
 000052c0: 0067 0068 0074 005f 0074 006f 006f 006c  .g.h.t._.t.o.o.l
-000052d0: 0073 7068 3153 636f 6d70 0000 0000 0002  .sph1Scomp......
-000052e0: 6000 0000 000f 0063 0075 0065 005f 006c  `......c.u.e._.l
+000052d0: 0073 7068 3153 636f 6d70 0000 0000 0003  .sph1Scomp......
+000052e0: 7000 0000 000f 0063 0075 0065 005f 006c  p......c.u.e._.l
 000052f0: 0069 0067 0068 0074 005f 0074 006f 006f  .i.g.h.t._.t.o.o
 00005300: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
 00005310: 0000 0008 0064 0061 0073 0068 005f 0061  .....d.a.s.h._.a
 00005320: 0070 0070 6277 7370 626c 6f62 0000 00c9  .p.pbwspblob....
 00005330: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
 00005340: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
 00005350: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
@@ -1341,18 +1341,18 @@
 000053c0: 3237 2c20 3536 387d 7d09 0817 2531 3d49  27, 568}}...%1=I
 000053d0: 606d 797a 7b7c 7d7e 9900 0000 0000 0001  `myz{|}~........
 000053e0: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 000053f0: 0000 0000 0000 0000 9a00 0000 0800 6400  ..............d.
 00005400: 6100 7300 6800 5f00 6100 7000 706c 6731  a.s.h._.a.p.plg1
 00005410: 5363 6f6d 7000 0000 0000 0135 6200 0000  Scomp......5b...
 00005420: 0800 6400 6100 7300 6800 5f00 6100 7000  ..d.a.s.h._.a.p.
-00005430: 706d 6f44 4462 6c6f 6200 0000 087e 81a5  pmoDDblob....~..
-00005440: d736 fec4 4100 0000 0800 6400 6100 7300  .6..A.....d.a.s.
+00005430: 706d 6f44 4462 6c6f 6200 0000 0874 2dd3  pmoDDblob....t-.
+00005440: 1049 1ec5 4100 0000 0800 6400 6100 7300  .I..A.....d.a.s.
 00005450: 6800 5f00 6100 7000 706d 6f64 4462 6c6f  h._.a.p.pmodDblo
-00005460: 6200 0000 087e 81a5 d736 fec4 4100 0000  b....~...6..A...
+00005460: 6200 0000 0874 2dd3 1049 1ec5 4100 0000  b....t-..I..A...
 00005470: 0800 6400 6100 7300 6800 5f00 6100 7000  ..d.a.s.h._.a.p.
 00005480: 7070 6831 5363 6f6d 7000 0000 0000 0150  pph1Scomp......P
 00005490: 0000 0000 0800 6400 6100 7300 6800 5f00  ......d.a.s.h._.
 000054a0: 6100 7000 7076 5372 6e6c 6f6e 6700 0000  a.p.pvSrnlong...
 000054b0: 0100 0000 0f00 6400 6100 7400 6100 5f00  ......d.a.t.a._.
 000054c0: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
 000054d0: 7200 7362 7773 7062 6c6f 6200 0000 ca62  r.sbwspblob....b
@@ -1370,15 +1370,15 @@
 00005590: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 000055a0: 0000 0000 0000 0000 9b00 0000 0f00 6400  ..............d.
 000055b0: 6100 7400 6100 5f00 7000 7200 6f00 6300  a.t.a._.p.r.o.c.
 000055c0: 6500 7300 7300 6f00 7200 7364 7363 6c62  e.s.s.o.r.sdsclb
 000055d0: 6f6f 6c00 0000 000f 0064 0061 0074 0061  ool......d.a.t.a
 000055e0: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
 000055f0: 006f 0072 0073 6c67 3153 636f 6d70 0000  .o.r.slg1Scomp..
-00005600: 0000 0003 9633 0000 000f 0064 0061 0074  .....3.....d.a.t
+00005600: 0000 0005 24b1 0000 000f 0064 0061 0074  ....$......d.a.t
 00005610: 0061 005f 0070 0072 006f 0063 0065 0073  .a._.p.r.o.c.e.s
 00005620: 0073 006f 0072 0073 6c73 7643 626c 6f62  .s.o.r.slsvCblob
 00005630: 0000 0281 6270 6c69 7374 3030 d801 0203  ....bplist00....
 00005640: 0405 0607 0809 0a0b 1646 4748 0a5f 1012  .........FGH._..
 00005650: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
 00005660: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
 00005670: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
@@ -1457,22 +1457,22 @@
 00005b00: 6301 6501 6e01 6f01 7101 7201 7401 7d01  c.e.n.o.q.r.t.}.
 00005b10: 7e01 8001 8101 8301 8c01 8d01 9001 9101  ~...............
 00005b20: 9301 9401 9d01 aa01 b300 0000 0000 0002  ................
 00005b30: 0100 0000 0000 0000 4900 0000 0000 0000  ........I.......
 00005b40: 0000 0000 0000 0001 b400 0000 0f00 6400  ..............d.
 00005b50: 6100 7400 6100 5f00 7000 7200 6f00 6300  a.t.a._.p.r.o.c.
 00005b60: 6500 7300 7300 6f00 7200 736d 6f44 4462  e.s.s.o.r.smoDDb
-00005b70: 6c6f 6200 0000 0853 3db3 ac56 1cc5 4100  lob....S=..V..A.
+00005b70: 6c6f 6200 0000 082d 2344 c1db 1dc5 4100  lob....-#D....A.
 00005b80: 0000 0f00 6400 6100 7400 6100 5f00 7000  ....d.a.t.a._.p.
 00005b90: 7200 6f00 6300 6500 7300 7300 6f00 7200  r.o.c.e.s.s.o.r.
-00005ba0: 736d 6f64 4462 6c6f 6200 0000 0853 3db3  smodDblob....S=.
-00005bb0: ac56 1cc5 4100 0000 0f00 6400 6100 7400  .V..A.....d.a.t.
+00005ba0: 736d 6f64 4462 6c6f 6200 0000 082d 2344  smodDblob....-#D
+00005bb0: c1db 1dc5 4100 0000 0f00 6400 6100 7400  ....A.....d.a.t.
 00005bc0: 6100 5f00 7000 7200 6f00 6300 6500 7300  a._.p.r.o.c.e.s.
 00005bd0: 7300 6f00 7200 7370 6831 5363 6f6d 7000  s.o.r.sph1Scomp.
-00005be0: 0000 0000 0480 0000 0000 0f00 6400 6100  ............d.a.
+00005be0: 0000 0000 0690 0000 0000 0f00 6400 6100  ............d.a.
 00005bf0: 7400 6100 5f00 7000 7200 6f00 6300 6500  t.a._.p.r.o.c.e.
 00005c00: 7300 7300 6f00 7200 7376 5372 6e6c 6f6e  s.s.o.r.svSrnlon
 00005c10: 6700 0000 0100 0000 1200 6600 6500 6100  g.........f.e.a.
 00005c20: 7400 7500 7200 6500 5f00 6500 7800 7400  t.u.r.e._.e.x.t.
 00005c30: 7200 6100 6300 7400 6f00 7200 7362 7773  r.a.c.t.o.r.sbws
 00005c40: 7062 6c6f 6200 0000 c962 706c 6973 7430  pblob....bplist0
 00005c50: 30d7 0102 0304 0506 0708 080a 080a 0d0a  0...............
@@ -1489,32 +1489,32 @@
 00005d00: 000f 0000 0000 0000 0000 0000 0000 0000  ................
 00005d10: 009a 0000 0012 0066 0065 0061 0074 0075  .......f.e.a.t.u
 00005d20: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
 00005d30: 0063 0074 006f 0072 0073 6473 636c 626f  .c.t.o.r.sdsclbo
 00005d40: 6f6c 0000 0000 1200 6600 6500 6100 7400  ol......f.e.a.t.
 00005d50: 7500 7200 6500 5f00 6500 7800 7400 7200  u.r.e._.e.x.t.r.
 00005d60: 6100 6300 7400 6f00 7200 736c 6731 5363  a.c.t.o.r.slg1Sc
-00005d70: 6f6d 7000 0000 0000 0903 cb09 5863 6f6d  omp.........Xcom
-00005d80: 6d65 6e74 73d4 0d0e 0f10 163e 1640 0810  ments......>.@..
-00005d90: c808 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
-00005da0: 64d4 0d0e 0f10 161c 1644 0808 5964 6174  d........D..Ydat
-00005db0: 6541 6464 6564 0823 4028 0000 0000 0000  eAdded.#@(......
-00005dc0: 546e 616d 6523 4030 0000 0000 0000 0900  Tname#@0........
-00005dd0: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
-00005de0: 7900 8c00 8e00 8f00 9b00 a400 ac00 b200  y...............
-00005df0: bc00 c700 c800 cb00 cc00 d100 da00 db00  ................
-00005e00: dd00 de00 e700 f000 f100 f300 f401 0101  ................
-00005e10: 0a01 0b01 0c01 1801 2101 2201 2401 2501  ........!.".$.%.
-00005e20: 2a01 3301 3401 3601 3701 3c01 4501 4601  *.3.4.6.7.<.E.F.
-00005e30: 4801 4901 4f01 5801 5901 5b01 5c01 6401  H.I.O.X.Y.[.\.d.
-00005e40: 6d01 6e01 7101 7201 7b01 8401 8501 8701  m.n.q.r.{.......
-00005e50: 8801 9701 a001 a101 a201 ac01 ad01 b601  ................
-00005e60: bb01 c400 0000 0000 0002 0100 0000 0000  ................
-00005e70: 0000 4a00 0000 0000 0000 0000 0000 0000  ..J.............
-00005e80: 0001 c500 0000 0000 0000 0000 0000 0000  ................
+00005d70: 6f6d 7000 0000 0000 093f 8016 4008 10c8  omp......?..@...
+00005d80: 085e 6461 7465 4c61 7374 4f70 656e 6564  .^dateLastOpened
+00005d90: d40d 0e0f 1016 1c16 4408 0859 6461 7465  ........D..Ydate
+00005da0: 4164 6465 6408 2340 2800 0000 0000 0054  Added.#@(......T
+00005db0: 6e61 6d65 2340 3000 0000 0000 0009 0008  name#@0.........
+00005dc0: 0019 002e 0040 0048 005c 0065 0070 0079  .....@.H.\.e.p.y
+00005dd0: 008c 008e 008f 009b 00a4 00ac 00b2 00bc  ................
+00005de0: 00c7 00c8 00cb 00cc 00d1 00da 00db 00dd  ................
+00005df0: 00de 00e7 00f0 00f1 00f3 00f4 0101 010a  ................
+00005e00: 010b 010c 0118 0121 0122 0124 0125 012a  .......!.".$.%.*
+00005e10: 0133 0134 0136 0137 013c 0145 0146 0148  .3.4.6.7.<.E.F.H
+00005e20: 0149 014f 0158 0159 015b 015c 0164 016d  .I.O.X.Y.[.\.d.m
+00005e30: 016e 0171 0172 017b 0184 0185 0187 0188  .n.q.r.{........
+00005e40: 0197 01a0 01a1 01a2 01ac 01ad 01b6 01bb  ................
+00005e50: 01c4 0000 0000 0000 0201 0000 0000 0000  ................
+00005e60: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
+00005e70: 01c5 0000 0000 0000 0000 0000 0000 0000  ................
+00005e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1586,15 +1586,15 @@
 00006310: 0869 3ef0 203f 0dc5 4100 0000 1200 6600  .i>. ?..A.....f.
 00006320: 6500 6100 7400 7500 7200 6500 5f00 6500  e.a.t.u.r.e._.e.
 00006330: 7800 7400 7200 6100 6300 7400 6f00 7200  x.t.r.a.c.t.o.r.
 00006340: 736d 6f64 4462 6c6f 6200 0000 0869 3ef0  smodDblob....i>.
 00006350: 203f 0dc5 4100 0000 1200 6600 6500 6100   ?..A.....f.e.a.
 00006360: 7400 7500 7200 6500 5f00 6500 7800 7400  t.u.r.e._.e.x.t.
 00006370: 7200 6100 6300 7400 6f00 7200 7370 6831  r.a.c.t.o.r.sph1
-00006380: 5363 6f6d 7000 0000 0000 0b10 0000 0000  Scomp...........
+00006380: 5363 6f6d 7000 0000 0000 0b60 0000 0000  Scomp......`....
 00006390: 1200 6600 6500 6100 7400 7500 7200 6500  ..f.e.a.t.u.r.e.
 000063a0: 5f00 6500 7800 7400 7200 6100 6300 7400  _.e.x.t.r.a.c.t.
 000063b0: 6f00 7200 7376 5372 6e6c 6f6e 6700 0000  o.r.svSrnlong...
 000063c0: 0100 0000 0900 6c00 6100 6200 6500 6c00  ......l.a.b.e.l.
 000063d0: 6c00 6900 6e00 6762 7773 7062 6c6f 6200  l.i.n.gbwspblob.
 000063e0: 0000 c962 706c 6973 7430 30d7 0102 0304  ...bplist00.....
 000063f0: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
@@ -1606,16 +1606,16 @@
 00006450: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
 00006460: 095f 1018 7b7b 3333 352c 2031 3938 7d2c  ._..{{335, 198},
 00006470: 207b 3932 372c 2035 3638 7d7d 0908 1725   {927, 568}}...%
 00006480: 313d 4960 6d79 7a7b 7c7d 7e99 0000 0000  1=I`myz{|}~.....
 00006490: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 000064a0: 0000 0000 0000 0000 0000 009a 0000 0009  ................
 000064b0: 006c 0061 0062 0065 006c 006c 0069 006e  .l.a.b.e.l.l.i.n
-000064c0: 0067 6c67 3153 636f 6d70 0000 0000 0001  .glg1Scomp......
-000064d0: 9f56 0000 0009 006c 0061 0062 0065 006c  .V.....l.a.b.e.l
+000064c0: 0067 6c67 3153 636f 6d70 0000 0000 0002  .glg1Scomp......
+000064d0: 35ef 0000 0009 006c 0061 0062 0065 006c  5......l.a.b.e.l
 000064e0: 006c 0069 006e 0067 6c73 7643 626c 6f62  .l.i.n.glsvCblob
 000064f0: 0000 0279 6270 6c69 7374 3030 d801 0203  ...ybplist00....
 00006500: 0405 0607 0809 0a0b 1646 4748 0a5f 1012  .........FGH._..
 00006510: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
 00006520: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
 00006530: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
 00006540: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
@@ -1696,15 +1696,15 @@
 000069f0: 0900 6c00 6100 6200 6500 6c00 6c00 6900  ..l.a.b.e.l.l.i.
 00006a00: 6e00 676d 6f44 4462 6c6f 6200 0000 0834  n.gmoDDblob....4
 00006a10: 23b2 c431 1bc5 4100 0000 0900 6c00 6100  #..1..A.....l.a.
 00006a20: 6200 6500 6c00 6c00 6900 6e00 676d 6f64  b.e.l.l.i.n.gmod
 00006a30: 4462 6c6f 6200 0000 0834 23b2 c431 1bc5  Dblob....4#..1..
 00006a40: 4100 0000 0900 6c00 6100 6200 6500 6c00  A.....l.a.b.e.l.
 00006a50: 6c00 6900 6e00 6770 6831 5363 6f6d 7000  l.i.n.gph1Scomp.
-00006a60: 0000 0000 01e0 0000 0000 0900 6c00 6100  ............l.a.
+00006a60: 0000 0000 0290 0000 0000 0900 6c00 6100  ............l.a.
 00006a70: 6200 6500 6c00 6c00 6900 6e00 6776 5372  b.e.l.l.i.n.gvSr
 00006a80: 6e6c 6f6e 6700 0000 0100 0000 0600 6d00  nlong.........m.
 00006a90: 6900 7800 6900 6e00 7362 7773 7062 6c6f  i.x.i.n.sbwspblo
 00006aa0: 6200 0000 c862 706c 6973 7430 30d7 0102  b....bplist00...
 00006ab0: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
 00006ac0: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
 00006ad0: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
@@ -1714,15 +1714,15 @@
 00006b10: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
 00006b20: 0908 095f 1017 7b7b 302c 2031 3035 7d2c  ..._..{{0, 105},
 00006b30: 207b 3131 3939 2c20 3736 397d 7d09 0817   {1199, 769}}...
 00006b40: 2531 3d49 606d 797a 7b7c 7d7e 9800 0000  %1=I`myz{|}~....
 00006b50: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
 00006b60: 0000 0000 0000 0000 0000 0000 9900 0000  ................
 00006b70: 0600 6d00 6900 7800 6900 6e00 736c 6731  ..m.i.x.i.n.slg1
-00006b80: 5363 6f6d 7000 0000 0000 0a25 9900 0000  Scomp......%....
+00006b80: 5363 6f6d 7000 0000 0000 0d3e 5500 0000  Scomp......>U...
 00006b90: 0600 6d00 6900 7800 6900 6e00 736c 7376  ..m.i.x.i.n.slsv
 00006ba0: 4362 6c6f 6200 0002 8162 706c 6973 7430  Cblob....bplist0
 00006bb0: 30d8 0102 0304 0506 0708 090a 0b16 4647  0.............FG
 00006bc0: 480a 5f10 1276 6965 774f 7074 696f 6e73  H._..viewOptions
 00006bd0: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
 00006be0: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
 00006bf0: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
@@ -1756,21 +1756,21 @@
 00006db0: 00ff 0100 0101 010a 0116 0117 0118 0121  ...............!
 00006dc0: 0126 0128 0129 012a 0133 0138 013a 013b  .&.(.).*.3.8.:.;
 00006dd0: 013c 0145 014b 014d 014e 014f 0158 0160  .<.E.K.M.N.O.X.`
 00006de0: 0162 0163 0164 016d 0176 0179 017a 017b  .b.c.d.m.v.y.z.{
 00006df0: 0184 0193 0195 0196 0197 01a0 01a1 01a2  ................
 00006e00: 01ac 01ad 01b6 01c3 01cc 0000 0000 0000  ................
 00006e10: 0201 0000 0000 0000 004a 0000 0000 0000  .........J......
-00006e20: 0000 0000 0000 0000 01cd 3c01 4501 4601  ..........<.E.F.
-00006e30: 4801 4901 4f01 5801 5901 5b01 5c01 6401  H.I.O.X.Y.[.\.d.
-00006e40: 6d01 6e01 7101 7201 7b01 8401 8501 8701  m.n.q.r.{.......
-00006e50: 8801 9701 a001 a101 a201 ac01 ad01 b601  ................
-00006e60: bb01 c400 0000 0000 0002 0100 0000 0000  ................
-00006e70: 0000 4a00 0000 0000 0000 0000 0000 0000  ..J.............
-00006e80: 0001 c500 0000 0000 0000 0000 0000 0000  ................
+00006e20: 0000 0000 0000 0000 01cd 015c 0164 016d  ...........\.d.m
+00006e30: 016e 0171 0172 017b 0184 0185 0187 0188  .n.q.r.{........
+00006e40: 0197 01a0 01a1 01a2 01ac 01ad 01b6 01bb  ................
+00006e50: 01c4 0000 0000 0000 0201 0000 0000 0000  ................
+00006e60: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
+00006e70: 01c5 0000 0000 0000 0000 0000 0000 0000  ................
+00006e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1788,20 +1788,20 @@
 00006fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007000: 0000 0000 0000 0000 0000 0016 0000 0006  ................
 00007010: 006d 0069 0078 0069 006e 0073 6d6f 4444  .m.i.x.i.n.smoDD
-00007020: 626c 6f62 0000 0008 86ab 263d 9118 c541  blob......&=...A
+00007020: 626c 6f62 0000 0008 6a17 4f60 b41d c541  blob....j.O`...A
 00007030: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
-00007040: 6d6f 6444 626c 6f62 0000 0008 86ab 263d  modDblob......&=
-00007050: 9118 c541 0000 0006 006d 0069 0078 0069  ...A.....m.i.x.i
+00007040: 6d6f 6444 626c 6f62 0000 0008 6a17 4f60  modDblob....j.O`
+00007050: b41d c541 0000 0006 006d 0069 0078 0069  ...A.....m.i.x.i
 00007060: 006e 0073 7068 3153 636f 6d70 0000 0000  .n.sph1Scomp....
-00007070: 000b 0000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
+00007070: 000e 6000 0000 0006 006d 0069 0078 0069  ..`......m.i.x.i
 00007080: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00007090: 0000 0005 006d 006f 0064 0065 006c 6277  .....m.o.d.e.lbw
 000070a0: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
 000070b0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 000070c0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 000070d0: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
 000070e0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
@@ -1810,16 +1810,16 @@
 00007110: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
 00007120: 6261 7208 0809 0809 5f10 187b 7b33 3037  bar....._..{{307
 00007130: 2c20 3836 7d2c 207b 3130 3736 2c20 3632  , 86}, {1076, 62
 00007140: 317d 7d09 0817 2531 3d49 606d 797a 7b7c  1}}...%1=I`myz{|
 00007150: 7d7e 9900 0000 0000 0001 0100 0000 0000  }~..............
 00007160: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
 00007170: 0000 9a00 0000 0500 6d00 6f00 6400 6500  ........m.o.d.e.
-00007180: 6c6c 6731 5363 6f6d 7000 0000 0000 013b  llg1Scomp......;
-00007190: 3700 0000 0500 6d00 6f00 6400 6500 6c6c  7.....m.o.d.e.ll
+00007180: 6c6c 6731 5363 6f6d 7000 0000 0000 01a4  llg1Scomp.......
+00007190: 7d00 0000 0500 6d00 6f00 6400 6500 6c6c  }.....m.o.d.e.ll
 000071a0: 7376 4362 6c6f 6200 0002 7962 706c 6973  svCblob...ybplis
 000071b0: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
 000071c0: 4647 0a49 5869 636f 6e53 697a 655f 100f  FG.IXiconSize_..
 000071d0: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
 000071e0: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
 000071f0: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
 00007200: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e5f  SizeZsortColumn_
@@ -1897,15 +1897,15 @@
 00007680: 0000 0201 0000 0000 0000 0049 0000 0000  ...........I....
 00007690: 0000 0000 0000 0000 0000 01ac 0000 0005  ................
 000076a0: 006d 006f 0064 0065 006c 6d6f 4444 626c  .m.o.d.e.lmoDDbl
 000076b0: 6f62 0000 0008 574d 2d38 4017 c541 0000  ob....WM-8@..A..
 000076c0: 0005 006d 006f 0064 0065 006c 6d6f 6444  ...m.o.d.e.lmodD
 000076d0: 626c 6f62 0000 0008 574d 2d38 4017 c541  blob....WM-8@..A
 000076e0: 0000 0005 006d 006f 0064 0065 006c 7068  .....m.o.d.e.lph
-000076f0: 3153 636f 6d70 0000 0000 0001 7000 0000  1Scomp......p...
+000076f0: 3153 636f 6d70 0000 0000 0001 f000 0000  1Scomp..........
 00007700: 0005 006d 006f 0064 0065 006c 7653 726e  ...m.o.d.e.lvSrn
 00007710: 6c6f 6e67 0000 0001 0000 000d 006f 0075  long.........o.u
 00007720: 0074 006c 0069 0065 0072 005f 0074 006f  .t.l.i.e.r._.t.o
 00007730: 006f 006c 0073 6277 7370 626c 6f62 0000  .o.l.sbwspblob..
 00007740: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
 00007750: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
 00007760: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
@@ -1917,15 +1917,15 @@
 000077c0: 5f10 197b 7b33 3534 2c20 3132 347d 2c20  _..{{354, 124}, 
 000077d0: 7b31 3037 362c 2036 3231 7d7d 0908 1725  {1076, 621}}...%
 000077e0: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
 000077f0: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 00007800: 0000 0000 0000 0000 0000 009b 0000 000d  ................
 00007810: 006f 0075 0074 006c 0069 0065 0072 005f  .o.u.t.l.i.e.r._
 00007820: 0074 006f 006f 006c 0073 6c67 3153 636f  .t.o.o.l.slg1Sco
-00007830: 6d70 0000 0000 0000 bdc6 0000 000d 006f  mp.............o
+00007830: 6d70 0000 0000 0000 f7bc 0000 000d 006f  mp.............o
 00007840: 0075 0074 006c 0069 0065 0072 005f 0074  .u.t.l.i.e.r._.t
 00007850: 006f 006f 006c 0073 6c73 7643 626c 6f62  .o.o.l.slsvCblob
 00007860: 0000 02b0 6270 6c69 7374 3030 da01 0203  ....bplist00....
 00007870: 0405 0607 0809 0a0b 0c0d 1848 4948 4a0c  ...........HIHJ.
 00007880: 4c5f 1012 7669 6577 4f70 7469 6f6e 7356  L_..viewOptionsV
 00007890: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
 000078a0: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
@@ -2016,15 +2016,15 @@
 00007df0: 736d 6f44 4462 6c6f 6200 0000 08aa 2e11  smoDDblob.......
 00007e00: 6564 14c5 4100 0000 0d00 6f00 7500 7400  ed..A.....o.u.t.
 00007e10: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
 00007e20: 6c00 736d 6f64 4462 6c6f 6200 0000 08aa  l.smodDblob.....
 00007e30: 2e11 6564 14c5 4100 0000 0d00 6f00 7500  ..ed..A.....o.u.
 00007e40: 7400 6c00 6900 6500 7200 5f00 7400 6f00  t.l.i.e.r._.t.o.
 00007e50: 6f00 6c00 7370 6831 5363 6f6d 7000 0000  o.l.sph1Scomp...
-00007e60: 0000 0150 0000 0000 0d00 6f00 7500 7400  ...P......o.u.t.
+00007e60: 0000 01b0 0000 0000 0d00 6f00 7500 7400  ..........o.u.t.
 00007e70: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
 00007e80: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
 00007e90: 0000 0800 7000 6c00 6f00 7400 7400 6900  ....p.l.o.t.t.i.
 00007ea0: 6e00 6762 7773 7062 6c6f 6200 0000 ca62  n.gbwspblob....b
 00007eb0: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
 00007ec0: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
 00007ed0: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
@@ -2035,15 +2035,15 @@
 00007f20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
 00007f30: 7b7b 3238 372c 2031 3036 7d2c 207b 3130  {{287, 106}, {10
 00007f40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
 00007f50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
 00007f60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 00007f70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
 00007f80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
-00007f90: 5363 6f6d 7000 0000 0000 08c5 3600 0000  Scomp.......6...
+00007f90: 5363 6f6d 7000 0000 0000 0c7f 3d00 0000  Scomp.......=...
 00007fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008000: 0000 0000 0000 0000 0000 0015 0000 0008  ................
@@ -2088,20 +2088,20 @@
 00008270: 7a01 7c01 7d01 7e01 8701 8901 8b01 8c01  z.|.}.~.........
 00008280: 8d01 9601 9801 9a01 9b01 9c01 a501 a701  ................
 00008290: a901 aa01 ab01 b401 b601 b901 ba01 bb01  ................
 000082a0: bc01 c501 ce01 db01 e400 0000 0000 0002  ................
 000082b0: 0100 0000 0000 0000 4c00 0000 0000 0000  ........L.......
 000082c0: 0000 0000 0000 0001 e500 0000 0800 7000  ..............p.
 000082d0: 6c00 6f00 7400 7400 6900 6e00 676d 6f44  l.o.t.t.i.n.gmoD
-000082e0: 4462 6c6f 6200 0000 08a5 6a92 865a 16c5  Dblob.....j..Z..
+000082e0: 4462 6c6f 6200 0000 083d d3c5 a9d2 1dc5  Dblob....=......
 000082f0: 4100 0000 0800 7000 6c00 6f00 7400 7400  A.....p.l.o.t.t.
 00008300: 6900 6e00 676d 6f64 4462 6c6f 6200 0000  i.n.gmodDblob...
-00008310: 08a5 6a92 865a 16c5 4100 0000 0800 7000  ..j..Z..A.....p.
+00008310: 083d d3c5 a9d2 1dc5 4100 0000 0800 7000  .=......A.....p.
 00008320: 6c00 6f00 7400 7400 6900 6e00 6770 6831  l.o.t.t.i.n.gph1
-00008330: 5363 6f6d 7000 0000 0000 0ae0 0000 0000  Scomp...........
+00008330: 5363 6f6d 7000 0000 0000 0fb0 0000 0000  Scomp...........
 00008340: 0800 7000 6c00 6f00 7400 7400 6900 6e00  ..p.l.o.t.t.i.n.
 00008350: 6776 5372 6e6c 6f6e 6700 0000 0100 0000  gvSrnlong.......
 00008360: 1300 7000 6f00 7300 6500 5f00 6300 6f00  ..p.o.s.e._.c.o.
 00008370: 6e00 6600 6900 6700 7500 7200 6100 7400  n.f.i.g.u.r.a.t.
 00008380: 6900 6f00 6e00 7362 7773 7062 6c6f 6200  i.o.n.sbwspblob.
 00008390: 0000 ca62 706c 6973 7430 30d7 0102 0304  ...bplist00.....
 000083a0: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
@@ -2264,23 +2264,23 @@
 00008d70: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 00008d80: 0000 0000 0000 0000 0000 009a 0000 000e  ................
 00008d90: 0070 006f 0073 0065 005f 0069 006d 0070  .p.o.s.e._.i.m.p
 00008da0: 006f 0072 0074 0065 0072 0073 6473 636c  .o.r.t.e.r.sdscl
 00008db0: 626f 6f6c 0000 0000 0e00 7000 6f00 7300  bool......p.o.s.
 00008dc0: 6500 5f00 6900 6d00 7000 6f00 7200 7400  e._.i.m.p.o.r.t.
 00008dd0: 6500 7200 736c 6731 5363 6f6d 7000 0000  e.r.slg1Scomp...
-00008de0: 0000 020c 7a00 5f00 7400 6f00 6f00 6c00  ....z._.t.o.o.l.
+00008de0: 0000 02c9 b900 5f00 7400 6f00 6f00 6c00  ......_.t.o.o.l.
 00008df0: 736d 6f44 4462 6c6f 6200 0000 08aa 2e11  smoDDblob.......
 00008e00: 6564 14c5 4100 0000 0d00 6f00 7500 7400  ed..A.....o.u.t.
 00008e10: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
 00008e20: 6c00 736d 6f64 4462 6c6f 6200 0000 08aa  l.smodDblob.....
 00008e30: 2e11 6564 14c5 4100 0000 0d00 6f00 7500  ..ed..A.....o.u.
 00008e40: 7400 6c00 6900 6500 7200 5f00 7400 6f00  t.l.i.e.r._.t.o.
 00008e50: 6f00 6c00 7370 6831 5363 6f6d 7000 0000  o.l.sph1Scomp...
-00008e60: 0000 0150 0000 0000 0d00 6f00 7500 7400  ...P......o.u.t.
+00008e60: 0000 01b0 0000 0000 0d00 6f00 7500 7400  ..........o.u.t.
 00008e70: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
 00008e80: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
 00008e90: 0000 0800 7000 6c00 6f00 7400 7400 6900  ....p.l.o.t.t.i.
 00008ea0: 6e00 6762 7773 7062 6c6f 6200 0000 ca62  n.gbwspblob....b
 00008eb0: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
 00008ec0: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
 00008ed0: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
@@ -2291,15 +2291,15 @@
 00008f20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
 00008f30: 7b7b 3238 372c 2031 3036 7d2c 207b 3130  {{287, 106}, {10
 00008f40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
 00008f50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
 00008f60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 00008f70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
 00008f80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
-00008f90: 5363 6f6d 7000 0000 0000 08c5 3600 0000  Scomp.......6...
+00008f90: 5363 6f6d 7000 0000 0000 0c7f 3d00 0000  Scomp.......=...
 00008fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009000: 0000 0000 0000 0000 0000 0010 0000 000e  ................
@@ -2349,15 +2349,15 @@
 000092c0: 4444 626c 6f62 0000 0008 23bd 51ed cc0c  DDblob....#.Q...
 000092d0: c541 0000 000e 0070 006f 0073 0065 005f  .A.....p.o.s.e._
 000092e0: 0069 006d 0070 006f 0072 0074 0065 0072  .i.m.p.o.r.t.e.r
 000092f0: 0073 6d6f 6444 626c 6f62 0000 0008 23bd  .smodDblob....#.
 00009300: 51ed cc0c c541 0000 000e 0070 006f 0073  Q....A.....p.o.s
 00009310: 0065 005f 0069 006d 0070 006f 0072 0074  .e._.i.m.p.o.r.t
 00009320: 0065 0072 0073 7068 3153 636f 6d70 0000  .e.r.sph1Scomp..
-00009330: 0000 0002 8000 0000 000e 0070 006f 0073  ...........p.o.s
+00009330: 0000 0003 8000 0000 000e 0070 006f 0073  ...........p.o.s
 00009340: 0065 005f 0069 006d 0070 006f 0072 0074  .e._.i.m.p.o.r.t
 00009350: 0065 0072 0073 7653 726e 6c6f 6e67 0000  .e.r.svSrnlong..
 00009360: 0001 0000 000f 0070 006f 0073 0065 005f  .......p.o.s.e._
 00009370: 0070 0072 006f 0063 0065 0073 0073 006f  .p.r.o.c.e.s.s.o
 00009380: 0072 0073 6277 7370 626c 6f62 0000 00ca  .r.sbwspblob....
 00009390: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
 000093a0: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
@@ -2370,15 +2370,15 @@
 00009410: 197b 7b32 3332 2c20 3139 317d 2c20 7b31  .{{232, 191}, {1
 00009420: 3330 322c 2037 3134 7d7d 0908 1725 313d  302, 714}}...%1=
 00009430: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
 00009440: 0101 0000 0000 0000 000f 0000 0000 0000  ................
 00009450: 0000 0000 0000 0000 009b 0000 000f 0070  ...............p
 00009460: 006f 0073 0065 005f 0070 0072 006f 0063  .o.s.e._.p.r.o.c
 00009470: 0065 0073 0073 006f 0072 0073 6c67 3153  .e.s.s.o.r.slg1S
-00009480: 636f 6d70 0000 0000 0000 9702 0000 000f  comp............
+00009480: 636f 6d70 0000 0000 0000 def3 0000 000f  comp............
 00009490: 0070 006f 0073 0065 005f 0070 0072 006f  .p.o.s.e._.p.r.o
 000094a0: 0063 0065 0073 0073 006f 0072 0073 6c73  .c.e.s.s.o.r.sls
 000094b0: 7643 626c 6f62 0000 0297 6270 6c69 7374  vCblob....bplist
 000094c0: 3030 d801 0203 0405 0607 0809 0a0b 1949  00.............I
 000094d0: 4a0a 4c58 6963 6f6e 5369 7a65 5f10 0f73  J.LXiconSize_..s
 000094e0: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
 000094f0: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
@@ -2458,22 +2458,22 @@
 00009990: 6101 6a01 6b01 6d01 6e01 7001 7901 7a01  a.j.k.m.n.p.y.z.
 000099a0: 7c01 7d01 7f01 8801 8901 8c01 8d01 8f01  |.}.............
 000099b0: 9801 9901 9a01 9c01 9d01 a601 ab00 0000  ................
 000099c0: 0000 0002 0100 0000 0000 0000 4900 0000  ............I...
 000099d0: 0000 0000 0000 0000 0000 0001 ac00 0000  ................
 000099e0: 0f00 7000 6f00 7300 6500 5f00 7000 7200  ..p.o.s.e._.p.r.
 000099f0: 6f00 6300 6500 7300 7300 6f00 7200 736d  o.c.e.s.s.o.r.sm
-00009a00: 6f44 4462 6c6f 6200 0000 08e3 bf98 f1cc  oDDblob.........
-00009a10: 0cc5 4100 0000 0f00 7000 6f00 7300 6500  ..A.....p.o.s.e.
+00009a00: 6f44 4462 6c6f 6200 0000 08e2 486d c51b  oDDblob.....Hm..
+00009a10: 1fc5 4100 0000 0f00 7000 6f00 7300 6500  ..A.....p.o.s.e.
 00009a20: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
 00009a30: 6f00 7200 736d 6f64 4462 6c6f 6200 0000  o.r.smodDblob...
-00009a40: 08e3 bf98 f1cc 0cc5 4100 0000 0f00 7000  ........A.....p.
+00009a40: 08e2 486d c51b 1fc5 4100 0000 0f00 7000  ..Hm....A.....p.
 00009a50: 6f00 7300 6500 5f00 7000 7200 6f00 6300  o.s.e._.p.r.o.c.
 00009a60: 6500 7300 7300 6f00 7200 7370 6831 5363  e.s.s.o.r.sph1Sc
-00009a70: 6f6d 7000 0000 0000 0100 0000 0000 0f00  omp.............
+00009a70: 6f6d 7000 0000 0000 0180 0000 0000 0f00  omp.............
 00009a80: 7000 6f00 7300 6500 5f00 7000 7200 6f00  p.o.s.e._.p.r.o.
 00009a90: 6300 6500 7300 7300 6f00 7200 7376 5372  c.e.s.s.o.r.svSr
 00009aa0: 6e6c 6f6e 6700 0000 0100 0000 0900 7200  nlong.........r.
 00009ab0: 6f00 6900 5f00 7400 6f00 6f00 6c00 7362  o.i._.t.o.o.l.sb
 00009ac0: 7773 7062 6c6f 6200 0000 ca62 706c 6973  wspblob....bplis
 00009ad0: 7430 30d7 0102 0304 0506 0708 080a 080a  t00.............
 00009ae0: 0d0a 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
@@ -2485,15 +2485,15 @@
 00009b40: 6562 6172 0808 0908 095f 1019 7b7b 3233  ebar....._..{{23
 00009b50: 322c 2031 3931 7d2c 207b 3133 3032 2c20  2, 191}, {1302, 
 00009b60: 3731 347d 7d09 0817 2531 3d49 606d 797a  714}}...%1=I`myz
 00009b70: 7b7c 7d7e 9a00 0000 0000 0001 0100 0000  {|}~............
 00009b80: 0000 0000 0f00 0000 0000 0000 0000 0000  ................
 00009b90: 0000 0000 9b00 0000 0900 7200 6f00 6900  ..........r.o.i.
 00009ba0: 5f00 7400 6f00 6f00 6c00 736c 6731 5363  _.t.o.o.l.slg1Sc
-00009bb0: 6f6d 7000 0000 0000 043d 1800 0000 0900  omp......=......
+00009bb0: 6f6d 7000 0000 0000 05ec 0b00 0000 0900  omp.............
 00009bc0: 7200 6f00 6900 5f00 7400 6f00 6f00 6c00  r.o.i._.t.o.o.l.
 00009bd0: 736c 7376 4362 6c6f 6200 0002 7962 706c  slsvCblob...ybpl
 00009be0: 6973 7430 30d8 0102 0304 0506 0708 090a  ist00...........
 00009bf0: 0b16 4647 480a 5f10 1276 6965 774f 7074  ..FGH._..viewOpt
 00009c00: 696f 6e73 5665 7273 696f 6e5f 100f 7368  ionsVersion_..sh
 00009c10: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
 00009c20: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
@@ -2528,15 +2528,15 @@
 00009df0: 0125 012a 0133 0134 0136 0137 013c 0145  .%.*.3.4.6.7.<.E
 00009e00: 0146 0148 0149 014f 0158 0159 015b 015c  .F.H.I.O.X.Y.[.\
 00009e10: 0164 016d 016e 0171 0172 017b 0184 0185  .d.m.n.q.r.{....
 00009e20: 0187 0188 0197 01a0 01a1 01a2 01ac 01ad  ................
 00009e30: 01b6 01bb 01c4 0000 0000 0000 0201 0000  ................
 00009e40: 0000 0000 004a 0000 0000 0000 0000 0000  .....J..........
 00009e50: 0000 0000 01c5 6831 5363 6f6d 7000 0000  ......h1Scomp...
-00009e60: 0000 0150 0000 0000 0d00 6f00 7500 7400  ...P......o.u.t.
+00009e60: 0000 01b0 0000 0000 0d00 6f00 7500 7400  ..........o.u.t.
 00009e70: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
 00009e80: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
 00009e90: 0000 0800 7000 6c00 6f00 7400 7400 6900  ....p.l.o.t.t.i.
 00009ea0: 6e00 6762 7773 7062 6c6f 6200 0000 ca62  n.gbwspblob....b
 00009eb0: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
 00009ec0: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
 00009ed0: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
@@ -2547,271 +2547,271 @@
 00009f20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
 00009f30: 7b7b 3238 372c 2031 3036 7d2c 207b 3130  {{287, 106}, {10
 00009f40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
 00009f50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
 00009f60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 00009f70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
 00009f80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
-00009f90: 5363 6f6d 7000 0000 0000 08c5 3600 0000  Scomp.......6...
+00009f90: 5363 6f6d 7000 0000 0000 0c7f 3d00 0000  Scomp.......=...
 00009fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-0000a000: 0000 0000 0000 0000 0000 0014 0000 0009  ................
+0000a000: 0000 0000 0000 0000 0000 0018 0000 0009  ................
 0000a010: 0072 006f 0069 005f 0074 006f 006f 006c  .r.o.i._.t.o.o.l
 0000a020: 0073 6d6f 4444 626c 6f62 0000 0008 5519  .smoDDblob....U.
 0000a030: 3cb9 d51b c541 0000 0009 0072 006f 0069  <....A.....r.o.i
 0000a040: 005f 0074 006f 006f 006c 0073 6d6f 6444  ._.t.o.o.l.smodD
 0000a050: 626c 6f62 0000 0008 5519 3cb9 d51b c541  blob....U.<....A
 0000a060: 0000 0009 0072 006f 0069 005f 0074 006f  .....r.o.i._.t.o
 0000a070: 006f 006c 0073 7068 3153 636f 6d70 0000  .o.l.sph1Scomp..
-0000a080: 0000 0005 2000 0000 0009 0072 006f 0069  .... ......r.o.i
+0000a080: 0000 0007 5000 0000 0009 0072 006f 0069  ....P......r.o.i
 0000a090: 005f 0074 006f 006f 006c 0073 7653 726e  ._.t.o.o.l.svSrn
-0000a0a0: 6c6f 6e67 0000 0001 0000 001b 0074 0068  long.........t.h
-0000a0b0: 0069 0072 0064 005f 0070 0061 0072 0074  .i.r.d._.p.a.r.t
-0000a0c0: 0079 005f 006c 0061 0062 0065 006c 005f  .y._.l.a.b.e.l._
-0000a0d0: 0061 0070 0070 0065 006e 0064 0065 0072  .a.p.p.e.n.d.e.r
-0000a0e0: 0073 6277 7370 626c 6f62 0000 00ca 6270  .sbwspblob....bp
-0000a0f0: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
-0000a100: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
-0000a110: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
-0000a120: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
-0000a130: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-0000a140: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-0000a150: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-0000a160: 5369 6465 6261 7208 0809 0809 5f10 197b  Sidebar....._..{
-0000a170: 7b33 3535 2c20 3132 357d 2c20 7b31 3037  {355, 125}, {107
-0000a180: 362c 2036 3231 7d7d 0908 1725 313d 4960  6, 621}}...%1=I`
-0000a190: 6d79 7a7b 7c7d 7e9a 0000 0000 0000 0101  myz{|}~.........
-0000a1a0: 0000 0000 0000 000f 0000 0000 0000 0000  ................
-0000a1b0: 0000 0000 0000 009b 0000 001b 0074 0068  .............t.h
-0000a1c0: 0069 0072 0064 005f 0070 0061 0072 0074  .i.r.d._.p.a.r.t
-0000a1d0: 0079 005f 006c 0061 0062 0065 006c 005f  .y._.l.a.b.e.l._
-0000a1e0: 0061 0070 0070 0065 006e 0064 0065 0072  .a.p.p.e.n.d.e.r
-0000a1f0: 0073 6c67 3153 636f 6d70 0000 0000 0002  .slg1Scomp......
-0000a200: 27d2 0000 001b 0074 0068 0069 0072 0064  '......t.h.i.r.d
-0000a210: 005f 0070 0061 0072 0074 0079 005f 006c  ._.p.a.r.t.y._.l
-0000a220: 0061 0062 0065 006c 005f 0061 0070 0070  .a.b.e.l._.a.p.p
-0000a230: 0065 006e 0064 0065 0072 0073 6c73 7643  .e.n.d.e.r.slsvC
-0000a240: 626c 6f62 0000 0279 6270 6c69 7374 3030  blob...ybplist00
-0000a250: d801 0203 0405 0607 0809 0a0b 1646 4748  .............FGH
-0000a260: 0a5f 1012 7669 6577 4f70 7469 6f6e 7356  ._..viewOptionsV
-0000a270: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
-0000a280: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
-0000a290: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
-0000a2a0: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
-0000a2b0: 7274 436f 6c75 6d6e 5869 636f 6e53 697a  rtColumnXiconSiz
-0000a2c0: 655f 1010 7573 6552 656c 6174 6976 6544  e_..useRelativeD
-0000a2d0: 6174 6573 1001 09ab 0c15 1a1f 2328 2d32  ates........#(-2
-0000a2e0: 373c 41d4 0d0e 0f10 0a12 0a14 5776 6973  7<A.........Wvis
-0000a2f0: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
-0000a300: 6469 6e67 5a69 6465 6e74 6966 6965 7209  dingZidentifier.
-0000a310: 1101 a609 546e 616d 65d4 0d0e 0f10 1617  ....Tname.......
-0000a320: 1619 0810 2308 5875 6269 7175 6974 79d4  ....#.Xubiquity.
-0000a330: 0d0e 0f10 0a1c 161e 0910 b508 5c64 6174  ............\dat
-0000a340: 654d 6f64 6966 6965 64d4 0d0e 0f10 161c  eModified.......
-0000a350: 1622 0808 5b64 6174 6543 7265 6174 6564  ."..[dateCreated
-0000a360: d40d 0e0f 100a 2516 2709 1061 0854 7369  ......%.'..a.Tsi
-0000a370: 7a65 d40d 0e0f 100a 2a0a 2c09 1073 0954  ze......*.,..s.T
-0000a380: 6b69 6e64 d40d 0e0f 1016 2f0a 3108 1064  kind....../.1..d
-0000a390: 0955 6c61 6265 6cd4 0d0e 0f10 1634 0a36  .Ulabel......4.6
-0000a3a0: 0810 4b09 5776 6572 7369 6f6e d40d 0e0f  ..K.Wversion....
-0000a3b0: 1016 390a 3b08 1101 2c09 5863 6f6d 6d65  ..9.;...,.Xcomme
-0000a3c0: 6e74 73d4 0d0e 0f10 163e 1640 0810 c808  nts......>.@....
-0000a3d0: 5e64 6174 654c 6173 744f 7065 6e65 64d4  ^dateLastOpened.
-0000a3e0: 0d0e 0f10 161c 1644 0808 5964 6174 6541  .......D..YdateA
-0000a3f0: 6464 6564 0823 4028 0000 0000 0000 546e  dded.#@(......Tn
-0000a400: 616d 6523 4030 0000 0000 0000 0900 0800  ame#@0..........
-0000a410: 1900 2e00 4000 4800 5c00 6500 7000 7900  ....@.H.\.e.p.y.
-0000a420: 8c00 8e00 8f00 9b00 a400 ac00 b200 bc00  ................
-0000a430: c700 c800 cb00 cc00 d100 da00 db00 dd00  ................
-0000a440: de00 e700 f000 f100 f300 f401 0101 0a01  ................
-0000a450: 0b01 0c01 1801 2101 2201 2401 2501 2a01  ......!.".$.%.*.
-0000a460: 3301 3401 3601 3701 3c01 4501 4601 4801  3.4.6.7.<.E.F.H.
-0000a470: 4901 4f01 5801 5901 5b01 5c01 6401 6d01  I.O.X.Y.[.\.d.m.
-0000a480: 6e01 7101 7201 7b01 8401 8501 8701 8801  n.q.r.{.........
-0000a490: 9701 a001 a101 a201 ac01 ad01 b601 bb01  ................
-0000a4a0: c400 0000 0000 0002 0100 0000 0000 0000  ................
-0000a4b0: 4a00 0000 0000 0000 0000 0000 0000 0001  J...............
-0000a4c0: c500 0000 1b00 7400 6800 6900 7200 6400  ......t.h.i.r.d.
-0000a4d0: 5f00 7000 6100 7200 7400 7900 5f00 6c00  _.p.a.r.t.y._.l.
-0000a4e0: 6100 6200 6500 6c00 5f00 6100 7000 7000  a.b.e.l._.a.p.p.
-0000a4f0: 6500 6e00 6400 6500 7200 736c 7376 7062  e.n.d.e.r.slsvpb
-0000a500: 6c6f 6200 0002 5e62 706c 6973 7430 30d8  lob...^bplist00.
-0000a510: 0102 0304 0506 0708 090a 0b1d 4546 470a  ............EFG.
-0000a520: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
-0000a530: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
-0000a540: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
-0000a550: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
-0000a560: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
-0000a570: 7443 6f6c 756d 6e58 6963 6f6e 5369 7a65  tColumnXiconSize
-0000a580: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-0000a590: 7465 7310 0109 d90c 0d0e 0f10 1112 1314  tes.............
-0000a5a0: 151e 2327 2b30 353a 3f58 636f 6d6d 656e  ..#'+05:?Xcommen
-0000a5b0: 7473 5e64 6174 654c 6173 744f 7065 6e65  ts^dateLastOpene
-0000a5c0: 645c 6461 7465 4d6f 6469 6669 6564 5b64  d\dateModified[d
-0000a5d0: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
-0000a5e0: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
-0000a5f0: 6f6e 546e 616d 65d4 1617 1819 1a1b 0a1d  onTname.........
-0000a600: 5569 6e64 6578 5577 6964 7468 5961 7363  UindexUwidthYasc
-0000a610: 656e 6469 6e67 5776 6973 6962 6c65 1007  endingWvisible..
-0000a620: 1101 2c09 08d4 1617 1819 1f20 1d1d 1008  ..,........ ....
-0000a630: 10c8 0808 d416 1718 1909 241d 0a10 b508  ..........$.....
-0000a640: 09d4 1617 1819 2824 1d1d 1002 0808 d416  ......($........
-0000a650: 1718 192c 2d1d 0a10 0310 6108 09d4 1617  ...,-.....a.....
-0000a660: 1819 3132 0a1d 1005 1064 0908 d416 1718  ..12.....d......
-0000a670: 1936 370a 0a10 0410 7309 09d4 1617 1819  .67.....s.......
-0000a680: 3b3c 0a1d 1006 104b 0908 d416 1718 1940  ;<.....K.......@
-0000a690: 410a 0a10 0011 01a6 0909 0823 4028 0000  A..........#@(..
-0000a6a0: 0000 0000 546e 616d 6523 4030 0000 0000  ....Tname#@0....
-0000a6b0: 0000 0900 0800 1900 2e00 4000 4800 5c00  ..........@.H.\.
-0000a6c0: 6500 7000 7900 8c00 8e00 8f00 a200 ab00  e.p.y...........
-0000a6d0: ba00 c700 d300 d800 de00 e300 eb00 f000  ................
-0000a6e0: f900 ff01 0501 0f01 1701 1901 1c01 1d01  ................
-0000a6f0: 1e01 2701 2901 2b01 2c01 2d01 3601 3801  ..'.).+.,.-.6.8.
-0000a700: 3901 3a01 4301 4501 4601 4701 5001 5201  9.:.C.E.F.G.P.R.
-0000a710: 5401 5501 5601 5f01 6101 6301 6401 6501  T.U.V._.a.c.d.e.
-0000a720: 6e01 7001 7201 7301 7401 7d01 7f01 8101  n.p.r.s.t.}.....
-0000a730: 8201 8301 8c01 8e01 9101 9201 9301 9401  ................
-0000a740: 9d01 a201 ab00 0000 0000 0002 0100 0000  ................
-0000a750: 0000 0000 4900 0000 0000 0000 0000 0000  ....I...........
-0000a760: 0000 0001 ac00 0000 1b00 7400 6800 6900  ..........t.h.i.
-0000a770: 7200 6400 5f00 7000 6100 7200 7400 7900  r.d._.p.a.r.t.y.
-0000a780: 5f00 6c00 6100 6200 6500 6c00 5f00 6100  _.l.a.b.e.l._.a.
-0000a790: 7000 7000 6500 6e00 6400 6500 7200 736d  p.p.e.n.d.e.r.sm
-0000a7a0: 6f44 4462 6c6f 6200 0000 08ed 45eb 2346  oDDblob.....E.#F
-0000a7b0: 19c5 4100 0000 1b00 7400 6800 6900 7200  ..A.....t.h.i.r.
-0000a7c0: 6400 5f00 7000 6100 7200 7400 7900 5f00  d._.p.a.r.t.y._.
-0000a7d0: 6c00 6100 6200 6500 6c00 5f00 6100 7000  l.a.b.e.l._.a.p.
-0000a7e0: 7000 6500 6e00 6400 6500 7200 736d 6f64  p.e.n.d.e.r.smod
-0000a7f0: 4462 6c6f 6200 0000 08ed 45eb 2346 19c5  Dblob.....E.#F..
-0000a800: 4100 0000 1b00 7400 6800 6900 7200 6400  A.....t.h.i.r.d.
-0000a810: 5f00 7000 6100 7200 7400 7900 5f00 6c00  _.p.a.r.t.y._.l.
-0000a820: 6100 6200 6500 6c00 5f00 6100 7000 7000  a.b.e.l._.a.p.p.
-0000a830: 6500 6e00 6400 6500 7200 7370 6831 5363  e.n.d.e.r.sph1Sc
-0000a840: 6f6d 7000 0000 0000 02b0 0000 0000 1b00  omp.............
-0000a850: 7400 6800 6900 7200 6400 5f00 7000 6100  t.h.i.r.d._.p.a.
-0000a860: 7200 7400 7900 5f00 6c00 6100 6200 6500  r.t.y._.l.a.b.e.
-0000a870: 6c00 5f00 6100 7000 7000 6500 6e00 6400  l._.a.p.p.e.n.d.
-0000a880: 6500 7200 7376 5372 6e6c 6f6e 6700 0000  e.r.svSrnlong...
-0000a890: 0100 0000 0200 7500 6962 7773 7062 6c6f  ......u.ibwspblo
-0000a8a0: 6200 0000 ca62 706c 6973 7430 30d7 0102  b....bplist00...
-0000a8b0: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
-0000a8c0: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
-0000a8d0: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
-0000a8e0: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
-0000a8f0: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
-0000a900: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
-0000a910: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
-0000a920: 0908 095f 1019 7b7b 3335 342c 2031 3234  ..._..{{354, 124
-0000a930: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
-0000a940: 0817 2531 3d49 606d 797a 7b7c 7d7e 9a00  ..%1=I`myz{|}~..
-0000a950: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
-0000a960: 0000 0000 0000 0000 0000 0000 0000 9b00  ................
-0000a970: 0000 0200 7500 6964 7363 6c62 6f6f 6c00  ....u.idsclbool.
-0000a980: 0000 0002 0075 0069 6c67 3153 636f 6d70  .....u.ilg1Scomp
-0000a990: 0000 0000 0009 7bb2 0000 0002 0075 0069  ......{......u.i
-0000a9a0: 6c73 7643 626c 6f62 0000 0279 6270 6c69  lsvCblob...ybpli
-0000a9b0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
-0000a9c0: 1846 4748 0a5f 1012 7669 6577 4f70 7469  .FGH._..viewOpti
-0000a9d0: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
-0000a9e0: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
-0000a9f0: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
-0000aa00: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
-0000aa10: 655a 736f 7274 436f 6c75 6d6e 5869 636f  eZsortColumnXico
-0000aa20: 6e53 697a 655f 1010 7573 6552 656c 6174  nSize_..useRelat
-0000aa30: 6976 6544 6174 6573 1001 09ab 0c15 1a1f  iveDates........
-0000aa40: 2328 2d32 373c 41d4 0d0e 0f10 0a12 0a14  #(-27<A.........
-0000aa50: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
-0000aa60: 7363 656e 6469 6e67 5a69 6465 6e74 6966  scendingZidentif
-0000aa70: 6965 7209 1101 c709 546e 616d 65d4 100e  ier.....Tname...
-0000aa80: 0f0d 1617 1818 5875 6269 7175 6974 7910  ......Xubiquity.
-0000aa90: 2308 08d4 100f 0e0d 1b18 1d0a 5c64 6174  #...........\dat
-0000aaa0: 654d 6f64 6966 6965 6408 10b5 09d4 100f  eModified.......
-0000aab0: 0e0d 2018 1d18 5b64 6174 6543 7265 6174  .. ...[dateCreat
-0000aac0: 6564 0808 d410 0f0e 0d24 1826 0a54 7369  ed.......$.&.Tsi
-0000aad0: 7a65 0810 6109 d410 0f0e 0d29 0a2b 0a54  ze..a......).+.T
-0000aae0: 6b69 6e64 0910 7309 d410 0f0e 0d2e 0a30  kind..s........0
-0000aaf0: 1855 6c61 6265 6c09 1064 08d4 100f 0e0d  .Ulabel..d......
-0000ab00: 330a 3518 5776 6572 7369 6f6e 0910 4b08  3.5.Wversion..K.
-0000ab10: d410 0f0e 0d38 0a3a 1858 636f 6d6d 656e  .....8.:.Xcommen
-0000ab20: 7473 0911 012c 08d4 100f 0e0d 3d18 3f18  ts...,......=.?.
-0000ab30: 5e64 6174 654c 6173 744f 7065 6e65 6408  ^dateLastOpened.
-0000ab40: 10c8 08d4 100e 0f0d 421d 1818 5964 6174  ........B...Ydat
-0000ab50: 6541 6464 6564 0808 0823 4028 0000 0000  eAdded...#@(....
-0000ab60: 0000 546e 616d 6523 4030 0000 0000 0000  ..Tname#@0......
-0000ab70: 0900 0800 1900 2e00 4000 4800 5c00 6500  ........@.H.\.e.
-0000ab80: 7000 7900 8c00 8e00 8f00 9b00 a400 ac00  p.y.............
-0000ab90: b200 bc00 c700 c800 cb00 cc00 d100 da00  ................
-0000aba0: e300 e500 e600 e700 f000 fd00 fe01 0001  ................
-0000abb0: 0101 0a01 1601 1701 1801 2101 2601 2701  ..........!.&.'.
-0000abc0: 2901 2a01 3301 3801 3901 3b01 3c01 4501  ).*.3.8.9.;.<.E.
-0000abd0: 4b01 4c01 4e01 4f01 5801 6001 6101 6301  K.L.N.O.X.`.a.c.
-0000abe0: 6401 6d01 7601 7701 7a01 7b01 8401 9301  d.m.v.w.z.{.....
-0000abf0: 9401 9601 9701 a001 aa01 ab01 ac01 ad01  ................
-0000ac00: b601 bb01 c400 0000 0000 0002 0100 0000  ................
-0000ac10: 0000 0000 4a00 0000 0000 0000 0000 0000  ....J...........
-0000ac20: 0000 0001 c500 0000 0200 7500 696c 7376  ..........u.ilsv
-0000ac30: 7062 6c6f 6200 0002 5e62 706c 6973 7430  pblob...^bplist0
-0000ac40: 30d8 0102 0304 0506 0708 090a 0b1a 4546  0.............EF
-0000ac50: 470a 5f10 1276 6965 774f 7074 696f 6e73  G._..viewOptions
-0000ac60: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
-0000ac70: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
-0000ac80: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
-0000ac90: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
-0000aca0: 6f72 7443 6f6c 756d 6e58 6963 6f6e 5369  ortColumnXiconSi
-0000acb0: 7a65 5f10 1075 7365 5265 6c61 7469 7665  ze_..useRelative
-0000acc0: 4461 7465 7310 0109 d90c 0d0e 0f10 1112  Dates...........
-0000acd0: 1314 151e 2327 2b30 353a 3f58 636f 6d6d  ....#'+05:?Xcomm
-0000ace0: 656e 7473 5e64 6174 654c 6173 744f 7065  ents^dateLastOpe
-0000acf0: 6e65 645c 6461 7465 4d6f 6469 6669 6564  ned\dateModified
-0000ad00: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
-0000ad10: 6555 6c61 6265 6c54 6b69 6e64 5776 6572  eUlabelTkindWver
-0000ad20: 7369 6f6e 546e 616d 65d4 1617 1819 1a0a  sionTname.......
-0000ad30: 1c1d 5776 6973 6962 6c65 5961 7363 656e  ..WvisibleYascen
-0000ad40: 6469 6e67 5577 6964 7468 5569 6e64 6578  dingUwidthUindex
-0000ad50: 0809 1101 2c10 07d4 1617 1819 1a1a 2122  ....,.........!"
-0000ad60: 0808 10c8 1008 d416 1718 190a 1a26 0909  .............&..
-0000ad70: 0810 b5d4 1617 1819 1a1a 262a 0808 1002  ..........&*....
-0000ad80: d416 1718 190a 1a2e 2f09 0810 6110 03d4  ......../...a...
-0000ad90: 1617 1819 1a0a 3334 0809 1064 1005 d416  ......34...d....
-0000ada0: 1718 190a 0a38 3909 0910 7310 04d4 1617  .....89...s.....
-0000adb0: 1819 1a0a 3d3e 0809 104b 1006 d419 1817  ....=>...K......
-0000adc0: 1640 410a 0a10 0011 01c7 0909 0823 4028  .@A..........#@(
-0000add0: 0000 0000 0000 546e 616d 6523 4030 0000  ......Tname#@0..
-0000ade0: 0000 0000 0900 0800 1900 2e00 4000 4800  ............@.H.
-0000adf0: 5c00 6500 7000 7900 8c00 8e00 8f00 a200  \.e.p.y.........
-0000ae00: ab00 ba00 c700 d300 d800 de00 e300 eb00  ................
-0000ae10: f000 f901 0101 0b01 1101 1701 1801 1901  ................
-0000ae20: 1c01 1e01 2701 2801 2901 2b01 2d01 3601  ....'.(.).+.-.6.
-0000ae30: 3701 3801 3a01 4301 4401 4501 4701 5001  7.8.:.C.D.E.G.P.
-0000ae40: 5101 5201 5401 5601 5f01 6001 6101 6301  Q.R.T.V._.`.a.c.
-0000ae50: 6501 6e01 6f01 7001 7201 7401 7d01 7e01  e.n.o.p.r.t.}.~.
-0000ae60: 7f01 8101 8301 8c01 8e01 9101 9201 9301  ................
-0000ae70: 9401 9d01 a201 ab00 0000 0000 0002 0100  ................
-0000ae80: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
-0000ae90: 0000 0000 0001 ac00 0000 0200 7500 696d  ............u.im
-0000aea0: 6f44 4462 6c6f 6200 0000 0870 649a f46e  oDDblob....pd..n
-0000aeb0: 1cc5 4100 0000 0200 7500 696d 6f64 4462  ..A.....u.imodDb
-0000aec0: 6c6f 6200 0000 0870 649a f46e 1cc5 4100  lob....pd..n..A.
-0000aed0: 0000 0200 7500 6970 6831 5363 6f6d 7000  ....u.iph1Scomp.
-0000aee0: 0000 0000 0c90 006f 6c62 6172 5b53 686f  .......olbar[Sho
-0000aef0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
-0000af00: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
-0000af10: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-0000af20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
-0000af30: 7b7b 3238 372c 2031 3036 7d2c 207b 3130  {{287, 106}, {10
-0000af40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
+0000a0a0: 6c6f 6e67 0000 0001 0000 0002 0073 0074  long.........s.t
+0000a0b0: 6c67 3153 636f 6d70 0000 0000 0000 30b5  lg1Scomp......0.
+0000a0c0: 0000 0002 0073 0074 6d6f 4444 626c 6f62  .....s.tmoDDblob
+0000a0d0: 0000 0008 16c0 6cac 051f c541 0000 0002  ......l....A....
+0000a0e0: 0073 0074 6d6f 6444 626c 6f62 0000 0008  .s.tmodDblob....
+0000a0f0: 16c0 6cac 051f c541 0000 0002 0073 0074  ..l....A.....s.t
+0000a100: 7068 3153 636f 6d70 0000 0000 0000 a000  ph1Scomp........
+0000a110: 0000 001b 0074 0068 0069 0072 0064 005f  .....t.h.i.r.d._
+0000a120: 0070 0061 0072 0074 0079 005f 006c 0061  .p.a.r.t.y._.l.a
+0000a130: 0062 0065 006c 005f 0061 0070 0070 0065  .b.e.l._.a.p.p.e
+0000a140: 006e 0064 0065 0072 0073 6277 7370 626c  .n.d.e.r.sbwspbl
+0000a150: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
+0000a160: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
+0000a170: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+0000a180: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
+0000a190: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
+0000a1a0: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
+0000a1b0: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
+0000a1c0: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
+0000a1d0: 0809 0809 5f10 197b 7b33 3535 2c20 3132  ...._..{{355, 12
+0000a1e0: 357d 2c20 7b31 3037 362c 2036 3231 7d7d  5}, {1076, 621}}
+0000a1f0: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e9a  ...%1=I`myz{|}~.
+0000a200: 0000 0000 0000 0101 0000 0000 0000 000f  ................
+0000a210: 0000 0000 0000 0000 0000 0000 0000 009b  ................
+0000a220: 0000 001b 0074 0068 0069 0072 0064 005f  .....t.h.i.r.d._
+0000a230: 0070 0061 0072 0074 0079 005f 006c 0061  .p.a.r.t.y._.l.a
+0000a240: 0062 0065 006c 005f 0061 0070 0070 0065  .b.e.l._.a.p.p.e
+0000a250: 006e 0064 0065 0072 0073 6c67 3153 636f  .n.d.e.r.slg1Sco
+0000a260: 6d70 0000 0000 0003 2437 0000 001b 0074  mp......$7.....t
+0000a270: 0068 0069 0072 0064 005f 0070 0061 0072  .h.i.r.d._.p.a.r
+0000a280: 0074 0079 005f 006c 0061 0062 0065 006c  .t.y._.l.a.b.e.l
+0000a290: 005f 0061 0070 0070 0065 006e 0064 0065  ._.a.p.p.e.n.d.e
+0000a2a0: 0072 0073 6c73 7643 626c 6f62 0000 0279  .r.slsvCblob...y
+0000a2b0: 6270 6c69 7374 3030 d801 0203 0405 0607  bplist00........
+0000a2c0: 0809 0a0b 1646 4748 0a5f 1012 7669 6577  .....FGH._..view
+0000a2d0: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
+0000a2e0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+0000a2f0: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+0000a300: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
+0000a310: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
+0000a320: 5869 636f 6e53 697a 655f 1010 7573 6552  XiconSize_..useR
+0000a330: 656c 6174 6976 6544 6174 6573 1001 09ab  elativeDates....
+0000a340: 0c15 1a1f 2328 2d32 373c 41d4 0d0e 0f10  ....#(-27<A.....
+0000a350: 0a12 0a14 5776 6973 6962 6c65 5577 6964  ....WvisibleUwid
+0000a360: 7468 5961 7363 656e 6469 6e67 5a69 6465  thYascendingZide
+0000a370: 6e74 6966 6965 7209 1101 a609 546e 616d  ntifier.....Tnam
+0000a380: 65d4 0d0e 0f10 1617 1619 0810 2308 5875  e...........#.Xu
+0000a390: 6269 7175 6974 79d4 0d0e 0f10 0a1c 161e  biquity.........
+0000a3a0: 0910 b508 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
+0000a3b0: 64d4 0d0e 0f10 161c 1622 0808 5b64 6174  d........"..[dat
+0000a3c0: 6543 7265 6174 6564 d40d 0e0f 100a 2516  eCreated......%.
+0000a3d0: 2709 1061 0854 7369 7a65 d40d 0e0f 100a  '..a.Tsize......
+0000a3e0: 2a0a 2c09 1073 0954 6b69 6e64 d40d 0e0f  *.,..s.Tkind....
+0000a3f0: 1016 2f0a 3108 1064 0955 6c61 6265 6cd4  ../.1..d.Ulabel.
+0000a400: 0d0e 0f10 1634 0a36 0810 4b09 5776 6572  .....4.6..K.Wver
+0000a410: 7369 6f6e d40d 0e0f 1016 390a 3b08 1101  sion......9.;...
+0000a420: 2c09 5863 6f6d 6d65 6e74 73d4 0d0e 0f10  ,.Xcomments.....
+0000a430: 163e 1640 0810 c808 5e64 6174 654c 6173  .>.@....^dateLas
+0000a440: 744f 7065 6e65 64d4 0d0e 0f10 161c 1644  tOpened........D
+0000a450: 0808 5964 6174 6541 6464 6564 0823 4028  ..YdateAdded.#@(
+0000a460: 0000 0000 0000 546e 616d 6523 4030 0000  ......Tname#@0..
+0000a470: 0000 0000 0900 0800 1900 2e00 4000 4800  ............@.H.
+0000a480: 5c00 6500 7000 7900 8c00 8e00 8f00 9b00  \.e.p.y.........
+0000a490: a400 ac00 b200 bc00 c700 c800 cb00 cc00  ................
+0000a4a0: d100 da00 db00 dd00 de00 e700 f000 f100  ................
+0000a4b0: f300 f401 0101 0a01 0b01 0c01 1801 2101  ..............!.
+0000a4c0: 2201 2401 2501 2a01 3301 3401 3601 3701  ".$.%.*.3.4.6.7.
+0000a4d0: 3c01 4501 4601 4801 4901 4f01 5801 5901  <.E.F.H.I.O.X.Y.
+0000a4e0: 5b01 5c01 6401 6d01 6e01 7101 7201 7b01  [.\.d.m.n.q.r.{.
+0000a4f0: 8401 8501 8701 8801 9701 a001 a101 a201  ................
+0000a500: ac01 ad01 b601 bb01 c400 0000 0000 0002  ................
+0000a510: 0100 0000 0000 0000 4a00 0000 0000 0000  ........J.......
+0000a520: 0000 0000 0000 0001 c500 0000 1b00 7400  ..............t.
+0000a530: 6800 6900 7200 6400 5f00 7000 6100 7200  h.i.r.d._.p.a.r.
+0000a540: 7400 7900 5f00 6c00 6100 6200 6500 6c00  t.y._.l.a.b.e.l.
+0000a550: 5f00 6100 7000 7000 6500 6e00 6400 6500  _.a.p.p.e.n.d.e.
+0000a560: 7200 736c 7376 7062 6c6f 6200 0002 5e62  r.slsvpblob...^b
+0000a570: 706c 6973 7430 30d8 0102 0304 0506 0708  plist00.........
+0000a580: 090a 0b1d 4546 470a 5f10 1276 6965 774f  ....EFG._..viewO
+0000a590: 7074 696f 6e73 5665 7273 696f 6e5f 100f  ptionsVersion_..
+0000a5a0: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
+0000a5b0: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
+0000a5c0: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
+0000a5d0: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e58  SizeZsortColumnX
+0000a5e0: 6963 6f6e 5369 7a65 5f10 1075 7365 5265  iconSize_..useRe
+0000a5f0: 6c61 7469 7665 4461 7465 7310 0109 d90c  lativeDates.....
+0000a600: 0d0e 0f10 1112 1314 151e 2327 2b30 353a  ..........#'+05:
+0000a610: 3f58 636f 6d6d 656e 7473 5e64 6174 654c  ?Xcomments^dateL
+0000a620: 6173 744f 7065 6e65 645c 6461 7465 4d6f  astOpened\dateMo
+0000a630: 6469 6669 6564 5b64 6174 6543 7265 6174  dified[dateCreat
+0000a640: 6564 5473 697a 6555 6c61 6265 6c54 6b69  edTsizeUlabelTki
+0000a650: 6e64 5776 6572 7369 6f6e 546e 616d 65d4  ndWversionTname.
+0000a660: 1617 1819 1a1b 0a1d 5569 6e64 6578 5577  ........UindexUw
+0000a670: 6964 7468 5961 7363 656e 6469 6e67 5776  idthYascendingWv
+0000a680: 6973 6962 6c65 1007 1101 2c09 08d4 1617  isible....,.....
+0000a690: 1819 1f20 1d1d 1008 10c8 0808 d416 1718  ... ............
+0000a6a0: 1909 241d 0a10 b508 09d4 1617 1819 2824  ..$...........($
+0000a6b0: 1d1d 1002 0808 d416 1718 192c 2d1d 0a10  ...........,-...
+0000a6c0: 0310 6108 09d4 1617 1819 3132 0a1d 1005  ..a.......12....
+0000a6d0: 1064 0908 d416 1718 1936 370a 0a10 0410  .d.......67.....
+0000a6e0: 7309 09d4 1617 1819 3b3c 0a1d 1006 104b  s.......;<.....K
+0000a6f0: 0908 d416 1718 1940 410a 0a10 0011 01a6  .......@A.......
+0000a700: 0909 0823 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
+0000a710: 6523 4030 0000 0000 0000 0900 0800 1900  e#@0............
+0000a720: 2e00 4000 4800 5c00 6500 7000 7900 8c00  ..@.H.\.e.p.y...
+0000a730: 8e00 8f00 a200 ab00 ba00 c700 d300 d800  ................
+0000a740: de00 e300 eb00 f000 f900 ff01 0501 0f01  ................
+0000a750: 1701 1901 1c01 1d01 1e01 2701 2901 2b01  ..........'.).+.
+0000a760: 2c01 2d01 3601 3801 3901 3a01 4301 4501  ,.-.6.8.9.:.C.E.
+0000a770: 4601 4701 5001 5201 5401 5501 5601 5f01  F.G.P.R.T.U.V._.
+0000a780: 6101 6301 6401 6501 6e01 7001 7201 7301  a.c.d.e.n.p.r.s.
+0000a790: 7401 7d01 7f01 8101 8201 8301 8c01 8e01  t.}.............
+0000a7a0: 9101 9201 9301 9401 9d01 a201 ab00 0000  ................
+0000a7b0: 0000 0002 0100 0000 0000 0000 4900 0000  ............I...
+0000a7c0: 0000 0000 0000 0000 0000 0001 ac00 0000  ................
+0000a7d0: 1b00 7400 6800 6900 7200 6400 5f00 7000  ..t.h.i.r.d._.p.
+0000a7e0: 6100 7200 7400 7900 5f00 6c00 6100 6200  a.r.t.y._.l.a.b.
+0000a7f0: 6500 6c00 5f00 6100 7000 7000 6500 6e00  e.l._.a.p.p.e.n.
+0000a800: 6400 6500 7200 736d 6f44 4462 6c6f 6200  d.e.r.smoDDblob.
+0000a810: 0000 08ed 45eb 2346 19c5 4100 0000 1b00  ....E.#F..A.....
+0000a820: 7400 6800 6900 7200 6400 5f00 7000 6100  t.h.i.r.d._.p.a.
+0000a830: 7200 7400 7900 5f00 6c00 6100 6200 6500  r.t.y._.l.a.b.e.
+0000a840: 6c00 5f00 6100 7000 7000 6500 6e00 6400  l._.a.p.p.e.n.d.
+0000a850: 6500 7200 736d 6f64 4462 6c6f 6200 0000  e.r.smodDblob...
+0000a860: 08ed 45eb 2346 19c5 4100 0000 1b00 7400  ..E.#F..A.....t.
+0000a870: 6800 6900 7200 6400 5f00 7000 6100 7200  h.i.r.d._.p.a.r.
+0000a880: 7400 7900 5f00 6c00 6100 6200 6500 6c00  t.y._.l.a.b.e.l.
+0000a890: 5f00 6100 7000 7000 6500 6e00 6400 6500  _.a.p.p.e.n.d.e.
+0000a8a0: 7200 7370 6831 5363 6f6d 7000 0000 0000  r.sph1Scomp.....
+0000a8b0: 0400 0000 0000 1b00 7400 6800 6900 7200  ........t.h.i.r.
+0000a8c0: 6400 5f00 7000 6100 7200 7400 7900 5f00  d._.p.a.r.t.y._.
+0000a8d0: 6c00 6100 6200 6500 6c00 5f00 6100 7000  l.a.b.e.l._.a.p.
+0000a8e0: 7000 6500 6e00 6400 6500 7200 7376 5372  p.e.n.d.e.r.svSr
+0000a8f0: 6e6c 6f6e 6700 0000 0100 0000 0200 7500  nlong.........u.
+0000a900: 6962 7773 7062 6c6f 6200 0000 ca62 706c  ibwspblob....bpl
+0000a910: 6973 7430 30d7 0102 0304 0506 0708 080a  ist00...........
+0000a920: 080a 0d0a 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
+0000a930: 6172 5b53 686f 7750 6174 6862 6172 5b53  ar[ShowPathbar[S
+0000a940: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
+0000a950: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
+0000a960: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
+0000a970: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
+0000a980: 6964 6562 6172 0808 0908 095f 1019 7b7b  idebar....._..{{
+0000a990: 3335 342c 2031 3234 7d2c 207b 3130 3736  354, 124}, {1076
+0000a9a0: 2c20 3632 317d 7d09 0817 2531 3d49 606d  , 621}}...%1=I`m
+0000a9b0: 797a 7b7c 7d7e 9a00 0000 0000 0001 0100  yz{|}~..........
+0000a9c0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
+0000a9d0: 0000 0000 0000 9b00 0000 0200 7500 6964  ............u.id
+0000a9e0: 7363 6c62 6f6f 6c00 0000 0002 0075 0069  sclbool......u.i
+0000a9f0: 6c67 3153 636f 6d70 0000 0000 000d 9176  lg1Scomp.......v
+0000aa00: 0000 0002 0075 0069 6c73 7643 626c 6f62  .....u.ilsvCblob
+0000aa10: 0000 0279 6270 6c69 7374 3030 d801 0203  ...ybplist00....
+0000aa20: 0405 0607 0809 0a0b 1846 4748 0a5f 1012  .........FGH._..
+0000aa30: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
+0000aa40: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
+0000aa50: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+0000aa60: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+0000aa70: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
+0000aa80: 6c75 6d6e 5869 636f 6e53 697a 655f 1010  lumnXiconSize_..
+0000aa90: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+0000aaa0: 1001 09ab 0c15 1a1f 2328 2d32 373c 41d4  ........#(-27<A.
+0000aab0: 0d0e 0f10 0a12 0a14 5776 6973 6962 6c65  ........Wvisible
+0000aac0: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
+0000aad0: 5a69 6465 6e74 6966 6965 7209 1101 c709  Zidentifier.....
+0000aae0: 546e 616d 65d4 100e 0f0d 1617 1818 5875  Tname.........Xu
+0000aaf0: 6269 7175 6974 7910 2308 08d4 100f 0e0d  biquity.#.......
+0000ab00: 1b18 1d0a 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
+0000ab10: 6408 10b5 09d4 100f 0e0d 2018 1d18 5b64  d......... ...[d
+0000ab20: 6174 6543 7265 6174 6564 0808 d410 0f0e  ateCreated......
+0000ab30: 0d24 1826 0a54 7369 7a65 0810 6109 d410  .$.&.Tsize..a...
+0000ab40: 0f0e 0d29 0a2b 0a54 6b69 6e64 0910 7309  ...).+.Tkind..s.
+0000ab50: d410 0f0e 0d2e 0a30 1855 6c61 6265 6c09  .......0.Ulabel.
+0000ab60: 1064 08d4 100f 0e0d 330a 3518 5776 6572  .d......3.5.Wver
+0000ab70: 7369 6f6e 0910 4b08 d410 0f0e 0d38 0a3a  sion..K......8.:
+0000ab80: 1858 636f 6d6d 656e 7473 0911 012c 08d4  .Xcomments...,..
+0000ab90: 100f 0e0d 3d18 3f18 5e64 6174 654c 6173  ....=.?.^dateLas
+0000aba0: 744f 7065 6e65 6408 10c8 08d4 100e 0f0d  tOpened.........
+0000abb0: 421d 1818 5964 6174 6541 6464 6564 0808  B...YdateAdded..
+0000abc0: 0823 4028 0000 0000 0000 546e 616d 6523  .#@(......Tname#
+0000abd0: 4030 0000 0000 0000 0900 0800 1900 2e00  @0..............
+0000abe0: 4000 4800 5c00 6500 7000 7900 8c00 8e00  @.H.\.e.p.y.....
+0000abf0: 8f00 9b00 a400 ac00 b200 bc00 c700 c800  ................
+0000ac00: cb00 cc00 d100 da00 e300 e500 e600 e700  ................
+0000ac10: f000 fd00 fe01 0001 0101 0a01 1601 1701  ................
+0000ac20: 1801 2101 2601 2701 2901 2a01 3301 3801  ..!.&.'.).*.3.8.
+0000ac30: 3901 3b01 3c01 4501 4b01 4c01 4e01 4f01  9.;.<.E.K.L.N.O.
+0000ac40: 5801 6001 6101 6301 6401 6d01 7601 7701  X.`.a.c.d.m.v.w.
+0000ac50: 7a01 7b01 8401 9301 9401 9601 9701 a001  z.{.............
+0000ac60: aa01 ab01 ac01 ad01 b601 bb01 c400 0000  ................
+0000ac70: 0000 0002 0100 0000 0000 0000 4a00 0000  ............J...
+0000ac80: 0000 0000 0000 0000 0000 0001 c500 0000  ................
+0000ac90: 0200 7500 696c 7376 7062 6c6f 6200 0002  ..u.ilsvpblob...
+0000aca0: 5e62 706c 6973 7430 30d8 0102 0304 0506  ^bplist00.......
+0000acb0: 0708 090a 0b1a 4546 470a 5f10 1276 6965  ......EFG._..vie
+0000acc0: 774f 7074 696f 6e73 5665 7273 696f 6e5f  wOptionsVersion_
+0000acd0: 100f 7368 6f77 4963 6f6e 5072 6576 6965  ..showIconPrevie
+0000ace0: 7757 636f 6c75 6d6e 735f 1011 6361 6c63  wWcolumns_..calc
+0000acf0: 756c 6174 6541 6c6c 5369 7a65 7358 7465  ulateAllSizesXte
+0000ad00: 7874 5369 7a65 5a73 6f72 7443 6f6c 756d  xtSizeZsortColum
+0000ad10: 6e58 6963 6f6e 5369 7a65 5f10 1075 7365  nXiconSize_..use
+0000ad20: 5265 6c61 7469 7665 4461 7465 7310 0109  RelativeDates...
+0000ad30: d90c 0d0e 0f10 1112 1314 151e 2327 2b30  ............#'+0
+0000ad40: 353a 3f58 636f 6d6d 656e 7473 5e64 6174  5:?Xcomments^dat
+0000ad50: 654c 6173 744f 7065 6e65 645c 6461 7465  eLastOpened\date
+0000ad60: 4d6f 6469 6669 6564 5b64 6174 6543 7265  Modified[dateCre
+0000ad70: 6174 6564 5473 697a 6555 6c61 6265 6c54  atedTsizeUlabelT
+0000ad80: 6b69 6e64 5776 6572 7369 6f6e 546e 616d  kindWversionTnam
+0000ad90: 65d4 1617 1819 1a0a 1c1d 5776 6973 6962  e.........Wvisib
+0000ada0: 6c65 5961 7363 656e 6469 6e67 5577 6964  leYascendingUwid
+0000adb0: 7468 5569 6e64 6578 0809 1101 2c10 07d4  thUindex....,...
+0000adc0: 1617 1819 1a1a 2122 0808 10c8 1008 d416  ......!"........
+0000add0: 1718 190a 1a26 0909 0810 b5d4 1617 1819  .....&..........
+0000ade0: 1a1a 262a 0808 1002 d416 1718 190a 1a2e  ..&*............
+0000adf0: 2f09 0810 6110 03d4 1617 1819 1a0a 3334  /...a.........34
+0000ae00: 0809 1064 1005 d416 1718 190a 0a38 3909  ...d.........89.
+0000ae10: 0910 7310 04d4 1617 1819 1a0a 3d3e 0809  ..s.........=>..
+0000ae20: 104b 1006 d419 1817 1640 410a 0a10 0011  .K.......@A.....
+0000ae30: 01c7 0909 0823 4028 0000 0000 0000 546e  .....#@(......Tn
+0000ae40: 616d 6523 4030 0000 0000 0000 0900 0800  ame#@0..........
+0000ae50: 1900 2e00 4000 4800 5c00 6500 7000 7900  ....@.H.\.e.p.y.
+0000ae60: 8c00 8e00 8f00 a200 ab00 ba00 c700 d300  ................
+0000ae70: d800 de00 e300 eb00 f000 f901 0101 0b01  ................
+0000ae80: 1101 1701 1801 1901 1c01 1e01 2701 2801  ............'.(.
+0000ae90: 2901 2b01 2d01 3601 3701 3801 3a01 4301  ).+.-.6.7.8.:.C.
+0000aea0: 4401 4501 4701 5001 5101 5201 5401 5601  D.E.G.P.Q.R.T.V.
+0000aeb0: 5f01 6001 6101 6301 6501 6e01 6f01 7001  _.`.a.c.e.n.o.p.
+0000aec0: 7201 7401 7d01 7e01 7f01 8101 8301 8c01  r.t.}.~.........
+0000aed0: 8e01 9101 9201 9301 9401 9d01 a201 ab00  ................
+0000aee0: 0000 0000 0002 0100 0000 0000 0000 4900  ..............I.
+0000aef0: 0000 0000 0000 0000 0000 0000 0001 ac00  ................
+0000af00: 0000 0200 7500 696d 6f44 4462 6c6f 6200  ....u.imoDDblob.
+0000af10: 0000 0870 649a f46e 1cc5 4100 0000 0200  ...pd..n..A.....
+0000af20: 7500 696d 6f64 4462 6c6f 6200 0000 0870  u.imodDblob....p
+0000af30: 649a f46e 1cc5 4100 0000 0200 7500 6970  d..n..A.....u.ip
+0000af40: 6831 5363 6f6d 7000 0000 0000 1220 0049  h1Scomp...... .I
 0000af50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
 0000af60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 0000af70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
 0000af80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
-0000af90: 5363 6f6d 7000 0000 0000 08c5 3600 0000  Scomp.......6...
+0000af90: 5363 6f6d 7000 0000 0000 0c7f 3d00 0000  Scomp.......=...
 0000afa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000aff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000b000: 0000 0000 0000 0000 0000 000a 0000 000c  ................
@@ -2939,135 +2939,135 @@
 0000b7a0: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
 0000b7b0: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
 0000b7c0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
 0000b7d0: 0809 5f10 187b 7b32 302c 2032 3336 7d2c  .._..{{20, 236},
 0000b7e0: 207b 3130 3736 2c20 3632 317d 7d09 0817   {1076, 621}}...
 0000b7f0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
 0000b800: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-0000b810: 0000 0000 0000 0000 0000 0000 9a00 6c00  ..............l.
-0000b820: 6100 6200 6500 6c00 5f00 6100 7000 7000  a.b.e.l._.a.p.p.
-0000b830: 6500 6e00 6400 6500 7200 7370 6831 5363  e.n.d.e.r.sph1Sc
-0000b840: 6f6d 7000 0000 0000 02b0 0000 0000 1b00  omp.............
-0000b850: 7400 6800 6900 7200 6400 5f00 7000 6100  t.h.i.r.d._.p.a.
-0000b860: 7200 7400 7900 5f00 6c00 6100 6200 6500  r.t.y._.l.a.b.e.
-0000b870: 6c00 5f00 6100 7000 7000 6500 6e00 6400  l._.a.p.p.e.n.d.
-0000b880: 6500 7200 7376 5372 6e6c 6f6e 6700 0000  e.r.svSrnlong...
-0000b890: 0100 0000 0200 7500 6962 7773 7062 6c6f  ......u.ibwspblo
-0000b8a0: 6200 0000 ca62 706c 6973 7430 30d7 0102  b....bplist00...
-0000b8b0: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
-0000b8c0: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
-0000b8d0: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
-0000b8e0: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
-0000b8f0: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
-0000b900: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
-0000b910: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
-0000b920: 0908 095f 1019 7b7b 3335 342c 2031 3234  ..._..{{354, 124
-0000b930: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
-0000b940: 0817 2531 3d49 606d 797a 7b7c 7d7e 9a00  ..%1=I`myz{|}~..
-0000b950: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
-0000b960: 0000 0000 0000 0000 0000 0000 0000 9b00  ................
-0000b970: 0000 0200 7500 6964 7363 6c62 6f6f 6c00  ....u.idsclbool.
-0000b980: 0000 0002 0075 0069 6c67 3153 636f 6d70  .....u.ilg1Scomp
-0000b990: 0000 0000 0009 7bb2 0000 0002 0075 0069  ......{......u.i
-0000b9a0: 6c73 7643 626c 6f62 0000 0279 6270 6c69  lsvCblob...ybpli
-0000b9b0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
-0000b9c0: 1846 4748 0a5f 1012 7669 6577 4f70 7469  .FGH._..viewOpti
-0000b9d0: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
-0000b9e0: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
-0000b9f0: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
-0000ba00: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
-0000ba10: 655a 736f 7274 436f 6c75 6d6e 5869 636f  eZsortColumnXico
-0000ba20: 6e53 697a 655f 1010 7573 6552 656c 6174  nSize_..useRelat
-0000ba30: 6976 6544 6174 6573 1001 09ab 0c15 1a1f  iveDates........
-0000ba40: 2328 2d32 373c 41d4 0d0e 0f10 0a12 0a14  #(-27<A.........
-0000ba50: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
-0000ba60: 7363 656e 6469 6e67 5a69 6465 6e74 6966  scendingZidentif
-0000ba70: 6965 7209 1101 c709 546e 616d 65d4 100e  ier.....Tname...
-0000ba80: 0f0d 1617 1818 5875 6269 7175 6974 7910  ......Xubiquity.
-0000ba90: 2308 08d4 100f 0e0d 1b18 1d0a 5c64 6174  #...........\dat
-0000baa0: 654d 6f64 6966 6965 6408 10b5 09d4 100f  eModified.......
-0000bab0: 0e0d 2018 1d18 5b64 6174 6543 7265 6174  .. ...[dateCreat
-0000bac0: 6564 0808 d410 0f0e 0d24 1826 0a54 7369  ed.......$.&.Tsi
-0000bad0: 7a65 0810 6109 d410 0f0e 0d29 0a2b 0a54  ze..a......).+.T
-0000bae0: 6b69 6e64 0910 7309 d410 0f0e 0d2e 0a30  kind..s........0
-0000baf0: 1855 6c61 6265 6c09 1064 08d4 100f 0e0d  .Ulabel..d......
-0000bb00: 330a 3518 5776 6572 7369 6f6e 0910 4b08  3.5.Wversion..K.
-0000bb10: d410 0f0e 0d38 0a3a 1858 636f 6d6d 656e  .....8.:.Xcommen
-0000bb20: 7473 0911 012c 08d4 100f 0e0d 3d18 3f18  ts...,......=.?.
-0000bb30: 5e64 6174 654c 6173 744f 7065 6e65 6408  ^dateLastOpened.
-0000bb40: 10c8 08d4 100e 0f0d 421d 1818 5964 6174  ........B...Ydat
-0000bb50: 6541 6464 6564 0808 0823 4028 0000 0000  eAdded...#@(....
-0000bb60: 0000 546e 616d 6523 4030 0000 0000 0000  ..Tname#@0......
-0000bb70: 0900 0800 1900 2e00 4000 4800 5c00 6500  ........@.H.\.e.
-0000bb80: 7000 7900 8c00 8e00 8f00 9b00 a400 ac00  p.y.............
-0000bb90: b200 bc00 c700 c800 cb00 cc00 d100 da00  ................
-0000bba0: e300 e500 e600 e700 f000 fd00 fe01 0001  ................
-0000bbb0: 0101 0a01 1601 1701 1801 2101 2601 2701  ..........!.&.'.
-0000bbc0: 2901 2a01 3301 3801 3901 3b01 3c01 4501  ).*.3.8.9.;.<.E.
-0000bbd0: 4b01 4c01 4e01 4f01 5801 6001 6101 6301  K.L.N.O.X.`.a.c.
-0000bbe0: 6401 6d01 7601 7701 7a01 7b01 8401 9301  d.m.v.w.z.{.....
-0000bbf0: 9401 9601 9701 a001 aa01 ab01 ac01 ad01  ................
-0000bc00: b601 bb01 c400 0000 0000 0002 0100 0000  ................
-0000bc10: 0000 0000 4a00 0000 0000 0000 0000 0000  ....J...........
-0000bc20: 0000 0001 c500 0000 0200 7500 696c 7376  ..........u.ilsv
-0000bc30: 7062 6c6f 6200 0002 5e62 706c 6973 7430  pblob...^bplist0
-0000bc40: 30d8 0102 0304 0506 0708 090a 0b1a 4546  0.............EF
-0000bc50: 470a 5f10 1276 6965 774f 7074 696f 6e73  G._..viewOptions
-0000bc60: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
-0000bc70: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
-0000bc80: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
-0000bc90: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
-0000bca0: 6f72 7443 6f6c 756d 6e58 6963 6f6e 5369  ortColumnXiconSi
-0000bcb0: 7a65 5f10 1075 7365 5265 6c61 7469 7665  ze_..useRelative
-0000bcc0: 4461 7465 7310 0109 d90c 0d0e 0f10 1112  Dates...........
-0000bcd0: 1314 151e 2327 2b30 353a 3f58 636f 6d6d  ....#'+05:?Xcomm
-0000bce0: 656e 7473 5e64 6174 654c 6173 744f 7065  ents^dateLastOpe
-0000bcf0: 6e65 645c 6461 7465 4d6f 6469 6669 6564  ned\dateModified
-0000bd00: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
-0000bd10: 6555 6c61 6265 6c54 6b69 6e64 5776 6572  eUlabelTkindWver
-0000bd20: 7369 6f6e 546e 616d 65d4 1617 1819 1a0a  sionTname.......
-0000bd30: 1c1d 5776 6973 6962 6c65 5961 7363 656e  ..WvisibleYascen
-0000bd40: 6469 6e67 5577 6964 7468 5569 6e64 6578  dingUwidthUindex
-0000bd50: 0809 1101 2c10 07d4 1617 1819 1a1a 2122  ....,.........!"
-0000bd60: 0808 10c8 1008 d416 1718 190a 1a26 0909  .............&..
-0000bd70: 0810 b5d4 1617 1819 1a1a 262a 0808 1002  ..........&*....
-0000bd80: d416 1718 190a 1a2e 2f09 0810 6110 03d4  ......../...a...
-0000bd90: 1617 1819 1a0a 3334 0809 1064 1005 d416  ......34...d....
-0000bda0: 1718 190a 0a38 3909 0910 7310 04d4 1617  .....89...s.....
-0000bdb0: 1819 1a0a 3d3e 0809 104b 1006 d419 1817  ....=>...K......
-0000bdc0: 1640 410a 0a10 0011 01c7 0909 0823 4028  .@A..........#@(
-0000bdd0: 0000 0000 0000 546e 616d 6523 4030 0000  ......Tname#@0..
-0000bde0: 0000 0000 0900 0800 1900 2e00 4000 4800  ............@.H.
-0000bdf0: 5c00 6500 7000 7900 8c00 8e00 8f00 a200  \.e.p.y.........
-0000be00: ab00 ba00 c700 d300 d800 de00 e300 eb00  ................
-0000be10: f000 f901 0101 0b01 1101 1701 1801 1901  ................
-0000be20: 1c01 1e01 2701 2801 2901 2b01 2d01 3601  ....'.(.).+.-.6.
-0000be30: 3701 3801 3a01 4301 4401 4501 4701 5001  7.8.:.C.D.E.G.P.
-0000be40: 5101 5201 5401 5601 5f01 6001 6101 6301  Q.R.T.V._.`.a.c.
-0000be50: 6501 6e01 6f01 7001 7201 7401 7d01 7e01  e.n.o.p.r.t.}.~.
-0000be60: 7f01 8101 8301 8c01 8e01 9101 9201 9301  ................
-0000be70: 9401 9d01 a201 ab00 0000 0000 0002 0100  ................
-0000be80: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
-0000be90: 0000 0000 0001 ac00 0000 0200 7500 696d  ............u.im
-0000bea0: 6f44 4462 6c6f 6200 0000 0870 649a f46e  oDDblob....pd..n
-0000beb0: 1cc5 4100 0000 0200 7500 696d 6f64 4462  ..A.....u.imodDb
-0000bec0: 6c6f 6200 0000 0870 649a f46e 1cc5 4100  lob....pd..n..A.
-0000bed0: 0000 0200 7500 6970 6831 5363 6f6d 7000  ....u.iph1Scomp.
-0000bee0: 0000 0000 0c90 006f 6c62 6172 5b53 686f  .......olbar[Sho
-0000bef0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
-0000bf00: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
-0000bf10: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-0000bf20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
-0000bf30: 7b7b 3238 372c 2031 3036 7d2c 207b 3130  {{287, 106}, {10
-0000bf40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
+0000b810: 0000 0000 0000 0000 0000 0000 9a00 1b00  ................
+0000b820: 7400 6800 6900 7200 6400 5f00 7000 6100  t.h.i.r.d._.p.a.
+0000b830: 7200 7400 7900 5f00 6c00 6100 6200 6500  r.t.y._.l.a.b.e.
+0000b840: 6c00 5f00 6100 7000 7000 6500 6e00 6400  l._.a.p.p.e.n.d.
+0000b850: 6500 7200 736d 6f64 4462 6c6f 6200 0000  e.r.smodDblob...
+0000b860: 08ed 45eb 2346 19c5 4100 0000 1b00 7400  ..E.#F..A.....t.
+0000b870: 6800 6900 7200 6400 5f00 7000 6100 7200  h.i.r.d._.p.a.r.
+0000b880: 7400 7900 5f00 6c00 6100 6200 6500 6c00  t.y._.l.a.b.e.l.
+0000b890: 5f00 6100 7000 7000 6500 6e00 6400 6500  _.a.p.p.e.n.d.e.
+0000b8a0: 7200 7370 6831 5363 6f6d 7000 0000 0000  r.sph1Scomp.....
+0000b8b0: 0400 0000 0000 1b00 7400 6800 6900 7200  ........t.h.i.r.
+0000b8c0: 6400 5f00 7000 6100 7200 7400 7900 5f00  d._.p.a.r.t.y._.
+0000b8d0: 6c00 6100 6200 6500 6c00 5f00 6100 7000  l.a.b.e.l._.a.p.
+0000b8e0: 7000 6500 6e00 6400 6500 7200 7376 5372  p.e.n.d.e.r.svSr
+0000b8f0: 6e6c 6f6e 6700 0000 0100 0000 0200 7500  nlong.........u.
+0000b900: 6962 7773 7062 6c6f 6200 0000 ca62 706c  ibwspblob....bpl
+0000b910: 6973 7430 30d7 0102 0304 0506 0708 080a  ist00...........
+0000b920: 080a 0d0a 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
+0000b930: 6172 5b53 686f 7750 6174 6862 6172 5b53  ar[ShowPathbar[S
+0000b940: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
+0000b950: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
+0000b960: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
+0000b970: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
+0000b980: 6964 6562 6172 0808 0908 095f 1019 7b7b  idebar....._..{{
+0000b990: 3335 342c 2031 3234 7d2c 207b 3130 3736  354, 124}, {1076
+0000b9a0: 2c20 3632 317d 7d09 0817 2531 3d49 606d  , 621}}...%1=I`m
+0000b9b0: 797a 7b7c 7d7e 9a00 0000 0000 0001 0100  yz{|}~..........
+0000b9c0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
+0000b9d0: 0000 0000 0000 9b00 0000 0200 7500 6964  ............u.id
+0000b9e0: 7363 6c62 6f6f 6c00 0000 0002 0075 0069  sclbool......u.i
+0000b9f0: 6c67 3153 636f 6d70 0000 0000 000d 9176  lg1Scomp.......v
+0000ba00: 0000 0002 0075 0069 6c73 7643 626c 6f62  .....u.ilsvCblob
+0000ba10: 0000 0279 6270 6c69 7374 3030 d801 0203  ...ybplist00....
+0000ba20: 0405 0607 0809 0a0b 1846 4748 0a5f 1012  .........FGH._..
+0000ba30: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
+0000ba40: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
+0000ba50: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+0000ba60: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+0000ba70: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
+0000ba80: 6c75 6d6e 5869 636f 6e53 697a 655f 1010  lumnXiconSize_..
+0000ba90: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+0000baa0: 1001 09ab 0c15 1a1f 2328 2d32 373c 41d4  ........#(-27<A.
+0000bab0: 0d0e 0f10 0a12 0a14 5776 6973 6962 6c65  ........Wvisible
+0000bac0: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
+0000bad0: 5a69 6465 6e74 6966 6965 7209 1101 c709  Zidentifier.....
+0000bae0: 546e 616d 65d4 100e 0f0d 1617 1818 5875  Tname.........Xu
+0000baf0: 6269 7175 6974 7910 2308 08d4 100f 0e0d  biquity.#.......
+0000bb00: 1b18 1d0a 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
+0000bb10: 6408 10b5 09d4 100f 0e0d 2018 1d18 5b64  d......... ...[d
+0000bb20: 6174 6543 7265 6174 6564 0808 d410 0f0e  ateCreated......
+0000bb30: 0d24 1826 0a54 7369 7a65 0810 6109 d410  .$.&.Tsize..a...
+0000bb40: 0f0e 0d29 0a2b 0a54 6b69 6e64 0910 7309  ...).+.Tkind..s.
+0000bb50: d410 0f0e 0d2e 0a30 1855 6c61 6265 6c09  .......0.Ulabel.
+0000bb60: 1064 08d4 100f 0e0d 330a 3518 5776 6572  .d......3.5.Wver
+0000bb70: 7369 6f6e 0910 4b08 d410 0f0e 0d38 0a3a  sion..K......8.:
+0000bb80: 1858 636f 6d6d 656e 7473 0911 012c 08d4  .Xcomments...,..
+0000bb90: 100f 0e0d 3d18 3f18 5e64 6174 654c 6173  ....=.?.^dateLas
+0000bba0: 744f 7065 6e65 6408 10c8 08d4 100e 0f0d  tOpened.........
+0000bbb0: 421d 1818 5964 6174 6541 6464 6564 0808  B...YdateAdded..
+0000bbc0: 0823 4028 0000 0000 0000 546e 616d 6523  .#@(......Tname#
+0000bbd0: 4030 0000 0000 0000 0900 0800 1900 2e00  @0..............
+0000bbe0: 4000 4800 5c00 6500 7000 7900 8c00 8e00  @.H.\.e.p.y.....
+0000bbf0: 8f00 9b00 a400 ac00 b200 bc00 c700 c800  ................
+0000bc00: cb00 cc00 d100 da00 e300 e500 e600 e700  ................
+0000bc10: f000 fd00 fe01 0001 0101 0a01 1601 1701  ................
+0000bc20: 1801 2101 2601 2701 2901 2a01 3301 3801  ..!.&.'.).*.3.8.
+0000bc30: 3901 3b01 3c01 4501 4b01 4c01 4e01 4f01  9.;.<.E.K.L.N.O.
+0000bc40: 5801 6001 6101 6301 6401 6d01 7601 7701  X.`.a.c.d.m.v.w.
+0000bc50: 7a01 7b01 8401 9301 9401 9601 9701 a001  z.{.............
+0000bc60: aa01 ab01 ac01 ad01 b601 bb01 c400 0000  ................
+0000bc70: 0000 0002 0100 0000 0000 0000 4a00 0000  ............J...
+0000bc80: 0000 0000 0000 0000 0000 0001 c500 0000  ................
+0000bc90: 0200 7500 696c 7376 7062 6c6f 6200 0002  ..u.ilsvpblob...
+0000bca0: 5e62 706c 6973 7430 30d8 0102 0304 0506  ^bplist00.......
+0000bcb0: 0708 090a 0b1a 4546 470a 5f10 1276 6965  ......EFG._..vie
+0000bcc0: 774f 7074 696f 6e73 5665 7273 696f 6e5f  wOptionsVersion_
+0000bcd0: 100f 7368 6f77 4963 6f6e 5072 6576 6965  ..showIconPrevie
+0000bce0: 7757 636f 6c75 6d6e 735f 1011 6361 6c63  wWcolumns_..calc
+0000bcf0: 756c 6174 6541 6c6c 5369 7a65 7358 7465  ulateAllSizesXte
+0000bd00: 7874 5369 7a65 5a73 6f72 7443 6f6c 756d  xtSizeZsortColum
+0000bd10: 6e58 6963 6f6e 5369 7a65 5f10 1075 7365  nXiconSize_..use
+0000bd20: 5265 6c61 7469 7665 4461 7465 7310 0109  RelativeDates...
+0000bd30: d90c 0d0e 0f10 1112 1314 151e 2327 2b30  ............#'+0
+0000bd40: 353a 3f58 636f 6d6d 656e 7473 5e64 6174  5:?Xcomments^dat
+0000bd50: 654c 6173 744f 7065 6e65 645c 6461 7465  eLastOpened\date
+0000bd60: 4d6f 6469 6669 6564 5b64 6174 6543 7265  Modified[dateCre
+0000bd70: 6174 6564 5473 697a 6555 6c61 6265 6c54  atedTsizeUlabelT
+0000bd80: 6b69 6e64 5776 6572 7369 6f6e 546e 616d  kindWversionTnam
+0000bd90: 65d4 1617 1819 1a0a 1c1d 5776 6973 6962  e.........Wvisib
+0000bda0: 6c65 5961 7363 656e 6469 6e67 5577 6964  leYascendingUwid
+0000bdb0: 7468 5569 6e64 6578 0809 1101 2c10 07d4  thUindex....,...
+0000bdc0: 1617 1819 1a1a 2122 0808 10c8 1008 d416  ......!"........
+0000bdd0: 1718 190a 1a26 0909 0810 b5d4 1617 1819  .....&..........
+0000bde0: 1a1a 262a 0808 1002 d416 1718 190a 1a2e  ..&*............
+0000bdf0: 2f09 0810 6110 03d4 1617 1819 1a0a 3334  /...a.........34
+0000be00: 0809 1064 1005 d416 1718 190a 0a38 3909  ...d.........89.
+0000be10: 0910 7310 04d4 1617 1819 1a0a 3d3e 0809  ..s.........=>..
+0000be20: 104b 1006 d419 1817 1640 410a 0a10 0011  .K.......@A.....
+0000be30: 01c7 0909 0823 4028 0000 0000 0000 546e  .....#@(......Tn
+0000be40: 616d 6523 4030 0000 0000 0000 0900 0800  ame#@0..........
+0000be50: 1900 2e00 4000 4800 5c00 6500 7000 7900  ....@.H.\.e.p.y.
+0000be60: 8c00 8e00 8f00 a200 ab00 ba00 c700 d300  ................
+0000be70: d800 de00 e300 eb00 f000 f901 0101 0b01  ................
+0000be80: 1101 1701 1801 1901 1c01 1e01 2701 2801  ............'.(.
+0000be90: 2901 2b01 2d01 3601 3701 3801 3a01 4301  ).+.-.6.7.8.:.C.
+0000bea0: 4401 4501 4701 5001 5101 5201 5401 5601  D.E.G.P.Q.R.T.V.
+0000beb0: 5f01 6001 6101 6301 6501 6e01 6f01 7001  _.`.a.c.e.n.o.p.
+0000bec0: 7201 7401 7d01 7e01 7f01 8101 8301 8c01  r.t.}.~.........
+0000bed0: 8e01 9101 9201 9301 9401 9d01 a201 ab00  ................
+0000bee0: 0000 0000 0002 0100 0000 0000 0000 4900  ..............I.
+0000bef0: 0000 0000 0000 0000 0000 0000 0001 ac00  ................
+0000bf00: 0000 0200 7500 696d 6f44 4462 6c6f 6200  ....u.imoDDblob.
+0000bf10: 0000 0870 649a f46e 1cc5 4100 0000 0200  ...pd..n..A.....
+0000bf20: 7500 696d 6f64 4462 6c6f 6200 0000 0870  u.imodDblob....p
+0000bf30: 649a f46e 1cc5 4100 0000 0200 7500 6970  d..n..A.....u.ip
+0000bf40: 6831 5363 6f6d 7000 0000 0000 1220 0049  h1Scomp...... .I
 0000bf50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
 0000bf60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 0000bf70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
 0000bf80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
-0000bf90: 5363 6f6d 7000 0000 0000 08c5 3600 0000  Scomp.......6...
+0000bf90: 5363 6f6d 7000 0000 0000 0c7f 3d00 0000  Scomp.......=...
 0000bfa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000c000: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/shap_log_mp_2.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/shap_log_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/shap_log_mp.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/shap_log_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/read_files_mp_2.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/read_files_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -276,23 +276,23 @@
 00001130: 5f10 197b 7b34 3732 2c20 3134 327d 2c20  _..{{472, 142}, 
 00001140: 7b31 3037 362c 2036 3231 7d7d 0908 1725  {1076, 621}}...%
 00001150: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
 00001160: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 00001170: 0000 0000 0000 0000 0000 009b 0000 000b  ................
 00001180: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001190: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-000011a0: 0000 0002 0498 0000 000b 005f 005f 0070  ..........._._.p
+000011a0: 0000 0002 404d 0000 000b 005f 005f 0070  ....@M....._._.p
 000011b0: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-000011c0: 6d6f 4444 626c 6f62 0000 0008 336e 1026  moDDblob....3n.&
-000011d0: 3f0d c541 0000 000b 005f 005f 0070 0079  ?..A....._._.p.y
+000011c0: 6d6f 4444 626c 6f62 0000 0008 d51e e6c2  moDDblob........
+000011d0: 1b1f c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 000011e0: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-000011f0: 6444 626c 6f62 0000 0008 336e 1026 3f0d  dDblob....3n.&?.
+000011f0: 6444 626c 6f62 0000 0008 d51e e6c2 1b1f  dDblob..........
 00001200: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 00001210: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-00001220: 636f 6d70 0000 0000 0002 5000 0000 000b  comp......P.....
+00001220: 636f 6d70 0000 0000 0002 a000 0000 000b  comp............
 00001230: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001240: 0065 005f 005f 7653 726e 6c6f 6e67 0000  .e._._vSrnlong..
 00001250: 0001 0000 0004 006d 0069 0073 0063 6277  .......m.i.s.cbw
 00001260: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
 00001270: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 00001280: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 00001290: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
```

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.63.2/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/requirements.txt` & `Simba-UW-tf-dev-1.63.2/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.63.2/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.63.2/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.63.2/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi` & `Simba-UW-tf-dev-1.63.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi` & `Simba-UW-tf-dev-1.63.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi` & `Simba-UW-tf-dev-1.63.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc` & `Simba-UW-tf-dev-1.63.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc` & `Simba-UW-tf-dev-1.63.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc` & `Simba-UW-tf-dev-1.63.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc` & `Simba-UW-tf-dev-1.63.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.63.2/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.63.2/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.63.2/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.63.2/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.63.2/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.63.2/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.63.2/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.63.2/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.63.2/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.63.2/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.63.2/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.63.2/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/model/.DS_Store`

 * *Files 12% similar despite different names*

```diff
@@ -44,23 +44,23 @@
 000002b0: 5f10 187b 7b33 3335 2c20 3139 387d 2c20  _..{{335, 198}, 
 000002c0: 7b39 3237 2c20 3536 387d 7d09 0817 2531  {927, 568}}...%1
 000002d0: 3d49 606d 797a 7b7c 7d7e 9900 0000 0000  =I`myz{|}~......
 000002e0: 0001 0100 0000 0000 0000 0f00 0000 0000  ................
 000002f0: 0000 0000 0000 0000 0000 9a00 0000 0b00  ................
 00000300: 5f00 5f00 7000 7900 6300 6100 6300 6800  _._.p.y.c.a.c.h.
 00000310: 6500 5f00 5f6c 6731 5363 6f6d 7000 0000  e._._lg1Scomp...
-00000320: 0000 00bf 3300 0000 0b00 5f00 5f00 7000  ....3....._._.p.
+00000320: 0000 00d2 7c00 0000 0b00 5f00 5f00 7000  ....|....._._.p.
 00000330: 7900 6300 6100 6300 6800 6500 5f00 5f6d  y.c.a.c.h.e._._m
-00000340: 6f44 4462 6c6f 6200 0000 08de bf03 80cc  oDDblob.........
-00000350: 0cc5 4100 0000 0b00 5f00 5f00 7000 7900  ..A....._._.p.y.
+00000340: 6f44 4462 6c6f 6200 0000 0897 88b1 bf1b  oDDblob.........
+00000350: 1fc5 4100 0000 0b00 5f00 5f00 7000 7900  ..A....._._.p.y.
 00000360: 6300 6100 6300 6800 6500 5f00 5f6d 6f64  c.a.c.h.e._._mod
-00000370: 4462 6c6f 6200 0000 08de bf03 80cc 0cc5  Dblob...........
+00000370: 4462 6c6f 6200 0000 0897 88b1 bf1b 1fc5  Dblob...........
 00000380: 4100 0000 0b00 5f00 5f00 7000 7900 6300  A....._._.p.y.c.
 00000390: 6100 6300 6800 6500 5f00 5f70 6831 5363  a.c.h.e._._ph1Sc
-000003a0: 6f6d 7000 0000 0000 0110 0000 0000 0b00  omp.............
+000003a0: 6f6d 7000 0000 0000 0100 0000 0000 0b00  omp.............
 000003b0: 5f00 5f00 7000 7900 6300 6100 6300 6800  _._.p.y.c.a.c.h.
 000003c0: 6500 5f00 5f76 5372 6e6c 6f6e 6700 0000  e._._vSrnlong...
 000003d0: 0100 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.1/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.63.2/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.63.2/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.63.2/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.63.2/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.63.2/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.63.2/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.63.2/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/utils/enums.py` & `Simba-UW-tf-dev-1.63.2/simba/utils/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 __author__ = "Simon Nilsson"
 
 from enum import Enum
 import pkg_resources
 from pathlib import Path
+import sys
 import cv2
 import numpy as np
 
 class ConfigKey(Enum):
     GENERAL_SETTINGS = 'General settings'
     PROJECT_PATH = 'project_path'
     SML_SETTINGS = 'SML settings'
@@ -312,14 +313,15 @@
     PARTIAL_DEPENDENCY = 'partial_dependency'
     TRAIN_TEST_SPLIT_TYPE = 'train_test_split_type'
 
 class OS(Enum):
     WINDOWS = 'Windows'
     LINUX = 'Linux'
     MAC = 'Darwin'
+    PYTHON_VER = float(f'{sys.version_info.major}.{sys.version_info.minor}')
 
 class Links(Enum):
     FEATURE_SUBSETS = 'https://github.com/sgoldenlab/simba/blob/master/docs/feature_subsets.md'
     HEATMAP_LOCATION = 'https://github.com/sgoldenlab/simba/blob/master/docs/ROI_tutorial.md#heatmaps'
     HEATMAP_CLF = 'https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#visualizing-classification-heatmaps'
     DATA_TABLES = 'https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#visualizing-data-tables'
     CONCAT_VIDEOS = 'https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#merging-concatenating-videos'
```

### Comparing `Simba-UW-tf-dev-1.63.1/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/utils/.DS_Store`

 * *Files 6% similar despite different names*

```diff
@@ -253,23 +253,23 @@
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 000e 0000 000b  ................
 00001010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00001030: 0000 0002 0922 0000 000b 005f 005f 0070  ....."....._._.p
+00001030: 0000 0004 15bd 0000 000b 005f 005f 0070  ..........._._.p
 00001040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00001050: 6d6f 4444 626c 6f62 0000 0008 f869 742d  moDDblob.....it-
-00001060: 561c c541 0000 000b 005f 005f 0070 0079  V..A....._._.p.y
+00001050: 6d6f 4444 626c 6f62 0000 0008 0480 4f38  moDDblob......O8
+00001060: 1d1f c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 00001070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00001080: 6444 626c 6f62 0000 0008 f869 742d 561c  dDblob.....it-V.
+00001080: 6444 626c 6f62 0000 0008 0480 4f38 1d1f  dDblob......O8..
 00001090: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000010a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000010b0: 636f 6d70 0000 0000 0002 6000 0000 0003  comp......`.....
+000010b0: 636f 6d70 0000 0000 0004 e000 0000 0003  comp............
 000010c0: 0063 006c 0069 6277 7370 626c 6f62 0000  .c.l.ibwspblob..
 000010d0: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
 000010e0: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
 000010f0: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
 00001100: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
 00001110: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
 00001120: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
```

### Comparing `Simba-UW-tf-dev-1.63.1/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.63.2/simba/utils/warnings.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,7 +119,11 @@
     stdout_warning(msg=f'SIMBA INPUT AND OUTPUT WARNING: {msg}')
 
 def ROIWarning(msg: str):
     stdout_warning(msg=f'SIMBA ROI WARNING: {msg}')
 
 def MultiProcessingFailedWarning(msg: str):
     stdout_warning(msg=f'SIMBA MULTI-PROCESSING WARNING: {msg}')
+
+def PythonVersionWarning(msg: str):
+    stdout_warning(msg=f'SIMBA PYTHON VERSION WARNING: {msg}')
+
```

### Comparing `Simba-UW-tf-dev-1.63.1/simba/utils/checks.py` & `Simba-UW-tf-dev-1.63.2/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.63.2/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.63.2/simba/utils/lookups.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __author__ = "Simon Nilsson"
 
-import os, glob
+import os, glob, sys
 import pandas as pd
 import re
 import struct
 import simba
 from typing import List
 from simba.utils.enums import Paths, Methods
 from simba.utils.checks import check_file_exist_and_readable, check_if_dir_exists
@@ -127,20 +127,30 @@
             'BENTO': 'annot'}
 
 
 def get_emojis() -> dict:
     """
     Helper to get dictionary of emojis with names as keys and emojis as values.
     """
-    return {'thank_you': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001f64f'.encode('utf-16be'))),
-            'relaxed': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001F600'.encode('utf-16be'))),
-            'error': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001F6A8'.encode('utf-16be'))),
-            'complete': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001F680'.encode('utf-16be'))),
-            'warning': ''.join(chr(x) for x in struct.unpack('>2H', '\u2757\uFE0F'.encode('utf-16be'))),
-            'trash': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001F5D1'.encode('utf-16be')))}
+    python_version = float(f'{sys.version_info.major}.{sys.version_info.minor}')
+    if python_version <= 3.6:
+        return {'thank_you': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001f64f'.encode('utf-16be'))),
+                'relaxed': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001F600'.encode('utf-16be'))),
+                'error': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001F6A8'.encode('utf-16be'))),
+                'complete': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001F680'.encode('utf-16be'))),
+                'warning': ''.join(chr(x) for x in struct.unpack('>2H', '\u2757\uFE0F'.encode('utf-16be'))),
+                'trash': ''.join(chr(x) for x in struct.unpack('>2H', '\U0001F5D1'.encode('utf-16be')))}
+
+    if python_version > 3.6:
+        return {'thank_you': '\U0001f64f'.encode('utf16', errors='surrogatepass').decode('utf16'),
+                'relaxed': '\U0001F600'.encode('utf16', errors='surrogatepass').decode('utf16'),
+                'error': '\U0001F6A8'.encode('utf16', errors='surrogatepass').decode('utf16'),
+                'complete': '\U0001F680'.encode('utf16', errors='surrogatepass').decode('utf16'),
+                'warning': '\u2757\uFE0F'.encode('utf16', errors='surrogatepass').decode('utf16'),
+                'trash': 'U0001F5D1F'.encode('utf16', errors='surrogatepass').decode('utf16')}
 
 
 def get_meta_data_file_headers() -> List[str]:
     """
     Get List of headers for SimBA classifier metadata output.
 
     :return List[str]:
```

### Comparing `Simba-UW-tf-dev-1.63.1/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.63.2/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/utils/errors.py` & `Simba-UW-tf-dev-1.63.2/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/utils/data.py` & `Simba-UW-tf-dev-1.63.2/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/utils/printing.py` & `Simba-UW-tf-dev-1.63.2/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.63.2/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.63.2/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.63.2/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.63.2/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/mixins/.DS_Store`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
-00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
+00000010: 0000 1000 0000 0108 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0008  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0004  ................
 00000050: 0000 0001 0000 1000 0063 0061 0063 0068  .........c.a.c.h
 00000060: 0065 005f 0000 0000 0000 0000 0000 0000  .e._............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
+00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
+00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
+00000130: 0000 0008 db95 0000 000b 005f 005f 0070  ..........._._.p
+00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
+00000150: 6d6f 4444 626c 6f62 0000 0008 e768 c2c2  moDDblob.....h..
+00000160: 1b1f c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
+00000180: 6444 626c 6f62 0000 0008 e768 c2c2 1b1f  dDblob.....h....
+00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
+000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
+000001b0: 636f 6d70 0000 0000 0009 b000 0000 0000  comp............
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0008 0000 000b  ................
-00000210: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
-00000220: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000230: 0000 0003 67d9 0000 000b 005f 005f 0070  ....g......_._.p
-00000240: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000250: 6d6f 4444 626c 6f62 0000 0008 ff1e 2714  moDDblob......'.
-00000260: 8716 c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
-00000270: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000280: 6444 626c 6f62 0000 0008 ff1e 2714 8716  dDblob......'...
-00000290: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
-000002a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000002b0: 636f 6d70 0000 0000 0004 7000 0000 0005  comp......p.....
-000002c0: 0074 006f 006f 006c 0073 6c67 3153 636f  .t.o.o.l.slg1Sco
-000002d0: 6d70 0000 0000 0000 293c 0000 0005 0074  mp......)<.....t
-000002e0: 006f 006f 006c 0073 6d6f 4444 626c 6f62  .o.o.l.smoDDblob
-000002f0: 0000 0008 1e86 d77f cc0c c541 0000 0005  ...........A....
-00000300: 0074 006f 006f 006c 0073 6d6f 6444 626c  .t.o.o.l.smodDbl
-00000310: 6f62 0000 0008 1e86 d77f cc0c c541 0000  ob...........A..
-00000320: 0005 0074 006f 006f 006c 0073 7068 3153  ...t.o.o.l.sph1S
-00000330: 636f 6d70 0000 0000 0000 4000 0000 0000  comp......@.....
+00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -251,15 +251,15 @@
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0003 0000 0000 0000 100b  ................
-00001010: 0000 0045 0000 0209 0000 0000 0000 0000  ...E............
+00001010: 0000 0045 0000 0108 0000 0000 0000 0000  ...E............
 00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -318,15 +318,15 @@
 000013d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 00001410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-00001440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
+00001440: 0100 0000 8000 0000 0000 0000 0100 0002  ................
 00001450: 0000 0000 0100 0004 0000 0000 0200 0008  ................
 00001460: 0000 0018 0000 0000 0000 0000 0100 0020  ............... 
 00001470: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
 00001480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 000014a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 000014b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
```

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/pose_plotter_mp.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/pose_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.63.2/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.63.2/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.63.2/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.63.2/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.63.2/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.63.2/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.63.2/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.63.2/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.63.2/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.63.2/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.63.2/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.63.2/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.63.2/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.63.2/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.63.2/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.63.2/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.63.2/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.63.2/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.63.2/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/model/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/cue_light_tools/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -44,23 +44,23 @@
 000002b0: 5f10 187b 7b33 3335 2c20 3139 387d 2c20  _..{{335, 198}, 
 000002c0: 7b39 3237 2c20 3536 387d 7d09 0817 2531  {927, 568}}...%1
 000002d0: 3d49 606d 797a 7b7c 7d7e 9900 0000 0000  =I`myz{|}~......
 000002e0: 0001 0100 0000 0000 0000 0f00 0000 0000  ................
 000002f0: 0000 0000 0000 0000 0000 9a00 0000 0b00  ................
 00000300: 5f00 5f00 7000 7900 6300 6100 6300 6800  _._.p.y.c.a.c.h.
 00000310: 6500 5f00 5f6c 6731 5363 6f6d 7000 0000  e._._lg1Scomp...
-00000320: 0000 0069 3600 0000 0b00 5f00 5f00 7000  ...i6....._._.p.
+00000320: 0000 017d af00 0000 0b00 5f00 5f00 7000  ...}......_._.p.
 00000330: 7900 6300 6100 6300 6800 6500 5f00 5f6d  y.c.a.c.h.e._._m
-00000340: 6f44 4462 6c6f 6200 0000 08cd db45 bb40  oDDblob......E.@
-00000350: 17c5 4100 0000 0b00 5f00 5f00 7000 7900  ..A....._._.p.y.
+00000340: 6f44 4462 6c6f 6200 0000 08f7 cfab be1b  oDDblob.........
+00000350: 1fc5 4100 0000 0b00 5f00 5f00 7000 7900  ..A....._._.p.y.
 00000360: 6300 6100 6300 6800 6500 5f00 5f6d 6f64  c.a.c.h.e._._mod
-00000370: 4462 6c6f 6200 0000 08cd db45 bb40 17c5  Dblob......E.@..
+00000370: 4462 6c6f 6200 0000 08f7 cfab be1b 1fc5  Dblob...........
 00000380: 4100 0000 0b00 5f00 5f00 7000 7900 6300  A....._._.p.y.c.
 00000390: 6100 6300 6800 6500 5f00 5f70 6831 5363  a.c.h.e._._ph1Sc
-000003a0: 6f6d 7000 0000 0000 0080 0000 0000 0b00  omp.............
+000003a0: 6f6d 7000 0000 0000 0220 0000 0000 0b00  omp...... ......
 000003b0: 5f00 5f00 7000 7900 6300 6100 6300 6800  _._.p.y.c.a.c.h.
 000003c0: 6500 5f00 5f76 5372 6e6c 6f6e 6700 0000  e._._vSrnlong...
 000003d0: 0100 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.1/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.63.2/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.63.2/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.63.2/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.63.2/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.63.2/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.63.2/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.63.2/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/plotting/.DS_Store`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0009  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0008  ................
 00000050: 0000 0001 0000 1000 0063 0061 0063 0068  .........c.a.c.h
 00000060: 0065 005f 0000 0000 0000 0000 0000 0000  .e._............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -26,35 +26,35 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0009 0000 000b  ................
+00000200: 0000 0000 0000 0000 0000 0008 0000 000b  ................
 00000210: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000220: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000230: 0000 0001 7b5b 0000 000b 005f 005f 0070  ....{[....._._.p
+00000230: 0000 0006 ec07 0000 000b 005f 005f 0070  ..........._._.p
 00000240: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000250: 6d6f 4444 626c 6f62 0000 0008 efc0 0270  moDDblob.......p
-00000260: 4305 c541 0000 000b 005f 005f 0070 0079  C..A....._._.p.y
+00000250: 6d6f 4444 626c 6f62 0000 0008 d3cb d3c2  moDDblob........
+00000260: 1b1f c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 00000270: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000280: 6444 626c 6f62 0000 0008 efc0 0270 4305  dDblob.......pC.
+00000280: 6444 626c 6f62 0000 0008 d3cb d3c2 1b1f  dDblob..........
 00000290: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000002a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000002b0: 636f 6d70 0000 0000 0001 e000 0000 0004  comp............
-000002c0: 006d 0069 0073 0063 6473 636c 626f 6f6c  .m.i.s.cdsclbool
-000002d0: 0000 0000 0400 6d00 6900 7300 636c 6731  ......m.i.s.clg1
-000002e0: 5363 6f6d 7000 0000 0000 0037 0b00 0000  Scomp......7....
-000002f0: 0400 6d00 6900 7300 636d 6f44 4462 6c6f  ..m.i.s.cmoDDblo
-00000300: 6200 0000 082f 5e95 c45e 05c5 4100 0000  b..../^..^..A...
-00000310: 0400 6d00 6900 7300 636d 6f64 4462 6c6f  ..m.i.s.cmodDblo
-00000320: 6200 0000 082f 5e95 c45e 05c5 4100 0000  b..../^..^..A...
-00000330: 0400 6d00 6900 7300 6370 6831 5363 6f6d  ..m.i.s.cph1Scom
-00000340: 7000 0000 0000 0040 0000 0000 0000 0000  p......@........
+000002b0: 636f 6d70 0000 0000 0009 0000 0000 0005  comp............
+000002c0: 0074 006f 006f 006c 0073 6c67 3153 636f  .t.o.o.l.slg1Sco
+000002d0: 6d70 0000 0000 0000 3d66 0000 0005 0074  mp......=f.....t
+000002e0: 006f 006f 006c 0073 6d6f 4444 626c 6f62  .o.o.l.smoDDblob
+000002f0: 0000 0008 1e86 d77f cc0c c541 0000 0005  ...........A....
+00000300: 0074 006f 006f 006c 0073 6d6f 6444 626c  .t.o.o.l.smodDbl
+00000310: 6f62 0000 0008 1e86 d77f cc0c c541 0000  ob...........A..
+00000320: 0005 0074 006f 006f 006c 0073 7068 3153  ...t.o.o.l.sph1S
+00000330: 636f 6d70 0000 0000 0000 6000 0000 0000  comp......`.....
+00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.63.2/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.63.2/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.63.2/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.63.2/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.63.2/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.63.2/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.63.2/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.63.2/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/video_processors/.DS_Store`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 1800 0000 0800  ....Bud1........
 00000010: 0000 1800 0000 100b 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0004  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0008  ................
 00000050: 0000 0001 0000 1000 0063 0061 0063 0068  .........c.a.c.h
 00000060: 0065 005f 0000 0000 0000 0000 0000 0000  .e._............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -250,15 +250,15 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0000 0000 0004 0000 000b  ................
+00001000: 0000 0000 0000 0000 0000 0008 0000 000b  ................
 00001010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001020: 0065 005f 005f 6277 7370 626c 6f62 0000  .e._._bwspblob..
 00001030: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
 00001040: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
 00001050: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
 00001060: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
 00001070: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
@@ -267,118 +267,118 @@
 000010a0: 5368 6f77 5369 6465 6261 7208 0809 0809  ShowSidebar.....
 000010b0: 5f10 197b 7b31 3036 322c 2033 3733 7d2c  _..{{1062, 373},
 000010c0: 207b 3737 302c 2034 3336 7d7d 0908 1725   {770, 436}}...%
 000010d0: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
 000010e0: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 000010f0: 0000 0000 0000 0000 0000 009b 0000 000b  ................
 00001100: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
-00001110: 0065 005f 005f 6c73 7643 626c 6f62 0000  .e._._lsvCblob..
-00001120: 02d4 6270 6c69 7374 3030 da01 0203 0405  ..bplist00......
-00001130: 0607 0809 0a0b 0c0d 1d4a 4b4c 4d0c 4f5f  .........JKLM.O_
-00001140: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
-00001150: 7369 6f6e 5f10 0f73 686f 7749 636f 6e50  sion_..showIconP
-00001160: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
-00001170: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
-00001180: 6573 5f10 0f73 6372 6f6c 6c50 6f73 6974  es_..scrollPosit
-00001190: 696f 6e59 5874 6578 7453 697a 655f 100f  ionYXtextSize_..
-000011a0: 7363 726f 6c6c 506f 7369 7469 6f6e 585a  scrollPositionXZ
-000011b0: 736f 7274 436f 6c75 6d6e 5f10 1075 7365  sortColumn_..use
-000011c0: 5265 6c61 7469 7665 4461 7465 7358 6963  RelativeDatesXic
-000011d0: 6f6e 5369 7a65 1001 09ab 0e17 1f24 282d  onSize.......$(-
-000011e0: 3237 3c40 45d4 0f10 1112 130c 150c 5a69  27<@E.........Zi
-000011f0: 6465 6e74 6966 6965 7259 6173 6365 6e64  dentifierYascend
-00001200: 696e 6755 7769 6474 6857 7669 7369 626c  ingUwidthWvisibl
-00001210: 6554 6e61 6d65 0911 012c 09d4 0f18 191a  eTname...,......
-00001220: 1b1c 1d1d 5577 6964 7468 5961 7363 656e  ....UwidthYascen
-00001230: 6469 6e67 5776 6973 6962 6c65 5875 6269  dingWvisibleXubi
-00001240: 7175 6974 7910 2308 08d4 0f10 1112 201d  quity.#....... .
-00001250: 220c 5c64 6174 654d 6f64 6966 6965 6408  ".\dateModified.
-00001260: 10b5 09d4 0f10 1112 251d 221d 5b64 6174  ........%.".[dat
-00001270: 6543 7265 6174 6564 0808 d40f 1011 1229  eCreated.......)
-00001280: 1d2b 0c54 7369 7a65 0810 6109 d40f 1011  .+.Tsize..a.....
-00001290: 122e 0c30 0c54 6b69 6e64 0910 7309 d40f  ...0.Tkind..s...
-000012a0: 1011 1233 0c35 1d55 6c61 6265 6c09 1064  ...3.5.Ulabel..d
-000012b0: 08d4 0f10 1112 380c 3a1d 5776 6572 7369  ......8.:.Wversi
-000012c0: 6f6e 0910 4b08 d40f 1011 123d 0c15 1d58  on..K......=...X
-000012d0: 636f 6d6d 656e 7473 0908 d40f 1011 1241  comments.......A
-000012e0: 1d43 1d5e 6461 7465 4c61 7374 4f70 656e  .C.^dateLastOpen
-000012f0: 6564 0810 c808 d40f 1819 1a46 221d 1d59  ed.........F"..Y
-00001300: 6461 7465 4164 6465 6408 0808 2300 0000  dateAdded...#...
-00001310: 0000 0000 0023 4028 0000 0000 0000 2340  .....#@(......#@
-00001320: 1400 0000 0000 0054 6e61 6d65 0923 4030  .......Tname.#@0
-00001330: 0000 0000 0000 0008 001d 0032 0044 004c  ...........2.D.L
-00001340: 0060 0072 007b 008d 0098 00ab 00b4 00b6  .`.r.{..........
-00001350: 00b7 00c3 00cc 00d7 00e1 00e7 00ef 00f4  ................
-00001360: 00f5 00f8 00f9 0102 0108 0112 011a 0123  ...............#
-00001370: 0125 0126 0127 0130 013d 013e 0140 0141  .%.&.'.0.=.>.@.A
-00001380: 014a 0156 0157 0158 0161 0166 0167 0169  .J.V.W.X.a.f.g.i
-00001390: 016a 0173 0178 0179 017b 017c 0185 018b  .j.s.x.y.{.|....
-000013a0: 018c 018e 018f 0198 01a0 01a1 01a3 01a4  ................
-000013b0: 01ad 01b6 01b7 01b8 01c1 01d0 01d1 01d3  ................
-000013c0: 01d4 01dd 01e7 01e8 01e9 01ea 01f3 01fc  ................
-000013d0: 0205 020a 020b 0000 0000 0000 0201 0000  ................
-000013e0: 0000 0000 0050 0000 0000 0000 0000 0000  .....P..........
-000013f0: 0000 0000 0214 0000 000b 005f 005f 0070  ..........._._.p
-00001400: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00001410: 6c73 7670 626c 6f62 0000 029b 6270 6c69  lsvpblob....bpli
-00001420: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
-00001430: 0c0d 1c46 4748 490c 4b5f 1012 7669 6577  ...FGHI.K_..view
-00001440: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
-00001450: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-00001460: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-00001470: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
-00001480: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
-00001490: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
-000014a0: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
-000014b0: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
-000014c0: 7665 4461 7465 7358 6963 6f6e 5369 7a65  veDatesXiconSize
-000014d0: 1001 09d9 0e0f 1011 1213 1415 1617 2025  .............. %
-000014e0: 2a2f 3439 3e42 5863 6f6d 6d65 6e74 735e  */49>BXcomments^
-000014f0: 6461 7465 4c61 7374 4f70 656e 6564 5b64  dateLastOpened[d
-00001500: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
-00001510: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
-00001520: 6f6e 546e 616d 655c 6461 7465 4d6f 6469  onTname\dateModi
-00001530: 6669 6564 d418 191a 1b1c 0c1e 1f57 7669  fied.........Wvi
-00001540: 7369 626c 6559 6173 6365 6e64 696e 6755  sibleYascendingU
-00001550: 7769 6474 6855 696e 6465 7808 0911 012c  widthUindex....,
-00001560: 1007 d418 191a 1b1c 1c23 2408 0810 c810  .........#$.....
-00001570: 08d4 1819 1a1b 1c1c 2829 0808 10b5 1002  ........()......
-00001580: d418 191a 1b0c 1c2d 2e09 0810 6110 03d4  .......-....a...
-00001590: 1819 1a1b 1c0c 3233 0809 1064 1005 d418  ......23...d....
-000015a0: 191a 1b0c 0c37 3809 0910 7310 04d4 1819  .....78...s.....
-000015b0: 1a1b 1c0c 3c3d 0809 104b 1006 d418 191a  ....<=...K......
-000015c0: 1b0c 0c1e 4109 0910 00d4 1819 1a1b 0c1c  ....A...........
-000015d0: 280b 0908 0823 0000 0000 0000 0000 2340  (....#........#@
-000015e0: 2800 0000 0000 0023 4014 0000 0000 0000  (......#@.......
-000015f0: 546e 616d 6509 2340 3000 0000 0000 0000  Tname.#@0.......
-00001600: 0800 1d00 3200 4400 4c00 6000 7200 7b00  ....2.D.L.`.r.{.
-00001610: 8d00 9800 ab00 b400 b600 b700 ca00 d300  ................
-00001620: e200 ee00 f300 f900 fe01 0601 0b01 1801  ................
-00001630: 2101 2901 3301 3901 3f01 4001 4101 4401  !.).3.9.?.@.A.D.
-00001640: 4601 4f01 5001 5101 5301 5501 5e01 5f01  F.O.P.Q.S.U.^._.
-00001650: 6001 6201 6401 6d01 6e01 6f01 7101 7301  `.b.d.m.n.o.q.s.
-00001660: 7c01 7d01 7e01 8001 8201 8b01 8c01 8d01  |.}.~...........
-00001670: 8f01 9101 9a01 9b01 9c01 9e01 a001 a901  ................
-00001680: aa01 ab01 ad01 b601 b701 b801 b901 c201  ................
-00001690: cb01 d401 d901 da00 0000 0000 0002 0100  ................
-000016a0: 0000 0000 0000 4c00 0000 0000 0000 0000  ......L.........
-000016b0: 0000 0000 0001 e300 0000 0b00 5f00 5f00  ............_._.
-000016c0: 7000 7900 6300 6100 6300 6800 6500 5f00  p.y.c.a.c.h.e._.
-000016d0: 5f76 5372 6e6c 6f6e 6700 0000 0100 0000  _vSrnlong.......
-000016e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000016f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001110: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
+00001120: 0000 0002 9e74 0000 000b 005f 005f 0070  .....t....._._.p
+00001130: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
+00001140: 6c73 7643 626c 6f62 0000 02d4 6270 6c69  lsvCblob....bpli
+00001150: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
+00001160: 0c0d 1d4a 4b4c 4d0c 4f5f 1012 7669 6577  ...JKLM.O_..view
+00001170: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
+00001180: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+00001190: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+000011a0: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
+000011b0: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
+000011c0: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
+000011d0: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
+000011e0: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
+000011f0: 7665 4461 7465 7358 6963 6f6e 5369 7a65  veDatesXiconSize
+00001200: 1001 09ab 0e17 1f24 282d 3237 3c40 45d4  .......$(-27<@E.
+00001210: 0f10 1112 130c 150c 5a69 6465 6e74 6966  ........Zidentif
+00001220: 6965 7259 6173 6365 6e64 696e 6755 7769  ierYascendingUwi
+00001230: 6474 6857 7669 7369 626c 6554 6e61 6d65  dthWvisibleTname
+00001240: 0911 012c 09d4 0f18 191a 1b1c 1d1d 5577  ...,..........Uw
+00001250: 6964 7468 5961 7363 656e 6469 6e67 5776  idthYascendingWv
+00001260: 6973 6962 6c65 5875 6269 7175 6974 7910  isibleXubiquity.
+00001270: 2308 08d4 0f10 1112 201d 220c 5c64 6174  #....... .".\dat
+00001280: 654d 6f64 6966 6965 6408 10b5 09d4 0f10  eModified.......
+00001290: 1112 251d 221d 5b64 6174 6543 7265 6174  ..%.".[dateCreat
+000012a0: 6564 0808 d40f 1011 1229 1d2b 0c54 7369  ed.......).+.Tsi
+000012b0: 7a65 0810 6109 d40f 1011 122e 0c30 0c54  ze..a........0.T
+000012c0: 6b69 6e64 0910 7309 d40f 1011 1233 0c35  kind..s......3.5
+000012d0: 1d55 6c61 6265 6c09 1064 08d4 0f10 1112  .Ulabel..d......
+000012e0: 380c 3a1d 5776 6572 7369 6f6e 0910 4b08  8.:.Wversion..K.
+000012f0: d40f 1011 123d 0c15 1d58 636f 6d6d 656e  .....=...Xcommen
+00001300: 7473 0908 d40f 1011 1241 1d43 1d5e 6461  ts.......A.C.^da
+00001310: 7465 4c61 7374 4f70 656e 6564 0810 c808  teLastOpened....
+00001320: d40f 1819 1a46 221d 1d59 6461 7465 4164  .....F"..YdateAd
+00001330: 6465 6408 0808 2300 0000 0000 0000 0023  ded...#........#
+00001340: 4028 0000 0000 0000 2340 1400 0000 0000  @(......#@......
+00001350: 0054 6e61 6d65 0923 4030 0000 0000 0000  .Tname.#@0......
+00001360: 0008 001d 0032 0044 004c 0060 0072 007b  .....2.D.L.`.r.{
+00001370: 008d 0098 00ab 00b4 00b6 00b7 00c3 00cc  ................
+00001380: 00d7 00e1 00e7 00ef 00f4 00f5 00f8 00f9  ................
+00001390: 0102 0108 0112 011a 0123 0125 0126 0127  .........#.%.&.'
+000013a0: 0130 013d 013e 0140 0141 014a 0156 0157  .0.=.>.@.A.J.V.W
+000013b0: 0158 0161 0166 0167 0169 016a 0173 0178  .X.a.f.g.i.j.s.x
+000013c0: 0179 017b 017c 0185 018b 018c 018e 018f  .y.{.|..........
+000013d0: 0198 01a0 01a1 01a3 01a4 01ad 01b6 01b7  ................
+000013e0: 01b8 01c1 01d0 01d1 01d3 01d4 01dd 01e7  ................
+000013f0: 01e8 01e9 01ea 01f3 01fc 0205 020a 020b  ................
+00001400: 0000 0000 0000 0201 0000 0000 0000 0050  ...............P
+00001410: 0000 0000 0000 0000 0000 0000 0000 0214  ................
+00001420: 0000 000b 005f 005f 0070 0079 0063 0061  ....._._.p.y.c.a
+00001430: 0063 0068 0065 005f 005f 6c73 7670 626c  .c.h.e._._lsvpbl
+00001440: 6f62 0000 029b 6270 6c69 7374 3030 da01  ob....bplist00..
+00001450: 0203 0405 0607 0809 0a0b 0c0d 1c46 4748  .............FGH
+00001460: 490c 4b5f 1012 7669 6577 4f70 7469 6f6e  I.K_..viewOption
+00001470: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
+00001480: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
+00001490: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
+000014a0: 6c53 697a 6573 5f10 0f73 6372 6f6c 6c50  lSizes_..scrollP
+000014b0: 6f73 6974 696f 6e59 5874 6578 7453 697a  ositionYXtextSiz
+000014c0: 655f 100f 7363 726f 6c6c 506f 7369 7469  e_..scrollPositi
+000014d0: 6f6e 585a 736f 7274 436f 6c75 6d6e 5f10  onXZsortColumn_.
+000014e0: 1075 7365 5265 6c61 7469 7665 4461 7465  .useRelativeDate
+000014f0: 7358 6963 6f6e 5369 7a65 1001 09d9 0e0f  sXiconSize......
+00001500: 1011 1213 1415 1617 2025 2a2f 3439 3e42  ........ %*/49>B
+00001510: 5863 6f6d 6d65 6e74 735e 6461 7465 4c61  Xcomments^dateLa
+00001520: 7374 4f70 656e 6564 5b64 6174 6543 7265  stOpened[dateCre
+00001530: 6174 6564 5473 697a 6555 6c61 6265 6c54  atedTsizeUlabelT
+00001540: 6b69 6e64 5776 6572 7369 6f6e 546e 616d  kindWversionTnam
+00001550: 655c 6461 7465 4d6f 6469 6669 6564 d418  e\dateModified..
+00001560: 191a 1b1c 0c1e 1f57 7669 7369 626c 6559  .......WvisibleY
+00001570: 6173 6365 6e64 696e 6755 7769 6474 6855  ascendingUwidthU
+00001580: 696e 6465 7808 0911 012c 1007 d418 191a  index....,......
+00001590: 1b1c 1c23 2408 0810 c810 08d4 1819 1a1b  ...#$...........
+000015a0: 1c1c 2829 0808 10b5 1002 d418 191a 1b0c  ..()............
+000015b0: 1c2d 2e09 0810 6110 03d4 1819 1a1b 1c0c  .-....a.........
+000015c0: 3233 0809 1064 1005 d418 191a 1b0c 0c37  23...d.........7
+000015d0: 3809 0910 7310 04d4 1819 1a1b 1c0c 3c3d  8...s.........<=
+000015e0: 0809 104b 1006 d418 191a 1b0c 0c1e 4109  ...K..........A.
+000015f0: 0910 00d4 1819 1a1b 0c1c 280b 0908 0823  ..........(....#
+00001600: 0000 0000 0000 0000 2340 2800 0000 0000  ........#@(.....
+00001610: 0023 4014 0000 0000 0000 546e 616d 6509  .#@.......Tname.
+00001620: 2340 3000 0000 0000 0000 0800 1d00 3200  #@0...........2.
+00001630: 4400 4c00 6000 7200 7b00 8d00 9800 ab00  D.L.`.r.{.......
+00001640: b400 b600 b700 ca00 d300 e200 ee00 f300  ................
+00001650: f900 fe01 0601 0b01 1801 2101 2901 3301  ..........!.).3.
+00001660: 3901 3f01 4001 4101 4401 4601 4f01 5001  9.?.@.A.D.F.O.P.
+00001670: 5101 5301 5501 5e01 5f01 6001 6201 6401  Q.S.U.^._.`.b.d.
+00001680: 6d01 6e01 6f01 7101 7301 7c01 7d01 7e01  m.n.o.q.s.|.}.~.
+00001690: 8001 8201 8b01 8c01 8d01 8f01 9101 9a01  ................
+000016a0: 9b01 9c01 9e01 a001 a901 aa01 ab01 ad01  ................
+000016b0: b601 b701 b801 b901 c201 cb01 d401 d901  ................
+000016c0: da00 0000 0000 0002 0100 0000 0000 0000  ................
+000016d0: 4c00 0000 0000 0000 0000 0000 0000 0001  L...............
+000016e0: e300 0000 0b00 5f00 5f00 7000 7900 6300  ......_._.p.y.c.
+000016f0: 6100 6300 6800 6500 5f00 5f6d 6f44 4462  a.c.h.e._._moDDb
+00001700: 6c6f 6200 0000 083b d4ec c21b 1fc5 4100  lob....;......A.
+00001710: 0000 0b00 5f00 5f00 7000 7900 6300 6100  ...._._.p.y.c.a.
+00001720: 6300 6800 6500 5f00 5f6d 6f64 4462 6c6f  c.h.e._._modDblo
+00001730: 6200 0000 083b d4ec c21b 1fc5 4100 0000  b....;......A...
+00001740: 0b00 5f00 5f00 7000 7900 6300 6100 6300  .._._.p.y.c.a.c.
+00001750: 6800 6500 5f00 5f70 6831 5363 6f6d 7000  h.e._._ph1Scomp.
+00001760: 0000 0000 0350 0000 0000 0b00 5f00 5f00  .....P......_._.
+00001770: 7000 7900 6300 6100 6300 6800 6500 5f00  p.y.c.a.c.h.e._.
+00001780: 5f76 5372 6e6c 6f6e 6700 0000 0100 0000  _vSrnlong.......
 00001790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000017a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000017b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000017c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000017d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000017e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000017f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -457,56 +457,56 @@
 00001c80: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001c90: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 00001ca0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 00001cb0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
 00001cc0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
 00001cd0: 0000 0000 0104 0000 0000 0000 0108 0000  ................
 00001ce0: 0000 0000 0110 0000 0000 0000 0120 0000  ............. ..
-00001cf0: 0000 0000 0140 0000 0000 0000 0064 5b64  .....@.......d[d
-00001d00: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
-00001d10: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
-00001d20: 6f6e 546e 616d 655c 6461 7465 4d6f 6469  onTname\dateModi
-00001d30: 6669 6564 d418 191a 1b1c 0c1e 1f57 7669  fied.........Wvi
-00001d40: 7369 626c 6559 6173 6365 6e64 696e 6755  sibleYascendingU
-00001d50: 7769 6474 6855 696e 6465 7808 0911 012c  widthUindex....,
-00001d60: 1007 d418 191a 1b1c 1c23 2408 0810 c810  .........#$.....
-00001d70: 08d4 1819 1a1b 1c1c 2829 0808 10b5 1002  ........()......
-00001d80: d418 191a 1b0c 1c2d 2e09 0810 6110 03d4  .......-....a...
-00001d90: 1819 1a1b 1c0c 3233 0809 1064 1005 d418  ......23...d....
-00001da0: 191a 1b0c 0c37 3809 0910 7310 04d4 1819  .....78...s.....
-00001db0: 1a1b 1c0c 3c3d 0809 104b 1006 d418 191a  ....<=...K......
-00001dc0: 1b0c 0c1e 4109 0910 00d4 1819 1a1b 0c1c  ....A...........
-00001dd0: 280b 0908 0823 0000 0000 0000 0000 2340  (....#........#@
-00001de0: 2800 0000 0000 0023 4014 0000 0000 0000  (......#@.......
-00001df0: 546e 616d 6509 2340 3000 0000 0000 0000  Tname.#@0.......
-00001e00: 0800 1d00 3200 4400 4c00 6000 7200 7b00  ....2.D.L.`.r.{.
-00001e10: 8d00 9800 ab00 b400 b600 b700 ca00 d300  ................
-00001e20: e200 ee00 f300 f900 fe01 0601 0b01 1801  ................
-00001e30: 2101 2901 3301 3901 3f01 4001 4101 4401  !.).3.9.?.@.A.D.
-00001e40: 4601 4f01 5001 5101 5301 5501 5e01 5f01  F.O.P.Q.S.U.^._.
-00001e50: 6001 6201 6401 6d01 6e01 6f01 7101 7301  `.b.d.m.n.o.q.s.
-00001e60: 7c01 7d01 7e01 8001 8201 8b01 8c01 8d01  |.}.~...........
-00001e70: 8f01 9101 9a01 9b01 9c01 9e01 a001 a901  ................
-00001e80: aa01 ab01 ad01 b601 b701 b801 b901 c201  ................
-00001e90: cb01 d401 d901 da00 0000 0000 0002 0100  ................
-00001ea0: 0000 0000 0000 4c00 0000 0000 0000 0000  ......L.........
-00001eb0: 0000 0000 0001 e300 0000 0b00 5f00 5f00  ............_._.
-00001ec0: 7000 7900 6300 6100 6300 6800 6500 5f00  p.y.c.a.c.h.e._.
-00001ed0: 5f76 5372 6e6c 6f6e 6700 0000 0100 0000  _vSrnlong.......
-00001ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cf0: 0000 0000 0140 0000 0000 0000 00d9 0e0f  .....@..........
+00001d00: 1011 1213 1415 1617 2025 2a2f 3439 3e42  ........ %*/49>B
+00001d10: 5863 6f6d 6d65 6e74 735e 6461 7465 4c61  Xcomments^dateLa
+00001d20: 7374 4f70 656e 6564 5b64 6174 6543 7265  stOpened[dateCre
+00001d30: 6174 6564 5473 697a 6555 6c61 6265 6c54  atedTsizeUlabelT
+00001d40: 6b69 6e64 5776 6572 7369 6f6e 546e 616d  kindWversionTnam
+00001d50: 655c 6461 7465 4d6f 6469 6669 6564 d418  e\dateModified..
+00001d60: 191a 1b1c 0c1e 1f57 7669 7369 626c 6559  .......WvisibleY
+00001d70: 6173 6365 6e64 696e 6755 7769 6474 6855  ascendingUwidthU
+00001d80: 696e 6465 7808 0911 012c 1007 d418 191a  index....,......
+00001d90: 1b1c 1c23 2408 0810 c810 08d4 1819 1a1b  ...#$...........
+00001da0: 1c1c 2829 0808 10b5 1002 d418 191a 1b0c  ..()............
+00001db0: 1c2d 2e09 0810 6110 03d4 1819 1a1b 1c0c  .-....a.........
+00001dc0: 3233 0809 1064 1005 d418 191a 1b0c 0c37  23...d.........7
+00001dd0: 3809 0910 7310 04d4 1819 1a1b 1c0c 3c3d  8...s.........<=
+00001de0: 0809 104b 1006 d418 191a 1b0c 0c1e 4109  ...K..........A.
+00001df0: 0910 00d4 1819 1a1b 0c1c 280b 0908 0823  ..........(....#
+00001e00: 0000 0000 0000 0000 2340 2800 0000 0000  ........#@(.....
+00001e10: 0023 4014 0000 0000 0000 546e 616d 6509  .#@.......Tname.
+00001e20: 2340 3000 0000 0000 0000 0800 1d00 3200  #@0...........2.
+00001e30: 4400 4c00 6000 7200 7b00 8d00 9800 ab00  D.L.`.r.{.......
+00001e40: b400 b600 b700 ca00 d300 e200 ee00 f300  ................
+00001e50: f900 fe01 0601 0b01 1801 2101 2901 3301  ..........!.).3.
+00001e60: 3901 3f01 4001 4101 4401 4601 4f01 5001  9.?.@.A.D.F.O.P.
+00001e70: 5101 5301 5501 5e01 5f01 6001 6201 6401  Q.S.U.^._.`.b.d.
+00001e80: 6d01 6e01 6f01 7101 7301 7c01 7d01 7e01  m.n.o.q.s.|.}.~.
+00001e90: 8001 8201 8b01 8c01 8d01 8f01 9101 9a01  ................
+00001ea0: 9b01 9c01 9e01 a001 a901 aa01 ab01 ad01  ................
+00001eb0: b601 b701 b801 b901 c201 cb01 d401 d901  ................
+00001ec0: da00 0000 0000 0002 0100 0000 0000 0000  ................
+00001ed0: 4c00 0000 0000 0000 0000 0000 0000 0001  L...............
+00001ee0: e300 0000 0b00 5f00 5f00 7000 7900 6300  ......_._.p.y.c.
+00001ef0: 6100 6300 6800 6500 5f00 5f6d 6f44 4462  a.c.h.e._._moDDb
+00001f00: 6c6f 6200 0000 083b d4ec c21b 1fc5 4100  lob....;......A.
+00001f10: 0000 0b00 5f00 5f00 7000 7900 6300 6100  ...._._.p.y.c.a.
+00001f20: 6300 6800 6500 5f00 5f6d 6f64 4462 6c6f  c.h.e._._modDblo
+00001f30: 6200 0000 083b d4ec c21b 1fc5 4100 0000  b....;......A...
+00001f40: 0b00 5f00 5f00 7000 7900 6300 6100 6300  .._._.p.y.c.a.c.
+00001f50: 6800 6500 5f00 5f70 6831 5363 6f6d 7000  h.e._._ph1Scomp.
+00001f60: 0000 0000 0350 0000 0000 0b00 5f00 5f00  .....P......_._.
+00001f70: 7000 7900 6300 6100 6300 6800 6500 5f00  p.y.c.a.c.h.e._.
+00001f80: 5f76 5372 6e6c 6f6e 6700 0000 0100 0000  _vSrnlong.......
 00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.1/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.63.2/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.63.2/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.63.2/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.63.2/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.63.2/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.63.2/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.63.2/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.63.2/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/outlier_tools/.DS_Store`

 * *Files 19% similar despite different names*

```diff
@@ -37,23 +37,23 @@
 00000240: 0000 0008 993b 4774 e2dd c441 0000 0005  .....;Gt...A....
 00000250: 002e 0069 0064 0065 0061 6d6f 6444 626c  ...i.d.e.amodDbl
 00000260: 6f62 0000 0008 993b 4774 e2dd c441 0000  ob.....;Gt...A..
 00000270: 0005 002e 0069 0064 0065 0061 7068 3153  .....i.d.e.aph1S
 00000280: 636f 6d70 0000 0000 0000 8000 0000 000b  comp............
 00000290: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 000002a0: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-000002b0: 0000 0000 9cc1 0000 000b 005f 005f 0070  ..........._._.p
+000002b0: 0000 0000 73e1 0000 000b 005f 005f 0070  ....s......_._.p
 000002c0: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-000002d0: 6d6f 4444 626c 6f62 0000 0008 4084 ed50  moDDblob....@..P
-000002e0: 0b04 c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+000002d0: 6d6f 4444 626c 6f62 0000 0008 b6b0 7cbf  moDDblob......|.
+000002e0: 1b1f c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 000002f0: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000300: 6444 626c 6f62 0000 0008 4084 ed50 0b04  dDblob....@..P..
+00000300: 6444 626c 6f62 0000 0008 b6b0 7cbf 1b1f  dDblob......|...
 00000310: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 00000320: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-00000330: 636f 6d70 0000 0000 0001 1000 0000 0000  comp............
+00000330: 636f 6d70 0000 0000 0000 c000 0000 0000  comp............
 00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.1/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.63.2/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.63.2/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.63.2/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.63.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.63.2/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/SimBA.py` & `Simba-UW-tf-dev-1.63.2/simba/SimBA.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from simba.utils.checks import check_file_exist_and_readable, check_int
 from simba.roi_tools.ROI_define import *
 from simba.roi_tools.ROI_menus import *
 from simba.roi_tools.ROI_reset import *
 from simba.utils.read_write import get_video_meta_data
 from simba.utils.data import run_user_defined_feature_extraction_class
 from simba.utils.printing import stdout_success, stdout_warning
+
 from simba.video_processors.video_processing import (video_to_greyscale,
                                                      superimpose_frame_count,
                                                      extract_frames_from_all_videos_in_directory)
 from simba.ui.pop_ups.roi_analysis_time_bins_pop_up import ROIAnalysisTimeBinsPopUp
 from simba.ui.pop_ups.movement_analysis_pop_up import MovementAnalysisPopUp
 from simba.ui.pop_ups.roi_analysis_pop_up import ROIAnalysisPopUp
 from simba.ui.pop_ups.append_roi_features_animals_pop_up import AppendROIFeaturesByAnimalPopUp
@@ -112,14 +113,15 @@
 from simba.bounding_box_tools.boundary_menus import BoundaryMenus
 from simba.labelling.labelling_interface import select_labelling_video
 from simba.labelling.labelling_advanced_interface import select_labelling_video_advanced
 from simba.utils.enums import (Formats,
                                OS,
                                Defaults,
                                TagNames)
+from simba.utils.warnings import PythonVersionWarning
 from simba.utils.errors import InvalidInputError
 from simba.utils.lookups import get_bp_config_code_class_pairs, get_icons_paths
 from simba.mixins.pop_up_mixin import PopUpMixin
 from simba.ui.create_project_ui import ProjectCreatorPopUp
 from simba.utils.lookups import get_emojis
 import sys
 import subprocess
@@ -829,17 +831,19 @@
         y_sb.pack(side=RIGHT, fill=Y)
         self.txt.pack(expand=True, fill='both')
         y_sb.config(command=self.txt.yview)
         self.txt.config(state=DISABLED, font=Formats.TKINTER_FONT.value)
 
         clear_txt_btn = Button(self.frame, text=' CLEAR', compound=LEFT, image=self.menu_icons['clean']['img'], font=Formats.LABELFRAME_HEADER_FORMAT.value, command=lambda: self.clean_txt())
         clear_txt_btn.pack(side=BOTTOM, fill=X)
-
         sys.stdout = StdRedirector(self.txt)
 
+        if OS.PYTHON_VER.value != 3.6:
+            PythonVersionWarning(msg=f'SimBA is not extensively tested beyond python3.6. You are using python{OS.PYTHON_VER.value}. If you encounter errors, in python>={OS.PYTHON_VER.value}, please report them on GitHub or Gitter and w (links in the help toolbar)')
+
     def restart(self):
         confirm_restart = askyesno(title='RESTART', message='Are you sure that you want restart SimBA?')
         if confirm_restart:
             self.root.destroy()
             python = sys.executable
             os.execl(python, python, *sys.argv)
 
@@ -905,26 +909,24 @@
         else:
             if os.path.isfile(splash_path_linux):
                 self.splash_img = PIL.Image.open(splash_path_linux)
             else:
                 self.splash_img = PIL.Image.open(splash_path_win)
         self.splash_img_tk = ImageTk.PhotoImage(self.splash_img)
 
-
     def display_splash(self):
         width, height = self.splash_img.size
         half_width = int((self.parent.winfo_screenwidth()-width)//2)
         half_height = int((self.parent.winfo_screenheight()-height)//2)
         self.parent.geometry("%ix%i+%i+%i" %(width, height, half_width, half_height))
         Label(self.parent, image=self.splash_img_tk).pack()
 
 
 class SplashMovie():
     def __init__(self):
-        #self.parent = Tk()
         self.parent, self.img_cnt = Tk(), 0
         self.parent.overrideredirect(True)
         self.parent.configure(bg='white')
         splash_path = os.path.join(os.path.dirname(__file__), Paths.SPLASH_PATH_MOVIE.value)
         self.meta_ = get_video_meta_data(splash_path)
         self.cap = cv2.VideoCapture(splash_path)
         width, height = self.meta_['width'], self.meta_['height']
@@ -953,10 +955,10 @@
         process.terminate()
 
 def main():
     if currentPlatform == OS.WINDOWS.value:
         import ctypes
         myappid = 'SimBA development wheel'
         ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(myappid)
-    splash = SplashMovie()
+    SplashMovie()
     app = App()
     app.root.mainloop()
```

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.63.2/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.63.2/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.63.2/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.63.2/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.63.2/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/assets/shap/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -253,130 +253,130 @@
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 0008 0000 0012  ................
 00001010: 0066 0065 0061 0074 0075 0072 0065 005f  .f.e.a.t.u.r.e._
 00001020: 0063 0061 0074 0065 0067 006f 0072 0069  .c.a.t.e.g.o.r.i
-00001030: 0065 0073 6277 7370 626c 6f62 0000 00c9  .e.sbwspblob....
-00001040: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
-00001050: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
-00001060: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
-00001070: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
-00001080: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
-00001090: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
-000010a0: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
-000010b0: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
-000010c0: 187b 7b32 302c 2031 3232 7d2c 207b 3130  .{{20, 122}, {10
-000010d0: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
-000010e0: 606d 797a 7b7c 7d7e 9900 0000 0000 0001  `myz{|}~........
-000010f0: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
-00001100: 0000 0000 0000 0000 9a00 0000 1200 6600  ..............f.
-00001110: 6500 6100 7400 7500 7200 6500 5f00 6300  e.a.t.u.r.e._.c.
-00001120: 6100 7400 6500 6700 6f00 7200 6900 6500  a.t.e.g.o.r.i.e.
-00001130: 736c 6731 5363 6f6d 7000 0000 0000 0044  slg1Scomp......D
-00001140: 7900 0000 1200 6600 6500 6100 7400 7500  y.....f.e.a.t.u.
-00001150: 7200 6500 5f00 6300 6100 7400 6500 6700  r.e._.c.a.t.e.g.
-00001160: 6f00 7200 6900 6500 736c 7376 4362 6c6f  o.r.i.e.slsvCblo
-00001170: 6200 0002 7962 706c 6973 7430 30d8 0102  b...ybplist00...
-00001180: 0304 0506 0708 090a 0b18 4647 0a49 5869  ..........FG.IXi
-00001190: 636f 6e53 697a 655f 100f 7368 6f77 4963  conSize_..showIc
-000011a0: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
-000011b0: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
-000011c0: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
-000011d0: 6f72 7443 6f6c 756d 6e5f 1010 7573 6552  ortColumn_..useR
-000011e0: 656c 6174 6976 6544 6174 6573 5f10 1276  elativeDates_..v
-000011f0: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
-00001200: 6e23 4030 0000 0000 0000 09ab 0c15 1a1f  n#@0............
-00001210: 2328 2d32 373c 41d4 0d0e 0f10 1112 0a0a  #(-27<A.........
-00001220: 5a69 6465 6e74 6966 6965 7255 7769 6474  ZidentifierUwidt
-00001230: 6859 6173 6365 6e64 696e 6757 7669 7369  hYascendingWvisi
-00001240: 626c 6554 6e61 6d65 1101 2709 09d4 0d0e  bleTname..'.....
-00001250: 0f10 1617 1818 5875 6269 7175 6974 7910  ......Xubiquity.
-00001260: 2308 08d4 0d0e 0f10 1b1c 180a 5c64 6174  #...........\dat
-00001270: 654d 6f64 6966 6965 6410 b508 09d4 0d0e  eModified.......
-00001280: 0f10 201c 1818 5b64 6174 6543 7265 6174  .. ...[dateCreat
-00001290: 6564 0808 d40d 0e0f 1024 2518 0a54 7369  ed.......$%..Tsi
-000012a0: 7a65 1061 0809 d40d 0e0f 1029 2a0a 0a54  ze.a.......)*..T
-000012b0: 6b69 6e64 1073 0909 d40d 0e0f 102e 2f0a  kind.s......../.
-000012c0: 1855 6c61 6265 6c10 6409 08d4 0d0e 0f10  .Ulabel.d.......
-000012d0: 3334 0a18 5776 6572 7369 6f6e 104b 0908  34..Wversion.K..
-000012e0: d40d 0e0f 1038 390a 1858 636f 6d6d 656e  .....89..Xcommen
-000012f0: 7473 1101 2c09 08d4 0d0e 0f10 3d3e 1818  ts..,.......=>..
-00001300: 5e64 6174 654c 6173 744f 7065 6e65 6410  ^dateLastOpened.
-00001310: c808 08d4 0d0e 0f10 421c 1818 5964 6174  ........B...Ydat
-00001320: 6541 6464 6564 0808 0823 4028 0000 0000  eAdded...#@(....
-00001330: 0000 546e 616d 6509 1001 0008 0019 0022  ..Tname........"
-00001340: 0034 003c 0050 0059 0064 0077 008c 0095  .4.<.P.Y.d.w....
-00001350: 0096 00a2 00ab 00b6 00bc 00c6 00ce 00d3  ................
-00001360: 00d6 00d7 00d8 00e1 00ea 00ec 00ed 00ee  ................
-00001370: 00f7 0104 0106 0107 0108 0111 011d 011e  ................
-00001380: 011f 0128 012d 012f 0130 0131 013a 013f  ...(.-./.0.1.:.?
-00001390: 0141 0142 0143 014c 0152 0154 0155 0156  .A.B.C.L.R.T.U.V
-000013a0: 015f 0167 0169 016a 016b 0174 017d 0180  ._.g.i.j.k.t.}..
-000013b0: 0181 0182 018b 019a 019c 019d 019e 01a7  ................
-000013c0: 01b1 01b2 01b3 01b4 01bd 01c2 01c3 0000  ................
-000013d0: 0000 0000 0201 0000 0000 0000 004a 0000  .............J..
-000013e0: 0000 0000 0000 0000 0000 0000 01c5 0000  ................
-000013f0: 0012 0066 0065 0061 0074 0075 0072 0065  ...f.e.a.t.u.r.e
-00001400: 005f 0063 0061 0074 0065 0067 006f 0072  ._.c.a.t.e.g.o.r
-00001410: 0069 0065 0073 6c73 7670 626c 6f62 0000  .i.e.slsvpblob..
-00001420: 025e 6270 6c69 7374 3030 d801 0203 0405  .^bplist00......
-00001430: 0607 0809 0a0b 1a46 470a 2758 6963 6f6e  .......FG.'Xicon
-00001440: 5369 7a65 5f10 0f73 686f 7749 636f 6e50  Size_..showIconP
-00001450: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
-00001460: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
-00001470: 6573 5874 6578 7453 697a 655a 736f 7274  esXtextSizeZsort
-00001480: 436f 6c75 6d6e 5f10 1075 7365 5265 6c61  Column_..useRela
-00001490: 7469 7665 4461 7465 735f 1012 7669 6577  tiveDates_..view
-000014a0: 4f70 7469 6f6e 7356 6572 7369 6f6e 2340  OptionsVersion#@
-000014b0: 3000 0000 0000 0009 d90c 0d0e 0f10 1112  0...............
-000014c0: 1314 151e 2328 2c31 363b 4058 636f 6d6d  ....#(,16;@Xcomm
-000014d0: 656e 7473 5e64 6174 654c 6173 744f 7065  ents^dateLastOpe
-000014e0: 6e65 645c 6461 7465 4d6f 6469 6669 6564  ned\dateModified
-000014f0: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
-00001500: 6555 6c61 6265 6c54 6b69 6e64 5776 6572  eUlabelTkindWver
-00001510: 7369 6f6e 546e 616d 65d4 1617 1819 1a1b  sionTname.......
-00001520: 0a1d 5776 6973 6962 6c65 5577 6964 7468  ..WvisibleUwidth
-00001530: 5961 7363 656e 6469 6e67 5569 6e64 6578  YascendingUindex
-00001540: 0811 012c 0910 07d4 1617 1819 1a20 1a22  ...,......... ."
-00001550: 0810 c808 1008 d416 1718 190a 251a 2709  ............%.'.
-00001560: 10b5 0810 01d4 1617 1819 1a25 1a2b 0808  ...........%.+..
-00001570: 1002 d416 1718 190a 2e1a 3009 1061 0810  ..........0..a..
-00001580: 03d4 1617 1819 1a33 0a35 0810 6409 1005  .......3.5..d...
-00001590: d416 1718 190a 380a 3a09 1073 0910 04d4  ......8.:..s....
-000015a0: 1617 1819 1a3d 0a3f 0810 4b09 1006 d416  .....=.?..K.....
-000015b0: 1718 190a 420a 4409 1101 2709 1000 0823  ....B.D...'....#
-000015c0: 4028 0000 0000 0000 546e 616d 6509 0008  @(......Tname...
-000015d0: 0019 0022 0034 003c 0050 0059 0064 0077  ...".4.<.P.Y.d.w
-000015e0: 008c 0095 0096 00a9 00b2 00c1 00ce 00da  ................
-000015f0: 00df 00e5 00ea 00f2 00f7 0100 0108 010e  ................
-00001600: 0118 011e 011f 0122 0123 0125 012e 012f  .......".#.%.../
-00001610: 0131 0132 0134 013d 013e 0140 0141 0143  .1.2.4.=.>.@.A.C
-00001620: 014c 014d 014e 0150 0159 015a 015c 015d  .L.M.N.P.Y.Z.\.]
-00001630: 015f 0168 0169 016b 016c 016e 0177 0178  ._.h.i.k.l.n.w.x
-00001640: 017a 017b 017d 0186 0187 0189 018a 018c  .z.{.}..........
-00001650: 0195 0196 0199 019a 019c 019d 01a6 01ab  ................
-00001660: 0000 0000 0000 0201 0000 0000 0000 0049  ...............I
-00001670: 0000 0000 0000 0000 0000 0000 0000 01ac  ................
-00001680: 0000 0012 0066 0065 0061 0074 0075 0072  .....f.e.a.t.u.r
-00001690: 0065 005f 0063 0061 0074 0065 0067 006f  .e._.c.a.t.e.g.o
-000016a0: 0072 0069 0065 0073 6d6f 4444 626c 6f62  .r.i.e.smoDDblob
-000016b0: 0000 0008 9da1 3b74 e2dd c441 0000 0012  ......;t...A....
-000016c0: 0066 0065 0061 0074 0075 0072 0065 005f  .f.e.a.t.u.r.e._
-000016d0: 0063 0061 0074 0065 0067 006f 0072 0069  .c.a.t.e.g.o.r.i
-000016e0: 0065 0073 6d6f 6444 626c 6f62 0000 0008  .e.smodDblob....
-000016f0: 9da1 3b74 e2dd c441 0000 0012 0066 0065  ..;t...A.....f.e
-00001700: 0061 0074 0075 0072 0065 005f 0063 0061  .a.t.u.r.e._.c.a
-00001710: 0074 0065 0067 006f 0072 0069 0065 0073  .t.e.g.o.r.i.e.s
-00001720: 7068 3153 636f 6d70 0000 0000 0000 6000  ph1Scomp......`.
-00001730: 0000 0012 0066 0065 0061 0074 0075 0072  .....f.e.a.t.u.r
-00001740: 0065 005f 0063 0061 0074 0065 0067 006f  .e._.c.a.t.e.g.o
-00001750: 0072 0069 0065 0073 7653 726e 6c6f 6e67  .r.i.e.svSrnlong
-00001760: 0000 0001 0000 0000 0000 0000 0000 0000  ................
+00001030: 0065 0073 6277 7370 626c 6f62 0000 00b9  .e.sbwspblob....
+00001040: 6270 6c69 7374 3030 d601 0203 0405 0607  bplist00........
+00001050: 0807 080b 085d 5368 6f77 5374 6174 7573  .....]ShowStatus
+00001060: 4261 725b 5368 6f77 546f 6f6c 6261 725b  Bar[ShowToolbar[
+00001070: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
+00001080: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
+00001090: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
+000010a0: 5368 6f77 5369 6465 6261 7208 0908 095f  ShowSidebar...._
+000010b0: 1019 7b7b 3130 342c 2031 3632 7d2c 207b  ..{{104, 162}, {
+000010c0: 3131 3933 2c20 3731 337d 7d09 0815 232f  1193, 713}}...#/
+000010d0: 3b52 5f6b 6c6d 6e6f 8b00 0000 0000 0001  ;R_klmno........
+000010e0: 0100 0000 0000 0000 0d00 0000 0000 0000  ................
+000010f0: 0000 0000 0000 0000 8c00 0000 1200 6600  ..............f.
+00001100: 6500 6100 7400 7500 7200 6500 5f00 6300  e.a.t.u.r.e._.c.
+00001110: 6100 7400 6500 6700 6f00 7200 6900 6500  a.t.e.g.o.r.i.e.
+00001120: 736c 6731 5363 6f6d 7000 0000 0000 0044  slg1Scomp......D
+00001130: 7900 0000 1200 6600 6500 6100 7400 7500  y.....f.e.a.t.u.
+00001140: 7200 6500 5f00 6300 6100 7400 6500 6700  r.e._.c.a.t.e.g.
+00001150: 6f00 7200 6900 6500 736c 7376 4362 6c6f  o.r.i.e.slsvCblo
+00001160: 6200 0002 7962 706c 6973 7430 30d8 0102  b...ybplist00...
+00001170: 0304 0506 0708 090a 0b18 4647 0a49 5869  ..........FG.IXi
+00001180: 636f 6e53 697a 655f 100f 7368 6f77 4963  conSize_..showIc
+00001190: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
+000011a0: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
+000011b0: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
+000011c0: 6f72 7443 6f6c 756d 6e5f 1010 7573 6552  ortColumn_..useR
+000011d0: 656c 6174 6976 6544 6174 6573 5f10 1276  elativeDates_..v
+000011e0: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
+000011f0: 6e23 4030 0000 0000 0000 09ab 0c15 1a1f  n#@0............
+00001200: 2328 2d32 373c 41d4 0d0e 0f10 1112 0a0a  #(-27<A.........
+00001210: 5a69 6465 6e74 6966 6965 7255 7769 6474  ZidentifierUwidt
+00001220: 6859 6173 6365 6e64 696e 6757 7669 7369  hYascendingWvisi
+00001230: 626c 6554 6e61 6d65 1101 2709 09d4 0d0e  bleTname..'.....
+00001240: 0f10 1617 1818 5875 6269 7175 6974 7910  ......Xubiquity.
+00001250: 2308 08d4 0d0e 0f10 1b1c 180a 5c64 6174  #...........\dat
+00001260: 654d 6f64 6966 6965 6410 b508 09d4 0d0e  eModified.......
+00001270: 0f10 201c 1818 5b64 6174 6543 7265 6174  .. ...[dateCreat
+00001280: 6564 0808 d40d 0e0f 1024 2518 0a54 7369  ed.......$%..Tsi
+00001290: 7a65 1061 0809 d40d 0e0f 1029 2a0a 0a54  ze.a.......)*..T
+000012a0: 6b69 6e64 1073 0909 d40d 0e0f 102e 2f0a  kind.s......../.
+000012b0: 1855 6c61 6265 6c10 6409 08d4 0d0e 0f10  .Ulabel.d.......
+000012c0: 3334 0a18 5776 6572 7369 6f6e 104b 0908  34..Wversion.K..
+000012d0: d40d 0e0f 1038 390a 1858 636f 6d6d 656e  .....89..Xcommen
+000012e0: 7473 1101 2c09 08d4 0d0e 0f10 3d3e 1818  ts..,.......=>..
+000012f0: 5e64 6174 654c 6173 744f 7065 6e65 6410  ^dateLastOpened.
+00001300: c808 08d4 0d0e 0f10 421c 1818 5964 6174  ........B...Ydat
+00001310: 6541 6464 6564 0808 0823 4028 0000 0000  eAdded...#@(....
+00001320: 0000 546e 616d 6509 1001 0008 0019 0022  ..Tname........"
+00001330: 0034 003c 0050 0059 0064 0077 008c 0095  .4.<.P.Y.d.w....
+00001340: 0096 00a2 00ab 00b6 00bc 00c6 00ce 00d3  ................
+00001350: 00d6 00d7 00d8 00e1 00ea 00ec 00ed 00ee  ................
+00001360: 00f7 0104 0106 0107 0108 0111 011d 011e  ................
+00001370: 011f 0128 012d 012f 0130 0131 013a 013f  ...(.-./.0.1.:.?
+00001380: 0141 0142 0143 014c 0152 0154 0155 0156  .A.B.C.L.R.T.U.V
+00001390: 015f 0167 0169 016a 016b 0174 017d 0180  ._.g.i.j.k.t.}..
+000013a0: 0181 0182 018b 019a 019c 019d 019e 01a7  ................
+000013b0: 01b1 01b2 01b3 01b4 01bd 01c2 01c3 0000  ................
+000013c0: 0000 0000 0201 0000 0000 0000 004a 0000  .............J..
+000013d0: 0000 0000 0000 0000 0000 0000 01c5 0000  ................
+000013e0: 0012 0066 0065 0061 0074 0075 0072 0065  ...f.e.a.t.u.r.e
+000013f0: 005f 0063 0061 0074 0065 0067 006f 0072  ._.c.a.t.e.g.o.r
+00001400: 0069 0065 0073 6c73 7670 626c 6f62 0000  .i.e.slsvpblob..
+00001410: 025e 6270 6c69 7374 3030 d801 0203 0405  .^bplist00......
+00001420: 0607 0809 0a0b 1a46 470a 2758 6963 6f6e  .......FG.'Xicon
+00001430: 5369 7a65 5f10 0f73 686f 7749 636f 6e50  Size_..showIconP
+00001440: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
+00001450: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
+00001460: 6573 5874 6578 7453 697a 655a 736f 7274  esXtextSizeZsort
+00001470: 436f 6c75 6d6e 5f10 1075 7365 5265 6c61  Column_..useRela
+00001480: 7469 7665 4461 7465 735f 1012 7669 6577  tiveDates_..view
+00001490: 4f70 7469 6f6e 7356 6572 7369 6f6e 2340  OptionsVersion#@
+000014a0: 3000 0000 0000 0009 d90c 0d0e 0f10 1112  0...............
+000014b0: 1314 151e 2328 2c31 363b 4058 636f 6d6d  ....#(,16;@Xcomm
+000014c0: 656e 7473 5e64 6174 654c 6173 744f 7065  ents^dateLastOpe
+000014d0: 6e65 645c 6461 7465 4d6f 6469 6669 6564  ned\dateModified
+000014e0: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
+000014f0: 6555 6c61 6265 6c54 6b69 6e64 5776 6572  eUlabelTkindWver
+00001500: 7369 6f6e 546e 616d 65d4 1617 1819 1a1b  sionTname.......
+00001510: 0a1d 5776 6973 6962 6c65 5577 6964 7468  ..WvisibleUwidth
+00001520: 5961 7363 656e 6469 6e67 5569 6e64 6578  YascendingUindex
+00001530: 0811 012c 0910 07d4 1617 1819 1a20 1a22  ...,......... ."
+00001540: 0810 c808 1008 d416 1718 190a 251a 2709  ............%.'.
+00001550: 10b5 0810 01d4 1617 1819 1a25 1a2b 0808  ...........%.+..
+00001560: 1002 d416 1718 190a 2e1a 3009 1061 0810  ..........0..a..
+00001570: 03d4 1617 1819 1a33 0a35 0810 6409 1005  .......3.5..d...
+00001580: d416 1718 190a 380a 3a09 1073 0910 04d4  ......8.:..s....
+00001590: 1617 1819 1a3d 0a3f 0810 4b09 1006 d416  .....=.?..K.....
+000015a0: 1718 190a 420a 4409 1101 2709 1000 0823  ....B.D...'....#
+000015b0: 4028 0000 0000 0000 546e 616d 6509 0008  @(......Tname...
+000015c0: 0019 0022 0034 003c 0050 0059 0064 0077  ...".4.<.P.Y.d.w
+000015d0: 008c 0095 0096 00a9 00b2 00c1 00ce 00da  ................
+000015e0: 00df 00e5 00ea 00f2 00f7 0100 0108 010e  ................
+000015f0: 0118 011e 011f 0122 0123 0125 012e 012f  .......".#.%.../
+00001600: 0131 0132 0134 013d 013e 0140 0141 0143  .1.2.4.=.>.@.A.C
+00001610: 014c 014d 014e 0150 0159 015a 015c 015d  .L.M.N.P.Y.Z.\.]
+00001620: 015f 0168 0169 016b 016c 016e 0177 0178  ._.h.i.k.l.n.w.x
+00001630: 017a 017b 017d 0186 0187 0189 018a 018c  .z.{.}..........
+00001640: 0195 0196 0199 019a 019c 019d 01a6 01ab  ................
+00001650: 0000 0000 0000 0201 0000 0000 0000 0049  ...............I
+00001660: 0000 0000 0000 0000 0000 0000 0000 01ac  ................
+00001670: 0000 0012 0066 0065 0061 0074 0075 0072  .....f.e.a.t.u.r
+00001680: 0065 005f 0063 0061 0074 0065 0067 006f  .e._.c.a.t.e.g.o
+00001690: 0072 0069 0065 0073 6d6f 4444 626c 6f62  .r.i.e.smoDDblob
+000016a0: 0000 0008 9da1 3b74 e2dd c441 0000 0012  ......;t...A....
+000016b0: 0066 0065 0061 0074 0075 0072 0065 005f  .f.e.a.t.u.r.e._
+000016c0: 0063 0061 0074 0065 0067 006f 0072 0069  .c.a.t.e.g.o.r.i
+000016d0: 0065 0073 6d6f 6444 626c 6f62 0000 0008  .e.smodDblob....
+000016e0: 9da1 3b74 e2dd c441 0000 0012 0066 0065  ..;t...A.....f.e
+000016f0: 0061 0074 0075 0072 0065 005f 0063 0061  .a.t.u.r.e._.c.a
+00001700: 0074 0065 0067 006f 0072 0069 0065 0073  .t.e.g.o.r.i.e.s
+00001710: 7068 3153 636f 6d70 0000 0000 0000 6000  ph1Scomp......`.
+00001720: 0000 0012 0066 0065 0061 0074 0075 0072  .....f.e.a.t.u.r
+00001730: 0065 005f 0063 0061 0074 0065 0067 006f  .e._.c.a.t.e.g.o
+00001740: 0072 0069 0065 0073 7653 726e 6c6f 6e67  .r.i.e.svSrnlong
+00001750: 0000 0001 0000 0000 0000 0000 0000 0000  ................
+00001760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000017a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000017b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000017c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000017d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -457,54 +457,54 @@
 00001c80: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001c90: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 00001ca0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 00001cb0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
 00001cc0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
 00001cd0: 0000 0000 0104 0000 0000 0000 0108 0000  ................
 00001ce0: 0000 0000 0110 0000 0000 0000 0120 0000  ............. ..
-00001cf0: 0000 0000 0140 0000 0000 0000 0073 697a  .....@.......siz
-00001d00: 6555 6c61 6265 6c54 6b69 6e64 5776 6572  eUlabelTkindWver
-00001d10: 7369 6f6e 546e 616d 65d4 1617 1819 1a1b  sionTname.......
-00001d20: 0a1d 5776 6973 6962 6c65 5577 6964 7468  ..WvisibleUwidth
-00001d30: 5961 7363 656e 6469 6e67 5569 6e64 6578  YascendingUindex
-00001d40: 0811 012c 0910 07d4 1617 1819 1a20 1a22  ...,......... ."
-00001d50: 0810 c808 1008 d416 1718 190a 251a 2709  ............%.'.
-00001d60: 10b5 0810 01d4 1617 1819 1a25 1a2b 0808  ...........%.+..
-00001d70: 1002 d416 1718 190a 2e1a 3009 1061 0810  ..........0..a..
-00001d80: 03d4 1617 1819 1a33 0a35 0810 6409 1005  .......3.5..d...
-00001d90: d416 1718 190a 380a 3a09 1073 0910 04d4  ......8.:..s....
-00001da0: 1617 1819 1a3d 0a3f 0810 4b09 1006 d416  .....=.?..K.....
-00001db0: 1718 190a 420a 4409 1101 2709 1000 0823  ....B.D...'....#
-00001dc0: 4028 0000 0000 0000 546e 616d 6509 0008  @(......Tname...
-00001dd0: 0019 0022 0034 003c 0050 0059 0064 0077  ...".4.<.P.Y.d.w
-00001de0: 008c 0095 0096 00a9 00b2 00c1 00ce 00da  ................
-00001df0: 00df 00e5 00ea 00f2 00f7 0100 0108 010e  ................
-00001e00: 0118 011e 011f 0122 0123 0125 012e 012f  .......".#.%.../
-00001e10: 0131 0132 0134 013d 013e 0140 0141 0143  .1.2.4.=.>.@.A.C
-00001e20: 014c 014d 014e 0150 0159 015a 015c 015d  .L.M.N.P.Y.Z.\.]
-00001e30: 015f 0168 0169 016b 016c 016e 0177 0178  ._.h.i.k.l.n.w.x
-00001e40: 017a 017b 017d 0186 0187 0189 018a 018c  .z.{.}..........
-00001e50: 0195 0196 0199 019a 019c 019d 01a6 01ab  ................
-00001e60: 0000 0000 0000 0201 0000 0000 0000 0049  ...............I
-00001e70: 0000 0000 0000 0000 0000 0000 0000 01ac  ................
-00001e80: 0000 0012 0066 0065 0061 0074 0075 0072  .....f.e.a.t.u.r
-00001e90: 0065 005f 0063 0061 0074 0065 0067 006f  .e._.c.a.t.e.g.o
-00001ea0: 0072 0069 0065 0073 6d6f 4444 626c 6f62  .r.i.e.smoDDblob
-00001eb0: 0000 0008 9da1 3b74 e2dd c441 0000 0012  ......;t...A....
-00001ec0: 0066 0065 0061 0074 0075 0072 0065 005f  .f.e.a.t.u.r.e._
-00001ed0: 0063 0061 0074 0065 0067 006f 0072 0069  .c.a.t.e.g.o.r.i
-00001ee0: 0065 0073 6d6f 6444 626c 6f62 0000 0008  .e.smodDblob....
-00001ef0: 9da1 3b74 e2dd c441 0000 0012 0066 0065  ..;t...A.....f.e
-00001f00: 0061 0074 0075 0072 0065 005f 0063 0061  .a.t.u.r.e._.c.a
-00001f10: 0074 0065 0067 006f 0072 0069 0065 0073  .t.e.g.o.r.i.e.s
-00001f20: 7068 3153 636f 6d70 0000 0000 0000 6000  ph1Scomp......`.
-00001f30: 0000 0012 0066 0065 0061 0074 0075 0072  .....f.e.a.t.u.r
-00001f40: 0065 005f 0063 0061 0074 0065 0067 006f  .e._.c.a.t.e.g.o
-00001f50: 0072 0069 0065 0073 7653 726e 6c6f 6e67  .r.i.e.svSrnlong
-00001f60: 0000 0001 0000 0000 0000 0000 0000 0000  ................
+00001cf0: 0000 0000 0140 0000 0000 0000 0076 6572  .....@.......ver
+00001d00: 7369 6f6e 546e 616d 65d4 1617 1819 1a1b  sionTname.......
+00001d10: 0a1d 5776 6973 6962 6c65 5577 6964 7468  ..WvisibleUwidth
+00001d20: 5961 7363 656e 6469 6e67 5569 6e64 6578  YascendingUindex
+00001d30: 0811 012c 0910 07d4 1617 1819 1a20 1a22  ...,......... ."
+00001d40: 0810 c808 1008 d416 1718 190a 251a 2709  ............%.'.
+00001d50: 10b5 0810 01d4 1617 1819 1a25 1a2b 0808  ...........%.+..
+00001d60: 1002 d416 1718 190a 2e1a 3009 1061 0810  ..........0..a..
+00001d70: 03d4 1617 1819 1a33 0a35 0810 6409 1005  .......3.5..d...
+00001d80: d416 1718 190a 380a 3a09 1073 0910 04d4  ......8.:..s....
+00001d90: 1617 1819 1a3d 0a3f 0810 4b09 1006 d416  .....=.?..K.....
+00001da0: 1718 190a 420a 4409 1101 2709 1000 0823  ....B.D...'....#
+00001db0: 4028 0000 0000 0000 546e 616d 6509 0008  @(......Tname...
+00001dc0: 0019 0022 0034 003c 0050 0059 0064 0077  ...".4.<.P.Y.d.w
+00001dd0: 008c 0095 0096 00a9 00b2 00c1 00ce 00da  ................
+00001de0: 00df 00e5 00ea 00f2 00f7 0100 0108 010e  ................
+00001df0: 0118 011e 011f 0122 0123 0125 012e 012f  .......".#.%.../
+00001e00: 0131 0132 0134 013d 013e 0140 0141 0143  .1.2.4.=.>.@.A.C
+00001e10: 014c 014d 014e 0150 0159 015a 015c 015d  .L.M.N.P.Y.Z.\.]
+00001e20: 015f 0168 0169 016b 016c 016e 0177 0178  ._.h.i.k.l.n.w.x
+00001e30: 017a 017b 017d 0186 0187 0189 018a 018c  .z.{.}..........
+00001e40: 0195 0196 0199 019a 019c 019d 01a6 01ab  ................
+00001e50: 0000 0000 0000 0201 0000 0000 0000 0049  ...............I
+00001e60: 0000 0000 0000 0000 0000 0000 0000 01ac  ................
+00001e70: 0000 0012 0066 0065 0061 0074 0075 0072  .....f.e.a.t.u.r
+00001e80: 0065 005f 0063 0061 0074 0065 0067 006f  .e._.c.a.t.e.g.o
+00001e90: 0072 0069 0065 0073 6d6f 4444 626c 6f62  .r.i.e.smoDDblob
+00001ea0: 0000 0008 9da1 3b74 e2dd c441 0000 0012  ......;t...A....
+00001eb0: 0066 0065 0061 0074 0075 0072 0065 005f  .f.e.a.t.u.r.e._
+00001ec0: 0063 0061 0074 0065 0067 006f 0072 0069  .c.a.t.e.g.o.r.i
+00001ed0: 0065 0073 6d6f 6444 626c 6f62 0000 0008  .e.smodDblob....
+00001ee0: 9da1 3b74 e2dd c441 0000 0012 0066 0065  ..;t...A.....f.e
+00001ef0: 0061 0074 0075 0072 0065 005f 0063 0061  .a.t.u.r.e._.c.a
+00001f00: 0074 0065 0067 006f 0072 0069 0065 0073  .t.e.g.o.r.i.e.s
+00001f10: 7068 3153 636f 6d70 0000 0000 0000 6000  ph1Scomp......`.
+00001f20: 0000 0012 0066 0065 0061 0074 0075 0072  .....f.e.a.t.u.r
+00001f30: 0065 005f 0063 0061 0074 0065 0067 006f  .e._.c.a.t.e.g.o
+00001f40: 0072 0069 0065 0073 7653 726e 6c6f 6e67  .r.i.e.svSrnlong
+00001f50: 0000 0001 0000 0000 0000 0000 0000 0000  ................
+00001f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.63.2/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.63.2/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.63.2/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.63.2/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.63.2/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.63.2/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.63.2/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.63.2/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.63.2/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.63.2/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.63.2/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.63.2/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/assets/.DS_Store`

 * *Files 12% similar despite different names*

```diff
@@ -428,337 +428,337 @@
 00001ab0: 0007 006c 006f 006f 006b 0075 0070 0073  ...l.o.o.k.u.p.s
 00001ac0: 6d6f 6444 626c 6f62 0000 0008 1a04 dcb9  modDblob........
 00001ad0: b8e5 c441 0000 0007 006c 006f 006f 006b  ...A.....l.o.o.k
 00001ae0: 0075 0070 0073 7068 3153 636f 6d70 0000  .u.p.sph1Scomp..
 00001af0: 0000 0004 e000 0000 0007 006c 006f 006f  ...........l.o.o
 00001b00: 006b 0075 0070 0073 7653 726e 6c6f 6e67  .k.u.p.svSrnlong
 00001b10: 0000 0001 0000 0004 0073 0068 0061 0070  .........s.h.a.p
-00001b20: 6277 7370 626c 6f62 0000 00c9 6270 6c69  bwspblob....bpli
-00001b30: 7374 3030 d701 0203 0405 0607 0808 0a08  st00............
-00001b40: 0a0d 0a5d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
-00001b50: 725b 5368 6f77 5061 7468 6261 725b 5368  r[ShowPathbar[Sh
-00001b60: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
-00001b70: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
-00001b80: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
-00001b90: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
-00001ba0: 6465 6261 7208 0809 0809 5f10 187b 7b38  debar....._..{{8
-00001bb0: 3930 2c20 3230 307d 2c20 7b37 3730 2c20  90, 200}, {770, 
-00001bc0: 3433 367d 7d09 0817 2531 3d49 606d 797a  436}}...%1=I`myz
-00001bd0: 7b7c 7d7e 9900 0000 0000 0001 0100 0000  {|}~............
-00001be0: 0000 0000 0f00 0000 0000 0000 0000 0000  ................
-00001bf0: 0000 0000 9a00 0000 0400 7300 6800 6100  ..........s.h.a.
-00001c00: 706c 6731 5363 6f6d 7000 0000 0000 0927  plg1Scomp......'
-00001c10: 3400 0000 0400 7300 6800 6100 706c 7376  4.....s.h.a.plsv
-00001c20: 4362 6c6f 6200 0002 7962 706c 6973 7430  Cblob...ybplist0
-00001c30: 30d8 0102 0304 0506 0708 090a 0b18 4647  0.............FG
-00001c40: 0a49 5869 636f 6e53 697a 655f 100f 7368  .IXiconSize_..sh
-00001c50: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
-00001c60: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
-00001c70: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
-00001c80: 7a65 5a73 6f72 7443 6f6c 756d 6e5f 1010  zeZsortColumn_..
-00001c90: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-00001ca0: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
-00001cb0: 7273 696f 6e23 4030 0000 0000 0000 09ab  rsion#@0........
-00001cc0: 0c15 1a1f 2328 2d32 373c 41d4 0d0e 0f10  ....#(-27<A.....
-00001cd0: 1112 0a0a 5a69 6465 6e74 6966 6965 7255  ....ZidentifierU
-00001ce0: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
-00001cf0: 7669 7369 626c 6554 6e61 6d65 1101 2709  visibleTname..'.
-00001d00: 09d4 0d0e 0f10 1617 1818 5875 6269 7175  ..........Xubiqu
-00001d10: 6974 7910 2308 08d4 0d0e 0f10 1b1c 180a  ity.#...........
-00001d20: 5c64 6174 654d 6f64 6966 6965 6410 b508  \dateModified...
-00001d30: 09d4 0d0e 0f10 201c 1818 5b64 6174 6543  ...... ...[dateC
-00001d40: 7265 6174 6564 0808 d40d 0e0f 1024 2518  reated.......$%.
-00001d50: 0a54 7369 7a65 1061 0809 d40d 0e0f 1029  .Tsize.a.......)
-00001d60: 2a0a 0a54 6b69 6e64 1073 0909 d40d 0e0f  *..Tkind.s......
-00001d70: 102e 2f0a 1855 6c61 6265 6c10 6409 08d4  ../..Ulabel.d...
-00001d80: 0d0e 0f10 3334 0a18 5776 6572 7369 6f6e  ....34..Wversion
-00001d90: 104b 0908 d40d 0e0f 1038 390a 1858 636f  .K.......89..Xco
-00001da0: 6d6d 656e 7473 1101 2c09 08d4 0d0e 0f10  mments..,.......
-00001db0: 3d3e 1818 5e64 6174 654c 6173 744f 7065  =>..^dateLastOpe
-00001dc0: 6e65 6410 c808 08d4 0d0e 0f10 421c 1818  ned.........B...
-00001dd0: 5964 6174 6541 6464 6564 0808 0823 4028  YdateAdded...#@(
-00001de0: 0000 0000 0000 546e 616d 6509 1001 0008  ......Tname.....
-00001df0: 0019 0022 0034 003c 0050 0059 0064 0077  ...".4.<.P.Y.d.w
-00001e00: 008c 0095 0096 00a2 00ab 00b6 00bc 00c6  ................
-00001e10: 00ce 00d3 00d6 00d7 00d8 00e1 00ea 00ec  ................
-00001e20: 00ed 00ee 00f7 0104 0106 0107 0108 0111  ................
-00001e30: 011d 011e 011f 0128 012d 012f 0130 0131  .......(.-./.0.1
-00001e40: 013a 013f 0141 0142 0143 014c 0152 0154  .:.?.A.B.C.L.R.T
-00001e50: 0155 0156 015f 0167 0169 016a 016b 0174  .U.V._.g.i.j.k.t
-00001e60: 017d 0180 0181 0182 018b 019a 019c 019d  .}..............
-00001e70: 019e 01a7 01b1 01b2 01b3 01b4 01bd 01c2  ................
-00001e80: 01c3 0000 0000 0000 0201 0000 0000 0000  ................
-00001e90: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
-00001ea0: 01c5 0063 006f 006e 0073 6d6f 4444 626c  ...c.o.n.smoDDbl
-00001eb0: 6f62 0000 0008 dc05 45af 18fa c441 0000  ob......E....A..
-00001ec0: 0005 0069 0063 006f 006e 0073 6d6f 6444  ...i.c.o.n.smodD
-00001ed0: 626c 6f62 0000 0008 dc05 45af 18fa c441  blob......E....A
-00001ee0: 0000 0005 0069 0063 006f 006e 0073 7068  .....i.c.o.n.sph
-00001ef0: 3153 636f 6d70 0000 0000 0008 1000 0000  1Scomp..........
-00001f00: 0005 0069 0063 006f 006e 0073 7653 726e  ...i.c.o.n.svSrn
-00001f10: 6c6f 6e67 0000 0001 0000 0003 0069 006d  long.........i.m
-00001f20: 0067 6277 7370 626c 6f62 0000 00c9 6270  .gbwspblob....bp
-00001f30: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
-00001f40: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
-00001f50: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
-00001f60: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
-00001f70: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-00001f80: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-00001f90: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-00001fa0: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
-00001fb0: 7b31 3132 2c20 3535 7d2c 207b 3131 3939  {112, 55}, {1199
-00001fc0: 2c20 3736 397d 7d09 0817 2531 3d49 606d  , 769}}...%1=I`m
-00001fd0: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
-00001fe0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
-00001ff0: 0000 0000 0000 9a00 0000 0300 6900 6d00  ............i.m.
-00002000: 676c 6731 0000 0000 0000 0012 0000 0005  glg1............
+00001b20: 6277 7370 626c 6f62 0000 00b9 6270 6c69  bwspblob....bpli
+00001b30: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
+00001b40: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+00001b50: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+00001b60: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+00001b70: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+00001b80: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+00001b90: 5369 6465 6261 7208 0908 095f 1019 7b7b  Sidebar...._..{{
+00001ba0: 3130 342c 2031 3632 7d2c 207b 3131 3933  104, 162}, {1193
+00001bb0: 2c20 3731 337d 7d09 0815 232f 3b52 5f6b  , 713}}...#/;R_k
+00001bc0: 6c6d 6e6f 8b00 0000 0000 0001 0100 0000  lmno............
+00001bd0: 0000 0000 0d00 0000 0000 0000 0000 0000  ................
+00001be0: 0000 0000 8c00 0000 0400 7300 6800 6100  ..........s.h.a.
+00001bf0: 706c 6731 5363 6f6d 7000 0000 0000 0927  plg1Scomp......'
+00001c00: 3400 0000 0400 7300 6800 6100 706c 7376  4.....s.h.a.plsv
+00001c10: 4362 6c6f 6200 0002 7962 706c 6973 7430  Cblob...ybplist0
+00001c20: 30d8 0102 0304 0506 0708 090a 0b18 4647  0.............FG
+00001c30: 0a49 5869 636f 6e53 697a 655f 100f 7368  .IXiconSize_..sh
+00001c40: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
+00001c50: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
+00001c60: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
+00001c70: 7a65 5a73 6f72 7443 6f6c 756d 6e5f 1010  zeZsortColumn_..
+00001c80: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+00001c90: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+00001ca0: 7273 696f 6e23 4030 0000 0000 0000 09ab  rsion#@0........
+00001cb0: 0c15 1a1f 2328 2d32 373c 41d4 0d0e 0f10  ....#(-27<A.....
+00001cc0: 1112 0a0a 5a69 6465 6e74 6966 6965 7255  ....ZidentifierU
+00001cd0: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
+00001ce0: 7669 7369 626c 6554 6e61 6d65 1101 2709  visibleTname..'.
+00001cf0: 09d4 0d0e 0f10 1617 1818 5875 6269 7175  ..........Xubiqu
+00001d00: 6974 7910 2308 08d4 0d0e 0f10 1b1c 180a  ity.#...........
+00001d10: 5c64 6174 654d 6f64 6966 6965 6410 b508  \dateModified...
+00001d20: 09d4 0d0e 0f10 201c 1818 5b64 6174 6543  ...... ...[dateC
+00001d30: 7265 6174 6564 0808 d40d 0e0f 1024 2518  reated.......$%.
+00001d40: 0a54 7369 7a65 1061 0809 d40d 0e0f 1029  .Tsize.a.......)
+00001d50: 2a0a 0a54 6b69 6e64 1073 0909 d40d 0e0f  *..Tkind.s......
+00001d60: 102e 2f0a 1855 6c61 6265 6c10 6409 08d4  ../..Ulabel.d...
+00001d70: 0d0e 0f10 3334 0a18 5776 6572 7369 6f6e  ....34..Wversion
+00001d80: 104b 0908 d40d 0e0f 1038 390a 1858 636f  .K.......89..Xco
+00001d90: 6d6d 656e 7473 1101 2c09 08d4 0d0e 0f10  mments..,.......
+00001da0: 3d3e 1818 5e64 6174 654c 6173 744f 7065  =>..^dateLastOpe
+00001db0: 6e65 6410 c808 08d4 0d0e 0f10 421c 1818  ned.........B...
+00001dc0: 5964 6174 6541 6464 6564 0808 0823 4028  YdateAdded...#@(
+00001dd0: 0000 0000 0000 546e 616d 6509 1001 0008  ......Tname.....
+00001de0: 0019 0022 0034 003c 0050 0059 0064 0077  ...".4.<.P.Y.d.w
+00001df0: 008c 0095 0096 00a2 00ab 00b6 00bc 00c6  ................
+00001e00: 00ce 00d3 00d6 00d7 00d8 00e1 00ea 00ec  ................
+00001e10: 00ed 00ee 00f7 0104 0106 0107 0108 0111  ................
+00001e20: 011d 011e 011f 0128 012d 012f 0130 0131  .......(.-./.0.1
+00001e30: 013a 013f 0141 0142 0143 014c 0152 0154  .:.?.A.B.C.L.R.T
+00001e40: 0155 0156 015f 0167 0169 016a 016b 0174  .U.V._.g.i.j.k.t
+00001e50: 017d 0180 0181 0182 018b 019a 019c 019d  .}..............
+00001e60: 019e 01a7 01b1 01b2 01b3 01b4 01bd 01c2  ................
+00001e70: 01c3 0000 0000 0000 0201 0000 0000 0000  ................
+00001e80: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
+00001e90: 01c5 6801 6901 6b01 7401 7501 7701 7801  ..h.i.k.t.u.w.x.
+00001ea0: 7a01 8301 8401 8601 8701 8901 9201 9301  z...............
+00001eb0: 9401 9601 9f01 a001 a201 a301 a501 ae01  ................
+00001ec0: b001 b301 b401 b501 be01 bf01 c101 c201  ................
+00001ed0: c401 c501 ce01 d701 e001 e500 0000 0000  ................
+00001ee0: 0002 0100 0000 0000 0000 4d00 0000 0000  ..........M.....
+00001ef0: 0000 0000 0000 0000 0001 e600 0000 0500  ................
+00001f00: 6900 6300 6f00 6e00 736d 6f44 4462 6c6f  i.c.o.n.smoDDblo
+00001f10: 6200 0000 08dc 0545 af18 fac4 4100 0000  b......E....A...
+00001f20: 0500 6900 6300 6f00 6e00 736d 6f64 4462  ..i.c.o.n.smodDb
+00001f30: 6c6f 6200 0000 08dc 0545 af18 fac4 4100  lob......E....A.
+00001f40: 0000 0500 6900 6300 6f00 6e00 7370 6831  ....i.c.o.n.sph1
+00001f50: 5363 6f6d 7000 0000 0000 0810 0000 0000  Scomp...........
+00001f60: 0500 6900 6300 6f00 6e00 7376 5372 6e6c  ..i.c.o.n.svSrnl
+00001f70: 6f6e 6700 0000 0100 0000 0300 6900 6d00  ong.........i.m.
+00001f80: 6762 7773 7062 6c6f 6200 0000 b862 706c  gbwspblob....bpl
+00001f90: 6973 7430 30d6 0102 0304 0506 0708 0708  ist00...........
+00001fa0: 0b08 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
+00001fb0: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
+00001fc0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
+00001fd0: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
+00001fe0: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
+00001ff0: 7753 6964 6562 6172 0809 0809 5f10 187b  wSidebar...._..{
+00002000: 7b33 3335 0000 0000 0000 0012 0000 0005  {335............
 00002010: 0069 0063 006f 006e 0073 6277 7370 626c  .i.c.o.n.sbwspbl
-00002020: 6f62 0000 00c9 6270 6c69 7374 3030 d701  ob....bplist00..
-00002030: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
-00002040: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-00002050: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
-00002060: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
-00002070: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
-00002080: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00002090: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-000020a0: 0809 0809 5f10 187b 7b31 3132 2c20 3535  ...._..{{112, 55
-000020b0: 7d2c 207b 3131 3939 2c20 3736 397d 7d09  }, {1199, 769}}.
-000020c0: 0817 2531 3d49 606d 797a 7b7c 7d7e 9900  ..%1=I`myz{|}~..
-000020d0: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
-000020e0: 0000 0000 0000 0000 0000 0000 0000 9a00  ................
-000020f0: 0000 0500 6900 6300 6f00 6e00 736c 6731  ....i.c.o.n.slg1
-00002100: 5363 6f6d 7000 0000 0000 05a1 0300 0000  Scomp...........
-00002110: 0500 6900 6300 6f00 6e00 736c 7376 4362  ..i.c.o.n.slsvCb
-00002120: 6c6f 6200 0002 bb62 706c 6973 7430 30da  lob....bplist00.
-00002130: 0102 0304 0506 0708 090a 0b0c 0d1a 4849  ..............HI
-00002140: 4a4b 4c0c 5f10 1276 6965 774f 7074 696f  JKL._..viewOptio
-00002150: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
-00002160: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
-00002170: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
-00002180: 6c6c 5369 7a65 735f 100f 7363 726f 6c6c  llSizes_..scroll
-00002190: 506f 7369 7469 6f6e 5958 7465 7874 5369  PositionYXtextSi
-000021a0: 7a65 5f10 0f73 6372 6f6c 6c50 6f73 6974  ze_..scrollPosit
-000021b0: 696f 6e58 5a73 6f72 7443 6f6c 756d 6e58  ionXZsortColumnX
-000021c0: 6963 6f6e 5369 7a65 5f10 1075 7365 5265  iconSize_..useRe
-000021d0: 6c61 7469 7665 4461 7465 7310 0109 ab0e  lativeDates.....
-000021e0: 171c 2125 2a2f 3439 3e43 d40f 1011 120c  ..!%*/49>C......
-000021f0: 140c 1657 7669 7369 626c 6555 7769 6474  ...WvisibleUwidt
-00002200: 6859 6173 6365 6e64 696e 675a 6964 656e  hYascendingZiden
-00002210: 7469 6669 6572 0911 0160 0954 6e61 6d65  tifier...`.Tname
-00002220: d412 1011 0f18 191a 1a58 7562 6971 7569  .........Xubiqui
-00002230: 7479 1023 0808 d412 1011 0f1d 1e1a 0c5c  ty.#...........\
-00002240: 6461 7465 4d6f 6469 6669 6564 10b5 0809  dateModified....
-00002250: d412 1011 0f22 1e1a 1a5b 6461 7465 4372  ....."...[dateCr
-00002260: 6561 7465 6408 08d4 1210 110f 2627 1a0c  eated.......&'..
-00002270: 5473 697a 6510 6108 09d4 1210 110f 2b2c  Tsize.a.......+,
-00002280: 0c0c 546b 696e 6410 7309 09d4 1210 110f  ..Tkind.s.......
-00002290: 3031 0c1a 556c 6162 656c 1064 0908 d412  01..Ulabel.d....
-000022a0: 1011 0f35 360c 1a57 7665 7273 696f 6e10  ...56..Wversion.
-000022b0: 4b09 08d4 1210 110f 3a3b 0c1a 5863 6f6d  K.......:;..Xcom
-000022c0: 6d65 6e74 7311 012c 0908 d412 1011 0f3f  ments..,.......?
-000022d0: 401a 1a5e 6461 7465 4c61 7374 4f70 656e  @..^dateLastOpen
-000022e0: 6564 10c8 0808 d412 1011 0f44 1e1a 1a59  ed.........D...Y
-000022f0: 6461 7465 4164 6465 6408 0808 2340 72b0  dateAdded...#@r.
-00002300: 0000 0000 0023 4028 0000 0000 0000 2300  .....#@(......#.
-00002310: 0000 0000 0000 0054 6e61 6d65 2340 3000  .......Tname#@0.
-00002320: 0000 0000 0009 0008 001d 0032 0044 004c  ...........2.D.L
-00002330: 0060 0072 007b 008d 0098 00a1 00b4 00b6  .`.r.{..........
-00002340: 00b7 00c3 00cc 00d4 00da 00e4 00ef 00f0  ................
-00002350: 00f3 00f4 00f9 0102 010b 010d 010e 010f  ................
-00002360: 0118 0125 0127 0128 0129 0132 013e 013f  ...%.'.(.).2.>.?
-00002370: 0140 0149 014e 0150 0151 0152 015b 0160  .@.I.N.P.Q.R.[.`
-00002380: 0162 0163 0164 016d 0173 0175 0176 0177  .b.c.d.m.s.u.v.w
-00002390: 0180 0188 018a 018b 018c 0195 019e 01a1  ................
-000023a0: 01a2 01a3 01ac 01bb 01bd 01be 01bf 01c8  ................
-000023b0: 01d2 01d3 01d4 01d5 01de 01e7 01f0 01f5  ................
-000023c0: 01fe 0000 0000 0000 0201 0000 0000 0000  ................
-000023d0: 004e 0000 0000 0000 0000 0000 0000 0000  .N..............
-000023e0: 01ff 0000 0005 0069 0063 006f 006e 0073  .......i.c.o.n.s
-000023f0: 6c73 7670 626c 6f62 0000 02a0 6270 6c69  lsvpblob....bpli
-00002400: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
-00002410: 0c0d 1c47 4849 4a4b 0c5f 1012 7669 6577  ...GHIJK._..view
-00002420: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
-00002430: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-00002440: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-00002450: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
-00002460: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
-00002470: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
-00002480: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
-00002490: 6c75 6d6e 5869 636f 6e53 697a 655f 1010  lumnXiconSize_..
-000024a0: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-000024b0: 1001 09d9 0e0f 1011 1213 1415 1617 2025  .............. %
-000024c0: 292d 3237 3c41 5863 6f6d 6d65 6e74 735e  )-27<AXcomments^
-000024d0: 6461 7465 4c61 7374 4f70 656e 6564 5c64  dateLastOpened\d
-000024e0: 6174 654d 6f64 6966 6965 645b 6461 7465  ateModified[date
-000024f0: 4372 6561 7465 6454 7369 7a65 556c 6162  CreatedTsizeUlab
-00002500: 656c 546b 696e 6457 7665 7273 696f 6e54  elTkindWversionT
-00002510: 6e61 6d65 d418 191a 1b1c 1d0c 1f57 7669  name.........Wvi
-00002520: 7369 626c 6555 7769 6474 6859 6173 6365  sibleUwidthYasce
-00002530: 6e64 696e 6755 696e 6465 7808 1101 2c09  ndingUindex...,.
-00002540: 1007 d418 191a 1b1c 221c 2408 10c8 0810  ........".$.....
-00002550: 08d4 1819 1a1b 0c27 1c0b 0910 b508 d418  .......'........
-00002560: 191a 1b1c 271c 2c08 0810 02d4 1819 1a1b  ....'.,.........
-00002570: 0c2f 1c31 0910 6108 1003 d418 191a 1b1c  ./.1..a.........
-00002580: 340c 3608 1064 0910 05d4 1819 1a1b 0c39  4.6..d.........9
-00002590: 0c3b 0910 7309 1004 d418 191a 1b1c 3e0c  .;..s.........>.
-000025a0: 4008 104b 0910 06d4 1b19 1a18 4243 0c0c  @..K........BC..
-000025b0: 1000 1101 6009 0908 2340 72b0 0000 0000  ....`...#@r.....
-000025c0: 0023 4028 0000 0000 0000 2300 0000 0000  .#@(......#.....
-000025d0: 0000 0054 6e61 6d65 2340 3000 0000 0000  ...Tname#@0.....
-000025e0: 0009 0008 001d 0032 0044 004c 0060 0072  .......2.D.L.`.r
-000025f0: 007b 008d 0098 00a1 00b4 00b6 00b7 00ca  .{..............
-00002600: 00d3 00e2 00ef 00fb 0100 0106 010b 0113  ................
-00002610: 0118 0121 0129 012f 0139 013f 0140 0143  ...!.)./.9.?.@.C
-00002620: 0144 0146 014f 0150 0152 0153 0155 015e  .D.F.O.P.R.S.U.^
-00002630: 015f 0161 0162 016b 016c 016d 016f 0178  ._.a.b.k.l.m.o.x
-00002640: 0179 017b 017c 017e 0187 0188 018a 018b  .y.{.|.~........
-00002650: 018d 0196 0197 0199 019a 019c 01a5 01a6  ................
-00002660: 01a8 01a9 01ab 01b4 01b6 01b9 01ba 01bb  ................
-00002670: 01bc 01c5 01ce 01d7 01dc 01e5 0000 0000  ................
-00002680: 0000 0201 0000 0000 0000 004d 0000 0000  ...........M....
-00002690: 0000 0000 0000 0000 0000 01e6 0000 0005  ................
-000026a0: 0069 0063 006f 006e 0073 6d6f 4444 626c  .i.c.o.n.smoDDbl
-000026b0: 6f62 0000 0008 dc05 45af 18fa c441 0000  ob......E....A..
-000026c0: 0005 0069 0063 006f 006e 0073 6d6f 6444  ...i.c.o.n.smodD
-000026d0: 626c 6f62 0000 0008 dc05 45af 18fa c441  blob......E....A
-000026e0: 0000 0005 0069 0063 006f 006e 0073 7068  .....i.c.o.n.sph
-000026f0: 3153 636f 6d70 0000 0000 0008 1000 0000  1Scomp..........
-00002700: 0005 0069 0063 006f 006e 0073 7653 726e  ...i.c.o.n.svSrn
-00002710: 6c6f 6e67 0000 0001 0000 0003 0069 006d  long.........i.m
-00002720: 0067 6277 7370 626c 6f62 0000 00c9 6270  .gbwspblob....bp
-00002730: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
-00002740: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
-00002750: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
-00002760: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
-00002770: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-00002780: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-00002790: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-000027a0: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
-000027b0: 7b31 3132 2c20 3535 7d2c 207b 3131 3939  {112, 55}, {1199
-000027c0: 2c20 3736 397d 7d09 0817 2531 3d49 606d  , 769}}...%1=I`m
-000027d0: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
-000027e0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
-000027f0: 0000 0000 0000 9a00 0000 0300 6900 6d00  ............i.m.
-00002800: 676c 6731 5363 6f6d 7000 0000 0000 1111  glg1Scomp.......
-00002810: 6400 0000 0300 6900 6d00 676c 7376 4362  d.....i.m.glsvCb
-00002820: 6c6f 6200 0002 b062 706c 6973 7430 30da  lob....bplist00.
-00002830: 0102 0304 0506 0708 090a 0b0b 0d18 4849  ..............HI
-00002840: 484a 4b4c 5f10 1075 7365 5265 6c61 7469  HJKL_..useRelati
-00002850: 7665 4461 7465 735f 100f 7368 6f77 4963  veDates_..showIc
-00002860: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
-00002870: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
-00002880: 5369 7a65 735f 100f 7363 726f 6c6c 506f  Sizes_..scrollPo
-00002890: 7369 7469 6f6e 5958 7465 7874 5369 7a65  sitionYXtextSize
-000028a0: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
-000028b0: 6e58 5a73 6f72 7443 6f6c 756d 6e58 6963  nXZsortColumnXic
-000028c0: 6f6e 5369 7a65 5f10 1276 6965 774f 7074  onSize_..viewOpt
-000028d0: 696f 6e73 5665 7273 696f 6e09 09ab 0e17  ionsVersion.....
-000028e0: 1c21 252a 2f34 393e 43d4 0f10 1112 0b14  .!%*/49>C.......
-000028f0: 0b16 5776 6973 6962 6c65 5577 6964 7468  ..WvisibleUwidth
-00002900: 5961 7363 656e 6469 6e67 5a69 6465 6e74  YascendingZident
-00002910: 6966 6965 7209 1101 c709 546e 616d 65d4  ifier.....Tname.
-00002920: 0f10 1112 1819 181b 0810 2308 5875 6269  ..........#.Xubi
-00002930: 7175 6974 79d4 0f10 1112 0b1e 1820 0910  quity........ ..
-00002940: b508 5c64 6174 654d 6f64 6966 6965 64d4  ..\dateModified.
-00002950: 0f10 1112 181e 1824 0808 5b64 6174 6543  .......$..[dateC
-00002960: 7265 6174 6564 d40f 1011 120b 2718 2909  reated......'.).
-00002970: 1061 0854 7369 7a65 d40f 1011 120b 2c0b  .a.Tsize......,.
-00002980: 2e09 1073 0954 6b69 6e64 d40f 1011 1218  ...s.Tkind......
-00002990: 310b 3308 1064 0955 6c61 6265 6cd4 0f10  1.3..d.Ulabel...
-000029a0: 1112 1836 0b38 0810 4b09 5776 6572 7369  ...6.8..K.Wversi
-000029b0: 6f6e d40f 1011 1218 3b0b 3d08 1101 2c09  on......;.=...,.
-000029c0: 5863 6f6d 6d65 6e74 73d4 0f10 1112 1840  Xcomments......@
-000029d0: 1842 0810 c808 5e64 6174 654c 6173 744f  .B....^dateLastO
-000029e0: 7065 6e65 64d4 0f10 1112 181e 1846 0808  pened........F..
-000029f0: 5964 6174 6541 6464 6564 0823 0000 0000  YdateAdded.#....
-00002a00: 0000 0000 2340 2800 0000 0000 0054 6e61  ....#@(......Tna
-00002a10: 6d65 2340 3000 0000 0000 0010 0100 0800  me#@0...........
-00002a20: 1d00 3000 4200 4a00 5e00 7000 7900 8b00  ..0.B.J.^.p.y...
-00002a30: 9600 9f00 b400 b500 b600 c200 cb00 d300  ................
-00002a40: d900 e300 ee00 ef00 f200 f300 f801 0101  ................
-00002a50: 0201 0401 0501 0e01 1701 1801 1a01 1b01  ................
-00002a60: 2801 3101 3201 3301 3f01 4801 4901 4b01  (.1.2.3.?.H.I.K.
-00002a70: 4c01 5101 5a01 5b01 5d01 5e01 6301 6c01  L.Q.Z.[.].^.c.l.
-00002a80: 6d01 6f01 7001 7601 7f01 8001 8201 8301  m.o.p.v.........
-00002a90: 8b01 9401 9501 9801 9901 a201 ab01 ac01  ................
-00002aa0: ae01 af01 be01 c701 c801 c901 d301 d401  ................
-00002ab0: dd01 e601 eb01 f400 0000 0000 0002 0100  ................
-00002ac0: 0000 0000 0000 4d00 0000 0000 0000 0000  ......M.........
-00002ad0: 0000 0000 0001 f600 0000 0300 6900 6d00  ............i.m.
-00002ae0: 676c 7376 7062 6c6f 6200 0002 9562 706c  glsvpblob....bpl
-00002af0: 6973 7430 30da 0102 0304 0506 0708 090a  ist00...........
-00002b00: 0b0b 0d1f 4849 484a 4b26 5f10 1075 7365  ....HIHJK&_..use
-00002b10: 5265 6c61 7469 7665 4461 7465 735f 100f  RelativeDates_..
-00002b20: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
-00002b30: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
-00002b40: 6174 6541 6c6c 5369 7a65 735f 100f 7363  ateAllSizes_..sc
-00002b50: 726f 6c6c 506f 7369 7469 6f6e 5958 7465  rollPositionYXte
-00002b60: 7874 5369 7a65 5f10 0f73 6372 6f6c 6c50  xtSize_..scrollP
-00002b70: 6f73 6974 696f 6e58 5a73 6f72 7443 6f6c  ositionXZsortCol
-00002b80: 756d 6e58 6963 6f6e 5369 7a65 5f10 1276  umnXiconSize_..v
-00002b90: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
-00002ba0: 6e09 09d9 0e0f 1011 1213 1415 1617 2025  n............. %
-00002bb0: 2a2e 3338 3d42 5863 6f6d 6d65 6e74 735e  *.38=BXcomments^
-00002bc0: 6461 7465 4c61 7374 4f70 656e 6564 5c64  dateLastOpened\d
-00002bd0: 6174 654d 6f64 6966 6965 645b 6461 7465  ateModified[date
-00002be0: 4372 6561 7465 6454 7369 7a65 556c 6162  CreatedTsizeUlab
-00002bf0: 656c 546b 696e 6457 7665 7273 696f 6e54  elTkindWversionT
-00002c00: 6e61 6d65 d418 191a 1b1c 1d0b 1f55 696e  name.........Uin
-00002c10: 6465 7855 7769 6474 6859 6173 6365 6e64  dexUwidthYascend
-00002c20: 696e 6757 7669 7369 626c 6510 0711 012c  ingWvisible....,
-00002c30: 0908 d418 191a 1b21 221f 1f10 0810 c808  .......!".......
-00002c40: 08d4 1819 1a1b 2627 1f0b 1001 10b5 0809  ......&'........
-00002c50: d418 191a 1b2b 271f 1f10 0208 08d4 1819  .....+'.........
-00002c60: 1a1b 2f30 1f0b 1003 1061 0809 d418 191a  ../0.....a......
-00002c70: 1b34 350b 1f10 0510 6409 08d4 1819 1a1b  .45.....d.......
-00002c80: 393a 0b0b 1004 1073 0909 d418 191a 1b3e  9:.....s.......>
-00002c90: 3f0b 1f10 0610 4b09 08d4 1819 1a1b 4344  ?.....K.......CD
-00002ca0: 0b0b 1000 1101 c709 0908 2300 0000 0000  ..........#.....
-00002cb0: 0000 0023 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
-00002cc0: 6523 4030 0000 0000 0000 0008 001d 0030  e#@0...........0
-00002cd0: 0042 004a 005e 0070 0079 008b 0096 009f  .B.J.^.p.y......
-00002ce0: 00b4 00b5 00b6 00c9 00d2 00e1 00ee 00fa  ................
-00002cf0: 00ff 0105 010a 0112 0117 0120 0126 012c  ........... .&.,
-00002d00: 0136 013e 0140 0143 0144 0145 014e 0150  .6.>.@.C.D.E.N.P
-00002d10: 0152 0153 0154 015d 015f 0161 0162 0163  .R.S.T.]._.a.b.c
-00002d20: 016c 016e 016f 0170 0179 017b 017d 017e  .l.n.o.p.y.{.}.~
-00002d30: 017f 0188 018a 018c 018d 018e 0197 0199  ................
-00002d40: 019b 019c 019d 01a6 01a8 01aa 01ab 01ac  ................
-00002d50: 01b5 01b7 01ba 01bb 01bc 01bd 01c6 01cf  ................
-00002d60: 01d4 0000 0000 0000 0201 0000 0000 0000  ................
-00002d70: 004c 0000 0000 0000 0000 0000 0000 0000  .L..............
-00002d80: 01dd 0000 0003 0069 006d 0067 6d6f 4444  .......i.m.gmoDD
-00002d90: 626c 6f62 0000 0008 7c5a d8a5 7105 c541  blob....|Z..q..A
-00002da0: 0000 0003 0069 006d 0067 6d6f 6444 626c  .....i.m.gmodDbl
-00002db0: 6f62 0000 0008 7c5a d8a5 7105 c541 0000  ob....|Z..q..A..
-00002dc0: 0003 0069 006d 0067 7068 3153 636f 6d70  ...i.m.gph1Scomp
-00002dd0: 0000 0000 0011 4000 0000 0003 0069 006d  ......@......i.m
-00002de0: 0067 7653 726e 6c6f 6e67 0000 0001 0000  .gvSrnlong......
-00002df0: 0007 006c 006f 006f 006b 0075 0070 0073  ...l.o.o.k.u.p.s
-00002e00: 6277 7370 626c 6f62 0000 00c8 6270 6c69  bwspblob....bpli
-00002e10: 7374 3030 d701 0203 0405 0607 0808 0a08  st00............
-00002e20: 0a0d 0a5d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
-00002e30: 725b 5368 6f77 5061 7468 6261 725b 5368  r[ShowPathbar[Sh
-00002e40: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
-00002e50: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
-00002e60: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
-00002e70: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
-00002e80: 6465 6261 7208 0809 0809 5f10 177b 7b32  debar....._..{{2
-00002e90: 302c 2039 307d 2c20 7b31 3031 352c 2037  0, 90}, {1015, 7
-00002ea0: 3637 7d7d 0908 1725 313d 4960 6d79 7a7b  67}}...%1=I`myz{
-00002eb0: 7c7d 7e98 0000 0000 0000 0101 0000 0000  |}~.............
-00002ec0: 0000 000f 0000 0000 0000 0000 0000 0000  ................
-00002ed0: 0000 0099 0000 0007 006c 006f 006f 006b  .........l.o.o.k
-00002ee0: 0075 0070 0073 6c67 3153 636f 6d70 0000  .u.p.slg1Scomp..
-00002ef0: 0000 0004 b42c 0000 0000 0000 0000 0000  .....,..........
-00002f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002020: 6f62 0000 00b8 6270 6c69 7374 3030 d601  ob....bplist00..
+00002030: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
+00002040: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
+00002050: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
+00002060: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
+00002070: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
+00002080: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
+00002090: 7208 0908 095f 1018 7b7b 3637 302c 2033  r...._..{{670, 3
+000020a0: 3939 7d2c 207b 3737 302c 2034 3336 7d7d  99}, {770, 436}}
+000020b0: 0908 1523 2f3b 525f 6b6c 6d6e 6f8a 0000  ...#/;R_klmno...
+000020c0: 0000 0000 0101 0000 0000 0000 000d 0000  ................
+000020d0: 0000 0000 0000 0000 0000 0000 008b 0000  ................
+000020e0: 0005 0069 0063 006f 006e 0073 6c67 3153  ...i.c.o.n.slg1S
+000020f0: 636f 6d70 0000 0000 0005 a103 0000 0005  comp............
+00002100: 0069 0063 006f 006e 0073 6c73 7643 626c  .i.c.o.n.slsvCbl
+00002110: 6f62 0000 032b 6270 6c69 7374 3030 da01  ob...+bplist00..
+00002120: 0203 0405 0607 0809 0a0b 0c0d 1a55 5657  .............UVW
+00002130: 580c 5a58 6963 6f6e 5369 7a65 5f10 0f73  X.ZXiconSize_..s
+00002140: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
+00002150: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
+00002160: 7465 416c 6c53 697a 6573 5f10 0f73 6372  teAllSizes_..scr
+00002170: 6f6c 6c50 6f73 6974 696f 6e59 5874 6578  ollPositionYXtex
+00002180: 7453 697a 655f 100f 7363 726f 6c6c 506f  tSize_..scrollPo
+00002190: 7369 7469 6f6e 585a 736f 7274 436f 6c75  sitionXZsortColu
+000021a0: 6d6e 5f10 1075 7365 5265 6c61 7469 7665  mn_..useRelative
+000021b0: 4461 7465 735f 1012 7669 6577 4f70 7469  Dates_..viewOpti
+000021c0: 6f6e 7356 6572 7369 6f6e 2340 3000 0000  onsVersion#@0...
+000021d0: 0000 0009 ae0e 171c 2125 2a2f 3439 3e43  ........!%*/49>C
+000021e0: 474c 50d4 0f10 1112 0c14 0c16 5776 6973  GLP.........Wvis
+000021f0: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
+00002200: 6469 6e67 5a69 6465 6e74 6966 6965 7209  dingZidentifier.
+00002210: 1101 6009 546e 616d 65d4 1210 110f 1819  ..`.Tname.......
+00002220: 1a1a 5875 6269 7175 6974 7910 2308 08d4  ..Xubiquity.#...
+00002230: 1210 110f 1d1e 1a0c 5c64 6174 654d 6f64  ........\dateMod
+00002240: 6966 6965 6410 b508 09d4 1210 110f 221e  ified.........".
+00002250: 1a1a 5b64 6174 6543 7265 6174 6564 0808  ..[dateCreated..
+00002260: d412 1011 0f26 271a 0c54 7369 7a65 1061  .....&'..Tsize.a
+00002270: 0809 d412 1011 0f2b 2c0c 0c54 6b69 6e64  .......+,..Tkind
+00002280: 1073 0909 d412 1011 0f30 310c 1a55 6c61  .s.......01..Ula
+00002290: 6265 6c10 6409 08d4 1210 110f 3536 0c1a  bel.d.......56..
+000022a0: 5776 6572 7369 6f6e 104b 0908 d412 1011  Wversion.K......
+000022b0: 0f3a 3b0c 1a58 636f 6d6d 656e 7473 1101  .:;..Xcomments..
+000022c0: 2c09 08d4 1210 110f 3f40 1a1a 5e64 6174  ,.......?@..^dat
+000022d0: 654c 6173 744f 7065 6e65 6410 c808 08d4  eLastOpened.....
+000022e0: 1210 110f 441e 1a1a 5964 6174 6541 6464  ....D...YdateAdd
+000022f0: 6564 0808 d40f 1011 121a 491a 4b08 10d2  ed........I.K...
+00002300: 085a 7368 6172 654f 776e 6572 d40f 1011  .ZshareOwner....
+00002310: 121a 491a 4f08 085f 100f 7368 6172 654c  ..I.O.._..shareL
+00002320: 6173 7445 6469 746f 72d4 0f10 1112 1a49  astEditor......I
+00002330: 1a53 0808 5f10 1069 6e76 6974 6174 696f  .S.._..invitatio
+00002340: 6e53 7461 7475 7308 2340 81b8 0000 0000  nStatus.#@......
+00002350: 0023 4028 0000 0000 0000 2300 0000 0000  .#@(......#.....
+00002360: 0000 0054 6e61 6d65 0910 0100 0800 1d00  ...Tname........
+00002370: 2600 3800 4000 5400 6600 6f00 8100 8c00  &.8.@.T.f.o.....
+00002380: 9f00 b400 bd00 be00 cd00 d600 de00 e400  ................
+00002390: ee00 f900 fa00 fd00 fe01 0301 0c01 1501  ................
+000023a0: 1701 1801 1901 2201 2f01 3101 3201 3301  ......"./.1.2.3.
+000023b0: 3c01 4801 4901 4a01 5301 5801 5a01 5b01  <.H.I.J.S.X.Z.[.
+000023c0: 5c01 6501 6a01 6c01 6d01 6e01 7701 7d01  \.e.j.l.m.n.w.}.
+000023d0: 7f01 8001 8101 8a01 9201 9401 9501 9601  ................
+000023e0: 9f01 a801 ab01 ac01 ad01 b601 c501 c701  ................
+000023f0: c801 c901 d201 dc01 dd01 de01 e701 e801  ................
+00002400: ea01 eb01 f601 ff02 0002 0102 1302 1c02  ................
+00002410: 1d02 1e02 3102 3202 3b02 4402 4d02 5202  ....1.2.;.D.M.R.
+00002420: 5300 0000 0000 0002 0100 0000 0000 0000  S...............
+00002430: 5b00 0000 0000 0000 0000 0000 0000 0002  [...............
+00002440: 5500 0000 0500 6900 6300 6f00 6e00 736c  U.....i.c.o.n.sl
+00002450: 7376 7062 6c6f 6200 0002 a062 706c 6973  svpblob....bplis
+00002460: 7430 30da 0102 0304 0506 0708 090a 0b0c  t00.............
+00002470: 0d1c 4849 4a4b 0c37 5869 636f 6e53 697a  ..HIJK.7XiconSiz
+00002480: 655f 100f 7368 6f77 4963 6f6e 5072 6576  e_..showIconPrev
+00002490: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
+000024a0: 6c63 756c 6174 6541 6c6c 5369 7a65 735f  lculateAllSizes_
+000024b0: 100f 7363 726f 6c6c 506f 7369 7469 6f6e  ..scrollPosition
+000024c0: 5958 7465 7874 5369 7a65 5f10 0f73 6372  YXtextSize_..scr
+000024d0: 6f6c 6c50 6f73 6974 696f 6e58 5a73 6f72  ollPositionXZsor
+000024e0: 7443 6f6c 756d 6e5f 1010 7573 6552 656c  tColumn_..useRel
+000024f0: 6174 6976 6544 6174 6573 5f10 1276 6965  ativeDates_..vie
+00002500: 774f 7074 696f 6e73 5665 7273 696f 6e23  wOptionsVersion#
+00002510: 4030 0000 0000 0000 09d9 0e0f 1011 1213  @0..............
+00002520: 1415 1617 2025 2a2f 3438 3d42 5863 6f6d  .... %*/48=BXcom
+00002530: 6d65 6e74 7355 6c61 6265 6c57 7665 7273  mentsUlabelWvers
+00002540: 696f 6e5b 6461 7465 4372 6561 7465 6454  ion[dateCreatedT
+00002550: 7369 7a65 5c64 6174 654d 6f64 6966 6965  size\dateModifie
+00002560: 6454 6b69 6e64 546e 616d 655e 6461 7465  dTkindTname^date
+00002570: 4c61 7374 4f70 656e 6564 d418 191a 1b1c  LastOpened......
+00002580: 1d0c 1f57 7669 7369 626c 6555 7769 6474  ...WvisibleUwidt
+00002590: 6859 6173 6365 6e64 696e 6755 696e 6465  hYascendingUinde
+000025a0: 7808 1101 2c09 1007 d418 191a 1b1c 220c  x...,.........".
+000025b0: 2408 1064 0910 05d4 1819 1a1b 1c27 0c29  $..d.........'.)
+000025c0: 0810 4b09 1006 d418 191a 1b1c 2c1c 2e08  ..K.........,...
+000025d0: 10b5 0810 02d4 1819 1a1b 0c31 1c33 0910  ...........1.3..
+000025e0: 6108 1003 d418 191a 1b0c 2c1c 3709 0810  a.........,.7...
+000025f0: 01d4 1819 1a1b 0c3a 0c3c 0910 7309 1004  .......:.<..s...
+00002600: d41b 191a 183e 3f0c 0c10 0011 0160 0909  .....>?......`..
+00002610: d418 191a 1b1c 441c 4608 10c8 0810 0808  ......D.F.......
+00002620: 2340 81b8 0000 0000 0023 4028 0000 0000  #@.......#@(....
+00002630: 0000 2300 0000 0000 0000 0054 6e61 6d65  ..#........Tname
+00002640: 0900 0800 1d00 2600 3800 4000 5400 6600  ......&.8.@.T.f.
+00002650: 6f00 8100 8c00 9f00 b400 bd00 be00 d100  o...............
+00002660: da00 e000 e800 f400 f901 0601 0b01 1001  ................
+00002670: 1f01 2801 3001 3601 4001 4601 4701 4a01  ..(.0.6.@.F.G.J.
+00002680: 4b01 4d01 5601 5701 5901 5a01 5c01 6501  K.M.V.W.Y.Z.\.e.
+00002690: 6601 6801 6901 6b01 7401 7501 7701 7801  f.h.i.k.t.u.w.x.
+000026a0: 7a01 8301 8401 8601 8701 8901 9201 9301  z...............
+000026b0: 9401 9601 9f01 a001 a201 a301 a501 ae01  ................
+000026c0: b001 b301 b401 b501 be01 bf01 c101 c201  ................
+000026d0: c401 c501 ce01 d701 e001 e500 0000 0000  ................
+000026e0: 0002 0100 0000 0000 0000 4d00 0000 0000  ..........M.....
+000026f0: 0000 0000 0000 0000 0001 e600 0000 0500  ................
+00002700: 6900 6300 6f00 6e00 736d 6f44 4462 6c6f  i.c.o.n.smoDDblo
+00002710: 6200 0000 08dc 0545 af18 fac4 4100 0000  b......E....A...
+00002720: 0500 6900 6300 6f00 6e00 736d 6f64 4462  ..i.c.o.n.smodDb
+00002730: 6c6f 6200 0000 08dc 0545 af18 fac4 4100  lob......E....A.
+00002740: 0000 0500 6900 6300 6f00 6e00 7370 6831  ....i.c.o.n.sph1
+00002750: 5363 6f6d 7000 0000 0000 0810 0000 0000  Scomp...........
+00002760: 0500 6900 6300 6f00 6e00 7376 5372 6e6c  ..i.c.o.n.svSrnl
+00002770: 6f6e 6700 0000 0100 0000 0300 6900 6d00  ong.........i.m.
+00002780: 6762 7773 7062 6c6f 6200 0000 b862 706c  gbwspblob....bpl
+00002790: 6973 7430 30d6 0102 0304 0506 0708 0708  ist00...........
+000027a0: 0b08 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
+000027b0: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
+000027c0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
+000027d0: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
+000027e0: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
+000027f0: 7753 6964 6562 6172 0809 0809 5f10 187b  wSidebar...._..{
+00002800: 7b33 3335 2c20 3139 387d 2c20 7b39 3237  {335, 198}, {927
+00002810: 2c20 3536 387d 7d09 0815 232f 3b52 5f6b  , 568}}...#/;R_k
+00002820: 6c6d 6e6f 8a00 0000 0000 0001 0100 0000  lmno............
+00002830: 0000 0000 0d00 0000 0000 0000 0000 0000  ................
+00002840: 0000 0000 8b00 0000 0300 6900 6d00 676c  ..........i.m.gl
+00002850: 6731 5363 6f6d 7000 0000 0000 1110 bf00  g1Scomp.........
+00002860: 0000 0300 6900 6d00 676c 7376 4362 6c6f  ....i.m.glsvCblo
+00002870: 6200 0002 b062 706c 6973 7430 30da 0102  b....bplist00...
+00002880: 0304 0506 0708 090a 0b0b 0d18 4849 484a  ............HIHJ
+00002890: 4b4c 5f10 1075 7365 5265 6c61 7469 7665  KL_..useRelative
+000028a0: 4461 7465 735f 100f 7368 6f77 4963 6f6e  Dates_..showIcon
+000028b0: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
+000028c0: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
+000028d0: 7a65 735f 100f 7363 726f 6c6c 506f 7369  zes_..scrollPosi
+000028e0: 7469 6f6e 5958 7465 7874 5369 7a65 5f10  tionYXtextSize_.
+000028f0: 0f73 6372 6f6c 6c50 6f73 6974 696f 6e58  .scrollPositionX
+00002900: 5a73 6f72 7443 6f6c 756d 6e58 6963 6f6e  ZsortColumnXicon
+00002910: 5369 7a65 5f10 1276 6965 774f 7074 696f  Size_..viewOptio
+00002920: 6e73 5665 7273 696f 6e09 09ab 0e17 1c21  nsVersion......!
+00002930: 252a 2f34 393e 43d4 0f10 1112 0b14 0b16  %*/49>C.........
+00002940: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
+00002950: 7363 656e 6469 6e67 5a69 6465 6e74 6966  scendingZidentif
+00002960: 6965 7209 1101 c709 546e 616d 65d4 0f10  ier.....Tname...
+00002970: 1112 1819 181b 0810 2308 5875 6269 7175  ........#.Xubiqu
+00002980: 6974 79d4 0f10 1112 0b1e 1820 0910 b508  ity........ ....
+00002990: 5c64 6174 654d 6f64 6966 6965 64d4 0f10  \dateModified...
+000029a0: 1112 181e 1824 0808 5b64 6174 6543 7265  .....$..[dateCre
+000029b0: 6174 6564 d40f 1011 120b 2718 2909 1061  ated......'.)..a
+000029c0: 0854 7369 7a65 d40f 1011 120b 2c0b 2e09  .Tsize......,...
+000029d0: 1073 0954 6b69 6e64 d40f 1011 1218 310b  .s.Tkind......1.
+000029e0: 3308 1064 0955 6c61 6265 6cd4 0f10 1112  3..d.Ulabel.....
+000029f0: 1836 0b38 0810 4b09 5776 6572 7369 6f6e  .6.8..K.Wversion
+00002a00: d40f 1011 1218 3b0b 3d08 1101 2c09 5863  ......;.=...,.Xc
+00002a10: 6f6d 6d65 6e74 73d4 0f10 1112 1840 1842  omments......@.B
+00002a20: 0810 c808 5e64 6174 654c 6173 744f 7065  ....^dateLastOpe
+00002a30: 6e65 64d4 0f10 1112 181e 1846 0808 5964  ned........F..Yd
+00002a40: 6174 6541 6464 6564 0823 0000 0000 0000  ateAdded.#......
+00002a50: 0000 2340 2800 0000 0000 0054 6e61 6d65  ..#@(......Tname
+00002a60: 2340 3000 0000 0000 0010 0100 0800 1d00  #@0.............
+00002a70: 3000 4200 4a00 5e00 7000 7900 8b00 9600  0.B.J.^.p.y.....
+00002a80: 9f00 b400 b500 b600 c200 cb00 d300 d900  ................
+00002a90: e300 ee00 ef00 f200 f300 f801 0101 0201  ................
+00002aa0: 0401 0501 0e01 1701 1801 1a01 1b01 2801  ..............(.
+00002ab0: 3101 3201 3301 3f01 4801 4901 4b01 4c01  1.2.3.?.H.I.K.L.
+00002ac0: 5101 5a01 5b01 5d01 5e01 6301 6c01 6d01  Q.Z.[.].^.c.l.m.
+00002ad0: 6f01 7001 7601 7f01 8001 8201 8301 8b01  o.p.v...........
+00002ae0: 9401 9501 9801 9901 a201 ab01 ac01 ae01  ................
+00002af0: af01 be01 c701 c801 c901 d301 d401 dd01  ................
+00002b00: e601 eb01 f400 0000 0000 0002 0100 0000  ................
+00002b10: 0000 0000 4d00 0000 0000 0000 0000 0000  ....M...........
+00002b20: 0000 0001 f600 0000 0300 6900 6d00 676c  ..........i.m.gl
+00002b30: 7376 7062 6c6f 6200 0002 9562 706c 6973  svpblob....bplis
+00002b40: 7430 30da 0102 0304 0506 0708 090a 0b0b  t00.............
+00002b50: 0d1f 4849 484a 4b26 5f10 1075 7365 5265  ..HIHJK&_..useRe
+00002b60: 6c61 7469 7665 4461 7465 735f 100f 7368  lativeDates_..sh
+00002b70: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
+00002b80: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
+00002b90: 6541 6c6c 5369 7a65 735f 100f 7363 726f  eAllSizes_..scro
+00002ba0: 6c6c 506f 7369 7469 6f6e 5958 7465 7874  llPositionYXtext
+00002bb0: 5369 7a65 5f10 0f73 6372 6f6c 6c50 6f73  Size_..scrollPos
+00002bc0: 6974 696f 6e58 5a73 6f72 7443 6f6c 756d  itionXZsortColum
+00002bd0: 6e58 6963 6f6e 5369 7a65 5f10 1276 6965  nXiconSize_..vie
+00002be0: 774f 7074 696f 6e73 5665 7273 696f 6e09  wOptionsVersion.
+00002bf0: 09d9 0e0f 1011 1213 1415 1617 2025 2a2e  ............ %*.
+00002c00: 3338 3d42 5863 6f6d 6d65 6e74 735e 6461  38=BXcomments^da
+00002c10: 7465 4c61 7374 4f70 656e 6564 5c64 6174  teLastOpened\dat
+00002c20: 654d 6f64 6966 6965 645b 6461 7465 4372  eModified[dateCr
+00002c30: 6561 7465 6454 7369 7a65 556c 6162 656c  eatedTsizeUlabel
+00002c40: 546b 696e 6457 7665 7273 696f 6e54 6e61  TkindWversionTna
+00002c50: 6d65 d418 191a 1b1c 1d0b 1f55 696e 6465  me.........Uinde
+00002c60: 7855 7769 6474 6859 6173 6365 6e64 696e  xUwidthYascendin
+00002c70: 6757 7669 7369 626c 6510 0711 012c 0908  gWvisible....,..
+00002c80: d418 191a 1b21 221f 1f10 0810 c808 08d4  .....!".........
+00002c90: 1819 1a1b 2627 1f0b 1001 10b5 0809 d418  ....&'..........
+00002ca0: 191a 1b2b 271f 1f10 0208 08d4 1819 1a1b  ...+'...........
+00002cb0: 2f30 1f0b 1003 1061 0809 d418 191a 1b34  /0.....a.......4
+00002cc0: 350b 1f10 0510 6409 08d4 1819 1a1b 393a  5.....d.......9:
+00002cd0: 0b0b 1004 1073 0909 d418 191a 1b3e 3f0b  .....s.......>?.
+00002ce0: 1f10 0610 4b09 08d4 1819 1a1b 4344 0b0b  ....K.......CD..
+00002cf0: 1000 1101 c709 0908 2300 0000 0000 0000  ........#.......
+00002d00: 0023 4028 0000 0000 0000 546e 616d 6523  .#@(......Tname#
+00002d10: 4030 0000 0000 0000 0008 001d 0030 0042  @0...........0.B
+00002d20: 004a 005e 0070 0079 008b 0096 009f 00b4  .J.^.p.y........
+00002d30: 00b5 00b6 00c9 00d2 00e1 00ee 00fa 00ff  ................
+00002d40: 0105 010a 0112 0117 0120 0126 012c 0136  ......... .&.,.6
+00002d50: 013e 0140 0143 0144 0145 014e 0150 0152  .>.@.C.D.E.N.P.R
+00002d60: 0153 0154 015d 015f 0161 0162 0163 016c  .S.T.]._.a.b.c.l
+00002d70: 016e 016f 0170 0179 017b 017d 017e 017f  .n.o.p.y.{.}.~..
+00002d80: 0188 018a 018c 018d 018e 0197 0199 019b  ................
+00002d90: 019c 019d 01a6 01a8 01aa 01ab 01ac 01b5  ................
+00002da0: 01b7 01ba 01bb 01bc 01bd 01c6 01cf 01d4  ................
+00002db0: 0000 0000 0000 0201 0000 0000 0000 004c  ...............L
+00002dc0: 0000 0000 0000 0000 0000 0000 0000 01dd  ................
+00002dd0: 0000 0003 0069 006d 0067 6d6f 4444 626c  .....i.m.gmoDDbl
+00002de0: 6f62 0000 0008 4551 1b75 c60b c541 0000  ob....EQ.u...A..
+00002df0: 0003 0069 006d 0067 6d6f 6444 626c 6f62  ...i.m.gmodDblob
+00002e00: 0000 0008 4551 1b75 c60b c541 0000 0003  ....EQ.u...A....
+00002e10: 0069 006d 0067 7068 3153 636f 6d70 0000  .i.m.gph1Scomp..
+00002e20: 0000 0011 3000 0000 0003 0069 006d 0067  ....0......i.m.g
+00002e30: 7653 726e 6c6f 6e67 0000 0001 0000 0007  vSrnlong........
+00002e40: 006c 006f 006f 006b 0075 0070 0073 6277  .l.o.o.k.u.p.sbw
+00002e50: 7370 626c 6f62 0000 00c8 6270 6c69 7374  spblob....bplist
+00002e60: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
+00002e70: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+00002e80: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
+00002e90: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+00002ea0: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+00002eb0: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+00002ec0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+00002ed0: 6261 7208 0809 0809 5f10 177b 7b32 302c  bar....._..{{20,
+00002ee0: 2039 307d 2c20 7b31 3031 352c 2037 3637   90}, {1015, 767
+00002ef0: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
+00002f00: 7e98 0000 0000 0000 0101 0000 0000 0000  ~...............
+00002f10: 000f 0000 0000 0000 0000 0000 0000 0000  ................
+00002f20: 0099 0000 0007 006c 006f 006f 006b 0075  .......l.o.o.k.u
+00002f30: 0070 0073 6c67 3153 636f 6d70 0000 0000  .p.slg1Scomp....
+00002f40: 0004 b42c 0000 0000 0000 0000 0000 0000  ...,............
 00002f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -845,60 +845,60 @@
 000034c0: 1801 1e01 1f01 2201 2301 2501 2e01 2f01  ......".#.%.../.
 000034d0: 3101 3201 3401 3d01 3e01 4001 4101 4301  1.2.4.=.>.@.A.C.
 000034e0: 4c01 4d01 4e01 5001 5901 5a01 5c01 5d01  L.M.N.P.Y.Z.\.].
 000034f0: 5f01 6801 6901 6b01 6c01 6e01 7701 7801  _.h.i.k.l.n.w.x.
 00003500: 7a01 7b01 7d01 8601 8701 8901 8a01 8c01  z.{.}...........
 00003510: 9501 9601 9901 9a01 9c01 9d01 a601 ab00  ................
 00003520: 0000 0000 0002 0100 0000 0000 0000 4900  ..............I.
-00003530: 0000 0000 0000 0000 0000 0000 0001 ac43  ...............C
-00003540: 7265 6174 6564 0808 d40d 0e0f 1024 2518  reated.......$%.
-00003550: 0a54 7369 7a65 1061 0809 d40d 0e0f 1029  .Tsize.a.......)
-00003560: 2a0a 0a54 6b69 6e64 1073 0909 d40d 0e0f  *..Tkind.s......
-00003570: 102e 2f0a 1855 6c61 6265 6c10 6409 08d4  ../..Ulabel.d...
-00003580: 0d0e 0f10 3334 0a18 5776 6572 7369 6f6e  ....34..Wversion
-00003590: 104b 0908 d40d 0e0f 1038 390a 1858 636f  .K.......89..Xco
-000035a0: 6d6d 656e 7473 1101 2c09 08d4 0d0e 0f10  mments..,.......
-000035b0: 3d3e 1818 5e64 6174 654c 6173 744f 7065  =>..^dateLastOpe
-000035c0: 6e65 6410 c808 08d4 0d0e 0f10 421c 1818  ned.........B...
-000035d0: 5964 6174 6541 6464 6564 0808 0823 4028  YdateAdded...#@(
-000035e0: 0000 0000 0000 546e 616d 6509 1001 0008  ......Tname.....
-000035f0: 0019 0022 0034 003c 0050 0059 0064 0077  ...".4.<.P.Y.d.w
-00003600: 008c 0095 0096 00a2 00ab 00b6 00bc 00c6  ................
-00003610: 00ce 00d3 00d6 00d7 00d8 00e1 00ea 00ec  ................
-00003620: 00ed 00ee 00f7 0104 0106 0107 0108 0111  ................
-00003630: 011d 011e 011f 0128 012d 012f 0130 0131  .......(.-./.0.1
-00003640: 013a 013f 0141 0142 0143 014c 0152 0154  .:.?.A.B.C.L.R.T
-00003650: 0155 0156 015f 0167 0169 016a 016b 0174  .U.V._.g.i.j.k.t
-00003660: 017d 0180 0181 0182 018b 019a 019c 019d  .}..............
-00003670: 019e 01a7 01b1 01b2 01b3 01b4 01bd 01c2  ................
-00003680: 01c3 0000 0000 0000 0201 0000 0000 0000  ................
-00003690: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
-000036a0: 01c5 0063 006f 006e 0073 6d6f 4444 626c  ...c.o.n.smoDDbl
-000036b0: 6f62 0000 0008 dc05 45af 18fa c441 0000  ob......E....A..
-000036c0: 0005 0069 0063 006f 006e 0073 6d6f 6444  ...i.c.o.n.smodD
-000036d0: 626c 6f62 0000 0008 dc05 45af 18fa c441  blob......E....A
-000036e0: 0000 0005 0069 0063 006f 006e 0073 7068  .....i.c.o.n.sph
-000036f0: 3153 636f 6d70 0000 0000 0008 1000 0000  1Scomp..........
-00003700: 0005 0069 0063 006f 006e 0073 7653 726e  ...i.c.o.n.svSrn
-00003710: 6c6f 6e67 0000 0001 0000 0003 0069 006d  long.........i.m
-00003720: 0067 6277 7370 626c 6f62 0000 00c9 6270  .gbwspblob....bp
-00003730: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
-00003740: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
-00003750: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
-00003760: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
-00003770: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-00003780: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-00003790: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-000037a0: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
-000037b0: 7b31 3132 2c20 3535 7d2c 207b 3131 3939  {112, 55}, {1199
-000037c0: 2c20 3736 397d 7d09 0817 2531 3d49 606d  , 769}}...%1=I`m
-000037d0: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
-000037e0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
-000037f0: 0000 0000 0000 9a00 0000 0300 6900 6d00  ............i.m.
-00003800: 676c 6731 0000 0006 0000 0000 0000 380b  glg1..........8.
+00003530: 0000 0000 0000 0000 0000 0000 0001 ac18  ................
+00003540: 0a54 7369 7a65 1061 0809 d40d 0e0f 1029  .Tsize.a.......)
+00003550: 2a0a 0a54 6b69 6e64 1073 0909 d40d 0e0f  *..Tkind.s......
+00003560: 102e 2f0a 1855 6c61 6265 6c10 6409 08d4  ../..Ulabel.d...
+00003570: 0d0e 0f10 3334 0a18 5776 6572 7369 6f6e  ....34..Wversion
+00003580: 104b 0908 d40d 0e0f 1038 390a 1858 636f  .K.......89..Xco
+00003590: 6d6d 656e 7473 1101 2c09 08d4 0d0e 0f10  mments..,.......
+000035a0: 3d3e 1818 5e64 6174 654c 6173 744f 7065  =>..^dateLastOpe
+000035b0: 6e65 6410 c808 08d4 0d0e 0f10 421c 1818  ned.........B...
+000035c0: 5964 6174 6541 6464 6564 0808 0823 4028  YdateAdded...#@(
+000035d0: 0000 0000 0000 546e 616d 6509 1001 0008  ......Tname.....
+000035e0: 0019 0022 0034 003c 0050 0059 0064 0077  ...".4.<.P.Y.d.w
+000035f0: 008c 0095 0096 00a2 00ab 00b6 00bc 00c6  ................
+00003600: 00ce 00d3 00d6 00d7 00d8 00e1 00ea 00ec  ................
+00003610: 00ed 00ee 00f7 0104 0106 0107 0108 0111  ................
+00003620: 011d 011e 011f 0128 012d 012f 0130 0131  .......(.-./.0.1
+00003630: 013a 013f 0141 0142 0143 014c 0152 0154  .:.?.A.B.C.L.R.T
+00003640: 0155 0156 015f 0167 0169 016a 016b 0174  .U.V._.g.i.j.k.t
+00003650: 017d 0180 0181 0182 018b 019a 019c 019d  .}..............
+00003660: 019e 01a7 01b1 01b2 01b3 01b4 01bd 01c2  ................
+00003670: 01c3 0000 0000 0000 0201 0000 0000 0000  ................
+00003680: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
+00003690: 01c5 6801 6901 6b01 7401 7501 7701 7801  ..h.i.k.t.u.w.x.
+000036a0: 7a01 8301 8401 8601 8701 8901 9201 9301  z...............
+000036b0: 9401 9601 9f01 a001 a201 a301 a501 ae01  ................
+000036c0: b001 b301 b401 b501 be01 bf01 c101 c201  ................
+000036d0: c401 c501 ce01 d701 e001 e500 0000 0000  ................
+000036e0: 0002 0100 0000 0000 0000 4d00 0000 0000  ..........M.....
+000036f0: 0000 0000 0000 0000 0001 e600 0000 0500  ................
+00003700: 6900 6300 6f00 6e00 736d 6f44 4462 6c6f  i.c.o.n.smoDDblo
+00003710: 6200 0000 08dc 0545 af18 fac4 4100 0000  b......E....A...
+00003720: 0500 6900 6300 6f00 6e00 736d 6f64 4462  ..i.c.o.n.smodDb
+00003730: 6c6f 6200 0000 08dc 0545 af18 fac4 4100  lob......E....A.
+00003740: 0000 0500 6900 6300 6f00 6e00 7370 6831  ....i.c.o.n.sph1
+00003750: 5363 6f6d 7000 0000 0000 0810 0000 0000  Scomp...........
+00003760: 0500 6900 6300 6f00 6e00 7376 5372 6e6c  ..i.c.o.n.svSrnl
+00003770: 6f6e 6700 0000 0100 0000 0300 6900 6d00  ong.........i.m.
+00003780: 6762 7773 7062 6c6f 6200 0000 b862 706c  gbwspblob....bpl
+00003790: 6973 7430 30d6 0102 0304 0506 0708 0708  ist00...........
+000037a0: 0b08 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
+000037b0: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
+000037c0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
+000037d0: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
+000037e0: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
+000037f0: 7753 6964 6562 6172 0809 0809 5f10 187b  wSidebar...._..{
+00003800: 7b33 3335 0000 0006 0000 0000 0000 380b  {335..........8.
 00003810: 0000 0045 0000 100b 0000 300b 0000 200c  ...E......0... .
 00003820: 0000 180b 0000 0000 0000 0000 0000 0000  ................
 00003830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -973,53 +973,53 @@
 00003cc0: 0101 0000 0000 0000 0102 0000 0000 0000  ................
 00003cd0: 0104 0000 0000 0000 0108 0000 0000 0000  ................
 00003ce0: 0110 0000 0000 0000 0120 0000 0000 0000  ......... ......
 00003cf0: 0140 0000 0000 0000 0001 6e01 7701 7801  .@........n.w.x.
 00003d00: 7a01 7b01 7d01 8601 8701 8901 8a01 8c01  z.{.}...........
 00003d10: 9501 9601 9901 9a01 9c01 9d01 a601 ab00  ................
 00003d20: 0000 0000 0002 0100 0000 0000 0000 4900  ..............I.
-00003d30: 0000 0000 0000 0000 0000 0000 0001 ac43  ...............C
-00003d40: 7265 6174 6564 0808 d40d 0e0f 1024 2518  reated.......$%.
-00003d50: 0a54 7369 7a65 1061 0809 d40d 0e0f 1029  .Tsize.a.......)
-00003d60: 2a0a 0a54 6b69 6e64 1073 0909 d40d 0e0f  *..Tkind.s......
-00003d70: 102e 2f0a 1855 6c61 6265 6c10 6409 08d4  ../..Ulabel.d...
-00003d80: 0d0e 0f10 3334 0a18 5776 6572 7369 6f6e  ....34..Wversion
-00003d90: 104b 0908 d40d 0e0f 1038 390a 1858 636f  .K.......89..Xco
-00003da0: 6d6d 656e 7473 1101 2c09 08d4 0d0e 0f10  mments..,.......
-00003db0: 3d3e 1818 5e64 6174 654c 6173 744f 7065  =>..^dateLastOpe
-00003dc0: 6e65 6410 c808 08d4 0d0e 0f10 421c 1818  ned.........B...
-00003dd0: 5964 6174 6541 6464 6564 0808 0823 4028  YdateAdded...#@(
-00003de0: 0000 0000 0000 546e 616d 6509 1001 0008  ......Tname.....
-00003df0: 0019 0022 0034 003c 0050 0059 0064 0077  ...".4.<.P.Y.d.w
-00003e00: 008c 0095 0096 00a2 00ab 00b6 00bc 00c6  ................
-00003e10: 00ce 00d3 00d6 00d7 00d8 00e1 00ea 00ec  ................
-00003e20: 00ed 00ee 00f7 0104 0106 0107 0108 0111  ................
-00003e30: 011d 011e 011f 0128 012d 012f 0130 0131  .......(.-./.0.1
-00003e40: 013a 013f 0141 0142 0143 014c 0152 0154  .:.?.A.B.C.L.R.T
-00003e50: 0155 0156 015f 0167 0169 016a 016b 0174  .U.V._.g.i.j.k.t
-00003e60: 017d 0180 0181 0182 018b 019a 019c 019d  .}..............
-00003e70: 019e 01a7 01b1 01b2 01b3 01b4 01bd 01c2  ................
-00003e80: 01c3 0000 0000 0000 0201 0000 0000 0000  ................
-00003e90: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
-00003ea0: 01c5 0063 006f 006e 0073 6d6f 4444 626c  ...c.o.n.smoDDbl
-00003eb0: 6f62 0000 0008 dc05 45af 18fa c441 0000  ob......E....A..
-00003ec0: 0005 0069 0063 006f 006e 0073 6d6f 6444  ...i.c.o.n.smodD
-00003ed0: 626c 6f62 0000 0008 dc05 45af 18fa c441  blob......E....A
-00003ee0: 0000 0005 0069 0063 006f 006e 0073 7068  .....i.c.o.n.sph
-00003ef0: 3153 636f 6d70 0000 0000 0008 1000 0000  1Scomp..........
-00003f00: 0005 0069 0063 006f 006e 0073 7653 726e  ...i.c.o.n.svSrn
-00003f10: 6c6f 6e67 0000 0001 0000 0003 0069 006d  long.........i.m
-00003f20: 0067 6277 7370 626c 6f62 0000 00c9 6270  .gbwspblob....bp
-00003f30: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
-00003f40: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
-00003f50: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
-00003f60: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
-00003f70: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-00003f80: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-00003f90: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-00003fa0: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
-00003fb0: 7b31 3132 2c20 3535 7d2c 207b 3131 3939  {112, 55}, {1199
-00003fc0: 2c20 3736 397d 7d09 0817 2531 3d49 606d  , 769}}...%1=I`m
-00003fd0: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
-00003fe0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
-00003ff0: 0000 0000 0000 9a00 0000 0300 6900 6d00  ............i.m.
-00004000: 676c 6731                                glg1
+00003d30: 0000 0000 0000 0000 0000 0000 0001 ac18  ................
+00003d40: 0a54 7369 7a65 1061 0809 d40d 0e0f 1029  .Tsize.a.......)
+00003d50: 2a0a 0a54 6b69 6e64 1073 0909 d40d 0e0f  *..Tkind.s......
+00003d60: 102e 2f0a 1855 6c61 6265 6c10 6409 08d4  ../..Ulabel.d...
+00003d70: 0d0e 0f10 3334 0a18 5776 6572 7369 6f6e  ....34..Wversion
+00003d80: 104b 0908 d40d 0e0f 1038 390a 1858 636f  .K.......89..Xco
+00003d90: 6d6d 656e 7473 1101 2c09 08d4 0d0e 0f10  mments..,.......
+00003da0: 3d3e 1818 5e64 6174 654c 6173 744f 7065  =>..^dateLastOpe
+00003db0: 6e65 6410 c808 08d4 0d0e 0f10 421c 1818  ned.........B...
+00003dc0: 5964 6174 6541 6464 6564 0808 0823 4028  YdateAdded...#@(
+00003dd0: 0000 0000 0000 546e 616d 6509 1001 0008  ......Tname.....
+00003de0: 0019 0022 0034 003c 0050 0059 0064 0077  ...".4.<.P.Y.d.w
+00003df0: 008c 0095 0096 00a2 00ab 00b6 00bc 00c6  ................
+00003e00: 00ce 00d3 00d6 00d7 00d8 00e1 00ea 00ec  ................
+00003e10: 00ed 00ee 00f7 0104 0106 0107 0108 0111  ................
+00003e20: 011d 011e 011f 0128 012d 012f 0130 0131  .......(.-./.0.1
+00003e30: 013a 013f 0141 0142 0143 014c 0152 0154  .:.?.A.B.C.L.R.T
+00003e40: 0155 0156 015f 0167 0169 016a 016b 0174  .U.V._.g.i.j.k.t
+00003e50: 017d 0180 0181 0182 018b 019a 019c 019d  .}..............
+00003e60: 019e 01a7 01b1 01b2 01b3 01b4 01bd 01c2  ................
+00003e70: 01c3 0000 0000 0000 0201 0000 0000 0000  ................
+00003e80: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
+00003e90: 01c5 6801 6901 6b01 7401 7501 7701 7801  ..h.i.k.t.u.w.x.
+00003ea0: 7a01 8301 8401 8601 8701 8901 9201 9301  z...............
+00003eb0: 9401 9601 9f01 a001 a201 a301 a501 ae01  ................
+00003ec0: b001 b301 b401 b501 be01 bf01 c101 c201  ................
+00003ed0: c401 c501 ce01 d701 e001 e500 0000 0000  ................
+00003ee0: 0002 0100 0000 0000 0000 4d00 0000 0000  ..........M.....
+00003ef0: 0000 0000 0000 0000 0001 e600 0000 0500  ................
+00003f00: 6900 6300 6f00 6e00 736d 6f44 4462 6c6f  i.c.o.n.smoDDblo
+00003f10: 6200 0000 08dc 0545 af18 fac4 4100 0000  b......E....A...
+00003f20: 0500 6900 6300 6f00 6e00 736d 6f64 4462  ..i.c.o.n.smodDb
+00003f30: 6c6f 6200 0000 08dc 0545 af18 fac4 4100  lob......E....A.
+00003f40: 0000 0500 6900 6300 6f00 6e00 7370 6831  ....i.c.o.n.sph1
+00003f50: 5363 6f6d 7000 0000 0000 0810 0000 0000  Scomp...........
+00003f60: 0500 6900 6300 6f00 6e00 7376 5372 6e6c  ..i.c.o.n.svSrnl
+00003f70: 6f6e 6700 0000 0100 0000 0300 6900 6d00  ong.........i.m.
+00003f80: 6762 7773 7062 6c6f 6200 0000 b862 706c  gbwspblob....bpl
+00003f90: 6973 7430 30d6 0102 0304 0506 0708 0708  ist00...........
+00003fa0: 0b08 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
+00003fb0: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
+00003fc0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
+00003fd0: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
+00003fe0: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
+00003ff0: 7753 6964 6562 6172 0809 0809 5f10 187b  wSidebar...._..{
+00004000: 7b33 3335                                {335
```

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.63.2/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.63.2/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.63.2/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.63.2/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.63.2/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.63.2/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.63.2/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.63.2/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.63.2/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.63.2/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.63.2/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.63.2/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.63.2/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.63.2/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.63.2/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.63.1
+Version: 1.63.2
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.63.1/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.63.2/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,17 @@
 simba/cue_light_tools/cue_light_clf_statistics.py
 simba/cue_light_tools/cue_light_menues.py
 simba/cue_light_tools/cue_light_movement_statistics.py
 simba/cue_light_tools/cue_light_tools.py
 simba/cue_light_tools/cue_light_visualizer.py
 simba/dash_app/SimBA_dash_app.py
 simba/dash_app/dash_app.py
+simba/dash_app/plotly_dash.py
 simba/dash_app/run_dash_tkinter.py
+simba/data_processors/.DS_Store
 simba/data_processors/__init__.py
 simba/data_processors/agg_clf_calculator.py
 simba/data_processors/directing_other_animals_calculator.py
 simba/data_processors/fsttc_calculator.py
 simba/data_processors/interpolate_pose.py
 simba/data_processors/interpolation_smoothing.py
 simba/data_processors/kleinberg_calculator.py
@@ -313,14 +315,15 @@
 simba/pose_importers/read_DANNCE_mat.py
 simba/pose_importers/sleap_csv_importer.py
 simba/pose_importers/sleap_h5_importer.py
 simba/pose_importers/sleap_slp_importer.py
 simba/pose_importers/trk_importer.py
 simba/pose_importers/misc/.DS_Store
 simba/pose_importers/misc/apt_trk_importer.py
+simba/pose_processors/.DS_Store
 simba/pose_processors/__init__.py
 simba/pose_processors/pose_reset.py
 simba/pose_processors/remove_keypoints.py
 simba/pose_processors/reorganize_keypoint.py
 simba/pose_processors/reverse_pose.py
 simba/roi_tools/.DS_Store
 simba/roi_tools/ROI_analyzer.py
@@ -334,14 +337,21 @@
 simba/roi_tools/ROI_movement_analyzer.py
 simba/roi_tools/ROI_multiply.py
 simba/roi_tools/ROI_reset.py
 simba/roi_tools/ROI_size_calculations.py
 simba/roi_tools/ROI_time_bin_calculator.py
 simba/roi_tools/ROI_zoom.py
 simba/roi_tools/__init__.py
+simba/st/__init__.py
+simba/st/aggregate_statistics.py
+simba/st/app.py
+simba/st/enums.py
+simba/st/select_groups_pg.py
+simba/st/welcome_page.py
+simba/third_party_label_appenders/.DS_Store
 simba/third_party_label_appenders/BENTO_appender.py
 simba/third_party_label_appenders/BORIS_appender.py
 simba/third_party_label_appenders/__init__.py
 simba/third_party_label_appenders/deepethogram_importer.py
 simba/third_party_label_appenders/ethovision_import.py
 simba/third_party_label_appenders/observer_importer.py
 simba/third_party_label_appenders/solomon_importer.py
```

### Comparing `Simba-UW-tf-dev-1.63.1/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.63.2/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/LICENSE.md` & `Simba-UW-tf-dev-1.63.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.63.2/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/tests/test_distance_plotter.py` & `Simba-UW-tf-dev-1.63.2/tests/test_distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/tests/test_train_model_mixin.py` & `Simba-UW-tf-dev-1.63.2/tests/test_train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/tests/test_pose_importers.py` & `Simba-UW-tf-dev-1.63.2/tests/test_pose_importers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/tests/test_feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.63.2/tests/test_feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/tests/test_utils_data.py` & `Simba-UW-tf-dev-1.63.2/tests/test_utils_data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/tests/test_config_reader_mixin.py` & `Simba-UW-tf-dev-1.63.2/tests/test_config_reader_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.63.2/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/tests/test_visualize_directing_animals.py` & `Simba-UW-tf-dev-1.63.2/tests/test_visualize_directing_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.63.2/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/tests/test_video_processors.py` & `Simba-UW-tf-dev-1.63.2/tests/test_video_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py` & `Simba-UW-tf-dev-1.63.2/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.63.2/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/tests/test_validation_clips.py` & `Simba-UW-tf-dev-1.63.2/tests/test_validation_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/tests/test_roi_tools.py` & `Simba-UW-tf-dev-1.63.2/tests/test_roi_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/README.md` & `Simba-UW-tf-dev-1.63.2/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.1/setup.py` & `Simba-UW-tf-dev-1.63.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.63.1",
+    version="1.63.2",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

