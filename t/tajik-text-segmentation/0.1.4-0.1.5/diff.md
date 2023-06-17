# Comparing `tmp/tajik_text_segmentation-0.1.4.tar.gz` & `tmp/tajik_text_segmentation-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tajik_text_segmentation-0.1.4.tar", last modified: Fri Jun 16 21:50:40 2023, max compression
+gzip compressed data, was "tajik_text_segmentation-0.1.5.tar", last modified: Sat Jun 17 08:34:41 2023, max compression
```

## Comparing `tajik_text_segmentation-0.1.4.tar` & `tajik_text_segmentation-0.1.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 21:50:40.548758 tajik_text_segmentation-0.1.4/
--rw-rw-rw-   0        0        0       38 2023-06-16 20:52:08.000000 tajik_text_segmentation-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6366 2023-06-16 21:50:40.547466 tajik_text_segmentation-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     5611 2023-06-16 20:23:43.000000 tajik_text_segmentation-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 21:50:40.548758 tajik_text_segmentation-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1204 2023-06-16 21:33:05.000000 tajik_text_segmentation-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 21:50:40.480033 tajik_text_segmentation-0.1.4/tajik_text_segmentation/
--rw-rw-rw-   0        0        0       43 2023-06-16 19:33:51.000000 tajik_text_segmentation-0.1.4/tajik_text_segmentation/__init__.py
--rw-rw-rw-   0        0        0     8336 2023-06-16 19:30:58.000000 tajik_text_segmentation-0.1.4/tajik_text_segmentation/annotated.py
--rw-rw-rw-   0        0        0     4675 2023-06-16 19:18:47.000000 tajik_text_segmentation-0.1.4/tajik_text_segmentation/boundary_resolver.py
-drwxrwxrwx   0        0        0        0 2023-06-16 21:50:40.528244 tajik_text_segmentation-0.1.4/tajik_text_segmentation/checkpoints/
--rw-rw-rw-   0        0        0   105452 2023-06-15 21:04:02.000000 tajik_text_segmentation-0.1.4/tajik_text_segmentation/checkpoints/checkpoint.pt
--rw-rw-rw-   0        0        0      495 2023-06-16 19:30:21.000000 tajik_text_segmentation-0.1.4/tajik_text_segmentation/config.json
--rw-rw-rw-   0        0        0     5936 2023-06-16 19:28:56.000000 tajik_text_segmentation-0.1.4/tajik_text_segmentation/heuristic_model.py
-drwxrwxrwx   0        0        0        0 2023-06-16 21:50:40.532984 tajik_text_segmentation-0.1.4/tajik_text_segmentation/nn_model/
--rw-rw-rw-   0        0        0        0 2023-06-16 20:37:57.000000 tajik_text_segmentation-0.1.4/tajik_text_segmentation/nn_model/__init__.py
--rw-rw-rw-   0        0        0     8121 2023-06-16 21:05:06.000000 tajik_text_segmentation-0.1.4/tajik_text_segmentation/nn_model/model.py
--rw-rw-rw-   0        0        0     6834 2023-06-16 19:29:28.000000 tajik_text_segmentation-0.1.4/tajik_text_segmentation/nn_model/vocab.py
--rw-rw-rw-   0        0        0     3588 2023-06-16 20:59:36.000000 tajik_text_segmentation-0.1.4/tajik_text_segmentation/text_segmenter.py
--rw-rw-rw-   0        0        0      551 2023-06-16 19:18:47.000000 tajik_text_segmentation-0.1.4/tajik_text_segmentation/tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-06-16 21:50:40.527244 tajik_text_segmentation-0.1.4/tajik_text_segmentation.egg-info/
--rw-rw-rw-   0        0        0     6366 2023-06-16 21:50:40.000000 tajik_text_segmentation-0.1.4/tajik_text_segmentation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      881 2023-06-16 21:50:40.000000 tajik_text_segmentation-0.1.4/tajik_text_segmentation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 21:50:40.000000 tajik_text_segmentation-0.1.4/tajik_text_segmentation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-06-16 21:50:40.000000 tajik_text_segmentation-0.1.4/tajik_text_segmentation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-16 21:50:40.000000 tajik_text_segmentation-0.1.4/tajik_text_segmentation.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-16 21:50:40.540215 tajik_text_segmentation-0.1.4/tests/
--rw-rw-rw-   0        0        0     1350 2023-06-16 20:26:44.000000 tajik_text_segmentation-0.1.4/tests/test_dataset.py
--rw-rw-rw-   0        0        0     1489 2023-06-16 20:30:33.000000 tajik_text_segmentation-0.1.4/tests/test_evaluate.py
--rw-rw-rw-   0        0        0     4071 2023-06-16 19:38:17.000000 tajik_text_segmentation-0.1.4/tests/test_heuristic_model.py
--rw-rw-rw-   0        0        0     1939 2023-06-16 19:38:23.000000 tajik_text_segmentation-0.1.4/tests/test_tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-06-16 21:50:40.546579 tajik_text_segmentation-0.1.4/training/
--rw-rw-rw-   0        0        0      450 2023-06-16 20:30:59.000000 tajik_text_segmentation-0.1.4/training/dummy_model.py
--rw-rw-rw-   0        0        0     4903 2023-06-16 19:27:26.000000 tajik_text_segmentation-0.1.4/training/evaluate.py
--rw-rw-rw-   0        0        0      498 2023-06-16 19:18:47.000000 tajik_text_segmentation-0.1.4/training/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-17 08:34:41.863035 tajik_text_segmentation-0.1.5/
+-rw-rw-rw-   0        0        0       38 2023-06-16 20:52:08.000000 tajik_text_segmentation-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     6366 2023-06-17 08:34:41.859032 tajik_text_segmentation-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5611 2023-06-16 20:23:43.000000 tajik_text_segmentation-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-17 08:34:41.863035 tajik_text_segmentation-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1204 2023-06-17 08:33:09.000000 tajik_text_segmentation-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 08:34:41.731562 tajik_text_segmentation-0.1.5/tajik_text_segmentation/
+-rw-rw-rw-   0        0        0       43 2023-06-16 19:33:51.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/__init__.py
+-rw-rw-rw-   0        0        0     8336 2023-06-16 19:30:58.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/annotated.py
+-rw-rw-rw-   0        0        0     7003 2023-06-17 08:30:57.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/boundary_resolver.py
+drwxrwxrwx   0        0        0        0 2023-06-17 08:34:41.810335 tajik_text_segmentation-0.1.5/tajik_text_segmentation/checkpoints/
+-rw-rw-rw-   0        0        0   105452 2023-06-15 21:04:02.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/checkpoints/checkpoint.pt
+-rw-rw-rw-   0        0        0      557 2023-06-17 08:28:26.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/config.json
+-rw-rw-rw-   0        0        0     5936 2023-06-16 19:28:56.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/heuristic_model.py
+drwxrwxrwx   0        0        0        0 2023-06-17 08:34:41.821538 tajik_text_segmentation-0.1.5/tajik_text_segmentation/nn_model/
+-rw-rw-rw-   0        0        0        0 2023-06-16 20:37:57.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/nn_model/__init__.py
+-rw-rw-rw-   0        0        0     8125 2023-06-17 08:26:48.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/nn_model/model.py
+-rw-rw-rw-   0        0        0     6834 2023-06-16 19:29:28.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/nn_model/vocab.py
+-rw-rw-rw-   0        0        0     3588 2023-06-17 08:22:16.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/text_segmenter.py
+-rw-rw-rw-   0        0        0      551 2023-06-16 19:18:47.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-06-17 08:34:41.805336 tajik_text_segmentation-0.1.5/tajik_text_segmentation.egg-info/
+-rw-rw-rw-   0        0        0     6366 2023-06-17 08:34:41.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      881 2023-06-17 08:34:41.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 08:34:41.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-06-17 08:34:41.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-17 08:34:41.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 08:34:41.842033 tajik_text_segmentation-0.1.5/tests/
+-rw-rw-rw-   0        0        0     1350 2023-06-16 20:26:44.000000 tajik_text_segmentation-0.1.5/tests/test_dataset.py
+-rw-rw-rw-   0        0        0     1489 2023-06-16 20:30:33.000000 tajik_text_segmentation-0.1.5/tests/test_evaluate.py
+-rw-rw-rw-   0        0        0     4071 2023-06-16 19:38:17.000000 tajik_text_segmentation-0.1.5/tests/test_heuristic_model.py
+-rw-rw-rw-   0        0        0     1939 2023-06-16 19:38:23.000000 tajik_text_segmentation-0.1.5/tests/test_tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-06-17 08:34:41.854035 tajik_text_segmentation-0.1.5/training/
+-rw-rw-rw-   0        0        0      450 2023-06-16 20:30:59.000000 tajik_text_segmentation-0.1.5/training/dummy_model.py
+-rw-rw-rw-   0        0        0     4903 2023-06-17 08:29:26.000000 tajik_text_segmentation-0.1.5/training/evaluate.py
+-rw-rw-rw-   0        0        0      498 2023-06-16 19:18:47.000000 tajik_text_segmentation-0.1.5/training/utils.py
```

### Comparing `tajik_text_segmentation-0.1.4/PKG-INFO` & `tajik_text_segmentation-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tajik_text_segmentation
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package for Tajik text segmentation using a heuristic algorithm and neural network.
 Home-page: https://github.com/sobir-git/tajik-text-segmentation
 Author: Sobir Bobiev
 Author-email: sobir.bobiev@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tajik_text_segmentation-0.1.4/README.md` & `tajik_text_segmentation-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.4/setup.py` & `tajik_text_segmentation-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="tajik_text_segmentation",
