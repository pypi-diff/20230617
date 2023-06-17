# Comparing `tmp/hyfi-0.7.1.tar.gz` & `tmp/hyfi-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-0.7.1.tar", max compression
+gzip compressed data, was "hyfi-0.7.2.tar", max compression
```

## Comparing `hyfi-0.7.1.tar` & `hyfi-0.7.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0     1071 2023-06-17 08:06:19.610584 hyfi-0.7.1/LICENSE
--rw-r--r--   0        0        0     1828 2023-06-17 08:06:19.610584 hyfi-0.7.1/README.md
--rw-r--r--   0        0        0     4592 2023-06-17 08:06:42.867187 hyfi-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     3804 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     2544 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/__click__.py
--rw-r--r--   0        0        0      647 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/__global__/__init__.py
--rw-r--r--   0        0        0     9856 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/__global__/config.py
--rw-r--r--   0        0        0      735 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-06-17 08:06:42.799185 hyfi-0.7.1/src/hyfi/_version.py
--rw-r--r--   0        0        0      777 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     3182 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     6832 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0     1206 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/common.py
--rw-r--r--   0        0        0     1923 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/file_lock.py
--rw-r--r--   0        0        0     3440 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1244 2023-06-17 08:06:19.614584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/util.py
--rw-r--r--   0        0        0      464 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/cached_path/_cached_path/version.py
--rw-r--r--   0        0        0        0 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-06-17 08:06:42.799185 hyfi-0.7.1/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      407 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       49 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      141 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0      320 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      559 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      725 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      291 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      948 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/mode/debug.yaml
--rw-r--r--   0        0        0       61 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0      120 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0     1719 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      609 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      806 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0      121 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      130 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0     6369 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0     3045 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0        0 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8396 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4330 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     5966 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0    21338 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/hydra/__init__.py
--rw-r--r--   0        0        0     7618 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/hydra/main.py
--rw-r--r--   0        0        0     3487 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     2099 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    16589 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0     2579 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/joblib/pipe.py
--rw-r--r--   0        0        0    30690 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      217 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     2903 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     5743 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/path/batch.py
--rw-r--r--   0        0        0     5564 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/py.typed
--rw-r--r--   0        0        0     4907 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     5239 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0     5667 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/env.py
--rw-r--r--   0        0        0    12630 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/file.py
--rw-r--r--   0        0        0     9920 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/func.py
--rw-r--r--   0        0        0     1114 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/google.py
--rw-r--r--   0        0        0     3699 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/gpu.py
--rw-r--r--   0        0        0     4162 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/lib.py
--rw-r--r--   0        0        0     1986 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0     9766 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/notebook.py
--rw-r--r--   0        0        0     5476 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/tools.py
--rw-r--r--   0        0        0      232 2023-06-17 08:06:19.618584 hyfi-0.7.1/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 hyfi-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-17 11:43:48.311136 hyfi-0.7.2/LICENSE
+-rw-r--r--   0        0        0     1828 2023-06-17 11:43:48.311136 hyfi-0.7.2/README.md
+-rw-r--r--   0        0        0     4592 2023-06-17 11:44:20.783312 hyfi-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     3804 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     2544 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      647 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/__global__/__init__.py
+-rw-r--r--   0        0        0     9856 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/__global__/config.py
+-rw-r--r--   0        0        0      735 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-17 11:44:20.683312 hyfi-0.7.2/src/hyfi/_version.py
+-rw-r--r--   0        0        0      777 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     3182 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     6832 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0     1206 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/common.py
+-rw-r--r--   0        0        0     1923 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/file_lock.py
+-rw-r--r--   0        0        0     3440 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1244 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/version.py
+-rw-r--r--   0        0        0        0 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-17 11:44:20.683312 hyfi-0.7.2/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      407 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      141 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0      320 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      559 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      725 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      291 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      948 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/conf/mode/debug.yaml
+-rw-r--r--   0        0        0       61 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0      120 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0     1719 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      609 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      806 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      121 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      130 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0     6369 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0     3045 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8363 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4535 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     6610 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0    21338 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/hydra/__init__.py
+-rw-r--r--   0        0        0     7618 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/hydra/main.py
+-rw-r--r--   0        0        0     3487 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     2099 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    16589 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0     2579 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/joblib/pipe.py
+-rw-r--r--   0        0        0    30754 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      217 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     2903 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     5743 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0     5564 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/py.typed
+-rw-r--r--   0        0        0     4907 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     5239 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0     5667 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/env.py
+-rw-r--r--   0        0        0    12630 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/file.py
+-rw-r--r--   0        0        0     9920 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/func.py
+-rw-r--r--   0        0        0     1114 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/google.py
+-rw-r--r--   0        0        0     3699 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/gpu.py
+-rw-r--r--   0        0        0     4162 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/lib.py
+-rw-r--r--   0        0        0     1986 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0     9766 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/notebook.py
+-rw-r--r--   0        0        0     5476 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/tools.py
+-rw-r--r--   0        0        0      232 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 hyfi-0.7.2/PKG-INFO
```

### Comparing `hyfi-0.7.1/LICENSE` & `hyfi-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/README.md` & `hyfi-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/pyproject.toml` & `hyfi-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "0.7.1"
+version = "0.7.2"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-0.7.1/src/hyfi/__cli__.py` & `hyfi-0.7.2/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/__click__.py` & `hyfi-0.7.2/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/__global__/__init__.py` & `hyfi-0.7.2/src/hyfi/__global__/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/__global__/config.py` & `hyfi-0.7.2/src/hyfi/__global__/config.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/__init__.py` & `hyfi-0.7.2/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/about/__init__.py` & `hyfi-0.7.2/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/batch/__init__.py` & `hyfi-0.7.2/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/cached_path/__init__.py` & `hyfi-0.7.2/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/__init__.py` & `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/_cached_path.py` & `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/cache_file.py` & `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/common.py` & `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/file_lock.py` & `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/meta.py` & `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/progress.py` & `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/schemes/__init__.py` & `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/schemes/beaker.py` & `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/schemes/hf.py` & `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/schemes/http.py` & `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py` & `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/testing.py` & `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/cached_path/_cached_path/util.py` & `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/conf/copier/conf.yaml` & `hyfi-0.7.2/src/hyfi/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-0.7.2/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-0.7.2/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/conf/mode/__init__.yaml` & `hyfi-0.7.2/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/conf/path/__init__.yaml` & `hyfi-0.7.2/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/conf/path/__task__.yaml` & `hyfi-0.7.2/src/hyfi/conf/path/__task__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/conf/project/__init__.yaml` & `hyfi-0.7.2/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/copier/__init__.py` & `hyfi-0.7.2/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/dotenv/__init__.py` & `hyfi-0.7.2/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/graphics/collage.py` & `hyfi-0.7.2/src/hyfi/graphics/collage.py`

 * *Files 10% similar despite different names*

```diff
@@ -162,26 +162,22 @@
         ax.set_xlabel(xlabel, fontsize=xlabel_fontsize, color=fg_fontcolor)
     if ylabel is not None:
         # plt.ylabel(ylabel, fontdict={"fontsize": ylabel_fontsize})
         ax.set_ylabel(ylabel, fontsize=ylabel_fontsize, color=fg_fontcolor)
     if xticklabels is not None:
         # get ncols number of xticks from xlim
         xlim = ax.get_xlim()
