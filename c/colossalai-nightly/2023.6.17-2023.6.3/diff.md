# Comparing `tmp/colossalai-nightly-2023.6.17.tar.gz` & `tmp/colossalai-nightly-2023.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colossalai-nightly-2023.6.17.tar", last modified: Sat Jun 17 00:15:15 2023, max compression
+gzip compressed data, was "colossalai-nightly-2023.6.3.tar", last modified: Sat Jun  3 00:15:29 2023, max compression
```

## Comparing `colossalai-nightly-2023.6.17.tar` & `colossalai-nightly-2023.6.3.tar`

### file list

```diff
@@ -1,907 +1,901 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.804906 colossalai-nightly-2023.6.17/
--rw-r--r--   0 runner    (1001) docker     (123)    22244 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25400 2023-06-17 00:15:15.804906 colossalai-nightly-2023.6.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20789 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.712901 colossalai-nightly-2023.6.17/colossalai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.712901 colossalai-nightly-2023.6.17/colossalai/_C/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_C/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.712901 colossalai-nightly-2023.6.17/colossalai/_analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_analyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.712901 colossalai-nightly-2023.6.17/colossalai/_analyzer/_subclasses/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_analyzer/_subclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_analyzer/_subclasses/_meta_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_analyzer/_subclasses/_monkey_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    18694 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_analyzer/_subclasses/flop_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_analyzer/_subclasses/meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_analyzer/envs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.712901 colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/graph_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/node_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.716901 colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/passes/graph_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/passes/shape_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/symbolic_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.716901 colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/tracer/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/tracer/bias_addition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/tracer/custom_leaf_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/tracer/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/tracer/symbolic_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/tracer/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.716901 colossalai-nightly-2023.6.17/colossalai/amp/
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/amp/amp_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.716901 colossalai-nightly-2023.6.17/colossalai/amp/apex_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/amp/apex_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/amp/apex_amp/apex_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.716901 colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/_fp16_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.716901 colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/grad_scaler/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/grad_scaler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.716901 colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/mixed_precision_mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/mixed_precision_mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/mixed_precision_mixin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/mixed_precision_mixin/bf16.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/mixed_precision_mixin/fp16.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/naive_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.716901 colossalai-nightly-2023.6.17/colossalai/amp/torch_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/amp/torch_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/amp/torch_amp/_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/amp/torch_amp/torch_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.716901 colossalai-nightly-2023.6.17/colossalai/auto_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.720901 colossalai-nightly-2023.6.17/colossalai/auto_parallel/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/checkpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/checkpoint/build_c_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py
--rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/checkpoint/operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.720901 colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.720901 colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/where.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/shard_metainfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.720901 colossalai-nightly-2023.6.17/colossalai/auto_parallel/offload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/offload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/offload/amp_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/offload/base_offload_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/offload/mem_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/offload/region.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/offload/region_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/offload/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/offload/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/offload/training_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/offload/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.724901 colossalai-nightly-2023.6.17/colossalai/auto_parallel/passes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/passes/comm_metainfo_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/passes/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/passes/meta_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/passes/runtime_apply_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    22686 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/passes/runtime_preparation_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.724901 colossalai-nightly-2023.6.17/colossalai/auto_parallel/pipeline_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/pipeline_shard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.724901 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.728902 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.728902 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    43503 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/sharding_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.728902 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/solver/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.732902 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/utils/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/utils/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/utils/reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/utils/sharding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.732902 colossalai-nightly-2023.6.17/colossalai/booster/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/booster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/booster/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/booster/booster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.732902 colossalai-nightly-2023.6.17/colossalai/booster/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/booster/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/booster/mixed_precision/bf16.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/booster/mixed_precision/fp16_apex.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/booster/mixed_precision/fp16_naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/booster/mixed_precision/fp16_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/booster/mixed_precision/fp8.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/booster/mixed_precision/mixed_precision_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.732902 colossalai-nightly-2023.6.17/colossalai/booster/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/booster/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/booster/plugin/dp_plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14029 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/booster/plugin/gemini_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9520 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/booster/plugin/low_level_zero_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/booster/plugin/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/booster/plugin/torch_ddp_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/booster/plugin/torch_fsdp_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.732902 colossalai-nightly-2023.6.17/colossalai/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/builder/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.732902 colossalai-nightly-2023.6.17/colossalai/checkpoint_io/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/checkpoint_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/checkpoint_io/checkpoint_io_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/checkpoint_io/general_checkpoint_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/checkpoint_io/index_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/checkpoint_io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.732902 colossalai-nightly-2023.6.17/colossalai/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.736902 colossalai-nightly-2023.6.17/colossalai/cli/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/cli/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/cli/benchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/cli/benchmark/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/cli/benchmark/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.736902 colossalai-nightly-2023.6.17/colossalai/cli/check/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/cli/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/cli/check/check_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.736902 colossalai-nightly-2023.6.17/colossalai/cli/launcher/
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/cli/launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/cli/launcher/hostinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/cli/launcher/multinode_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10169 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/cli/launcher/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.736902 colossalai-nightly-2023.6.17/colossalai/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/cluster/device_mesh_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/cluster/dist_coordinator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/cluster/process_group_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.736902 colossalai-nightly-2023.6.17/colossalai/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/communication/collective.py
--rw-r--r--   0 runner    (1001) docker     (123)    19462 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/communication/p2p.py
--rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/communication/p2p_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/communication/ring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/communication/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.736902 colossalai-nightly-2023.6.17/colossalai/context/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/context/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/context/moe_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    23924 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/context/parallel_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/context/parallel_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.740902 colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/initializer_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/initializer_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/initializer_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/initializer_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/initializer_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/initializer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/initializer_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/initializer_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/initializer_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/process_group_initializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.740902 colossalai-nightly-2023.6.17/colossalai/context/random/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/context/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/context/random/_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/context/random/seed_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/context/singleton_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.740902 colossalai-nightly-2023.6.17/colossalai/device/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/device/alpha_beta_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/device/calc_pipeline_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/device/device_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.740902 colossalai-nightly-2023.6.17/colossalai/engine/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/engine/_base_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.740902 colossalai-nightly-2023.6.17/colossalai/engine/gradient_accumulation/
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/engine/gradient_accumulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/engine/gradient_accumulation/_gradient_accumulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.740902 colossalai-nightly-2023.6.17/colossalai/engine/gradient_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/engine/gradient_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/engine/gradient_handler/_base_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/engine/gradient_handler/_moe_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/engine/gradient_handler/_zero_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/engine/gradient_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.740902 colossalai-nightly-2023.6.17/colossalai/engine/schedule/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/engine/schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/engine/schedule/_base_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/engine/schedule/_non_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    41258 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/engine/schedule/_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/engine/schedule/_pipeline_schedule_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.740902 colossalai-nightly-2023.6.17/colossalai/fx/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    19408 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/_meta_regist_12.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/_meta_regist_13.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.740902 colossalai-nightly-2023.6.17/colossalai/fx/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44753 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/codegen/activation_checkpoint_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/graph_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.744902 colossalai-nightly-2023.6.17/colossalai/fx/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/passes/adding_split_node_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/passes/concrete_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/passes/meta_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/passes/passes_for_gpt2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/passes/shard_1d_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/passes/split_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/passes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.744902 colossalai-nightly-2023.6.17/colossalai/fx/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/dataflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.744902 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.744902 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_function/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_function/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_function/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_function/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_function/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_function/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_function/python_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.748903 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_module/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_module/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_module/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_module/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_module/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_module/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_module/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_module/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_module/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_module/torch_op.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/shard_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/memory_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/opcount.py
--rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/shard_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/profiler/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.748903 colossalai-nightly-2023.6.17/colossalai/fx/tracer/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/_meta_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/_symbolic_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/_tracer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.748903 colossalai-nightly-2023.6.17/colossalai/fx/tracer/bias_addition_patch/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/bias_addition_patch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.748903 colossalai-nightly-2023.6.17/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.748903 colossalai-nightly-2023.6.17/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    26969 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.748903 colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.748903 colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_function/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_function/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_function/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_function/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_function/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.752903 colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_module/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_module/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_module/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_module/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_module/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_module/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_module/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    24624 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/fx/tracer/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/global_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.752903 colossalai-nightly-2023.6.17/colossalai/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/interface/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/interface/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.752903 colossalai-nightly-2023.6.17/colossalai/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.752903 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.756903 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/compat.h
--rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/cpu_adam.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.756903 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu
--rw-r--r--   0 runner    (1001) docker     (123)    37586 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.756903 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/context.h
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h
--rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/ls_cub.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h
--rw-r--r--   0 runner    (1001) docker     (123)    48403 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22850 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/type_shim.h
--rw-r--r--   0 runner    (1001) docker     (123)    24864 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/scaled_softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.756903 colossalai-nightly-2023.6.17/colossalai/kernel/jit/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/jit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/jit/bias_dropout_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/jit/bias_gelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/jit/option.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.760903 colossalai-nightly-2023.6.17/colossalai/kernel/op_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/op_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/op_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/op_builder/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/op_builder/fused_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/op_builder/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/op_builder/moe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/op_builder/multi_head_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/op_builder/scaled_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/kernel/op_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.760903 colossalai-nightly-2023.6.17/colossalai/lazy/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23336 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/lazy/lazy_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.760903 colossalai-nightly-2023.6.17/colossalai/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.760903 colossalai-nightly-2023.6.17/colossalai/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.760903 colossalai-nightly-2023.6.17/colossalai/nn/_ops/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/_ops/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/_ops/addmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/_ops/batch_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/_ops/element_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/_ops/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/_ops/embedding_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/_ops/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/_ops/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/_ops/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/_ops/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.760903 colossalai-nightly-2023.6.17/colossalai/nn/layer/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/base_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.760903 colossalai-nightly-2023.6.17/colossalai/nn/layer/colossalai_layer/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/colossalai_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/colossalai_layer/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/colossalai_layer/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/colossalai_layer/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/colossalai_layer/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/colossalai_layer/normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.764904 colossalai-nightly-2023.6.17/colossalai/nn/layer/moe/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/moe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/moe/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/moe/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/moe/experts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/moe/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/moe/routers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/moe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.764904 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_1d/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_1d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_1d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    49753 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_1d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.764904 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_2d/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_2d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_2d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    50524 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_2d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.764904 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_2p5d/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_2p5d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37643 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_2p5d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_2p5d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    50769 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_2p5d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.764904 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_3d/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_3d/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22769 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_3d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_3d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    51441 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_3d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.764904 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_sequence/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_sequence/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_sequence/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_sequence/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.764904 colossalai-nightly-2023.6.17/colossalai/nn/layer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/utils/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.764904 colossalai-nightly-2023.6.17/colossalai/nn/layer/vanilla/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/vanilla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/vanilla/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.764904 colossalai-nightly-2023.6.17/colossalai/nn/layer/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/layer/wrapper/pipeline_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.768904 colossalai-nightly-2023.6.17/colossalai/nn/loss/
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/loss/loss_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/loss/loss_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/loss/loss_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/loss/loss_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/loss/loss_moe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.768904 colossalai-nightly-2023.6.17/colossalai/nn/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/lr_scheduler/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/lr_scheduler/delayed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/lr_scheduler/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/lr_scheduler/multistep.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/lr_scheduler/onecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/lr_scheduler/poly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/lr_scheduler/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.768904 colossalai-nightly-2023.6.17/colossalai/nn/metric/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/metric/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/metric/accuracy_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/metric/accuracy_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/metric/accuracy_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.768904 colossalai-nightly-2023.6.17/colossalai/nn/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/optimizer/colossalai_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/optimizer/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/optimizer/fused_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/optimizer/fused_lamb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/optimizer/fused_sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/optimizer/hybrid_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/optimizer/lamb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/optimizer/lars.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/optimizer/nvme_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.768904 colossalai-nightly-2023.6.17/colossalai/nn/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/parallel/data_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.768904 colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.772904 colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/cache_embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/cache_embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    28600 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/cache_embedding/copyer.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/colo_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/nn/parallel/reducer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.772904 colossalai-nightly-2023.6.17/colossalai/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/pipeline/layer_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.772904 colossalai-nightly-2023.6.17/colossalai/pipeline/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/pipeline/middleware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.772904 colossalai-nightly-2023.6.17/colossalai/pipeline/middleware/adaptor/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/pipeline/middleware/adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/pipeline/middleware/adaptor/fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/pipeline/middleware/topo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/pipeline/pipelinable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/pipeline/pipeline_process_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.772904 colossalai-nightly-2023.6.17/colossalai/pipeline/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/pipeline/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59170 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/pipeline/rpc/_pipeline_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/pipeline/rpc/_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/pipeline/rpc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/pipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.772904 colossalai-nightly-2023.6.17/colossalai/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/registry/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.776904 colossalai-nightly-2023.6.17/colossalai/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/colo_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/colo_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22269 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/comm_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/compute_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.776904 colossalai-nightly-2023.6.17/colossalai/tensor/d_tensor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/d_tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/d_tensor/comm_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/d_tensor/d_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/d_tensor/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    25229 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/d_tensor/layout_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/d_tensor/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/d_tensor/sharding_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/d_tensor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/dist_spec_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/distspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/op_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/param_op_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/process_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    36501 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/shape_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/sharding_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/tensor_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.776904 colossalai-nightly-2023.6.17/colossalai/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/testing/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/testing/pytest_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/testing/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.776904 colossalai-nightly-2023.6.17/colossalai/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/trainer/_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.776904 colossalai-nightly-2023.6.17/colossalai/trainer/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/trainer/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/trainer/hooks/_base_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/trainer/hooks/_checkpoint_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/trainer/hooks/_commons_.py
--rw-r--r--   0 runner    (1001) docker     (123)    13106 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/trainer/hooks/_log_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/trainer/hooks/_lr_scheduler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/trainer/hooks/_metric_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.780905 colossalai-nightly-2023.6.17/colossalai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/activation_checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.780905 colossalai-nightly-2023.6.17/colossalai/utils/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/checkpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/checkpoint/module_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/checkpoint/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.780905 colossalai-nightly-2023.6.17/colossalai/utils/checkpoint_io/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/checkpoint_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/checkpoint_io/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/checkpoint_io/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/checkpoint_io/convertor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/checkpoint_io/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/checkpoint_io/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/checkpoint_io/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/checkpoint_io/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/checkpoint_io/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/checkpoint_io/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/checkpointing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.780905 colossalai-nightly-2023.6.17/colossalai/utils/data_sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/data_sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/data_sampler/base_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/data_sampler/data_parallel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.780905 colossalai-nightly-2023.6.17/colossalai/utils/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/moe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.780905 colossalai-nightly-2023.6.17/colossalai/utils/multi_tensor_apply/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/multi_tensor_apply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.780905 colossalai-nightly-2023.6.17/colossalai/utils/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/profiler/extention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.780905 colossalai-nightly-2023.6.17/colossalai/utils/profiler/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/profiler/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/profiler/legacy/comm_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/profiler/legacy/pcie_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/profiler/legacy/prof_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/profiler/stateful_tensor_mem_extention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.780905 colossalai-nightly-2023.6.17/colossalai/utils/rank_recorder/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/rank_recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/rank_recorder/rank_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.780905 colossalai-nightly-2023.6.17/colossalai/utils/tensor_detector/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/tensor_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/tensor_detector/tensor_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.780905 colossalai-nightly-2023.6.17/colossalai/zero/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.784905 colossalai-nightly-2023.6.17/colossalai/zero/gemini/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.784905 colossalai-nightly-2023.6.17/colossalai/zero/gemini/chunk/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/chunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/chunk/chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/chunk/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/chunk/search_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/chunk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/colo_init_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    37658 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/gemini_ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/gemini_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/gemini_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/gemini_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.784905 colossalai-nightly-2023.6.17/colossalai/zero/gemini/memory_tracer/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/memory_tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/memory_tracer/memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/memory_tracer/memory_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/memory_tracer/memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/memory_tracer/param_runtime_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/memory_tracer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/placement_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/gemini/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.784905 colossalai-nightly-2023.6.17/colossalai/zero/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.784905 colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/gemini_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.784905 colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/ophooks/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/ophooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/ophooks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.788905 colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/paramhooks/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/paramhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/stateful_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/tensor_placement_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/tensor_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.788905 colossalai-nightly-2023.6.17/colossalai/zero/legacy/init_ctx/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/init_ctx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/init_ctx/init_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.788905 colossalai-nightly-2023.6.17/colossalai/zero/legacy/shard_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/shard_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/shard_utils/base_shard_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/shard_utils/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.788905 colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_model/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_model/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_model/reduce_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29261 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_model/sharded_model_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_model/zero_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.788905 colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_optim/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.788905 colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_param/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_param/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_param/sharded_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_param/sharded_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.788905 colossalai-nightly-2023.6.17/colossalai/zero/low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/low_level/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.788905 colossalai-nightly-2023.6.17/colossalai/zero/low_level/bookkeeping/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/low_level/bookkeeping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/low_level/bookkeeping/base_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/low_level/bookkeeping/bucket_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/low_level/bookkeeping/gradient_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/low_level/bookkeeping/parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/low_level/bookkeeping/tensor_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    26595 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/low_level/low_level_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/colossalai/zero/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.792905 colossalai-nightly-2023.6.17/colossalai_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25400 2023-06-17 00:15:15.000000 colossalai-nightly-2023.6.17/colossalai_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37585 2023-06-17 00:15:15.000000 colossalai-nightly-2023.6.17/colossalai_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 00:15:15.000000 colossalai-nightly-2023.6.17/colossalai_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-17 00:15:15.000000 colossalai-nightly-2023.6.17/colossalai_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-17 00:15:15.000000 colossalai-nightly-2023.6.17/colossalai_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-17 00:15:15.000000 colossalai-nightly-2023.6.17/colossalai_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.792905 colossalai-nightly-2023.6.17/op_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/op_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/op_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/op_builder/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/op_builder/fused_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/op_builder/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/op_builder/moe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/op_builder/multi_head_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/op_builder/scaled_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/op_builder/scaled_upper_triangle_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/op_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.792905 colossalai-nightly-2023.6.17/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 00:15:15.804906 colossalai-nightly-2023.6.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.712901 colossalai-nightly-2023.6.17/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.792905 colossalai-nightly-2023.6.17/tests/components_to_test/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/components_to_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/components_to_test/albert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/components_to_test/beit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/components_to_test/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/components_to_test/gpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/components_to_test/hanging_param_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/components_to_test/inline_op_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/components_to_test/nested_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/components_to_test/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/components_to_test/repeated_computed_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/components_to_test/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/components_to_test/simple_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.792905 colossalai-nightly-2023.6.17/tests/components_to_test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/components_to_test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/components_to_test/utils/dummy_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/components_to_test/utils/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.792905 colossalai-nightly-2023.6.17/tests/kit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/kit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.792905 colossalai-nightly-2023.6.17/tests/kit/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/kit/model_zoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.792905 colossalai-nightly-2023.6.17/tests/kit/model_zoo/diffusers/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/kit/model_zoo/diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/kit/model_zoo/diffusers/diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/kit/model_zoo/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.792905 colossalai-nightly-2023.6.17/tests/kit/model_zoo/timm/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/kit/model_zoo/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/kit/model_zoo/timm/timm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.796906 colossalai-nightly-2023.6.17/tests/kit/model_zoo/torchaudio/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/kit/model_zoo/torchaudio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/kit/model_zoo/torchaudio/torchaudio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.796906 colossalai-nightly-2023.6.17/tests/kit/model_zoo/torchrec/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/kit/model_zoo/torchrec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/kit/model_zoo/torchrec/torchrec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.796906 colossalai-nightly-2023.6.17/tests/kit/model_zoo/torchvision/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/kit/model_zoo/torchvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/kit/model_zoo/torchvision/torchvision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.796906 colossalai-nightly-2023.6.17/tests/kit/model_zoo/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/kit/model_zoo/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/kit/model_zoo/transformers/albert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/kit/model_zoo/transformers/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/kit/model_zoo/transformers/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/kit/model_zoo/transformers/opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/kit/model_zoo/transformers/t5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.796906 colossalai-nightly-2023.6.17/tests/test_analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_analyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.796906 colossalai-nightly-2023.6.17/tests/test_analyzer/test_fx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_analyzer/test_fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_analyzer/test_fx/test_bias_addition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_analyzer/test_fx/test_mod_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_analyzer/test_fx/test_nested_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_analyzer/test_fx/test_shape_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_analyzer/test_fx/test_symbolic_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_analyzer/test_fx/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.796906 colossalai-nightly-2023.6.17/tests/test_analyzer/test_subclasses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_analyzer/test_subclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_analyzer/test_subclasses/test_aten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_analyzer/test_subclasses/test_flop_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_analyzer/test_subclasses/test_meta_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.796906 colossalai-nightly-2023.6.17/tests/test_auto_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.796906 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_pass/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_pass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_pass/test_node_converting_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.800906 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.800906 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:15.800906 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-17 00:15:03.000000 colossalai-nightly-2023.6.17/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.073204 colossalai-nightly-2023.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    22244 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-06-03 00:15:29.073204 colossalai-nightly-2023.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20789 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.933204 colossalai-nightly-2023.6.3/colossalai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.933204 colossalai-nightly-2023.6.3/colossalai/_C/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_C/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.933204 colossalai-nightly-2023.6.3/colossalai/_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.933204 colossalai-nightly-2023.6.3/colossalai/_analyzer/_subclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/_subclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/_subclasses/_meta_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/_subclasses/_monkey_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18694 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/_subclasses/flop_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/_subclasses/meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/envs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.933204 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/graph_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/node_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.937204 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/passes/graph_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/passes/shape_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/symbolic_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.937204 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/tracer/bias_addition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/tracer/custom_leaf_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/tracer/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/tracer/symbolic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/tracer/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.937204 colossalai-nightly-2023.6.3/colossalai/amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/amp_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.937204 colossalai-nightly-2023.6.3/colossalai/amp/apex_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/apex_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/apex_amp/apex_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.937204 colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/_fp16_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.937204 colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/grad_scaler/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/grad_scaler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/naive_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.937204 colossalai-nightly-2023.6.3/colossalai/amp/torch_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/torch_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/torch_amp/_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/amp/torch_amp/torch_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.937204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.941204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/build_c_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.941204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.941204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/shard_metainfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.945204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/amp_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/base_offload_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/mem_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/region_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/training_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.945204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/comm_metainfo_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/meta_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/runtime_apply_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22686 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/runtime_preparation_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.945204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/pipeline_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/pipeline_shard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.945204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.949204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.953204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43503 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/sharding_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.953204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/solver/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.953204 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/sharding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.957204 colossalai-nightly-2023.6.3/colossalai/booster/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11106 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/booster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.957204 colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/bf16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/fp16_apex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/fp16_naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/fp16_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/fp8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/mixed_precision_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.957204 colossalai-nightly-2023.6.3/colossalai/booster/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/plugin/dp_plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13628 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/plugin/gemini_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/plugin/low_level_zero_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/plugin/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/plugin/torch_ddp_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/booster/plugin/torch_fsdp_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.957204 colossalai-nightly-2023.6.3/colossalai/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/builder/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.957204 colossalai-nightly-2023.6.3/colossalai/checkpoint_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/checkpoint_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/checkpoint_io/checkpoint_io_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/checkpoint_io/general_checkpoint_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/checkpoint_io/index_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/checkpoint_io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.957204 colossalai-nightly-2023.6.3/colossalai/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.961204 colossalai-nightly-2023.6.3/colossalai/cli/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/benchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/benchmark/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/benchmark/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.961204 colossalai-nightly-2023.6.3/colossalai/cli/check/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/check/check_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.961204 colossalai-nightly-2023.6.3/colossalai/cli/launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/launcher/hostinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/launcher/multinode_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10169 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cli/launcher/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.961204 colossalai-nightly-2023.6.3/colossalai/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cluster/device_mesh_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cluster/dist_coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/cluster/process_group_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.961204 colossalai-nightly-2023.6.3/colossalai/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/communication/collective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19462 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/communication/p2p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/communication/p2p_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/communication/ring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/communication/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.965204 colossalai-nightly-2023.6.3/colossalai/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/moe_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23924 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/parallel_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/parallel_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.965204 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/process_group_initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.965204 colossalai-nightly-2023.6.3/colossalai/context/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/random/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/random/seed_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/context/singleton_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.965204 colossalai-nightly-2023.6.3/colossalai/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/device/alpha_beta_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/device/calc_pipeline_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/device/device_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.965204 colossalai-nightly-2023.6.3/colossalai/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/_base_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.965204 colossalai-nightly-2023.6.3/colossalai/engine/gradient_accumulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/gradient_accumulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/gradient_accumulation/_gradient_accumulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.969204 colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_base_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_moe_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_zero_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.969204 colossalai-nightly-2023.6.3/colossalai/engine/schedule/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/schedule/_base_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/schedule/_non_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41258 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/schedule/_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/engine/schedule/_pipeline_schedule_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.969204 colossalai-nightly-2023.6.3/colossalai/fx/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19408 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/_meta_regist_12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/_meta_regist_13.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.969204 colossalai-nightly-2023.6.3/colossalai/fx/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44753 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/codegen/activation_checkpoint_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/graph_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.973204 colossalai-nightly-2023.6.3/colossalai/fx/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/passes/adding_split_node_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/passes/concrete_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/passes/meta_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/passes/passes_for_gpt2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/passes/shard_1d_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/passes/split_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/passes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.973204 colossalai-nightly-2023.6.3/colossalai/fx/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/dataflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.973204 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.973204 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/python_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.977204 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/torch_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/shard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/memory_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/opcount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/shard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/profiler/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.977204 colossalai-nightly-2023.6.3/colossalai/fx/tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/_meta_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/_symbolic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/_tracer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.977204 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.977204 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.981204 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26969 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.981204 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.981204 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.981204 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24624 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/fx/tracer/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/global_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.981204 colossalai-nightly-2023.6.3/colossalai/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/interface/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/interface/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.981204 colossalai-nightly-2023.6.3/colossalai/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.985204 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.989204 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/cpu_adam.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.989204 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    37586 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.989204 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/context.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/ls_cub.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48403 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22850 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/type_shim.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24864 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/scaled_softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.993204 colossalai-nightly-2023.6.3/colossalai/kernel/jit/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/jit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/jit/bias_dropout_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/jit/bias_gelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/jit/option.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.993204 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/fused_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/moe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/multi_head_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/scaled_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.993204 colossalai-nightly-2023.6.3/colossalai/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.993204 colossalai-nightly-2023.6.3/colossalai/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.997204 colossalai-nightly-2023.6.3/colossalai/nn/_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/addmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/element_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/embedding_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/_ops/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.997204 colossalai-nightly-2023.6.3/colossalai/nn/layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/base_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.997204 colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.997204 colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/experts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.997204 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_1d/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_1d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_1d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_1d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49753 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_1d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.997204 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2d/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50524 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.001204 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2p5d/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2p5d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37643 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2p5d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2p5d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50769 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2p5d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.001204 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_3d/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_3d/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22769 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_3d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_3d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51441 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_3d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.001204 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_sequence/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_sequence/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_sequence/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.001204 colossalai-nightly-2023.6.3/colossalai/nn/layer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/utils/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.001204 colossalai-nightly-2023.6.3/colossalai/nn/layer/vanilla/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/vanilla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/vanilla/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.001204 colossalai-nightly-2023.6.3/colossalai/nn/layer/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/layer/wrapper/pipeline_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.001204 colossalai-nightly-2023.6.3/colossalai/nn/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/loss/loss_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/loss/loss_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/loss/loss_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/loss/loss_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/loss/loss_moe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.005204 colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/delayed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/multistep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/onecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.005204 colossalai-nightly-2023.6.3/colossalai/nn/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/metric/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/metric/accuracy_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/metric/accuracy_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/metric/accuracy_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.005204 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/colossalai_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/fused_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/fused_lamb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/fused_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/hybrid_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/lamb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/lars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/optimizer/nvme_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.009204 colossalai-nightly-2023.6.3/colossalai/nn/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/data_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.009204 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.009204 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28600 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/copyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/colo_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/nn/parallel/reducer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.009204 colossalai-nightly-2023.6.3/colossalai/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/layer_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.009204 colossalai-nightly-2023.6.3/colossalai/pipeline/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/middleware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.009204 colossalai-nightly-2023.6.3/colossalai/pipeline/middleware/adaptor/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/middleware/adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/middleware/adaptor/fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/middleware/topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/pipelinable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/pipeline_process_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.013204 colossalai-nightly-2023.6.3/colossalai/pipeline/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59163 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/rpc/_pipeline_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/rpc/_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/rpc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/pipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.013204 colossalai-nightly-2023.6.3/colossalai/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/registry/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.013204 colossalai-nightly-2023.6.3/colossalai/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/colo_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/colo_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22269 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/comm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/compute_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.017204 colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/comm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/d_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25229 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/layout_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/sharding_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/dist_spec_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/distspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/op_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/param_op_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/process_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36495 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/shape_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/sharding_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/tensor_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.017204 colossalai-nightly-2023.6.3/colossalai/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/testing/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/testing/pytest_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/testing/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.017204 colossalai-nightly-2023.6.3/colossalai/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/trainer/_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.017204 colossalai-nightly-2023.6.3/colossalai/trainer/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/trainer/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_base_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_checkpoint_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_commons_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13106 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_log_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_lr_scheduler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_metric_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.017204 colossalai-nightly-2023.6.3/colossalai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/activation_checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.021204 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint/module_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.021204 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/convertor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/checkpointing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.021204 colossalai-nightly-2023.6.3/colossalai/utils/data_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/data_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/data_sampler/base_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/data_sampler/data_parallel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.021204 colossalai-nightly-2023.6.3/colossalai/utils/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/model/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/model/lazy_init_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/moe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.021204 colossalai-nightly-2023.6.3/colossalai/utils/multi_tensor_apply/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/multi_tensor_apply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.021204 colossalai-nightly-2023.6.3/colossalai/utils/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/profiler/extention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.025204 colossalai-nightly-2023.6.3/colossalai/utils/profiler/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/profiler/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/profiler/legacy/comm_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/profiler/legacy/pcie_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/profiler/legacy/prof_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/profiler/stateful_tensor_mem_extention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.025204 colossalai-nightly-2023.6.3/colossalai/utils/rank_recorder/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/rank_recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/rank_recorder/rank_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.025204 colossalai-nightly-2023.6.3/colossalai/utils/tensor_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/tensor_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/tensor_detector/tensor_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.025204 colossalai-nightly-2023.6.3/colossalai/zero/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.025204 colossalai-nightly-2023.6.3/colossalai/zero/gemini/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.025204 colossalai-nightly-2023.6.3/colossalai/zero/gemini/chunk/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/chunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22078 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/chunk/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/chunk/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/chunk/search_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/chunk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/colo_init_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/gemini_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/gemini_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/gemini_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/gemini_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.029204 colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/memory_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/param_runtime_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/placement_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/gemini/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.029204 colossalai-nightly-2023.6.3/colossalai/zero/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.029204 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/gemini_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.029204 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/ophooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/ophooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/ophooks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.029204 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/paramhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/paramhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/stateful_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/tensor_placement_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/tensor_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.029204 colossalai-nightly-2023.6.3/colossalai/zero/legacy/init_ctx/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/init_ctx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/init_ctx/init_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.033204 colossalai-nightly-2023.6.3/colossalai/zero/legacy/shard_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/shard_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/shard_utils/base_shard_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/shard_utils/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.033204 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/reduce_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29015 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/sharded_model_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/zero_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.033204 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.033204 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_param/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_param/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_param/sharded_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_param/sharded_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.033204 colossalai-nightly-2023.6.3/colossalai/zero/low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/low_level/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.033204 colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/base_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/bucket_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/gradient_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/tensor_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25694 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/low_level/low_level_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/colossalai/zero/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.037204 colossalai-nightly-2023.6.3/colossalai_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-06-03 00:15:28.000000 colossalai-nightly-2023.6.3/colossalai_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37387 2023-06-03 00:15:28.000000 colossalai-nightly-2023.6.3/colossalai_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 00:15:28.000000 colossalai-nightly-2023.6.3/colossalai_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 00:15:28.000000 colossalai-nightly-2023.6.3/colossalai_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-03 00:15:28.000000 colossalai-nightly-2023.6.3/colossalai_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-03 00:15:28.000000 colossalai-nightly-2023.6.3/colossalai_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.037204 colossalai-nightly-2023.6.3/op_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/op_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/op_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/op_builder/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/op_builder/fused_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/op_builder/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/op_builder/moe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/op_builder/multi_head_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/op_builder/scaled_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/op_builder/scaled_upper_triangle_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/op_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.037204 colossalai-nightly-2023.6.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 00:15:29.073204 colossalai-nightly-2023.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:28.929204 colossalai-nightly-2023.6.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/components_to_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/albert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/beit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/hanging_param_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/inline_op_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/nested_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/repeated_computed_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/simple_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/components_to_test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/utils/dummy_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/components_to_test/utils/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/kit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/kit/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/kit/model_zoo/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/diffusers/diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/kit/model_zoo/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/timm/timm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchaudio/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchaudio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchaudio/torchaudio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchrec/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchrec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchrec/torchrec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchvision/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchvision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchvision/torchvision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/albert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/t5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.041204 colossalai-nightly-2023.6.3/tests/test_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.049204 colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/test_bias_addition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/test_mod_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/test_nested_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/test_shape_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/test_symbolic_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.053204 colossalai-nightly-2023.6.3/tests/test_analyzer/test_subclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_subclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_subclasses/test_aten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_subclasses/test_flop_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_analyzer/test_subclasses/test_meta_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.053204 colossalai-nightly-2023.6.3/tests/test_auto_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.053204 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_pass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_pass/test_node_converting_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.057204 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.057204 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:29.069204 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-03 00:15:17.000000 colossalai-nightly-2023.6.3/version.txt
```

### Comparing `colossalai-nightly-2023.6.17/LICENSE` & `colossalai-nightly-2023.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/PKG-INFO` & `colossalai-nightly-2023.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colossalai-nightly
-Version: 2023.6.17
+Version: 2023.6.3
 Summary: An integrated large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org
 License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.6.17 Summary: An
+Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.6.3 Summary: An
 integrated large-scale model training system with efficient parallelization
 techniques Home-page: https://www.colossalai.org License: Apache Software
 License 2.0 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/
 discussions Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/
 issues Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io Project-URL:
 Github, https://github.com/hpcaitech/ColossalAI Description: # Colossal-AI
```

### Comparing `colossalai-nightly-2023.6.17/README.md` & `colossalai-nightly-2023.6.3/README.md`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/_analyzer/_subclasses/_meta_registration.py` & `colossalai-nightly-2023.6.3/colossalai/_analyzer/_subclasses/_meta_registration.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/_analyzer/_subclasses/_monkey_patch.py` & `colossalai-nightly-2023.6.3/colossalai/_analyzer/_subclasses/_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/_analyzer/_subclasses/flop_tensor.py` & `colossalai-nightly-2023.6.3/colossalai/_analyzer/_subclasses/flop_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/_analyzer/_subclasses/meta_tensor.py` & `colossalai-nightly-2023.6.3/colossalai/_analyzer/_subclasses/meta_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/codegen.py` & `colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/codegen.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/graph_module.py` & `colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/graph_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/node_util.py` & `colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/node_util.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/passes/graph_profile.py` & `colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/passes/graph_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/passes/shape_prop.py` & `colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/passes/shape_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/symbolic_profile.py` & `colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/symbolic_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/tracer/bias_addition.py` & `colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/tracer/bias_addition.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/tracer/custom_leaf_module.py` & `colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/tracer/custom_leaf_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/tracer/proxy.py` & `colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/tracer/proxy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/tracer/symbolic_trace.py` & `colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/tracer/symbolic_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/_analyzer/fx/tracer/tracer.py` & `colossalai-nightly-2023.6.3/colossalai/_analyzer/fx/tracer/tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/amp/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/amp/apex_amp/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/amp/apex_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/amp/apex_amp/apex_amp.py` & `colossalai-nightly-2023.6.3/colossalai/amp/apex_amp/apex_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/_fp16_optimizer.py` & `colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/_fp16_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/_utils.py` & `colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py` & `colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py` & `colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py` & `colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/amp/naive_amp/naive_amp.py` & `colossalai-nightly-2023.6.3/colossalai/amp/naive_amp/naive_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/amp/torch_amp/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/amp/torch_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/amp/torch_amp/_grad_scaler.py` & `colossalai-nightly-2023.6.3/colossalai/amp/torch_amp/_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/amp/torch_amp/torch_amp.py` & `colossalai-nightly-2023.6.3/colossalai/amp/torch_amp/torch_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/checkpoint/operation.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/checkpoint/operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/meta_registry/where.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/meta_registry/where.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/registry.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/meta_profiler/shard_metainfo.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/meta_profiler/shard_metainfo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/offload/amp_optimizer.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/amp_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/offload/base_offload_module.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/base_offload_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/offload/mem_optimize.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/mem_optimize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/offload/region.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/region.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/offload/region_manager.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/region_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/offload/runtime.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/runtime.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/offload/solver.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/solver.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/offload/training_simulator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/training_simulator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/offload/util.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/offload/util.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/passes/comm_metainfo_pass.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/comm_metainfo_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/passes/meta_info_prop.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/meta_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/passes/runtime_apply_pass.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/runtime_apply_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/passes/runtime_preparation_pass.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/passes/runtime_preparation_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/constants.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/initialize.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/initialize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/registry.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/options.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/options.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/sharding_strategy.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/sharding_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/solver/solver.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/solver/solver.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/utils/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/utils/broadcast.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/broadcast.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/utils/factory.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/factory.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/utils/misc.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/misc.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/utils/reshape.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/reshape.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/auto_parallel/tensor_shard/utils/sharding.py` & `colossalai-nightly-2023.6.3/colossalai/auto_parallel/tensor_shard/utils/sharding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/booster/accelerator.py` & `colossalai-nightly-2023.6.3/colossalai/booster/accelerator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/booster/booster.py` & `colossalai-nightly-2023.6.3/colossalai/booster/booster.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,19 +21,19 @@
     """
     Booster is a high-level API for training neural networks. It provides a unified interface for
     training with different precision, accelerator, and plugin.
 
     Examples:
         ```python
         colossalai.launch(...)
-        plugin = GeminiPlugin(...)
+        plugin = GeminiPlugin(stage=3, ...)
         booster = Booster(precision='fp16', plugin=plugin)
 
         model = GPT2()
-        optimizer = HybridAdam(model.parameters())
+        optimizer = Adam(model.parameters())
         dataloader = Dataloader(Dataset)
         lr_scheduler = LinearWarmupScheduler()
         criterion = GPTLMLoss()
 
         model, optimizer, lr_scheduler, dataloader = booster.boost(model, optimizer, lr_scheduler, dataloader)
 
         for epoch in range(max_epochs):
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/booster/mixed_precision/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/booster/mixed_precision/fp16_apex.py` & `colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/fp16_apex.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/booster/mixed_precision/fp16_naive.py` & `colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/fp16_naive.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/booster/mixed_precision/fp16_torch.py` & `colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/fp16_torch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/booster/mixed_precision/mixed_precision_base.py` & `colossalai-nightly-2023.6.3/colossalai/booster/mixed_precision/mixed_precision_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/booster/plugin/dp_plugin_base.py` & `colossalai-nightly-2023.6.3/colossalai/booster/plugin/dp_plugin_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/booster/plugin/gemini_plugin.py` & `colossalai-nightly-2023.6.3/colossalai/booster/plugin/gemini_plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,17 +19,14 @@
 from colossalai.zero import GeminiDDP, zero_model_wrapper, zero_optim_wrapper
 from colossalai.zero.gemini.memory_tracer import MemStats
 
 from .dp_plugin_base import DPPluginBase
 
 __all__ = ['GeminiPlugin']
 
-SUPPORTED_PRECISION = ['fp16', 'bf16']
-PRECISION_STR_TO_DTYPE = {'fp16': torch.half, 'bf16': torch.bfloat16}
-
 
 class GeminiCheckpointIO(GeneralCheckpointIO):
 
     def __init__(self) -> None:
         super().__init__()
         self.coordinator = DistCoordinator()
 
@@ -170,15 +167,14 @@
         >>> train_dataloader = plugin.prepare_dataloader(train_dataset, batch_size=8)
         >>> booster = Booster(plugin=plugin)
         >>> model, optimizer, train_dataloader, criterion = booster.boost(model, optimizer, train_dataloader, criterion)
 
     Args:
         device (torch.device): device to place the model.
         placement_policy (str, optional): "cpu", "cuda", "auto". Defaults to "cpu".
-        precision (str, optional): precision. Support 'fp16' and 'bf16'. Defaults to 'fp16'.
         pin_memory (bool, optional): use pin memory on CPU. Defaults to False.
         force_outputs_fp32 (bool, optional): force outputs are fp32. Defaults to False.
         strict_ddp_mode (bool, optional): use strict ddp mode (only use dp without other parallelism). Defaults to False.
         search_range_mb (int, optional): chunk size searching range in MegaByte. Defaults to 32.
         hidden_dim (int, optional): the hidden dimension of DNN.
             Users can provide this argument to speed up searching.
             If users do not know this argument before training, it is ok. We will use a default value 1024.
