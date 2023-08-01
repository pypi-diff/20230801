# Comparing `tmp/ml-starter-0.1.41.tar.gz` & `tmp/ml-starter-0.1.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.1.41.tar", last modified: Fri Jul 28 21:52:34 2023, max compression
+gzip compressed data, was "ml-starter-0.1.42.tar", last modified: Tue Aug  1 02:02:55 2023, max compression
```

## Comparing `ml-starter-0.1.41.tar` & `ml-starter-0.1.42.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.550255 ml-starter-0.1.41/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-28 21:52:19.000000 ml-starter-0.1.41/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-28 21:52:19.000000 ml-starter-0.1.41/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-28 21:52:34.550255 ml-starter-0.1.41/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-28 21:52:19.000000 ml-starter-0.1.41/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.530255 ml-starter-0.1.41/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.530255 ml-starter-0.1.41/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.534255 ml-starter-0.1.41/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/launchers/sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.534255 ml-starter-0.1.41/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    46173 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.534255 ml-starter-0.1.41/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/lr_schedulers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.534255 ml-starter-0.1.41/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.534255 ml-starter-0.1.41/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/activations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.534255 ml-starter-0.1.41/ml/models/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/architectures/bifpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/architectures/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/codebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    56335 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.538255 ml-starter-0.1.41/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/optimizers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.538255 ml-starter-0.1.41/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.538255 ml-starter-0.1.41/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19251 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.538255 ml-starter-0.1.41/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.538255 ml-starter-0.1.41/ml/tasks/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/diffusion/beta_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/diffusion/gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.542255 ml-starter-0.1.41/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.542255 ml-starter-0.1.41/ml/tasks/gan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/gan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/gan/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.542255 ml-starter-0.1.41/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/losses/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/losses/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/losses/kl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/losses/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.542255 ml-starter-0.1.41/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.542255 ml-starter-0.1.41/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.542255 ml-starter-0.1.41/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24976 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.542255 ml-starter-0.1.41/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.546255 ml-starter-0.1.41/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    38804 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.550255 ml-starter-0.1.41/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/torch_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.550255 ml-starter-0.1.41/ml/utils/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/triton/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/triton/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-07-28 21:52:19.000000 ml-starter-0.1.41/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:34.550255 ml-starter-0.1.41/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-28 21:52:34.000000 ml-starter-0.1.41/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-28 21:52:34.000000 ml-starter-0.1.41/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 21:52:34.000000 ml-starter-0.1.41/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-28 21:52:34.000000 ml-starter-0.1.41/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-28 21:52:34.000000 ml-starter-0.1.41/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-28 21:52:19.000000 ml-starter-0.1.41/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-28 21:52:34.550255 ml-starter-0.1.41/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-28 21:52:19.000000 ml-starter-0.1.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.400644 ml-starter-0.1.42/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-01 02:02:40.000000 ml-starter-0.1.42/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-01 02:02:40.000000 ml-starter-0.1.42/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-01 02:02:55.400644 ml-starter-0.1.42/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-01 02:02:40.000000 ml-starter-0.1.42/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.368644 ml-starter-0.1.42/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.372644 ml-starter-0.1.42/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.372644 ml-starter-0.1.42/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/launchers/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.372644 ml-starter-0.1.42/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46173 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.376644 ml-starter-0.1.42/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/lr_schedulers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.376644 ml-starter-0.1.42/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.376644 ml-starter-0.1.42/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/models/activations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.376644 ml-starter-0.1.42/ml/models/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/models/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/models/architectures/bifpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/models/architectures/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17399 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/models/codebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/models/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56335 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/models/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.380644 ml-starter-0.1.42/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/optimizers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.380644 ml-starter-0.1.42/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.380644 ml-starter-0.1.42/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19251 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.384644 ml-starter-0.1.42/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.384644 ml-starter-0.1.42/ml/tasks/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/diffusion/beta_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/diffusion/gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.384644 ml-starter-0.1.42/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.388644 ml-starter-0.1.42/ml/tasks/gan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/gan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/gan/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.388644 ml-starter-0.1.42/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/losses/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/losses/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/losses/kl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/losses/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.388644 ml-starter-0.1.42/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.388644 ml-starter-0.1.42/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.388644 ml-starter-0.1.42/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24976 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/trainers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.392644 ml-starter-0.1.42/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.400644 ml-starter-0.1.42/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38804 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.400644 ml-starter-0.1.42/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.400644 ml-starter-0.1.42/ml/utils/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/triton/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-08-01 02:02:40.000000 ml-starter-0.1.42/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:02:55.400644 ml-starter-0.1.42/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-01 02:02:55.000000 ml-starter-0.1.42/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-01 02:02:55.000000 ml-starter-0.1.42/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 02:02:55.000000 ml-starter-0.1.42/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-01 02:02:55.000000 ml-starter-0.1.42/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-01 02:02:55.000000 ml-starter-0.1.42/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-08-01 02:02:40.000000 ml-starter-0.1.42/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-01 02:02:55.404644 ml-starter-0.1.42/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-01 02:02:40.000000 ml-starter-0.1.42/setup.py
```

### Comparing `ml-starter-0.1.41/LICENSE` & `ml-starter-0.1.42/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/PKG-INFO` & `ml-starter-0.1.42/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.41
+Version: 0.1.42
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.41/README.md` & `ml-starter-0.1.42/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/api.py` & `ml-starter-0.1.42/ml/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,22 +58,24 @@
     "Clamp",
     "ClippifyDataset",
     "collate_non_null",
     "collate",
     "CollateMode",
     "colorize",
     "ColumnParallelLinear",
