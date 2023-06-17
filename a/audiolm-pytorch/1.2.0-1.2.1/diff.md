# Comparing `tmp/audiolm-pytorch-1.2.0.tar.gz` & `tmp/audiolm-pytorch-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiolm-pytorch-1.2.0.tar", last modified: Thu Jun 15 16:05:11 2023, max compression
+gzip compressed data, was "audiolm-pytorch-1.2.1.tar", last modified: Sat Jun 17 00:21:13 2023, max compression
```

## Comparing `audiolm-pytorch-1.2.0.tar` & `audiolm-pytorch-1.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:05:11.507958 audiolm-pytorch-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-15 16:05:11.507958 audiolm-pytorch-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19103 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:05:11.507958 audiolm-pytorch-1.2.0/audiolm_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    66183 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/audiolm_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/encodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/hubert_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30270 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/soundstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)    42310 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/audiolm_pytorch/vq_wav2vec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:05:11.507958 audiolm-pytorch-1.2.0/audiolm_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-15 16:05:11.000000 audiolm-pytorch-1.2.0/audiolm_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-15 16:05:11.000000 audiolm-pytorch-1.2.0/audiolm_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:05:11.000000 audiolm-pytorch-1.2.0/audiolm_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-15 16:05:11.000000 audiolm-pytorch-1.2.0/audiolm_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 16:05:11.000000 audiolm-pytorch-1.2.0/audiolm_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:05:11.507958 audiolm-pytorch-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-15 16:04:59.000000 audiolm-pytorch-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:21:13.628920 audiolm-pytorch-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-17 00:21:00.000000 audiolm-pytorch-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-17 00:21:13.628920 audiolm-pytorch-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18642 2023-06-17 00:21:00.000000 audiolm-pytorch-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:21:13.628920 audiolm-pytorch-1.2.1/audiolm_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-17 00:21:00.000000 audiolm-pytorch-1.2.1/audiolm_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-17 00:21:00.000000 audiolm-pytorch-1.2.1/audiolm_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66279 2023-06-17 00:21:00.000000 audiolm-pytorch-1.2.1/audiolm_pytorch/audiolm_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-17 00:21:00.000000 audiolm-pytorch-1.2.1/audiolm_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-17 00:21:00.000000 audiolm-pytorch-1.2.1/audiolm_pytorch/encodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-17 00:21:00.000000 audiolm-pytorch-1.2.1/audiolm_pytorch/hubert_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-17 00:21:00.000000 audiolm-pytorch-1.2.1/audiolm_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30270 2023-06-17 00:21:00.000000 audiolm-pytorch-1.2.1/audiolm_pytorch/soundstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-17 00:21:00.000000 audiolm-pytorch-1.2.1/audiolm_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42310 2023-06-17 00:21:00.000000 audiolm-pytorch-1.2.1/audiolm_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-17 00:21:00.000000 audiolm-pytorch-1.2.1/audiolm_pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 00:21:00.000000 audiolm-pytorch-1.2.1/audiolm_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-17 00:21:00.000000 audiolm-pytorch-1.2.1/audiolm_pytorch/vq_wav2vec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:21:13.628920 audiolm-pytorch-1.2.1/audiolm_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-17 00:21:13.000000 audiolm-pytorch-1.2.1/audiolm_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-17 00:21:13.000000 audiolm-pytorch-1.2.1/audiolm_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 00:21:13.000000 audiolm-pytorch-1.2.1/audiolm_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-17 00:21:13.000000 audiolm-pytorch-1.2.1/audiolm_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 00:21:13.000000 audiolm-pytorch-1.2.1/audiolm_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 00:21:13.628920 audiolm-pytorch-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-17 00:21:00.000000 audiolm-pytorch-1.2.1/setup.py
```

### Comparing `audiolm-pytorch-1.2.0/LICENSE` & `audiolm-pytorch-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.0/PKG-INFO` & `audiolm-pytorch-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.2.0
+Version: 1.2.1
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.2.0/README.md` & `audiolm-pytorch-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 
 - <a href="https://github.com/AndreyBocharnikov">Andrey</a> for identifying a missing loss in soundstream and guiding me through the proper mel spectrogram hyperparameters
 
 - <a href="https://github.com/alexdemartos">Alejandro</a> and <a href="https://github.com/ilya16">Ilya</a> for sharing their results with training soundstream, and for working through a few issues with the local attention positional embeddings
 
 - <a href="https://github.com/LWprogramming">LWprogramming</a> for adding Encodec compatibility!
 
