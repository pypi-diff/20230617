# Comparing `tmp/tajik_text_segmentation-0.1.5.tar.gz` & `tmp/tajik_text_segmentation-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tajik_text_segmentation-0.1.5.tar", last modified: Sat Jun 17 08:34:41 2023, max compression
+gzip compressed data, was "tajik_text_segmentation-0.1.6.tar", last modified: Sat Jun 17 09:06:20 2023, max compression
```

## Comparing `tajik_text_segmentation-0.1.5.tar` & `tajik_text_segmentation-0.1.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 08:34:41.863035 tajik_text_segmentation-0.1.5/
--rw-rw-rw-   0        0        0       38 2023-06-16 20:52:08.000000 tajik_text_segmentation-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6366 2023-06-17 08:34:41.859032 tajik_text_segmentation-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     5611 2023-06-16 20:23:43.000000 tajik_text_segmentation-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-17 08:34:41.863035 tajik_text_segmentation-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1204 2023-06-17 08:33:09.000000 tajik_text_segmentation-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 08:34:41.731562 tajik_text_segmentation-0.1.5/tajik_text_segmentation/
--rw-rw-rw-   0        0        0       43 2023-06-16 19:33:51.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/__init__.py
--rw-rw-rw-   0        0        0     8336 2023-06-16 19:30:58.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/annotated.py
--rw-rw-rw-   0        0        0     7003 2023-06-17 08:30:57.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/boundary_resolver.py
-drwxrwxrwx   0        0        0        0 2023-06-17 08:34:41.810335 tajik_text_segmentation-0.1.5/tajik_text_segmentation/checkpoints/
--rw-rw-rw-   0        0        0   105452 2023-06-15 21:04:02.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/checkpoints/checkpoint.pt
--rw-rw-rw-   0        0        0      557 2023-06-17 08:28:26.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/config.json
--rw-rw-rw-   0        0        0     5936 2023-06-16 19:28:56.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/heuristic_model.py
-drwxrwxrwx   0        0        0        0 2023-06-17 08:34:41.821538 tajik_text_segmentation-0.1.5/tajik_text_segmentation/nn_model/
--rw-rw-rw-   0        0        0        0 2023-06-16 20:37:57.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/nn_model/__init__.py
--rw-rw-rw-   0        0        0     8125 2023-06-17 08:26:48.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/nn_model/model.py
--rw-rw-rw-   0        0        0     6834 2023-06-16 19:29:28.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/nn_model/vocab.py
--rw-rw-rw-   0        0        0     3588 2023-06-17 08:22:16.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/text_segmenter.py
--rw-rw-rw-   0        0        0      551 2023-06-16 19:18:47.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation/tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-06-17 08:34:41.805336 tajik_text_segmentation-0.1.5/tajik_text_segmentation.egg-info/
--rw-rw-rw-   0        0        0     6366 2023-06-17 08:34:41.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      881 2023-06-17 08:34:41.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 08:34:41.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-06-17 08:34:41.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-17 08:34:41.000000 tajik_text_segmentation-0.1.5/tajik_text_segmentation.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-17 08:34:41.842033 tajik_text_segmentation-0.1.5/tests/
--rw-rw-rw-   0        0        0     1350 2023-06-16 20:26:44.000000 tajik_text_segmentation-0.1.5/tests/test_dataset.py
--rw-rw-rw-   0        0        0     1489 2023-06-16 20:30:33.000000 tajik_text_segmentation-0.1.5/tests/test_evaluate.py
--rw-rw-rw-   0        0        0     4071 2023-06-16 19:38:17.000000 tajik_text_segmentation-0.1.5/tests/test_heuristic_model.py
--rw-rw-rw-   0        0        0     1939 2023-06-16 19:38:23.000000 tajik_text_segmentation-0.1.5/tests/test_tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-06-17 08:34:41.854035 tajik_text_segmentation-0.1.5/training/
--rw-rw-rw-   0        0        0      450 2023-06-16 20:30:59.000000 tajik_text_segmentation-0.1.5/training/dummy_model.py
--rw-rw-rw-   0        0        0     4903 2023-06-17 08:29:26.000000 tajik_text_segmentation-0.1.5/training/evaluate.py
--rw-rw-rw-   0        0        0      498 2023-06-16 19:18:47.000000 tajik_text_segmentation-0.1.5/training/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-17 09:06:20.009430 tajik_text_segmentation-0.1.6/
+-rw-rw-rw-   0        0        0       38 2023-06-16 20:52:08.000000 tajik_text_segmentation-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     6366 2023-06-17 09:06:20.004711 tajik_text_segmentation-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5611 2023-06-16 20:23:43.000000 tajik_text_segmentation-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-17 09:06:20.009430 tajik_text_segmentation-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1204 2023-06-17 09:04:59.000000 tajik_text_segmentation-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 09:06:19.909957 tajik_text_segmentation-0.1.6/tajik_text_segmentation/
+-rw-rw-rw-   0        0        0       43 2023-06-16 19:33:51.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/__init__.py
+-rw-rw-rw-   0        0        0     8336 2023-06-16 19:30:58.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/annotated.py
+-rw-rw-rw-   0        0        0     7106 2023-06-17 09:05:32.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/boundary_resolver.py
+drwxrwxrwx   0        0        0        0 2023-06-17 09:06:19.970491 tajik_text_segmentation-0.1.6/tajik_text_segmentation/checkpoints/
+-rw-rw-rw-   0        0        0   105452 2023-06-15 21:04:02.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/checkpoints/checkpoint.pt
+-rw-rw-rw-   0        0        0      557 2023-06-17 08:28:26.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/config.json
+-rw-rw-rw-   0        0        0     5936 2023-06-16 19:28:56.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/heuristic_model.py
+drwxrwxrwx   0        0        0        0 2023-06-17 09:06:19.978757 tajik_text_segmentation-0.1.6/tajik_text_segmentation/nn_model/
+-rw-rw-rw-   0        0        0        0 2023-06-16 20:37:57.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/nn_model/__init__.py
+-rw-rw-rw-   0        0        0     8125 2023-06-17 08:26:48.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/nn_model/model.py
+-rw-rw-rw-   0        0        0     6834 2023-06-16 19:29:28.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/nn_model/vocab.py
+-rw-rw-rw-   0        0        0     3588 2023-06-17 08:22:16.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/text_segmenter.py
+-rw-rw-rw-   0        0        0      551 2023-06-16 19:18:47.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-06-17 09:06:19.967970 tajik_text_segmentation-0.1.6/tajik_text_segmentation.egg-info/
+-rw-rw-rw-   0        0        0     6366 2023-06-17 09:06:19.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      881 2023-06-17 09:06:19.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 09:06:19.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-06-17 09:06:19.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-17 09:06:19.000000 tajik_text_segmentation-0.1.6/tajik_text_segmentation.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 09:06:19.992978 tajik_text_segmentation-0.1.6/tests/
+-rw-rw-rw-   0        0        0     1350 2023-06-16 20:26:44.000000 tajik_text_segmentation-0.1.6/tests/test_dataset.py
+-rw-rw-rw-   0        0        0     1489 2023-06-16 20:30:33.000000 tajik_text_segmentation-0.1.6/tests/test_evaluate.py
+-rw-rw-rw-   0        0        0     4071 2023-06-16 19:38:17.000000 tajik_text_segmentation-0.1.6/tests/test_heuristic_model.py
+-rw-rw-rw-   0        0        0     1939 2023-06-16 19:38:23.000000 tajik_text_segmentation-0.1.6/tests/test_tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-06-17 09:06:19.999528 tajik_text_segmentation-0.1.6/training/
+-rw-rw-rw-   0        0        0      450 2023-06-16 20:30:59.000000 tajik_text_segmentation-0.1.6/training/dummy_model.py
+-rw-rw-rw-   0        0        0     4903 2023-06-17 08:29:26.000000 tajik_text_segmentation-0.1.6/training/evaluate.py
+-rw-rw-rw-   0        0        0      498 2023-06-16 19:18:47.000000 tajik_text_segmentation-0.1.6/training/utils.py
```

### Comparing `tajik_text_segmentation-0.1.5/PKG-INFO` & `tajik_text_segmentation-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tajik_text_segmentation
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for Tajik text segmentation using a heuristic algorithm and neural network.
 Home-page: https://github.com/sobir-git/tajik-text-segmentation
 Author: Sobir Bobiev
 Author-email: sobir.bobiev@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tajik_text_segmentation-0.1.5/README.md` & `tajik_text_segmentation-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.5/setup.py` & `tajik_text_segmentation-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="tajik_text_segmentation",