+    "combine_grads",
     "ConcatSpeakerDataset",
     "conf_field",
     "configure_logging",
     "detect_device",
     "DictIndex",
     "DiffusionBetaSchedule",
     "ensure_downloaded",
     "Environment",
+    "FixedTargetCodebook",
     "FolderSpeakerDataset",
     "format_timedelta",
     "freeze_non_lora_",
     "from_args",
     "GaussianDiffusion",
     "GenerativeAdversarialNetworkTask",
     "GenerativeAdversarialNetworkTaskConfig",
@@ -174,14 +176,15 @@
     "register_trainer",
     "ReinforcementLearningTask",
     "ReinforcementLearningTaskConfig",
     "ReinforcementLearningTrainer",
     "ReinforcementLearningTrainerConfig",
     "reset_lora_weights_",
     "reset_parallelism",
+    "ResidualVectorQuantization",
     "RotaryEmbeddings",
     "RowParallelLinear",
     "scale_grad",
     "set_default_audio_reader",
     "set_default_audio_writer",
     "set_distributed_backend",
     "set_random_seed",
@@ -195,25 +198,27 @@
     "State",
     "StreamingDataset",
     "StreamingDatasetNoIndex",
     "SupervisedLearningTask",
     "SupervisedLearningTaskConfig",
     "SupervisedLearningTrainer",
     "SupervisedLearningTrainerConfig",
+    "swap_grads",
     "SyncEnvironmentWorker",
     "SyncWorkerPool",
     "test_dataset",
     "test_environment",
     "test_task",
     "timeout",
     "Timer",
     "TokenReader",
     "TokenWriter",
     "transforms",
     "UNet",
+    "VectorQuantization",
     "VideoFileDataset",
     "WorkerPool",
     "write_audio",
     "write_gif",
     "write_video",
 ]
 
@@ -243,14 +248,15 @@
 from ml.launchers.slurm import SlurmLauncher, SlurmLauncherConfig, set_slurm_master_addr, set_slurm_rank_and_world_size
 from ml.loggers.multi import namespace_context
 from ml.lr_schedulers.base import BaseLRScheduler, BaseLRSchedulerConfig
 from ml.models.activations import ActivationType, Clamp, cast_activation_type, get_activation
 from ml.models.architectures.bifpn import BiFPN
 from ml.models.architectures.unet import UNet
 from ml.models.base import BaseModel, BaseModelConfig
+from ml.models.codebook import FixedTargetCodebook, ResidualVectorQuantization, VectorQuantization
 from ml.models.embeddings import (
     LearnedPositionalEmbeddings,
     RotaryEmbeddings,
     SinusoidalEmbeddings,
     cast_embedding_kind,
     get_positional_embeddings,
 )
@@ -267,15 +273,15 @@
     LoraLSTM,
     freeze_non_lora_,
     lora,
     maybe_lora,
     maybe_lora_weight_norm,
     reset_lora_weights_,
 )