+- <a href="https://github.com/LWprogramming">LWprogramming</a> for finding an issue with handling of the EOS token when sampling from the `FineTransformer`!
+
 - <a href="https://github.com/YoungloLee">@YoungloLee</a> for identifying a big bug in the 1d causal convolution for soundstream related to padding not accounting for strides!
 
 - <a href="https://github.com/haydenshively">Hayden</a> for pointing out some discrepancies in the multi-scale discriminator for Soundstream
 
 ## Install
 
 ```bash
@@ -432,48 +434,31 @@
     year    = {2022},
     url     = {https://openreview.net/forum?id=GMYWzWztDx5},
     note    = {under review}
 }
 ```
 
 ```bibtex
-@article{Li2021LocalViTBL,
-    title   = {LocalViT: Bringing Locality to Vision Transformers},
-    author  = {Yawei Li and K. Zhang and Jie Cao and Radu Timofte and Luc Van Gool},
-    journal = {ArXiv},
-    year    = {2021},
-    volume  = {abs/2104.05707}
-}
-```
-
-```bibtex
 @misc{liu2021swin,
     title   = {Swin Transformer V2: Scaling Up Capacity and Resolution},
     author  = {Ze Liu and Han Hu and Yutong Lin and Zhuliang Yao and Zhenda Xie and Yixuan Wei and Jia Ning and Yue Cao and Zheng Zhang and Li Dong and Furu Wei and Baining Guo},
     year    = {2021},
     eprint  = {2111.09883},
     archivePrefix = {arXiv},
     primaryClass = {cs.CV}
 }
 ```
 
 ```bibtex
-@inproceedings{Ma2022MegaMA,
-    title   = {Mega: Moving Average Equipped Gated Attention},
-    author  = {Xuezhe Ma and Chunting Zhou and Xiang Kong and Junxian He and Liangke Gui and Graham Neubig and Jonathan May and Luke Zettlemoyer},
-    year    = {2022}
-}
-```
-
-```bibtex
-@misc{gilmer2023intriguing
-    title  = {Intriguing Properties of Transformer Training Instabilities},
-    author = {Justin Gilmer, Andrea Schioppa, and Jeremy Cohen},
-    year   = {2023},
-    status = {to be published - one attention stabilization technique is circulating within Google Brain, being used by multiple teams}
+@article{Li2021LocalViTBL,
+    title   = {LocalViT: Bringing Locality to Vision Transformers},
+    author  = {Yawei Li and K. Zhang and Jie Cao and Radu Timofte and Luc Van Gool},
+    journal = {ArXiv},
+    year    = {2021},
+    volume  = {abs/2104.05707}
 }
 ```
 
 ```bibtex
 @article{Defossez2022HighFN,
     title   = {High Fidelity Neural Audio Compression},
     author  = {Alexandre D'efossez and Jade Copet and Gabriel Synnaeve and Yossi Adi},
```

#### html2text {}