@@ -203,15 +199,14 @@
         verbose (bool, optional): verbose mode. Debug info including chunk search result will be printed. Defaults to False.
     """
 
     def __init__(
         self,
         device: Optional[torch.device] = None,
         placement_policy: str = "cpu",
-        precision: str = "fp16",
         pin_memory: bool = False,
         force_outputs_fp32: bool = False,
         strict_ddp_mode: bool = False,
         search_range_mb: int = 32,
         hidden_dim: Optional[int] = None,
         min_chunk_size_mb: float = 32,
         memstats: Optional[MemStats] = None,
@@ -224,26 +219,24 @@
         hysteresis: int = 2,
         max_scale: float = 2**32,
         max_norm: float = 0.0,
         norm_type: float = 2.0,
         verbose: bool = False,
     ) -> None:
         super().__init__()
-        assert precision in SUPPORTED_PRECISION, f'precision {precision} is not supported'
         self.gemini_config = dict(
             device=(device or get_current_device()),
             placement_policy=placement_policy,
             pin_memory=pin_memory,
             force_outputs_fp32=force_outputs_fp32,
             strict_ddp_mode=strict_ddp_mode,
             search_range_mb=search_range_mb,
             hidden_dim=hidden_dim,
             min_chunk_size_mb=min_chunk_size_mb,
             memstats=memstats,
-            mixed_precision=PRECISION_STR_TO_DTYPE[precision],
         )
         self.zero_optim_config = dict(gpu_margin_mem_ratio=gpu_margin_mem_ratio,)
         self.optim_kwargs = dict(initial_scale=initial_scale,
                                  growth_factor=growth_factor,
                                  backoff_factor=backoff_factor,
                                  growth_interval=growth_interval,
                                  hysteresis=hysteresis,
@@ -256,15 +249,15 @@
     def support_no_sync(self) -> bool:
         return False
 
     def control_precision(self) -> bool:
         return True
 
     def supported_precisions(self) -> List[str]:
-        return SUPPORTED_PRECISION
+        return ['fp16']
 
     def control_device(self) -> bool:
         return True
 
     def supported_devices(self) -> List[str]:
         return ['cuda']
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/booster/plugin/low_level_zero_plugin.py` & `colossalai-nightly-2023.6.3/colossalai/booster/plugin/low_level_zero_plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import warnings
-from functools import partial
 from typing import Callable, Iterator, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 from torch import Tensor
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
@@ -17,23 +16,20 @@
 
 from .dp_plugin_base import DPPluginBase
 from .torch_ddp_plugin import TorchDDPCheckpointIO
 
 __all__ = ['LowLevelZeroPlugin']
 
 
-def _convert_floating_point(x, dtype: torch.dtype = torch.float16):
+def _convert_to_fp16(x):
     if isinstance(x, torch.Tensor) and torch.is_floating_point(x):
-        return x.to(dtype)
+        return x.half()
     return x
 
 
-SUPPORTED_PRECISION = ['fp16', 'bf16', 'fp32']
-
-
 class LowLevelZeroCheckpointIO(TorchDDPCheckpointIO):
 
     def save_unsharded_optimizer(self, optimizer: Optimizer, checkpoint: str, gather_dtensor: bool):
         """
         Save optimizer to checkpoint but only on master process.
         """
         # TODO(ver217): optimizer state dict is sharded, and cannot get full state dict now
@@ -49,32 +45,25 @@
         super().load_optimizer(optimizer, checkpoint)
 
 
 class LowLevelZeroModel(ModelWrapper):
 
     def __init__(self, module: nn.Module, stage: int, precision: str) -> None:
         super().__init__(module)
-        self.dtype = None
-        if precision == 'fp16':
-            self.dtype = torch.float16
-        elif precision == 'bf16':
-            self.dtype = torch.bfloat16
+        self.convert_inputs = (precision == 'fp16')
         module = zero_model_wrapper(module, zero_stage=stage)
-        if self.dtype is not None:
-            module = module.to(self.dtype)
+        if precision == 'fp16':
+            module = module.half()
         module = module.to(get_current_device())
         self.module = module
-        self.convert_fn = None
-        if self.dtype is not None:
-            self.convert_fn = partial(_convert_floating_point, dtype=self.dtype)
 
     def forward(self, *args, **kwargs):
-        if self.convert_fn is not None:
-            args = tree_map(self.convert_fn, args)
-            kwargs = tree_map(self.convert_fn, kwargs)
+        if self.convert_inputs:
+            args = tree_map(_convert_to_fp16, args)
+            kwargs = tree_map(_convert_to_fp16, kwargs)
         return super().forward(*args, **kwargs)
 
 
 class LowLevelZeroOptimizer(OptimizerWrapper):
 
     def __init__(self,
                  module: nn.Module,
@@ -117,15 +106,15 @@
 
         >>> train_dataloader = plugin.prepare_dataloader(train_dataset, batch_size=8)
         >>> booster = Booster(plugin=plugin)
         >>> model, optimizer, train_dataloader, criterion = booster.boost(model, optimizer, train_dataloader, criterion)
 
     Args:
         strage (int, optional): ZeRO stage. Defaults to 1.
-        precision (str, optional): precision. Support 'fp16', 'bf16' and 'fp32'. Defaults to 'fp16'.
+        precision (str, optional): precision. Support 'fp16' and 'fp32'. Defaults to 'fp16'.
         initial_scale (float, optional): Initial scale used by DynamicGradScaler. Defaults to 2**32.
         min_scale (float, optional): Min scale used by DynamicGradScaler. Defaults to 1.
         growth_factor (float, optional): growth_factor used by DynamicGradScaler. Defaults to 2.
         backoff_factor (float, optional): backoff_factor used by DynamicGradScaler. Defaults to 0.5.
         growth_interval (float, optional): growth_interval used by DynamicGradScaler. Defaults to 1000.
         hysteresis (float, optional): hysteresis used by DynamicGradScaler. Defaults to 2.
         max_scale (int, optional): max_scale used by DynamicGradScaler. Defaults to 2**32.
@@ -156,15 +145,15 @@
         communication_dtype: Optional[torch.dtype] = None,
         overlap_communication: bool = True,
         cpu_offload: bool = False,
         verbose: bool = False,
     ) -> None:
         super().__init__()
         assert stage in (1, 2), f'LowLevelZeroPlugin only supports stage 1/2 training'
-        assert precision in SUPPORTED_PRECISION, f'LowLevelZeroPlugin only supports {SUPPORTED_PRECISION} training'
+        assert precision in ('fp16', 'fp32'), f'LowLevelZeroPlugin only supports fp16/fp32 training'
 
         self.stage = stage
         self.precision = precision
         self.zero_optim_config = dict(reduce_bucket_size=reduce_bucket_size_in_m * 1024 * 1024,
                                       communication_dtype=communication_dtype,
                                       overlap_communication=overlap_communication,
                                       cpu_offload=cpu_offload)
@@ -182,15 +171,15 @@
     def support_no_sync(self) -> bool:
         return False
 
     def control_precision(self) -> bool:
         return True
 
     def supported_precisions(self) -> List[str]:
-        return SUPPORTED_PRECISION
+        return ['fp16', 'fp32']
 
     def control_device(self) -> bool:
         return True
 
     def supported_devices(self) -> List[str]:
         return ['cuda']
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/booster/plugin/plugin_base.py` & `colossalai-nightly-2023.6.3/colossalai/booster/plugin/plugin_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/booster/plugin/torch_ddp_plugin.py` & `colossalai-nightly-2023.6.3/colossalai/booster/plugin/torch_ddp_plugin.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/booster/plugin/torch_fsdp_plugin.py` & `colossalai-nightly-2023.6.3/colossalai/booster/plugin/torch_fsdp_plugin.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/builder/builder.py` & `colossalai-nightly-2023.6.3/colossalai/builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/checkpoint_io/checkpoint_io_base.py` & `colossalai-nightly-2023.6.3/colossalai/checkpoint_io/checkpoint_io_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/checkpoint_io/general_checkpoint_io.py` & `colossalai-nightly-2023.6.3/colossalai/checkpoint_io/general_checkpoint_io.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/checkpoint_io/index_file.py` & `colossalai-nightly-2023.6.3/colossalai/checkpoint_io/index_file.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/checkpoint_io/utils.py` & `colossalai-nightly-2023.6.3/colossalai/checkpoint_io/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/cli/benchmark/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/cli/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/cli/benchmark/benchmark.py` & `colossalai-nightly-2023.6.3/colossalai/cli/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/cli/benchmark/utils.py` & `colossalai-nightly-2023.6.3/colossalai/cli/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/cli/check/check_installation.py` & `colossalai-nightly-2023.6.3/colossalai/cli/check/check_installation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/cli/launcher/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/cli/launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/cli/launcher/hostinfo.py` & `colossalai-nightly-2023.6.3/colossalai/cli/launcher/hostinfo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/cli/launcher/multinode_runner.py` & `colossalai-nightly-2023.6.3/colossalai/cli/launcher/multinode_runner.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/cli/launcher/run.py` & `colossalai-nightly-2023.6.3/colossalai/cli/launcher/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             else:
                 extra_launch_args_dict[arg] = None
         extra_launch_args = extra_launch_args_dict
     else:
         extra_launch_args = dict()
 
     torch_version = version.parse(torch.__version__)
-    assert torch_version.major >= 1
+    assert torch_version.major == 1
 
     if torch_version.minor < 9:
         cmd = [
             sys.executable, "-m", "torch.distributed.launch", f"--nproc_per_node={nproc_per_node}",
             f"--master_addr={master_addr}", f"--master_port={master_port}", f"--nnodes={num_nodes}",
             f"--node_rank={node_rank}"
         ]
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/cluster/device_mesh_manager.py` & `colossalai-nightly-2023.6.3/colossalai/cluster/device_mesh_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/cluster/dist_coordinator.py` & `colossalai-nightly-2023.6.3/colossalai/cluster/dist_coordinator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/cluster/process_group_manager.py` & `colossalai-nightly-2023.6.3/colossalai/cluster/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/communication/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/communication/collective.py` & `colossalai-nightly-2023.6.3/colossalai/communication/collective.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/communication/p2p.py` & `colossalai-nightly-2023.6.3/colossalai/communication/p2p.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/communication/p2p_v2.py` & `colossalai-nightly-2023.6.3/colossalai/communication/p2p_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/communication/ring.py` & `colossalai-nightly-2023.6.3/colossalai/communication/ring.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/communication/utils.py` & `colossalai-nightly-2023.6.3/colossalai/communication/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/constants.py` & `colossalai-nightly-2023.6.3/colossalai/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/context/config.py` & `colossalai-nightly-2023.6.3/colossalai/context/config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/context/moe_context.py` & `colossalai-nightly-2023.6.3/colossalai/context/moe_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/context/parallel_context.py` & `colossalai-nightly-2023.6.3/colossalai/context/parallel_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/context/parallel_mode.py` & `colossalai-nightly-2023.6.3/colossalai/context/parallel_mode.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/initializer_1d.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_1d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/initializer_2d.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/initializer_2p5d.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/initializer_3d.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/initializer_data.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_data.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/initializer_model.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/initializer_pipeline.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_pipeline.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/initializer_sequence.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_sequence.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/initializer_tensor.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/initializer_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/context/process_group_initializer/process_group_initializer.py` & `colossalai-nightly-2023.6.3/colossalai/context/process_group_initializer/process_group_initializer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/context/random/_helper.py` & `colossalai-nightly-2023.6.3/colossalai/context/random/_helper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/context/random/seed_manager.py` & `colossalai-nightly-2023.6.3/colossalai/context/random/seed_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/context/singleton_meta.py` & `colossalai-nightly-2023.6.3/colossalai/context/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/device/alpha_beta_profiler.py` & `colossalai-nightly-2023.6.3/colossalai/device/alpha_beta_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/device/calc_pipeline_strategy.py` & `colossalai-nightly-2023.6.3/colossalai/device/calc_pipeline_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/device/device_mesh.py` & `colossalai-nightly-2023.6.3/colossalai/device/device_mesh.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/engine/_base_engine.py` & `colossalai-nightly-2023.6.3/colossalai/engine/_base_engine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/engine/gradient_accumulation/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/engine/gradient_accumulation/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/engine/gradient_accumulation/_gradient_accumulation.py` & `colossalai-nightly-2023.6.3/colossalai/engine/gradient_accumulation/_gradient_accumulation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/engine/gradient_handler/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/engine/gradient_handler/_base_gradient_handler.py` & `colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_base_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py` & `colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/engine/gradient_handler/_moe_gradient_handler.py` & `colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_moe_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py` & `colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py` & `colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/engine/gradient_handler/_zero_gradient_handler.py` & `colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/_zero_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/engine/gradient_handler/utils.py` & `colossalai-nightly-2023.6.3/colossalai/engine/gradient_handler/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/engine/schedule/_base_schedule.py` & `colossalai-nightly-2023.6.3/colossalai/engine/schedule/_base_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/engine/schedule/_non_pipeline_schedule.py` & `colossalai-nightly-2023.6.3/colossalai/engine/schedule/_non_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/engine/schedule/_pipeline_schedule.py` & `colossalai-nightly-2023.6.3/colossalai/engine/schedule/_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/engine/schedule/_pipeline_schedule_v2.py` & `colossalai-nightly-2023.6.3/colossalai/engine/schedule/_pipeline_schedule_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/_compatibility.py` & `colossalai-nightly-2023.6.3/colossalai/fx/_compatibility.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/_meta_regist_12.py` & `colossalai-nightly-2023.6.3/colossalai/fx/_meta_regist_12.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/_meta_regist_13.py` & `colossalai-nightly-2023.6.3/colossalai/fx/_meta_regist_13.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/codegen/activation_checkpoint_codegen.py` & `colossalai-nightly-2023.6.3/colossalai/fx/codegen/activation_checkpoint_codegen.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/graph_module.py` & `colossalai-nightly-2023.6.3/colossalai/fx/graph_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/passes/adding_split_node_pass.py` & `colossalai-nightly-2023.6.3/colossalai/fx/passes/adding_split_node_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/passes/concrete_info_prop.py` & `colossalai-nightly-2023.6.3/colossalai/fx/passes/concrete_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/passes/meta_info_prop.py` & `colossalai-nightly-2023.6.3/colossalai/fx/passes/meta_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/passes/passes_for_gpt2_test.py` & `colossalai-nightly-2023.6.3/colossalai/fx/passes/passes_for_gpt2_test.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/passes/shard_1d_pass.py` & `colossalai-nightly-2023.6.3/colossalai/fx/passes/shard_1d_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/passes/split_module.py` & `colossalai-nightly-2023.6.3/colossalai/fx/passes/split_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/passes/utils.py` & `colossalai-nightly-2023.6.3/colossalai/fx/passes/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/constants.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/dataflow.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/dataflow.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/constants.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_function/activation_function.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/activation_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_function/embedding.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_function/normalization.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_function/pooling.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_module/activation_function.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/activation_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_module/attention.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_module/convolution.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_module/normalization.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_module/pooling.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/profiler_module/rnn.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/profiler_module/rnn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/registry.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/experimental/shard_utils.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/experimental/shard_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/memory_utils.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/memory_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/opcount.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/opcount.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/profiler.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/shard_utils.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/shard_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/profiler/tensor.py` & `colossalai-nightly-2023.6.3/colossalai/fx/profiler/tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/proxy.py` & `colossalai-nightly-2023.6.3/colossalai/fx/proxy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/_meta_trace.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/_meta_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/_symbolic_trace.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/_symbolic_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/_tracer_utils.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/_tracer_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/experimental.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/experimental.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_function/convolution.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_function/embedding.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_function/normalization.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_module/convolution.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_module/normalization.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_module/pooling.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/meta_patch/patched_module/rnn.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/meta_patch/patched_module/rnn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/registry.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/fx/tracer/tracer.py` & `colossalai-nightly-2023.6.3/colossalai/fx/tracer/tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/global_variables.py` & `colossalai-nightly-2023.6.3/colossalai/global_variables.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/initialize.py` & `colossalai-nightly-2023.6.3/colossalai/initialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
                lr_scheduler: Optional[_LRScheduler] = None,
                ophooks: Optional[List[BaseOpHook]] = None,
                verbose: bool = True) -> Tuple[Engine, DataLoader, DataLoader, _LRScheduler]:
     """Core function to wrap the essential training components with our functionality based on the config which is
     loaded into gpc.config.
 
     Args:
-        model (:class:`torch.nn.Module` or Callable): Your model instance or a function to build the model.
+        model (:class:`torch.nn.Module` or Callbale): Your model instance or a function to build the model.
         optimizer (:class:`torch.optim.optimizer.Optimizer` or :class:`Type[torch.optim.optimizer]`):
             Your optimizer instance.
         criterion (:class:`torch.nn.modules.loss._Loss`, optional): Your criterion instance.
         train_dataloader (:class:`torch.utils.data.DataLoader`, optional): Dataloader for training.
         test_dataloader (:class:`torch.utils.data.DataLoader`, optional): Dataloader for testing.
         lr_scheduler (:class:`torch.nn.lr_scheduler._LRScheduler`, optional): Your lr scheduler instance, optional.
         verbose (bool, optional): Whether to print logs.
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/interface/model.py` & `colossalai-nightly-2023.6.3/colossalai/interface/model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/interface/optimizer.py` & `colossalai-nightly-2023.6.3/colossalai/interface/optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/cpu_adam.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/cpu_adam.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/context.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/context.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/csrc/type_shim.h` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/csrc/type_shim.h`

 * *Files 10% similar despite different names*

