# Comparing `tmp/mosaicml-cli-0.4.8.tar.gz` & `tmp/mosaicml-cli-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.4.8.tar", last modified: Tue Jun 13 23:02:45 2023, max compression
+gzip compressed data, was "mosaicml-cli-0.4.9.tar", last modified: Thu Jun 15 20:53:05 2023, max compression
```

## Comparing `mosaicml-cli-0.4.8.tar` & `mosaicml-cli-0.4.9.tar`

### file list

```diff
@@ -1,202 +1,202 @@
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.943381 mosaicml-cli-0.4.8/
--rw-r--r--   0 tylerlee   (502) staff       (20)      696 2023-06-13 23:02:45.943082 mosaicml-cli-0.4.8/PKG-INFO
--rw-r--r--   0 tylerlee   (502) staff       (20)     7089 2023-06-13 22:57:11.000000 mosaicml-cli-0.4.8/README.md
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.898764 mosaicml-cli-0.4.8/mcli/
--rw-r--r--   0 tylerlee   (502) staff       (20)     2092 2023-05-24 19:54:07.000000 mosaicml-cli-0.4.8/mcli/__init__.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.899802 mosaicml-cli-0.4.8/mcli/api/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.8/mcli/api/__init__.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.900548 mosaicml-cli-0.4.8/mcli/api/cluster/
--rw-r--r--   0 tylerlee   (502) staff       (20)      134 2022-11-02 22:22:14.000000 mosaicml-cli-0.4.8/mcli/api/cluster/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4228 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/cluster/api_get_clusters.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.900943 mosaicml-cli-0.4.8/mcli/api/engine/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.8/mcli/api/engine/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    26219 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/engine/engine.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10784 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/exceptions.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.903414 mosaicml-cli-0.4.8/mcli/api/inference_deployments/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1521 2023-05-24 19:54:07.000000 mosaicml-cli-0.4.8/mcli/api/inference_deployments/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3297 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5096 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3603 2023-05-24 19:54:07.000000 mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     8441 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2053 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_ping.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2347 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_predict_inference_deployment.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6474 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_update_inference_deployments.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.903921 mosaicml-cli-0.4.8/mcli/api/mint/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.8/mcli/api/mint/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     7840 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/mint/shell.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2676 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.8/mcli/api/mint/tty.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.905161 mosaicml-cli-0.4.8/mcli/api/model/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1114 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/api/model/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6322 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/api/model/cluster_details.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4583 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/api/model/inference_deployment.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10439 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/api/model/run.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.907663 mosaicml-cli-0.4.8/mcli/api/runs/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1199 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.8/mcli/api/runs/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2804 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/api/runs/api_create_run.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4202 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/runs/api_delete_runs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     8888 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/runs/api_get_run_logs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10924 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/runs/api_get_runs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5204 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/runs/api_start_run.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5396 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/runs/api_stop_runs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3928 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/runs/api_update_run_metadata.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10619 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.8/mcli/api/runs/api_watch_run.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.909013 mosaicml-cli-0.4.8/mcli/api/schema/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.8/mcli/api/schema/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      636 2022-08-23 15:11:52.000000 mosaicml-cli-0.4.8/mcli/api/schema/generic_model.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.909947 mosaicml-cli-0.4.8/mcli/api/secrets/
--rw-r--r--   0 tylerlee   (502) staff       (20)      309 2022-09-23 17:32:12.000000 mosaicml-cli-0.4.8/mcli/api/secrets/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2386 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/api/secrets/api_create_secret.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3010 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/secrets/api_delete_secrets.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3709 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/secrets/api_get_secrets.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2354 2022-03-24 04:29:23.000000 mosaicml-cli-0.4.8/mcli/api/typing_future.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.910287 mosaicml-cli-0.4.8/mcli/api/users/
--rw-r--r--   0 tylerlee   (502) staff       (20)      139 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.8/mcli/api/users/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2715 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/api/users/api_get_users.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      920 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/api/utils.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.910685 mosaicml-cli-0.4.8/mcli/cli/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.8/mcli/cli/__init__.py
--rwxr-xr-x   0 tylerlee   (502) staff       (20)     6378 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/cli/cli.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.911353 mosaicml-cli-0.4.8/mcli/cli/common/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.8/mcli/cli/common/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2560 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/common/deployment_filters.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6922 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/common/run_filters.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.911677 mosaicml-cli-0.4.8/mcli/cli/m_connect/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.8/mcli/cli/m_connect/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6143 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/cli/m_connect/m_connect.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.912173 mosaicml-cli-0.4.8/mcli/cli/m_create/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.8/mcli/cli/m_create/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2385 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_create/m_create.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    16900 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/m_create/secret.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.912824 mosaicml-cli-0.4.8/mcli/cli/m_delete/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.8/mcli/cli/m_delete/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6448 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/m_delete/delete.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5805 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_delete/m_delete.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.913138 mosaicml-cli-0.4.8/mcli/cli/m_deploy/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.8/mcli/cli/m_deploy/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4001 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/m_deploy/m_deploy.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.914056 mosaicml-cli-0.4.8/mcli/cli/m_describe/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-01-26 00:46:18.000000 mosaicml-cli-0.4.8/mcli/cli/m_describe/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3929 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     9988 2023-06-13 22:57:06.000000 mosaicml-cli-0.4.8/mcli/cli/m_describe/describe_runs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2002 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.8/mcli/cli/m_describe/m_describe.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.915910 mosaicml-cli-0.4.8/mcli/cli/m_get/
--rw-r--r--   0 tylerlee   (502) staff       (20)      467 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_get/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6226 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_get/clusters.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6447 2023-05-24 19:54:07.000000 mosaicml-cli-0.4.8/mcli/cli/m_get/display.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5669 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/m_get/inference_deployments.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4803 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_get/m_get.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     9800 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/m_get/runs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2189 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_get/secrets.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1580 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.8/mcli/cli/m_get/users.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.916311 mosaicml-cli-0.4.8/mcli/cli/m_init/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.8/mcli/cli/m_init/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3908 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/cli/m_init/m_init.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.917343 mosaicml-cli-0.4.8/mcli/cli/m_interactive/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.8/mcli/cli/m_interactive/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6793 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/cli/m_interactive/interactive.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    44284 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_interactive/kube_config.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     9484 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/cli/m_interactive/m_interactive.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.918609 mosaicml-cli-0.4.8/mcli/cli/m_kube/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_kube/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5523 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_kube/m_get_config.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1398 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_kube/m_kube.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2050 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_kube/m_merge_config.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6946 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_kube/utils.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.918965 mosaicml-cli-0.4.8/mcli/cli/m_log/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.8/mcli/cli/m_log/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    11253 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/cli/m_log/m_log.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.919389 mosaicml-cli-0.4.8/mcli/cli/m_ping/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.8/mcli/cli/m_ping/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1103 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/m_ping/m_ping.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.919870 mosaicml-cli-0.4.8/mcli/cli/m_predict/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.8/mcli/cli/m_predict/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1661 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/m_predict/m_predict.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.920308 mosaicml-cli-0.4.8/mcli/cli/m_root/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.8/mcli/cli/m_root/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      536 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_root/m_config.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.920696 mosaicml-cli-0.4.8/mcli/cli/m_run/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.8/mcli/cli/m_run/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     8258 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/cli/m_run/m_run.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.922013 mosaicml-cli-0.4.8/mcli/cli/m_set_unset/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-10-04 23:53:41.000000 mosaicml-cli-0.4.8/mcli/cli/m_set_unset/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2964 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/cli/m_set_unset/api_key.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1793 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/cli/m_set_unset/feature_flag.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1940 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_set_unset/m_set.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1421 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_set_unset/m_unset.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      745 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/cli/m_set_unset/user.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.922285 mosaicml-cli-0.4.8/mcli/cli/m_stop/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-10-04 23:53:41.000000 mosaicml-cli-0.4.8/mcli/cli/m_stop/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4066 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/cli/m_stop/m_stop.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.923083 mosaicml-cli-0.4.8/mcli/cli/m_util/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-08-10 05:32:44.000000 mosaicml-cli-0.4.8/mcli/cli/m_util/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      797 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/cli/m_util/m_util.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6837 2023-06-13 22:57:06.000000 mosaicml-cli-0.4.8/mcli/cli/m_util/util.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    12143 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/config.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.925382 mosaicml-cli-0.4.8/mcli/models/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1047 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/models/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2103 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/models/gpu_type.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10374 2023-06-13 22:57:11.000000 mosaicml-cli-0.4.8/mcli/models/inference_deployment_config.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      427 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/models/mcli_cluster.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      456 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/models/mcli_envvar.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6724 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/models/mcli_secret.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    19538 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/models/run_config.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.925915 mosaicml-cli-0.4.8/mcli/objects/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.8/mcli/objects/__init__.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.927874 mosaicml-cli-0.4.8/mcli/objects/secrets/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1090 2022-12-07 21:26:59.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/__init__.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.929494 mosaicml-cli-0.4.8/mcli/objects/secrets/create/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/create/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1646 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/create/base.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2244 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/create/docker_registry.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2408 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/create/gcp.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6377 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/create/generic.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3858 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/create/oci.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3001 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/create/s3.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5342 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/create/ssh.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      783 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/docker_registry.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1017 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/env_var.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      556 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/gcp.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1267 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/mounted.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      967 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/oci.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      961 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/s3.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1718 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/objects/secrets/ssh.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.929805 mosaicml-cli-0.4.8/mcli/proto/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.8/mcli/proto/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1477 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.8/mcli/proto/mint_pb2.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.930082 mosaicml-cli-0.4.8/mcli/sdk/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1976 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.8/mcli/sdk/__init__.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.934542 mosaicml-cli-0.4.8/mcli/utils/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.8/mcli/utils/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5306 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.8/mcli/utils/utils_cli.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6073 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.8/mcli/utils/utils_config.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      740 2022-09-27 01:25:02.000000 mosaicml-cli-0.4.8/mcli/utils/utils_date.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10749 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/utils/utils_docker.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2225 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/utils/utils_epilog.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10774 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/utils/utils_interactive.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4527 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/utils/utils_logging.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2160 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.8/mcli/utils/utils_message_decoding.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6605 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/utils/utils_pypi.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3115 2023-03-15 17:23:44.000000 mosaicml-cli-0.4.8/mcli/utils/utils_rich.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5033 2023-06-06 15:18:59.000000 mosaicml-cli-0.4.8/mcli/utils/utils_run_status.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4350 2022-03-30 16:04:08.000000 mosaicml-cli-0.4.8/mcli/utils/utils_serializable_dataclass.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1103 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.8/mcli/utils/utils_spinner.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10751 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/utils/utils_string_functions.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1677 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/mcli/utils/utils_types.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1001 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.8/mcli/utils/utils_yaml.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3876 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/mcli/version.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.938033 mosaicml-cli-0.4.8/mosaicml_cli.egg-info/
--rw-r--r--   0 tylerlee   (502) staff       (20)      696 2023-06-13 23:02:45.000000 mosaicml-cli-0.4.8/mosaicml_cli.egg-info/PKG-INFO
--rw-r--r--   0 tylerlee   (502) staff       (20)     4922 2023-06-13 23:02:45.000000 mosaicml-cli-0.4.8/mosaicml_cli.egg-info/SOURCES.txt
--rw-r--r--   0 tylerlee   (502) staff       (20)        1 2023-06-13 23:02:45.000000 mosaicml-cli-0.4.8/mosaicml_cli.egg-info/dependency_links.txt
--rw-r--r--   0 tylerlee   (502) staff       (20)       75 2023-06-13 23:02:45.000000 mosaicml-cli-0.4.8/mosaicml_cli.egg-info/entry_points.txt
--rw-r--r--   0 tylerlee   (502) staff       (20)     1655 2023-06-13 23:02:45.000000 mosaicml-cli-0.4.8/mosaicml_cli.egg-info/requires.txt
--rw-r--r--   0 tylerlee   (502) staff       (20)        5 2023-06-13 23:02:45.000000 mosaicml-cli-0.4.8/mosaicml_cli.egg-info/top_level.txt
--rw-r--r--   0 tylerlee   (502) staff       (20)    31087 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/pyproject.toml
--rw-r--r--   0 tylerlee   (502) staff       (20)       38 2023-06-13 23:02:45.943565 mosaicml-cli-0.4.8/setup.cfg
--rw-r--r--   0 tylerlee   (502) staff       (20)     3057 2023-06-13 22:57:11.000000 mosaicml-cli-0.4.8/setup.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-13 23:02:45.941898 mosaicml-cli-0.4.8/tests/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.8/tests/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      618 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.8/tests/conftest.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     7127 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.8/tests/test_config.py
--rw-r--r--   0 tylerlee   (502) staff       (20)       62 2022-03-03 05:25:48.000000 mosaicml-cli-0.4.8/tests/test_simple.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6116 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.8/tests/test_upgrade.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.920695 mosaicml-cli-0.4.9/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      696 2023-06-15 20:53:05.920546 mosaicml-cli-0.4.9/PKG-INFO
+-rw-r--r--   0 tylerlee   (502) staff       (20)     7089 2023-06-13 22:57:11.000000 mosaicml-cli-0.4.9/README.md
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.885680 mosaicml-cli-0.4.9/mcli/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2092 2023-05-24 19:54:07.000000 mosaicml-cli-0.4.9/mcli/__init__.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.886401 mosaicml-cli-0.4.9/mcli/api/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.9/mcli/api/__init__.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.886886 mosaicml-cli-0.4.9/mcli/api/cluster/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      134 2022-11-02 22:22:14.000000 mosaicml-cli-0.4.9/mcli/api/cluster/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4280 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/cluster/api_get_clusters.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.887223 mosaicml-cli-0.4.9/mcli/api/engine/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.9/mcli/api/engine/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    26224 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/engine/engine.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10824 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/exceptions.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.889526 mosaicml-cli-0.4.9/mcli/api/inference_deployments/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1521 2023-05-24 19:54:07.000000 mosaicml-cli-0.4.9/mcli/api/inference_deployments/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3297 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5096 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3603 2023-05-24 19:54:07.000000 mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     8441 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2053 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_ping.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2347 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_predict_inference_deployment.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6474 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_update_inference_deployments.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.890764 mosaicml-cli-0.4.9/mcli/api/mint/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.9/mcli/api/mint/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     7840 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/api/mint/shell.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2676 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.9/mcli/api/mint/tty.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.891812 mosaicml-cli-0.4.9/mcli/api/model/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1114 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/api/model/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6435 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/model/cluster_details.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4583 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/api/model/inference_deployment.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    11259 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/model/run.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.895731 mosaicml-cli-0.4.9/mcli/api/runs/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1199 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.9/mcli/api/runs/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2964 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/runs/api_create_run.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4362 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/runs/api_delete_runs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     8930 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/runs/api_get_run_logs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    11418 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/runs/api_get_runs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5364 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/runs/api_start_run.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5556 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/runs/api_stop_runs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4088 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/runs/api_update_run_metadata.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10619 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.9/mcli/api/runs/api_watch_run.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.896223 mosaicml-cli-0.4.9/mcli/api/schema/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.9/mcli/api/schema/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      636 2022-08-23 15:11:52.000000 mosaicml-cli-0.4.9/mcli/api/schema/generic_model.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.897215 mosaicml-cli-0.4.9/mcli/api/secrets/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      309 2022-09-23 17:32:12.000000 mosaicml-cli-0.4.9/mcli/api/secrets/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2386 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/api/secrets/api_create_secret.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3010 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/api/secrets/api_delete_secrets.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3709 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/api/secrets/api_get_secrets.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2354 2022-03-24 04:29:23.000000 mosaicml-cli-0.4.9/mcli/api/typing_future.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.897557 mosaicml-cli-0.4.9/mcli/api/users/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      139 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.9/mcli/api/users/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2715 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/api/users/api_get_users.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      920 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/api/utils.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.897908 mosaicml-cli-0.4.9/mcli/cli/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.9/mcli/cli/__init__.py
+-rwxr-xr-x   0 tylerlee   (502) staff       (20)     6383 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/cli.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.898487 mosaicml-cli-0.4.9/mcli/cli/common/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.9/mcli/cli/common/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2560 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/cli/common/deployment_filters.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6937 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/common/run_filters.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.898792 mosaicml-cli-0.4.9/mcli/cli/m_connect/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.9/mcli/cli/m_connect/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6143 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/cli/m_connect/m_connect.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.899300 mosaicml-cli-0.4.9/mcli/cli/m_create/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.9/mcli/cli/m_create/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2385 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_create/m_create.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    16900 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/cli/m_create/secret.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.900141 mosaicml-cli-0.4.9/mcli/cli/m_delete/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.9/mcli/cli/m_delete/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6448 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/cli/m_delete/delete.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5804 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/m_delete/m_delete.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.900568 mosaicml-cli-0.4.9/mcli/cli/m_deploy/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.9/mcli/cli/m_deploy/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4001 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/cli/m_deploy/m_deploy.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.901439 mosaicml-cli-0.4.9/mcli/cli/m_describe/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-01-26 00:46:18.000000 mosaicml-cli-0.4.9/mcli/cli/m_describe/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3929 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/cli/m_describe/describe_inference_deployments.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     9433 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/m_describe/describe_runs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2002 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.9/mcli/cli/m_describe/m_describe.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.903319 mosaicml-cli-0.4.9/mcli/cli/m_get/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      467 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_get/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     7136 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/m_get/clusters.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6447 2023-05-24 19:54:07.000000 mosaicml-cli-0.4.9/mcli/cli/m_get/display.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5668 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/m_get/inference_deployments.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4802 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/m_get/m_get.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     8027 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/m_get/runs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2189 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_get/secrets.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1580 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.9/mcli/cli/m_get/users.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.903708 mosaicml-cli-0.4.9/mcli/cli/m_init/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.9/mcli/cli/m_init/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3908 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/cli/m_init/m_init.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.905003 mosaicml-cli-0.4.9/mcli/cli/m_interactive/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.9/mcli/cli/m_interactive/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6793 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/cli/m_interactive/interactive.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    44284 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_interactive/kube_config.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     9487 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/m_interactive/m_interactive.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.906198 mosaicml-cli-0.4.9/mcli/cli/m_kube/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_kube/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5523 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_kube/m_get_config.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1398 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_kube/m_kube.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2050 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_kube/m_merge_config.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6946 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_kube/utils.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.906503 mosaicml-cli-0.4.9/mcli/cli/m_log/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.9/mcli/cli/m_log/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    11303 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/m_log/m_log.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.906792 mosaicml-cli-0.4.9/mcli/cli/m_ping/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.9/mcli/cli/m_ping/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1103 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/cli/m_ping/m_ping.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.907192 mosaicml-cli-0.4.9/mcli/cli/m_predict/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.9/mcli/cli/m_predict/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1661 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/cli/m_predict/m_predict.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.907519 mosaicml-cli-0.4.9/mcli/cli/m_root/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.9/mcli/cli/m_root/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      536 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_root/m_config.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.907781 mosaicml-cli-0.4.9/mcli/cli/m_run/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.9/mcli/cli/m_run/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     8219 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/m_run/m_run.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.908862 mosaicml-cli-0.4.9/mcli/cli/m_set_unset/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-10-04 23:53:41.000000 mosaicml-cli-0.4.9/mcli/cli/m_set_unset/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2964 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/cli/m_set_unset/api_key.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1793 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/cli/m_set_unset/feature_flag.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1940 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_set_unset/m_set.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1421 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_set_unset/m_unset.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      745 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/cli/m_set_unset/user.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.909184 mosaicml-cli-0.4.9/mcli/cli/m_stop/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-10-04 23:53:41.000000 mosaicml-cli-0.4.9/mcli/cli/m_stop/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4066 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/cli/m_stop/m_stop.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.909597 mosaicml-cli-0.4.9/mcli/cli/m_util/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-08-10 05:32:44.000000 mosaicml-cli-0.4.9/mcli/cli/m_util/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      797 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_util/m_util.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6837 2023-06-13 22:57:06.000000 mosaicml-cli-0.4.9/mcli/cli/m_util/util.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    12143 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/config.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.910986 mosaicml-cli-0.4.9/mcli/models/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1047 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/models/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2103 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/models/gpu_type.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10374 2023-06-13 22:57:11.000000 mosaicml-cli-0.4.9/mcli/models/inference_deployment_config.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      427 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/models/mcli_cluster.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      456 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/models/mcli_envvar.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6724 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/models/mcli_secret.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    19505 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/models/run_config.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.911291 mosaicml-cli-0.4.9/mcli/objects/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.9/mcli/objects/__init__.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.912922 mosaicml-cli-0.4.9/mcli/objects/secrets/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1090 2022-12-07 21:26:59.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/__init__.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.914112 mosaicml-cli-0.4.9/mcli/objects/secrets/create/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/create/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1646 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/create/base.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2244 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/create/docker_registry.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2408 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/create/gcp.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6377 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/create/generic.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3858 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/create/oci.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3001 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/create/s3.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5342 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/create/ssh.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      783 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/docker_registry.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1017 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/env_var.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      556 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/gcp.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1267 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/mounted.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      967 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/oci.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      961 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/s3.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1718 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/ssh.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.914387 mosaicml-cli-0.4.9/mcli/proto/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.9/mcli/proto/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1477 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.9/mcli/proto/mint_pb2.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.914608 mosaicml-cli-0.4.9/mcli/sdk/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1976 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/sdk/__init__.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.918207 mosaicml-cli-0.4.9/mcli/utils/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.9/mcli/utils/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5315 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/utils/utils_cli.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6073 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.9/mcli/utils/utils_config.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      740 2022-09-27 01:25:02.000000 mosaicml-cli-0.4.9/mcli/utils/utils_date.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10749 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/utils/utils_docker.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2225 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/utils/utils_epilog.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10774 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/utils/utils_interactive.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4527 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/utils/utils_logging.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2160 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.9/mcli/utils/utils_message_decoding.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6605 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/utils/utils_pypi.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3115 2023-03-15 17:23:44.000000 mosaicml-cli-0.4.9/mcli/utils/utils_rich.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5033 2023-06-06 15:18:59.000000 mosaicml-cli-0.4.9/mcli/utils/utils_run_status.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4350 2022-03-30 16:04:08.000000 mosaicml-cli-0.4.9/mcli/utils/utils_serializable_dataclass.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1103 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.9/mcli/utils/utils_spinner.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10751 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/utils/utils_string_functions.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1677 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/utils/utils_types.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1001 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.9/mcli/utils/utils_yaml.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3876 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/version.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.919120 mosaicml-cli-0.4.9/mosaicml_cli.egg-info/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      696 2023-06-15 20:53:05.000000 mosaicml-cli-0.4.9/mosaicml_cli.egg-info/PKG-INFO
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4922 2023-06-15 20:53:05.000000 mosaicml-cli-0.4.9/mosaicml_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 tylerlee   (502) staff       (20)        1 2023-06-15 20:53:05.000000 mosaicml-cli-0.4.9/mosaicml_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 tylerlee   (502) staff       (20)       75 2023-06-15 20:53:05.000000 mosaicml-cli-0.4.9/mosaicml_cli.egg-info/entry_points.txt
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1655 2023-06-15 20:53:05.000000 mosaicml-cli-0.4.9/mosaicml_cli.egg-info/requires.txt
+-rw-r--r--   0 tylerlee   (502) staff       (20)        5 2023-06-15 20:53:05.000000 mosaicml-cli-0.4.9/mosaicml_cli.egg-info/top_level.txt
+-rw-r--r--   0 tylerlee   (502) staff       (20)    31087 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/pyproject.toml
+-rw-r--r--   0 tylerlee   (502) staff       (20)       38 2023-06-15 20:53:05.920738 mosaicml-cli-0.4.9/setup.cfg
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3057 2023-06-13 22:57:11.000000 mosaicml-cli-0.4.9/setup.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.920139 mosaicml-cli-0.4.9/tests/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.9/tests/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      618 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/tests/conftest.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     7127 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/tests/test_config.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)       62 2022-03-03 05:25:48.000000 mosaicml-cli-0.4.9/tests/test_simple.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6116 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.9/tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.4.8/PKG-INFO` & `mosaicml-cli-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.8
+Version: 0.4.9
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.8/README.md` & `mosaicml-cli-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/__init__.py` & `mosaicml-cli-0.4.9/mcli/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/api/cluster/api_get_clusters.py` & `mosaicml-cli-0.4.9/mcli/api/cluster/api_get_clusters.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 query GetClusters(${VARIABLE_DATA_NAME}: GetClustersInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
     id
     name
     provider
     allowFractional
     allowMultinode
+    allowedSubmissionType
     allowedInstances {{
       name
       gpuType
       gpusPerNode
       gpuNums
       numNodes
       nodes {{
@@ -39,14 +40,15 @@
 }}"""
 QUERY_UTILIZATION = f"""
 query GetClusters(${VARIABLE_DATA_NAME}: GetClustersInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
     id
     name
     provider
+    allowedSubmissionType
     utilization {{
       clusterInstanceUtils {{
         clusterId
         gpuType
         gpusPerNode
         numNodes
         gpusUsed
```

### Comparing `mosaicml-cli-0.4.8/mcli/api/engine/engine.py` & `mosaicml-cli-0.4.9/mcli/api/engine/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -626,15 +626,15 @@
         endpoint,
         headers=headers,
         data=payload,
     )
     try:
         return response.json()
     except requests.JSONDecodeError as e:
-        mapi_error = MAPIException.from_requests_error(e)
+        mapi_error = MAPIException.from_bad_response(response)
         raise mapi_error from e
 
 
 def _deserialize_response(
     response: Dict[str, Any],
     query_function: str,
     model_type: Optional[Type[ModelT]],
```

### Comparing `mosaicml-cli-0.4.8/mcli/api/exceptions.py` & `mosaicml-cli-0.4.9/mcli/api/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -109,30 +109,35 @@
         # Optionally translate to a more specific error, if one matches
         if RunConfigException.match(message):
             return RunConfigException(status=status, message=message)
 
         return MAPIException(status=status, message=message)
 
     @classmethod
+    def from_bad_response(cls, response: requests.Response) -> MAPIException:
+        return MAPIException(
+            status=HTTPStatus(response.status_code),
+            message=response.reason,
+        )
+
+    @classmethod
     def from_requests_error(cls, error: requests.exceptions.RequestException) -> MAPIException:
         """Initializes a new exception based on a requests RequestException
         """
-        msg = 'Unable to connect'
+        msg = 'Unable to connect to MAPI'
         if error.args:
             con = error.args[0]
             try:
                 # Try to get the destination we tried to connect to
                 # if the app is fully not accessible
                 source = f'http://{con.pool.host}:{con.pool.port}{con.url}'
             except AttributeError:
-                # Not all RequestException have pool information, examples:
-                #   1.  app is partially up but not fully responding
-                #   2.  host is correct but full URL is not
-                source = 'MAPI'
-            msg = f'{msg} to {source}'
+                pass
+            else:
+                msg = f'{msg} at {source}'
         return MAPIException(status=HTTPStatus.SERVICE_UNAVAILABLE, message=msg)
 
 
 class MintException(MCLIException):
     """Exception raised when connection to MINT fails or is broken
     """
```

### Comparing `mosaicml-cli-0.4.8/mcli/api/inference_deployments/__init__.py` & `mosaicml-cli-0.4.9/mcli/api/inference_deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_create_inference_deployment.py` & `mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_create_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_delete_inference_deployments.py` & `mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_delete_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_get_inference_deployment_logs.py` & `mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_get_inference_deployment_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_get_inference_deployments.py` & `mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_get_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_ping.py` & `mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_predict_inference_deployment.py` & `mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_predict_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/api/inference_deployments/api_update_inference_deployments.py` & `mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_update_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/api/mint/shell.py` & `mosaicml-cli-0.4.9/mcli/api/mint/shell.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/api/mint/tty.py` & `mosaicml-cli-0.4.9/mcli/api/mint/tty.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/api/model/__init__.py` & `mosaicml-cli-0.4.9/mcli/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/api/model/cluster_details.py` & `mosaicml-cli-0.4.9/mcli/api/model/cluster_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -157,14 +157,15 @@
     """
 
     name: str
     provider: str = 'MosaicML'
     allow_fractional: bool = False
     allow_multinode: bool = False
     cluster_instances: List[Instance] = field(default_factory=list)
+    submission_type: str = ''
     utilization: Optional[ClusterUtilization] = None
 
     kubernetes_context: str = ''
     namespace: str = ''
 
     id: Optional[str] = None
 
@@ -174,12 +175,13 @@
         utilization = None if 'utilization' not in response else ClusterUtilization.from_mapi_response(
             response['utilization'])
         return cls(name=response['name'],
                    provider=get_provider_name(response.get('provider', '')),
                    allow_fractional=response.get('allowFractional', False),
                    allow_multinode=response.get('allowMultinode', False),
                    cluster_instances=[Instance.from_mapi_response(i) for i in response.get('allowedInstances', [])],
+                   submission_type=str(response.get('allowedSubmissionType', '')),
                    utilization=utilization,
                    id=response.get('id'))
 
     def __lt__(self, other: ClusterDetails):
         return self.name < other.name
```

### Comparing `mosaicml-cli-0.4.8/mcli/api/model/inference_deployment.py` & `mosaicml-cli-0.4.9/mcli/api/model/inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/api/model/run.py` & `mosaicml-cli-0.4.9/mcli/api/model/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dataclasses import dataclass, field
 from datetime import datetime
 from http import HTTPStatus
 from typing import Any, Dict, List, Optional, Tuple
 
 from mcli.api.exceptions import MAPIException
 from mcli.api.schema.generic_model import DeserializableModel, convert_datetime
-from mcli.models.run_config import FinalRunConfig, RunConfig
+from mcli.models.run_config import RunConfig
 from mcli.utils.utils_run_status import RunStatus
 
 
 @dataclass
 class Node(DeserializableModel):
     """Node linked to a run
     """
@@ -29,33 +29,33 @@
 
 
 @dataclass
 class RunLifecycle:
     """Status of a run at a moment in time
     """
 
-    attempt_id: int
+    resumption_id: int
     status: RunStatus
     started_at: datetime
     ended_at: Optional[datetime] = None
     reason: Optional[str] = None
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]) -> RunLifecycle:
         return RunLifecycle(
-            attempt_id=response['executionIndex'],
+            resumption_id=response['executionIndex'],
             status=RunStatus.from_string(response['status']),
             started_at=convert_datetime(response['startTime']),
             ended_at=convert_datetime(response['endTime']) if response['endTime'] else None,
             reason=response.get('reason'),
         )
 
     def to_dict(self):
         return {
-            "attempt_id": str(self.attempt_id),
+            "resumption_id": str(self.resumption_id),
             "status": self.status,
             "started_at": str(self.started_at),
             "ended_at": str(self.ended_at),
             "reason": self.reason
         }
 
 
@@ -79,34 +79,48 @@
     """
 
     run_uid: str
     name: str
     status: RunStatus
     created_at: datetime
     updated_at: datetime
-    config: FinalRunConfig
     created_by: str
+    priority: str
+    preemptible: bool
+    retry_on_system_failure: bool
+    cluster: str
+    gpus: int
+    gpu_type: str
+    cpus: int
+    node_count: int
 
+    max_retries: Optional[int] = None
     started_at: Optional[datetime] = None
     completed_at: Optional[datetime] = None
     reason: Optional[str] = None
     nodes: List[Node] = field(default_factory=list)
     submitted_config: Optional[RunConfig] = None
     metadata: Optional[Dict[str, Any]] = None
-    last_attempt_id: Optional[str] = None
+    last_resumption_id: Optional[str] = None
     lifecycle: List[RunLifecycle] = field(default_factory=list)
+    image: Optional[str] = None
 
     _required_properties: Tuple[str] = tuple([
         'id',
         'name',
         'status',
         'createdAt',
+        'completedAt',
         'updatedAt',
-        'runInput',
+        'reason',
         'createdByEmail',
+        'priority',
+        'preemptible',
+        'retryOnSystemFailure',
+        'lastExecution',
     ])
 
     def _get_time_in_status(self, status: RunStatus) -> float:
         """Returns the time spent in a given status
 
         Args:
             status (:class:`~mcli.utils.utils_run_status.RunStatus`): The status to get the time for
@@ -139,21 +153,21 @@
 
         Returns:
             The cumulative time (seconds) spent in the RUNNING state
         """
         return self._get_time_in_status(RunStatus.RUNNING)
 
     @property
-    def attempts(self) -> int:
-        """Number of times the run has been attempted
+    def resumptions(self) -> int:
+        """Number of times the run has been resumed
 
         Returns:
-            The number of times the run has been attempted
+            The number of times the run has been resumed
         """
-        return len({i.attempt_id for i in self.lifecycle})
+        return len({i.resumption_id for i in self.lifecycle})
 
     def clone(
         self,
         name: Optional[str] = None,
         image: Optional[str] = None,
         cluster: Optional[str] = None,
         instance: Optional[str] = None,
@@ -283,24 +297,33 @@
             'run_uid': response['id'],
             'name': response['name'],
             'created_at': convert_datetime(response['createdAt']),
             'started_at': started_at,
             'completed_at': completed_at,
             'updated_at': convert_datetime(response['updatedAt']),
             'status': RunStatus.from_string(response['status']),
-            'created_by': response['createdByEmail'],
-            'config': FinalRunConfig.from_mapi_response(response['runInput']),
             'reason': response['reason'],
+            'created_by': response['createdByEmail'],
+            'priority': response['priority'],
+            'max_retries': response.get('maxRetries'),
+            'preemptible': response['preemptible'],
+            'retry_on_system_failure': response['retryOnSystemFailure'],
+            'cluster': response['lastExecution']['clusterName'],
+            'gpus': response['lastExecution']['gpus'],
+            'gpu_type': response['lastExecution']['gpuType'],
+            'cpus': response['lastExecution']['cpus'],
+            'node_count': response['lastExecution']['nodes'],
         }
 
         details = response.get('details', {})
         if details:
             submitted_run_input = details.get('originalRunInput')
             args['submitted_config'] = RunConfig.from_mapi_response(
                 submitted_run_input) if submitted_run_input is not None else None
 
             args['metadata'] = details.get('metadata')
-            args['last_attempt_id'] = details.get('lastExecutionId')
+            args['last_resumption_id'] = details.get('lastExecutionId')
             args['lifecycle'] = [RunLifecycle.from_mapi_response(l) for l in details.get('lifecycle', [])]
             args['nodes'] = [Node.from_mapi_response(n) for n in details.get('nodes', [])]
+            args['image'] = details.get('image')
 
         return cls(**args)
```

### Comparing `mosaicml-cli-0.4.8/mcli/api/runs/__init__.py` & `mosaicml-cli-0.4.9/mcli/api/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/api/runs/api_create_run.py` & `mosaicml-cli-0.4.9/mcli/api/runs/api_create_run.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,22 +15,32 @@
 QUERY_FUNCTION = 'createRun'
 VARIABLE_DATA_NAME = 'createRunData'
 QUERY = f"""
 mutation CreateRun(${VARIABLE_DATA_NAME}: CreateRunInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
     id
     name
-    runInput
     createdByEmail
     status
     createdAt
     startedAt
     completedAt
     updatedAt
     reason
+    priority
+    maxRetries
+    preemptible
+    retryOnSystemFailure
+    lastExecution {{
+        clusterName
+        cpus
+        gpuType
+        gpus
+        nodes
+    }}
     details {{
         originalRunInput
         metadata
         lastExecutionId
     }}
   }}
 }}"""
```

### Comparing `mosaicml-cli-0.4.8/mcli/api/runs/api_delete_runs.py` & `mosaicml-cli-0.4.9/mcli/api/runs/api_delete_runs.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,22 +15,32 @@
 QUERY_FUNCTION = 'deleteRuns'
 VARIABLE_DATA_NAME = 'getRunsData'
 QUERY = f"""
 mutation DeleteRuns(${VARIABLE_DATA_NAME}: GetRunsInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
     id
     name
-    runInput
     createdByEmail
     status
     createdAt
     startedAt
     completedAt
     updatedAt
     reason
+    priority
+    maxRetries
+    preemptible
+    retryOnSystemFailure
+    lastExecution {{
+        clusterName
+        cpus
+        gpuType
+        gpus
+        nodes
+    }}
   }}
 }}"""
 
 
 @overload
 def delete_run(
     run: Union[str, Run],
```

### Comparing `mosaicml-cli-0.4.8/mcli/api/runs/api_get_run_logs.py` & `mosaicml-cli-0.4.9/mcli/api/runs/api_get_run_logs.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,40 +25,40 @@
 def get_run_logs(
     run: Union[str, Run],
     rank: Optional[int] = None,
     *,
     timeout: Optional[float] = None,
     future: Literal[False] = False,
     failed: Optional[bool] = False,
-    attempt: Optional[int] = None,
+    resumption: Optional[int] = None,
 ) -> Generator[str, None, None]:
     ...
 
 
 @overload
 def get_run_logs(
     run: Union[str, Run],
     rank: Optional[int] = None,
     *,
     timeout: Optional[float] = None,
     future: Literal[True] = True,
     failed: Optional[bool] = False,
-    attempt: Optional[int] = None,
+    resumption: Optional[int] = None,
 ) -> Generator[Future[str], None, None]:
     ...
 
 
 def get_run_logs(
     run: Union[str, Run],
     rank: Optional[int] = None,
     *,
     timeout: Optional[float] = None,
     future: bool = False,
     failed: Optional[bool] = False,
-    attempt: Optional[int] = None,
+    resumption: Optional[int] = None,
 ) -> Union[Generator[str, None, None], Generator[Future[str], None, None]]:
     """Get the current logs for an active or completed run
 
     Get the current logs for an active or completed run in the MosaicML platform.
     This returns the full logs as a ``str``, as they exist at the time the request is
     made. If you want to follow the logs for an active run line-by-line, use
     :func:`follow_run_logs`.
@@ -72,33 +72,33 @@
             If the the call takes too long, a :exc:`~concurrent.futures.TimeoutError`
             will be raised. If ``future`` is ``True``, this value will be ignored.
         future (``bool``): Return the output as a :class:`~concurrent.futures.Future` . If True, the
             call to :func:`get_run_logs` will return immediately and the request will be
             processed in the background. This takes precedence over the ``timeout``
             argument. To get the log text, use ``return_value.result()`` with an optional
             ``timeout`` argument.
-        failed (``bool``): Return the logs of the first failed rank for the provided attempt if ``True``.
+        failed (``bool``): Return the logs of the first failed rank for the provided resumption if ``True``.
             ``False`` by default.
-        attempt (``Optional[int]``): Attempt (0-indexed) of a run to get logs for. Defaults to the last attempt
+        resumption (``Optional[int]``): Resumption (0-indexed) of a run to get logs for. Defaults to the last resumption
 
     Returns:
         If future is False:
             The full log text for a run at the time of the request as a :obj:`str`
         Otherwise:
             A :class:`~concurrent.futures.Future` for the log text
     """
     # Convert to strings
     run_name = run.name if isinstance(run, Run) else run
 
     filters: Dict[str, Any] = {'name': run_name, 'follow': False, 'failed': failed}
     if rank is not None:
         filters['nodeRank'] = rank
 
-    if attempt is not None:
-        filters['attemptIndex'] = attempt
+    if resumption is not None:
+        filters['attemptIndex'] = resumption
 
     cfg = MCLIConfig.load_config()
     if cfg.user_id:
         filters['entity'] = {
             'userIds': [cfg.user_id],
         }
 
@@ -116,38 +116,38 @@
 @overload
 def follow_run_logs(
     run: Union[str, Run],
     rank: Optional[int] = None,
     *,
     timeout: Optional[float] = None,
     future: Literal[False] = False,
-    attempt: Optional[int] = None,
+    resumption: Optional[int] = None,
 ) -> Generator[str, None, None]:
     ...
 
 
 @overload
 def follow_run_logs(
     run: Union[str, Run],
     rank: Optional[int] = None,
     *,
     timeout: Optional[float] = None,
     future: Literal[True] = True,
-    attempt: Optional[int] = None,
+    resumption: Optional[int] = None,
 ) -> Generator[Future[str], None, None]:
     ...
 
 
 def follow_run_logs(
     run: Union[str, Run],
     rank: Optional[int] = None,
     *,
     timeout: Optional[float] = None,
     future: bool = False,
-    attempt: Optional[int] = None,
+    resumption: Optional[int] = None,
 ) -> Union[Generator[str, None, None], Generator[Future[str], None, None]]:
     """Follow the logs for an active or completed run in the MosaicML platform
 
     This returns a :obj:`generator` of individual log lines, line-by-line, and will wait until
     new lines are produced if the run is still active.
 
     Args:
@@ -177,16 +177,16 @@
     # Convert to strings
     run_name = run.name if isinstance(run, Run) else run
 
     filters: Dict[str, Any] = {'name': run_name, 'follow': True}
     if rank is not None:
         filters['nodeRank'] = rank
 
-    if attempt is not None:
-        filters['attemptIndex'] = attempt
+    if resumption is not None:
+        filters['attemptIndex'] = resumption
 
     cfg = MCLIConfig.load_config()
     if cfg.user_id:
         filters['entity'] = {
             'userIds': [cfg.user_id],
         }
```

### Comparing `mosaicml-cli-0.4.8/mcli/api/runs/api_get_runs.py` & `mosaicml-cli-0.4.9/mcli/api/runs/api_get_runs.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,16 +28,26 @@
     name
     status
     createdAt
     startedAt
     completedAt
     updatedAt
     reason
-    runInput
     createdByEmail
+    priority
+    maxRetries
+    preemptible
+    retryOnSystemFailure
+    lastExecution {{
+        clusterName
+        cpus
+        gpuType
+        gpus
+        nodes
+    }}
   }}
 }}"""
 
 QUERY_WITH_DETAILS = f"""
 query GetRuns(${VARIABLE_DATA_NAME}: GetRunsInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
     id
@@ -45,16 +55,27 @@
     status
     createdAt
     startedAt
     completedAt
     updatedAt
     reason
     createdByEmail
-    runInput
+    priority
+    maxRetries
+    preemptible
+    retryOnSystemFailure
+    lastExecution {{
+        clusterName
+        cpus
+        gpuType
+        gpus
+        nodes
+    }}
     details {{
+        image
         originalRunInput
         metadata
         lastExecutionId
         lifecycle {{
             executionIndex
             status
             startTime
@@ -79,16 +100,26 @@
     name
     status
     createdAt
     startedAt
     completedAt
     updatedAt
     reason
-    runInput
     createdByEmail
+    priority
+    maxRetries
+    preemptible
+    retryOnSystemFailure
+    lastExecution {{
+        clusterName
+        cpus
+        gpuType
+        gpus
+        nodes
+    }}
   }}
   }}
 }}"""
 
 
 @overload
 def get_run(
```

### Comparing `mosaicml-cli-0.4.8/mcli/api/runs/api_start_run.py` & `mosaicml-cli-0.4.9/mcli/api/runs/api_start_run.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,22 +15,32 @@
 QUERY_FUNCTION = 'startRuns'
 VARIABLE_DATA_NAME = 'getRunsData'
 QUERY = f"""
 mutation StartRuns(${VARIABLE_DATA_NAME}: GetRunsInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
     id
     name
-    runInput
     createdByEmail
     status
     createdAt
     startedAt
     completedAt
     updatedAt
     reason
+    priority
+    maxRetries
+    preemptible
+    retryOnSystemFailure
+    lastExecution {{
+        clusterName
+        cpus
+        gpuType
+        gpus
+        nodes
+    }}
   }}
 }}"""
 
 
 @overload
 def start_run(
     run: Union[str, Run],
```

### Comparing `mosaicml-cli-0.4.8/mcli/api/runs/api_stop_runs.py` & `mosaicml-cli-0.4.9/mcli/api/runs/api_stop_runs.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,22 +15,32 @@
 QUERY_FUNCTION = 'stopRuns'
 VARIABLE_DATA_NAME = 'getRunsData'
 QUERY = f"""
 mutation StopRuns(${VARIABLE_DATA_NAME}: GetRunsInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
     id
     name
-    runInput
     createdByEmail
     status
     createdAt
     startedAt
     completedAt
     updatedAt
     reason
+    priority
+    maxRetries
+    preemptible
+    retryOnSystemFailure
+    lastExecution {{
+        clusterName
+        cpus
+        gpuType
+        gpus
+        nodes
+    }}
   }}
 }}"""
 
 
 @overload
 def stop_run(
     run: Union[str, Run],
```

### Comparing `mosaicml-cli-0.4.8/mcli/api/runs/api_update_run_metadata.py` & `mosaicml-cli-0.4.9/mcli/api/runs/api_update_run_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,22 +16,32 @@
 VARIABLE_DATA_GET_RUNS = 'getRunsData'
 VARIABLE_DATA_UPDATE_RUN_METADATA = 'updateRunMetadataData'
 QUERY = f"""
 mutation UpdateRunMetadata(${VARIABLE_DATA_GET_RUNS}: GetRunsInput!, ${VARIABLE_DATA_UPDATE_RUN_METADATA}: UpdateRunMetadataInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_GET_RUNS}: ${VARIABLE_DATA_GET_RUNS}, {VARIABLE_DATA_UPDATE_RUN_METADATA}: ${VARIABLE_DATA_UPDATE_RUN_METADATA}) {{
     id
     name
-    runInput
     createdByEmail
     status
     createdAt
     startedAt
     completedAt
     updatedAt
     reason
+    priority
+    maxRetries
+    preemptible
+    retryOnSystemFailure
+    lastExecution {{
+        clusterName
+        cpus
+        gpuType
+        gpus
+        nodes
+    }}
     details {{
         metadata
     }}
   }}
 }}"""
```

### Comparing `mosaicml-cli-0.4.8/mcli/api/runs/api_watch_run.py` & `mosaicml-cli-0.4.9/mcli/api/runs/api_watch_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/api/schema/generic_model.py` & `mosaicml-cli-0.4.9/mcli/api/schema/generic_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/api/secrets/api_create_secret.py` & `mosaicml-cli-0.4.9/mcli/api/secrets/api_create_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/api/secrets/api_delete_secrets.py` & `mosaicml-cli-0.4.9/mcli/api/secrets/api_delete_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/api/secrets/api_get_secrets.py` & `mosaicml-cli-0.4.9/mcli/api/secrets/api_get_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/api/typing_future.py` & `mosaicml-cli-0.4.9/mcli/api/typing_future.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/api/users/api_get_users.py` & `mosaicml-cli-0.4.9/mcli/api/users/api_get_users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/api/utils.py` & `mosaicml-cli-0.4.9/mcli/api/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/cli.py` & `mosaicml-cli-0.4.9/mcli/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         kube_interactive_argparser(subparser=subparser)
 
     add_create_argparser(subparser=subparser)
     add_delete_argparser(subparser=subparser)
     add_deploy_argparser(subparser=subparser)
     add_describe_parser(subparser=subparser)
     add_get_argparser(subparser=subparser, is_admin=is_admin)
-    add_log_parser(subparser=subparser, submission_type=SubmissionType.RUN)
+    add_log_parser(subparser=subparser, submission_type=SubmissionType.TRAINING)
     add_ping_parser(subparser=subparser)
     add_predict_parser(subparser=subparser)
     add_kube_argparser(subparser=subparser)
     add_run_argparser(subparser=subparser)
     add_stop_parser(subparser=subparser)
     add_util_argparser(subparser=subparser)
     add_set_argparser(subparser=subparser, is_admin=is_admin)
```

### Comparing `mosaicml-cli-0.4.8/mcli/cli/common/deployment_filters.py` & `mosaicml-cli-0.4.9/mcli/cli/common/deployment_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/common/run_filters.py` & `mosaicml-cli-0.4.9/mcli/cli/common/run_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 def configure_submission_filter_argparser(action: str,
                                           parser: argparse.ArgumentParser,
                                           include_all: bool = True,
-                                          submission_type: SubmissionType = SubmissionType.RUN) -> None:
+                                          submission_type: SubmissionType = SubmissionType.TRAINING) -> None:
     parser.add_argument(
         '-c',
         '--cluster',
         '-p',
         '--platform',
         dest='cluster_filter',
         metavar='CLUSTER',
@@ -69,15 +69,15 @@
         default=None,
         type=functools.partial(comma_separated, fun=int),
         help=f'{action.capitalize()} {submission_type.value}s with specific number of GPUs. '
         'Multiple values should be specified using a comma-separated list, e.g. "1,8"',
     )
 
     def status(value: str):
-        if submission_type.value == SubmissionType.RUN:
+        if submission_type.value == SubmissionType.TRAINING:
             res = comma_separated(value, RunStatus.from_string)
             if res == [RunStatus.UNKNOWN] and value != [RunStatus.UNKNOWN.value]:
                 raise TypeError(f'Unknown value {value}')
             return res
         else:
             res = comma_separated(value)
             return res
@@ -90,15 +90,15 @@
         metavar='STATUS',
         type=status,
         help=f'{action.capitalize()} {submission_type.value}s with the specified statuses (choices: '
         f'{", ".join(submission_type.get_status_options())}). Multiple statuses should be specified '
         'using a comma-separated list, e.g. "failed,pending"',
     )
 
-    if submission_type == SubmissionType.RUN:
+    if submission_type == SubmissionType.TRAINING:
         parser.add_argument(
             '-l',
             '--latest',
             action='store_true',
             dest='latest',
             default=False,
             help=f'Connect to the latest {submission_type.value}',
```

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_connect/m_connect.py` & `mosaicml-cli-0.4.9/mcli/cli/m_connect/m_connect.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_create/m_create.py` & `mosaicml-cli-0.4.9/mcli/cli/m_create/m_create.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_create/secret.py` & `mosaicml-cli-0.4.9/mcli/cli/m_create/secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_delete/delete.py` & `mosaicml-cli-0.4.9/mcli/cli/m_delete/delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_delete/m_delete.py` & `mosaicml-cli-0.4.9/mcli/cli/m_delete/m_delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         metavar='DEPLOYMENT',
         default=None,
         help='String or glob of the name(s) of the deployments to delete',
     )
     # backwards compatibility
     deployments_parser.add_argument('--name', dest='old_name_filter')
 
-    configure_submission_filter_argparser('delete', deployments_parser, submission_type=SubmissionType.DEPLOYMENT)
+    configure_submission_filter_argparser('delete', deployments_parser, submission_type=SubmissionType.INFERENCE)
     deployments_parser.set_defaults(func=delete_deployment)
     add_common_args(deployments_parser)
 
     return parser
 
 
 def add_delete_argparser(subparser: argparse._SubParsersAction,
```

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_deploy/m_deploy.py` & `mosaicml-cli-0.4.9/mcli/cli/m_deploy/m_deploy.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_describe/describe_inference_deployments.py` & `mosaicml-cli-0.4.9/mcli/cli/m_describe/describe_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_describe/describe_runs.py` & `mosaicml-cli-0.4.9/mcli/cli/m_describe/describe_runs.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from rich.table import Table
 
 from mcli.api.exceptions import cli_error_handler
 from mcli.api.model.run import Node, Run, RunLifecycle
 from mcli.cli.common.run_filters import get_runs_with_filters
 from mcli.cli.m_get.display import (MCLIDisplayItem, MCLIGetDisplay, OutputDisplay, create_vertical_display_table,
                                     format_timestamp)
-from mcli.models.run_config import DEFAULT_PRIORITY_NAME, ComputeConfig
+from mcli.models.run_config import ComputeConfig
 from mcli.utils.utils_logging import FormatString, console, format_string, print_timedelta, seconds_to_str
 
 logger = logging.getLogger(__name__)
 
 DISPLAY_RUN_STATUSES = ['PENDING', 'RUNNING', 'COMPLETED']
 
 
@@ -26,67 +26,63 @@
     RUNNING = 'RUNNING'
     COMPLETED = 'COMPLETED'
 
 
 class DescribeRunDetailColumns(Enum):
     NAME = 'name'
     RUN_ID = 'run_uid'
-    LAST_ATTEMPT_ID = 'last_attempt_id'
+    LAST_RESUMPTION_ID = 'last_resumption_id'
     CLUSTER = 'cluster'
     GPU_TYPE = 'gpu_type'
     GPU_NUM = 'gpu_num'
     CPUS = 'cpus'
     IMAGE = 'image'
     PRIORITY = 'priority'
 
 
 class DescribeRunOriginalInputColumns(Enum):
     SUBMITTED_CONFIG = 'submitted_config'
 
 
-RUN_DETAIL_DISPLAY_NAMES = ['Run Name', 'Run ID', 'Last Attempt ID', 'Cluster', 'Image', 'Priority']
+RUN_DETAIL_DISPLAY_NAMES = ['Run Name', 'Run ID', 'Last Resumption ID', 'Cluster', 'Image', 'Priority']
 
 RUN_LIFECYCLE_DISPLAY_NAMES = ['Status', 'Reached At', 'Duration', 'Reason']
 RUN_NODES_DISPLAY_NAMES = ['Node Name']
 SUBMITTED_CONFIG = ['Run Config']
 
 
 @dataclass
 class DescribeRunDetailDisplayItem(MCLIDisplayItem):
     """Tuple that extracts detailed run data for display purposes"""
     name: str
     run_uid: str
-    last_attempt_id: str
+    last_resumption_id: str
     cluster: str
     image: str
-    last_attempt_id: str
+    last_resumption_id: str
     priority: str
 
     @classmethod
     def from_run(cls, run: Run) -> DescribeRunDetailDisplayItem:
-        priority = run.config.scheduling.get('priority', None) or DEFAULT_PRIORITY_NAME
-        if priority and priority.lower() == 'default':
-            priority = DEFAULT_PRIORITY_NAME
-
         extracted: Dict[str, Any] = {
-            DescribeRunDetailColumns.NAME.value: run.config.name,
+            DescribeRunDetailColumns.NAME.value: run.name,
             DescribeRunDetailColumns.RUN_ID.value: run.run_uid,
-            DescribeRunDetailColumns.LAST_ATTEMPT_ID.value: run.last_attempt_id,
-            DescribeRunDetailColumns.CLUSTER.value: run.config.cluster,
-            DescribeRunDetailColumns.IMAGE.value: run.config.image,
-            DescribeRunDetailColumns.PRIORITY.value: priority.lower(),
+            DescribeRunDetailColumns.LAST_RESUMPTION_ID.value: run.last_resumption_id,
+            DescribeRunDetailColumns.CLUSTER.value: run.cluster,
+            DescribeRunDetailColumns.IMAGE.value: run.image,
+            DescribeRunDetailColumns.PRIORITY.value: run.priority.lower(),
         }
 
         return DescribeRunDetailDisplayItem(**extracted)
 
 
 @dataclass
 class DescribeRunLifecycleDisplayItem(MCLIDisplayItem):
     """Tuple that extracts run data for run lifecycle display purposes"""
-    attempt: str
+    resumption: str
     status: str
     reached_at: str
     duration: str
     reason: str
 
 
 @dataclass
@@ -141,25 +137,25 @@
     def __iter__(self) -> Generator[DescribeRunLifecycleDisplayItem, None, None]:
         last_index: Optional[int] = None
         for e in self.model:
             duration = ''
             if e.started_at and e.ended_at:
                 duration = print_timedelta(e.ended_at - e.started_at)
             yield DescribeRunLifecycleDisplayItem(
-                attempt=str(e.attempt_id) if last_index != e.attempt_id else '',
+                resumption=str(e.resumption_id) if last_index != e.resumption_id else '',
                 status=e.status.display_name,
                 reached_at=format_timestamp(e.started_at),
                 duration=duration,
                 reason=e.reason or '',
             )
-            last_index = e.attempt_id
+            last_index = e.resumption_id
 
     @property
     def index_label(self) -> str:
-        return 'attempt'
+        return 'resumption'
 
 
 class MCLIDescribeRunMetadataDisplay(MCLIGetDisplay):
     """ Vertical table view of run metadata """
 
     def __init__(self, metadata: Dict[str, Any]):
         self.columns = sorted(metadata.keys())
@@ -207,38 +203,37 @@
 @dataclass
 class DescribeComputeRequests():
     """Describer for compute requests"""
     cluster: Optional[str] = None
     gpu_type: Optional[str] = None
     gpus: Optional[int] = None
     cpus: Optional[int] = None
-    instance: Optional[str] = None
     nodes: Optional[int] = None
 
+    # TODO: add instance type
+
     @property
     def display_names(self) -> Dict[str, str]:
         # Return display name mapping for table
         return {
             'cluster': 'Cluster',
             'gpu_type': 'GPU Type',
             'gpus': 'GPUs',
             'cpus': 'CPUs',
-            'instance': 'Instance',
             'nodes': 'Nodes',
         }
 
     @classmethod
     def from_run(cls, run: Run) -> DescribeComputeRequests:
         return DescribeComputeRequests(
-            cluster=compute_or_deprecated(run.config.compute, 'cluster', run.config.cluster),
-            gpu_type=compute_or_deprecated(run.config.compute, 'gpu_type', run.config.gpu_type),
-            gpus=compute_or_deprecated(run.config.compute, 'gpus', run.config.gpu_num),
-            cpus=compute_or_deprecated(run.config.compute, 'cpus', run.config.cpus),
-            instance=run.config.compute.get('instance', None),
-            nodes=run.config.compute.get('nodes', None),
+            cluster=run.cluster,
+            gpu_type=run.gpu_type,
+            gpus=run.gpus,
+            cpus=run.cpus,
+            nodes=run.node_count,
         )
 
     def to_table(self) -> Table:
         data = {self.display_names.get(k, k.capitalize()): str(v) for k, v in asdict(self).items() if v is not None}
         columns = list(data.keys())
         values = [tuple(data.values())]
         return create_vertical_display_table(data=values, columns=columns)
@@ -274,15 +269,15 @@
     print()
 
     # Run lifecycle section
     print(format_string('Run Lifecycle', FormatString.BOLD))
     lifecycle_display = MCLIDescribeRunLifecycleDisplay(run.lifecycle)
     lifecycle_display.print(output)
     print()
-    print(f'Total Attempts: {run.attempts:,}')
+    print(f'Total Attempts: {run.resumptions:,}')
     print(f'Total time spent in Pending: {seconds_to_str(run.cumulative_pending_time)}')
     print(f'Total time spent in Running: {seconds_to_str(run.cumulative_running_time)}')
     print()
 
     if run.metadata:
         print(format_string('Run Metadata', FormatString.BOLD))
         metadata_display = MCLIDescribeRunMetadataDisplay(run.metadata)
```

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_describe/m_describe.py` & `mosaicml-cli-0.4.9/mcli/cli/m_describe/m_describe.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_get/clusters.py` & `mosaicml-cli-0.4.9/mcli/cli/m_get/clusters.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 from rich.table import Table
 
 from mcli.api.cluster import get_clusters as api_get_cluster
 from mcli.api.exceptions import cli_error_handler
 from mcli.api.model.cluster_details import ClusterDetails
 from mcli.cli.m_get.display import MCLIDisplayItem, MCLIGetDisplay, OutputDisplay, create_display_table
+from mcli.utils.utils_cli import SubmissionType
+from mcli.utils.utils_logging import FormatString, format_string
 
 logger = logging.getLogger(__name__)
 
 
 def get_gpu_description(gpus: int, nodes: int, allow_fractional: bool, allow_multinode: bool) -> str:
     """Get a string showing possible `gpus` values for the instance
 