-    version="0.1.5",
+    version="0.1.6",
     author="Sobir Bobiev",
     author_email="sobir.bobiev@gmail.com",
     description="A package for Tajik text segmentation using a heuristic algorithm and neural network.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sobir-git/tajik-text-segmentation",
     packages=find_packages(exclude=['training', 'tests']),
```

### Comparing `tajik_text_segmentation-0.1.5/tajik_text_segmentation/annotated.py` & `tajik_text_segmentation-0.1.6/tajik_text_segmentation/annotated.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.5/tajik_text_segmentation/boundary_resolver.py` & `tajik_text_segmentation-0.1.6/tajik_text_segmentation/boundary_resolver.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,18 +50,19 @@
         # The algorithm tries to maximize the segmentation likelyhood defined as the sum of log probabilities
         # of individual choices (is_start, not_is_start, is_end, not_is_end) made at each token.
         # Note that not all segmentations are valid, thus simply selecting the choice with the highest
         # log probability is not sufficient.
 
         max_gap = self.max_gap
 
+        probs = np.concatenate([probs, [[1,1]]])  # dummy token that is supposed to be a sentence in itself
 
         # log probability
         logp = np.log(probs).tolist()
-        
+
         # log complementary probability
         logcomp = np.log(1-probs).tolist()
 
         # cumulative log complementary probabilities used for calculating sum in token ranges
         cumul = np.cumsum(logcomp, axis=1).sum(axis=1).tolist()
 
         assert len(cumul) == len(logcomp), (len(cumul), len(logcomp))