```diff
@@ -167,29 +167,14 @@
     using g_scalar_t_##LEVEL = at::Half;                                       \
     using p_scalar_t_##LEVEL = float;                                          \
     __VA_ARGS__;                                                               \
   } else if (GTYPE == at::ScalarType::Half && PTYPE == at::ScalarType::Half) { \
     using g_scalar_t_##LEVEL = at::Half;                                       \
     using p_scalar_t_##LEVEL = at::Half;                                       \
     __VA_ARGS__;                                                               \
-  } else if (GTYPE == at::ScalarType::Float &&                                 \
-             PTYPE == at::ScalarType::BFloat16) {                              \
-    using g_scalar_t_##LEVEL = float;                                          \
-    using p_scalar_t_##LEVEL = at::BFloat16;                                   \
-    __VA_ARGS__;                                                               \
-  } else if (GTYPE == at::ScalarType::BFloat16 &&                              \
-             PTYPE == at::ScalarType::Float) {                                 \
-    using g_scalar_t_##LEVEL = at::BFloat16;                                   \
-    using p_scalar_t_##LEVEL = float;                                          \
-    __VA_ARGS__;                                                               \
-  } else if (GTYPE == at::ScalarType::BFloat16 &&                              \
-             PTYPE == at::ScalarType::BFloat16) {                              \
-    using g_scalar_t_##LEVEL = at::BFloat16;                                   \
-    using p_scalar_t_##LEVEL = at::BFloat16;                                   \
-    __VA_ARGS__;                                                               \
   } else {                                                                     \
     AT_ERROR(#NAME, "not implemented for '", toString(GTYPE), toString(PTYPE), \
              "'");                                                             \
   }
 
 template <typename T>
 __device__ __forceinline__ T reduce_block_into_lanes(
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/flash_attention.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/flash_attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/layer_norm.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/layer_norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/multihead_attention.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/cuda_native/scaled_softmax.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/cuda_native/scaled_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/jit/bias_dropout_add.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/jit/bias_dropout_add.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/jit/bias_gelu.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/jit/bias_gelu.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/jit/option.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/jit/option.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/op_builder/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/op_builder/builder.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/op_builder/cpu_adam.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/op_builder/fused_optim.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/fused_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/op_builder/layernorm.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/op_builder/moe.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/op_builder/multi_head_attn.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/multi_head_attn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/op_builder/scaled_masked_softmax.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/scaled_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/kernel/op_builder/utils.py` & `colossalai-nightly-2023.6.3/colossalai/kernel/op_builder/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/lazy/lazy_init.py` & `colossalai-nightly-2023.6.3/colossalai/utils/model/experimental.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ]
 
 _EARLY_MATERIALIZED_OPS = ['__getitem__', 'split']
 
 # If your intent is to change the metadata of a Tensor (such as sizes / strides / storage / storage_offset)
 # without autograd tracking the change, remove the .data / .detach() call and wrap the change in a `with torch.no_grad():` block.
 # These ops cannot be unwrapped using .data
-_CHANGE_META_OPS = ['_cudnn_rnn_flatten_weight', 'requires_grad_', '__get__', '__set__', 'numel', 'size', 'dim']
+_CHANGE_META_OPS = ['_cudnn_rnn_flatten_weight', 'requires_grad_', '__get__', '__set__']
 
 _LEGACY_TENSOR_CONSTRUCTOR = {
     'FloatTensor': torch.float,
     'DoubleTensor': torch.double,
     'HalfTensor': torch.half,
     'BFloat16Tensor': torch.bfloat16,
     'ByteTensor': torch.uint8,
@@ -346,22 +346,15 @@
             # if self is materialized, return self
             new_tensor = self.materialize() if type(self) is LazyTensor else self
             copied = new_tensor.detach().clone()
             if new_tensor.requires_grad:
                 copied.requires_grad_()
             return copied
 
-        if self._materialized_data is not None:
-            # self is early materialized
-            copied = self._materialized_data.detach().clone()
-            if self.requires_grad:
-                copied.requires_grad_()
-            target = LazyTensor(lambda: None, concrete_data=copied)
-        else:
-            target = LazyTensor(factory_fn, meta_data=self._meta_data)
+        target = LazyTensor(factory_fn, meta_data=self._meta_data)
 
         memo[id(self)] = target
         return target
 
     @property
     def data(self):
         return self
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/logging/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/logging/logger.py` & `colossalai-nightly-2023.6.3/colossalai/logging/logger.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/_ops/_utils.py` & `colossalai-nightly-2023.6.3/colossalai/nn/_ops/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/_ops/addmm.py` & `colossalai-nightly-2023.6.3/colossalai/nn/_ops/addmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/_ops/batch_norm.py` & `colossalai-nightly-2023.6.3/colossalai/nn/_ops/batch_norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/_ops/element_wise.py` & `colossalai-nightly-2023.6.3/colossalai/nn/_ops/element_wise.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/_ops/embedding.py` & `colossalai-nightly-2023.6.3/colossalai/nn/_ops/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/_ops/embedding_bag.py` & `colossalai-nightly-2023.6.3/colossalai/nn/_ops/embedding_bag.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/_ops/layernorm.py` & `colossalai-nightly-2023.6.3/colossalai/nn/_ops/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/_ops/linear.py` & `colossalai-nightly-2023.6.3/colossalai/nn/_ops/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/_ops/loss.py` & `colossalai-nightly-2023.6.3/colossalai/nn/_ops/loss.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/_ops/view.py` & `colossalai-nightly-2023.6.3/colossalai/nn/_ops/view.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/init.py` & `colossalai-nightly-2023.6.3/colossalai/nn/init.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/base_layer.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/base_layer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/colossalai_layer/_utils.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/colossalai_layer/dropout.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/dropout.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/colossalai_layer/embedding.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/colossalai_layer/linear.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/colossalai_layer/normalization.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/colossalai_layer/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/moe/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/moe/_operation.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/moe/checkpoint.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/moe/experts.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/experts.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/moe/layers.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/moe/routers.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/routers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/moe/utils.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/moe/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_1d/_operation.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_1d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_1d/_utils.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_1d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_1d/layers.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_1d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_2d/_operation.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_2d/_utils.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_2d/layers.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_2p5d/_operation.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2p5d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_2p5d/_utils.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2p5d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_2p5d/layers.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_2p5d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_3d/_operation.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_3d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_3d/_utils.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_3d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_3d/layers.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_3d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_sequence/_operation.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_sequence/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/parallel_sequence/layers.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/parallel_sequence/layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         bias: If true, add bias
         init_method: method to initialize weights. Note that bias is always set
                      to zero.
         stride: For the strided linear layers.
         keep_master_weight_for_test: This was added for testing and should be
                                      set to False. It returns the master weights
                                      used for initialization.
-        skip_bias_add: This was added to enable performance optimizations where bias
+        skip_bias_add: This was added to enable performance optimations where bias
                        can be fused with other elementwise operations. we skip
                        adding bias but instead return it.
     """
 
     def __init__(self, input_size, output_size, bias=True, skip_bias_add=False):
         super(_Linear, self).__init__()
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/utils/common.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/utils/common.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/vanilla/layers.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/vanilla/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/layer/wrapper/pipeline_wrapper.py` & `colossalai-nightly-2023.6.3/colossalai/nn/layer/wrapper/pipeline_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/loss/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/nn/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/loss/loss_1d.py` & `colossalai-nightly-2023.6.3/colossalai/nn/loss/loss_1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
         # Maximum value along vocab dimension across all GPUs.
         logits_max = torch.max(vocab_parallel_logits, dim=-1)[0]
         torch.distributed.all_reduce(logits_max, op=torch.distributed.ReduceOp.MAX, group=process_group)
         # Subtract the maximum value.
         vocab_parallel_logits.sub_(logits_max.unsqueeze(dim=-1))
 
-        # Get the partition's vocab indices
+        # Get the partition's vocab indecies
         partition_vocab_size = vocab_parallel_logits.size()[-1]
         rank = dist.get_rank(process_group)
         vocab_start_index = partition_vocab_size * rank
         vocab_end_index = vocab_start_index + partition_vocab_size
 
         # Create a mask of valid vocab ids (1 means it needs to be masked).
         target_mask = (targets < vocab_start_index) | (targets >= vocab_end_index)
@@ -57,18 +57,18 @@
         ctx.save_for_backward(exp_logits, target_mask, masked_target_1d)
         return loss
 
     @staticmethod
     @custom_bwd
     def backward(ctx, grad_output):
 
-        # Retrieve tensors from the forward path.
+        # Retreive tensors from the forward path.
         softmax, target_mask, masked_target_1d = ctx.saved_tensors
 
-        # All the inputs have softmax as their gradient.
+        # All the inputs have softmax as thier gradient.
         grad_input = softmax
         # For simplicity, work with the 2D gradient.
         partition_vocab_size = softmax.size()[-1]
         grad_2d = grad_input.view(-1, partition_vocab_size)
 
         # Add the gradient from matching classes.
         arange_1d = torch.arange(start=0, end=grad_2d.size()[0], device=grad_2d.device)
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/loss/loss_2d.py` & `colossalai-nightly-2023.6.3/colossalai/nn/loss/loss_2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         ctx.save_for_backward(exp_logits, target_mask, masked_target)
 
         return loss
 
     @staticmethod
     @custom_bwd
     def backward(ctx, output_grad):
-        # Retrieve tensors from the forward path.
+        # Retreive tensors from the forward path.
         softmax, target_mask, masked_target = ctx.saved_tensors
 
         # All the inputs have softmax as their gradient.
         grad_input = softmax
 
         # For simplicity, work with the 2D gradient.
         partition_vocab_size = softmax.size()[-1]
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/loss/loss_2p5d.py` & `colossalai-nightly-2023.6.3/colossalai/nn/loss/loss_2p5d.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         ctx.save_for_backward(exp_logits, target_mask, masked_target)
 
         return loss
 
     @staticmethod
     @custom_bwd
     def backward(ctx, output_grad):
-        # Retrieve tensors from the forward path.
+        # Retreive tensors from the forward path.
         softmax, target_mask, masked_target = ctx.saved_tensors
 
         # All the inputs have softmax as their gradient.
         grad_input = softmax
 
         # For simplicity, work with the 2D gradient.
         partition_vocab_size = softmax.size()[-1]
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/loss/loss_3d.py` & `colossalai-nightly-2023.6.3/colossalai/nn/loss/loss_3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,18 +95,18 @@
         ctx.save_for_backward(exp_logits, target_mask, masked_target)
 
         return loss
 
     @staticmethod
     @custom_bwd
     def backward(ctx, output_grad):
-        # Retrieve tensors from the forward path.
+        # Retreive tensors from the forward path.
         softmax, target_mask, masked_target = ctx.saved_tensors
 
-        # All the inputs have softmax as their gradient.
+        # All the inputs have softmax as thier gradient.
         input_grad = softmax
         # For simplicity, work with the 2D gradient.
         partition_vocab_size = softmax.size()[-1]
         grad_2d = input_grad.view(-1, partition_vocab_size)
 
         # Add the gradient from matching classes.
         arange_1d = torch.arange(start=0, end=grad_2d.size()[0], device=get_current_device())
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/loss/loss_moe.py` & `colossalai-nightly-2023.6.3/colossalai/nn/loss/loss_moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/lr_scheduler/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/lr_scheduler/cosine.py` & `colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/cosine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/lr_scheduler/delayed.py` & `colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/delayed.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/lr_scheduler/linear.py` & `colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/lr_scheduler/multistep.py` & `colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/multistep.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/lr_scheduler/onecycle.py` & `colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/onecycle.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/lr_scheduler/poly.py` & `colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/poly.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/lr_scheduler/torch.py` & `colossalai-nightly-2023.6.3/colossalai/nn/lr_scheduler/torch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/metric/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/nn/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/metric/accuracy_2d.py` & `colossalai-nightly-2023.6.3/colossalai/nn/metric/accuracy_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/metric/accuracy_2p5d.py` & `colossalai-nightly-2023.6.3/colossalai/nn/metric/accuracy_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/metric/accuracy_3d.py` & `colossalai-nightly-2023.6.3/colossalai/nn/metric/accuracy_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/optimizer/colossalai_optimizer.py` & `colossalai-nightly-2023.6.3/colossalai/nn/optimizer/colossalai_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/optimizer/cpu_adam.py` & `colossalai-nightly-2023.6.3/colossalai/nn/optimizer/cpu_adam.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 from .nvme_optimizer import NVMeOptimizer
 
 
 @OPTIMIZERS.register_module
 class CPUAdam(NVMeOptimizer):
     """Implements Adam algorithm.
 
-    Supports parameters updating on both GPU and CPU, depending on the device of parameters.
+    Supports parameters updating on both GPU and CPU, depanding on the device of parameters.
     But the parameters and gradients should on the same device:
       * Parameters on CPU and gradients on CPU is allowed.
       * Parameters on GPU and gradients on GPU is allowed.
       * Parameters on GPU and gradients on CPU is **not** allowed.
 
     `CPUAdam` requires CUDA extensions which can be built during installation or runtime.
 
-    This version of CPU Adam accelerates parameters updating on CPU with SIMD.
+    This version of CPU Adam accelates parameters updating on CPU with SIMD.
     Support of AVX2 or AVX512 is required.
 
     The GPU part is implemented in an naive way.
 
     CPU Adam also supports the hybrid precision calculation, eg. fp32 parameters and fp16 gradients.
 
     :class:`colossalai.nn.optimizer.CPUAdam` may be used as a drop-in replacement for ``torch.optim.AdamW``,
@@ -89,15 +89,16 @@
                           beta1,
                           beta2,
                           eps,
                           weight_decay,
                           bias_correction1,
                           bias_correction2,
                           use_adamw=False):
-        grad = grad.to(data.dtype)
+        # FIXME(ver217): remove the below line when replace torch adam with fused adam
+        grad = grad.float()
 
         if weight_decay != 0:
             if use_adamw:
                 data.mul_(1 - lr * weight_decay)
             else:
                 grad = grad.add(data, alpha=weight_decay)
 
@@ -128,41 +129,31 @@
 
                 state = self.state[p]
 
                 target_device = p.device
                 if len(state) == 0:
                     state['step'] = 0
 
-                    # FIXME(ver217): CPU adam kernel only supports fp32 states now
-                    assert p.dtype is torch.float, "CPUAdam only support fp32 parameters"
                     # gradient momentums
-                    state['exp_avg'] = torch.zeros_like(p, device=target_device)
+                    state['exp_avg'] = torch.zeros_like(p, dtype=torch.float, device=target_device)
                     # gradient variances
-                    state['exp_avg_sq'] = torch.zeros_like(p, device=target_device)
+                    state['exp_avg_sq'] = torch.zeros_like(p, dtype=torch.float, device=target_device)
                     self._post_state_init(p)
 
                 state['step'] += 1
                 beta1, beta2 = group['betas']
 
                 if target_device.type == 'cpu':
                     assert p.data.numel() == p.grad.data.numel(), "parameter and gradient should have the same size"
                     assert state['exp_avg'].device.type == 'cpu', "exp_avg should stay on cpu"
                     assert state['exp_avg_sq'].device.type == 'cpu', "exp_avg should stay on cpu"
                     self._pre_update(p, 'exp_avg', 'exp_avg_sq')
-                    if p.grad.dtype is torch.bfloat16:
-                        # cpu adam kernel does not support bf16 now
-                        bias_correction1 = 1 - beta1**state['step']
-                        bias_correction2 = 1 - beta2**state['step']
-                        self.torch_adam_update(p.data, p.grad.data, state['exp_avg'], state['exp_avg_sq'], group['lr'],
-                                               beta1, beta2, group['eps'], group['weight_decay'], bias_correction1,
-                                               bias_correction2, self.adamw_mode)
-                    else:
-                        self.cpu_adam_op.step(state['step'], group['lr'], beta1, beta2, group['eps'],
-                                              group['weight_decay'], group['bias_correction'], p.data, p.grad.data,
-                                              state['exp_avg'], state['exp_avg_sq'], div_scale)
+                    self.cpu_adam_op.step(state['step'], group['lr'], beta1, beta2, group['eps'], group['weight_decay'],
+                                          group['bias_correction'], p.data, p.grad.data, state['exp_avg'],
+                                          state['exp_avg_sq'], div_scale)
                     self._post_update(p, 'exp_avg', 'exp_avg_sq')
                 elif target_device.type == 'cuda':
                     assert div_scale == -1, "div_scale should remain default"
                     assert state['exp_avg'].device.type == 'cuda', "exp_avg should stay on cuda"
                     assert state['exp_avg_sq'].device.type == 'cuda', "exp_avg should stay on cuda"
 
                     bias_correction1 = 1 - beta1**state['step']
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/optimizer/fused_adam.py` & `colossalai-nightly-2023.6.3/colossalai/nn/optimizer/fused_adam.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,16 +130,16 @@
                 # State initialization
                 if len(state) == 0:
                     # Exponential moving average of gradient values
                     state['exp_avg'] = torch.zeros_like(p)
                     # Exponential moving average of squared gradient values
                     state['exp_avg_sq'] = torch.zeros_like(p)
 
-                if p.dtype not in [torch.float16, torch.float32, torch.bfloat16]:
-                    raise RuntimeError('FusedAdam only support fp16, fp32 and bf16.')
+                if p.dtype not in [torch.float16, torch.float32]:
+                    raise RuntimeError('FusedAdam only support fp16 and fp32.')
 
                 g_l.append(p.grad.data)
                 p_l.append(p.data)
                 m_l.append(state['exp_avg'])
                 v_l.append(state['exp_avg_sq'])
 
             multi_tensor_applier(self.multi_tensor_adam, self._dummy_overflow_buf, [g_l, p_l, m_l, v_l], group['lr'],
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/optimizer/fused_lamb.py` & `colossalai-nightly-2023.6.3/colossalai/nn/optimizer/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/optimizer/fused_sgd.py` & `colossalai-nightly-2023.6.3/colossalai/nn/optimizer/fused_sgd.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/optimizer/hybrid_adam.py` & `colossalai-nightly-2023.6.3/colossalai/nn/optimizer/hybrid_adam.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from typing import Any, Optional
 
 import torch
-from torch.optim import Adam
 
-from colossalai.kernel.op_builder import FusedOptimBuilder
+from colossalai.kernel.op_builder import CPUAdamBuilder, FusedOptimBuilder
 from colossalai.registry import OPTIMIZERS
 from colossalai.utils import multi_tensor_applier
 
-from .cpu_adam import CPUAdam
+from .nvme_optimizer import NVMeOptimizer
 
 
 @OPTIMIZERS.register_module
-class HybridAdam(CPUAdam):
+class HybridAdam(NVMeOptimizer):
     """Implements Adam algorithm.
 
-    Supports parameters updating on both GPU and CPU, depending on the device of parameters.
+    Supports parameters updating on both GPU and CPU, depanding on the device of parameters.
     But the parameters and gradients should on the same device:
       * Parameters on CPU and gradients on CPU is allowed.
       * Parameters on GPU and gradients on GPU is allowed.
       * Parameters on GPU and gradients on CPU is **not** allowed.
 
     `HybridAdam` requires CUDA extensions which can be built during installation or runtime.
 
@@ -71,17 +70,23 @@
                  eps=1e-8,
                  weight_decay=0,
                  adamw_mode=True,
                  nvme_offload_fraction: float = 0.0,
                  nvme_offload_dir: Optional[str] = None,
                  **defaults: Any):
 
-        super().__init__(model_params, lr, bias_correction, betas, eps, weight_decay, adamw_mode, nvme_offload_fraction,
-                         nvme_offload_dir)
+        default_args = dict(lr=lr, betas=betas, eps=eps, weight_decay=weight_decay, bias_correction=bias_correction)
+        super(HybridAdam, self).__init__(model_params, default_args, nvme_offload_fraction, nvme_offload_dir)
+        self.adamw_mode = adamw_mode
+
+        # build during runtime if not found
+        cpu_optim = CPUAdamBuilder().load()
         fused_optim = FusedOptimBuilder().load()
+        self.cpu_adam_op = cpu_optim.CPUAdamOptimizer(lr, betas[0], betas[1], eps, weight_decay, adamw_mode)
+
         self.gpu_adam_op = fused_optim.multi_tensor_adam
         self._dummy_overflow_buf = torch.cuda.IntTensor([0])
 
     @torch.no_grad()
     def step(self, closure=None, div_scale: float = -1):
         loss = None
         if closure is not None:
@@ -99,41 +104,31 @@
 
                 state = self.state[p]
 
                 target_device = p.device
                 if len(state) == 0:
                     state['step'] = 0
 
-                    # FIXME(ver217): CPU adam kernel only supports fp32 states now
-                    assert p.dtype is torch.float, "HybridAdam only support fp32 parameters"
                     # gradient momentums
-                    state['exp_avg'] = torch.zeros_like(p, device=target_device)
+                    state['exp_avg'] = torch.zeros_like(p, dtype=torch.float, device=target_device)
                     # gradient variances
-                    state['exp_avg_sq'] = torch.zeros_like(p, device=target_device)
+                    state['exp_avg_sq'] = torch.zeros_like(p, dtype=torch.float, device=target_device)
                     self._post_state_init(p)
 
                 state['step'] += 1
                 group_step = state['step']
                 beta1, beta2 = group['betas']
 
                 if target_device.type == 'cpu':
                     assert state['exp_avg'].device.type == 'cpu', "exp_avg should stay on cpu"
                     assert state['exp_avg_sq'].device.type == 'cpu', "exp_avg should stay on cpu"
                     self._pre_update(p, 'exp_avg', 'exp_avg_sq')
-                    if p.grad.dtype is torch.bfloat16:
-                        # cpu adam kernel does not support bf16 now
-                        bias_correction1 = 1 - beta1**state['step']
-                        bias_correction2 = 1 - beta2**state['step']
-                        self.torch_adam_update(p.data, p.grad.data, state['exp_avg'], state['exp_avg_sq'], group['lr'],
-                                               beta1, beta2, group['eps'], group['weight_decay'], bias_correction1,
-                                               bias_correction2, self.adamw_mode)
-                    else:
-                        self.cpu_adam_op.step(state['step'], group['lr'], beta1, beta2, group['eps'],
-                                              group['weight_decay'], group['bias_correction'], p.data, p.grad.data,
-                                              state['exp_avg'], state['exp_avg_sq'], div_scale)
+                    self.cpu_adam_op.step(state['step'], group['lr'], beta1, beta2, group['eps'], group['weight_decay'],
+                                          group['bias_correction'], p.data, p.grad.data, state['exp_avg'],
+                                          state['exp_avg_sq'], div_scale)
                     self._post_update(p, 'exp_avg', 'exp_avg_sq')
 
                 elif target_device.type == 'cuda':
                     assert state['exp_avg'].device.type == 'cuda', "exp_avg should stay on cuda"
                     assert state['exp_avg_sq'].device.type == 'cuda', "exp_avg should stay on cuda"
 
                     # record the state by group and update at once
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/optimizer/lamb.py` & `colossalai-nightly-2023.6.3/colossalai/nn/optimizer/lamb.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
         for group in self.param_groups:
             for p in group['params']:
                 if p.grad is None:
                     continue
                 grad = p.grad.data
                 if grad.is_sparse:
-                    raise RuntimeError('Lamb does not support sparse gradients, consider SparseAdam instead.')
+                    raise RuntimeError('Lamb does not support sparse gradients, consider SparseAdam instad.')
 
                 state = self.state[p]
 
                 # State initialization
                 if len(state) == 0:
                     state['step'] = 0
                     # Exponential moving average of gradient values
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/optimizer/lars.py` & `colossalai-nightly-2023.6.3/colossalai/nn/optimizer/lars.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/optimizer/nvme_optimizer.py` & `colossalai-nightly-2023.6.3/colossalai/nn/optimizer/nvme_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             backend = 'uring' if 'uring' in get_backends() else 'aio'
             self.offloader = DiskOffloader(self.offload_dir, 8, backend=backend)
         else:
             self.offload_dir = None
             self.offloader = None
         self.is_on_nvme: Dict[Parameter, bool] = {}
         self.offloaded_numel: int = 0
-        # As param may be not materialized here, these attributes are initialized when the first step
+        # As param may be not materialized here, these attributes are initalized when the first step
         self.total_numel: Optional[int] = None
         self.can_offload_numel: Optional[int] = None
 
         self.prefetch_params: List[Parameter] = []
         self.param_to_prefetch_idx: Dict[Parameter, int] = {}
 
     def _get_numel(self) -> int:
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/parallel/data_parallel.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/cache_embedding/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 
 
 class CachedEmbeddingBag(BaseEmbeddingBag):
     """CachedEmbeddingBag
 
     Cached Embedding. Apply a GPU-based software cache approaches to dynamically manage the embedding table in the CPU and GPU memory space.
     It can leverage the id's frequency statistics of the target dataset, by passing a frequency list to param `ids_freq_mapping`.
-    You can also apply a naive LFU cache eviction strategy by setting `evict_strategy` as EvictionStrategy.LFU.
+    You can also apply a navie LFU cache eviction strategy by setting `evict_strategy` as EvictionStrategy.LFU.
 
     Args:
         num_embeddings (int): size of the dictionary of embeddings
         embedding_dim (int):  the size of each embedding vector
         padding_idx (int, optional): If specified, the entries at padding_idx do not contribute to the gradient; therefore, the embedding vector at padding_idx is not updated during training, i.e. it remains as a fixed “pad”. For a newly constructed EmbeddingBag, the embedding vector at padding_idx will default to all zeros, but can be updated to another value to be used as the padding vector. Note that the embedding vector at padding_idx is excluded from the reduction.
         max_norm (float, optional): If given, each embedding vector with norm larger than max_norm is renormalized to have norm max_norm
-        norm_type (str, optional): The p of the p-norm to compute for the max_norm option. Defaults to 2.
+        norm_type (str, optional): The p of the p-norm to compute for the max_norm option. Defaults to 2..
         scale_grad_by_freq (bool, optional): if given, this will scale gradients by the inverse of frequency of the words in the mini-batch. Default False. Note: this option is not supported when mode="max". Defaults to False.
         sparse (bool, optional): if True, gradient w.r.t. weight matrix will be a sparse tensor. See Notes for more details regarding sparse gradients. Note: this option is not supported when mode="max".. Defaults to False.
-        _weight (torch.Tensor, optional): an embedding weight tensor. Concatenate multiple tables in a embedding bag as a single one. Defaults to None.
+        _weight (torch.Tensor, optional): an embedding weight tensor. Concate multiple tables in a embedding bag as a single one. Defaults to None.
         mode (str, optional): "sum", "mean" or "max". Specifies the way to reduce the bag. "sum" computes the weighted sum, taking per_sample_weights into consideration. "mean" computes the average of the values in the bag, "max" computes the max value over each bag. Default: "mean". Defaults to 'mean'.
         include_last_offset (bool, optional): if True, offsets has one additional element, where the last element is equivalent to the size of indices. This matches the CSR format.. Defaults to False.
         dtype (torch.dtype, optional): data type of the cpu weight initialization. Defaults to None meaning float32.
         device (torch.device, optional): device type to the cpu weight. Defaults to None meaning cpu.
         cache_ratio (float, float): cache ratio of the #cuda_weight_row / #cpu_weight_row 
-        ids_freq_mapping (Union[List, torch.Tensor], optional): the frequency of each embedding vector occurs in dataset. Defaults to None.
+        ids_freq_mapping (Union[List, torch.Tensor], optional): the frequency of each embedding vector occures in dataset. Defaults to None.
         warmup_ratio (float, optional): the ratio of cuda cache is warmuped with. Defaults to 0.7.
         buffer_size (int, optional): the max number of vectors in transmitter buffer. If set to 0, the buffer is not used. Defaults to 0.
         pin_weight (bool, optional): pin the cpu weight. Defaults to False.
         evict_strategy (EvictionStrategy, optional): evict strategy of the software cache. Defaults to EvictionStrategy.DATASET.
     """
 
     def __init__(self,
@@ -141,15 +141,15 @@
     def num_write_back_history(self):
         return self.cache_weight_mgr.num_write_back_history
 
     @property
     def swap_in_bandwidth(self):
         if self.cache_weight_mgr._cpu_to_cuda_numel > 0:
             return self.cache_weight_mgr._cpu_to_cuda_numel * self.cache_weight_mgr.elem_size_in_byte / 1e6 / \
-                   self.cache_weight_mgr._cpu_to_cuda_elapse
+                   self.cache_weight_mgr._cpu_to_cuda_elpase
         else:
             return 0
 
     @property
     def swap_out_bandwidth(self):
         if self.cache_weight_mgr._cuda_to_cpu_numel > 0:
             return self.cache_weight_mgr._cuda_to_cpu_numel * self.cache_weight_mgr.elem_size_in_byte / 1e6 / \
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/cache_embedding/copyer.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/copyer.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def __init__(self, size: int) -> None:
         self._buff_size = size
 
     @torch.no_grad()
     def index_copy(self, dim: int, src_index: LongTensor, tgt_index: LongTensor, src: torch.Tensor, tgt: torch.Tensor):
         """copy 
         src tensor[src_index] -(index_select)-> tmp -(index_copy_)-> tgt tensor [tgt_index]
-        The valid rows in the src tensor are continuous, while rows in tgt tensor is scattered.
+        The valid rows in the src tensor are continous, while rows in tgt tensor is scattered.
 
         Args:
             dim (int):  dimension along which to index
             src_index (int): indices of src tensor to select from
             tgt_index (int): indices of tgt tensor to select from
             src (torch.Tensor):  the tensor containing values to copy
             tgt (torch.Tensor):  the tensor to be copied
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                     local_per_sample_weights = per_sample_weights[indices_start_position:indices_end_position]
             with record_function("(tablewise) tablewise forward"):
                 local_output_list.append(self.cached_embedding_bag_list[i](local_indices, local_offsets,
                                                                            local_per_sample_weights))
 
         # get result of shape = (batch_size, (len(assigned_table_list)*embedding_dim))
         local_output = torch.cat(local_output_list, 1)
-        # then concatenate those local_output on the second dimension.
+        # then concatenate those local_output on the second demension.
         # use all_to_all
         remains = batch_size % self.world_size
         scatter_strides = [batch_size // self.world_size + int(i < remains) for i in range(self.world_size)]
         output_full = dual_all_to_all_tablewise(local_output, self.pg, scatter_strides, self.embedding_dim_per_rank)
         if shape_hook is not None:
             output_full = shape_hook(output_full)
         return output_full
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/colo_module.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/colo_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/embedding.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/linear.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/parallel/layers/module_utils.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/layers/module_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/nn/parallel/reducer.py` & `colossalai-nightly-2023.6.3/colossalai/nn/parallel/reducer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/pipeline/layer_spec.py` & `colossalai-nightly-2023.6.3/colossalai/pipeline/layer_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/pipeline/middleware/adaptor/fx.py` & `colossalai-nightly-2023.6.3/colossalai/pipeline/middleware/adaptor/fx.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/pipeline/middleware/topo.py` & `colossalai-nightly-2023.6.3/colossalai/pipeline/middleware/topo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/pipeline/pipelinable.py` & `colossalai-nightly-2023.6.3/colossalai/pipeline/pipelinable.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             modified_args.append(arg)
 
         # to the same for the keyword arguments
         modified_kwargs = {}
         for k, v in kwargs.items():
             if isinstance(v, torch.nn.Module):
                 v = self._layer_spec_dict[id(v)]
-            # (lyl)TODO: analyze ColoTensor as well
+            # (lyl)TODO: analyse ColoTensor as well
             modified_kwargs[k] = v
 
         # keep track of the module children
         # as torch.nn.Module.__init__ is called from inner module to outer module,
         # the final value of self._model will be the outermost model
         # e.g. if the model is torchvision.models.resnet18, then the final value of self._model
         # will be the ``ResNet`` object.
@@ -113,15 +113,15 @@
             if hasattr(module, name):
                 delattr(module, name)
             setattr(module, name, ColoParameter.from_torch_tensor(tensor=param.data, requires_grad=param.requires_grad))
 
     def to_layer_list(self, exec_seq=None):
         """
         Create a layer spec list and func list with execution sequence given by user.
-        If exec_seq is None, we will take the module initializing order as execution order.
+        If exec_seq is None, we will take the module initizing order as execution order.
         """
 
         self._exec_seq = exec_seq
         if exec_seq is None:
             # if user do not provide the model executing sequence, we use the initialization order as the executing order.
             children_name = []
             for child in self._root_children:
@@ -173,15 +173,15 @@
                     if isinstance(element, tuple):
                         self._func_dict[func_key].append(element[0])
                     else:
                         self._func_dict[func_key].append(element)
 
     def partition(self, num_chunks, pipeline_size, rank):
         """
-        Partitioned model will be built respect to partition policy.
+        Partitioned model will be built respect to partion policy.
         The real module instance will be built in this method.
         """
         if isinstance(self._policy, str):
             if self._policy == "uniform":
                 parts = partition_uniform(len(self._layer_spec_list), pipeline_size, num_chunks)[rank]
             elif self._policy == "balanced":
                 param_counts = []
@@ -189,15 +189,15 @@
                     param_counts.append(layer_spec.count_params())
                 parts = partition_balanced(param_counts, pipeline_size, num_chunks)[rank]
             elif self._policy == "customized":
                 assert self._exec_seq is not None, f'An explicit exec_seq must be defined by user in customized policy mode.'
                 self.customized_parts = customized_partition(self._exec_seq)
                 assert len(self.customized_parts) == gpc.get_world_size(
                     ParallelMode.PIPELINE
-                ), f'World size is {gpc.get_world_size(ParallelMode.PIPELINE)}, but the number of partitions is {len(self.customized_parts)}'
+                ), f'World size is {gpc.get_world_size(ParallelMode.PIPELINE)}, but the number of partions is {len(self.customized_parts)}'
                 parts = self.customized_parts[rank]
             else:
                 raise ValueError("A string partition policy should be one of ['uniform', 'balanced', 'customized'].")
         elif isinstance(self._policy, dict):
             parts = self._policy[rank]
         else:
             raise ValueError("A partition policy should be either a string or a dictionary.")
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/pipeline/pipeline_process_group.py` & `colossalai-nightly-2023.6.3/colossalai/pipeline/pipeline_process_group.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/pipeline/rpc/_pipeline_base.py` & `colossalai-nightly-2023.6.3/colossalai/pipeline/rpc/_pipeline_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
         if data_process_func is not None:
             self.data_process_func = partial(data_process_func, pp_rank)
 
         self.device = device
         self._initialize_outstanding_range()
 
-        # variable and const for context management
+        # variable and const for context managment
         self.outstanding = 0
         self.forward_times = 0
         self.backward_times = 0
         self.reset_key = UniqueKey(0, Phase.FORWARD)
 
         # rref of other workers
         self.pp_rank_to_worker_rref: Dict[int, PyRRef] = None
@@ -222,15 +222,15 @@
 
     def sync_global_worker_rrefs(self, pp_rank_to_worker_rref: Dict[int, PyRRef]) -> None:
         assert self.pp_rank_to_worker_rref is None, f"in rank {self.pp_rank}, worker has sync global workers rrefs"
         assert pp_rank_to_worker_rref is not None, "stage_to_workers must be a dict instead of None"
         self.pp_rank_to_worker_rref = pp_rank_to_worker_rref
 
         # for some schedule need the other worker's info to initialise partition (like Chimera)
-        # construction of partition is executed after the registration of pp_rank_to_worker_rref
+        # construction of partition is executed after the registion of pp_rank_to_worker_rref
         self._initialize_partition()
 
     # res_use works for lifecycle counter,
     # if ref_use is True, lifecycle won't add.
     # offset supports get partial output to reduce comm costs.
     def get_output_by_key(self, key: UniqueKey, ref_use=False, rank=None, offsets=None) -> Any:
         output = self._get_output_all(key, ref_use, rank)
@@ -414,15 +414,15 @@
     def subscribe_producer(self, microbatch_id: int, forward_only: bool):
         key = UniqueKey(microbatch_id, Phase.FORWARD)
         with self.work_list_condition_lock:
             if key not in self.work_list:
                 # On current PP middleware design for DAG, get_output_by_key used by _subscribe_producer
                 # can only be executed once for every producer-consumer stage pair, which is necessary
                 # to count the lifecycle of work_item. So, keeping the _subscribe_producer in the same
-                # lock of work_item queue operation guarantees the consistency of lifecycle counter.
+                # lock of work_item queue operation gurantees the consistency of lifecycle counter.
                 work_item_from_producer = self._subscribe_producer(microbatch_id, forward_only)
                 self.work_list[key] = work_item_from_producer
                 self.work_list_condition_lock.notify_all()
 
     def _subscribe_consumer(self, microbatch_id: int):
         """
         You should call this function asynchronously
@@ -456,15 +456,15 @@
     def subscribe_consumer(self, microbatch_id: int):
         key = UniqueKey(microbatch_id, Phase.BACKWARD)
         with self.work_list_condition_lock:
             if key not in self.work_list:
                 # On current PP middleware design for DAG, get_output_by_key used by subscribe_consumer
                 # can only be executed once for every producer-consumer stage pair, which is necessary
                 # to count the lifecycle of work_item. So, keeping the subscribe_consumer in the same
-                # lock of work_item queue operation guarantees the consistency of lifecycle counter.
+                # lock of work_item queue operation gurantees the consistency of lifecycle counter.
                 work_item_from_consumer = self._subscribe_consumer(microbatch_id)
                 self.work_list[key] = work_item_from_consumer
                 self.work_list_condition_lock.notify_all()
 
     def get_producer_stage_ids(self):
         producer_stage_ids = []
         rank = self.pp_rank
@@ -504,15 +504,15 @@
         return consumer_stage_ids
 
     def _get_producer_consumer(self) -> None:
         rank = self.pp_rank
         assert self.producer_stage_ids is None, f"all the producers of rank {rank} has been subscribed"
         assert self.consumer_stage_ids is None, f"all the consumers of rank {rank} has been subscribed"
 
-        # should be arranged in order, the order of the input of current forward
+        # should be aranged in order, the order of the input of current forward
         self.producer_stage_ids = self.get_producer_stage_ids()
         self.consumer_stage_ids = self.get_consumer_stage_ids()
 
     def pp_rank_to_partition_id(self, pp_rank: int, topo: Topo):
         partition_ids = topo.get_mid_partition_ids()
         return partition_ids[pp_rank]
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/pipeline/rpc/_pipeline_schedule.py` & `colossalai-nightly-2023.6.3/colossalai/pipeline/rpc/_pipeline_schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         rank = self.pp_rank
         min_pp_rank = (rank // self.actual_stage_num) * self.actual_stage_num
         max_pp_rank = min_pp_rank + self.actual_stage_num - 1
 
         assert self.producer_stage_ids is None, f"all the producers of rank {rank} has been subscribed"
         assert self.consumer_stage_ids is None, f"all the consumers of rank {rank} has been subscribed"
 
-        # should be arranged in order, the order of the input of current forward
+        # should be aranged in order, the order of the input of current forward
         self.producer_stage_ids = []
         self.consumer_stage_ids = []
 
         # Just for demo
         prev_rank = rank - 1
         next_rank = rank + 1
         if prev_rank >= min_pp_rank:
@@ -170,15 +170,15 @@
         stage_num = self.actual_stage_num
         device = self.device
         if pp_rank < stage_num:
             super()._initialize_partition()
         else:
             # if it is down pipeline, create partition by origin method
             co_up_pp_worker_rref = self.pp_rank_to_worker_rref[pp_rank - stage_num]
-            # get the corresponding model state dict and wait for its init
+            # get the coresponding model state dict and wait for its init
             state_dict = co_up_pp_worker_rref.rpc_sync().get_partition_state_dict()
             super()._initialize_partition()
             self.module_partition.load_state_dict(state_dict)
 
         # init group for chimera in ppg
         ppg.get_chimera_all_reduce_group(pp_rank)
 
@@ -224,15 +224,15 @@
 
     def _hook_before_step(self):
         self.have_grad_lock.release()
         pp_rank = self.pp_rank
         stage_num = self.actual_stage_num
         co_pp_rank = (pp_rank + stage_num) % (2 * stage_num)
 
-        # if current pp_rank is not the first to do step
+        # if currrent pp_rank is not the first to do step
         # wait its previous pp_rank finish step
         grads = self.get_parameter_gradients()
 
         # send
         co_worker = self.pp_rank_to_worker_rref[co_pp_rank]
         co_grads = co_worker.rpc_sync()._get_lock_gradient()
         # sync
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/pipeline/rpc/utils.py` & `colossalai-nightly-2023.6.3/colossalai/pipeline/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/pipeline/utils.py` & `colossalai-nightly-2023.6.3/colossalai/pipeline/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         intervals = _heap_addition(prefix, intervals, num - num_block)
 
     return intervals
 
 
 def partition_uniform(num_items, pipeline_parallel_size, num_chunks):
     assert num_items % num_chunks == 0, \
-        "Layer length should be divided by the number of chunks, otherwise parameter method is recommended"
+        "Layer length should be divided by the number of chunks, otherwise parameter method is recomended"
 
     logger = get_dist_logger()
     parts = [[] for _ in range(pipeline_parallel_size)]
     partition_items = num_items // num_chunks
     for idx in range(num_chunks):
         base_idx = idx * partition_items
         chunk_size = partition_items // pipeline_parallel_size
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/registry/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/registry/registry.py` & `colossalai-nightly-2023.6.3/colossalai/registry/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/tensor/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/tensor/colo_parameter.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/colo_parameter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/tensor/colo_tensor.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/colo_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/tensor/comm_spec.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/comm_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/tensor/compute_spec.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/compute_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/tensor/d_tensor/comm_spec.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/comm_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     '''
     Communication spec is used to record the communication action. It converts the communication spec
     to real action which will be used in runtime. It contains comm_pattern to determine the
     communication method, process_groups_dict to determine the process groups, gather_dim and shard_dim
     to determine the buffer shape, and logical_process_axis
 
     Argument:
-        comm_pattern(CollectiveCommPattern): describe the communication method used in this spec.
+        comm_pattern(CollectiveCommPattern): decribe the communication method used in this spec.
         process_groups_dict(Dict): A dict which contains the process groups used to apply this CommSpec.
         gather_dim(int, Optional): The gather_dim of the tensor will be gathered.
         shard_dim(int, Optional): The shard_dim of the tensor will be sharded.
         logical_process_axis(Union(int, List[int]), Optional): The mesh_dim to implement the communication action.
     '''
 
     def __init__(self,
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/tensor/d_tensor/d_tensor.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/d_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/tensor/d_tensor/layout.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/layout.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/tensor/d_tensor/layout_converter.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/layout_converter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/tensor/d_tensor/sharding_spec.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/sharding_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         target = 'S'
         for dim in self.shard_list:
             target += str(dim)
         return target
 
     def _convert_str_to_shard_list(self, str_spec):
         '''
-        Convert str_spec into shard_list.
+        Conver str_spec into shard_list.
 
         Argument:
             str_spec(str): dim spec in str type.
         '''
 
         if str_spec == 'R':
             return []
@@ -54,15 +54,15 @@
         if str_spec == 'S1':
             return [1]
         if str_spec == 'S01':
             return [0, 1]
 
     def build_difference_2d_dict(self):
         '''
-        Build a difference mapping for 2D device mesh case. It will be used to
+        Build a difference maping for 2D device mesh case. It will be used to
         compute the difference between DimSpec pairs.
         '''
 
         source_spec_list = ['R', 'S0', 'S1', 'S01']
         target_spec_list = ['R', 'S0', 'S1', 'S01']
         difference_dict = {}
         for source_spec in source_spec_list:
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/tensor/d_tensor/utils.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/d_tensor/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/tensor/dist_spec_mgr.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/dist_spec_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/tensor/distspec.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/distspec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/tensor/op_wrapper.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/op_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/tensor/param_op_hook.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/param_op_hook.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     # if there is no grad tensors, do nothing
     if not _has_grad_tensor(args):
         return args, None
     # returns the identical args if there is a grad tensor
     for obj in args:
         if _is_grad_tensor(obj):
             return args, None
-    # otherwise, the first argument should be a tuple of grad tensors
+    # otherwise, the first arguement should be a tuple of grad tensors
     # if there is no grad tensor, the backward of PreFwdPostBwd can't be triggered
     arg_zero = args[0]
     if not isinstance(arg_zero, tuple):
         raise NotImplementedError("Some torch function is incompatible because of its complicated inputs.")
     check_grad_flag = False
     for obj in arg_zero:
         check_grad_flag |= _is_grad_tensor(obj)
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/tensor/process_group.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/process_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
             PYTORCHPGDICT_.get(j_dp_list, 'gloo')
 
         self._has_cpu_groups = True
 
     @property
     def has_cpu_groups(self) -> bool:
         """has_cpu_groups
-        If cpu groups have been initialized.
+        If cpu groups have been initailized.
 
         Returns:
             bool: cpu process groups have been initialized or not.
         """
         return self._has_cpu_groups
 
     def __repr__(self):
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/tensor/shape_consistency.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/shape_consistency.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,15 @@
                     pass
 
         return valid_spec_dict
 
     def get_all_shard_spec(self, source_spec: ShardingSpec, orig_cost_dict):
         '''
         Get all valid sharding specs from source_spec with single shard operation, and
-        accumulate communication cost on origin cost which will finally be used in auto sharding solver.
+        accumulate commucation cost on origin cost which will finally be used in auto sharding solver.
         For the sharding operation, we just care about legal sharding dimensions.
 
         Argument:
             source_spec(ShardingSpec): the ShardingSpec of the source_spec.
             orig_cost(float): the original communication cost before this operation.
 
         Return:
@@ -382,15 +382,15 @@
                     pass
 
         return valid_spec_dict
 
     def get_all_one_step_transform_spec(self, source_spec: ShardingSpec, orig_cost_dict) -> Dict[ShardingSpec, float]:
         '''
         Get all valid sharding specs from source_spec with one step transform, and
-        accumulate communication cost on origin cost which will finally be used in auto sharding solver.
+        accumulate commucation cost on origin cost which will finally be used in auto sharding solver.
         Note:
             all-gather will eliminate a sharding dimension, all-to-all will keep sharding dimension same as before,
             and shard will add a sharding dimension. Therefore, the result of above operations are mutual exclusive,
             we could safely put them together.
 
         Argument:
             source_spec(ShardingSpec): the ShardingSpec of the source_spec.
@@ -573,15 +573,15 @@
         Step1:
             Generate all one-step transform sequences from source_spec.
         Step2:
             Pick the 'best' sharding spec following the heuristic function.
         Step3:
             Repeat above steps until the source spec transform to target spec.
 
-        During finding the transform path, communication cost will be accumulated, and it
+        During finding the transform path, commucation cost will be accumulated, and it
         will be finally used in auto parallel solver.
 
         Additionally, to avoid repeating the path search in runtime, we cached all solved path
         in auto parallel strategy building time, which could handle most of cases in runtime.
 
         Argument:
             source_spec(ShardingSpec): ShardingSpec of the source activation.
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/tensor/sharding_spec.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/sharding_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         target = 'S'
         for dim in self.shard_list:
             target += str(dim)
         return target
 
     def _convert_str_to_shard_list(self, str_spec):
         '''
-        Convert str_spec into shard_list.
+        Conver str_spec into shard_list.
 
         Argument:
             str_spec(str): dim spec in str type.
         '''
 
         if str_spec == 'R':
             return []
@@ -58,15 +58,15 @@
         if str_spec == 'S1':
             return [1]
         if str_spec == 'S01':
             return [0, 1]
 
     def build_difference_2d_dict(self):
         '''
-        Build a difference mapping for 2D device mesh case. It will be used to
+        Build a difference maping for 2D device mesh case. It will be used to
         compute the difference between DimSpec pairs.
         '''
 
         source_spec_list = ['R', 'S0', 'S1', 'S01']
         target_spec_list = ['R', 'S0', 'S1', 'S01']
         difference_dict = {}
         for source_spec in source_spec_list:
@@ -162,15 +162,15 @@
     to, the entire shape of the tensor before sharded, and the sharding sequence looks like
     [R, R, S0, S1].
 
     Argument:
         device_mesh(DeviceMesh): A logical view of a physical mesh.
         entire_shape(torch.Size): The entire shape of tensor before sharded.
         dim_partition_dict(Dict[int, List[int]]， optional): The key is the dimension of tensor to be sharded,
-            and the value of the key describe which logical axis will be sharded in that dimension.
+            and the value of the key decribe which logical axis will be sharded in that dimension.
         sharding_sequence(List[_DimSpec], optional): A straight view of ShardingSpec looks like [R, R, S0, S1].
     '''
 
     def __init__(self,
                  device_mesh: DeviceMesh,
                  entire_shape: torch.Size,
                  dim_partition_dict=None,
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/tensor/tensor_spec.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/tensor_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/tensor/utils.py` & `colossalai-nightly-2023.6.3/colossalai/tensor/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         shard(R) -> S0
     For the S dimension, we need to make sure the shard_list after sharding still keep rising order.
     e.g:
         shard(S0) -> S01
 
     Argument:
         target_pair(Tuple[int, List[int]]): The first element is the dimension of tensor to be sharded,
-        and the second element describes which logical axis will be sharded in that dimension.
+        and the second element decribes which logical axis will be sharded in that dimension.
     '''
     _, shard_list = target_pair
     shard_list_list = []
     for dim in legal_sharding_dims:
         if len(shard_list) != 0 and dim <= shard_list[-1]:
             continue
         new_shard_list = shard_list + [dim]
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/testing/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/testing/comparison.py` & `colossalai-nightly-2023.6.3/colossalai/testing/comparison.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/testing/pytest_wrapper.py` & `colossalai-nightly-2023.6.3/colossalai/testing/pytest_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/testing/random.py` & `colossalai-nightly-2023.6.3/colossalai/testing/random.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/testing/utils.py` & `colossalai-nightly-2023.6.3/colossalai/testing/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/trainer/_trainer.py` & `colossalai-nightly-2023.6.3/colossalai/trainer/_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,17 @@
         >>> model = ...
         >>> criterion = ...
         >>> optimizer = ...
         >>> train_dataloader = ...
         >>> # Initialize your engine, train_dataloader, test_dataloader, lr_scheduler
         >>> engine, train_dataloader, _, _ = colossalai.initialize(model, optimizer, criterion)
         >>> # Beginning training progress
-        >>> timer = ...
+        >>> timier = ...
         >>> logger = ...
-        >>> trainer = Trainer(engine=engine, logger=logger, timer=timer)
+        >>> trainer = Trainer(engine=engine, logger=logger, timer=timier)
         >>> # add hooks you would like to use here.
         >>> hook_list = []
         >>> trainer.fit(
         >>>    train_dataloader=train_dataloader,
         >>>    epochs=gpc.config.NUM_EPOCHS,
         >>>    test_interval=1,
         >>>    hooks=hook_list,
@@ -52,15 +52,15 @@
 
     def __init__(
         self,
         engine: Engine,
         timer: MultiTimer = None,
         logger: DistributedLogger = None,
     ):
-        # training-related params
+        # training-ralated params
         self._engine = engine
         self._max_epochs = 0
         self._cur_epoch = 0
         self._max_steps = 0
         self._cur_step = 0
         self._steps_per_epoch = 0
 
@@ -114,15 +114,15 @@
 
         Args:
             epoch (int): Step number to be set.
         """
         self._cur_step = epoch * self._steps_per_epoch
 
     def _call_timer(self, action: str, item: str, *args, **kwargs) -> None:
-        """Call timer function with a given timer name.
+        """Call timer funciton with a given timer name.
 
         Args:
             action (str): Function to be called on timer.
             item (str): Name of the timer.
             args (list): args used for action function.
             kwargs (dict): kwargs used for action function.
         """
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/trainer/hooks/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/trainer/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/trainer/hooks/_base_hook.py` & `colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_base_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/trainer/hooks/_checkpoint_hook.py` & `colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_checkpoint_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/trainer/hooks/_log_hook.py` & `colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_log_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/trainer/hooks/_lr_scheduler_hook.py` & `colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_lr_scheduler_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/trainer/hooks/_metric_hook.py` & `colossalai-nightly-2023.6.3/colossalai/trainer/hooks/_metric_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/activation_checkpoint.py` & `colossalai-nightly-2023.6.3/colossalai/utils/activation_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/checkpoint/module_checkpoint.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpoint/module_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/checkpoint/utils.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpoint/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/checkpoint_io/backend.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/backend.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/checkpoint_io/convertor.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/convertor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/checkpoint_io/distributed.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/distributed.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/checkpoint_io/io.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/io.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/checkpoint_io/meta.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/meta.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/checkpoint_io/reader.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/reader.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/checkpoint_io/utils.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/checkpoint_io/writer.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpoint_io/writer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/checkpointing.py` & `colossalai-nightly-2023.6.3/colossalai/utils/checkpointing.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/common.py` & `colossalai-nightly-2023.6.3/colossalai/utils/common.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/cuda.py` & `colossalai-nightly-2023.6.3/colossalai/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/data_sampler/data_parallel_sampler.py` & `colossalai-nightly-2023.6.3/colossalai/utils/data_sampler/data_parallel_sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
-# adapted from torch.utils.data.DistributedSampler
+# adpated from torch.utils.data.DistributedSampler
 
 import math
 import random
 import numpy as np
 from typing import TypeVar, Iterator
 
 import torch
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/memory.py` & `colossalai-nightly-2023.6.3/colossalai/utils/memory.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/model/utils.py` & `colossalai-nightly-2023.6.3/colossalai/utils/model/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             cls.__init__ = preprocess_after(cls.__init__)
 
         # The function is called during init subclass.
         def _init_subclass(cls, **kwargs):
             cls.__init__ = preprocess_after(cls.__init__)
 
         # Replace .__init__() for all existing subclasses of torch.nn.Module
-        # Execution self._post_init_method after the default init function.
+        # Excution self._post_init_method after the default init function.
         substitute_init_recursively(torch.nn.modules.module.Module, _enable_class, set())
 
         # holding on to the current __init__subclass__ for exit
         torch.nn.modules.module.Module._old_init_subclass = (torch.nn.modules.module.Module.__init_subclass__)
         # Replace .__init__() for future subclasses of torch.nn.Module
         torch.nn.modules.module.Module.__init_subclass__ = classmethod(_init_subclass)
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/moe.py` & `colossalai-nightly-2023.6.3/colossalai/utils/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py` & `colossalai-nightly-2023.6.3/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/profiler/legacy/comm_profiler.py` & `colossalai-nightly-2023.6.3/colossalai/utils/profiler/legacy/comm_profiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,32 +107,32 @@
 
         def append(s: str = None):
             if s is not None:
                 res.append(s)
             res.append(sep)
 
         if self.warn_flag:
-            append("Warning: there exists multiple communication operations in the same time. As a result, "
+            append("Warnning: there exists multiple communication operations in the same time. As a result, "
                    "the profiling result is not accurate.")
 
         if self.total_cuda_time == 0:
             return "No collective communication has been called yet!"
 
         append("Collective communication profiling result:")
         append("total cuda time: {}".format(_format_time(self.total_cuda_time)))
         append("average bandwidth: {}".format(_format_bandwidth(self.total_comm_vol, self.total_cuda_time)))
         append("total number of calls: {}".format(self.total_count))
         append("All events:")
 
-        separation = '-' * 74
+        seperation = '-' * 74
         row_format = '{:^10}' + '{:^12}' * 2 + '{:^16}' + '{:^12}' * 2
 
-        append(separation)
+        append(seperation)
         append(row_format.format('Location', 'GPU time', 'Percentage', 'Comm volume', 'Bandwidth', 'Num of calls'))
-        append(separation)
+        append(seperation)
 
         show_list = sorted(self.ops_record.items(), key=lambda kv: -kv[1].self_cuda_time)
         for location, event in show_list:
             append(location)
             append(
                 row_format.format('', _format_time(event.self_cuda_time),
                                   '{:.1f}%'.format(event.self_cuda_time / self.total_cuda_time * 100.0),
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/profiler/legacy/pcie_profiler.py` & `colossalai-nightly-2023.6.3/colossalai/utils/profiler/legacy/pcie_profiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,20 +126,20 @@
         append("time of data transmission (CPU -> GPU): {}".format(_format_time(self.h2d_time)))
         append("number of transmission (CPU -> GPU): {}".format(self.h2d_count))
         append("time of data transmission (GPU -> CPU): {}".format(_format_time(self.d2h_time)))
         append("number of transmission (GPU -> CPU): {}".format(self.d2h_count))
 
         append("Possible data transmission events in PCIE:")
 
-        separation = '-' * 62
+        seperation = '-' * 62
         row_format = '{:^10}' + '{:^12}' + '{:^16}' + '{:^12}' * 2
 
-        append(separation)
+        append(seperation)
         append(row_format.format('Location', 'GPU time', 'Trans volume', 'Bandwidth', 'Num of calls'))
-        append(separation)
+        append(seperation)
 
         show_list = sorted(self.ops_record.items(), key=lambda kv: -kv[1].cuda_time)
         for location, event in show_list:
             append(location)
             append(
                 row_format.format('', _format_time(event.cuda_time), _format_memory(event.pcie_vol),
                                   _format_bandwidth(event.pcie_vol, event.cuda_time), event.count))
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/profiler/legacy/prof_utils.py` & `colossalai-nightly-2023.6.3/colossalai/utils/profiler/legacy/prof_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,17 @@
         return '{:.2f} MB'.format(nbytes * 1.0 / MB)
     elif (abs(nbytes) >= KB):
         return '{:.2f} KB'.format(nbytes * 1.0 / KB)
     else:
         return str(nbytes) + ' B'
 
 
-def _format_bandwidth(volume: float or int, time_us: int):
+def _format_bandwidth(volme: float or int, time_us: int):
     sec_div_mb = (1000.0 / 1024.0)**2
-    mb_per_sec = volume / time_us * sec_div_mb
+    mb_per_sec = volme / time_us * sec_div_mb
 
     if mb_per_sec >= 1024.0:
         return '{:.3f} GB/s'.format(mb_per_sec / 1024.0)
     else:
         return '{:.3f} MB/s'.format(mb_per_sec)
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/profiler/profiler.py` & `colossalai-nightly-2023.6.3/colossalai/utils/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/profiler/stateful_tensor_mem_extention.py` & `colossalai-nightly-2023.6.3/colossalai/utils/profiler/stateful_tensor_mem_extention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/rank_recorder/rank_recorder.py` & `colossalai-nightly-2023.6.3/colossalai/utils/rank_recorder/rank_recorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
                         'name': rec['name']
                     })
 
         shutil.rmtree(LOG_FOLDER)
         with open(self.export_name + '.json', 'w', encoding='utf-8') as f:
             json.dump(recoders, f, ensure_ascii=False)
 
-    def visualize_record(self):
+    def visualise_record(self):
         with open(self.export_name + '.json', 'r', encoding='utf-8') as f:
             records = json.load(f)
         records = dict(records)
         ranks = list(sorted(records.keys()))
 
         name_list = {}
         plots = {}
@@ -167,12 +167,12 @@
         self.dump_record()
         # if this is rank 0, wait for merge
         rank = dist.get_rank()
 
         if rank == 1:
             # take the base time of rank 0 as standard
             self.merge_recode()
-            self.visualize_record()
+            self.visualise_record()
 
 
 recorder = Recorder()
 atexit.register(recorder.exit_worker)
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/tensor_detector/tensor_detector.py` & `colossalai-nightly-2023.6.3/colossalai/utils/tensor_detector/tensor_detector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/utils/timer.py` & `colossalai-nightly-2023.6.3/colossalai/utils/timer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/zero/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/gemini/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/gemini/chunk/chunk.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/chunk/chunk.py`

 * *Files 0% similar despite different names*