-        xticks = np.linspace(xlim[0], xlim[1], ncols + 1)
-        xticks = xticks - (xticks[1] - xticks[0]) / 2
-        xticks[0] = xlim[0]
+        xticks = _get_ticks(xlim, ncols)
         ax.set_xticks(xticks, color=fg_fontcolor)
         xticklabels = [""] + xticklabels
         ax.set_xticklabels(xticklabels, fontsize=xlabel_fontsize, color=fg_fontcolor)
     if yticklabels is not None:
         # get nrows number of yticks from ylim
         ylim = ax.get_ylim()
-        yticks = np.linspace(ylim[0], ylim[1], nrows + 1)
-        yticks = yticks - (yticks[1] - yticks[0]) / 2
-        yticks[0] = ylim[0]
+        yticks = _get_ticks(ylim, nrows)
         ax.set_yticks(yticks, color=fg_fontcolor)
         yticklabels = [""] + yticklabels
         ax.set_yticklabels(yticklabels, fontsize=ylabel_fontsize, color=fg_fontcolor)
 
     plt.tight_layout()
     if caption is not None:
         print(f"[{caption}]")
@@ -203,14 +199,21 @@
         width=img.width,
         height=img.height,
         ncols=ncols,
         nrows=nrows,
     )
 
 
+def _get_ticks(lim, n):
+    result = np.linspace(lim[0], lim[1], n + 1)
+    result = result - (result[1] - result[0]) / 2
+    result[0] = lim[0]
+    return result
+
+
 def grid_of_images(
     images: List[Image.Image],
     ncols: int = 3,
     padding: int = 10,
     bg_color: str = "black",
 ) -> Collage:
     """
```

### Comparing `hyfi-0.7.1/src/hyfi/graphics/motion.py` & `hyfi-0.7.2/src/hyfi/graphics/motion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,85 +1,87 @@
 """Motion image processing functions."""
 import os
 import subprocess
 from pathlib import Path
 
+from hyfi.graphics.utils import load_images
 from hyfi.utils.file import get_filepaths
 from hyfi.utils.logging import getLogger
 from hyfi.utils.notebook import display_image
 
 logger = getLogger(__name__)
 
 
 def make_gif(
     image_filepaths=None,
-    filename_patterns=None,
-    base_dir=None,
-    output_filepath=None,
-    duration=100,
-    loop=0,
-    width=None,
-    optimize=True,
-    quality=50,
-    show=False,
-    force=False,
+    filename_patterns: str = "",
+    base_dir: str = "",
+    output_filepath: str = "",
+    duration: int = 100,
+    loop: int = 0,
+    width: int = 0,
+    optimize: bool = True,
+    quality: int = 50,
+    show: bool = False,
+    force: bool = False,
     **kwargs,
 ):
     """
     Create a GIF from a list of images or a list of filenames.
     """
-    from PIL import Image
-
-    logger.info(f"Making GIF from {filename_patterns}")
+    logger.info("Making GIF from %s", filename_patterns)
     if os.path.exists(output_filepath) and not force:
-        logger.info(f"Skipping GIF creation, already exists: {output_filepath}")
+        logger.info("Skipping GIF creation, already exists: %s", output_filepath)
         logger.info("If you want to re-create the GIF, set force=True")
     else:
         if image_filepaths is None:
             image_filepaths = sorted(
                 get_filepaths(filename_patterns, base_dir=base_dir)
             )
         if not image_filepaths:
             logger.warning("no images found")
             return
-        if frames := [Image.open(image) for image in image_filepaths]:
+        if frames := load_images(image_filepaths):
             frame_one = frames[0]
             frame_one.save(
                 output_filepath,
                 format="GIF",
                 append_images=frames,
                 save_all=True,
                 duration=duration,
                 loop=loop,
                 optimize=optimize,
                 quality=quality,
             )
-            print(f"Saved GIF to {output_filepath}")
+            logger.info("Saved GIF to %s", output_filepath)
         else:
-            logger.warning(f"No frames found for {filename_patterns}")
+            logger.warning("No frames found for %s", filename_patterns)
 
     if show and os.path.exists(output_filepath):
         display_image(data=open(output_filepath, "rb").read(), width=width)
 
     return output_filepath
 
 
 def extract_frames(
-    video_path, extract_nth_frame, extracted_frame_dir, frame_filename="%04d.jpg"
+    video_path: str,
+    extract_nth_frame: int,
+    extracted_frame_dir: str,
+    frame_filename: str = "%04d.jpg",
 ):
     """
     Extract frames from a video.
     """
-    logger.info(f"Exporting Video Frames (1 every {extract_nth_frame})...")
+    logger.info("Exporting Video Frames (1 every %s)...", extract_nth_frame)
     try:
         for f in Path(f"{extracted_frame_dir}").glob("*.jpg"):
             f.unlink()
     except FileNotFoundError:
-        logger.info(f"No video frames found in {extracted_frame_dir}")
-    vf = f"select=not(mod(n\,{extract_nth_frame}))"
+        logger.info("No video frames found in %s", extracted_frame_dir)
+    vf = f"select=not(mod(n\\,{extract_nth_frame}))"
 
     ffmpeg_path = "/usr/bin/ffmpeg"
     if not os.path.exists(ffmpeg_path):
         ffmpeg_path = "ffmpeg"
     if os.path.exists(video_path):
         subprocess.run(
             [
@@ -97,28 +99,35 @@
                 "-stats",
                 f"{extracted_frame_dir}/{frame_filename}",
             ],
             stdout=subprocess.PIPE,
         ).stdout.decode("utf-8")
     else:
         logger.warning(
-            f"WARNING!\n\nVideo not found: {video_path}.\nPlease check your video path."
+            "WARNING!\n\nVideo not found: %s.\nPlease check your video path.",
+            video_path,
         )
 
 
 def create_video(
-    base_dir, video_path, input_url, fps, start_number, vframes, force=False
+    base_dir: str,
+    video_path: str,
+    input_url: str,
+    fps: int,
+    start_number: int,
+    vframes: int,
+    force: bool = False,
 ):
     """
     Create a video from a list of images.
     """
 
-    logger.info(f"Creating video from {input_url}")
+    logger.info("Creating video from %s", input_url)
     if os.path.exists(video_path) and not force:
-        logger.info(f"Skipping video creation, already exists: {video_path}")
+        logger.info("Skipping video creation, already exists: %s", video_path)
         logger.info("If you want to re-create the video, set force=True")
         return video_path
 
     cmd = [
         "ffmpeg",
         "-y",
         "-vcodec",
@@ -146,15 +155,15 @@
 
     process = subprocess.Popen(
         cmd,
         cwd=f"{base_dir}",
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     )
-    stdout, stderr = process.communicate()
+    _, stderr = process.communicate()
     if process.returncode != 0:
-        print(stderr)
+        logger.error(stderr)
         raise RuntimeError(stderr)
     else:
-        print(f"The video is ready and saved to {video_path}")
+        logger.info("Video created successfully and saved to %s", video_path)
 
     return video_path
```

### Comparing `hyfi-0.7.1/src/hyfi/graphics/utils.py` & `hyfi-0.7.2/src/hyfi/graphics/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,24 +22,27 @@
     max_height: int = 0,
     max_pixels: int = 0,
     scale: float = 1.0,
     resize_to_multiple_of: int = 8,
     resample: int = Image.LANCZOS,
 ) -> Image.Image:
     """Scale image to have at most `max_pixels` pixels."""
+    if resize_to_multiple_of is None:
+        resize_to_multiple_of = 0
+
     w, h = image.size
 
     if max_width <= 0 and max_height > 0:
         max_width = int(w * max_height / h)
     elif max_height <= 0 and max_width > 0:
         max_height = int(h * max_width / w)
 
-    if max_width <= 0 and max_height >= 0:
+    if max_width > 0 and max_height > 0:
         max_pixels = max_width * max_height
-    if max_pixels >= 0:
+    if max_pixels > 0:
         scale = np.sqrt(max_pixels / (w * h))
 
     max_width = int(w * scale)
     max_height = int(h * scale)
     if resize_to_multiple_of > 0:
         max_width = (max_width // resize_to_multiple_of) * resize_to_multiple_of
         max_height = (max_height // resize_to_multiple_of) * resize_to_multiple_of
@@ -59,16 +62,24 @@
     crop_box=None,
     mode="RGB",
     **kwargs,
 ) -> Image.Image:
     """Load image from file or URI."""
     from PIL import Image
 
+    if max_width is None:
+        max_width = 0
+    if max_height is None:
+        max_height = 0
+    if max_pixels is None:
+        max_pixels = 0
     if isinstance(image_or_uri, Image.Image):
         img = image_or_uri.convert(mode)
+    elif Path(image_or_uri).is_file():
+        img = Image.open(image_or_uri).convert(mode)
     else:
         img = Image.open(io.BytesIO(read(image_or_uri, **kwargs))).convert(mode)
     img = scale_image(
         img,
         max_width=max_width,
         max_height=max_height,
         max_pixels=max_pixels,
@@ -86,15 +97,15 @@
     max_height: int = 0,
     max_pixels: int = 0,
     scale: float = 1.0,
     resize_to_multiple_of: int = 0,
     crop_to_min_size: bool = False,
     mode: str = "RGB",
     **kwargs,
-):
+) -> List[Image.Image]:
     """Load images from files or URIs."""
     imgs = [
         load_image(
             image_or_uri,
             max_width=max_width,
             max_height=max_height,
             max_pixels=max_pixels,
@@ -112,31 +123,37 @@
             min_width = (min_width // resize_to_multiple_of) * resize_to_multiple_of
             min_height = (min_height // resize_to_multiple_of) * resize_to_multiple_of
         imgs = [img.crop((0, 0, min_width, min_height)) for img in imgs]
 
     return imgs
 
 
-def get_image_font(fontname: str = "", fontsize: int = 12):
+def get_image_font(fontname: str = "", fontsize: int = 12, lang: str = "en"):
     """Get font for PIL image."""
     fontname, fontpath = get_plot_font(set_font_for_matplot=False, fontname=fontname)
     return ImageFont.truetype(fontpath, fontsize) if fontpath else None
 
 
 def get_default_system_font(
-    fontname: str = "", fontpath: str = "", verbose: bool = False
+    fontname: str = "",
+    fontpath: str = "",
+    lang: str = "ko",
+    verbose: bool = False,
 ):
     if platform.system() == "Darwin":
-        fontname = fontname or "AppleGothic.ttf"
+        default_fontname = "AppleGothic.ttf" if lang == "ko" else "Arial.ttf"
+        fontname = fontname or default_fontname
         fontpath = os.path.join("/System/Library/Fonts/Supplemental/", fontname)
     elif platform.system() == "Windows":
-        fontname = fontname or "malgun.ttf"
+        default_fontname = "malgun.ttf" if lang == "ko" else "arial.ttf"
+        fontname = fontname or default_fontname
         fontpath = os.path.join("c:/Windows/Fonts/", fontname)
     elif platform.system() == "Linux":
-        fontname = fontname or "NanumGothic.ttf"
+        default_fontname = "NanumGothic.ttf" if lang == "ko" else "DejaVuSans.ttf"
+        fontname = fontname or default_fontname
         if fontname.lower().startswith("nanum"):
             fontpath = os.path.join("/usr/share/fonts/truetype/nanum/", fontname)
         else:
             fontpath = os.path.join("/usr/share/fonts/truetype/", fontname)
     if fontpath and not Path(fontpath).is_file():
         paths = find_font_file(fontname)
         fontpath = paths[0] if len(paths) > 0 else ""
@@ -145,21 +162,22 @@
     return fontname, fontpath
 
 
 def get_plot_font(
     set_font_for_matplot: bool = True,
     fontpath: str = "",
     fontname: str = "",
+    lang: str = "en",
     verbose: bool = False,
 ):
     """Get font for plot"""
     if fontname and not fontname.endswith(".ttf"):
         fontname += ".ttf"
     if not fontpath:
-        fontname, fontpath = get_default_system_font(fontname, fontpath, verbose)
+        fontname, fontpath = get_default_system_font(fontname, fontpath, lang, verbose)
 
     if fontpath and Path(fontpath).is_file():
         font_manager.fontManager.addfont(fontpath)
         fontname = font_manager.FontProperties(fname=fontpath).get_name()  # type: ignore
 
         if set_font_for_matplot and fontname:
             rc("font", family=fontname)
```

### Comparing `hyfi-0.7.1/src/hyfi/hydra/__init__.py` & `hyfi-0.7.2/src/hyfi/hydra/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/hydra/main.py` & `hyfi-0.7.2/src/hyfi/hydra/main.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/joblib/__init__.py` & `hyfi-0.7.2/src/hyfi/joblib/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/joblib/batch/apply.py` & `hyfi-0.7.2/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-0.7.2/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/joblib/batch/batcher.py` & `hyfi-0.7.2/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/joblib/pipe.py` & `hyfi-0.7.2/src/hyfi/joblib/pipe.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/main/__init__.py` & `hyfi-0.7.2/src/hyfi/main/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -582,24 +582,24 @@
             fontcolor=fontcolor,
             **kwargs,
         )
 
     @staticmethod
     def make_gif(
         image_filepaths=None,
-        filename_patterns=None,
-        base_dir=None,
-        output_filepath=None,
-        duration=100,
-        loop=0,
-        width=None,
-        optimize=True,
-        quality=50,
-        show=False,
-        force=False,
+        filename_patterns: str = "",
+        base_dir: str = "",
+        output_filepath: str = "",
+        duration: int = 100,
+        loop: int = 0,
+        width: int = 0,
+        optimize: bool = True,
+        quality: int = 50,
+        show: bool = False,
+        force: bool = False,
         **kwargs,
     ):
         from hyfi.graphics.motion import make_gif as _make_gif
 
         return _make_gif(
             image_filepaths=image_filepaths,
             filename_patterns=filename_patterns,
```

### Comparing `hyfi-0.7.1/src/hyfi/path/__init__.py` & `hyfi-0.7.2/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/path/batch.py` & `hyfi-0.7.2/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/project/__init__.py` & `hyfi-0.7.2/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/task/__init__.py` & `hyfi-0.7.2/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/task/batch.py` & `hyfi-0.7.2/src/hyfi/task/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/utils/env.py` & `hyfi-0.7.2/src/hyfi/utils/env.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/utils/file.py` & `hyfi-0.7.2/src/hyfi/utils/file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/utils/func.py` & `hyfi-0.7.2/src/hyfi/utils/func.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/utils/google.py` & `hyfi-0.7.2/src/hyfi/utils/google.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/utils/gpu.py` & `hyfi-0.7.2/src/hyfi/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/utils/lib.py` & `hyfi-0.7.2/src/hyfi/utils/lib.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/utils/logging.py` & `hyfi-0.7.2/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/utils/notebook.py` & `hyfi-0.7.2/src/hyfi/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/src/hyfi/utils/tools.py` & `hyfi-0.7.2/src/hyfi/utils/tools.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.1/PKG-INFO` & `hyfi-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 0.7.1
+Version: 0.7.2
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