```diff
@@ -19,53 +19,54 @@
 debugging of soundstream - Allen and LWprogramming for reviewing the code and
 submitting bug fixes! - Ilya for finding an issue with multi-scale
 discriminator downsampling and for soundstream trainer improvements - Andrey
 for identifying a missing loss in soundstream and guiding me through the proper
 mel spectrogram hyperparameters - Alejandro and Ilya for sharing their results
 with training soundstream, and for working through a few issues with the local
 attention positional embeddings - LWprogramming for adding Encodec
-compatibility! - @YoungloLee for identifying a big bug in the 1d causal
-convolution for soundstream related to padding not accounting for strides! -
-Hayden for pointing out some discrepancies in the multi-scale discriminator for
-Soundstream ## Install ```bash $ pip install audiolm-pytorch ``` ## Usage ###
-SoundStream & Encodec There are two options for the neural codec. If you want
-to use the pretrained 24kHz Encodec, just create an Encodec object as follows:
-```python from audiolm_pytorch import EncodecWrapper encodec = EncodecWrapper()
-# Now you can use the encodec variable in the same way you'd use the
-soundstream variables below. ``` Otherwise, to stay more true to the original
-paper, you can use `SoundStream`. First, `SoundStream` needs to be trained on a
-large corpus of audio data ```python from audiolm_pytorch import SoundStream,
-SoundStreamTrainer soundstream = SoundStream( codebook_size = 1024,
-rq_num_quantizers = 8, rq_groups = 2, # this paper proposes using multi-headed
-residual vector quantization - https://arxiv.org/abs/2305.02765
-attn_window_size = 128, # local attention receptive field at bottleneck
-attn_depth = 2 # 2 local attention transformer blocks - the soundstream folks
-were not experts with attention, so i took the liberty to add some. encodec
-went with lstms, but attention should be better ) trainer = SoundStreamTrainer
-( soundstream, folder = '/path/to/audio/files', batch_size = 4,
-grad_accum_every = 8, # effective batch size of 32 data_max_length_seconds = 2,
-# train on 2 second audio num_train_steps = 1_000_000 ).cuda() trainer.train()
-# after a lot of training, you can test the autoencoding as so audio =
-torch.randn(10080).cuda() recons = soundstream(audio, return_recons_only =
-True) # (1, 10080) - 1 channel ``` You can also use soundstreams that are
-specific to `AudioLM` and `MusicLM` by importing `AudioLMSoundStream` and
-`MusicLMSoundStream` respectively ```python from audiolm_pytorch import
-AudioLMSoundStream, MusicLMSoundStream soundstream = AudioLMSoundStream(...) #
-say you want the hyperparameters as in Audio LM paper # rest is the same as
-above ``` As of version `0.17.0`, you can now invoke the class method on
-`SoundStream` to load from checkpoint files, without having to remember your
-configurations. ```python from audiolm_pytorch import SoundStream soundstream =
-SoundStream.init_and_load_from('./path/to/checkpoint.pt') ``` ### Hierarchical
-Transformers Then three separate transformers (`SemanticTransformer`,
-`CoarseTransformer`, `FineTransformer`) need to be trained ex.
-`SemanticTransformer` ```python import torch from audiolm_pytorch import
-HubertWithKmeans, SemanticTransformer, SemanticTransformerTrainer # hubert
-checkpoints can be downloaded at # https://github.com/facebookresearch/fairseq/
-tree/main/examples/hubert wav2vec = HubertWithKmeans( checkpoint_path = './
-hubert/hubert_base_ls960.pt', kmeans_path = './hubert/
+compatibility! - LWprogramming for finding an issue with handling of the EOS
+token when sampling from the `FineTransformer`! - @YoungloLee for identifying a
+big bug in the 1d causal convolution for soundstream related to padding not
+accounting for strides! - Hayden for pointing out some discrepancies in the
+multi-scale discriminator for Soundstream ## Install ```bash $ pip install
+audiolm-pytorch ``` ## Usage ### SoundStream & Encodec There are two options
+for the neural codec. If you want to use the pretrained 24kHz Encodec, just
+create an Encodec object as follows: ```python from audiolm_pytorch import
+EncodecWrapper encodec = EncodecWrapper() # Now you can use the encodec
+variable in the same way you'd use the soundstream variables below. ```
+Otherwise, to stay more true to the original paper, you can use `SoundStream`.
+First, `SoundStream` needs to be trained on a large corpus of audio data
+```python from audiolm_pytorch import SoundStream, SoundStreamTrainer
+soundstream = SoundStream( codebook_size = 1024, rq_num_quantizers = 8,
+rq_groups = 2, # this paper proposes using multi-headed residual vector
+quantization - https://arxiv.org/abs/2305.02765 attn_window_size = 128, # local
+attention receptive field at bottleneck attn_depth = 2 # 2 local attention
+transformer blocks - the soundstream folks were not experts with attention, so
+i took the liberty to add some. encodec went with lstms, but attention should
+be better ) trainer = SoundStreamTrainer( soundstream, folder = '/path/to/
+audio/files', batch_size = 4, grad_accum_every = 8, # effective batch size of
+32 data_max_length_seconds = 2, # train on 2 second audio num_train_steps =
+1_000_000 ).cuda() trainer.train() # after a lot of training, you can test the
+autoencoding as so audio = torch.randn(10080).cuda() recons = soundstream
+(audio, return_recons_only = True) # (1, 10080) - 1 channel ``` You can also
+use soundstreams that are specific to `AudioLM` and `MusicLM` by importing
+`AudioLMSoundStream` and `MusicLMSoundStream` respectively ```python from
+audiolm_pytorch import AudioLMSoundStream, MusicLMSoundStream soundstream =
+AudioLMSoundStream(...) # say you want the hyperparameters as in Audio LM paper
+# rest is the same as above ``` As of version `0.17.0`, you can now invoke the
+class method on `SoundStream` to load from checkpoint files, without having to
+remember your configurations. ```python from audiolm_pytorch import SoundStream
+soundstream = SoundStream.init_and_load_from('./path/to/checkpoint.pt') ``` ###
+Hierarchical Transformers Then three separate transformers
+(`SemanticTransformer`, `CoarseTransformer`, `FineTransformer`) need to be
+trained ex. `SemanticTransformer` ```python import torch from audiolm_pytorch
+import HubertWithKmeans, SemanticTransformer, SemanticTransformerTrainer #
+hubert checkpoints can be downloaded at # https://github.com/facebookresearch/
+fairseq/tree/main/examples/hubert wav2vec = HubertWithKmeans( checkpoint_path =
+'./hubert/hubert_base_ls960.pt', kmeans_path = './hubert/
 hubert_base_ls960_L9_km500.bin' ) semantic_transformer = SemanticTransformer
 ( num_semantic_tokens = wav2vec.codebook_size, dim = 1024, depth = 6,
 flash_attn = True ).cuda() trainer = SemanticTransformerTrainer( transformer =
 semantic_transformer, wav2vec = wav2vec, folder ='/path/to/audio/files',
 batch_size = 1, data_max_length = 320 * 32, num_train_steps = 1 ) trainer.train
 () ``` ex. `CoarseTransformer` ```python import torch from audiolm_pytorch
 import HubertWithKmeans, SoundStream, CoarseTransformer,
@@ -179,33 +180,25 @@
 Makes Causal Language Models Better Zero-Shot Learners}, author = {Hao Liu and
 Xinyang Geng and Lisa Lee and Igor Mordatch and Sergey Levine and Sharan Narang
 and P. Abbeel}, journal = {ArXiv}, year = {2022}, volume = {abs/2210.13432} }
 ``` ```bibtex @inproceedings{anonymous2022normformer, title = {NormFormer:
 Improved Transformer Pretraining with Extra Normalization}, author =
 {Anonymous}, booktitle = {Submitted to The Tenth International Conference on
 Learning Representations }, year = {2022}, url = {https://openreview.net/
-forum?id=GMYWzWztDx5}, note = {under review} } ``` ```bibtex @article
-{Li2021LocalViTBL, title = {LocalViT: Bringing Locality to Vision
-Transformers}, author = {Yawei Li and K. Zhang and Jie Cao and Radu Timofte and
-Luc Van Gool}, journal = {ArXiv}, year = {2021}, volume = {abs/2104.05707} }
-``` ```bibtex @misc{liu2021swin, title = {Swin Transformer V2: Scaling Up
-Capacity and Resolution}, author = {Ze Liu and Han Hu and Yutong Lin and
-Zhuliang Yao and Zhenda Xie and Yixuan Wei and Jia Ning and Yue Cao and Zheng
-Zhang and Li Dong and Furu Wei and Baining Guo}, year = {2021}, eprint =
-{2111.09883}, archivePrefix = {arXiv}, primaryClass = {cs.CV} } ``` ```bibtex
-@inproceedings{Ma2022MegaMA, title = {Mega: Moving Average Equipped Gated
-Attention}, author = {Xuezhe Ma and Chunting Zhou and Xiang Kong and Junxian He
-and Liangke Gui and Graham Neubig and Jonathan May and Luke Zettlemoyer}, year
-= {2022} } ``` ```bibtex @misc{gilmer2023intriguing title = {Intriguing
-Properties of Transformer Training Instabilities}, author = {Justin Gilmer,
-Andrea Schioppa, and Jeremy Cohen}, year = {2023}, status = {to be published -
-one attention stabilization technique is circulating within Google Brain, being
-used by multiple teams} } ``` ```bibtex @article{Defossez2022HighFN, title =
-{High Fidelity Neural Audio Compression}, author = {Alexandre D'efossez and
-Jade Copet and Gabriel Synnaeve and Yossi Adi}, journal = {ArXiv}, year =
+forum?id=GMYWzWztDx5}, note = {under review} } ``` ```bibtex @misc{liu2021swin,
+title = {Swin Transformer V2: Scaling Up Capacity and Resolution}, author = {Ze
+Liu and Han Hu and Yutong Lin and Zhuliang Yao and Zhenda Xie and Yixuan Wei
+and Jia Ning and Yue Cao and Zheng Zhang and Li Dong and Furu Wei and Baining
+Guo}, year = {2021}, eprint = {2111.09883}, archivePrefix = {arXiv},
+primaryClass = {cs.CV} } ``` ```bibtex @article{Li2021LocalViTBL, title =
+{LocalViT: Bringing Locality to Vision Transformers}, author = {Yawei Li and K.
+Zhang and Jie Cao and Radu Timofte and Luc Van Gool}, journal = {ArXiv}, year =
+{2021}, volume = {abs/2104.05707} } ``` ```bibtex @article{Defossez2022HighFN,
+title = {High Fidelity Neural Audio Compression}, author = {Alexandre D'efossez
+and Jade Copet and Gabriel Synnaeve and Yossi Adi}, journal = {ArXiv}, year =
 {2022}, volume = {abs/2210.13438} } ``` ```bibtex @article
 {Hu2017SqueezeandExcitationN, title = {Squeeze-and-Excitation Networks}, author
 = {Jie Hu and Li Shen and Gang Sun}, journal = {2018 IEEE/CVF Conference on
 Computer Vision and Pattern Recognition}, year = {2017}, pages = {7132-7141} }
 ``` ```bibtex @inproceedings{Yang2023HiFiCodecGV, title = {HiFi-Codec: Group-
 residual Vector quantization for High Fidelity Audio Codec}, author = {Dongchao
 Yang and Songxiang Liu and Rongjie Huang and Jinchuan Tian and Chao Weng and
```

### Comparing `audiolm-pytorch-1.2.0/audiolm_pytorch/__init__.py` & `audiolm-pytorch-1.2.1/audiolm_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.0/audiolm_pytorch/attend.py` & `audiolm-pytorch-1.2.1/audiolm_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.0/audiolm_pytorch/audiolm_pytorch.py` & `audiolm-pytorch-1.2.1/audiolm_pytorch/audiolm_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1359,29 +1359,29 @@
         # initialize
 
         init_coarse_time_step = coarse_token_ids.shape[-1]
         sampled_coarse_token_ids = coarse_token_ids.clone()
 
         for time_step in tqdm(range(init_coarse_time_step, max_time_steps), desc = 'generating coarse'):
             for ind in range(self.num_coarse_quantizers):
-                is_last_step = ind == (self.num_coarse_quantizers - 1)
+                just_finished_quantizer_step = (ind == 0 and time_step > 0)
 
                 _, coarse_logits = self.transformer.forward_with_cond_scale(
                     coarse_token_ids = sampled_coarse_token_ids,
                     semantic_token_ids = semantic_token_ids,
                     text_embeds = text_embeds,
                     cond_scale = cond_scale,
                     return_only_coarse_logits = True,
                     **kwargs
                 )
 
                 last_coarse_logits = coarse_logits[:, -1]
 
-                if not is_last_step:
-                    last_coarse_logits[:, -1] = float('-inf') # prevent from eos if not last quantizer step, but move this to masking logic within the transformer at some point, for both training and eval
+                if not just_finished_quantizer_step:
+                    last_coarse_logits[:, -1] = float('-inf') # prevent from eos in the middle of a time step
 
                 filtered_logits = top_k(last_coarse_logits, thres = filter_thres)
                 sampled = gumbel_sample(filtered_logits, temperature = temperature, dim = -1)
 
                 sampled = rearrange(sampled, 'b -> b 1')
                 sampled_coarse_token_ids = torch.cat((sampled_coarse_token_ids, sampled), dim = -1)
 
@@ -1586,27 +1586,30 @@
         init_fine_time_step = fine_token_ids.shape[-1]
         max_time_steps = coarse_token_ids.shape[1] // self.num_coarse_quantizers
 
         sampled_fine_token_ids = fine_token_ids.clone()
 
         for time_step in tqdm(range(init_fine_time_step, max_time_steps), desc = 'generating fine'):
             for ind in range(self.num_fine_quantizers):
-                is_last_step = ind == (self.num_fine_quantizers - 1)
+                just_finished_quantizer_step = (ind == 0 and time_step > 0)
 
                 _, fine_logits = self.transformer.forward_with_cond_scale(
                     coarse_token_ids = coarse_token_ids,
                     fine_token_ids = sampled_fine_token_ids,
                     text_embeds = text_embeds,
                     cond_scale = cond_scale,
                     return_only_fine_logits = True,
                     **kwargs
                 )
 
                 last_fine_logits = fine_logits[:, -1]
 
+                if not just_finished_quantizer_step:
+                    last_fine_logits[:, -1] = float('-inf')  # prevent from eos in the middle of a time step
+
                 filtered_logits = top_k(last_fine_logits, thres = filter_thres)
                 sampled = gumbel_sample(filtered_logits, temperature = temperature, dim = -1)
 
                 sampled = rearrange(sampled, 'b -> b 1')
                 sampled_fine_token_ids = torch.cat((sampled_fine_token_ids, sampled), dim = -1)
 
         sampled_fine_token_ids = mask_out_after_eos_id(sampled_fine_token_ids, self.eos_id, keep_eos = False)
```

### Comparing `audiolm-pytorch-1.2.0/audiolm_pytorch/data.py` & `audiolm-pytorch-1.2.1/audiolm_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.0/audiolm_pytorch/encodec.py` & `audiolm-pytorch-1.2.1/audiolm_pytorch/encodec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.0/audiolm_pytorch/hubert_kmeans.py` & `audiolm-pytorch-1.2.1/audiolm_pytorch/hubert_kmeans.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.0/audiolm_pytorch/optimizer.py` & `audiolm-pytorch-1.2.1/audiolm_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.0/audiolm_pytorch/soundstream.py` & `audiolm-pytorch-1.2.1/audiolm_pytorch/soundstream.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.0/audiolm_pytorch/t5.py` & `audiolm-pytorch-1.2.1/audiolm_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.0/audiolm_pytorch/trainer.py` & `audiolm-pytorch-1.2.1/audiolm_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.0/audiolm_pytorch/vq_wav2vec.py` & `audiolm-pytorch-1.2.1/audiolm_pytorch/vq_wav2vec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.0/audiolm_pytorch.egg-info/PKG-INFO` & `audiolm-pytorch-1.2.1/audiolm_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.2.0
+Version: 1.2.1
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.2.0/audiolm_pytorch.egg-info/SOURCES.txt` & `audiolm-pytorch-1.2.1/audiolm_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.0/setup.py` & `audiolm-pytorch-1.2.1/setup.py`

 * *Files identical despite different names*

