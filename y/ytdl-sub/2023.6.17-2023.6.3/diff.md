# Comparing `tmp/ytdl-sub-2023.6.17.tar.gz` & `tmp/ytdl-sub-2023.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdl-sub-2023.6.17.tar", last modified: Sat Jun 17 20:03:52 2023, max compression
+gzip compressed data, was "ytdl-sub-2023.6.3.tar", last modified: Sat Jun  3 14:43:38 2023, max compression
```

## Comparing `ytdl-sub-2023.6.17.tar` & `ytdl-sub-2023.6.3.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:52.010176 ytdl-sub-2023.6.17/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-06-17 20:03:52.010176 ytdl-sub-2023.6.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-17 20:03:52.010176 ytdl-sub-2023.6.17/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:51.982176 ytdl-sub-2023.6.17/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:51.986176 ytdl-sub-2023.6.17/src/ytdl_sub/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-17 20:03:31.000000 ytdl-sub-2023.6.17/src/ytdl_sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:51.986176 ytdl-sub-2023.6.17/src/ytdl_sub/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/cli/download_args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/cli/main_args_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:51.990176 ytdl-sub-2023.6.17/src/ytdl_sub/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/config/config_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/config/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/config/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/config/preset_class_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/config/preset_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:51.990176 ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/base_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:51.990176 ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/info_json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/info_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:51.994176 ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21911 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/url/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/url/multi_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/url/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/url/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/ytdl_options_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:51.994176 ytdl-sub-2023.6.17/src/ytdl_sub/entries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/entries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/entries/base_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/entries/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/entries/entry_parent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:51.994176 ytdl-sub-2023.6.17/src/ytdl_sub/entries/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/entries/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19114 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/entries/variables/entry_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/entries/variables/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:51.998176 ytdl-sub-2023.6.17/src/ytdl_sub/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/plugins/audio_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/plugins/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/plugins/date_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/plugins/file_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:51.998176 ytdl-sub-2023.6.17/src/ytdl_sub/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/plugins/internal/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/plugins/match_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/plugins/music_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/plugins/nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/plugins/output_directory_nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/plugins/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/plugins/split_by_chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/plugins/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/plugins/video_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:51.998176 ytdl-sub-2023.6.17/src/ytdl_sub/prebuilt_presets/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/prebuilt_presets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:51.998176 ytdl-sub-2023.6.17/src/ytdl_sub/prebuilt_presets/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:51.998176 ytdl-sub-2023.6.17/src/ytdl_sub/prebuilt_presets/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/prebuilt_presets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/prebuilt_presets/internal/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:52.002176 ytdl-sub-2023.6.17/src/ytdl_sub/prebuilt_presets/tv_show/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:52.002176 ytdl-sub-2023.6.17/src/ytdl_sub/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/subscriptions/base_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/subscriptions/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/subscriptions/subscription_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:52.002176 ytdl-sub-2023.6.17/src/ytdl_sub/thread/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/thread/log_entries_downloaded_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:52.006176 ytdl-sub-2023.6.17/src/ytdl_sub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/utils/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/utils/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/utils/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/utils/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/utils/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:52.010176 ytdl-sub-2023.6.17/src/ytdl_sub/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/validators/audo_codec_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/validators/file_path_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/validators/nfo_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/validators/source_variable_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/validators/strict_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/validators/string_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/validators/string_formatter_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/validators/string_select_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:52.010176 ytdl-sub-2023.6.17/src/ytdl_sub/ytdl_additions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/ytdl_additions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-06-17 20:03:30.000000 ytdl-sub-2023.6.17/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:03:51.986176 ytdl-sub-2023.6.17/src/ytdl_sub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-06-17 20:03:51.000000 ytdl-sub-2023.6.17/src/ytdl_sub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-17 20:03:51.000000 ytdl-sub-2023.6.17/src/ytdl_sub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 20:03:51.000000 ytdl-sub-2023.6.17/src/ytdl_sub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-17 20:03:51.000000 ytdl-sub-2023.6.17/src/ytdl_sub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-17 20:03:51.000000 ytdl-sub-2023.6.17/src/ytdl_sub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 20:03:51.000000 ytdl-sub-2023.6.17/src/ytdl_sub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.665356 ytdl-sub-2023.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10691 2023-06-03 14:43:38.669356 ytdl-sub-2023.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-03 14:43:38.669356 ytdl-sub-2023.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.641356 ytdl-sub-2023.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.645356 ytdl-sub-2023.6.3/src/ytdl_sub/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.649356 ytdl-sub-2023.6.3/src/ytdl_sub/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/cli/download_args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/cli/main_args_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.649356 ytdl-sub-2023.6.3/src/ytdl_sub/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/config/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/config/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/config/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/config/preset_class_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/config/preset_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.653356 ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/base_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.653356 ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/info_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/info_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.653356 ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21911 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/url/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/url/multi_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/url/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/url/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/ytdl_options_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.653356 ytdl-sub-2023.6.3/src/ytdl_sub/entries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/entries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/entries/base_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/entries/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/entries/entry_parent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.653356 ytdl-sub-2023.6.3/src/ytdl_sub/entries/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/entries/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19114 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/entries/variables/entry_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/entries/variables/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.657356 ytdl-sub-2023.6.3/src/ytdl_sub/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/plugins/audio_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/plugins/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/plugins/date_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/plugins/file_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.657356 ytdl-sub-2023.6.3/src/ytdl_sub/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/plugins/internal/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/plugins/match_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/plugins/music_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/plugins/nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/plugins/output_directory_nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16806 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/plugins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/plugins/split_by_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/plugins/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/plugins/video_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.657356 ytdl-sub-2023.6.3/src/ytdl_sub/prebuilt_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/prebuilt_presets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.657356 ytdl-sub-2023.6.3/src/ytdl_sub/prebuilt_presets/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.657356 ytdl-sub-2023.6.3/src/ytdl_sub/prebuilt_presets/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/prebuilt_presets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/prebuilt_presets/internal/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.661356 ytdl-sub-2023.6.3/src/ytdl_sub/prebuilt_presets/tv_show/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.661356 ytdl-sub-2023.6.3/src/ytdl_sub/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/subscriptions/base_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/subscriptions/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/subscriptions/subscription_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.661356 ytdl-sub-2023.6.3/src/ytdl_sub/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/thread/log_entries_downloaded_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.665356 ytdl-sub-2023.6.3/src/ytdl_sub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/utils/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/utils/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/utils/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/utils/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/utils/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.665356 ytdl-sub-2023.6.3/src/ytdl_sub/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/validators/audo_codec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/validators/file_path_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/validators/nfo_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/validators/source_variable_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/validators/strict_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/validators/string_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/validators/string_formatter_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/validators/string_select_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.665356 ytdl-sub-2023.6.3/src/ytdl_sub/ytdl_additions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/ytdl_additions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-06-03 14:43:17.000000 ytdl-sub-2023.6.3/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:43:38.649356 ytdl-sub-2023.6.3/src/ytdl_sub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10691 2023-06-03 14:43:38.000000 ytdl-sub-2023.6.3/src/ytdl_sub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-03 14:43:38.000000 ytdl-sub-2023.6.3/src/ytdl_sub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 14:43:38.000000 ytdl-sub-2023.6.3/src/ytdl_sub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-03 14:43:38.000000 ytdl-sub-2023.6.3/src/ytdl_sub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-03 14:43:38.000000 ytdl-sub-2023.6.3/src/ytdl_sub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 14:43:38.000000 ytdl-sub-2023.6.3/src/ytdl_sub.egg-info/top_level.txt
```

### Comparing `ytdl-sub-2023.6.17/LICENSE` & `ytdl-sub-2023.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/PKG-INFO` & `ytdl-sub-2023.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.6.17
+Version: 2023.6.3
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.6.17/README.md` & `ytdl-sub-2023.6.3/README.md`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/pyproject.toml` & `ytdl-sub-2023.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/setup.cfg` & `ytdl-sub-2023.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/cli/download_args_parser.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/cli/download_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/cli/main.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/cli/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/cli/main_args_parser.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/cli/main_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/config/config_file.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/config/config_file.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/config/config_validator.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/config/config_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/config/preset.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/config/preset.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/config/preset_class_mappings.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/config/preset_class_mappings.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/config/preset_options.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/config/preset_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/base_downloader.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/base_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/info_json/info_json_downloader.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/info_json/info_json_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/url/downloader.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/url/downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/url/multi_url.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/url/multi_url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/url/url.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/url/url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/url/validators.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/url/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/ytdl_options_builder.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/ytdl_options_builder.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/downloaders/ytdlp.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/downloaders/ytdlp.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/entries/base_entry.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/entries/base_entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/entries/entry.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/entries/entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/entries/entry_parent.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/entries/entry_parent.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/entries/variables/entry_variables.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/entries/variables/entry_variables.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/entries/variables/kwargs.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/entries/variables/kwargs.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/main.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/plugins/audio_extract.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/plugins/audio_extract.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/plugins/chapters.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/plugins/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/plugins/date_range.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/plugins/date_range.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/plugins/file_convert.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/plugins/file_convert.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/plugins/internal/view.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/plugins/internal/view.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/plugins/match_filters.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/plugins/match_filters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/plugins/music_tags.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/plugins/music_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/plugins/nfo_tags.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/plugins/nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/plugins/output_directory_nfo_tags.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/plugins/output_directory_nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/plugins/plugin.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/plugins/regex.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/plugins/regex.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,27 +7,26 @@
 
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.entries.variables.kwargs import YTDL_SUB_REGEX_SOURCE_VARS
 from ytdl_sub.plugins.plugin import Plugin
 from ytdl_sub.plugins.plugin import PluginOptions
 from ytdl_sub.plugins.plugin import PluginPriority
 from ytdl_sub.utils.exceptions import RegexNoMatchException
-from ytdl_sub.utils.exceptions import StringFormattingVariableNotFoundException
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.validators.regex_validator import RegexListValidator
 from ytdl_sub.validators.source_variable_validator import SourceVariableNameListValidator
 from ytdl_sub.validators.strict_dict_validator import StrictDictValidator
 from ytdl_sub.validators.string_formatter_validators import ListFormatterValidator
 from ytdl_sub.validators.string_formatter_validators import StringFormatterValidator
 from ytdl_sub.validators.validators import BoolValidator
 
 logger = Logger.get(name="regex")
 
 
-class VariableRegex(StrictDictValidator):
+class SourceVariableRegex(StrictDictValidator):
 
     _optional_keys = {"match", "exclude", "capture_group_defaults", "capture_group_names"}
 
     def __init__(self, name, value):
         super().__init__(name, value)
         self._match = self._validate_key_if_present(key="match", validator=RegexListValidator)
         self._exclude = self._validate_key_if_present(key="exclude", validator=RegexListValidator)
@@ -62,26 +61,25 @@
                 f"number of capture group names must match number of capture groups, "
                 f"{len(self._capture_group_names.list)} != {self._match.num_capture_groups}"
             )
 
     @property
     def match(self) -> Optional[RegexListValidator]:
         """
-        List of regex strings to try to match against a source or override variable. Each regex
+        List of regex strings to try to match against a source variable. Each regex
         string must have the same number of capture groups.
         """
         return self._match
 
     @property
     def exclude(self) -> Optional[RegexListValidator]:
         """
-        List of regex strings to try to match against a source or override variable. If one of the
-        regex strings match, then the entry will be skipped. If both ``exclude`` and ``match`` are
-        specified, entries will get skipped if the regex matches against both ``exclude`` and
-        ``match``.
+        List of regex strings to try to match against a source variable. If one of the regex strings
+        match, then the entry will be skipped. If both ``exclude`` and ``match`` are specified,
+        entries will get skipped if the regex matches against both ``exclude`` and ``match``.
         """
         return self._exclude
 
     @property
     def capture_group_names(self) -> Optional[List[str]]:
         """
         Optional (only when no capture groups are in the regex string). List of names to store the
@@ -112,33 +110,27 @@
 class FromSourceVariablesRegex(StrictDictValidator):
 
     _optional_keys = Entry.source_variables()
     _allow_extra_keys = True
 
     def __init__(self, name, value):
         super().__init__(name, value)
-        self.variable_capture_dict: Dict[str, VariableRegex] = {
-            key: self._validate_key(key=key, validator=VariableRegex) for key in self._keys
+        self.source_variable_capture_dict: Dict[str, SourceVariableRegex] = {
+            key: self._validate_key(key=key, validator=SourceVariableRegex) for key in self._keys
         }
 
 
 class RegexOptions(PluginOptions):
     r"""
-    Performs regex matching on an entry's source or override variables. Regex can be used to filter
-    entries from proceeding with download or capture groups to create new source variables. NOTE to
+    Performs regex matching on an entry's source variables. Regex can be used to filter entries
+    from proceeding with download or capture groups to create new source variables. NOTE to
     use backslashes anywhere in your regex, i.e. ``\d``, you must add another backslash escape. This
     means ``\d`` should be written as ``\\d``. This is because YAML requires an escape for any
     backslash usage.
 
-    If you want to regex-search multiple source variables to create a logical OR effect, you can
-    create an override variable that contains the concatenation of them, and search that with regex.
-    For example, creating the override variable ``"title_and_description": "{title} {description}"``
-    and using ``title_and_description`` can regex match/exclude from either ``title`` or
-    ``description``.
-
     Usage:
 
     .. code-block:: yaml
 
        presets:
          my_example_preset:
            regex:
@@ -220,17 +212,17 @@
         source_variables
             Available source variables when running the plugin
         override_variables
             Available override variables when running the plugin
         """
         for key, regex_options in self.source_variable_capture_dict.items():
             # Ensure each variable getting captured is a source variable
-            if key not in source_variables and key not in override_variables:
+            if key not in source_variables:
                 raise self._validation_exception(
-                    f"cannot regex capture '{key}' because it is not a source or override variable"
+                    f"cannot regex capture '{key}' because it is not a source variable"
                 )
 
             # Ensure the capture group names are not existing source/override variables
             for capture_group_name in regex_options.capture_group_names:
                 if capture_group_name in source_variables:
                     raise self._validation_exception(
                         f"'{capture_group_name}' cannot be used as a capture group name because it "
@@ -239,21 +231,21 @@
                 if capture_group_name in override_variables:
                     raise self._validation_exception(
                         f"'{capture_group_name}' cannot be used as a capture group name because it "
                         f"is an override variable"
                     )
 
     @property
-    def source_variable_capture_dict(self) -> Dict[str, VariableRegex]:
+    def source_variable_capture_dict(self) -> Dict[str, SourceVariableRegex]:
         """
         Returns
         -------
         Dict of { source variable: capture options }
         """
-        return self._from.variable_capture_dict
+        return self._from.source_variable_capture_dict
 
     def added_source_variables(self) -> List[str]:
         """
         Returns
         -------
         List of new source variables created via regex capture
         """
@@ -271,64 +263,36 @@
 class RegexPlugin(Plugin[RegexOptions]):
     plugin_options_type = RegexOptions
     priority = PluginPriority(
         modify_entry=PluginPriority.MODIFY_ENTRY_AFTER_SPLIT + 0,
     )
 
     @classmethod
-    def _add_processed_regex_variable_name(cls, entry: Entry, source_var: str) -> None:
+    def _add_processed_regex_source_var(cls, entry: Entry, source_var: str) -> None:
         if not entry.kwargs_contains(YTDL_SUB_REGEX_SOURCE_VARS):
             entry.add_kwargs({YTDL_SUB_REGEX_SOURCE_VARS: []})
 
         entry.kwargs(YTDL_SUB_REGEX_SOURCE_VARS).append(source_var)
 
     @classmethod
-    def _contains_processed_regex_variable(cls, entry: Entry, variable_name: str) -> bool:
-        return variable_name in entry.kwargs_get(YTDL_SUB_REGEX_SOURCE_VARS, [])
+    def _contains_processed_regex_source_var(cls, entry: Entry, source_var: str) -> bool:
+        return source_var in entry.kwargs_get(YTDL_SUB_REGEX_SOURCE_VARS, [])
 
-    def _try_skip_entry(self, entry: Entry, variable_name: str) -> None:
+    def _try_skip_entry(self, entry: Entry, source_var: str) -> None:
         # Skip the entry if toggled
         if self.plugin_options.skip_if_match_fails:
             logger.info(
                 "Regex failed to match '%s' from '%s', skipping.",
-                variable_name,
+                source_var,
                 entry.title,
             )
             return None
 
         # Otherwise, error
-        raise RegexNoMatchException(f"Regex failed to match '{variable_name}' from '{entry.title}'")
-
-    def _can_process_at_metadata_stage(self, entry: Entry, variable_name: str) -> bool:
-        # If the variable is an override...
-        if variable_name in self.overrides.dict:
-            # Try to see if it can resolve
-            try:
-                self.overrides.apply_formatter(
-                    formatter=self.overrides.dict[variable_name],
-                    entry=entry,
-                )
-            # If it can not from missing variables (from post-metadata stage), return False
-            except StringFormattingVariableNotFoundException:
-                return False
-        # If it is a source variable and not present, return false
-        elif variable_name not in entry.to_dict():
-            return False
-
-        return True
-
-    def _get_regex_input_string(self, entry: Entry, variable_name: str) -> str:
-        # Apply override formatter if it's an override
-        if variable_name in self.overrides.dict:
-            return self.overrides.apply_formatter(
-                formatter=self.overrides.dict[variable_name],
-                entry=entry,
-            )
-        # Otherwise pluck from the entry's source variable
-        return entry.to_dict()[variable_name]
+        raise RegexNoMatchException(f"Regex failed to match '{source_var}' from '{entry.title}'")
 
     def _modify_entry_metadata(self, entry: Entry, is_metadata_stage: bool) -> Optional[Entry]:
         """
         Parameters
         ----------
         entry
             Entry to add source variables to
@@ -340,58 +304,54 @@
         Entry with regex capture variables added to its source variables
 
         Raises
         ------
         ValidationException
             If no capture and no defaults
         """
+        entry_variable_dict = entry.to_dict()
+
         # Iterate each source var to capture and add to the entry
-        for (
-            variable_name,
-            regex_options,
-        ) in self.plugin_options.source_variable_capture_dict.items():
+        for source_var, regex_options in self.plugin_options.source_variable_capture_dict.items():
 
             # Record which regex source variables are processed, to
             # process as many variables as possible in the metadata stage, then the rest
             # after the media file has been downloaded.
-            if self._contains_processed_regex_variable(entry, variable_name):
+            if self._contains_processed_regex_source_var(entry, source_var):
                 continue
 
-            # If it's the metadata stage, and it can't be processed, skip until post-metadata
-            if is_metadata_stage and not self._can_process_at_metadata_stage(
-                entry=entry, variable_name=variable_name
-            ):
+            # Continue if the source var isn't in the dict since entry variables could be added
+            # after the metadata stage
+            if is_metadata_stage and source_var not in entry_variable_dict:
                 continue
 
-            self._add_processed_regex_variable_name(entry, variable_name)
-
-            regex_input_str = self._get_regex_input_string(
-                entry=entry,
-                variable_name=variable_name,
-            )
+            self._add_processed_regex_source_var(entry, source_var)
 
             if (
                 regex_options.exclude is not None
-                and regex_options.exclude.match_any(input_str=regex_input_str) is not None
+                and regex_options.exclude.match_any(input_str=entry_variable_dict[source_var])
+                is not None
             ):
-                return self._try_skip_entry(entry=entry, variable_name=variable_name)
+                return self._try_skip_entry(entry=entry, source_var=source_var)
 
             # If match is present
             if regex_options.match is not None:
-                maybe_capture = regex_options.match.match_any(input_str=regex_input_str)
+                maybe_capture = regex_options.match.match_any(
+                    input_str=entry_variable_dict[source_var]
+                )
 
                 # And nothing matched
                 if maybe_capture is None:
                     # and no defaults
                     if not regex_options.has_defaults:
-                        return self._try_skip_entry(entry=entry, variable_name=variable_name)
+                        return self._try_skip_entry(entry=entry, source_var=source_var)
 
                     # otherwise, use defaults (apply them using the original entry source dict)
                     source_variables_and_overrides_dict = dict(
-                        entry.to_dict(), **self.overrides.dict_with_format_strings
+                        entry_variable_dict, **self.overrides.dict_with_format_strings
                     )
 
                     # add both the default...
                     entry.add_variables(
                         variables_to_add={
                             regex_options.capture_group_names[i]: default.apply_formatter(
                                 variable_dict=source_variables_and_overrides_dict
```

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/plugins/split_by_chapters.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/plugins/split_by_chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/plugins/subtitles.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/plugins/subtitles.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/plugins/video_tags.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/plugins/video_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/prebuilt_presets/__init__.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/prebuilt_presets/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/prebuilt_presets/helpers/__init__.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/prebuilt_presets/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml` & `ytdl-sub-2023.6.3/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml` & `ytdl-sub-2023.6.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml` & `ytdl-sub-2023.6.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/subscriptions/base_subscription.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/subscriptions/base_subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/subscriptions/subscription.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/subscriptions/subscription_download.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/subscriptions/subscription_download.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/subscriptions/subscription_ytdl_options.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/subscriptions/subscription_ytdl_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/thread/log_entries_downloaded_listener.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/thread/log_entries_downloaded_listener.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/utils/chapters.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/utils/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/utils/datetime.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/utils/exceptions.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/utils/ffmpeg.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/utils/file_handler.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/utils/file_lock.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/utils/file_lock.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/utils/logger.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/utils/retry.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/utils/retry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/utils/thumbnail.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/utils/thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/utils/xml.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/utils/xml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/utils/yaml.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/validators/audo_codec_validator.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/validators/audo_codec_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/validators/file_path_validators.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/validators/file_path_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/validators/nfo_validators.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/validators/nfo_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/validators/regex_validator.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/validators/source_variable_validator.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/validators/source_variable_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/validators/strict_dict_validator.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/validators/strict_dict_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/validators/string_datetime.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/validators/string_datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/validators/string_formatter_validators.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/validators/string_formatter_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/validators/string_select_validator.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/validators/string_select_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/validators/validators.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/validators/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py` & `ytdl-sub-2023.6.3/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub.egg-info/PKG-INFO` & `ytdl-sub-2023.6.3/src/ytdl_sub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.6.17
+Version: 2023.6.3
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.6.17/src/ytdl_sub.egg-info/SOURCES.txt` & `ytdl-sub-2023.6.3/src/ytdl_sub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

