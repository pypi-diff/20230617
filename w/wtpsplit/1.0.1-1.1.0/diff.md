# Comparing `tmp/wtpsplit-1.0.1.tar.gz` & `tmp/wtpsplit-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/benjamin_cohere_com/nnsplit/dist/.tmp-lfgwvf1a/wtpsplit-1.0.1.tar", last modified: Wed May 31 11:17:38 2023, max compression
+gzip compressed data, was "wtpsplit-1.1.0.tar", last modified: Sat Jun 17 09:54:08 2023, max compression
```

## Comparing `wtpsplit-1.0.1.tar` & `wtpsplit-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-05-31 11:17:38.847082 wtpsplit-1.0.1/
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      246 2023-05-31 11:17:38.847082 wtpsplit-1.0.1/PKG-INFO
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    10223 2023-05-31 11:16:52.000000 wtpsplit-1.0.1/README.md
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)       73 2023-05-31 11:16:52.000000 wtpsplit-1.0.1/pyproject.toml
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)       97 2023-05-31 11:17:38.847082 wtpsplit-1.0.1/setup.cfg
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      494 2023-05-31 11:17:06.000000 wtpsplit-1.0.1/setup.py
-drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-05-31 11:17:38.843082 wtpsplit-1.0.1/wtpsplit/
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    13654 2023-05-31 11:16:57.000000 wtpsplit-1.0.1/wtpsplit/__init__.py
-drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-05-31 11:17:38.847082 wtpsplit-1.0.1/wtpsplit/data/
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     3434 2023-05-31 11:16:52.000000 wtpsplit-1.0.1/wtpsplit/data/language_info.csv
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    38208 2023-05-31 11:16:52.000000 wtpsplit-1.0.1/wtpsplit/data/punctuation.json
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      408 2023-05-31 11:16:52.000000 wtpsplit-1.0.1/wtpsplit/data/punctuation.txt
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     7560 2023-05-31 11:16:52.000000 wtpsplit-1.0.1/wtpsplit/extract.py
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    40289 2023-05-31 11:16:52.000000 wtpsplit-1.0.1/wtpsplit/models.py
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     5814 2023-05-31 11:16:52.000000 wtpsplit-1.0.1/wtpsplit/utils.py
-drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-05-31 11:17:38.843082 wtpsplit-1.0.1/wtpsplit.egg-info/
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      246 2023-05-31 11:17:38.000000 wtpsplit-1.0.1/wtpsplit.egg-info/PKG-INFO
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      373 2023-05-31 11:17:38.000000 wtpsplit-1.0.1/wtpsplit.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        1 2023-05-31 11:17:38.000000 wtpsplit-1.0.1/wtpsplit.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)       49 2023-05-31 11:17:38.000000 wtpsplit-1.0.1/wtpsplit.egg-info/requires.txt
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        9 2023-05-31 11:17:38.000000 wtpsplit-1.0.1/wtpsplit.egg-info/top_level.txt
+drwxrwxr-x   0 bminixhofer  (1000) bminixhofer  (1000)        0 2023-06-17 09:54:08.886826 wtpsplit-1.1.0/
+-rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)     1076 2023-06-17 09:16:50.000000 wtpsplit-1.1.0/LICENSE
+-rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)      268 2023-06-17 09:54:08.886826 wtpsplit-1.1.0/PKG-INFO
+-rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)    11432 2023-06-17 09:52:02.000000 wtpsplit-1.1.0/README.md
+-rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)       73 2023-06-17 09:16:50.000000 wtpsplit-1.1.0/pyproject.toml
+-rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)       97 2023-06-17 09:54:08.886826 wtpsplit-1.1.0/setup.cfg
+-rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)      494 2023-06-17 09:53:23.000000 wtpsplit-1.1.0/setup.py
+drwxrwxr-x   0 bminixhofer  (1000) bminixhofer  (1000)        0 2023-06-17 09:54:08.886826 wtpsplit-1.1.0/wtpsplit/
+-rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)    14249 2023-06-17 09:52:37.000000 wtpsplit-1.1.0/wtpsplit/__init__.py
+drwxrwxr-x   0 bminixhofer  (1000) bminixhofer  (1000)        0 2023-06-17 09:54:08.886826 wtpsplit-1.1.0/wtpsplit/data/
+-rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)     3434 2023-06-17 09:16:50.000000 wtpsplit-1.1.0/wtpsplit/data/language_info.csv
+-rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)    38208 2023-06-17 09:16:50.000000 wtpsplit-1.1.0/wtpsplit/data/punctuation.json
+-rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)      408 2023-06-17 09:16:50.000000 wtpsplit-1.1.0/wtpsplit/data/punctuation.txt
+-rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)     7560 2023-06-17 09:16:50.000000 wtpsplit-1.1.0/wtpsplit/extract.py
+-rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)    40289 2023-06-17 09:16:50.000000 wtpsplit-1.1.0/wtpsplit/models.py
+-rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)     5814 2023-06-17 09:16:50.000000 wtpsplit-1.1.0/wtpsplit/utils.py
+drwxrwxr-x   0 bminixhofer  (1000) bminixhofer  (1000)        0 2023-06-17 09:54:08.886826 wtpsplit-1.1.0/wtpsplit.egg-info/
+-rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)      268 2023-06-17 09:54:08.000000 wtpsplit-1.1.0/wtpsplit.egg-info/PKG-INFO
+-rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)      381 2023-06-17 09:54:08.000000 wtpsplit-1.1.0/wtpsplit.egg-info/SOURCES.txt
+-rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)        1 2023-06-17 09:54:08.000000 wtpsplit-1.1.0/wtpsplit.egg-info/dependency_links.txt
+-rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)       49 2023-06-17 09:54:08.000000 wtpsplit-1.1.0/wtpsplit.egg-info/requires.txt
+-rw-rw-r--   0 bminixhofer  (1000) bminixhofer  (1000)        9 2023-06-17 09:54:08.000000 wtpsplit-1.1.0/wtpsplit.egg-info/top_level.txt
```

### Comparing `wtpsplit-1.0.1/README.md` & `wtpsplit-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # wtpsplit🪓
 
