# Comparing `tmp/hyfi-0.7.0.tar.gz` & `tmp/hyfi-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-0.7.0.tar", max compression
+gzip compressed data, was "hyfi-0.7.1.tar", max compression
```

## Comparing `hyfi-0.7.0.tar` & `hyfi-0.7.1.tar`

### file list

```diff
@@ -1,85 +1,83 @@
--rw-r--r--   0        0        0     1071 2023-06-16 11:04:36.665550 hyfi-0.7.0/LICENSE
--rw-r--r--   0        0        0     1828 2023-06-16 11:04:36.665550 hyfi-0.7.0/README.md
--rw-r--r--   0        0        0     4592 2023-06-16 11:05:00.213687 hyfi-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3804 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     2544 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/__click__.py
--rw-r--r--   0        0        0      598 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/__global__/__init__.py
--rw-r--r--   0        0        0     9601 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/__global__/config.py
--rw-r--r--   0        0        0      417 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-06-16 11:05:00.145686 hyfi-0.7.0/src/hyfi/_version.py
--rw-r--r--   0        0        0      777 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     3182 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     6832 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0     1206 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/common.py
--rw-r--r--   0        0        0     1923 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/file_lock.py
--rw-r--r--   0        0        0     3440 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1244 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/util.py
--rw-r--r--   0        0        0      464 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/cached_path/_cached_path/version.py
--rw-r--r--   0        0        0        0 2023-06-16 11:04:36.669550 hyfi-0.7.0/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-06-16 11:05:00.145686 hyfi-0.7.0/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      407 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       49 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      141 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0      320 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      559 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      725 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      291 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      967 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/mode/debug.yaml
--rw-r--r--   0        0        0       61 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0      120 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0     1719 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      609 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      806 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0      121 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      130 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0     6369 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/graphic/__init__.py
--rw-r--r--   0        0        0     8395 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/graphic/collage.py
--rw-r--r--   0        0        0     4330 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/graphic/motion.py
--rw-r--r--   0        0        0     2497 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/graphic/plot.py
--rw-r--r--   0        0        0     3331 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/graphic/utils.py
--rw-r--r--   0        0        0     5886 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/hydra/__init__.py
--rw-r--r--   0        0        0    12854 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/hydra/main.py
--rw-r--r--   0        0        0     3480 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     2099 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    16589 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0     2086 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/joblib/pipe.py
--rw-r--r--   0        0        0    30681 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      217 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     2903 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     5743 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/path/batch.py
--rw-r--r--   0        0        0     5566 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/py.typed
--rw-r--r--   0        0        0        0 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/tasks/__init__.py
--rw-r--r--   0        0        0     4920 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/tasks/base.py
--rw-r--r--   0        0        0     5289 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/tasks/batch.py
--rw-r--r--   0        0        0        0 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0     5668 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/env.py
--rw-r--r--   0        0        0    12472 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/file.py
--rw-r--r--   0        0        0     9920 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/func.py
--rw-r--r--   0        0        0     1114 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/google.py
--rw-r--r--   0        0        0     3699 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/gpu.py
--rw-r--r--   0        0        0     4145 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/lib.py
--rw-r--r--   0        0        0     1986 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0     9766 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/notebook.py
--rw-r--r--   0        0        0     5476 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/tools.py
--rw-r--r--   0        0        0      232 2023-06-16 11:04:36.673550 hyfi-0.7.0/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 hyfi-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-17 08:06:19.610584 hyfi-0.7.1/LICENSE
+-rw-r--r--   0        0        0     1828 2023-06-17 08:06:19.610584 hyfi-0.7.1/README.md
+-rw-r--r--   0        0        0     4592 2023-06-17 08:06:42.867187 hyfi-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3804 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     2544 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      647 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/__global__/__init__.py
+-rw-r--r--   0        0        0     9856 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/__global__/config.py
+-rw-r--r--   0        0        0      735 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-17 08:06:42.799185 hyfi-0.7.1/src/hyfi/_version.py
+-rw-r--r--   0        0        0      777 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     3182 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     6832 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0     1206 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/common.py
+-rw-r--r--   0        0        0     1923 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/file_lock.py
+-rw-r--r--   0        0        0     3440 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1244 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/version.py
+-rw-r--r--   0        0        0        0 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-17 08:06:42.799185 hyfi-0.7.1/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      407 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      141 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0      320 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      559 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      725 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      291 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      948 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/mode/debug.yaml
+-rw-r--r--   0        0        0       61 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0      120 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0     1719 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      609 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      806 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      121 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      130 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0     6369 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0     3045 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8396 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4330 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     5966 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0    21338 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/hydra/__init__.py
+-rw-r--r--   0        0        0     7618 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/hydra/main.py
+-rw-r--r--   0        0        0     3487 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     2099 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    16589 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0     2579 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/joblib/pipe.py
+-rw-r--r--   0        0        0    30690 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      217 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     2903 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     5743 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0     5564 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/py.typed
+-rw-r--r--   0        0        0     4907 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     5239 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0     5667 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/env.py
+-rw-r--r--   0        0        0    12630 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/file.py
+-rw-r--r--   0        0        0     9920 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/func.py
+-rw-r--r--   0        0        0     1114 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/google.py
+-rw-r--r--   0        0        0     3699 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/gpu.py
+-rw-r--r--   0        0        0     4162 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/lib.py
+-rw-r--r--   0        0        0     1986 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0     9766 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/notebook.py
+-rw-r--r--   0        0        0     5476 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/tools.py
+-rw-r--r--   0        0        0      232 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 hyfi-0.7.1/PKG-INFO
```

### Comparing `hyfi-0.7.0/LICENSE` & `hyfi-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/README.md` & `hyfi-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/pyproject.toml` & `hyfi-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "0.7.0"
+version = "0.7.1"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-0.7.0/src/hyfi/__cli__.py` & `hyfi-0.7.1/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/__click__.py` & `hyfi-0.7.1/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/__global__/__init__.py` & `hyfi-0.7.1/src/hyfi/__global__/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from hyfi.about import AboutConfig
 from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 __hydra_version_base__ = "1.2"
+__hydra_default_config_group_value__ = "default"
 
 __about__ = AboutConfig()
 
 
 class HydraConfig(BaseModel):
     """HyFI config primary class"""
