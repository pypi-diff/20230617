# Comparing `tmp/joes_giant_toolbox-0.2.23.tar.gz` & `tmp/joes_giant_toolbox-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joes_giant_toolbox-0.2.23.tar", last modified: Sat May  6 11:35:23 2023, max compression
+gzip compressed data, was "joes_giant_toolbox-0.3.1.tar", last modified: Sat Jun 17 20:54:24 2023, max compression
```

## Comparing `joes_giant_toolbox-0.2.23.tar` & `joes_giant_toolbox-0.3.1.tar`

### file list

```diff
@@ -1,66 +1,69 @@
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-06 11:35:23.535082 joes_giant_toolbox-0.2.23/
--rw-r--r--   0 josephbolton   (501) staff       (20)    35149 2023-03-02 13:11:21.000000 joes_giant_toolbox-0.2.23/LICENSE
--rw-r--r--   0 josephbolton   (501) staff       (20)    59255 2023-05-06 11:35:23.534823 joes_giant_toolbox-0.2.23/PKG-INFO
--rw-r--r--   0 josephbolton   (501) staff       (20)    17973 2023-05-03 09:24:44.000000 joes_giant_toolbox-0.2.23/README.md
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-06 11:35:23.520392 joes_giant_toolbox-0.2.23/joes_giant_toolbox/
--rw-r--r--   0 josephbolton   (501) staff       (20)        0 2023-04-13 17:58:22.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/__init__.py
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-06 11:35:23.530411 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/
--rw-r--r--   0 josephbolton   (501) staff       (20)        0 2023-04-13 17:58:22.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/__init__.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    10700 2023-04-12 10:02:27.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4964 2023-04-17 13:22:54.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/ascii_density_histogram.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     9531 2023-04-30 11:40:27.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/compare_metric_to_prev_period.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      967 2023-03-03 07:53:04.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/conjugate_prior_beta_binomial.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     5416 2023-05-05 09:35:57.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/create_gcloud_vm_docker_template.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4317 2023-04-17 13:55:24.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/create_project_scope_doc.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1727 2023-03-21 12:21:56.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1430 2023-03-20 07:50:22.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    10974 2023-04-06 12:30:49.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/duckduckgo_search_multipage.py
--rw-r--r--   0 josephbolton   (501) staff       (20)        0 2023-05-05 08:14:30.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/gcloud_vm_kills_itself.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2261 2023-04-17 14:00:23.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/list_all_python_imports.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      878 2023-03-20 07:49:14.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/list_files_in_gcloud_bucket.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4736 2023-04-17 14:11:08.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4358 2023-03-03 08:08:14.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/make_url_request.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      376 2023-04-23 20:15:27.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/manual_keyword_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2318 2023-04-19 11:00:23.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1845 2023-04-01 21:15:07.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/print_progress_bar.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2117 2023-04-27 07:33:31.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/python_plotting_tutorials.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      501 2023-03-29 13:35:25.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/query_bigquery_to_pandas_df.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    48271 2023-04-10 13:38:46.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/rapid_binary_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     8677 2023-05-03 12:01:21.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/regex_rules_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4608 2023-03-30 09:37:03.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/run_python_function_in_parallel.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     5776 2023-04-17 12:08:12.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    13751 2023-05-06 11:30:11.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/string_cleaner.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1536 2023-04-13 10:47:28.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2360 2023-03-29 14:15:20.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/url_to_filename_to_url_mapper.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2282 2023-04-17 13:33:49.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/view_nested_dict_structure.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1805 2023-03-21 10:01:14.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/write_pandas_df_to_google_bigquery_table.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      264 2023-04-17 12:16:19.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/convenience.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      413 2023-04-25 07:40:31.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/dataviz.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1300 2023-05-03 07:44:59.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/google_cloud.py
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-06 11:35:23.532483 joes_giant_toolbox-0.2.23/joes_giant_toolbox/in_progress/
--rw-r--r--   0 josephbolton   (501) staff       (20)     2126 2023-04-03 18:18:28.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/in_progress/ascii_barplot.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1108 2023-03-07 09:48:13.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/in_progress/conjugate_prior_normal_normal.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     3563 2023-03-16 08:04:10.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/in_progress/imdb_item_page_scraper.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2088 2023-03-15 19:17:57.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/in_progress/longest_portion_of_phrase_in_search_string.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      446 2023-03-10 07:50:35.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/in_progress/query_wikipedia_api.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1161 2023-04-10 13:40:03.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/in_progress/rapid_bag_of_words_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    47227 2023-04-01 21:12:12.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/in_progress/recsys_data_simulator.py
--rw-r--r--   0 josephbolton   (501) staff       (20)       85 2023-04-17 13:38:24.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/proj_mgmt.py
--rw-r--r--   0 josephbolton   (501) staff       (20)       81 2023-04-17 14:03:06.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/sklearn.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      161 2023-04-26 19:46:54.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/stats.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      450 2023-05-03 07:44:37.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/text.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      515 2023-04-17 12:09:22.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox/web.py
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-06 11:35:23.521451 joes_giant_toolbox-0.2.23/joes_giant_toolbox.egg-info/
--rw-r--r--   0 josephbolton   (501) staff       (20)    59255 2023-05-06 11:35:23.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 josephbolton   (501) staff       (20)     2724 2023-05-06 11:35:23.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 josephbolton   (501) staff       (20)        1 2023-05-06 11:35:23.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 josephbolton   (501) staff       (20)      186 2023-05-06 11:35:23.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox.egg-info/requires.txt
--rw-r--r--   0 josephbolton   (501) staff       (20)       19 2023-05-06 11:35:23.000000 joes_giant_toolbox-0.2.23/joes_giant_toolbox.egg-info/top_level.txt
--rw-r--r--   0 josephbolton   (501) staff       (20)     1085 2023-05-06 11:34:22.000000 joes_giant_toolbox-0.2.23/pyproject.toml
--rw-r--r--   0 josephbolton   (501) staff       (20)       38 2023-05-06 11:35:23.535137 joes_giant_toolbox-0.2.23/setup.cfg
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-05-06 11:35:23.534315 joes_giant_toolbox-0.2.23/tests/
--rw-r--r--   0 josephbolton   (501) staff       (20)      557 2023-04-26 19:48:17.000000 joes_giant_toolbox-0.2.23/tests/test_conjugate_prior_beta_binomial.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      571 2023-04-25 09:26:34.000000 joes_giant_toolbox-0.2.23/tests/test_longest_sentence_subsequence_plagiarism_detector.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2617 2023-04-25 09:27:22.000000 joes_giant_toolbox-0.2.23/tests/test_make_url_request.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     8681 2023-04-25 09:28:50.000000 joes_giant_toolbox-0.2.23/tests/test_rapid_binary_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4500 2023-04-25 09:29:06.000000 joes_giant_toolbox-0.2.23/tests/test_string_cleaner.py
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-06-17 20:54:24.030395 joes_giant_toolbox-0.3.1/
+-rw-r--r--   0 josephbolton   (501) staff       (20)    35149 2023-03-02 13:11:21.000000 joes_giant_toolbox-0.3.1/LICENSE
+-rw-r--r--   0 josephbolton   (501) staff       (20)    60529 2023-06-17 20:54:24.030156 joes_giant_toolbox-0.3.1/PKG-INFO
+-rw-r--r--   0 josephbolton   (501) staff       (20)    19249 2023-06-15 14:31:57.000000 joes_giant_toolbox-0.3.1/README.md
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-06-17 20:54:24.011605 joes_giant_toolbox-0.3.1/joes_giant_toolbox/
+-rw-r--r--   0 josephbolton   (501) staff       (20)        0 2023-04-13 17:58:22.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/__init__.py
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-06-17 20:54:24.024752 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/
+-rw-r--r--   0 josephbolton   (501) staff       (20)        0 2023-04-13 17:58:22.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/__init__.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    10700 2023-04-12 10:02:27.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4964 2023-04-17 13:22:54.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/ascii_density_histogram.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     9531 2023-04-30 11:40:27.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/compare_metric_to_prev_period.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      967 2023-03-03 07:53:04.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/conjugate_prior_beta_binomial.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      720 2023-06-06 19:54:23.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/cosine_similarity.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    10222 2023-06-14 09:08:13.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/create_gcloud_vm_docker_template.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    11774 2023-06-17 20:38:49.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/create_parallel_google_cloud_run_job_template.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4317 2023-04-17 13:55:24.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/create_project_scope_doc.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1727 2023-03-21 12:21:56.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1430 2023-03-20 07:50:22.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    10974 2023-04-06 12:30:49.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/duckduckgo_search_multipage.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     3585 2023-06-15 14:32:03.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/gcloud_vm_deletes_itself.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2791 2023-06-11 19:39:57.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/list_all_python_imports.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1098 2023-05-30 08:06:59.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/list_files_in_gcloud_bucket.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4736 2023-04-17 14:11:08.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4358 2023-03-03 08:08:14.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/make_url_request.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      376 2023-04-23 20:15:27.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/manual_keyword_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2318 2023-04-19 11:00:23.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1845 2023-04-01 21:15:07.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/print_progress_bar.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2117 2023-04-27 07:33:31.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/python_plotting_tutorials.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      501 2023-03-29 13:35:25.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/query_bigquery_to_pandas_df.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    48271 2023-04-10 13:38:46.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/rapid_binary_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     8743 2023-05-07 19:34:54.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/regex_rules_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4776 2023-05-30 08:19:34.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/run_python_function_in_parallel.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     5776 2023-04-17 12:08:12.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    13751 2023-05-06 11:30:11.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/string_cleaner.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1793 2023-06-11 19:47:40.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2360 2023-03-29 14:15:20.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/url_to_filename_to_url_mapper.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2282 2023-04-17 13:33:49.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/view_nested_dict_structure.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2804 2023-05-30 08:07:39.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/write_pandas_df_to_google_bigquery_table.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      496 2023-05-30 08:02:52.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/convenience.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      413 2023-04-25 07:40:31.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/dataviz.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1635 2023-06-15 14:31:51.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/google_cloud.py
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-06-17 20:54:24.027439 joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2126 2023-04-03 18:18:28.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/ascii_barplot.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1108 2023-03-07 09:48:13.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/conjugate_prior_normal_normal.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     3563 2023-03-16 08:04:10.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/imdb_item_page_scraper.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2088 2023-03-15 19:17:57.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/longest_portion_of_phrase_in_search_string.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      446 2023-03-10 07:50:35.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/query_wikipedia_api.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1161 2023-04-10 13:40:03.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/rapid_bag_of_words_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    47227 2023-04-01 21:12:12.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/recsys_data_simulator.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      205 2023-06-04 10:41:28.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/maths.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)       85 2023-04-17 13:38:24.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/proj_mgmt.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)       81 2023-04-17 14:03:06.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/sklearn.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      161 2023-04-26 19:46:54.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/stats.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      450 2023-05-03 07:44:37.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/text.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      515 2023-04-17 12:09:22.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/web.py
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-06-17 20:54:24.012630 joes_giant_toolbox-0.3.1/joes_giant_toolbox.egg-info/
+-rw-r--r--   0 josephbolton   (501) staff       (20)    60529 2023-06-17 20:54:24.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2870 2023-06-17 20:54:24.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 josephbolton   (501) staff       (20)        1 2023-06-17 20:54:24.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 josephbolton   (501) staff       (20)      215 2023-06-17 20:54:24.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox.egg-info/requires.txt
+-rw-r--r--   0 josephbolton   (501) staff       (20)       19 2023-06-17 20:54:24.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1118 2023-06-17 20:46:17.000000 joes_giant_toolbox-0.3.1/pyproject.toml
+-rw-r--r--   0 josephbolton   (501) staff       (20)       38 2023-06-17 20:54:24.030448 joes_giant_toolbox-0.3.1/setup.cfg
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-06-17 20:54:24.029591 joes_giant_toolbox-0.3.1/tests/
+-rw-r--r--   0 josephbolton   (501) staff       (20)      557 2023-04-26 19:48:17.000000 joes_giant_toolbox-0.3.1/tests/test_conjugate_prior_beta_binomial.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      571 2023-04-25 09:26:34.000000 joes_giant_toolbox-0.3.1/tests/test_longest_sentence_subsequence_plagiarism_detector.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2617 2023-04-25 09:27:22.000000 joes_giant_toolbox-0.3.1/tests/test_make_url_request.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     8681 2023-04-25 09:28:50.000000 joes_giant_toolbox-0.3.1/tests/test_rapid_binary_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4500 2023-04-25 09:29:06.000000 joes_giant_toolbox-0.3.1/tests/test_string_cleaner.py
```

### Comparing `joes_giant_toolbox-0.2.23/LICENSE` & `joes_giant_toolbox-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/PKG-INFO` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: joes_giant_toolbox
-Version: 0.2.23
+Name: joes-giant-toolbox
+Version: 0.3.1
 Summary: A large collection of general python functions and classes that I use in my daily work
 Author-email: Joseph Bolton <joseph.jazz.bolton@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -681,15 +681,15 @@
 Project-URL: Homepage, https://github.com/J-sephB-lt-n/joes_giant_toolbox
 Keywords: api,web,dataviz,google cloud,project management,convenience,statistics,hypothesis testing,machine learning,NLP
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: all
+Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: google
 License-File: LICENSE
 
 # Joe's Giant Tool Box
 
 https://github.com/J-sephB-lt-n/joes_giant_toolbox
@@ -712,201 +712,224 @@
  `-------------._______.----'                        /  `.
     .,.,.,.,.,.,.,.,.,.,.,.,.,                      /     \
    ((O) o o o o ======= o o(O))                 ._.'      /
 LGB `-.,.,.,.,.,.,.,.,.,.,.,-'                   `.......'
 ```
 source: https://ascii.co.uk
 
-![PyPI](https://img.shields.io/pypi/v/joes-giant-toolbox?label=pypi%20package)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/joes-giant-toolbox) 
+[![PyPI Status](https://badge.fury.io/py/joes-giant-toolbox.svg)](https://badge.fury.io/py/joes-giant-toolbox)
+[![PyPI Status](https://pepy.tech/badge/joes-giant-toolbox)](https://pepy.tech/project/joes-giant-toolbox)
 (this badge lags by 1 release on pypi)
 
 # Installation
 
 ```bash
 pip install joes-giant-toolbox
 ```
 
 # Usage
 
 The scripts exist at varying levels of completeness (some have seen extensive use in many projects whereas others have been used little or have incomplete documentation and missing unit tests). In order to measure this, I have added in a confidence score for each:
 
-Confidence Score | Description                      
+Confidence Score | Description
 -----------------|-----------------------------------------
 5                | Code has been used (without any observed failures) in multiple production environments (or large real world projects)
 4                | Code has been used (without any observed failures) in a production environment (or large real world project)
-3                | Code appears to work perfectly and passes a suite of unit tests but has not yet been used in a production environment or large real world project 
+3                | Code appears to work perfectly and passes a suite of unit tests but has not yet been used in a production environment or large real world project
 2                | The code appears to work perfectly but has not been thoroughly tested
-1                | Skeleton of function/class is present but the code does not work fully yet 
+1                | Skeleton of function/class is present but the code does not work fully yet
 
 You can search by category:
 
-* [API and Web](#api-and-web) 
+* [API and Web](#api-and-web)
 
 * [Data Visualisation](#data-visualisation)
 
 * [Google Cloud](#google-cloud)
 
 * [Project Managment](#project-management)
 
-* [Python Convenience Functions](#python-convenience-functions) 
+* [Python Convenience Functions](#python-convenience-functions)
 
 * [Statistical Inference and Hypothesis Testing](#statistical-inference-and-hypothesis-testing)
 
 * [Statistical Modelling and Machine Learning](#statistical-modelling-and-machine-learning)
 
 * [Text and Natural Language Processing](#text-and-natural-language-processing)
 
 ..or you can just scroll through the master list:
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | anonymous_view_public_linkedin_page               | Extracts the information (HTML) from a public LinkedIn page (e.g. person or company) using a virtual browser |         2        |
 | ascii_density_histogram                           | Draws a histogram using only raw text symbols                                                                |         2        |
 | conjugate_prior_beta_binomial                     | Calculates the posterior distribution of the success probability parameter [p] of a binomial distribution, from observed data and a user-specified beta prior | 4                |
+| cosine_similarity                                 | Calculates the cosine similarity between two 1-dimensional numpy arrays | 2 |
 | create_gcloud_vm_docker_template | Creates a folder containing the files necessary to quickly build a python docker container to run on a google cloud Virtual Machine | 4
-| create_project_scope_doc                          | Creates a basic project scope document (markdown) by prompting the user for input                            |         3        | 
+| create_parallel_google_cloud_run_job_template | Run a task in parallel using a Google Cloud Run job (code-generating function)| 2 |
+| create_project_scope_doc                          | Creates a basic project scope document (markdown) by prompting the user for input                            |         3        |
 | delete_file_in_gcloud_bucket                      | Deletes a file which is in a google cloud bucket                                                             |         4        |
 | download_file_from_gcloud_bucket_to_python        | Reads a file from a google cloud bucket into python memory                                                   |         4        |
 | duckduckgo_search_multipage                       | Fetches search results from the DuckDuckGo Lite search engine                                                |         2        |
+| gcloud_vm_deletes_itself                          | Running this function on a google cloud Virtual Machine (VM) causes the VM to delete itself                  |         4        |
 | list_all_python_imports                           | Searches every python script in a given folder and lists all python modules imported within those scripts    |         2        |
 | list_files_in_gcloud_bucket                       | Returns a list of the files present in a specified google cloud bucket                                       |         4        |
 | longest_sentence_subsequence_plagiarism_detector  | Finds phrases (sequences of consecutive words) common to 2 documents (e.g. to act as a naive plagiarism detector) |    3        |
 | make_url_request                                  | A convenience function for making API requests using the urllib library                                      |         3        |
 | move_or_rename_file_in_gcloud_bucket              | Move or rename a file which is in a google cloud bucket (which includes moving it to a different bucket)     |         4        |
 | print_progress_bar                                | Prints a progress bar (to standard out) while code is running                                                |         3        |
 | PythonPlottingTutorials                           | Example code snippets for creating common data visualisations in python                                      |         4        |
 | query_bigquery_to_pandas_df                       | Runs a query on Google BigQuery and writes the result into a local pandas.DataFrame                          |         4        |
 | RapidBinaryClassifier                             | Ultra rapid generation of binary classifier models in scikit-learn by abstracting away a lot of the decisions and model code| 3 |
 | RegexRulesClassifier | A multi-class text classifier using manual regex rules | 2
 | run_python_function_in_parallel                   | Runs a python function in parallel on multiple cores or threads                                              |         4        |
-| scrape_webpage_and_all_linked_webpages            | Extracts HTML from given web page, and also follows all of the hyperlinks on that page and scrapes those too |         1        | 
+| scrape_webpage_and_all_linked_webpages            | Extracts HTML from given web page, and also follows all of the hyperlinks on that page and scrapes those too |         1        |
 | StringCleaner                                     | Performs common string-cleaning operations to a text string, also allowing them to be chained in sequence    |         1        |
 | upload_file_python_to_gcloud_bucket               | Writes an object in python memory to a file (blob) on a google cloud bucket                                  |         4        |
 | url_to_filename_to_url_mapper                     | Converts a webpage URL into a useable filename, where the URL can be recovered directly from the filename    |         2        |
 | view_nested_dict_structure                        | Generates a simple printout for understanding the structure of a complex nested python dictionary            |         4        |
 | write_pandas_df_to_google_bigquery_table          | Writes a pandas dataframe to a table on Google BigQuery                                                      |         4        |
 
 ## API and Web
 
 ```python
 import joes_giant_toolbox.web
