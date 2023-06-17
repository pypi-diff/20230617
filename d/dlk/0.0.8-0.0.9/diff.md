# Comparing `tmp/dlk-0.0.8.tar.gz` & `tmp/dlk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dlk-0.0.8.tar", last modified: Tue Mar 22 13:01:20 2022, max compression
+gzip compressed data, was "dist/dlk-0.0.9.tar", last modified: Wed Mar 23 18:09:00 2022, max compression
```

## Comparing `dlk-0.0.8.tar` & `dlk-0.0.9.tar`

### file list

```diff
@@ -1,383 +1,383 @@
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:20.036630 dlk-0.0.8/
--rw-r--r--   0 sun       (1000) sun       (1000)      351 2021-12-23 12:39:24.000000 dlk-0.0.8/.gitignore
--rw-r--r--   0 sun       (1000) sun       (1000)      753 2021-12-23 14:24:24.000000 dlk-0.0.8/.readthedocs.yaml
--rw-r--r--   0 sun       (1000) sun       (1000)    11382 2021-12-17 16:45:41.000000 dlk-0.0.8/LICENSE
--rw-r--r--   0 sun       (1000) sun       (1000)     1827 2022-03-22 13:01:20.035632 dlk-0.0.8/PKG-INFO
--rw-r--r--   0 sun       (1000) sun       (1000)     1516 2021-12-23 15:27:28.000000 dlk-0.0.8/README.md
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.825552 dlk-0.0.8/dlk/
--rw-r--r--   0 sun       (1000) sun       (1000)      617 2022-03-22 12:57:22.000000 dlk-0.0.8/dlk/__init__.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.804608 dlk-0.0.8/dlk/configures/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.802614 dlk-0.0.8/dlk/configures/core/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.844502 dlk-0.0.8/dlk/configures/core/callbacks/
--rw-r--r--   0 sun       (1000) sun       (1000)      858 2021-12-17 18:19:33.000000 dlk-0.0.8/dlk/configures/core/callbacks/checkpoint.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      187 2021-12-17 18:19:16.000000 dlk-0.0.8/dlk/configures/core/callbacks/checkpoint@train_loss.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      214 2021-12-17 18:19:02.000000 dlk-0.0.8/dlk/configures/core/callbacks/checkpoint@val_loss.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      560 2021-12-17 18:30:29.000000 dlk-0.0.8/dlk/configures/core/callbacks/early_stop.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      260 2021-12-17 18:33:03.000000 dlk-0.0.8/dlk/configures/core/callbacks/lr_monitor.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      122 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/core/callbacks/progressbar.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      610 2021-12-17 18:37:22.000000 dlk-0.0.8/dlk/configures/core/callbacks/weight_average.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.848491 dlk-0.0.8/dlk/configures/core/imodels/
--rw-r--r--   0 sun       (1000) sun       (1000)      263 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/core/imodels/basic.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      358 2021-12-22 15:37:11.000000 dlk-0.0.8/dlk/configures/core/imodels/basic@seq_lab#crf.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      309 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/core/imodels/basic@seq_lab.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      309 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/imodels/basic@span_cls.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      309 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/core/imodels/basic@txt_cls.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      513 2021-12-20 14:37:30.000000 dlk-0.0.8/dlk/configures/core/imodels/basic@txt_log_reg.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      513 2021-12-20 14:37:40.000000 dlk-0.0.8/dlk/configures/core/imodels/basic@txt_reg.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.851483 dlk-0.0.8/dlk/configures/core/initmethods/
--rw-r--r--   0 sun       (1000) sun       (1000)       50 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/core/initmethods/default.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)       75 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/core/initmethods/range_norm.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)       78 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/core/initmethods/range_uniform.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.801616 dlk-0.0.8/dlk/configures/core/layers/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.853477 dlk-0.0.8/dlk/configures/core/layers/decoders/
--rw-r--r--   0 sun       (1000) sun       (1000)      526 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/layers/decoders/biaffine.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      132 2021-12-19 09:24:47.000000 dlk-0.0.8/dlk/configures/core/layers/decoders/identity.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      473 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/layers/decoders/linear.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      680 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/layers/decoders/linear_crf.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.858464 dlk-0.0.8/dlk/configures/core/layers/embeddings/
--rw-r--r--   0 sun       (1000) sun       (1000)     2666 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/layers/embeddings/combine_word_char_cnn.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      103 2021-12-17 18:45:52.000000 dlk-0.0.8/dlk/configures/core/layers/embeddings/identity.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      601 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/layers/embeddings/pretrained_transformers.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      643 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/layers/embeddings/pretrained_transformers@gather.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      240 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/layers/embeddings/random.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      779 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/layers/embeddings/static.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1282 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/layers/embeddings/static_char_cnn.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.860459 dlk-0.0.8/dlk/configures/core/layers/encoders/
--rw-r--r--   0 sun       (1000) sun       (1000)      132 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/core/layers/encoders/identity.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      444 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/layers/encoders/linear.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      478 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/layers/encoders/lstm.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.863451 dlk-0.0.8/dlk/configures/core/losses/
--rw-r--r--   0 sun       (1000) sun       (1000)      441 2021-12-20 13:50:20.000000 dlk-0.0.8/dlk/configures/core/losses/bce.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      469 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/core/losses/cross_entropy.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      597 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/core/losses/cross_entropy@cls.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      286 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/core/losses/identity.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      413 2021-12-18 21:32:23.000000 dlk-0.0.8/dlk/configures/core/losses/mse.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.869435 dlk-0.0.8/dlk/configures/core/models/
--rw-r--r--   0 sun       (1000) sun       (1000)     3457 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/models/basic@seq_lab#lstm_cnn_crf.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2139 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/models/basic@seq_lab#lstm_crf.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2190 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/models/basic@seq_lab#lstm_linear.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1277 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/models/basic@seq_lab#pretrained_transformers.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1226 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/models/basic@seq_lab#pretrained_transformers_crf.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1461 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/models/basic@seq_lab#pretrained_transformers_lstm_crf.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1186 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/models/basic@span_cls#pretrained_transformer.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2145 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/models/basic@txt_cls#lstm_linear.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1143 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/models/basic@txt_cls#pretrained_transformers.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.875419 dlk-0.0.8/dlk/configures/core/modules/
--rw-r--r--   0 sun       (1000) sun       (1000)      168 2021-12-20 14:27:27.000000 dlk-0.0.8/dlk/configures/core/modules/bert.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      215 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/core/modules/biaffine.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      200 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/core/modules/conv1d.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      158 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/core/modules/crf.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      175 2021-12-20 14:27:31.000000 dlk-0.0.8/dlk/configures/core/modules/distil_bert.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      177 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/core/modules/linear.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      315 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/core/modules/lstm.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      171 2021-12-20 14:27:35.000000 dlk-0.0.8/dlk/configures/core/modules/roberta.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.877413 dlk-0.0.8/dlk/configures/core/optimizers/
--rw-r--r--   0 sun       (1000) sun       (1000)      798 2021-12-22 15:37:11.000000 dlk-0.0.8/dlk/configures/core/optimizers/adamw.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      538 2021-12-22 15:37:11.000000 dlk-0.0.8/dlk/configures/core/optimizers/adamw@bias_nodecay.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      816 2021-12-22 15:37:11.000000 dlk-0.0.8/dlk/configures/core/optimizers/sgd.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.880406 dlk-0.0.8/dlk/configures/core/schedulers/
--rw-r--r--   0 sun       (1000) sun       (1000)       77 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/core/schedulers/constant.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      116 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/core/schedulers/constant_warmup.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      175 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/core/schedulers/cosine_warmup.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      150 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/core/schedulers/linear_warmup.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      172 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/core/schedulers/rec_decay.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.803611 dlk-0.0.8/dlk/configures/data/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.885391 dlk-0.0.8/dlk/configures/data/datamodules/
--rw-r--r--   0 sun       (1000) sun       (1000)      883 2022-02-08 13:48:24.000000 dlk-0.0.8/dlk/configures/data/datamodules/basic.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      914 2022-02-08 13:48:24.000000 dlk-0.0.8/dlk/configures/data/datamodules/basic@seq_lab#with_char.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      960 2022-02-08 13:48:24.000000 dlk-0.0.8/dlk/configures/data/datamodules/basic@seq_lab#wordmask.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      881 2022-02-08 13:48:24.000000 dlk-0.0.8/dlk/configures/data/datamodules/basic@seq_lab.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      967 2022-02-08 13:48:24.000000 dlk-0.0.8/dlk/configures/data/datamodules/basic@span_cls.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      842 2022-02-08 13:48:24.000000 dlk-0.0.8/dlk/configures/data/datamodules/basic@txt_cls.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      810 2022-02-08 13:48:24.000000 dlk-0.0.8/dlk/configures/data/datamodules/basic@txt_reg.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.889381 dlk-0.0.8/dlk/configures/data/postprocessors/
--rw-r--r--   0 sun       (1000) sun       (1000)       28 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/data/postprocessors/identity.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1651 2022-01-08 15:40:43.000000 dlk-0.0.8/dlk/configures/data/postprocessors/seq_lab.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1458 2022-02-08 13:48:24.000000 dlk-0.0.8/dlk/configures/data/postprocessors/span_cls.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      866 2021-12-23 13:03:12.000000 dlk-0.0.8/dlk/configures/data/postprocessors/txt_cls.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      769 2021-12-22 15:37:11.000000 dlk-0.0.8/dlk/configures/data/postprocessors/txt_reg.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.896363 dlk-0.0.8/dlk/configures/data/processors/
--rw-r--r--   0 sun       (1000) sun       (1000)     5707 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/data/processors/basic@seq_lab#norm_static.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     7108 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/data/processors/basic@seq_lab#norm_static_word_char.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     3944 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/data/processors/basic@seq_lab#pretrained.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     5112 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/data/processors/basic@seq_lab#static.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     3413 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/data/processors/basic@span_cls#pretrained.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     3365 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/data/processors/basic@txt_cls#pretrained.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     4468 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/data/processors/basic@txt_cls.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2690 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/data/processors/basic@txt_match#pretrained.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1628 2021-12-31 16:56:37.000000 dlk-0.0.8/dlk/configures/data/processors/basic@txt_match_reg#pretrained.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2058 2021-12-31 16:56:37.000000 dlk-0.0.8/dlk/configures/data/processors/basic@txt_reg#pretrained.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.908331 dlk-0.0.8/dlk/configures/data/subprocessors/
--rw-r--r--   0 sun       (1000) sun       (1000)      838 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/configures/data/subprocessors/basic_data_loader@seq_lab.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1089 2021-12-31 16:56:37.000000 dlk-0.0.8/dlk/configures/data/subprocessors/basic_data_loader@txt_cls.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      986 2022-02-08 13:48:24.000000 dlk-0.0.8/dlk/configures/data/subprocessors/basic_data_loader@txt_cls_pair.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1090 2021-12-31 16:56:37.000000 dlk-0.0.8/dlk/configures/data/subprocessors/basic_data_loader@txt_reg.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      987 2022-02-08 13:48:24.000000 dlk-0.0.8/dlk/configures/data/subprocessors/basic_data_loader@txt_reg_pair.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      796 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/data/subprocessors/char_gather.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2876 2021-12-31 16:56:37.000000 dlk-0.0.8/dlk/configures/data/subprocessors/fast_tokenizer.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2777 2021-12-20 15:46:38.000000 dlk-0.0.8/dlk/configures/data/subprocessors/fast_tokenizer@pair.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      164 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/data/subprocessors/load.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      119 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/data/subprocessors/save.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1376 2022-01-12 12:59:43.000000 dlk-0.0.8/dlk/configures/data/subprocessors/seq_lab_firstpiece_relabel.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1229 2022-01-12 12:59:43.000000 dlk-0.0.8/dlk/configures/data/subprocessors/seq_lab_relabel.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1245 2022-01-12 12:59:43.000000 dlk-0.0.8/dlk/configures/data/subprocessors/span_cls_relabel.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      759 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/data/subprocessors/token2charid.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      690 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/data/subprocessors/token2id.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      639 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/data/subprocessors/token_embedding.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      878 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/data/subprocessors/token_gather.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      920 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/configures/data/subprocessors/token_norm.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.909328 dlk-0.0.8/dlk/configures/managers/
--rw-r--r--   0 sun       (1000) sun       (1000)     2123 2022-03-22 12:56:04.000000 dlk-0.0.8/dlk/configures/managers/lightning.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2785 2022-03-22 12:56:04.000000 dlk-0.0.8/dlk/configures/managers/lightning@advance.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.911323 dlk-0.0.8/dlk/configures/tasks/
--rw-r--r--   0 sun       (1000) sun       (1000)      441 2021-12-18 17:41:20.000000 dlk-0.0.8/dlk/configures/tasks/test_base.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1915 2021-12-18 17:41:14.000000 dlk-0.0.8/dlk/configures/tasks/test_base_search.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.912320 dlk-0.0.8/dlk/core/
--rw-r--r--   0 sun       (1000) sun       (1000)      595 2021-12-21 17:46:19.000000 dlk-0.0.8/dlk/core/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     9951 2022-03-22 12:56:04.000000 dlk-0.0.8/dlk/core/base_module.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.915312 dlk-0.0.8/dlk/core/callbacks/
--rw-r--r--   0 sun       (1000) sun       (1000)     1447 2021-12-21 17:45:09.000000 dlk-0.0.8/dlk/core/callbacks/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3243 2021-12-23 14:42:18.000000 dlk-0.0.8/dlk/core/callbacks/checkpoint.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2780 2021-12-22 18:51:40.000000 dlk-0.0.8/dlk/core/callbacks/early_stop.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2011 2021-12-22 18:51:40.000000 dlk-0.0.8/dlk/core/callbacks/lr_monitor.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2746 2021-12-22 18:51:40.000000 dlk-0.0.8/dlk/core/callbacks/weight_average.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.917307 dlk-0.0.8/dlk/core/imodels/
--rw-r--r--   0 sun       (1000) sun       (1000)     3493 2021-12-23 12:36:26.000000 dlk-0.0.8/dlk/core/imodels/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)    13363 2022-03-22 12:56:04.000000 dlk-0.0.8/dlk/core/imodels/basic.py
--rw-r--r--   0 sun       (1000) sun       (1000)      672 2021-12-21 17:45:18.000000 dlk-0.0.8/dlk/core/imodels/distill.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.920299 dlk-0.0.8/dlk/core/initmethods/
--rw-r--r--   0 sun       (1000) sun       (1000)     1500 2021-12-21 17:45:19.000000 dlk-0.0.8/dlk/core/initmethods/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5290 2021-12-22 18:51:40.000000 dlk-0.0.8/dlk/core/initmethods/default.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2413 2021-12-22 18:51:40.000000 dlk-0.0.8/dlk/core/initmethods/range_norm.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2837 2021-12-22 18:51:40.000000 dlk-0.0.8/dlk/core/initmethods/range_uniform.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.921296 dlk-0.0.8/dlk/core/layers/
--rw-r--r--   0 sun       (1000) sun       (1000)      596 2021-12-21 17:45:21.000000 dlk-0.0.8/dlk/core/layers/__init__.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.924288 dlk-0.0.8/dlk/core/layers/decoders/
--rw-r--r--   0 sun       (1000) sun       (1000)     1459 2021-12-21 17:45:21.000000 dlk-0.0.8/dlk/core/layers/decoders/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3901 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/core/layers/decoders/biaffine.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1577 2021-12-22 18:51:40.000000 dlk-0.0.8/dlk/core/layers/decoders/identity.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3205 2021-12-22 18:51:40.000000 dlk-0.0.8/dlk/core/layers/decoders/linear.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5390 2021-12-22 18:51:40.000000 dlk-0.0.8/dlk/core/layers/decoders/linear_crf.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.929275 dlk-0.0.8/dlk/core/layers/embeddings/
--rw-r--r--   0 sun       (1000) sun       (1000)     1900 2021-12-21 17:45:23.000000 dlk-0.0.8/dlk/core/layers/embeddings/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     7628 2021-12-22 18:51:40.000000 dlk-0.0.8/dlk/core/layers/embeddings/combine_word_char_cnn.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1645 2021-12-22 18:51:40.000000 dlk-0.0.8/dlk/core/layers/embeddings/identity.py
--rw-r--r--   0 sun       (1000) sun       (1000)     6148 2021-12-22 18:53:49.000000 dlk-0.0.8/dlk/core/layers/embeddings/pretrained_transformers.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3412 2021-12-22 18:51:40.000000 dlk-0.0.8/dlk/core/layers/embeddings/random.py
--rw-r--r--   0 sun       (1000) sun       (1000)     4532 2021-12-22 18:51:40.000000 dlk-0.0.8/dlk/core/layers/embeddings/static.py
--rw-r--r--   0 sun       (1000) sun       (1000)     6084 2021-12-22 18:51:40.000000 dlk-0.0.8/dlk/core/layers/embeddings/static_char_cnn.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.932267 dlk-0.0.8/dlk/core/layers/encoders/
--rw-r--r--   0 sun       (1000) sun       (1000)     1415 2021-12-21 17:45:26.000000 dlk-0.0.8/dlk/core/layers/encoders/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1617 2021-12-22 18:51:41.000000 dlk-0.0.8/dlk/core/layers/encoders/identity.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3149 2021-12-22 18:51:41.000000 dlk-0.0.8/dlk/core/layers/encoders/linear.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3293 2021-12-22 18:51:41.000000 dlk-0.0.8/dlk/core/layers/encoders/lstm.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.936256 dlk-0.0.8/dlk/core/losses/
--rw-r--r--   0 sun       (1000) sun       (1000)     1415 2021-12-21 17:45:28.000000 dlk-0.0.8/dlk/core/losses/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5002 2021-12-22 18:58:35.000000 dlk-0.0.8/dlk/core/losses/bce.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5572 2021-12-22 18:58:35.000000 dlk-0.0.8/dlk/core/losses/cross_entropy.py
--rw-r--r--   0 sun       (1000) sun       (1000)     4061 2021-12-22 19:06:58.000000 dlk-0.0.8/dlk/core/losses/identity.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5004 2021-12-22 18:58:33.000000 dlk-0.0.8/dlk/core/losses/mse.py
--rw-r--r--   0 sun       (1000) sun       (1000)     4068 2021-12-22 18:58:48.000000 dlk-0.0.8/dlk/core/losses/multi_loss.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.937899 dlk-0.0.8/dlk/core/models/
--rw-r--r--   0 sun       (1000) sun       (1000)     1419 2021-12-21 17:45:31.000000 dlk-0.0.8/dlk/core/models/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     9621 2022-01-12 15:49:24.000000 dlk-0.0.8/dlk/core/models/basic.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.944875 dlk-0.0.8/dlk/core/modules/
--rw-r--r--   0 sun       (1000) sun       (1000)     3230 2022-01-12 15:49:24.000000 dlk-0.0.8/dlk/core/modules/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5854 2022-03-22 12:56:04.000000 dlk-0.0.8/dlk/core/modules/bert.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3423 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/core/modules/biaffine.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2719 2021-12-22 18:51:41.000000 dlk-0.0.8/dlk/core/modules/conv1d.py
--rw-r--r--   0 sun       (1000) sun       (1000)    10299 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/core/modules/crf.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5450 2021-12-23 12:36:26.000000 dlk-0.0.8/dlk/core/modules/distil_bert.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2765 2021-12-22 18:51:41.000000 dlk-0.0.8/dlk/core/modules/linear.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3533 2022-03-22 12:56:04.000000 dlk-0.0.8/dlk/core/modules/logits_gather.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3463 2021-12-22 18:51:41.000000 dlk-0.0.8/dlk/core/modules/lstm.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5885 2021-12-22 18:51:41.000000 dlk-0.0.8/dlk/core/modules/roberta.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.946870 dlk-0.0.8/dlk/core/optimizers/
--rw-r--r--   0 sun       (1000) sun       (1000)     4066 2021-12-22 18:28:20.000000 dlk-0.0.8/dlk/core/optimizers/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2869 2021-12-22 18:51:41.000000 dlk-0.0.8/dlk/core/optimizers/adamw.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2918 2021-12-22 18:51:41.000000 dlk-0.0.8/dlk/core/optimizers/sgd.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.951856 dlk-0.0.8/dlk/core/schedulers/
--rw-r--r--   0 sun       (1000) sun       (1000)     1881 2021-12-22 18:28:20.000000 dlk-0.0.8/dlk/core/schedulers/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1903 2021-12-22 18:51:41.000000 dlk-0.0.8/dlk/core/schedulers/constant.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2388 2021-12-22 18:51:41.000000 dlk-0.0.8/dlk/core/schedulers/constant_warmup.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3047 2021-12-22 18:51:41.000000 dlk-0.0.8/dlk/core/schedulers/cosine_warmup.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3025 2021-12-22 18:51:41.000000 dlk-0.0.8/dlk/core/schedulers/linear_warmup.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2617 2021-12-21 17:45:41.000000 dlk-0.0.8/dlk/core/schedulers/multi_group_schedule.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2966 2021-12-22 18:51:41.000000 dlk-0.0.8/dlk/core/schedulers/rec_decay.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.951856 dlk-0.0.8/dlk/data/
--rw-r--r--   0 sun       (1000) sun       (1000)      596 2021-12-21 17:45:41.000000 dlk-0.0.8/dlk/data/__init__.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.953851 dlk-0.0.8/dlk/data/datamodules/
--rw-r--r--   0 sun       (1000) sun       (1000)     5164 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/data/datamodules/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     8952 2022-02-08 13:48:24.000000 dlk-0.0.8/dlk/data/datamodules/basic.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1889 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/data/datamodules/readme.md
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.957840 dlk-0.0.8/dlk/data/postprocessors/
--rw-r--r--   0 sun       (1000) sun       (1000)     9461 2022-03-22 12:56:04.000000 dlk-0.0.8/dlk/data/postprocessors/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1619 2021-12-21 17:45:43.000000 dlk-0.0.8/dlk/data/postprocessors/identity.py
--rw-r--r--   0 sun       (1000) sun       (1000)    34482 2022-03-22 12:56:04.000000 dlk-0.0.8/dlk/data/postprocessors/seq_lab.py
--rw-r--r--   0 sun       (1000) sun       (1000)    18650 2022-03-22 12:56:04.000000 dlk-0.0.8/dlk/data/postprocessors/span_cls.py
--rw-r--r--   0 sun       (1000) sun       (1000)    11011 2022-03-22 12:56:04.000000 dlk-0.0.8/dlk/data/postprocessors/txt_cls.py
--rw-r--r--   0 sun       (1000) sun       (1000)     8979 2022-03-22 12:56:04.000000 dlk-0.0.8/dlk/data/postprocessors/txt_reg.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.959835 dlk-0.0.8/dlk/data/processors/
--rw-r--r--   0 sun       (1000) sun       (1000)     1976 2021-12-22 18:40:25.000000 dlk-0.0.8/dlk/data/processors/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     7983 2021-12-22 18:51:41.000000 dlk-0.0.8/dlk/data/processors/basic.py
--rw-r--r--   0 sun       (1000) sun       (1000)     6747 2021-12-23 12:36:26.000000 dlk-0.0.8/dlk/data/processors/readme.md
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.969808 dlk-0.0.8/dlk/data/subprocessors/
--rw-r--r--   0 sun       (1000) sun       (1000)     2159 2021-12-22 18:51:41.000000 dlk-0.0.8/dlk/data/subprocessors/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5381 2021-12-31 16:56:37.000000 dlk-0.0.8/dlk/data/subprocessors/basic_data_loader.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5309 2021-12-22 18:51:41.000000 dlk-0.0.8/dlk/data/subprocessors/char_gather.py
--rw-r--r--   0 sun       (1000) sun       (1000)    12655 2021-12-22 18:51:41.000000 dlk-0.0.8/dlk/data/subprocessors/fast_tokenizer.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3025 2021-12-22 18:51:41.000000 dlk-0.0.8/dlk/data/subprocessors/load.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3913 2021-12-22 18:51:41.000000 dlk-0.0.8/dlk/data/subprocessors/save.py
--rw-r--r--   0 sun       (1000) sun       (1000)    12051 2022-01-12 12:59:43.000000 dlk-0.0.8/dlk/data/subprocessors/seq_lab_firstpiece_relable.py
--rw-r--r--   0 sun       (1000) sun       (1000)    10420 2022-01-12 12:59:43.000000 dlk-0.0.8/dlk/data/subprocessors/seq_lab_relabel.py
--rw-r--r--   0 sun       (1000) sun       (1000)    10159 2022-01-12 12:59:43.000000 dlk-0.0.8/dlk/data/subprocessors/span_cls_relabel.py
--rw-r--r--   0 sun       (1000) sun       (1000)     5041 2021-12-22 18:51:42.000000 dlk-0.0.8/dlk/data/subprocessors/token2charid.py
--rw-r--r--   0 sun       (1000) sun       (1000)     4209 2021-12-22 18:51:42.000000 dlk-0.0.8/dlk/data/subprocessors/token2id.py
--rw-r--r--   0 sun       (1000) sun       (1000)     7709 2021-12-22 18:51:42.000000 dlk-0.0.8/dlk/data/subprocessors/token_embedding.py
--rw-r--r--   0 sun       (1000) sun       (1000)     6887 2022-01-09 16:52:56.000000 dlk-0.0.8/dlk/data/subprocessors/token_gather.py
--rw-r--r--   0 sun       (1000) sun       (1000)     8670 2021-12-31 16:56:37.000000 dlk-0.0.8/dlk/data/subprocessors/token_norm.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3580 2021-12-17 16:45:41.000000 dlk-0.0.8/dlk/dlk.drawio
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.970806 dlk-0.0.8/dlk/managers/
--rw-r--r--   0 sun       (1000) sun       (1000)     1446 2021-12-21 17:45:54.000000 dlk-0.0.8/dlk/managers/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)    11092 2021-12-22 18:40:48.000000 dlk-0.0.8/dlk/managers/lightning.py
--rw-r--r--   0 sun       (1000) sun       (1000)      635 2021-12-21 17:45:55.000000 dlk-0.0.8/dlk/online.py
--rw-r--r--   0 sun       (1000) sun       (1000)     6631 2022-01-13 14:00:54.000000 dlk-0.0.8/dlk/predict.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1865 2022-01-12 12:59:43.000000 dlk-0.0.8/dlk/process.py
--rw-r--r--   0 sun       (1000) sun       (1000)     6593 2021-12-18 21:28:01.000000 dlk-0.0.8/dlk/readme.md
--rw-r--r--   0 sun       (1000) sun       (1000)     6974 2021-12-31 14:50:29.000000 dlk-0.0.8/dlk/train.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.977787 dlk-0.0.8/dlk/utils/
--rw-r--r--   0 sun       (1000) sun       (1000)      596 2021-12-21 17:45:57.000000 dlk-0.0.8/dlk/utils/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     7812 2022-02-08 13:48:24.000000 dlk-0.0.8/dlk/utils/config.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1400 2021-12-22 18:45:49.000000 dlk-0.0.8/dlk/utils/get_root.py
--rw-r--r--   0 sun       (1000) sun       (1000)     4263 2021-12-22 18:45:49.000000 dlk-0.0.8/dlk/utils/logger.py
--rw-r--r--   0 sun       (1000) sun       (1000)    28010 2022-01-08 09:28:18.000000 dlk-0.0.8/dlk/utils/parser.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3012 2022-01-08 09:28:18.000000 dlk-0.0.8/dlk/utils/quick_search.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2197 2021-12-22 18:45:49.000000 dlk-0.0.8/dlk/utils/register.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3195 2022-01-08 15:40:43.000000 dlk-0.0.8/dlk/utils/tokenizer_util.py
--rw-r--r--   0 sun       (1000) sun       (1000)     6500 2021-12-22 18:45:49.000000 dlk-0.0.8/dlk/utils/vocab.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.839514 dlk-0.0.8/dlk.egg-info/
--rw-r--r--   0 sun       (1000) sun       (1000)     1827 2022-03-22 13:01:19.000000 dlk-0.0.8/dlk.egg-info/PKG-INFO
--rw-r--r--   0 sun       (1000) sun       (1000)    12263 2022-03-22 13:01:19.000000 dlk-0.0.8/dlk.egg-info/SOURCES.txt
--rw-r--r--   0 sun       (1000) sun       (1000)        1 2022-03-22 13:01:19.000000 dlk-0.0.8/dlk.egg-info/dependency_links.txt
--rw-r--r--   0 sun       (1000) sun       (1000)      328 2022-03-22 13:01:19.000000 dlk-0.0.8/dlk.egg-info/requires.txt
--rw-r--r--   0 sun       (1000) sun       (1000)        4 2022-03-22 13:01:19.000000 dlk-0.0.8/dlk.egg-info/top_level.txt
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.979781 dlk-0.0.8/docs/
--rw-r--r--   0 sun       (1000) sun       (1000)      638 2021-12-23 13:05:09.000000 dlk-0.0.8/docs/Makefile
--rw-r--r--   0 sun       (1000) sun       (1000)      799 2021-12-23 13:05:09.000000 dlk-0.0.8/docs/make.bat
--rw-r--r--   0 sun       (1000) sun       (1000)     3686 2021-12-23 12:36:26.000000 dlk-0.0.8/docs/readme.md
--rw-r--r--   0 sun       (1000) sun       (1000)       74 2021-12-23 13:47:14.000000 dlk-0.0.8/docs/requirements.txt
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.997733 dlk-0.0.8/docs/source/
--rw-r--r--   0 sun       (1000) sun       (1000)     6593 2021-12-18 21:28:01.000000 dlk-0.0.8/docs/source/appointment.md
--rw-r--r--   0 sun       (1000) sun       (1000)     2830 2021-12-23 14:08:37.000000 dlk-0.0.8/docs/source/conf.py
--rw-r--r--   0 sun       (1000) sun       (1000)      922 2021-12-23 13:52:10.000000 dlk-0.0.8/docs/source/dlk.core.callbacks.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      510 2021-12-23 13:52:10.000000 dlk-0.0.8/docs/source/dlk.core.imodels.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      756 2021-12-23 13:52:10.000000 dlk-0.0.8/docs/source/dlk.core.initmethods.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      784 2021-12-23 13:52:10.000000 dlk-0.0.8/docs/source/dlk.core.layers.decoders.rst
--rw-r--r--   0 sun       (1000) sun       (1000)     1493 2021-12-23 13:52:10.000000 dlk-0.0.8/docs/source/dlk.core.layers.embeddings.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      764 2021-12-23 13:52:10.000000 dlk-0.0.8/docs/source/dlk.core.layers.encoders.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      310 2021-12-23 13:52:10.000000 dlk-0.0.8/docs/source/dlk.core.layers.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      991 2021-12-23 13:52:10.000000 dlk-0.0.8/docs/source/dlk.core.losses.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      343 2021-12-23 13:52:10.000000 dlk-0.0.8/docs/source/dlk.core.models.rst
--rw-r--r--   0 sun       (1000) sun       (1000)     1480 2021-12-23 13:52:10.000000 dlk-0.0.8/docs/source/dlk.core.modules.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      525 2021-12-23 13:52:10.000000 dlk-0.0.8/docs/source/dlk.core.optimizers.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      566 2021-12-23 13:52:10.000000 dlk-0.0.8/docs/source/dlk.core.rst
--rw-r--r--   0 sun       (1000) sun       (1000)     1343 2021-12-23 13:52:10.000000 dlk-0.0.8/docs/source/dlk.core.schedulers.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      373 2021-12-23 13:52:10.000000 dlk-0.0.8/docs/source/dlk.data.datamodules.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      952 2021-12-23 13:52:10.000000 dlk-0.0.8/docs/source/dlk.data.postprocessors.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      367 2021-12-23 13:52:10.000000 dlk-0.0.8/docs/source/dlk.data.processors.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      303 2021-12-23 13:52:10.000000 dlk-0.0.8/docs/source/dlk.data.rst
--rw-r--r--   0 sun       (1000) sun       (1000)     2975 2021-12-23 13:52:10.000000 dlk-0.0.8/docs/source/dlk.data.subprocessors.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      337 2021-12-23 13:52:10.000000 dlk-0.0.8/docs/source/dlk.managers.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      743 2021-12-23 13:52:10.000000 dlk-0.0.8/docs/source/dlk.rst
--rw-r--r--   0 sun       (1000) sun       (1000)     1326 2021-12-23 13:52:10.000000 dlk-0.0.8/docs/source/dlk.utils.rst
--rw-r--r--   0 sun       (1000) sun       (1000)      769 2021-12-23 13:08:24.000000 dlk-0.0.8/docs/source/index.rst
--rw-r--r--   0 sun       (1000) sun       (1000)     1516 2021-12-23 15:27:28.000000 dlk-0.0.8/docs/source/introduction.md
--rw-r--r--   0 sun       (1000) sun       (1000)     6747 2021-12-23 12:36:26.000000 dlk-0.0.8/docs/source/process_progress.md
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.811590 dlk-0.0.8/examples/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.809595 dlk-0.0.8/examples/sequence_labeling/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.999728 dlk-0.0.8/examples/sequence_labeling/conll2003/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:20.000725 dlk-0.0.8/examples/sequence_labeling/conll2003/bert_firstpiece_lstm_crf/
--rw-r--r--   0 sun       (1000) sun       (1000)     5357 2022-01-08 15:40:43.000000 dlk-0.0.8/examples/sequence_labeling/conll2003/bert_firstpiece_lstm_crf/main.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1594 2022-01-10 14:59:38.000000 dlk-0.0.8/examples/sequence_labeling/conll2003/bert_firstpiece_lstm_crf/prepro.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:20.003718 dlk-0.0.8/examples/sequence_labeling/conll2003/norm_char_lstm_crf/
--rw-r--r--   0 sun       (1000) sun       (1000)     4679 2022-02-08 13:48:24.000000 dlk-0.0.8/examples/sequence_labeling/conll2003/norm_char_lstm_crf/main.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2113 2021-12-18 07:18:07.000000 dlk-0.0.8/examples/sequence_labeling/conll2003/norm_char_lstm_crf/pre_prepro.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1151 2022-01-10 14:59:38.000000 dlk-0.0.8/examples/sequence_labeling/conll2003/norm_char_lstm_crf/prepro.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1669 2021-12-31 17:11:38.000000 dlk-0.0.8/examples/sequence_labeling/conll2003/process.py
--rw-r--r--   0 sun       (1000) sun       (1000)      391 2021-12-13 15:15:43.000000 dlk-0.0.8/examples/sequence_labeling/conll2003/readme.md
--rw-r--r--   0 sun       (1000) sun       (1000)      922 2022-01-10 14:59:38.000000 dlk-0.0.8/examples/sequence_labeling/conll2003/train.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:20.005712 dlk-0.0.8/examples/sequence_labeling/conll2003/utils/
--rw-r--r--   0 sun       (1000) sun       (1000)     2708 2021-12-22 15:37:11.000000 dlk-0.0.8/examples/sequence_labeling/conll2003/utils/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3491 2021-12-22 15:37:11.000000 dlk-0.0.8/examples/sequence_labeling/conll2003/utils/cls_bio2json.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2728 2021-12-22 15:37:11.000000 dlk-0.0.8/examples/sequence_labeling/conll2003/utils/cls_json2bio.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1172 2021-12-22 15:37:11.000000 dlk-0.0.8/examples/sequence_labeling/conll2003/utils/get_vocab.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.810592 dlk-0.0.8/examples/text_cls/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:20.007707 dlk-0.0.8/examples/text_cls/sst2/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:20.009701 dlk-0.0.8/examples/text_cls/sst2/distil_bert/
--rw-r--r--   0 sun       (1000) sun       (1000)     2467 2022-02-08 13:48:24.000000 dlk-0.0.8/examples/text_cls/sst2/distil_bert/main.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      622 2022-01-10 14:59:38.000000 dlk-0.0.8/examples/text_cls/sst2/distil_bert/prepro.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1527 2021-12-21 17:48:43.000000 dlk-0.0.8/examples/text_cls/sst2/process.py
--rw-r--r--   0 sun       (1000) sun       (1000)       59 2021-12-18 16:17:29.000000 dlk-0.0.8/examples/text_cls/sst2/readme.md
--rw-r--r--   0 sun       (1000) sun       (1000)      963 2021-12-21 17:48:43.000000 dlk-0.0.8/examples/text_cls/sst2/train.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.810592 dlk-0.0.8/examples/text_match/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:20.011696 dlk-0.0.8/examples/text_match/snli/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:20.012694 dlk-0.0.8/examples/text_match/snli/distil_bert/
--rw-r--r--   0 sun       (1000) sun       (1000)     2636 2022-02-08 13:48:24.000000 dlk-0.0.8/examples/text_match/snli/distil_bert/main.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      796 2022-01-10 14:59:38.000000 dlk-0.0.8/examples/text_match/snli/distil_bert/prepro.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1718 2021-12-31 14:50:29.000000 dlk-0.0.8/examples/text_match/snli/process.py
--rw-r--r--   0 sun       (1000) sun       (1000)       63 2021-12-18 15:35:09.000000 dlk-0.0.8/examples/text_match/snli/readme.md
--rw-r--r--   0 sun       (1000) sun       (1000)      963 2021-12-21 17:48:45.000000 dlk-0.0.8/examples/text_match/snli/train.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:19.811590 dlk-0.0.8/examples/text_reg/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:20.014688 dlk-0.0.8/examples/text_reg/sst2/
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:20.015685 dlk-0.0.8/examples/text_reg/sst2/distil_bert/
--rw-r--r--   0 sun       (1000) sun       (1000)     2497 2022-02-08 13:48:24.000000 dlk-0.0.8/examples/text_reg/sst2/distil_bert/main.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)      622 2022-01-10 14:59:38.000000 dlk-0.0.8/examples/text_reg/sst2/distil_bert/prepro.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1482 2021-12-21 17:48:46.000000 dlk-0.0.8/examples/text_reg/sst2/process.py
--rw-r--r--   0 sun       (1000) sun       (1000)       67 2021-12-20 12:35:51.000000 dlk-0.0.8/examples/text_reg/sst2/readme.md
--rw-r--r--   0 sun       (1000) sun       (1000)      963 2021-12-21 17:48:46.000000 dlk-0.0.8/examples/text_reg/sst2/train.py
--rw-r--r--   0 sun       (1000) sun       (1000)      430 2022-01-12 12:59:43.000000 dlk-0.0.8/requirements-f.txt
--rw-r--r--   0 sun       (1000) sun       (1000)      329 2022-01-12 12:59:43.000000 dlk-0.0.8/requirements.txt
--rw-r--r--   0 sun       (1000) sun       (1000)       38 2022-03-22 13:01:20.036630 dlk-0.0.8/setup.cfg
--rw-r--r--   0 sun       (1000) sun       (1000)     1712 2021-12-23 14:10:36.000000 dlk-0.0.8/setup.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2112 2022-02-08 13:48:24.000000 dlk-0.0.8/test_predict.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1218 2021-12-21 17:48:14.000000 dlk-0.0.8/test_process.py
--rw-r--r--   0 sun       (1000) sun       (1000)      871 2021-12-21 17:48:16.000000 dlk-0.0.8/test_train.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:20.017680 dlk-0.0.8/tests/
--rw-r--r--   0 sun       (1000) sun       (1000)        0 2021-09-16 13:28:15.000000 dlk-0.0.8/tests/__init__.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:20.020672 dlk-0.0.8/tests/parser/
--rw-r--r--   0 sun       (1000) sun       (1000)        0 2021-11-01 16:26:30.000000 dlk-0.0.8/tests/parser/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     2168 2021-11-07 08:29:13.000000 dlk-0.0.8/tests/parser/test_base.json
--rw-r--r--   0 sun       (1000) sun       (1000)     2173 2021-12-17 16:45:41.000000 dlk-0.0.8/tests/parser/test_base.py
--rw-r--r--   0 sun       (1000) sun       (1000)      515 2021-12-16 13:42:00.000000 dlk-0.0.8/tests/parser/test_base_inp.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2057 2021-11-02 22:00:17.000000 dlk-0.0.8/tests/parser/test_base_out.hjson
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:20.024662 dlk-0.0.8/tests/processors/
--rw-r--r--   0 sun       (1000) sun       (1000)        0 2021-10-28 17:13:32.000000 dlk-0.0.8/tests/processors/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)    40746 2021-10-11 11:48:46.000000 dlk-0.0.8/tests/processors/bpe_token.json
--rw-r--r--   0 sun       (1000) sun       (1000)     4888 2021-12-16 13:42:00.000000 dlk-0.0.8/tests/processors/process.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     1947 2021-12-17 16:45:41.000000 dlk-0.0.8/tests/processors/test_wordpiece_tokenizer.py
--rw-r--r--   0 sun       (1000) sun       (1000)    18702 2021-10-11 11:48:46.000000 dlk-0.0.8/tests/processors/uni_token.json
--rw-r--r--   0 sun       (1000) sun       (1000)    23944 2021-10-11 11:48:46.000000 dlk-0.0.8/tests/processors/wp_token.json
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:20.025659 dlk-0.0.8/tests/test_test/
--rw-r--r--   0 sun       (1000) sun       (1000)    14948 2021-12-16 13:42:00.000000 dlk-0.0.8/tests/test_test/lightning.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:20.027654 dlk-0.0.8/tests/test_test/trace/
--rw-r--r--   0 sun       (1000) sun       (1000)        0 2021-10-31 15:02:48.000000 dlk-0.0.8/tests/test_test/trace/__init__.py
--rw-r--r--   0 sun       (1000) sun       (1000)     3249 2021-12-17 16:45:41.000000 dlk-0.0.8/tests/test_test/trace/dict_trace.py
--rw-r--r--   0 sun       (1000) sun       (1000)      605 2021-12-16 13:42:00.000000 dlk-0.0.8/tests/test_test/trace/simple_trace.py
--rw-r--r--   0 sun       (1000) sun       (1000)      304 2021-12-17 16:45:41.000000 dlk-0.0.8/tests/test_vocab.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:20.028650 dlk-0.0.8/tools/
--rw-r--r--   0 sun       (1000) sun       (1000)     1936 2021-12-22 19:11:14.000000 dlk-0.0.8/tools/conf.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:20.031643 dlk-0.0.8/tools/convert_tokenizer/
--rw-r--r--   0 sun       (1000) sun       (1000)      151 2021-12-22 15:37:11.000000 dlk-0.0.8/tools/convert_tokenizer/convert.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2063 2021-12-22 15:37:11.000000 dlk-0.0.8/tools/convert_tokenizer/convert.py
--rw-r--r--   0 sun       (1000) sun       (1000)      230 2021-12-31 16:56:37.000000 dlk-0.0.8/tools/convert_tokenizer/vocab2tokenizer.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     6274 2021-12-21 17:47:44.000000 dlk-0.0.8/tools/convert_tokenizer/vocab2tokenizer.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:20.032640 dlk-0.0.8/tools/tokenize/
--rw-r--r--   0 sun       (1000) sun       (1000)     1882 2021-12-16 13:42:00.000000 dlk-0.0.8/tools/tokenize/tokenizer.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     2406 2021-12-21 17:47:45.000000 dlk-0.0.8/tools/tokenize/tokenizer.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:20.033637 dlk-0.0.8/tools/train_tokenizer/
--rw-r--r--   0 sun       (1000) sun       (1000)      606 2021-12-16 13:42:00.000000 dlk-0.0.8/tools/train_tokenizer/train_tokenizer.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     5276 2021-12-21 17:47:46.000000 dlk-0.0.8/tools/train_tokenizer/train_tokenizer.py
--rw-r--r--   0 sun       (1000) sun       (1000)     1160 2021-12-21 17:47:47.000000 dlk-0.0.8/tools/view_config.py
-drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-22 13:01:20.035632 dlk-0.0.8/tools/word2vec/
--rw-r--r--   0 sun       (1000) sun       (1000)     1861 2021-12-31 16:56:37.000000 dlk-0.0.8/tools/word2vec/word2vec.hjson
--rw-r--r--   0 sun       (1000) sun       (1000)     6096 2021-12-31 16:56:37.000000 dlk-0.0.8/tools/word2vec/word2vec.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.262345 dlk-0.0.9/
+-rw-r--r--   0 sun       (1000) sun       (1000)      351 2021-12-23 12:39:24.000000 dlk-0.0.9/.gitignore
+-rw-r--r--   0 sun       (1000) sun       (1000)      753 2021-12-23 14:24:24.000000 dlk-0.0.9/.readthedocs.yaml
+-rw-r--r--   0 sun       (1000) sun       (1000)    11382 2021-12-17 16:45:41.000000 dlk-0.0.9/LICENSE
+-rw-r--r--   0 sun       (1000) sun       (1000)     1827 2022-03-23 18:09:00.262345 dlk-0.0.9/PKG-INFO
+-rw-r--r--   0 sun       (1000) sun       (1000)     1516 2021-12-23 15:27:28.000000 dlk-0.0.9/README.md
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.061312 dlk-0.0.9/dlk/
+-rw-r--r--   0 sun       (1000) sun       (1000)      617 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/__init__.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.041365 dlk-0.0.9/dlk/configures/
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.039370 dlk-0.0.9/dlk/configures/core/
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.074277 dlk-0.0.9/dlk/configures/core/callbacks/
+-rw-r--r--   0 sun       (1000) sun       (1000)      858 2021-12-17 18:19:33.000000 dlk-0.0.9/dlk/configures/core/callbacks/checkpoint.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      187 2021-12-17 18:19:16.000000 dlk-0.0.9/dlk/configures/core/callbacks/checkpoint@train_loss.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      214 2021-12-17 18:19:02.000000 dlk-0.0.9/dlk/configures/core/callbacks/checkpoint@val_loss.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      560 2021-12-17 18:30:29.000000 dlk-0.0.9/dlk/configures/core/callbacks/early_stop.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      260 2021-12-17 18:33:03.000000 dlk-0.0.9/dlk/configures/core/callbacks/lr_monitor.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      122 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/callbacks/progressbar.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      610 2021-12-17 18:37:22.000000 dlk-0.0.9/dlk/configures/core/callbacks/weight_average.hjson
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.079264 dlk-0.0.9/dlk/configures/core/imodels/
+-rw-r--r--   0 sun       (1000) sun       (1000)      263 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/imodels/basic.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      358 2021-12-22 15:37:11.000000 dlk-0.0.9/dlk/configures/core/imodels/basic@seq_lab#crf.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      309 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/imodels/basic@seq_lab.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      309 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/imodels/basic@span_cls.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      309 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/imodels/basic@txt_cls.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      513 2021-12-20 14:37:30.000000 dlk-0.0.9/dlk/configures/core/imodels/basic@txt_log_reg.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      513 2021-12-20 14:37:40.000000 dlk-0.0.9/dlk/configures/core/imodels/basic@txt_reg.hjson
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.081258 dlk-0.0.9/dlk/configures/core/initmethods/
+-rw-r--r--   0 sun       (1000) sun       (1000)       50 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/initmethods/default.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)       75 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/initmethods/range_norm.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)       78 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/initmethods/range_uniform.hjson
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.039370 dlk-0.0.9/dlk/configures/core/layers/
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.084251 dlk-0.0.9/dlk/configures/core/layers/decoders/
+-rw-r--r--   0 sun       (1000) sun       (1000)      526 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/decoders/biaffine.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      132 2021-12-19 09:24:47.000000 dlk-0.0.9/dlk/configures/core/layers/decoders/identity.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      473 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/decoders/linear.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      680 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/decoders/linear_crf.hjson
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.088240 dlk-0.0.9/dlk/configures/core/layers/embeddings/
+-rw-r--r--   0 sun       (1000) sun       (1000)     2666 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/embeddings/combine_word_char_cnn.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      103 2021-12-17 18:45:52.000000 dlk-0.0.9/dlk/configures/core/layers/embeddings/identity.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      601 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/embeddings/pretrained_transformers.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      643 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/embeddings/pretrained_transformers@gather.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      240 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/embeddings/random.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      779 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/embeddings/static.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     1282 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/embeddings/static_char_cnn.hjson
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.090235 dlk-0.0.9/dlk/configures/core/layers/encoders/
+-rw-r--r--   0 sun       (1000) sun       (1000)      132 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/layers/encoders/identity.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      444 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/encoders/linear.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      478 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/layers/encoders/lstm.hjson
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.093226 dlk-0.0.9/dlk/configures/core/losses/
+-rw-r--r--   0 sun       (1000) sun       (1000)      441 2021-12-20 13:50:20.000000 dlk-0.0.9/dlk/configures/core/losses/bce.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      469 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/losses/cross_entropy.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      597 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/losses/cross_entropy@cls.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      286 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/losses/identity.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      413 2021-12-18 21:32:23.000000 dlk-0.0.9/dlk/configures/core/losses/mse.hjson
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.100208 dlk-0.0.9/dlk/configures/core/models/
+-rw-r--r--   0 sun       (1000) sun       (1000)     3457 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/models/basic@seq_lab#lstm_cnn_crf.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     2139 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/models/basic@seq_lab#lstm_crf.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     2190 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/models/basic@seq_lab#lstm_linear.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     1277 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/models/basic@seq_lab#pretrained_transformers.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     1226 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/models/basic@seq_lab#pretrained_transformers_crf.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     1461 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/models/basic@seq_lab#pretrained_transformers_lstm_crf.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     1186 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/models/basic@span_cls#pretrained_transformer.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     2145 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/models/basic@txt_cls#lstm_linear.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     1143 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/models/basic@txt_cls#pretrained_transformers.hjson
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.105194 dlk-0.0.9/dlk/configures/core/modules/
+-rw-r--r--   0 sun       (1000) sun       (1000)      168 2021-12-20 14:27:27.000000 dlk-0.0.9/dlk/configures/core/modules/bert.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      215 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/core/modules/biaffine.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      200 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/modules/conv1d.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      158 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/modules/crf.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      175 2021-12-20 14:27:31.000000 dlk-0.0.9/dlk/configures/core/modules/distil_bert.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      177 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/modules/linear.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      315 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/modules/lstm.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      171 2021-12-20 14:27:35.000000 dlk-0.0.9/dlk/configures/core/modules/roberta.hjson
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.107189 dlk-0.0.9/dlk/configures/core/optimizers/
+-rw-r--r--   0 sun       (1000) sun       (1000)      798 2021-12-22 15:37:11.000000 dlk-0.0.9/dlk/configures/core/optimizers/adamw.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      538 2021-12-22 15:37:11.000000 dlk-0.0.9/dlk/configures/core/optimizers/adamw@bias_nodecay.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      816 2021-12-22 15:37:11.000000 dlk-0.0.9/dlk/configures/core/optimizers/sgd.hjson
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.110181 dlk-0.0.9/dlk/configures/core/schedulers/
+-rw-r--r--   0 sun       (1000) sun       (1000)       77 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/schedulers/constant.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      116 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/schedulers/constant_warmup.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      175 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/schedulers/cosine_warmup.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      150 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/schedulers/linear_warmup.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      172 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/core/schedulers/rec_decay.hjson
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.040368 dlk-0.0.9/dlk/configures/data/
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.115167 dlk-0.0.9/dlk/configures/data/datamodules/
+-rw-r--r--   0 sun       (1000) sun       (1000)      883 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/data/datamodules/basic.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      914 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/data/datamodules/basic@seq_lab#with_char.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      960 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/data/datamodules/basic@seq_lab#wordmask.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      881 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/data/datamodules/basic@seq_lab.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      967 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/data/datamodules/basic@span_cls.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      842 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/data/datamodules/basic@txt_cls.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      810 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/data/datamodules/basic@txt_reg.hjson
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.118159 dlk-0.0.9/dlk/configures/data/postprocessors/
+-rw-r--r--   0 sun       (1000) sun       (1000)       28 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/data/postprocessors/identity.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     1651 2022-01-08 15:40:43.000000 dlk-0.0.9/dlk/configures/data/postprocessors/seq_lab.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     1458 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/data/postprocessors/span_cls.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      866 2021-12-23 13:03:12.000000 dlk-0.0.9/dlk/configures/data/postprocessors/txt_cls.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      769 2021-12-22 15:37:11.000000 dlk-0.0.9/dlk/configures/data/postprocessors/txt_reg.hjson
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.125141 dlk-0.0.9/dlk/configures/data/processors/
+-rw-r--r--   0 sun       (1000) sun       (1000)     5707 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/data/processors/basic@seq_lab#norm_static.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     7108 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/data/processors/basic@seq_lab#norm_static_word_char.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     3944 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/data/processors/basic@seq_lab#pretrained.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     5112 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/data/processors/basic@seq_lab#static.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     3413 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/data/processors/basic@span_cls#pretrained.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     3365 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/data/processors/basic@txt_cls#pretrained.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     4468 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/data/processors/basic@txt_cls.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     2690 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/data/processors/basic@txt_match#pretrained.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     1628 2021-12-31 16:56:37.000000 dlk-0.0.9/dlk/configures/data/processors/basic@txt_match_reg#pretrained.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     2058 2021-12-31 16:56:37.000000 dlk-0.0.9/dlk/configures/data/processors/basic@txt_reg#pretrained.hjson
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.137109 dlk-0.0.9/dlk/configures/data/subprocessors/
+-rw-r--r--   0 sun       (1000) sun       (1000)      838 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/configures/data/subprocessors/basic_data_loader@seq_lab.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      889 2022-03-23 18:07:30.000000 dlk-0.0.9/dlk/configures/data/subprocessors/basic_data_loader@txt_cls.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      986 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/data/subprocessors/basic_data_loader@txt_cls_pair.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      890 2022-03-23 18:07:43.000000 dlk-0.0.9/dlk/configures/data/subprocessors/basic_data_loader@txt_reg.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      987 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/data/subprocessors/basic_data_loader@txt_reg_pair.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      796 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/data/subprocessors/char_gather.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     2876 2021-12-31 16:56:37.000000 dlk-0.0.9/dlk/configures/data/subprocessors/fast_tokenizer.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     2777 2021-12-20 15:46:38.000000 dlk-0.0.9/dlk/configures/data/subprocessors/fast_tokenizer@pair.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      164 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/data/subprocessors/load.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      119 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/data/subprocessors/save.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     1376 2022-01-12 12:59:43.000000 dlk-0.0.9/dlk/configures/data/subprocessors/seq_lab_firstpiece_relabel.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     1229 2022-01-12 12:59:43.000000 dlk-0.0.9/dlk/configures/data/subprocessors/seq_lab_relabel.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     1245 2022-01-12 12:59:43.000000 dlk-0.0.9/dlk/configures/data/subprocessors/span_cls_relabel.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      759 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/data/subprocessors/token2charid.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      690 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/data/subprocessors/token2id.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      639 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/data/subprocessors/token_embedding.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      878 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/data/subprocessors/token_gather.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      920 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/configures/data/subprocessors/token_norm.hjson
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.138106 dlk-0.0.9/dlk/configures/managers/
+-rw-r--r--   0 sun       (1000) sun       (1000)     2123 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/managers/lightning.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     2785 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/configures/managers/lightning@advance.hjson
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.139104 dlk-0.0.9/dlk/configures/tasks/
+-rw-r--r--   0 sun       (1000) sun       (1000)      441 2021-12-18 17:41:20.000000 dlk-0.0.9/dlk/configures/tasks/test_base.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     1915 2021-12-18 17:41:14.000000 dlk-0.0.9/dlk/configures/tasks/test_base_search.hjson
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.141098 dlk-0.0.9/dlk/core/
+-rw-r--r--   0 sun       (1000) sun       (1000)     1334 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/core/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     9951 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/core/base_module.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.144090 dlk-0.0.9/dlk/core/callbacks/
+-rw-r--r--   0 sun       (1000) sun       (1000)     1447 2021-12-21 17:45:09.000000 dlk-0.0.9/dlk/core/callbacks/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3243 2021-12-23 14:42:18.000000 dlk-0.0.9/dlk/core/callbacks/checkpoint.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     2780 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/callbacks/early_stop.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     2011 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/callbacks/lr_monitor.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     2746 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/callbacks/weight_average.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.146084 dlk-0.0.9/dlk/core/imodels/
+-rw-r--r--   0 sun       (1000) sun       (1000)     3493 2021-12-23 12:36:26.000000 dlk-0.0.9/dlk/core/imodels/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)    13363 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/core/imodels/basic.py
+-rw-r--r--   0 sun       (1000) sun       (1000)      672 2021-12-21 17:45:18.000000 dlk-0.0.9/dlk/core/imodels/distill.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.149077 dlk-0.0.9/dlk/core/initmethods/
+-rw-r--r--   0 sun       (1000) sun       (1000)     1500 2021-12-21 17:45:19.000000 dlk-0.0.9/dlk/core/initmethods/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     5290 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/initmethods/default.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     2413 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/initmethods/range_norm.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     2837 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/initmethods/range_uniform.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.149077 dlk-0.0.9/dlk/core/layers/
+-rw-r--r--   0 sun       (1000) sun       (1000)      838 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/core/layers/__init__.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.153066 dlk-0.0.9/dlk/core/layers/decoders/
+-rw-r--r--   0 sun       (1000) sun       (1000)     1459 2021-12-21 17:45:21.000000 dlk-0.0.9/dlk/core/layers/decoders/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3901 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/core/layers/decoders/biaffine.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     1577 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/layers/decoders/identity.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3205 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/layers/decoders/linear.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     5390 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/layers/decoders/linear_crf.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.157055 dlk-0.0.9/dlk/core/layers/embeddings/
+-rw-r--r--   0 sun       (1000) sun       (1000)     1900 2021-12-21 17:45:23.000000 dlk-0.0.9/dlk/core/layers/embeddings/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     7628 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/layers/embeddings/combine_word_char_cnn.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     1645 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/layers/embeddings/identity.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     6148 2021-12-22 18:53:49.000000 dlk-0.0.9/dlk/core/layers/embeddings/pretrained_transformers.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3412 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/layers/embeddings/random.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     4532 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/layers/embeddings/static.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     6084 2021-12-22 18:51:40.000000 dlk-0.0.9/dlk/core/layers/embeddings/static_char_cnn.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.160048 dlk-0.0.9/dlk/core/layers/encoders/
+-rw-r--r--   0 sun       (1000) sun       (1000)     1415 2021-12-21 17:45:26.000000 dlk-0.0.9/dlk/core/layers/encoders/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     1617 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/layers/encoders/identity.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3149 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/layers/encoders/linear.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3293 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/layers/encoders/lstm.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.164037 dlk-0.0.9/dlk/core/losses/
+-rw-r--r--   0 sun       (1000) sun       (1000)     1415 2021-12-21 17:45:28.000000 dlk-0.0.9/dlk/core/losses/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     5002 2021-12-22 18:58:35.000000 dlk-0.0.9/dlk/core/losses/bce.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     5572 2021-12-22 18:58:35.000000 dlk-0.0.9/dlk/core/losses/cross_entropy.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     4061 2021-12-22 19:06:58.000000 dlk-0.0.9/dlk/core/losses/identity.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     5004 2021-12-22 18:58:33.000000 dlk-0.0.9/dlk/core/losses/mse.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     4068 2021-12-22 18:58:48.000000 dlk-0.0.9/dlk/core/losses/multi_loss.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.165034 dlk-0.0.9/dlk/core/models/
+-rw-r--r--   0 sun       (1000) sun       (1000)     1419 2021-12-21 17:45:31.000000 dlk-0.0.9/dlk/core/models/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     9621 2022-03-23 13:52:15.000000 dlk-0.0.9/dlk/core/models/basic.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.172016 dlk-0.0.9/dlk/core/modules/
+-rw-r--r--   0 sun       (1000) sun       (1000)     3230 2022-03-23 13:52:15.000000 dlk-0.0.9/dlk/core/modules/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     5854 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/core/modules/bert.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3423 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/core/modules/biaffine.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     2719 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/modules/conv1d.py
+-rw-r--r--   0 sun       (1000) sun       (1000)    10299 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/core/modules/crf.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     5450 2021-12-23 12:36:26.000000 dlk-0.0.9/dlk/core/modules/distil_bert.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     2765 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/modules/linear.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3533 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/core/modules/logits_gather.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3463 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/modules/lstm.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     5885 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/modules/roberta.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.174010 dlk-0.0.9/dlk/core/optimizers/
+-rw-r--r--   0 sun       (1000) sun       (1000)     4066 2021-12-22 18:28:20.000000 dlk-0.0.9/dlk/core/optimizers/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     2869 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/optimizers/adamw.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     2918 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/optimizers/sgd.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.177999 dlk-0.0.9/dlk/core/schedulers/
+-rw-r--r--   0 sun       (1000) sun       (1000)     1881 2021-12-22 18:28:20.000000 dlk-0.0.9/dlk/core/schedulers/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     1903 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/schedulers/constant.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     2388 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/schedulers/constant_warmup.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3047 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/schedulers/cosine_warmup.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3025 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/schedulers/linear_warmup.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     2617 2021-12-21 17:45:41.000000 dlk-0.0.9/dlk/core/schedulers/multi_group_schedule.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     2966 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/core/schedulers/rec_decay.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.178997 dlk-0.0.9/dlk/data/
+-rw-r--r--   0 sun       (1000) sun       (1000)      931 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/data/__init__.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.180992 dlk-0.0.9/dlk/data/datamodules/
+-rw-r--r--   0 sun       (1000) sun       (1000)     5164 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/data/datamodules/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     8952 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/data/datamodules/basic.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     1889 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/data/datamodules/readme.md
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.185978 dlk-0.0.9/dlk/data/postprocessors/
+-rw-r--r--   0 sun       (1000) sun       (1000)     9461 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/data/postprocessors/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     1619 2021-12-21 17:45:43.000000 dlk-0.0.9/dlk/data/postprocessors/identity.py
+-rw-r--r--   0 sun       (1000) sun       (1000)    34482 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/data/postprocessors/seq_lab.py
+-rw-r--r--   0 sun       (1000) sun       (1000)    18650 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/data/postprocessors/span_cls.py
+-rw-r--r--   0 sun       (1000) sun       (1000)    11011 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/data/postprocessors/txt_cls.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     8979 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/data/postprocessors/txt_reg.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.187973 dlk-0.0.9/dlk/data/processors/
+-rw-r--r--   0 sun       (1000) sun       (1000)     1976 2021-12-22 18:40:25.000000 dlk-0.0.9/dlk/data/processors/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     7983 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/data/processors/basic.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     6747 2021-12-23 12:36:26.000000 dlk-0.0.9/dlk/data/processors/readme.md
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.196949 dlk-0.0.9/dlk/data/subprocessors/
+-rw-r--r--   0 sun       (1000) sun       (1000)     2159 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/data/subprocessors/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     5377 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/data/subprocessors/basic_data_loader.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     5309 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/data/subprocessors/char_gather.py
+-rw-r--r--   0 sun       (1000) sun       (1000)    12655 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/data/subprocessors/fast_tokenizer.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3118 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/data/subprocessors/load.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3913 2021-12-22 18:51:41.000000 dlk-0.0.9/dlk/data/subprocessors/save.py
+-rw-r--r--   0 sun       (1000) sun       (1000)    12051 2022-01-12 12:59:43.000000 dlk-0.0.9/dlk/data/subprocessors/seq_lab_firstpiece_relable.py
+-rw-r--r--   0 sun       (1000) sun       (1000)    10420 2022-01-12 12:59:43.000000 dlk-0.0.9/dlk/data/subprocessors/seq_lab_relabel.py
+-rw-r--r--   0 sun       (1000) sun       (1000)    10159 2022-01-12 12:59:43.000000 dlk-0.0.9/dlk/data/subprocessors/span_cls_relabel.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     5041 2021-12-22 18:51:42.000000 dlk-0.0.9/dlk/data/subprocessors/token2charid.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     4209 2021-12-22 18:51:42.000000 dlk-0.0.9/dlk/data/subprocessors/token2id.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     7709 2021-12-22 18:51:42.000000 dlk-0.0.9/dlk/data/subprocessors/token_embedding.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     6887 2022-01-09 16:52:56.000000 dlk-0.0.9/dlk/data/subprocessors/token_gather.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     8670 2021-12-31 16:56:37.000000 dlk-0.0.9/dlk/data/subprocessors/token_norm.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3580 2021-12-17 16:45:41.000000 dlk-0.0.9/dlk/dlk.drawio
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.198943 dlk-0.0.9/dlk/managers/
+-rw-r--r--   0 sun       (1000) sun       (1000)     1446 2021-12-21 17:45:54.000000 dlk-0.0.9/dlk/managers/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)    11092 2022-03-22 14:40:41.000000 dlk-0.0.9/dlk/managers/lightning.py
+-rw-r--r--   0 sun       (1000) sun       (1000)      635 2021-12-21 17:45:55.000000 dlk-0.0.9/dlk/online.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     6631 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/predict.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     1865 2022-01-12 12:59:43.000000 dlk-0.0.9/dlk/process.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     6593 2021-12-18 21:28:01.000000 dlk-0.0.9/dlk/readme.md
+-rw-r--r--   0 sun       (1000) sun       (1000)     6974 2021-12-31 14:50:29.000000 dlk-0.0.9/dlk/train.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.204928 dlk-0.0.9/dlk/utils/
+-rw-r--r--   0 sun       (1000) sun       (1000)      596 2021-12-21 17:45:57.000000 dlk-0.0.9/dlk/utils/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     7812 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/utils/config.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     1400 2021-12-22 18:45:49.000000 dlk-0.0.9/dlk/utils/get_root.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     4263 2021-12-22 18:45:49.000000 dlk-0.0.9/dlk/utils/logger.py
+-rw-r--r--   0 sun       (1000) sun       (1000)    29807 2022-03-23 13:51:46.000000 dlk-0.0.9/dlk/utils/parser.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3012 2022-01-08 09:28:18.000000 dlk-0.0.9/dlk/utils/quick_search.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     2197 2021-12-22 18:45:49.000000 dlk-0.0.9/dlk/utils/register.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3195 2022-01-08 15:40:43.000000 dlk-0.0.9/dlk/utils/tokenizer_util.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     6500 2021-12-22 18:45:49.000000 dlk-0.0.9/dlk/utils/vocab.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.070288 dlk-0.0.9/dlk.egg-info/
+-rw-r--r--   0 sun       (1000) sun       (1000)     1827 2022-03-23 18:08:59.000000 dlk-0.0.9/dlk.egg-info/PKG-INFO
+-rw-r--r--   0 sun       (1000) sun       (1000)    12263 2022-03-23 18:08:59.000000 dlk-0.0.9/dlk.egg-info/SOURCES.txt
+-rw-r--r--   0 sun       (1000) sun       (1000)        1 2022-03-23 18:08:59.000000 dlk-0.0.9/dlk.egg-info/dependency_links.txt
+-rw-r--r--   0 sun       (1000) sun       (1000)      328 2022-03-23 18:08:59.000000 dlk-0.0.9/dlk.egg-info/requires.txt
+-rw-r--r--   0 sun       (1000) sun       (1000)        4 2022-03-23 18:08:59.000000 dlk-0.0.9/dlk.egg-info/top_level.txt
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.207919 dlk-0.0.9/docs/
+-rw-r--r--   0 sun       (1000) sun       (1000)      638 2021-12-23 13:05:09.000000 dlk-0.0.9/docs/Makefile
+-rw-r--r--   0 sun       (1000) sun       (1000)      799 2021-12-23 13:05:09.000000 dlk-0.0.9/docs/make.bat
+-rw-r--r--   0 sun       (1000) sun       (1000)     3686 2021-12-23 12:36:26.000000 dlk-0.0.9/docs/readme.md
+-rw-r--r--   0 sun       (1000) sun       (1000)       74 2021-12-23 13:47:14.000000 dlk-0.0.9/docs/requirements.txt
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.224446 dlk-0.0.9/docs/source/
+-rw-r--r--   0 sun       (1000) sun       (1000)     6593 2021-12-18 21:28:01.000000 dlk-0.0.9/docs/source/appointment.md
+-rw-r--r--   0 sun       (1000) sun       (1000)     2830 2021-12-23 14:08:37.000000 dlk-0.0.9/docs/source/conf.py
+-rw-r--r--   0 sun       (1000) sun       (1000)      922 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.callbacks.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)      510 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.imodels.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)      756 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.initmethods.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)      784 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.layers.decoders.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)     1493 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.layers.embeddings.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)      764 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.layers.encoders.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)      310 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.layers.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)      991 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.losses.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)      343 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.models.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)     1480 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.modules.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)      525 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.optimizers.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)      566 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)     1343 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.core.schedulers.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)      373 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.data.datamodules.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)      952 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.data.postprocessors.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)      367 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.data.processors.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)      303 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.data.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)     2975 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.data.subprocessors.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)      337 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.managers.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)      743 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)     1326 2021-12-23 13:52:10.000000 dlk-0.0.9/docs/source/dlk.utils.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)      769 2021-12-23 13:08:24.000000 dlk-0.0.9/docs/source/index.rst
+-rw-r--r--   0 sun       (1000) sun       (1000)     1516 2021-12-23 15:27:28.000000 dlk-0.0.9/docs/source/introduction.md
+-rw-r--r--   0 sun       (1000) sun       (1000)     6747 2021-12-23 12:36:26.000000 dlk-0.0.9/docs/source/process_progress.md
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.048346 dlk-0.0.9/examples/
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.046352 dlk-0.0.9/examples/sequence_labeling/
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.226441 dlk-0.0.9/examples/sequence_labeling/conll2003/
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.228435 dlk-0.0.9/examples/sequence_labeling/conll2003/bert_firstpiece_lstm_crf/
+-rw-r--r--   0 sun       (1000) sun       (1000)     5357 2022-01-08 15:40:43.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/bert_firstpiece_lstm_crf/main.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     1594 2022-01-10 14:59:38.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/bert_firstpiece_lstm_crf/prepro.hjson
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.230430 dlk-0.0.9/examples/sequence_labeling/conll2003/norm_char_lstm_crf/
+-rw-r--r--   0 sun       (1000) sun       (1000)     4679 2022-03-23 13:51:46.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/norm_char_lstm_crf/main.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     2113 2021-12-18 07:18:07.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/norm_char_lstm_crf/pre_prepro.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     1151 2022-01-10 14:59:38.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/norm_char_lstm_crf/prepro.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     1669 2021-12-31 17:11:38.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/process.py
+-rw-r--r--   0 sun       (1000) sun       (1000)      391 2021-12-13 15:15:43.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/readme.md
+-rw-r--r--   0 sun       (1000) sun       (1000)      922 2022-01-10 14:59:38.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/train.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.232425 dlk-0.0.9/examples/sequence_labeling/conll2003/utils/
+-rw-r--r--   0 sun       (1000) sun       (1000)     2708 2021-12-22 15:37:11.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/utils/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3491 2021-12-22 15:37:11.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/utils/cls_bio2json.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     2728 2021-12-22 15:37:11.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/utils/cls_json2bio.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     1172 2021-12-22 15:37:11.000000 dlk-0.0.9/examples/sequence_labeling/conll2003/utils/get_vocab.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.047349 dlk-0.0.9/examples/text_cls/
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.234419 dlk-0.0.9/examples/text_cls/sst2/
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.236414 dlk-0.0.9/examples/text_cls/sst2/distil_bert/
+-rw-r--r--   0 sun       (1000) sun       (1000)     2467 2022-03-23 13:51:46.000000 dlk-0.0.9/examples/text_cls/sst2/distil_bert/main.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      622 2022-01-10 14:59:38.000000 dlk-0.0.9/examples/text_cls/sst2/distil_bert/prepro.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     1527 2021-12-21 17:48:43.000000 dlk-0.0.9/examples/text_cls/sst2/process.py
+-rw-r--r--   0 sun       (1000) sun       (1000)       59 2021-12-18 16:17:29.000000 dlk-0.0.9/examples/text_cls/sst2/readme.md
+-rw-r--r--   0 sun       (1000) sun       (1000)      963 2021-12-21 17:48:43.000000 dlk-0.0.9/examples/text_cls/sst2/train.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.047349 dlk-0.0.9/examples/text_match/
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.238409 dlk-0.0.9/examples/text_match/snli/
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.239406 dlk-0.0.9/examples/text_match/snli/distil_bert/
+-rw-r--r--   0 sun       (1000) sun       (1000)     2636 2022-03-23 13:51:46.000000 dlk-0.0.9/examples/text_match/snli/distil_bert/main.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      796 2022-01-10 14:59:38.000000 dlk-0.0.9/examples/text_match/snli/distil_bert/prepro.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     1718 2021-12-31 14:50:29.000000 dlk-0.0.9/examples/text_match/snli/process.py
+-rw-r--r--   0 sun       (1000) sun       (1000)       63 2021-12-18 15:35:09.000000 dlk-0.0.9/examples/text_match/snli/readme.md
+-rw-r--r--   0 sun       (1000) sun       (1000)      963 2021-12-21 17:48:45.000000 dlk-0.0.9/examples/text_match/snli/train.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.048346 dlk-0.0.9/examples/text_reg/
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.241401 dlk-0.0.9/examples/text_reg/sst2/
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.242398 dlk-0.0.9/examples/text_reg/sst2/distil_bert/
+-rw-r--r--   0 sun       (1000) sun       (1000)     2497 2022-03-23 13:51:46.000000 dlk-0.0.9/examples/text_reg/sst2/distil_bert/main.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)      622 2022-01-10 14:59:38.000000 dlk-0.0.9/examples/text_reg/sst2/distil_bert/prepro.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     1482 2021-12-21 17:48:46.000000 dlk-0.0.9/examples/text_reg/sst2/process.py
+-rw-r--r--   0 sun       (1000) sun       (1000)       67 2021-12-20 12:35:51.000000 dlk-0.0.9/examples/text_reg/sst2/readme.md
+-rw-r--r--   0 sun       (1000) sun       (1000)      963 2021-12-21 17:48:46.000000 dlk-0.0.9/examples/text_reg/sst2/train.py
+-rw-r--r--   0 sun       (1000) sun       (1000)      430 2022-01-12 12:59:43.000000 dlk-0.0.9/requirements-f.txt
+-rw-r--r--   0 sun       (1000) sun       (1000)      329 2022-01-12 12:59:43.000000 dlk-0.0.9/requirements.txt
+-rw-r--r--   0 sun       (1000) sun       (1000)       38 2022-03-23 18:09:00.262345 dlk-0.0.9/setup.cfg
+-rw-r--r--   0 sun       (1000) sun       (1000)     1712 2021-12-23 14:10:36.000000 dlk-0.0.9/setup.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     2112 2022-03-23 13:51:46.000000 dlk-0.0.9/test_predict.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     1218 2021-12-21 17:48:14.000000 dlk-0.0.9/test_process.py
+-rw-r--r--   0 sun       (1000) sun       (1000)      871 2021-12-21 17:48:16.000000 dlk-0.0.9/test_train.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.243395 dlk-0.0.9/tests/
+-rw-r--r--   0 sun       (1000) sun       (1000)        0 2021-09-16 13:28:15.000000 dlk-0.0.9/tests/__init__.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.246387 dlk-0.0.9/tests/parser/
+-rw-r--r--   0 sun       (1000) sun       (1000)        0 2021-11-01 16:26:30.000000 dlk-0.0.9/tests/parser/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     2168 2021-11-07 08:29:13.000000 dlk-0.0.9/tests/parser/test_base.json
+-rw-r--r--   0 sun       (1000) sun       (1000)     2173 2021-12-17 16:45:41.000000 dlk-0.0.9/tests/parser/test_base.py
+-rw-r--r--   0 sun       (1000) sun       (1000)      515 2021-12-16 13:42:00.000000 dlk-0.0.9/tests/parser/test_base_inp.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     2057 2021-11-02 22:00:17.000000 dlk-0.0.9/tests/parser/test_base_out.hjson
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.251374 dlk-0.0.9/tests/processors/
+-rw-r--r--   0 sun       (1000) sun       (1000)        0 2021-10-28 17:13:32.000000 dlk-0.0.9/tests/processors/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)    40746 2021-10-11 11:48:46.000000 dlk-0.0.9/tests/processors/bpe_token.json
+-rw-r--r--   0 sun       (1000) sun       (1000)     4888 2021-12-16 13:42:00.000000 dlk-0.0.9/tests/processors/process.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     1947 2021-12-17 16:45:41.000000 dlk-0.0.9/tests/processors/test_wordpiece_tokenizer.py
+-rw-r--r--   0 sun       (1000) sun       (1000)    18702 2021-10-11 11:48:46.000000 dlk-0.0.9/tests/processors/uni_token.json
+-rw-r--r--   0 sun       (1000) sun       (1000)    23944 2021-10-11 11:48:46.000000 dlk-0.0.9/tests/processors/wp_token.json
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.251374 dlk-0.0.9/tests/test_test/
+-rw-r--r--   0 sun       (1000) sun       (1000)    14948 2021-12-16 13:42:00.000000 dlk-0.0.9/tests/test_test/lightning.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.253368 dlk-0.0.9/tests/test_test/trace/
+-rw-r--r--   0 sun       (1000) sun       (1000)        0 2021-10-31 15:02:48.000000 dlk-0.0.9/tests/test_test/trace/__init__.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     3249 2021-12-17 16:45:41.000000 dlk-0.0.9/tests/test_test/trace/dict_trace.py
+-rw-r--r--   0 sun       (1000) sun       (1000)      605 2021-12-16 13:42:00.000000 dlk-0.0.9/tests/test_test/trace/simple_trace.py
+-rw-r--r--   0 sun       (1000) sun       (1000)      304 2021-12-17 16:45:41.000000 dlk-0.0.9/tests/test_vocab.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.254366 dlk-0.0.9/tools/
+-rw-r--r--   0 sun       (1000) sun       (1000)     1936 2021-12-22 19:11:14.000000 dlk-0.0.9/tools/conf.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.257358 dlk-0.0.9/tools/convert_tokenizer/
+-rw-r--r--   0 sun       (1000) sun       (1000)      151 2021-12-22 15:37:11.000000 dlk-0.0.9/tools/convert_tokenizer/convert.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     2063 2021-12-22 15:37:11.000000 dlk-0.0.9/tools/convert_tokenizer/convert.py
+-rw-r--r--   0 sun       (1000) sun       (1000)      230 2021-12-31 16:56:37.000000 dlk-0.0.9/tools/convert_tokenizer/vocab2tokenizer.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     6274 2021-12-21 17:47:44.000000 dlk-0.0.9/tools/convert_tokenizer/vocab2tokenizer.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.258355 dlk-0.0.9/tools/tokenize/
+-rw-r--r--   0 sun       (1000) sun       (1000)     1882 2021-12-16 13:42:00.000000 dlk-0.0.9/tools/tokenize/tokenizer.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     2406 2021-12-21 17:47:45.000000 dlk-0.0.9/tools/tokenize/tokenizer.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.260350 dlk-0.0.9/tools/train_tokenizer/
+-rw-r--r--   0 sun       (1000) sun       (1000)      606 2021-12-16 13:42:00.000000 dlk-0.0.9/tools/train_tokenizer/train_tokenizer.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     5276 2021-12-21 17:47:46.000000 dlk-0.0.9/tools/train_tokenizer/train_tokenizer.py
+-rw-r--r--   0 sun       (1000) sun       (1000)     1160 2021-12-21 17:47:47.000000 dlk-0.0.9/tools/view_config.py
+drwxr-xr-x   0 sun       (1000) sun       (1000)        0 2022-03-23 18:09:00.261347 dlk-0.0.9/tools/word2vec/
+-rw-r--r--   0 sun       (1000) sun       (1000)     1861 2021-12-31 16:56:37.000000 dlk-0.0.9/tools/word2vec/word2vec.hjson
+-rw-r--r--   0 sun       (1000) sun       (1000)     6096 2021-12-31 16:56:37.000000 dlk-0.0.9/tools/word2vec/word2vec.py
```

### Comparing `dlk-0.0.8/.readthedocs.yaml` & `dlk-0.0.9/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/LICENSE` & `dlk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/PKG-INFO` & `dlk-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlk
-Version: 0.0.8
+Version: 0.0.9
 Summary: dlk: Deep Learning Kit
 Home-page: https://github.com/cstsunfu/dlk
 Author: cstsunfu
 Author-email: cstsunfu@gmail.com
 License: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `dlk-0.0.8/README.md` & `dlk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/__init__.py` & `dlk-0.0.9/dlk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = 'v0.0.8'
+__version__ = 'v0.0.9'
```