@@ -120,26 +121,25 @@
             dp[i][1] = cumul[i] + best_v + logp[i][1] - logcomp[i][1]
             prev[i][1] = best_k
         
         return self.backtrack(prev, binarize_output)
 
     def backtrack(self, prev, binarize_output):
         # backtrack to return sentence boundaries
+        i = prev[len(prev)-1][0]  # that dummy sentence start
         if binarize_output:
-            bounds = [[0,0] for _ in range(len(prev))]
-            i = len(prev) - 1
+            bounds = [[0,0] for _ in range(len(prev)-1)]
             while i is not None:
                 bounds[i][1] = 1
                 j = prev[i][1]
                 bounds[j][0] = 1
                 i = prev[j][0]
             return np.array(bounds)
         else:
             spans = []
-            i = len(prev) - 1
             while i is not None:
                 j = prev[i][1]
                 spans.append((j,i+1))
                 i = prev[j][0]
 
             return spans[::-1]
 
@@ -153,15 +153,15 @@
     row0 = [1] + x
     row1 = row0[1:] + [1]
     x = np.array([row0, row1], dtype=np.float64).T  # (N, 2)
     print(x)
 
     # print original boundaries
     # add some noise to binary probabilities
-    noise = np.clip(np.abs(np.random.normal(0, 0.25, size=x.shape)), 0.01, 0.99)
+    noise = np.clip(np.abs(np.random.normal(0, 0.1, size=x.shape)), 0.01, 0.99)
     noisy_x = np.copy(x)
     noisy_x[x==0] += noise[x==0]
     noisy_x[x==1] -= noise[x==1]
 
     # print noisy boundaries (probabilities)
     print(np.round(noisy_x, 2))
```

### Comparing `tajik_text_segmentation-0.1.5/tajik_text_segmentation/checkpoints/checkpoint.pt` & `tajik_text_segmentation-0.1.6/tajik_text_segmentation/checkpoints/checkpoint.pt`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.5/tajik_text_segmentation/config.json` & `tajik_text_segmentation-0.1.6/tajik_text_segmentation/config.json`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.5/tajik_text_segmentation/heuristic_model.py` & `tajik_text_segmentation-0.1.6/tajik_text_segmentation/heuristic_model.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.5/tajik_text_segmentation/nn_model/model.py` & `tajik_text_segmentation-0.1.6/tajik_text_segmentation/nn_model/model.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.5/tajik_text_segmentation/nn_model/vocab.py` & `tajik_text_segmentation-0.1.6/tajik_text_segmentation/nn_model/vocab.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.5/tajik_text_segmentation/text_segmenter.py` & `tajik_text_segmentation-0.1.6/tajik_text_segmentation/text_segmenter.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.5/tajik_text_segmentation/tokenizer.py` & `tajik_text_segmentation-0.1.6/tajik_text_segmentation/tokenizer.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.5/tajik_text_segmentation.egg-info/PKG-INFO` & `tajik_text_segmentation-0.1.6/tajik_text_segmentation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tajik-text-segmentation
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for Tajik text segmentation using a heuristic algorithm and neural network.
 Home-page: https://github.com/sobir-git/tajik-text-segmentation
 Author: Sobir Bobiev
 Author-email: sobir.bobiev@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tajik_text_segmentation-0.1.5/tajik_text_segmentation.egg-info/SOURCES.txt` & `tajik_text_segmentation-0.1.6/tajik_text_segmentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.5/tests/test_dataset.py` & `tajik_text_segmentation-0.1.6/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.5/tests/test_evaluate.py` & `tajik_text_segmentation-0.1.6/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.5/tests/test_heuristic_model.py` & `tajik_text_segmentation-0.1.6/tests/test_heuristic_model.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.5/tests/test_tokenizer.py` & `tajik_text_segmentation-0.1.6/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `tajik_text_segmentation-0.1.5/training/evaluate.py` & `tajik_text_segmentation-0.1.6/training/evaluate.py`

 * *Files identical despite different names*

