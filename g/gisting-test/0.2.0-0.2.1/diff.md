# Comparing `tmp/gisting_test-0.2.0.tar.gz` & `tmp/gisting_test-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gisting_test-0.2.0.tar", last modified: Sat Jun 17 03:49:01 2023, max compression
+gzip compressed data, was "gisting_test-0.2.1.tar", last modified: Sat Jun 17 04:05:17 2023, max compression
```

## Comparing `gisting_test-0.2.0.tar` & `gisting_test-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-17 03:49:01.656901 gisting_test-0.2.0/
--rw-r--r--   0 owaiszahid   (501) staff       (20)      288 2023-06-17 03:49:01.656788 gisting_test-0.2.0/PKG-INFO
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-17 03:49:01.652113 gisting_test-0.2.0/gisting_test/
--rw-r--r--   0 owaiszahid   (501) staff       (20)       18 2023-06-01 17:36:38.000000 gisting_test-0.2.0/gisting_test/__init__.py
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-17 03:49:01.656056 gisting_test-0.2.0/gisting_test/src/
--rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-06-01 17:49:51.000000 gisting_test-0.2.0/gisting_test/src/__init__.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    11076 2023-05-30 23:00:39.000000 gisting_test-0.2.0/gisting_test/src/arguments.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     3462 2023-05-30 23:00:39.000000 gisting_test-0.2.0/gisting_test/src/benchmarking.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     8819 2023-06-17 03:48:25.000000 gisting_test-0.2.0/gisting_test/src/compress.py
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-17 03:49:01.656559 gisting_test-0.2.0/gisting_test/src/data/
--rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-05-30 23:00:39.000000 gisting_test-0.2.0/gisting_test/src/data/__init__.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     8550 2023-05-30 23:00:39.000000 gisting_test-0.2.0/gisting_test/src/data/gist.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)      554 2023-05-30 23:00:39.000000 gisting_test-0.2.0/gisting_test/src/data/utils.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    21595 2023-05-30 23:00:39.000000 gisting_test-0.2.0/gisting_test/src/generation_utils.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     4748 2023-05-30 23:00:39.000000 gisting_test-0.2.0/gisting_test/src/gist_caching.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    34287 2023-05-30 23:00:39.000000 gisting_test-0.2.0/gisting_test/src/gist_llama.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    41427 2023-05-30 23:00:39.000000 gisting_test-0.2.0/gisting_test/src/gist_t5.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     2954 2023-05-30 23:00:39.000000 gisting_test-0.2.0/gisting_test/src/integrations.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     4277 2023-05-30 23:00:39.000000 gisting_test-0.2.0/gisting_test/src/metrics.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    13819 2023-05-30 23:00:39.000000 gisting_test-0.2.0/gisting_test/src/train.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    52559 2023-05-30 23:00:39.000000 gisting_test-0.2.0/gisting_test/src/trainer_seq2seq.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)      426 2023-05-30 23:00:39.000000 gisting_test-0.2.0/gisting_test/src/utils.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     7880 2023-05-30 23:00:39.000000 gisting_test-0.2.0/gisting_test/src/weight_diff.py
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-17 03:49:01.652856 gisting_test-0.2.0/gisting_test.egg-info/
--rw-r--r--   0 owaiszahid   (501) staff       (20)      288 2023-06-17 03:49:01.000000 gisting_test-0.2.0/gisting_test.egg-info/PKG-INFO
--rw-r--r--   0 owaiszahid   (501) staff       (20)      703 2023-06-17 03:49:01.000000 gisting_test-0.2.0/gisting_test.egg-info/SOURCES.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)        1 2023-06-17 03:49:01.000000 gisting_test-0.2.0/gisting_test.egg-info/dependency_links.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)       52 2023-06-17 03:49:01.000000 gisting_test-0.2.0/gisting_test.egg-info/top_level.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)       38 2023-06-17 03:49:01.656950 gisting_test-0.2.0/setup.cfg
--rw-r--r--   0 owaiszahid   (501) staff       (20)      411 2023-06-17 03:48:41.000000 gisting_test-0.2.0/setup.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-17 04:05:17.020139 gisting_test-0.2.1/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      288 2023-06-17 04:05:17.020020 gisting_test-0.2.1/PKG-INFO
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-17 04:05:17.015529 gisting_test-0.2.1/gisting_test/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       18 2023-06-01 17:36:38.000000 gisting_test-0.2.1/gisting_test/__init__.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-17 04:05:17.019305 gisting_test-0.2.1/gisting_test/src/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-06-01 17:49:51.000000 gisting_test-0.2.1/gisting_test/src/__init__.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    11076 2023-05-30 23:00:39.000000 gisting_test-0.2.1/gisting_test/src/arguments.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     3462 2023-05-30 23:00:39.000000 gisting_test-0.2.1/gisting_test/src/benchmarking.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     8880 2023-06-17 04:04:24.000000 gisting_test-0.2.1/gisting_test/src/compress.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-17 04:05:17.019786 gisting_test-0.2.1/gisting_test/src/data/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-05-30 23:00:39.000000 gisting_test-0.2.1/gisting_test/src/data/__init__.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     8550 2023-05-30 23:00:39.000000 gisting_test-0.2.1/gisting_test/src/data/gist.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      554 2023-05-30 23:00:39.000000 gisting_test-0.2.1/gisting_test/src/data/utils.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    21595 2023-05-30 23:00:39.000000 gisting_test-0.2.1/gisting_test/src/generation_utils.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     4748 2023-05-30 23:00:39.000000 gisting_test-0.2.1/gisting_test/src/gist_caching.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    34287 2023-05-30 23:00:39.000000 gisting_test-0.2.1/gisting_test/src/gist_llama.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    41427 2023-05-30 23:00:39.000000 gisting_test-0.2.1/gisting_test/src/gist_t5.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     2954 2023-05-30 23:00:39.000000 gisting_test-0.2.1/gisting_test/src/integrations.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     4277 2023-05-30 23:00:39.000000 gisting_test-0.2.1/gisting_test/src/metrics.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    13819 2023-05-30 23:00:39.000000 gisting_test-0.2.1/gisting_test/src/train.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    52559 2023-05-30 23:00:39.000000 gisting_test-0.2.1/gisting_test/src/trainer_seq2seq.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      426 2023-05-30 23:00:39.000000 gisting_test-0.2.1/gisting_test/src/utils.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     7880 2023-05-30 23:00:39.000000 gisting_test-0.2.1/gisting_test/src/weight_diff.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-17 04:05:17.016240 gisting_test-0.2.1/gisting_test.egg-info/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      288 2023-06-17 04:05:16.000000 gisting_test-0.2.1/gisting_test.egg-info/PKG-INFO
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      703 2023-06-17 04:05:16.000000 gisting_test-0.2.1/gisting_test.egg-info/SOURCES.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)        1 2023-06-17 04:05:16.000000 gisting_test-0.2.1/gisting_test.egg-info/dependency_links.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       52 2023-06-17 04:05:16.000000 gisting_test-0.2.1/gisting_test.egg-info/top_level.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       38 2023-06-17 04:05:17.020183 gisting_test-0.2.1/setup.cfg
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      411 2023-06-17 04:05:01.000000 gisting_test-0.2.1/setup.py
```

### Comparing `gisting_test-0.2.0/gisting_test/src/arguments.py` & `gisting_test-0.2.1/gisting_test/src/arguments.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.0/gisting_test/src/benchmarking.py` & `gisting_test-0.2.1/gisting_test/src/benchmarking.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.0/gisting_test/src/compress.py` & `gisting_test-0.2.1/gisting_test/src/compress.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             diff, not the full model. If loading one of the Hugging Face LLaMA
             models, use this argument to specify the path to the raw LLaMA model.
     """
     is_llama = "llama" in model_name_or_path.lower()
     is_t5 = "t5" in model_name_or_path.lower()
 
     # Load config
-    config = AutoConfig.from_pretrained(model_name_or_path, cache_dir=cache_dir)
+    config = AutoConfig.from_pretrained(model_name_or_path, cache_dir=cache_dir, device_map="balanced")
 
     # Load model
     print(f"Loading model {model_name_or_path}")
     if is_t5:
         model_cls = GistT5ForConditionalGeneration
     elif is_llama:
         model_cls = GistLlamaForCausalLM
@@ -88,14 +88,15 @@
             raise ValueError(
                 f"{model_name_or_path} is a weight diff huggingface repo. "
                 "You must specify a `base_llama_path` for this to work."
             )
         else:
             print("Weight diff detected. Applying to original model...")
         model, _ = weight_diff.recover(
+            dty
             path_raw=base_llama_path,
             path_diff=model_name_or_path,
             test_inference=False,
             cache_dir=cache_dir,
         )
     else:
         
@@ -118,15 +119,15 @@
     if is_llama:
         tokenizer = LlamaTokenizer.from_pretrained(model_name_or_path)
         tokenizer.pad_token = tokenizer.eos_token
         tokenizer.padding_side = "left"
         assert len(tokenizer) == gist_llama.PRETRAINED_VOCAB_SIZE + 1
         assert model.lm_head.weight.shape[0] == gist_llama.PRETRAINED_VOCAB_SIZE + 1
     else:
-        tokenizer = AutoTokenizer.from_pretrained(model_name_or_path)
+        tokenizer = AutoTokenizer.from_pretrained(model_name_or_path,device_map="balanced")
         assert len(tokenizer) == gist_t5.PRETRAINED_VOCAB_SIZE + 1
         assert model.shared.weight.shape[0] == gist_t5.PRETRAINED_VOCAB_SIZE + 1
     gist_token = tokenizer.additional_special_tokens_ids[-1]
 
     # Compress instruction
     print("Compressing instruction")
     gist_str = "<GIST>" * num_gist_tokens
```

### Comparing `gisting_test-0.2.0/gisting_test/src/data/gist.py` & `gisting_test-0.2.1/gisting_test/src/data/gist.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.0/gisting_test/src/data/utils.py` & `gisting_test-0.2.1/gisting_test/src/data/utils.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.0/gisting_test/src/generation_utils.py` & `gisting_test-0.2.1/gisting_test/src/generation_utils.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.0/gisting_test/src/gist_caching.py` & `gisting_test-0.2.1/gisting_test/src/gist_caching.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.0/gisting_test/src/gist_llama.py` & `gisting_test-0.2.1/gisting_test/src/gist_llama.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.0/gisting_test/src/gist_t5.py` & `gisting_test-0.2.1/gisting_test/src/gist_t5.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.0/gisting_test/src/integrations.py` & `gisting_test-0.2.1/gisting_test/src/integrations.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.0/gisting_test/src/metrics.py` & `gisting_test-0.2.1/gisting_test/src/metrics.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.0/gisting_test/src/train.py` & `gisting_test-0.2.1/gisting_test/src/train.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.0/gisting_test/src/trainer_seq2seq.py` & `gisting_test-0.2.1/gisting_test/src/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.0/gisting_test/src/weight_diff.py` & `gisting_test-0.2.1/gisting_test/src/weight_diff.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.0/gisting_test.egg-info/SOURCES.txt` & `gisting_test-0.2.1/gisting_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