@@ -91,42 +93,44 @@
 SEP = ['│']
 
 
 class ClusterDisplay(MCLIGetDisplay):
     """`mcli get cluster` display class
     """
 
-    def __init__(self, cluster: List[ClusterDetails], include_ids: bool = False):
+    def __init__(self, cluster: List[ClusterDetails], submission_type: SubmissionType, include_ids: bool = False):
         self.cluster = sorted(cluster)
         self.include_ids = include_ids
+        self.submission_type = submission_type
 
     def __iter__(self) -> Generator[ClusterDisplayItem, None, None]:
         for c in self.cluster:
             for instance in sorted(c.cluster_instances, reverse=True):
 
                 # cpu instance sometimes captures non-worker nodes, so we'll just set
                 # the value to 1 (unless it was 0)
                 nodes = get_nodes_description(instance.nodes, c.allow_multinode)
                 if instance.name == 'cpu' and nodes != '-':
                     nodes = '1'
 
-                yield ClusterDisplayItem(
-                    id=c.id if self.include_ids else None,
-                    name=c.name,
-                    provider=c.provider,
-                    instance=instance.name,
-                    nodes=nodes,
-                    gpu_type=instance.gpu_type.lower(),
-                    gpus=get_gpu_description(
-                        instance.gpus,
-                        instance.nodes,
-                        c.allow_fractional,
-                        c.allow_multinode,
-                    ),
-                )
+                if self.submission_type.name == c.submission_type:
+                    yield ClusterDisplayItem(
+                        id=c.id if self.include_ids else None,
+                        name=c.name,
+                        provider=c.provider,
+                        instance=instance.name,
+                        nodes=nodes,
+                        gpu_type=instance.gpu_type.lower(),
+                        gpus=get_gpu_description(
+                            instance.gpus,
+                            instance.nodes,
+                            c.allow_fractional,
+                            c.allow_multinode,
+                        ),
+                    )
 
     def to_name(self, items: List[Dict[str, Any]]) -> List[str]:
         """Customized name output for clusters that removes duplicates
         """
         return list({item['name']: None for item in items}.keys())
 
     def to_table(self, items: List[Dict[str, Any]]) -> Table:
@@ -187,11 +191,22 @@
     output: OutputDisplay = OutputDisplay.TABLE,
     include_ids: bool = False,
     **kwargs,
 ) -> int:
     del kwargs
 
     clusters = api_get_cluster()
-    display = ClusterDisplay(clusters, include_ids=include_ids)
-    display.print(output)
+    training_display = ClusterDisplay(clusters, SubmissionType.TRAINING, include_ids=include_ids)
+    if list(iter(training_display)):
+        print(format_string('Training Clusters', FormatString.BOLD))
+        training_display.print(output)
+    else:
+        print(format_string('No training clusters found', FormatString.BOLD))
+    print('\n')
+    inference_display = ClusterDisplay(clusters, SubmissionType.INFERENCE, include_ids=include_ids)
+    if list(iter(inference_display)):
+        print(format_string('Inference Clusters', FormatString.BOLD))
+        inference_display.print(output)
+    else:
+        print(format_string('No inference clusters found', FormatString.BOLD))
 
     return 0
```

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_get/display.py` & `mosaicml-cli-0.4.9/mcli/cli/m_get/display.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_get/inference_deployments.py` & `mosaicml-cli-0.4.9/mcli/cli/m_get/inference_deployments.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         default=None,
         help='String or glob of the name(s) of the deployments to get',
     )
 
     configure_submission_filter_argparser('get',
                                           deployments_parser,
                                           include_all=False,
-                                          submission_type=SubmissionType.DEPLOYMENT)
+                                          submission_type=SubmissionType.INFERENCE)
     deployments_parser.set_defaults(func=cli_get_deployments)
 
     deployments_parser.add_argument('--ids',
                                     action='store_true',
                                     dest='include_ids',
                                     default=config.ADMIN_MODE,
                                     help='Include the deployment ids in the output')
```

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_get/m_get.py` & `mosaicml-cli-0.4.9/mcli/cli/m_get/m_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     runs_parser = get_runs_argparser(subparsers)
     add_common_arguments(runs_parser)
     deployments_parser = get_deployments_argparser(subparsers)
     add_common_arguments(deployments_parser)
     deployment_details_parsers = deployments_parser.add_subparsers(title='Deployment Details')
 
     # mcli get deployment logs