+
 help( joes_giant_toolbox.web.anonymous_view_public_linkedin_page )
 help( joes_giant_toolbox.web.duckduckgo_search_multipage )
 help( joes_giant_toolbox.web.make_url_request )
 help( joes_giant_toolbox.web.scrape_webpage_and_all_linked_webpages )
-help( joes_giant_toolbox.web.url_to_filename_to_url_mapper ) 
+help( joes_giant_toolbox.web.url_to_filename_to_url_mapper )
 ```
 
 | Name                                                     | Description                                                                                                  | Confidence Score |
 |----------------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | anonymous_view_public_linkedin_page                      | Extracts the information (HTML) from a public LinkedIn page (e.g. person or company) using a virtual browser |         2        |
 | duckduckgo_search_multipage                              | Fetches search results from the DuckDuckGo Lite search engine                                                |         2        |
 | make_url_request                                         | A convenience function for making API requests using the urllib library                                      |         3        |
-| scrape_webpage_and_all_linked_webpages                   | Extracts HTML from given web page, and also follows all of the hyperlinks on that page and scrapes those too |         1        | 
+| scrape_webpage_and_all_linked_webpages                   | Extracts HTML from given web page, and also follows all of the hyperlinks on that page and scrapes those too |         1        |
 | url_to_filename_to_url_mapper                            | Converts a webpage URL into a useable filename, where the URL can be recovered directly from the filename    |         2        |
 
 ## Data Visualisation
 
 ```python
 import joes_giant_toolbox.dataviz