```

### Comparing `hyfi-0.7.0/src/hyfi/__global__/config.py` & `hyfi-0.7.1/src/hyfi/__global__/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 Hyfi configuration file.
 """
+import os
 from typing import Any, Dict, Optional, Union
 
 from omegaconf import DictConfig
 from pydantic import BaseModel, root_validator, validator
 
 from hyfi.__global__ import __about__, __hydra_config__
 from hyfi.about import AboutConfig
 from hyfi.dotenv import DotEnvConfig
 from hyfi.hydra import _compose
 from hyfi.project import ProjectConfig
-from hyfi.utils.env import _check_and_set_value, expand_posix_vars
+from hyfi.task import TaskConfig
+from hyfi.utils.env import check_and_set_osenv, expand_posix_vars
 from hyfi.utils.logging import getLogger, setLogger
 from hyfi.utils.notebook import load_extentions, set_matplotlib_formats
 
 logger = getLogger(__name__)
 
 
 def __version__():
@@ -43,60 +45,61 @@
     print_resolved_config: bool = False
     verbose: bool = False
     logging_level: str = "WARNING"
 
     hydra: Optional[DictConfig] = None
 
     about: AboutConfig = AboutConfig()
-    project: Optional[ProjectConfig] = None
     copier: Optional[DictConfig] = None
+    project: Optional[ProjectConfig] = None
+    task: Optional[TaskConfig] = None
 
     __version__: str = __version__()
     __initilized__: bool = False
 
     class Config:
         arbitrary_types_allowed = True
         underscore_attrs_are_private = True
         validate_assignment = True
         extra = "allow"
 
     @root_validator()
-    def _check_and_set_values(cls, values):
+    def _check_and_set_osenvs(cls, values):
         """
         Validate and set values for the config file.
 
         Args:
                 cls: Class to use for config lookup
                 values: Dictionary of values to check and set
 
         Returns:
                 Same dictionary with hyfi_config
         """
         key = "hyfi_config_path"
-        val = _check_and_set_value(key, values.get(key))
+        val = check_and_set_osenv(key, values.get(key))
         values[key] = val
         # Set the hyfi_config_module value in the configuration file.
         if val is not None:
             key = "hyfi_config_module"
-            values[key] = _check_and_set_value(key, val.replace("pkg://", ""))
+            values[key] = check_and_set_osenv(key, val.replace("pkg://", ""))
         return values
 
     @validator("hyfi_user_config_path")
     def _validate_hyfi_user_config_path(cls, v):
         """
         Validate and set hyfi_user_config_path.
 
         Args:
                 cls: Class to use for validation.
                 v: Value to set if valid.
 
         Returns:
                 True if valid False otherwise
         """
-        return _check_and_set_value("hyfi_user_config_path", v)
+        return check_and_set_osenv("hyfi_user_config_path", v)
 
     @validator("logging_level")
     def _validate_logging_level(cls, v, values):
         """
         Validate and set the logging level
 
         Args:
@@ -218,17 +221,15 @@
             config = _compose(
                 overrides=["+project=__init__"], config_module=__about__.config_module
             )
             logger.debug("Using default config.")
 
         # Skip project config initialization.
         if "project" not in config:
-            logger.info(
-                "No project config found, skip project config initialization."
-            )
+            logger.info("No project config found, skip project config initialization.")
             return
         self.project = ProjectConfig(**config["project"])
         self.project.init_project()
         # Initialize joblib backend if joblib is not set.
         if self.project.joblib:
             self.project.joblib.init_backend()
 