-from ml.models.modules import invert_grad, scale_grad
+from ml.models.modules import combine_grads, invert_grad, scale_grad, swap_grads
 from ml.models.norms import NormType, cast_norm_type, get_norm_1d, get_norm_2d, get_norm_3d, get_norm_linear
 from ml.models.parallel import ColumnParallelLinear, ParallelEmbedding, RowParallelLinear
 from ml.optimizers.base import BaseOptimizer, BaseOptimizerConfig
 from ml.tasks.base import BaseTask, BaseTaskConfig
 from ml.tasks.datasets import transforms
 from ml.tasks.datasets.async_iterable import AsyncIterableDataset
 from ml.tasks.datasets.clippify import ClippifyDataset
```

### Comparing `ml-starter-0.1.41/ml/core/common_types.py` & `ml-starter-0.1.42/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/core/config.py` & `ml-starter-0.1.42/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/core/env.py` & `ml-starter-0.1.42/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/core/registry.py` & `ml-starter-0.1.42/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/core/state.py` & `ml-starter-0.1.42/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/launchers/base.py` & `ml-starter-0.1.42/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/launchers/mp.py` & `ml-starter-0.1.42/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/launchers/sagemaker.py` & `ml-starter-0.1.42/ml/launchers/sagemaker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/launchers/slurm.py` & `ml-starter-0.1.42/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/launchers/torchrun.py` & `ml-starter-0.1.42/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/loggers/base.py` & `ml-starter-0.1.42/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/loggers/meter.py` & `ml-starter-0.1.42/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/loggers/multi.py` & `ml-starter-0.1.42/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/loggers/stdout.py` & `ml-starter-0.1.42/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/loggers/tensorboard.py` & `ml-starter-0.1.42/ml/loggers/tensorboard.py`

 * *Files 3% similar despite different names*

```diff
@@ -288,14 +288,15 @@
             cur_time = time.time()
             if cur_time - self.last_tensorboard_write_time > WRITE_PROC_TEXT_EVERY_N_SECONDS:
                 logger.info("Running TensorBoard process:\n%s", make_bold([self.line_str], "light-green", "cyan"))
                 self.last_tensorboard_write_time = cur_time
 
         writer = self.get_writer(state.phase)
         all_keys: set[str] = set()
+        walltime = state.start_time_s + state.elapsed_time_s
 
         def filter_items(items: Iterable[tuple[str, T]]) -> Iterable[tuple[str, T]]:
             duplicate_keys: set[str] = set()
             for k, v in items:
                 if k in all_keys:
                     duplicate_keys
                 else:
@@ -305,79 +306,79 @@
                 logger.warning("Found duplicate logging key(s): %s", duplicate_keys)
 
         for scalar_key, scalar_value in filter_items(self.scalars[state.phase].items()):
             writer.add_scalar(
                 scalar_key,
                 scalar_value(),
                 global_step=state.num_steps,
-                walltime=state.elapsed_time_s,
+                walltime=walltime,
             )
 
         for string_key, string_value in filter_items(self.strings[state.phase].items()):
             writer.add_text(
                 string_key,
                 string_value(),
                 global_step=state.num_steps,
-                walltime=state.elapsed_time_s,
+                walltime=walltime,
             )
 
         for image_key, image_value in filter_items(self.images[state.phase].items()):
             writer.add_image(
                 image_key,
                 image_value(),
                 global_step=state.num_steps,
-                walltime=state.elapsed_time_s,
+                walltime=walltime,
             )
 
         for audio_key, audio_value in filter_items(self.audio[state.phase].items()):
             audio_wav, audio_sample_rate = audio_value()
             writer.add_audio(
                 audio_key,
                 audio_wav,
                 global_step=state.num_steps,
-                walltime=state.elapsed_time_s,
+                walltime=walltime,
                 sample_rate=audio_sample_rate,
             )
 
         for video_key, video_value in filter_items(self.videos[state.phase].items()):
             writer.add_video(
                 video_key,
                 video_value().unsqueeze(0),
                 global_step=state.num_steps,
-                walltime=state.elapsed_time_s,
+                walltime=walltime,
                 fps=TARGET_FPS,
             )
 
         for hist_key, hist_value in filter_items(self.histograms[state.phase].items()):
             writer.add_histogram(
                 hist_key,
                 hist_value(),
                 global_step=state.num_steps,
-                walltime=state.elapsed_time_s,
+                walltime=walltime,
             )
 
         for pc_key, pc_value_func in filter_items(self.point_clouds[state.phase].items()):
             pc_value = pc_value_func()
             bsz, _, _ = pc_value.shape
             colors = torch.randint(0, 255, (bsz, 1, 3), device=pc_value.device).expand_as(pc_value)
             pc_value, colors = pc_value.flatten(0, 1).unsqueeze(0), colors.flatten(0, 1).unsqueeze(0)
             writer.add_mesh(
                 pc_key,
                 pc_value,
                 colors=colors,
                 global_step=state.num_steps,
-                walltime=state.elapsed_time_s,
+                walltime=walltime,
             )
 
         if not self.logged_run_config and self.run_config is not None:
             writer.add_text(
                 "config",
                 to_markdown_table(self.run_config),
                 global_step=state.num_steps,
-                walltime=state.elapsed_time_s,
+                walltime=walltime,
             )
             self.logged_run_config = True
 
         self.clear(state)
 
     def clear(self, state: State) -> None:
         self.scalars[state.phase].clear()