+
 help( joes_giant_toolbox.dataviz )
+
 help( joes_giant_toolbox.dataviz.ascii_density_histogram )
 help( joes_giant_toolbox.dataviz.PythonPlottingTutorials )
 help( joes_giant_toolbox.dataviz.view_nested_dict_structure )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | ascii_density_histogram                           | Draws a histogram using only raw text symbols                                                                |         2        |
 | PythonPlottingTutorials                           | Example code snippets for creating common data visualisations in python                                      |         4        |
 | view_nested_dict_structure                        | Generates a simple printout for understanding the structure of a complex nested python dictionary            |         4        |
 
 ## Google Cloud
-
+To additionally install the package dependencies of this module:
 ```bash
 pip install joes-giant-toolbox[google]
 ```
 
 ```python
 import joes_giant_toolbox.google_cloud
 
 help(joes_giant_toolbox.google_cloud)
 
-help( joes_giant_toolbox.google_cloud.create_gcloud_vm_docker_template ) 
+help( joes_giant_toolbox.google_cloud.create_gcloud_vm_docker_template )
+help( joes_giant_toolbox.google_cloud.create_parallel_google_cloud_run_job_template )
 help( joes_giant_toolbox.google_cloud.delete_file_in_gcloud_bucket )
 help( joes_giant_toolbox.google_cloud.download_file_from_gcloud_bucket_to_python )
+help( joes_giant_toolbox.google_cloud.gcloud_vm_deletes_itself )
 help( joes_giant_toolbox.google_cloud.list_files_in_gcloud_bucket )
 help( joes_giant_toolbox.google_cloud.move_or_rename_file_in_gcloud_bucket )
 help( joes_giant_toolbox.google_cloud.query_bigquery_to_pandas_df )
 help( joes_giant_toolbox.google_cloud.upload_file_python_to_gcloud_bucket )
 help( joes_giant_toolbox.google_cloud.write_pandas_df_to_google_bigquery_table )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
-| create_gcloud_vm_docker_template | Creates a folder containing the files necessary to quickly build a python docker container to run on a google cloud Virtual Machine | 4
+| create_gcloud_vm_docker_template                  | Creates a folder containing the files necessary to quickly build a python docker container to run on a google cloud Virtual Machine | 4
+| create_parallel_google_cloud_run_job_template     | Run a task in parallel using a Google Cloud Run job (code-generating function)| 2 |
 | delete_file_in_gcloud_bucket                      | Deletes a file which is in a google cloud bucket                                                             |         4        |
 | download_file_from_gcloud_bucket_to_python        | Reads a file from a google cloud bucket into python memory                                                   |         4        |
+| gcloud_vm_deletes_itself                          | Running this function on a google cloud Virtual Machine (VM) causes the VM to delete itself                  |         4        |
 | list_files_in_gcloud_bucket                       | Returns a list of the files present in a specified google cloud bucket                                       |         4        |
 | move_or_rename_file_in_gcloud_bucket              | Move or rename a file which is in a google cloud bucket (which includes moving it to a different bucket)     |         4        |
 | query_bigquery_to_pandas_df                       | Runs a query on Google BigQuery and writes the result into a local pandas.DataFrame                          |         4        |
 | upload_file_python_to_gcloud_bucket               | Writes an object in python memory to a file (blob) on a google cloud bucket                                  |         4        |
 | write_pandas_df_to_google_bigquery_table          | Writes a pandas dataframe to a table on Google BigQuery                                                      |         4        |
 
 ## Project Management
 ```python
 import joes_giant_toolbox.proj_mgmt
 help( joes_giant_toolbox.proj_mgmt.create_project_scope_doc )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
-| create_project_scope_doc                          | Creates a basic project scope document (markdown) by prompting the user for input                            |         3        | 
+| create_project_scope_doc                          | Creates a basic project scope document (markdown) by prompting the user for input                            |         3        |
 
 
-## Python Convenience Functions 
+## Python Convenience Functions
 ```python
 import joes_giant_toolbox.convenience
+
 help( joes_giant_toolbox.convenience.list_all_python_imports )
 help( joes_giant_toolbox.convenience.print_progress_bar )
 help( joes_giant_toolbox.convenience.run_python_function_in_parallel )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | list_all_python_imports                           | Searches every python script in a given folder and lists all python modules imported within those scripts    |         2        |
 | print_progress_bar                                | Prints a progress bar (to standard out) while code is running                                                |         3        |
 | run_python_function_in_parallel                   | Runs a python function in parallel on multiple cores or threads                                              |         4        |
 
-## Statistical Inference and Hypothesis Testing 
+## Statistical Inference and Hypothesis Testing
 ```python
 import joes_giant_toolbox.stats
+
 help( joes_giant_toolbox.stats )
+
 help( joes_giant_toolbox.stats.conjugate_prior_beta_binomial )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | conjugate_prior_beta_binomial                     | Calculates the posterior distribution of the success probability parameter [p] of a binomial distribution, from observed data and a user-specified beta prior | 4                |
 
-## Statistical Modelling and Machine Learning 
+## Statistical Modelling and Machine Learning
+```python
+import joes_giant_toolbox.maths
+
+help( joes_giant_toolbox.maths.cosine_similarity )
+```
+
 ```python
 import joes_giant_toolbox.sklearn
+
 help( joes_giant_toolbox.sklearn.RapidBinaryClassifier )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
+| cosine_similarity                                 | Calculates the cosine similarity between two 1-dimensional numpy arrays | 2 |
 | RapidBinaryClassifier                             | Ultra rapid generation of binary classifier models in scikit-learn by abstracting away a lot of the decisions and model code| 3 |
 
 ## Text and Natural Language Processing
-```python 
+```python
 import joes_giant_toolbox.text
+
 help( joes_giant_toolbox.text )
+
 help( joes_giant_toolbox.text.longest_sentence_subsequence_plagiarism_detector )
 help( joes_giant_toolbox.text.RegexRulesClassifier )
 help( joes_giant_toolbox.text.StringCleaner )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
```