@@ -278,9 +279,21 @@
 
 
         Returns:
                 The version of the application
         """
         return self.about.version
 
+    @property
+    def dotenv(self):
+        return DotEnvConfig()
+
+    @property
+    def osenv(self):
+        return os.environ
+
 
 __global_config__ = HyfiConfig()
+
+
+def __search_package_path__():
+    return __global_config__.hyfi_config_path
```

### Comparing `hyfi-0.7.0/src/hyfi/about/__init__.py` & `hyfi-0.7.1/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/batch/__init__.py` & `hyfi-0.7.1/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/cached_path/__init__.py` & `hyfi-0.7.1/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/__init__.py` & `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/_cached_path.py` & `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/cache_file.py` & `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/common.py` & `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/file_lock.py` & `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/meta.py` & `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/progress.py` & `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/schemes/__init__.py` & `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/schemes/beaker.py` & `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/schemes/hf.py` & `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/schemes/http.py` & `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py` & `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/testing.py` & `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/cached_path/_cached_path/util.py` & `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/conf/copier/conf.yaml` & `hyfi-0.7.1/src/hyfi/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-0.7.1/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-0.7.1/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/conf/mode/__init__.yaml` & `hyfi-0.7.1/src/hyfi/conf/mode/__init__.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # @package _global_
 debug_mode: false
 print_config: false
 print_resolved_config: true
 verbose: false
 ignore_warnings: true
 logging_level: ${oc.env:HYFI_LOG_LEVEL,WARNING}
-project_name: ${oc.select:project.project_name, ${oc.select:task.project.project_name, ${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi-project}}}
-log_dir: ${oc.select:project.path.project_logs, ${oc.select:task.path.task_logs, ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}/logs}}}
+hydra_log_dir: ${oc.select:project.path.project_logs, ${oc.select:task.path.task_logs, ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}/logs}}/hydra
 
 hydra:
   job:
-    name: ${project_name}
+    name: ${oc.select:project.project_name, ${oc.select:task.project.project_name, ${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi-project}}}
     chdir: true
   run:
-    dir: ${log_dir}/hydra/${hydra.job.name}/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
+    dir: ${hydra_log_dir}/${hydra.job.name}/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
   sweep:
-    dir: ${log_dir}/hydra/${hydra.job.name}/multiruns/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
+    dir: ${hydra_log_dir}/${hydra.job.name}/multiruns/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
     subdir: ${hydra.job.num}
   verbose: false
   job_logging:
     handlers:
       console:
         level: ${hydra.job_logging.root.level}
       file:
```

### Comparing `hyfi-0.7.0/src/hyfi/conf/path/__init__.yaml` & `hyfi-0.7.1/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/conf/path/__task__.yaml` & `hyfi-0.7.1/src/hyfi/conf/path/__task__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/conf/project/__init__.yaml` & `hyfi-0.7.1/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/copier/__init__.py` & `hyfi-0.7.1/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/dotenv/__init__.py` & `hyfi-0.7.1/src/hyfi/dotenv/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,19 @@
             env_settings: SettingsSourceCallable,
             file_secret_settings: SettingsSourceCallable,
         ) -> Tuple[SettingsSourceCallable, ...]:
             load_dotenv()
             return env_settings, file_secret_settings, init_settings
 
     @root_validator()
-    def _check_and_set_values(cls, values):
+    def check_and_set_osenvs(cls, values):
         for k, v in values.items():
             if v is not None:
                 old_value = os.getenv(k.upper())
                 if old_value is None or old_value != str(v):
                     os.environ[k.upper()] = str(v)
                     logger.debug(f"Set environment variable {k.upper()}={v}")
         return values
+
+    @property
+    def os(self):
+        return os.environ
```

### Comparing `hyfi-0.7.0/src/hyfi/graphic/collage.py` & `hyfi-0.7.1/src/hyfi/graphics/collage.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import List
 
 import matplotlib.pyplot as plt
 import numpy as np
 from PIL import Image, ImageDraw
 from pydantic import BaseModel
 
-from hyfi.graphic.utils import get_image_font, load_image, load_images, scale_image
+from hyfi.graphics.utils import get_image_font, load_image, load_images, scale_image
 
 log = logging.getLogger(__name__)
 
 
 class Collage(BaseModel):
     """Collage of images."""
```

### Comparing `hyfi-0.7.0/src/hyfi/graphic/motion.py` & `hyfi-0.7.1/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/joblib/__init__.py` & `hyfi-0.7.1/src/hyfi/joblib/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,53 +62,53 @@
             backend_handle = None
             backend = self.distributed_framework.backend
 
             if backend == "dask":
                 from dask.distributed import Client  # type: ignore
 
                 dask_cfg = {"n_workers": self.distributed_framework.num_workers}
-                logger.info(f"initializing dask client with {dask_cfg}")
+                logger.debug(f"initializing dask client with {dask_cfg}")
                 client = Client(**dask_cfg)
                 logger.debug(client)
 
             elif backend == "ray":
                 import ray  # type: ignore
 
                 ray_cfg = {"num_cpus": self.distributed_framework.num_workers}
-                logger.info(f"initializing ray with {ray_cfg}")
+                logger.debug(f"initializing ray with {ray_cfg}")
                 ray.init(**ray_cfg)
                 backend_handle = ray
 
             batcher.batcher_instance = batcher.Batcher(
                 backend_handle=backend_handle, **self.batcher.dict()
             )
-            logger.info(f"initialized batcher with {batcher.batcher_instance}")
+            logger.debug(f"initialized batcher with {batcher.batcher_instance}")
         self.__initilized__ = True
 
     def stop_backend(self):
         """Stop the backend for joblib"""
         backend = self.distributed_framework.backend
         if batcher.batcher_instance:
-            logger.info("stopping batcher")
+            logger.debug("stopping batcher")
             del batcher.batcher_instance
 
-        logger.info("stopping distributed framework")
+        logger.debug("stopping distributed framework")
         if self.distributed_framework.initialize:
             if backend == "ray":
                 try:
                     import ray  # type: ignore
 
                     if ray.is_initialized():
                         ray.shutdown()
-                        logger.info("shutting down ray")
+                        logger.debug("shutting down ray")
                 except ImportError:
                     logger.warning("ray is not installed")
 
             elif backend == "dask":
                 try:
                     from dask.distributed import Client  # type: ignore
 
                     if Client.initialized():
                         Client.close()
-                        logger.info("shutting down dask client")
+                        logger.debug("shutting down dask client")
                 except ImportError:
                     logger.warning("dask is not installed")
```

### Comparing `hyfi-0.7.0/src/hyfi/joblib/batch/apply.py` & `hyfi-0.7.1/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-0.7.1/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/joblib/batch/batcher.py` & `hyfi-0.7.1/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/joblib/pipe.py` & `hyfi-0.7.1/src/hyfi/joblib/pipe.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,78 @@
+"""
+A class to apply a pipe to a dataframe or a dictionary of dataframes.
+"""
 from tqdm.auto import tqdm
 
-from hyfi.hydra.main import SpecialKeys, _partial
+from hyfi.hydra import SpecialKeys
+from hyfi.hydra.main import XC
 from hyfi.joblib.batch import batcher
 from hyfi.joblib.batch.apply import decorator_apply
 from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
-def _pipe(data, pipe):
-    _func_ = pipe.get(SpecialKeys.FUNC)
-    _fn = _partial(_func_)
-    logger.info("Applying pipe: %s", _fn)
-    if isinstance(data, dict):
-        if "concat_dataframes" in str(_fn):
-            return _fn(data, pipe)
-        dfs = {}
-        for df_no, df_name in enumerate(data):
-            df_each = data[df_name]
-
-            logger.info(
-                "Applying pipe to dataframe [%s], %d/%d", df_name, df_no + 1, len(data)
-            )
-
-            pipe[SpecialKeys.SUFFIX.value] = df_name
-            dfs[df_name] = _fn(df_each, pipe)
-        return dfs
-    return _fn(data, pipe)
-
-
-def _apply(
-    func,
-    series,
-    description=None,
-    use_batcher=True,
-    minibatch_size=None,
-    num_workers=None,
-    **kwargs,
-):
-    batcher_instance = batcher.batcher_instance
-    if use_batcher and batcher_instance is not None:
-        batcher_minibatch_size = batcher_instance.minibatch_size
-        if minibatch_size is None:
-            minibatch_size = batcher_minibatch_size
-        if num_workers is not None:
-            batcher_instance.procs = int(num_workers)
-        if batcher_instance.procs > 1:
-            batcher_instance.minibatch_size = min(
-                int(len(series) / batcher_instance.procs) + 1, minibatch_size
-            )
-            logger.info(
-                f"Using batcher with minibatch size: {batcher_instance.minibatch_size}"
-            )
-            results = decorator_apply(func, batcher_instance, description=description)(
-                series
-            )
-            if batcher_instance is not None:
-                batcher_instance.minibatch_size = batcher_minibatch_size
-            return results
-
-    if batcher_instance is None:
-        logger.info("Warning: batcher not initialized")
-    tqdm.pandas(desc=description)
-    return series.progress_apply(func)
+class PIPE:
+    """
+    A class to apply a pipe to a dataframe or a dictionary of dataframes.
+    """
+
+    @staticmethod
+    def pipe(data, pipe):
+        _func_ = pipe.get(SpecialKeys.FUNC)
+        _fn = XC.partial(_func_)
+        logger.info("Applying pipe: %s", _fn)
+        if isinstance(data, dict):
+            if "concat_dataframes" in str(_fn):
+                return _fn(data, pipe)
+            dfs = {}
+            for df_no, df_name in enumerate(data):
+                df_each = data[df_name]
+
+                logger.info(
+                    "Applying pipe to dataframe [%s], %d/%d",
+                    df_name,
+                    df_no + 1,
+                    len(data),
+                )
+
+                pipe[SpecialKeys.SUFFIX.value] = df_name
+                dfs[df_name] = _fn(df_each, pipe)
+            return dfs
+        return _fn(data, pipe)
+
+    @staticmethod
+    def apply(
+        func,
+        series,
+        description=None,
+        use_batcher=True,
+        minibatch_size=None,
+        num_workers=None,
+        **kwargs,
+    ):
+        batcher_instance = batcher.batcher_instance
+        if use_batcher and batcher_instance is not None:
+            batcher_minibatch_size = batcher_instance.minibatch_size
+            if minibatch_size is None:
+                minibatch_size = batcher_minibatch_size
+            if num_workers is not None:
+                batcher_instance.procs = int(num_workers)
+            if batcher_instance.procs > 1:
+                batcher_instance.minibatch_size = min(
+                    int(len(series) / batcher_instance.procs) + 1, minibatch_size
+                )
+                logger.info(
+                    f"Using batcher with minibatch size: {batcher_instance.minibatch_size}"
+                )
+                results = decorator_apply(
+                    func, batcher_instance, description=description
+                )(series)
+                if batcher_instance is not None:
+                    batcher_instance.minibatch_size = batcher_minibatch_size
+                return results
+
+        if batcher_instance is None:
+            logger.info("Warning: batcher not initialized")
+        tqdm.pandas(desc=description)
+        return series.progress_apply(func)
```

### Comparing `hyfi-0.7.0/src/hyfi/main/__init__.py` & `hyfi-0.7.1/src/hyfi/main/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,25 @@
 """
     This module contains the primary class for the hyfi config package, HyFI,
     as well as various utility functions and imports.
 """
-from pathlib import Path
+import os
+from pathlib import Path, PosixPath, WindowsPath
 from typing import IO, Any, Dict, List, Tuple, Union
 
+import pandas as pd
 from omegaconf import DictConfig, ListConfig, SCMode
 
 from hyfi.__global__ import __home_path__, __hyfi_path__
 from hyfi.__global__.config import __global_config__
 from hyfi.cached_path import cached_path
 from hyfi.dotenv import DotEnvConfig
-from hyfi.hydra import _compose, _select, _to_config, _to_dict
-from hyfi.hydra.main import (
-    DictKeyType,
-    SpecialKeys,
-    _ensure_kwargs,
-    _ensure_list,
-    _function,
-    _getsource,
-    _instantiate,
-    _is_config,
-    _is_instantiatable,
-    _is_list,
-    _load,
-    _load_json,
-    _merge,
-    _methods,
-    _partial,
-    _print,
-    _run,
-    _save,
-    _save_json,
-    _to_container,
-    _to_yaml,
-    _update,
-    _viewsource,
-)
-from hyfi.joblib.pipe import _apply, _pipe
+from hyfi.hydra import Composer, DictKeyType, SpecialKeys
+from hyfi.hydra.main import XC
+from hyfi.joblib.pipe import PIPE
 from hyfi.project import ProjectConfig
 from hyfi.utils.env import expand_posix_vars, get_osenv, load_dotenv, set_osenv
 from hyfi.utils.file import exists, is_dir, is_file, join_path, mkdir
 from hyfi.utils.func import (
     dict_product,
     dict_to_dataframe,
     records_to_dataframe,
@@ -109,19 +87,14 @@
 
     @staticmethod
     def terminate():
         """Terminate the global config"""
         __global_config__.terminate()
 
     @staticmethod
-    def envs() -> DotEnvConfig:
-        """Return the current environments"""
-        return DotEnvConfig()  # type: ignore
-
-    @staticmethod
     def expand_posix_vars(posix_expr: str, context: dict = None) -> str:  # type: ignore
         """
         Expand POSIX variables in a string.
 
         Args:
             posix_expr (str): The string containing POSIX variables to be expanded.
             context (dict, optional): A dictionary containing additional variables to be used in the expansion.