### Comparing `dlk-0.0.8/dlk/configures/core/callbacks/checkpoint.hjson` & `dlk-0.0.9/dlk/configures/core/callbacks/checkpoint.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/callbacks/early_stop.hjson` & `dlk-0.0.9/dlk/configures/core/callbacks/early_stop.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/callbacks/weight_average.hjson` & `dlk-0.0.9/dlk/configures/core/callbacks/weight_average.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/imodels/basic@txt_log_reg.hjson` & `dlk-0.0.9/dlk/configures/core/imodels/basic@txt_log_reg.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/imodels/basic@txt_reg.hjson` & `dlk-0.0.9/dlk/configures/core/imodels/basic@txt_reg.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/layers/decoders/biaffine.hjson` & `dlk-0.0.9/dlk/configures/core/layers/decoders/biaffine.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/layers/decoders/linear_crf.hjson` & `dlk-0.0.9/dlk/configures/core/layers/decoders/linear_crf.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/layers/embeddings/combine_word_char_cnn.hjson` & `dlk-0.0.9/dlk/configures/core/layers/embeddings/combine_word_char_cnn.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/layers/embeddings/pretrained_transformers.hjson` & `dlk-0.0.9/dlk/configures/core/layers/embeddings/pretrained_transformers.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/layers/embeddings/pretrained_transformers@gather.hjson` & `dlk-0.0.9/dlk/configures/core/layers/embeddings/pretrained_transformers@gather.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/layers/embeddings/static.hjson` & `dlk-0.0.9/dlk/configures/core/layers/embeddings/static.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/layers/embeddings/static_char_cnn.hjson` & `dlk-0.0.9/dlk/configures/core/layers/embeddings/static_char_cnn.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/losses/cross_entropy@cls.hjson` & `dlk-0.0.9/dlk/configures/core/losses/cross_entropy@cls.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/models/basic@seq_lab#lstm_cnn_crf.hjson` & `dlk-0.0.9/dlk/configures/core/models/basic@seq_lab#lstm_cnn_crf.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/models/basic@seq_lab#lstm_crf.hjson` & `dlk-0.0.9/dlk/configures/core/models/basic@seq_lab#lstm_crf.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/models/basic@seq_lab#lstm_linear.hjson` & `dlk-0.0.9/dlk/configures/core/models/basic@seq_lab#lstm_linear.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/models/basic@seq_lab#pretrained_transformers.hjson` & `dlk-0.0.9/dlk/configures/core/models/basic@seq_lab#pretrained_transformers.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/models/basic@seq_lab#pretrained_transformers_crf.hjson` & `dlk-0.0.9/dlk/configures/core/models/basic@seq_lab#pretrained_transformers_crf.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/models/basic@seq_lab#pretrained_transformers_lstm_crf.hjson` & `dlk-0.0.9/dlk/configures/core/models/basic@seq_lab#pretrained_transformers_lstm_crf.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/models/basic@span_cls#pretrained_transformer.hjson` & `dlk-0.0.9/dlk/configures/core/models/basic@span_cls#pretrained_transformer.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/models/basic@txt_cls#lstm_linear.hjson` & `dlk-0.0.9/dlk/configures/core/models/basic@txt_cls#lstm_linear.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/models/basic@txt_cls#pretrained_transformers.hjson` & `dlk-0.0.9/dlk/configures/core/models/basic@txt_cls#pretrained_transformers.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/optimizers/adamw.hjson` & `dlk-0.0.9/dlk/configures/core/optimizers/adamw.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/optimizers/adamw@bias_nodecay.hjson` & `dlk-0.0.9/dlk/configures/core/optimizers/adamw@bias_nodecay.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/core/optimizers/sgd.hjson` & `dlk-0.0.9/dlk/configures/core/optimizers/sgd.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/datamodules/basic.hjson` & `dlk-0.0.9/dlk/configures/data/datamodules/basic.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/datamodules/basic@seq_lab#with_char.hjson` & `dlk-0.0.9/dlk/configures/data/datamodules/basic@seq_lab#with_char.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/datamodules/basic@seq_lab#wordmask.hjson` & `dlk-0.0.9/dlk/configures/data/datamodules/basic@seq_lab#wordmask.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/datamodules/basic@seq_lab.hjson` & `dlk-0.0.9/dlk/configures/data/datamodules/basic@seq_lab.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/datamodules/basic@span_cls.hjson` & `dlk-0.0.9/dlk/configures/data/datamodules/basic@span_cls.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/datamodules/basic@txt_cls.hjson` & `dlk-0.0.9/dlk/configures/data/datamodules/basic@txt_cls.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/datamodules/basic@txt_reg.hjson` & `dlk-0.0.9/dlk/configures/data/datamodules/basic@txt_reg.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/postprocessors/seq_lab.hjson` & `dlk-0.0.9/dlk/configures/data/postprocessors/seq_lab.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/postprocessors/span_cls.hjson` & `dlk-0.0.9/dlk/configures/data/postprocessors/span_cls.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/postprocessors/txt_cls.hjson` & `dlk-0.0.9/dlk/configures/data/postprocessors/txt_cls.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/postprocessors/txt_reg.hjson` & `dlk-0.0.9/dlk/configures/data/postprocessors/txt_reg.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/processors/basic@seq_lab#norm_static.hjson` & `dlk-0.0.9/dlk/configures/data/processors/basic@seq_lab#norm_static.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/processors/basic@seq_lab#norm_static_word_char.hjson` & `dlk-0.0.9/dlk/configures/data/processors/basic@seq_lab#norm_static_word_char.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/processors/basic@seq_lab#pretrained.hjson` & `dlk-0.0.9/dlk/configures/data/processors/basic@seq_lab#pretrained.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/processors/basic@seq_lab#static.hjson` & `dlk-0.0.9/dlk/configures/data/processors/basic@seq_lab#static.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/processors/basic@span_cls#pretrained.hjson` & `dlk-0.0.9/dlk/configures/data/processors/basic@span_cls#pretrained.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/processors/basic@txt_cls#pretrained.hjson` & `dlk-0.0.9/dlk/configures/data/processors/basic@txt_cls#pretrained.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/processors/basic@txt_cls.hjson` & `dlk-0.0.9/dlk/configures/data/processors/basic@txt_cls.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/processors/basic@txt_match#pretrained.hjson` & `dlk-0.0.9/dlk/configures/data/processors/basic@txt_match#pretrained.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/processors/basic@txt_match_reg#pretrained.hjson` & `dlk-0.0.9/dlk/configures/data/processors/basic@txt_match_reg#pretrained.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/processors/basic@txt_reg#pretrained.hjson` & `dlk-0.0.9/dlk/configures/data/processors/basic@txt_reg#pretrained.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/subprocessors/basic_data_loader@seq_lab.hjson` & `dlk-0.0.9/dlk/configures/data/subprocessors/basic_data_loader@seq_lab.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/subprocessors/basic_data_loader@txt_cls.hjson` & `dlk-0.0.9/dlk/configures/data/subprocessors/basic_data_loader@txt_cls.hjson`

 * *Files 17% similar despite different names*