### Comparing `joes_giant_toolbox-0.2.23/README.md` & `joes_giant_toolbox-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,201 +20,224 @@
  `-------------._______.----'                        /  `.
     .,.,.,.,.,.,.,.,.,.,.,.,.,                      /     \
    ((O) o o o o ======= o o(O))                 ._.'      /
 LGB `-.,.,.,.,.,.,.,.,.,.,.,-'                   `.......'
 ```
 source: https://ascii.co.uk
 
-![PyPI](https://img.shields.io/pypi/v/joes-giant-toolbox?label=pypi%20package)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/joes-giant-toolbox) 
+[![PyPI Status](https://badge.fury.io/py/joes-giant-toolbox.svg)](https://badge.fury.io/py/joes-giant-toolbox)
+[![PyPI Status](https://pepy.tech/badge/joes-giant-toolbox)](https://pepy.tech/project/joes-giant-toolbox)
 (this badge lags by 1 release on pypi)
 
 # Installation
 
 ```bash
 pip install joes-giant-toolbox
 ```
 
 # Usage
 
 The scripts exist at varying levels of completeness (some have seen extensive use in many projects whereas others have been used little or have incomplete documentation and missing unit tests). In order to measure this, I have added in a confidence score for each:
 
-Confidence Score | Description                      
+Confidence Score | Description
 -----------------|-----------------------------------------
 5                | Code has been used (without any observed failures) in multiple production environments (or large real world projects)
 4                | Code has been used (without any observed failures) in a production environment (or large real world project)
-3                | Code appears to work perfectly and passes a suite of unit tests but has not yet been used in a production environment or large real world project 
+3                | Code appears to work perfectly and passes a suite of unit tests but has not yet been used in a production environment or large real world project
 2                | The code appears to work perfectly but has not been thoroughly tested
-1                | Skeleton of function/class is present but the code does not work fully yet 
+1                | Skeleton of function/class is present but the code does not work fully yet
 
 You can search by category:
 
-* [API and Web](#api-and-web) 
+* [API and Web](#api-and-web)
 
 * [Data Visualisation](#data-visualisation)
 
 * [Google Cloud](#google-cloud)
 
 * [Project Managment](#project-management)
 
-* [Python Convenience Functions](#python-convenience-functions) 
+* [Python Convenience Functions](#python-convenience-functions)
 
 * [Statistical Inference and Hypothesis Testing](#statistical-inference-and-hypothesis-testing)
 
 * [Statistical Modelling and Machine Learning](#statistical-modelling-and-machine-learning)
 
 * [Text and Natural Language Processing](#text-and-natural-language-processing)
 
 ..or you can just scroll through the master list:
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | anonymous_view_public_linkedin_page               | Extracts the information (HTML) from a public LinkedIn page (e.g. person or company) using a virtual browser |         2        |
 | ascii_density_histogram                           | Draws a histogram using only raw text symbols                                                                |         2        |
 | conjugate_prior_beta_binomial                     | Calculates the posterior distribution of the success probability parameter [p] of a binomial distribution, from observed data and a user-specified beta prior | 4                |
+| cosine_similarity                                 | Calculates the cosine similarity between two 1-dimensional numpy arrays | 2 |
 | create_gcloud_vm_docker_template | Creates a folder containing the files necessary to quickly build a python docker container to run on a google cloud Virtual Machine | 4
-| create_project_scope_doc                          | Creates a basic project scope document (markdown) by prompting the user for input                            |         3        | 
+| create_parallel_google_cloud_run_job_template | Run a task in parallel using a Google Cloud Run job (code-generating function)| 2 |
+| create_project_scope_doc                          | Creates a basic project scope document (markdown) by prompting the user for input                            |         3        |
 | delete_file_in_gcloud_bucket                      | Deletes a file which is in a google cloud bucket                                                             |         4        |
 | download_file_from_gcloud_bucket_to_python        | Reads a file from a google cloud bucket into python memory                                                   |         4        |
 | duckduckgo_search_multipage                       | Fetches search results from the DuckDuckGo Lite search engine                                                |         2        |
+| gcloud_vm_deletes_itself                          | Running this function on a google cloud Virtual Machine (VM) causes the VM to delete itself                  |         4        |
 | list_all_python_imports                           | Searches every python script in a given folder and lists all python modules imported within those scripts    |         2        |
 | list_files_in_gcloud_bucket                       | Returns a list of the files present in a specified google cloud bucket                                       |         4        |
 | longest_sentence_subsequence_plagiarism_detector  | Finds phrases (sequences of consecutive words) common to 2 documents (e.g. to act as a naive plagiarism detector) |    3        |
 | make_url_request                                  | A convenience function for making API requests using the urllib library                                      |         3        |
 | move_or_rename_file_in_gcloud_bucket              | Move or rename a file which is in a google cloud bucket (which includes moving it to a different bucket)     |         4        |
 | print_progress_bar                                | Prints a progress bar (to standard out) while code is running                                                |         3        |
 | PythonPlottingTutorials                           | Example code snippets for creating common data visualisations in python                                      |         4        |
 | query_bigquery_to_pandas_df                       | Runs a query on Google BigQuery and writes the result into a local pandas.DataFrame                          |         4        |
 | RapidBinaryClassifier                             | Ultra rapid generation of binary classifier models in scikit-learn by abstracting away a lot of the decisions and model code| 3 |
 | RegexRulesClassifier | A multi-class text classifier using manual regex rules | 2
 | run_python_function_in_parallel                   | Runs a python function in parallel on multiple cores or threads                                              |         4        |
-| scrape_webpage_and_all_linked_webpages            | Extracts HTML from given web page, and also follows all of the hyperlinks on that page and scrapes those too |         1        | 
+| scrape_webpage_and_all_linked_webpages            | Extracts HTML from given web page, and also follows all of the hyperlinks on that page and scrapes those too |         1        |
 | StringCleaner                                     | Performs common string-cleaning operations to a text string, also allowing them to be chained in sequence    |         1        |
 | upload_file_python_to_gcloud_bucket               | Writes an object in python memory to a file (blob) on a google cloud bucket                                  |         4        |
 | url_to_filename_to_url_mapper                     | Converts a webpage URL into a useable filename, where the URL can be recovered directly from the filename    |         2        |
 | view_nested_dict_structure                        | Generates a simple printout for understanding the structure of a complex nested python dictionary            |         4        |
 | write_pandas_df_to_google_bigquery_table          | Writes a pandas dataframe to a table on Google BigQuery                                                      |         4        |
 
 ## API and Web
 
 ```python
 import joes_giant_toolbox.web
+
 help( joes_giant_toolbox.web.anonymous_view_public_linkedin_page )
 help( joes_giant_toolbox.web.duckduckgo_search_multipage )
 help( joes_giant_toolbox.web.make_url_request )
 help( joes_giant_toolbox.web.scrape_webpage_and_all_linked_webpages )
-help( joes_giant_toolbox.web.url_to_filename_to_url_mapper ) 
+help( joes_giant_toolbox.web.url_to_filename_to_url_mapper )
 ```
 
 | Name                                                     | Description                                                                                                  | Confidence Score |
 |----------------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | anonymous_view_public_linkedin_page                      | Extracts the information (HTML) from a public LinkedIn page (e.g. person or company) using a virtual browser |         2        |
 | duckduckgo_search_multipage                              | Fetches search results from the DuckDuckGo Lite search engine                                                |         2        |
 | make_url_request                                         | A convenience function for making API requests using the urllib library                                      |         3        |
-| scrape_webpage_and_all_linked_webpages                   | Extracts HTML from given web page, and also follows all of the hyperlinks on that page and scrapes those too |         1        | 
+| scrape_webpage_and_all_linked_webpages                   | Extracts HTML from given web page, and also follows all of the hyperlinks on that page and scrapes those too |         1        |
 | url_to_filename_to_url_mapper                            | Converts a webpage URL into a useable filename, where the URL can be recovered directly from the filename    |         2        |
 
 ## Data Visualisation
 
 ```python
 import joes_giant_toolbox.dataviz
+
 help( joes_giant_toolbox.dataviz )
+
 help( joes_giant_toolbox.dataviz.ascii_density_histogram )
 help( joes_giant_toolbox.dataviz.PythonPlottingTutorials )
 help( joes_giant_toolbox.dataviz.view_nested_dict_structure )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | ascii_density_histogram                           | Draws a histogram using only raw text symbols                                                                |         2        |
 | PythonPlottingTutorials                           | Example code snippets for creating common data visualisations in python                                      |         4        |
 | view_nested_dict_structure                        | Generates a simple printout for understanding the structure of a complex nested python dictionary            |         4        |
 
 ## Google Cloud
-
+To additionally install the package dependencies of this module:
 ```bash
 pip install joes-giant-toolbox[google]
 ```
 
 ```python
 import joes_giant_toolbox.google_cloud
 
 help(joes_giant_toolbox.google_cloud)
 
-help( joes_giant_toolbox.google_cloud.create_gcloud_vm_docker_template ) 
+help( joes_giant_toolbox.google_cloud.create_gcloud_vm_docker_template )
+help( joes_giant_toolbox.google_cloud.create_parallel_google_cloud_run_job_template )
 help( joes_giant_toolbox.google_cloud.delete_file_in_gcloud_bucket )
 help( joes_giant_toolbox.google_cloud.download_file_from_gcloud_bucket_to_python )
+help( joes_giant_toolbox.google_cloud.gcloud_vm_deletes_itself )
 help( joes_giant_toolbox.google_cloud.list_files_in_gcloud_bucket )
 help( joes_giant_toolbox.google_cloud.move_or_rename_file_in_gcloud_bucket )
 help( joes_giant_toolbox.google_cloud.query_bigquery_to_pandas_df )
 help( joes_giant_toolbox.google_cloud.upload_file_python_to_gcloud_bucket )
 help( joes_giant_toolbox.google_cloud.write_pandas_df_to_google_bigquery_table )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
-| create_gcloud_vm_docker_template | Creates a folder containing the files necessary to quickly build a python docker container to run on a google cloud Virtual Machine | 4
+| create_gcloud_vm_docker_template                  | Creates a folder containing the files necessary to quickly build a python docker container to run on a google cloud Virtual Machine | 4
+| create_parallel_google_cloud_run_job_template     | Run a task in parallel using a Google Cloud Run job (code-generating function)| 2 |
 | delete_file_in_gcloud_bucket                      | Deletes a file which is in a google cloud bucket                                                             |         4        |
 | download_file_from_gcloud_bucket_to_python        | Reads a file from a google cloud bucket into python memory                                                   |         4        |
+| gcloud_vm_deletes_itself                          | Running this function on a google cloud Virtual Machine (VM) causes the VM to delete itself                  |         4        |
 | list_files_in_gcloud_bucket                       | Returns a list of the files present in a specified google cloud bucket                                       |         4        |
 | move_or_rename_file_in_gcloud_bucket              | Move or rename a file which is in a google cloud bucket (which includes moving it to a different bucket)     |         4        |
 | query_bigquery_to_pandas_df                       | Runs a query on Google BigQuery and writes the result into a local pandas.DataFrame                          |         4        |
 | upload_file_python_to_gcloud_bucket               | Writes an object in python memory to a file (blob) on a google cloud bucket                                  |         4        |
 | write_pandas_df_to_google_bigquery_table          | Writes a pandas dataframe to a table on Google BigQuery                                                      |         4        |
 
 ## Project Management
 ```python
 import joes_giant_toolbox.proj_mgmt
 help( joes_giant_toolbox.proj_mgmt.create_project_scope_doc )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
-| create_project_scope_doc                          | Creates a basic project scope document (markdown) by prompting the user for input                            |         3        | 
+| create_project_scope_doc                          | Creates a basic project scope document (markdown) by prompting the user for input                            |         3        |
 
 
-## Python Convenience Functions 
+## Python Convenience Functions
 ```python
 import joes_giant_toolbox.convenience
+
 help( joes_giant_toolbox.convenience.list_all_python_imports )
 help( joes_giant_toolbox.convenience.print_progress_bar )
 help( joes_giant_toolbox.convenience.run_python_function_in_parallel )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | list_all_python_imports                           | Searches every python script in a given folder and lists all python modules imported within those scripts    |         2        |
 | print_progress_bar                                | Prints a progress bar (to standard out) while code is running                                                |         3        |
 | run_python_function_in_parallel                   | Runs a python function in parallel on multiple cores or threads                                              |         4        |
 
-## Statistical Inference and Hypothesis Testing 
+## Statistical Inference and Hypothesis Testing
 ```python
 import joes_giant_toolbox.stats
+
 help( joes_giant_toolbox.stats )