@@ -136,51 +109,64 @@
             >>> expand_posix_vars("$HOME/$USER", {"USER": "testuser"})
             '/home/user/testuser'
 
         """
         return expand_posix_vars(posix_expr, context=context)
 
     @staticmethod
-    def environ(key: str = "", default: Union[str, None] = None) -> Any:
+    def dotenv() -> DotEnvConfig:
+        """Return the DotEnvConfig"""
+        return DotEnvConfig()
+
+    @staticmethod
+    def osenv():
+        """Return the DotEnvConfig"""
+        return os.environ
+
+    @staticmethod
+    def get_osenv(key: str = "", default: Union[str, None] = None) -> Any:
         """Get the value of an environment variable or return the default value"""
         return get_osenv(key, default=default)
 
     @staticmethod
+    def set_osenv(key, value):
+        return set_osenv(key, value)
+
+    @staticmethod
     def compose(
         config_group: Union[str, None] = None,
         overrides: Union[List[str], None] = None,
         config_data: Union[Dict[str, Any], DictConfig, None] = None,
-        *,
         return_as_dict: bool = True,
         throw_on_resolution_failure: bool = True,
         throw_on_missing: bool = False,
         config_name: Union[str, None] = None,
         config_module: Union[str, None] = None,
         global_package: bool = False,
         verbose: bool = False,
     ) -> Union[DictConfig, Dict]:
         """
         Compose a configuration by applying overrides
 
         Args:
             config_group: Name of the config group to compose (`config_group=name`)
             overrides: List of config groups to apply overrides to (`overrides=["override_name"]`)