```diff
@@ -412,15 +412,15 @@
         self.__update_one_tensor_info(self.tensors_info[tensor], tensor_state)
 
     def copy_tensor_to_chunk_slice(self, tensor: torch.Tensor, data_slice: torch.Tensor) -> None:
         """
         Copy data slice to the memory space indexed by the input tensor in the chunk.
 
         Args:
-            tensor (torch.Tensor): the tensor used to retrieve meta information
+            tensor (torch.Tensor): the tensor used to retrive meta information
             data_slice (torch.Tensor): the tensor to be copied to the chunk
         """
         # sanity check
         assert self.is_gathered
 
         tensor_info = self.tensors_info[tensor]
         self.cuda_global_chunk[tensor_info.offset:tensor_info.end].copy_(data_slice.data.flatten())
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/gemini/chunk/manager.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/chunk/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         self.__sub_accessed_chunk(chunk)
 
     def copy_tensor_to_chunk_slice(self, tensor: torch.Tensor, data: torch.Tensor) -> None:
         """
         Copy data to the chunk.
 
         Args:
-            tensor (torch.Tensor): the tensor used to retrieve meta information
+            tensor (torch.Tensor): the tensor used to retrive meta information
             data (torch.Tensor): the tensor to be copied to the chunk
         """
         chunk = self.tensor_chunk_map[tensor]
         chunk.copy_tensor_to_chunk_slice(tensor, data)
 
     def get_chunk(self, tensor: torch.Tensor) -> Chunk:
         """
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/gemini/chunk/search_utils.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/chunk/search_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/gemini/chunk/utils.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/chunk/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/gemini/colo_init_context.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/colo_init_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/gemini/gemini_ddp.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/gemini_ddp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import itertools
 from collections import OrderedDict
 from contextlib import nullcontext
 from functools import partial
-from typing import Dict, Iterator, List, Optional, Set, Tuple, Union
+from typing import Dict, Iterator, List, Optional, Union, Tuple, Set
 
 import torch
 import torch.distributed as dist
 import torch.nn as nn
 
 from colossalai.checkpoint_io.utils import calculate_tensor_size
-from colossalai.lazy import LazyTensor
 from colossalai.logging import get_dist_logger
 from colossalai.nn.parallel.data_parallel import ColoDDP, _cast_float, free_storage
 from colossalai.tensor import ProcessGroup as ColoProcessGroup
 from colossalai.tensor import ReplicaSpec
 from colossalai.tensor.colo_parameter import ColoParameter, ColoTensor, ColoTensorSpec
 from colossalai.tensor.param_op_hook import ColoParamOpHookManager
 from colossalai.utils import get_current_device, is_ddp_ignored
+from colossalai.utils.model.experimental import LazyTensor
 
 from .chunk import Chunk, ChunkManager, TensorState, init_chunk_manager
 from .gemini_hook import GeminiZeROHook
 from .gemini_mgr import GeminiManager
 from .memory_tracer import MemStats, OrderedParamGenerator
 from .utils import get_temp_total_chunk_on_cuda
 
@@ -47,38 +47,34 @@
             For more details, see the API reference of ``GeminiManager``.
         pin_memory (bool): Chunks on CPU Memory use pin-memory.
         force_outputs_fp32 (bool): If set to True, outputs will be fp32. Otherwise, outputs will be fp16.
             Defaults to False.
         strict_ddp_mode (bool): If set to True, there is no tensor sharding, each tensor is replicated.
             Defaults to False. Users can set it to True, when they clearly know that they only need DDP.
         scatter_after_inference (bool): If set to True, the model will be scattered after inference. This will save memory but slow down the consecutive inference.
-        mixed_precision (torch.dtype): If set to torch.float16, the model will be trained in fp16. Otherwise, the model will be trained in bf16. Defaults to torch.float16.
     """
 
     def __init__(self,
                  module: torch.nn.Module,
                  gemini_manager: GeminiManager,
                  pin_memory: bool = False,
                  force_outputs_fp32: bool = False,
                  strict_ddp_mode: bool = False,
-                 scatter_after_inference: bool = True,
-                 mixed_precision: torch.dtype = torch.float16) -> None:
-        assert mixed_precision in (torch.float16, torch.bfloat16)
+                 scatter_after_inference: bool = True) -> None:
         self.gemini_manager = gemini_manager
         self.chunk_manager: ChunkManager = gemini_manager.chunk_manager
         self.force_outputs_fp32 = force_outputs_fp32
         self.param_op_hook = GeminiZeROHook(gemini_manager)
         self.fp32_params: List[ColoTensor] = list()
         self.fp16_params: List[ColoParameter] = list()
         self.overflow_counter = 0
         self.grads_device: Dict[torch.Tensor, torch.device] = dict()
         self.param2name: Dict[nn.Parameter, str] = dict()
         self.name2param: Dict[str, nn.Parameter] = dict()
         self.scatter_after_inference = scatter_after_inference
-        self.mixed_precision = mixed_precision
 
         self._logger = get_dist_logger()
 
         if self.gemini_manager._premade_memstats_:
             # build chunk in param runtime visited order.
             param_order = self.gemini_manager.memstats()._param_runtime_order
         else:
@@ -96,46 +92,42 @@
         for name, param in module.named_parameters():
             self.param2name[param] = name
         for m_name, m_var in module.named_modules():
             for p_name, p_var in m_var.named_parameters(recurse=False):
                 param_name = m_name + '.' + p_name if m_name else p_name
                 self.name2param[param_name] = p_var
         super().__init__(module, process_group=ColoProcessGroup())
-        self._non_persistent_buffers_set = self._get_non_persistent_buffers_set(module)
+        self._non_persistent_buffers_set=self._get_non_persistent_buffers_set(module)
         self._cast_buffers()
 
-    def _get_non_persistent_buffers_set(self,
-                                        module,
-                                        memo: Optional[Set[nn.Module]] = None,
-                                        prefix: str = '',
-                                        remove_duplicate: bool = True):
-        r"""
-        Args:
-            memo: a memo to store the set of modules already added to the result
-            prefix: a prefix that will be added to the name of the module
-            remove_duplicate: whether to remove the duplicated module instances in the result
-                or not
-        """
-
-        if memo is None:
-            memo = set()
-        self_non_persistent_set = set()
-        if module not in memo:
-            if remove_duplicate:
-                memo.add(module)
-            self_non_persistent_set = set(
-                map(lambda key: prefix + ('.' if prefix else '') + key, module._non_persistent_buffers_set))
-            for name, sub_module in module._modules.items():
-                if sub_module is None:
-                    continue
-                submodule_prefix = prefix + ('.' if prefix else '') + name
-                child_non_persistent_set = self._get_non_persistent_buffers_set(sub_module, memo, submodule_prefix,
-                                                                                remove_duplicate)
-                self_non_persistent_set = set.union(self_non_persistent_set, child_non_persistent_set)
-        return self_non_persistent_set
+    def _get_non_persistent_buffers_set(self, module, memo: Optional[Set[nn.Module]] = None, prefix: str = '', remove_duplicate: bool = True):
+
+            r"""
+            Args:
+                memo: a memo to store the set of modules already added to the result
+                prefix: a prefix that will be added to the name of the module
+                remove_duplicate: whether to remove the duplicated module instances in the result
+                    or not
+            """
+
+            if memo is None:
+                memo = set()
+            self_non_persistent_set = set()
+            if module not in memo:
+                if remove_duplicate:
+                    memo.add(module)
+                self_non_persistent_set = set(map(lambda key: prefix + ('.' if prefix else '') + key, module._non_persistent_buffers_set))
+                for name, sub_module in module._modules.items():
+                    if sub_module is None:
+                        continue
+                    submodule_prefix = prefix + ('.' if prefix else '') + name
+                    child_non_persistent_set = self._get_non_persistent_buffers_set(sub_module, memo, submodule_prefix, remove_duplicate)
+                    self_non_persistent_set = set.union(self_non_persistent_set, child_non_persistent_set)
+            return self_non_persistent_set
+    
 
     def _post_forward(self):
         """This function is only triggered for inference.
         """
         access_list = list(self.chunk_manager.accessed_chunks)
         # we need to scatter all accessed chunks and move them to their original places
         for chunk in access_list:
@@ -151,15 +143,15 @@
     def forward(self, *args, **kwargs):
         # check whether we are in a inference mode
         grad_flag = torch.is_grad_enabled()
         if not grad_flag:
             assert not self.gemini_manager.need_warmup or not self.gemini_manager.is_warmup(
             ), "You should run a completed iteration as your warmup iter"
 
-        args, kwargs = _cast_float(args, self.mixed_precision), _cast_float(kwargs, self.mixed_precision)
+        args, kwargs = _cast_float(args, torch.half), _cast_float(kwargs, torch.half)
         self.module.zero_grad(set_to_none=True)
         if not grad_flag:
             outputs = self._inference_forward(*args, **kwargs)
         else:
             self.gemini_manager.pre_iter(*args)
             with ColoParamOpHookManager.use_hooks(self.param_op_hook):
                 outputs = self.module(*args, **kwargs)
@@ -570,22 +562,22 @@
 
             # ignore the parameters with no gradient
             if not p.requires_grad:
                 self.set_params_to_ignore([p])
 
             # move ignored parameters to CUDA
             if is_ddp_ignored(p):
-                p.data = p.data.to(device=get_current_device(), dtype=self.mixed_precision)
+                p.data = p.data.to(device=get_current_device(), dtype=torch.float16)
                 continue
 
             # create a fp32 parameter
             fp32_data = p.data.float()
             fp32_p = ColoTensor(fp32_data, spec=ColoTensorSpec(p.process_group))
             # create a fp16 parameter
-            p.data = p.data.to(self.mixed_precision)
+            p.data = p.data.half()
 
             # register the fp16 parameter and fp32 parameter in the chunk manager
             dp_world_size = p.process_group.dp_world_size()
             self.chunk_manager.register_tensor(tensor=p,
                                                group_type='fp16_param',
                                                config_key=dp_world_size,
                                                cpu_offload=cpu_offload,
@@ -613,15 +605,15 @@
 
     def _cast_buffers(self):
         for buffer in self.module.buffers():
             if isinstance(buffer, LazyTensor):
                 buffer.materialize()
             buffer.data = buffer.cuda()
             if torch.is_floating_point(buffer):
-                buffer.data = buffer.to(self.mixed_precision)
+                buffer.data = buffer.half()
 
     def _preprocess_param(self, p: Union[nn.Parameter, ColoParameter, 'LazyTensor']) -> None:
         """Convert parameter to ColoParameter in-place.
         Args:
             p (Union[nn.Parameter, ColoParameter, LazyTensor]): parameter to be converted
         """
         if type(p) is ColoParameter:
@@ -736,15 +728,14 @@
                  force_outputs_fp32: bool = False,
                  strict_ddp_mode: bool = False,
                  scatter_after_inference: bool = True,
                  search_range_mb: int = 32,
                  hidden_dim: Optional[int] = None,
                  min_chunk_size_mb: float = 32,
                  memstats: Optional[MemStats] = None,
-                 mixed_precision: torch.dtype = torch.float16,
                  verbose: bool = False) -> None:
         """
         A torch.Module wrapper using ZeRO-DP and Gemini.
         ZeRO is for parallel. Gemini is for memory management.
         WARNING: The class will modify the module inline!
 
         Example:
@@ -777,14 +768,9 @@
                                            init_device=device,
                                            hidden_dim=hidden_dim,
                                            search_range_mb=search_range_mb,
                                            min_chunk_size_mb=min_chunk_size_mb,
                                            strict_ddp_flag=strict_ddp_mode,
                                            verbose=verbose)
         gemini_manager = GeminiManager(placement_policy, chunk_manager, memstats)
-        super().__init__(module,
-                         gemini_manager,
-                         pin_memory,
-                         force_outputs_fp32,
-                         strict_ddp_mode,
-                         scatter_after_inference,
-                         mixed_precision=mixed_precision)
+        super().__init__(module, gemini_manager, pin_memory, force_outputs_fp32, strict_ddp_mode,
+                         scatter_after_inference)
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/gemini/gemini_hook.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/gemini_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/gemini/gemini_mgr.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/gemini_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/gemini/gemini_optimizer.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/gemini_optimizer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,34 @@
 # this code is inspired by the DeepSpeed library and implemented with our own design from scratch
 import math
 import warnings
+from enum import Enum
 from typing import Any, Dict, Set, Tuple
 
 import torch
 import torch.distributed as dist
 from torch.nn import Parameter
 from torch.optim import Optimizer
 
-from colossalai.amp.naive_amp.mixed_precision_mixin import BF16MixedPrecisionMixin, FP16MixedPrecisionMixin
+from colossalai.amp.naive_amp.grad_scaler import DynamicGradScaler
 from colossalai.logging import get_dist_logger
 from colossalai.nn.optimizer import ColossalaiOptimizer, CPUAdam, FusedAdam, HybridAdam
 from colossalai.utils import disposable, get_current_device, is_ddp_ignored
 
 from .chunk import Chunk, ChunkManager
 from .gemini_ddp import ZeroDDP
 
 __all__ = ['ZeroOptimizer', 'GeminiAdamOptimizer']
 
 _AVAIL_OPTIM_LIST = {FusedAdam, CPUAdam, HybridAdam}
 
 
-class GeminiFP16MixedPrecisionMixin(FP16MixedPrecisionMixin):
-
-    def __init__(self,
-                 module: ZeroDDP,
-                 initial_scale: float = 2**16,
-                 min_scale: float = 1,
-                 growth_factor: float = 2,
-                 backoff_factor: float = 0.5,
-                 growth_interval: int = 1000,
-                 hysteresis: int = 2,
-                 max_scale: float = 2**32) -> None:
-        super().__init__(initial_scale, min_scale, growth_factor, backoff_factor, growth_interval, hysteresis,
-                         max_scale)
-        self.module = module
-
-    def check_local_overflow(self) -> bool:
-        return self.module.overflow_counter > 0
-
-    def pre_zero_grad(self) -> None:
-        self.module.overflow_counter = 0
+class OptimState(Enum):
+    SCALED = 0
+    UNSCALED = 1
 
 
 class ZeroOptimizer(ColossalaiOptimizer):
     """A wrapper for optimizer. ``ZeroDDP`` and ``ZeroOptimizer`` implement Zero Redundancy Optimizer (ZeRO state-3).
 
     Note:
         You must use ``ZeroDDP`` with ``ZeroOptimizer``.
@@ -91,14 +75,15 @@
         super().__init__(optim)
         assert isinstance(module, ZeroDDP)
         assert type(optim) in _AVAIL_OPTIM_LIST, "You should use an optimizer in the available list:\n" \
             f"{_AVAIL_OPTIM_LIST}"
         self.module = module
         self.gemini_manager = module.gemini_manager
         self.chunk_manager: ChunkManager = self.gemini_manager.chunk_manager
+        self.optim_state = OptimState.UNSCALED
         self.param_to_range: Dict[Parameter, Tuple[int, int]] = dict()
         self.param_to_chunk32: Dict[Parameter, Chunk] = dict()
         self.chunk16_set: Set[Chunk] = set()
         self.clipping_flag = clipping_norm > 0.0
         self.max_norm = clipping_norm
         self.verbose = verbose
 
@@ -118,28 +103,23 @@
             chunk_16 = self.chunk_manager.get_chunk(p)
             if chunk_16 not in self.chunk16_set:
                 chunk_16.l2_norm_flag = self.clipping_flag
                 self.chunk16_set.add(chunk_16)
 
         self.__init__optimizer()
 
-        if module.mixed_precision is torch.float16:
-            self.mix_precision_mixin = GeminiFP16MixedPrecisionMixin(module,
-                                                                     initial_scale=initial_scale,
-                                                                     min_scale=min_scale,
-                                                                     growth_factor=growth_factor,
-                                                                     backoff_factor=backoff_factor,
-                                                                     growth_interval=growth_interval,
-                                                                     hysteresis=hysteresis,
-                                                                     max_scale=max_scale)
-        elif module.mixed_precision is torch.bfloat16:
-            self.mix_precision_mixin = BF16MixedPrecisionMixin()
-        else:
-            raise RuntimeError(f"Unsupported mixed precision type: {module.mixed_precision}")
-
+        # Grad scaler
+        self.grad_scaler = DynamicGradScaler(initial_scale=initial_scale,
+                                             min_scale=min_scale,
+                                             growth_factor=growth_factor,
+                                             backoff_factor=backoff_factor,
+                                             growth_interval=growth_interval,
+                                             hysteresis=hysteresis,
+                                             max_scale=max_scale)
+        self._found_overflow: torch.Tensor = torch.zeros(1, dtype=torch.int64, device=get_current_device())
         self._logger = get_dist_logger()
 
         self.gpu_margin_mem_ratio: float = float(gpu_margin_mem_ratio)
         assert 0.0 <= self.gpu_margin_mem_ratio <= 1.0, f'gpu_margin_mem_ratio must >=0.0 and <=1.0'
         # Only move fp32 shards from CPU to GPU when user allows and inner optimizer is valid
         # Inner optimizer must support optimizing hybrid (CPU and CUDA) tensors,
         # and it must set `num_fp32_shards_per_param` correctly
@@ -167,14 +147,23 @@
             for fake_param in group['params']:
                 assert fake_param.grad is None
                 fake_param.data = none_tensor.to(fake_param.device)
 
         for chunk16 in self.chunk16_set:
             chunk16.optim_update()
 
+    def _check_overflow(self):
+        # clear previous overflow record
+        self._found_overflow.fill_(self.module.overflow_counter)
+
+        # all-reduce across global group
+        dist.all_reduce(self._found_overflow)
+
+        return self._found_overflow.item() > 0
+
     def _clear_global_norm(self) -> None:
         for c16 in self.chunk16_set:
             c16.l2_norm = None
 
     def _calc_global_norm(self) -> float:
         norm_sqr: float = 0.0
         group_to_norm = dict()
@@ -197,63 +186,80 @@
             dist.all_reduce(comm_buffer, group=group)
             norm_sqr += comm_buffer.item()
 
         global_norm = math.sqrt(norm_sqr)
         return global_norm
 
     def _get_combined_scale(self):
-        div_scale = self.mix_precision_mixin.get_grad_div_scale()
+        loss_scale = 1
+
+        if self.optim_state == OptimState.SCALED:
+            loss_scale = self.loss_scale
+            self.optim_state = OptimState.UNSCALED
 
+        combined_scale = loss_scale
         if self.clipping_flag:
             total_norm = self._calc_global_norm()
-            clip = ((total_norm / div_scale) + 1e-6) / self.max_norm
+            clip = ((total_norm / loss_scale) + 1e-6) / self.max_norm
             if clip > 1:
-                div_scale = clip * div_scale
+                combined_scale = clip * loss_scale
 
-        return -1 if div_scale == 1.0 else div_scale
+        if combined_scale == 1:
+            return -1
+        else:
+            return combined_scale
+
+    @property
+    def loss_scale(self):
+        return self.grad_scaler.scale.item()
 
     def zero_grad(self, *args, **kwargs):
-        self.mix_precision_mixin.pre_zero_grad()
+        self.module.overflow_counter = 0
         return self.optim.zero_grad(set_to_none=True)
 
     def step(self, *args, **kwargs):
         self._maybe_move_fp32_params()
         self._set_grad_ptr()
 
-        if self.mix_precision_mixin.should_skip_step():
+        found_inf = self._check_overflow()
+        if found_inf:
+            self.optim_state = OptimState.UNSCALED    # no need to unscale grad
+            self.grad_scaler.update(found_inf)    # update gradient scaler
             if self.verbose:
                 self._logger.info(f'Found overflow. Skip step')
             self._clear_global_norm()    # clear recorded norm
             self.zero_grad()    # reset all gradients
             self._update_fp16_params()
             return
 
         # get combined scale. combined scale = loss scale * clipping norm
         # so that gradient = gradient / combined scale
         combined_scale = self._get_combined_scale()
+        self.grad_scaler.update(found_inf)
 
         ret = self.optim.step(div_scale=combined_scale, *args, **kwargs)
         self._register_states()
         self.zero_grad()
         self._update_fp16_params()
         return ret
 
     def clip_grad_norm(self, model: torch.nn.Module, max_norm: float, norm_type: float = 2.0):
         raise NotImplementedError
 
     def backward(self, loss: torch.Tensor):
-        loss = self.mix_precision_mixin.pre_backward(loss)
+        loss = self.loss_scale * loss
+        self.optim_state = OptimState.SCALED
         self.module.backward(loss)
 
     def backward_by_grad(self, tensor: torch.Tensor, grad: torch.Tensor):
         # This function is called except the last stage of pipeline parallel
         # It receives the scaled grad from the previous rank
         # No need to scale the grad again
         # Need to unscale when optimizing
-        grad = self.mix_precision_mixin.pre_backward_by_grad(grad)
+        self.optim_state = OptimState.SCALED
         self.module.backward_by_grad(tensor, grad)
 
     def _maybe_move_fp32_params(self):
         if self._should_move_fp32_params_h2d:
             self._should_move_fp32_params_h2d = False
             available_cuda_margin_mem = self.gemini_manager.cuda_margin_mem * self.gpu_margin_mem_ratio
             fp32_params_available_cuda_margin_mem = available_cuda_margin_mem / self.optim.num_fp32_shards_per_param
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/gemini/memory_tracer/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         """
         super().__init__(memstats)
         self._chunk_manager = chunk_manager
 
     # override
     def record_model_data_volume(self) -> None:
         """
-        record model data volume on cuda and cpu.
+        record model data volumn on cuda and cpu.
         """
         if self._start_flag and not self.use_outside_memstats:
             cuda_mem = self._chunk_manager.total_mem['cuda']
             self._memstats.record_max_cuda_model_data(cuda_mem)
 
     @property
     def cuda_margin_mem(self) -> float:
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/gemini/memory_tracer/memory_monitor.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/memory_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     def clear(self):
         self.mem_stats.clear()
         self.time_stamps.clear()
 
 
 class AsyncMemoryMonitor(MemoryMonitor):
     """
-    An Async Memory Monitor running during computing. Sampling memory usage of the current GPU
+    An Async Memory Monitor runing during computing. Sampling memory usage of the current GPU
     at interval of `1/(10**power)` sec.
 
     The idea comes from Runtime Memory Tracer of PatrickStar
     `PatrickStar: Parallel Training of Pre-trained Models via Chunk-based Memory Management`_
 
     Usage::
 
@@ -63,15 +63,15 @@
         async_mem_monitor.finish()
         async_mem_monitor.start()
         output = OP2(output)
         async_mem_monitor.finish()
         async_mem_monitor.save('log.pkl')
 
     Args:
-        power (int, optional): the power of time interval. Defaults to 10.
+        power (int, optional): the power of time interva. Defaults to 10.
 
     .. _PatrickStar: Parallel Training of Pre-trained Models via Chunk-based Memory Management:
         https://arxiv.org/abs/2108.05818
     """
 
     def __init__(self, power: int = 10):
         super().__init__()
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/gemini/memory_tracer/memory_stats.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/memory_stats.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/gemini/memory_tracer/memstats_collector.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/gemini/memory_tracer/param_runtime_order.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/param_runtime_order.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/gemini/memory_tracer/utils.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/memory_tracer/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import torch
 
 
 def colo_model_optimizer_usage(optim) -> Tuple[int, int]:
     """Trace the optimizer memory usage
 
     Args:
-        optim (ShardedOptimV2): an instance of ShardedOptimizer
+        optim (ShardedOptimV2): an instance of ShardedOptimver
 
     Returns:
         Tuple[int, int]: cuda/cpu memory usage in Byte
     """
     if optim is None:
         return 0, 0
     assert hasattr(optim, 'get_memory_usage'), f"{type(optim)} has no attr get_memory_usage()"
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/gemini/placement_policy.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/placement_policy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/gemini/utils.py` & `colossalai-nightly-2023.6.3/colossalai/zero/gemini/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     Thus, you can use the original model in further training.
     But you should not use the returned torch model to train, this can cause unexpected errors.
 
     Args:
         zero_ddp_model (ZeroDDP): a zero ddp model
         device (torch.device): the device of the final torch model
         dtype (torch.dtype): the dtype of the final torch model
-        only_rank_0 (bool): if True, only rank0 has the converted torch model
+        only_rank_0 (bool): if True, only rank0 has the coverted torch model
 
     Returns:
         torch.nn.Module: a static torch model used for saving checkpoints or numeric checks
     """
     from colossalai.zero.gemini.gemini_ddp import ZeroDDP
     assert isinstance(zero_ddp_model, ZeroDDP)
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/__init__.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/gemini_context.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/gemini_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/ophooks/utils.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/ophooks/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,30 +84,30 @@
         return (None, None) + args
 
 
 def register_ophooks_recursively(module: torch.nn.Module,
                                  ophook_list: List[BaseOpHook],
                                  name: str = "",
                                  filter_fn: Optional[Callable] = None):
-    r"""Recursively register pre/post hooks for all submodules in the module in FWD and BWD."""
+    r"""Recursilvely register pre/post hooks for all submodules in the module in FWD and BWD."""
     assert isinstance(module, torch.nn.Module)
     assert isinstance(ophook_list, (list, tuple))
     assert len(ophook_list) > 0, 'expected at least 1 hook in the argument ophook_list but found 0'
     for hook in ophook_list:
         assert (isinstance(hook, BaseOpHook))
 
     # Add hooks for submodules
     for child_name, child in module.named_children():
         register_ophooks_recursively(child, ophook_list, name + child_name, filter_fn)
 
     # Early return on modules with no parameters.
     if len(list(module.parameters(recurse=False))) == 0:
         return
 
-    # return from filtered module
+    # return from flitered module
     if filter_fn is not None and filter_fn(module):
         return
 
     def _pre_forward_module_hook(submodule, *args):
         for hook in ophook_list:
             assert isinstance(submodule, torch.nn.Module)
             hook.pre_fwd_exec(submodule, *args)
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/stateful_tensor.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/stateful_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/tensor_placement_policy.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/tensor_placement_policy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/gemini/tensor_utils.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/gemini/tensor_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 def colo_model_data_tensor_move_inline(t: Union[StatefulTensor, torch.Tensor], target_device: Union[torch.device,
                                                                                                     int]) -> None:
     """
     move a tensor to the target_device
     Args:
         t (Union[StatefulTensor, torch.Tensor]): the tensor be moved
-        target_device: a target device, if type is int, it the index of cuda card.
+        target_device: a traget device, if type is int, it the index of cuda card.
     """
     if not isinstance(target_device, torch.device):
         target_device = torch.device(f'cuda:{target_device}')
 
     if isinstance(t, torch.Tensor):
         t.data = t.data.to(target_device)
     elif isinstance(t, StatefulTensor):
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/init_ctx/init_context.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/init_ctx/init_context.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from colossalai.context.parallel_mode import ParallelMode
 from colossalai.context.singleton_meta import SingletonMeta
 from colossalai.core import global_context as gpc
 from colossalai.logging import get_dist_logger
 from colossalai.utils.model.utils import InsertPostInitMethodToModuleSubClasses
 from colossalai.zero.legacy.shard_utils import BaseShardStrategy
-from colossalai.zero.legacy.sharded_model._utils import cast_tensor_to_bf16, cast_tensor_to_fp16
+from colossalai.zero.legacy.sharded_model._utils import cast_tensor_to_fp16
 from colossalai.zero.legacy.sharded_model.sharded_model_v2 import ShardedModelV2
 from colossalai.zero.legacy.sharded_param import ShardedParamV2
 
 
 @dataclass
 class ZeroContextConfig:
     """The configuration used to control zero context initialization.
@@ -42,42 +42,39 @@
             assert self.target_device.type == 'cuda', "Replicated no-shard parameters should be located in cuda."
 
 
 class ZeroInitContext(InsertPostInitMethodToModuleSubClasses):
     """A context to initialize model.
 
     1. Convert the model to fp16.
-    2. The parameters of the module are adapted to type ShardedParameter.
+    2. The paramaters of the module are adapted to type ShardedParameter.
     3. Shard the param and grad according to flags.
 
     Args:
         target_device (torch.device): The device where param data are after exiting the context.
         shard_strategy (BaseShardStrategy): Shard strategy instance.
         seed (int, optional): Random seed for weight initialization
         shard_param (bool, optional): Is param sharded after exiting the context. Defaults to False.
         default_dtype (torch.dtype, optional): If it's not None, parameters will be initialized as ``default_dtype`` then converted to fp16.
-        bf16 (bool, optional): If it's True, parameters will be initialized as ``torch.bfloat16``. Otherwise, parameters will be initialized as ``torch.float16``. Defaults to False.
         model_numel_tensor (torch.Tensor, optional): A tensor which will store the number of elements of model. Defaults to torch.zeros(1, dtype=torch.int).
     """
 
     def __init__(self,
                  target_device: torch.device,
                  shard_strategy: BaseShardStrategy,
                  seed: int = 2**10 - 1,
                  shard_param: bool = False,
                  default_dtype: Optional[torch.dtype] = None,
-                 bf16: bool = False,
                  model_numel_tensor: torch.Tensor = torch.zeros(1, dtype=torch.long)):
 
         super().__init__(default_dtype=default_dtype)
         self.shard_strategy = shard_strategy
         self.param_list = []
         self.model_numel_tensor = model_numel_tensor
         self.seed = seed
-        self.bf16 = bf16
         self.dp_process_group = gpc.get_group(ParallelMode.DATA)
 
         self.config = ZeroContextConfig(target_device=target_device, is_replicated=True, shard_param=shard_param)
 
         ZeroContextMgr().current_context = self
 
         self.param_numel = {}
@@ -182,18 +179,17 @@
 
     def _post_init_method(self, module: torch.nn.Module, *args, **kwargs):
         """
         The function to call at the end of the constructor of each module.
         NOTE() The module may be passed to this function multiple times.
         """
         self.top_module = module
-        half_dtype = torch.float16 if not self.bf16 else torch.bfloat16
 
         def half_fn(t: torch.Tensor):
-            return t.to(half_dtype) if t.is_floating_point() else t
+            return t.half() if t.is_floating_point() else t
 
         for param in module.parameters(recurse=False):
             # avoid adapting a param to ShardedParam twice
             if hasattr(param, 'colo_attr'):
                 continue
 
             self.param_numel[param] = param.numel()
@@ -226,18 +222,17 @@
             param.colo_attr.keep_not_shard = not self.shard_param
 
             self.param_list.append(param)
 
         # We must cast buffers
         # If we use BN, buffers may be on CPU and Float
         # We must cast them
-        cast_fn = cast_tensor_to_fp16 if not self.bf16 else cast_tensor_to_bf16
         for buffer in module.buffers(recurse=False):
             buffer.data = buffer.data.to(device=torch.cuda.current_device())
-            buffer.data = cast_fn(buffer.data)
+            buffer.data = cast_tensor_to_fp16(buffer.data)
 
 
 class ZeroContextMgr(metaclass=SingletonMeta):
     current_context: Optional[ZeroInitContext] = None
 
     @contextlib.contextmanager
     def hijack_context_config(self, **kwargs):
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/shard_utils/base_shard_strategy.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/shard_utils/base_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/shard_utils/commons.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/shard_utils/commons.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_model/_utils.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,27 +39,19 @@
     return tensor
 
 
 def cast_tensor_to_fp32(tensor: Union[torch.Tensor, StatefulTensor]) -> torch.Tensor:
     if isinstance(tensor, StatefulTensor):
         tensor = tensor.payload
 
-    if torch.is_floating_point(tensor) and tensor.dtype in (torch.float16, torch.bfloat16):
+    if torch.is_floating_point(tensor) and tensor.dtype is torch.float16:
         return tensor.float()
     return tensor
 
 
-def cast_tensor_to_bf16(tensor: torch.Tensor) -> torch.Tensor:
-    if isinstance(tensor, StatefulTensor):
-        tensor = tensor.payload
-    if torch.is_floating_point(tensor) and tensor.dtype is torch.float32:
-        return tensor.bfloat16()
-    return tensor
-
-
 def apply_to_tensors(x: Any, fn: Callable):
     if torch.is_tensor(x):
         return fn(x)
     elif isinstance(x, list):
         return [apply_to_tensors(t, fn) for t in x]
     elif isinstance(x, tuple):
         return tuple(apply_to_tensors(t, fn) for t in x)
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_model/reduce_scatter.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/reduce_scatter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_model/sharded_model_v2.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/sharded_model_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from colossalai.zero.legacy.gemini.tensor_placement_policy import TensorPlacementPolicy, TensorPlacementPolicyFactory
 from colossalai.zero.legacy.gemini.tensor_utils import colo_model_data_move_to_cpu
 from colossalai.zero.legacy.shard_utils import BaseShardStrategy
 from colossalai.zero.legacy.sharded_model.reduce_scatter import ReduceScatterBucketer
 
 from ._utils import (
     cast_float_arguments,
-    cast_tensor_to_bf16,
     cast_tensor_to_fp16,
     cast_tensor_to_fp32,
     chunk_and_pad,
     free_storage,
     get_gradient_predivide_factor,
 )
 from .zero_hook import ZeroHook
@@ -65,40 +64,37 @@
         fp32_reduce_scatter (bool, optional): If set to `True`, gradients are forced to FP32 before reduce-scatter. Defaults to False.
         tensor_placement_policy (str): Which device to place *held* tensors. It can be 'cpu', 'cuda' and 'auto'.
             If it's 'cpu', parameters, gradients and optimizer states will be offloaded to CPU, which means min CUDA memory will be used.
             If it's 'cuda', they won't be offloaded, which means max CUDA memory will be used.
             If it's 'auto', they are moving dynamically based on CPU and CUDA memory usage. It will utilize heterogeneous memory space evenly and well.
             Note that 'auto' policy can only work well when no other processes use CUDA during your training.
             Defaults to 'cuda'.
-        gradient_predivide_factor (Optional[float], optional): Gradient is divided by this value before reduce-scatter. Defaults to 1.0.
+        gradient_predivide_factor (Optional[float], optional): Gradient is divived by this value before reduce-scatter. Defaults to 1.0.
         reuse_fp16_shard (bool, optional): Whether to reuse fp16 shard for param and grad.
             Enabling this can reduce GPU memory usage, but you have to make sure you disable it when using gradient accumulation.
             In this mode, grad will be fp16. Make sure your optimizer supports mixed precision (fp32 param and fp16 grad).
             We find that PyTorch's optimizers don't support mixed precision,
             so we recommend you enable this only when using our CPUAdam with CPU offload. Defaults to False.
-        bf16 (bool, optional): Whether to use bfloat16 for param and grad. Defaults to False.
     """
 
     def __init__(self,
                  module: nn.Module,
                  shard_strategy: BaseShardStrategy,
                  process_group: Optional[ProcessGroup] = None,
                  reduce_scatter_process_group: Optional[ProcessGroup] = None,
                  reduce_scatter_bucket_size_mb: int = 25,
                  fp32_reduce_scatter: bool = False,
                  tensor_placement_policy: str = 'cuda',
                  gradient_predivide_factor: Optional[float] = 1.0,
                  reuse_fp16_shard: bool = False,
-                 bf16: bool = False,
                  *args,
                  **kwargs):
         assert not isinstance(module, ShardedModelV2), 'Nested ShardedModelV2 is not supported.'
         super().__init__()
         self.logger = get_dist_logger()
-        self.bf16 = bf16
 
         # We force users to use ZeroInitContext
         for submodule in module.modules():
             sharded_cnt = 0
             unshard_cnt = 0
             for param in submodule.parameters(recurse=False):
                 assert hasattr(param, 'colo_attr'), 'You must use ZeroInitContext to init your module first.'
@@ -201,15 +197,15 @@
             # forward: model(inputs)
             # backward: optimizer.backward()
         except Exception as e:
             model.dump_memory_stats()
             exit(0)
         """
         if self._use_memory_tracer:
-            self.logger.error(f'dump memory tracer collected information to a {filename}', ranks=[0])
+            self.logger.error(f'dump memort tracer collected information to a {filename}', ranks=[0])
             if gpc.get_global_rank() == 0:
                 with open(filename, 'w+') as f:
                     f.write(f'cuda reserved {torch.cuda.memory_reserved(get_current_device()) / 1e9} GB\n')
                     f.write(f'cuda max allocated {torch.cuda.max_memory_allocated(get_current_device()) / 1e9} GB\n')
                     f.write('CUDA model data (GB)\n')
                     f.write('\n')
                     f.write('CUDA non model data (GB)\n')
@@ -232,16 +228,15 @@
     def _post_forward_operations(self):
         for p in self.module.parameters():
             if hasattr(p, 'colo_attr'):
                 p.colo_attr.sharded_data_tensor.trans_state(TensorState.HOLD)
 
     def forward(self, *args: Any, **kwargs: Any) -> torch.Tensor:
         self._pre_forward_operations(*args)
-        cast_fn = cast_tensor_to_bf16 if self.bf16 else cast_tensor_to_fp16
-        args, kwargs = cast_float_arguments(cast_fn, *args, **kwargs)
+        args, kwargs = cast_float_arguments(cast_tensor_to_fp16, *args, **kwargs)
         outputs = self.module(*args, **kwargs)
         self._post_forward_operations()
         return outputs
 
     def backward(self, loss):
         loss.backward()
         self._post_backward_operations()
@@ -381,15 +376,15 @@
         if param.colo_attr.offload_grad:
             colo_model_data_move_to_cpu(grad)
 
         if self.reuse_fp16_shard:
             # make parameters point to gradient
 
             assert param.colo_attr.saved_grad.is_null(
-            ), 'Gradient accumulation is not supported when reuse_fp16_shard=True'
+            ), 'Gradien accumulation is not supported when reuse_fp16_shard=True'
 
             param.colo_attr.grad_payload_reset(grad.data)
             # release the memory of param
             # we set a false None for parameter's payload
             # so we can get parameter's device and dtype later in optimizer
             param.colo_attr.data_payload_reset(torch.empty(0, device=grad.device, dtype=grad.dtype))
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_model/utils.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_model/zero_hook.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_model/zero_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,15 +90,14 @@
                  verbose: bool = False) -> None:
         assert isinstance(sharded_model, ShardedModelV2), 'model must be wrapped with ShardedModel'
         assert not isinstance(optimizer, ShardedOptimizerV2), 'Nested ShardedOptimizerV2 is not supported.'
 
         super().__init__(optimizer)
         self.shard_strategy = sharded_model.shard_strategy
         self.model: ShardedModelV2 = sharded_model
-        self.bf16 = sharded_model.bf16
 
         self.gpu_margin_mem_ratio: float = float(gpu_margin_mem_ratio)
         assert 0.0 <= self.gpu_margin_mem_ratio <= 1.0, f'gpu_margin_mem_ratio must >=0.0 and <=1.0'
         # Only move fp32 shards from CPU to GPU when user allows and inner optimizer is valid
         # Inner optimizer must support optimizing hybrid (CPU and CUDA) tensors,
         # and it must set `num_fp32_shards_per_param` correctly
         self._should_move_fp32_shards_h2d: bool = sharded_model.cpu_offload and self.gpu_margin_mem_ratio > 0.0 and getattr(
@@ -114,15 +113,14 @@
                                              backoff_factor=backoff_factor,
                                              growth_interval=growth_interval,
                                              hysteresis=hysteresis,
                                              max_scale=max_scale)
         self._found_overflow: Tensor = torch.IntTensor([0]).to(torch.cuda.current_device())
         self._logger = get_dist_logger("ShardedOptimizerV2")
         self._verbose = verbose
-        self._grad_prepared: bool = False    # this should be set to true when _prepare_grads() and reset to false when backward
 
         # Store fp32 param shards
         self._register_master_weight()
         if self.gpu_margin_mem_ratio != 0.0 and not isinstance(sharded_model._tensor_placement_policy,
                                                                AutoTensorPlacementPolicy):
             self._logger.warning(f'gpu_margin_mem_ratio is meaningless when tensor_placement_policy is not "auto"',
                                  ranks=[0])
@@ -164,52 +162,47 @@
 
         return cuda_use, cpu_use
 
     def zero_grad(self, *args, **kwargs):
         self._zero_grad()
 
     def backward(self, loss: Tensor) -> None:
-        if not self.bf16:
-            loss = self.loss_scale * loss
-            self.optim_state = OptimState.SCALED
-        self._grad_prepared = False
+        loss = self.loss_scale * loss
+        self.optim_state = OptimState.SCALED
         self.model.backward(loss)
 
     def backward_by_grad(self, tensor: Tensor, grad: Tensor) -> None:
         # This function is called except the last stage of pipeline parallel
         # It receives the scaled grad from the previous rank
         # No need to scale the grad again
         # Need to unscale when optimizing
-        if not self.bf16:
-            self.optim_state = OptimState.SCALED
-        self._grad_prepared = False
+        self.optim_state = OptimState.SCALED
         self.model.backward_by_grad(tensor, grad)
 
     def clip_grad_norm(self, model: nn.Module, max_norm: float):
-        self._prepare_grads()
-        if not self.bf16 and self.optim_state == OptimState.SCALED:
+        if self.optim_state == OptimState.SCALED:
+            self._prepare_grads()
             self._unscale_grads()
         return super().clip_grad_norm(model, max_norm)
 
     def step(self, *args, **kwargs):
 
-        self._prepare_grads()
         # unscale grads if scaled
-        if not self.bf16 and self.optim_state == OptimState.SCALED:
+        if self.optim_state == OptimState.SCALED:
+            self._prepare_grads()
             self._unscale_grads()
 
         self._maybe_move_fp32_shards()
-        if not self.bf16:
-            found_inf = self._check_overflow()
-            self.grad_scaler.update(found_inf)
-
-            if found_inf:
-                self._logger.warning('found inf during ShardedOptimV2 step')
-                self._zero_grad(recover_data=True)
-                return
+        found_inf = self._check_overflow()
+        self.grad_scaler.update(found_inf)
+
+        if found_inf:
+            self._logger.warning('found inf during ShardedOptimV2 step')
+            self._zero_grad(recover_data=True)
+            return
 
         self._point_param_fp16_to_master_param()
 
         if self._verbose:
             gpu_mem, cpu_mem = self.get_memory_usage()
             self._logger.debug(
                 f"Before step ShardedOptimizerV2 consumes {gpu_mem / 1e6} MB CUDA Memory, {cpu_mem / 1e6} MB CUDA Memory!",
@@ -307,16 +300,14 @@
                         fp32_shards_used_cuda_margin_mem += shard_mem
                         state = self.optim.state[p]
                         for k, v in state.items():
                             if isinstance(v, Tensor):
                                 state[k] = v.cuda()
 
     def _prepare_grads(self):
-        if self._grad_prepared:
-            return
         for group in self.optim.param_groups:
             for p in group['params']:
                 if p.colo_attr.saved_grad.is_null():
                     continue
                 p.colo_attr.saved_grad.trans_state(TensorState.COMPUTE)
                 # If reuse_fp16_shard, grad fp16 which wasn't be offloaded may be evicted to CPU
                 if not p.colo_attr.offload_grad:
@@ -325,15 +316,14 @@
                 # If we change p.grad directly
                 # it may raise error because of different shape/dtype/device of p.data and p.grad
                 # We just set p.data = p.colo_attr.saved_grad.payload here
                 p.data = p.colo_attr.grad_payload
                 p.grad = p.colo_attr.grad_payload
                 # Set p.data to empty tensor, in case of memory leaking
                 p.colo_attr.set_data_none()
-        self._grad_prepared = True
 
     def _point_param_fp16_to_master_param(self):
         # assign master param pointers to p.data.
         # We will not trigger data copy here.
         for group in self.optim.param_groups:
             for p in group['params']:
                 self.master_params[p].trans_state(TensorState.COMPUTE)
@@ -363,16 +353,15 @@
         # we need to allocate new memory for keep_not_shard parameters
         # in order to use copy, otherwise, the sizes of tensor is not compatible
         if p.colo_attr.data_payload.numel() != p.data.numel():
             p.colo_attr.data_payload_reset(
                 torch.empty(p.data.shape, dtype=p.colo_attr.data_payload.dtype, device=p.colo_attr.data_payload.device))
 
         # TODO() optimize this line CPU (fp32) -> GPU (fp16)
-        half_dtype = torch.bfloat16 if self.bf16 else torch.float16
-        p.colo_attr.sharded_data_tensor.payload_copy(p.to(half_dtype).detach())
+        p.colo_attr.sharded_data_tensor.payload_copy(p.half().detach())
         p.colo_attr.set_data_none()
 
         if p.colo_attr.keep_not_shard and p.colo_attr.is_replicated:
             # We gather full fp16 param here
             p.colo_attr.sharded_data_tensor.is_sharded = True    # since only gradient is sharded, we should set to True
             self.shard_strategy.gather([p.colo_attr.sharded_data_tensor], self.dp_process_group)
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_param/sharded_param.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_param/sharded_param.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/legacy/sharded_param/sharded_tensor.py` & `colossalai-nightly-2023.6.3/colossalai/zero/legacy/sharded_param/sharded_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/low_level/_utils.py` & `colossalai-nightly-2023.6.3/colossalai/zero/low_level/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,15 @@
     """
     Synchronize the flattened tensor and unflattened tensor list. When
     a list of tensor are flattened with `torch._utils._unflatten_dense_tensors`,
     a new tensor is created. Thus, the flat tensor and original tensor list do not
     share the same memory space. This function will update the tensor list so that
     they point to the same value.
 
-    :param flat_tensor: A flat tensor obtained by calling `torch._utils._unflatten_dense_tensors` on a tensor list
+    :param flat_tensor: A flat tensor obtained by calling `torch._utils._unflatten_dense_tensors` on a tensor lsit
     :param tensor_list: A list of tensors corresponding to the flattened tensor
     :type flat_tensor: torch.Tensor
     :type tensor_list: List[torch.Tensor]
     """
     updated_params = unflatten(flat_tensor, tensor_list)
 
     # update the tensor data
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/low_level/bookkeeping/bucket_store.py` & `colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/bucket_store.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/low_level/bookkeeping/gradient_store.py` & `colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/gradient_store.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/low_level/bookkeeping/parameter_store.py` & `colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/parameter_store.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/low_level/bookkeeping/tensor_bucket.py` & `colossalai-nightly-2023.6.3/colossalai/zero/low_level/bookkeeping/tensor_bucket.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/low_level/low_level_optim.py` & `colossalai-nightly-2023.6.3/colossalai/zero/low_level/low_level_optim.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 from functools import partial
 from typing import Optional
 
 import torch
 import torch.distributed as dist
 from torch.optim import Optimizer
 
-from colossalai.amp.naive_amp.mixed_precision_mixin import (
-    BF16MixedPrecisionMixin,
-    FP16MixedPrecisionMixin,
-    MixedPrecisionMixin,
-)
+from colossalai.amp.naive_amp.grad_scaler import DynamicGradScaler
 from colossalai.context import ParallelMode
 from colossalai.core import global_context as gpc
 from colossalai.logging import get_dist_logger
 from colossalai.nn.optimizer import ColossalaiOptimizer
 from colossalai.tensor import ColoParameter, ProcessGroup
 from colossalai.utils.cuda import get_current_device
 
@@ -27,39 +23,14 @@
     release_param_grad,
     split_by_dtype,
     sync_param,
 )
 from .bookkeeping import BucketStore, GradientStore, ParameterStore, TensorBucket
 
 
-class LowLevelZeroFP16MixedPrecisionMixin(FP16MixedPrecisionMixin):
-
-    def __init__(self,
-                 num_working_param_groups: int,
-                 grad_store: GradientStore,
-                 initial_scale: float = 2**16,
-                 min_scale: float = 1,
-                 growth_factor: float = 2,
-                 backoff_factor: float = 0.5,
-                 growth_interval: int = 1000,
-                 hysteresis: int = 2,
-                 max_scale: float = 2**32) -> None:
-        super().__init__(initial_scale, min_scale, growth_factor, backoff_factor, growth_interval, hysteresis,
-                         max_scale)
-        self.num_working_param_groups = num_working_param_groups
-        self.grad_store = grad_store
-
-    def check_local_overflow(self) -> bool:
-        for group_id in range(self.num_working_param_groups):
-            for avg_grad in self.grad_store.get_averaged_gradients_by_group(group_id):
-                if avg_grad is not None and has_inf_or_nan(avg_grad):
-                    return True
-        return False
-
-
 class LowLevelZeroOptimizer(ColossalaiOptimizer):
     """Optimizer used for ZeRO-1 and ZeRO-2.
     """
 
     def __init__(
             self,
             optimizer: Optimizer,
@@ -125,14 +96,25 @@
         self._master_flat_param_groups_of_current_rank = dict()
 
         # communication params
         self._overlap_communication = overlap_communication
         self._reduce_bucket_size = reduce_bucket_size
         self._communication_dtype = communication_dtype
 
+        # gradient scaler
+        self.grad_scaler = DynamicGradScaler(initial_scale=initial_scale,
+                                             min_scale=min_scale,
+                                             growth_factor=growth_factor,
+                                             backoff_factor=backoff_factor,
+                                             growth_interval=growth_interval,
+                                             hysteresis=hysteresis,
+                                             max_scale=max_scale,
+                                             verbose=verbose)
+        self._found_overflow = torch.FloatTensor([0]).to(get_current_device())
+
         # gradient clipping
         self._clip_grad_norm = clip_grad_norm
 
         if forced_dtype:
             for group in self.optim.param_groups:
                 group_params = group['params']
                 for param in group_params:
@@ -203,45 +185,34 @@
             # managed by this data parallel rank
             param_group['params'] = [master_flat_current_rank]
 
             # set reduction state
             for param in self._working_param_groups[group_id]:
                 self._param_store.set_param_reduction_state(param, False)
 
-        # initialize communication stream for
-        # communication-computation overlapping
+        # intialize communication stream for
+        # communication-compuation overlapping
         if self._overlap_communication:
             self._comm_stream = torch.cuda.Stream()
 
         # reduction hook is only used if overlapping communication
         # or stage 2 is used
         # if it is stage 1 without overlapping, no hook will be attached
         if self._overlap_communication or self._partition_grads:
             self._attach_reduction_hook()
 
-        # initialize mixed precision mixin
-        self.mixed_precision_mixin: Optional[MixedPrecisionMixin] = None
-        if self._dtype is torch.float16:
-            self.mixed_precision_mixin = LowLevelZeroFP16MixedPrecisionMixin(self.num_param_groups,
-                                                                             self._grad_store,
-                                                                             initial_scale=initial_scale,
-                                                                             min_scale=min_scale,
-                                                                             growth_factor=growth_factor,
-                                                                             backoff_factor=backoff_factor,
-                                                                             growth_interval=growth_interval,
-                                                                             hysteresis=hysteresis,
-                                                                             max_scale=max_scale)
-        elif self._dtype is torch.bfloat16:
-            self.mixed_precision_mixin = BF16MixedPrecisionMixin()
-
     @property
     def dtype(self):
         return self._dtype
 
     @property
+    def loss_scale(self):
+        return self.grad_scaler.scale
+
+    @property
     def num_param_groups(self):
         return len(self._working_param_groups)
 
     def _sanity_checks(self):
         assert torch.cuda.is_available(), 'CUDA is required'
         for param_group in self.optim.param_groups:
             group_params = param_group['params']
@@ -265,15 +236,15 @@
                     raise RuntimeError("All parameters should be ColoParameter if you use ColoParameter.")
         return colo_pg
 
     def _partition_param_list(self, param_list):
         params_per_rank = [[] for _ in range(self._world_size)]
         numel_per_rank = [0 for _ in range(self._world_size)]
 
-        # partition the parameters in a greedy fashion
+        # partititon the parameters in a greedy fashion
         sorted_params = sorted(param_list, key=lambda x: x.numel(), reverse=True)
         for param in sorted_params:
             # allocate this parameter to the rank with
             # the smallest numel for load balancing purpose
             rank_to_go = numel_per_rank.index(min(numel_per_rank))
             params_per_rank[rank_to_go].append(param)
             numel_per_rank[rank_to_go] += param.numel()
@@ -293,15 +264,15 @@
     def _attach_reduction_hook(self):
         # we iterate over the working params
         # on each param, we register a hook to its AccumulateGrad object
         for group_id in range(self.num_param_groups):
             param_group = self._working_param_groups[group_id]
             for param in param_group:
                 if param.requires_grad:
-                    # determines the reduction destination rank
+                    # determines the reduction destionation rank
                     # this is only valid for stage 2
                     # dst_rank = None means using all-reduce
                     # else using reduce
                     if self._partition_grads:
                         reduce_rank = self._param_store.get_param_rank(param)
                     else:
                         reduce_rank = None
@@ -417,16 +388,15 @@
         self._bucket_store.add_param(param, reduce_rank)
 
     ################################
     # torch.optim.Optimizer methods
     ################################
 
     def backward(self, loss, retain_graph=False, sync_grad=True):
-        if self.mixed_precision_mixin is not None:
-            loss = self.mixed_precision_mixin.pre_backward(loss)
+        loss = self.loss_scale * loss
         loss.backward(retain_graph=retain_graph)
 
         # finish gradient reduction
         if not self._partition_grads:
             self._reduce_grad_stage1()
         else:
             # TODO: support async comm in reduce
@@ -445,16 +415,14 @@
         """
         Set parameter gradients to zero. If set_to_none = True, gradient
         will be set to None to save memory.
 
         :param set_to_none: Whether set the gradient to None. Default value is True.
         :type set_to_none: bool
         """
-        if self.mixed_precision_mixin is not None:
-            self.mixed_precision_mixin.pre_zero_grad()
         for _, param_group in self._working_param_groups.items():
             for param in param_group:
                 if set_to_none:
                     param.grad = None
                 else:
                     if param.grad is not None:
                         param.grad.detach()
@@ -463,15 +431,20 @@
     ####################
     # Update Parameter #
     ####################
 
     def step(self, closure=None):
         assert closure is None, 'closure is not supported by step()'
 
-        if self.mixed_precision_mixin is not None and self.mixed_precision_mixin.should_skip_step():
+        # check for overflow
+        found_inf = self._check_overflow()
+        self.grad_scaler.update(found_inf)
+
+        # update loss scale if overflow occurs
+        if found_inf:
             self._grad_store.reset_all_average_gradients()
             if self._verbose:
                 self._logger.info(f'Found overflow. Skip step')
             self.zero_grad()
             return
 
         # copy the grad of working param to master param
@@ -530,28 +503,49 @@
         for handle in handles:
             handle.wait()
 
     #############################
     # Mixed Precision Utilities #
     #############################
 
+    def _check_overflow(self):
+        # clear previous overflow record
+        self._found_overflow.fill_(0.0)
+
+        # check for overflow
+        for group_id in range(len(self._working_param_groups)):
+            for avg_grad in self._grad_store.get_averaged_gradients_by_group(group_id):
+                if avg_grad is not None and has_inf_or_nan(avg_grad):
+                    self._found_overflow.fill_(1.0)
+                    break
+
+        # all-reduce across dp group
+        dist.all_reduce(self._found_overflow, op=dist.ReduceOp.MAX, group=self._dp_torch_group)
+
+        # all-reduce over model parallel group
+        if self._mp_torch_group:
+            dist.all_reduce(self._found_overflow, op=dist.ReduceOp.MAX, group=self._mp_torch_group)
+
+        if self._found_overflow.item() > 0:
+            return True
+        else:
+            return False
+
     def _unscale_and_clip_grads(self, grad_groups_flat, total_norm):
         # compute combined scale factor for this group
-        div_scale = 1.0
-        if self.mixed_precision_mixin is not None:
-            div_scale = self.mixed_precision_mixin.get_grad_div_scale()
+        combined_scale = self.loss_scale
 
         if self._clip_grad_norm > 0.:
             # norm is in fact norm*scale
-            clip = ((total_norm / div_scale) + 1e-6) / self._clip_grad_norm
+            clip = ((total_norm / self.loss_scale) + 1e-6) / self._clip_grad_norm
             if clip > 1:
-                div_scale = clip * div_scale
+                combined_scale = clip * self.loss_scale
 
         for grad in grad_groups_flat:
-            grad.data.mul_(1. / div_scale)
+            grad.data.mul_(1. / combined_scale)
 
     ############################
     # Gradient Synchronization #
     ############################
 
     def _sync_grad(self):
         # update param already reduced flag
```