-    add_log_parser(deployment_details_parsers, SubmissionType.DEPLOYMENT)
+    add_log_parser(deployment_details_parsers, SubmissionType.INFERENCE)
 
     return parser
 
 
 def add_get_argparser(subparser: argparse._SubParsersAction,
                       is_admin: bool = False,
                       parents: Optional[List[argparse.ArgumentParser]] = None) -> argparse.ArgumentParser:
```

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_get/runs.py` & `mosaicml-cli-0.4.9/mcli/cli/m_get/runs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Implementation of mcli get runs"""
 from __future__ import annotations
 
 import argparse
 import logging
-import math
 from dataclasses import dataclass
 from enum import Enum
-from typing import Dict, Generator, List, Optional, Tuple
+from typing import Dict, Generator, List, Optional
 
 from mcli import config
 from mcli.api.exceptions import cli_error_handler
 from mcli.api.model.run import Run
 from mcli.cli.common.run_filters import configure_submission_filter_argparser, get_runs_with_filters
 from mcli.cli.m_get.display import MCLIDisplayItem, MCLIGetDisplay, OutputDisplay, format_timestamp
 from mcli.utils.utils_cli import comma_separated
@@ -53,21 +52,21 @@
     id: Optional[str] = None
 
     @classmethod
     def from_run(cls, run: Run, include_ids: bool = False) -> RunDisplayItem:
         display_status = run.status.display_name
         if run.reason:
             display_status = f"{display_status} ({run.reason})"
-        instance, nodes = get_instance_name_and_nodes(run)
+        instance = get_instance_name(run)
         extracted: Dict[str, str] = {
             RunColumns.NAME.value: run.name,
             RunColumns.USER.value: run.created_by,
-            RunColumns.CLUSTER.value: run.config.cluster,
+            RunColumns.CLUSTER.value: run.cluster,
             RunColumns.INSTANCE.value: instance,
-            RunColumns.NODES.value: str(nodes),
+            RunColumns.NODES.value: str(run.node_count),
             RunColumns.CREATED_TIME.value: format_timestamp(run.created_at),
             RunColumns.START_TIME.value: format_timestamp(run.started_at),
             RunColumns.END_TIME.value: format_timestamp(run.completed_at),
             RunColumns.STATUS.value: display_status,
         }
         if include_ids:
             extracted[RunColumns.ID.value] = run.run_uid
@@ -96,82 +95,41 @@
 
     def __iter__(self) -> Generator[RunDisplayItem, None, None]:
         for model in self.models:
             item = RunDisplayItem.from_run(model, include_ids=self.include_ids)
             yield item
 
 
-def get_instance_name_and_nodes(run: Run) -> Tuple[str, int]:
-    """Get the run's instance name and number of nodes
+def get_instance_name(run: Run) -> str:
+    """Get the run's instance name
 
     We'll try to create a human-readable name based on the gpu number and type (ie 8x v100),
     if possible.
 
-    With the addition of `compute` to the run config, all values should be filled in, so much
-    of the logic here is for older runs. These have a limited set of possible values, so we
-    make some assumptions which should largely be correct.
-
     Args:
         run (Run): a Run
 
     Returns:
-        Tuple[str, int]: The instance name and number of nodes
+        str: The instance name
     """
 
-    # Extract GPU Type
-    # Default to 'cpu' type
-    gpu_type = 'cpu'
-    if run.config.compute.get('gpu_type', None):
-        assert 'gpu_type' in run.config.compute  # for the linter
-        gpu_type = run.config.compute['gpu_type']
-        assert gpu_type is not None  # Also for the linter...
-    elif run.config.gpu_type:
-        gpu_type = run.config.gpu_type
+    gpu_type = run.gpu_type
 
     # Convert 'None' to 'cpu'
     if gpu_type.lower() == 'none':
         gpu_type = 'cpu'
 
-    # Extract GPU Number
-    # Default to 0 because some older runs may only set gpu type, which was probably "None"
-    total_gpus = 0
-    if 'gpus' in run.config.compute and run.config.compute['gpus'] is not None:
-        total_gpus = run.config.compute['gpus']
-    elif run.config.gpu_num is not None:
-        total_gpus = run.config.gpu_num
-
-    # Get the instance type as a fallback
-    instance = run.config.compute.get('instance', None)
-
-    # Get the number of nodes
-    nodes = run.config.compute.get('nodes', None)
-    if nodes is not None:
-        # Trim to gpus per node
-        gpus = int(total_gpus / nodes)
-    elif total_gpus > GPUS_PER_NODE:
-        # If we have more than 8 gpus, we can reasonably assume we're on multinode
-        # This assumes 8 gpus per node, which should be valid for all old runs
-        nodes = math.ceil(total_gpus / GPUS_PER_NODE)
-        gpus = GPUS_PER_NODE
-    else:
-        nodes = 1
-        gpus = total_gpus
-
     if gpu_type != 'cpu':
+        gpus = int(run.gpus / run.node_count) if run.node_count > 0 else run.gpus
+
         # Prefer the gpu type as a description, if available
-        return f"{gpus}x {gpu_type.lower()}", nodes
-    elif instance:
-        # Fall back on instance type (especially for cpu instances)
-        return instance, nodes
-    elif gpu_type == 'cpu':
-        # Otherwise just use "cpu"
-        return gpu_type, nodes
+        return f"{gpus}x {gpu_type.lower()}"
     else:
-        # Last resort, go with unknown
-        return 'unknown', nodes
+        # Otherwise just use "cpu", which is the default value
+        return gpu_type
 
 
 @cli_error_handler('mcli get runs')
 def cli_get_runs(
     name_filter: Optional[List[str]] = None,
     cluster_filter: Optional[List[str]] = None,
     before_filter: Optional[str] = None,
```

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_get/secrets.py` & `mosaicml-cli-0.4.9/mcli/cli/m_get/secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_get/users.py` & `mosaicml-cli-0.4.9/mcli/cli/m_get/users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_init/m_init.py` & `mosaicml-cli-0.4.9/mcli/cli/m_init/m_init.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_interactive/interactive.py` & `mosaicml-cli-0.4.9/mcli/cli/m_interactive/interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_interactive/kube_config.py` & `mosaicml-cli-0.4.9/mcli/cli/m_interactive/kube_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_interactive/m_interactive.py` & `mosaicml-cli-0.4.9/mcli/cli/m_interactive/m_interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
         namespace = simple_prompt(
             f'Which kube namespace should be used to connect to the interactive run? [{default_namespace}]',
             default=default_namespace,
             mandatory=False,
         )
 
