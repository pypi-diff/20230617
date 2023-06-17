# Comparing `tmp/numalogic_prometheus-0.4.8.tar.gz` & `tmp/numalogic_prometheus-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic_prometheus-0.4.8.tar", max compression
+gzip compressed data, was "numalogic_prometheus-0.4.9.tar", max compression
```

## Comparing `numalogic_prometheus-0.4.8.tar` & `numalogic_prometheus-0.4.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/LICENSE
--rw-r--r--   0        0        0     1894 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/__init__.py
--rw-r--r--   0        0        0     1400 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/_config.py
--rw-r--r--   0        0        0      561 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/_constants.py
--rw-r--r--   0        0        0        0 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/clients/__init__.py
--rw-r--r--   0        0        0     3832 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/clients/prometheus.py
--rw-r--r--   0        0        0     1260 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/clients/redis.py
--rw-r--r--   0        0        0     2488 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/clients/sentinel.py
--rw-r--r--   0        0        0     2145 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/configs/config.yaml
--rw-r--r--   0        0        0     1841 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/default-configs/config.yaml
--rw-r--r--   0        0        0      337 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/default-configs/numalogic_config.yaml
--rw-r--r--   0        0        0      382 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/default-configs/pipeline_config.yaml
--rw-r--r--   0        0        0     4503 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/entities.py
--rw-r--r--   0        0        0      950 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/factory.py
--rw-r--r--   0        0        0     7169 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/tools.py
--rw-r--r--   0        0        0      366 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/udf/__init__.py
--rw-r--r--   0        0        0      689 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/udf/filter.py
--rw-r--r--   0        0        0     4702 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/udf/inference.py
--rw-r--r--   0        0        0     7339 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/udf/postprocess.py
--rw-r--r--   0        0        0     3473 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/udf/preprocess.py
--rw-r--r--   0        0        0     4932 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/udf/threshold.py
--rw-r--r--   0        0        0     4184 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/udf/window.py
--rw-r--r--   0        0        0      134 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/udsink/__init__.py
--rw-r--r--   0        0        0     7399 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/udsink/train.py
--rw-r--r--   0        0        0     8541 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/udsink/train_rollout.py
--rw-r--r--   0        0        0     5979 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/watcher.py
--rw-r--r--   0        0        0     1661 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     1065 1970-01-01 00:00:00.000000 numalogic_prometheus-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-15 20:58:37.542413 numalogic_prometheus-0.4.9/LICENSE
+-rw-r--r--   0        0        0     1894 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/__init__.py
+-rw-r--r--   0        0        0     1400 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/_config.py
+-rw-r--r--   0        0        0      561 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/_constants.py
+-rw-r--r--   0        0        0        0 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/clients/__init__.py
+-rw-r--r--   0        0        0     3832 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/clients/prometheus.py
+-rw-r--r--   0        0        0     1260 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/clients/redis.py
+-rw-r--r--   0        0        0     2488 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/clients/sentinel.py
+-rw-r--r--   0        0        0     2145 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/configs/config.yaml
+-rw-r--r--   0        0        0     1841 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/default-configs/config.yaml
+-rw-r--r--   0        0        0      337 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/default-configs/numalogic_config.yaml
+-rw-r--r--   0        0        0      382 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/default-configs/pipeline_config.yaml
+-rw-r--r--   0        0        0     4503 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/entities.py
+-rw-r--r--   0        0        0      950 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/factory.py
+-rw-r--r--   0        0        0     7169 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/tools.py
+-rw-r--r--   0        0        0      366 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/udf/__init__.py
+-rw-r--r--   0        0        0      689 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/udf/filter.py
+-rw-r--r--   0        0        0     4702 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/udf/inference.py
+-rw-r--r--   0        0        0     7339 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/udf/postprocess.py
+-rw-r--r--   0        0        0     3473 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/udf/preprocess.py
+-rw-r--r--   0        0        0     4932 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/udf/threshold.py
+-rw-r--r--   0        0        0     4184 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/udf/window.py
+-rw-r--r--   0        0        0      134 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/udsink/__init__.py
+-rw-r--r--   0        0        0     7399 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/udsink/train.py
+-rw-r--r--   0        0        0     8540 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/udsink/train_rollout.py
+-rw-r--r--   0        0        0     5979 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/numaprom/watcher.py
+-rw-r--r--   0        0        0     1661 2023-06-15 20:58:37.546413 numalogic_prometheus-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     1065 1970-01-01 00:00:00.000000 numalogic_prometheus-0.4.9/PKG-INFO
```

### Comparing `numalogic_prometheus-0.4.8/LICENSE` & `numalogic_prometheus-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.8/numaprom/__init__.py` & `numalogic_prometheus-0.4.9/numaprom/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.8/numaprom/_config.py` & `numalogic_prometheus-0.4.9/numaprom/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.8/numaprom/_constants.py` & `numalogic_prometheus-0.4.9/numaprom/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.8/numaprom/clients/prometheus.py` & `numalogic_prometheus-0.4.9/numaprom/clients/prometheus.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.8/numaprom/clients/redis.py` & `numalogic_prometheus-0.4.9/numaprom/clients/redis.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.8/numaprom/clients/sentinel.py` & `numalogic_prometheus-0.4.9/numaprom/clients/sentinel.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.8/numaprom/configs/config.yaml` & `numalogic_prometheus-0.4.9/numaprom/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.8/numaprom/default-configs/config.yaml` & `numalogic_prometheus-0.4.9/numaprom/default-configs/config.yaml`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.8/numaprom/entities.py` & `numalogic_prometheus-0.4.9/numaprom/entities.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.8/numaprom/factory.py` & `numalogic_prometheus-0.4.9/numaprom/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.8/numaprom/tools.py` & `numalogic_prometheus-0.4.9/numaprom/tools.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.8/numaprom/udf/filter.py` & `numalogic_prometheus-0.4.9/numaprom/udf/filter.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.8/numaprom/udf/inference.py` & `numalogic_prometheus-0.4.9/numaprom/udf/inference.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.8/numaprom/udf/postprocess.py` & `numalogic_prometheus-0.4.9/numaprom/udf/postprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.8/numaprom/udf/preprocess.py` & `numalogic_prometheus-0.4.9/numaprom/udf/preprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.8/numaprom/udf/threshold.py` & `numalogic_prometheus-0.4.9/numaprom/udf/threshold.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.8/numaprom/udf/window.py` & `numalogic_prometheus-0.4.9/numaprom/udf/window.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.8/numaprom/udsink/train.py` & `numalogic_prometheus-0.4.9/numaprom/udsink/train.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.8/numaprom/udsink/train_rollout.py` & `numalogic_prometheus-0.4.9/numaprom/udsink/train_rollout.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     model = model_factory.get_instance(model_cfg)
     dataset = StreamingDataset(x, model.seq_len)
 
     trainer = AutoencoderTrainer(**trainer_cfg)
     trainer.fit(model, train_dataloaders=DataLoader(dataset, batch_size=64))
 
     LOGGER.debug(
-        "{uuid} - Time taken to train model: {time}} sec",
+        "{uuid} - Time taken to train model: {time} sec",
         uuid=uuid,
         time=time.perf_counter() - _start_train,
     )
 
     train_reconerr = trainer.predict(model, dataloaders=DataLoader(dataset, batch_size=64))
     # return the trainer to avoid Weakreference error
     return train_reconerr.numpy(), model, trainer
```

### Comparing `numalogic_prometheus-0.4.8/numaprom/watcher.py` & `numalogic_prometheus-0.4.9/numaprom/watcher.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.8/pyproject.toml` & `numalogic_prometheus-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic-prometheus"
-version = "0.4.8"
+version = "0.4.9"
 description = "ML inference on numaflow using numalogic on Prometheus metrics"
 authors = ["Numalogic developers"]
 packages = [{ include = "numaprom" }]
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
     "Nandita Koppisetty <nandita.iitkgp@gmail.com>",
 ]
```

### Comparing `numalogic_prometheus-0.4.8/PKG-INFO` & `numalogic_prometheus-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numalogic-prometheus
-Version: 0.4.8
+Version: 0.4.9
 Summary: ML inference on numaflow using numalogic on Prometheus metrics
 Home-page: https://github.com/numaproj/numalogic-prometheus
 Author: Numalogic developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Intended Audience :: Developers
```