```diff
@@ -5,23 +5,19 @@
             "data_set": {                   // for different stage, this processor will process different part of data
                 "train": ['train', 'valid', 'test', 'predict'],
                 "predict": ['predict'],
                 "online": ['online']
             },
             "input_map": {   // without necessery don't change this
                 "sentence": "sentence", //for single
-                "sentence_a": "sentence_a",  // for pair
-                "sentence_b": "sentence_b",
                 "uuid": "uuid",
                 "labels": "labels",
             },
             "output_map": {   // without necessery don't change this
                 "sentence": "sentence", //for single
-                "sentence_a": "sentence_a", //for pair
-                "sentence_b": "sentence_b",
                 "uuid": "uuid",
                 "labels": "labels",
             },
             "data_type": "single", // single or pair
         },
         "predict": "train",
         "online": "train",
```

### Comparing `dlk-0.0.8/dlk/configures/data/subprocessors/basic_data_loader@txt_cls_pair.hjson` & `dlk-0.0.9/dlk/configures/data/subprocessors/basic_data_loader@txt_cls_pair.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/subprocessors/basic_data_loader@txt_reg_pair.hjson` & `dlk-0.0.9/dlk/configures/data/subprocessors/basic_data_loader@txt_reg_pair.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/subprocessors/char_gather.hjson` & `dlk-0.0.9/dlk/configures/data/subprocessors/char_gather.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/subprocessors/fast_tokenizer.hjson` & `dlk-0.0.9/dlk/configures/data/subprocessors/fast_tokenizer.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/subprocessors/fast_tokenizer@pair.hjson` & `dlk-0.0.9/dlk/configures/data/subprocessors/fast_tokenizer@pair.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/subprocessors/seq_lab_firstpiece_relabel.hjson` & `dlk-0.0.9/dlk/configures/data/subprocessors/seq_lab_firstpiece_relabel.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/subprocessors/seq_lab_relabel.hjson` & `dlk-0.0.9/dlk/configures/data/subprocessors/seq_lab_relabel.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/subprocessors/span_cls_relabel.hjson` & `dlk-0.0.9/dlk/configures/data/subprocessors/span_cls_relabel.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/subprocessors/token2charid.hjson` & `dlk-0.0.9/dlk/configures/data/subprocessors/token2charid.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/subprocessors/token2id.hjson` & `dlk-0.0.9/dlk/configures/data/subprocessors/token2id.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/subprocessors/token_embedding.hjson` & `dlk-0.0.9/dlk/configures/data/subprocessors/token_embedding.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/subprocessors/token_gather.hjson` & `dlk-0.0.9/dlk/configures/data/subprocessors/token_gather.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/data/subprocessors/token_norm.hjson` & `dlk-0.0.9/dlk/configures/data/subprocessors/token_norm.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/managers/lightning.hjson` & `dlk-0.0.9/dlk/configures/managers/lightning.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/managers/lightning@advance.hjson` & `dlk-0.0.9/dlk/configures/managers/lightning@advance.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/configures/tasks/test_base_search.hjson` & `dlk-0.0.9/dlk/configures/tasks/test_base_search.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/__init__.py` & `dlk-0.0.9/dlk/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,7 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+
```

### Comparing `dlk-0.0.8/dlk/core/base_module.py` & `dlk-0.0.9/dlk/core/base_module.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/callbacks/__init__.py` & `dlk-0.0.9/dlk/core/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/callbacks/checkpoint.py` & `dlk-0.0.9/dlk/core/callbacks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/callbacks/early_stop.py` & `dlk-0.0.9/dlk/core/callbacks/early_stop.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/callbacks/lr_monitor.py` & `dlk-0.0.9/dlk/core/callbacks/lr_monitor.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/callbacks/weight_average.py` & `dlk-0.0.9/dlk/core/callbacks/weight_average.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/imodels/__init__.py` & `dlk-0.0.9/dlk/core/imodels/__init__.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/imodels/basic.py` & `dlk-0.0.9/dlk/core/imodels/basic.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/imodels/distill.py` & `dlk-0.0.9/dlk/core/imodels/distill.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/initmethods/__init__.py` & `dlk-0.0.9/dlk/core/initmethods/__init__.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/initmethods/default.py` & `dlk-0.0.9/dlk/core/initmethods/default.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/initmethods/range_norm.py` & `dlk-0.0.9/dlk/core/initmethods/range_norm.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/initmethods/range_uniform.py` & `dlk-0.0.9/dlk/core/initmethods/range_uniform.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/layers/__init__.py` & `dlk-0.0.9/dlk/online.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,8 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
+# for online server
+# TODO: Coming soon
```

### Comparing `dlk-0.0.8/dlk/core/layers/decoders/__init__.py` & `dlk-0.0.9/dlk/core/layers/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/layers/decoders/biaffine.py` & `dlk-0.0.9/dlk/core/layers/decoders/biaffine.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/layers/decoders/identity.py` & `dlk-0.0.9/dlk/core/layers/decoders/identity.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/layers/decoders/linear.py` & `dlk-0.0.9/dlk/core/layers/decoders/linear.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/layers/decoders/linear_crf.py` & `dlk-0.0.9/dlk/core/layers/decoders/linear_crf.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/layers/embeddings/__init__.py` & `dlk-0.0.9/dlk/core/layers/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/layers/embeddings/combine_word_char_cnn.py` & `dlk-0.0.9/dlk/core/layers/embeddings/combine_word_char_cnn.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/layers/embeddings/identity.py` & `dlk-0.0.9/dlk/core/layers/embeddings/identity.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/layers/embeddings/pretrained_transformers.py` & `dlk-0.0.9/dlk/core/layers/embeddings/pretrained_transformers.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/layers/embeddings/random.py` & `dlk-0.0.9/dlk/core/layers/embeddings/random.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/layers/embeddings/static.py` & `dlk-0.0.9/dlk/core/layers/embeddings/static.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/layers/embeddings/static_char_cnn.py` & `dlk-0.0.9/dlk/core/layers/embeddings/static_char_cnn.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/layers/encoders/__init__.py` & `dlk-0.0.9/dlk/core/layers/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/layers/encoders/identity.py` & `dlk-0.0.9/dlk/core/layers/encoders/identity.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/layers/encoders/linear.py` & `dlk-0.0.9/dlk/core/layers/encoders/linear.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/layers/encoders/lstm.py` & `dlk-0.0.9/dlk/core/layers/encoders/lstm.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/losses/__init__.py` & `dlk-0.0.9/dlk/core/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/losses/bce.py` & `dlk-0.0.9/dlk/core/losses/bce.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/losses/cross_entropy.py` & `dlk-0.0.9/dlk/core/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/losses/identity.py` & `dlk-0.0.9/dlk/core/losses/identity.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/losses/mse.py` & `dlk-0.0.9/dlk/core/losses/mse.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/losses/multi_loss.py` & `dlk-0.0.9/dlk/core/losses/multi_loss.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/models/__init__.py` & `dlk-0.0.9/dlk/core/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/models/basic.py` & `dlk-0.0.9/dlk/core/models/basic.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/modules/__init__.py` & `dlk-0.0.9/dlk/core/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/modules/bert.py` & `dlk-0.0.9/dlk/core/modules/bert.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/modules/biaffine.py` & `dlk-0.0.9/dlk/core/modules/biaffine.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/modules/conv1d.py` & `dlk-0.0.9/dlk/core/modules/conv1d.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/modules/crf.py` & `dlk-0.0.9/dlk/core/modules/crf.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/modules/distil_bert.py` & `dlk-0.0.9/dlk/core/modules/distil_bert.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/modules/linear.py` & `dlk-0.0.9/dlk/core/modules/linear.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/modules/logits_gather.py` & `dlk-0.0.9/dlk/core/modules/logits_gather.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/modules/lstm.py` & `dlk-0.0.9/dlk/core/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/modules/roberta.py` & `dlk-0.0.9/dlk/core/modules/roberta.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/optimizers/__init__.py` & `dlk-0.0.9/dlk/core/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/optimizers/adamw.py` & `dlk-0.0.9/dlk/core/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/optimizers/sgd.py` & `dlk-0.0.9/dlk/core/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/schedulers/__init__.py` & `dlk-0.0.9/dlk/core/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/schedulers/constant.py` & `dlk-0.0.9/dlk/core/schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/schedulers/constant_warmup.py` & `dlk-0.0.9/dlk/core/schedulers/constant_warmup.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/schedulers/cosine_warmup.py` & `dlk-0.0.9/dlk/core/schedulers/cosine_warmup.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/schedulers/linear_warmup.py` & `dlk-0.0.9/dlk/core/schedulers/linear_warmup.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/schedulers/multi_group_schedule.py` & `dlk-0.0.9/dlk/core/schedulers/multi_group_schedule.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/core/schedulers/rec_decay.py` & `dlk-0.0.9/dlk/core/schedulers/rec_decay.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/datamodules/__init__.py` & `dlk-0.0.9/dlk/data/datamodules/__init__.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/datamodules/basic.py` & `dlk-0.0.9/dlk/data/datamodules/basic.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/datamodules/readme.md` & `dlk-0.0.9/dlk/data/datamodules/readme.md`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/postprocessors/__init__.py` & `dlk-0.0.9/dlk/data/postprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/postprocessors/identity.py` & `dlk-0.0.9/dlk/data/postprocessors/identity.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/postprocessors/seq_lab.py` & `dlk-0.0.9/dlk/data/postprocessors/seq_lab.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/postprocessors/span_cls.py` & `dlk-0.0.9/dlk/data/postprocessors/span_cls.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/postprocessors/txt_cls.py` & `dlk-0.0.9/dlk/data/postprocessors/txt_cls.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/postprocessors/txt_reg.py` & `dlk-0.0.9/dlk/data/postprocessors/txt_reg.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/processors/__init__.py` & `dlk-0.0.9/dlk/data/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/processors/basic.py` & `dlk-0.0.9/dlk/data/processors/basic.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/processors/readme.md` & `dlk-0.0.9/dlk/data/processors/readme.md`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/subprocessors/__init__.py` & `dlk-0.0.9/dlk/data/subprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/subprocessors/basic_data_loader.py` & `dlk-0.0.9/dlk/data/subprocessors/basic_data_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         >>>                 "entities_info": "entities_info",
         >>>             },
         >>>             "output_map": {   // without necessery don't change this
         >>>                 "sentence": "sentence",
         >>>                 "uuid": "uuid",
         >>>                 "entities_info": "entities_info",
         >>>             },
