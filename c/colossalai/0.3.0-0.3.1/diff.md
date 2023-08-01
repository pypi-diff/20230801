# Comparing `tmp/colossalai-0.3.0.tar.gz` & `tmp/colossalai-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colossalai-0.3.0.tar", last modified: Thu May 25 08:21:07 2023, max compression
+gzip compressed data, was "colossalai-0.3.1.tar", last modified: Tue Aug  1 07:02:16 2023, max compression
```

## Comparing `colossalai-0.3.0.tar` & `colossalai-0.3.1.tar`

### file list

```diff
@@ -1,902 +1,956 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.884923 colossalai-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    22244 2023-05-25 08:20:55.000000 colossalai-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-25 08:20:55.000000 colossalai-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25388 2023-05-25 08:21:07.884923 colossalai-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20789 2023-05-25 08:20:55.000000 colossalai-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.756918 colossalai-0.3.0/colossalai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.760918 colossalai-0.3.0/colossalai/_C/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_C/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.760918 colossalai-0.3.0/colossalai/_analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_analyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.760918 colossalai-0.3.0/colossalai/_analyzer/_subclasses/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_analyzer/_subclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_analyzer/_subclasses/_meta_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_analyzer/_subclasses/_monkey_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    18694 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_analyzer/_subclasses/flop_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_analyzer/_subclasses/meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_analyzer/envs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.760918 colossalai-0.3.0/colossalai/_analyzer/fx/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_analyzer/fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_analyzer/fx/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_analyzer/fx/graph_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_analyzer/fx/node_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.760918 colossalai-0.3.0/colossalai/_analyzer/fx/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_analyzer/fx/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_analyzer/fx/passes/graph_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_analyzer/fx/passes/shape_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_analyzer/fx/symbolic_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.760918 colossalai-0.3.0/colossalai/_analyzer/fx/tracer/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_analyzer/fx/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_analyzer/fx/tracer/bias_addition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_analyzer/fx/tracer/custom_leaf_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_analyzer/fx/tracer/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_analyzer/fx/tracer/symbolic_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/_analyzer/fx/tracer/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.764918 colossalai-0.3.0/colossalai/amp/
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/amp/amp_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.764918 colossalai-0.3.0/colossalai/amp/apex_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/amp/apex_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/amp/apex_amp/apex_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.764918 colossalai-0.3.0/colossalai/amp/naive_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/amp/naive_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/amp/naive_amp/_fp16_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/amp/naive_amp/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.764918 colossalai-0.3.0/colossalai/amp/naive_amp/grad_scaler/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/amp/naive_amp/grad_scaler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/amp/naive_amp/naive_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.764918 colossalai-0.3.0/colossalai/amp/torch_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/amp/torch_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/amp/torch_amp/_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/amp/torch_amp/torch_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.764918 colossalai-0.3.0/colossalai/auto_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.764918 colossalai-0.3.0/colossalai/auto_parallel/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/checkpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/checkpoint/build_c_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py
--rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/checkpoint/operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.764918 colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.768919 colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/where.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/shard_metainfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.768919 colossalai-0.3.0/colossalai/auto_parallel/offload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/offload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/offload/amp_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/offload/base_offload_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/offload/mem_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/offload/region.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/offload/region_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/offload/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/offload/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/offload/training_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/offload/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.772919 colossalai-0.3.0/colossalai/auto_parallel/passes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/passes/comm_metainfo_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/passes/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/passes/meta_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/passes/runtime_apply_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    22686 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/passes/runtime_preparation_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.772919 colossalai-0.3.0/colossalai/auto_parallel/pipeline_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/pipeline_shard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.772919 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.776919 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.780919 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    43503 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/sharding_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.780919 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/solver/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.788919 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/utils/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/utils/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/utils/reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/utils/sharding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.788919 colossalai-0.3.0/colossalai/booster/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/booster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/booster/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11106 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/booster/booster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.788919 colossalai-0.3.0/colossalai/booster/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/booster/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/booster/mixed_precision/bf16.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/booster/mixed_precision/fp16_apex.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/booster/mixed_precision/fp16_naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/booster/mixed_precision/fp16_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/booster/mixed_precision/fp8.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/booster/mixed_precision/mixed_precision_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.788919 colossalai-0.3.0/colossalai/booster/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/booster/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/booster/plugin/dp_plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13628 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/booster/plugin/gemini_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/booster/plugin/low_level_zero_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/booster/plugin/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/booster/plugin/torch_ddp_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/booster/plugin/torch_fsdp_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.788919 colossalai-0.3.0/colossalai/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/builder/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.788919 colossalai-0.3.0/colossalai/checkpoint_io/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/checkpoint_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/checkpoint_io/checkpoint_io_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/checkpoint_io/general_checkpoint_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/checkpoint_io/index_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/checkpoint_io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.788919 colossalai-0.3.0/colossalai/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.788919 colossalai-0.3.0/colossalai/cli/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/cli/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/cli/benchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/cli/benchmark/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/cli/benchmark/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.792919 colossalai-0.3.0/colossalai/cli/check/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/cli/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/cli/check/check_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.792919 colossalai-0.3.0/colossalai/cli/launcher/
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/cli/launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/cli/launcher/hostinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/cli/launcher/multinode_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/cli/launcher/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.792919 colossalai-0.3.0/colossalai/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/cluster/device_mesh_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/cluster/dist_coordinator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/cluster/process_group_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.792919 colossalai-0.3.0/colossalai/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/communication/collective.py
--rw-r--r--   0 runner    (1001) docker     (123)    19462 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/communication/p2p.py
--rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/communication/p2p_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/communication/ring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/communication/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.792919 colossalai-0.3.0/colossalai/context/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/context/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/context/moe_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    23924 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/context/parallel_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/context/parallel_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.796920 colossalai-0.3.0/colossalai/context/process_group_initializer/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/context/process_group_initializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/context/process_group_initializer/initializer_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/context/process_group_initializer/initializer_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/context/process_group_initializer/initializer_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/context/process_group_initializer/initializer_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/context/process_group_initializer/initializer_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/context/process_group_initializer/initializer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/context/process_group_initializer/initializer_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/context/process_group_initializer/initializer_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/context/process_group_initializer/initializer_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/context/process_group_initializer/process_group_initializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.796920 colossalai-0.3.0/colossalai/context/random/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/context/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/context/random/_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/context/random/seed_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/context/singleton_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.796920 colossalai-0.3.0/colossalai/device/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17419 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/device/alpha_beta_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/device/calc_pipeline_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/device/device_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.796920 colossalai-0.3.0/colossalai/engine/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/engine/_base_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.796920 colossalai-0.3.0/colossalai/engine/gradient_accumulation/
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/engine/gradient_accumulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/engine/gradient_accumulation/_gradient_accumulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.796920 colossalai-0.3.0/colossalai/engine/gradient_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/engine/gradient_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/engine/gradient_handler/_base_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/engine/gradient_handler/_moe_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/engine/gradient_handler/_zero_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/engine/gradient_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.800920 colossalai-0.3.0/colossalai/engine/schedule/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/engine/schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/engine/schedule/_base_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/engine/schedule/_non_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    41258 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/engine/schedule/_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/engine/schedule/_pipeline_schedule_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.800920 colossalai-0.3.0/colossalai/fx/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    19408 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/_meta_regist_12.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/_meta_regist_13.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.800920 colossalai-0.3.0/colossalai/fx/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44753 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/codegen/activation_checkpoint_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/graph_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.800920 colossalai-0.3.0/colossalai/fx/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/passes/adding_split_node_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/passes/concrete_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/passes/meta_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/passes/passes_for_gpt2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/passes/shard_1d_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/passes/split_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/passes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.804920 colossalai-0.3.0/colossalai/fx/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/dataflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.804920 colossalai-0.3.0/colossalai/fx/profiler/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.804920 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_function/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_function/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_function/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_function/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_function/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_function/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_function/python_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.808920 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_module/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_module/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_module/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_module/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_module/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_module/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_module/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_module/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_module/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_module/torch_op.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/experimental/shard_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/memory_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/opcount.py
--rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/shard_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/profiler/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.808920 colossalai-0.3.0/colossalai/fx/tracer/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/_meta_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/_symbolic_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/_tracer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.808920 colossalai-0.3.0/colossalai/fx/tracer/bias_addition_patch/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/bias_addition_patch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.808920 colossalai-0.3.0/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.808920 colossalai-0.3.0/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.808920 colossalai-0.3.0/colossalai/fx/tracer/meta_patch/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/meta_patch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.812920 colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_function/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_function/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_function/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_function/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_function/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.812920 colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_module/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_module/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_module/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_module/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_module/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_module/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_module/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    24623 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/fx/tracer/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/global_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.812920 colossalai-0.3.0/colossalai/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/interface/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/interface/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.812920 colossalai-0.3.0/colossalai/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.816920 colossalai-0.3.0/colossalai/kernel/cuda_native/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.820921 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/compat.h
--rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/cpu_adam.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.820921 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu
--rw-r--r--   0 runner    (1001) docker     (123)    37586 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.820921 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/context.h
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h
--rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/ls_cub.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h
--rw-r--r--   0 runner    (1001) docker     (123)    48403 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22850 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/type_shim.h
--rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/cuda_native/scaled_softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.824921 colossalai-0.3.0/colossalai/kernel/jit/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/jit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/jit/bias_dropout_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/jit/bias_gelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/jit/option.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.824921 colossalai-0.3.0/colossalai/kernel/op_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/op_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/op_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/op_builder/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/op_builder/fused_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/op_builder/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/op_builder/moe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/op_builder/multi_head_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/op_builder/scaled_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/kernel/op_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.824921 colossalai-0.3.0/colossalai/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.824921 colossalai-0.3.0/colossalai/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.824921 colossalai-0.3.0/colossalai/nn/_ops/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/_ops/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/_ops/addmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/_ops/batch_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/_ops/element_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/_ops/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/_ops/embedding_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/_ops/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/_ops/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/_ops/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/_ops/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.828921 colossalai-0.3.0/colossalai/nn/layer/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/base_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.828921 colossalai-0.3.0/colossalai/nn/layer/colossalai_layer/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/colossalai_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/colossalai_layer/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/colossalai_layer/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/colossalai_layer/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/colossalai_layer/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/colossalai_layer/normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.828921 colossalai-0.3.0/colossalai/nn/layer/moe/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/moe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/moe/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/moe/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/moe/experts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/moe/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/moe/routers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/moe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.828921 colossalai-0.3.0/colossalai/nn/layer/parallel_1d/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/parallel_1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/parallel_1d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/parallel_1d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    49753 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/parallel_1d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.828921 colossalai-0.3.0/colossalai/nn/layer/parallel_2d/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/parallel_2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/parallel_2d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/parallel_2d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    50524 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/parallel_2d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.832921 colossalai-0.3.0/colossalai/nn/layer/parallel_2p5d/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/parallel_2p5d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37643 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/parallel_2p5d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/parallel_2p5d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    50769 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/parallel_2p5d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.832921 colossalai-0.3.0/colossalai/nn/layer/parallel_3d/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/parallel_3d/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22769 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/parallel_3d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/parallel_3d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    51441 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/parallel_3d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.832921 colossalai-0.3.0/colossalai/nn/layer/parallel_sequence/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/parallel_sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/parallel_sequence/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/parallel_sequence/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/parallel_sequence/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.832921 colossalai-0.3.0/colossalai/nn/layer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/utils/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.832921 colossalai-0.3.0/colossalai/nn/layer/vanilla/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/vanilla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/vanilla/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.832921 colossalai-0.3.0/colossalai/nn/layer/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/layer/wrapper/pipeline_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.832921 colossalai-0.3.0/colossalai/nn/loss/
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/loss/loss_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/loss/loss_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/loss/loss_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/loss/loss_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/loss/loss_moe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.836921 colossalai-0.3.0/colossalai/nn/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/lr_scheduler/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/lr_scheduler/delayed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/lr_scheduler/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/lr_scheduler/multistep.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/lr_scheduler/onecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/lr_scheduler/poly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/lr_scheduler/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.836921 colossalai-0.3.0/colossalai/nn/metric/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/metric/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/metric/accuracy_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/metric/accuracy_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/metric/accuracy_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.836921 colossalai-0.3.0/colossalai/nn/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/optimizer/colossalai_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/optimizer/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/optimizer/fused_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/optimizer/fused_lamb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/optimizer/fused_sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/optimizer/hybrid_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/optimizer/lamb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/optimizer/lars.py
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/optimizer/nvme_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.836921 colossalai-0.3.0/colossalai/nn/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/parallel/data_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.840921 colossalai-0.3.0/colossalai/nn/parallel/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/parallel/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.840921 colossalai-0.3.0/colossalai/nn/parallel/layers/cache_embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/parallel/layers/cache_embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    28600 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/parallel/layers/cache_embedding/copyer.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/parallel/layers/colo_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/parallel/layers/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/parallel/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/parallel/layers/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/nn/parallel/reducer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.840921 colossalai-0.3.0/colossalai/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/pipeline/layer_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.840921 colossalai-0.3.0/colossalai/pipeline/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/pipeline/middleware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.840921 colossalai-0.3.0/colossalai/pipeline/middleware/adaptor/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/pipeline/middleware/adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/pipeline/middleware/adaptor/fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/pipeline/middleware/topo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/pipeline/pipelinable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/pipeline/pipeline_process_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.844921 colossalai-0.3.0/colossalai/pipeline/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/pipeline/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59163 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/pipeline/rpc/_pipeline_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/pipeline/rpc/_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/pipeline/rpc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/pipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.844921 colossalai-0.3.0/colossalai/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/registry/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.844921 colossalai-0.3.0/colossalai/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/colo_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/colo_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22269 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/comm_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/compute_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.848922 colossalai-0.3.0/colossalai/tensor/d_tensor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/d_tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/d_tensor/comm_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/d_tensor/d_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/d_tensor/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    25229 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/d_tensor/layout_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/d_tensor/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/d_tensor/sharding_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/d_tensor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/dist_spec_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/distspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/op_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/param_op_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/process_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    36495 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/shape_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/sharding_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/tensor_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.848922 colossalai-0.3.0/colossalai/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/testing/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/testing/pytest_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/testing/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.848922 colossalai-0.3.0/colossalai/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/trainer/_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.848922 colossalai-0.3.0/colossalai/trainer/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/trainer/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/trainer/hooks/_base_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/trainer/hooks/_checkpoint_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/trainer/hooks/_commons_.py
--rw-r--r--   0 runner    (1001) docker     (123)    13106 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/trainer/hooks/_log_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/trainer/hooks/_lr_scheduler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/trainer/hooks/_metric_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.848922 colossalai-0.3.0/colossalai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/activation_checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.848922 colossalai-0.3.0/colossalai/utils/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/checkpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/checkpoint/module_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/checkpoint/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.852922 colossalai-0.3.0/colossalai/utils/checkpoint_io/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/checkpoint_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/checkpoint_io/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/checkpoint_io/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/checkpoint_io/convertor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/checkpoint_io/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/checkpoint_io/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/checkpoint_io/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/checkpoint_io/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/checkpoint_io/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/checkpoint_io/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/checkpointing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.852922 colossalai-0.3.0/colossalai/utils/data_sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/data_sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/data_sampler/base_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/data_sampler/data_parallel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.852922 colossalai-0.3.0/colossalai/utils/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/model/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/model/lazy_init_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/moe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.852922 colossalai-0.3.0/colossalai/utils/multi_tensor_apply/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/multi_tensor_apply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.852922 colossalai-0.3.0/colossalai/utils/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/profiler/extention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.856922 colossalai-0.3.0/colossalai/utils/profiler/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/profiler/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/profiler/legacy/comm_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/profiler/legacy/pcie_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/profiler/legacy/prof_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/profiler/stateful_tensor_mem_extention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.856922 colossalai-0.3.0/colossalai/utils/rank_recorder/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/rank_recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/rank_recorder/rank_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.856922 colossalai-0.3.0/colossalai/utils/tensor_detector/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/tensor_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/tensor_detector/tensor_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 08:21:07.000000 colossalai-0.3.0/colossalai/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.856922 colossalai-0.3.0/colossalai/zero/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.856922 colossalai-0.3.0/colossalai/zero/gemini/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.856922 colossalai-0.3.0/colossalai/zero/gemini/chunk/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/chunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22078 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/chunk/chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/chunk/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/chunk/search_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/chunk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/colo_init_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/gemini_ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/gemini_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/gemini_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/gemini_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.860922 colossalai-0.3.0/colossalai/zero/gemini/memory_tracer/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/memory_tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/memory_tracer/memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/memory_tracer/memory_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/memory_tracer/memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/memory_tracer/param_runtime_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/memory_tracer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/placement_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/gemini/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.860922 colossalai-0.3.0/colossalai/zero/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.860922 colossalai-0.3.0/colossalai/zero/legacy/gemini/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/gemini/gemini_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.860922 colossalai-0.3.0/colossalai/zero/legacy/gemini/ophooks/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/gemini/ophooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/gemini/ophooks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.860922 colossalai-0.3.0/colossalai/zero/legacy/gemini/paramhooks/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/gemini/paramhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/gemini/stateful_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/gemini/tensor_placement_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/gemini/tensor_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.860922 colossalai-0.3.0/colossalai/zero/legacy/init_ctx/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/init_ctx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/init_ctx/init_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.860922 colossalai-0.3.0/colossalai/zero/legacy/shard_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/shard_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/shard_utils/base_shard_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/shard_utils/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.864922 colossalai-0.3.0/colossalai/zero/legacy/sharded_model/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/sharded_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/sharded_model/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/sharded_model/reduce_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29015 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/sharded_model/sharded_model_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/sharded_model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/sharded_model/zero_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.864922 colossalai-0.3.0/colossalai/zero/legacy/sharded_optim/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/sharded_optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.864922 colossalai-0.3.0/colossalai/zero/legacy/sharded_param/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/sharded_param/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/sharded_param/sharded_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/legacy/sharded_param/sharded_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.864922 colossalai-0.3.0/colossalai/zero/low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/low_level/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.864922 colossalai-0.3.0/colossalai/zero/low_level/bookkeeping/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/low_level/bookkeeping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/low_level/bookkeeping/base_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/low_level/bookkeeping/bucket_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/low_level/bookkeeping/gradient_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/low_level/bookkeeping/parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/low_level/bookkeeping/tensor_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    25694 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/low_level/low_level_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-25 08:20:55.000000 colossalai-0.3.0/colossalai/zero/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.760918 colossalai-0.3.0/colossalai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25388 2023-05-25 08:21:07.000000 colossalai-0.3.0/colossalai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37361 2023-05-25 08:21:07.000000 colossalai-0.3.0/colossalai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 08:21:07.000000 colossalai-0.3.0/colossalai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-25 08:21:07.000000 colossalai-0.3.0/colossalai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 08:21:07.000000 colossalai-0.3.0/colossalai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 08:21:07.000000 colossalai-0.3.0/colossalai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.868922 colossalai-0.3.0/op_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-25 08:20:55.000000 colossalai-0.3.0/op_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-05-25 08:20:55.000000 colossalai-0.3.0/op_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-25 08:20:55.000000 colossalai-0.3.0/op_builder/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-25 08:20:55.000000 colossalai-0.3.0/op_builder/fused_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-25 08:20:55.000000 colossalai-0.3.0/op_builder/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-25 08:20:55.000000 colossalai-0.3.0/op_builder/moe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-25 08:20:55.000000 colossalai-0.3.0/op_builder/multi_head_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-25 08:20:55.000000 colossalai-0.3.0/op_builder/scaled_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-25 08:20:55.000000 colossalai-0.3.0/op_builder/scaled_upper_triangle_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-25 08:20:55.000000 colossalai-0.3.0/op_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.868922 colossalai-0.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-25 08:20:55.000000 colossalai-0.3.0/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 08:20:55.000000 colossalai-0.3.0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 08:21:07.884923 colossalai-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-05-25 08:20:55.000000 colossalai-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.756918 colossalai-0.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.872923 colossalai-0.3.0/tests/components_to_test/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/components_to_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/components_to_test/albert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/components_to_test/beit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/components_to_test/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/components_to_test/gpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/components_to_test/hanging_param_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/components_to_test/inline_op_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/components_to_test/nested_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/components_to_test/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/components_to_test/repeated_computed_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/components_to_test/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/components_to_test/simple_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.872923 colossalai-0.3.0/tests/components_to_test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/components_to_test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/components_to_test/utils/dummy_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/components_to_test/utils/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.872923 colossalai-0.3.0/tests/kit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/kit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.872923 colossalai-0.3.0/tests/kit/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/kit/model_zoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.872923 colossalai-0.3.0/tests/kit/model_zoo/diffusers/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/kit/model_zoo/diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/kit/model_zoo/diffusers/diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/kit/model_zoo/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.872923 colossalai-0.3.0/tests/kit/model_zoo/timm/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/kit/model_zoo/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/kit/model_zoo/timm/timm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.872923 colossalai-0.3.0/tests/kit/model_zoo/torchaudio/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/kit/model_zoo/torchaudio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/kit/model_zoo/torchaudio/torchaudio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.872923 colossalai-0.3.0/tests/kit/model_zoo/torchrec/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/kit/model_zoo/torchrec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/kit/model_zoo/torchrec/torchrec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.872923 colossalai-0.3.0/tests/kit/model_zoo/torchvision/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/kit/model_zoo/torchvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/kit/model_zoo/torchvision/torchvision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.872923 colossalai-0.3.0/tests/kit/model_zoo/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/kit/model_zoo/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/kit/model_zoo/transformers/albert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/kit/model_zoo/transformers/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/kit/model_zoo/transformers/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/kit/model_zoo/transformers/opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/kit/model_zoo/transformers/t5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.872923 colossalai-0.3.0/tests/test_analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_analyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.876923 colossalai-0.3.0/tests/test_analyzer/test_fx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_analyzer/test_fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_analyzer/test_fx/test_bias_addition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_analyzer/test_fx/test_mod_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_analyzer/test_fx/test_nested_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_analyzer/test_fx/test_shape_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_analyzer/test_fx/test_symbolic_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_analyzer/test_fx/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.876923 colossalai-0.3.0/tests/test_analyzer/test_subclasses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_analyzer/test_subclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_analyzer/test_subclasses/test_aten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_analyzer/test_subclasses/test_flop_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_analyzer/test_subclasses/test_meta_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.876923 colossalai-0.3.0/tests/test_auto_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.876923 colossalai-0.3.0/tests/test_auto_parallel/test_pass/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_pass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_pass/test_node_converting_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.876923 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.880923 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:21:07.884923 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-25 08:20:55.000000 colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 08:20:55.000000 colossalai-0.3.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.160021 colossalai-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    22244 2023-08-01 07:02:06.000000 colossalai-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-01 07:02:06.000000 colossalai-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26072 2023-08-01 07:02:16.160021 colossalai-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21385 2023-08-01 07:02:06.000000 colossalai-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.048020 colossalai-0.3.1/colossalai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.048020 colossalai-0.3.1/colossalai/_C/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_C/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.056020 colossalai-0.3.1/colossalai/_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_analyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.056020 colossalai-0.3.1/colossalai/_analyzer/_subclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_analyzer/_subclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_analyzer/_subclasses/_meta_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_analyzer/_subclasses/_monkey_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18694 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_analyzer/_subclasses/flop_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_analyzer/_subclasses/meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_analyzer/envs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.056020 colossalai-0.3.1/colossalai/_analyzer/fx/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_analyzer/fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_analyzer/fx/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_analyzer/fx/graph_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_analyzer/fx/node_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.056020 colossalai-0.3.1/colossalai/_analyzer/fx/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_analyzer/fx/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_analyzer/fx/passes/graph_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_analyzer/fx/passes/shape_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_analyzer/fx/symbolic_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.056020 colossalai-0.3.1/colossalai/_analyzer/fx/tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_analyzer/fx/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_analyzer/fx/tracer/bias_addition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_analyzer/fx/tracer/custom_leaf_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_analyzer/fx/tracer/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_analyzer/fx/tracer/symbolic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/_analyzer/fx/tracer/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.056020 colossalai-0.3.1/colossalai/amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/amp/amp_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.056020 colossalai-0.3.1/colossalai/amp/apex_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/amp/apex_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/amp/apex_amp/apex_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.056020 colossalai-0.3.1/colossalai/amp/naive_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/amp/naive_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/amp/naive_amp/_fp16_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/amp/naive_amp/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.056020 colossalai-0.3.1/colossalai/amp/naive_amp/grad_scaler/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/amp/naive_amp/grad_scaler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.060020 colossalai-0.3.1/colossalai/amp/naive_amp/mixed_precision_mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/amp/naive_amp/mixed_precision_mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/amp/naive_amp/mixed_precision_mixin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/amp/naive_amp/mixed_precision_mixin/bf16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/amp/naive_amp/mixed_precision_mixin/fp16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/amp/naive_amp/naive_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.060020 colossalai-0.3.1/colossalai/amp/torch_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/amp/torch_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/amp/torch_amp/_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/amp/torch_amp/torch_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.060020 colossalai-0.3.1/colossalai/auto_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.060020 colossalai-0.3.1/colossalai/auto_parallel/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/checkpoint/build_c_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/checkpoint/operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.060020 colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.060020 colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/shard_metainfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.060020 colossalai-0.3.1/colossalai/auto_parallel/offload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/offload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/offload/amp_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/offload/base_offload_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/offload/mem_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/offload/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/offload/region_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/offload/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/offload/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/offload/training_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/offload/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.064020 colossalai-0.3.1/colossalai/auto_parallel/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/passes/comm_metainfo_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/passes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/passes/meta_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/passes/runtime_apply_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/passes/runtime_preparation_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.064020 colossalai-0.3.1/colossalai/auto_parallel/pipeline_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/pipeline_shard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.064020 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.064020 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.068020 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43483 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/sharding_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.068020 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/solver/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.068020 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/utils/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/utils/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/utils/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/utils/sharding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.068020 colossalai-0.3.1/colossalai/booster/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/booster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/booster/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/booster/booster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.068020 colossalai-0.3.1/colossalai/booster/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/booster/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/booster/mixed_precision/bf16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/booster/mixed_precision/fp16_apex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/booster/mixed_precision/fp16_naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/booster/mixed_precision/fp16_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/booster/mixed_precision/fp8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/booster/mixed_precision/mixed_precision_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.072020 colossalai-0.3.1/colossalai/booster/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/booster/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/booster/plugin/dp_plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18997 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/booster/plugin/gemini_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13170 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/booster/plugin/low_level_zero_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/booster/plugin/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/booster/plugin/torch_ddp_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/booster/plugin/torch_fsdp_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.072020 colossalai-0.3.1/colossalai/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/builder/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.072020 colossalai-0.3.1/colossalai/checkpoint_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/checkpoint_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15021 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/checkpoint_io/checkpoint_io_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/checkpoint_io/general_checkpoint_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/checkpoint_io/index_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23714 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/checkpoint_io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.072020 colossalai-0.3.1/colossalai/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.072020 colossalai-0.3.1/colossalai/cli/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/cli/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/cli/benchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/cli/benchmark/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/cli/benchmark/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.072020 colossalai-0.3.1/colossalai/cli/check/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/cli/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/cli/check/check_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.072020 colossalai-0.3.1/colossalai/cli/launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/cli/launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/cli/launcher/hostinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/cli/launcher/multinode_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/cli/launcher/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.076020 colossalai-0.3.1/colossalai/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/cluster/device_mesh_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/cluster/dist_coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/cluster/process_group_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.076020 colossalai-0.3.1/colossalai/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/communication/collective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19462 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/communication/p2p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/communication/p2p_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/communication/ring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/communication/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.076020 colossalai-0.3.1/colossalai/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/context/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/context/moe_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23924 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/context/parallel_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/context/parallel_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.076020 colossalai-0.3.1/colossalai/context/process_group_initializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/context/process_group_initializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/context/process_group_initializer/initializer_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/context/process_group_initializer/initializer_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/context/process_group_initializer/initializer_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/context/process_group_initializer/initializer_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/context/process_group_initializer/initializer_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/context/process_group_initializer/initializer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/context/process_group_initializer/initializer_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/context/process_group_initializer/initializer_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/context/process_group_initializer/initializer_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/context/process_group_initializer/process_group_initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.076020 colossalai-0.3.1/colossalai/context/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/context/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/context/random/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/context/random/seed_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/context/singleton_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.076020 colossalai-0.3.1/colossalai/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/device/alpha_beta_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/device/calc_pipeline_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23687 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/device/device_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.076020 colossalai-0.3.1/colossalai/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/engine/_base_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.076020 colossalai-0.3.1/colossalai/engine/gradient_accumulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/engine/gradient_accumulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/engine/gradient_accumulation/_gradient_accumulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.080020 colossalai-0.3.1/colossalai/engine/gradient_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/engine/gradient_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/engine/gradient_handler/_base_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/engine/gradient_handler/_moe_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/engine/gradient_handler/_zero_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/engine/gradient_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.080020 colossalai-0.3.1/colossalai/engine/schedule/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/engine/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/engine/schedule/_base_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/engine/schedule/_non_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41258 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/engine/schedule/_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/engine/schedule/_pipeline_schedule_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.080020 colossalai-0.3.1/colossalai/fx/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19408 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/_meta_regist_12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/_meta_regist_13.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.080020 colossalai-0.3.1/colossalai/fx/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44753 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/codegen/activation_checkpoint_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/graph_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.084020 colossalai-0.3.1/colossalai/fx/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/passes/adding_split_node_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/passes/concrete_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/passes/meta_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/passes/passes_for_gpt2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/passes/shard_1d_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/passes/split_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/passes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.084020 colossalai-0.3.1/colossalai/fx/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/dataflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.084020 colossalai-0.3.1/colossalai/fx/profiler/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.084020 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_function/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_function/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_function/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_function/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_function/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_function/python_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.088020 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_module/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_module/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_module/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_module/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_module/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_module/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_module/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_module/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_module/torch_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/experimental/shard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/memory_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/opcount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/shard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/profiler/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.088020 colossalai-0.3.1/colossalai/fx/tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/_meta_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/_symbolic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/_tracer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.088020 colossalai-0.3.1/colossalai/fx/tracer/bias_addition_patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/bias_addition_patch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.088020 colossalai-0.3.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.088020 colossalai-0.3.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26969 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.088020 colossalai-0.3.1/colossalai/fx/tracer/meta_patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/meta_patch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.088020 colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_function/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_function/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_function/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_function/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.092020 colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_module/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_module/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_module/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_module/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_module/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_module/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24624 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/fx/tracer/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/global_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.092020 colossalai-0.3.1/colossalai/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/interface/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/interface/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.092020 colossalai-0.3.1/colossalai/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.092020 colossalai-0.3.1/colossalai/kernel/cuda_native/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.096020 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/cpu_adam.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.096020 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    37586 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.096020 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/context.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/ls_cub.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48403 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22850 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/type_shim.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24864 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/cuda_native/scaled_softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.096020 colossalai-0.3.1/colossalai/kernel/jit/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/jit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/jit/bias_dropout_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/jit/bias_gelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/jit/option.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.100020 colossalai-0.3.1/colossalai/kernel/op_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/op_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/op_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/op_builder/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/op_builder/fused_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/op_builder/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/op_builder/moe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/op_builder/multi_head_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/op_builder/scaled_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/kernel/op_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.100020 colossalai-0.3.1/colossalai/lazy/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24273 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/lazy/lazy_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.100020 colossalai-0.3.1/colossalai/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.100020 colossalai-0.3.1/colossalai/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.100020 colossalai-0.3.1/colossalai/nn/_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/_ops/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/_ops/addmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/_ops/batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/_ops/element_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/_ops/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/_ops/embedding_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/_ops/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/_ops/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/_ops/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/_ops/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.100020 colossalai-0.3.1/colossalai/nn/layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/base_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.100020 colossalai-0.3.1/colossalai/nn/layer/colossalai_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/colossalai_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/colossalai_layer/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/colossalai_layer/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/colossalai_layer/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/colossalai_layer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/colossalai_layer/normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.104020 colossalai-0.3.1/colossalai/nn/layer/moe/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/moe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/moe/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/moe/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/moe/experts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/moe/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/moe/routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/moe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.104020 colossalai-0.3.1/colossalai/nn/layer/parallel_1d/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/parallel_1d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/parallel_1d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/parallel_1d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49753 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/parallel_1d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.104020 colossalai-0.3.1/colossalai/nn/layer/parallel_2d/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/parallel_2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/parallel_2d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/parallel_2d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50524 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/parallel_2d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.108020 colossalai-0.3.1/colossalai/nn/layer/parallel_2p5d/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/parallel_2p5d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37643 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/parallel_2p5d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/parallel_2p5d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50769 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/parallel_2p5d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.108020 colossalai-0.3.1/colossalai/nn/layer/parallel_3d/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/parallel_3d/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22769 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/parallel_3d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/parallel_3d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51441 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/parallel_3d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.108020 colossalai-0.3.1/colossalai/nn/layer/parallel_sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/parallel_sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/parallel_sequence/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/parallel_sequence/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/parallel_sequence/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.108020 colossalai-0.3.1/colossalai/nn/layer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/utils/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.112020 colossalai-0.3.1/colossalai/nn/layer/vanilla/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/vanilla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/vanilla/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.112020 colossalai-0.3.1/colossalai/nn/layer/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/layer/wrapper/pipeline_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.112020 colossalai-0.3.1/colossalai/nn/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/loss/loss_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/loss/loss_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/loss/loss_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/loss/loss_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/loss/loss_moe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.116020 colossalai-0.3.1/colossalai/nn/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/lr_scheduler/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/lr_scheduler/delayed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/lr_scheduler/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/lr_scheduler/multistep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/lr_scheduler/onecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/lr_scheduler/poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/lr_scheduler/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.116020 colossalai-0.3.1/colossalai/nn/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/metric/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/metric/accuracy_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/metric/accuracy_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/metric/accuracy_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.120020 colossalai-0.3.1/colossalai/nn/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/optimizer/colossalai_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/optimizer/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/optimizer/fused_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/optimizer/fused_lamb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/optimizer/fused_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/optimizer/hybrid_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/optimizer/lamb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/optimizer/lars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/optimizer/nvme_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.120020 colossalai-0.3.1/colossalai/nn/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/parallel/data_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.120020 colossalai-0.3.1/colossalai/nn/parallel/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/parallel/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.120020 colossalai-0.3.1/colossalai/nn/parallel/layers/cache_embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/parallel/layers/cache_embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28600 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/parallel/layers/cache_embedding/copyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/parallel/layers/colo_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/parallel/layers/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/parallel/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/parallel/layers/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/nn/parallel/reducer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.120020 colossalai-0.3.1/colossalai/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/pipeline/layer_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.120020 colossalai-0.3.1/colossalai/pipeline/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/pipeline/middleware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.120020 colossalai-0.3.1/colossalai/pipeline/middleware/adaptor/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/pipeline/middleware/adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/pipeline/middleware/adaptor/fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/pipeline/middleware/topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/pipeline/pipelinable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/pipeline/pipeline_process_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.124020 colossalai-0.3.1/colossalai/pipeline/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/pipeline/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59170 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/pipeline/rpc/_pipeline_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/pipeline/rpc/_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/pipeline/rpc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/pipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.124020 colossalai-0.3.1/colossalai/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/registry/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.124020 colossalai-0.3.1/colossalai/shardformer/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.124020 colossalai-0.3.1/colossalai/shardformer/layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/layer/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/layer/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/layer/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/layer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/layer/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/layer/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/layer/parallel_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20697 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/layer/qkv_fused_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/layer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.124020 colossalai-0.3.1/colossalai/shardformer/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/modeling/bloom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.128020 colossalai-0.3.1/colossalai/shardformer/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/policies/autopolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/policies/basepolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/policies/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/policies/bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/policies/gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/policies/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/policies/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/policies/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/policies/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.128020 colossalai-0.3.1/colossalai/shardformer/shard/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/shard/shard_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/shard/sharder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/shardformer/shard/shardformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.128020 colossalai-0.3.1/colossalai/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/colo_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/colo_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21790 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/comm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/compute_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.128020 colossalai-0.3.1/colossalai/tensor/d_tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/d_tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/d_tensor/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/d_tensor/comm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/d_tensor/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24565 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/d_tensor/layout_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/d_tensor/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/d_tensor/sharding_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/d_tensor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/dist_spec_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/distspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/op_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/param_op_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/process_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36486 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/shape_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11605 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/sharding_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/tensor_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.132020 colossalai-0.3.1/colossalai/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/testing/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/testing/pytest_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/testing/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.136021 colossalai-0.3.1/colossalai/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/trainer/_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.136021 colossalai-0.3.1/colossalai/trainer/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/trainer/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/trainer/hooks/_base_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/trainer/hooks/_checkpoint_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/trainer/hooks/_commons_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13106 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/trainer/hooks/_log_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/trainer/hooks/_lr_scheduler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/trainer/hooks/_metric_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.136021 colossalai-0.3.1/colossalai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/activation_checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.136021 colossalai-0.3.1/colossalai/utils/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/checkpoint/module_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/checkpoint/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.140020 colossalai-0.3.1/colossalai/utils/checkpoint_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/checkpoint_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/checkpoint_io/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/checkpoint_io/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/checkpoint_io/convertor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/checkpoint_io/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/checkpoint_io/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/checkpoint_io/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/checkpoint_io/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/checkpoint_io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/checkpoint_io/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/checkpointing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.140020 colossalai-0.3.1/colossalai/utils/data_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/data_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/data_sampler/base_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/data_sampler/data_parallel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.140020 colossalai-0.3.1/colossalai/utils/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/moe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.140020 colossalai-0.3.1/colossalai/utils/multi_tensor_apply/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/multi_tensor_apply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.140020 colossalai-0.3.1/colossalai/utils/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/profiler/extention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.140020 colossalai-0.3.1/colossalai/utils/profiler/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/profiler/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/profiler/legacy/comm_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/profiler/legacy/pcie_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/profiler/legacy/prof_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/profiler/stateful_tensor_mem_extention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.140020 colossalai-0.3.1/colossalai/utils/rank_recorder/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/rank_recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/rank_recorder/rank_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.140020 colossalai-0.3.1/colossalai/utils/tensor_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/tensor_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/tensor_detector/tensor_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 07:02:15.000000 colossalai-0.3.1/colossalai/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.140020 colossalai-0.3.1/colossalai/zero/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.140020 colossalai-0.3.1/colossalai/zero/gemini/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.144020 colossalai-0.3.1/colossalai/zero/gemini/chunk/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/chunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/chunk/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/chunk/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/chunk/search_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/chunk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/colo_init_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37822 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/gemini_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/gemini_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/gemini_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33517 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/gemini_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.144020 colossalai-0.3.1/colossalai/zero/gemini/memory_tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/memory_tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/memory_tracer/memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/memory_tracer/memory_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/memory_tracer/memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/memory_tracer/param_runtime_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/memory_tracer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/placement_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/gemini/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.144020 colossalai-0.3.1/colossalai/zero/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.144020 colossalai-0.3.1/colossalai/zero/legacy/gemini/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/gemini/gemini_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.144020 colossalai-0.3.1/colossalai/zero/legacy/gemini/ophooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/gemini/ophooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/gemini/ophooks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.144020 colossalai-0.3.1/colossalai/zero/legacy/gemini/paramhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/gemini/paramhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/gemini/stateful_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/gemini/tensor_placement_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/gemini/tensor_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.144020 colossalai-0.3.1/colossalai/zero/legacy/init_ctx/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/init_ctx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/init_ctx/init_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.144020 colossalai-0.3.1/colossalai/zero/legacy/shard_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/shard_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/shard_utils/base_shard_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/shard_utils/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.144020 colossalai-0.3.1/colossalai/zero/legacy/sharded_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/sharded_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/sharded_model/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/sharded_model/reduce_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29261 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/sharded_model/sharded_model_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/sharded_model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/sharded_model/zero_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.144020 colossalai-0.3.1/colossalai/zero/legacy/sharded_optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/sharded_optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.148021 colossalai-0.3.1/colossalai/zero/legacy/sharded_param/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/sharded_param/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/sharded_param/sharded_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/legacy/sharded_param/sharded_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.148021 colossalai-0.3.1/colossalai/zero/low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/low_level/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.148021 colossalai-0.3.1/colossalai/zero/low_level/bookkeeping/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/low_level/bookkeeping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/low_level/bookkeeping/base_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/low_level/bookkeeping/bucket_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/low_level/bookkeeping/gradient_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/low_level/bookkeeping/parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/low_level/bookkeeping/tensor_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24933 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/low_level/low_level_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-08-01 07:02:06.000000 colossalai-0.3.1/colossalai/zero/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.048020 colossalai-0.3.1/colossalai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26072 2023-08-01 07:02:15.000000 colossalai-0.3.1/colossalai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39338 2023-08-01 07:02:16.000000 colossalai-0.3.1/colossalai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 07:02:15.000000 colossalai-0.3.1/colossalai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-01 07:02:15.000000 colossalai-0.3.1/colossalai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 07:02:15.000000 colossalai-0.3.1/colossalai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 07:02:15.000000 colossalai-0.3.1/colossalai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.148021 colossalai-0.3.1/op_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-01 07:02:06.000000 colossalai-0.3.1/op_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-08-01 07:02:06.000000 colossalai-0.3.1/op_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-01 07:02:06.000000 colossalai-0.3.1/op_builder/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-01 07:02:06.000000 colossalai-0.3.1/op_builder/fused_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-01 07:02:06.000000 colossalai-0.3.1/op_builder/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-01 07:02:06.000000 colossalai-0.3.1/op_builder/moe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-08-01 07:02:06.000000 colossalai-0.3.1/op_builder/multi_head_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-01 07:02:06.000000 colossalai-0.3.1/op_builder/scaled_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-08-01 07:02:06.000000 colossalai-0.3.1/op_builder/scaled_upper_triangle_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-08-01 07:02:06.000000 colossalai-0.3.1/op_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.148021 colossalai-0.3.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-01 07:02:06.000000 colossalai-0.3.1/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 07:02:06.000000 colossalai-0.3.1/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 07:02:16.160021 colossalai-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-08-01 07:02:06.000000 colossalai-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.048020 colossalai-0.3.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.148021 colossalai-0.3.1/tests/components_to_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/components_to_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/components_to_test/albert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/components_to_test/beit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/components_to_test/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/components_to_test/gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/components_to_test/hanging_param_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/components_to_test/inline_op_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/components_to_test/nested_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/components_to_test/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/components_to_test/repeated_computed_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/components_to_test/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/components_to_test/simple_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.148021 colossalai-0.3.1/tests/components_to_test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/components_to_test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/components_to_test/utils/dummy_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/components_to_test/utils/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.148021 colossalai-0.3.1/tests/kit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/kit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.148021 colossalai-0.3.1/tests/kit/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/kit/model_zoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.148021 colossalai-0.3.1/tests/kit/model_zoo/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/kit/model_zoo/diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/kit/model_zoo/diffusers/diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/kit/model_zoo/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.152021 colossalai-0.3.1/tests/kit/model_zoo/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/kit/model_zoo/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/kit/model_zoo/timm/timm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.152021 colossalai-0.3.1/tests/kit/model_zoo/torchaudio/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/kit/model_zoo/torchaudio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/kit/model_zoo/torchaudio/torchaudio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.152021 colossalai-0.3.1/tests/kit/model_zoo/torchrec/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/kit/model_zoo/torchrec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/kit/model_zoo/torchrec/torchrec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.152021 colossalai-0.3.1/tests/kit/model_zoo/torchvision/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/kit/model_zoo/torchvision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/kit/model_zoo/torchvision/torchvision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.152021 colossalai-0.3.1/tests/kit/model_zoo/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/kit/model_zoo/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/kit/model_zoo/transformers/albert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/kit/model_zoo/transformers/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/kit/model_zoo/transformers/bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/kit/model_zoo/transformers/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/kit/model_zoo/transformers/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/kit/model_zoo/transformers/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/kit/model_zoo/transformers/t5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.152021 colossalai-0.3.1/tests/test_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_analyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.152021 colossalai-0.3.1/tests/test_analyzer/test_fx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_analyzer/test_fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_analyzer/test_fx/test_bias_addition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_analyzer/test_fx/test_mod_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_analyzer/test_fx/test_nested_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_analyzer/test_fx/test_shape_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_analyzer/test_fx/test_symbolic_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_analyzer/test_fx/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.152021 colossalai-0.3.1/tests/test_analyzer/test_subclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_analyzer/test_subclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_analyzer/test_subclasses/test_aten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_analyzer/test_subclasses/test_flop_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_analyzer/test_subclasses/test_meta_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.152021 colossalai-0.3.1/tests/test_auto_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.152021 colossalai-0.3.1/tests/test_auto_parallel/test_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_pass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_pass/test_node_converting_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.152021 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.156020 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.156020 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.156020 colossalai-0.3.1/tests/test_shardformer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_shardformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:16.160021 colossalai-0.3.1/tests/test_shardformer/test_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_shardformer/test_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_shardformer/test_model/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_shardformer/test_model/test_shard_bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_shardformer/test_model/test_shard_bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_shardformer/test_model/test_shard_gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_shardformer/test_model/test_shard_llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_shardformer/test_model/test_shard_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_shardformer/test_model/test_shard_t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_shardformer/test_model/test_shard_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-08-01 07:02:06.000000 colossalai-0.3.1/tests/test_shardformer/test_with_torch_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 07:02:06.000000 colossalai-0.3.1/version.txt
```

### Comparing `colossalai-0.3.0/LICENSE` & `colossalai-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/PKG-INFO` & `colossalai-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colossalai
-Version: 0.3.0
+Version: 0.3.1
 Summary: An integrated large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org
 License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io
@@ -32,14 +32,15 @@
         
         
            | [English](README.md) | [中文](docs/README-zh-Hans.md) |
         
         </div>
         
         ## Latest News
+        * [2023/07] [65B Model Pretraining Accelerated by 38%, Best Practices for Building LLaMA-Like Base Models Open-Source](https://www.hpc-ai.tech/blog/large-model-pretraining)
         * [2023/03] [ColossalChat: An Open-Source Solution for Cloning ChatGPT With a Complete RLHF Pipeline](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b)
         * [2023/03] [Intel and Colossal-AI Partner to Deliver Cost-Efficient Open-Source Solution for Protein Folding Structure Prediction](https://www.hpc-ai.tech/blog/intel-habana)
         * [2023/03] [AWS and Google Fund Colossal-AI with Startup Cloud Programs](https://www.hpc-ai.tech/blog/aws-and-google-fund-colossal-ai-with-startup-cloud-programs)
         * [2023/02] [Open Source Solution Replicates ChatGPT Training Process! Ready to go with only 1.6GB GPU Memory](https://www.hpc-ai.tech/blog/colossal-ai-chatgpt)
         * [2023/01] [Hardware Savings Up to 46 Times for AIGC and  Automatic Parallelism](https://medium.com/pytorch/latest-colossal-ai-boasts-novel-automatic-parallelism-and-offers-savings-up-to-46x-for-stable-1453b48f3f02)
         * [2022/11] [Diffusion Pretraining and Hardware Fine-Tuning Can Be Almost 7X Cheaper](https://www.hpc-ai.tech/blog/diffusion-pretraining-and-hardware-fine-tuning-can-be-almost-7x-cheaper)
         * [2022/10] [Use a Laptop to Analyze 90% of Proteins, With a Single-GPU Inference Sequence Exceeding 10,000](https://www.hpc-ai.tech/blog/use-a-laptop-to-analyze-90-of-proteins-with-a-single-gpu-inference-sequence-exceeding)
@@ -56,14 +57,15 @@
              <li><a href="#AIGC">AIGC: Acceleration of Stable Diffusion</a></li>
              <li><a href="#Biomedicine">Biomedicine: Acceleration of AlphaFold Protein Structure</a></li>
            </ul>
          </li>
          <li>
            <a href="#Parallel-Training-Demo">Parallel Training Demo</a>
            <ul>
+             <li><a href="#LLaMA">LLaMA</a></li>
              <li><a href="#GPT-3">GPT-3</a></li>
              <li><a href="#GPT-2">GPT-2</a></li>
              <li><a href="#BERT">BERT</a></li>
              <li><a href="#PaLM">PaLM</a></li>
              <li><a href="#OPT">OPT</a></li>
              <li><a href="#ViT">ViT</a></li>
              <li><a href="#Recommendation-System-Models">Recommendation System Models</a></li>
@@ -223,14 +225,23 @@
         - [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer): accelerating structure prediction of protein monomers and multimer by 11x.
         
         
         <p align="right">(<a href="#top">back to top</a>)</p>
         
         ## Parallel Training Demo
         
+        ### LLaMA
+        <p align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/examples/images/LLaMA_pretraining.png" width=600/>
+        </p>
+        
+        - 65-billion-parameter large model pretraining accelerated by 38%
+        [[code]](https://github.com/hpcaitech/ColossalAI/tree/example/llama/examples/language/llama)
+        [[blog]](https://www.hpc-ai.tech/blog/large-model-pretraining)
+        
         ### GPT-3
         <p align="center">
         <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT3-v5.png" width=700/>
         </p>
         
         - Save 50% GPU resources and 10.7% acceleration
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colossalai Version: 0.3.0 Summary: An integrated
+Metadata-Version: 2.1 Name: colossalai Version: 0.3.1 Summary: An integrated
 large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io Project-URL:
 Github, https://github.com/hpcaitech/ColossalAI Description: # Colossal-AI
@@ -22,43 +22,47 @@
  (https://img.shields.io/badge/%F0%9F%A4%97HuggingFace-Join-yellow)](https://
 huggingface.co/hpcai-tech) [![slack badge](https://img.shields.io/badge/Slack-
   join-blueviolet?logo=slack&)](https://join.slack.com/t/colossalaiworkspace/
   shared_invite/zt-z7b26eeb-CBp7jouvu~r0~lcFzX832w) [![WeChat badge](https://
        img.shields.io/badge/å¾®ä¿¡-å å¥-green?logo=wechat&)](https://
     raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
     WeChat.png) | [English](README.md) | [ä¸­æ](docs/README-zh-Hans.md) |
-## Latest News * [2023/03] [ColossalChat: An Open-Source Solution for Cloning
-ChatGPT With a Complete RLHF Pipeline](https://medium.com/@yangyou_berkeley/
-colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-
-pipeline-5edf08fb538b) * [2023/03] [Intel and Colossal-AI Partner to Deliver
-Cost-Efficient Open-Source Solution for Protein Folding Structure Prediction]
-(https://www.hpc-ai.tech/blog/intel-habana) * [2023/03] [AWS and Google Fund
-Colossal-AI with Startup Cloud Programs](https://www.hpc-ai.tech/blog/aws-and-
-google-fund-colossal-ai-with-startup-cloud-programs) * [2023/02] [Open Source
-Solution Replicates ChatGPT Training Process! Ready to go with only 1.6GB GPU
-Memory](https://www.hpc-ai.tech/blog/colossal-ai-chatgpt) * [2023/01] [Hardware
-Savings Up to 46 Times for AIGC and Automatic Parallelism](https://medium.com/
-pytorch/latest-colossal-ai-boasts-novel-automatic-parallelism-and-offers-
-savings-up-to-46x-for-stable-1453b48f3f02) * [2022/11] [Diffusion Pretraining
-and Hardware Fine-Tuning Can Be Almost 7X Cheaper](https://www.hpc-ai.tech/
-blog/diffusion-pretraining-and-hardware-fine-tuning-can-be-almost-7x-cheaper) *
-[2022/10] [Use a Laptop to Analyze 90% of Proteins, With a Single-GPU Inference
-Sequence Exceeding 10,000](https://www.hpc-ai.tech/blog/use-a-laptop-to-
-analyze-90-of-proteins-with-a-single-gpu-inference-sequence-exceeding) * [2022/
-09] [HPC-AI Tech Completes $6 Million Seed and Angel Round Fundraising](https:/
-/www.hpc-ai.tech/blog/hpc-ai-tech-completes-6-million-seed-and-angel-round-
-fundraising-led-by-bluerun-ventures-in-the) ## Table of Contents
+## Latest News * [2023/07] [65B Model Pretraining Accelerated by 38%, Best
+Practices for Building LLaMA-Like Base Models Open-Source](https://www.hpc-
+ai.tech/blog/large-model-pretraining) * [2023/03] [ColossalChat: An Open-Source
+Solution for Cloning ChatGPT With a Complete RLHF Pipeline](https://medium.com/
+@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-
+with-a-complete-rlhf-pipeline-5edf08fb538b) * [2023/03] [Intel and Colossal-AI
+Partner to Deliver Cost-Efficient Open-Source Solution for Protein Folding
+Structure Prediction](https://www.hpc-ai.tech/blog/intel-habana) * [2023/03]
+[AWS and Google Fund Colossal-AI with Startup Cloud Programs](https://www.hpc-
+ai.tech/blog/aws-and-google-fund-colossal-ai-with-startup-cloud-programs) *
+[2023/02] [Open Source Solution Replicates ChatGPT Training Process! Ready to
+go with only 1.6GB GPU Memory](https://www.hpc-ai.tech/blog/colossal-ai-
+chatgpt) * [2023/01] [Hardware Savings Up to 46 Times for AIGC and Automatic
+Parallelism](https://medium.com/pytorch/latest-colossal-ai-boasts-novel-
+automatic-parallelism-and-offers-savings-up-to-46x-for-stable-1453b48f3f02) *
+[2022/11] [Diffusion Pretraining and Hardware Fine-Tuning Can Be Almost 7X
+Cheaper](https://www.hpc-ai.tech/blog/diffusion-pretraining-and-hardware-fine-
+tuning-can-be-almost-7x-cheaper) * [2022/10] [Use a Laptop to Analyze 90% of
+Proteins, With a Single-GPU Inference Sequence Exceeding 10,000](https://
+www.hpc-ai.tech/blog/use-a-laptop-to-analyze-90-of-proteins-with-a-single-gpu-
+inference-sequence-exceeding) * [2022/09] [HPC-AI Tech Completes $6 Million
+Seed and Angel Round Fundraising](https://www.hpc-ai.tech/blog/hpc-ai-tech-
+completes-6-million-seed-and-angel-round-fundraising-led-by-bluerun-ventures-
+in-the) ## Table of Contents
     * Why_Colossal-AI
     * Features
     * Colossal-AI_for_Real_World_Applications
           o ColossalChat:_An_Open-Source_Solution_for_Cloning_ChatGPT_With_a
             Complete_RLHF_Pipeline
           o AIGC:_Acceleration_of_Stable_Diffusion
           o Biomedicine:_Acceleration_of_AlphaFold_Protein_Structure
     * Parallel_Training_Demo
+          o LLaMA
           o GPT-3
           o GPT-2
           o BERT
           o PaLM
           o OPT
           o ViT
           o Recommendation_System_Models
@@ -151,15 +155,20 @@
 - [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference
 acceleration and 39% cost reduce.
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                            xTrimoMultimer_Table.jpg]
 - [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer):
 accelerating structure prediction of protein monomers and multimer by 11x.
                                                                   (back_to_top)
-## Parallel Training Demo ### GPT-3
+## Parallel Training Demo ### LLaMA
+   [https://raw.githubusercontent.com/hpcaitech/public_assets/main/examples/
+                         images/LLaMA_pretraining.png]
+- 65-billion-parameter large model pretraining accelerated by 38% [[code]]
+(https://github.com/hpcaitech/ColossalAI/tree/example/llama/examples/language/
+llama) [[blog]](https://www.hpc-ai.tech/blog/large-model-pretraining) ### GPT-3
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                                  GPT3-v5.png]
 - Save 50% GPU resources and 10.7% acceleration ### GPT-2 [https://
 raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT2.png]
 - 11x lower GPU memory consumption, and superlinear scaling efficiency with
 Tensor Parallelism [https://raw.githubusercontent.com/hpcaitech/public_assets/
 main/colossalai/img/(updated)GPT-2.png] - 24x larger model size on the same
```

### Comparing `colossalai-0.3.0/README.md` & `colossalai-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 
    | [English](README.md) | [中文](docs/README-zh-Hans.md) |
 
 </div>
 
 ## Latest News
+* [2023/07] [65B Model Pretraining Accelerated by 38%, Best Practices for Building LLaMA-Like Base Models Open-Source](https://www.hpc-ai.tech/blog/large-model-pretraining)
 * [2023/03] [ColossalChat: An Open-Source Solution for Cloning ChatGPT With a Complete RLHF Pipeline](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b)
 * [2023/03] [Intel and Colossal-AI Partner to Deliver Cost-Efficient Open-Source Solution for Protein Folding Structure Prediction](https://www.hpc-ai.tech/blog/intel-habana)
 * [2023/03] [AWS and Google Fund Colossal-AI with Startup Cloud Programs](https://www.hpc-ai.tech/blog/aws-and-google-fund-colossal-ai-with-startup-cloud-programs)
 * [2023/02] [Open Source Solution Replicates ChatGPT Training Process! Ready to go with only 1.6GB GPU Memory](https://www.hpc-ai.tech/blog/colossal-ai-chatgpt)
 * [2023/01] [Hardware Savings Up to 46 Times for AIGC and  Automatic Parallelism](https://medium.com/pytorch/latest-colossal-ai-boasts-novel-automatic-parallelism-and-offers-savings-up-to-46x-for-stable-1453b48f3f02)
 * [2022/11] [Diffusion Pretraining and Hardware Fine-Tuning Can Be Almost 7X Cheaper](https://www.hpc-ai.tech/blog/diffusion-pretraining-and-hardware-fine-tuning-can-be-almost-7x-cheaper)
 * [2022/10] [Use a Laptop to Analyze 90% of Proteins, With a Single-GPU Inference Sequence Exceeding 10,000](https://www.hpc-ai.tech/blog/use-a-laptop-to-analyze-90-of-proteins-with-a-single-gpu-inference-sequence-exceeding)
@@ -45,14 +46,15 @@
      <li><a href="#AIGC">AIGC: Acceleration of Stable Diffusion</a></li>
      <li><a href="#Biomedicine">Biomedicine: Acceleration of AlphaFold Protein Structure</a></li>
    </ul>
  </li>
  <li>
    <a href="#Parallel-Training-Demo">Parallel Training Demo</a>
    <ul>
+     <li><a href="#LLaMA">LLaMA</a></li>
      <li><a href="#GPT-3">GPT-3</a></li>
      <li><a href="#GPT-2">GPT-2</a></li>
      <li><a href="#BERT">BERT</a></li>
      <li><a href="#PaLM">PaLM</a></li>
      <li><a href="#OPT">OPT</a></li>
      <li><a href="#ViT">ViT</a></li>
      <li><a href="#Recommendation-System-Models">Recommendation System Models</a></li>
@@ -212,14 +214,23 @@
 - [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer): accelerating structure prediction of protein monomers and multimer by 11x.
 
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Parallel Training Demo
 
+### LLaMA
+<p align="center">
+<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/examples/images/LLaMA_pretraining.png" width=600/>
+</p>
+
+- 65-billion-parameter large model pretraining accelerated by 38%
+[[code]](https://github.com/hpcaitech/ColossalAI/tree/example/llama/examples/language/llama)
+[[blog]](https://www.hpc-ai.tech/blog/large-model-pretraining)
+
 ### GPT-3
 <p align="center">
 <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT3-v5.png" width=700/>
 </p>
 
 - Save 50% GPU resources and 10.7% acceleration
```

#### html2text {}

```diff
@@ -15,43 +15,47 @@
  (https://img.shields.io/badge/%F0%9F%A4%97HuggingFace-Join-yellow)](https://
 huggingface.co/hpcai-tech) [![slack badge](https://img.shields.io/badge/Slack-
   join-blueviolet?logo=slack&)](https://join.slack.com/t/colossalaiworkspace/
   shared_invite/zt-z7b26eeb-CBp7jouvu~r0~lcFzX832w) [![WeChat badge](https://
        img.shields.io/badge/å¾®ä¿¡-å å¥-green?logo=wechat&)](https://
     raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
     WeChat.png) | [English](README.md) | [ä¸­æ](docs/README-zh-Hans.md) |
-## Latest News * [2023/03] [ColossalChat: An Open-Source Solution for Cloning
-ChatGPT With a Complete RLHF Pipeline](https://medium.com/@yangyou_berkeley/
-colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-
-pipeline-5edf08fb538b) * [2023/03] [Intel and Colossal-AI Partner to Deliver
-Cost-Efficient Open-Source Solution for Protein Folding Structure Prediction]
-(https://www.hpc-ai.tech/blog/intel-habana) * [2023/03] [AWS and Google Fund
-Colossal-AI with Startup Cloud Programs](https://www.hpc-ai.tech/blog/aws-and-
-google-fund-colossal-ai-with-startup-cloud-programs) * [2023/02] [Open Source
-Solution Replicates ChatGPT Training Process! Ready to go with only 1.6GB GPU
-Memory](https://www.hpc-ai.tech/blog/colossal-ai-chatgpt) * [2023/01] [Hardware
-Savings Up to 46 Times for AIGC and Automatic Parallelism](https://medium.com/
-pytorch/latest-colossal-ai-boasts-novel-automatic-parallelism-and-offers-
-savings-up-to-46x-for-stable-1453b48f3f02) * [2022/11] [Diffusion Pretraining
-and Hardware Fine-Tuning Can Be Almost 7X Cheaper](https://www.hpc-ai.tech/
-blog/diffusion-pretraining-and-hardware-fine-tuning-can-be-almost-7x-cheaper) *
-[2022/10] [Use a Laptop to Analyze 90% of Proteins, With a Single-GPU Inference
-Sequence Exceeding 10,000](https://www.hpc-ai.tech/blog/use-a-laptop-to-
-analyze-90-of-proteins-with-a-single-gpu-inference-sequence-exceeding) * [2022/
-09] [HPC-AI Tech Completes $6 Million Seed and Angel Round Fundraising](https:/
-/www.hpc-ai.tech/blog/hpc-ai-tech-completes-6-million-seed-and-angel-round-
-fundraising-led-by-bluerun-ventures-in-the) ## Table of Contents
+## Latest News * [2023/07] [65B Model Pretraining Accelerated by 38%, Best
+Practices for Building LLaMA-Like Base Models Open-Source](https://www.hpc-
+ai.tech/blog/large-model-pretraining) * [2023/03] [ColossalChat: An Open-Source
+Solution for Cloning ChatGPT With a Complete RLHF Pipeline](https://medium.com/
+@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-
+with-a-complete-rlhf-pipeline-5edf08fb538b) * [2023/03] [Intel and Colossal-AI
+Partner to Deliver Cost-Efficient Open-Source Solution for Protein Folding
+Structure Prediction](https://www.hpc-ai.tech/blog/intel-habana) * [2023/03]
+[AWS and Google Fund Colossal-AI with Startup Cloud Programs](https://www.hpc-
+ai.tech/blog/aws-and-google-fund-colossal-ai-with-startup-cloud-programs) *
+[2023/02] [Open Source Solution Replicates ChatGPT Training Process! Ready to
+go with only 1.6GB GPU Memory](https://www.hpc-ai.tech/blog/colossal-ai-
+chatgpt) * [2023/01] [Hardware Savings Up to 46 Times for AIGC and Automatic
+Parallelism](https://medium.com/pytorch/latest-colossal-ai-boasts-novel-
+automatic-parallelism-and-offers-savings-up-to-46x-for-stable-1453b48f3f02) *
+[2022/11] [Diffusion Pretraining and Hardware Fine-Tuning Can Be Almost 7X
+Cheaper](https://www.hpc-ai.tech/blog/diffusion-pretraining-and-hardware-fine-
+tuning-can-be-almost-7x-cheaper) * [2022/10] [Use a Laptop to Analyze 90% of
+Proteins, With a Single-GPU Inference Sequence Exceeding 10,000](https://
+www.hpc-ai.tech/blog/use-a-laptop-to-analyze-90-of-proteins-with-a-single-gpu-
+inference-sequence-exceeding) * [2022/09] [HPC-AI Tech Completes $6 Million
+Seed and Angel Round Fundraising](https://www.hpc-ai.tech/blog/hpc-ai-tech-
+completes-6-million-seed-and-angel-round-fundraising-led-by-bluerun-ventures-
+in-the) ## Table of Contents
     * Why_Colossal-AI
     * Features
     * Colossal-AI_for_Real_World_Applications
           o ColossalChat:_An_Open-Source_Solution_for_Cloning_ChatGPT_With_a
             Complete_RLHF_Pipeline
           o AIGC:_Acceleration_of_Stable_Diffusion
           o Biomedicine:_Acceleration_of_AlphaFold_Protein_Structure
     * Parallel_Training_Demo
+          o LLaMA
           o GPT-3
           o GPT-2
           o BERT
           o PaLM
           o OPT
           o ViT
           o Recommendation_System_Models
@@ -144,15 +148,20 @@
 - [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference
 acceleration and 39% cost reduce.
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                            xTrimoMultimer_Table.jpg]
 - [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer):
 accelerating structure prediction of protein monomers and multimer by 11x.
                                                                   (back_to_top)
-## Parallel Training Demo ### GPT-3
+## Parallel Training Demo ### LLaMA
+   [https://raw.githubusercontent.com/hpcaitech/public_assets/main/examples/
+                         images/LLaMA_pretraining.png]
+- 65-billion-parameter large model pretraining accelerated by 38% [[code]]
+(https://github.com/hpcaitech/ColossalAI/tree/example/llama/examples/language/
+llama) [[blog]](https://www.hpc-ai.tech/blog/large-model-pretraining) ### GPT-3
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                                  GPT3-v5.png]
 - Save 50% GPU resources and 10.7% acceleration ### GPT-2 [https://
 raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT2.png]
 - 11x lower GPU memory consumption, and superlinear scaling efficiency with
 Tensor Parallelism [https://raw.githubusercontent.com/hpcaitech/public_assets/
 main/colossalai/img/(updated)GPT-2.png] - 24x larger model size on the same
```

### Comparing `colossalai-0.3.0/colossalai/__init__.py` & `colossalai-0.3.1/colossalai/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/_analyzer/_subclasses/_meta_registration.py` & `colossalai-0.3.1/colossalai/_analyzer/_subclasses/_meta_registration.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/_analyzer/_subclasses/_monkey_patch.py` & `colossalai-0.3.1/colossalai/_analyzer/_subclasses/_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/_analyzer/_subclasses/flop_tensor.py` & `colossalai-0.3.1/colossalai/_analyzer/_subclasses/flop_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/_analyzer/_subclasses/meta_tensor.py` & `colossalai-0.3.1/colossalai/_analyzer/_subclasses/meta_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/_analyzer/fx/codegen.py` & `colossalai-0.3.1/colossalai/_analyzer/fx/codegen.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/_analyzer/fx/graph_module.py` & `colossalai-0.3.1/colossalai/_analyzer/fx/graph_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/_analyzer/fx/node_util.py` & `colossalai-0.3.1/colossalai/_analyzer/fx/node_util.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/_analyzer/fx/passes/graph_profile.py` & `colossalai-0.3.1/colossalai/_analyzer/fx/passes/graph_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/_analyzer/fx/passes/shape_prop.py` & `colossalai-0.3.1/colossalai/_analyzer/fx/passes/shape_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/_analyzer/fx/symbolic_profile.py` & `colossalai-0.3.1/colossalai/_analyzer/fx/symbolic_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/_analyzer/fx/tracer/bias_addition.py` & `colossalai-0.3.1/colossalai/_analyzer/fx/tracer/bias_addition.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/_analyzer/fx/tracer/custom_leaf_module.py` & `colossalai-0.3.1/colossalai/_analyzer/fx/tracer/custom_leaf_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/_analyzer/fx/tracer/proxy.py` & `colossalai-0.3.1/colossalai/_analyzer/fx/tracer/proxy.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/_analyzer/fx/tracer/symbolic_trace.py` & `colossalai-0.3.1/colossalai/_analyzer/fx/tracer/symbolic_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/_analyzer/fx/tracer/tracer.py` & `colossalai-0.3.1/colossalai/_analyzer/fx/tracer/tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/amp/__init__.py` & `colossalai-0.3.1/colossalai/amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/amp/apex_amp/__init__.py` & `colossalai-0.3.1/colossalai/amp/apex_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/amp/apex_amp/apex_amp.py` & `colossalai-0.3.1/colossalai/amp/apex_amp/apex_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/amp/naive_amp/__init__.py` & `colossalai-0.3.1/colossalai/amp/naive_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/amp/naive_amp/_fp16_optimizer.py` & `colossalai-0.3.1/colossalai/amp/naive_amp/_fp16_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/amp/naive_amp/_utils.py` & `colossalai-0.3.1/colossalai/amp/naive_amp/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py` & `colossalai-0.3.1/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py` & `colossalai-0.3.1/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py` & `colossalai-0.3.1/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/amp/naive_amp/naive_amp.py` & `colossalai-0.3.1/colossalai/amp/naive_amp/naive_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/amp/torch_amp/__init__.py` & `colossalai-0.3.1/colossalai/amp/torch_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/amp/torch_amp/_grad_scaler.py` & `colossalai-0.3.1/colossalai/amp/torch_amp/_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/amp/torch_amp/torch_amp.py` & `colossalai-0.3.1/colossalai/amp/torch_amp/torch_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py` & `colossalai-0.3.1/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py` & `colossalai-0.3.1/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py` & `colossalai-0.3.1/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/checkpoint/operation.py` & `colossalai-0.3.1/colossalai/auto_parallel/checkpoint/operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py` & `colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py` & `colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py` & `colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py` & `colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py` & `colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py` & `colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py` & `colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py` & `colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py` & `colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/meta_registry/where.py` & `colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/meta_registry/where.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/registry.py` & `colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/meta_profiler/shard_metainfo.py` & `colossalai-0.3.1/colossalai/auto_parallel/meta_profiler/shard_metainfo.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/offload/amp_optimizer.py` & `colossalai-0.3.1/colossalai/auto_parallel/offload/amp_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-from typing import Dict, Tuple
 from enum import Enum
+from typing import Dict, Tuple
+
 import torch
 from torch.optim import Optimizer
 
+from colossalai.amp.naive_amp.grad_scaler import DynamicGradScaler
 from colossalai.logging import get_dist_logger
 from colossalai.nn.optimizer import ColossalaiOptimizer
-from colossalai.amp.naive_amp.grad_scaler import DynamicGradScaler
 from colossalai.utils import get_current_device
 
 from .base_offload_module import BaseOffloadModule
-from .region_manager import RegionManager
 from .region import Region
+from .region_manager import RegionManager
 
 
 class OptimState(Enum):
     SCALED = 0
     UNSCALED = 1
 
-class AMPOptimizer(ColossalaiOptimizer):
 
+class AMPOptimizer(ColossalaiOptimizer):
     """
     A wrapper for Optimizer.
     Code reference: https://github.com/hpcaitech/ColossalAI/blob/main/colossalai/nn/optimizer/zero_optimizer.py
 
     Args:
         optimizer (Optimizer): An Optimizer instance.
         module (BaseOffloadModule): A ``BaseOffloadModule`` instance.
@@ -170,8 +171,8 @@
                 if param in self.optim.state:
                     self.optim.state[fake_param] = self.optim.state.pop(param)
 
             group['params'] = fake_params_list
 
         # Leverage state_dict() and load_state_dict() to
         # recast preexisting per-param state tensors
-        self.optim.load_state_dict(self.optim.state_dict())
+        self.optim.load_state_dict(self.optim.state_dict())
```

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/offload/base_offload_module.py` & `colossalai-0.3.1/colossalai/auto_parallel/offload/base_offload_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/offload/mem_optimize.py` & `colossalai-0.3.1/colossalai/auto_parallel/offload/mem_optimize.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/offload/region.py` & `colossalai-0.3.1/colossalai/auto_parallel/offload/region.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/offload/region_manager.py` & `colossalai-0.3.1/colossalai/auto_parallel/offload/region_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/offload/runtime.py` & `colossalai-0.3.1/colossalai/auto_parallel/offload/runtime.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/offload/solver.py` & `colossalai-0.3.1/colossalai/auto_parallel/offload/solver.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/offload/training_simulator.py` & `colossalai-0.3.1/colossalai/auto_parallel/offload/training_simulator.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/offload/util.py` & `colossalai-0.3.1/colossalai/auto_parallel/offload/util.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/passes/comm_metainfo_pass.py` & `colossalai-0.3.1/colossalai/auto_parallel/passes/comm_metainfo_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/passes/meta_info_prop.py` & `colossalai-0.3.1/colossalai/auto_parallel/passes/meta_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/passes/runtime_apply_pass.py` & `colossalai-0.3.1/colossalai/auto_parallel/passes/runtime_apply_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/passes/runtime_preparation_pass.py` & `colossalai-0.3.1/colossalai/auto_parallel/passes/runtime_preparation_pass.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                 size[dim] = dim_size * total_shard_size
         size = torch.Size(size)
 
     return size
 
 
 def solution_annotation_pass(gm: torch.fx.GraphModule, solution: List[int],
-                               strategies_constructor: StrategiesConstructor):
+                             strategies_constructor: StrategiesConstructor):
     """
     This method is used to stick the solution strategy to the nodes and add the information
     required in runtime into graph as placeholder nodes.
     """
     mod_graph = gm.graph
 
     nodes = [strategies_vector.node for strategies_vector in strategies_constructor.leaf_strategies]
```

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/constants.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/initialize.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/initialize.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
             for op_data, sharding_spec in strategy.sharding_specs.items():
                 if op_data.data is not None and isinstance(op_data.data, torch.Tensor):
                     check_sharding_spec_validity(sharding_spec, op_data.data)
 
         remove_strategy_list = []
         for strategy in self.strategies_vector:
             shard_axis_list = []
-            last_axis = len(self.device_mesh.mesh_shape) - 1
+            last_axis = len(self.device_mesh.shape) - 1
             for op_data, sharding_spec in strategy.sharding_specs.items():
                 if op_data.data is not None and isinstance(op_data.data, torch.Tensor):
                     for dim, shard_axes in sharding_spec.dim_partition_dict.items():
                         for shard_axis in shard_axes:
                             if shard_axis not in shard_axis_list:
                                 shard_axis_list.append(shard_axis)
```

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/registry.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -980,26 +980,26 @@
         return self.get_sharding_strategy(name=name,
                                           sharding_spec_mapping=sharding_spec_mapping,
                                           communication_action_mapping=communication_action_mapping)
 
     def collate_strategies(self) -> List[ShardingStrategy]:
         strategy_list = []
         device_mesh_is_1d = True
-        if len(self.device_mesh.mesh_shape) == 2 and 1 not in self.device_mesh.mesh_shape:
+        if len(self.device_mesh.shape) == 2 and 1 not in self.device_mesh.shape:
             device_mesh_is_1d = False
 
         if device_mesh_is_1d:
             # split only the batch dimension
             # Sb = Sb x Sb
             # can be None as it is only for 1D device mesh
             # only for 1D device mesh
-            if len(self.device_mesh.mesh_shape) == 1:
+            if len(self.device_mesh.shape) == 1:
                 mesh_dim = 0
             else:
-                mesh_dim = self.device_mesh.mesh_shape.index(1)
+                mesh_dim = self.device_mesh.shape.index(1)
             strategy_list.append(self.split_one_batch_dim(mesh_dim))
         else:
             # for 2D device mesh
             # split batch dim of two inputs and the i dim of the first tensor
             # SbSi = SbSi x Sb
             strategy_list.append(self.split_batch_dim_lhs_space(0, 1))
             strategy_list.append(self.split_batch_dim_lhs_space(1, 0))
```

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import copy
 from typing import List
 
-from colossalai.auto_parallel.tensor_shard.sharding_strategy import (MemoryCost, ShardingStrategy, TrainCycleItem)
+from colossalai.auto_parallel.tensor_shard.sharding_strategy import MemoryCost, ShardingStrategy, TrainCycleItem
 
 from .strategy_generator import FollowingStrategyGenerator
 
 __all__ = ['UnaryElementwiseGenerator']
 
 
 class UnaryElementwiseGenerator(FollowingStrategyGenerator):
```

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/options.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/options.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/sharding_strategy.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/sharding_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/solver/solver.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/solver/solver.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/utils/__init__.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/utils/broadcast.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/utils/broadcast.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/utils/factory.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/utils/factory.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/utils/misc.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/utils/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,16 @@
         2. the sharding spec for each dimension is divisible by the number of devices.
         3. the sharding spec's entire shape must match the tensor shape
     #
     """
     # make sure all dims are covered in sharding spec
     sharding_len = len(sharding_spec.sharding_sequence)
     tensor_num_dim = tensor.dim()
-    num_devices_in_col = sharding_spec.device_mesh.mesh_shape[0]
-    num_devices_in_row = sharding_spec.device_mesh.mesh_shape[1]
+    num_devices_in_col = sharding_spec.device_mesh.shape[0]
+    num_devices_in_row = sharding_spec.device_mesh.shape[1]
     assert sharding_len == tensor_num_dim, \
         f'The ShardingSpec ({sharding_spec.sharding_sequence}) is created for {sharding_len}-dimension tensor, but the given tensor is {tensor_num_dim}-dimension ({tensor.shape}).'
 
     # make sure the sharding is valid for each dim
     for i in range(tensor_num_dim):
         dim_size = tensor.shape[i]
         dim_spec = sharding_spec.sharding_sequence[i]
```

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/utils/reshape.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/utils/reshape.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/auto_parallel/tensor_shard/utils/sharding.py` & `colossalai-0.3.1/colossalai/auto_parallel/tensor_shard/utils/sharding.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/booster/accelerator.py` & `colossalai-0.3.1/colossalai/booster/accelerator.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/booster/booster.py` & `colossalai-0.3.1/colossalai/booster/booster.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import torch
 import torch.nn as nn
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
 from torch.utils.data import DataLoader
 
 from colossalai.checkpoint_io import GeneralCheckpointIO
+from colossalai.interface import ModelWrapper, OptimizerWrapper
 
 from .accelerator import Accelerator
 from .mixed_precision import MixedPrecision, mixed_precision_factory
 from .plugin import Plugin
 
 __all__ = ['Booster']
 
@@ -21,19 +22,19 @@
     """
     Booster is a high-level API for training neural networks. It provides a unified interface for
     training with different precision, accelerator, and plugin.
 
     Examples:
         ```python
         colossalai.launch(...)
-        plugin = GeminiPlugin(stage=3, ...)
+        plugin = GeminiPlugin(...)
         booster = Booster(precision='fp16', plugin=plugin)
 
         model = GPT2()
-        optimizer = Adam(model.parameters())
+        optimizer = HybridAdam(model.parameters())
         dataloader = Dataloader(Dataset)
         lr_scheduler = LinearWarmupScheduler()
         criterion = GPTLMLoss()
 
         model, optimizer, lr_scheduler, dataloader = booster.boost(model, optimizer, lr_scheduler, dataloader)
 
         for epoch in range(max_epochs):
@@ -93,18 +94,18 @@
             self.checkpoint_io = self.plugin.get_checkpoint_io()
         else:
             self.checkpoint_io = GeneralCheckpointIO()
 
     def boost(
         self,
         model: nn.Module,
-        optimizer: Optimizer,
-        criterion: Callable = None,
-        dataloader: DataLoader = None,
-        lr_scheduler: LRScheduler = None,
+        optimizer: Optional[Optimizer] = None,
+        criterion: Optional[Callable] = None,
+        dataloader: Optional[DataLoader] = None,
+        lr_scheduler: Optional[LRScheduler] = None,
     ) -> List[Union[nn.Module, Optimizer, LRScheduler, DataLoader]]:
         """
         Boost the model, optimizer, criterion, lr_scheduler, and dataloader.
 
         Args:
             model (nn.Module): The model to be boosted.
             optimizer (Optimizer): The optimizer to be boosted.
@@ -148,83 +149,107 @@
                          return_loss: bool = True,
                          return_outputs: bool = False) -> Tuple[Optional[torch.Tensor], ...]:
         # TODO: implement this method
         # run pipeline forward backward pass
         # return loss or outputs if needed
         pass
 
-    def no_sync(self, model: nn.Module) -> contextmanager:
+    def no_sync(self, model: nn.Module = None, optimizer: OptimizerWrapper = None) -> contextmanager:
         """Context manager to disable gradient synchronization across DP process groups.
+           Support torch DDP and Low Level ZeRO-1 for now.
 
         Args:
-            model (nn.Module): The model to be disabled gradient synchronization.
+            model (nn.Module): The model to be disabled gradient synchronization, for DDP
+            optimizer (OptimizerWrapper): The optimizer to be disabled gradient synchronization, for ZeRO1-1
 
         Returns:
             contextmanager: Context to disable gradient synchronization.
         """
         assert self.plugin is not None, f'no_sync is only enabled when a plugin is provided and the plugin supports no_sync.'
-        assert self.plugin.support_no_sync, f'The plugin {self.plugin.__class__.__name__} does not support no_sync.'
-        return self.plugin.no_sync(model)
+        assert self.plugin.support_no_sync(), f'The plugin {self.plugin.__class__.__name__} does not support no_sync.'
+        return self.plugin.no_sync(model, optimizer)
 
-    def load_model(self, model: nn.Module, checkpoint: str, strict: bool = True):
+    def load_model(self, model: Union[nn.Module, ModelWrapper], checkpoint: str, strict: bool = True):
         """Load model from checkpoint.
 
         Args:
-            model (nn.Module): A model boosted by Booster.
+            model (nn.Module or ModelWrapper): A model boosted by Booster.
             checkpoint (str): Path to the checkpoint. It must be a local path.
                 It should be a directory path if the checkpoint is sharded. Otherwise, it should be a file path.
             strict (bool, optional): whether to strictly enforce that the keys
                 in :attr:`state_dict` match the keys returned by this module's
                 :meth:`~torch.nn.Module.state_dict` function. Defaults to True.
         """
         self.checkpoint_io.load_model(model, checkpoint, strict)
 
     def save_model(self,
-                   model: nn.Module,
+                   model: Union[nn.Module, ModelWrapper],
                    checkpoint: str,
-                   prefix: str = None,
                    shard: bool = False,
-                   size_per_shard: int = 1024):
+                   gather_dtensor: bool = True,
+                   prefix: Optional[str] = None,
+                   size_per_shard: int = 1024,
+                   use_safetensors: bool = False):
         """Save model to checkpoint.
 
         Args:
-            model (nn.Module): A model boosted by Booster.
+            model (nn.Module or ModelWrapper): A model boosted by Booster.
             checkpoint (str): Path to the checkpoint. It must be a local path.
                 It is a file path if ``shard=False``. Otherwise, it is a directory path.
-            prefix (str, optional): A prefix added to parameter and buffer
-                names to compose the keys in state_dict. Defaults to None.
             shard (bool, optional): Whether to save checkpoint a sharded way.
                 If true, the checkpoint will be a folder. Otherwise, it will be a single file. Defaults to False.
+            gather_dtensor (bool, optional): whether to gather the distributed tensor to the first device. Default: True.
+            prefix (str, optional): A prefix added to parameter and buffer
+                names to compose the keys in state_dict. Defaults to None.
             size_per_shard (int, optional): Maximum size of checkpoint shard file in MB. This is useful only when ``shard=True``. Defaults to 1024.
+            use_safetensors (bool, optional): whether to use safe tensors. Default: False. If set to True, the checkpoint will be saved.
         """
-        self.checkpoint_io.save_model(model, checkpoint=checkpoint, shard=shard, size_per_shard=size_per_shard)
+        self.checkpoint_io.save_model(model,
+                                      checkpoint=checkpoint,
+                                      shard=shard,
+                                      gather_dtensor=gather_dtensor,
+                                      prefix=prefix,
+                                      size_per_shard=size_per_shard,
+                                      use_safetensors=use_safetensors)
 
     def load_optimizer(self, optimizer: Optimizer, checkpoint: str):
         """Load optimizer from checkpoint.
 
         Args:
             optimizer (Optimizer): An optimizer boosted by Booster.
             checkpoint (str): Path to the checkpoint. It must be a local path.
                 It should be a directory path if the checkpoint is sharded. Otherwise, it should be a file path.
+            prefix (str, optional): A prefix added to parameter and buffer
+                names to compose the keys in state_dict. Defaults to None.
+            size_per_shard (int, optional): Maximum size of checkpoint shard file in MB. This is useful only when ``shard=True``. Defaults to 1024.
         """
         self.checkpoint_io.load_optimizer(optimizer, checkpoint)
 
-    def save_optimizer(self, optimizer: Optimizer, checkpoint: str, shard: bool = False, size_per_shard: int = 1024):
-        """Save optimizer to checkpoint.
-        Warning: Saving sharded optimizer checkpoint is not supported yet.
+    def save_optimizer(self,
+                       optimizer: Optimizer,
+                       checkpoint: str,
+                       shard: bool = False,
+                       gather_dtensor: bool = True,
+                       prefix: Optional[str] = None,
+                       size_per_shard: int = 1024):
+        """
+        Save optimizer to checkpoint.
 
         Args:
             optimizer (Optimizer): An optimizer boosted by Booster.
             checkpoint (str): Path to the checkpoint. It must be a local path.
                 It is a file path if ``shard=False``. Otherwise, it is a directory path.
             shard (bool, optional): Whether to save checkpoint a sharded way.
                 If true, the checkpoint will be a folder. Otherwise, it will be a single file. Defaults to False.
+            gather_dtensor (bool): whether to gather the distributed tensor to the first device. Default: True.
+            prefix (str, optional): A prefix added to parameter and buffer
+                names to compose the keys in state_dict. Defaults to None.
             size_per_shard (int, optional): Maximum size of checkpoint shard file in MB. This is useful only when ``shard=True``. Defaults to 1024.
         """
-        self.checkpoint_io.save_optimizer(optimizer, checkpoint, shard, size_per_shard)
+        self.checkpoint_io.save_optimizer(optimizer, checkpoint, shard, gather_dtensor, prefix, size_per_shard)
 
     def save_lr_scheduler(self, lr_scheduler: LRScheduler, checkpoint: str):
         """Save lr scheduler to checkpoint.
 
         Args:
             lr_scheduler (LRScheduler): A lr scheduler boosted by Booster.
             checkpoint (str): Path to the checkpoint. It must be a local file path.
```

### Comparing `colossalai-0.3.0/colossalai/booster/mixed_precision/__init__.py` & `colossalai-0.3.1/colossalai/booster/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/booster/mixed_precision/fp16_apex.py` & `colossalai-0.3.1/colossalai/booster/mixed_precision/fp16_apex.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/booster/mixed_precision/fp16_naive.py` & `colossalai-0.3.1/colossalai/booster/mixed_precision/fp16_naive.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/booster/mixed_precision/fp16_torch.py` & `colossalai-0.3.1/colossalai/booster/mixed_precision/fp16_torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,16 @@
         self.torch_amp_kwargs = dict(init_scale=init_scale,
                                      growth_factor=growth_factor,
                                      backoff_factor=backoff_factor,
                                      growth_interval=growth_interval)
 
     def configure(self,
                   model: nn.Module,
-                  optimizer: Optimizer,
-                  criterion: Callable = None) -> Tuple[nn.Module, OptimizerWrapper, Callable]:
+                  optimizer: Optional[Optimizer] = None,
+                  criterion: Optional[Callable] = None,
+                  ) -> Tuple[nn.Module, OptimizerWrapper, Callable]:
         model = TorchAMPModule(model)
-        optimizer = TorchAMPOptimizer(optimizer, **self.torch_amp_kwargs)
+        if optimizer is not None:
+            optimizer = TorchAMPOptimizer(optimizer, **self.torch_amp_kwargs)
         if criterion is not None:
             criterion = TorchAMPModule(criterion)
         return model, optimizer, criterion
```

### Comparing `colossalai-0.3.0/colossalai/booster/mixed_precision/mixed_precision_base.py` & `colossalai-0.3.1/colossalai/booster/mixed_precision/mixed_precision_base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from abc import ABC, abstractmethod
-from typing import Callable, Tuple
+from typing import Callable, Optional, Tuple
 
 import torch.nn as nn
 from torch.optim import Optimizer
 
 from colossalai.interface import OptimizerWrapper
 
 
 class MixedPrecision(ABC):
     """
     An abstract class for mixed precision training.
     """
 
     @abstractmethod
-    def configure(self,
-                  model: nn.Module,
-                  optimizer: Optimizer,
-                  criterion: Callable = None) -> Tuple[nn.Module, OptimizerWrapper, Callable]:
+    def configure(
+        self,
+        model: nn.Module,
+        optimizer: Optional[Optimizer] = None,
+        criterion: Optional[Callable] = None,
+    ) -> Tuple[nn.Module, OptimizerWrapper, Callable]:
         # TODO: implement this method
         pass
```

### Comparing `colossalai-0.3.0/colossalai/booster/plugin/dp_plugin_base.py` & `colossalai-0.3.1/colossalai/booster/plugin/dp_plugin_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/booster/plugin/gemini_plugin.py` & `colossalai-0.3.1/colossalai/booster/plugin/low_level_zero_plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,299 +1,292 @@
 import logging
 import os
 import warnings
+from functools import partial
 from pathlib import Path
 from typing import Callable, Iterator, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 from torch import Tensor
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
+from torch.utils._pytree import tree_map
 from torch.utils.data import DataLoader
 
-from colossalai.checkpoint_io import CheckpointIndexFile, CheckpointIO, GeneralCheckpointIO
-from colossalai.checkpoint_io.utils import get_base_filenames, get_shard_filename, save_state_dict
-from colossalai.cluster import DistCoordinator
+from colossalai.checkpoint_io import CheckpointIndexFile, CheckpointIO
+from colossalai.checkpoint_io.utils import (
+    get_optimizer_base_filenames,
+    get_shard_filename,
+    save_param_groups,
+    save_state_dict,
+)
 from colossalai.interface import ModelWrapper, OptimizerWrapper
 from colossalai.utils import get_current_device
-from colossalai.zero import GeminiDDP, zero_model_wrapper, zero_optim_wrapper
-from colossalai.zero.gemini.memory_tracer import MemStats
+from colossalai.zero import LowLevelZeroOptimizer, zero_model_wrapper, zero_optim_wrapper
 
 from .dp_plugin_base import DPPluginBase
+from .torch_ddp_plugin import TorchDDPCheckpointIO
 
-__all__ = ['GeminiPlugin']
+__all__ = ['LowLevelZeroPlugin']
 
 
-class GeminiCheckpointIO(GeneralCheckpointIO):
+def _convert_floating_point(x, dtype: torch.dtype = torch.float16):
+    if isinstance(x, torch.Tensor) and torch.is_floating_point(x):
+        return x.to(dtype)
+    return x
 
-    def __init__(self) -> None:
-        super().__init__()
-        self.coordinator = DistCoordinator()
 
-    def load_unsharded_model(self, model: GeminiDDP, checkpoint: str, strict: bool = True):
-        """
-        Load model from checkpoint with automatic unwrapping.
-        """
-        # the model should be unwrapped in self.load_model via ModelWrapper.unwrap
-        return super().load_unsharded_model(model, checkpoint, strict=strict)
+SUPPORTED_PRECISION = ['fp16', 'bf16', 'fp32']
 
-    def save_unsharded_model(self, model: GeminiDDP, checkpoint: str, gather_dtensor: bool, use_safetensors: bool):
-        """
-        Save model to checkpoint but only on master process.
-        """
-        # the model should be unwrapped in self.load_model via ModelWrapper.unwrap
-        # as there is communication when get state dict, this must be called on all processes
-        state_dict = model.state_dict(only_rank_0=True)
-        if self.coordinator.is_master():
-            save_state_dict(state_dict, checkpoint, use_safetensors)
 
-    def save_unsharded_optimizer(self, optimizer: Optimizer, checkpoint: str, gather_dtensor: bool):
-        """
-        Save optimizer to checkpoint but only on master process.
-        """
-        # TODO(ver217): optimizer state dict is sharded
-        warnings.warn('GeminiPlugin does not support save full optimizer checkpoint now. Save it on every process.')
-        checkpoint = f'{checkpoint}.rank{self.coordinator.rank}'
-        super().save_unsharded_optimizer(optimizer, checkpoint, gather_dtensor)
-
-    def load_optimizer(self, optimizer: Optimizer, checkpoint: str):
-        warnings.warn(
-            'GeminiPlugin can only load optimizer checkpoint saved by itself with the same number of processes.')
-        checkpoint = f'{checkpoint}.rank{self.coordinator.rank}'
-        super().load_optimizer(optimizer, checkpoint)
+class LowLevelZeroCheckpointIO(TorchDDPCheckpointIO):
 
-    def save_lr_scheduler(self, lr_scheduler: LRScheduler, checkpoint: str):
-        """
-        Save model to checkpoint but only on master process.
+    def save_unsharded_optimizer(self, optimizer: OptimizerWrapper, checkpoint: str, gather_dtensor: bool = False):
+        """Save optimizer to checkpoint but only on master process.
+
+        Args:
+            optimizer (OptimizerWrapper): Optimizer to save state_dict
+            checkpoint (str): Path to save checkpoint
+            gather_dtensor (bool): Whether to gather_dtensor, not used
         """
+
+        # the `state_dict` in LowLevelZeroOptimizer has communication
+        # if only the master rank collect state_dict and save,
+        # the communication on each rank would not match
+        state_dict = optimizer.state_dict()
         if self.coordinator.is_master():
-            super().save_lr_scheduler(lr_scheduler, checkpoint)
+            save_state_dict(state_dict, checkpoint, use_safetensors=False)
 
-    def save_sharded_model(self,
-                           model: GeminiDDP,
-                           checkpoint_path: str,
-                           gather_dtensor: bool = False,
-                           variant: Optional[str] = None,
-                           max_shard_size: int = 1024,
-                           use_safetensors: bool = False):
-        """
-        Save sharded model
-        """
-        state_dict_shard = model.state_dict_shard(max_shard_size=max_shard_size, only_rank_0=True, dtype=torch.float32)
-        weights_name, save_index_file = get_base_filenames(variant, use_safetensors)
-        total_size = 0
-        index_file = CheckpointIndexFile(checkpoint_path)
-        for idx, shard_pair in enumerate(state_dict_shard):
-            if not self.coordinator.is_master():
-                continue
-            shard = shard_pair[0]
-            shard_file = get_shard_filename(weights_name, idx)
-            total_size = total_size + shard_pair[1]
-            for key in shard.keys():
-                index_file.append_weight_map(key, shard_file)
+    def save_sharded_optimizer(self,
+                               optimizer: OptimizerWrapper,
+                               checkpoint: str,
+                               gather_dtensor: bool = False,
+                               prefix: str = None,
+                               size_per_shard: int = 1024):
+        """
+        Save sharded Zero-optimizer checkpoint under the given checkpointing path.
+        The following files will be created under the path:
+        - An index file (pytorch_optim.bin.index.json) containing a map between optimizer states and file names
+        - A group file (pytorch_optim_group.bin) recording information of param_groups
+        - Multiple files (pytorch_optim-000XX.bin) that store state tensors of optimizer in a sharding way
+
+        Args:
+            optimizer (OptimizerWrapper): Optimizer to save sharded state_dict
+            checkpoint (str): Path to save optimizer state_dict
+            gather_dtensor (bool): Whether to gather_dtensor, not used
+            prefix (str): Perfix of file to save
+            size_per_shard (int): Max file size of each file that store state tensors
+        """
+        if os.path.isfile(checkpoint):
+            logging.error(f"Provided path ({checkpoint}) should be a directory, not a file")
+            return
+
+        Path(checkpoint).mkdir(parents=True, exist_ok=True)
+
+        # state_dict only provide only 'param_groups'
+        state_dict = optimizer.optim.state_dict()
+        # state shard would be handled by the low-level zero optimizer
+        sharded_state = optimizer.state_dict_shard(max_shard_size=size_per_shard)
+
+        # Preparing file paths and index file.
+        states_name, save_index_file, param_group_file = get_optimizer_base_filenames(prefix)
+        index_file = CheckpointIndexFile(checkpoint)
+
+        # Store the information of param groups to param_group_file.
+        index_file.append_meta_data("param_groups", param_group_file)
+        group_file_path = os.path.join(checkpoint, param_group_file)
+        save_param_groups(state_dict, group_file_path)
 
-            checkpoint_file_path = os.path.join(checkpoint_path, shard_file)
-            save_state_dict(shard, checkpoint_file_path, use_safetensors)
+        # Save shards of optimizer states.
+        total_size = 0
+        for idx, shard_pair in enumerate(sharded_state):
+            shard, current_size = shard_pair
+            shard_file = get_shard_filename(states_name, idx)
+            total_size = total_size + current_size
+            for param_id in shard.keys():
+                index_file.append_weight_map(str(param_id), shard_file)
+
+            checkpoint_file_path = os.path.join(checkpoint, shard_file)
+            if self.coordinator.is_master():
+                save_state_dict(shard, checkpoint_file_path, use_safetensors=False)
 
+        # Wrap up index file.
         index_file.append_meta_data("total_size", total_size)
-        index_file.write_index_file(save_index_file)
-        logging.info(f"The model is going to be split to checkpoint shards. "
+        if self.coordinator.is_master():
+            index_file.write_index_file(save_index_file)
+        logging.info(f"The optimizer is going to be split to checkpoint shards. "
                      f"You can find where each parameters has been saved in the "
                      f"index located at {save_index_file}.")
 
-    def load_sharded_model(self,
-                           model: GeminiDDP,
-                           checkpoint_index_file: Path,
-                           strict: bool = False,
-                           use_safetensors: bool = False):
-        """
-        load shard model, load model from multiple files
-        """
-        return super().load_sharded_model(model, checkpoint_index_file, strict, use_safetensors, load_sub_module=False)
-
+    def load_sharded_optimizer(self, optimizer: OptimizerWrapper, index_file_path: str, prefix: str):
+        """Load sharded optimizer with the given path to index file.
 
-class GeminiModel(ModelWrapper):
+        Args:
+            optimizer (OptimizerWrapper): Optimizer to load state_dict
+            index_file_path (str): Path to the index file
+            prefix (str): Not used.
+        """
+        super().load_sharded_optimizer(optimizer, index_file_path, prefix)
+        current_rank_state_dict = optimizer.optim.state_dict()['state']
+        for param_idx, state in current_rank_state_dict.items():
+            for k, v in state.items():
+                if isinstance(v, torch.Tensor) and k != 'step':
+                    padding_size = (self.coordinator.world_size -
+                                    v.numel() % self.coordinator.world_size) % self.coordinator.world_size
+                    with torch.no_grad():
+                        v = v.flatten()
+                        if padding_size > 0:
+                            v = torch.nn.functional.pad(v, [0, padding_size])
+                        v_list = v.split(v.numel() // self.coordinator.world_size)
+                        current_rank_state_dict[param_idx][k] = v_list[self.coordinator.rank].detach()
 
-    def __init__(self, module: nn.Module, gemini_config: dict, verbose: bool = False) -> None:
-        super().__init__(module)
-        self.module = zero_model_wrapper(module, zero_stage=3, gemini_config=gemini_config, verbose=verbose)
 
-    def unwrap(self):
-        # as save/load state dict is coupled with the GeminiDDP, we only return GeminiDDP model
-        return self.module
-
-
-class GeminiOptimizer(OptimizerWrapper):
-
-    def __init__(self,
-                 module: GeminiDDP,
-                 optimizer: Optimizer,
-                 zero_optim_config: dict,
-                 optim_kwargs: dict,
-                 verbose: bool = False) -> None:
-        optimizer = zero_optim_wrapper(module,
-                                       optimizer,
-                                       optim_config=zero_optim_config,
-                                       **optim_kwargs,
-                                       verbose=verbose)
-        super().__init__(optimizer)
-
-    def backward(self, loss: Tensor, *args, **kwargs):
-        self.optim.backward(loss)
-
-    def clip_grad_by_norm(self,
-                          max_norm: Union[float, int],
-                          norm_type: Union[float, int] = 2,
-                          error_if_nonfinite: bool = False,
-                          *args,
-                          **kwargs) -> Tensor:
-        warnings.warn(f'Gemini controls grad clipping by itself, so you should not use clip_grad_by_norm')
+class LowLevelZeroModel(ModelWrapper):
 
-    def clip_grad_by_value(self, clip_value: float, *args, **kwargs) -> None:
-        raise NotImplementedError('Gemini does not support clip_grad_by_value')
+    def __init__(self, module: nn.Module, stage: int, precision: str) -> None:
+        super().__init__(module)
+        self.dtype = None
+        if precision == 'fp16':
+            self.dtype = torch.float16
+        elif precision == 'bf16':
+            self.dtype = torch.bfloat16
+        module = zero_model_wrapper(module, zero_stage=stage)
+        if self.dtype is not None:
+            module = module.to(self.dtype)
+        module = module.to(get_current_device())
+        self.module = module
+        self.convert_fn = None
+        if self.dtype is not None:
+            self.convert_fn = partial(_convert_floating_point, dtype=self.dtype)
+
+    def forward(self, *args, **kwargs):
+        if self.convert_fn is not None:
+            args = tree_map(self.convert_fn, args)
+            kwargs = tree_map(self.convert_fn, kwargs)
+        return super().forward(*args, **kwargs)
 
 
-class GeminiPlugin(DPPluginBase):
+class LowLevelZeroPlugin(DPPluginBase):
     """
-    Plugin for Gemini.
+    Plugin for low level zero.
 
     Example:
         >>> from colossalai.booster import Booster
-        >>> from colossalai.booster.plugin import GeminiPlugin
+        >>> from colossalai.booster.plugin import LowLevelZeroPlugin
         >>>
         >>> model, train_dataset, optimizer, criterion = ...
-        >>> plugin = GeminiPlugin()
+        >>> plugin = LowLevelZeroPlugin()
 
         >>> train_dataloader = plugin.prepare_dataloader(train_dataset, batch_size=8)
         >>> booster = Booster(plugin=plugin)
         >>> model, optimizer, train_dataloader, criterion = booster.boost(model, optimizer, train_dataloader, criterion)
 
     Args:
-        device (torch.device): device to place the model.
-        placement_policy (str, optional): "cpu", "cuda", "auto". Defaults to "cpu".
-        pin_memory (bool, optional): use pin memory on CPU. Defaults to False.
-        force_outputs_fp32 (bool, optional): force outputs are fp32. Defaults to False.
-        strict_ddp_mode (bool, optional): use strict ddp mode (only use dp without other parallelism). Defaults to False.
-        search_range_mb (int, optional): chunk size searching range in MegaByte. Defaults to 32.
-        hidden_dim (int, optional): the hidden dimension of DNN.
-            Users can provide this argument to speed up searching.
-            If users do not know this argument before training, it is ok. We will use a default value 1024.
-        min_chunk_size_mb (float, optional): the minimum chunk size in MegaByte.
-            If the aggregate size of parameters is still smaller than the minimum chunk size,
-            all parameters will be compacted into one small chunk.
-        memstats (MemStats, optional) the memory statistics collector by a runtime memory tracer.
-        gpu_margin_mem_ratio (float, optional): The ratio of GPU remaining memory (after the first forward-backward)
-            which will be used when using hybrid CPU optimizer.
-            This argument is meaningless when `placement_policy` of `GeminiManager` is not "auto".
-            Defaults to 0.0.
+        strage (int, optional): ZeRO stage. Defaults to 1.
+        precision (str, optional): precision. Support 'fp16', 'bf16' and 'fp32'. Defaults to 'fp16'.
         initial_scale (float, optional): Initial scale used by DynamicGradScaler. Defaults to 2**32.
         min_scale (float, optional): Min scale used by DynamicGradScaler. Defaults to 1.
         growth_factor (float, optional): growth_factor used by DynamicGradScaler. Defaults to 2.
         backoff_factor (float, optional): backoff_factor used by DynamicGradScaler. Defaults to 0.5.
         growth_interval (float, optional): growth_interval used by DynamicGradScaler. Defaults to 1000.
         hysteresis (float, optional): hysteresis used by DynamicGradScaler. Defaults to 2.
         max_scale (int, optional): max_scale used by DynamicGradScaler. Defaults to 2**32.
         max_norm (float, optional): max_norm used for `clip_grad_norm`. You should notice that you shall not do
             clip_grad_norm by yourself when using ZeRO DDP. The ZeRO optimizer will take care of clip_grad_norm.
         norm_type (float, optional): norm_type used for `clip_grad_norm`.
-        verbose (bool, optional): verbose mode. Debug info including chunk search result will be printed. Defaults to False.
+        reduce_bucket_size_in_m (int, optional): grad reduce bucket size in M. Defaults to 12.
+        communication_dtype (torch.dtype, optional): communication dtype. If not specified, the dtype of param will be used. Defaults to None.
+        overlap_communication (bool, optional): whether to overlap communication and computation. Defaults to True.
+        cpu_offload (bool, optional): whether to offload grad, master weight and optimizer state to cpu. Defaults to False.
+        verbose (bool, optional): verbose mode. Debug info including grad overflow will be printed. Defaults to False.
     """
 
     def __init__(
         self,
-        device: Optional[torch.device] = None,
-        placement_policy: str = "cpu",
-        pin_memory: bool = False,
-        force_outputs_fp32: bool = False,
-        strict_ddp_mode: bool = False,
-        search_range_mb: int = 32,
-        hidden_dim: Optional[int] = None,
-        min_chunk_size_mb: float = 32,
-        memstats: Optional[MemStats] = None,
-        gpu_margin_mem_ratio: float = 0.0,
+        stage: int = 1,
+        precision: str = 'fp16',
         initial_scale: float = 2**32,
         min_scale: float = 1,
         growth_factor: float = 2,
         backoff_factor: float = 0.5,
         growth_interval: int = 1000,
         hysteresis: int = 2,
         max_scale: float = 2**32,
         max_norm: float = 0.0,
         norm_type: float = 2.0,
+        reduce_bucket_size_in_m: int = 12,
+        communication_dtype: Optional[torch.dtype] = None,
+        overlap_communication: bool = True,
+        cpu_offload: bool = False,
         verbose: bool = False,
     ) -> None:
         super().__init__()
-        self.gemini_config = dict(
-            device=(device or get_current_device()),
-            placement_policy=placement_policy,
-            pin_memory=pin_memory,
-            force_outputs_fp32=force_outputs_fp32,
-            strict_ddp_mode=strict_ddp_mode,
-            search_range_mb=search_range_mb,
-            hidden_dim=hidden_dim,
-            min_chunk_size_mb=min_chunk_size_mb,
-            memstats=memstats,
-        )
-        self.zero_optim_config = dict(gpu_margin_mem_ratio=gpu_margin_mem_ratio,)
+        assert stage in (1, 2), f'LowLevelZeroPlugin only supports stage 1/2 training'
+        assert precision in SUPPORTED_PRECISION, f'LowLevelZeroPlugin only supports {SUPPORTED_PRECISION} training'
+
+        self.stage = stage
+        self.precision = precision
+        self.zero_optim_config = dict(reduce_bucket_size=reduce_bucket_size_in_m * 1024 * 1024,
+                                      communication_dtype=communication_dtype,
+                                      overlap_communication=overlap_communication,
+                                      cpu_offload=cpu_offload)
         self.optim_kwargs = dict(initial_scale=initial_scale,
                                  growth_factor=growth_factor,
                                  backoff_factor=backoff_factor,
                                  growth_interval=growth_interval,
                                  hysteresis=hysteresis,
                                  min_scale=min_scale,
                                  max_scale=max_scale,
                                  max_norm=max_norm,
                                  norm_type=norm_type)
         self.verbose = verbose
 
+        # set class name with stage, for better error message
+        setattr(self.__class__, "__name__", f"LowLevelZeroPlugin_ZeRO-{stage}")
+
     def support_no_sync(self) -> bool:
-        return False
+        return self.stage == 1
 
     def control_precision(self) -> bool:
         return True
 
     def supported_precisions(self) -> List[str]:
-        return ['fp16']
+        return SUPPORTED_PRECISION
 
     def control_device(self) -> bool:
         return True
 
     def supported_devices(self) -> List[str]:
         return ['cuda']
 
     def configure(
         self,
         model: nn.Module,
-        optimizer: Optimizer,
-        criterion: Callable = None,
-        dataloader: DataLoader = None,
-        lr_scheduler: LRScheduler = None,
-    ) -> Tuple[Union[nn.Module, OptimizerWrapper, LRScheduler, DataLoader]]:
+        optimizer: Optional[Optimizer] = None,
+        criterion: Optional[Callable] = None,
+        dataloader: Optional[DataLoader] = None,
+        lr_scheduler: Optional[LRScheduler] = None,
+    ) -> Tuple[nn.Module, OptimizerWrapper, Callable, DataLoader, LRScheduler]:
 
         if not isinstance(model, ModelWrapper):
-            # convert model to sync bn
-            # FIXME(ver217): gemini does not support sync bn
-            # In torch/nn/modules/_functions.py, line 22, ``mean, invstd = torch.batch_norm_stats(input, eps)`` will get fp32 mean and invstd even though the input is fp16.
-            # This inconsistency of dtype will cause the error.
-            # We have two possible solutions:
-            # 1. keep batch norm always in fp32. This is hard for gemini, as it use chunks.
-            # 2. patch sync bn or write a new on. This is relatively easy, but we need to test it.
-            # model = nn.SyncBatchNorm.convert_sync_batchnorm(model, None)
-
-            # wrap the model with Gemini
-            model = GeminiModel(model, self.gemini_config, self.verbose)
-
-        if not isinstance(optimizer, OptimizerWrapper):
-            optimizer = GeminiOptimizer(model.unwrap(), optimizer, self.zero_optim_config, self.optim_kwargs,
-                                        self.verbose)
+            model = LowLevelZeroModel(model, self.stage, self.precision)
+
+        if optimizer is not None and \
+                not isinstance(optimizer, OptimizerWrapper):
+            optimizer = zero_optim_wrapper(model.unwrap(),
+                                           optimizer,
+                                           optim_config=self.zero_optim_config,
+                                           **self.optim_kwargs,
+                                           verbose=self.verbose)
 
         return model, optimizer, criterion, dataloader, lr_scheduler
 
     def control_checkpoint_io(self) -> bool:
         return True
 
     def get_checkpoint_io(self) -> CheckpointIO:
-        return GeminiCheckpointIO()
+        return LowLevelZeroCheckpointIO()
 
-    def no_sync(self, model: nn.Module) -> Iterator[None]:
-        raise NotImplementedError
+    def no_sync(self, model: nn.Module, optimizer: OptimizerWrapper) -> Iterator[None]:
+        assert isinstance(optimizer, LowLevelZeroOptimizer)
+        return optimizer.optim.no_sync()
```

### Comparing `colossalai-0.3.0/colossalai/booster/plugin/low_level_zero_plugin.py` & `colossalai-0.3.1/colossalai/nn/init.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,211 +1,252 @@
+import math
 import warnings
-from typing import Callable, Iterator, List, Optional, Tuple, Union
 
-import torch
-import torch.nn as nn
 from torch import Tensor
-from torch.optim import Optimizer
-from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
-from torch.utils._pytree import tree_map
-from torch.utils.data import DataLoader
-
-from colossalai.checkpoint_io import CheckpointIO, GeneralCheckpointIO
-from colossalai.interface import ModelWrapper, OptimizerWrapper
-from colossalai.utils import get_current_device
-from colossalai.zero import zero_model_wrapper, zero_optim_wrapper
-
-from .dp_plugin_base import DPPluginBase
-from .torch_ddp_plugin import TorchDDPCheckpointIO
-
-__all__ = ['LowLevelZeroPlugin']
-
-
-def _convert_to_fp16(x):
-    if isinstance(x, torch.Tensor) and torch.is_floating_point(x):
-        return x.half()
-    return x
-
-
-class LowLevelZeroCheckpointIO(TorchDDPCheckpointIO):
-
-    def save_unsharded_optimizer(self, optimizer: Optimizer, checkpoint: str, gather_dtensor: bool):
-        """
-        Save optimizer to checkpoint but only on master process.
-        """
-        # TODO(ver217): optimizer state dict is sharded, and cannot get full state dict now
-        warnings.warn(
-            'LowLevelZeroPlugin does not support save full optimizer checkpoint now. Save it on every process.')
-        checkpoint = f'{checkpoint}.rank{self.coordinator.rank}'
-        GeneralCheckpointIO.save_unsharded_optimizer(self, optimizer, checkpoint, gather_dtensor)
-
-    def load_optimizer(self, optimizer: Optimizer, checkpoint: str):
-        warnings.warn(
-            'LowLevelZeroPlugin can only load optimizer checkpoint saved by itself with the same number of processes.')
-        checkpoint = f'{checkpoint}.rank{self.coordinator.rank}'
-        super().load_optimizer(optimizer, checkpoint)
-
-
-class LowLevelZeroModel(ModelWrapper):
-
-    def __init__(self, module: nn.Module, stage: int, precision: str) -> None:
-        super().__init__(module)
-        self.convert_inputs = (precision == 'fp16')
-        module = zero_model_wrapper(module, zero_stage=stage)
-        if precision == 'fp16':
-            module = module.half()
-        module = module.to(get_current_device())
-        self.module = module
-
-    def forward(self, *args, **kwargs):
-        if self.convert_inputs:
-            args = tree_map(_convert_to_fp16, args)
-            kwargs = tree_map(_convert_to_fp16, kwargs)
-        return super().forward(*args, **kwargs)
-
-
-class LowLevelZeroOptimizer(OptimizerWrapper):
-
-    def __init__(self,
-                 module: nn.Module,
-                 optimizer: Optimizer,
-                 zero_optim_config: dict,
-                 optim_kwargs: dict,
-                 verbose: bool = False) -> None:
-        optimizer = zero_optim_wrapper(module,
-                                       optimizer,
-                                       optim_config=zero_optim_config,
-                                       **optim_kwargs,
-                                       verbose=verbose)
-        super().__init__(optimizer)
-
-    def backward(self, loss: Tensor, *args, **kwargs):
-        self.optim.backward(loss)
-
-    def clip_grad_by_norm(self,
-                          max_norm: Union[float, int],
-                          norm_type: Union[float, int] = 2,
-                          error_if_nonfinite: bool = False,
-                          *args,
-                          **kwargs) -> Tensor:
-        warnings.warn(f'LowLevelZero controls grad clipping by itself, so you should not use clip_grad_by_norm')
-
-    def clip_grad_by_value(self, clip_value: float, *args, **kwargs) -> None:
-        raise NotImplementedError('LowLevelZero does not support clip_grad_by_value')
-
-
-class LowLevelZeroPlugin(DPPluginBase):
-    """
-    Plugin for low level zero.
-
-    Example:
-        >>> from colossalai.booster import Booster
-        >>> from colossalai.booster.plugin import LowLevelZeroPlugin
-        >>>
-        >>> model, train_dataset, optimizer, criterion = ...
-        >>> plugin = LowLevelZeroPlugin()
-
-        >>> train_dataloader = plugin.prepare_dataloader(train_dataset, batch_size=8)
-        >>> booster = Booster(plugin=plugin)
-        >>> model, optimizer, train_dataloader, criterion = booster.boost(model, optimizer, train_dataloader, criterion)
-
-    Args:
-        strage (int, optional): ZeRO stage. Defaults to 1.
-        precision (str, optional): precision. Support 'fp16' and 'fp32'. Defaults to 'fp16'.
-        initial_scale (float, optional): Initial scale used by DynamicGradScaler. Defaults to 2**32.
-        min_scale (float, optional): Min scale used by DynamicGradScaler. Defaults to 1.
-        growth_factor (float, optional): growth_factor used by DynamicGradScaler. Defaults to 2.
-        backoff_factor (float, optional): backoff_factor used by DynamicGradScaler. Defaults to 0.5.
-        growth_interval (float, optional): growth_interval used by DynamicGradScaler. Defaults to 1000.
-        hysteresis (float, optional): hysteresis used by DynamicGradScaler. Defaults to 2.
-        max_scale (int, optional): max_scale used by DynamicGradScaler. Defaults to 2**32.
-        max_norm (float, optional): max_norm used for `clip_grad_norm`. You should notice that you shall not do
-            clip_grad_norm by yourself when using ZeRO DDP. The ZeRO optimizer will take care of clip_grad_norm.
-        norm_type (float, optional): norm_type used for `clip_grad_norm`.
-        reduce_bucket_size_in_m (int, optional): grad reduce bucket size in M. Defaults to 12.
-        communication_dtype (torch.dtype, optional): communication dtype. If not specified, the dtype of param will be used. Defaults to None.
-        overlap_communication (bool, optional): whether to overlap communication and computation. Defaults to True.
-        cpu_offload (bool, optional): whether to offload grad, master weight and optimizer state to cpu. Defaults to False.
-        verbose (bool, optional): verbose mode. Debug info including grad overflow will be printed. Defaults to False.
-    """
-
-    def __init__(
-        self,
-        stage: int = 1,
-        precision: str = 'fp16',
-        initial_scale: float = 2**32,
-        min_scale: float = 1,
-        growth_factor: float = 2,
-        backoff_factor: float = 0.5,
-        growth_interval: int = 1000,
-        hysteresis: int = 2,
-        max_scale: float = 2**32,
-        max_norm: float = 0.0,
-        norm_type: float = 2.0,
-        reduce_bucket_size_in_m: int = 12,
-        communication_dtype: Optional[torch.dtype] = None,
-        overlap_communication: bool = True,
-        cpu_offload: bool = False,
-        verbose: bool = False,
-    ) -> None:
-        super().__init__()
-        assert stage in (1, 2), f'LowLevelZeroPlugin only supports stage 1/2 training'
-        assert precision in ('fp16', 'fp32'), f'LowLevelZeroPlugin only supports fp16/fp32 training'
-
-        self.stage = stage
-        self.precision = precision
-        self.zero_optim_config = dict(reduce_bucket_size=reduce_bucket_size_in_m * 1024 * 1024,
-                                      communication_dtype=communication_dtype,
-                                      overlap_communication=overlap_communication,
-                                      cpu_offload=cpu_offload)
-        self.optim_kwargs = dict(initial_scale=initial_scale,
-                                 growth_factor=growth_factor,
-                                 backoff_factor=backoff_factor,
-                                 growth_interval=growth_interval,
-                                 hysteresis=hysteresis,
-                                 min_scale=min_scale,
-                                 max_scale=max_scale,
-                                 max_norm=max_norm,
-                                 norm_type=norm_type)
-        self.verbose = verbose
-
-    def support_no_sync(self) -> bool:
-        return False
-
-    def control_precision(self) -> bool:
-        return True
-
-    def supported_precisions(self) -> List[str]:
-        return ['fp16', 'fp32']
-
-    def control_device(self) -> bool:
-        return True
-
-    def supported_devices(self) -> List[str]:
-        return ['cuda']
-
-    def configure(
-        self,
-        model: nn.Module,
-        optimizer: Optimizer,
-        criterion: Callable = None,
-        dataloader: DataLoader = None,
-        lr_scheduler: LRScheduler = None,
-    ) -> Tuple[Union[nn.Module, OptimizerWrapper, LRScheduler, DataLoader]]:
-
-        if not isinstance(model, ModelWrapper):
-            model = LowLevelZeroModel(model, self.stage, self.precision)
-
-        if not isinstance(optimizer, OptimizerWrapper):
-            optimizer = LowLevelZeroOptimizer(model.unwrap(), optimizer, self.zero_optim_config, self.optim_kwargs,
-                                              self.verbose)
-
-        return model, optimizer, criterion, dataloader, lr_scheduler
+import torch.nn as nn
+
+
+def zeros_():
+    """Return the initializer filling the input Tensor with the scalar zeros"""
+
+    def initializer(tensor: Tensor, fan_in: int = None, fan_out: int = None):
+        return nn.init.zeros_(tensor)
+
+    return initializer
+
+
+def ones_():
+    """Return the initializer filling the input Tensor with the scalar ones"""
+
+    def initializer(tensor: Tensor, fan_in: int = None, fan_out: int = None):
+        return nn.init.ones_(tensor)
+
+    return initializer
+
+
+def uniform_(a: float = 0., b: float = 1.):
+    r"""Return the initializer filling the input Tensor with values drawn from the uniform
+    distribution :math:`\mathcal{U}(a, b)`.
+
+    Args:
+        a (float): the lower bound of the uniform distribution. Defaults 0.0.
+        b (float): the upper bound of the uniform distribution. Defaults 1.0.
+    """
+
+    def initializer(tensor: Tensor, fan_in: int = None, fan_out: int = None):
+        return nn.init.uniform_(tensor, a, b)
+
+    return initializer
+
+
+def normal_(mean: float = 0., std: float = 1.):
+    r"""Return the initializer filling the input Tensor with values drawn from the normal distribution
+
+     .. math::
+        \mathcal{N}(\text{mean}, \text{std}^2)
+
+    Args:
+        mean (float): the mean of the normal distribution. Defaults 0.0.
+        std (float): the standard deviation of the normal distribution. Defaults 1.0.
+     """
+
+    def initializer(tensor: Tensor, fan_in: int = None, fan_out: int = None):
+        return nn.init.normal_(tensor, mean, std)
+
+    return initializer
+
+
+def trunc_normal_(mean: float = 0., std: float = 1., a: float = -2., b: float = 2.):
+    r"""Return the initializer filling the input Tensor with values drawn from a truncated
+    normal distribution. The values are effectively drawn from the
+    normal distribution :math:`\mathcal{N}(\text{mean}, \text{std}^2)`
+    with values outside :math:`[a, b]` redrawn until they are within
+    the bounds. The method used for generating the random values works
+    best when :math:`a \leq \text{mean} \leq b`.
+
+    Args:
+        mean (float): the mean of the normal distribution. Defaults 0.0.
+        std (float): the standard deviation of the normal distribution. Defaults 1.0.
+        a (float): the minimum cutoff value. Defaults -2.0.
+        b (float): the maximum cutoff value. Defaults 2.0.
+    """
+
+    def initializer(tensor: Tensor, fan_in: int = None, fan_out: int = None):
+        return nn.init.trunc_normal_(tensor, mean, std, a, b)
+
+    return initializer
+
+
+def kaiming_uniform_(a=0, mode='fan_in', nonlinearity='leaky_relu'):
+    r"""Return the initializer filling the input `Tensor` with values according to the method
+    described in `Delving deep into rectifiers: Surpassing human-level
+    performance on ImageNet classification` - He, K. et al. (2015), using a
+    uniform distribution. The resulting tensor will have values sampled from
+    :math:`\mathcal{U}(-\text{bound}, \text{bound})` where
+
+    .. math::
+        \text{bound} = \text{gain} \times \sqrt{\frac{3}{\text{fan_mode}}}
+
+    Also known as 'He initialization'.
+
+    Args:
+        a (int): the negative slope of the rectifier used after this layer (only used with ``'leaky_relu'``).
+        mode (str, optional): either ``'fan_in'`` (default) or ``'fan_out'``. Choosing ``'fan_in'``
+                preserves the magnitude of the variance of the weights in the
+                forward pass. Choosing ``'fan_out'`` preserves the magnitudes in the
+                backwards pass.
+        nonlinearity (str, optional): the non-linear function (`nn.functional` name),
+                        recommended to use only with ``'relu'`` or ``'leaky_relu'`` (default).
+    """
+
+    # adapted from torch.nn.init
+    def initializer(tensor: Tensor, fan_in: int = None, fan_out: int = None):
+        if 0 in tensor.shape:
+            warnings.warn("Initializing zero-element tensors is a no-op")
+            return tensor
+
+        if mode == 'fan_in':
+            assert fan_in is not None, 'Fan_in is not provided.'
+            fan = fan_in
+        elif mode == 'fan_out':
+            assert fan_out is not None, 'Fan_out is not provided.'
+            fan = fan_out
+        else:
+            raise ValueError(f'Invalid initialization mode \'{mode}\'')
+
+        std = nn.init.calculate_gain(nonlinearity, a) / math.sqrt(fan)
+        bound = math.sqrt(3.) * std
+        return nn.init.uniform_(tensor, -bound, bound)
+
+    return initializer
+
+
+def kaiming_normal_(a=0, mode='fan_in', nonlinearity='leaky_relu'):
+    r"""Return the initializer filling the input `Tensor` with values according to the method
+    described in `Delving deep into rectifiers: Surpassing human-level
+    performance on ImageNet classification` - He, K. et al. (2015), using a
+    normal distribution. The resulting tensor will have values sampled from
+    :math:`\mathcal{N}(0, \text{std}^2)` where
+
+    .. math::
+        \text{std} = \frac{\text{gain}}{\sqrt{\text{fan_mode}}}
+
+    Also known as 'He initialization'.
+
+    Args:
+        a (int): the negative slope of the rectifier used after this layer (only used with ``'leaky_relu'``).
+        mode (str, optional): either ``'fan_in'`` (default) or ``'fan_out'``. Choosing ``'fan_in'``
+                preserves the magnitude of the variance of the weights in the
+                forward pass. Choosing ``'fan_out'`` preserves the magnitudes in the
+                backwards pass.
+        nonlinearity (str, optional): the non-linear function (`nn.functional` name),
+                        recommended to use only with ``'relu'`` or ``'leaky_relu'`` (default).
+    """
+
+    # adapted from torch.nn.init
+    def initializer(tensor: Tensor, fan_in: int = None, fan_out: int = None):
+        if 0 in tensor.shape:
+            warnings.warn("Initializing zero-element tensors is a no-op")
+            return tensor
+
+        if mode == 'fan_in':
+            assert fan_in is not None, 'Fan_in is not provided.'
+            fan = fan_in
+        elif mode == 'fan_out':
+            assert fan_out is not None, 'Fan_out is not provided.'
+            fan = fan_out
+        else:
+            raise ValueError(f'Invalid initialization mode \'{mode}\'')
+
+        std = nn.init.calculate_gain(nonlinearity, a) / math.sqrt(fan)
+        return nn.init.normal_(tensor, 0, std)
+
+    return initializer
+
+
+def xavier_uniform_(a: float = math.sqrt(3.), scale: float = 2., gain: float = 1.):
+    r"""Return the initializer filling the input `Tensor` with values according to the method
+    described in `Understanding the difficulty of training deep feedforward
+    neural networks` - Glorot, X. & Bengio, Y. (2010), using a uniform
+    distribution. The resulting tensor will have values sampled from
+    :math:`\mathcal{U}(-a, a)` where
+
+    .. math::
+        a = \text{gain} \times \sqrt{\frac{6}{\text{fan_in} + \text{fan_out}}}
+
+    Also known as 'Glorot initialization'.
+
+    Args:
+        a (float, optional): an optional scaling factor used to calculate uniform
+            bounds from standard deviation. Defaults ``math.sqrt(3.)``.
+        scale (float, optional): an optional scaling factor used to calculate standard deviation. Defaults 2.0.
+        gain (float, optional): an optional scaling factor. Defaults 1.0.
+    """
+
+    # adapted from torch.nn.init
+    def initializer(tensor: Tensor, fan_in: int = None, fan_out: int = None):
+        assert fan_in is not None, 'Fan_in is not provided.'
+
+        fan = fan_in
+        if fan_out is not None:
+            fan += fan_out
+
+        std = gain * math.sqrt(scale / float(fan))
+        bound = a * std
+        return nn.init.uniform_(tensor, -bound, bound)
+
+    return initializer
+
+
+def xavier_normal_(scale: float = 2., gain: float = 1.):
+    r"""Return the initializer filling the input `Tensor` with values according to the method
+    described in `Understanding the difficulty of training deep feedforward
+    neural networks` - Glorot, X. & Bengio, Y. (2010), using a normal
+    distribution. The resulting tensor will have values sampled from
+    :math:`\mathcal{N}(0, \text{std}^2)` where
+
+    .. math::
+        \text{std} = \text{gain} \times \sqrt{\frac{2}{\text{fan_in} + \text{fan_out}}}
+
+    Also known as 'Glorot initialization'.
+
+    Args:
+        scale (float, optional): an optional scaling factor used to calculate standard deviation. Defaults 2.0.
+        gain (float, optional): an optional scaling factor. Defaults 1.0.
+    """
+
+    # adapted from torch.nn.init
+    def initializer(tensor: Tensor, fan_in: int = None, fan_out: int = None):
+        assert fan_in is not None, 'Fan_in is not provided.'
+
+        fan = fan_in
+        if fan_out is not None:
+            fan += fan_out
+
+        std = gain * math.sqrt(scale / float(fan))
+
+        return nn.init.normal_(tensor, 0., std)
+
+    return initializer
+
+
+def lecun_uniform_():
+    # adapted from jax.nn.initializers
+    def initializer(tensor: Tensor, fan_in: int = None, fan_out: int = None):
+        assert fan_in is not None, 'Fan_in is not provided.'
+
+        var = 1.0 / fan_in
+        bound = math.sqrt(3 * var)
+        return nn.init.uniform_(tensor, -bound, bound)
+
+    return initializer
+
 
-    def control_checkpoint_io(self) -> bool:
-        return True
+def lecun_normal_():
+    # adapted from jax.nn.initializers
+    def initializer(tensor: Tensor, fan_in: int = None, fan_out: int = None):
+        assert fan_in is not None, 'Fan_in is not provided.'
 
-    def get_checkpoint_io(self) -> CheckpointIO:
-        return LowLevelZeroCheckpointIO()
+        std = math.sqrt(1.0 / fan_in)
+        return nn.init.trunc_normal_(tensor, std=std / .87962566103423978)
 
-    def no_sync(self, model: nn.Module) -> Iterator[None]:
-        raise NotImplementedError
+    return initializer
```

### Comparing `colossalai-0.3.0/colossalai/booster/plugin/plugin_base.py` & `colossalai-0.3.1/colossalai/booster/plugin/plugin_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import Callable, Iterator, List, Tuple, Union
+from typing import Callable, Iterator, List, Optional, Tuple, Union
 
 import torch.nn as nn
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
 from torch.utils.data import DataLoader, Dataset
 
 from colossalai.checkpoint_io import CheckpointIO
@@ -34,19 +34,19 @@
     def support_no_sync(self) -> bool:
         pass
 
     @abstractmethod
     def configure(
         self,
         model: nn.Module,
-        optimizer: Optimizer,
-        criterion: Callable = None,
-        dataloader: DataLoader = None,
-        lr_scheduler: LRScheduler = None,
-    ) -> Tuple[Union[nn.Module, OptimizerWrapper, LRScheduler, DataLoader]]:
+        optimizer: Optional[Optimizer] = None,
+        criterion: Optional[Callable] = None,
+        dataloader: Optional[DataLoader] = None,
+        lr_scheduler: Optional[LRScheduler] = None,
+    ) -> Tuple[nn.Module, OptimizerWrapper, Callable, DataLoader, LRScheduler]:
         # implement this method
         pass
 
     @abstractmethod
     def control_checkpoint_io(self) -> bool:
         """
         Whether the plugin controls the checkpoint io
@@ -57,15 +57,15 @@
     def get_checkpoint_io(self) -> CheckpointIO:
         """
         Get checkpoint io object for this plugin, only invoked when control_checkpoint_io is True.
         """
         pass
 
     @abstractmethod
-    def no_sync(self, model: nn.Module) -> Iterator[None]:
+    def no_sync(self, model: nn.Module, optimizer: OptimizerWrapper) -> Iterator[None]:
         """
         Context manager to disable gradient synchronization.
         """
         pass
 
     @abstractmethod
     def prepare_dataloader(self,
```

### Comparing `colossalai-0.3.0/colossalai/booster/plugin/torch_ddp_plugin.py` & `colossalai-0.3.1/colossalai/booster/plugin/torch_ddp_plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,14 @@
         # the model should be unwrapped in self.load_model via ModelWrapper.unwrap
         return super().load_unsharded_model(model, checkpoint, strict=strict)
 
     def save_unsharded_model(self, model: nn.Module, checkpoint: str, gather_dtensor: bool, use_safetensors: bool):
         """
         Save model to checkpoint but only on master process.
         """
-        # the model should be unwrapped in self.load_model via ModelWrapper.unwrap
         if self.coordinator.is_master():
             super().save_unsharded_model(model, checkpoint, gather_dtensor, use_safetensors)
 
     def save_unsharded_optimizer(self, optimizer: Optimizer, checkpoint: str, gather_dtensor: bool):
         """
         Save optimizer to checkpoint but only on master process.
         """
@@ -49,20 +48,35 @@
         """
         if self.coordinator.is_master():
             super().save_lr_scheduler(lr_scheduler, checkpoint)
 
     def save_sharded_model(self,
                            model: nn.Module,
                            checkpoint_path: str,
-                           gather_dtensor: bool = False,
-                           variant: Optional[str] = None,
+                           gather_dtensor: bool = True,
+                           prefix: Optional[str] = None,
                            max_shard_size: int = 1024,
                            use_safetensors: bool = False):
+        """
+        Save model to checkpoint but only on master process.
+        """
+        if self.coordinator.is_master():
+            super().save_sharded_model(model, checkpoint_path, gather_dtensor, prefix, max_shard_size, use_safetensors)
+
+    def save_sharded_optimizer(self,
+                               optimizer: Optimizer,
+                               checkpoint: str,
+                               gather_dtensor: bool = True,
+                               prefix: Optional[str] = None,
+                               size_per_shard: int = 1024):
+        """
+        Save optimizer to checkpoint but only on master process.
+        """
         if self.coordinator.is_master():
-            super().save_sharded_model(model, checkpoint_path, gather_dtensor, variant, max_shard_size, use_safetensors)
+            super().save_sharded_optimizer(optimizer, checkpoint, gather_dtensor, prefix, size_per_shard)
 
 
 class TorchDDPModel(ModelWrapper):
 
     def __init__(self, module: nn.Module, *args, **kwargs) -> None:
         super().__init__(module)
         self.module = DDP(module, *args, **kwargs)
@@ -124,35 +138,36 @@
 
     def supported_devices(self) -> List[str]:
         return ['cuda']
 
     def configure(
         self,
         model: nn.Module,
-        optimizer: Optimizer,
-        criterion: Callable = None,
-        dataloader: DataLoader = None,
-        lr_scheduler: LRScheduler = None,
-    ) -> Tuple[Union[nn.Module, OptimizerWrapper, LRScheduler, DataLoader]]:
+        optimizer: Optional[Optimizer] = None,
+        criterion: Optional[Callable] = None,
+        dataloader: Optional[DataLoader] = None,
+        lr_scheduler: Optional[LRScheduler] = None,
+    ) -> Tuple[nn.Module, OptimizerWrapper, Callable, DataLoader, LRScheduler]:
         # cast model to cuda
         model = model.cuda()
 
         # convert model to sync bn
         model = nn.SyncBatchNorm.convert_sync_batchnorm(model, None)
 
         # wrap the model with PyTorch DDP
         model = TorchDDPModel(model, **self.ddp_kwargs)
 
-        if not isinstance(optimizer, OptimizerWrapper):
+        if optimizer is not None and \
+                not isinstance(optimizer, OptimizerWrapper):
             optimizer = OptimizerWrapper(optimizer)
 
         return model, optimizer, criterion, dataloader, lr_scheduler
 
     def control_checkpoint_io(self) -> bool:
         return True
 
     def get_checkpoint_io(self) -> CheckpointIO:
         return TorchDDPCheckpointIO()
 
-    def no_sync(self, model: nn.Module) -> Iterator[None]:
+    def no_sync(self, model: nn.Module, optimizer: OptimizerWrapper) -> Iterator[None]:
         assert isinstance(model, TorchDDPModel), 'Model is not boosted by TorchDDPPlugin.'
         return model.module.no_sync()
```

### Comparing `colossalai-0.3.0/colossalai/booster/plugin/torch_fsdp_plugin.py` & `colossalai-0.3.1/colossalai/booster/plugin/torch_fsdp_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+import warnings
 from pathlib import Path
 from typing import Callable, Iterable, Iterator, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
-import warnings
 from packaging import version
 from torch.distributed import ProcessGroup
 
 if version.parse(torch.__version__) >= version.parse('1.12.0'):
     from torch.distributed.fsdp import FullStateDictConfig
     from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
     from torch.distributed.fsdp import StateDictType
@@ -65,15 +65,15 @@
         Save optimizer to checkpoint but only on master process.
         """
         assert isinstance(optimizer, FSDPOptimizerWrapper)
         fsdp_model = optimizer.unwrap_model()
         full_optimizer_state = FSDP.full_optim_state_dict(fsdp_model, optim=optimizer, rank0_only=True)
         utils.save_state_dict(full_optimizer_state, checkpoint_file_path=checkpoint, use_safetensors=False)
 
-    def save_sharded_model(self, model: nn.Module, checkpoint: str, gather_dtensor: bool, variant: Optional[str],
+    def save_sharded_model(self, model: nn.Module, checkpoint: str, gather_dtensor: bool, prefix: Optional[str],
                            size_per_shard: int, use_safetensors: bool):
         """
         Save model to checkpoint but only on master process.
         """
         raise NotImplementedError("Sharded model checkpoint is not supported yet.")
 
     def load_sharded_model(self,
@@ -83,21 +83,22 @@
                            use_safetensors: bool = False,
                            load_sub_module: bool = True):
         """
         Load model to checkpoint but only on master process.
         """
         raise NotImplementedError("Sharded model checkpoint is not supported yet.")
 
-    def save_sharded_optimizer(self, optimizer: Optimizer, checkpoint: str, gather_dtensor: bool):
+    def save_sharded_optimizer(self, optimizer: Optimizer, checkpoint: str, gather_dtensor: bool, prefix: str,
+                               size_per_shard: int):
         """
         Save optimizer to checkpoint but only on master process.
         """
         raise NotImplementedError("Sharded optimizer checkpoint is not supported yet.")
 
-    def load_sharded_optimizer(self, optimizer: Optimizer, index_file_path: str, prefix: str, size_per_shard: int):
+    def load_sharded_optimizer(self, optimizer: Optimizer, index_file_path: str, size_per_shard: int):
         """
         Load optimizer to checkpoint but only on master process.
         """
         raise NotImplementedError("Sharded optimizer checkpoint is not supported yet.")
 
     def save_lr_scheduler(self, lr_scheduler: LRScheduler, checkpoint: str):
         """
@@ -172,15 +173,15 @@
                                     sync_module_states=sync_module_states)
     else:
         raise RuntimeError("FSDP is not supported while torch version under 1.12.0.")
 
     def support_no_sync(self) -> bool:
         False
 
-    def no_sync(self, model: nn.Module) -> Iterator[None]:
+    def no_sync(self, model: nn.Module, optimizer: OptimizerWrapper) -> Iterator[None]:
         raise NotImplementedError("Torch fsdp no_sync func not supported yet.")
 
     def control_precision(self) -> bool:
         return True
 
     def supported_precisions(self) -> List[str]:
         return ['fp16', 'bf16']
@@ -190,31 +191,32 @@
 
     def supported_devices(self) -> List[str]:
         return ['cuda']
 
     def configure(
         self,
         model: nn.Module,
-        optimizer: Optimizer,
-        criterion: Callable = None,
-        dataloader: DataLoader = None,
-        lr_scheduler: LRScheduler = None,
-    ) -> Tuple[Union[nn.Module, OptimizerWrapper, LRScheduler, DataLoader]]:
+        optimizer: Optional[Optimizer] = None,
+        criterion: Optional[Callable] = None,
+        dataloader: Optional[DataLoader] = None,
+        lr_scheduler: Optional[LRScheduler] = None,
+    ) -> Tuple[nn.Module, OptimizerWrapper, Callable, DataLoader, LRScheduler]:
 
         # wrap the model with PyTorch FSDP
         fsdp_model = TorchFSDPModel(model, device_id=torch.cuda.current_device(), **self.fsdp_kwargs)
 
-        if len(optimizer.param_groups) > 1:
-            warnings.warn(
-                'TorchFSDPPlugin does not support optimizer that use multi param groups. The results may not be as expected if used.'
-            )
-        optimizer.__init__(fsdp_model.parameters(), **optimizer.defaults)
+        if optimizer is not None:
+            if len(optimizer.param_groups) > 1:
+                warnings.warn(
+                    'TorchFSDPPlugin does not support optimizer that use multi param groups. The results may not be as expected if used.'
+                )
+            optimizer.__init__(fsdp_model.parameters(), **optimizer.defaults)
 
-        if not isinstance(optimizer, FSDPOptimizerWrapper):
-            optimizer = FSDPOptimizerWrapper(optimizer, fsdp_model)
+            if not isinstance(optimizer, FSDPOptimizerWrapper):
+                optimizer = FSDPOptimizerWrapper(optimizer, fsdp_model)
 
         return fsdp_model, optimizer, criterion, dataloader, lr_scheduler
 
     def control_checkpoint_io(self) -> bool:
         return True
 
     def get_checkpoint_io(self) -> CheckpointIO:
```

### Comparing `colossalai-0.3.0/colossalai/builder/builder.py` & `colossalai-0.3.1/colossalai/builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/checkpoint_io/checkpoint_io_base.py` & `colossalai-0.3.1/colossalai/checkpoint_io/checkpoint_io_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         return origin_model
 
     def save_model(self,
                    model: Union[nn.Module, ModelWrapper],
                    checkpoint: str,
                    shard: bool = False,
                    gather_dtensor: bool = True,
-                   variant: str = None,
+                   prefix: str = None,
                    size_per_shard: int = 1024,
                    use_safetensors: bool = False):
         """
         Save model to checkpoint.
 
         Examples:
             >>> from colossalai.checkpoint_io import GeneralCheckpointIO
@@ -124,44 +124,48 @@
             checkpoint (str): checkpoint path. The checkpoint path can be :
                 1. a file path, e.g. 'model.pt'
                 2. a directory path to save the sharded checkpoint, e.g. './checkpoints/' when shard = True.
             shard (bool): whether to shard the checkpoint. Default: False. If set to True, the checkpoint will be sharded into
                 multiple files. The model shards will be specified by a `model.index.json` file. When shard = True, please ensure
                 that the checkpoint path is a directory path instead of a file path.
             gather_dtensor (bool): whether to gather the distributed tensor to the first device. Default: True.
-            variant (str): If specified, weights are saved in the format pytorch_model.<variant>.bin. Default: None.
+            prefix (str): If specified, weights are saved in the format pytorch_model.<prefix>.bin. Default: None.
             size_per_shard (int): size per shard in MB. Default: 1024. This value is only used when shard = True.
             use_safetensors (bool): whether to use safe tensors. Default: False. If set to True, the checkpoint will be saved
         """
 
         if isinstance(model, ModelWrapper):
             model = model.unwrap()
 
         if shard:
-            self.save_sharded_model(model, checkpoint, gather_dtensor, variant, size_per_shard, use_safetensors)
+            self.save_sharded_model(model, checkpoint, gather_dtensor, prefix, size_per_shard, use_safetensors)
         else:
             self.save_unsharded_model(model, checkpoint, gather_dtensor, use_safetensors)
 
-    def load_optimizer(self, optimizer: Optimizer, checkpoint: str):
+    def load_optimizer(self, optimizer: Optimizer, checkpoint: str, prefix: str = None, size_per_shard: int = 1024):
         """
         Load optimizer from checkpoint.
 
         Args:
             optimizer (Optimizer): optimizer to be loaded.
             checkpoint (str): checkpoint path. This value is made compatibility with the model checkpoints in the
+            prefix (str, optional): A prefix added to parameter and buffer
+                names to compose the keys in state_dict. Defaults to None.
+            size_per_shard (int, optional): Maximum size of checkpoint shard file in MB. This is useful only when ``shard=True``. Defaults to 1024.
         """
+
         index_file_exists, index_file_path = has_index_file(checkpoint)
 
         if Path(checkpoint).is_dir() and not index_file_exists:
             # if the checkpoint is a directory and there is no index file, raise error
             raise ValueError(f'Cannot find index file in {checkpoint}')
 
         if index_file_exists:
             # the existence of index file means it is a sharded checkpoint
-            self.load_sharded_optimizer(optimizer, index_file_path)
+            self.load_sharded_optimizer(optimizer, index_file_path, prefix)
         else:
             self.load_unsharded_optimizer(optimizer, checkpoint)
 
     def save_optimizer(self,
                        optimizer: Optimizer,
                        checkpoint: str,
                        shard: bool = False,
@@ -179,14 +183,15 @@
                 3. a path to a folder containing a unique .index.json file for sharded checkpoint
             shard (bool): whether to shard the checkpoint. Default: False. If set to True, the checkpoint will be sharded into
                 multiple files. The optimizer shards will be specified by a `optimizer.index.json` file.
             gather_dtensor (bool): whether to gather the distributed tensor to the first device. Default: True.
             prefix (str): prefix for the optimizer checkpoint when shard = True. Default: None.
             size_per_shard (int): size per shard in MB. Default: 1024. This value is only used when shard is set to True.
         """
+
         if shard:
             self.save_sharded_optimizer(optimizer, checkpoint, gather_dtensor, prefix, size_per_shard)
         else:
             self.save_unsharded_optimizer(optimizer, checkpoint, gather_dtensor)
 
     # ========================================================
     # Abstract methods for model loading/saving implementation
@@ -214,15 +219,15 @@
             checkpoint (str): checkpoint path. It should be a single file path pointing to a model weight binary.
             strict (bool): whether to strictly enforce that the param name in
                 the checkpoint match the keys returned by this module's.
         """
         pass
 
     @abstractmethod
-    def save_sharded_model(self, model: nn.Module, checkpoint: str, gather_dtensor: bool, variant: Optional[str],
+    def save_sharded_model(self, model: nn.Module, checkpoint: str, gather_dtensor: bool, prefix: Optional[str],
                            size_per_shard: int, use_safetensors: bool):
         """
         Save model to sharded checkpoint.
 
         Args:
             model (nn.Module): model to be saved.
             checkpoint (str): checkpoint path. It should be a directory path.
@@ -247,23 +252,22 @@
         pass
 
     # ========================================================
     # Abstract methods for optimizer loading/saving implementation
     # ========================================================
 
     @abstractmethod
-    def load_sharded_optimizer(self, optimizer: Optimizer, index_file_path: str, prefix: str, size_per_shard: int):
+    def load_sharded_optimizer(self, optimizer: Optimizer, index_file_path: str, prefix: str):
         """
         Load optimizer from sharded checkpoint.
 
         Args:
             optimizer (Optimizer): optimizer to be loaded.
             index_file_path (str): checkpoint path. It should be path to the .index.json file or a path to a directory which contains a .index.json file.
             prefix (str): prefix for the optimizer checkpoint.
-            size_per_shard (int): size per shard in MB.
         """
         pass
 
     @abstractmethod
     def load_unsharded_optimizer(self, optimizer: Optimizer, checkpoint: Path):
         """
         Load optimizer from unsharded checkpoint.
```

### Comparing `colossalai-0.3.0/colossalai/checkpoint_io/index_file.py` & `colossalai-0.3.1/colossalai/checkpoint_io/index_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
-from pathlib import Path
-from typing import Any, List, Union
 import os
-import json
+from collections import OrderedDict
+from pathlib import Path
+from typing import Any, Dict, List, Union
 
 from .utils import is_dtensor_checkpoint
 
 __all__ = ['CheckpointIndexFile']
 
 
 class CheckpointIndexFile:
@@ -18,16 +18,18 @@
         >>> index.append_metadata('model_type', 'bert')
         >>> index.append_weight_map('bert.embeddings.word_embeddings.weight', 'model_0001-of-0002.bin')
         >>> index.export('new_index.json')
     """
 
     def __init__(self, root_path=None) -> None:
         self.root_path = root_path
-        self.metadata: dict = dict()
-        self.weight_map: dict = dict()
+
+        # use ordered dict to preserve the tensor checkpoint order
+        self.metadata: Dict = OrderedDict()
+        self.weight_map: Dict = OrderedDict()
 
     @staticmethod
     def from_file(index_path: Union[str, Path]):
         """
         Create a CheckpointIndexFile object from a json file.
 
         Args:
@@ -105,15 +107,15 @@
             bool: True if the index file contains any distributed tensor, False otherwise.
         """
         for value in self.weight_map.values():
             if value.endswith(".*.bin") or value.endswith(".*.safetensors"):
                 return True
         return False
 
-    def get_checkpoint_fileanames(self) -> List[str]:
+    def get_checkpoint_filenames(self) -> List[str]:
         """
         Get the set of checkpoint filenames in the weight map.
 
         Returns:
             list: checkpoint shard filenames.
         """
         # read the checkpoint file list from the json file and get a list of unique file names
@@ -146,23 +148,35 @@
             param_name (str): name of the parameter.
 
         Returns:
             str: checkpoint file name.
         """
         ckpt_path = self.weight_map[param_name]
         return ckpt_path
-    
+
     def get_all_param_names(self):
         """
         Get all the weight keys.
         """
         return list(self.weight_map.keys())
-    
+
+    def get_param_group_filename(self) -> Union[str, None]:
+        """
+        Get the file name of param_group file if this is a checkpoint for optimizer.
+        Returns:
+            str: param_group file name
+        """
+        filename = self.metadata.get("param_groups", None)
+        if filename:
+            return str(self.root_path.joinpath(filename))
+        else:
+            return None
+
     def write_index_file(self, save_index_file):
         """
         Write index file.
         """
         save_index_file = os.path.join(self.root_path, save_index_file)
         index = {"metadata": self.metadata, "weight_map": self.weight_map}
         with open(save_index_file, "w", encoding="utf-8") as f:
-            content = json.dumps(index, indent=2, sort_keys=True) + "\n"
+            content = json.dumps(index, indent=2) + "\n"
             f.write(content)
```

### Comparing `colossalai-0.3.0/colossalai/cli/benchmark/__init__.py` & `colossalai-0.3.1/colossalai/cli/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/cli/benchmark/benchmark.py` & `colossalai-0.3.1/colossalai/cli/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/cli/benchmark/utils.py` & `colossalai-0.3.1/colossalai/cli/benchmark/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import math
 import time
+from typing import Callable, Dict, List, Tuple
+
 import torch
 
+from colossalai.context import Config, ParallelMode
 from colossalai.utils import MultiTimer
-from colossalai.context import ParallelMode, Config
-from typing import List, Dict, Tuple, Callable
 
 
 def get_time_stamp() -> int:
     """
     Return the time stamp for profiling.
 
     Returns:
@@ -21,16 +22,16 @@
 
 
 def get_memory_states() -> Tuple[float]:
     """
     Return the memory statistics.
 
     Returns:
-        max_allocated (float): the allocated CUDA memory 
-        max_cached (float):  the cached CUDA memory 
+        max_allocated (float): the allocated CUDA memory
+        max_cached (float):  the cached CUDA memory
     """
 
     max_allocated = torch.cuda.max_memory_allocated() / (1024**3)
     max_cached = torch.cuda.max_memory_reserved() / (1024**3)
     torch.cuda.reset_peak_memory_stats()
     torch.cuda.empty_cache()
     return max_allocated, max_cached
@@ -97,15 +98,15 @@
 
     Args:
         model (torch.nn.Module): a PyTorch model
         warmup_steps (int): the number of steps for warmup
         profile_steps (int): the number of steps for profiling
         data_func (Callable): a function to generate random data
         timer (colossalai.utils.Multitimer): a timer instance for time recording
-    
+
     Returns:
         fwd_time (float): the average forward time taken by forward pass in second
         bwd_time (float): the average backward time taken by forward pass in second
         max_allocated (float): the maximum GPU memory allocated in GB
         max_cached (float): the maximum GPU memory cached in GB
     """
```

### Comparing `colossalai-0.3.0/colossalai/cli/check/check_installation.py` & `colossalai-0.3.1/colossalai/cli/check/check_installation.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/cli/launcher/__init__.py` & `colossalai-0.3.1/colossalai/cli/launcher/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
               help="Specify computing devices to use during execution. String format is <host1>,<host2>,"
               " only effective when used with --hostfile.")
 @click.option(
     "--exclude",
     type=str,
     default=None,
     help=
-    "Specify computing devices to NOT use during execution. Mutually exclusive with --include. Formatting is the same as --includ,"
+    "Specify computing devices to NOT use during execution. Mutually exclusive with --include. Formatting is the same as --include,"
     " only effective when used with --hostfile.")
 @click.option("--num_nodes",
               type=int,
               default=-1,
               help="Total number of worker nodes to use, only effective when used with --hostfile.")
 @click.option("--nproc_per_node", type=int, default=None, help="Number of GPUs to use on each node.")
 @click.option("--master_port",
```

### Comparing `colossalai-0.3.0/colossalai/cli/launcher/hostinfo.py` & `colossalai-0.3.1/colossalai/cli/launcher/hostinfo.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,27 +34,24 @@
         """
 
         if port is None:
             port = 22    # no port specified, lets just use the ssh port
 
         # socket.getfqdn("127.0.0.1") does not return localhost
         # on some users' machines
-        # thus, we directly return True if hostname is locahost, 127.0.0.1 or 0.0.0.0
+        # thus, we directly return True if hostname is localhost, 127.0.0.1 or 0.0.0.0
         if hostname in ("localhost", "127.0.0.1", "0.0.0.0"):
             return True
 
         hostname = socket.getfqdn(hostname)
         localhost = socket.gethostname()
         localaddrs = socket.getaddrinfo(localhost, port)
         targetaddrs = socket.getaddrinfo(hostname, port)
-        for (family, socktype, proto, canonname, sockaddr) in localaddrs:
-            for (rfamily, rsocktype, rproto, rcanonname, rsockaddr) in targetaddrs:
-                if rsockaddr[0] == sockaddr[0]:
-                    return True
-        return False
+
+        return localaddrs == targetaddrs
 
     def __str__(self):
         return f'hostname: {self.hostname}, port: {self.port}'
 
     def __repr__(self):
         return self.__str__()
```

### Comparing `colossalai-0.3.0/colossalai/cli/launcher/multinode_runner.py` & `colossalai-0.3.1/colossalai/cli/launcher/multinode_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,14 +110,14 @@
             conn.send('exit')
 
     def recv_from_all(self) -> dict:
         """
         Receive messages from all hosts
 
         Returns:
-            msg_from_node (dict): a dictionry which contains messages from each node
+            msg_from_node (dict): a dictionary which contains messages from each node
         """
 
         msg_from_node = dict()
         for hostname, conn in self.master_recv_conns.items():
             msg_from_node[hostname] = conn.recv()
         return msg_from_node
```

### Comparing `colossalai-0.3.0/colossalai/cli/launcher/run.py` & `colossalai-0.3.1/colossalai/cli/launcher/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,27 +150,25 @@
             else:
                 extra_launch_args_dict[arg] = None
         extra_launch_args = extra_launch_args_dict
     else:
         extra_launch_args = dict()
 
     torch_version = version.parse(torch.__version__)
-    assert torch_version.major == 1
+    assert torch_version.major >= 1
 
     if torch_version.minor < 9:
         cmd = [
             sys.executable, "-m", "torch.distributed.launch", f"--nproc_per_node={nproc_per_node}",
             f"--master_addr={master_addr}", f"--master_port={master_port}", f"--nnodes={num_nodes}",
             f"--node_rank={node_rank}"
         ]
     else:
         # extra launch args for torch distributed launcher with torch >= 1.9
-        default_torchrun_rdzv_args = dict(rdzv_backend="c10d",
-                                          rdzv_endpoint=f"{master_addr}:{master_port}",
-                                          rdzv_id="colossalai-default-job")
+        default_torchrun_rdzv_args = dict(master_addr=master_addr, master_port=master_port)
 
         # update rdzv arguments
         for key in default_torchrun_rdzv_args.keys():
             if key in extra_launch_args:
                 value = extra_launch_args.pop(key)
                 default_torchrun_rdzv_args[key] = value
 
@@ -294,15 +292,15 @@
 
     # stop all nodes
     runner.stop_all()
 
     # receive the stop status
     msg_from_node = runner.recv_from_all()
 
-    # printe node status
+    # print node status
     click.echo("\n====== Stopping All Nodes =====")
     for hostname, msg in msg_from_node.items():
         click.echo(f"{hostname}: {msg}")
 
     # give the process an exit code
     # so that it behaves like a normal process
     if has_error:
```

### Comparing `colossalai-0.3.0/colossalai/cluster/device_mesh_manager.py` & `colossalai-0.3.1/colossalai/cluster/device_mesh_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/cluster/dist_coordinator.py` & `colossalai-0.3.1/colossalai/cluster/dist_coordinator.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/cluster/process_group_manager.py` & `colossalai-0.3.1/colossalai/cluster/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/communication/__init__.py` & `colossalai-0.3.1/colossalai/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/communication/collective.py` & `colossalai-0.3.1/colossalai/communication/collective.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/communication/p2p.py` & `colossalai-0.3.1/colossalai/communication/p2p.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
+import operator
+from functools import reduce
 from typing import List, Tuple, Union
+
 import torch
 import torch.distributed as dist
 
 from colossalai.context.parallel_mode import ParallelMode
 from colossalai.core import global_context as gpc
 from colossalai.utils import get_current_device
-from functools import reduce
-import operator
-from .utils import split_tensor_into_1d_equal_chunks, gather_split_1d_tensor
+
+from .utils import gather_split_1d_tensor, split_tensor_into_1d_equal_chunks
 
 TensorShape = Union[torch.Size, List[int], Tuple[int]]
 
 
 def _get_tensor_shape(tensor_shape: TensorShape, chunk_tensor: bool = False) -> Tuple[TensorShape, bool]:
     """get the exact tensor shape when communicating and return whether the tensor is a chunk
 
@@ -256,15 +258,15 @@
 
 def send_forward_recv_backward(output_tensor,
                                output_grad_shape,
                                recv_next=True,
                                next_rank=None,
                                dtype=torch.float,
                                scatter_gather_tensors=False) -> Union[torch.Tensor, List[torch.Tensor]]:
-    """Batched communication operation. Sends the input tensor to the 
+    """Batched communication operation. Sends the input tensor to the
     next stage in pipeline, while receives the gradient tensor from the
     next stage in pipeline as the input gradient tensor of this stage.
 
     Args:
         output_tensor (Union[:class:`torch.Tensor`, List[:class:`torch.Tensor`]]): Tensor to be sent.
         output_grad_shape (Union[:class:`torch.Size`, List[:class:`torch.Size`]]): The shape of the tensor to be received.
 
@@ -315,15 +317,15 @@
 def send_forward_recv_forward(output_tensor,
                               input_tensor_shape,
                               recv_prev=True,
                               prev_rank=None,
                               next_rank=None,
                               dtype=torch.float,
                               scatter_gather_tensors=False) -> Union[torch.Tensor, List[torch.Tensor]]:
-    """Batched communication operation. Sends the input tensor to the 
+    """Batched communication operation. Sends the input tensor to the
     next stage in pipeline, while receives the output tensor from the
     previous stage in pipeline as the input of this stage.
 
     Args:
         output_tensor (Union[:class:`torch.Tensor`, List[:class:`torch.Tensor`]]): Tensor to be sent.
         input_tensor_shape (Union[:class:`torch.Size`, List[:class:`torch.Size`]]): The shape of the tensor to be received.
```

### Comparing `colossalai-0.3.0/colossalai/communication/p2p_v2.py` & `colossalai-0.3.1/colossalai/communication/p2p_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/communication/ring.py` & `colossalai-0.3.1/colossalai/communication/ring.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/communication/utils.py` & `colossalai-0.3.1/colossalai/communication/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from typing import List, Tuple, Union
+
 import torch
 import torch.distributed as dist
 
 from colossalai.context.parallel_mode import ParallelMode
 from colossalai.core import global_context as gpc
 from colossalai.utils import get_current_device
-from typing import Union, List, Tuple
 
 TensorShape = Union[torch.Size, List[int], Tuple[int]]
 
 
 def send_meta_helper(obj, next_rank, tensor_kwargs):
     send_shape = torch.tensor(obj.size(), **tensor_kwargs)
     send_ndims = torch.tensor(len(obj.size()), **tensor_kwargs)
```

### Comparing `colossalai-0.3.0/colossalai/constants.py` & `colossalai-0.3.1/colossalai/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/context/config.py` & `colossalai-0.3.1/colossalai/context/config.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/context/moe_context.py` & `colossalai-0.3.1/colossalai/context/moe_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/context/parallel_context.py` & `colossalai-0.3.1/colossalai/context/parallel_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/context/parallel_mode.py` & `colossalai-0.3.1/colossalai/context/parallel_mode.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/context/process_group_initializer/__init__.py` & `colossalai-0.3.1/colossalai/context/process_group_initializer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/context/process_group_initializer/initializer_1d.py` & `colossalai-0.3.1/colossalai/context/process_group_initializer/initializer_1d.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/context/process_group_initializer/initializer_2d.py` & `colossalai-0.3.1/colossalai/context/process_group_initializer/initializer_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/context/process_group_initializer/initializer_2p5d.py` & `colossalai-0.3.1/colossalai/context/process_group_initializer/initializer_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/context/process_group_initializer/initializer_3d.py` & `colossalai-0.3.1/colossalai/context/process_group_initializer/initializer_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/context/process_group_initializer/initializer_data.py` & `colossalai-0.3.1/colossalai/context/process_group_initializer/initializer_data.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/context/process_group_initializer/initializer_model.py` & `colossalai-0.3.1/colossalai/context/process_group_initializer/initializer_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/context/process_group_initializer/initializer_pipeline.py` & `colossalai-0.3.1/colossalai/context/process_group_initializer/initializer_pipeline.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/context/process_group_initializer/initializer_sequence.py` & `colossalai-0.3.1/colossalai/context/process_group_initializer/initializer_sequence.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/context/process_group_initializer/initializer_tensor.py` & `colossalai-0.3.1/colossalai/context/process_group_initializer/initializer_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/context/process_group_initializer/process_group_initializer.py` & `colossalai-0.3.1/colossalai/context/process_group_initializer/process_group_initializer.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/context/random/_helper.py` & `colossalai-0.3.1/colossalai/context/random/_helper.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/context/random/seed_manager.py` & `colossalai-0.3.1/colossalai/context/random/seed_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/context/singleton_meta.py` & `colossalai-0.3.1/colossalai/context/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/device/alpha_beta_profiler.py` & `colossalai-0.3.1/colossalai/device/alpha_beta_profiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
             else:
                 beta = 1 / bandwidth
 
             broadcast_list = [alpha, beta]
             dist.broadcast_object_list(broadcast_list, src=process_group[0])
             alpha_beta_dict[process_group] = tuple(broadcast_list)
 
-        # add symmetry pair to the apha_beta_dict
+        # add symmetry pair to the alpha_beta_dict
         symmetry_ab_dict = {}
         for process_group, alpha_beta_pair in alpha_beta_dict.items():
             symmetry_process_group = (process_group[1], process_group[0])
             symmetry_ab_dict[symmetry_process_group] = alpha_beta_pair
 
         alpha_beta_dict.update(symmetry_ab_dict)
```

### Comparing `colossalai-0.3.0/colossalai/device/calc_pipeline_strategy.py` & `colossalai-0.3.1/colossalai/device/calc_pipeline_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/engine/_base_engine.py` & `colossalai-0.3.1/colossalai/engine/_base_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from torch.nn import Module
 from torch.nn.modules.loss import _Loss
 
 from colossalai.engine.gradient_handler import BaseGradientHandler
 from colossalai.engine.schedule import BaseSchedule, InterleavedPipelineSchedule, NonPipelineSchedule, PipelineSchedule
 from colossalai.logging import get_dist_logger
 from colossalai.zero.legacy.gemini import BaseOpHook, register_ophooks_recursively
-
+from colossalai.nn.optimizer import ColossalaiOptimizer
 
 class Engine:
     """Basic engine class for training and evaluation. It runs a specific process method
     :meth:`step` which is based on the given :attr:`schedule` over each batch of a dataset.
     It controls a iteration in training.
 
     Args:
```

### Comparing `colossalai-0.3.0/colossalai/engine/gradient_accumulation/__init__.py` & `colossalai-0.3.1/colossalai/engine/gradient_accumulation/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/engine/gradient_accumulation/_gradient_accumulation.py` & `colossalai-0.3.1/colossalai/engine/gradient_accumulation/_gradient_accumulation.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/engine/gradient_handler/__init__.py` & `colossalai-0.3.1/colossalai/engine/gradient_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/engine/gradient_handler/_base_gradient_handler.py` & `colossalai-0.3.1/colossalai/engine/gradient_handler/_base_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py` & `colossalai-0.3.1/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/engine/gradient_handler/_moe_gradient_handler.py` & `colossalai-0.3.1/colossalai/engine/gradient_handler/_moe_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py` & `colossalai-0.3.1/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py` & `colossalai-0.3.1/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/engine/gradient_handler/_zero_gradient_handler.py` & `colossalai-0.3.1/colossalai/engine/gradient_handler/_zero_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/engine/gradient_handler/utils.py` & `colossalai-0.3.1/colossalai/engine/gradient_handler/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/engine/schedule/_base_schedule.py` & `colossalai-0.3.1/colossalai/engine/schedule/_base_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/engine/schedule/_non_pipeline_schedule.py` & `colossalai-0.3.1/colossalai/engine/schedule/_non_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/engine/schedule/_pipeline_schedule.py` & `colossalai-0.3.1/colossalai/engine/schedule/_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/engine/schedule/_pipeline_schedule_v2.py` & `colossalai-0.3.1/colossalai/engine/schedule/_pipeline_schedule_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/_compatibility.py` & `colossalai-0.3.1/colossalai/fx/_compatibility.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/_meta_regist_12.py` & `colossalai-0.3.1/colossalai/fx/_meta_regist_12.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/_meta_regist_13.py` & `colossalai-0.3.1/colossalai/fx/_meta_regist_13.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/codegen/activation_checkpoint_codegen.py` & `colossalai-0.3.1/colossalai/fx/codegen/activation_checkpoint_codegen.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/graph_module.py` & `colossalai-0.3.1/colossalai/fx/graph_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/passes/adding_split_node_pass.py` & `colossalai-0.3.1/colossalai/fx/passes/adding_split_node_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/passes/concrete_info_prop.py` & `colossalai-0.3.1/colossalai/fx/passes/concrete_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/passes/meta_info_prop.py` & `colossalai-0.3.1/colossalai/fx/passes/meta_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/passes/passes_for_gpt2_test.py` & `colossalai-0.3.1/colossalai/fx/passes/passes_for_gpt2_test.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/passes/shard_1d_pass.py` & `colossalai-0.3.1/colossalai/fx/passes/shard_1d_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/passes/split_module.py` & `colossalai-0.3.1/colossalai/fx/passes/split_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/passes/utils.py` & `colossalai-0.3.1/colossalai/fx/passes/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/__init__.py` & `colossalai-0.3.1/colossalai/fx/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/constants.py` & `colossalai-0.3.1/colossalai/fx/profiler/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/dataflow.py` & `colossalai-0.3.1/colossalai/fx/profiler/dataflow.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/experimental/constants.py` & `colossalai-0.3.1/colossalai/fx/profiler/experimental/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler.py` & `colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_function/activation_function.py` & `colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_function/activation_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py` & `colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_function/embedding.py` & `colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_function/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_function/normalization.py` & `colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_function/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_function/pooling.py` & `colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_function/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py` & `colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_module/activation_function.py` & `colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_module/activation_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_module/attention.py` & `colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_module/attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_module/convolution.py` & `colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_module/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_module/normalization.py` & `colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_module/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_module/pooling.py` & `colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_module/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/experimental/profiler_module/rnn.py` & `colossalai-0.3.1/colossalai/fx/profiler/experimental/profiler_module/rnn.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/experimental/registry.py` & `colossalai-0.3.1/colossalai/fx/profiler/experimental/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/experimental/shard_utils.py` & `colossalai-0.3.1/colossalai/fx/profiler/experimental/shard_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/memory_utils.py` & `colossalai-0.3.1/colossalai/fx/profiler/memory_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/opcount.py` & `colossalai-0.3.1/colossalai/fx/profiler/opcount.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/profiler.py` & `colossalai-0.3.1/colossalai/fx/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/shard_utils.py` & `colossalai-0.3.1/colossalai/fx/profiler/shard_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/profiler/tensor.py` & `colossalai-0.3.1/colossalai/fx/profiler/tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/proxy.py` & `colossalai-0.3.1/colossalai/fx/proxy.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/_meta_trace.py` & `colossalai-0.3.1/colossalai/fx/tracer/_meta_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/_symbolic_trace.py` & `colossalai-0.3.1/colossalai/fx/tracer/_symbolic_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/_tracer_utils.py` & `colossalai-0.3.1/colossalai/fx/tracer/_tracer_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py` & `colossalai-0.3.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py` & `colossalai-0.3.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py` & `colossalai-0.3.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py` & `colossalai-0.3.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py` & `colossalai-0.3.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     @abstractmethod
     def extract_kwargs_from_mod(self):
         """
         This method is used to extract the kwargs for non-bias computation.
 
         For example:
             The kwargs for conv2d module is {} because the attributes like 'padding' or 'groups' are
-            considered during module initilizing. However, we need to consider those attributes as kwargs
+            considered during module initializing. However, we need to consider those attributes as kwargs
             in F.conv2d.
         """
         pass
 
     def create_non_bias_func_proxy(self, input_proxy=None):
         """
         This method is used to create the non_bias_func proxy, the node created by this proxy will
```

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py` & `colossalai-0.3.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py` & `colossalai-0.3.1/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/experimental.py` & `colossalai-0.3.1/colossalai/fx/tracer/experimental.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,15 @@
         if enabled:
             orig_ckpt_func = torch.utils.checkpoint.CheckpointFunction
 
             class PatchedCheckpointFunction(torch.autograd.Function):
 
                 @staticmethod
                 def forward(ctx, run_function, preserve_rng_state, *args):
-                    # signal that the current tracing occurs within activaton checkpoint part
+                    # signal that the current tracing occurs within activation checkpoint part
                     self.inside_torch_checkpoint_func = True
                     out = run_function(*args)
                     self.inside_torch_checkpoint_func = False
                     self.act_ckpt_region_count += 1
                     return out
 
                 @staticmethod
```

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py` & `colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_function/convolution.py` & `colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_function/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_function/embedding.py` & `colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_function/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_function/normalization.py` & `colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_function/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py` & `colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py` & `colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_module/convolution.py` & `colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_module/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_module/normalization.py` & `colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_module/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_module/pooling.py` & `colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_module/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/meta_patch/patched_module/rnn.py` & `colossalai-0.3.1/colossalai/fx/tracer/meta_patch/patched_module/rnn.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/registry.py` & `colossalai-0.3.1/colossalai/fx/tracer/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/fx/tracer/tracer.py` & `colossalai-0.3.1/colossalai/fx/tracer/tracer.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         if self.tracer_type == TracerType.DEFAULT:
             # since meta_args is not given
             # we just fall back to the original torch.fx.Tracer
             proxy = super().create_proxy(kind, target, args, kwargs, name, type_expr, proxy_factory_fn)
             return proxy
 
         # if graph is traced for auto parallelism module, some extra node will be added during
-        # graph construction to deal with the compatability between bias addition and all reduce.
+        # graph construction to deal with the compatibility between bias addition and all reduce.
 
         # if no extra manipulation is applied, we just pass the origin arguments to create_proxy function
         # to create node on computation graph
         origin_arguments = (kind, target, args, kwargs, name, type_expr, proxy_factory_fn)
         # dispatch the arguments generator depending on the kind and target in origin arguments.
         args_metas, _ = extract_meta(*args, **kwargs)
         handle = None
@@ -204,15 +204,15 @@
         if tracer_type == TracerType.DEFAULT:
             self.proxy_cls = Proxy
             self.tracer_type = TracerType.DEFAULT
         elif tracer_type == TracerType.META:
             self.proxy_cls = ColoProxy
             self.tracer_type = TracerType.META
         else:
-            raise ValueError(f"Unrecognised tracer type {tracer_type}")
+            raise ValueError(f"Unrecognized tracer type {tracer_type}")
 
     def _meta_data_computing(self, kind, target, args, kwargs):
 
         if kind == "placeholder" and target in self.meta_args and self.meta_args[target].is_meta:
             meta_out = self.meta_args[target]
             return meta_out
 
@@ -441,15 +441,15 @@
         if enabled:
             orig_ckpt_func = torch.utils.checkpoint.CheckpointFunction
 
             class PatchedCheckpointFunction(torch.autograd.Function):
 
                 @staticmethod
                 def forward(ctx, run_function, preserve_rng_state, *args):
-                    # signal that the current tracing occurs within activaton checkpoint part
+                    # signal that the current tracing occurs within activation checkpoint part
                     self.inside_torch_checkpoint_func = True
                     out = run_function(*args)
                     self.inside_torch_checkpoint_func = False
                     self.act_ckpt_region_count += 1
                     return out
 
                 @staticmethod
```

### Comparing `colossalai-0.3.0/colossalai/global_variables.py` & `colossalai-0.3.1/colossalai/global_variables.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/initialize.py` & `colossalai-0.3.1/colossalai/initialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
                lr_scheduler: Optional[_LRScheduler] = None,
                ophooks: Optional[List[BaseOpHook]] = None,
                verbose: bool = True) -> Tuple[Engine, DataLoader, DataLoader, _LRScheduler]:
     """Core function to wrap the essential training components with our functionality based on the config which is
     loaded into gpc.config.
 
     Args:
-        model (:class:`torch.nn.Module` or Callbale): Your model instance or a function to build the model.
+        model (:class:`torch.nn.Module` or Callable): Your model instance or a function to build the model.
         optimizer (:class:`torch.optim.optimizer.Optimizer` or :class:`Type[torch.optim.optimizer]`):
             Your optimizer instance.
         criterion (:class:`torch.nn.modules.loss._Loss`, optional): Your criterion instance.
         train_dataloader (:class:`torch.utils.data.DataLoader`, optional): Dataloader for training.
         test_dataloader (:class:`torch.utils.data.DataLoader`, optional): Dataloader for testing.
         lr_scheduler (:class:`torch.nn.lr_scheduler._LRScheduler`, optional): Your lr scheduler instance, optional.
         verbose (bool, optional): Whether to print logs.
```

### Comparing `colossalai-0.3.0/colossalai/interface/model.py` & `colossalai-0.3.1/colossalai/interface/model.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/interface/optimizer.py` & `colossalai-0.3.1/colossalai/interface/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,7 +115,13 @@
         """
         Unscale the gradients for mixed precision training.
 
         Note: Only available for optimizers with mixed precision training.
         """
         raise NotImplementedError(
             "The method unscale_grad is only available for optimizers with mixed precision training")
+
+    def unwrap(self):
+        """
+        Unwrap the optimizer for checkpoint saving/loading.
+        """
+        return self.optim
```

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/cpu_adam.h` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/cpu_adam.h`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/context.h` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/context.h`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/csrc/type_shim.h` & `colossalai-0.3.1/colossalai/kernel/cuda_native/csrc/type_shim.h`

 * *Files 10% similar despite different names*

```diff
@@ -167,14 +167,29 @@
     using g_scalar_t_##LEVEL = at::Half;                                       \
     using p_scalar_t_##LEVEL = float;                                          \
     __VA_ARGS__;                                                               \
   } else if (GTYPE == at::ScalarType::Half && PTYPE == at::ScalarType::Half) { \
     using g_scalar_t_##LEVEL = at::Half;                                       \
     using p_scalar_t_##LEVEL = at::Half;                                       \
     __VA_ARGS__;                                                               \
+  } else if (GTYPE == at::ScalarType::Float &&                                 \
+             PTYPE == at::ScalarType::BFloat16) {                              \
+    using g_scalar_t_##LEVEL = float;                                          \
+    using p_scalar_t_##LEVEL = at::BFloat16;                                   \
+    __VA_ARGS__;                                                               \
+  } else if (GTYPE == at::ScalarType::BFloat16 &&                              \
+             PTYPE == at::ScalarType::Float) {                                 \
+    using g_scalar_t_##LEVEL = at::BFloat16;                                   \
+    using p_scalar_t_##LEVEL = float;                                          \
+    __VA_ARGS__;                                                               \
+  } else if (GTYPE == at::ScalarType::BFloat16 &&                              \
+             PTYPE == at::ScalarType::BFloat16) {                              \
+    using g_scalar_t_##LEVEL = at::BFloat16;                                   \
+    using p_scalar_t_##LEVEL = at::BFloat16;                                   \
+    __VA_ARGS__;                                                               \
   } else {                                                                     \
     AT_ERROR(#NAME, "not implemented for '", toString(GTYPE), toString(PTYPE), \
              "'");                                                             \
   }
 
 template <typename T>
 __device__ __forceinline__ T reduce_block_into_lanes(
```

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/flash_attention.py` & `colossalai-0.3.1/colossalai/kernel/cuda_native/flash_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
                     if batch_size > 1:
                         query = rearrange(query, "b s ... -> c (b s) ...", c=1)
                         key, value = self.unpad(torch.stack([query, key, value], dim=2), kv_indices).unbind(dim=2)
                 attn_bias = BlockDiagonalMask.from_seqlens(q_seqlen, kv_seqlen)
             elif attn_mask_type == AttnMaskType.causal:    # gpt style
                 attn_bias = LowerTriangularMask()
 
-            if bias is not None:    # alibi / relative position emebedding
+            if bias is not None:    # alibi / relative position embedding
                 assert allow_alibi, "flash attention with bias is not supported in this system."
                 assert attn_mask_type == AttnMaskType.causal, \
                     "attention with bias is only supported for causal attention so far."
                 attn_bias = attn_bias.add_bias(bias)
 
             out = memory_efficient_attention(query, key, value, attn_bias=attn_bias, p=self.dropout, scale=self.scale)
```

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/layer_norm.py` & `colossalai-0.3.1/colossalai/kernel/cuda_native/layer_norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/multihead_attention.py` & `colossalai-0.3.1/colossalai/kernel/cuda_native/multihead_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     max_batch_tokens: int    # max batch token numbers
     max_seq_len: int    # max sequence length
     hidden_size: int    # size of transformer hidden layers
     nhead: int    # number of heads in attention
     attn_prob_dropout_ratio: float    # attention score dropout ratio
     hidden_dropout_ratio: float    # dropout ration before residual
     norm_first: bool    # norm_first
-    fp16: bool    # fp16 presion
+    fp16: bool    # fp16 precision
 
 
 class MultiHeadAttention1DFunc(Function):
 
     @staticmethod
     def forward(ctx, input, input_mask, in_proj_weight, in_proj_bias, out_proj_weight, out_proj_bias, norm_weight,
                 norm_bias, config):
```

### Comparing `colossalai-0.3.0/colossalai/kernel/cuda_native/scaled_softmax.py` & `colossalai-0.3.1/colossalai/kernel/cuda_native/scaled_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/jit/bias_dropout_add.py` & `colossalai-0.3.1/colossalai/kernel/jit/bias_dropout_add.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import torch
+from torch import Tensor
 
 
 def bias_dropout_add(x, bias, residual, prob, training):
     # type: (Tensor, Tensor, Tensor, float, bool) -> Tensor
     out = torch.nn.functional.dropout(x + bias, p=prob, training=training)
     out = residual + out
     return out
```

### Comparing `colossalai-0.3.0/colossalai/kernel/jit/bias_gelu.py` & `colossalai-0.3.1/colossalai/kernel/jit/bias_gelu.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/jit/option.py` & `colossalai-0.3.1/colossalai/kernel/jit/option.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 
 def warmup_jit_fusion(batch_size: int,
                       hidden_size: int,
                       seq_length: int = 512,
                       vocab_size: int = 32768,
                       dtype: torch.dtype = torch.float32):
-    """ Compilie JIT functions before the main training steps """
+    """ Compile JIT functions before the main training steps """
 
     embed = Embedding(vocab_size, hidden_size).to(get_current_device())
     linear_1 = Linear(hidden_size, hidden_size * 4, skip_bias_add=True).to(get_current_device())
     linear_2 = Linear(hidden_size * 4, hidden_size, skip_bias_add=True).to(get_current_device())
 
     x = torch.randint(vocab_size, (batch_size, seq_length), dtype=torch.long, device=get_current_device())
     x = embed(x)
```

### Comparing `colossalai-0.3.0/colossalai/kernel/op_builder/__init__.py` & `colossalai-0.3.1/colossalai/kernel/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/op_builder/builder.py` & `colossalai-0.3.1/colossalai/kernel/op_builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/op_builder/cpu_adam.py` & `colossalai-0.3.1/colossalai/kernel/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/op_builder/fused_optim.py` & `colossalai-0.3.1/colossalai/kernel/op_builder/fused_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/op_builder/layernorm.py` & `colossalai-0.3.1/colossalai/kernel/op_builder/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/op_builder/moe.py` & `colossalai-0.3.1/colossalai/kernel/op_builder/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/op_builder/multi_head_attn.py` & `colossalai-0.3.1/colossalai/kernel/op_builder/multi_head_attn.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/op_builder/scaled_masked_softmax.py` & `colossalai-0.3.1/colossalai/kernel/op_builder/scaled_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py` & `colossalai-0.3.1/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/kernel/op_builder/utils.py` & `colossalai-0.3.1/colossalai/kernel/op_builder/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/logging/__init__.py` & `colossalai-0.3.1/colossalai/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/logging/logger.py` & `colossalai-0.3.1/colossalai/logging/logger.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/_ops/_utils.py` & `colossalai-0.3.1/colossalai/nn/_ops/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/_ops/addmm.py` & `colossalai-0.3.1/colossalai/nn/_ops/addmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/_ops/batch_norm.py` & `colossalai-0.3.1/colossalai/nn/_ops/batch_norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/_ops/element_wise.py` & `colossalai-0.3.1/colossalai/nn/_ops/element_wise.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/_ops/embedding.py` & `colossalai-0.3.1/colossalai/nn/_ops/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/_ops/embedding_bag.py` & `colossalai-0.3.1/colossalai/nn/_ops/embedding_bag.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/_ops/layernorm.py` & `colossalai-0.3.1/colossalai/nn/_ops/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/_ops/linear.py` & `colossalai-0.3.1/colossalai/nn/_ops/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/_ops/loss.py` & `colossalai-0.3.1/colossalai/nn/_ops/loss.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/_ops/view.py` & `colossalai-0.3.1/colossalai/nn/_ops/view.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/base_layer.py` & `colossalai-0.3.1/colossalai/nn/layer/base_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
+from contextlib import contextmanager
+
 import torch.nn as nn
 
 from colossalai.context import ParallelMode
 from colossalai.core import global_context as gpc
-from contextlib import contextmanager
 
 
 class ParallelLayer(nn.Module):
+
     global_state_dict: bool = True
 
     def __init__(self):
         super().__init__()
         self.data_parallel_rank = 0 if not gpc.is_initialized(ParallelMode.DATA) else gpc.get_local_rank(
             ParallelMode.DATA)
         self.data_parallel_size = 1 if not gpc.is_initialized(ParallelMode.DATA) else gpc.get_world_size(
```

### Comparing `colossalai-0.3.0/colossalai/nn/layer/colossalai_layer/_utils.py` & `colossalai-0.3.1/colossalai/nn/layer/colossalai_layer/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/colossalai_layer/dropout.py` & `colossalai-0.3.1/colossalai/nn/layer/colossalai_layer/dropout.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/colossalai_layer/embedding.py` & `colossalai-0.3.1/colossalai/nn/layer/colossalai_layer/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/colossalai_layer/linear.py` & `colossalai-0.3.1/colossalai/nn/layer/colossalai_layer/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/colossalai_layer/normalization.py` & `colossalai-0.3.1/colossalai/nn/layer/colossalai_layer/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/moe/__init__.py` & `colossalai-0.3.1/colossalai/nn/layer/moe/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/moe/_operation.py` & `colossalai-0.3.1/colossalai/nn/layer/moe/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/moe/checkpoint.py` & `colossalai-0.3.1/colossalai/nn/layer/moe/checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/moe/experts.py` & `colossalai-0.3.1/colossalai/nn/layer/moe/experts.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/moe/layers.py` & `colossalai-0.3.1/colossalai/nn/layer/moe/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/moe/routers.py` & `colossalai-0.3.1/colossalai/nn/layer/moe/routers.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/moe/utils.py` & `colossalai-0.3.1/colossalai/nn/layer/moe/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/parallel_1d/_operation.py` & `colossalai-0.3.1/colossalai/nn/layer/parallel_1d/_operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import torch
 import torch.distributed as dist
+
 from colossalai.core import global_context as gpc
 
 try:
     import fused_mix_prec_layer_norm_cuda
 except:
     fused_mix_prec_layer_norm_cuda = None
```

### Comparing `colossalai-0.3.0/colossalai/nn/layer/parallel_1d/_utils.py` & `colossalai-0.3.1/colossalai/nn/layer/parallel_1d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/parallel_1d/layers.py` & `colossalai-0.3.1/colossalai/nn/layer/parallel_1d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/parallel_2d/_operation.py` & `colossalai-0.3.1/colossalai/nn/layer/parallel_2d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/parallel_2d/_utils.py` & `colossalai-0.3.1/colossalai/nn/layer/parallel_2d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/parallel_2d/layers.py` & `colossalai-0.3.1/colossalai/nn/layer/parallel_2d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/parallel_2p5d/_operation.py` & `colossalai-0.3.1/colossalai/nn/layer/parallel_2p5d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/parallel_2p5d/_utils.py` & `colossalai-0.3.1/colossalai/nn/layer/parallel_2p5d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/parallel_2p5d/layers.py` & `colossalai-0.3.1/colossalai/nn/layer/parallel_2p5d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/parallel_3d/_operation.py` & `colossalai-0.3.1/colossalai/nn/layer/parallel_3d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/parallel_3d/_utils.py` & `colossalai-0.3.1/colossalai/nn/layer/parallel_3d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/parallel_3d/layers.py` & `colossalai-0.3.1/colossalai/nn/layer/parallel_3d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/parallel_sequence/_operation.py` & `colossalai-0.3.1/colossalai/nn/layer/parallel_sequence/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/parallel_sequence/layers.py` & `colossalai-0.3.1/colossalai/nn/layer/parallel_sequence/layers.py`

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
-        skip_bias_add: This was added to enable performance optimations where bias
+        skip_bias_add: This was added to enable performance optimizations where bias
                        can be fused with other elementwise operations. we skip
                        adding bias but instead return it.
     """
 
     def __init__(self, input_size, output_size, bias=True, skip_bias_add=False):
         super(_Linear, self).__init__()
```

### Comparing `colossalai-0.3.0/colossalai/nn/layer/utils/common.py` & `colossalai-0.3.1/colossalai/nn/layer/utils/common.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/vanilla/layers.py` & `colossalai-0.3.1/colossalai/nn/layer/vanilla/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/layer/wrapper/pipeline_wrapper.py` & `colossalai-0.3.1/colossalai/nn/layer/wrapper/pipeline_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/loss/__init__.py` & `colossalai-0.3.1/colossalai/nn/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/loss/loss_1d.py` & `colossalai-0.3.1/colossalai/nn/loss/loss_1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
         # Maximum value along vocab dimension across all GPUs.
         logits_max = torch.max(vocab_parallel_logits, dim=-1)[0]
         torch.distributed.all_reduce(logits_max, op=torch.distributed.ReduceOp.MAX, group=process_group)
         # Subtract the maximum value.
         vocab_parallel_logits.sub_(logits_max.unsqueeze(dim=-1))
 
-        # Get the partition's vocab indecies
+        # Get the partition's vocab indices
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
 
-        # Retreive tensors from the forward path.
+        # Retrieve tensors from the forward path.
         softmax, target_mask, masked_target_1d = ctx.saved_tensors
 
-        # All the inputs have softmax as thier gradient.
+        # All the inputs have softmax as their gradient.
         grad_input = softmax
         # For simplicity, work with the 2D gradient.
         partition_vocab_size = softmax.size()[-1]
         grad_2d = grad_input.view(-1, partition_vocab_size)
 
         # Add the gradient from matching classes.
         arange_1d = torch.arange(start=0, end=grad_2d.size()[0], device=grad_2d.device)
```

### Comparing `colossalai-0.3.0/colossalai/nn/loss/loss_2d.py` & `colossalai-0.3.1/colossalai/nn/loss/loss_2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         ctx.save_for_backward(exp_logits, target_mask, masked_target)
 
         return loss
 
     @staticmethod
     @custom_bwd
     def backward(ctx, output_grad):
-        # Retreive tensors from the forward path.
+        # Retrieve tensors from the forward path.
         softmax, target_mask, masked_target = ctx.saved_tensors
 
         # All the inputs have softmax as their gradient.
         grad_input = softmax
 
         # For simplicity, work with the 2D gradient.
         partition_vocab_size = softmax.size()[-1]
```

### Comparing `colossalai-0.3.0/colossalai/nn/loss/loss_2p5d.py` & `colossalai-0.3.1/colossalai/nn/loss/loss_2p5d.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         ctx.save_for_backward(exp_logits, target_mask, masked_target)
 
         return loss
 
     @staticmethod
     @custom_bwd
     def backward(ctx, output_grad):
-        # Retreive tensors from the forward path.
+        # Retrieve tensors from the forward path.
         softmax, target_mask, masked_target = ctx.saved_tensors
 
         # All the inputs have softmax as their gradient.
         grad_input = softmax
 
         # For simplicity, work with the 2D gradient.
         partition_vocab_size = softmax.size()[-1]
```

### Comparing `colossalai-0.3.0/colossalai/nn/loss/loss_3d.py` & `colossalai-0.3.1/colossalai/nn/loss/loss_3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,18 +95,18 @@
         ctx.save_for_backward(exp_logits, target_mask, masked_target)
 
         return loss
 
     @staticmethod
     @custom_bwd
     def backward(ctx, output_grad):
-        # Retreive tensors from the forward path.
+        # Retrieve tensors from the forward path.
         softmax, target_mask, masked_target = ctx.saved_tensors
 
-        # All the inputs have softmax as thier gradient.
+        # All the inputs have softmax as their gradient.
         input_grad = softmax
         # For simplicity, work with the 2D gradient.
         partition_vocab_size = softmax.size()[-1]
         grad_2d = input_grad.view(-1, partition_vocab_size)
 
         # Add the gradient from matching classes.
         arange_1d = torch.arange(start=0, end=grad_2d.size()[0], device=get_current_device())
```

### Comparing `colossalai-0.3.0/colossalai/nn/loss/loss_moe.py` & `colossalai-0.3.1/colossalai/nn/loss/loss_moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/lr_scheduler/__init__.py` & `colossalai-0.3.1/colossalai/nn/lr_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/lr_scheduler/cosine.py` & `colossalai-0.3.1/colossalai/nn/lr_scheduler/cosine.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/lr_scheduler/delayed.py` & `colossalai-0.3.1/colossalai/nn/lr_scheduler/delayed.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/lr_scheduler/linear.py` & `colossalai-0.3.1/colossalai/nn/lr_scheduler/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/lr_scheduler/multistep.py` & `colossalai-0.3.1/colossalai/nn/lr_scheduler/multistep.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/lr_scheduler/onecycle.py` & `colossalai-0.3.1/colossalai/nn/lr_scheduler/onecycle.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/lr_scheduler/poly.py` & `colossalai-0.3.1/colossalai/nn/lr_scheduler/poly.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/lr_scheduler/torch.py` & `colossalai-0.3.1/colossalai/nn/lr_scheduler/torch.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/metric/__init__.py` & `colossalai-0.3.1/colossalai/nn/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/metric/accuracy_2d.py` & `colossalai-0.3.1/colossalai/nn/metric/accuracy_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/metric/accuracy_2p5d.py` & `colossalai-0.3.1/colossalai/nn/metric/accuracy_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/metric/accuracy_3d.py` & `colossalai-0.3.1/colossalai/nn/metric/accuracy_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/optimizer/colossalai_optimizer.py` & `colossalai-0.3.1/colossalai/nn/optimizer/colossalai_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/optimizer/cpu_adam.py` & `colossalai-0.3.1/colossalai/nn/optimizer/cpu_adam.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 from .nvme_optimizer import NVMeOptimizer
 
 
 @OPTIMIZERS.register_module
 class CPUAdam(NVMeOptimizer):
     """Implements Adam algorithm.
 
-    Supports parameters updating on both GPU and CPU, depanding on the device of parameters.
+    Supports parameters updating on both GPU and CPU, depending on the device of parameters.
     But the parameters and gradients should on the same device:
       * Parameters on CPU and gradients on CPU is allowed.
       * Parameters on GPU and gradients on GPU is allowed.
       * Parameters on GPU and gradients on CPU is **not** allowed.
 
     `CPUAdam` requires CUDA extensions which can be built during installation or runtime.
 
-    This version of CPU Adam accelates parameters updating on CPU with SIMD.
+    This version of CPU Adam accelerates parameters updating on CPU with SIMD.
     Support of AVX2 or AVX512 is required.
 
     The GPU part is implemented in an naive way.
 
     CPU Adam also supports the hybrid precision calculation, eg. fp32 parameters and fp16 gradients.
 
     :class:`colossalai.nn.optimizer.CPUAdam` may be used as a drop-in replacement for ``torch.optim.AdamW``,
@@ -89,16 +89,15 @@
                           beta1,
                           beta2,
                           eps,
                           weight_decay,
                           bias_correction1,
                           bias_correction2,
                           use_adamw=False):
-        # FIXME(ver217): remove the below line when replace torch adam with fused adam
-        grad = grad.float()
+        grad = grad.to(data.dtype)
 
         if weight_decay != 0:
             if use_adamw:
                 data.mul_(1 - lr * weight_decay)
             else:
                 grad = grad.add(data, alpha=weight_decay)
 
@@ -129,31 +128,41 @@
 
                 state = self.state[p]
 
                 target_device = p.device
                 if len(state) == 0:
                     state['step'] = 0
 
+                    # FIXME(ver217): CPU adam kernel only supports fp32 states now
+                    assert p.dtype is torch.float, "CPUAdam only support fp32 parameters"
                     # gradient momentums
-                    state['exp_avg'] = torch.zeros_like(p, dtype=torch.float, device=target_device)
+                    state['exp_avg'] = torch.zeros_like(p, device=target_device)
                     # gradient variances
-                    state['exp_avg_sq'] = torch.zeros_like(p, dtype=torch.float, device=target_device)
+                    state['exp_avg_sq'] = torch.zeros_like(p, device=target_device)
                     self._post_state_init(p)
 
                 state['step'] += 1
                 beta1, beta2 = group['betas']
 
                 if target_device.type == 'cpu':
                     assert p.data.numel() == p.grad.data.numel(), "parameter and gradient should have the same size"
                     assert state['exp_avg'].device.type == 'cpu', "exp_avg should stay on cpu"
                     assert state['exp_avg_sq'].device.type == 'cpu', "exp_avg should stay on cpu"
                     self._pre_update(p, 'exp_avg', 'exp_avg_sq')
-                    self.cpu_adam_op.step(state['step'], group['lr'], beta1, beta2, group['eps'], group['weight_decay'],
-                                          group['bias_correction'], p.data, p.grad.data, state['exp_avg'],
-                                          state['exp_avg_sq'], div_scale)
+                    if p.grad.dtype is torch.bfloat16:
+                        # cpu adam kernel does not support bf16 now
+                        bias_correction1 = 1 - beta1**state['step']
+                        bias_correction2 = 1 - beta2**state['step']
+                        self.torch_adam_update(p.data, p.grad.data, state['exp_avg'], state['exp_avg_sq'], group['lr'],
+                                               beta1, beta2, group['eps'], group['weight_decay'], bias_correction1,
+                                               bias_correction2, self.adamw_mode)
+                    else:
+                        self.cpu_adam_op.step(state['step'], group['lr'], beta1, beta2, group['eps'],
+                                              group['weight_decay'], group['bias_correction'], p.data, p.grad.data,
+                                              state['exp_avg'], state['exp_avg_sq'], div_scale)
                     self._post_update(p, 'exp_avg', 'exp_avg_sq')
                 elif target_device.type == 'cuda':
                     assert div_scale == -1, "div_scale should remain default"
                     assert state['exp_avg'].device.type == 'cuda', "exp_avg should stay on cuda"
                     assert state['exp_avg_sq'].device.type == 'cuda', "exp_avg should stay on cuda"
 
                     bias_correction1 = 1 - beta1**state['step']
```

### Comparing `colossalai-0.3.0/colossalai/nn/optimizer/fused_adam.py` & `colossalai-0.3.1/colossalai/nn/optimizer/fused_adam.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,16 +130,16 @@
                 # State initialization
                 if len(state) == 0:
                     # Exponential moving average of gradient values
                     state['exp_avg'] = torch.zeros_like(p)
                     # Exponential moving average of squared gradient values
                     state['exp_avg_sq'] = torch.zeros_like(p)
 
-                if p.dtype not in [torch.float16, torch.float32]:
-                    raise RuntimeError('FusedAdam only support fp16 and fp32.')
+                if p.dtype not in [torch.float16, torch.float32, torch.bfloat16]:
+                    raise RuntimeError('FusedAdam only support fp16, fp32 and bf16.')
 
                 g_l.append(p.grad.data)
                 p_l.append(p.data)
                 m_l.append(state['exp_avg'])
                 v_l.append(state['exp_avg_sq'])
 
             multi_tensor_applier(self.multi_tensor_adam, self._dummy_overflow_buf, [g_l, p_l, m_l, v_l], group['lr'],
```

### Comparing `colossalai-0.3.0/colossalai/nn/optimizer/fused_lamb.py` & `colossalai-0.3.1/colossalai/nn/optimizer/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/optimizer/fused_sgd.py` & `colossalai-0.3.1/colossalai/nn/optimizer/fused_sgd.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/optimizer/hybrid_adam.py` & `colossalai-0.3.1/colossalai/nn/optimizer/hybrid_adam.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from typing import Any, Optional
 
 import torch
+from torch.optim import Adam
 
-from colossalai.kernel.op_builder import CPUAdamBuilder, FusedOptimBuilder
+from colossalai.kernel.op_builder import FusedOptimBuilder
 from colossalai.registry import OPTIMIZERS
 from colossalai.utils import multi_tensor_applier
 
-from .nvme_optimizer import NVMeOptimizer
+from .cpu_adam import CPUAdam
 
 
 @OPTIMIZERS.register_module
-class HybridAdam(NVMeOptimizer):
+class HybridAdam(CPUAdam):
     """Implements Adam algorithm.
 
-    Supports parameters updating on both GPU and CPU, depanding on the device of parameters.
+    Supports parameters updating on both GPU and CPU, depending on the device of parameters.
     But the parameters and gradients should on the same device:
       * Parameters on CPU and gradients on CPU is allowed.
       * Parameters on GPU and gradients on GPU is allowed.
       * Parameters on GPU and gradients on CPU is **not** allowed.
 
     `HybridAdam` requires CUDA extensions which can be built during installation or runtime.
 
@@ -70,23 +71,17 @@
                  eps=1e-8,
                  weight_decay=0,
                  adamw_mode=True,
                  nvme_offload_fraction: float = 0.0,
                  nvme_offload_dir: Optional[str] = None,
                  **defaults: Any):
 
-        default_args = dict(lr=lr, betas=betas, eps=eps, weight_decay=weight_decay, bias_correction=bias_correction)
-        super(HybridAdam, self).__init__(model_params, default_args, nvme_offload_fraction, nvme_offload_dir)
-        self.adamw_mode = adamw_mode
-
-        # build during runtime if not found
-        cpu_optim = CPUAdamBuilder().load()
+        super().__init__(model_params, lr, bias_correction, betas, eps, weight_decay, adamw_mode, nvme_offload_fraction,
+                         nvme_offload_dir)
         fused_optim = FusedOptimBuilder().load()
-        self.cpu_adam_op = cpu_optim.CPUAdamOptimizer(lr, betas[0], betas[1], eps, weight_decay, adamw_mode)
-
         self.gpu_adam_op = fused_optim.multi_tensor_adam
         self._dummy_overflow_buf = torch.cuda.IntTensor([0])
 
     @torch.no_grad()
     def step(self, closure=None, div_scale: float = -1):
         loss = None
         if closure is not None:
@@ -104,31 +99,41 @@
 
                 state = self.state[p]
 
                 target_device = p.device
                 if len(state) == 0:
                     state['step'] = 0
 
+                    # FIXME(ver217): CPU adam kernel only supports fp32 states now
+                    assert p.dtype is torch.float, "HybridAdam only support fp32 parameters"
                     # gradient momentums
-                    state['exp_avg'] = torch.zeros_like(p, dtype=torch.float, device=target_device)
+                    state['exp_avg'] = torch.zeros_like(p, device=target_device)
                     # gradient variances
-                    state['exp_avg_sq'] = torch.zeros_like(p, dtype=torch.float, device=target_device)
+                    state['exp_avg_sq'] = torch.zeros_like(p, device=target_device)
                     self._post_state_init(p)
 
                 state['step'] += 1
                 group_step = state['step']
                 beta1, beta2 = group['betas']
 
                 if target_device.type == 'cpu':
                     assert state['exp_avg'].device.type == 'cpu', "exp_avg should stay on cpu"
                     assert state['exp_avg_sq'].device.type == 'cpu', "exp_avg should stay on cpu"
                     self._pre_update(p, 'exp_avg', 'exp_avg_sq')
-                    self.cpu_adam_op.step(state['step'], group['lr'], beta1, beta2, group['eps'], group['weight_decay'],
-                                          group['bias_correction'], p.data, p.grad.data, state['exp_avg'],
-                                          state['exp_avg_sq'], div_scale)
+                    if p.grad.dtype is torch.bfloat16:
+                        # cpu adam kernel does not support bf16 now
+                        bias_correction1 = 1 - beta1**state['step']
+                        bias_correction2 = 1 - beta2**state['step']
+                        self.torch_adam_update(p.data, p.grad.data, state['exp_avg'], state['exp_avg_sq'], group['lr'],
+                                               beta1, beta2, group['eps'], group['weight_decay'], bias_correction1,
+                                               bias_correction2, self.adamw_mode)
+                    else:
+                        self.cpu_adam_op.step(state['step'], group['lr'], beta1, beta2, group['eps'],
+                                              group['weight_decay'], group['bias_correction'], p.data, p.grad.data,
+                                              state['exp_avg'], state['exp_avg_sq'], div_scale)
                     self._post_update(p, 'exp_avg', 'exp_avg_sq')
 
                 elif target_device.type == 'cuda':
                     assert state['exp_avg'].device.type == 'cuda', "exp_avg should stay on cuda"
                     assert state['exp_avg_sq'].device.type == 'cuda', "exp_avg should stay on cuda"
 
                     # record the state by group and update at once
```

### Comparing `colossalai-0.3.0/colossalai/nn/optimizer/lamb.py` & `colossalai-0.3.1/colossalai/nn/optimizer/lamb.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
         for group in self.param_groups:
             for p in group['params']:
                 if p.grad is None:
                     continue
                 grad = p.grad.data
                 if grad.is_sparse:
-                    raise RuntimeError('Lamb does not support sparse gradients, consider SparseAdam instad.')
+                    raise RuntimeError('Lamb does not support sparse gradients, consider SparseAdam instead.')
 
                 state = self.state[p]
 
                 # State initialization
                 if len(state) == 0:
                     state['step'] = 0
                     # Exponential moving average of gradient values
```

### Comparing `colossalai-0.3.0/colossalai/nn/optimizer/lars.py` & `colossalai-0.3.1/colossalai/nn/optimizer/lars.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/optimizer/nvme_optimizer.py` & `colossalai-0.3.1/colossalai/nn/optimizer/nvme_optimizer.py`

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
-        # As param may be not materialized here, these attributes are initalized when the first step
+        # As param may be not materialized here, these attributes are initialized when the first step
         self.total_numel: Optional[int] = None
         self.can_offload_numel: Optional[int] = None
 
         self.prefetch_params: List[Parameter] = []
         self.param_to_prefetch_idx: Dict[Parameter, int] = {}
 
     def _get_numel(self) -> int:
```

### Comparing `colossalai-0.3.0/colossalai/nn/parallel/data_parallel.py` & `colossalai-0.3.1/colossalai/nn/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/parallel/layers/__init__.py` & `colossalai-0.3.1/colossalai/nn/parallel/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/parallel/layers/cache_embedding/__init__.py` & `colossalai-0.3.1/colossalai/nn/parallel/layers/cache_embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py` & `colossalai-0.3.1/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py` & `colossalai-0.3.1/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py` & `colossalai-0.3.1/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 
 
 class CachedEmbeddingBag(BaseEmbeddingBag):
     """CachedEmbeddingBag
 
     Cached Embedding. Apply a GPU-based software cache approaches to dynamically manage the embedding table in the CPU and GPU memory space.
     It can leverage the id's frequency statistics of the target dataset, by passing a frequency list to param `ids_freq_mapping`.
-    You can also apply a navie LFU cache eviction strategy by setting `evict_strategy` as EvictionStrategy.LFU.
+    You can also apply a naive LFU cache eviction strategy by setting `evict_strategy` as EvictionStrategy.LFU.
 
     Args:
         num_embeddings (int): size of the dictionary of embeddings
         embedding_dim (int):  the size of each embedding vector
         padding_idx (int, optional): If specified, the entries at padding_idx do not contribute to the gradient; therefore, the embedding vector at padding_idx is not updated during training, i.e. it remains as a fixed “pad”. For a newly constructed EmbeddingBag, the embedding vector at padding_idx will default to all zeros, but can be updated to another value to be used as the padding vector. Note that the embedding vector at padding_idx is excluded from the reduction.
         max_norm (float, optional): If given, each embedding vector with norm larger than max_norm is renormalized to have norm max_norm
-        norm_type (str, optional): The p of the p-norm to compute for the max_norm option. Defaults to 2..
+        norm_type (str, optional): The p of the p-norm to compute for the max_norm option. Defaults to 2.
         scale_grad_by_freq (bool, optional): if given, this will scale gradients by the inverse of frequency of the words in the mini-batch. Default False. Note: this option is not supported when mode="max". Defaults to False.
         sparse (bool, optional): if True, gradient w.r.t. weight matrix will be a sparse tensor. See Notes for more details regarding sparse gradients. Note: this option is not supported when mode="max".. Defaults to False.
-        _weight (torch.Tensor, optional): an embedding weight tensor. Concate multiple tables in a embedding bag as a single one. Defaults to None.
+        _weight (torch.Tensor, optional): an embedding weight tensor. Concatenate multiple tables in a embedding bag as a single one. Defaults to None.
         mode (str, optional): "sum", "mean" or "max". Specifies the way to reduce the bag. "sum" computes the weighted sum, taking per_sample_weights into consideration. "mean" computes the average of the values in the bag, "max" computes the max value over each bag. Default: "mean". Defaults to 'mean'.
         include_last_offset (bool, optional): if True, offsets has one additional element, where the last element is equivalent to the size of indices. This matches the CSR format.. Defaults to False.
         dtype (torch.dtype, optional): data type of the cpu weight initialization. Defaults to None meaning float32.
         device (torch.device, optional): device type to the cpu weight. Defaults to None meaning cpu.
         cache_ratio (float, float): cache ratio of the #cuda_weight_row / #cpu_weight_row 
-        ids_freq_mapping (Union[List, torch.Tensor], optional): the frequency of each embedding vector occures in dataset. Defaults to None.
+        ids_freq_mapping (Union[List, torch.Tensor], optional): the frequency of each embedding vector occurs in dataset. Defaults to None.
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
-                   self.cache_weight_mgr._cpu_to_cuda_elpase
+                   self.cache_weight_mgr._cpu_to_cuda_elapse
         else:
             return 0
 
     @property
     def swap_out_bandwidth(self):
         if self.cache_weight_mgr._cuda_to_cpu_numel > 0:
             return self.cache_weight_mgr._cuda_to_cpu_numel * self.cache_weight_mgr.elem_size_in_byte / 1e6 / \
```

### Comparing `colossalai-0.3.0/colossalai/nn/parallel/layers/cache_embedding/copyer.py` & `colossalai-0.3.1/colossalai/nn/parallel/layers/cache_embedding/copyer.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def __init__(self, size: int) -> None:
         self._buff_size = size
 
     @torch.no_grad()
     def index_copy(self, dim: int, src_index: LongTensor, tgt_index: LongTensor, src: torch.Tensor, tgt: torch.Tensor):
         """copy 
         src tensor[src_index] -(index_select)-> tmp -(index_copy_)-> tgt tensor [tgt_index]
-        The valid rows in the src tensor are continous, while rows in tgt tensor is scattered.
+        The valid rows in the src tensor are continuous, while rows in tgt tensor is scattered.
 
         Args:
             dim (int):  dimension along which to index
             src_index (int): indices of src tensor to select from
             tgt_index (int): indices of tgt tensor to select from
             src (torch.Tensor):  the tensor containing values to copy
             tgt (torch.Tensor):  the tensor to be copied
```

### Comparing `colossalai-0.3.0/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py` & `colossalai-0.3.1/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py` & `colossalai-0.3.1/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py` & `colossalai-0.3.1/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py` & `colossalai-0.3.1/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                     local_per_sample_weights = per_sample_weights[indices_start_position:indices_end_position]
             with record_function("(tablewise) tablewise forward"):
                 local_output_list.append(self.cached_embedding_bag_list[i](local_indices, local_offsets,
                                                                            local_per_sample_weights))
 
         # get result of shape = (batch_size, (len(assigned_table_list)*embedding_dim))
         local_output = torch.cat(local_output_list, 1)
-        # then concatenate those local_output on the second demension.
+        # then concatenate those local_output on the second dimension.
         # use all_to_all
         remains = batch_size % self.world_size
         scatter_strides = [batch_size // self.world_size + int(i < remains) for i in range(self.world_size)]
         output_full = dual_all_to_all_tablewise(local_output, self.pg, scatter_strides, self.embedding_dim_per_rank)
         if shape_hook is not None:
             output_full = shape_hook(output_full)
         return output_full
```

### Comparing `colossalai-0.3.0/colossalai/nn/parallel/layers/colo_module.py` & `colossalai-0.3.1/colossalai/nn/parallel/layers/colo_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/parallel/layers/embedding.py` & `colossalai-0.3.1/colossalai/nn/parallel/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/parallel/layers/linear.py` & `colossalai-0.3.1/colossalai/nn/parallel/layers/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/parallel/layers/module_utils.py` & `colossalai-0.3.1/colossalai/nn/parallel/layers/module_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/nn/parallel/reducer.py` & `colossalai-0.3.1/colossalai/nn/parallel/reducer.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/pipeline/layer_spec.py` & `colossalai-0.3.1/colossalai/pipeline/layer_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/pipeline/middleware/adaptor/fx.py` & `colossalai-0.3.1/colossalai/pipeline/middleware/adaptor/fx.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/pipeline/middleware/topo.py` & `colossalai-0.3.1/colossalai/pipeline/middleware/topo.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/pipeline/pipelinable.py` & `colossalai-0.3.1/colossalai/pipeline/pipelinable.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             modified_args.append(arg)
 
         # to the same for the keyword arguments
         modified_kwargs = {}
         for k, v in kwargs.items():
             if isinstance(v, torch.nn.Module):
                 v = self._layer_spec_dict[id(v)]
-            # (lyl)TODO: analyse ColoTensor as well
+            # (lyl)TODO: analyze ColoTensor as well
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
-        If exec_seq is None, we will take the module initizing order as execution order.
+        If exec_seq is None, we will take the module initializing order as execution order.
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
-        Partitioned model will be built respect to partion policy.
+        Partitioned model will be built respect to partition policy.
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
-                ), f'World size is {gpc.get_world_size(ParallelMode.PIPELINE)}, but the number of partions is {len(self.customized_parts)}'
+                ), f'World size is {gpc.get_world_size(ParallelMode.PIPELINE)}, but the number of partitions is {len(self.customized_parts)}'
                 parts = self.customized_parts[rank]
             else:
                 raise ValueError("A string partition policy should be one of ['uniform', 'balanced', 'customized'].")
         elif isinstance(self._policy, dict):
             parts = self._policy[rank]
         else:
             raise ValueError("A partition policy should be either a string or a dictionary.")
```

### Comparing `colossalai-0.3.0/colossalai/pipeline/pipeline_process_group.py` & `colossalai-0.3.1/colossalai/pipeline/pipeline_process_group.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/pipeline/rpc/_pipeline_base.py` & `colossalai-0.3.1/colossalai/pipeline/rpc/_pipeline_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
         if data_process_func is not None:
             self.data_process_func = partial(data_process_func, pp_rank)
 
         self.device = device
         self._initialize_outstanding_range()
 
-        # variable and const for context managment
+        # variable and const for context management
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
-        # construction of partition is executed after the registion of pp_rank_to_worker_rref
+        # construction of partition is executed after the registration of pp_rank_to_worker_rref
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
-                # lock of work_item queue operation gurantees the consistency of lifecycle counter.
+                # lock of work_item queue operation guarantees the consistency of lifecycle counter.
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
-                # lock of work_item queue operation gurantees the consistency of lifecycle counter.
+                # lock of work_item queue operation guarantees the consistency of lifecycle counter.
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
 
-        # should be aranged in order, the order of the input of current forward
+        # should be arranged in order, the order of the input of current forward
         self.producer_stage_ids = self.get_producer_stage_ids()
         self.consumer_stage_ids = self.get_consumer_stage_ids()
 
     def pp_rank_to_partition_id(self, pp_rank: int, topo: Topo):
         partition_ids = topo.get_mid_partition_ids()
         return partition_ids[pp_rank]
```

### Comparing `colossalai-0.3.0/colossalai/pipeline/rpc/_pipeline_schedule.py` & `colossalai-0.3.1/colossalai/pipeline/rpc/_pipeline_schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         rank = self.pp_rank
         min_pp_rank = (rank // self.actual_stage_num) * self.actual_stage_num
         max_pp_rank = min_pp_rank + self.actual_stage_num - 1
 
         assert self.producer_stage_ids is None, f"all the producers of rank {rank} has been subscribed"
         assert self.consumer_stage_ids is None, f"all the consumers of rank {rank} has been subscribed"
 
-        # should be aranged in order, the order of the input of current forward
+        # should be arranged in order, the order of the input of current forward
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
-            # get the coresponding model state dict and wait for its init
+            # get the corresponding model state dict and wait for its init
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
 
-        # if currrent pp_rank is not the first to do step
+        # if current pp_rank is not the first to do step
         # wait its previous pp_rank finish step
         grads = self.get_parameter_gradients()
 
         # send
         co_worker = self.pp_rank_to_worker_rref[co_pp_rank]
         co_grads = co_worker.rpc_sync()._get_lock_gradient()
         # sync
```

### Comparing `colossalai-0.3.0/colossalai/pipeline/rpc/utils.py` & `colossalai-0.3.1/colossalai/pipeline/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/pipeline/utils.py` & `colossalai-0.3.1/colossalai/pipeline/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         intervals = _heap_addition(prefix, intervals, num - num_block)
 
     return intervals
 
 
 def partition_uniform(num_items, pipeline_parallel_size, num_chunks):
     assert num_items % num_chunks == 0, \
-        "Layer length should be divided by the number of chunks, otherwise parameter method is recomended"
+        "Layer length should be divided by the number of chunks, otherwise parameter method is recommended"
 
     logger = get_dist_logger()
     parts = [[] for _ in range(pipeline_parallel_size)]
     partition_items = num_items // num_chunks
     for idx in range(num_chunks):
         base_idx = idx * partition_items
         chunk_size = partition_items // pipeline_parallel_size
```

### Comparing `colossalai-0.3.0/colossalai/registry/__init__.py` & `colossalai-0.3.1/colossalai/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/registry/registry.py` & `colossalai-0.3.1/colossalai/registry/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/tensor/__init__.py` & `colossalai-0.3.1/colossalai/tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/tensor/colo_parameter.py` & `colossalai-0.3.1/colossalai/tensor/colo_parameter.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/tensor/colo_tensor.py` & `colossalai-0.3.1/colossalai/tensor/colo_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/tensor/comm_spec.py` & `colossalai-0.3.1/colossalai/tensor/comm_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,77 +12,74 @@
 ]
 
 
 def _all_gather(tensor, comm_spec):
     '''
     Implement all gather operation on device mesh based on information provided by comm_spec.
     '''
-    process_groups_list = comm_spec.device_mesh.process_groups_dict[comm_spec.logical_process_axis]
-    for rank_list, process_group in process_groups_list:
-        if dist.get_rank() in rank_list:
-            tensor_list = [
-                torch.zeros(tensor.shape, dtype=tensor.dtype, device=tensor.device)
-                for _ in range(comm_spec.device_mesh.mesh_shape[comm_spec.logical_process_axis])
-            ]
-            # without this contiguous operation, the all gather may get some unexpected results.
-            tensor = tensor.contiguous()
-            dist.all_gather(tensor_list, tensor, group=process_group)
-            output = torch.cat(tuple(tensor_list), comm_spec.gather_dim).contiguous()
-            return output
+    process_groups = comm_spec.device_mesh.get_process_group_for_all_axes()
+    process_group = process_groups[comm_spec.logical_process_axis]
+
+    tensor_list = [
+        torch.zeros(tensor.shape, dtype=tensor.dtype, device=tensor.device)
+        for _ in range(comm_spec.device_mesh.shape[comm_spec.logical_process_axis])
+    ]
+    # without this contiguous operation, the all gather may get some unexpected results.
+    tensor = tensor.contiguous()
+    dist.all_gather(tensor_list, tensor, group=process_group)
+    output = torch.cat(tuple(tensor_list), comm_spec.gather_dim).contiguous()
+    return output
 
 
 def _split(tensor, comm_spec):
     '''
     Implement shard operation on device mesh based on information provided by comm_spec.
     '''
-    process_groups_list = comm_spec.device_mesh.process_groups_dict[comm_spec.logical_process_axis]
-    for rank_list, _ in process_groups_list:
-        if dist.get_rank() in rank_list:
-            dim = comm_spec.shard_dim
-            length = tensor.shape[comm_spec.shard_dim] // len(rank_list)
-            start = length * rank_list.index(dist.get_rank())
-            output = torch.narrow(tensor, dim, start, length).contiguous()
-            return output
+    process_groups = comm_spec.device_mesh.get_process_group_for_all_axes()
+    process_group = process_groups[comm_spec.logical_process_axis]
+
+    dim = comm_spec.shard_dim
+    length = tensor.shape[comm_spec.shard_dim] // dist.get_world_size(process_group)
+    start = length * dist.get_rank(process_group)
+    output = torch.narrow(tensor, dim, start, length).contiguous()
+    return output
 
 
 def _all_to_all(tensor, comm_spec):
     '''
     Implement all to all operation on device mesh based on information provided by comm_spec.
     '''
-    process_groups_list = comm_spec.device_mesh.process_groups_dict[comm_spec.logical_process_axis]
-    for rank_list, process_group in process_groups_list:
-        if dist.get_rank() in rank_list:
-            new_shape = list(tensor.shape)
-            new_shape[comm_spec.shard_dim] = new_shape[comm_spec.shard_dim] // len(rank_list)
-            new_shape = torch.Size(new_shape)
-            output_tensor_list = [
-                torch.zeros(new_shape, dtype=tensor.dtype, device=tensor.device) for _ in range(len(rank_list))
-            ]
-            dim = comm_spec.shard_dim
-            length = tensor.shape[comm_spec.shard_dim] // len(rank_list)
-            input_tensor_list = [
-                torch.narrow(tensor, dim, length * i, length).contiguous() for i in range(len(rank_list))
-            ]
-            group = process_group
-            dist.all_to_all(output_tensor_list, input_tensor_list, group)
-            output = torch.cat(tuple(output_tensor_list), comm_spec.gather_dim).contiguous()
-            return output
+    process_groups = comm_spec.device_mesh.get_process_group_for_all_axes()
+    process_group = process_groups[comm_spec.logical_process_axis]
+    world_size = dist.get_world_size(process_group)
+
+    new_shape = list(tensor.shape)
+    new_shape[comm_spec.shard_dim] = new_shape[comm_spec.shard_dim] // world_size
+    new_shape = torch.Size(new_shape)
+    output_tensor_list = [torch.zeros(new_shape, dtype=tensor.dtype, device=tensor.device) for _ in range(world_size)]
+    dim = comm_spec.shard_dim
+    length = tensor.shape[comm_spec.shard_dim] // world_size
+    input_tensor_list = [torch.narrow(tensor, dim, length * i, length).contiguous() for i in range(world_size)]
+    group = process_group
+    dist.all_to_all(output_tensor_list, input_tensor_list, group)
+    output = torch.cat(tuple(output_tensor_list), comm_spec.gather_dim).contiguous()
+    return output
 
 
 def _all_reduce(tensor, comm_spec, async_op=False):
     '''
     Implement all reduce operation on device mesh based on information provided by comm_spec.
     '''
-    process_groups_list = comm_spec.device_mesh.process_groups_dict[comm_spec.logical_process_axis]
-    for rank_list, process_group in process_groups_list:
-        if dist.get_rank() in rank_list:
-            if not tensor.is_contiguous():
-                tensor = tensor.contiguous()
-            dist.all_reduce(tensor, op=ReduceOp.SUM, group=process_group, async_op=async_op)
-            return tensor
+    process_groups = comm_spec.device_mesh.get_process_group_for_all_axes()
+    process_group = process_groups[comm_spec.logical_process_axis]
+
+    if not tensor.is_contiguous():
+        tensor = tensor.contiguous()
+    dist.all_reduce(tensor, op=ReduceOp.SUM, group=process_group, async_op=async_op)
+    return tensor
 
 
 def _mix_gather(tensor, comm_spec):
     '''
     Implement mix gather operation on device mesh based on information provided by comm_spec.
     Mix gather is the all-gather operation on all devices in the device_mesh(FlattenDeviceMesh) of the comm_spec. It is
     different from _all_gather because _mix_gather does all-gather in two dimensions of device mesh, while _all_gather
@@ -124,15 +121,15 @@
     process_group = "[0, 4, 1, 5, 2, 6, 3, 7]"
     tensor_list = [(0,0),(1,0),(2,0),(3,0),(4,0),(5,0),(6,0),(7,0)]
     S01R:
     leading_group_dim = 1
     process_group = "[0, 1, 2, 3, 4, 5, 6, 7]"
     tensor_list = [(0,0),(1,0),(2,0),(3,0),(4,0),(5,0),(6,0),(7,0)]
     '''
-    total_slices = comm_spec.device_mesh.mesh_shape[0]
+    total_slices = comm_spec.device_mesh.shape[0]
     tensor_list = [torch.zeros(tensor.shape, dtype=tensor.dtype, device=tensor.device) for _ in range(total_slices)]
     leading_group_dim = comm_spec.logical_process_axes[0]
     assert len(comm_spec.device_mesh.process_groups_dict) == 1
     _, process_group = comm_spec.device_mesh.process_groups_dict[0][0]
     process_number_list = comm_spec.device_meshes.process_number_dict[leading_group_dim]
 
     # Global all_gather
@@ -145,15 +142,15 @@
     for i in range(total_slices):
         tensor_list_sorted[i] = tensor_list[process_number_list[i]]
     tensor_list = tensor_list_sorted
 
     if comm_spec.logical_process_axes[0] == comm_spec.logical_process_axes[1]:
         output = torch.cat(tuple(tensor_list), comm_spec.gather_dim[0]).contiguous()
     else:
-        mesh_shape = comm_spec.device_meshes.mesh_shape
+        mesh_shape = comm_spec.device_meshes.shape
         cat_slice = [mesh_shape[comm_spec.logical_process_axes[0]], mesh_shape[comm_spec.logical_process_axes[1]]]
         tmp_tensor_shape = list(tensor.shape)
         tmp_tensor_shape[comm_spec.gather_dim[0]] *= cat_slice[0]
         tmp_tensor_shape = torch.Size(tmp_tensor_shape)
         tmp_tensor_list = [
             torch.zeros(tmp_tensor_shape, dtype=tensor.dtype, device=tensor.device) for _ in range(cat_slice[1])
         ]
@@ -177,17 +174,17 @@
     RS01 => [b], (0, 0)
     Example:
     mesh_shape = (2,4)
             # [[0, 1, 2, 3],
             #  [4, 5, 6, 7]]
             # return {0: [0, 4, 1, 5, 2, 6, 3, 7], 1: [0, 1, 2, 3, 4, 5, 6, 7]}
     '''
-    mesh_shape = comm_spec.device_meshes.mesh_shape
+    mesh_shape = comm_spec.device_meshes.shape
     dim = comm_spec.gather_dim
-    total_slices = comm_spec.device_mesh.mesh_shape[0]
+    total_slices = comm_spec.device_mesh.shape[0]
 
     # Get global rank
     rank = dist.get_rank()
 
     leading_group_dim = comm_spec.logical_process_axes[0]
     process_number_list = comm_spec.device_meshes.process_number_dict[leading_group_dim]
     rank = process_number_list.index(rank)
@@ -410,15 +407,15 @@
         self.sharding_spec = sharding_spec
         self.gather_dim = gather_dim
         self.shard_dim = shard_dim
         self.logical_process_axis = logical_process_axis
         self.forward_only = forward_only
         if isinstance(self.logical_process_axis, list):
             if not mix_gather:
-                self.device_mesh = self.sharding_spec.device_mesh.flatten_device_mesh
+                self.device_mesh = self.sharding_spec.device_mesh.flatten()
                 self.logical_process_axis = 0
             else:
                 self.device_meshes = self.sharding_spec.device_mesh.flatten_device_meshes
                 self.device_mesh = self.sharding_spec.device_mesh.flatten_device_mesh
                 # Create a new member `logical_process_axes` to distinguish from original flatten
                 self.logical_process_axes = logical_process_axis
         else:
```

### Comparing `colossalai-0.3.0/colossalai/tensor/compute_spec.py` & `colossalai-0.3.1/colossalai/tensor/compute_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/tensor/d_tensor/comm_spec.py` & `colossalai-0.3.1/colossalai/tensor/d_tensor/comm_spec.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,36 +20,36 @@
     MIXGATHER_FWD_SPLIT_BWD = "mixgather_fwd_split_bwd"
 
 
 class CommSpec:
     '''
     Communication spec is used to record the communication action. It converts the communication spec
     to real action which will be used in runtime. It contains comm_pattern to determine the
-    communication method, process_groups_dict to determine the process groups, gather_dim and shard_dim
+    communication method, process_group_dict to determine the process groups, gather_dim and shard_dim
     to determine the buffer shape, and logical_process_axis
 
     Argument:
         comm_pattern(CollectiveCommPattern): decribe the communication method used in this spec.
-        process_groups_dict(Dict): A dict which contains the process groups used to apply this CommSpec.
+        process_group_dict(Dict): A dict which contains the process groups used to apply this CommSpec.
         gather_dim(int, Optional): The gather_dim of the tensor will be gathered.
         shard_dim(int, Optional): The shard_dim of the tensor will be sharded.
         logical_process_axis(Union(int, List[int]), Optional): The mesh_dim to implement the communication action.
     '''
 
     def __init__(self,
                  comm_pattern: CollectiveCommPattern,
-                 process_groups_dict: Dict,
+                 process_group_dict: Dict,
                  gather_dim: int = None,
                  shard_dim: int = None,
                  logical_process_axis: int = None):
         self.comm_pattern = comm_pattern
         self.gather_dim = gather_dim
         self.shard_dim = shard_dim
         self.logical_process_axis = logical_process_axis
-        self.process_groups_dict = process_groups_dict
+        self.process_group_dict = process_group_dict
 
     def __repr__(self):
         res_list = ["CommSpec:("]
         if self.comm_pattern == CollectiveCommPattern.GATHER_FWD_SPLIT_BWD:
             res_list.append(f"comm_pattern:GATHER_FWD_SPLIT_BWD, ")
             res_list.append(f"gather_dim:{self.gather_dim}, ")
             res_list.append(f"shard_dim:{self.gather_dim}, ")
@@ -88,76 +88,64 @@
         return tensor
 
 
 def _all_gather(tensor: torch.Tensor, comm_spec: CommSpec):
     '''
     Implement all gather operation on device mesh based on information provided by comm_spec.
     '''
-    process_groups_list = comm_spec.process_groups_dict[comm_spec.logical_process_axis]
-    for rank_list, process_group in process_groups_list:
-        if dist.get_rank() in rank_list:
-            tensor_list = [
-                torch.zeros(tensor.shape, dtype=tensor.dtype, device=tensor.device) for _ in range(len(rank_list))
-            ]
-            # without this contiguous operation, the all gather may get some unexpected results.
-            tensor = tensor.contiguous()
-            dist.all_gather(tensor_list, tensor, group=process_group)
-            output = torch.cat(tuple(tensor_list), comm_spec.gather_dim).contiguous()
-            return output
+    process_group = comm_spec.process_group_dict[comm_spec.logical_process_axis]
+    world_size = dist.get_world_size(process_group)
+    tensor_list = [torch.zeros(tensor.shape, dtype=tensor.dtype, device=tensor.device) for _ in range(world_size)]
+    # without this contiguous operation, the all gather may get some unexpected results.
+    tensor = tensor.contiguous()
+    dist.all_gather(tensor_list, tensor, group=process_group)
+    output = torch.cat(tuple(tensor_list), comm_spec.gather_dim).contiguous()
+    return output
 
 
 def _split(tensor: torch.Tensor, comm_spec: CommSpec):
     '''
     Implement shard operation on device mesh based on information provided by comm_spec.
     '''
-    process_groups_list = comm_spec.process_groups_dict[comm_spec.logical_process_axis]
-    for rank_list, _ in process_groups_list:
-        if dist.get_rank() in rank_list:
-            dim = comm_spec.shard_dim
-            length = tensor.shape[comm_spec.shard_dim] // len(rank_list)
-            start = length * rank_list.index(dist.get_rank())
-            output = torch.narrow(tensor, dim, start, length).contiguous()
-            return output
+    process_group = comm_spec.process_group_dict[comm_spec.logical_process_axis]
+    dim = comm_spec.shard_dim
+    length = tensor.shape[comm_spec.shard_dim] // dist.get_world_size(process_group)
+    start = length * dist.get_rank(process_group)
+    output = torch.narrow(tensor, dim, start, length).contiguous()
+    return output
 
 
 def _all_to_all(tensor: torch.Tensor, comm_spec: CommSpec):
     '''
     Implement all to all operation on device mesh based on information provided by comm_spec.
     '''
-    process_groups_list = comm_spec.process_groups_dict[comm_spec.logical_process_axis]
-    for rank_list, process_group in process_groups_list:
-        if dist.get_rank() in rank_list:
-            new_shape = list(tensor.shape)
-            new_shape[comm_spec.shard_dim] = new_shape[comm_spec.shard_dim] // len(rank_list)
-            new_shape = torch.Size(new_shape)
-            output_tensor_list = [
-                torch.zeros(new_shape, dtype=tensor.dtype, device=tensor.device) for _ in range(len(rank_list))
-            ]
-            dim = comm_spec.shard_dim
-            length = tensor.shape[comm_spec.shard_dim] // len(rank_list)
-            input_tensor_list = [
-                torch.narrow(tensor, dim, length * i, length).contiguous() for i in range(len(rank_list))
-            ]
-            group = process_group
-            dist.all_to_all(output_tensor_list, input_tensor_list, group)
-            output = torch.cat(tuple(output_tensor_list), comm_spec.gather_dim).contiguous()
-            return output
+    process_group = comm_spec.process_group_dict[comm_spec.logical_process_axis]
+    world_size = dist.get_world_size(process_group)
+    new_shape = list(tensor.shape)
+    new_shape[comm_spec.shard_dim] = new_shape[comm_spec.shard_dim] // world_size
+    new_shape = torch.Size(new_shape)
+    output_tensor_list = [torch.zeros(new_shape, dtype=tensor.dtype, device=tensor.device) for _ in range(world_size)]
+    dim = comm_spec.shard_dim
+    length = tensor.shape[comm_spec.shard_dim] // world_size
+    input_tensor_list = [torch.narrow(tensor, dim, length * i, length).contiguous() for i in range(world_size)]
+    group = process_group
+    dist.all_to_all(output_tensor_list, input_tensor_list, group)
+    output = torch.cat(tuple(output_tensor_list), comm_spec.gather_dim).contiguous()
+    return output
 
 
 def _all_reduce(tensor: torch.Tensor, comm_spec: CommSpec, async_op: bool = False):
     '''
     Implement all reduce operation on device mesh based on information provided by comm_spec.
     '''
-    process_groups_list = comm_spec.process_groups_dict[comm_spec.logical_process_axis]
-    for rank_list, process_group in process_groups_list:
-        if dist.get_rank() in rank_list:
-            if not tensor.is_contiguous():
-                tensor = tensor.contiguous()
-            dist.all_reduce(tensor, op=ReduceOp.SUM, group=process_group, async_op=async_op)
-            return tensor
+    process_group = comm_spec.process_group_dict[comm_spec.logical_process_axis]
+    if not tensor.is_contiguous():
+        tensor = tensor.contiguous()
+    dist.all_reduce(tensor, op=ReduceOp.SUM, group=process_group, async_op=async_op)
+    return tensor
 
 
 class _ReduceGrad(torch.autograd.Function):
     """
     A customized communication operation which forward is an identity operation,
     backward is all_reduce operation.
 
@@ -265,15 +253,15 @@
     def symbolic(graph, input_):
         return _all_to_all(input_)
 
     @staticmethod
     def forward(ctx, input_, comm_spec):
         output = _all_to_all(input_, comm_spec)
         comm_spec_for_backward = CommSpec(comm_pattern=comm_spec.comm_pattern,
-                                          process_groups_dict=comm_spec.process_groups_dict,
+                                          process_group_dict=comm_spec.process_group_dict,
                                           gather_dim=comm_spec.shard_dim,
                                           shard_dim=comm_spec.gather_dim,
                                           logical_process_axis=comm_spec.logical_process_axis)
         ctx.comm_spec = comm_spec_for_backward
         return output
 
     @staticmethod
```

### Comparing `colossalai-0.3.0/colossalai/tensor/d_tensor/layout.py` & `colossalai-0.3.1/colossalai/tensor/d_tensor/layout.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,65 @@
 import operator
-from dataclasses import dataclass
 from functools import reduce
 
 import torch
 
 from colossalai.device.device_mesh import DeviceMesh
 
-from .misc import DuplicatedShardingDimensionError, LayoutException, ShardingNotDivisibleError
+from .misc import DuplicatedShardingDimensionError, ShardingNotDivisibleError
 from .sharding_spec import ShardingSpec
 
 
 class Layout:
     """Layout of a tensor.
 
     Attributes:
         device_mesh: the device mesh to store the tensor distributed.
-        device_type: the type of the device mesh, e.g. 'cpu' or 'cuda'.
         sharding_spec: the sharding specification to describe how the tensor is sharded.
-        entire_shape: the entire shape of the global tensor.
+        global_shape: the entire shape of the global tensor.
     """
 
-    def __init__(self, device_mesh: DeviceMesh, device_type: torch.device, sharding_spec: ShardingSpec,
-                 entire_shape: torch.Size):
+    def __init__(self, device_mesh: DeviceMesh, sharding_spec: ShardingSpec, global_shape: torch.Size):
         self.device_mesh = device_mesh
-        self.device_type = device_type
         self.sharding_spec = sharding_spec
-        self.entire_shape = entire_shape
+        self.global_shape = global_shape
         self._sanity_check()
 
     def __hash__(self) -> int:
         return hash(f'{self.sharding_spec}')
 
     def get_sharded_shape_per_device(self):
-        sharded_shape = list(self.entire_shape)
+        sharded_shape = list(self.global_shape)
         for dim, shard_list in self.sharding_spec.dim_partition_dict.items():
-            mesh_list = [self.device_mesh.mesh_shape[mesh_dim] for mesh_dim in shard_list]
+            mesh_list = [self.device_mesh.shape[mesh_dim] for mesh_dim in shard_list]
             shard_partitions = reduce(operator.mul, mesh_list, 1)
             assert sharded_shape[
                 dim] % shard_partitions == 0, f'Cannot shard dimension {dim} into {shard_partitions} partitions.'
             sharded_shape[dim] //= shard_partitions
         return torch.Size(sharded_shape)
 
     def _sanity_check(self):
         sharding_spec = self.sharding_spec
 
         # make sure all axes in logical device mesh only be used once
-        dim_check_list = list(range(self.device_mesh.logical_mesh_id.dim()))
-        for dim, shard_list in sharding_spec.dim_partition_dict.items():
-            for element in shard_list:
-                if element in dim_check_list:
-                    dim_check_list.remove(element)
-                else:
-                    raise DuplicatedShardingDimensionError(
-                        f"find an invalid sharding axis {element} in dim_partition_dict in tensor dimension {dim}.")
+        if self.device_mesh.logical_mesh_id is not None:
+            dim_check_list = list(range(self.device_mesh.logical_mesh_id.dim()))
+            for dim, shard_list in sharding_spec.dim_partition_dict.items():
+                for element in shard_list:
+                    if element in dim_check_list:
+                        dim_check_list.remove(element)
+                    else:
+                        raise DuplicatedShardingDimensionError(
+                            f"find an invalid sharding axis {element} in dim_partition_dict in tensor dimension {dim}.")
 
         # make sure that the sharding for a dimension is divisible by the number of devices
         for dim, shard_list in sharding_spec.dim_partition_dict.items():
-            tensor_dim_size = self.entire_shape[dim]
+            tensor_dim_size = self.global_shape[dim]
             num_devices = 1
 
             for element in shard_list:
-                num_devices *= self.device_mesh.mesh_shape[element]
+                num_devices *= self.device_mesh.shape[element]
 
             if tensor_dim_size % num_devices != 0:
                 raise ShardingNotDivisibleError(
                     f'The size of dimension at index {dim} is {tensor_dim_size}, it cannot be sharded over {num_devices} devices.'
                 )
```

### Comparing `colossalai-0.3.0/colossalai/tensor/d_tensor/layout_converter.py` & `colossalai-0.3.1/colossalai/tensor/d_tensor/layout_converter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import math
 from copy import deepcopy
 from dataclasses import dataclass
 from typing import Dict, List, Tuple
 
-import numpy as np
 import torch
 
-from colossalai.auto_parallel.tensor_shard.sharding_strategy import MemoryCost, TrainCycleItem
 from colossalai.context.singleton_meta import SingletonMeta
 from colossalai.tensor.d_tensor.comm_spec import *
 from colossalai.tensor.d_tensor.layout import Layout
 from colossalai.tensor.d_tensor.misc import LayoutException
 from colossalai.tensor.utils import all_gather_simulator, all_to_all_simulator, shard_simulator
 
 from .sharding_spec import ShardingSpec
@@ -24,35 +22,26 @@
     """
     LayoutConverterOptions is a dataclass which specifies the preferences for layout converting.
     """
     # TODO: layout converter option is not implemented yet
     pass
 
 
-def to_global(distributed_tensor: torch.Tensor, layout: Layout) -> torch.Tensor:
-    layout_converter = LayoutConverter()
-    global_sharding_spec = ShardingSpec(distributed_tensor.dim(), {})
-    global_layout = Layout(device_mesh=layout.device_mesh,
-                           device_type=layout.device_type,
-                           sharding_spec=global_sharding_spec,
-                           entire_shape=layout.entire_shape)
-    with torch.no_grad():
-        global_tensor = layout_converter.apply(distributed_tensor, layout, global_layout)
-    return global_tensor
-
-
 def set_layout_converting_options(options: LayoutConverterOptions):
     """
     Configure the shape consistency manager via function call.
     """
     manager = LayoutConverter()
     manager.options = options
 
 
 class LayoutConverter(metaclass=SingletonMeta):
+    """
+    LayoutConverter is a singleton class which converts the layout of a distributed tensor.
+    """
 
     def __init__(self):
         self._options = None
         self._forward_only = False
         self.cached_solution = {}
 
     @property
@@ -87,36 +76,40 @@
         Example:
             layout_converter = LayoutConverter()
             physical_mesh_id = torch.arange(0, 4)
             mesh_shape = (2, 2)
             # [[0, 1,
             #  [2, 3]]
             device_mesh = DeviceMesh(physical_mesh_id, mesh_shape, init_process_group=True)
-            entire_shape = (4, 4, 4)
+            global_shape = (4, 4, 4)
             dim_partition_dict = {0: [0], 1: [1]}
 
             # [S0,S1,R]
             sharding_spec = ShardingSpec(dim_size=3, dim_partition_dict=dim_partition_dict)
             layout = Layout(device_mesh=device_mesh,
-                            device_type=torch.device('cuda'),
                             sharding_spec=sharding_spec,
-                            entire_shape=entire_shape)
+                            global_shape=global_shape)
 
             rst_dict = layout_converter.all_gather_transform_layouts(layout)
             for layout, comm_spec in rst_dict.items():
                 print(f'{layout.sharding_spec.sharding_sequence}: {comm_spec}')
 
         Output:
             [R, S1, R]: CommSpec:(comm_pattern:GATHER_FWD_SPLIT_BWD, gather_dim:0, shard_dim:0, logical_process_axis:0)
             [S0, R, R]: CommSpec:(comm_pattern:GATHER_FWD_SPLIT_BWD, gather_dim:1, shard_dim:1, logical_process_axis:1)
         '''
         valid_spec_dict = {}
         comm_pattern = CollectiveCommPattern.GATHER_FWD_SPLIT_BWD
         source_spec = source_layout.sharding_spec
-        process_groups_dict = source_layout.device_mesh.process_groups_dict
+
+        # the key of the dict is the axis
+        # the value is the process group
+        current_rank = source_layout.device_mesh._global_rank_of_current_process
+        process_group_dict = source_layout.device_mesh._process_group_dict[current_rank]
+
         for target_pair in source_spec.dim_partition_dict.items():
             shard_list = all_gather_simulator(target_pair)
             index = target_pair[0]
             new_dim_partition_dict = deepcopy(source_spec.dim_partition_dict)
 
             # We won't add empty list into dim_partition_dict
             # The key will be popped if the related shard_list is empty
@@ -126,27 +119,26 @@
                 new_dim_partition_dict.pop(index)
 
             # generate the CommSpec to record the action of source_sharding_spec->new_sharding_spec
             gather_dim = index
             logical_process_axis = target_pair[1][-1]
             comm_spec = CommSpec(
                 comm_pattern,
-                process_groups_dict=process_groups_dict,
+                process_group_dict=process_group_dict,
                 gather_dim=gather_dim,
             # shard_dim will be used during backward
                 shard_dim=gather_dim,
                 logical_process_axis=logical_process_axis)
 
             # generate new sharding spec
             try:
                 new_sharding_spec = ShardingSpec(source_spec.dims, dim_partition_dict=new_dim_partition_dict)
                 new_layout = Layout(device_mesh=source_layout.device_mesh,
                                     sharding_spec=new_sharding_spec,
-                                    device_type=source_layout.device_type,
-                                    entire_shape=source_layout.entire_shape)
+                                    global_shape=source_layout.global_shape)
 
                 valid_spec_dict[new_layout] = comm_spec
             except LayoutException:
                 pass
         return valid_spec_dict
 
     def all_to_all_transform_layout(self, source_layout: Layout) -> Dict[Layout, CommSpec]:
@@ -163,36 +155,40 @@
         Example:
             layout_converter = LayoutConverter()
             physical_mesh_id = torch.arange(0, 4)
             mesh_shape = (2, 2)
             # [[0, 1,
             #  [2, 3]]
             device_mesh = DeviceMesh(physical_mesh_id, mesh_shape, init_process_group=True)
-            entire_shape = (4, 4, 4)
+            global_shape = (4, 4, 4)
             dim_partition_dict = {0: [0], 1: [1]}
 
             # [S0,S1,R]
             sharding_spec = ShardingSpec(dim_size=3, dim_partition_dict=dim_partition_dict)
             layout = Layout(device_mesh=device_mesh,
-                                    device_type=torch.device('cuda'),
                                     sharding_spec=sharding_spec,
-                                    entire_shape=entire_shape)
+                                    global_shape=global_shape)
             rst_dict = layout_converter.all_to_all_transform_layout(layout)
 
             for layout, comm_spec in rst_dict.items():
                 print(f'{layout.sharding_spec.sharding_sequence}: {comm_spec}')
 
         Output:
             [S01, R, R]: CommSpec:(comm_pattern:ALL2ALL_FWD_ALL2ALL_BWD, gather_dim:1, shard_dim:0, logical_process_axis: 1)
             [R, S1, S0]: CommSpec:(comm_pattern:ALL2ALL_FWD_ALL2ALL_BWD, gather_dim:0, shard_dim:2, logical_process_axis: 0)
             [S0, R, S1]: CommSpec:(comm_pattern:ALL2ALL_FWD_ALL2ALL_BWD, gather_dim:1, shard_dim:2, logical_process_axis: 1)
         '''
         valid_spec_dict = {}
         comm_pattern = CollectiveCommPattern.ALL2ALL_FWD_ALL2ALL_BWD
-        process_groups_dict = source_layout.device_mesh.process_groups_dict
+
+        # the key of the dict is the axis
+        # the value is the process group
+        current_rank = source_layout.device_mesh._global_rank_of_current_process
+        process_group_dict = source_layout.device_mesh._process_group_dict[current_rank]
+
         source_spec = source_layout.sharding_spec
         tensor_dims = source_spec.dims
         for f_index in range(tensor_dims - 1):
             for b_index in range(f_index + 1, tensor_dims):
                 # skip (R, R) cases
                 if f_index not in source_spec.dim_partition_dict and b_index not in source_spec.dim_partition_dict:
                     continue
@@ -225,15 +221,15 @@
                     shard_dim = b_index
                     logical_process_axis = f_target_pair[1][-1]
                 else:
                     gather_dim = b_index
                     shard_dim = f_index
                     logical_process_axis = b_target_pair[1][-1]
                 comm_spec = CommSpec(comm_pattern,
-                                     process_groups_dict,
+                                     process_group_dict=process_group_dict,
                                      gather_dim=gather_dim,
                                      shard_dim=shard_dim,
                                      logical_process_axis=logical_process_axis)
 
                 new_dim_partition_dict = deepcopy(source_spec.dim_partition_dict)
 
                 # We won't add empty list into dim_partition_dict
@@ -248,16 +244,15 @@
                     new_dim_partition_dict.pop(b_index)
 
                 # generate new sharding spec
                 try:
                     new_sharding_spec = ShardingSpec(source_spec.dims, dim_partition_dict=new_dim_partition_dict)
                     new_layout = Layout(device_mesh=source_layout.device_mesh,
                                         sharding_spec=new_sharding_spec,
-                                        device_type=source_layout.device_type,
-                                        entire_shape=source_layout.entire_shape)
+                                        global_shape=source_layout.global_shape)
                     valid_spec_dict[new_layout] = comm_spec
                 except LayoutException:
                     pass
 
         return valid_spec_dict
 
     def shard_transform_layout(self, source_layout: Layout) -> Dict[Layout, CommSpec]:
@@ -274,41 +269,44 @@
         Example:
             layout_converter = LayoutConverter()
             physical_mesh_id = torch.arange(0, 4)
             mesh_shape = (2, 2)
             # [[0, 1,
             #  [2, 3]]
             device_mesh = DeviceMesh(physical_mesh_id, mesh_shape, init_process_group=True)
-            entire_shape = (4, 4, 4)
+            global_shape = (4, 4, 4)
 
             dim_partition_dict = {0: [0]}
 
             # [S0,R,R]
             sharding_spec = ShardingSpec(dim_size=3, dim_partition_dict=dim_partition_dict)
             layout = Layout(device_mesh=device_mesh,
-                          device_type=torch.device('cuda'),
                           sharding_spec=sharding_spec,
-                          entire_shape=entire_shape)
+                          global_shape=global_shape)
             rst_dict = layout_converter.shard_transform_layout(layout)
 
             for layout, comm_spec in rst_dict.items():
                 print(f'{layout.sharding_spec.sharding_sequence}: {comm_spec}')
 
         Output:
             [S01, R, R]: CommSpec:(comm_pattern:SPLIT_FWD_GATHER_BWD, gather_dim:0, shard_dim:0, logical_process_axis:1)
             [S0, S1, R]: CommSpec:(comm_pattern:SPLIT_FWD_GATHER_BWD, gather_dim:1, shard_dim:1, logical_process_axis:1)
             [S0, R, S1]: CommSpec:(comm_pattern:SPLIT_FWD_GATHER_BWD, gather_dim:2, shard_dim:2, logical_process_axis:1)
         '''
         valid_spec_dict = {}
         comm_pattern = CollectiveCommPattern.SPLIT_FWD_GATHER_BWD
         source_spec = source_layout.sharding_spec
-        process_groups_dict = source_layout.device_mesh.process_groups_dict
+
+        # the key of the dict is the axis
+        # the value is the process group
+        current_rank = source_layout.device_mesh._global_rank_of_current_process
+        process_group_dict = source_layout.device_mesh._process_group_dict[current_rank]
 
         # legal sharding dims means the mesh_id is still available to use.
-        legal_sharding_dims = [i for i in range(len(source_layout.device_mesh.mesh_shape))]
+        legal_sharding_dims = [i for i in range(len(source_layout.device_mesh.shape))]
         for dim, shard_list in source_spec.dim_partition_dict.items():
             for element in shard_list:
                 legal_sharding_dims.remove(element)
 
         if len(legal_sharding_dims) == 0:
             return valid_spec_dict
 
@@ -325,27 +323,26 @@
                 new_dim_partition_dict = deepcopy(source_spec.dim_partition_dict)
                 new_dim_partition_dict[index] = shard_list
 
                 # generate the CommSpec to record the action of source_sharding_spec->new_sharding_spec
                 shard_dim = index
                 logical_process_axis = shard_list[-1]
                 comm_spec = CommSpec(comm_pattern,
-                                     process_groups_dict,
+                                     process_group_dict=process_group_dict,
                                      gather_dim=shard_dim,
                                      shard_dim=shard_dim,
                                      logical_process_axis=logical_process_axis)
 
                 # generate new sharding spec
                 try:
                     new_sharding_spec = ShardingSpec(dim_size=source_spec.dims,
                                                      dim_partition_dict=new_dim_partition_dict)
                     new_layout = Layout(device_mesh=source_layout.device_mesh,
                                         sharding_spec=new_sharding_spec,
-                                        device_type=source_layout.device_type,
-                                        entire_shape=source_layout.entire_shape)
+                                        global_shape=source_layout.global_shape)
                     valid_spec_dict[new_layout] = comm_spec
                 except LayoutException:
                     pass
         return valid_spec_dict
 
     def get_all_one_step_transform_spec(self, source_layout: Layout) -> Dict[Layout, CommSpec]:
         '''
@@ -395,32 +392,30 @@
 
         Example:
             physical_mesh_id = torch.arange(0, 4)
             mesh_shape = (2, 2)
             # [[0, 1,
             #  [2, 3]]
             device_mesh = DeviceMesh(physical_mesh_id, mesh_shape, init_process_group=True)
-            entire_shape = (4, 4, 4)
+            global_shape = (4, 4, 4)
 
             dim_partition_source = {1: [0, 1]}
             dim_partition_target = {0: [0, 1]}
 
             # [R,S01,R]
             sharding_spec_source = ShardingSpec(dim_size=3, dim_partition_dict=dim_partition_source)
             source_layout = Layout(device_mesh=device_mesh,
-                                device_type=torch.device('cuda'),
                                 sharding_spec=sharding_spec_source,
-                                entire_shape=entire_shape)
+                                global_shape=global_shape)
 
             # [S01,R,R]
             sharding_spec_target = ShardingSpec(dim_size=3, dim_partition_dict=dim_partition_target)
             target_layout = Layout(device_mesh=device_mesh,
-                                device_type=torch.device('cuda'),
                                 sharding_spec=sharding_spec_target,
-                                entire_shape=entire_shape)
+                                global_shape=global_shape)
 
             transform_path, comm_action_sequence = layout_converter.layout_converting(source_layout, target_layout)
             transform_path_str = '->'.join([str(layout.sharding_spec.sharding_sequence) for layout in transform_path])
             print(transform_path_str)
 
         output:
             [R, S01, R]->[R, S0, R]->[S0, R, R]->[S01, R, R]
@@ -501,29 +496,27 @@
             dim_partition_source = {0: [0]}
             dim_partition_target = {1: [0]}
             physical_mesh_id = torch.arange(0, 4)
             mesh_shape = (2, 2)
             # [[0, 1,
             #  [2, 3]]
             device_mesh = DeviceMesh(physical_mesh_id, mesh_shape, init_process_group=True)
-            entire_shape = (4, 4, 4)
+            global_shape = (4, 4, 4)
 
             # [S0,R,R]
             sharding_spec_source = ShardingSpec(dim_size=3, dim_partition_dict=dim_partition_source)
             source_layout = Layout(device_mesh=device_mesh,
-                                device_type=torch.device('cuda'),
                                 sharding_spec=sharding_spec_source,
-                                entire_shape=entire_shape)
+                                global_shape=global_shape)
 
             # [R,S0,R]
             sharding_spec_target = ShardingSpec(dim_size=3, dim_partition_dict=dim_partition_target)
             target_layout = Layout(device_mesh=device_mesh,
-                                device_type=torch.device('cuda'),
                                 sharding_spec=sharding_spec_target,
-                                entire_shape=entire_shape)
+                                global_shape=global_shape)
 
             if rank in (0, 1):
                 sharded_tensor_0 = torch.zeros(2, 1)
                 sharded_tensor_1 = torch.ones(2, 1)
                 # tensor([[0., 1.],
                 #         [0., 1.]])
                 tensor_to_comm = torch.cat((sharded_tensor_0, sharded_tensor_1), 1).cuda()
@@ -549,8 +542,9 @@
                     [1.],
                     [3.],
                     [3.]])
         '''
         _, comm_action_sequence = self.layout_converting(source_layout, target_layout)
         for comm_spec in comm_action_sequence:
             tensor = comm_spec.covert_spec_to_action(tensor)
+        tensor.dist_layout = target_layout
         return tensor
```

### Comparing `colossalai-0.3.0/colossalai/tensor/d_tensor/sharding_spec.py` & `colossalai-0.3.1/colossalai/tensor/d_tensor/sharding_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         target = 'S'
         for dim in self.shard_list:
             target += str(dim)
         return target
 
     def _convert_str_to_shard_list(self, str_spec):
         '''
-        Conver str_spec into shard_list.
+        Convert str_spec into shard_list.
 
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
-        Build a difference maping for 2D device mesh case. It will be used to
+        Build a difference mapping for 2D device mesh case. It will be used to
         compute the difference between DimSpec pairs.
         '''
 
         source_spec_list = ['R', 'S0', 'S1', 'S01']
         target_spec_list = ['R', 'S0', 'S1', 'S01']
         difference_dict = {}
         for source_spec in source_spec_list:
```

### Comparing `colossalai-0.3.0/colossalai/tensor/d_tensor/utils.py` & `colossalai-0.3.1/colossalai/tensor/d_tensor/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     logical_process_axis = comm_spec.logical_process_axis
     cost_dict = {}
 
     if comm_pattern == CollectiveCommPattern.GATHER_FWD_SPLIT_BWD:
         # the comm size for all gather is the size of the gathered tensor
         gather_dim = comm_spec.gather_dim
         all_gather_axis = layout.sharding_spec.dim_partition_dict[gather_dim][-1]
-        all_gather_size = device_mesh.mesh_shape[all_gather_axis]
+        all_gather_size = device_mesh.shape[all_gather_axis]
         comm_size_for_all_gather = comm_size * all_gather_size
         forward_communication_cost = device_mesh.all_gather_cost(comm_size_for_all_gather, logical_process_axis)
         # give a tiny cost to shard
         backward_communication_cost = 100
 
     if comm_pattern == CollectiveCommPattern.ALL2ALL_FWD_ALL2ALL_BWD:
         forward_communication_cost = device_mesh.all_to_all_cost(comm_size, logical_process_axis)
```

### Comparing `colossalai-0.3.0/colossalai/tensor/dist_spec_mgr.py` & `colossalai-0.3.1/colossalai/tensor/dist_spec_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/tensor/distspec.py` & `colossalai-0.3.1/colossalai/tensor/distspec.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/tensor/op_wrapper.py` & `colossalai-0.3.1/colossalai/tensor/op_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/tensor/param_op_hook.py` & `colossalai-0.3.1/colossalai/tensor/param_op_hook.py`

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
-    # otherwise, the first arguement should be a tuple of grad tensors
+    # otherwise, the first argument should be a tuple of grad tensors
     # if there is no grad tensor, the backward of PreFwdPostBwd can't be triggered
     arg_zero = args[0]
     if not isinstance(arg_zero, tuple):
         raise NotImplementedError("Some torch function is incompatible because of its complicated inputs.")
     check_grad_flag = False
     for obj in arg_zero:
         check_grad_flag |= _is_grad_tensor(obj)
```

### Comparing `colossalai-0.3.0/colossalai/tensor/process_group.py` & `colossalai-0.3.1/colossalai/tensor/process_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
             PYTORCHPGDICT_.get(j_dp_list, 'gloo')
 
         self._has_cpu_groups = True
 
     @property
     def has_cpu_groups(self) -> bool:
         """has_cpu_groups
-        If cpu groups have been initailized.
+        If cpu groups have been initialized.
 
         Returns:
             bool: cpu process groups have been initialized or not.
         """
         return self._has_cpu_groups
 
     def __repr__(self):
```

### Comparing `colossalai-0.3.0/colossalai/tensor/shape_consistency.py` & `colossalai-0.3.1/colossalai/tensor/shape_consistency.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,15 @@
                     pass
 
         return valid_spec_dict
 
     def get_all_shard_spec(self, source_spec: ShardingSpec, orig_cost_dict):
         '''
         Get all valid sharding specs from source_spec with single shard operation, and
-        accumulate commucation cost on origin cost which will finally be used in auto sharding solver.
+        accumulate communication cost on origin cost which will finally be used in auto sharding solver.
         For the sharding operation, we just care about legal sharding dimensions.
 
         Argument:
             source_spec(ShardingSpec): the ShardingSpec of the source_spec.
             orig_cost(float): the original communication cost before this operation.
 
         Return:
@@ -281,15 +281,15 @@
             shard_sequence: S0,R,S1
             device_mesh_shape: (4, 4): 0}
         '''
         valid_spec_dict = {}
         comm_pattern = CollectiveCommPattern.SPLIT_FWD_GATHER_BWD
 
         # legal sharding dims means the mesh_id is still available to use.
-        legal_sharding_dims = [i for i in range(len(source_spec.device_mesh.mesh_shape))]
+        legal_sharding_dims = [i for i in range(len(source_spec.device_mesh.shape))]
         for dim, shard_list in source_spec.dim_partition_dict.items():
             for element in shard_list:
                 legal_sharding_dims.remove(element)
         if len(legal_sharding_dims) == 0:
             return valid_spec_dict
 
         tensor_dims = len(source_spec.entire_shape)
@@ -382,15 +382,15 @@
                     pass
 
         return valid_spec_dict
 
     def get_all_one_step_transform_spec(self, source_spec: ShardingSpec, orig_cost_dict) -> Dict[ShardingSpec, float]:
         '''
         Get all valid sharding specs from source_spec with one step transform, and
-        accumulate commucation cost on origin cost which will finally be used in auto sharding solver.
+        accumulate communication cost on origin cost which will finally be used in auto sharding solver.
         Note:
             all-gather will eliminate a sharding dimension, all-to-all will keep sharding dimension same as before,
             and shard will add a sharding dimension. Therefore, the result of above operations are mutual exclusive,
             we could safely put them together.
 
         Argument:
             source_spec(ShardingSpec): the ShardingSpec of the source_spec.
@@ -431,15 +431,15 @@
                 comm_spec (CommSpec): input CommSpec
                 discard_input (bool): whether to discard the input tensor
                 alloc_numel (int): current allocated numel
                 peak_numel (int): current peak numel
             """
             input_shape = compute_shape(comm_spec.sharding_spec)
             input_numel = np.prod(input_shape)
-            output_numel = input_numel * comm_spec.device_mesh.mesh_shape[comm_spec.logical_process_axis]
+            output_numel = input_numel * comm_spec.device_mesh.shape[comm_spec.logical_process_axis]
             peak_numel = max(peak_numel, alloc_numel + output_numel * 2)
             alloc_numel += output_numel
             if discard_input:
                 alloc_numel -= input_numel
 
             return alloc_numel, peak_numel
 
@@ -457,15 +457,15 @@
             """
             shard_dim = comm_spec.shard_dim
             if shard_dim != 0:
                 # if we don't shard the tensor on the first dimension, the split action will
                 # generate a new tensor
                 input_shape = compute_shape(comm_spec.sharding_spec)
                 input_numel = np.prod(input_shape)
-                output_numel = input_numel // comm_spec.device_mesh.mesh_shape[comm_spec.logical_process_axis]
+                output_numel = input_numel // comm_spec.device_mesh.shape[comm_spec.logical_process_axis]
                 alloc_numel += output_numel
                 peak_numel = max(peak_numel, alloc_numel)
                 if discard_input:
                     alloc_numel -= input_numel
             else:
                 # if we shard the tensor on the first dimension, the split action will not generate
                 # a new tensor, and as it will preserve a reference to the input tensor, we could
@@ -573,15 +573,15 @@
         Step1:
             Generate all one-step transform sequences from source_spec.
         Step2:
             Pick the 'best' sharding spec following the heuristic function.
         Step3:
             Repeat above steps until the source spec transform to target spec.
 
-        During finding the transform path, commucation cost will be accumulated, and it
+        During finding the transform path, communication cost will be accumulated, and it
         will be finally used in auto parallel solver.
 
         Additionally, to avoid repeating the path search in runtime, we cached all solved path
         in auto parallel strategy building time, which could handle most of cases in runtime.
 
         Argument:
             source_spec(ShardingSpec): ShardingSpec of the source activation.
```

### Comparing `colossalai-0.3.0/colossalai/tensor/sharding_spec.py` & `colossalai-0.3.1/colossalai/tensor/sharding_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         target = 'S'
         for dim in self.shard_list:
             target += str(dim)
         return target
 
     def _convert_str_to_shard_list(self, str_spec):
         '''
-        Conver str_spec into shard_list.
+        Convert str_spec into shard_list.
 
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
-        Build a difference maping for 2D device mesh case. It will be used to
+        Build a difference mapping for 2D device mesh case. It will be used to
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
-            and the value of the key decribe which logical axis will be sharded in that dimension.
+            and the value of the key describe which logical axis will be sharded in that dimension.
         sharding_sequence(List[_DimSpec], optional): A straight view of ShardingSpec looks like [R, R, S0, S1].
     '''
 
     def __init__(self,
                  device_mesh: DeviceMesh,
                  entire_shape: torch.Size,
                  dim_partition_dict=None,
@@ -191,15 +191,15 @@
             assert self.sharding_sequence is not None, f'sharding_sequence should not be None, if dim_partition_dict is NoneType object.'
             self.convert_shard_sequence_to_dict()
         self._sanity_check()
 
     def __repr__(self):
         res_list = ["DistSpec:"]
         res_list.append(f"\n\tshard_sequence: " + ",".join(str(dimspec) for dimspec in self.sharding_sequence))
-        res_list.append(f"\n\tdevice_mesh_shape: {self.device_mesh.mesh_shape}")
+        res_list.append(f"\n\tdevice_mesh_shape: {self.device_mesh.shape}")
         return ' '.join(res_list)
 
     def _sanity_check(self):
         # make sure all axes in logical device mesh only be used once
         dim_check_list = list(range(self.device_mesh.logical_mesh_id.dim()))
         for dim, shard_list in self.dim_partition_dict.items():
             for element in shard_list:
@@ -218,15 +218,15 @@
 
         # make sure that the sharding for a dimension is divisible by the number of devices
         for dim, shard_list in self.dim_partition_dict.items():
             tensor_dim_size = self.entire_shape[dim]
             num_devices = 1
 
             for element in shard_list:
-                num_devices *= self.device_mesh.mesh_shape[element]
+                num_devices *= self.device_mesh.shape[element]
 
             if tensor_dim_size % num_devices != 0:
                 raise ShardingNotDivisibleError(
                     f'The size of dimension at index {dim} is {tensor_dim_size}, it cannot be sharded over {num_devices} devices.'
                 )
 
     def convert_dict_to_shard_sequence(self):
@@ -284,13 +284,13 @@
             difference += orig_dim_spec.difference(other_dim_spec)
         return difference
 
     def get_sharded_shape_per_device(self):
 
         sharded_shape = list(self.entire_shape)
         for dim, shard_list in self.dim_partition_dict.items():
-            mesh_list = [self.device_mesh.mesh_shape[mesh_dim] for mesh_dim in shard_list]
+            mesh_list = [self.device_mesh.shape[mesh_dim] for mesh_dim in shard_list]
             shard_partitions = reduce(operator.mul, mesh_list, 1)
             assert sharded_shape[
                 dim] % shard_partitions == 0, f'Cannot shard dimension {dim} into {shard_partitions} partitions.'
             sharded_shape[dim] //= shard_partitions
         return torch.Size(sharded_shape)
```

### Comparing `colossalai-0.3.0/colossalai/tensor/tensor_spec.py` & `colossalai-0.3.1/colossalai/tensor/tensor_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/tensor/utils.py` & `colossalai-0.3.1/colossalai/tensor/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         shard(R) -> S0
     For the S dimension, we need to make sure the shard_list after sharding still keep rising order.
     e.g:
         shard(S0) -> S01
 
     Argument:
         target_pair(Tuple[int, List[int]]): The first element is the dimension of tensor to be sharded,
-        and the second element decribes which logical axis will be sharded in that dimension.
+        and the second element describes which logical axis will be sharded in that dimension.
     '''
     _, shard_list = target_pair
     shard_list_list = []
     for dim in legal_sharding_dims:
         if len(shard_list) != 0 and dim <= shard_list[-1]:
             continue
         new_shard_list = shard_list + [dim]
```

### Comparing `colossalai-0.3.0/colossalai/testing/__init__.py` & `colossalai-0.3.1/colossalai/testing/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .comparison import (
     assert_close,
     assert_close_loose,
     assert_equal,
     assert_equal_in_group,
+    assert_hf_output_close,
     assert_not_equal,
     check_state_dict_equal,
 )
 from .pytest_wrapper import run_on_environment_flag
 from .utils import (
     clear_cache_before_run,
     free_port,
@@ -16,9 +17,9 @@
     skip_if_not_enough_gpus,
     spawn,
 )
 
 __all__ = [
     'assert_equal', 'assert_not_equal', 'assert_close', 'assert_close_loose', 'assert_equal_in_group', 'parameterize',
     'rerun_on_exception', 'rerun_if_address_is_in_use', 'skip_if_not_enough_gpus', 'free_port', 'spawn',
-    'clear_cache_before_run', 'run_on_environment_flag', 'check_state_dict_equal'
+    'clear_cache_before_run', 'run_on_environment_flag', 'check_state_dict_equal', 'assert_hf_output_close'
 ]
```

### Comparing `colossalai-0.3.0/colossalai/testing/pytest_wrapper.py` & `colossalai-0.3.1/colossalai/testing/pytest_wrapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 This file will not be automatically imported by `colossalai.testing`
-as this file has a dependency on `pytest`. Therefore, you need to 
+as this file has a dependency on `pytest`. Therefore, you need to
 explicitly import this file `from colossalai.testing.pytest_wrapper import <func>`.from
 """
 
-import pytest
 import os
 
 
 def run_on_environment_flag(name: str):
     """
     Conditionally run a test based on the environment variable. If this environment variable is set
     to 1, this test will be executed. Otherwise, this test is skipped. The environment variable is default to 0.
@@ -26,14 +25,20 @@
         # this will execute your test
         SOME_FLAG=1 pytest test_for_something.py
 
         # this will skip your test
         pytest test_for_something.py
 
     """
+    try:
+        import pytest
+    except ImportError:
+        raise ImportError(
+            'This function requires `pytest` to be installed, please do `pip install pytest` and try again.')
+
     assert isinstance(name, str)
     flag = os.environ.get(name.upper(), '0')
 
     reason = f'Environment variable {name} is {flag}'
     if flag == '1':
         return pytest.mark.skipif(False, reason=reason)
     else:
```

### Comparing `colossalai-0.3.0/colossalai/testing/random.py` & `colossalai-0.3.1/colossalai/testing/random.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/testing/utils.py` & `colossalai-0.3.1/colossalai/testing/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/trainer/_trainer.py` & `colossalai-0.3.1/colossalai/trainer/_trainer.py`

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
-        >>> timier = ...
+        >>> timer = ...
         >>> logger = ...
-        >>> trainer = Trainer(engine=engine, logger=logger, timer=timier)
+        >>> trainer = Trainer(engine=engine, logger=logger, timer=timer)
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
-        # training-ralated params
+        # training-related params
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
-        """Call timer funciton with a given timer name.
+        """Call timer function with a given timer name.
 
         Args:
             action (str): Function to be called on timer.
             item (str): Name of the timer.
             args (list): args used for action function.
             kwargs (dict): kwargs used for action function.
         """
```

### Comparing `colossalai-0.3.0/colossalai/trainer/hooks/__init__.py` & `colossalai-0.3.1/colossalai/trainer/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/trainer/hooks/_base_hook.py` & `colossalai-0.3.1/colossalai/trainer/hooks/_base_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/trainer/hooks/_checkpoint_hook.py` & `colossalai-0.3.1/colossalai/trainer/hooks/_checkpoint_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/trainer/hooks/_log_hook.py` & `colossalai-0.3.1/colossalai/trainer/hooks/_log_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/trainer/hooks/_lr_scheduler_hook.py` & `colossalai-0.3.1/colossalai/trainer/hooks/_lr_scheduler_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/trainer/hooks/_metric_hook.py` & `colossalai-0.3.1/colossalai/trainer/hooks/_metric_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/__init__.py` & `colossalai-0.3.1/colossalai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/activation_checkpoint.py` & `colossalai-0.3.1/colossalai/utils/activation_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/checkpoint/module_checkpoint.py` & `colossalai-0.3.1/colossalai/utils/checkpoint/module_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/checkpoint/utils.py` & `colossalai-0.3.1/colossalai/utils/checkpoint/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/checkpoint_io/backend.py` & `colossalai-0.3.1/colossalai/utils/checkpoint_io/backend.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/checkpoint_io/convertor.py` & `colossalai-0.3.1/colossalai/utils/checkpoint_io/convertor.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/checkpoint_io/distributed.py` & `colossalai-0.3.1/colossalai/utils/checkpoint_io/distributed.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/checkpoint_io/io.py` & `colossalai-0.3.1/colossalai/utils/checkpoint_io/io.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/checkpoint_io/meta.py` & `colossalai-0.3.1/colossalai/utils/checkpoint_io/meta.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/checkpoint_io/reader.py` & `colossalai-0.3.1/colossalai/utils/checkpoint_io/reader.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/checkpoint_io/utils.py` & `colossalai-0.3.1/colossalai/utils/checkpoint_io/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/checkpoint_io/writer.py` & `colossalai-0.3.1/colossalai/utils/checkpoint_io/writer.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/checkpointing.py` & `colossalai-0.3.1/colossalai/utils/checkpointing.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/common.py` & `colossalai-0.3.1/colossalai/utils/common.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/cuda.py` & `colossalai-0.3.1/colossalai/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/data_sampler/data_parallel_sampler.py` & `colossalai-0.3.1/colossalai/utils/data_sampler/data_parallel_sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
-# adpated from torch.utils.data.DistributedSampler
+# adapted from torch.utils.data.DistributedSampler
 
 import math
 import random
 import numpy as np
 from typing import TypeVar, Iterator
 
 import torch
```

### Comparing `colossalai-0.3.0/colossalai/utils/memory.py` & `colossalai-0.3.1/colossalai/utils/memory.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/model/experimental.py` & `colossalai-0.3.1/colossalai/lazy/lazy_init.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from contextlib import contextmanager
 from types import MethodType
-from typing import Callable, Optional, Union
+from typing import Callable, Dict, Optional, Union
 
 import torch
 import torch.distributed as dist
 import torch.nn as nn
 from torch import Tensor
 from torch.utils._pytree import tree_map
 
 from colossalai._analyzer._subclasses import MetaTensor
-from colossalai.tensor.d_tensor.d_tensor import DTensor
-from colossalai.tensor.d_tensor.layout import Layout
+from colossalai.device.device_mesh import DeviceMesh
+from colossalai.tensor.d_tensor import distribute_tensor
+from colossalai.tensor.d_tensor.sharding_spec import ShardingSpec
 
 # reference: https://pytorch.org/cppdocs/notes/tensor_creation.html
 _NORMAL_FACTORY = [
     "arange",
     "full",
     "empty",
     "linspace",
@@ -33,15 +35,15 @@
 ]
 
 _EARLY_MATERIALIZED_OPS = ['__getitem__', 'split']
 
 # If your intent is to change the metadata of a Tensor (such as sizes / strides / storage / storage_offset)
 # without autograd tracking the change, remove the .data / .detach() call and wrap the change in a `with torch.no_grad():` block.
 # These ops cannot be unwrapped using .data
-_CHANGE_META_OPS = ['_cudnn_rnn_flatten_weight', 'requires_grad_', '__get__', '__set__']
+_CHANGE_META_OPS = ['_cudnn_rnn_flatten_weight', 'requires_grad_', '__get__', '__set__', 'numel', 'size', 'dim']
 
 _LEGACY_TENSOR_CONSTRUCTOR = {
     'FloatTensor': torch.float,
     'DoubleTensor': torch.double,
     'HalfTensor': torch.half,
     'BFloat16Tensor': torch.bfloat16,
     'ByteTensor': torch.uint8,
@@ -56,20 +58,23 @@
 
 
 class _MyTensor(Tensor):
     """This class is only for correctness verification.
     """
     _pre_op_fn: Callable[['LazyTensor'], None] = lambda *args: None
 
+    default_device: Optional[torch.device] = None
+
     def __new__(cls, func, *args, concrete_data=None, **kwargs) -> '_MyTensor':
         cls._pre_op_fn()
         if concrete_data is not None:
             # uniform api as LazyTensor
             data = concrete_data
         else:
+            kwargs['device'] = cls.default_device
             data = func(*args, **kwargs)
         return Tensor._make_subclass(cls, data, require_grad=data.requires_grad)
 
     @classmethod
     def __torch_function__(cls, func, types, args=(), kwargs=None):
         cls._pre_op_fn()
         return super().__torch_function__(func, types, args, kwargs)
@@ -137,14 +142,16 @@
 
     """
 
     _repr = True
     _meta_data: Optional[MetaTensor] = None    # shape, dtype, device
     _pre_op_fn: Callable[['LazyTensor'], None] = lambda *args: None
 
+    default_device: Optional[torch.device] = None
+
     @staticmethod
     def __new__(cls, func, *args, meta_data=None, concrete_data=None, **kwargs):
         if concrete_data is not None:
             # some ops don't support meta backend and should have concrete data
             elem = concrete_data
         else:
             if meta_data is None:
@@ -154,40 +161,42 @@
             elem = meta_data._tensor
         # As a meta tensor cannot be modified __class__ to torch.Tensor, we should use an empty real tensor here
         r = torch.Tensor._make_subclass(cls, _EMPTY_DATA, require_grad=elem.requires_grad)
         r._meta_data = meta_data
         return r
 
     def __init__(self, func, *args, meta_data=None, concrete_data=None, **kwargs):
+        if func.__name__ in _NORMAL_FACTORY:
+            kwargs = {**kwargs, 'device': LazyTensor.default_device}
         self._factory_method = (func, args, kwargs)    # (func, args, kwargs)
         self._op_buffer = []    # (func, args, kwargs, replace)
         self._materialized_data: Optional[torch.Tensor] = concrete_data    # materialized data
 
     def materialize(self) -> torch.Tensor:
         """Materialize the ``LazyTensor`` to ``torch.Tensor`` by modifying __class__ (inplace).
 
         Returns:
             torch.Tensor: The materialized tensor (self).
         """
         target = self._materialize_data()
         self.clean()
         return _convert_cls(self, target)
 
-    def distribute(self, layout: Layout) -> torch.Tensor:
+    def distribute(self, device_mesh: DeviceMesh, sharding_spec: ShardingSpec) -> torch.Tensor:
         """Distribute the ``LazyTensor`` to ``torch.Tensor`` by modifying __class__ (inplace), according to the layout.
 
         Args:
             layout (Layout): Distribution layout.
 
         Returns:
             torch.Tensor: The distributed tensor (self).
         """
         target = self._materialize_data()
         self.clean()
-        local_tensor = DTensor(target, layout).local_tensor
+        local_tensor = distribute_tensor(target, device_mesh, sharding_spec)
         return _convert_cls(self, local_tensor)
 
     def clean(self) -> None:
         """Clean all stored operations, meta data and materialized data, which prevents memory leaking. This should be called after all tensors are materialized.
         """
         self._factory_method = None
         self._op_buffer = None
@@ -201,24 +210,19 @@
         return x
 
     def _materialize_data(self) -> torch.Tensor:
         # self._materialized_data should be generated after the first call of this function
         if self._materialized_data is None:
             # apply factory method
             func, args, kwargs = self._factory_method
-
             # apply cached sequence
             self._pre_op_fn()
 
-            try:
-                init_val = func(*tree_map(self._replace_with_materialized, args),
-                                **tree_map(self._replace_with_materialized, kwargs))
-            except TypeError as e:
-                print(f'init fn: {func.__name__}')
-                raise e
+            init_val = func(*tree_map(self._replace_with_materialized, args),
+                            **tree_map(self._replace_with_materialized, kwargs))
 
             self._materialized_data = self._rerun_ops(init_val)
         return self._materialized_data
 
     def _rerun_ops(self, target=None) -> torch.Tensor:
         """Do lazy execution by rerunning all (stored) related operations.
 
@@ -300,14 +304,15 @@
                 if isinstance(y, MetaTensor):
                     if y in meta_to_lazy:
                         # inplace op, just return origin lazy tensor
                         return meta_to_lazy[y]
                     else:
                         # out of place op, create new lazy tensor
                         fn = lambda *a, **kw: func(*a, **kw) if i is None else func(*a, **kw)[i]
+                        fn.__name__ = func.__name__
                         lazy_y = LazyTensor(fn, *args, meta_data=y, **kwargs)
                         return lazy_y
                 elif type(y) is Tensor:
                     # for early materialized tensor
                     return LazyTensor(lambda: None, concrete_data=y)
                 return y
 
@@ -346,15 +351,22 @@
             # if self is materialized, return self
             new_tensor = self.materialize() if type(self) is LazyTensor else self
             copied = new_tensor.detach().clone()
             if new_tensor.requires_grad:
                 copied.requires_grad_()
             return copied
 
-        target = LazyTensor(factory_fn, meta_data=self._meta_data)
+        if self._materialized_data is not None:
+            # self is early materialized
+            copied = self._materialized_data.detach().clone()
+            if self.requires_grad:
+                copied.requires_grad_()
+            target = LazyTensor(lambda: None, concrete_data=copied)
+        else:
+            target = LazyTensor(factory_fn, meta_data=self._meta_data)
 
         memo[id(self)] = target
         return target
 
     @property
     def data(self):
         return self
@@ -423,22 +435,29 @@
         This API is still experimental and further modifications can be made to it.
         For example:
             1. Quantization strategies can be applied before allocating real memory.
             2. Lazy initialization seems slower than normal initialization.
     """
     _replaced: bool = False
 
-    def __init__(self, tensor_cls: Union[_MyTensor, LazyTensor] = LazyTensor):
+    def __init__(self,
+                 tensor_cls: Union[_MyTensor, LazyTensor] = LazyTensor,
+                 default_device: Optional[Union[torch.device, str, int]] = None):
+        assert tensor_cls is LazyTensor or tensor_cls is _MyTensor
         self.overrides = {}
         self.tensor_cls = tensor_cls
+        self.old_default_device = LazyTensor.default_device
+        self.default_device = default_device
 
     def __enter__(self):
         if LazyInitContext._replaced:
             raise RuntimeError(f'LazyInitContext is not reentrant')
         LazyInitContext._replaced = True
+        self.old_default_device = self.tensor_cls.default_device
+        self.tensor_cls.default_device = self.default_device
 
         def wrap_factory_method(target):
             # factory functions (eg. torch.empty())
             def wrapper(*args, **kwargs):
                 return self.tensor_cls(target, *args, **kwargs)
 
             return wrapper, target
@@ -506,14 +525,15 @@
             if callable(getattr(torch, target, None))
         })
 
         for name, (wrapper, orig) in self.overrides.items():
             setattr(torch, name, wrapper)
 
     def __exit__(self, exc_type, exc_val, exc_tb):
+        self.tensor_cls.default_device = self.old_default_device
         LazyInitContext._replaced = False
         for name, (wrapper, orig) in self.overrides.items():
             setattr(torch, name, orig)
 
     @staticmethod
     def materialize(module: nn.Module, verbose: bool = False) -> nn.Module:
         """Initialize all ``nn.Parameter`` from ``LazyTensor``. This function will modify the module in-place.
@@ -525,25 +545,28 @@
 
         def apply_fn(name: str, p: LazyTensor):
             p.materialize()
 
         return _apply_to_lazy_module(module, apply_fn, verbose)
 
     @staticmethod
-    def distribute(module: nn.Module, layout_dict: dict, verbose: bool = False) -> nn.Module:
+    def distribute(module: nn.Module,
+                   device_mesh: DeviceMesh,
+                   sharding_spec_dict: Dict[str, ShardingSpec],
+                   verbose: bool = False) -> nn.Module:
         """Distribute all ``nn.Parameter`` from ``LazyTensor``. This function will modify the module in-place.
 
         Args:
             module (nn.Module): Target ``nn.Module``
             layout_dict (dict): Dict of layout for each parameter/buffer. The key is the parameter/buffer name, and the value is the layout.
             verbose (bool, optional): Whether to print lazy initialization rate. Defaults to False.
         """
 
         def apply_fn(name: str, p: LazyTensor):
-            p.distribute(layout_dict[name])
+            p.distribute(device_mesh, sharding_spec_dict[name])
 
         return _apply_to_lazy_module(module, apply_fn, verbose)
 
 
 def _apply_to_lazy_module(module: nn.Module,
                           apply_fn: Callable[[str, torch.Tensor], None],
                           verbose: bool = False) -> nn.Module:
```

### Comparing `colossalai-0.3.0/colossalai/utils/model/utils.py` & `colossalai-0.3.1/colossalai/utils/model/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             cls.__init__ = preprocess_after(cls.__init__)
 
         # The function is called during init subclass.
         def _init_subclass(cls, **kwargs):
             cls.__init__ = preprocess_after(cls.__init__)
 
         # Replace .__init__() for all existing subclasses of torch.nn.Module
-        # Excution self._post_init_method after the default init function.
+        # Execution self._post_init_method after the default init function.
         substitute_init_recursively(torch.nn.modules.module.Module, _enable_class, set())
 
         # holding on to the current __init__subclass__ for exit
         torch.nn.modules.module.Module._old_init_subclass = (torch.nn.modules.module.Module.__init_subclass__)
         # Replace .__init__() for future subclasses of torch.nn.Module
         torch.nn.modules.module.Module.__init_subclass__ = classmethod(_init_subclass)
```

### Comparing `colossalai-0.3.0/colossalai/utils/moe.py` & `colossalai-0.3.1/colossalai/utils/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py` & `colossalai-0.3.1/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/profiler/legacy/comm_profiler.py` & `colossalai-0.3.1/colossalai/utils/profiler/legacy/comm_profiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,32 +107,32 @@
 
         def append(s: str = None):
             if s is not None:
                 res.append(s)
             res.append(sep)
 
         if self.warn_flag:
-            append("Warnning: there exists multiple communication operations in the same time. As a result, "
+            append("Warning: there exists multiple communication operations in the same time. As a result, "
                    "the profiling result is not accurate.")
 
         if self.total_cuda_time == 0:
             return "No collective communication has been called yet!"
 
         append("Collective communication profiling result:")
         append("total cuda time: {}".format(_format_time(self.total_cuda_time)))
         append("average bandwidth: {}".format(_format_bandwidth(self.total_comm_vol, self.total_cuda_time)))
         append("total number of calls: {}".format(self.total_count))
         append("All events:")
 
-        seperation = '-' * 74
+        separation = '-' * 74
         row_format = '{:^10}' + '{:^12}' * 2 + '{:^16}' + '{:^12}' * 2
 
-        append(seperation)
+        append(separation)
         append(row_format.format('Location', 'GPU time', 'Percentage', 'Comm volume', 'Bandwidth', 'Num of calls'))
-        append(seperation)
+        append(separation)
 
         show_list = sorted(self.ops_record.items(), key=lambda kv: -kv[1].self_cuda_time)
         for location, event in show_list:
             append(location)
             append(
                 row_format.format('', _format_time(event.self_cuda_time),
                                   '{:.1f}%'.format(event.self_cuda_time / self.total_cuda_time * 100.0),
```

### Comparing `colossalai-0.3.0/colossalai/utils/profiler/legacy/pcie_profiler.py` & `colossalai-0.3.1/colossalai/utils/profiler/legacy/pcie_profiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,20 +126,20 @@
         append("time of data transmission (CPU -> GPU): {}".format(_format_time(self.h2d_time)))
         append("number of transmission (CPU -> GPU): {}".format(self.h2d_count))
         append("time of data transmission (GPU -> CPU): {}".format(_format_time(self.d2h_time)))
         append("number of transmission (GPU -> CPU): {}".format(self.d2h_count))
 
         append("Possible data transmission events in PCIE:")
 
-        seperation = '-' * 62
+        separation = '-' * 62
         row_format = '{:^10}' + '{:^12}' + '{:^16}' + '{:^12}' * 2
 
-        append(seperation)
+        append(separation)
         append(row_format.format('Location', 'GPU time', 'Trans volume', 'Bandwidth', 'Num of calls'))
-        append(seperation)
+        append(separation)
 
         show_list = sorted(self.ops_record.items(), key=lambda kv: -kv[1].cuda_time)
         for location, event in show_list:
             append(location)
             append(
                 row_format.format('', _format_time(event.cuda_time), _format_memory(event.pcie_vol),
                                   _format_bandwidth(event.pcie_vol, event.cuda_time), event.count))
```

### Comparing `colossalai-0.3.0/colossalai/utils/profiler/legacy/prof_utils.py` & `colossalai-0.3.1/colossalai/utils/profiler/legacy/prof_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,17 @@
         return '{:.2f} MB'.format(nbytes * 1.0 / MB)
     elif (abs(nbytes) >= KB):
         return '{:.2f} KB'.format(nbytes * 1.0 / KB)
     else:
         return str(nbytes) + ' B'
 
 
-def _format_bandwidth(volme: float or int, time_us: int):
+def _format_bandwidth(volume: float or int, time_us: int):
     sec_div_mb = (1000.0 / 1024.0)**2
-    mb_per_sec = volme / time_us * sec_div_mb
+    mb_per_sec = volume / time_us * sec_div_mb
 
     if mb_per_sec >= 1024.0:
         return '{:.3f} GB/s'.format(mb_per_sec / 1024.0)
     else:
         return '{:.3f} MB/s'.format(mb_per_sec)
```

### Comparing `colossalai-0.3.0/colossalai/utils/profiler/profiler.py` & `colossalai-0.3.1/colossalai/utils/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/profiler/stateful_tensor_mem_extention.py` & `colossalai-0.3.1/colossalai/utils/profiler/stateful_tensor_mem_extention.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/rank_recorder/rank_recorder.py` & `colossalai-0.3.1/colossalai/utils/rank_recorder/rank_recorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
                         'name': rec['name']
                     })
 
         shutil.rmtree(LOG_FOLDER)
         with open(self.export_name + '.json', 'w', encoding='utf-8') as f:
             json.dump(recoders, f, ensure_ascii=False)
 
-    def visualise_record(self):
+    def visualize_record(self):
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
-            self.visualise_record()
+            self.visualize_record()
 
 
 recorder = Recorder()
 atexit.register(recorder.exit_worker)
```

### Comparing `colossalai-0.3.0/colossalai/utils/tensor_detector/tensor_detector.py` & `colossalai-0.3.1/colossalai/utils/tensor_detector/tensor_detector.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/utils/timer.py` & `colossalai-0.3.1/colossalai/utils/timer.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/__init__.py` & `colossalai-0.3.1/colossalai/zero/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/gemini/__init__.py` & `colossalai-0.3.1/colossalai/zero/gemini/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/gemini/chunk/chunk.py` & `colossalai-0.3.1/colossalai/zero/gemini/chunk/chunk.py`

 * *Files 0% similar despite different names*

```diff
@@ -412,15 +412,15 @@
         self.__update_one_tensor_info(self.tensors_info[tensor], tensor_state)
 
     def copy_tensor_to_chunk_slice(self, tensor: torch.Tensor, data_slice: torch.Tensor) -> None:
         """
         Copy data slice to the memory space indexed by the input tensor in the chunk.
 
         Args:
-            tensor (torch.Tensor): the tensor used to retrive meta information
+            tensor (torch.Tensor): the tensor used to retrieve meta information
             data_slice (torch.Tensor): the tensor to be copied to the chunk
         """
         # sanity check
         assert self.is_gathered
 
         tensor_info = self.tensors_info[tensor]
         self.cuda_global_chunk[tensor_info.offset:tensor_info.end].copy_(data_slice.data.flatten())
```

### Comparing `colossalai-0.3.0/colossalai/zero/gemini/chunk/manager.py` & `colossalai-0.3.1/colossalai/zero/gemini/chunk/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         self.__sub_accessed_chunk(chunk)
 
     def copy_tensor_to_chunk_slice(self, tensor: torch.Tensor, data: torch.Tensor) -> None:
         """
         Copy data to the chunk.
 
         Args:
-            tensor (torch.Tensor): the tensor used to retrive meta information
+            tensor (torch.Tensor): the tensor used to retrieve meta information
             data (torch.Tensor): the tensor to be copied to the chunk
         """
         chunk = self.tensor_chunk_map[tensor]
         chunk.copy_tensor_to_chunk_slice(tensor, data)
 
     def get_chunk(self, tensor: torch.Tensor) -> Chunk:
         """
```

### Comparing `colossalai-0.3.0/colossalai/zero/gemini/chunk/search_utils.py` & `colossalai-0.3.1/colossalai/zero/gemini/chunk/search_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,29 +110,29 @@
         params_dict[param_key].append(param)
 
     return params_dict
 
 
 def search_chunk_configuration(
         model: nn.Module,
-        search_range_mb: float,
-        search_interval_byte: int,    # hidden size is the best value for the interval
-        min_chunk_size_mb: float = 32,
+        search_range_m: float,
+        search_interval: int,    # hidden size is the best value for the interval
+        min_chunk_size_m: float = 32,
         filter_exlarge_params: bool = True,
         strict_ddp_flag: bool = False,
         memstas: Optional[MemStats] = None) -> Tuple[Dict, int, int]:
     """search_chunk_configuration
 
     Search the chunk configuration for a model.
 
     Args:
         model (nn.Module): torch module
-        search_range_mb (float): searching range in mega byte.
-        search_interval_byte (int): searching interval in byte.
-        min_chunk_size_mb (float, optional): the minimum size of a distributed chunk.
+        search_range_m (float): searching range divided by 2^20.
+        search_interval (int): searching interval.
+        min_chunk_size_m (float, optional): the minimum size of a distributed chunk, divided by 2^20..
         filter_exlarge_params (bool, optional): filter extreme large parameters. Defaults to True.
         strict_ddp_flag (bool, optional): whether to enable the strict ddp mode.
             all parameters keep replicated in this mode.
 
     Returns:
         Tuple[Dict, int]: chunk config (a dict of dp_degree -> chunk init args) and its memory chunk waste in byte.
     """
@@ -141,48 +141,48 @@
         param_order = memstas.param_order()
     else:
         # build the param visited order right now
         param_order = OrderedParamGenerator()
         for p in model.parameters():
             param_order.append(p)
 
-    search_range_byte = round(search_range_mb * 1024**2)
-    min_chunk_size_byte = round(min_chunk_size_mb * 1024**2)
-    assert search_range_byte >= 0
+    search_range = round(search_range_m * 1024**2)
+    min_chunk_size = round(min_chunk_size_m * 1024**2)
+    assert search_range >= 0
 
     params_dict = classify_params_by_dp_degree(param_order, strict_ddp_flag)
     size_lcm = np.lcm.reduce(list(params_dict.keys()))
     config_dict: Dict[int, Dict] = dict()
     total_param_size = 0
 
     size_dict: Dict[int, List[int]] = dict()
     for dp_degree in params_dict:
         params_list = params_dict[dp_degree]
         size_list = [_tensor_numel(p, strict_ddp_flag) for p in params_list]
         group_acc_size = sum(size_list)
         total_param_size += group_acc_size
 
         # let small parameters keep gathered in CUDA all the time
-        if group_acc_size < min_chunk_size_byte:
+        if group_acc_size < min_chunk_size:
             config_dict[dp_degree] = dict(chunk_size=group_acc_size, keep_gathered=True)
         else:
             size_dict[dp_degree] = size_list
 
     if filter_exlarge_params:
         _filter_exlarge_params(model, size_dict)
 
-    max_size = min_chunk_size_byte
+    max_size = min_chunk_size
     for key in size_dict:
         max_size = max(max_size, max(size_dict[key]))
-    start_size = int(math.ceil(max_size / search_interval_byte) * search_interval_byte)
+    start_size = int(math.ceil(max_size / search_interval) * search_interval)
 
     min_chunk_waste = float('+inf')
     best_chunk_size = start_size
 
-    for chunk_size in range(start_size, start_size + search_range_byte + 1, search_interval_byte):
+    for chunk_size in range(start_size, start_size + search_range + 1, search_interval):
         temp_waste = 0
         for key in size_dict:
             temp_waste += _get_unused_byte(size_dict[key], chunk_size)
         if temp_waste < min_chunk_waste:
             min_chunk_waste = temp_waste
             best_chunk_size = chunk_size
```

### Comparing `colossalai-0.3.0/colossalai/zero/gemini/chunk/utils.py` & `colossalai-0.3.1/colossalai/zero/gemini/chunk/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,34 +19,34 @@
 
 def init_chunk_manager(model: nn.Module,
                        init_device: Optional[torch.device] = None,
                        hidden_dim: Optional[int] = None,
                        verbose: bool = False,
                        **kwargs) -> ChunkManager:
     if hidden_dim:
-        search_interval_byte = hidden_dim
+        search_interval = hidden_dim
     else:
-        search_interval_byte = 1024    # defaults to 1kb
-    kwargs["search_interval_byte"] = search_interval_byte
+        search_interval = 1024    # defaults to 1024
+    kwargs["search_interval"] = search_interval
 
     dist.barrier()
     begin = time()
 
     config_dict, total_size, wasted_size = search_chunk_configuration(model, **kwargs)
 
     dist.barrier()
     end = time()
     span_s = end - begin
-    mb_size = 1024**2
-    total_size /= mb_size
-    wasted_size /= mb_size
+    mega_unit = 1024**2
+    total_size /= mega_unit
+    wasted_size /= mega_unit
 
     if verbose and dist.get_rank() == 0:
         print("searching chunk configuration is completed in {:.2f} s.\n".format(span_s),
-              "used number: {:.2f} MB, wasted number: {:.2f} MB\n".format(total_size, wasted_size),
+              "used number: {:.2f} * 2^20, wasted number: {:.2f} * 2^20\n".format(total_size, wasted_size),
               "total wasted percentage is {:.2f}%".format(100 * safe_div(wasted_size, total_size + wasted_size)),
               sep='',
               flush=True)
     dist.barrier()
 
     chunk_manager = ChunkManager(config_dict, init_device)
     return chunk_manager
```

### Comparing `colossalai-0.3.0/colossalai/zero/gemini/colo_init_context.py` & `colossalai-0.3.1/colossalai/zero/gemini/colo_init_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/gemini/gemini_ddp.py` & `colossalai-0.3.1/colossalai/zero/gemini/gemini_ddp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import itertools
 from collections import OrderedDict
 from contextlib import nullcontext
 from functools import partial
-from typing import Dict, Iterator, List, Optional, Union, Tuple, Set
+from typing import Dict, Iterator, List, Optional, Set, Tuple, Union
 
 import torch
 import torch.distributed as dist
 import torch.nn as nn
 
 from colossalai.checkpoint_io.utils import calculate_tensor_size
+from colossalai.lazy import LazyTensor
 from colossalai.logging import get_dist_logger
 from colossalai.nn.parallel.data_parallel import ColoDDP, _cast_float, free_storage
 from colossalai.tensor import ProcessGroup as ColoProcessGroup
 from colossalai.tensor import ReplicaSpec
 from colossalai.tensor.colo_parameter import ColoParameter, ColoTensor, ColoTensorSpec
 from colossalai.tensor.param_op_hook import ColoParamOpHookManager
 from colossalai.utils import get_current_device, is_ddp_ignored
-from colossalai.utils.model.experimental import LazyTensor
 
 from .chunk import Chunk, ChunkManager, TensorState, init_chunk_manager
 from .gemini_hook import GeminiZeROHook
 from .gemini_mgr import GeminiManager
 from .memory_tracer import MemStats, OrderedParamGenerator
 from .utils import get_temp_total_chunk_on_cuda
 
@@ -47,34 +47,38 @@
             For more details, see the API reference of ``GeminiManager``.
         pin_memory (bool): Chunks on CPU Memory use pin-memory.
         force_outputs_fp32 (bool): If set to True, outputs will be fp32. Otherwise, outputs will be fp16.
             Defaults to False.
         strict_ddp_mode (bool): If set to True, there is no tensor sharding, each tensor is replicated.
             Defaults to False. Users can set it to True, when they clearly know that they only need DDP.
         scatter_after_inference (bool): If set to True, the model will be scattered after inference. This will save memory but slow down the consecutive inference.
+        mixed_precision (torch.dtype): If set to torch.float16, the model will be trained in fp16. Otherwise, the model will be trained in bf16. Defaults to torch.float16.
     """
 
     def __init__(self,
                  module: torch.nn.Module,
                  gemini_manager: GeminiManager,
                  pin_memory: bool = False,
                  force_outputs_fp32: bool = False,
                  strict_ddp_mode: bool = False,
-                 scatter_after_inference: bool = True) -> None:
+                 scatter_after_inference: bool = True,
+                 mixed_precision: torch.dtype = torch.float16) -> None:
+        assert mixed_precision in (torch.float16, torch.bfloat16)
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
+        self.mixed_precision = mixed_precision
 
         self._logger = get_dist_logger()
 
         if self.gemini_manager._premade_memstats_:
             # build chunk in param runtime visited order.
             param_order = self.gemini_manager.memstats()._param_runtime_order
         else:
@@ -92,42 +96,46 @@
         for name, param in module.named_parameters():
             self.param2name[param] = name
         for m_name, m_var in module.named_modules():
             for p_name, p_var in m_var.named_parameters(recurse=False):
                 param_name = m_name + '.' + p_name if m_name else p_name
                 self.name2param[param_name] = p_var
         super().__init__(module, process_group=ColoProcessGroup())
-        self._non_persistent_buffers_set=self._get_non_persistent_buffers_set(module)
+        self._non_persistent_buffers_set = self._get_non_persistent_buffers_set(module)
         self._cast_buffers()
 
-    def _get_non_persistent_buffers_set(self, module, memo: Optional[Set[nn.Module]] = None, prefix: str = '', remove_duplicate: bool = True):
-
-            r"""
-            Args:
-                memo: a memo to store the set of modules already added to the result
-                prefix: a prefix that will be added to the name of the module
-                remove_duplicate: whether to remove the duplicated module instances in the result
-                    or not
-            """
-
-            if memo is None:
-                memo = set()
-            self_non_persistent_set = set()
-            if module not in memo:
-                if remove_duplicate:
-                    memo.add(module)
-                self_non_persistent_set = set(map(lambda key: prefix + ('.' if prefix else '') + key, module._non_persistent_buffers_set))
-                for name, sub_module in module._modules.items():
-                    if sub_module is None:
-                        continue
-                    submodule_prefix = prefix + ('.' if prefix else '') + name
-                    child_non_persistent_set = self._get_non_persistent_buffers_set(sub_module, memo, submodule_prefix, remove_duplicate)
-                    self_non_persistent_set = set.union(self_non_persistent_set, child_non_persistent_set)
-            return self_non_persistent_set
-    
+    def _get_non_persistent_buffers_set(self,
+                                        module,
+                                        memo: Optional[Set[nn.Module]] = None,
+                                        prefix: str = '',
+                                        remove_duplicate: bool = True):
+        r"""
+        Args:
+            memo: a memo to store the set of modules already added to the result
+            prefix: a prefix that will be added to the name of the module
+            remove_duplicate: whether to remove the duplicated module instances in the result
+                or not
+        """
+
+        if memo is None:
+            memo = set()
+        self_non_persistent_set = set()
+        if module not in memo:
+            if remove_duplicate:
+                memo.add(module)
+            self_non_persistent_set = set(
+                map(lambda key: prefix + ('.' if prefix else '') + key, module._non_persistent_buffers_set))
+            for name, sub_module in module._modules.items():
+                if sub_module is None:
+                    continue
+                submodule_prefix = prefix + ('.' if prefix else '') + name
+                child_non_persistent_set = self._get_non_persistent_buffers_set(sub_module, memo, submodule_prefix,
+                                                                                remove_duplicate)
+                self_non_persistent_set = set.union(self_non_persistent_set, child_non_persistent_set)
+        return self_non_persistent_set
 
     def _post_forward(self):
         """This function is only triggered for inference.
         """
         access_list = list(self.chunk_manager.accessed_chunks)
         # we need to scatter all accessed chunks and move them to their original places
         for chunk in access_list:
@@ -143,15 +151,15 @@
     def forward(self, *args, **kwargs):
         # check whether we are in a inference mode
         grad_flag = torch.is_grad_enabled()
         if not grad_flag:
             assert not self.gemini_manager.need_warmup or not self.gemini_manager.is_warmup(
             ), "You should run a completed iteration as your warmup iter"
 
-        args, kwargs = _cast_float(args, torch.half), _cast_float(kwargs, torch.half)
+        args, kwargs = _cast_float(args, self.mixed_precision), _cast_float(kwargs, self.mixed_precision)
         self.module.zero_grad(set_to_none=True)
         if not grad_flag:
             outputs = self._inference_forward(*args, **kwargs)
         else:
             self.gemini_manager.pre_iter(*args)
             with ColoParamOpHookManager.use_hooks(self.param_op_hook):
                 outputs = self.module(*args, **kwargs)
@@ -562,22 +570,22 @@
 
             # ignore the parameters with no gradient
             if not p.requires_grad:
                 self.set_params_to_ignore([p])
 
             # move ignored parameters to CUDA
             if is_ddp_ignored(p):
-                p.data = p.data.to(device=get_current_device(), dtype=torch.float16)
+                p.data = p.data.to(device=get_current_device(), dtype=self.mixed_precision)
                 continue
 
             # create a fp32 parameter
             fp32_data = p.data.float()
             fp32_p = ColoTensor(fp32_data, spec=ColoTensorSpec(p.process_group))
             # create a fp16 parameter
-            p.data = p.data.half()
+            p.data = p.data.to(self.mixed_precision)
 
             # register the fp16 parameter and fp32 parameter in the chunk manager
             dp_world_size = p.process_group.dp_world_size()
             self.chunk_manager.register_tensor(tensor=p,
                                                group_type='fp16_param',
                                                config_key=dp_world_size,
                                                cpu_offload=cpu_offload,
@@ -605,15 +613,15 @@
 
     def _cast_buffers(self):
         for buffer in self.module.buffers():
             if isinstance(buffer, LazyTensor):
                 buffer.materialize()
             buffer.data = buffer.cuda()
             if torch.is_floating_point(buffer):
-                buffer.data = buffer.half()
+                buffer.data = buffer.to(self.mixed_precision)
 
     def _preprocess_param(self, p: Union[nn.Parameter, ColoParameter, 'LazyTensor']) -> None:
         """Convert parameter to ColoParameter in-place.
         Args:
             p (Union[nn.Parameter, ColoParameter, LazyTensor]): parameter to be converted
         """
         if type(p) is ColoParameter:
@@ -704,15 +712,18 @@
         self.current_block = OrderedDict()
         self.current_block_size = 0
 
     def append(self, name: str, tensor: torch.Tensor) -> Tuple[Optional[OrderedDict], int]:
         tensor_size = calculate_tensor_size(tensor)
         ret_block = None
         ret_block_size = 0
-        if self.current_block_size + tensor_size > self.max_shard_size:
+
+        # before we return the current block and create a new block,
+        # we need to ensure that the current block is not empty
+        if self.current_block_size + tensor_size > self.max_shard_size and self.current_block_size > 0:
             ret_block = self.current_block
             ret_block_size = self.current_block_size
             self.current_block = OrderedDict()
             self.current_block_size = 0
         self.current_block[name] = tensor
         self.current_block_size += tensor_size
         return ret_block, ret_block_size
@@ -724,18 +735,19 @@
                  module: torch.nn.Module,
                  device: torch.device,
                  placement_policy: str = "cpu",
                  pin_memory: bool = False,
                  force_outputs_fp32: bool = False,
                  strict_ddp_mode: bool = False,
                  scatter_after_inference: bool = True,
-                 search_range_mb: int = 32,
+                 search_range_m: int = 32,
                  hidden_dim: Optional[int] = None,
-                 min_chunk_size_mb: float = 32,
+                 min_chunk_size_m: float = 32,
                  memstats: Optional[MemStats] = None,
+                 mixed_precision: torch.dtype = torch.float16,
                  verbose: bool = False) -> None:
         """
         A torch.Module wrapper using ZeRO-DP and Gemini.
         ZeRO is for parallel. Gemini is for memory management.
         WARNING: The class will modify the module inline!
 
         Example:
@@ -747,30 +759,35 @@
 
         Args:
             module (torch.nn.Module): the model to be wrapped.
             device (torch.device): device to place the model.
             placement_policy (str, optional): "cpu", "cuda", "auto". Defaults to "cpu".
             pin_memory (bool, optional): use pin memory on CPU. Defaults to False.
             force_outputs_fp32 (bool, optional): force outputs are fp32. Defaults to False.
-            search_range_mb (int, optional): chunk size searching range in MegaByte. Defaults to 32.
+            search_range_m (int, optional): chunk size searching range divided by 2^20. Defaults to 32.
             hidden_dim (int, optional): the hidden dimension of DNN.
                 Users can provide this argument to speed up searching.
                 If users do not know this argument before training, it is ok. We will use a default value 1024.
-            min_chunk_size_mb (float, optional): the minimum chunk size in MegaByte.
+            min_chunk_size_m (float, optional): the minimum chunk size divided by 2^20.
                 If the aggregate size of parameters is still smaller than the minimum chunk size,
                 all parameters will be compacted into one small chunk.
             memstats (MemStats, optional) the memory statistics collector by a runtime memory tracer.
         """
         # some ugly hotfix for the compatibility with Lightning
-        if search_range_mb is None:
-            search_range_mb = 32
+        if search_range_m is None:
+            search_range_m = 32
 
         chunk_manager = init_chunk_manager(model=module,
                                            init_device=device,
                                            hidden_dim=hidden_dim,
-                                           search_range_mb=search_range_mb,
-                                           min_chunk_size_mb=min_chunk_size_mb,
+                                           search_range_m=search_range_m,
+                                           min_chunk_size_m=min_chunk_size_m,
                                            strict_ddp_flag=strict_ddp_mode,
                                            verbose=verbose)
         gemini_manager = GeminiManager(placement_policy, chunk_manager, memstats)
-        super().__init__(module, gemini_manager, pin_memory, force_outputs_fp32, strict_ddp_mode,
-                         scatter_after_inference)
+        super().__init__(module,
+                         gemini_manager,
+                         pin_memory,
+                         force_outputs_fp32,
+                         strict_ddp_mode,
+                         scatter_after_inference,
+                         mixed_precision=mixed_precision)
```

### Comparing `colossalai-0.3.0/colossalai/zero/gemini/gemini_hook.py` & `colossalai-0.3.1/colossalai/zero/gemini/gemini_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/gemini/gemini_mgr.py` & `colossalai-0.3.1/colossalai/zero/gemini/gemini_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/gemini/gemini_optimizer.py` & `colossalai-0.3.1/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,335 +1,399 @@
 # this code is inspired by the DeepSpeed library and implemented with our own design from scratch
-import math
-import warnings
 from enum import Enum
-from typing import Any, Dict, Set, Tuple
+from os import stat
+from typing import Dict, Optional, Tuple
 
 import torch
 import torch.distributed as dist
-from torch.nn import Parameter
+import torch.nn as nn
+from torch import Tensor
+from torch.distributed import ProcessGroup
+from torch.nn.parameter import Parameter
 from torch.optim import Optimizer
 
 from colossalai.amp.naive_amp.grad_scaler import DynamicGradScaler
+from colossalai.context.parallel_mode import ParallelMode
+from colossalai.core import global_context as gpc
 from colossalai.logging import get_dist_logger
-from colossalai.nn.optimizer import ColossalaiOptimizer, CPUAdam, FusedAdam, HybridAdam
-from colossalai.utils import disposable, get_current_device, is_ddp_ignored
+from colossalai.nn.optimizer import ColossalaiOptimizer
+from colossalai.zero.legacy.gemini.stateful_tensor import StatefulTensor, TensorState
+from colossalai.zero.legacy.gemini.tensor_placement_policy import AutoTensorPlacementPolicy
+from colossalai.zero.legacy.gemini.tensor_utils import colo_model_data_tensor_move_inline, colo_tensor_mem_usage
+from colossalai.zero.legacy.sharded_model import ShardedModelV2
+from colossalai.zero.legacy.sharded_model._utils import cast_tensor_to_fp32
 
-from .chunk import Chunk, ChunkManager
-from .gemini_ddp import ZeroDDP
 
-__all__ = ['ZeroOptimizer', 'GeminiAdamOptimizer']
+class OptimState(Enum):
+    SCALED = 1
+    UNSCALED = 2
 
-_AVAIL_OPTIM_LIST = {FusedAdam, CPUAdam, HybridAdam}
 
+class ShardedOptimizerV2(ColossalaiOptimizer):
+    """A wrapper for optimizer. ``ShardedOptimizerV2`` and ``ShardedModelV2`` implement Zero Redundancy Optimizer (ZeRO).
 
-class OptimState(Enum):
-    SCALED = 0
-    UNSCALED = 1
+    By default the ZeRO optimizer stage 3 offload Optimizer States on CPU.
+
+    We apply the Device-aware Operator Placement technique for OS placement from the following paper.
+
+    `PatrickStar: Parallel Training of Pre-trained Models via Chunk-based Memory Management`_
+
+    GPU margin space is the remaining space after removing peak non-model data from the overall GPU memory,
+    which is detected by a runtime memory tracer.
 
+    We place as many OS chunks in the margin space as possible.
 
-class ZeroOptimizer(ColossalaiOptimizer):
-    """A wrapper for optimizer. ``ZeroDDP`` and ``ZeroOptimizer`` implement Zero Redundancy Optimizer (ZeRO state-3).
+    The size of margin space can be controlled by ``gpu_margin_mem_ratio``.
+    If it is set as ``0.0``, it is the same as classical ZeRO optimizer.
 
     Note:
-        You must use ``ZeroDDP`` with ``ZeroOptimizer``.
+        You must use ``ShardedOptimizerV2`` with ``ShardedModelV2``.
 
     Note:
-        Make sure you set ``placement_policy`` of ``GeminiManager`` to `"auto"`,
+        Make sure you set ``tensor_placement_policy`` in ``ShardedModelV2`` to `"auto"`,
         if you set ``gpu_margin_mem_ratio > 0``.
 
     Args:
-        optim (Optimizer): An Optimizer instance.
-        module (ZeroDDP): A ``ZeroDDP`` instance.
+        sharded_model (ShardedModelV2): A sharded model initialized by class ShardedModelV2. The optimizer will use the
+            shard strategy provided by sharded model to shard param fp32 tensors.
+        optimizer (Optimizer): An Optimizer instance.
         gpu_margin_mem_ratio (float, optional): The ratio of GPU remaining memory (after the first forward-backward)
             which will be used when using hybrid CPU optimizer.
-            This argument is meaningless when `placement_policy` of `GeminiManager` is not "auto".
+            This argument is meaningless when `tensor_placement_policy` of `ShardedModelV2` is not "auto".
             Defaults to 0.0.
         initial_scale (float, optional): Initial scale used by DynamicGradScaler. Defaults to 2**32.
         min_scale (float, optional): Min scale used by DynamicGradScaler. Defaults to 1.
-        growth_factor (float, optional): Growth_factor used by DynamicGradScaler. Defaults to 2.
-        backoff_factor (float, optional): Backoff_factor used by DynamicGradScaler. Defaults to 0.5.
-        growth_interval (float, optional): Growth_interval used by DynamicGradScaler. Defaults to 1000.
-        hysteresis (float, optional): Hysteresis used by DynamicGradScaler. Defaults to 2.
-        max_scale (int, optional): Max_scale used by DynamicGradScaler. Defaults to 2**32.
-        clipping_norm (float, optional): The norm value used to clip gradient. Defaults to 0.0.
-        norm_type (float, optional): The type of norm used for gradient clipping. Currently, only L2-norm (norm_type=2.0)
-            is supported in ZeroOptimizer. Defaults to 2.0.
-        verbose (bool, optional): Whether to print verbose information, including grad overflow info. Defaults to False.
+        growth_factor (float, optional): growth_factor used by DynamicGradScaler. Defaults to 2.
+        backoff_factor (float, optional): backoff_factor used by DynamicGradScaler. Defaults to 0.5.
+        growth_interval (float, optional): growth_interval used by DynamicGradScaler. Defaults to 1000.
+        hysteresis (float, optional): hysteresis used by DynamicGradScaler. Defaults to 2.
+        max_scale (int, optional): max_scale used by DynamicGradScaler. Defaults to 2**32.
+        dp_process_group (Optional[ProcessGroup], optional): data parallel process group. Defaults to None.
+        mp_process_group (Optional[ProcessGroup], optional): model parallel process group. Defaults to None.
+
+    .. _PatrickStar\: Parallel Training of Pre-trained Models via Chunk-based Memory Management:
+        https://arxiv.org/abs/2108.05818
     """
 
     def __init__(self,
-                 optim: Optimizer,
-                 module: ZeroDDP,
+                 sharded_model: ShardedModelV2,
+                 optimizer: Optimizer,
                  gpu_margin_mem_ratio: float = 0.0,
                  initial_scale: float = 2**32,
                  min_scale: float = 1,
                  growth_factor: float = 2,
                  backoff_factor: float = 0.5,
                  growth_interval: int = 1000,
                  hysteresis: int = 2,
                  max_scale: float = 2**32,
-                 clipping_norm: float = 0.0,
-                 norm_type: float = 2.0,
-                 verbose: bool = False,
-                 **defaults: Any):
-        super().__init__(optim)
-        assert isinstance(module, ZeroDDP)
-        assert type(optim) in _AVAIL_OPTIM_LIST, "You should use an optimizer in the available list:\n" \
-            f"{_AVAIL_OPTIM_LIST}"
-        self.module = module
-        self.gemini_manager = module.gemini_manager
-        self.chunk_manager: ChunkManager = self.gemini_manager.chunk_manager
-        self.optim_state = OptimState.UNSCALED
-        self.param_to_range: Dict[Parameter, Tuple[int, int]] = dict()
-        self.param_to_chunk32: Dict[Parameter, Chunk] = dict()
-        self.chunk16_set: Set[Chunk] = set()
-        self.clipping_flag = clipping_norm > 0.0
-        self.max_norm = clipping_norm
-        self.verbose = verbose
-
-        if self.clipping_flag:
-            assert norm_type == 2.0, "ZeroOptimizer only supports L2 norm now"
-
-        ddp_param_list = []
-        for name, param in module.named_parameters():
-            if is_ddp_ignored(param):
-                if param.requires_grad:
-                    warnings.warn(f"Parameter `{name}` is ignored by DDP but requires gradient! "
-                                  "You should handle its optimizer update by yourself!")
-            else:
-                ddp_param_list.append(param)
-
-        for p, fp32_p in zip(ddp_param_list, module.fp32_params):
-            chunk_16 = self.chunk_manager.get_chunk(p)
-            if chunk_16 not in self.chunk16_set:
-                chunk_16.l2_norm_flag = self.clipping_flag
-                self.chunk16_set.add(chunk_16)
-
-        self.__init__optimizer()
+                 dp_process_group: Optional[ProcessGroup] = None,
+                 mp_process_group: Optional[ProcessGroup] = None,
+                 verbose: bool = False) -> None:
+        assert isinstance(sharded_model, ShardedModelV2), 'model must be wrapped with ShardedModel'
+        assert not isinstance(optimizer, ShardedOptimizerV2), 'Nested ShardedOptimizerV2 is not supported.'
+
+        super().__init__(optimizer)
+        self.shard_strategy = sharded_model.shard_strategy
+        self.model: ShardedModelV2 = sharded_model
+        self.bf16 = sharded_model.bf16
 
+        self.gpu_margin_mem_ratio: float = float(gpu_margin_mem_ratio)
+        assert 0.0 <= self.gpu_margin_mem_ratio <= 1.0, f'gpu_margin_mem_ratio must >=0.0 and <=1.0'
+        # Only move fp32 shards from CPU to GPU when user allows and inner optimizer is valid
+        # Inner optimizer must support optimizing hybrid (CPU and CUDA) tensors,
+        # and it must set `num_fp32_shards_per_param` correctly
+        self._should_move_fp32_shards_h2d: bool = sharded_model.cpu_offload and self.gpu_margin_mem_ratio > 0.0 and getattr(
+            optimizer, 'num_fp32_shards_per_param', 0) >= 2
+        self.device = sharded_model._tensor_placement_policy.device or torch.device('cpu')
+        self.optim_state: OptimState = OptimState.UNSCALED
+        self.dp_process_group = dp_process_group or gpc.get_group(ParallelMode.DATA)
+        self.mp_process_group = mp_process_group or gpc.get_group(ParallelMode.MODEL)
         # Grad scaler
         self.grad_scaler = DynamicGradScaler(initial_scale=initial_scale,
                                              min_scale=min_scale,
                                              growth_factor=growth_factor,
                                              backoff_factor=backoff_factor,
                                              growth_interval=growth_interval,
                                              hysteresis=hysteresis,
                                              max_scale=max_scale)
-        self._found_overflow: torch.Tensor = torch.zeros(1, dtype=torch.int64, device=get_current_device())
-        self._logger = get_dist_logger()
-
-        self.gpu_margin_mem_ratio: float = float(gpu_margin_mem_ratio)
-        assert 0.0 <= self.gpu_margin_mem_ratio <= 1.0, f'gpu_margin_mem_ratio must >=0.0 and <=1.0'
-        # Only move fp32 shards from CPU to GPU when user allows and inner optimizer is valid
-        # Inner optimizer must support optimizing hybrid (CPU and CUDA) tensors,
-        # and it must set `num_fp32_shards_per_param` correctly
-        self._should_move_fp32_params_h2d: bool = self.gemini_manager.is_cuda_margin_mem_avail and self.gpu_margin_mem_ratio > 0.0 and getattr(
-            optim, 'num_fp32_shards_per_param', 0) >= 2
-        if self.gpu_margin_mem_ratio > 0.0 and not self.gemini_manager.is_cuda_margin_mem_avail:
-            self._logger.warning(f'gpu_margin_mem_ratio is meaningless when placement_policy is not "auto"', ranks=[0])
-
-        self._register_states = disposable(self._register_states_)
-
-    def _set_grad_ptr(self):
-        for group in self.param_groups:
-            for fake_param in group['params']:
-                chunk32 = self.param_to_chunk32[fake_param]
-                begin, end = self.param_to_range[fake_param]
-                chunk16 = chunk32.paired_chunk
-
-                fake_param.data = chunk16.payload[begin:end]
-                fake_param.grad = fake_param.data
-                fake_param.data = chunk32.payload[begin:end]
-
-    def _update_fp16_params(self):
-        none_tensor = torch.empty([0])
-        for group in self.param_groups:
-            for fake_param in group['params']:
-                assert fake_param.grad is None
-                fake_param.data = none_tensor.to(fake_param.device)
-
-        for chunk16 in self.chunk16_set:
-            chunk16.optim_update()
-
-    def _check_overflow(self):
-        # clear previous overflow record
-        self._found_overflow.fill_(self.module.overflow_counter)
-
-        # all-reduce across global group
-        dist.all_reduce(self._found_overflow)
-
-        return self._found_overflow.item() > 0
-
-    def _clear_global_norm(self) -> None:
-        for c16 in self.chunk16_set:
-            c16.l2_norm = None
-
-    def _calc_global_norm(self) -> float:
-        norm_sqr: float = 0.0
-        group_to_norm = dict()
-        for c16 in self.chunk16_set:
-            assert c16.l2_norm is not None
-
-            if c16.is_gathered:
-                norm_sqr += c16.l2_norm
-            else:
-                # this chunk is sharded, use communication to collect total norm
-                if c16.torch_pg not in group_to_norm:
-                    group_to_norm[c16.torch_pg] = 0.0
-                group_to_norm[c16.torch_pg] += c16.l2_norm
-
-            c16.l2_norm = None    # clear l2 norm
-
-        comm_buffer = torch.zeros(1, dtype=torch.float, device=get_current_device())
-        for group, part_norm in group_to_norm.items():
-            comm_buffer.fill_(part_norm)
-            dist.all_reduce(comm_buffer, group=group)
-            norm_sqr += comm_buffer.item()
-
-        global_norm = math.sqrt(norm_sqr)
-        return global_norm
-
-    def _get_combined_scale(self):
-        loss_scale = 1
-
-        if self.optim_state == OptimState.SCALED:
-            loss_scale = self.loss_scale
-            self.optim_state = OptimState.UNSCALED
-
-        combined_scale = loss_scale
-        if self.clipping_flag:
-            total_norm = self._calc_global_norm()
-            clip = ((total_norm / loss_scale) + 1e-6) / self.max_norm
-            if clip > 1:
-                combined_scale = clip * loss_scale
+        self._found_overflow: Tensor = torch.IntTensor([0]).to(torch.cuda.current_device())
+        self._logger = get_dist_logger("ShardedOptimizerV2")
+        self._verbose = verbose
+        self._grad_prepared: bool = False    # this should be set to true when _prepare_grads() and reset to false when backward
+
+        # Store fp32 param shards
+        self._register_master_weight()
+        if self.gpu_margin_mem_ratio != 0.0 and not isinstance(sharded_model._tensor_placement_policy,
+                                                               AutoTensorPlacementPolicy):
+            self._logger.warning(f'gpu_margin_mem_ratio is meaningless when tensor_placement_policy is not "auto"',
+                                 ranks=[0])
+
+        if self._verbose:
+            self._logger.debug(
+                f"After init ShardedOptimizerV2 consumes {self.get_memory_usage()[0] / 1e6} MB CUDA Memory!", ranks=[0])
 
-        if combined_scale == 1:
-            return -1
-        else:
-            return combined_scale
+        self._use_memory_tracer = self.model.use_memory_tracer
 
     @property
     def loss_scale(self):
         return self.grad_scaler.scale.item()
 
-    def zero_grad(self, *args, **kwargs):
-        self.module.overflow_counter = 0
-        return self.optim.zero_grad(set_to_none=True)
+    def get_memory_usage(self) -> Tuple[int, int]:
+        """ Get the memory usage of the optimizer. Including master_params (param fp32),
+        momentum (``self.state[p]['exp_avg']``) variance (``self.state[p]['exp_avg_sq']``)
+
+        Returns:
+            Tuple[int, int]: cuda/cpu memory usage in Byte.
+        """
+        cuda_use = 0
+        cpu_use = 0
+
+        def update_mem_use(t):
+            nonlocal cuda_use
+            nonlocal cpu_use
+            t_cuda_use, t_cpu_use = colo_tensor_mem_usage(t)
+            cuda_use += t_cuda_use
+            cpu_use += t_cpu_use
 
-    def step(self, *args, **kwargs):
-        self._maybe_move_fp32_params()
-        self._set_grad_ptr()
-
-        found_inf = self._check_overflow()
-        if found_inf:
-            self.optim_state = OptimState.UNSCALED    # no need to unscale grad
-            self.grad_scaler.update(found_inf)    # update gradient scaler
-            if self.verbose:
-                self._logger.info(f'Found overflow. Skip step')
-            self._clear_global_norm()    # clear recorded norm
-            self.zero_grad()    # reset all gradients
-            self._update_fp16_params()
-            return
+        for _, p_fp32 in self.master_params.items():
+            update_mem_use(p_fp32)
+        for group in self.optim.param_groups:
+            for p in group['params']:
+                state = self.optim.state[p]
+                for k, v in state.items():
+                    update_mem_use(v)
 
-        # get combined scale. combined scale = loss scale * clipping norm
-        # so that gradient = gradient / combined scale
-        combined_scale = self._get_combined_scale()
-        self.grad_scaler.update(found_inf)
-
-        ret = self.optim.step(div_scale=combined_scale, *args, **kwargs)
-        self._register_states()
-        self.zero_grad()
-        self._update_fp16_params()
-        return ret
+        return cuda_use, cpu_use
 
-    def clip_grad_norm(self, model: torch.nn.Module, max_norm: float, norm_type: float = 2.0):
-        raise NotImplementedError
+    def zero_grad(self, *args, **kwargs):
+        self._zero_grad()
 
-    def backward(self, loss: torch.Tensor):
-        loss = self.loss_scale * loss
-        self.optim_state = OptimState.SCALED
-        self.module.backward(loss)
+    def backward(self, loss: Tensor) -> None:
+        if not self.bf16:
+            loss = self.loss_scale * loss
+            self.optim_state = OptimState.SCALED
+        self._grad_prepared = False
+        self.model.backward(loss)
 
-    def backward_by_grad(self, tensor: torch.Tensor, grad: torch.Tensor):
+    def backward_by_grad(self, tensor: Tensor, grad: Tensor) -> None:
         # This function is called except the last stage of pipeline parallel
         # It receives the scaled grad from the previous rank
         # No need to scale the grad again
         # Need to unscale when optimizing
-        self.optim_state = OptimState.SCALED
-        self.module.backward_by_grad(tensor, grad)
+        if not self.bf16:
+            self.optim_state = OptimState.SCALED
+        self._grad_prepared = False
+        self.model.backward_by_grad(tensor, grad)
+
+    def clip_grad_norm(self, model: nn.Module, max_norm: float):
+        self._prepare_grads()
+        if not self.bf16 and self.optim_state == OptimState.SCALED:
+            self._unscale_grads()
+        return super().clip_grad_norm(model, max_norm)
 
-    def _maybe_move_fp32_params(self):
-        if self._should_move_fp32_params_h2d:
-            self._should_move_fp32_params_h2d = False
-            available_cuda_margin_mem = self.gemini_manager.cuda_margin_mem * self.gpu_margin_mem_ratio
-            fp32_params_available_cuda_margin_mem = available_cuda_margin_mem / self.optim.num_fp32_shards_per_param
-            fp32_params_used_cuda_margin_mem = 0
-
-            for group in self.param_groups:
-                for fake_param in group['params']:
-                    chunk32 = self.param_to_chunk32[fake_param]
-                    chunk16 = chunk32.paired_chunk
+    def step(self, *args, **kwargs):
 
-                    if chunk32.device_type == 'cuda':
-                        continue
+        self._prepare_grads()
+        # unscale grads if scaled
+        if not self.bf16 and self.optim_state == OptimState.SCALED:
+            self._unscale_grads()
+
+        self._maybe_move_fp32_shards()
+        if not self.bf16:
+            found_inf = self._check_overflow()
+            self.grad_scaler.update(found_inf)
+
+            if found_inf:
+                self._logger.warning('found inf during ShardedOptimV2 step')
+                self._zero_grad(recover_data=True)
+                return
+
+        self._point_param_fp16_to_master_param()
+
+        if self._verbose:
+            gpu_mem, cpu_mem = self.get_memory_usage()
+            self._logger.debug(
+                f"Before step ShardedOptimizerV2 consumes {gpu_mem / 1e6} MB CUDA Memory, {cpu_mem / 1e6} MB CUDA Memory!",
+                ranks=[0])
+        ret = self.optim.step(*args, **kwargs)
+
+        if self._verbose:
+            gpu_mem, cpu_mem = self.get_memory_usage()
+            self._logger.debug(
+                f"After step ShardedOptimizerV2 consumes {gpu_mem / 1e6} MB CUDA Memory, {cpu_mem / 1e6} MB CUDA Memory!",
+                ranks=[0])
 
-                    if fp32_params_used_cuda_margin_mem + chunk32.payload_mem < fp32_params_available_cuda_margin_mem:
-                        self.chunk_manager.move_chunk(chunk32, get_current_device())
-                        # stores grad now
-                        self.chunk_manager.move_chunk(chunk16, get_current_device())
-                        self.module.set_chunk_grad_device(chunk16, get_current_device())
-                        fp32_params_used_cuda_margin_mem += chunk32.payload_mem
-
-            for group in self.param_groups:
-                for fake_param in group['params']:
-                    chunk32 = self.param_to_chunk32[fake_param]
-                    if chunk32.device_type == 'cuda':
-                        state = self.optim.state[fake_param]
-                        for k, v in state.items():
-                            if isinstance(v, torch.Tensor):
-                                state[k] = v.to(get_current_device())
+        self._copy_master_model_to_model_fp16()
+        return ret
+
+    def _check_overflow(self):
+        # clear previous overflow record
+        self._found_overflow.fill_(self.model.overflow_counter)
+
+        # all-reduce across dp group
+        dist.all_reduce(self._found_overflow, group=self.dp_process_group)
 
-    def _register_states_(self):
+        # all-reduce over model parallel group
+        dist.all_reduce(self._found_overflow, group=self.mp_process_group)
+
+        return self._found_overflow.item() > 0
+
+    def _unscale_grads(self):
+        assert self.optim_state == OptimState.SCALED
         for group in self.optim.param_groups:
             for p in group['params']:
-                state = self.optim.state[p]
-                for val in state.values():
-                    if isinstance(val, torch.Tensor):
-                        self.chunk_manager.add_extern_static_tensor(val)
-
-    def __init__optimizer(self):
-
-        def get_range_pair(local_chunk: Chunk, local_param: Parameter):
-            param_info = local_chunk.tensors_info[local_param]
-            if local_chunk.keep_gathered:
-                return param_info.offset, param_info.end
-            begin = max(0, param_info.offset - local_chunk.shard_begin)
-            end = min(local_chunk.shard_size, param_info.end - local_chunk.shard_begin)
-            return begin, end
+                if p.grad is not None:
+                    p.grad.data.div_(self.loss_scale)
+        self.optim_state = OptimState.UNSCALED
 
+    def _zero_grad(self, recover_data: bool = False):
+        """zero grad and maybe recover fp16 params
+        When `reuse_fp16_shard` is enabled,
+        p.colo_attr.sharded_data_tensor stores grad here.
+        We have to recover them from fp32 params.
+
+        Args:
+            recover_data (bool, optional): Whether to recover fp16 param from fp32 param. Defaults to False.
+        """
+        # We must set grad to None
+        # Because grad here is sharded
+        # But next backward pass will create a full grad first
+        # Which leads to wrong accumulation
+        self.optim.zero_grad(set_to_none=True)
         for group in self.optim.param_groups:
-            fake_params_list = list()
-
-            for param in group['params']:
-                if is_ddp_ignored(param):
-                    continue
-                chunk16 = self.chunk_manager.get_chunk(param)
-                range_pair = get_range_pair(chunk16, param)
-                if range_pair[0] >= range_pair[1]:
-                    continue
+            for p in group['params']:
+                # p.colo_attr.sharded_data_tensor stores grad now
+                # we have to recover fp16 param
+                reuse_fp16_shard = (p.colo_attr.sharded_data_tensor.payload_size == 0)
+                if recover_data and reuse_fp16_shard:
+                    self._copy_master_param_to_param_fp16(p)
+                else:
+                    # release saved gradient
+                    p.colo_attr.saved_grad.set_null()
+        self.model.overflow_counter = 0    # set overflow counter to zero
 
-                grad_device = self.module.grads_device[param]
-                fake_param = torch.nn.Parameter(torch.empty([0], device=grad_device))
-                self.param_to_chunk32[fake_param] = chunk16.paired_chunk
-                self.param_to_range[fake_param] = range_pair
+    def sync_grad(self):
+        pass
 
-                fake_params_list.append(fake_param)
+    def _register_master_weight(self):
+        self.master_params: Dict[Parameter, StatefulTensor] = {}
+        for group in self.optim.param_groups:
+            for p in group['params']:
+                assert hasattr(p, 'colo_attr'), 'The parameter must be wrapped with ShardedParam'
+                shard_flag = not p.colo_attr.sharded_data_tensor.is_sharded and p.colo_attr.is_replicated
+                if shard_flag:
+                    # we always shard replicated parameters
+                    self.shard_strategy.shard([p.colo_attr.sharded_data_tensor], self.dp_process_group)
+                self.master_params[p] = StatefulTensor(cast_tensor_to_fp32(p.colo_attr.data_payload.to(self.device)))
+                if shard_flag:
+                    # In this branch, there's no need to shard param
+                    # So we gather here
+                    self.shard_strategy.gather([p.colo_attr.sharded_data_tensor], self.dp_process_group)
+
+    def _maybe_move_fp32_shards(self):
+        if self._should_move_fp32_shards_h2d:
+            self._should_move_fp32_shards_h2d = False
+            available_cuda_margin_mem = self.model.cuda_margin_space * self.gpu_margin_mem_ratio
+            fp32_shards_available_cuda_margin_mem = available_cuda_margin_mem / self.optim.num_fp32_shards_per_param
+            fp32_shards_used_cuda_margin_mem = 0
+            for group in self.optim.param_groups:
+                for p in group['params']:
+                    if p.colo_attr.saved_grad.is_null():
+                        continue
+                    shard_mem = self.master_params[p].payload.numel() * self.master_params[p].payload.element_size()
+                    if fp32_shards_used_cuda_margin_mem + shard_mem < fp32_shards_available_cuda_margin_mem:
+                        colo_model_data_tensor_move_inline(self.master_params[p], torch.cuda.current_device())
+                        colo_model_data_tensor_move_inline(p.colo_attr.saved_grad, torch.cuda.current_device())
+                        p.colo_attr.offload_grad = False
+                        fp32_shards_used_cuda_margin_mem += shard_mem
+                        state = self.optim.state[p]
+                        for k, v in state.items():
+                            if isinstance(v, Tensor):
+                                state[k] = v.cuda()
 
-            group['params'] = fake_params_list
+    def _prepare_grads(self):
+        if self._grad_prepared:
+            return
+        for group in self.optim.param_groups:
+            for p in group['params']:
+                if p.colo_attr.saved_grad.is_null():
+                    continue
+                p.colo_attr.saved_grad.trans_state(TensorState.COMPUTE)
+                # If reuse_fp16_shard, grad fp16 which wasn't be offloaded may be evicted to CPU
+                if not p.colo_attr.offload_grad:
+                    colo_model_data_tensor_move_inline(p.colo_attr.saved_grad, torch.cuda.current_device())
+                # FIXME(ver217): p.data here is an empty tensor on CUDA and has no useful information
+                # If we change p.grad directly
+                # it may raise error because of different shape/dtype/device of p.data and p.grad
+                # We just set p.data = p.colo_attr.saved_grad.payload here
+                p.data = p.colo_attr.grad_payload
+                p.grad = p.colo_attr.grad_payload
+                # Set p.data to empty tensor, in case of memory leaking
+                p.colo_attr.set_data_none()
+        self._grad_prepared = True
+
+    def _point_param_fp16_to_master_param(self):
+        # assign master param pointers to p.data.
+        # We will not trigger data copy here.
+        for group in self.optim.param_groups:
+            for p in group['params']:
+                self.master_params[p].trans_state(TensorState.COMPUTE)
+                p.data = self.master_params[p].payload
+                # Now p.data is sharded
+                # So optimizer states are sharded naturally
+
+    def _copy_master_model_to_model_fp16(self):
+        # Copy master param data (fp32) to payload of colo_attr (fp16)
+        # TODO() improve efficiency by gathering tensors into a chunk and transferring
+        # a chunk.
+        for group in self.optim.param_groups:
+            for p in group['params']:
+                self._copy_master_param_to_param_fp16(p)
 
+    def _copy_master_param_to_param_fp16(self, p):
+        # flush gradient
+        if p.colo_attr.sharded_data_tensor.payload_size == 0:
+            # here reuse_fp16_shard is True
+            # in order to use copy below, we should give sharded data tensor a payload
+            p.colo_attr.sharded_data_tensor.payload_relay(p.colo_attr.saved_grad)
+        else:
+            p.colo_attr.saved_grad.set_null()
 
-class GeminiAdamOptimizer(ZeroOptimizer):
+        p.data = self.master_params[p].payload
 
-    def __init__(self, model: torch.nn.Module, **defaults: Any) -> None:
-        optimizer = HybridAdam(model.parameters(), **defaults)
-        super().__init__(optimizer, model, **defaults)
+        # we need to allocate new memory for keep_not_shard parameters
+        # in order to use copy, otherwise, the sizes of tensor is not compatible
+        if p.colo_attr.data_payload.numel() != p.data.numel():
+            p.colo_attr.data_payload_reset(
+                torch.empty(p.data.shape, dtype=p.colo_attr.data_payload.dtype, device=p.colo_attr.data_payload.device))
+
+        # TODO() optimize this line CPU (fp32) -> GPU (fp16)
+        half_dtype = torch.bfloat16 if self.bf16 else torch.float16
+        p.colo_attr.sharded_data_tensor.payload_copy(p.to(half_dtype).detach())
+        p.colo_attr.set_data_none()
+
+        if p.colo_attr.keep_not_shard and p.colo_attr.is_replicated:
+            # We gather full fp16 param here
+            p.colo_attr.sharded_data_tensor.is_sharded = True    # since only gradient is sharded, we should set to True
+            self.shard_strategy.gather([p.colo_attr.sharded_data_tensor], self.dp_process_group)
+
+        self.master_params[p].trans_state(TensorState.HOLD)
+
+    def state_dict(self):
+        optim_state_dict = super().state_dict()
+        scaler_state_dict = self.grad_scaler.state_dict()
+        optim_state_dict['scaler'] = scaler_state_dict
+        return optim_state_dict
+
+    def load_state_dict(self, *args, **kwargs):
+        if 'scaler' not in args[0]:
+            self._logger.warning('Missing scaler when loading optimizer state dict', ranks=[0])
+        else:
+            scaler_state_dict = args[0].pop('scaler')
+            self.grad_scaler.load_state_dict(scaler_state_dict)
+        super().load_state_dict(*args, **kwargs)
+        for group in self.optim.param_groups:
+            for p in group['params']:
+                state = self.optim.state[p]
+                for k, v in state.items():
+                    if isinstance(v, Tensor):
+                        state[k] = v.to(dtype=self.master_params[p].dtype, device=self.master_params[p].device)
```

### Comparing `colossalai-0.3.0/colossalai/zero/gemini/memory_tracer/__init__.py` & `colossalai-0.3.1/colossalai/zero/gemini/memory_tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py` & `colossalai-0.3.1/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         """
         super().__init__(memstats)
         self._chunk_manager = chunk_manager
 
     # override
     def record_model_data_volume(self) -> None:
         """
-        record model data volumn on cuda and cpu.
+        record model data volume on cuda and cpu.
         """
         if self._start_flag and not self.use_outside_memstats:
             cuda_mem = self._chunk_manager.total_mem['cuda']
             self._memstats.record_max_cuda_model_data(cuda_mem)
 
     @property
     def cuda_margin_mem(self) -> float:
```

### Comparing `colossalai-0.3.0/colossalai/zero/gemini/memory_tracer/memory_monitor.py` & `colossalai-0.3.1/colossalai/zero/gemini/memory_tracer/memory_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     def clear(self):
         self.mem_stats.clear()
         self.time_stamps.clear()
 
 
 class AsyncMemoryMonitor(MemoryMonitor):
     """
-    An Async Memory Monitor runing during computing. Sampling memory usage of the current GPU
+    An Async Memory Monitor running during computing. Sampling memory usage of the current GPU
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
-        power (int, optional): the power of time interva. Defaults to 10.
+        power (int, optional): the power of time interval. Defaults to 10.
 
     .. _PatrickStar: Parallel Training of Pre-trained Models via Chunk-based Memory Management:
         https://arxiv.org/abs/2108.05818
     """
 
     def __init__(self, power: int = 10):
         super().__init__()
```

### Comparing `colossalai-0.3.0/colossalai/zero/gemini/memory_tracer/memory_stats.py` & `colossalai-0.3.1/colossalai/zero/gemini/memory_tracer/memory_stats.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/gemini/memory_tracer/memstats_collector.py` & `colossalai-0.3.1/colossalai/zero/gemini/memory_tracer/memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/gemini/memory_tracer/param_runtime_order.py` & `colossalai-0.3.1/colossalai/zero/gemini/memory_tracer/param_runtime_order.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py` & `colossalai-0.3.1/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py` & `colossalai-0.3.1/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/gemini/memory_tracer/utils.py` & `colossalai-0.3.1/colossalai/zero/gemini/memory_tracer/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import torch
 
 
 def colo_model_optimizer_usage(optim) -> Tuple[int, int]:
     """Trace the optimizer memory usage
 
     Args:
-        optim (ShardedOptimV2): an instance of ShardedOptimver
+        optim (ShardedOptimV2): an instance of ShardedOptimizer
 
     Returns:
         Tuple[int, int]: cuda/cpu memory usage in Byte
     """
     if optim is None:
         return 0, 0
     assert hasattr(optim, 'get_memory_usage'), f"{type(optim)} has no attr get_memory_usage()"
```

### Comparing `colossalai-0.3.0/colossalai/zero/gemini/placement_policy.py` & `colossalai-0.3.1/colossalai/zero/gemini/placement_policy.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/gemini/utils.py` & `colossalai-0.3.1/colossalai/zero/gemini/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     Thus, you can use the original model in further training.
     But you should not use the returned torch model to train, this can cause unexpected errors.
 
     Args:
         zero_ddp_model (ZeroDDP): a zero ddp model
         device (torch.device): the device of the final torch model
         dtype (torch.dtype): the dtype of the final torch model
-        only_rank_0 (bool): if True, only rank0 has the coverted torch model
+        only_rank_0 (bool): if True, only rank0 has the converted torch model
 
     Returns:
         torch.nn.Module: a static torch model used for saving checkpoints or numeric checks
     """
     from colossalai.zero.gemini.gemini_ddp import ZeroDDP
     assert isinstance(zero_ddp_model, ZeroDDP)
```

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/__init__.py` & `colossalai-0.3.1/colossalai/zero/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/gemini/gemini_context.py` & `colossalai-0.3.1/colossalai/zero/legacy/gemini/gemini_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py` & `colossalai-0.3.1/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py` & `colossalai-0.3.1/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py` & `colossalai-0.3.1/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/gemini/ophooks/utils.py` & `colossalai-0.3.1/colossalai/zero/legacy/gemini/ophooks/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,30 +84,30 @@
         return (None, None) + args
 
 
 def register_ophooks_recursively(module: torch.nn.Module,
                                  ophook_list: List[BaseOpHook],
                                  name: str = "",
                                  filter_fn: Optional[Callable] = None):
-    r"""Recursilvely register pre/post hooks for all submodules in the module in FWD and BWD."""
+    r"""Recursively register pre/post hooks for all submodules in the module in FWD and BWD."""
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
 
-    # return from flitered module
+    # return from filtered module
     if filter_fn is not None and filter_fn(module):
         return
 
     def _pre_forward_module_hook(submodule, *args):
         for hook in ophook_list:
             assert isinstance(submodule, torch.nn.Module)
             hook.pre_fwd_exec(submodule, *args)
```

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py` & `colossalai-0.3.1/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/gemini/stateful_tensor.py` & `colossalai-0.3.1/colossalai/zero/legacy/gemini/stateful_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py` & `colossalai-0.3.1/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/gemini/tensor_placement_policy.py` & `colossalai-0.3.1/colossalai/zero/legacy/gemini/tensor_placement_policy.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/gemini/tensor_utils.py` & `colossalai-0.3.1/colossalai/zero/legacy/gemini/tensor_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 def colo_model_data_tensor_move_inline(t: Union[StatefulTensor, torch.Tensor], target_device: Union[torch.device,
                                                                                                     int]) -> None:
     """
     move a tensor to the target_device
     Args:
         t (Union[StatefulTensor, torch.Tensor]): the tensor be moved
-        target_device: a traget device, if type is int, it the index of cuda card.
+        target_device: a target device, if type is int, it the index of cuda card.
     """
     if not isinstance(target_device, torch.device):
         target_device = torch.device(f'cuda:{target_device}')
 
     if isinstance(t, torch.Tensor):
         t.data = t.data.to(target_device)
     elif isinstance(t, StatefulTensor):
```

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/init_ctx/init_context.py` & `colossalai-0.3.1/colossalai/zero/legacy/init_ctx/init_context.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from colossalai.context.parallel_mode import ParallelMode
 from colossalai.context.singleton_meta import SingletonMeta
 from colossalai.core import global_context as gpc
 from colossalai.logging import get_dist_logger
 from colossalai.utils.model.utils import InsertPostInitMethodToModuleSubClasses
 from colossalai.zero.legacy.shard_utils import BaseShardStrategy
-from colossalai.zero.legacy.sharded_model._utils import cast_tensor_to_fp16
+from colossalai.zero.legacy.sharded_model._utils import cast_tensor_to_bf16, cast_tensor_to_fp16
 from colossalai.zero.legacy.sharded_model.sharded_model_v2 import ShardedModelV2
 from colossalai.zero.legacy.sharded_param import ShardedParamV2
 
 
 @dataclass
 class ZeroContextConfig:
     """The configuration used to control zero context initialization.
@@ -42,39 +42,42 @@
             assert self.target_device.type == 'cuda', "Replicated no-shard parameters should be located in cuda."
 
 
 class ZeroInitContext(InsertPostInitMethodToModuleSubClasses):
     """A context to initialize model.
 
     1. Convert the model to fp16.
-    2. The paramaters of the module are adapted to type ShardedParameter.
+    2. The parameters of the module are adapted to type ShardedParameter.
     3. Shard the param and grad according to flags.
 
     Args:
         target_device (torch.device): The device where param data are after exiting the context.
         shard_strategy (BaseShardStrategy): Shard strategy instance.
         seed (int, optional): Random seed for weight initialization
         shard_param (bool, optional): Is param sharded after exiting the context. Defaults to False.
         default_dtype (torch.dtype, optional): If it's not None, parameters will be initialized as ``default_dtype`` then converted to fp16.
+        bf16 (bool, optional): If it's True, parameters will be initialized as ``torch.bfloat16``. Otherwise, parameters will be initialized as ``torch.float16``. Defaults to False.
         model_numel_tensor (torch.Tensor, optional): A tensor which will store the number of elements of model. Defaults to torch.zeros(1, dtype=torch.int).
     """
 
     def __init__(self,
                  target_device: torch.device,
                  shard_strategy: BaseShardStrategy,
                  seed: int = 2**10 - 1,
                  shard_param: bool = False,
                  default_dtype: Optional[torch.dtype] = None,
+                 bf16: bool = False,
                  model_numel_tensor: torch.Tensor = torch.zeros(1, dtype=torch.long)):
 
         super().__init__(default_dtype=default_dtype)
         self.shard_strategy = shard_strategy
         self.param_list = []
         self.model_numel_tensor = model_numel_tensor
         self.seed = seed
+        self.bf16 = bf16
         self.dp_process_group = gpc.get_group(ParallelMode.DATA)
 
         self.config = ZeroContextConfig(target_device=target_device, is_replicated=True, shard_param=shard_param)
 
         ZeroContextMgr().current_context = self
 
         self.param_numel = {}
@@ -179,17 +182,18 @@
 
     def _post_init_method(self, module: torch.nn.Module, *args, **kwargs):
         """
         The function to call at the end of the constructor of each module.
         NOTE() The module may be passed to this function multiple times.
         """
         self.top_module = module
+        half_dtype = torch.float16 if not self.bf16 else torch.bfloat16
 
         def half_fn(t: torch.Tensor):
-            return t.half() if t.is_floating_point() else t
+            return t.to(half_dtype) if t.is_floating_point() else t
 
         for param in module.parameters(recurse=False):
             # avoid adapting a param to ShardedParam twice
             if hasattr(param, 'colo_attr'):
                 continue
 
             self.param_numel[param] = param.numel()
@@ -222,17 +226,18 @@
             param.colo_attr.keep_not_shard = not self.shard_param
 
             self.param_list.append(param)
 
         # We must cast buffers
         # If we use BN, buffers may be on CPU and Float
         # We must cast them
+        cast_fn = cast_tensor_to_fp16 if not self.bf16 else cast_tensor_to_bf16
         for buffer in module.buffers(recurse=False):
             buffer.data = buffer.data.to(device=torch.cuda.current_device())
-            buffer.data = cast_tensor_to_fp16(buffer.data)
+            buffer.data = cast_fn(buffer.data)
 
 
 class ZeroContextMgr(metaclass=SingletonMeta):
     current_context: Optional[ZeroInitContext] = None
 
     @contextlib.contextmanager
     def hijack_context_config(self, **kwargs):
```

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/shard_utils/base_shard_strategy.py` & `colossalai-0.3.1/colossalai/zero/legacy/shard_utils/base_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py` & `colossalai-0.3.1/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/shard_utils/commons.py` & `colossalai-0.3.1/colossalai/zero/legacy/shard_utils/commons.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py` & `colossalai-0.3.1/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/sharded_model/_utils.py` & `colossalai-0.3.1/colossalai/zero/legacy/sharded_model/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,27 @@
     return tensor
 
 
 def cast_tensor_to_fp32(tensor: Union[torch.Tensor, StatefulTensor]) -> torch.Tensor:
     if isinstance(tensor, StatefulTensor):
         tensor = tensor.payload
 
-    if torch.is_floating_point(tensor) and tensor.dtype is torch.float16:
+    if torch.is_floating_point(tensor) and tensor.dtype in (torch.float16, torch.bfloat16):
         return tensor.float()
     return tensor
 
 
+def cast_tensor_to_bf16(tensor: torch.Tensor) -> torch.Tensor:
+    if isinstance(tensor, StatefulTensor):
+        tensor = tensor.payload
+    if torch.is_floating_point(tensor) and tensor.dtype is torch.float32:
+        return tensor.bfloat16()
+    return tensor
+
+
 def apply_to_tensors(x: Any, fn: Callable):
     if torch.is_tensor(x):
         return fn(x)
     elif isinstance(x, list):
         return [apply_to_tensors(t, fn) for t in x]
     elif isinstance(x, tuple):
         return tuple(apply_to_tensors(t, fn) for t in x)
```

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/sharded_model/reduce_scatter.py` & `colossalai-0.3.1/colossalai/zero/legacy/sharded_model/reduce_scatter.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/sharded_model/sharded_model_v2.py` & `colossalai-0.3.1/colossalai/zero/legacy/sharded_model/sharded_model_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from colossalai.zero.legacy.gemini.tensor_placement_policy import TensorPlacementPolicy, TensorPlacementPolicyFactory
 from colossalai.zero.legacy.gemini.tensor_utils import colo_model_data_move_to_cpu
 from colossalai.zero.legacy.shard_utils import BaseShardStrategy
 from colossalai.zero.legacy.sharded_model.reduce_scatter import ReduceScatterBucketer
 
 from ._utils import (
     cast_float_arguments,
+    cast_tensor_to_bf16,
     cast_tensor_to_fp16,
     cast_tensor_to_fp32,
     chunk_and_pad,
     free_storage,
     get_gradient_predivide_factor,
 )
 from .zero_hook import ZeroHook
@@ -64,37 +65,40 @@
         fp32_reduce_scatter (bool, optional): If set to `True`, gradients are forced to FP32 before reduce-scatter. Defaults to False.
         tensor_placement_policy (str): Which device to place *held* tensors. It can be 'cpu', 'cuda' and 'auto'.
             If it's 'cpu', parameters, gradients and optimizer states will be offloaded to CPU, which means min CUDA memory will be used.
             If it's 'cuda', they won't be offloaded, which means max CUDA memory will be used.
             If it's 'auto', they are moving dynamically based on CPU and CUDA memory usage. It will utilize heterogeneous memory space evenly and well.
             Note that 'auto' policy can only work well when no other processes use CUDA during your training.
             Defaults to 'cuda'.
-        gradient_predivide_factor (Optional[float], optional): Gradient is divived by this value before reduce-scatter. Defaults to 1.0.
+        gradient_predivide_factor (Optional[float], optional): Gradient is divided by this value before reduce-scatter. Defaults to 1.0.
         reuse_fp16_shard (bool, optional): Whether to reuse fp16 shard for param and grad.
             Enabling this can reduce GPU memory usage, but you have to make sure you disable it when using gradient accumulation.
             In this mode, grad will be fp16. Make sure your optimizer supports mixed precision (fp32 param and fp16 grad).
             We find that PyTorch's optimizers don't support mixed precision,
             so we recommend you enable this only when using our CPUAdam with CPU offload. Defaults to False.
+        bf16 (bool, optional): Whether to use bfloat16 for param and grad. Defaults to False.
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
+                 bf16: bool = False,
                  *args,
                  **kwargs):
         assert not isinstance(module, ShardedModelV2), 'Nested ShardedModelV2 is not supported.'
         super().__init__()
         self.logger = get_dist_logger()
+        self.bf16 = bf16
 
         # We force users to use ZeroInitContext
         for submodule in module.modules():
             sharded_cnt = 0
             unshard_cnt = 0
             for param in submodule.parameters(recurse=False):
                 assert hasattr(param, 'colo_attr'), 'You must use ZeroInitContext to init your module first.'
@@ -197,15 +201,15 @@
             # forward: model(inputs)
             # backward: optimizer.backward()
         except Exception as e:
             model.dump_memory_stats()
             exit(0)
         """
         if self._use_memory_tracer:
-            self.logger.error(f'dump memort tracer collected information to a {filename}', ranks=[0])
+            self.logger.error(f'dump memory tracer collected information to a {filename}', ranks=[0])
             if gpc.get_global_rank() == 0:
                 with open(filename, 'w+') as f:
                     f.write(f'cuda reserved {torch.cuda.memory_reserved(get_current_device()) / 1e9} GB\n')
                     f.write(f'cuda max allocated {torch.cuda.max_memory_allocated(get_current_device()) / 1e9} GB\n')
                     f.write('CUDA model data (GB)\n')
                     f.write('\n')
                     f.write('CUDA non model data (GB)\n')
@@ -228,15 +232,16 @@
     def _post_forward_operations(self):
         for p in self.module.parameters():
             if hasattr(p, 'colo_attr'):
                 p.colo_attr.sharded_data_tensor.trans_state(TensorState.HOLD)
 
     def forward(self, *args: Any, **kwargs: Any) -> torch.Tensor:
         self._pre_forward_operations(*args)
-        args, kwargs = cast_float_arguments(cast_tensor_to_fp16, *args, **kwargs)
+        cast_fn = cast_tensor_to_bf16 if self.bf16 else cast_tensor_to_fp16
+        args, kwargs = cast_float_arguments(cast_fn, *args, **kwargs)
         outputs = self.module(*args, **kwargs)
         self._post_forward_operations()
         return outputs
 
     def backward(self, loss):
         loss.backward()
         self._post_backward_operations()
@@ -376,15 +381,15 @@
         if param.colo_attr.offload_grad:
             colo_model_data_move_to_cpu(grad)
 
         if self.reuse_fp16_shard:
             # make parameters point to gradient
 
             assert param.colo_attr.saved_grad.is_null(
-            ), 'Gradien accumulation is not supported when reuse_fp16_shard=True'
+            ), 'Gradient accumulation is not supported when reuse_fp16_shard=True'
 
             param.colo_attr.grad_payload_reset(grad.data)
             # release the memory of param
             # we set a false None for parameter's payload
             # so we can get parameter's device and dtype later in optimizer
             param.colo_attr.data_payload_reset(torch.empty(0, device=grad.device, dtype=grad.dtype))
```

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/sharded_model/utils.py` & `colossalai-0.3.1/colossalai/zero/legacy/sharded_model/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/sharded_model/zero_hook.py` & `colossalai-0.3.1/colossalai/zero/legacy/sharded_model/zero_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/sharded_param/sharded_param.py` & `colossalai-0.3.1/colossalai/zero/legacy/sharded_param/sharded_param.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/legacy/sharded_param/sharded_tensor.py` & `colossalai-0.3.1/colossalai/zero/legacy/sharded_param/sharded_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/low_level/_utils.py` & `colossalai-0.3.1/colossalai/zero/low_level/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import math
 from typing import Optional
 
 import torch
 import torch.distributed as dist
-from torch import inf
+from torch import Tensor, inf
 from torch._utils import _flatten_dense_tensors, _unflatten_dense_tensors
+from torch.distributed import ProcessGroup
 
 from colossalai.tensor import ColoParameter
 from colossalai.utils import is_model_parallel_parameter
 
 
 def flatten(input_):
     return _flatten_dense_tensors(input_)
@@ -190,82 +191,69 @@
     """
     total_norm = 0.0
     for norm in norm_list:
         total_norm += norm**2.0
     return math.sqrt(total_norm)
 
 
-def compute_norm(gradients, params, dp_group, mp_group, norm_type=2):
+def compute_norm(gradients: Tensor, dp_group: ProcessGroup, tp_group: ProcessGroup, norm_type: int = 2) -> int:
     """Clips gradient norm of an iterable of parameters.
     This is adapted from torch.nn.utils.clip_grad.clip_grad_norm_ and
-    added functionality to handle model parallel parameters. Note that
-    the gradients are modified in place.
-    Arguments:
-        parameters (Iterable[Tensor] or Tensor): an iterable of Tensors or a
-            single Tensor that will have gradients normalized
-        max_norm (float or int): max norm of the gradients
-        norm_type (float or int): type of the used p-norm. Can be ``'inf'`` for
-            infinity norm.
+    added functionality to handle model parallel parameters.
+
+    Args:
+        gradients (Tensor): The gradients to compute norm
+        dp_group (ProcessGroup): The process group of ZeRO Data Parallelism
+        tp_group (ProcessGroup): The process group of Tensor Parallelism
+        norm_type (int, optional): type of the used p-norm, Can be ``'inf'`` for infinity norm. Defaults to 2.
+
     Returns:
-        Total norm of the parameters (viewed as a single vector).
+        int: The total norm of given gradients
     """
 
-    if mp_group is None:
-        mp_rank = 0
-    else:
-        mp_rank = dist.get_rank(mp_group)
-
     norm_type = float(norm_type)
     if norm_type == inf:
         total_norm = max(g.data.abs().max() for g in gradients)
         total_norm_cuda = torch.cuda.FloatTensor([float(total_norm)])
         dist.all_reduce(total_norm_cuda, op=torch.distributed.ReduceOp.MAX, group=dp_group)
 
         # Take max across all GPUs.
-        if mp_group is not None:
+        if tp_group is not None:
             dist.all_reduce(tensor=total_norm_cuda, op=torch.distributed.ReduceOp.MAX)
         total_norm = total_norm_cuda[0].item()
     else:
         total_norm = 0.0
-        # if dist.get_rank() == 0:
-        #    logger.info(f"Total Norm beginning {total_norm}")
-
-        for g, p in zip(gradients, params):
-            # Pipeline parallelism may replicate parameters. Avoid multi-counting.
-            tp_param_flag = False
-            if is_model_parallel_parameter(p) or (isinstance(p, ColoParameter) and not p.is_replicate()):
-                tp_param_flag = True
-            if tp_param_flag or mp_rank == 0:
-                param_norm = g.data.double().norm(2)
-                total_norm += param_norm.item()**2
+        for g in gradients:
+            param_norm = g.data.double().norm(2)
+            total_norm += param_norm.item()**2
 
         # Sum across all model parallel GPUs.
         total_norm_cuda = torch.cuda.FloatTensor([float(total_norm)])
         torch.distributed.all_reduce(total_norm_cuda, op=torch.distributed.ReduceOp.SUM, group=dp_group)
 
-        if mp_group is not None:
-            dist.all_reduce(tensor=total_norm_cuda, op=torch.distributed.ReduceOp.SUM, group=mp_group)
+        if tp_group is not None:
+            dist.all_reduce(tensor=total_norm_cuda, op=torch.distributed.ReduceOp.SUM, group=tp_group)
 
         total_norm = total_norm_cuda[0].item()**(1. / norm_type)
 
     if total_norm == float('inf') or total_norm == -float('inf') or total_norm != total_norm:
         total_norm = -1
 
     return total_norm
 
 
-def sync_param(flat_tensor, tensor_list):
+def sync_tensor(flat_tensor, tensor_list):
     """
     Synchronize the flattened tensor and unflattened tensor list. When
     a list of tensor are flattened with `torch._utils._unflatten_dense_tensors`,
     a new tensor is created. Thus, the flat tensor and original tensor list do not
     share the same memory space. This function will update the tensor list so that
     they point to the same value.
 
-    :param flat_tensor: A flat tensor obtained by calling `torch._utils._unflatten_dense_tensors` on a tensor lsit
+    :param flat_tensor: A flat tensor obtained by calling `torch._utils._unflatten_dense_tensors` on a tensor list
     :param tensor_list: A list of tensors corresponding to the flattened tensor
     :type flat_tensor: torch.Tensor
     :type tensor_list: List[torch.Tensor]
     """
     updated_params = unflatten(flat_tensor, tensor_list)
 
     # update the tensor data
```

### Comparing `colossalai-0.3.0/colossalai/zero/low_level/bookkeeping/tensor_bucket.py` & `colossalai-0.3.1/colossalai/zero/low_level/bookkeeping/tensor_bucket.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai/zero/wrapper.py` & `colossalai-0.3.1/colossalai/zero/wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/colossalai.egg-info/PKG-INFO` & `colossalai-0.3.1/colossalai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colossalai
-Version: 0.3.0
+Version: 0.3.1
 Summary: An integrated large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org
 License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io
@@ -32,14 +32,15 @@
         
         
            | [English](README.md) | [中文](docs/README-zh-Hans.md) |
         
         </div>
         
         ## Latest News
+        * [2023/07] [65B Model Pretraining Accelerated by 38%, Best Practices for Building LLaMA-Like Base Models Open-Source](https://www.hpc-ai.tech/blog/large-model-pretraining)
         * [2023/03] [ColossalChat: An Open-Source Solution for Cloning ChatGPT With a Complete RLHF Pipeline](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b)
         * [2023/03] [Intel and Colossal-AI Partner to Deliver Cost-Efficient Open-Source Solution for Protein Folding Structure Prediction](https://www.hpc-ai.tech/blog/intel-habana)
         * [2023/03] [AWS and Google Fund Colossal-AI with Startup Cloud Programs](https://www.hpc-ai.tech/blog/aws-and-google-fund-colossal-ai-with-startup-cloud-programs)
         * [2023/02] [Open Source Solution Replicates ChatGPT Training Process! Ready to go with only 1.6GB GPU Memory](https://www.hpc-ai.tech/blog/colossal-ai-chatgpt)
         * [2023/01] [Hardware Savings Up to 46 Times for AIGC and  Automatic Parallelism](https://medium.com/pytorch/latest-colossal-ai-boasts-novel-automatic-parallelism-and-offers-savings-up-to-46x-for-stable-1453b48f3f02)
         * [2022/11] [Diffusion Pretraining and Hardware Fine-Tuning Can Be Almost 7X Cheaper](https://www.hpc-ai.tech/blog/diffusion-pretraining-and-hardware-fine-tuning-can-be-almost-7x-cheaper)
         * [2022/10] [Use a Laptop to Analyze 90% of Proteins, With a Single-GPU Inference Sequence Exceeding 10,000](https://www.hpc-ai.tech/blog/use-a-laptop-to-analyze-90-of-proteins-with-a-single-gpu-inference-sequence-exceeding)
@@ -56,14 +57,15 @@
              <li><a href="#AIGC">AIGC: Acceleration of Stable Diffusion</a></li>
              <li><a href="#Biomedicine">Biomedicine: Acceleration of AlphaFold Protein Structure</a></li>
            </ul>
          </li>
          <li>
            <a href="#Parallel-Training-Demo">Parallel Training Demo</a>
            <ul>
+             <li><a href="#LLaMA">LLaMA</a></li>
              <li><a href="#GPT-3">GPT-3</a></li>
              <li><a href="#GPT-2">GPT-2</a></li>
              <li><a href="#BERT">BERT</a></li>
              <li><a href="#PaLM">PaLM</a></li>
              <li><a href="#OPT">OPT</a></li>
              <li><a href="#ViT">ViT</a></li>
              <li><a href="#Recommendation-System-Models">Recommendation System Models</a></li>
@@ -223,14 +225,23 @@
         - [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer): accelerating structure prediction of protein monomers and multimer by 11x.
         
         
         <p align="right">(<a href="#top">back to top</a>)</p>
         
         ## Parallel Training Demo
         
+        ### LLaMA
+        <p align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/examples/images/LLaMA_pretraining.png" width=600/>
+        </p>
+        
+        - 65-billion-parameter large model pretraining accelerated by 38%
+        [[code]](https://github.com/hpcaitech/ColossalAI/tree/example/llama/examples/language/llama)
+        [[blog]](https://www.hpc-ai.tech/blog/large-model-pretraining)
+        
         ### GPT-3
         <p align="center">
         <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT3-v5.png" width=700/>
         </p>
         
         - Save 50% GPU resources and 10.7% acceleration
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colossalai Version: 0.3.0 Summary: An integrated
+Metadata-Version: 2.1 Name: colossalai Version: 0.3.1 Summary: An integrated
 large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io Project-URL:
 Github, https://github.com/hpcaitech/ColossalAI Description: # Colossal-AI
@@ -22,43 +22,47 @@
  (https://img.shields.io/badge/%F0%9F%A4%97HuggingFace-Join-yellow)](https://
 huggingface.co/hpcai-tech) [![slack badge](https://img.shields.io/badge/Slack-
   join-blueviolet?logo=slack&)](https://join.slack.com/t/colossalaiworkspace/
   shared_invite/zt-z7b26eeb-CBp7jouvu~r0~lcFzX832w) [![WeChat badge](https://
        img.shields.io/badge/å¾®ä¿¡-å å¥-green?logo=wechat&)](https://
     raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
     WeChat.png) | [English](README.md) | [ä¸­æ](docs/README-zh-Hans.md) |
-## Latest News * [2023/03] [ColossalChat: An Open-Source Solution for Cloning
-ChatGPT With a Complete RLHF Pipeline](https://medium.com/@yangyou_berkeley/
-colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-
-pipeline-5edf08fb538b) * [2023/03] [Intel and Colossal-AI Partner to Deliver
-Cost-Efficient Open-Source Solution for Protein Folding Structure Prediction]
-(https://www.hpc-ai.tech/blog/intel-habana) * [2023/03] [AWS and Google Fund
-Colossal-AI with Startup Cloud Programs](https://www.hpc-ai.tech/blog/aws-and-
-google-fund-colossal-ai-with-startup-cloud-programs) * [2023/02] [Open Source
-Solution Replicates ChatGPT Training Process! Ready to go with only 1.6GB GPU
-Memory](https://www.hpc-ai.tech/blog/colossal-ai-chatgpt) * [2023/01] [Hardware
-Savings Up to 46 Times for AIGC and Automatic Parallelism](https://medium.com/
-pytorch/latest-colossal-ai-boasts-novel-automatic-parallelism-and-offers-
-savings-up-to-46x-for-stable-1453b48f3f02) * [2022/11] [Diffusion Pretraining
-and Hardware Fine-Tuning Can Be Almost 7X Cheaper](https://www.hpc-ai.tech/
-blog/diffusion-pretraining-and-hardware-fine-tuning-can-be-almost-7x-cheaper) *
-[2022/10] [Use a Laptop to Analyze 90% of Proteins, With a Single-GPU Inference
-Sequence Exceeding 10,000](https://www.hpc-ai.tech/blog/use-a-laptop-to-
-analyze-90-of-proteins-with-a-single-gpu-inference-sequence-exceeding) * [2022/
-09] [HPC-AI Tech Completes $6 Million Seed and Angel Round Fundraising](https:/
-/www.hpc-ai.tech/blog/hpc-ai-tech-completes-6-million-seed-and-angel-round-
-fundraising-led-by-bluerun-ventures-in-the) ## Table of Contents
+## Latest News * [2023/07] [65B Model Pretraining Accelerated by 38%, Best
+Practices for Building LLaMA-Like Base Models Open-Source](https://www.hpc-
+ai.tech/blog/large-model-pretraining) * [2023/03] [ColossalChat: An Open-Source
+Solution for Cloning ChatGPT With a Complete RLHF Pipeline](https://medium.com/
+@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-
+with-a-complete-rlhf-pipeline-5edf08fb538b) * [2023/03] [Intel and Colossal-AI
+Partner to Deliver Cost-Efficient Open-Source Solution for Protein Folding
+Structure Prediction](https://www.hpc-ai.tech/blog/intel-habana) * [2023/03]
+[AWS and Google Fund Colossal-AI with Startup Cloud Programs](https://www.hpc-
+ai.tech/blog/aws-and-google-fund-colossal-ai-with-startup-cloud-programs) *
+[2023/02] [Open Source Solution Replicates ChatGPT Training Process! Ready to
+go with only 1.6GB GPU Memory](https://www.hpc-ai.tech/blog/colossal-ai-
+chatgpt) * [2023/01] [Hardware Savings Up to 46 Times for AIGC and Automatic
+Parallelism](https://medium.com/pytorch/latest-colossal-ai-boasts-novel-
+automatic-parallelism-and-offers-savings-up-to-46x-for-stable-1453b48f3f02) *
+[2022/11] [Diffusion Pretraining and Hardware Fine-Tuning Can Be Almost 7X
+Cheaper](https://www.hpc-ai.tech/blog/diffusion-pretraining-and-hardware-fine-
+tuning-can-be-almost-7x-cheaper) * [2022/10] [Use a Laptop to Analyze 90% of
+Proteins, With a Single-GPU Inference Sequence Exceeding 10,000](https://
+www.hpc-ai.tech/blog/use-a-laptop-to-analyze-90-of-proteins-with-a-single-gpu-
+inference-sequence-exceeding) * [2022/09] [HPC-AI Tech Completes $6 Million
+Seed and Angel Round Fundraising](https://www.hpc-ai.tech/blog/hpc-ai-tech-
+completes-6-million-seed-and-angel-round-fundraising-led-by-bluerun-ventures-
+in-the) ## Table of Contents
     * Why_Colossal-AI
     * Features
     * Colossal-AI_for_Real_World_Applications
           o ColossalChat:_An_Open-Source_Solution_for_Cloning_ChatGPT_With_a
             Complete_RLHF_Pipeline
           o AIGC:_Acceleration_of_Stable_Diffusion
           o Biomedicine:_Acceleration_of_AlphaFold_Protein_Structure
     * Parallel_Training_Demo
+          o LLaMA
           o GPT-3
           o GPT-2
           o BERT
           o PaLM
           o OPT
           o ViT
           o Recommendation_System_Models
@@ -151,15 +155,20 @@
 - [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference
 acceleration and 39% cost reduce.
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                            xTrimoMultimer_Table.jpg]
 - [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer):
 accelerating structure prediction of protein monomers and multimer by 11x.
                                                                   (back_to_top)
-## Parallel Training Demo ### GPT-3
+## Parallel Training Demo ### LLaMA
+   [https://raw.githubusercontent.com/hpcaitech/public_assets/main/examples/
+                         images/LLaMA_pretraining.png]
+- 65-billion-parameter large model pretraining accelerated by 38% [[code]]
+(https://github.com/hpcaitech/ColossalAI/tree/example/llama/examples/language/
+llama) [[blog]](https://www.hpc-ai.tech/blog/large-model-pretraining) ### GPT-3
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                                  GPT3-v5.png]
 - Save 50% GPU resources and 10.7% acceleration ### GPT-2 [https://
 raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT2.png]
 - 11x lower GPU memory consumption, and superlinear scaling efficiency with
 Tensor Parallelism [https://raw.githubusercontent.com/hpcaitech/public_assets/
 main/colossalai/img/(updated)GPT-2.png] - 24x larger model size on the same
```

### Comparing `colossalai-0.3.0/colossalai.egg-info/SOURCES.txt` & `colossalai-0.3.1/colossalai.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -45,14 +45,18 @@
 colossalai/amp/naive_amp/_fp16_optimizer.py
 colossalai/amp/naive_amp/_utils.py
 colossalai/amp/naive_amp/naive_amp.py
 colossalai/amp/naive_amp/grad_scaler/__init__.py
 colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
 colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
 colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
+colossalai/amp/naive_amp/mixed_precision_mixin/__init__.py
+colossalai/amp/naive_amp/mixed_precision_mixin/base.py
+colossalai/amp/naive_amp/mixed_precision_mixin/bf16.py
+colossalai/amp/naive_amp/mixed_precision_mixin/fp16.py
 colossalai/amp/torch_amp/__init__.py
 colossalai/amp/torch_amp/_grad_scaler.py
 colossalai/amp/torch_amp/torch_amp.py
 colossalai/auto_parallel/__init__.py
 colossalai/auto_parallel/checkpoint/__init__.py
 colossalai/auto_parallel/checkpoint/build_c_ext.py
 colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
@@ -385,14 +389,16 @@
 colossalai/kernel/op_builder/fused_optim.py
 colossalai/kernel/op_builder/layernorm.py
 colossalai/kernel/op_builder/moe.py
 colossalai/kernel/op_builder/multi_head_attn.py
 colossalai/kernel/op_builder/scaled_masked_softmax.py
 colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py
 colossalai/kernel/op_builder/utils.py
+colossalai/lazy/__init__.py
+colossalai/lazy/lazy_init.py
 colossalai/logging/__init__.py
 colossalai/logging/logger.py
 colossalai/nn/__init__.py
 colossalai/nn/init.py
 colossalai/nn/_ops/__init__.py
 colossalai/nn/_ops/_utils.py
 colossalai/nn/_ops/addmm.py
@@ -502,14 +508,42 @@
 colossalai/pipeline/middleware/adaptor/fx.py
 colossalai/pipeline/rpc/__init__.py
 colossalai/pipeline/rpc/_pipeline_base.py
 colossalai/pipeline/rpc/_pipeline_schedule.py
 colossalai/pipeline/rpc/utils.py
 colossalai/registry/__init__.py
 colossalai/registry/registry.py
+colossalai/shardformer/__init__.py
+colossalai/shardformer/_utils.py
+colossalai/shardformer/layer/__init__.py
+colossalai/shardformer/layer/_operation.py
+colossalai/shardformer/layer/dropout.py
+colossalai/shardformer/layer/embedding.py
+colossalai/shardformer/layer/linear.py
+colossalai/shardformer/layer/loss.py
+colossalai/shardformer/layer/normalization.py
+colossalai/shardformer/layer/parallel_module.py
+colossalai/shardformer/layer/qkv_fused_linear.py
+colossalai/shardformer/layer/utils.py
+colossalai/shardformer/modeling/__init__.py
+colossalai/shardformer/modeling/bloom.py
+colossalai/shardformer/policies/__init__.py
+colossalai/shardformer/policies/autopolicy.py
+colossalai/shardformer/policies/basepolicy.py
+colossalai/shardformer/policies/bert.py
+colossalai/shardformer/policies/bloom.py
+colossalai/shardformer/policies/gpt2.py
+colossalai/shardformer/policies/llama.py
+colossalai/shardformer/policies/opt.py
+colossalai/shardformer/policies/t5.py
+colossalai/shardformer/policies/vit.py
+colossalai/shardformer/shard/__init__.py
+colossalai/shardformer/shard/shard_config.py
+colossalai/shardformer/shard/sharder.py
+colossalai/shardformer/shard/shardformer.py
 colossalai/tensor/__init__.py
 colossalai/tensor/colo_parameter.py
 colossalai/tensor/colo_tensor.py
 colossalai/tensor/comm_spec.py
 colossalai/tensor/compute_spec.py
 colossalai/tensor/const.py
 colossalai/tensor/dist_spec_mgr.py
@@ -518,16 +552,16 @@
 colossalai/tensor/param_op_hook.py
 colossalai/tensor/process_group.py
 colossalai/tensor/shape_consistency.py
 colossalai/tensor/sharding_spec.py
 colossalai/tensor/tensor_spec.py
 colossalai/tensor/utils.py
 colossalai/tensor/d_tensor/__init__.py
+colossalai/tensor/d_tensor/api.py
 colossalai/tensor/d_tensor/comm_spec.py
-colossalai/tensor/d_tensor/d_tensor.py
 colossalai/tensor/d_tensor/layout.py
 colossalai/tensor/d_tensor/layout_converter.py
 colossalai/tensor/d_tensor/misc.py
 colossalai/tensor/d_tensor/sharding_spec.py
 colossalai/tensor/d_tensor/utils.py
 colossalai/testing/__init__.py
 colossalai/testing/comparison.py
@@ -564,16 +598,14 @@
 colossalai/utils/checkpoint_io/reader.py
 colossalai/utils/checkpoint_io/utils.py
 colossalai/utils/checkpoint_io/writer.py
 colossalai/utils/data_sampler/__init__.py
 colossalai/utils/data_sampler/base_sampler.py
 colossalai/utils/data_sampler/data_parallel_sampler.py
 colossalai/utils/model/__init__.py
-colossalai/utils/model/experimental.py
-colossalai/utils/model/lazy_init_context.py
 colossalai/utils/model/utils.py
 colossalai/utils/multi_tensor_apply/__init__.py
 colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
 colossalai/utils/profiler/__init__.py
 colossalai/utils/profiler/extention.py
 colossalai/utils/profiler/profiler.py
 colossalai/utils/profiler/stateful_tensor_mem_extention.py
@@ -689,15 +721,17 @@
 tests/kit/model_zoo/torchrec/__init__.py
 tests/kit/model_zoo/torchrec/torchrec.py
 tests/kit/model_zoo/torchvision/__init__.py
 tests/kit/model_zoo/torchvision/torchvision.py
 tests/kit/model_zoo/transformers/__init__.py
 tests/kit/model_zoo/transformers/albert.py
 tests/kit/model_zoo/transformers/bert.py
+tests/kit/model_zoo/transformers/bloom.py
 tests/kit/model_zoo/transformers/gpt.py
+tests/kit/model_zoo/transformers/llama.py
 tests/kit/model_zoo/transformers/opt.py
 tests/kit/model_zoo/transformers/t5.py
 tests/test_analyzer/__init__.py
 tests/test_analyzer/test_fx/__init__.py
 tests/test_analyzer/test_fx/test_bias_addition.py
 tests/test_analyzer/test_fx/test_mod_dir.py
 tests/test_analyzer/test_fx/test_nested_ckpt.py
@@ -749,8 +783,19 @@
 tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
 tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
 tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
 tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
 tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
 tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
 tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
-tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
+tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
+tests/test_shardformer/__init__.py
+tests/test_shardformer/test_with_torch_ddp.py
+tests/test_shardformer/test_model/__init__.py
+tests/test_shardformer/test_model/_utils.py
+tests/test_shardformer/test_model/test_shard_bert.py
+tests/test_shardformer/test_model/test_shard_bloom.py
+tests/test_shardformer/test_model/test_shard_gpt2.py
+tests/test_shardformer/test_model/test_shard_llama.py
+tests/test_shardformer/test_model/test_shard_opt.py
+tests/test_shardformer/test_model/test_shard_t5.py
+tests/test_shardformer/test_model/test_shard_vit.py
```

### Comparing `colossalai-0.3.0/op_builder/__init__.py` & `colossalai-0.3.1/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/op_builder/builder.py` & `colossalai-0.3.1/op_builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/op_builder/cpu_adam.py` & `colossalai-0.3.1/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/op_builder/fused_optim.py` & `colossalai-0.3.1/op_builder/fused_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/op_builder/layernorm.py` & `colossalai-0.3.1/op_builder/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/op_builder/moe.py` & `colossalai-0.3.1/op_builder/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/op_builder/multi_head_attn.py` & `colossalai-0.3.1/op_builder/multi_head_attn.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/op_builder/scaled_masked_softmax.py` & `colossalai-0.3.1/op_builder/scaled_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/op_builder/scaled_upper_triangle_masked_softmax.py` & `colossalai-0.3.1/op_builder/scaled_upper_triangle_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/op_builder/utils.py` & `colossalai-0.3.1/op_builder/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/requirements/requirements-test.txt` & `colossalai-0.3.1/requirements/requirements-test.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 diffusers
 fbgemm-gpu==0.2.0
 pytest
 coverage==7.2.3
 git+https://github.com/hpcaitech/pytest-testmon
 torchvision
-transformers
+transformers==4.30.2
 timm
 titans
 torchaudio
 torchx-nightly==2022.6.29 # torchrec 0.2.0 requires torchx-nightly. This package is updated every day. We fix the version to a specific date to avoid breaking changes.
 torchrec==0.2.0
 contexttimer
 einops
 triton==2.0.0.dev20221202
 git+https://github.com/HazyResearch/flash-attention.git@c422fee3776eb3ea24e011ef641fd5fbeb212623#egg=flash_attn
 requests==2.27.1 # downgrade to avoid huggingface error https://github.com/huggingface/transformers/issues/17611
+SentencePiece
```

### Comparing `colossalai-0.3.0/setup.py` & `colossalai-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/components_to_test/albert.py` & `colossalai-0.3.1/tests/components_to_test/albert.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/components_to_test/beit.py` & `colossalai-0.3.1/tests/components_to_test/beit.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/components_to_test/bert.py` & `colossalai-0.3.1/tests/components_to_test/bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/components_to_test/gpt2.py` & `colossalai-0.3.1/tests/components_to_test/gpt2.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/components_to_test/hanging_param_model.py` & `colossalai-0.3.1/tests/components_to_test/hanging_param_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/components_to_test/inline_op_model.py` & `colossalai-0.3.1/tests/components_to_test/inline_op_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/components_to_test/nested_model.py` & `colossalai-0.3.1/tests/components_to_test/nested_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/components_to_test/registry.py` & `colossalai-0.3.1/tests/components_to_test/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/components_to_test/repeated_computed_layers.py` & `colossalai-0.3.1/tests/components_to_test/repeated_computed_layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/components_to_test/resnet.py` & `colossalai-0.3.1/tests/components_to_test/resnet.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/components_to_test/simple_net.py` & `colossalai-0.3.1/tests/components_to_test/simple_net.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/components_to_test/utils/executor.py` & `colossalai-0.3.1/tests/components_to_test/utils/executor.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/kit/model_zoo/diffusers/diffusers.py` & `colossalai-0.3.1/tests/kit/model_zoo/diffusers/diffusers.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/kit/model_zoo/registry.py` & `colossalai-0.3.1/tests/kit/model_zoo/registry.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 from dataclasses import dataclass
 from typing import Callable
 
-__all__ = ['ModelZooRegistry', 'ModelAttributem', 'model_zoo']
+__all__ = ['ModelZooRegistry', 'ModelAttribute', 'model_zoo']
 
 
 @dataclass
 class ModelAttribute:
     """
     Attributes of a model.
 
@@ -24,45 +24,55 @@
     """
 
     def register(self,
                  name: str,
                  model_fn: Callable,
                  data_gen_fn: Callable,
                  output_transform_fn: Callable,
+                 loss_fn: Callable = None,
                  model_attribute: ModelAttribute = None):
         """
         Register a model and data generation function.
 
         Examples:
-        >>> # Register
-        >>> model_zoo = ModelZooRegistry()
-        >>> model_zoo.register('resnet18', resnet18, resnet18_data_gen)
-        >>> # Run the model
-        >>> data = resnresnet18_data_gen() # do not input any argument
-        >>> model = resnet18() # do not input any argument
-        >>> out = model(**data)
+
+        ```python
+        # normal forward workflow
+        model = resnet18()
+        data = resnet18_data_gen()
+        output = model(**data)
+        transformed_output = output_transform_fn(output)
+        loss = loss_fn(transformed_output)
+
+        # Register
+        model_zoo = ModelZooRegistry()
+        model_zoo.register('resnet18', resnet18, resnet18_data_gen, output_transform_fn, loss_fn)
+        ```
 
         Args:
             name (str): Name of the model.
-            model_fn (callable): A function that returns a model. **It must not contain any arguments.**
-            output_transform_fn (callable): A function that transforms the output of the model into Dict.
-            data_gen_fn (callable): A function that returns a data sample in the form of Dict. **It must not contain any arguments.**
+            model_fn (Callable): A function that returns a model. **It must not contain any arguments.**
+            data_gen_fn (Callable): A function that returns a data sample in the form of Dict. **It must not contain any arguments.**
+            output_transform_fn (Callable): A function that transforms the output of the model into Dict.
+            loss_fn (Callable): a function to compute the loss from the given output. Defaults to None
             model_attribute (ModelAttribute): Attributes of the model. Defaults to None.
         """
-        self[name] = (model_fn, data_gen_fn, output_transform_fn, model_attribute)
+        self[name] = (model_fn, data_gen_fn, output_transform_fn, loss_fn, model_attribute)
 
     def get_sub_registry(self, keyword: str):
         """
         Get a sub registry with models that contain the keyword.
 
         Args:
             keyword (str): Keyword to filter models.
         """
         new_dict = dict()
 
         for k, v in self.items():
             if keyword in k:
                 new_dict[k] = v
+
+        assert len(new_dict) > 0, f'No model found with keyword {keyword}'
         return new_dict
 
 
 model_zoo = ModelZooRegistry()
```

### Comparing `colossalai-0.3.0/tests/kit/model_zoo/timm/timm.py` & `colossalai-0.3.1/tests/kit/model_zoo/timm/timm.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/kit/model_zoo/torchaudio/torchaudio.py` & `colossalai-0.3.1/tests/kit/model_zoo/torchaudio/torchaudio.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/kit/model_zoo/torchrec/torchrec.py` & `colossalai-0.3.1/tests/kit/model_zoo/torchrec/torchrec.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/kit/model_zoo/torchvision/torchvision.py` & `colossalai-0.3.1/tests/kit/model_zoo/torchvision/torchvision.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/kit/model_zoo/transformers/albert.py` & `colossalai-0.3.1/tests/kit/model_zoo/transformers/albert.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/kit/model_zoo/transformers/bert.py` & `colossalai-0.3.1/tests/kit/model_zoo/transformers/gpt.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,88 +1,94 @@
 import torch
 import transformers
 
 from ..registry import ModelAttribute, model_zoo
 
 # ===============================
-# Register single-sentence BERT
+# Register single-sentence GPT
 # ===============================
-BATCH_SIZE = 2
-SEQ_LENGTH = 16
 
 
-def data_gen_fn():
-    input_ids = torch.zeros((BATCH_SIZE, SEQ_LENGTH), dtype=torch.int64)
-    token_type_ids = torch.zeros((BATCH_SIZE, SEQ_LENGTH), dtype=torch.int64)
-    attention_mask = torch.zeros((BATCH_SIZE, SEQ_LENGTH), dtype=torch.int64)
-    return dict(input_ids=input_ids, token_type_ids=token_type_ids, attention_mask=attention_mask)
+def data_gen():
+    # Generated from following code snippet
+    #
+    # from transformers import GPT2Tokenizer
+    # input = 'Hello, my dog is cute'
+    # tokenized_input = tokenizer(input, return_tensors='pt')
+    # input_ids = tokenized_input['input_ids']
+    # attention_mask = tokenized_input['attention_mask']
+    input_ids = torch.tensor([[15496, 11, 616, 3290, 318, 13779]], dtype=torch.int64)
+    attention_mask = torch.tensor([[1, 1, 1, 1, 1, 1]], dtype=torch.int64)
+    return dict(input_ids=input_ids, attention_mask=attention_mask)
+
+
+def data_gen_for_lm():
+    # LM data gen
+    # the `labels` of LM is the token of the output, cause no padding, use `input_ids` as `labels`
+    data = data_gen()
+    data['labels'] = data['input_ids'].clone()
+    return data
+
+
+def data_gen_for_token_classification():
+    # token classification data gen
+    # `labels` is the type not the token id for token classification, 0 or 1
+    data = data_gen()
+    data['labels'] = torch.tensor([[0, 0, 0, 0, 0, 0]], dtype=torch.int64)
+    return data
+
+
+def data_gen_for_sequence_classification():
+    # sequence classification data gen
+    data = data_gen()
+    data['labels'] = torch.tensor([0], dtype=torch.int64)
+    return data
 
 
+# define output transform function
 output_transform_fn = lambda x: x
 
-config = transformers.BertConfig(hidden_size=128, num_hidden_layers=2, num_attention_heads=4, intermediate_size=256)
+# define loss function
+loss_fn_for_gpt2_model = lambda x: x.last_hidden_state.mean()
+loss_fn = lambda x: x.loss
+
+config = transformers.GPT2Config(n_layer=2,
+                                 n_head=4,
+                                 vocab_size=50258,
+                                 attn_pdrop=0,
+                                 embd_pdrop=0,
+                                 resid_pdrop=0,
+                                 summary_first_dropout=0,
+                                 hidden_dropout=0,
+                                 problem_type="single_label_classification")
 
-# register the BERT variants
-model_zoo.register(name='transformers_bert',
-                   model_fn=lambda: transformers.BertModel(config),
-                   data_gen_fn=data_gen_fn,
-                   output_transform_fn=output_transform_fn,
-                   model_attribute=ModelAttribute(has_control_flow=True))
-model_zoo.register(name='transformers_bert_for_pretraining',
-                   model_fn=lambda: transformers.BertForPreTraining(config),
-                   data_gen_fn=data_gen_fn,
-                   output_transform_fn=output_transform_fn,
-                   model_attribute=ModelAttribute(has_control_flow=True))
-model_zoo.register(name='transformers_bert_lm_head_model',
-                   model_fn=lambda: transformers.BertLMHeadModel(config),
-                   data_gen_fn=data_gen_fn,
-                   output_transform_fn=output_transform_fn,
-                   model_attribute=ModelAttribute(has_control_flow=True))
-model_zoo.register(name='transformers_bert_for_masked_lm',
-                   model_fn=lambda: transformers.BertForMaskedLM(config),
-                   data_gen_fn=data_gen_fn,
+# register the following models
+model_zoo.register(name='transformers_gpt',
+                   model_fn=lambda: transformers.GPT2Model(config),
+                   data_gen_fn=data_gen,
                    output_transform_fn=output_transform_fn,
+                   loss_fn=loss_fn_for_gpt2_model,
                    model_attribute=ModelAttribute(has_control_flow=True))
-model_zoo.register(name='transformers_bert_for_sequence_classification',
-                   model_fn=lambda: transformers.BertForSequenceClassification(config),
-                   data_gen_fn=data_gen_fn,
+model_zoo.register(name='transformers_gpt_lm',
+                   model_fn=lambda: transformers.GPT2LMHeadModel(config),
+                   data_gen_fn=data_gen_for_lm,
                    output_transform_fn=output_transform_fn,
+                   loss_fn=loss_fn,
                    model_attribute=ModelAttribute(has_control_flow=True))
-model_zoo.register(name='transformers_bert_for_token_classification',
-                   model_fn=lambda: transformers.BertForTokenClassification(config),
-                   data_gen_fn=data_gen_fn,
+model_zoo.register(name='transformers_gpt_double_heads',
+                   model_fn=lambda: transformers.GPT2DoubleHeadsModel(config),
+                   data_gen_fn=data_gen_for_lm,
                    output_transform_fn=output_transform_fn,
+                   loss_fn=loss_fn,
                    model_attribute=ModelAttribute(has_control_flow=True))
-
-
-# ===============================
-# Register multi-sentence BERT
-# ===============================
-def data_gen_for_next_sentence():
-    tokenizer = transformers.BertTokenizer.from_pretrained("bert-base-uncased")
-    prompt = "In Italy, pizza served in formal settings, such as at a restaurant, is presented unsliced."
-    next_sentence = "The sky is blue due to the shorter wavelength of blue light."
-    encoding = tokenizer(prompt, next_sentence, return_tensors="pt")
-    return encoding
-
-
-def data_gen_for_mcq():
-    tokenizer = transformers.BertTokenizer.from_pretrained("bert-base-uncased")
-    prompt = "In Italy, pizza served in formal settings, such as at a restaurant, is presented unsliced."
-    choice0 = "It is eaten with a fork and a knife."
-    choice1 = "It is eaten while held in the hand."
-    encoding = tokenizer([prompt, prompt], [choice0, choice1], return_tensors="pt", padding=True)
-    encoding = {k: v.unsqueeze(0) for k, v in encoding.items()}
-    return encoding
-
-
-# register the following models
-model_zoo.register(name='transformers_bert_for_next_sentence',
-                   model_fn=lambda: transformers.BertForNextSentencePrediction(config),
-                   data_gen_fn=data_gen_for_next_sentence,
+model_zoo.register(name='transformers_gpt_for_token_classification',
+                   model_fn=lambda: transformers.GPT2ForTokenClassification(config),
+                   data_gen_fn=data_gen_for_token_classification,
                    output_transform_fn=output_transform_fn,
+                   loss_fn=loss_fn,
                    model_attribute=ModelAttribute(has_control_flow=True))
-model_zoo.register(name='transformers_bert_for_mcq',
-                   model_fn=lambda: transformers.BertForMultipleChoice(config),
-                   data_gen_fn=data_gen_for_mcq,
+model_zoo.register(name='transformers_gpt_for_sequence_classification',
+                   model_fn=lambda: transformers.GPT2ForSequenceClassification(config),
+                   data_gen_fn=data_gen_for_sequence_classification,
                    output_transform_fn=output_transform_fn,
+                   loss_fn=loss_fn,
                    model_attribute=ModelAttribute(has_control_flow=True))
```

### Comparing `colossalai-0.3.0/tests/test_analyzer/test_fx/test_bias_addition.py` & `colossalai-0.3.1/tests/test_analyzer/test_fx/test_bias_addition.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_analyzer/test_fx/test_mod_dir.py` & `colossalai-0.3.1/tests/test_analyzer/test_fx/test_mod_dir.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_analyzer/test_fx/test_nested_ckpt.py` & `colossalai-0.3.1/tests/test_analyzer/test_fx/test_nested_ckpt.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_analyzer/test_fx/test_shape_prop.py` & `colossalai-0.3.1/tests/test_analyzer/test_fx/test_shape_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_analyzer/test_fx/test_symbolic_profile.py` & `colossalai-0.3.1/tests/test_analyzer/test_fx/test_symbolic_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_analyzer/test_fx/zoo.py` & `colossalai-0.3.1/tests/test_analyzer/test_fx/zoo.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_analyzer/test_subclasses/test_aten.py` & `colossalai-0.3.1/tests/test_analyzer/test_subclasses/test_aten.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_analyzer/test_subclasses/test_flop_tensor.py` & `colossalai-0.3.1/tests/test_analyzer/test_subclasses/test_flop_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_analyzer/test_subclasses/test_meta_mode.py` & `colossalai-0.3.1/tests/test_analyzer/test_subclasses/test_meta_mode.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_pass/test_node_converting_pass.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_pass/test_node_converting_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         print('=' * msg_length)
 
     dp_process_group = ProcessGroup(rank=rank, ranks=[0, 1, 2, 3], tp_degree=2, dp_degree=2)
     gemini_config = dict(strict_ddp_mode=False,
                          device=get_current_device(),
                          placement_policy='cpu',
                          pin_memory=True,
-                         search_range_mb=128)
+                         search_range_m=128)
 
     post_process_colo_init_ctx(gm, device=get_current_device(), default_pg=dp_process_group)
     gm = zero_model_wrapper(gm, zero_stage=3, gemini_config=gemini_config)
     optimizer = HybridAdam(gm.parameters(), betas=(0, 0))
     optimizer = zero_optim_wrapper(gm, optimizer, initial_scale=1)
     output = gm(input)
     if rank in (0, 1):
```

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     mesh_shape = (2, 2)
     device_mesh = DeviceMesh(physical_mesh_id, mesh_shape, init_process_group=True)
     input = torch.rand(4, 16, 64, 64).cuda()
     # the index of bn node in computation graph
     node_index = 1
     # the total number of bn strategies without sync bn mode
-    # TODO: add sync bn stategies after related passes ready
+    # TODO: add sync bn strategies after related passes ready
     strategy_number = 4
     numerical_test_for_node_strategy(model=model,
                                      device_mesh=device_mesh,
                                      node_index=node_index,
                                      strategy_number=strategy_number,
                                      input_args=[input],
                                      meta_arg_names=['input'])
```

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,31 +39,31 @@
 
     mesh_shape = (2, 2)
     device_mesh = DeviceMesh(physical_mesh_id, mesh_shape)
     output_node = list(graph.nodes)[2]
     output_strategies_vector = StrategiesVector(output_node)
 
     # build handler
-    otuput_handler = OutputHandler(node=output_node,
+    output_handler = OutputHandler(node=output_node,
                                    device_mesh=device_mesh,
                                    strategies_vector=output_strategies_vector,
                                    output_option=output_option)
 
-    otuput_handler.register_strategy(compute_resharding_cost=False)
+    output_handler.register_strategy(compute_resharding_cost=False)
     # check operation data mapping
-    mapping = otuput_handler.get_operation_data_mapping()
+    mapping = output_handler.get_operation_data_mapping()
 
     for name, op_data in mapping.items():
         op_data: OperationData
         # make sure they have valid values
         assert op_data.data is not None
 
     assert mapping['output'].name == "output"
     assert mapping['output'].type == OperationDataType.OUTPUT
-    strategy_name_list = [val.name for val in otuput_handler.strategies_vector]
+    strategy_name_list = [val.name for val in output_handler.strategies_vector]
     if output_option == 'distributed':
         assert "Distributed Output" in strategy_name_list
     else:
         assert "Replica Output" in strategy_name_list
 
 
 if __name__ == '__main__':
```

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-0.3.0/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py` & `colossalai-0.3.1/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py`

 * *Files identical despite different names*