+
 help( joes_giant_toolbox.stats.conjugate_prior_beta_binomial )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | conjugate_prior_beta_binomial                     | Calculates the posterior distribution of the success probability parameter [p] of a binomial distribution, from observed data and a user-specified beta prior | 4                |
 
-## Statistical Modelling and Machine Learning 
+## Statistical Modelling and Machine Learning
+```python
+import joes_giant_toolbox.maths
+
+help( joes_giant_toolbox.maths.cosine_similarity )
+```
+
 ```python
 import joes_giant_toolbox.sklearn
+
 help( joes_giant_toolbox.sklearn.RapidBinaryClassifier )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
+| cosine_similarity                                 | Calculates the cosine similarity between two 1-dimensional numpy arrays | 2 |
 | RapidBinaryClassifier                             | Ultra rapid generation of binary classifier models in scikit-learn by abstracting away a lot of the decisions and model code| 3 |
 
 ## Text and Natural Language Processing
-```python 
+```python
 import joes_giant_toolbox.text
+
 help( joes_giant_toolbox.text )
+
 help( joes_giant_toolbox.text.longest_sentence_subsequence_plagiarism_detector )
 help( joes_giant_toolbox.text.RegexRulesClassifier )
 help( joes_giant_toolbox.text.StringCleaner )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
@@ -224,8 +247,8 @@
 
 # Run Unit Tests
 
 ```bash
 pip install pytest
 cd joes_giant_toolbox/tests
 pytest -v
-```
+```
```

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/ascii_density_histogram.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/ascii_density_histogram.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/compare_metric_to_prev_period.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/compare_metric_to_prev_period.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/conjugate_prior_beta_binomial.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/conjugate_prior_beta_binomial.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/create_project_scope_doc.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/create_project_scope_doc.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/duckduckgo_search_multipage.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/duckduckgo_search_multipage.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/list_all_python_imports.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/list_all_python_imports.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,59 @@
+"""
+This script defines the function list_all_python_imports()
+"""
+
 import os
 import re
+from typing import Dict, Tuple
 import warnings
 
 
-def list_all_python_imports(dir_path: str) -> dict:
-    """Searches every python script in a given folder and lists all python modules imported within those scripts
-
-    (see "Example Usage")
-
+def list_all_python_imports(dir_path: str) -> Dict[str, Tuple[str]]:
+    """Searches every python script in a given folder and lists all python modules imported
+    within those scripts\n
+    (see "Example Usage")\n
     Parameters
     ----------
     dir_path: str
-        Folder in which to find the python scripts
-
+        Folder in which to find the python scripts\n
     Notes
     -----
     Package import statements are only searched for in files ending with .py or .ipynb
     Lines starting with a hash (i.e. commented lines) are ignored
-    Any line of a script on which no modules were found although the line contains the word "import" raises a warning
-
+    Any line of a script on which no modules were found although the line contains
+    the word "import" raises a warning\n
     Example Usage
     -------------
     >>> from pprint import pprint
-    >>> imports_found_dict = list_all_python_imports( os.getcwd() )
+    >>> import joes_giant_toolbox.convenience
+    >>> imports_found_dict = joes_giant_toolbox.convenience.list_all_python_imports( os.getcwd() )
     >>> pprint(imports_found_dict)
-    ...
-
+    {
+        '__init__.py': (),
+        'ascii_density_histogram.py': ('typing', 'math'),
+        'conjugate_prior_beta_binomial.py': (),
+        'cosine_similarity.py': ('numpy',),
+    }
     Returns
     -------
-    dict
+    Dict[str, Tuple[str]]
         {file_name: tuple_of_module_names}
         Dictionary, with key=filename and values=(tuple containing list of modules found)
     """
-    results_dict = {
-        filename: f"{dir_path}/{filename}"
+    results_dict: Dict[str, Tuple[str]] = {
+        filename: f"{dir_path}/{filename}"  # type: ignore
         for filename in os.listdir(dir_path)
         if filename != "list_all_python_imports.py"
         and (filename[-3:] == r".py" or filename[-6:] == r".ipynb")
     }
 
     for script in results_dict:
-        with open(results_dict[script], "r") as f:
-            temp_readlines = f.readlines()
+        with open(results_dict[script], "r", encoding="utf-8") as file:  # type: ignore
+            temp_readlines = file.readlines()
 
         imports_found = []
         for line in temp_readlines:
             words_in_line = line.strip().split()
             if len(words_in_line) > 0:
                 if words_in_line[0] == "#":
                     # ignore lines starting with a comment
@@ -53,14 +61,14 @@
                 elif words_in_line[0] == "import":
                     imports_found.append(words_in_line[1])
                 elif words_in_line[0] == "from" and words_in_line[2] == "import":
                     imports_found.append(words_in_line[1])
                 elif re.search(r"\bimport\b", line):
                     if ">>>" not in line:
                         warnings.warn(
-                            f"possible import missed due to unexpected import pattern: {script} {line}"
+                            f"possible import missed due to unexpected import pattern: {script} {line}"  # pylint: disable=line-too-long
                         )
 
-        results_dict[script] = tuple(set(imports_found))
+        results_dict[script] = tuple(set(imports_found))  # type: ignore
         del imports_found, temp_readlines
 
     return results_dict
```

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/list_files_in_gcloud_bucket.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/list_files_in_gcloud_bucket.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,17 @@
+"""
+This script defines the function list_files_in_gcloud_bucket
+"""
 from typing import List
-import google.cloud.storage
+import google.cloud.storage  # pylint: disable=import-error, no-name-in-module
 
 
-def list_files_in_gcloud_bucket(bucket_name: str, prefix: str = None) -> List[str]:
+def list_files_in_gcloud_bucket(
+    bucket_name: str, prefix: str | None = None
+) -> List[str]:
     """
     Returns a list of the files (filenames) present in a google cloud bucket
 
     Parameters
     ----------
     bucket_name: str
         The name of the google cloud bucket
@@ -14,15 +19,17 @@
         If present, only returns files whose path starts with the given prefix
 
     Returns
     -------
     List[str]
         List of filenames in the google cloud bucket (file pathes)
     """
+    # pylint: disable=c-extension-no-member
     storage_client = google.cloud.storage.Client()
+    # pylint: enable=c-extension-no-member
     if prefix is not None:
         blobs = storage_client.list_blobs(bucket_name, prefix=prefix)
     else:
         blobs = storage_client.list_blobs(bucket_name)
     all_filenames = []
     for blob in blobs:
         all_filenames.append(blob.name)
```

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/make_url_request.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/make_url_request.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/print_progress_bar.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/print_progress_bar.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/python_plotting_tutorials.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/python_plotting_tutorials.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/rapid_binary_classifier.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/rapid_binary_classifier.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/regex_rules_classifier.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/regex_rules_classifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,34 @@
+"""Defines the class 'RegexRulesClassifier', which is a multi-class text classifier using manual
+regex rules"""
+
 import random
 import re
 from typing import List
 
 
 class RegexRulesClassifier:
-    """A multi-class text classifier using manual regex rules
+    """A multi-class text classifier model using manual regex rules
 
-    For a particular example, points are awarded to class labels based on which regex rules match for that example..
-        ..and the class label with the highest points is then the model prediction for that example
+    For a particular example, points are awarded to class labels based on which regex rules
+    match for that example, and the class label with the highest total points is then the model
+    prediction for that example.
 
-    Refer to "Example Usage" below
+    Refer to "Example Usage" below.
 
     Notes
     -----
-    Unlike other popular python model packages, this model generates predictions for a single example at a time.
+    Unlike other popular python model packages, this model generates predictions for one
+    example at a time.
     Therefore, to predict for multiple examples, multiple calls must be made to .predict() function
     e.g.
-    >>> predictions: list = [my_model.predict(example_i) for example_i in ("example 1 text", "example 2 text", "example 3 text")]
+    >>> predictions: list = [
+    ...     my_model.predict(example_i)
+    ...     for example_i in ("example 1 text", "example 2 text", "example 3 text")
+    ... ]
 
     Attributes
     ----------
     verbose : bool
         Whether the model should print process information while it runs
 
     Methods
@@ -37,19 +45,19 @@
     Example Usage
     -------------
     >>> import joes_giant_toolbox.text
     >>> clothing_gender_classifier = joes_giant_toolbox.text.RegexRulesClassifier(verbose=True)
     >>> clothing_gender_classifier.define_rules(
     ...     {
     ...         r"\\bmen": {"mens": 10}, # e.g. will not match "women"
-    ...         r"(\\bbikini\\b)|(\\bskirt)|(\\bdress)": {"ladies": 10}, # must match 1 or more of these words
-    ...         r"(\\bchild)|(\\bkid)": {"childrens": 10}, # will match "child" or "children" or "kid" or "kids" etc.
+    ...         r"(\\bbikini\\b)|(\\bskirt)|(\\bdress)": {"ladies": 10}, # must match 1+ of these
+    ...         r"(\\bchild)|(\\bkid)": {"childrens": 10}, # match "child","children","kid","kids"
     ...         r"\\bgirls?\\b": {"ladies": 5, "childrens": 5},
     ...         r"\\badult": {"ladies":5, "mens":5},
-    ...         r"\\bhawaiian\\b.*\\bshirt\\b": {"mens":10}, # must contain both "hawaiian" and "shirt"
+    ...         r"\\bhawaiian\\b.*\\bshirt\\b": {"mens":10}, # must "hawaiian" AND "shirt"
     ...     }
     ... )
     defined 6 rules
     >>> clothing_gender_classifier.predict("girls bikini top")
     rule match: '(\bbikini\b)|(\bskirt)|(\bdress)'
             "ladies" +10
     rule match: '\bgirls?\b'
@@ -161,28 +169,26 @@
                 * A list of predicted class labels (if ties_handling=="all")
                 * None if no class label was awarded any points (i.e. no regex matches at all)
         """
         scores_dict: dict = self.__tally_label_scores(text_str)
         if max(scores_dict.values()) == 0:
             if ties_handling == "all":
                 return []
-            else:
-                return None
-        elif ties_handling == "first":
+            return None
+        if ties_handling == "first":
             return max(scores_dict, key=scores_dict.get)
-        elif ties_handling == "all":
+        if ties_handling == "all":
             return [
                 k for k in scores_dict if scores_dict[k] == max(scores_dict.values())
             ]
-        elif ties_handling == "random":
+        if ties_handling == "random":
             return random.choice(
                 [k for k in scores_dict if scores_dict[k] == max(scores_dict.values())]
             )
-        else:
-            raise ValueError("argument 'tie_handling' must be one of ['first','all']")
+        raise ValueError("argument 'tie_handling' must be one of ['first','all']")
 
     def predict_scores(self, text_str: str) -> dict:
         """Returns the total scores for all of the class labels for a single input example
 
         Parameters
         ----------
         text_str : str
```

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/run_python_function_in_parallel.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/run_python_function_in_parallel.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,50 @@
+"""
+This script defines the function run_python_function_in_parallel()
+"""
+
 import concurrent.futures