### Comparing `colossalai-nightly-2023.6.17/colossalai/zero/wrapper.py` & `colossalai-nightly-2023.6.3/colossalai/zero/wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/colossalai_nightly.egg-info/PKG-INFO` & `colossalai-nightly-2023.6.3/colossalai_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colossalai-nightly
-Version: 2023.6.17
+Version: 2023.6.3
 Summary: An integrated large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org
 License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.6.17 Summary: An
+Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.6.3 Summary: An
 integrated large-scale model training system with efficient parallelization
 techniques Home-page: https://www.colossalai.org License: Apache Software
 License 2.0 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/
 discussions Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/
 issues Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io Project-URL:
 Github, https://github.com/hpcaitech/ColossalAI Description: # Colossal-AI
```

### Comparing `colossalai-nightly-2023.6.17/colossalai_nightly.egg-info/SOURCES.txt` & `colossalai-nightly-2023.6.3/colossalai_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,18 +38,14 @@
 colossalai/amp/naive_amp/_fp16_optimizer.py
 colossalai/amp/naive_amp/_utils.py
 colossalai/amp/naive_amp/naive_amp.py
 colossalai/amp/naive_amp/grad_scaler/__init__.py
 colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
 colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
 colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
-colossalai/amp/naive_amp/mixed_precision_mixin/__init__.py
-colossalai/amp/naive_amp/mixed_precision_mixin/base.py
-colossalai/amp/naive_amp/mixed_precision_mixin/bf16.py
-colossalai/amp/naive_amp/mixed_precision_mixin/fp16.py
 colossalai/amp/torch_amp/__init__.py
 colossalai/amp/torch_amp/_grad_scaler.py
 colossalai/amp/torch_amp/torch_amp.py
 colossalai/auto_parallel/__init__.py
 colossalai/auto_parallel/checkpoint/__init__.py
 colossalai/auto_parallel/checkpoint/build_c_ext.py
 colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