-Code for the paper [Where's the Point? Self-Supervised Multilingual Punctuation-Agnostic Sentence Segmentation](https://arxiv.org/abs/2305.18893) accepted at ACL 2023.
+Code for the paper [Where's the Point? Self-Supervised Multilingual Punctuation-Agnostic Sentence Segmentation](https://arxiv.org/abs/2305.18893) with Jonas Pfeiffer and Ivan Vulić, accepted at ACL 2023.
 
 This repository contains `wtpsplit`, a package for robust and adaptible sentence segmentation across 85 languages, as well as the code and configs to reproduce the experiments in the paper.
 
 ## Installation
 
 ```bash
 pip install wtpsplit
@@ -26,15 +26,15 @@
 # returns an iterator yielding a lists of sentences for every text
 # do this instead of calling wtp.split on every text individually for much better performance
 wtp.split(["This is a test This is another test.", "And some more texts..."])
 
 # if you're using a model with language adapters, also pass a `lang_code`
 wtp.split("This is a test This is another test.", lang_code="en")
 
-# depending on your usecase, adaption to e.g. the Universal Dependencies style may give better results
+# depending on your usecase, adaptation to e.g. the Universal Dependencies style may give better results
 # this always requires a language code
 wtp.split("This is a test This is another test.", lang_code="en", style="ud")
 ```
 
 ## Available Models
 
 Pro tips: I recommend `wtp-bert-mini` for speed-sensitive applications, otherwise `wtp-canine-s-12l`. The `*-no-adapters` models provide a good tradeoff between speed and performance. You should *probably not* use `wtp-bert-tiny`.
@@ -84,14 +84,25 @@
 
 ```python
 # this requires a `lang_code`
 # check the paper or `wtp.mixtures` for supported styles
 wtp.split(text, lang_code="en", style="ud")
 ```
 
+This also allows changing the threshold, but inherently has higher thresholds values since it is not newline probablity anymore being thresholded:
+
+```python
+wtp.split(text, lang_code="en", style="ud", threshold=0.7)
+```
+
+To get the default threshold for a style:
+```python
+wtp.get_threshold("en", "ud", return_punctuation_threshold=True)
+```
+
 #### Threshold Adaptation
 ```python
 threshold = wtp.get_threshold("en", "ud")
 
 wtp.split(text, threshold=threshold)
 ```
 
@@ -140,15 +151,15 @@
 
 ```python
 wtp = WtP("wtp-bert-mini", onnx_providers=["CUDAExecutionProvider", "CPUExecutionProvider"])
 ```
 
 This requires `onnxruntime` and `onnxruntime-gpu`.
 
-However, on my hardware, it *did not* produce a speedup over PyTorch. The embeddings in ONNX inference still have to be computed using PyTorch because hash embeddings are supported by ONNX, so the moving around of tensors might cause it to be slower.
+However, on my hardware, it *did not* produce a speedup over PyTorch. The embeddings in ONNX inference still have to be computed using PyTorch because hash embeddings are not supported by ONNX, so the moving around of tensors might cause it to be slower.
 
 The `wtp-canine-*` models are currently not supported with ONNX because the pooling done by CANINE is not trivial to export. 
 
 Ideas to solve this (and the hash embeddings problem) are very welcome!
 
 ## Supported Languages
 
@@ -236,10 +247,29 @@
 | vi  | Vietnamese             |
 | xh  | Xhosa                  |
 | yi  | Yiddish                |
 | yo  | Yoruba                 |
 | zh  | Chinese                |
 | zu  | Zulu                   |
 
+## Citation
+
+Please cite `wtpsplit` as 
+
+```
+@misc{minixhofer2023wheres,
+      title={Where's the Point? Self-Supervised Multilingual Punctuation-Agnostic Sentence Segmentation}, 
+      author={Benjamin Minixhofer and Jonas Pfeiffer and Ivan Vulić},
+      year={2023},
+      eprint={2305.18893},
+      archivePrefix={arXiv},
+      primaryClass={cs.CL}
+}
+```
+
+## Acknowledgments
+
+Ivan Vulić is supported by a personal Royal Society University Research Fellowship ‘Inclusive and Sustainable Language Technology for a Truly Multilingual World’ (no 221137; 2022–). Research supported with Cloud TPUs from Google’s TPU Research Cloud (TRC). We thank Christoph Minixhofer for advice in the initial stage of this project. We also thank Sebastian Ruder and Srini Narayanan for helpful feedback on a draft of the paper.
+
 ## Previous Version
 
 *This repository previously contained `nnsplit`, the precursor to `wtpsplit`. You can still use the `nnsplit` branch (or the `nnsplit` PyPI releases) for the old version, however, this is highly discouraged and not maintained! Please let me know if you have a usecase which `nnsplit` can solve but `wtpsplit` can not.*
```

### Comparing `wtpsplit-1.0.1/wtpsplit/__init__.py` & `wtpsplit-1.1.0/wtpsplit/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from transformers import AutoModelForTokenClassification
 from transformers.utils.hub import cached_file
 import skops.io as sio
 
 from wtpsplit.extract import extract
 from wtpsplit.utils import Constants, encode, indices_to_sentences
 
-__version__ = "1.0.1"
+__version__ = "1.1.0"
 
 
 class ORTWrapper:
     def __init__(self, model, ort_session):
         self.model = model
         self.ort_session = ort_session
 
@@ -81,15 +81,18 @@
                 mixture_path = model_path / "mixture.skops"
                 if not mixture_path.exists():
                     mixture_path = None
                 onnx_path = model_path / "model.onnx"
                 if not onnx_path.exists():
                     onnx_path = None
             else:
-                mixture_path = cached_file(model_name_to_fetch, "mixtures.skops", **(from_pretrained_kwargs or {}))
+                try:
+                    mixture_path = cached_file(model_name_to_fetch, "mixtures.skops", **(from_pretrained_kwargs or {}))
+                except OSError:
+                    mixture_path = None
 
                 # no need to load if no ort_providers set
                 if ort_providers is not None:
                     onnx_path = cached_file(model_name_to_fetch, "model.onnx", **(from_pretrained_kwargs or {}))
                 else:
                     onnx_path = None
 
@@ -308,14 +311,25 @@
                 pad_last_batch=pad_last_batch,
                 remove_whitespace_before_inference=remove_whitespace_before_inference,
                 outer_batch_size=outer_batch_size,
                 paragraph_threshold=paragraph_threshold,
                 do_paragraph_segmentation=do_paragraph_segmentation,
                 verbose=verbose,
             )
+        
+    def get_threshold(self, lang_code: str, style: str, return_punctuation_threshold: bool = False):
+        try:
+            _, _, punctuation_threshold, threshold = self.mixtures[lang_code][style]
+        except KeyError:
+            raise ValueError(f"Could not find a mixture for the style '{style}' and language '{lang_code}'.")
+
+        if return_punctuation_threshold:
+            return punctuation_threshold
+
+        return threshold
 
     def _split(
         self,
         texts,
         lang_code: str,
         style: str,
         threshold: float,
@@ -335,20 +349,22 @@
 
             if self.mixtures is None:
                 raise ValueError(
                     "This model does not have any associated mixtures. Maybe they are missing from the model directory?"
                 )
 
             try:
-                _, _, sentence_threshold, _ = self.mixtures[lang_code][style]
+                _, _, default_threshold, _ = self.mixtures[lang_code][style]
             except KeyError:
                 raise ValueError(f"Could not find a mixture for the style '{style}'.")
         else:
             # the established default for newline prob threshold is 0.01
-            sentence_threshold = threshold if threshold is not None else 0.01
+            default_threshold = 0.01
+
+        sentence_threshold = threshold if threshold is not None else default_threshold
 
         for text, probs in zip(
             texts,
             self.predict_proba(
                 texts,
                 lang_code=lang_code,
                 style=style,
```

### Comparing `wtpsplit-1.0.1/wtpsplit/data/language_info.csv` & `wtpsplit-1.1.0/wtpsplit/data/language_info.csv`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.0.1/wtpsplit/data/punctuation.json` & `wtpsplit-1.1.0/wtpsplit/data/punctuation.json`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.0.1/wtpsplit/extract.py` & `wtpsplit-1.1.0/wtpsplit/extract.py`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.0.1/wtpsplit/models.py` & `wtpsplit-1.1.0/wtpsplit/models.py`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.0.1/wtpsplit/utils.py` & `wtpsplit-1.1.0/wtpsplit/utils.py`

 * *Files identical despite different names*

