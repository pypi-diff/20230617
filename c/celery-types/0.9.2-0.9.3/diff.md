# Comparing `tmp/celery-types-0.9.2.tar.gz` & `tmp/celery-types-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery-types-0.9.2.tar", max compression
+gzip compressed data, was "celery-types-0.9.3.tar", max compression
```

## Comparing `celery-types-0.9.2.tar` & `celery-types-0.9.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0    11357 2021-10-19 00:08:15.830205 celery-types-0.9.2/LICENSE
--rw-r--r--   0        0        0      900 2021-10-19 00:08:15.830461 celery-types-0.9.2/README.md
--rw-r--r--   0        0        0       63 2021-10-31 21:31:07.747114 celery-types-0.9.2/amqp-stubs/__init__.pyi
--rw-r--r--   0        0        0       70 2021-10-31 21:31:07.747326 celery-types-0.9.2/amqp-stubs/exceptions.pyi
--rw-r--r--   0        0        0       82 2021-10-31 21:31:07.747554 celery-types-0.9.2/billiard-stubs/__init__.pyi
--rw-r--r--   0        0        0       25 2021-10-31 21:31:07.747852 celery-types-0.9.2/billiard-stubs/einfo.pyi
--rw-r--r--   0        0        0      475 2021-10-31 21:31:07.748173 celery-types-0.9.2/billiard-stubs/exceptions.pyi
--rw-r--r--   0        0        0     1005 2021-10-31 21:31:07.748555 celery-types-0.9.2/celery-stubs/__init__.pyi
--rw-r--r--   0        0        0      108 2021-10-31 21:31:07.748810 celery-types-0.9.2/celery-stubs/_state.pyi
--rw-r--r--   0        0        0     2547 2021-10-31 21:31:07.749237 celery-types-0.9.2/celery-stubs/app/__init__.pyi
--rw-r--r--   0        0        0       16 2021-10-31 21:31:07.749444 celery-types-0.9.2/celery-stubs/app/amqp.pyi
--rw-r--r--   0        0        0    11982 2021-10-31 21:31:07.749850 celery-types-0.9.2/celery-stubs/app/base.pyi
--rw-r--r--   0        0        0       16 2021-10-31 21:31:07.750150 celery-types-0.9.2/celery-stubs/app/beat.pyi
--rw-r--r--   0        0        0     5875 2021-10-31 21:31:07.750447 celery-types-0.9.2/celery-stubs/app/control.pyi
--rw-r--r--   0        0        0       18 2021-10-31 21:31:07.750709 celery-types-0.9.2/celery-stubs/app/events.pyi
--rw-r--r--   0        0        0     1934 2021-10-31 21:31:07.750939 celery-types-0.9.2/celery-stubs/app/log.pyi
--rw-r--r--   0        0        0       70 2021-10-31 21:31:07.751173 celery-types-0.9.2/celery-stubs/app/registry.pyi
--rw-r--r--   0        0        0       18 2021-10-31 21:31:07.751399 celery-types-0.9.2/celery-stubs/app/routes.pyi
--rw-r--r--   0        0        0     7292 2021-11-03 02:11:34.134094 celery-types-0.9.2/celery-stubs/app/task.pyi
--rw-r--r--   0        0        0      118 2021-10-31 21:31:07.751907 celery-types-0.9.2/celery-stubs/app/utils.pyi
--rw-r--r--   0        0        0        0 2021-10-31 21:31:07.752166 celery-types-0.9.2/celery-stubs/apps/__init__.pyi
--rw-r--r--   0        0        0       76 2021-10-31 21:31:07.752416 celery-types-0.9.2/celery-stubs/apps/worker.pyi
--rw-r--r--   0        0        0        0 2021-10-31 21:31:07.752696 celery-types-0.9.2/celery-stubs/backends/__init__.pyi
--rw-r--r--   0        0        0       19 2021-10-31 21:31:07.752843 celery-types-0.9.2/celery-stubs/backends/base.pyi
--rw-r--r--   0        0        0    12999 2021-11-06 20:16:22.272339 celery-types-0.9.2/celery-stubs/canvas.pyi
--rw-r--r--   0        0        0        0 2021-10-31 21:31:07.753576 celery-types-0.9.2/celery-stubs/concurrency/__init__.pyi
--rw-r--r--   0        0        0       20 2021-10-31 21:31:07.753848 celery-types-0.9.2/celery-stubs/concurrency/base.pyi
--rw-r--r--   0        0        0     2789 2021-10-31 21:31:07.754112 celery-types-0.9.2/celery-stubs/exceptions.pyi
--rw-r--r--   0        0        0        0 2021-10-31 21:31:07.754325 celery-types-0.9.2/celery-stubs/loaders/__init__.pyi
--rw-r--r--   0        0        0      103 2021-10-31 21:31:07.754551 celery-types-0.9.2/celery-stubs/loaders/base.pyi
--rw-r--r--   0        0        0        0 2021-10-31 21:31:07.754712 celery-types-0.9.2/celery-stubs/local.pyi
--rw-r--r--   0        0        0     4050 2021-10-31 21:31:07.754985 celery-types-0.9.2/celery-stubs/result.pyi
--rw-r--r--   0        0        0     2882 2021-10-31 21:31:07.755222 celery-types-0.9.2/celery-stubs/schedules.pyi
--rw-r--r--   0        0        0     1502 2021-10-31 21:31:07.755466 celery-types-0.9.2/celery-stubs/signals.pyi
--rw-r--r--   0        0        0     1148 2021-10-31 21:31:07.755712 celery-types-0.9.2/celery-stubs/states.pyi
--rw-r--r--   0        0        0       42 2021-10-31 21:31:07.756055 celery-types-0.9.2/celery-stubs/utils/__init__.pyi
--rw-r--r--   0        0        0      109 2021-10-31 21:31:07.756228 celery-types-0.9.2/celery-stubs/utils/abstract.pyi
--rw-r--r--   0        0        0      325 2021-10-31 21:31:07.756388 celery-types-0.9.2/celery-stubs/utils/collections.pyi
--rw-r--r--   0        0        0       58 2021-10-31 21:31:07.756647 celery-types-0.9.2/celery-stubs/utils/dispatch/__init__.pyi
--rw-r--r--   0        0        0      344 2021-10-31 21:31:07.756840 celery-types-0.9.2/celery-stubs/utils/dispatch/signal.pyi
--rw-r--r--   0        0        0       53 2021-10-31 21:31:07.757038 celery-types-0.9.2/celery-stubs/utils/graph.pyi
--rw-r--r--   0        0        0      140 2021-10-31 21:31:07.757299 celery-types-0.9.2/celery-stubs/utils/log.pyi
--rw-r--r--   0        0        0       27 2021-10-31 21:31:07.757616 celery-types-0.9.2/celery-stubs/utils/objects.pyi
--rw-r--r--   0        0        0       19 2021-10-31 21:31:07.757930 celery-types-0.9.2/celery-stubs/utils/term.pyi
--rw-r--r--   0        0        0       23 2021-10-31 21:31:07.758146 celery-types-0.9.2/celery-stubs/utils/threads.pyi
--rw-r--r--   0        0        0       16 2021-10-31 21:31:07.758322 celery-types-0.9.2/celery-stubs/utils/time.pyi
--rw-r--r--   0        0        0       66 2021-10-31 21:31:07.758611 celery-types-0.9.2/celery-stubs/worker/__init__.pyi
--rw-r--r--   0        0        0     4511 2021-10-31 21:31:07.758836 celery-types-0.9.2/celery-stubs/worker/request.pyi
--rw-r--r--   0        0        0       26 2021-10-31 21:31:07.759019 celery-types-0.9.2/celery-stubs/worker/worker.pyi
--rw-r--r--   0        0        0        0 2021-10-31 21:31:07.759215 celery-types-0.9.2/django_celery_results-stubs/__init__.pyi
--rw-r--r--   0        0        0      895 2021-10-31 21:31:07.759471 celery-types-0.9.2/django_celery_results-stubs/managers.pyi
--rw-r--r--   0        0        0     1099 2021-10-31 21:31:07.759960 celery-types-0.9.2/django_celery_results-stubs/models.pyi
--rw-r--r--   0        0        0       20 2021-10-31 21:31:07.760226 celery-types-0.9.2/ephem-stubs/__init__.pyi
--rw-r--r--   0        0        0      290 2021-10-31 21:31:07.760426 celery-types-0.9.2/kombu-stubs/__init__.pyi
--rw-r--r--   0        0        0       55 2021-10-31 21:31:07.760568 celery-types-0.9.2/kombu-stubs/abstract.pyi
--rw-r--r--   0        0        0     1157 2021-10-31 21:31:07.760705 celery-types-0.9.2/kombu-stubs/connection.pyi
--rw-r--r--   0        0        0      121 2021-10-31 21:31:07.760835 celery-types-0.9.2/kombu-stubs/entity.pyi
--rw-r--r--   0        0        0      815 2021-10-31 21:31:07.760967 celery-types-0.9.2/kombu-stubs/exceptions.pyi
--rw-r--r--   0        0        0     1271 2021-10-31 21:31:07.761189 celery-types-0.9.2/kombu-stubs/message.pyi
--rw-r--r--   0        0        0       20 2021-10-31 21:31:07.761465 celery-types-0.9.2/kombu-stubs/messaging.pyi
--rw-r--r--   0        0        0       35 2021-10-31 21:31:07.761627 celery-types-0.9.2/kombu-stubs/pidbox.pyi
--rw-r--r--   0        0        0       71 2021-10-31 21:31:07.761789 celery-types-0.9.2/kombu-stubs/pools.pyi
--rw-r--r--   0        0        0       20 2021-10-31 21:31:07.762091 celery-types-0.9.2/kombu-stubs/resource.pyi
--rw-r--r--   0        0        0        0 2021-10-31 21:31:07.762441 celery-types-0.9.2/kombu-stubs/transport/__init__.pyi
--rw-r--r--   0        0        0       21 2021-10-31 21:31:07.762715 celery-types-0.9.2/kombu-stubs/transport/base.pyi
--rw-r--r--   0        0        0        0 2021-10-31 21:31:07.763074 celery-types-0.9.2/kombu-stubs/utils/__init__.pyi
--rw-r--r--   0        0        0      105 2021-10-31 21:31:07.763491 celery-types-0.9.2/kombu-stubs/utils/uuid.pyi
--rw-r--r--   0        0        0      989 2021-11-06 20:16:28.748779 celery-types-0.9.2/pyproject.toml
--rw-r--r--   0        0        0       68 2021-10-31 21:31:07.768488 celery-types-0.9.2/vine-stubs/__init__.pyi
--rw-r--r--   0        0        0        0 2021-10-31 21:31:07.768686 celery-types-0.9.2/vine-stubs/abstract.pyi
--rw-r--r--   0        0        0        0 2021-10-31 21:31:07.768840 celery-types-0.9.2/vine-stubs/funtools.pyi
--rw-r--r--   0        0        0       19 2021-10-31 21:31:07.769081 celery-types-0.9.2/vine-stubs/promises.pyi
--rw-r--r--   0        0        0        0 2021-10-31 21:31:07.769218 celery-types-0.9.2/vine-stubs/synchronization.pyi
--rw-r--r--   0        0        0     1925 2021-11-06 20:17:17.159733 celery-types-0.9.2/setup.py
--rw-r--r--   0        0        0     1578 2021-11-06 20:17:17.160283 celery-types-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-10-19 00:08:15.830205 celery-types-0.9.3/LICENSE
+-rw-r--r--   0        0        0      900 2021-10-19 00:08:15.830461 celery-types-0.9.3/README.md
+-rw-r--r--   0        0        0       63 2021-10-31 21:31:07.747114 celery-types-0.9.3/amqp-stubs/__init__.pyi
+-rw-r--r--   0        0        0       70 2021-10-31 21:31:07.747326 celery-types-0.9.3/amqp-stubs/exceptions.pyi
+-rw-r--r--   0        0        0       82 2021-10-31 21:31:07.747554 celery-types-0.9.3/billiard-stubs/__init__.pyi
+-rw-r--r--   0        0        0       25 2021-10-31 21:31:07.747852 celery-types-0.9.3/billiard-stubs/einfo.pyi
+-rw-r--r--   0        0        0      475 2021-10-31 21:31:07.748173 celery-types-0.9.3/billiard-stubs/exceptions.pyi
+-rw-r--r--   0        0        0     1005 2021-10-31 21:31:07.748555 celery-types-0.9.3/celery-stubs/__init__.pyi
+-rw-r--r--   0        0        0      108 2021-10-31 21:31:07.748810 celery-types-0.9.3/celery-stubs/_state.pyi
+-rw-r--r--   0        0        0     2547 2021-10-31 21:31:07.749237 celery-types-0.9.3/celery-stubs/app/__init__.pyi
+-rw-r--r--   0        0        0       16 2021-10-31 21:31:07.749444 celery-types-0.9.3/celery-stubs/app/amqp.pyi
+-rw-r--r--   0        0        0    11982 2021-10-31 21:31:07.749850 celery-types-0.9.3/celery-stubs/app/base.pyi
+-rw-r--r--   0        0        0       16 2021-10-31 21:31:07.750150 celery-types-0.9.3/celery-stubs/app/beat.pyi
+-rw-r--r--   0        0        0     5875 2021-10-31 21:31:07.750447 celery-types-0.9.3/celery-stubs/app/control.pyi
+-rw-r--r--   0        0        0       18 2021-10-31 21:31:07.750709 celery-types-0.9.3/celery-stubs/app/events.pyi
+-rw-r--r--   0        0        0     1934 2021-10-31 21:31:07.750939 celery-types-0.9.3/celery-stubs/app/log.pyi
+-rw-r--r--   0        0        0       70 2021-10-31 21:31:07.751173 celery-types-0.9.3/celery-stubs/app/registry.pyi
+-rw-r--r--   0        0        0       18 2021-10-31 21:31:07.751399 celery-types-0.9.3/celery-stubs/app/routes.pyi
+-rw-r--r--   0        0        0     7292 2021-11-03 02:11:34.134094 celery-types-0.9.3/celery-stubs/app/task.pyi
+-rw-r--r--   0        0        0      118 2021-10-31 21:31:07.751907 celery-types-0.9.3/celery-stubs/app/utils.pyi
+-rw-r--r--   0        0        0        0 2021-10-31 21:31:07.752166 celery-types-0.9.3/celery-stubs/apps/__init__.pyi
+-rw-r--r--   0        0        0       76 2021-10-31 21:31:07.752416 celery-types-0.9.3/celery-stubs/apps/worker.pyi
+-rw-r--r--   0        0        0        0 2021-10-31 21:31:07.752696 celery-types-0.9.3/celery-stubs/backends/__init__.pyi
+-rw-r--r--   0        0        0       19 2021-10-31 21:31:07.752843 celery-types-0.9.3/celery-stubs/backends/base.pyi
+-rw-r--r--   0        0        0    12999 2021-11-06 20:16:22.272339 celery-types-0.9.3/celery-stubs/canvas.pyi
+-rw-r--r--   0        0        0        0 2021-10-31 21:31:07.753576 celery-types-0.9.3/celery-stubs/concurrency/__init__.pyi
+-rw-r--r--   0        0        0       20 2021-10-31 21:31:07.753848 celery-types-0.9.3/celery-stubs/concurrency/base.pyi
+-rw-r--r--   0        0        0     2789 2021-10-31 21:31:07.754112 celery-types-0.9.3/celery-stubs/exceptions.pyi
+-rw-r--r--   0        0        0        0 2021-10-31 21:31:07.754325 celery-types-0.9.3/celery-stubs/loaders/__init__.pyi
+-rw-r--r--   0        0        0      103 2021-10-31 21:31:07.754551 celery-types-0.9.3/celery-stubs/loaders/base.pyi
+-rw-r--r--   0        0        0        0 2021-10-31 21:31:07.754712 celery-types-0.9.3/celery-stubs/local.pyi
+-rw-r--r--   0        0        0     4050 2021-10-31 21:31:07.754985 celery-types-0.9.3/celery-stubs/result.pyi
+-rw-r--r--   0        0        0     2943 2021-11-28 15:56:35.647423 celery-types-0.9.3/celery-stubs/schedules.pyi
+-rw-r--r--   0        0        0     1502 2021-10-31 21:31:07.755466 celery-types-0.9.3/celery-stubs/signals.pyi
+-rw-r--r--   0        0        0     1148 2021-10-31 21:31:07.755712 celery-types-0.9.3/celery-stubs/states.pyi
+-rw-r--r--   0        0        0       42 2021-10-31 21:31:07.756055 celery-types-0.9.3/celery-stubs/utils/__init__.pyi
+-rw-r--r--   0        0        0      109 2021-10-31 21:31:07.756228 celery-types-0.9.3/celery-stubs/utils/abstract.pyi
+-rw-r--r--   0        0        0      325 2021-10-31 21:31:07.756388 celery-types-0.9.3/celery-stubs/utils/collections.pyi
+-rw-r--r--   0        0        0       58 2021-10-31 21:31:07.756647 celery-types-0.9.3/celery-stubs/utils/dispatch/__init__.pyi
+-rw-r--r--   0        0        0      344 2021-10-31 21:31:07.756840 celery-types-0.9.3/celery-stubs/utils/dispatch/signal.pyi
+-rw-r--r--   0        0        0       53 2021-10-31 21:31:07.757038 celery-types-0.9.3/celery-stubs/utils/graph.pyi
+-rw-r--r--   0        0        0      140 2021-10-31 21:31:07.757299 celery-types-0.9.3/celery-stubs/utils/log.pyi
+-rw-r--r--   0        0        0       27 2021-10-31 21:31:07.757616 celery-types-0.9.3/celery-stubs/utils/objects.pyi
+-rw-r--r--   0        0        0       19 2021-10-31 21:31:07.757930 celery-types-0.9.3/celery-stubs/utils/term.pyi
+-rw-r--r--   0        0        0       23 2021-10-31 21:31:07.758146 celery-types-0.9.3/celery-stubs/utils/threads.pyi
+-rw-r--r--   0        0        0       16 2021-10-31 21:31:07.758322 celery-types-0.9.3/celery-stubs/utils/time.pyi
+-rw-r--r--   0        0        0       66 2021-10-31 21:31:07.758611 celery-types-0.9.3/celery-stubs/worker/__init__.pyi
+-rw-r--r--   0        0        0     4511 2021-10-31 21:31:07.758836 celery-types-0.9.3/celery-stubs/worker/request.pyi
+-rw-r--r--   0        0        0       26 2021-10-31 21:31:07.759019 celery-types-0.9.3/celery-stubs/worker/worker.pyi
+-rw-r--r--   0        0        0        0 2021-10-31 21:31:07.759215 celery-types-0.9.3/django_celery_results-stubs/__init__.pyi
+-rw-r--r--   0        0        0      895 2021-10-31 21:31:07.759471 celery-types-0.9.3/django_celery_results-stubs/managers.pyi
+-rw-r--r--   0        0        0     1099 2021-10-31 21:31:07.759960 celery-types-0.9.3/django_celery_results-stubs/models.pyi
+-rw-r--r--   0        0        0       20 2021-10-31 21:31:07.760226 celery-types-0.9.3/ephem-stubs/__init__.pyi
+-rw-r--r--   0        0        0      290 2021-10-31 21:31:07.760426 celery-types-0.9.3/kombu-stubs/__init__.pyi
+-rw-r--r--   0        0        0       55 2021-10-31 21:31:07.760568 celery-types-0.9.3/kombu-stubs/abstract.pyi
+-rw-r--r--   0        0        0     1157 2021-10-31 21:31:07.760705 celery-types-0.9.3/kombu-stubs/connection.pyi
+-rw-r--r--   0        0        0      121 2021-10-31 21:31:07.760835 celery-types-0.9.3/kombu-stubs/entity.pyi
+-rw-r--r--   0        0        0      815 2021-10-31 21:31:07.760967 celery-types-0.9.3/kombu-stubs/exceptions.pyi
+-rw-r--r--   0        0        0     1271 2021-10-31 21:31:07.761189 celery-types-0.9.3/kombu-stubs/message.pyi
+-rw-r--r--   0        0        0       20 2021-10-31 21:31:07.761465 celery-types-0.9.3/kombu-stubs/messaging.pyi
+-rw-r--r--   0        0        0       35 2021-10-31 21:31:07.761627 celery-types-0.9.3/kombu-stubs/pidbox.pyi
+-rw-r--r--   0        0        0       71 2021-10-31 21:31:07.761789 celery-types-0.9.3/kombu-stubs/pools.pyi
+-rw-r--r--   0        0        0       20 2021-10-31 21:31:07.762091 celery-types-0.9.3/kombu-stubs/resource.pyi
+-rw-r--r--   0        0        0        0 2021-10-31 21:31:07.762441 celery-types-0.9.3/kombu-stubs/transport/__init__.pyi
+-rw-r--r--   0        0        0       21 2021-10-31 21:31:07.762715 celery-types-0.9.3/kombu-stubs/transport/base.pyi
+-rw-r--r--   0        0        0        0 2021-10-31 21:31:07.763074 celery-types-0.9.3/kombu-stubs/utils/__init__.pyi
+-rw-r--r--   0        0        0      105 2021-10-31 21:31:07.763491 celery-types-0.9.3/kombu-stubs/utils/uuid.pyi
+-rw-r--r--   0        0        0      989 2021-11-28 15:56:59.716967 celery-types-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0       68 2021-10-31 21:31:07.768488 celery-types-0.9.3/vine-stubs/__init__.pyi
+-rw-r--r--   0        0        0        0 2021-10-31 21:31:07.768686 celery-types-0.9.3/vine-stubs/abstract.pyi
+-rw-r--r--   0        0        0        0 2021-10-31 21:31:07.768840 celery-types-0.9.3/vine-stubs/funtools.pyi
+-rw-r--r--   0        0        0       19 2021-10-31 21:31:07.769081 celery-types-0.9.3/vine-stubs/promises.pyi
+-rw-r--r--   0        0        0        0 2021-10-31 21:31:07.769218 celery-types-0.9.3/vine-stubs/synchronization.pyi
+-rw-r--r--   0        0        0     1925 2021-11-28 15:57:10.839716 celery-types-0.9.3/setup.py
+-rw-r--r--   0        0        0     1578 2021-11-28 15:57:10.840169 celery-types-0.9.3/PKG-INFO
```

### Comparing `celery-types-0.9.2/LICENSE` & `celery-types-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `celery-types-0.9.2/README.md` & `celery-types-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `celery-types-0.9.2/celery-stubs/__init__.pyi` & `celery-types-0.9.3/celery-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `celery-types-0.9.2/celery-stubs/app/__init__.pyi` & `celery-types-0.9.3/celery-stubs/app/__init__.pyi`

 * *Files identical despite different names*