-from typing import Callable, Iterator
+from typing import Any, Callable, Tuple, Iterator
 import os
 import threading
 import functools
 
 
 def run_python_function_in_parallel(
     func: Callable,
-    input_tuple: tuple,
+    input_tuple: Tuple[Any],
     parallel_method: str,
     verbose: bool,
     **kwargs,
 ) -> Iterator:
-    """Convenience function for running a python function in parallel on multiple cores or threads
-
+    """Convenience function for running a python function in parallel on multiple cores or threads\n
     Notes
     -----
-    If your function has multiple input parameters, you need to wrap these within the single input argument [x]...
-    ...and then unpack [x] within the function itself.
+    If your function has multiple input parameters, you need to wrap these within the single
+    input argument [x] and then unpack [x] within the function itself.
     e.g. [x] could be a dictionary, namedtuple or list (refer to the examples below)
-    If you require logging of the individual workers, then you should put explicit python logging within [func]
-
+    If you require logging of the individual workers, then you should put explicit python
+    logging within [func]\n
     Parameters
     ----------
     func: Callable
         A function taking a single argument (x)
     input_tuple: tuple
         A tuple (immutable list) containing the list of input objects (x) to process by the function
     parallel_method: str
         The method to use for parallelisation: one of ['multi_core', 'multi_thread']
     verbose: bool
         Whether to print worker information during the run or not
     **kwargs
-        Additional keyword arguments to pass to concurrent.futures.ProcessPoolExecutor() or concurrent.futures.ThreadPoolExecutor()
-
+        Additional keyword arguments to pass to concurrent.futures.ProcessPoolExecutor() or
+        concurrent.futures.ThreadPoolExecutor()\n
     Returns
     -------
     Iterator
-        Returns the function outputs as an iterator
-
+        Returns the function outputs as an iterator\n
     Example Usage
     -------------
     >>> def sum_squares(x): return sum([num**2 for num in x])
     >>> run_test = run_python_function_in_parallel(
     ...     func = sum_squares,
     ...     input_tuple = ( [1,2], [3,4], [5,6,7] ),
     ...     parallel_method = "multi_thread",
@@ -91,22 +93,23 @@
         "multi_thread",
     ]:
         raise ValueError(
             "parallel_method must be one of ['multi_core', 'multi_thread']"
         )
 
     def make_verbose(func):
-        """A decorator to make a function print process and thread information before and after running"""
+        """A decorator to make a function print process and thread information
+        before and after running"""
 
         @functools.wraps(func)
         def verbose_func(*args, **kwargs):
             print(
                 f"\nSTARTED: process_ID={os.getpid()} thread_ID={threading.get_native_id()}"
             )
-            result = func(*args, **kwargs)
+            result: Any = func(*args, **kwargs)
             print(
                 f"\nCOMPLETED: process_ID={os.getpid()} thread_ID={threading.get_native_id()}"
             )
             return result
 
         return verbose_func
 
@@ -117,19 +120,19 @@
             return func(*args, **kwargs)
 
     else:
         wrapped_func = func
 
     if parallel_method == "multi_core":
         with concurrent.futures.ProcessPoolExecutor(**kwargs) as executor:
-            result = executor.map(wrapped_func, input_tuple)
+            result: Iterator = executor.map(wrapped_func, input_tuple)
 
     elif parallel_method == "multi_thread":
-        with concurrent.futures.ThreadPoolExecutor(**kwargs) as executor:
-            result = executor.map(wrapped_func, input_tuple)
+        with concurrent.futures.ThreadPoolExecutor(**kwargs) as executor:  # type: ignore
+            result: Iterator = executor.map(wrapped_func, input_tuple)  # type: ignore
 
     else:
         raise ValueError(
             "parameter 'parallel_method' must be one of ['multi_core', 'multi_thread']"
         )
 
     return result
```

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/string_cleaner.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/string_cleaner.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-import google.cloud.storage
+"""
+This script defines the function upload_file_python_to_gcloud_bucket()
+"""
+
+import google.cloud.storage  # pylint: disable=import-error,no-name-in-module
 
 
 def upload_file_python_to_gcloud_bucket(
     contents_str: str, bucket_name: str, filename_on_bucket: str, file_type: str
 ) -> None:
     """Write an object in python memory to a file (blob) on a google cloud bucket
 
@@ -22,22 +26,23 @@
     -----
     In order to preserve unicode symbols when uploading a string (e.g. when uploading html) use:
         contents_str = my_string.encode("raw_unicode_escape")
 
 
     Example usage
     -------------
-    >>> upload_file_to_cloud_bucket(
+    >>> import joes_giant_toolbox.google_cloud
+    >>> joes_giant_toolbox.google_cloud.upload_file_python_to_gcloud_bucket(
     ...     contents_str = pd.DataFrame({"x":[1,2,3]}).to_csv(index=False),
     ...     bucket_name="my-bucket",
     ...     filename_on_bucket="pd_df.csv",
     ...     file_type="text/csv"
     ... )
 
-    >>> upload_file_to_cloud_bucket(
+    >>> joes_giant_toolbox.google_cloud.upload_file_python_to_gcloud_bucket(
     ...     contents_str = json.dumps( {"x":69, "y":[4,20]} ),
     ...     bucket_name="my-bucket",
     ...     filename_on_bucket="dict.json",
     ...     file_type="text/json"
     ... )
     """
     storage_client = google.cloud.storage.Client()
```

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/url_to_filename_to_url_mapper.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/url_to_filename_to_url_mapper.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/view_nested_dict_structure.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/view_nested_dict_structure.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/all/write_pandas_df_to_google_bigquery_table.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/write_pandas_df_to_google_bigquery_table.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,47 @@
+"""
+This script defines the function write_pandas_df_to_google_bigquery_table()
+"""
+
+from typing import List
 import pandas as pd
 import google.cloud.bigquery
 
 
+# pylint: disable=line-too-long
 def write_pandas_df_to_google_bigquery_table(
-    pandas_df: pd.DataFrame, bigquery_table_path: str, column_schema: list
+    pandas_df: pd.DataFrame,
+    bigquery_table_path: str,
+    column_schema: List[google.cloud.bigquery.SchemaField],
+    overwrite_strategy: str = "WRITE_APPEND",
 ) -> None:
     """
     Writes a pandas dataframe to a table on Google BigQuery
 
+    Notes
+    -----
+    If the table already exists on BigQuery, the default behaviour is to append the new data to it
+
     Parameters
     ----------
     pandas_df: pandas.DataFrame
         Table to be written to BigQuery
-    bigquery_table_path: str
+    bigquery_table_path : str
         Path to destination table e.g. "project_name.dataset_name.table_name"
-    column_schema: list of google.cloud.bigquery.enums.SqlTypeNames objects
+    column_schema : list of google.cloud.bigquery.enums.SqlTypeNames objects
         A list of column data types, informing BigQuery of the data type of each column (refer to the example below)
         This list is passed to the parameter "schema" in the function bigquery.LoadJobConfig()
+    overwrite_strategy : str
+        Controls the behaviour of the write when the destination table already exists and contains data
+        One of:
+            "WRITE_APPEND"   - new data is appended to existing data in the destination table
+            "WRITE_TRUNCATE" - new data overwrites existing data in the destination table
+            "WRITE_EMPTY"    - returns an error if there is existing data in the destination table
+        Refer to gcloud documentation:
+        https://cloud.google.com/bigquery/docs/reference/rest/v2/Job#JobConfigurationLoad.FIELDS.write_disposition
 
     Example Usage
     -------------
     import pandas as pd
     from google.cloud import bigquery
     example_df = pd.DataFrame(
       {
@@ -39,10 +60,12 @@
       ],
     )
     """
     client = google.cloud.bigquery.Client()
     job = client.load_table_from_dataframe(
         pandas_df,
         bigquery_table_path,
-        job_config=google.cloud.bigquery.LoadJobConfig(schema=column_schema),
+        job_config=google.cloud.bigquery.LoadJobConfig(
+            schema=column_schema, write_disposition=overwrite_strategy
+        ),
     )
     job.result()  # wait for the job to complete