-        >>>         }, //3
+        >>>         },
         >>>         "predict": "train",
         >>>         "online": "train",
         >>>     }
         >>> }
     """
     def __init__(self, stage, config: Dict):
```

### Comparing `dlk-0.0.8/dlk/data/subprocessors/char_gather.py` & `dlk-0.0.9/dlk/data/subprocessors/char_gather.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/subprocessors/fast_tokenizer.py` & `dlk-0.0.9/dlk/data/subprocessors/fast_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/subprocessors/load.py` & `dlk-0.0.9/dlk/data/subprocessors/load.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,18 @@
         self.stage = stage
         self.config = config.config
         if not self.config:
             logger.info(f"Skip 'load' at stage {self.stage}")
             return
         self.base_dir = config.base_dir
 
+        self.load_data = {}
+        for key, path in self.config.items():
+            self.load_data[key] = self.load(path)
+
     def load(self, path: str):
         """load data from path
 
         Args:
             path: the path to data
 
         Returns: 
@@ -86,12 +90,11 @@
             >>>     "tokenizer": ..
             >>> }
 
         Returns: 
             data + loaded_data
 
         """
-        for _, path in self.config.items():
-            meta = self.load(path)
+        for _, meta in self.load_data.items():
             for key, value in meta.items():
                 data[key] = value
         return data
```

### Comparing `dlk-0.0.8/dlk/data/subprocessors/save.py` & `dlk-0.0.9/dlk/data/subprocessors/save.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/subprocessors/seq_lab_firstpiece_relable.py` & `dlk-0.0.9/dlk/data/subprocessors/seq_lab_firstpiece_relable.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/subprocessors/seq_lab_relabel.py` & `dlk-0.0.9/dlk/data/subprocessors/seq_lab_relabel.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/subprocessors/span_cls_relabel.py` & `dlk-0.0.9/dlk/data/subprocessors/span_cls_relabel.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/subprocessors/token2charid.py` & `dlk-0.0.9/dlk/data/subprocessors/token2charid.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/subprocessors/token2id.py` & `dlk-0.0.9/dlk/data/subprocessors/token2id.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/subprocessors/token_embedding.py` & `dlk-0.0.9/dlk/data/subprocessors/token_embedding.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/subprocessors/token_gather.py` & `dlk-0.0.9/dlk/data/subprocessors/token_gather.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/data/subprocessors/token_norm.py` & `dlk-0.0.9/dlk/data/subprocessors/token_norm.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/dlk.drawio` & `dlk-0.0.9/dlk/dlk.drawio`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/managers/__init__.py` & `dlk-0.0.9/dlk/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/managers/lightning.py` & `dlk-0.0.9/dlk/managers/lightning.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/predict.py` & `dlk-0.0.9/dlk/predict.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/process.py` & `dlk-0.0.9/dlk/process.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/readme.md` & `dlk-0.0.9/dlk/readme.md`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/train.py` & `dlk-0.0.9/dlk/train.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/utils/config.py` & `dlk-0.0.9/dlk/utils/config.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/utils/get_root.py` & `dlk-0.0.9/dlk/utils/get_root.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/utils/logger.py` & `dlk-0.0.9/dlk/utils/logger.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/utils/parser.py` & `dlk-0.0.9/dlk/utils/parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,18 +12,58 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import hjson
 import os
 import copy
 from typing import Callable, List, Dict, Union
+from dlk.utils import register
 from dlk.utils.register import Register
 from dlk.utils.config import ConfigTool
 from dlk.utils.logger import Logger
 from dlk.utils.get_root import get_root
+from dlk.utils.register import Register
+from dlk.core import (
+    embedding_config_register,
+    embedding_register,
+    callback_config_register,
+    callback_register,
+    decoder_config_register,
+    decoder_register,
+    encoder_config_register,
+    encoder_register,
+    imodel_config_register,
+    imodel_register,
+    initmethod_config_register,
+    initmethod_register,
+    model_config_register,
+    model_register,
+    scheduler_config_register,
+    loss_config_register,
+    loss_register,
+    module_config_register,
+    module_register,
+    optimizer_config_register,
+    optimizer_register,
+    scheduler_register
+)
+from dlk.data import (
+    datamodule_config_register,
+    datamodule_register,
+    postprocessor_config_register,
+    postprocessor_register,
+    processor_config_register,
+    processor_register,
+    subprocessor_config_register,
+    subprocessor_register
+)
+from dlk.managers import (
+    manager_config_register, 
+    manager_register
+)
 import json
 
 logger = Logger.get_logger()
 
 config_parser_register = Register("Config parser register")
 
 
@@ -160,22 +200,26 @@
 class BaseConfigParser(object):
     """BaseConfigParser
     The config parser order is: inherit -> search -> link
 
     If some config is marked to "*@*", this means the para has not default value, you must coverd it(like 'label_nums', etc.).
 
     """
-    def __init__(self, config_file: Union[str, Dict, List], config_base_dir: str=""):
+    def __init__(self, config_file: Union[str, Dict, List], config_base_dir: str="", register: Register=None):
         super(BaseConfigParser, self).__init__()
         if isinstance(config_file, str):
             if config_file == '*@*':
                 self.config_file = "*@*"
                 return
             try:
-                self.config_file = self.load_hjson_file(os.path.join(get_root(), config_base_dir, config_file+'.hjson'))
+                if os.path.isfile(os.path.join(get_root(), config_base_dir, config_file+'.hjson')):
+                    self.config_file = self.load_hjson_file(os.path.join(get_root(), config_base_dir, config_file+'.hjson'))
+                else:
+                    self.config_file = register.get(config_file).default_config
+
             except Exception as e:
                 logger.error(f"There is an error occur when loading {os.path.join(get_root(), config_base_dir, config_file)}")
                 raise KeyError(e)
         elif isinstance(config_file, Dict):
             self.config_file = config_file
         else:
             raise KeyError('The config file must be str or dict. You provide {}.'.format(config_file))
@@ -654,112 +698,112 @@
         super(RootConfigParser, self).__init__(config_file, config_base_dir='')
 
 
 @config_parser_register('manager')
 class ManagerConfigParser(BaseConfigParser):
     """docstring for ManagerConfigParser"""
     def __init__(self, config_file):
-        super(ManagerConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/managers/')
+        super(ManagerConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/managers/', register=manager_config_register)
 
 
 @config_parser_register('callback')
 class CallbackConfigParser(BaseConfigParser):
     """docstring for CallbackConfigParser"""
     def __init__(self, config_file):
-        super(CallbackConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/callbacks/')
+        super(CallbackConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/callbacks/', register=callback_config_register)
 
 
 @config_parser_register('datamodule')
 class DatamoduleConfigParser(BaseConfigParser):
     """docstring for DatamoduleConfigParser"""
     def __init__(self, config_file):
-        super(DatamoduleConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/data/datamodules/')
+        super(DatamoduleConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/data/datamodules/', register=datamodule_config_register)
 
 
 @config_parser_register('imodel')
 class IModelConfigParser(BaseConfigParser):
     """docstring for IModelConfigParser"""
     def __init__(self, config_file):
-        super(IModelConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/imodels/')
+        super(IModelConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/imodels/', register=imodel_config_register)
 
 
 @config_parser_register('model')
 class ModelConfigParser(BaseConfigParser):
     """docstring for ModelConfigParser"""
     def __init__(self, config_file):
-        super(ModelConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/models/')
+        super(ModelConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/models/', register=model_config_register)
 
 
 @config_parser_register('optimizer')
 class OptimizerConfigParser(BaseConfigParser):
     """docstring for OptimizerConfigParser"""
     def __init__(self, config_file):
-        super(OptimizerConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/optimizers/')
+        super(OptimizerConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/optimizers/', register=optimizer_config_register)
 
 
 @config_parser_register('scheduler')
 class ScheduleConfigParser(BaseConfigParser):
     """docstring for ScheduleConfigParser"""
     def __init__(self, config_file):
-        super(ScheduleConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/schedulers/')
+        super(ScheduleConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/schedulers/', register=scheduler_config_register)
 
 @config_parser_register('initmethod')
 class InitMethodConfigParser(BaseConfigParser):
     """docstring for InitMethodConfigParser"""
     def __init__(self, config_file):
-        super(InitMethodConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/initmethods/')
+        super(InitMethodConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/initmethods/', register=initmethod_config_register)
 
 
 @config_parser_register('loss')
 class LossConfigParser(BaseConfigParser):
     """docstring for LossConfigParser"""
     def __init__(self, config_file):
-        super(LossConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/losses/')
+        super(LossConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/losses/', register=loss_config_register)
 
 
 @config_parser_register('encoder')
 class EncoderConfigParser(BaseConfigParser):
     """docstring for EncoderConfigParser"""
     def __init__(self, config_file):
-        super(EncoderConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/layers/encoders/')
+        super(EncoderConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/layers/encoders/', register=encoder_config_register)
 
 
 @config_parser_register('decoder')
 class DecoderConfigParser(BaseConfigParser):
     """docstring for DecoderConfigParser"""
     def __init__(self, config_file):
-        super(DecoderConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/layers/decoders/')
+        super(DecoderConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/layers/decoders/', register=decoder_config_register)
 
 
 @config_parser_register('embedding')
 class EmbeddingConfigParser(BaseConfigParser):
     """docstring for EmbeddingConfigParser"""
     def __init__(self, config_file):
-        super(EmbeddingConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/layers/embeddings/')
+        super(EmbeddingConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/layers/embeddings/', register=embedding_config_register)
 
 
 @config_parser_register('module')
 class ModuleConfigParser(BaseConfigParser):
     """docstring for ModuleConfigParser"""
     def __init__(self, config_file):
-        super(ModuleConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/modules/')
+        super(ModuleConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/core/modules/', register=module_config_register)
 
 @config_parser_register('processor')
 class ProcessorConfigParser(BaseConfigParser):
     """docstring for ProcessorConfigParser"""
     def __init__(self, config_file):
-        super(ProcessorConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/data/processors/')
+        super(ProcessorConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/data/processors/', register=processor_config_register)
 
 
 @config_parser_register('subprocessor')
 class SubProcessorConfigParser(BaseConfigParser):
     """docstring for SubProcessorConfigParser"""
     def __init__(self, config_file):
-        super(SubProcessorConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/data/subprocessors/')
+        super(SubProcessorConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/data/subprocessors/', register=subprocessor_config_register)
 
 
 @config_parser_register('postprocessor')
 class PostProcessorConfigParser(BaseConfigParser):
     """docstring for PostProcessorConfigParser"""
     def __init__(self, config_file):
-        super(PostProcessorConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/data/postprocessors/')
+        super(PostProcessorConfigParser, self).__init__(config_file, config_base_dir='dlk/configures/data/postprocessors/', register=postprocessor_config_register)
```

### Comparing `dlk-0.0.8/dlk/utils/quick_search.py` & `dlk-0.0.9/dlk/utils/quick_search.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/utils/register.py` & `dlk-0.0.9/dlk/utils/register.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/utils/tokenizer_util.py` & `dlk-0.0.9/dlk/utils/tokenizer_util.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk/utils/vocab.py` & `dlk-0.0.9/dlk/utils/vocab.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/dlk.egg-info/PKG-INFO` & `dlk-0.0.9/dlk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlk
-Version: 0.0.8
+Version: 0.0.9
 Summary: dlk: Deep Learning Kit
 Home-page: https://github.com/cstsunfu/dlk
 Author: cstsunfu
 Author-email: cstsunfu@gmail.com
 License: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `dlk-0.0.8/dlk.egg-info/SOURCES.txt` & `dlk-0.0.9/dlk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/Makefile` & `dlk-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/make.bat` & `dlk-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/readme.md` & `dlk-0.0.9/docs/readme.md`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/source/appointment.md` & `dlk-0.0.9/docs/source/appointment.md`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/source/conf.py` & `dlk-0.0.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/source/dlk.core.callbacks.rst` & `dlk-0.0.9/docs/source/dlk.core.callbacks.rst`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/source/dlk.core.initmethods.rst` & `dlk-0.0.9/docs/source/dlk.core.initmethods.rst`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/source/dlk.core.layers.decoders.rst` & `dlk-0.0.9/docs/source/dlk.core.layers.decoders.rst`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/source/dlk.core.layers.embeddings.rst` & `dlk-0.0.9/docs/source/dlk.core.layers.embeddings.rst`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/source/dlk.core.layers.encoders.rst` & `dlk-0.0.9/docs/source/dlk.core.layers.encoders.rst`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/source/dlk.core.losses.rst` & `dlk-0.0.9/docs/source/dlk.core.losses.rst`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/source/dlk.core.modules.rst` & `dlk-0.0.9/docs/source/dlk.core.modules.rst`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/source/dlk.core.optimizers.rst` & `dlk-0.0.9/docs/source/dlk.core.optimizers.rst`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/source/dlk.core.rst` & `dlk-0.0.9/docs/source/dlk.core.rst`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/source/dlk.core.schedulers.rst` & `dlk-0.0.9/docs/source/dlk.core.schedulers.rst`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/source/dlk.data.postprocessors.rst` & `dlk-0.0.9/docs/source/dlk.data.postprocessors.rst`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/source/dlk.data.subprocessors.rst` & `dlk-0.0.9/docs/source/dlk.data.subprocessors.rst`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/source/dlk.rst` & `dlk-0.0.9/docs/source/dlk.rst`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/source/dlk.utils.rst` & `dlk-0.0.9/docs/source/dlk.utils.rst`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/source/index.rst` & `dlk-0.0.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/source/introduction.md` & `dlk-0.0.9/docs/source/introduction.md`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/docs/source/process_progress.md` & `dlk-0.0.9/docs/source/process_progress.md`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/sequence_labeling/conll2003/bert_firstpiece_lstm_crf/main.hjson` & `dlk-0.0.9/examples/sequence_labeling/conll2003/bert_firstpiece_lstm_crf/main.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/sequence_labeling/conll2003/bert_firstpiece_lstm_crf/prepro.hjson` & `dlk-0.0.9/examples/sequence_labeling/conll2003/bert_firstpiece_lstm_crf/prepro.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/sequence_labeling/conll2003/norm_char_lstm_crf/main.hjson` & `dlk-0.0.9/examples/sequence_labeling/conll2003/norm_char_lstm_crf/main.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/sequence_labeling/conll2003/norm_char_lstm_crf/pre_prepro.hjson` & `dlk-0.0.9/examples/sequence_labeling/conll2003/norm_char_lstm_crf/pre_prepro.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/sequence_labeling/conll2003/norm_char_lstm_crf/prepro.hjson` & `dlk-0.0.9/examples/sequence_labeling/conll2003/norm_char_lstm_crf/prepro.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/sequence_labeling/conll2003/process.py` & `dlk-0.0.9/examples/sequence_labeling/conll2003/process.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/sequence_labeling/conll2003/train.py` & `dlk-0.0.9/examples/sequence_labeling/conll2003/train.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/sequence_labeling/conll2003/utils/__init__.py` & `dlk-0.0.9/examples/sequence_labeling/conll2003/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/sequence_labeling/conll2003/utils/cls_bio2json.py` & `dlk-0.0.9/examples/sequence_labeling/conll2003/utils/cls_bio2json.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/sequence_labeling/conll2003/utils/cls_json2bio.py` & `dlk-0.0.9/examples/sequence_labeling/conll2003/utils/cls_json2bio.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/sequence_labeling/conll2003/utils/get_vocab.py` & `dlk-0.0.9/examples/sequence_labeling/conll2003/utils/get_vocab.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/text_cls/sst2/distil_bert/main.hjson` & `dlk-0.0.9/examples/text_cls/sst2/distil_bert/main.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/text_cls/sst2/distil_bert/prepro.hjson` & `dlk-0.0.9/examples/text_cls/sst2/distil_bert/prepro.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/text_cls/sst2/process.py` & `dlk-0.0.9/examples/text_cls/sst2/process.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/text_cls/sst2/train.py` & `dlk-0.0.9/examples/text_cls/sst2/train.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/text_match/snli/distil_bert/main.hjson` & `dlk-0.0.9/examples/text_match/snli/distil_bert/main.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/text_match/snli/distil_bert/prepro.hjson` & `dlk-0.0.9/examples/text_match/snli/distil_bert/prepro.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/text_match/snli/process.py` & `dlk-0.0.9/examples/text_match/snli/process.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/text_match/snli/train.py` & `dlk-0.0.9/examples/text_match/snli/train.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/text_reg/sst2/distil_bert/main.hjson` & `dlk-0.0.9/examples/text_reg/sst2/distil_bert/main.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/text_reg/sst2/distil_bert/prepro.hjson` & `dlk-0.0.9/examples/text_reg/sst2/distil_bert/prepro.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/text_reg/sst2/process.py` & `dlk-0.0.9/examples/text_reg/sst2/process.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/examples/text_reg/sst2/train.py` & `dlk-0.0.9/examples/text_reg/sst2/train.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/setup.py` & `dlk-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/test_predict.py` & `dlk-0.0.9/test_predict.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/test_process.py` & `dlk-0.0.9/test_process.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/test_train.py` & `dlk-0.0.9/test_train.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tests/parser/test_base.json` & `dlk-0.0.9/tests/parser/test_base.json`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tests/parser/test_base.py` & `dlk-0.0.9/tests/parser/test_base.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tests/parser/test_base_inp.hjson` & `dlk-0.0.9/tests/parser/test_base_inp.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tests/parser/test_base_out.hjson` & `dlk-0.0.9/tests/parser/test_base_out.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tests/processors/bpe_token.json` & `dlk-0.0.9/tests/processors/bpe_token.json`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tests/processors/process.hjson` & `dlk-0.0.9/tests/processors/process.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tests/processors/test_wordpiece_tokenizer.py` & `dlk-0.0.9/tests/processors/test_wordpiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tests/processors/uni_token.json` & `dlk-0.0.9/tests/processors/uni_token.json`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tests/processors/wp_token.json` & `dlk-0.0.9/tests/processors/wp_token.json`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tests/test_test/lightning.py` & `dlk-0.0.9/tests/test_test/lightning.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tests/test_test/trace/dict_trace.py` & `dlk-0.0.9/tests/test_test/trace/dict_trace.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tests/test_test/trace/simple_trace.py` & `dlk-0.0.9/tests/test_test/trace/simple_trace.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tools/conf.py` & `dlk-0.0.9/tools/conf.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tools/convert_tokenizer/convert.py` & `dlk-0.0.9/tools/convert_tokenizer/convert.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tools/convert_tokenizer/vocab2tokenizer.py` & `dlk-0.0.9/tools/convert_tokenizer/vocab2tokenizer.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tools/tokenize/tokenizer.hjson` & `dlk-0.0.9/tools/tokenize/tokenizer.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tools/tokenize/tokenizer.py` & `dlk-0.0.9/tools/tokenize/tokenizer.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tools/train_tokenizer/train_tokenizer.hjson` & `dlk-0.0.9/tools/train_tokenizer/train_tokenizer.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tools/train_tokenizer/train_tokenizer.py` & `dlk-0.0.9/tools/train_tokenizer/train_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tools/view_config.py` & `dlk-0.0.9/tools/view_config.py`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tools/word2vec/word2vec.hjson` & `dlk-0.0.9/tools/word2vec/word2vec.hjson`

 * *Files identical despite different names*

### Comparing `dlk-0.0.8/tools/word2vec/word2vec.py` & `dlk-0.0.9/tools/word2vec/word2vec.py`

 * *Files identical despite different names*