-        pod_id = f"{run.last_attempt_id}-{rank}"
+        pod_id = f"{run.last_resumption_id}-{rank}"
         logger.info(f'{INFO} Waiting for session to start with pod [blue]{pod_id}[/]...')
         logger.info(f'{INFO} Press Ctrl+C to quit and interact with your session manually.')
         run = wait_for_run_status(run, status=RunStatus.RUNNING, timeout=300)
 
         rank_str = f"node rank [cyan]{rank}[/] of " if rank > 0 else ""
         logger.info(f'{OK} Connecting to {rank_str}interactive session [cyan]{run.name}[/]')
```

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_kube/m_get_config.py` & `mosaicml-cli-0.4.9/mcli/cli/m_kube/m_get_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_kube/m_kube.py` & `mosaicml-cli-0.4.9/mcli/cli/m_kube/m_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_kube/m_merge_config.py` & `mosaicml-cli-0.4.9/mcli/cli/m_kube/m_merge_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_kube/utils.py` & `mosaicml-cli-0.4.9/mcli/cli/m_kube/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_log/m_log.py` & `mosaicml-cli-0.4.9/mcli/cli/m_log/m_log.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 
 # Follow the logs for an ongoing run
 > mcli logs run-1234 --follow
 
 # View the logs for a failed run
 > mcli logs run-1234 --failed
 
-# View the logs for the run's first attempt
-> mcli logs run-1234 --attempt-index 0
+# View the logs for the run's first initial resumption
+> mcli logs run-1234 --resumption 0
 """
 
 # pylint: disable-next=invalid-name
 DEPLOYMENT_LOG_EXAMPLES = """
 
 Examples:
 
@@ -61,15 +61,15 @@
 
 # View the logs of a specific restart in a deployment
 > mcli get deployment logs deploy-1234 --restart 5
 """
 
 
 def _get_run_logs(run: Run, follow: bool, rank: Optional[int], failed: bool,
-                  attempt: Optional[int]) -> Tuple[Optional[str], int]:
+                  resumption: Optional[int]) -> Tuple[Optional[str], int]:
 
     if run.status == RunStatus.FAILED and not failed and rank is None:
         if run.reason and run.reason == "FailedImagePull":
             suggestion = 'Try `mcli describe run {run.name}` and double-check that your image name is correct.'
             logger.info(
                 f'{INFO} Run {run.name} has failed during image pull, so there are likely no logs. {suggestion}')
         else:
@@ -79,36 +79,36 @@
         failed = True
 
     if follow and run.status.before(RunStatus.RUNNING):
         with CloudEpilogSpinner(run, RunStatus.RUNNING) as watcher:
             run = watcher.follow()
 
     if run.status == RunStatus.FAILED_PULL:
-        CommonLog(logger).log_pod_failed_pull(run.name, run.config.image)
+        CommonLog(logger).log_pod_failed_pull(run.name, run.image)
         return '', 1
     elif run.status.before(RunStatus.QUEUED, inclusive=True):
         # Pod still waiting to be scheduled. Return
         logger.error(f'{FAIL} Run {run.name} has not been scheduled')
         return '', 1
     elif run.status.before(RunStatus.RUNNING):
         # Pod still not running, probably because follow==False
         logger.error(f'{FAIL} Run has not yet started. You can check the status with `mcli get runs` '
                      'and try again later.')
         return '', 1
 
     last_line: Optional[str] = None
     end: str = ''
     if follow:
-        for line in follow_run_logs(run, rank=rank, attempt=attempt):
+        for line in follow_run_logs(run, rank=rank, resumption=resumption):
             print(line, end=end)
             if line:
                 last_line = line
         return last_line, int(0)
     else:
-        log_lines = get_run_logs(run, rank=rank, failed=failed, attempt=attempt)
+        log_lines = get_run_logs(run, rank=rank, failed=failed, resumption=resumption)
         for line in log_lines:
             # When using progress bars we randomly get newlines added. By default,
             # kubernetes does not return empty lines when streaming, which is
             # replicated in `follow_run_logs`. We'll do that here for parity
             if line:
                 last_line = line
                 print(line, end='')
@@ -128,29 +128,29 @@
     return last_line, 0
 
 
 def get_with_filters(submission_type: SubmissionType,
                      name: Optional[str] = None,
                      latest: bool = False) -> Union[List[Run], List[InferenceDeployment]]:
     name_filter = [name] if name else None
-    if submission_type == SubmissionType.RUN:
+    if submission_type == SubmissionType.TRAINING:
         return get_runs_with_filters(name_filter=name_filter, latest=latest)
     else:
         return get_deployments_with_filters(name_filter=name_filter)
 
 
 # pylint: disable-next=too-many-statements
 def get_logs(
     submission_type: SubmissionType,
     submission_name: Optional[str] = None,
     rank: Optional[int] = None,
     restart: Optional[int] = None,
     follow: bool = False,
     failed: bool = False,
-    attempt: Optional[int] = None,
+    resumption: Optional[int] = None,
     **kwargs,
 ) -> int:
     del kwargs
 
     try:
         submission_type_str = submission_type.value.lower()
         with err_console.status(f'Getting {submission_type_str} details...') as spinner:
@@ -168,15 +168,15 @@
                 if not submissions:
                     raise MAPIException(status=HTTPStatus.NOT_FOUND,
                                         message=f'Could not find {submission_type_str}: [red]{submission_name}[/]')
 
         last_line: Optional[str] = None
         #Have to check type to satisfy pyright
         if isinstance(submissions[0], Run):
-            last_line, err = _get_run_logs(submissions[0], follow, rank, failed, attempt)
+            last_line, err = _get_run_logs(submissions[0], follow, rank, failed, resumption)
             if err == 1:
                 return 1
         elif isinstance(submissions[0], InferenceDeployment):
             last_line, err = _get_deployment_logs(submissions[0], restart)
             if err == 1:
                 return 1
 
@@ -200,45 +200,48 @@
 
         return 1
 
     return 0
 
 
 def configure_deployments_argparser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
-    parser.set_defaults(func=partial(get_logs, SubmissionType.DEPLOYMENT))
+    parser.set_defaults(func=partial(get_logs, SubmissionType.INFERENCE))
 
     parser.add_argument('submission_name',
                         metavar='DEPLOYMENT',
                         help='The name of the inference deployment to fetch logs for.')
     parser.add_argument('--restart',
                         type=int,
                         default=None,
                         help='Which restart to fetch logs for. If not provided, will fetch logs of most recent restart')
 
     return parser
 
 
 def configure_runs_argparser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
-    parser.set_defaults(func=partial(get_logs, SubmissionType.RUN))
+    parser.set_defaults(func=partial(get_logs, SubmissionType.TRAINING))
     parser.add_argument('submission_name',
                         metavar='RUN',
                         nargs='?',
                         help='The name of the run. If not provided, will return the logs of the latest run')
-    parser.add_argument('--attempt',
-                        type=int,
-                        default=None,
-                        metavar='N',
-                        dest='attempt',
-                        help="Attempt (0-indexed) of the run whose logs you'd like to view.")
+    parser.add_argument(
+        '--resumption',
+        type=int,
+        default=None,
+        metavar='N',
+        dest='resumption',
+        help='Resumption (0-indexed) of the run logs that you\'d like to view. '
+        'The default without the flag is the latest resumption.',
+    )
     rank_grp = parser.add_mutually_exclusive_group()
     rank_grp.add_argument('--rank',
                           type=int,
                           default=None,
                           metavar='N',
-                          help='Rank of the node in a multi-node run whose logs you\'d like to view')
+                          help='Rank of the node in a multi-node run logs that you\'d like to view')
     rank_grp.add_argument('--failed',
                           action='store_true',
                           dest='failed',
                           default=False,
                           help='Get the logs of the first failed node rank in a multinode run.')
     follow_grp = parser.add_mutually_exclusive_group()
     follow_grp.add_argument('--no-follow',
@@ -262,14 +265,14 @@
     """
 
     log_parser: argparse.ArgumentParser = subparser.add_parser(
         'logs',
         aliases=['log'],
         help=f'View the logs from a specific {submission_type.value.lower()}',
         description=f'View the logs of an ongoing, completed or failed {submission_type.value.lower()}',
-        epilog=RUN_LOG_EXAMPLES if submission_type == SubmissionType.RUN else DEPLOYMENT_LOG_EXAMPLES,
+        epilog=RUN_LOG_EXAMPLES if submission_type == SubmissionType.TRAINING else DEPLOYMENT_LOG_EXAMPLES,
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     log_parser = configure_runs_argparser(
-        log_parser) if submission_type == SubmissionType.RUN else configure_deployments_argparser(log_parser)
+        log_parser) if submission_type == SubmissionType.TRAINING else configure_deployments_argparser(log_parser)
 
     return log_parser
```

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_ping/m_ping.py` & `mosaicml-cli-0.4.9/mcli/cli/m_ping/m_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_predict/m_predict.py` & `mosaicml-cli-0.4.9/mcli/cli/m_predict/m_predict.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_root/m_config.py` & `mosaicml-cli-0.4.9/mcli/cli/m_root/m_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_run/m_run.py` & `mosaicml-cli-0.4.9/mcli/cli/m_run/m_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,28 +28,27 @@
     mock_parser = argparse.ArgumentParser()
     _configure_parser(mock_parser)
     mock_parser.print_help()
     return 1
 
 
 def follow_run(run: Run) -> int:
-    final_config = run.config
     last_status: Optional[RunStatus] = None
 
     with CloudEpilogSpinner(run, RunStatus.RUNNING) as watcher:
         run = watcher.follow()
         last_status = run.status
 
     # Wait timed out
     common_log = CommonLog(logger)
     if last_status is None:
         common_log.log_timeout()
         return 0
     elif last_status == RunStatus.FAILED_PULL:
-        common_log.log_pod_failed_pull(run.name, final_config.image)
+        common_log.log_pod_failed_pull(run.name, run.image)
         with console_status('Deleting failed run...'):
             delete_runs([run])
         return 1
     elif last_status == RunStatus.FAILED:
         common_log.log_pod_failed(run.name)
         return 1
     elif last_status.before(RunStatus.RUNNING):
```

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_set_unset/api_key.py` & `mosaicml-cli-0.4.9/mcli/cli/m_set_unset/api_key.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_set_unset/feature_flag.py` & `mosaicml-cli-0.4.9/mcli/cli/m_set_unset/feature_flag.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_set_unset/m_set.py` & `mosaicml-cli-0.4.9/mcli/cli/m_set_unset/m_set.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_set_unset/m_unset.py` & `mosaicml-cli-0.4.9/mcli/cli/m_set_unset/m_unset.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_set_unset/user.py` & `mosaicml-cli-0.4.9/mcli/cli/m_set_unset/user.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_stop/m_stop.py` & `mosaicml-cli-0.4.9/mcli/cli/m_stop/m_stop.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_util/m_util.py` & `mosaicml-cli-0.4.9/mcli/cli/m_util/m_util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/cli/m_util/util.py` & `mosaicml-cli-0.4.9/mcli/cli/m_util/util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/config.py` & `mosaicml-cli-0.4.9/mcli/config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/models/__init__.py` & `mosaicml-cli-0.4.9/mcli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/models/gpu_type.py` & `mosaicml-cli-0.4.9/mcli/models/gpu_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/models/inference_deployment_config.py` & `mosaicml-cli-0.4.9/mcli/models/inference_deployment_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/models/mcli_secret.py` & `mosaicml-cli-0.4.9/mcli/models/mcli_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/models/run_config.py` & `mosaicml-cli-0.4.9/mcli/models/run_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
                                                ensure_rfc1123_compatibility, snake_case_to_camel_case, validate_image,
                                                validate_rfc1123_name)
 
 logger = logging.getLogger(__name__)
 RUN_CONFIG_UID_LENGTH = 6
 VALID_OPTIMIZATION_LEVELS = frozenset([0, 1, 2, 3])
 MAX_RUN_NAME_LENGTH = MAX_KUBERNETES_LENGTH - RUN_CONFIG_UID_LENGTH - 1  # -1 for the dash
-DEFAULT_PRIORITY_NAME = 'medium'
 
 
 class SchedulingConfig(TypedDict, total=False):
     """Typed dictionary for nested scheduling configurations"""
     priority: Optional[str]
     resumable: Optional[bool]
     max_retries: Optional[int]
```