-    version="0.1.4",
+    version="0.1.5",
     author="Sobir Bobiev",
     author_email="sobir.bobiev@gmail.com",
     description="A package for Tajik text segmentation using a heuristic algorithm and neural network.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sobir-git/tajik-text-segmentation",
     packages=find_packages(exclude=['training', 'tests']),
```

### Comparing `tajik_text_segmentation-0.1.4/tajik_text_segmentation/annotated.py` & `tajik_text_segmentation-0.1.5/tajik_text_segmentation/annotated.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.4/tajik_text_segmentation/checkpoints/checkpoint.pt` & `tajik_text_segmentation-0.1.5/tajik_text_segmentation/checkpoints/checkpoint.pt`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.4/tajik_text_segmentation/heuristic_model.py` & `tajik_text_segmentation-0.1.5/tajik_text_segmentation/heuristic_model.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.4/tajik_text_segmentation/nn_model/model.py` & `tajik_text_segmentation-0.1.5/tajik_text_segmentation/nn_model/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             'model': self.model.state_dict(),
             'vocab': self.vocab.state_dict(),
             'metrics': self.metrics
         }, self.path)
 
     def load(self, device='cpu'):
         checkpoint = torch.load(self.path, map_location=device)
-        print(f"Loaded checkpoint: {self.path}; metrics: {checkpoint['metrics']}")
+        # print(f"Loaded checkpoint: {self.path}; metrics: {checkpoint['metrics']}")
         self.config = checkpoint['config']
         self.metrics = checkpoint['metrics']
         self.model.load_state_dict(checkpoint['model'])
         self.vocab.load_state_dict(checkpoint['vocab'])
 
     @classmethod
     def init_from_path(cls, path, device='cpu'):
@@ -43,15 +43,15 @@
         resource_path = f'checkpoints/checkpoint.pt'  # Relative path to the checkpoint file within your package
         
         # Getting the absolute path to the checkpoint file
         abs_path = pkg_resources.resource_filename(resource_package, resource_path)
         
         # Load the checkpoint
         checkpoint = torch.load(abs_path, map_location=device)
-        print(f"Loaded checkpoint: {path}; metrics: {checkpoint['metrics']}")
+        # print(f"Loaded checkpoint: {path}; metrics: {checkpoint['metrics']}")
         
         config = checkpoint['config']
 
         # init model and vocab
         model = SentenceBoundaryModel(config)
         vocab = Vocabulary()
```