### Comparing `celery-types-0.9.2/celery-stubs/app/base.pyi` & `celery-types-0.9.3/celery-stubs/app/base.pyi`

 * *Files identical despite different names*

### Comparing `celery-types-0.9.2/celery-stubs/app/control.pyi` & `celery-types-0.9.3/celery-stubs/app/control.pyi`

 * *Files identical despite different names*

### Comparing `celery-types-0.9.2/celery-stubs/app/log.pyi` & `celery-types-0.9.3/celery-stubs/app/log.pyi`

 * *Files identical despite different names*

### Comparing `celery-types-0.9.2/celery-stubs/app/task.pyi` & `celery-types-0.9.3/celery-stubs/app/task.pyi`

 * *Files identical despite different names*

### Comparing `celery-types-0.9.2/celery-stubs/canvas.pyi` & `celery-types-0.9.3/celery-stubs/canvas.pyi`

 * *Files identical despite different names*

### Comparing `celery-types-0.9.2/celery-stubs/exceptions.pyi` & `celery-types-0.9.3/celery-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `celery-types-0.9.2/celery-stubs/result.pyi` & `celery-types-0.9.3/celery-stubs/result.pyi`

 * *Files identical despite different names*

### Comparing `celery-types-0.9.2/celery-stubs/schedules.pyi` & `celery-types-0.9.3/celery-stubs/schedules.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numbers
 from datetime import datetime, timedelta