@@ -382,16 +378,14 @@
 colossalai/kernel/op_builder/fused_optim.py
 colossalai/kernel/op_builder/layernorm.py
 colossalai/kernel/op_builder/moe.py
 colossalai/kernel/op_builder/multi_head_attn.py
 colossalai/kernel/op_builder/scaled_masked_softmax.py
 colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py
 colossalai/kernel/op_builder/utils.py
-colossalai/lazy/__init__.py
-colossalai/lazy/lazy_init.py
 colossalai/logging/__init__.py
 colossalai/logging/logger.py
 colossalai/nn/__init__.py
 colossalai/nn/init.py
 colossalai/nn/_ops/__init__.py
 colossalai/nn/_ops/_utils.py
 colossalai/nn/_ops/addmm.py
@@ -563,14 +557,16 @@
 colossalai/utils/checkpoint_io/reader.py
 colossalai/utils/checkpoint_io/utils.py
 colossalai/utils/checkpoint_io/writer.py
 colossalai/utils/data_sampler/__init__.py
 colossalai/utils/data_sampler/base_sampler.py
 colossalai/utils/data_sampler/data_parallel_sampler.py
 colossalai/utils/model/__init__.py
+colossalai/utils/model/experimental.py
+colossalai/utils/model/lazy_init_context.py
 colossalai/utils/model/utils.py
 colossalai/utils/multi_tensor_apply/__init__.py
 colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
 colossalai/utils/profiler/__init__.py
 colossalai/utils/profiler/extention.py
 colossalai/utils/profiler/profiler.py
 colossalai/utils/profiler/stateful_tensor_mem_extention.py