### Comparing `mosaicml-cli-0.4.8/mcli/objects/secrets/__init__.py` & `mosaicml-cli-0.4.9/mcli/objects/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/objects/secrets/create/base.py` & `mosaicml-cli-0.4.9/mcli/objects/secrets/create/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/objects/secrets/create/docker_registry.py` & `mosaicml-cli-0.4.9/mcli/objects/secrets/create/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/objects/secrets/create/gcp.py` & `mosaicml-cli-0.4.9/mcli/objects/secrets/create/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/objects/secrets/create/generic.py` & `mosaicml-cli-0.4.9/mcli/objects/secrets/create/generic.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/objects/secrets/create/oci.py` & `mosaicml-cli-0.4.9/mcli/objects/secrets/create/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/objects/secrets/create/s3.py` & `mosaicml-cli-0.4.9/mcli/objects/secrets/create/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/objects/secrets/create/ssh.py` & `mosaicml-cli-0.4.9/mcli/objects/secrets/create/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/objects/secrets/docker_registry.py` & `mosaicml-cli-0.4.9/mcli/objects/secrets/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/objects/secrets/env_var.py` & `mosaicml-cli-0.4.9/mcli/objects/secrets/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/objects/secrets/gcp.py` & `mosaicml-cli-0.4.9/mcli/objects/secrets/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/objects/secrets/mounted.py` & `mosaicml-cli-0.4.9/mcli/objects/secrets/mounted.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/objects/secrets/oci.py` & `mosaicml-cli-0.4.9/mcli/objects/secrets/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/objects/secrets/s3.py` & `mosaicml-cli-0.4.9/mcli/objects/secrets/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/objects/secrets/ssh.py` & `mosaicml-cli-0.4.9/mcli/objects/secrets/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/proto/mint_pb2.py` & `mosaicml-cli-0.4.9/mcli/proto/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/sdk/__init__.py` & `mosaicml-cli-0.4.9/mcli/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/utils/utils_cli.py` & `mosaicml-cli-0.4.9/mcli/utils/utils_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         if action.choices is not None and value not in action.choices:
             args = {'value': value, 'choices': ', '.join(map(repr, action.choices))}
             msg = get_choice_message(value, action)
             raise argparse.ArgumentError(action, msg % args)
 
 
 class SubmissionType(Enum):