-            config_data: Keyword arguments to override config group values (will be converted to overrides of the form `config_group.key=value`)
+            config_data: Keyword arguments to override config group values (will be converted to overrides of the form `config_group_name.key=value`)
             return_as_dict: Return the result as a dict
             throw_on_resolution_failure: If True throw an exception if resolution fails
             throw_on_missing: If True throw an exception if config_group doesn't exist
             config_name: Name of the root config to be used (e.g. `hconf`)
             config_module: Module of the config to be used (e.g. `hyfi.conf`)
             global_package: If True, the config assumed to be a global package
             verbose: If True print configuration to stdout
 
         Returns:
             A config object or a dictionary with the composed config
         """
-        return _compose(
+        return Composer._compose(
             config_group=config_group,
             overrides=overrides,
             config_data=config_data,
             return_as_dict=return_as_dict,
             throw_on_resolution_failure=throw_on_resolution_failure,
             throw_on_missing=throw_on_missing,
             config_name=config_name,
@@ -194,93 +180,91 @@
         cfg: Any,
         key: str,
         *,
         default: Any = None,
         throw_on_resolution_failure: bool = True,
         throw_on_missing: bool = False,
     ):
-        return _select(
+        return Composer.select(
             cfg,
             key,
             default=default,
             throw_on_resolution_failure=throw_on_resolution_failure,
             throw_on_missing=throw_on_missing,
         )
 
     @staticmethod
     def to_dict(
         cfg: Any,
     ):
-        return _to_dict(cfg)
+        return Composer.to_dict(cfg)
 
     @staticmethod
     def to_config(
         cfg: Any,
     ):
-        return _to_config(cfg)
+        return Composer.to_config(cfg)
 
     @staticmethod
-    def to_yaml(cfg: Any, *, resolve: bool = False, sort_keys: bool = False) -> str:
-        if resolve:
-            cfg = _to_dict(cfg)
-        return _to_yaml(cfg, resolve=resolve, sort_keys=sort_keys)
+    def to_yaml(cfg: Any, resolve: bool = False, sort_keys: bool = False) -> str:
+        return Composer.to_yaml(cfg, resolve=resolve, sort_keys=sort_keys)
 
     @staticmethod
     def to_container(
         cfg: Any,
         *,
         resolve: bool = False,
         throw_on_missing: bool = False,
         enum_to_str: bool = False,
         structured_config_mode: SCMode = SCMode.DICT,
     ):
-        return _to_container(
+        return Composer.to_container(
             cfg=cfg,
             resolve=resolve,
             throw_on_missing=throw_on_missing,
             enum_to_str=enum_to_str,
             structured_config_mode=structured_config_mode,
         )
 
     @staticmethod
     def partial(
         config: Any = None,
         config_group: Union[str, None] = None,
         *args: Any,
         **kwargs: Any,
     ) -> Any:
-        return _partial(config=config, config_group=config_group, *args, **kwargs)
+        return XC.partial(config=config, config_group=config_group, *args, **kwargs)
 
     @staticmethod
     def instantiate(config: Any, *args: Any, **kwargs: Any) -> Any:
-        return _instantiate(config, *args, **kwargs)
+        return XC.instantiate(config, *args, **kwargs)
 
     @staticmethod
     def is_config(
         cfg: Any,
     ):
-        return _is_config(cfg)
+        return Composer.is_config(cfg)
 
     @staticmethod
     def is_list(
         cfg: Any,
     ):
-        return _is_list(cfg)
+        return Composer.is_list(cfg)
 
     @staticmethod
     def is_instantiatable(cfg: Any):
-        return _is_instantiatable(cfg)
+        return Composer.is_instantiatable(cfg)
 
     @staticmethod
     def load(file_: Union[str, Path, IO[Any]]) -> Union[DictConfig, ListConfig]:
-        return _load(file_)
+        return Composer.load(file_)
 
     @staticmethod
     def update(_dict, _overrides):
-        return _update(_dict, _overrides)
+        return Composer.update(_dict, _overrides)
 
     @staticmethod
     def merge(
         *configs: Union[
             DictConfig,
             ListConfig,
             Dict[DictKeyType, Any],
@@ -290,54 +274,54 @@
         ],
     ) -> Union[ListConfig, DictConfig]:
         """
         Merge a list of previously created configs into a single one
         :param configs: Input configs
         :return: the merged config object.
         """
-        return _merge(*configs)
+        return Composer.merge(*configs)
 
     @staticmethod
     def save(config: Any, f: Union[str, Path, IO[Any]], resolve: bool = False) -> None:
-        _save(config, f, resolve)
+        Composer.save(config, f, resolve)
 
     @staticmethod
     def save_json(
         json_dict: dict,
         f: Union[str, Path, IO[Any]],
         indent=4,
         ensure_ascii=False,
         default=None,
         **kwargs,
     ):
-        _save_json(json_dict, f, indent, ensure_ascii, default, **kwargs)
+        Composer.save_json(json_dict, f, indent, ensure_ascii, default, **kwargs)
 
     @staticmethod
     def load_json(f: Union[str, Path, IO[Any]], **kwargs) -> dict:
-        return _load_json(f, **kwargs)
+        return Composer.load_json(f, **kwargs)
 
     @staticmethod
     def pprint(cfg: Any, resolve: bool = True, **kwargs):
-        _print(cfg, resolve=resolve, **kwargs)
+        Composer.print(cfg, resolve=resolve, **kwargs)
 
     @staticmethod
     def print(cfg: Any, resolve: bool = True, **kwargs):
-        _print(cfg, resolve=resolve, **kwargs)
+        Composer.print(cfg, resolve=resolve, **kwargs)
 
     @staticmethod
     def methods(cfg: Any, obj: object, return_function=False):
-        return _methods(cfg, obj, return_function)
+        return Composer.methods(cfg, obj, return_function)
 
     @staticmethod
     def function(cfg: Any, _name_, return_function=False, **parms):
-        return _function(cfg, _name_, return_function, **parms)
+        return XC.function(cfg, _name_, return_function, **parms)
 
     @staticmethod
     def run(config: Any, **kwargs: Any) -> Any:
-        _run(config, **kwargs)
+        XC.run(config, **kwargs)
 
     @staticmethod
     def load_dotenv(
         override: bool = False,
         dotenv_dir: str = "",
         dotenv_filename: str = ".env",
         verbose: bool = False,
@@ -383,19 +367,19 @@
             return_parent_dir=return_parent_dir,
             cache_dir=cache_dir,
             verbose=verbose,
         )
 
     @staticmethod
     def pipe(data=None, cfg=None):
-        return _pipe(data, cfg)
+        return PIPE.pipe(data, cfg)
 
     @staticmethod
     def ensure_list(value):
-        return _ensure_list(value)
+        return Composer.ensure_list(value)
 
     @staticmethod
     def to_dateparm(_date, _format="%Y-%m-%d"):
         return to_dateparm(_date, _format)
 
     @staticmethod
     def exists(a, *p):
@@ -424,45 +408,43 @@
         description=None,
         use_batcher=True,
         minibatch_size=None,
         num_workers=None,
         verbose=False,
         **kwargs,
     ):
-        return _apply(
+        return PIPE.apply(
             func,
             series,
             description=description,
             use_batcher=use_batcher,
             minibatch_size=minibatch_size,
             num_workers=num_workers,
             verbose=verbose,
             **kwargs,
         )
 
     @staticmethod
     def ensure_kwargs(_kwargs, _fn):
-        return _ensure_kwargs(_kwargs, _fn)
+        return Composer.ensure_kwargs(_kwargs, _fn)
 
     @staticmethod
     def save_data(
-        data,
-        filename=None,
-        base_dir=None,
+        data: Union[pd.DataFrame, dict],
+        filename: str,
+        base_dir: str = "",
         columns=None,
-        index=False,
+        index: bool = False,
         filetype="parquet",
-        suffix=None,
-        verbose=False,
+        suffix: str = "",
+        verbose: bool = False,
         **kwargs,
     ):
         from hyfi.utils.file import save_data
 
-        if filename is None:
-            raise ValueError("filename must be specified")
         save_data(
             data,
             filename,
             base_dir=base_dir,
             columns=columns,
             index=index,
             filetype=filetype,
@@ -474,15 +456,15 @@
     @staticmethod
     def load_data(filename=None, base_dir=None, filetype=None, verbose=False, **kwargs):
         from hyfi.utils.file import load_data
 
         if filename is not None:
             filename = str(filename)
         if SpecialKeys.TARGET in kwargs:
-            return _instantiate(
+            return XC.instantiate(
                 kwargs,
                 filename=filename,
                 base_dir=base_dir,
                 verbose=verbose,
                 filetype=filetype,
             )
         if filename is None:
@@ -493,20 +475,22 @@
             verbose=verbose,
             filetype=filetype,
             **kwargs,
         )
 
     @staticmethod
     def get_filepaths(
-        filename_patterns=None, base_dir=None, recursive=True, verbose=True, **kwargs
+        filename_patterns: Union[str, PosixPath, WindowsPath],
+        base_dir: Union[str, PosixPath, WindowsPath] = "",
+        recursive: bool = True,
+        verbose: bool = False,
+        **kwargs,
     ):
         from hyfi.utils.file import get_filepaths
 
-        if filename_patterns is None:
-            raise ValueError("filename must be specified")
         return get_filepaths(
             filename_patterns,
             base_dir=base_dir,
             recursive=recursive,
             verbose=verbose,
             **kwargs,
         )
@@ -544,27 +528,25 @@
         return is_colab()
 
     @staticmethod
     def is_notebook():
         return is_notebook()
 
     @staticmethod
-    def osenv(key, default=None):
-        return get_osenv(key, default)
-
-    @staticmethod
-    def env_set(key, value):
-        return set_osenv(key, value)
-
-    @staticmethod
     def nvidia_smi():
         return nvidia_smi()
 
     @staticmethod
-    def ensure_import_module(name, libpath, liburi, specname=None, syspath=None):
+    def ensure_import_module(
+        name: str,
+        libpath: str,
+        liburi: str,
+        specname: str = "",
+        syspath: str = "",
+    ):
         from hyfi.utils.lib import ensure_import_module
 
         return ensure_import_module(name, libpath, liburi, specname, syspath)
 
     @staticmethod
     def collage(
         images_or_uris,
@@ -578,15 +560,15 @@
         show_filename=False,
         filename_offset=(5, 5),
         fontname=None,
         fontsize=12,
         fontcolor="#000",
         **kwargs,
     ):
-        from hyfi.graphic.collage import collage as _collage
+        from hyfi.graphics.collage import collage as _collage
 
         return _collage(
             images_or_uris,
             collage_filepath=collage_filepath,
             ncols=ncols,
             max_images=max_images,
             collage_width=collage_width,
@@ -612,15 +594,15 @@
         width=None,
         optimize=True,
         quality=50,
         show=False,
         force=False,
         **kwargs,
     ):
-        from hyfi.graphic.motion import make_gif as _make_gif
+        from hyfi.graphics.motion import make_gif as _make_gif
 
         return _make_gif(
             image_filepaths=image_filepaths,
             filename_patterns=filename_patterns,
             base_dir=base_dir,
             output_filepath=output_filepath,
             duration=duration,
@@ -641,17 +623,16 @@
     def to_numeric(data, _columns=None, errors="coerce", downcast=None, **kwargs):
         return to_numeric(data, _columns, errors, downcast, **kwargs)
 
     @staticmethod
     def getLogger(
         name=None,
         log_level=None,
-        fmt="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
     ):
-        return getLogger(name, log_level, fmt)
+        return getLogger(name, log_level)
 
     @staticmethod
     def setLogger(level=None, force=True, **kwargs):
         return setLogger(level, force, **kwargs)
 
     @staticmethod
     def set_cuda(device=0):
@@ -667,19 +648,19 @@
     ):
         return mount_google_drive(
             project_root, project_name, mountpoint, force_remount, timeout_ms
         )
 
     @staticmethod
     def getsource(obj):
-        return _getsource(obj)
+        return XC.getsource(obj)
 
     @staticmethod
     def viewsource(obj):
-        return _viewsource(obj)
+        return XC.viewsource(obj)
 
     @staticmethod
     def clear_output(wait=False):
         return clear_output(wait)
 
     @staticmethod
     def display(
@@ -727,23 +708,23 @@
             unconfined=unconfined,
             metadata=metadata,
             **kwargs,
         )
 
     @staticmethod
     def pip(
-        name,
-        upgrade=False,
-        prelease=False,
-        editable=False,
-        quiet=False,
-        find_links=None,
-        requirement=None,
-        force_reinstall=False,
-        verbose=False,
+        name: str,
+        upgrade: bool = False,
+        prelease: bool = False,
+        editable: bool = False,
+        quiet: bool = True,
+        find_links: str = "",
+        requirement: bool = False,
+        force_reinstall: bool = False,
+        verbose: bool = False,
         **kwargs,
     ):
         from hyfi.utils.lib import pip as _pip
 
         return _pip(
             name,
             upgrade,
@@ -754,15 +735,20 @@
             requirement,
             force_reinstall,
             verbose,
             **kwargs,
         )
 
     @staticmethod
-    def upgrade(prelease=False, quiet=False, force_reinstall=False, **kwargs):
+    def upgrade(
+        prelease=False,
+        quiet=False,
+        force_reinstall=False,
+        **kwargs,
+    ):
         from hyfi.utils.lib import pip
 
         return pip(
             name="hyfi",
             upgrade=True,
             prelease=prelease,
             quiet=quiet,
@@ -783,26 +769,42 @@
         return hide_code_in_slideshow()
 
     @staticmethod
     def cprint(str_color_tuples, **kwargs):
         return cprint(str_color_tuples)
 
     @staticmethod
-    def dict_to_dataframe(data, orient="columns", dtype=None, columns=None):
+    def dict_to_dataframe(
+        data,
+        orient="columns",
+        dtype=None,
+        columns=None,
+    ):
         return dict_to_dataframe(data, orient, dtype, columns)
 
     @staticmethod
     def records_to_dataframe(
-        data, index=None, exclude=None, columns=None, coerce_float=False, nrows=None
+        data,
+        index=None,
+        exclude=None,
+        columns=None,
+        coerce_float=False,
+        nrows=None,
     ):
         return records_to_dataframe(data, index, exclude, columns, coerce_float, nrows)
 
     @staticmethod
     def create_dropdown(
-        options, value, description, disabled=False, style=None, layout=None, **kwargs
+        options,
+        value,
+        description,
+        disabled=False,
+        style=None,
+        layout=None,
+        **kwargs,
     ):
         if style is None:
             style = {"description_width": "initial"}
         return create_dropdown(
             options,
             value,
             description,
@@ -832,15 +834,19 @@
             style,
             layout,
             **kwargs,
         )
 
     @staticmethod
     def create_button(
-        description, button_style="", icon="check", layout=None, **kwargs
+        description,
+        button_style="",
+        icon="check",
+        layout=None,
+        **kwargs,
     ):
         return create_button(description, button_style, icon, layout, **kwargs)
 
     @staticmethod
     def create_radiobutton(
         options,
         description,
@@ -903,40 +909,40 @@
             readout_format,
             style,
             layout,
             **kwargs,
         )
 
     @staticmethod
-    def get_image_font(fontname=None, fontsize=12):
-        from hyfi.graphic.collage import get_image_font
+    def get_image_font(fontname: str = "", fontsize: int = 12):
+        from hyfi.graphics.utils import get_image_font
 
         return get_image_font(fontname, fontsize)
 
     @staticmethod
     def read(uri, mode="rb", encoding=None, head=None, **kwargs):
         from hyfi.utils.file import read as _read
 
         return _read(uri, mode, encoding, head, **kwargs)
 
     @staticmethod
     def load_image(
         image_or_uri,
-        max_width: int = None,
-        max_height: int = None,
-        max_pixels: int = None,
+        max_width: int = 0,
+        max_height: int = 0,
+        max_pixels: int = 0,
         scale: float = 1.0,
-        resize_to_multiple_of: int = None,
+        resize_to_multiple_of: int = 0,
         crop_box=None,
         mode="RGB",
         **kwargs,
     ):
-        from hyfi.graphic.utils import load_image as _load_image
+        from hyfi.graphics.utils import load_image
 
-        return _load_image(
+        return load_image(
             image_or_uri,
             max_width,
             max_height,
             max_pixels,
             scale,
             resize_to_multiple_of,
             crop_box,
@@ -996,30 +1002,30 @@
             return __global_config__.project
         else:
             raise ValueError("Project not initialized.")
 
     @staticmethod
     def scale_image(
         image,
-        max_width: int = None,
-        max_height: int = None,
-        max_pixels: int = None,
+        max_width: int = 0,
+        max_height: int = 0,
+        max_pixels: int = 0,
         scale: float = 1.0,
         resize_to_multiple_of: int = 8,
         resample: int = 1,
     ):
         """
         Scale an image to a maximum width, height, or number of pixels.
 
         resample:   Image.NEAREST (0), Image.LANCZOS (1), Image.BILINEAR (2),
                     Image.BICUBIC (3), Image.BOX (4) or Image.HAMMING (5)
         """
-        from hyfi.graphic.utils import scale_image as _scale_image
+        from hyfi.graphics.utils import scale_image
 
-        return _scale_image(
+        return scale_image(
             image,
             max_width,
             max_height,
             max_pixels,
             scale,
             resize_to_multiple_of,
             resample,
```

### Comparing `hyfi-0.7.0/src/hyfi/path/__init__.py` & `hyfi-0.7.1/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/path/batch.py` & `hyfi-0.7.1/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/project/__init__.py` & `hyfi-0.7.1/src/hyfi/project/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             else:
                 logger.info(
                     "huggingface_hub.notebook_login() is only available in notebook,"
                     "set HUGGING_FACE_HUB_TOKEN manually"
                 )
 
     @property
-    def environ(self):
+    def osenv(self):
         return os.environ
 
     @property
     def project_workspace_dir(self):
         if self.path is None:
             raise ValueError("Path object not initialized")
         _p = Path(self.path.project_workspace_root)
```

### Comparing `hyfi-0.7.0/src/hyfi/tasks/base.py` & `hyfi-0.7.1/src/hyfi/task/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import contextlib
 from pathlib import Path
 from typing import Union
 
 from omegaconf import DictConfig
 from pydantic import BaseModel
 
-from hyfi.hydra import _compose, _to_config
-from hyfi.hydra.main import _merge, _methods, _print
+from hyfi.hydra import Composer
 from hyfi.module import ModuleConfig
 from hyfi.path.batch import BatchPathConfig
 from hyfi.project import ProjectConfig
 from hyfi.utils.lib import ensure_import_module
 from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
-class BaseTask(BaseModel):
+class TaskConfig(BaseModel):
     config_name: str = "__init__"
     config_group: str = "task"
     task_name: str
     path: BatchPathConfig = None  # type: ignore
     project: ProjectConfig = None  # type: ignore
     module: ModuleConfig = None  # type: ignore
     autoload: bool = False
@@ -51,17 +50,17 @@
         self,
         config_name: str = "",
         config_group: str = "",
         root_dir: str = "",
         **args,
     ):
         if config_group:
-            args = _merge(_compose(config_group), args)
+            args = Composer.merge(Composer._compose(config_group), args)
         else:
-            args = _to_config(args)
+            args = Composer.to_config(args)
         super().__init__(config_name=config_name, config_group=config_group, **args)
 
         object.__setattr__(self, "_config_", args)
         object.__setattr__(self, "_initial_config_", args.copy())
         self.initialize_configs(root_dir=root_dir)
 
     def __setattr__(self, key, val):
@@ -69,15 +68,15 @@
         method = self.__config__.property_set_methods.get(key)
         if method is not None:
             getattr(self, method)(val)
 
     def set_root_dir(self, root_dir: Union[str, Path]):
         path = self.config.path
         if path is None:
-            path = _compose("path=_batch_")
+            path = Composer._compose("path=_batch_")
             logger.info(
                 f"There is no path in the config, using default path: {path.root}"
             )
             self._config_.path = path
         if root_dir is not None:
             path.root = str(root_dir)
         self.path = BatchPathConfig(**path)
@@ -135,18 +134,18 @@
         return self.path.library_dir
 
     @property
     def verbose(self):
         return self.project.verbose
 
     def autorun(self):
-        return _methods(self.auto, self)
+        return Composer.methods(self.auto, self)
 
     def show_config(self):
-        _print(self.dict())
+        Composer.print(self.dict())
 
     def load_modules(self):
         """Load the modules"""
         if self.module.get("modules") is None:
             logger.info("No modules to load")
             return
         library_dir = self.library_dir
```

### Comparing `hyfi-0.7.0/src/hyfi/tasks/batch.py` & `hyfi-0.7.1/src/hyfi/task/batch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from omegaconf import DictConfig
 
 from hyfi.batch import BatchConfig
-from hyfi.hydra import _to_dict
-from hyfi.hydra.main import _load, _merge, _print, _save, _save_json
-from hyfi.tasks.base import BaseTask
+from hyfi.hydra.main import XC
+from hyfi.task import TaskConfig
 from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
-class BatchTask(BaseTask):
+class BatchTaskConfig(TaskConfig):
     batch: BatchConfig = None  # type: ignore
 
     class Config:
         arbitrary_types_allowed = True
         extra = "allow"
         validate_assignment = False
         exclude = {
@@ -100,43 +99,43 @@
         exclude=None,
         include=None,
     ):
         """Save the batch config"""
         if config is not None:
             self._config_ = config
         logger.info(f"Saving config to {self.batch.config_filepath}")
-        cfg = _to_dict(self.config)
+        cfg = XC.to_dict(self.config)
         if exclude is None:
             exclude = self.__config__.exclude
 
         if include:
             if isinstance(include, str):
                 include = [include]
             args = {key: cfg[key] for key in include}
         else:
             args = cfg
             if exclude:
                 if isinstance(exclude, str):
                     exclude = [exclude]
                 for key in exclude:
                     args.pop(key, None)
-        _save(args, self.batch.config_filepath)
+        XC.save(args, self.batch.config_filepath)
         self.save_settings(exclude=exclude)
         return self.batch.config_filename
 
     def save_settings(self, exclude=None, exclude_none=True):
         def dumper(obj):
-            return _to_dict(obj) if isinstance(obj, DictConfig) else str(obj)
+            return XC.to_dict(obj) if isinstance(obj, DictConfig) else str(obj)
 
         if exclude is None:
             exclude = self.__config__.exclude
         config = self.dict(exclude=exclude, exclude_none=exclude_none)
         if self.verbose:
             logger.info(f"Saving config to {self.batch.config_jsonpath}")
-        _save_json(config, self.batch.config_jsonpath, default=dumper)
+        XC.save_json(config, self.batch.config_jsonpath, default=dumper)
 
     def load_config(
         self,
         batch_name=None,
         batch_num=None,
         **args,
     ):
@@ -152,29 +151,29 @@
         if batch_num is not None:
             cfg = self._initial_config_.copy()
             self.batch.batch_name = batch_name
             self.batch.batch_num = batch_num
             _path = self.batch.config_filepath
             if _path.is_file():
                 logger.info(f"Loading config from {_path}")
-                batch_cfg = _load(_path)
+                batch_cfg = XC.load(_path)
                 if self.verbose:
                     logger.info("Merging config with the loaded config")
-                cfg = _merge(cfg, batch_cfg)
+                cfg = XC.merge(cfg, batch_cfg)
             else:
                 logger.info(f"No config file found at {_path}")
                 batch_num = None
         else:
             cfg = self.config
 
         if self.verbose:
             logger.info(f"Merging config with args: {args}")
-        self._config_ = _merge(cfg, args)
+        self._config_ = XC.merge(cfg, args)
 
         self.batch_num = batch_num
         self.batch_name = batch_name
 
         return self.config
 
     def show_config(self, batch_name=None, batch_num=None):
         self.load_config(batch_name, batch_num)
-        _print(self.dict())
+        XC.print(self.dict())
```

### Comparing `hyfi-0.7.0/src/hyfi/utils/env.py` & `hyfi-0.7.1/src/hyfi/utils/env.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     if pre_val := os.environ.get(key):
         logger.info("Overwriting %s=%s with %s", key, pre_val, value)
     else:
         logger.info("Setting %s=%s", key, value)
     os.environ[key] = value
 
 
-def _check_and_set_value(key: str, value: Any) -> Any:
+def check_and_set_osenv(key: str, value: Any) -> Any:
     """Check and set value to environment variable"""
     env_key = key.upper()
     if value is not None:
         old_value = os.getenv(env_key, "")
         if str(old_value).lower() != str(value).lower():
             os.environ[env_key] = str(value)
             logger.debug("Set environment variable %s=%s", env_key, str(value))
```

### Comparing `hyfi-0.7.0/src/hyfi/utils/file.py` & `hyfi-0.7.1/src/hyfi/utils/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,26 +49,28 @@
         file = os.path.join(base_dir, pattern) if base_dir else pattern
         files = glob(file, recursive=recursive)
     return files
 
 
 def get_filepaths(
     filename_patterns: Union[str, PosixPath, WindowsPath],
-    base_dir: Union[str, PosixPath, WindowsPath] = None,
+    base_dir: Union[str, PosixPath, WindowsPath] = "",
     recursive: bool = True,
     verbose: bool = False,
     **kwargs,
 ) -> List[str]:
     """Get a list of filepaths from a list of filename patterns"""
+    if filename_patterns is None:
+        raise ValueError("filename_patterns must be specified")
     if isinstance(filename_patterns, (PosixPath, WindowsPath)):
         filename_patterns = str(filename_patterns)
     if isinstance(filename_patterns, str):
         filename_patterns = [filename_patterns]
     filepaths = []
-    base_dir = str(base_dir) if base_dir else None
+    base_dir = str(base_dir) if base_dir else ""
     for file in filename_patterns:
         filepath = os.path.join(base_dir, file) if base_dir else file
         if os.path.exists(filepath):
             if Path(filepath).is_file():
                 filepaths.append(filepath)
         else:
             if os.path.dirname(file) != "":
@@ -247,32 +249,34 @@
             logger.info(f" >> elapsed time to load data: {elapsed()}")
     return data
 
 
 def save_data(
     data: Union[pd.DataFrame, dict],
     filename: str,
-    base_dir: str = None,
+    base_dir: str = "",
     columns=None,
-    index=False,
+    index: bool = False,
     filetype="parquet",
-    suffix: str = None,
+    suffix: str = "",
     verbose: bool = False,
     **kwargs,
 ):
     """Save data to a file"""
+    if filename is None:
+        raise ValueError("filename must be specified")
     fileinfo = os.path.splitext(filename)
     filename = fileinfo[0]
     filetype = fileinfo[1] if len(fileinfo) > 1 else filetype
     filetype = "." + filetype.replace(".", "")
-    if suffix is not None:
+    if suffix:
         filename = f"{filename}-{suffix}{filetype}"
     else:
         filename = f"{filename}{filetype}"
-    filepath = filename if base_dir is None else os.path.join(base_dir, filename)
+    filepath = os.path.join(base_dir, filename) if base_dir else filename
     base_dir = os.path.dirname(filepath)
     filename = os.path.basename(filepath)
     os.makedirs(base_dir, exist_ok=True)
 
     if isinstance(data, dict):
         for k, v in data.items():
             save_data(
```

### Comparing `hyfi-0.7.0/src/hyfi/utils/func.py` & `hyfi-0.7.1/src/hyfi/utils/func.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/utils/google.py` & `hyfi-0.7.1/src/hyfi/utils/google.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/utils/gpu.py` & `hyfi-0.7.1/src/hyfi/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/utils/lib.py` & `hyfi-0.7.1/src/hyfi/utils/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,19 @@
     if not specname:
         specname = spec.name
     sys.modules[specname] = module
     spec.loader.exec_module(module)
 
 
 def ensure_import_module(
-    name: str, libpath: str, liburi: str, specname: str = "", syspath: str = ""
+    name: str,
+    libpath: str,
+    liburi: str,
+    specname: str = "",
+    syspath: str = "",
 ) -> None:
     """Ensure a module is imported, if not, clone it from a git repo and load it"""
     try:
         if specname:
             importlib.import_module(specname)
         else:
             importlib.import_module(name)
```

### Comparing `hyfi-0.7.0/src/hyfi/utils/logging.py` & `hyfi-0.7.1/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/utils/notebook.py` & `hyfi-0.7.1/src/hyfi/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/src/hyfi/utils/tools.py` & `hyfi-0.7.1/src/hyfi/utils/tools.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.0/PKG-INFO` & `hyfi-0.7.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 0.7.0
+Version: 0.7.1
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