```

### Comparing `ml-starter-0.1.41/ml/lr_schedulers/base.py` & `ml-starter-0.1.42/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/lr_schedulers/constant.py` & `ml-starter-0.1.42/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/lr_schedulers/cosine.py` & `ml-starter-0.1.42/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.1.42/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/lr_schedulers/gan.py` & `ml-starter-0.1.42/ml/lr_schedulers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/lr_schedulers/linear.py` & `ml-starter-0.1.42/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.1.42/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.1.42/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/models/activations.py` & `ml-starter-0.1.42/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/models/architectures/bifpn.py` & `ml-starter-0.1.42/ml/models/architectures/bifpn.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/models/architectures/unet.py` & `ml-starter-0.1.42/ml/models/architectures/unet.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/models/base.py` & `ml-starter-0.1.42/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/models/embeddings.py` & `ml-starter-0.1.42/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/models/gan.py` & `ml-starter-0.1.42/ml/models/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/models/init.py` & `ml-starter-0.1.42/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/models/kmeans.py` & `ml-starter-0.1.42/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/models/lora.py` & `ml-starter-0.1.42/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/models/norms.py` & `ml-starter-0.1.42/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/models/parallel.py` & `ml-starter-0.1.42/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/optimizers/adam.py` & `ml-starter-0.1.42/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/optimizers/adan.py` & `ml-starter-0.1.42/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/optimizers/base.py` & `ml-starter-0.1.42/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/optimizers/common.py` & `ml-starter-0.1.42/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/optimizers/gan.py` & `ml-starter-0.1.42/ml/optimizers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/optimizers/lion.py` & `ml-starter-0.1.42/ml/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/optimizers/sgd.py` & `ml-starter-0.1.42/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/optimizers/shampoo.py` & `ml-starter-0.1.42/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/scripts/cli.py` & `ml-starter-0.1.42/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/scripts/stage.py` & `ml-starter-0.1.42/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/scripts/train.py` & `ml-starter-0.1.42/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/base.py` & `ml-starter-0.1.42/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.1.42/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/datasets/clippify.py` & `ml-starter-0.1.42/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/datasets/collate.py` & `ml-starter-0.1.42/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/datasets/error_handling.py` & `ml-starter-0.1.42/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.1.42/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/datasets/samplers.py` & `ml-starter-0.1.42/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/datasets/streaming.py` & `ml-starter-0.1.42/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/datasets/transforms.py` & `ml-starter-0.1.42/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/datasets/video_file.py` & `ml-starter-0.1.42/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/diffusion/beta_schedule.py` & `ml-starter-0.1.42/ml/tasks/diffusion/beta_schedule.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/diffusion/gaussian.py` & `ml-starter-0.1.42/ml/tasks/diffusion/gaussian.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/environments/base.py` & `ml-starter-0.1.42/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/environments/utils.py` & `ml-starter-0.1.42/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/environments/worker.py` & `ml-starter-0.1.42/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/gan/base.py` & `ml-starter-0.1.42/ml/tasks/gan/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/losses/audio.py` & `ml-starter-0.1.42/ml/tasks/losses/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/losses/image.py` & `ml-starter-0.1.42/ml/tasks/losses/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/losses/kl.py` & `ml-starter-0.1.42/ml/tasks/losses/kl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/losses/loss.py` & `ml-starter-0.1.42/ml/tasks/losses/loss.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/rl/base.py` & `ml-starter-0.1.42/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/rl/replay.py` & `ml-starter-0.1.42/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/tasks/sl/base.py` & `ml-starter-0.1.42/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/trainers/base.py` & `ml-starter-0.1.42/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/trainers/gan.py` & `ml-starter-0.1.42/ml/trainers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/trainers/learning.py` & `ml-starter-0.1.42/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/trainers/mixins/compile.py` & `ml-starter-0.1.42/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.1.42/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.1.42/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.1.42/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.1.42/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.1.42/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.1.42/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/trainers/mixins/profiler.py` & `ml-starter-0.1.42/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.1.42/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/trainers/rl.py` & `ml-starter-0.1.42/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/trainers/sl.py` & `ml-starter-0.1.42/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/amp.py` & `ml-starter-0.1.42/ml/utils/amp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/argparse.py` & `ml-starter-0.1.42/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/atomic.py` & `ml-starter-0.1.42/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/attention.py` & `ml-starter-0.1.42/ml/utils/attention.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/audio.py` & `ml-starter-0.1.42/ml/utils/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/augmentation.py` & `ml-starter-0.1.42/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/caching.py` & `ml-starter-0.1.42/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/checkpoint.py` & `ml-starter-0.1.42/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/cli.py` & `ml-starter-0.1.42/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/colors.py` & `ml-starter-0.1.42/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/containers.py` & `ml-starter-0.1.42/ml/utils/containers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/data.py` & `ml-starter-0.1.42/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/datetime.py` & `ml-starter-0.1.42/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/device/auto.py` & `ml-starter-0.1.42/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/device/base.py` & `ml-starter-0.1.42/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/device/cpu.py` & `ml-starter-0.1.42/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/device/gpu.py` & `ml-starter-0.1.42/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/device/metal.py` & `ml-starter-0.1.42/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/distributed.py` & `ml-starter-0.1.42/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/exceptions.py` & `ml-starter-0.1.42/ml/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/image.py` & `ml-starter-0.1.42/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/io.py` & `ml-starter-0.1.42/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/large_models.py` & `ml-starter-0.1.42/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/logging.py` & `ml-starter-0.1.42/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/meter.py` & `ml-starter-0.1.42/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/mixed_precision.py` & `ml-starter-0.1.42/ml/utils/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/networking.py` & `ml-starter-0.1.42/ml/utils/networking.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/numpy.py` & `ml-starter-0.1.42/ml/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/parallel.py` & `ml-starter-0.1.42/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/spectrogram.py` & `ml-starter-0.1.42/ml/utils/spectrogram.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/staging.py` & `ml-starter-0.1.42/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/testing.py` & `ml-starter-0.1.42/ml/utils/testing.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/timer.py` & `ml-starter-0.1.42/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/tokens.py` & `ml-starter-0.1.42/ml/utils/tokens.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,53 +50,69 @@
 import functools
 import gzip
 import logging
 import math
 import struct
 from pathlib import Path
 from types import TracebackType