-    RUN = "Run"
-    DEPLOYMENT = "Inference Deployment"
+    TRAINING = "Run"
+    INFERENCE = "Inference Deployment"
 
     def get_status_options(self):
-        if self == SubmissionType.RUN:
+        if self == SubmissionType.TRAINING:
             return CLI_STATUS_OPTIONS
         else:
             return ["Pending", "Starting", "Ready", "Failed", "Stopped"]
```

### Comparing `mosaicml-cli-0.4.8/mcli/utils/utils_config.py` & `mosaicml-cli-0.4.9/mcli/utils/utils_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/utils/utils_date.py` & `mosaicml-cli-0.4.9/mcli/utils/utils_date.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/utils/utils_docker.py` & `mosaicml-cli-0.4.9/mcli/utils/utils_docker.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/utils/utils_epilog.py` & `mosaicml-cli-0.4.9/mcli/utils/utils_epilog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/utils/utils_interactive.py` & `mosaicml-cli-0.4.9/mcli/utils/utils_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/utils/utils_logging.py` & `mosaicml-cli-0.4.9/mcli/utils/utils_logging.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/utils/utils_message_decoding.py` & `mosaicml-cli-0.4.9/mcli/utils/utils_message_decoding.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/utils/utils_pypi.py` & `mosaicml-cli-0.4.9/mcli/utils/utils_pypi.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/utils/utils_rich.py` & `mosaicml-cli-0.4.9/mcli/utils/utils_rich.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/utils/utils_run_status.py` & `mosaicml-cli-0.4.9/mcli/utils/utils_run_status.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/utils/utils_serializable_dataclass.py` & `mosaicml-cli-0.4.9/mcli/utils/utils_serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/utils/utils_spinner.py` & `mosaicml-cli-0.4.9/mcli/utils/utils_spinner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/utils/utils_string_functions.py` & `mosaicml-cli-0.4.9/mcli/utils/utils_string_functions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/utils/utils_types.py` & `mosaicml-cli-0.4.9/mcli/utils/utils_types.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/utils/utils_yaml.py` & `mosaicml-cli-0.4.9/mcli/utils/utils_yaml.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mcli/version.py` & `mosaicml-cli-0.4.9/mcli/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,14 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = '0.4.8'
+__version__ = '0.4.9'
 
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

### Comparing `mosaicml-cli-0.4.8/mosaicml_cli.egg-info/PKG-INFO` & `mosaicml-cli-0.4.9/mosaicml_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.8
+Version: 0.4.9
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.8/mosaicml_cli.egg-info/SOURCES.txt` & `mosaicml-cli-0.4.9/mosaicml_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/mosaicml_cli.egg-info/requires.txt` & `mosaicml-cli-0.4.9/mosaicml_cli.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -9,47 +9,47 @@
 questionary>=1.10.0
 rich>=10.16.2
 ruamel.yaml>=0.17.21
 typing_extensions>=4.0.1
 validators>=0.20.0
 
 [all]
-sphinx-panels==0.6.0
+yapf>=0.33.0
 sphinx-argparse==0.4.0
-sphinxcontrib-images>=0.9.4
-pre-commit>=2.17.0
+sphinxcontrib-serializinghtml==1.1.5
 sphinxemoji==0.2.0
-radon>=5.1.0
-isort>=5.9.3
+docutils>=0.17.0
+pylint>=2.12.2
+sphinx==4.4.0
+sphinxcontrib-devhelp>=1.0.2
+pre-commit>=2.17.0
+sphinx-panels==0.6.0
 pytest>=6.2.5
-sphinxcontrib-katex==0.9.4
-sphinxext-opengraph==0.8.2
+sphinx-copybutton==0.5.2
+sphinx-markdown-tables==0.0.17
 pyright==1.1.256
-sphinxcontrib-jsmath>=1.0.1
-pylint>=2.12.2
-pytest-cov>=4.0.0
-sphinx-rtd-theme==1.0.0
-sphinxcontrib-applehelp>=1.0.2
+sphinxcontrib-images>=0.9.4
 sphinx_external_toc==0.3.0
-sphinx-copybutton==0.5.2
-sphinxcontrib-htmlhelp>=2.0.0
+toml>=0.10.2
 sphinxcontrib-qthelp>=1.0.3
-sphinxcontrib-serializinghtml==1.1.5
 twine>=4.0.2
-myst-parser>=0.16.1
-docutils>=0.17.0
-yapf>=0.33.0
+sphinxcontrib-applehelp>=1.0.2
+radon>=5.1.0
+sphinxcontrib-htmlhelp>=2.0.0
 sphinx-design
 furo==2022.9.29
-build>=0.10.0
-sphinx==4.4.0
-sphinx-markdown-tables==0.0.17
-sphinxcontrib-devhelp>=1.0.2
-toml>=0.10.2
+sphinx-rtd-theme==1.0.0
+sphinxcontrib-jsmath>=1.0.1
+pytest-cov>=4.0.0
 pytest-mock>=3.7.0
+myst-parser>=0.16.1
+sphinxcontrib-katex==0.9.4
+sphinxext-opengraph==0.8.2
+build>=0.10.0
+isort>=5.9.3
 
 [dev]
 build>=0.10.0
 isort>=5.9.3
 pre-commit>=2.17.0
 pylint>=2.12.2
 pyright==1.1.256
```

### Comparing `mosaicml-cli-0.4.8/pyproject.toml` & `mosaicml-cli-0.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/setup.py` & `mosaicml-cli-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/tests/conftest.py` & `mosaicml-cli-0.4.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/tests/test_config.py` & `mosaicml-cli-0.4.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.8/tests/test_upgrade.py` & `mosaicml-cli-0.4.9/tests/test_upgrade.py`

 * *Files identical despite different names*