-from typing import Callable, NamedTuple, Optional, Set, Tuple, Union
+from typing import Callable, List, NamedTuple, Optional, Set, Tuple, Union
 
 from celery.app.base import Celery
 from celery.utils.time import ffwd
 from typing_extensions import Literal
 
 import ephem
 
@@ -57,19 +57,19 @@
     ParseException: _ModuleLevelParseException
     def __init__(self, max_: int = ..., min_: int = ...) -> None: ...
     def parse(self, spec: str) -> Set[int]: ...
 
 class crontab(BaseSchedule):
     def __init__(
         self,
-        minute: Union[str, int] = ...,
-        hour: Union[str, int] = ...,
-        day_of_week: Union[str, int] = ...,
-        day_of_month: Union[str, int] = ...,
-        month_of_year: Union[str, int] = ...,
+        minute: Union[str, int, List[int]] = ...,
+        hour: Union[str, int, List[int]] = ...,
+        day_of_week: Union[str, int, List[int]] = ...,
+        day_of_month: Union[str, int, List[int]] = ...,
+        month_of_year: Union[str, int, List[int]] = ...,
         nowfun: Optional[Callable[[], datetime]] = ...,
         app: Optional[Celery] = ...,
     ) -> None: ...
     def remaining_delta(
         self, last_run_at: datetime, tz: Optional[str] = ..., ffwd: ffwd = ...
     ) -> Tuple[datetime, timedelta, datetime]: ...