-from typing import BinaryIO, ContextManager, Literal, Sequence
+from typing import BinaryIO, ContextManager, Iterable, Literal
 
 logger = logging.getLogger(__name__)
 
 NumberFormat = Literal["Q", "I", "H", "B"]
 
 MAGIC = b"MLTK"  # Magic number for the token file format.
 OFFSET_MAGIC = b"MLTO"  # Magic number for the offsets file format.
 
 
-def _arr_to_bytes(tokens: Sequence[int], num_tokens: int) -> bytes:
+def _arr_to_bytes(tokens: Iterable[int], num_tokens: int, offset: int = 0) -> tuple[bytes, int]:
+    assert 0 <= offset < 8
     num_bits = (num_tokens - 1).bit_length()
-    assert all(0 <= token < num_tokens for token in tokens)
     byte_arr = bytearray()
-    cur_token = ""
+    cur_token = 0
+    cur_bits = 0
+    total_len = 0
     for token in tokens:
-        cur_token += f"{token:0{num_bits}b}"
-        byte_arr.extend(int(cur_token[i * 8 : (i + 1) * 8], 2) for i in range(len(cur_token) // 8))
-        cur_token = cur_token[len(cur_token) // 8 * 8 :]
-    if cur_token:
-        byte_arr.append(int(cur_token.ljust(8, "0"), 2))
-    # Visualize byte array: f'{int(byte_arr.hex(), base=16):b}'
-    return bytes(byte_arr)
+        total_len += 1
+        assert 0 <= token <= num_tokens
+        cur_token += token << cur_bits
+        cur_bits += num_bits
+        if offset > 0:
+            cur_token <<= offset
+            cur_bits += offset
+            offset = 0
+        while cur_bits >= 8:
+            byte_arr.append(cur_token & 0xFF)
+            cur_token >>= 8
+            cur_bits -= 8
+    if cur_bits:
+        byte_arr.append(cur_token)
+    return bytes(byte_arr), total_len
 
 
 def _bytes_to_arr(data: bytes, seq_len: int, num_tokens: int, offset: int = 0) -> list[int]:
+    assert 0 <= offset < 8
     num_bits = (num_tokens - 1).bit_length()
     arr: list[int] = []
-    cur_token = ""
+    cur_token = 0
+    cur_bits = 0
+    mask = (1 << num_bits) - 1
     for byte in data:
-        cur_token += f"{byte:08b}"
+        cur_token += byte << cur_bits
+        cur_bits += 8
         if offset != 0:
-            cur_token = cur_token[offset:]
+            cur_token >>= offset
+            cur_bits -= offset
             offset = 0
-        while len(cur_token) >= num_bits:
-            arr.append(int(cur_token[:num_bits], 2))
+        while cur_bits >= num_bits:
+            arr.append(cur_token & mask)
             if len(arr) == seq_len:
                 return arr
-            cur_token = cur_token[num_bits:]
+            cur_token >>= num_bits
+            cur_bits -= num_bits
     raise ValueError("Not enough bytes to fill sequence")
 
 
 class TokenWriter(ContextManager):
     """Helper class for writing a dataset of tokens to a file.
 
     This class can be used in conjunction with :class:`TokenReader` to write
@@ -152,22 +168,22 @@
         return self
 
     def __exit__(self, _t: type[BaseException] | None, _e: BaseException | None, _tr: TracebackType | None) -> None:
         assert self._fp is not None
 
         self._fp.close()
 
-    def write(self, tokens: Sequence[int]) -> None:
+    def write(self, tokens: Iterable[int]) -> None:
         assert self._fp is not None, "TokenWriter must be opened with a context manager"
 
         # Converts the tokens to a binary array.
-        byte_data = _arr_to_bytes(tokens, self._num_tokens)
+        byte_data, num_tokens = _arr_to_bytes(tokens, self._num_tokens)
 
         # Writes the binary data
-        self._fp.write(struct.pack(self._lengths_fmt, len(tokens)))
+        self._fp.write(struct.pack(self._lengths_fmt, num_tokens))
         self._fp.write(byte_data)
 
     def flush(self) -> None:
         assert self._fp is not None, "TokenWriter must be opened with a context manager"
 
         self._fp.flush()
```

### Comparing `ml-starter-0.1.41/ml/utils/torch_distributed.py` & `ml-starter-0.1.42/ml/utils/torch_distributed.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import os
 import sys
 import traceback
 from dataclasses import dataclass
 from typing import Callable
 
 import torch
+import torch.distributed
 import torch.distributed as dist
 import torch.multiprocessing as mp
 from omegaconf import MISSING
 
 from ml.core.config import conf_field
 from ml.utils.checkpoint import is_missing
 from ml.utils.distributed import get_init_method, get_rank, get_world_size, set_dist
```

### Comparing `ml-starter-0.1.41/ml/utils/triton/kmeans.py` & `ml-starter-0.1.42/ml/utils/triton/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/triton/lion.py` & `ml-starter-0.1.42/ml/utils/triton/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml/utils/video.py` & `ml-starter-0.1.42/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.1.42/ml_starter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.41
+Version: 0.1.42
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.41/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.1.42/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/pyproject.toml` & `ml-starter-0.1.42/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.41/setup.py` & `ml-starter-0.1.42/setup.py`

 * *Files identical despite different names*