```

### Comparing `colossalai-nightly-2023.6.17/op_builder/__init__.py` & `colossalai-nightly-2023.6.3/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/op_builder/builder.py` & `colossalai-nightly-2023.6.3/op_builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/op_builder/cpu_adam.py` & `colossalai-nightly-2023.6.3/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/op_builder/fused_optim.py` & `colossalai-nightly-2023.6.3/op_builder/fused_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/op_builder/layernorm.py` & `colossalai-nightly-2023.6.3/op_builder/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/op_builder/moe.py` & `colossalai-nightly-2023.6.3/op_builder/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/op_builder/multi_head_attn.py` & `colossalai-nightly-2023.6.3/op_builder/multi_head_attn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/op_builder/scaled_masked_softmax.py` & `colossalai-nightly-2023.6.3/op_builder/scaled_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/op_builder/scaled_upper_triangle_masked_softmax.py` & `colossalai-nightly-2023.6.3/op_builder/scaled_upper_triangle_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/op_builder/utils.py` & `colossalai-nightly-2023.6.3/op_builder/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/requirements/requirements-test.txt` & `colossalai-nightly-2023.6.3/requirements/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/setup.py` & `colossalai-nightly-2023.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/components_to_test/albert.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/albert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/components_to_test/beit.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/beit.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/components_to_test/bert.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/components_to_test/gpt2.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/gpt2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/components_to_test/hanging_param_model.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/hanging_param_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/components_to_test/inline_op_model.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/inline_op_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/components_to_test/nested_model.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/nested_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/components_to_test/registry.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/components_to_test/repeated_computed_layers.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/repeated_computed_layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/components_to_test/resnet.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/resnet.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/components_to_test/simple_net.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/simple_net.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/components_to_test/utils/executor.py` & `colossalai-nightly-2023.6.3/tests/components_to_test/utils/executor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/kit/model_zoo/diffusers/diffusers.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/diffusers/diffusers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/kit/model_zoo/registry.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 from dataclasses import dataclass
 from typing import Callable
 
-__all__ = ['ModelZooRegistry', 'ModelAttribute', 'model_zoo']
+__all__ = ['ModelZooRegistry', 'ModelAttributem', 'model_zoo']
 
 
 @dataclass
 class ModelAttribute:
     """
     Attributes of a model.
 
@@ -33,15 +33,15 @@
         Register a model and data generation function.
 
         Examples:
         >>> # Register
         >>> model_zoo = ModelZooRegistry()
         >>> model_zoo.register('resnet18', resnet18, resnet18_data_gen)
         >>> # Run the model
-        >>> data = resnet18_data_gen() # do not input any argument
+        >>> data = resnresnet18_data_gen() # do not input any argument
         >>> model = resnet18() # do not input any argument
         >>> out = model(**data)
 
         Args:
             name (str): Name of the model.
             model_fn (callable): A function that returns a model. **It must not contain any arguments.**
             output_transform_fn (callable): A function that transforms the output of the model into Dict.
```

### Comparing `colossalai-nightly-2023.6.17/tests/kit/model_zoo/timm/timm.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/timm/timm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/kit/model_zoo/torchaudio/torchaudio.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchaudio/torchaudio.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/kit/model_zoo/torchrec/torchrec.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchrec/torchrec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/kit/model_zoo/torchvision/torchvision.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/torchvision/torchvision.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/kit/model_zoo/transformers/albert.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/albert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/kit/model_zoo/transformers/bert.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/kit/model_zoo/transformers/gpt.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/gpt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/kit/model_zoo/transformers/opt.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/opt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/kit/model_zoo/transformers/t5.py` & `colossalai-nightly-2023.6.3/tests/kit/model_zoo/transformers/t5.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_analyzer/test_fx/test_bias_addition.py` & `colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/test_bias_addition.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_analyzer/test_fx/test_mod_dir.py` & `colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/test_mod_dir.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_analyzer/test_fx/test_nested_ckpt.py` & `colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/test_nested_ckpt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_analyzer/test_fx/test_shape_prop.py` & `colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/test_shape_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_analyzer/test_fx/test_symbolic_profile.py` & `colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/test_symbolic_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_analyzer/test_fx/zoo.py` & `colossalai-nightly-2023.6.3/tests/test_analyzer/test_fx/zoo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_analyzer/test_subclasses/test_aten.py` & `colossalai-nightly-2023.6.3/tests/test_analyzer/test_subclasses/test_aten.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_analyzer/test_subclasses/test_flop_tensor.py` & `colossalai-nightly-2023.6.3/tests/test_analyzer/test_subclasses/test_flop_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_analyzer/test_subclasses/test_meta_mode.py` & `colossalai-nightly-2023.6.3/tests/test_analyzer/test_subclasses/test_meta_mode.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_pass/test_node_converting_pass.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_pass/test_node_converting_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     mesh_shape = (2, 2)
     device_mesh = DeviceMesh(physical_mesh_id, mesh_shape, init_process_group=True)
     input = torch.rand(4, 16, 64, 64).cuda()
     # the index of bn node in computation graph
     node_index = 1
     # the total number of bn strategies without sync bn mode
-    # TODO: add sync bn strategies after related passes ready
+    # TODO: add sync bn stategies after related passes ready
     strategy_number = 4
     numerical_test_for_node_strategy(model=model,
                                      device_mesh=device_mesh,
                                      node_index=node_index,
                                      strategy_number=strategy_number,
                                      input_args=[input],
                                      meta_arg_names=['input'])
```

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,31 +39,31 @@
 
     mesh_shape = (2, 2)
     device_mesh = DeviceMesh(physical_mesh_id, mesh_shape)
     output_node = list(graph.nodes)[2]
     output_strategies_vector = StrategiesVector(output_node)
 
     # build handler
-    output_handler = OutputHandler(node=output_node,
+    otuput_handler = OutputHandler(node=output_node,
                                    device_mesh=device_mesh,
                                    strategies_vector=output_strategies_vector,
                                    output_option=output_option)
 
-    output_handler.register_strategy(compute_resharding_cost=False)
+    otuput_handler.register_strategy(compute_resharding_cost=False)
     # check operation data mapping
-    mapping = output_handler.get_operation_data_mapping()
+    mapping = otuput_handler.get_operation_data_mapping()
 
     for name, op_data in mapping.items():
         op_data: OperationData
         # make sure they have valid values
         assert op_data.data is not None
 
     assert mapping['output'].name == "output"
     assert mapping['output'].type == OperationDataType.OUTPUT
-    strategy_name_list = [val.name for val in output_handler.strategies_vector]
+    strategy_name_list = [val.name for val in otuput_handler.strategies_vector]
     if output_option == 'distributed':
         assert "Distributed Output" in strategy_name_list
     else:
         assert "Replica Output" in strategy_name_list
 
 
 if __name__ == '__main__':
```

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.6.17/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py` & `colossalai-nightly-2023.6.3/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py`

 * *Files identical despite different names*