```

### Comparing `celery-types-0.9.2/celery-stubs/signals.pyi` & `celery-types-0.9.3/celery-stubs/signals.pyi`

 * *Files identical despite different names*

### Comparing `celery-types-0.9.2/celery-stubs/states.pyi` & `celery-types-0.9.3/celery-stubs/states.pyi`

 * *Files identical despite different names*

### Comparing `celery-types-0.9.2/celery-stubs/worker/request.pyi` & `celery-types-0.9.3/celery-stubs/worker/request.pyi`

 * *Files identical despite different names*

### Comparing `celery-types-0.9.2/django_celery_results-stubs/managers.pyi` & `celery-types-0.9.3/django_celery_results-stubs/managers.pyi`

 * *Files identical despite different names*

### Comparing `celery-types-0.9.2/django_celery_results-stubs/models.pyi` & `celery-types-0.9.3/django_celery_results-stubs/models.pyi`

 * *Files identical despite different names*

### Comparing `celery-types-0.9.2/kombu-stubs/connection.pyi` & `celery-types-0.9.3/kombu-stubs/connection.pyi`

 * *Files identical despite different names*

### Comparing `celery-types-0.9.2/kombu-stubs/exceptions.pyi` & `celery-types-0.9.3/kombu-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `celery-types-0.9.2/kombu-stubs/message.pyi` & `celery-types-0.9.3/kombu-stubs/message.pyi`

 * *Files identical despite different names*