### Comparing `tajik_text_segmentation-0.1.4/tajik_text_segmentation/nn_model/vocab.py` & `tajik_text_segmentation-0.1.5/tajik_text_segmentation/nn_model/vocab.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.4/tajik_text_segmentation/text_segmenter.py` & `tajik_text_segmentation-0.1.5/tajik_text_segmentation/text_segmenter.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.4/tajik_text_segmentation/tokenizer.py` & `tajik_text_segmentation-0.1.5/tajik_text_segmentation/tokenizer.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.4/tajik_text_segmentation.egg-info/PKG-INFO` & `tajik_text_segmentation-0.1.5/tajik_text_segmentation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tajik-text-segmentation
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package for Tajik text segmentation using a heuristic algorithm and neural network.
 Home-page: https://github.com/sobir-git/tajik-text-segmentation
 Author: Sobir Bobiev
 Author-email: sobir.bobiev@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tajik_text_segmentation-0.1.4/tajik_text_segmentation.egg-info/SOURCES.txt` & `tajik_text_segmentation-0.1.5/tajik_text_segmentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.4/tests/test_dataset.py` & `tajik_text_segmentation-0.1.5/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.4/tests/test_evaluate.py` & `tajik_text_segmentation-0.1.5/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.4/tests/test_heuristic_model.py` & `tajik_text_segmentation-0.1.5/tests/test_heuristic_model.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.4/tests/test_tokenizer.py` & `tajik_text_segmentation-0.1.5/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.4/training/evaluate.py` & `tajik_text_segmentation-0.1.5/training/evaluate.py`

 * *Files identical despite different names*