```

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/google_cloud.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/google_cloud.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 """Utilities for interacting with Google Cloud
 
-Available modules: 
+Available modules:
     - create_gcloud_vm_docker_template
+    - create_parallel_google_cloud_run_job_template
     - delete_file_in_gcloud_bucket
     - download_file_from_gcloud_bucket_to_python
+    - gcloud_vm_deletes_itself
     - list_files_in_gcloud_bucket
     - move_or_rename_file_in_gcloud_bucket
     - query_bigquery_to_pandas_df
     - upload_file_python_to_gcloud_bucket
     - write_pandas_df_to_google_bigquery_table
 
 """
 
+# pylint: disable=unused-import
+
 from joes_giant_toolbox.all.create_gcloud_vm_docker_template import (
     create_gcloud_vm_docker_template,
 )
-
+from joes_giant_toolbox.all.create_parallel_google_cloud_run_job_template import (
+    create_parallel_google_cloud_run_job_template,
+)
 from joes_giant_toolbox.all.delete_file_in_gcloud_bucket import (
     delete_file_in_gcloud_bucket,
 )
 from joes_giant_toolbox.all.download_file_from_gcloud_bucket_to_python import (
     download_file_from_gcloud_bucket_to_python,
 )
+from joes_giant_toolbox.all.gcloud_vm_deletes_itself import gcloud_vm_deletes_itself
 from joes_giant_toolbox.all.list_files_in_gcloud_bucket import (
     list_files_in_gcloud_bucket,
 )
 from joes_giant_toolbox.all.move_or_rename_file_in_gcloud_bucket import (
     move_or_rename_file_in_gcloud_bucket,
 )
 from joes_giant_toolbox.all.query_bigquery_to_pandas_df import (
```

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/in_progress/ascii_barplot.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/ascii_barplot.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/in_progress/conjugate_prior_normal_normal.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/conjugate_prior_normal_normal.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/in_progress/imdb_item_page_scraper.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/imdb_item_page_scraper.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/in_progress/longest_portion_of_phrase_in_search_string.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/longest_portion_of_phrase_in_search_string.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/in_progress/rapid_bag_of_words_classifier.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/rapid_bag_of_words_classifier.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/in_progress/recsys_data_simulator.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/recsys_data_simulator.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox/web.py` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox/web.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox.egg-info/PKG-INFO` & `joes_giant_toolbox-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: joes-giant-toolbox
-Version: 0.2.23
+Name: joes_giant_toolbox
+Version: 0.3.1
 Summary: A large collection of general python functions and classes that I use in my daily work
 Author-email: Joseph Bolton <joseph.jazz.bolton@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -681,15 +681,15 @@
 Project-URL: Homepage, https://github.com/J-sephB-lt-n/joes_giant_toolbox
 Keywords: api,web,dataviz,google cloud,project management,convenience,statistics,hypothesis testing,machine learning,NLP
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: all
+Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: google
 License-File: LICENSE
 
 # Joe's Giant Tool Box
 
 https://github.com/J-sephB-lt-n/joes_giant_toolbox
@@ -712,201 +712,224 @@
  `-------------._______.----'                        /  `.
     .,.,.,.,.,.,.,.,.,.,.,.,.,                      /     \
    ((O) o o o o ======= o o(O))                 ._.'      /
 LGB `-.,.,.,.,.,.,.,.,.,.,.,-'                   `.......'
 ```
 source: https://ascii.co.uk
 
-![PyPI](https://img.shields.io/pypi/v/joes-giant-toolbox?label=pypi%20package)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/joes-giant-toolbox) 
+[![PyPI Status](https://badge.fury.io/py/joes-giant-toolbox.svg)](https://badge.fury.io/py/joes-giant-toolbox)
+[![PyPI Status](https://pepy.tech/badge/joes-giant-toolbox)](https://pepy.tech/project/joes-giant-toolbox)
 (this badge lags by 1 release on pypi)
 
 # Installation
 
 ```bash
 pip install joes-giant-toolbox
 ```
 
 # Usage
 
 The scripts exist at varying levels of completeness (some have seen extensive use in many projects whereas others have been used little or have incomplete documentation and missing unit tests). In order to measure this, I have added in a confidence score for each:
 
-Confidence Score | Description                      
+Confidence Score | Description
 -----------------|-----------------------------------------
 5                | Code has been used (without any observed failures) in multiple production environments (or large real world projects)
 4                | Code has been used (without any observed failures) in a production environment (or large real world project)
-3                | Code appears to work perfectly and passes a suite of unit tests but has not yet been used in a production environment or large real world project 
+3                | Code appears to work perfectly and passes a suite of unit tests but has not yet been used in a production environment or large real world project
 2                | The code appears to work perfectly but has not been thoroughly tested
-1                | Skeleton of function/class is present but the code does not work fully yet 
+1                | Skeleton of function/class is present but the code does not work fully yet
 
 You can search by category:
 
-* [API and Web](#api-and-web) 
+* [API and Web](#api-and-web)
 
 * [Data Visualisation](#data-visualisation)
 
 * [Google Cloud](#google-cloud)
 
 * [Project Managment](#project-management)
 
-* [Python Convenience Functions](#python-convenience-functions) 
+* [Python Convenience Functions](#python-convenience-functions)
 
 * [Statistical Inference and Hypothesis Testing](#statistical-inference-and-hypothesis-testing)
 
 * [Statistical Modelling and Machine Learning](#statistical-modelling-and-machine-learning)
 
 * [Text and Natural Language Processing](#text-and-natural-language-processing)
 
 ..or you can just scroll through the master list:
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | anonymous_view_public_linkedin_page               | Extracts the information (HTML) from a public LinkedIn page (e.g. person or company) using a virtual browser |         2        |
 | ascii_density_histogram                           | Draws a histogram using only raw text symbols                                                                |         2        |
 | conjugate_prior_beta_binomial                     | Calculates the posterior distribution of the success probability parameter [p] of a binomial distribution, from observed data and a user-specified beta prior | 4                |
+| cosine_similarity                                 | Calculates the cosine similarity between two 1-dimensional numpy arrays | 2 |
 | create_gcloud_vm_docker_template | Creates a folder containing the files necessary to quickly build a python docker container to run on a google cloud Virtual Machine | 4
-| create_project_scope_doc                          | Creates a basic project scope document (markdown) by prompting the user for input                            |         3        | 
+| create_parallel_google_cloud_run_job_template | Run a task in parallel using a Google Cloud Run job (code-generating function)| 2 |
+| create_project_scope_doc                          | Creates a basic project scope document (markdown) by prompting the user for input                            |         3        |
 | delete_file_in_gcloud_bucket                      | Deletes a file which is in a google cloud bucket                                                             |         4        |
 | download_file_from_gcloud_bucket_to_python        | Reads a file from a google cloud bucket into python memory                                                   |         4        |
 | duckduckgo_search_multipage                       | Fetches search results from the DuckDuckGo Lite search engine                                                |         2        |
+| gcloud_vm_deletes_itself                          | Running this function on a google cloud Virtual Machine (VM) causes the VM to delete itself                  |         4        |
 | list_all_python_imports                           | Searches every python script in a given folder and lists all python modules imported within those scripts    |         2        |
 | list_files_in_gcloud_bucket                       | Returns a list of the files present in a specified google cloud bucket                                       |         4        |
 | longest_sentence_subsequence_plagiarism_detector  | Finds phrases (sequences of consecutive words) common to 2 documents (e.g. to act as a naive plagiarism detector) |    3        |
 | make_url_request                                  | A convenience function for making API requests using the urllib library                                      |         3        |
 | move_or_rename_file_in_gcloud_bucket              | Move or rename a file which is in a google cloud bucket (which includes moving it to a different bucket)     |         4        |
 | print_progress_bar                                | Prints a progress bar (to standard out) while code is running                                                |         3        |
 | PythonPlottingTutorials                           | Example code snippets for creating common data visualisations in python                                      |         4        |
 | query_bigquery_to_pandas_df                       | Runs a query on Google BigQuery and writes the result into a local pandas.DataFrame                          |         4        |
 | RapidBinaryClassifier                             | Ultra rapid generation of binary classifier models in scikit-learn by abstracting away a lot of the decisions and model code| 3 |
 | RegexRulesClassifier | A multi-class text classifier using manual regex rules | 2
 | run_python_function_in_parallel                   | Runs a python function in parallel on multiple cores or threads                                              |         4        |
-| scrape_webpage_and_all_linked_webpages            | Extracts HTML from given web page, and also follows all of the hyperlinks on that page and scrapes those too |         1        | 
+| scrape_webpage_and_all_linked_webpages            | Extracts HTML from given web page, and also follows all of the hyperlinks on that page and scrapes those too |         1        |
 | StringCleaner                                     | Performs common string-cleaning operations to a text string, also allowing them to be chained in sequence    |         1        |
 | upload_file_python_to_gcloud_bucket               | Writes an object in python memory to a file (blob) on a google cloud bucket                                  |         4        |
 | url_to_filename_to_url_mapper                     | Converts a webpage URL into a useable filename, where the URL can be recovered directly from the filename    |         2        |
 | view_nested_dict_structure                        | Generates a simple printout for understanding the structure of a complex nested python dictionary            |         4        |
 | write_pandas_df_to_google_bigquery_table          | Writes a pandas dataframe to a table on Google BigQuery                                                      |         4        |
 
 ## API and Web
 
 ```python
 import joes_giant_toolbox.web
+
 help( joes_giant_toolbox.web.anonymous_view_public_linkedin_page )
 help( joes_giant_toolbox.web.duckduckgo_search_multipage )
 help( joes_giant_toolbox.web.make_url_request )
 help( joes_giant_toolbox.web.scrape_webpage_and_all_linked_webpages )
-help( joes_giant_toolbox.web.url_to_filename_to_url_mapper ) 
+help( joes_giant_toolbox.web.url_to_filename_to_url_mapper )
 ```
 
 | Name                                                     | Description                                                                                                  | Confidence Score |
 |----------------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | anonymous_view_public_linkedin_page                      | Extracts the information (HTML) from a public LinkedIn page (e.g. person or company) using a virtual browser |         2        |
 | duckduckgo_search_multipage                              | Fetches search results from the DuckDuckGo Lite search engine                                                |         2        |
 | make_url_request                                         | A convenience function for making API requests using the urllib library                                      |         3        |
-| scrape_webpage_and_all_linked_webpages                   | Extracts HTML from given web page, and also follows all of the hyperlinks on that page and scrapes those too |         1        | 
+| scrape_webpage_and_all_linked_webpages                   | Extracts HTML from given web page, and also follows all of the hyperlinks on that page and scrapes those too |         1        |
 | url_to_filename_to_url_mapper                            | Converts a webpage URL into a useable filename, where the URL can be recovered directly from the filename    |         2        |
 
 ## Data Visualisation
 
 ```python
 import joes_giant_toolbox.dataviz
+
 help( joes_giant_toolbox.dataviz )