### Comparing `celery-types-0.9.2/pyproject.toml` & `celery-types-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "celery-types"
-version = "0.9.2"
+version = "0.9.3"
 description = "Type stubs for Celery and its related packages"
 repository = "https://github.com/sbdchd/celery-types"
 readme = "README.md"
 authors = ["Steve Dignam <steve@dignam.xyz>"]
 keywords = [
   "celery",
   "kombu",
```

### Comparing `celery-types-0.9.2/setup.py` & `celery-types-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                   'utils/*',
                   'utils/dispatch/*',
                   'worker/*'],
  'kombu-stubs': ['transport/*', 'utils/*']}
 
 setup_kwargs = {
     'name': 'celery-types',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'Type stubs for Celery and its related packages',
     'long_description': '# celery-types [![PyPI](https://img.shields.io/pypi/v/celery-types.svg)](https://pypi.org/project/celery-types/)\n\nType stubs for celery related projects:\n\n- [`celery`](https://github.com/celery/celery)\n- [`django-celery-results`](https://github.com/celery/django-celery-results)\n- [`amqp`](http://github.com/celery/py-amqp)\n- [`kombu`](https://github.com/celery/kombu)\n- [`billiard`](https://github.com/celery/billiard)\n- [`vine`](https://github.com/celery/vine)\n- [`ephem`](https://github.com/brandon-rhodes/pyephem)\n\n## install\n\n```shell\npip install celery-types\n```\n\n## dev\n\n```shell\npoetry install\n\n# run formatting, linting, and typechecking\ns/lint\n\n# build and publish\npoetry publish --build\n```\n\n## related\n\n- <https://github.com/sbdchd/django-types>\n- <https://github.com/sbdchd/djangorestframework-types>\n- <https://github.com/sbdchd/mongo-types>\n- <https://github.com/sbdchd/msgpack-types>\n',
     'author': 'Steve Dignam',
     'author_email': 'steve@dignam.xyz',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/sbdchd/celery-types',
```

### Comparing `celery-types-0.9.2/PKG-INFO` & `celery-types-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery-types
-Version: 0.9.2
+Version: 0.9.3
 Summary: Type stubs for Celery and its related packages
 Home-page: https://github.com/sbdchd/celery-types
 Keywords: celery,kombu,vine,amqp,billiard,django_celery_results,types,mypy,stubs
 Author: Steve Dignam
 Author-email: steve@dignam.xyz
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
```