+
 help( joes_giant_toolbox.dataviz.ascii_density_histogram )
 help( joes_giant_toolbox.dataviz.PythonPlottingTutorials )
 help( joes_giant_toolbox.dataviz.view_nested_dict_structure )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | ascii_density_histogram                           | Draws a histogram using only raw text symbols                                                                |         2        |
 | PythonPlottingTutorials                           | Example code snippets for creating common data visualisations in python                                      |         4        |
 | view_nested_dict_structure                        | Generates a simple printout for understanding the structure of a complex nested python dictionary            |         4        |
 
 ## Google Cloud
-
+To additionally install the package dependencies of this module:
 ```bash
 pip install joes-giant-toolbox[google]
 ```
 
 ```python
 import joes_giant_toolbox.google_cloud
 
 help(joes_giant_toolbox.google_cloud)
 
-help( joes_giant_toolbox.google_cloud.create_gcloud_vm_docker_template ) 
+help( joes_giant_toolbox.google_cloud.create_gcloud_vm_docker_template )
+help( joes_giant_toolbox.google_cloud.create_parallel_google_cloud_run_job_template )
 help( joes_giant_toolbox.google_cloud.delete_file_in_gcloud_bucket )
 help( joes_giant_toolbox.google_cloud.download_file_from_gcloud_bucket_to_python )
+help( joes_giant_toolbox.google_cloud.gcloud_vm_deletes_itself )
 help( joes_giant_toolbox.google_cloud.list_files_in_gcloud_bucket )
 help( joes_giant_toolbox.google_cloud.move_or_rename_file_in_gcloud_bucket )
 help( joes_giant_toolbox.google_cloud.query_bigquery_to_pandas_df )
 help( joes_giant_toolbox.google_cloud.upload_file_python_to_gcloud_bucket )
 help( joes_giant_toolbox.google_cloud.write_pandas_df_to_google_bigquery_table )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
-| create_gcloud_vm_docker_template | Creates a folder containing the files necessary to quickly build a python docker container to run on a google cloud Virtual Machine | 4
+| create_gcloud_vm_docker_template                  | Creates a folder containing the files necessary to quickly build a python docker container to run on a google cloud Virtual Machine | 4
+| create_parallel_google_cloud_run_job_template     | Run a task in parallel using a Google Cloud Run job (code-generating function)| 2 |
 | delete_file_in_gcloud_bucket                      | Deletes a file which is in a google cloud bucket                                                             |         4        |
 | download_file_from_gcloud_bucket_to_python        | Reads a file from a google cloud bucket into python memory                                                   |         4        |
+| gcloud_vm_deletes_itself                          | Running this function on a google cloud Virtual Machine (VM) causes the VM to delete itself                  |         4        |
 | list_files_in_gcloud_bucket                       | Returns a list of the files present in a specified google cloud bucket                                       |         4        |
 | move_or_rename_file_in_gcloud_bucket              | Move or rename a file which is in a google cloud bucket (which includes moving it to a different bucket)     |         4        |
 | query_bigquery_to_pandas_df                       | Runs a query on Google BigQuery and writes the result into a local pandas.DataFrame                          |         4        |
 | upload_file_python_to_gcloud_bucket               | Writes an object in python memory to a file (blob) on a google cloud bucket                                  |         4        |
 | write_pandas_df_to_google_bigquery_table          | Writes a pandas dataframe to a table on Google BigQuery                                                      |         4        |
 
 ## Project Management
 ```python
 import joes_giant_toolbox.proj_mgmt
 help( joes_giant_toolbox.proj_mgmt.create_project_scope_doc )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
-| create_project_scope_doc                          | Creates a basic project scope document (markdown) by prompting the user for input                            |         3        | 
+| create_project_scope_doc                          | Creates a basic project scope document (markdown) by prompting the user for input                            |         3        |
 
 
-## Python Convenience Functions 
+## Python Convenience Functions
 ```python
 import joes_giant_toolbox.convenience
+
 help( joes_giant_toolbox.convenience.list_all_python_imports )
 help( joes_giant_toolbox.convenience.print_progress_bar )
 help( joes_giant_toolbox.convenience.run_python_function_in_parallel )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | list_all_python_imports                           | Searches every python script in a given folder and lists all python modules imported within those scripts    |         2        |
 | print_progress_bar                                | Prints a progress bar (to standard out) while code is running                                                |         3        |
 | run_python_function_in_parallel                   | Runs a python function in parallel on multiple cores or threads                                              |         4        |
 
-## Statistical Inference and Hypothesis Testing 
+## Statistical Inference and Hypothesis Testing
 ```python
 import joes_giant_toolbox.stats
+
 help( joes_giant_toolbox.stats )
+
 help( joes_giant_toolbox.stats.conjugate_prior_beta_binomial )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | conjugate_prior_beta_binomial                     | Calculates the posterior distribution of the success probability parameter [p] of a binomial distribution, from observed data and a user-specified beta prior | 4                |
 
-## Statistical Modelling and Machine Learning 
+## Statistical Modelling and Machine Learning
+```python
+import joes_giant_toolbox.maths
+
+help( joes_giant_toolbox.maths.cosine_similarity )
+```
+
 ```python
 import joes_giant_toolbox.sklearn
+
 help( joes_giant_toolbox.sklearn.RapidBinaryClassifier )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
+| cosine_similarity                                 | Calculates the cosine similarity between two 1-dimensional numpy arrays | 2 |
 | RapidBinaryClassifier                             | Ultra rapid generation of binary classifier models in scikit-learn by abstracting away a lot of the decisions and model code| 3 |
 
 ## Text and Natural Language Processing
-```python 
+```python
 import joes_giant_toolbox.text
+
 help( joes_giant_toolbox.text )
+
 help( joes_giant_toolbox.text.longest_sentence_subsequence_plagiarism_detector )
 help( joes_giant_toolbox.text.RegexRulesClassifier )
 help( joes_giant_toolbox.text.StringCleaner )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
```

### Comparing `joes_giant_toolbox-0.2.23/joes_giant_toolbox.egg-info/SOURCES.txt` & `joes_giant_toolbox-0.3.1/joes_giant_toolbox.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 joes_giant_toolbox/__init__.py
 joes_giant_toolbox/convenience.py
 joes_giant_toolbox/dataviz.py
 joes_giant_toolbox/google_cloud.py
+joes_giant_toolbox/maths.py
 joes_giant_toolbox/proj_mgmt.py
 joes_giant_toolbox/sklearn.py
 joes_giant_toolbox/stats.py
 joes_giant_toolbox/text.py
 joes_giant_toolbox/web.py
 joes_giant_toolbox.egg-info/PKG-INFO
 joes_giant_toolbox.egg-info/SOURCES.txt
@@ -16,20 +17,22 @@
 joes_giant_toolbox.egg-info/requires.txt
 joes_giant_toolbox.egg-info/top_level.txt
 joes_giant_toolbox/all/__init__.py
 joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py
 joes_giant_toolbox/all/ascii_density_histogram.py
 joes_giant_toolbox/all/compare_metric_to_prev_period.py
 joes_giant_toolbox/all/conjugate_prior_beta_binomial.py
+joes_giant_toolbox/all/cosine_similarity.py
 joes_giant_toolbox/all/create_gcloud_vm_docker_template.py
+joes_giant_toolbox/all/create_parallel_google_cloud_run_job_template.py
 joes_giant_toolbox/all/create_project_scope_doc.py
 joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py
 joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py
 joes_giant_toolbox/all/duckduckgo_search_multipage.py
-joes_giant_toolbox/all/gcloud_vm_kills_itself.py
+joes_giant_toolbox/all/gcloud_vm_deletes_itself.py
 joes_giant_toolbox/all/list_all_python_imports.py
 joes_giant_toolbox/all/list_files_in_gcloud_bucket.py
 joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py
 joes_giant_toolbox/all/make_url_request.py
 joes_giant_toolbox/all/manual_keyword_classifier.py
 joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py
 joes_giant_toolbox/all/print_progress_bar.py
```

### Comparing `joes_giant_toolbox-0.2.23/pyproject.toml` & `joes_giant_toolbox-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "joes_giant_toolbox"
-version = "0.2.23"
+version = "0.3.01"
 description = "A large collection of general python functions and classes that I use in my daily work"
 readme = "README.md"
 authors = [{ name = "Joseph Bolton", email = "joseph.jazz.bolton@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["api", "web", "dataviz", "google cloud", "project management", "convenience", "statistics", "hypothesis testing", "machine learning", "NLP"]
 dependencies = []
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
-all = ["black", "pytest"]
+dev = ["black", "pytest"]
 doc = ["m2r","sphinx"]
-google = ["db-dtypes==1.0.5", "google-cloud-bigquery-storage==2.18", "google-cloud-compute==1.10.0","google-cloud-logging==3.5.0","google-cloud-storage==2.7.0"]
+google = ["db-dtypes==1.0.5", "google-cloud-bigquery==3.4.1", "google-cloud-bigquery-storage==2.18", "google-cloud-compute==1.10.0","google-cloud-logging==3.5.0","google-cloud-storage==2.7.0"]
 
 [project.urls]
-Homepage = "https://github.com/J-sephB-lt-n/joes_giant_toolbox"
+Homepage = "https://github.com/J-sephB-lt-n/joes_giant_toolbox"
```

### Comparing `joes_giant_toolbox-0.2.23/tests/test_conjugate_prior_beta_binomial.py` & `joes_giant_toolbox-0.3.1/tests/test_conjugate_prior_beta_binomial.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/tests/test_longest_sentence_subsequence_plagiarism_detector.py` & `joes_giant_toolbox-0.3.1/tests/test_longest_sentence_subsequence_plagiarism_detector.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/tests/test_make_url_request.py` & `joes_giant_toolbox-0.3.1/tests/test_make_url_request.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/tests/test_rapid_binary_classifier.py` & `joes_giant_toolbox-0.3.1/tests/test_rapid_binary_classifier.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.2.23/tests/test_string_cleaner.py` & `joes_giant_toolbox-0.3.1/tests/test_string_cleaner.py`

 * *Files identical despite different names*

