# Comparing `tmp/zoobot-1.0.3.tar.gz` & `tmp/zoobot-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoobot-1.0.3.tar", last modified: Thu May  4 12:35:23 2023, max compression
+gzip compressed data, was "zoobot-1.0.4.tar", last modified: Tue Aug  1 07:42:36 2023, max compression
```

## Comparing `zoobot-1.0.3.tar` & `zoobot-1.0.4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.754416 zoobot-1.0.3/
--rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-05-04 12:35:10.000000 zoobot-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12426 2023-05-04 12:35:23.754416 zoobot-1.0.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    11701 2023-05-04 12:35:10.000000 zoobot-1.0.3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-05-04 12:35:10.000000 zoobot-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 12:35:23.754416 zoobot-1.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4072 2023-05-04 12:35:10.000000 zoobot-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.738416 zoobot-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-04 12:35:10.000000 zoobot-1.0.3/tests/test_loss_equivalence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.738416 zoobot-1.0.3/zoobot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.742416 zoobot-1.0.3/zoobot/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.742416 zoobot-1.0.3/zoobot/pytorch/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/estimators/cuda_check.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/estimators/custom_layers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16013 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/estimators/define_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3188 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/estimators/efficientnet_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/manchester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.742416 zoobot-1.0.3/zoobot/pytorch/predictions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/predictions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/predictions/predict_on_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.746416 zoobot-1.0.3/zoobot/pytorch/training/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20318 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/training/finetune.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5860 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/training/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/training/representations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/training/tensorboard_writers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16300 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/pytorch/training/train_with_pytorch_lightning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.746416 zoobot-1.0.3/zoobot/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/shared/benchmark_datasets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4437 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/shared/compress_representations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2071 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/shared/label_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/shared/load_predictions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2844 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/shared/save_predictions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11898 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/shared/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    12964 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/shared/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.750416 zoobot-1.0.3/zoobot/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.750416 zoobot-1.0.3/zoobot/tensorflow/estimators/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/estimators/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2508 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/estimators/alexnet_baseline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1795 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/estimators/custom_callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1370 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/estimators/custom_layers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7227 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/estimators/define_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2300 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/estimators/efficientnet_custom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    84167 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/estimators/efficientnet_standard.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1134 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/estimators/small_cnn_baseline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.750416 zoobot-1.0.3/zoobot/tensorflow/predictions/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/predictions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3417 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/predictions/predict_on_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5239 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/predictions/visualize_dirichlet_predictions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.754416 zoobot-1.0.3/zoobot/tensorflow/stats/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/stats/coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14433 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/stats/dirichlet_stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3526 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/stats/mixture_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.754416 zoobot-1.0.3/zoobot/tensorflow/training/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/training/custom_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/training/finetune.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6772 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/training/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/training/train_with_keras.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6505 2023-05-04 12:35:10.000000 zoobot-1.0.3/zoobot/tensorflow/training/training_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:35:23.738416 zoobot-1.0.3/zoobot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12426 2023-05-04 12:35:23.000000 zoobot-1.0.3/zoobot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-04 12:35:23.000000 zoobot-1.0.3/zoobot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:35:23.000000 zoobot-1.0.3/zoobot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-04 12:35:23.000000 zoobot-1.0.3/zoobot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 12:35:23.000000 zoobot-1.0.3/zoobot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:36.527461 zoobot-1.0.4/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-08-01 07:42:25.000000 zoobot-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-08-01 07:42:36.527461 zoobot-1.0.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12336 2023-08-01 07:42:25.000000 zoobot-1.0.4/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-08-01 07:42:25.000000 zoobot-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 07:42:36.527461 zoobot-1.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4036 2023-08-01 07:42:25.000000 zoobot-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:36.519461 zoobot-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-01 07:42:25.000000 zoobot-1.0.4/tests/test_loss_equivalence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:36.519461 zoobot-1.0.4/zoobot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:36.523461 zoobot-1.0.4/zoobot/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:36.523461 zoobot-1.0.4/zoobot/pytorch/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/pytorch/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/pytorch/estimators/cuda_check.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/pytorch/estimators/custom_layers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16079 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/pytorch/estimators/define_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3188 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/pytorch/estimators/efficientnet_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/pytorch/manchester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:36.523461 zoobot-1.0.4/zoobot/pytorch/predictions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/pytorch/predictions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/pytorch/predictions/predict_on_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:36.523461 zoobot-1.0.4/zoobot/pytorch/training/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/pytorch/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20932 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/pytorch/training/finetune.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5860 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/pytorch/training/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/pytorch/training/representations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/pytorch/training/tensorboard_writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16300 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/pytorch/training/train_with_pytorch_lightning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:36.523461 zoobot-1.0.4/zoobot/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/shared/benchmark_datasets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4437 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/shared/compress_representations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2071 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/shared/label_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/shared/load_predictions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2844 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/shared/save_predictions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12065 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/shared/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12964 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/shared/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:36.523461 zoobot-1.0.4/zoobot/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:36.527461 zoobot-1.0.4/zoobot/tensorflow/estimators/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/estimators/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2508 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/estimators/alexnet_baseline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1795 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/estimators/custom_callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1370 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/estimators/custom_layers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7227 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/estimators/define_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2300 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/estimators/efficientnet_custom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    84167 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/estimators/efficientnet_standard.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1134 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/estimators/small_cnn_baseline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:36.527461 zoobot-1.0.4/zoobot/tensorflow/predictions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/predictions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3417 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/predictions/predict_on_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5239 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/predictions/visualize_dirichlet_predictions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:36.527461 zoobot-1.0.4/zoobot/tensorflow/stats/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/stats/coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14433 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/stats/dirichlet_stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3526 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/stats/mixture_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:36.527461 zoobot-1.0.4/zoobot/tensorflow/training/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/training/custom_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/training/finetune.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6772 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/training/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/training/train_with_keras.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6505 2023-08-01 07:42:25.000000 zoobot-1.0.4/zoobot/tensorflow/training/training_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:42:36.519461 zoobot-1.0.4/zoobot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-08-01 07:42:36.000000 zoobot-1.0.4/zoobot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-08-01 07:42:36.000000 zoobot-1.0.4/zoobot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 07:42:36.000000 zoobot-1.0.4/zoobot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-01 07:42:36.000000 zoobot-1.0.4/zoobot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 07:42:36.000000 zoobot-1.0.4/zoobot.egg-info/top_level.txt
```

### Comparing `zoobot-1.0.3/LICENSE` & `zoobot-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/PKG-INFO` & `zoobot-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoobot
-Version: 1.0.3
+Version: 1.0.4
 Summary: Galaxy morphology classifiers
 Home-page: https://github.com/mwalmsley/zoobot
 Author: Mike Walmsley
 Author-email: walmsleymk1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -25,25 +25,26 @@
 
 [![Downloads](https://pepy.tech/badge/zoobot)](https://pepy.tech/project/zoobot)
 [![Documentation Status](https://readthedocs.org/projects/zoobot/badge/?version=latest)](https://zoobot.readthedocs.io/)
 ![build](https://github.com/mwalmsley/zoobot/actions/workflows/run_CI.yml/badge.svg)
 ![publish](https://github.com/mwalmsley/zoobot/actions/workflows/python-publish.yml/badge.svg)
 [![PyPI](https://badge.fury.io/py/zoobot.svg)](https://badge.fury.io/py/zoobot)
 [![DOI](https://zenodo.org/badge/343787617.svg)](https://zenodo.org/badge/latestdoi/343787617)
+[![status](https://joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f/status.svg)](https://joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f)
 <a href="https://ascl.net/2203.027"><img src="https://img.shields.io/badge/ascl-2203.027-blue.svg?colorB=262255" alt="ascl:2203.027" /></a>
 
 Zoobot classifies galaxy morphology with deep learning.
 <!-- At Galaxy Zoo, we use Zoobot to help our volunteers classify the galaxies in all our recent catalogues: GZ DECaLS, GZ DESI, GZ Rings and GZ Cosmic Dawn. -->
 
 Zoobot is trained using millions of answers by Galaxy Zoo volunteers. This code will let you **retrain** Zoobot to accurately solve your own prediction task.
 
 - [Install](#installation)
 - [Quickstart](#quickstart)
 - [Worked Examples](#worked-examples)
-- [Pretrained Weights](https://zoobot.readthedocs.io/data_notes.html)
+- [Pretrained Weights](https://zoobot.readthedocs.io/en/latest/data_notes.html)
 - [Datasets](https://www.github.com/mwalmsley/galaxy-datasets)
 - [Documentation](https://zoobot.readthedocs.io/) (for understanding/reference)
 
 ## Installation
 <a name="installation"></a>
 
 You can retrain Zoobot in the cloud with a free GPU using this [Google Colab notebook](https://colab.research.google.com/drive/17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing). To install locally, keep reading.
@@ -122,15 +123,15 @@
 ## Getting Started
 <a name="getting_started"></a>
 
 I suggest starting with the [Colab notebook](https://colab.research.google.com/drive/17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) or the worked examples below, which you can copy and adapt.
 
 For context and explanation, see the [documentation](https://zoobot.readthedocs.io/).
 
-For pretrained model weights, precalculated representations, catalogues, and so forth, see the [data notes](https://zoobot.readthedocs.io/data_notes.html) in particular.
+For pretrained model weights, precalculated representations, catalogues, and so forth, see the [data notes](https://zoobot.readthedocs.io/en/latest/data_notes.html) in particular.
 
 ### Worked Examples
 <a name="worked_examples"></a>
 
 PyTorch (recommended):
 - [pytorch/examples/finetuning/finetune_binary_classification.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/finetuning/finetune_binary_classification.py)
 - [pytorch/examples/finetuning/finetune_counts_full_tree.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/finetuning/finetune_counts_full_tree.py)
@@ -141,15 +142,15 @@
 - [tensorflow/examples/train_model_on_catalog.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/tensorflow/examples/train_model_on_catalog.py) (only necessary to train from scratch)
 - [tensorflow/examples/make_predictions.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/tensorflow/examples/make_predictions.py)
 - [tensorflow/examples/finetune_minimal.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/tensorflow/examples/finetune_minimal.py)
 - [tensorflow/examples/finetune_advanced.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/tensorflow/examples/finetune_advanced.py)
 
 There is more explanation and an API reference on the [docs](https://zoobot.readthedocs.io/).
 
-I also [include](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) the scripts used to create and benchmark our pretrained models. Many pretrained models are available [already](https://zoobot.readthedocs.io/data_notes.html), but if you need one trained on e.g. different input image sizes or with a specific architecture, I can probably make it for you.
+I also [include](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) the scripts used to create and benchmark our pretrained models. Many pretrained models are available [already](https://zoobot.readthedocs.io/en/latest/data_notes.html), but if you need one trained on e.g. different input image sizes or with a specific architecture, I can probably make it for you.
 
 When trained with a decision tree head (ZoobotTree, FinetuneableZoobotTree), Zoobot can learn from volunteer labels of varying confidence and predict posteriors for what the typical volunteer might say. Specifically, this Zoobot mode predicts the parameters for distributions, not simple class labels! For a demonstration of how to interpret these predictions, see the [gz_decals_data_release_analysis_demo.ipynb](https://github.com/mwalmsley/zoobot/blob/main/gz_decals_data_release_analysis_demo.ipynb).
 
 
 
 ### (Optional) Install PyTorch or TensorFlow, with CUDA
 <a name="install_cuda"></a>
@@ -167,15 +168,22 @@
 CUDA 11.2 and CUDNN 8.1 for TensorFlow 2.10.0:
 
     conda create --name zoobot38_tf python==3.8
     conda activate zoobot38_tf
     conda install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0
     export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$CONDA_PREFIX/lib/  # add this environment variable
 
-### Latest features (v1.0.0)
+### Latest minor features (v1.0.4)
+
+- Now supports multi-class finetuning. See `pytorch/examples/finetuning/finetune_multiclass_classification.py`
+- Removed `simplejpeg` dependency due to M1 install issue. 
+- Pinned `timm` version to ensure MaX-ViT models load correctly. Models supporting the latest `timm` will follow.
+- (internal until published) GZ Evo v2 now includes Cosmic Dawn (HSC). Significant performance improvement on HSC finetuning.
+
+### Latest major features (v1.0.0)
 
 v1.0.0 recognises that most of the complexity in this repo is training Zoobot from scratch, but most non-GZ users will probably simply want to load the pretrained Zoobot and finetune it on their data.
 
 - Adds new finetuning interface (`finetune.run_finetuning()`), examples.
 - Refocuses docs on finetuning rather than training from scratch.
 - Rework installation process to separate CUDA from Zoobot (simpler, easier)
 - Better wandb logging throughout, to monitor training
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zoobot Version: 1.0.3 Summary: Galaxy morphology
+Metadata-Version: 2.1 Name: zoobot Version: 1.0.4 Summary: Galaxy morphology
 classifiers Home-page: https://github.com/mwalmsley/zoobot Author: Mike
 Walmsley Author-email: walmsleymk1@gmail.com Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: GNU General Public
 License (GPL) Classifier: Operating System :: OS Independent Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: GPU :: NVIDIA CUDA
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 pytorch_cpu Provides-Extra: pytorch_m1 Provides-Extra: pytorch_cu113 Provides-
@@ -10,24 +10,26 @@
 Provides-Extra: docs License-File: LICENSE # Zoobot [![Downloads](https://
 pepy.tech/badge/zoobot)](https://pepy.tech/project/zoobot) [![Documentation
 Status](https://readthedocs.org/projects/zoobot/badge/?version=latest)](https:/
 /zoobot.readthedocs.io/) ![build](https://github.com/mwalmsley/zoobot/actions/
 workflows/run_CI.yml/badge.svg) ![publish](https://github.com/mwalmsley/zoobot/
 actions/workflows/python-publish.yml/badge.svg) [![PyPI](https://badge.fury.io/
 py/zoobot.svg)](https://badge.fury.io/py/zoobot) [![DOI](https://zenodo.org/
-badge/343787617.svg)](https://zenodo.org/badge/latestdoi/343787617) [ascl:
+badge/343787617.svg)](https://zenodo.org/badge/latestdoi/343787617) [![status]
+(https://joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f/status.svg)]
+(https://joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f) [ascl:
 2203.027] Zoobot classifies galaxy morphology with deep learning.  Zoobot is
 trained using millions of answers by Galaxy Zoo volunteers. This code will let
 you **retrain** Zoobot to accurately solve your own prediction task. -
 [Install](#installation) - [Quickstart](#quickstart) - [Worked Examples]
-(#worked-examples) - [Pretrained Weights](https://zoobot.readthedocs.io/
-data_notes.html) - [Datasets](https://www.github.com/mwalmsley/galaxy-datasets)
-- [Documentation](https://zoobot.readthedocs.io/) (for understanding/reference)
-## Installation  You can retrain Zoobot in the cloud with a free GPU using this
-[Google Colab notebook](https://colab.research.google.com/drive/
+(#worked-examples) - [Pretrained Weights](https://zoobot.readthedocs.io/en/
+latest/data_notes.html) - [Datasets](https://www.github.com/mwalmsley/galaxy-
+datasets) - [Documentation](https://zoobot.readthedocs.io/) (for understanding/
+reference) ## Installation  You can retrain Zoobot in the cloud with a free GPU
+using this [Google Colab notebook](https://colab.research.google.com/drive/
 17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing). To install locally, keep
 reading. Download the code using git: git clone git@github.com:mwalmsley/
 zoobot.git And then pick one of the three commands below to install Zoobot and
 either PyTorch (recommended) or TensorFlow: # Zoobot with PyTorch and a GPU.
 Requires CUDA 11.3. pip install -e "zoobot[pytorch_cu113]" --extra-index-url
 https://download.pytorch.org/whl/cu113 # OR Zoobot with PyTorch and no GPU pip
 install -e "zoobot[pytorch_cpu]" --extra-index-url https://
@@ -64,16 +66,16 @@
 many guides and working examples - see the [Getting Started](#getting-started)
 section below. ## Getting Started  I suggest starting with the [Colab notebook]
 (https://colab.research.google.com/drive/
 17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) or the worked examples below,
 which you can copy and adapt. For context and explanation, see the
 [documentation](https://zoobot.readthedocs.io/). For pretrained model weights,
 precalculated representations, catalogues, and so forth, see the [data notes]
-(https://zoobot.readthedocs.io/data_notes.html) in particular. ### Worked
-Examples  PyTorch (recommended): - [pytorch/examples/finetuning/
+(https://zoobot.readthedocs.io/en/latest/data_notes.html) in particular. ###
+Worked Examples  PyTorch (recommended): - [pytorch/examples/finetuning/
 finetune_binary_classification.py](https://github.com/mwalmsley/zoobot/blob/
 main/zoobot/pytorch/examples/finetuning/finetune_binary_classification.py) -
 [pytorch/examples/finetuning/finetune_counts_full_tree.py](https://github.com/
 mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/finetuning/
 finetune_counts_full_tree.py) - [pytorch/examples/representations/
 get_representations.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/
 pytorch/examples/representations/get_representations.py) - [pytorch/examples/
@@ -87,71 +89,77 @@
 examples/finetune_minimal.py](https://github.com/mwalmsley/zoobot/blob/main/
 zoobot/tensorflow/examples/finetune_minimal.py) - [tensorflow/examples/
 finetune_advanced.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/
 tensorflow/examples/finetune_advanced.py) There is more explanation and an API
 reference on the [docs](https://zoobot.readthedocs.io/). I also [include]
 (https://github.com/mwalmsley/zoobot/blob/main/benchmarks) the scripts used to
 create and benchmark our pretrained models. Many pretrained models are
-available [already](https://zoobot.readthedocs.io/data_notes.html), but if you
-need one trained on e.g. different input image sizes or with a specific
-architecture, I can probably make it for you. When trained with a decision tree
-head (ZoobotTree, FinetuneableZoobotTree), Zoobot can learn from volunteer
-labels of varying confidence and predict posteriors for what the typical
-volunteer might say. Specifically, this Zoobot mode predicts the parameters for
-distributions, not simple class labels! For a demonstration of how to interpret
-these predictions, see the [gz_decals_data_release_analysis_demo.ipynb](https:/
-/github.com/mwalmsley/zoobot/blob/main/
-gz_decals_data_release_analysis_demo.ipynb). ### (Optional) Install PyTorch or
-TensorFlow, with CUDA  *If you're not using a GPU, skip this step. Use the
-pytorch_cpu or tensorflow_cpu options in the section below.* Install PyTorch
-1.12.1 or Tensorflow 2.10.0 and compatible CUDA drivers. I highly recommend
-using [conda](https://docs.conda.io/en/latest/miniconda.html) to do this. Conda
-will handle both creating a new virtual environment (`conda create`) and
-installing CUDA (`cudatoolkit`, `cudnn`) CUDA 11.3 for PyTorch: conda create --
-name zoobot38_torch python==3.8 conda activate zoobot38_torch conda install -
-c conda-forge cudatoolkit=11.3 CUDA 11.2 and CUDNN 8.1 for TensorFlow 2.10.0:
-conda create --name zoobot38_tf python==3.8 conda activate zoobot38_tf conda
-install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0 export
+available [already](https://zoobot.readthedocs.io/en/latest/data_notes.html),
+but if you need one trained on e.g. different input image sizes or with a
+specific architecture, I can probably make it for you. When trained with a
+decision tree head (ZoobotTree, FinetuneableZoobotTree), Zoobot can learn from
+volunteer labels of varying confidence and predict posteriors for what the
+typical volunteer might say. Specifically, this Zoobot mode predicts the
+parameters for distributions, not simple class labels! For a demonstration of
+how to interpret these predictions, see the
+[gz_decals_data_release_analysis_demo.ipynb](https://github.com/mwalmsley/
+zoobot/blob/main/gz_decals_data_release_analysis_demo.ipynb). ### (Optional)
+Install PyTorch or TensorFlow, with CUDA  *If you're not using a GPU, skip this
+step. Use the pytorch_cpu or tensorflow_cpu options in the section below.*
+Install PyTorch 1.12.1 or Tensorflow 2.10.0 and compatible CUDA drivers. I
+highly recommend using [conda](https://docs.conda.io/en/latest/miniconda.html)
+to do this. Conda will handle both creating a new virtual environment (`conda
+create`) and installing CUDA (`cudatoolkit`, `cudnn`) CUDA 11.3 for PyTorch:
+conda create --name zoobot38_torch python==3.8 conda activate zoobot38_torch
+conda install -c conda-forge cudatoolkit=11.3 CUDA 11.2 and CUDNN 8.1 for
+TensorFlow 2.10.0: conda create --name zoobot38_tf python==3.8 conda activate
+zoobot38_tf conda install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0 export
 LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$CONDA_PREFIX/lib/ # add this environment
-variable ### Latest features (v1.0.0) v1.0.0 recognises that most of the
-complexity in this repo is training Zoobot from scratch, but most non-GZ users
-will probably simply want to load the pretrained Zoobot and finetune it on
-their data. - Adds new finetuning interface (`finetune.run_finetuning()`),
-examples. - Refocuses docs on finetuning rather than training from scratch. -
-Rework installation process to separate CUDA from Zoobot (simpler, easier) -
-Better wandb logging throughout, to monitor training - Remove need to make
-TFRecords. Now TF directly uses images. - Refactor out augmentations and
-datasets to `galaxy-datasets` repo. TF and Torch now use identical
-augmentations (via albumentations). - Many small quality-of-life improvements
-Contributions are very welcome and will be credited in any future work. Please
-get in touch! See [CONTRIBUTING.md](https://github.com/mwalmsley/zoobot/blob/
-main/benchmarks) for more. ### Benchmarks and Replication - Training from
-Scratch The [benchmarks](https://github.com/mwalmsley/zoobot/blob/main/
-benchmarks) folder contains slurm and Python scripts to train Zoobot from
-scratch. We use these scripts to make sure new code versions work well, and
-that TensorFlow and PyTorch achieve similar performance. Training Zoobot using
-the GZ DECaLS dataset option will create models very similar to those used for
-the GZ DECaLS catalogue and shared with the early versions of this repo. The GZ
-DESI Zoobot model is trained on additional data (GZD-1, GZD-2), as the GZ Evo
-Zoobot model (GZD-1/2/5, Hubble, Candels, GZ2). ### Citing We have submitted a
-JOSS paper to describe Zoobot itself. We hope this will become the single
-point-of-reference for Zoobot. Meanwhile, please cite the [Galaxy Zoo DECaLS]
-(https://arxiv.org/abs/2102.08414), which uses the code that evolved into
-Zoobot: @article{Walmsley2022decals, author = {Mike Walmsley and Chris Lintott
-and Geron Tobias and Sandor J Kruk and Coleman Krawczyk and Kyle Willett and
-Steven Bamford and William Keel and Lee S Kelvin and Lucy Fortson and Karen
-Masters and Vihang Mehta and Brooke Simmons and Rebecca J Smethurst and
-Elisabeth M L Baeten and Christine Macmillan}, issue = {3}, journal = {Monthly
-Notices of the Royal Astronomical Society}, month = {12}, pages = {3966-3988},
-title = {Galaxy Zoo DECaLS: Detailed Visual Morphology Measurements from
-Volunteers and Deep Learning for 314,000 Galaxies}, volume = {509}, url =
-{https://arxiv.org/abs/2102.08414}, year = {2022}, } You might be interested in
-reading papers using Zoobot: - [Galaxy Zoo DECaLS](https://arxiv.org/abs/
-2102.08414) (first use at Galaxy Zoo) - [A Comparison of Deep Learning
-Architectures for Optical Galaxy Morphology Classification](https://arxiv.org/
-abs/2111.04353) - [Practical Galaxy Morphology Tools from Deep Supervised
-Representation Learning](https://arxiv.org/abs/2110.12735) - [Towards
-Foundation Models for Galaxy Morphology](https://arxiv.org/abs/2206.11927)
-(adding contrastive learning) - [Harnessing the Hubble Space Telescope
-Archives: A Catalogue of 21,926 Interacting Galaxies](https://arxiv.org/abs/
-2303.00366) Many other works use Zoobot indirectly via the [Galaxy Zoo DECaLS]
-(https://arxiv.org/abs/2102.08414) catalog.
+variable ### Latest minor features (v1.0.4) - Now supports multi-class
+finetuning. See `pytorch/examples/finetuning/
+finetune_multiclass_classification.py` - Removed `simplejpeg` dependency due to
+M1 install issue. - Pinned `timm` version to ensure MaX-ViT models load
+correctly. Models supporting the latest `timm` will follow. - (internal until
+published) GZ Evo v2 now includes Cosmic Dawn (HSC). Significant performance
+improvement on HSC finetuning. ### Latest major features (v1.0.0) v1.0.0
+recognises that most of the complexity in this repo is training Zoobot from
+scratch, but most non-GZ users will probably simply want to load the pretrained
+Zoobot and finetune it on their data. - Adds new finetuning interface
+(`finetune.run_finetuning()`), examples. - Refocuses docs on finetuning rather
+than training from scratch. - Rework installation process to separate CUDA from
+Zoobot (simpler, easier) - Better wandb logging throughout, to monitor training
+- Remove need to make TFRecords. Now TF directly uses images. - Refactor out
+augmentations and datasets to `galaxy-datasets` repo. TF and Torch now use
+identical augmentations (via albumentations). - Many small quality-of-life
+improvements Contributions are very welcome and will be credited in any future
+work. Please get in touch! See [CONTRIBUTING.md](https://github.com/mwalmsley/
+zoobot/blob/main/benchmarks) for more. ### Benchmarks and Replication -
+Training from Scratch The [benchmarks](https://github.com/mwalmsley/zoobot/
+blob/main/benchmarks) folder contains slurm and Python scripts to train Zoobot
+from scratch. We use these scripts to make sure new code versions work well,
+and that TensorFlow and PyTorch achieve similar performance. Training Zoobot
+using the GZ DECaLS dataset option will create models very similar to those
+used for the GZ DECaLS catalogue and shared with the early versions of this
+repo. The GZ DESI Zoobot model is trained on additional data (GZD-1, GZD-2), as
+the GZ Evo Zoobot model (GZD-1/2/5, Hubble, Candels, GZ2). ### Citing We have
+submitted a JOSS paper to describe Zoobot itself. We hope this will become the
+single point-of-reference for Zoobot. Meanwhile, please cite the [Galaxy Zoo
+DECaLS](https://arxiv.org/abs/2102.08414), which uses the code that evolved
+into Zoobot: @article{Walmsley2022decals, author = {Mike Walmsley and Chris
+Lintott and Geron Tobias and Sandor J Kruk and Coleman Krawczyk and Kyle
+Willett and Steven Bamford and William Keel and Lee S Kelvin and Lucy Fortson
+and Karen Masters and Vihang Mehta and Brooke Simmons and Rebecca J Smethurst
+and Elisabeth M L Baeten and Christine Macmillan}, issue = {3}, journal =
+{Monthly Notices of the Royal Astronomical Society}, month = {12}, pages =
+{3966-3988}, title = {Galaxy Zoo DECaLS: Detailed Visual Morphology
+Measurements from Volunteers and Deep Learning for 314,000 Galaxies}, volume =
+{509}, url = {https://arxiv.org/abs/2102.08414}, year = {2022}, } You might be
+interested in reading papers using Zoobot: - [Galaxy Zoo DECaLS](https://
+arxiv.org/abs/2102.08414) (first use at Galaxy Zoo) - [A Comparison of Deep
+Learning Architectures for Optical Galaxy Morphology Classification](https://
+arxiv.org/abs/2111.04353) - [Practical Galaxy Morphology Tools from Deep
+Supervised Representation Learning](https://arxiv.org/abs/2110.12735) -
+[Towards Foundation Models for Galaxy Morphology](https://arxiv.org/abs/
+2206.11927) (adding contrastive learning) - [Harnessing the Hubble Space
+Telescope Archives: A Catalogue of 21,926 Interacting Galaxies](https://
+arxiv.org/abs/2303.00366) Many other works use Zoobot indirectly via the
+[Galaxy Zoo DECaLS](https://arxiv.org/abs/2102.08414) catalog.
```

### Comparing `zoobot-1.0.3/README.md` & `zoobot-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 [![Downloads](https://pepy.tech/badge/zoobot)](https://pepy.tech/project/zoobot)
 [![Documentation Status](https://readthedocs.org/projects/zoobot/badge/?version=latest)](https://zoobot.readthedocs.io/)
 ![build](https://github.com/mwalmsley/zoobot/actions/workflows/run_CI.yml/badge.svg)
 ![publish](https://github.com/mwalmsley/zoobot/actions/workflows/python-publish.yml/badge.svg)
 [![PyPI](https://badge.fury.io/py/zoobot.svg)](https://badge.fury.io/py/zoobot)
 [![DOI](https://zenodo.org/badge/343787617.svg)](https://zenodo.org/badge/latestdoi/343787617)
+[![status](https://joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f/status.svg)](https://joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f)
 <a href="https://ascl.net/2203.027"><img src="https://img.shields.io/badge/ascl-2203.027-blue.svg?colorB=262255" alt="ascl:2203.027" /></a>
 
 Zoobot classifies galaxy morphology with deep learning.
 <!-- At Galaxy Zoo, we use Zoobot to help our volunteers classify the galaxies in all our recent catalogues: GZ DECaLS, GZ DESI, GZ Rings and GZ Cosmic Dawn. -->
 
 Zoobot is trained using millions of answers by Galaxy Zoo volunteers. This code will let you **retrain** Zoobot to accurately solve your own prediction task.
 
 - [Install](#installation)
 - [Quickstart](#quickstart)
 - [Worked Examples](#worked-examples)
-- [Pretrained Weights](https://zoobot.readthedocs.io/data_notes.html)
+- [Pretrained Weights](https://zoobot.readthedocs.io/en/latest/data_notes.html)
 - [Datasets](https://www.github.com/mwalmsley/galaxy-datasets)
 - [Documentation](https://zoobot.readthedocs.io/) (for understanding/reference)
 
 ## Installation
 <a name="installation"></a>
 
 You can retrain Zoobot in the cloud with a free GPU using this [Google Colab notebook](https://colab.research.google.com/drive/17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing). To install locally, keep reading.
@@ -99,15 +100,15 @@
 ## Getting Started
 <a name="getting_started"></a>
 
 I suggest starting with the [Colab notebook](https://colab.research.google.com/drive/17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) or the worked examples below, which you can copy and adapt.
 
 For context and explanation, see the [documentation](https://zoobot.readthedocs.io/).
 
-For pretrained model weights, precalculated representations, catalogues, and so forth, see the [data notes](https://zoobot.readthedocs.io/data_notes.html) in particular.
+For pretrained model weights, precalculated representations, catalogues, and so forth, see the [data notes](https://zoobot.readthedocs.io/en/latest/data_notes.html) in particular.
 
 ### Worked Examples
 <a name="worked_examples"></a>
 
 PyTorch (recommended):
 - [pytorch/examples/finetuning/finetune_binary_classification.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/finetuning/finetune_binary_classification.py)
 - [pytorch/examples/finetuning/finetune_counts_full_tree.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/finetuning/finetune_counts_full_tree.py)
@@ -118,15 +119,15 @@
 - [tensorflow/examples/train_model_on_catalog.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/tensorflow/examples/train_model_on_catalog.py) (only necessary to train from scratch)
 - [tensorflow/examples/make_predictions.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/tensorflow/examples/make_predictions.py)
 - [tensorflow/examples/finetune_minimal.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/tensorflow/examples/finetune_minimal.py)
 - [tensorflow/examples/finetune_advanced.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/tensorflow/examples/finetune_advanced.py)
 
 There is more explanation and an API reference on the [docs](https://zoobot.readthedocs.io/).
 
-I also [include](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) the scripts used to create and benchmark our pretrained models. Many pretrained models are available [already](https://zoobot.readthedocs.io/data_notes.html), but if you need one trained on e.g. different input image sizes or with a specific architecture, I can probably make it for you.
+I also [include](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) the scripts used to create and benchmark our pretrained models. Many pretrained models are available [already](https://zoobot.readthedocs.io/en/latest/data_notes.html), but if you need one trained on e.g. different input image sizes or with a specific architecture, I can probably make it for you.
 
 When trained with a decision tree head (ZoobotTree, FinetuneableZoobotTree), Zoobot can learn from volunteer labels of varying confidence and predict posteriors for what the typical volunteer might say. Specifically, this Zoobot mode predicts the parameters for distributions, not simple class labels! For a demonstration of how to interpret these predictions, see the [gz_decals_data_release_analysis_demo.ipynb](https://github.com/mwalmsley/zoobot/blob/main/gz_decals_data_release_analysis_demo.ipynb).
 
 
 
 ### (Optional) Install PyTorch or TensorFlow, with CUDA
 <a name="install_cuda"></a>
@@ -144,15 +145,22 @@
 CUDA 11.2 and CUDNN 8.1 for TensorFlow 2.10.0:
 
     conda create --name zoobot38_tf python==3.8
     conda activate zoobot38_tf
     conda install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0
     export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$CONDA_PREFIX/lib/  # add this environment variable
 
-### Latest features (v1.0.0)
+### Latest minor features (v1.0.4)
+
+- Now supports multi-class finetuning. See `pytorch/examples/finetuning/finetune_multiclass_classification.py`
+- Removed `simplejpeg` dependency due to M1 install issue. 
+- Pinned `timm` version to ensure MaX-ViT models load correctly. Models supporting the latest `timm` will follow.
+- (internal until published) GZ Evo v2 now includes Cosmic Dawn (HSC). Significant performance improvement on HSC finetuning.
+
+### Latest major features (v1.0.0)
 
 v1.0.0 recognises that most of the complexity in this repo is training Zoobot from scratch, but most non-GZ users will probably simply want to load the pretrained Zoobot and finetune it on their data.
 
 - Adds new finetuning interface (`finetune.run_finetuning()`), examples.
 - Refocuses docs on finetuning rather than training from scratch.
 - Rework installation process to separate CUDA from Zoobot (simpler, easier)
 - Better wandb logging throughout, to monitor training
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
 # Zoobot [![Downloads](https://pepy.tech/badge/zoobot)](https://pepy.tech/
 project/zoobot) [![Documentation Status](https://readthedocs.org/projects/
 zoobot/badge/?version=latest)](https://zoobot.readthedocs.io/) ![build](https:/
 /github.com/mwalmsley/zoobot/actions/workflows/run_CI.yml/badge.svg) ![publish]
 (https://github.com/mwalmsley/zoobot/actions/workflows/python-publish.yml/
 badge.svg) [![PyPI](https://badge.fury.io/py/zoobot.svg)](https://
 badge.fury.io/py/zoobot) [![DOI](https://zenodo.org/badge/343787617.svg)]
-(https://zenodo.org/badge/latestdoi/343787617) [ascl:2203.027] Zoobot
+(https://zenodo.org/badge/latestdoi/343787617) [![status](https://
+joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f/status.svg)](https://
+joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f) [ascl:2203.027] Zoobot
 classifies galaxy morphology with deep learning.  Zoobot is trained using
 millions of answers by Galaxy Zoo volunteers. This code will let you
 **retrain** Zoobot to accurately solve your own prediction task. - [Install]
 (#installation) - [Quickstart](#quickstart) - [Worked Examples](#worked-
-examples) - [Pretrained Weights](https://zoobot.readthedocs.io/data_notes.html)
-- [Datasets](https://www.github.com/mwalmsley/galaxy-datasets) -
-[Documentation](https://zoobot.readthedocs.io/) (for understanding/reference)
+examples) - [Pretrained Weights](https://zoobot.readthedocs.io/en/latest/
+data_notes.html) - [Datasets](https://www.github.com/mwalmsley/galaxy-datasets)
+- [Documentation](https://zoobot.readthedocs.io/) (for understanding/reference)
 ## Installation  You can retrain Zoobot in the cloud with a free GPU using this
 [Google Colab notebook](https://colab.research.google.com/drive/
 17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing). To install locally, keep
 reading. Download the code using git: git clone git@github.com:mwalmsley/
 zoobot.git And then pick one of the three commands below to install Zoobot and
 either PyTorch (recommended) or TensorFlow: # Zoobot with PyTorch and a GPU.
 Requires CUDA 11.3. pip install -e "zoobot[pytorch_cu113]" --extra-index-url
@@ -55,16 +57,16 @@
 many guides and working examples - see the [Getting Started](#getting-started)
 section below. ## Getting Started  I suggest starting with the [Colab notebook]
 (https://colab.research.google.com/drive/
 17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) or the worked examples below,
 which you can copy and adapt. For context and explanation, see the
 [documentation](https://zoobot.readthedocs.io/). For pretrained model weights,
 precalculated representations, catalogues, and so forth, see the [data notes]
-(https://zoobot.readthedocs.io/data_notes.html) in particular. ### Worked
-Examples  PyTorch (recommended): - [pytorch/examples/finetuning/
+(https://zoobot.readthedocs.io/en/latest/data_notes.html) in particular. ###
+Worked Examples  PyTorch (recommended): - [pytorch/examples/finetuning/
 finetune_binary_classification.py](https://github.com/mwalmsley/zoobot/blob/
 main/zoobot/pytorch/examples/finetuning/finetune_binary_classification.py) -
 [pytorch/examples/finetuning/finetune_counts_full_tree.py](https://github.com/
 mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/finetuning/
 finetune_counts_full_tree.py) - [pytorch/examples/representations/
 get_representations.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/
 pytorch/examples/representations/get_representations.py) - [pytorch/examples/
@@ -78,71 +80,77 @@
 examples/finetune_minimal.py](https://github.com/mwalmsley/zoobot/blob/main/
 zoobot/tensorflow/examples/finetune_minimal.py) - [tensorflow/examples/
 finetune_advanced.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/
 tensorflow/examples/finetune_advanced.py) There is more explanation and an API
 reference on the [docs](https://zoobot.readthedocs.io/). I also [include]
 (https://github.com/mwalmsley/zoobot/blob/main/benchmarks) the scripts used to
 create and benchmark our pretrained models. Many pretrained models are
-available [already](https://zoobot.readthedocs.io/data_notes.html), but if you
-need one trained on e.g. different input image sizes or with a specific
-architecture, I can probably make it for you. When trained with a decision tree
-head (ZoobotTree, FinetuneableZoobotTree), Zoobot can learn from volunteer
-labels of varying confidence and predict posteriors for what the typical
-volunteer might say. Specifically, this Zoobot mode predicts the parameters for
-distributions, not simple class labels! For a demonstration of how to interpret
-these predictions, see the [gz_decals_data_release_analysis_demo.ipynb](https:/
-/github.com/mwalmsley/zoobot/blob/main/
-gz_decals_data_release_analysis_demo.ipynb). ### (Optional) Install PyTorch or
-TensorFlow, with CUDA  *If you're not using a GPU, skip this step. Use the
-pytorch_cpu or tensorflow_cpu options in the section below.* Install PyTorch
-1.12.1 or Tensorflow 2.10.0 and compatible CUDA drivers. I highly recommend
-using [conda](https://docs.conda.io/en/latest/miniconda.html) to do this. Conda
-will handle both creating a new virtual environment (`conda create`) and
-installing CUDA (`cudatoolkit`, `cudnn`) CUDA 11.3 for PyTorch: conda create --
-name zoobot38_torch python==3.8 conda activate zoobot38_torch conda install -
-c conda-forge cudatoolkit=11.3 CUDA 11.2 and CUDNN 8.1 for TensorFlow 2.10.0:
-conda create --name zoobot38_tf python==3.8 conda activate zoobot38_tf conda
-install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0 export
+available [already](https://zoobot.readthedocs.io/en/latest/data_notes.html),
+but if you need one trained on e.g. different input image sizes or with a
+specific architecture, I can probably make it for you. When trained with a
+decision tree head (ZoobotTree, FinetuneableZoobotTree), Zoobot can learn from
+volunteer labels of varying confidence and predict posteriors for what the
+typical volunteer might say. Specifically, this Zoobot mode predicts the
+parameters for distributions, not simple class labels! For a demonstration of
+how to interpret these predictions, see the
+[gz_decals_data_release_analysis_demo.ipynb](https://github.com/mwalmsley/
+zoobot/blob/main/gz_decals_data_release_analysis_demo.ipynb). ### (Optional)
+Install PyTorch or TensorFlow, with CUDA  *If you're not using a GPU, skip this
+step. Use the pytorch_cpu or tensorflow_cpu options in the section below.*
+Install PyTorch 1.12.1 or Tensorflow 2.10.0 and compatible CUDA drivers. I
+highly recommend using [conda](https://docs.conda.io/en/latest/miniconda.html)
+to do this. Conda will handle both creating a new virtual environment (`conda
+create`) and installing CUDA (`cudatoolkit`, `cudnn`) CUDA 11.3 for PyTorch:
+conda create --name zoobot38_torch python==3.8 conda activate zoobot38_torch
+conda install -c conda-forge cudatoolkit=11.3 CUDA 11.2 and CUDNN 8.1 for
+TensorFlow 2.10.0: conda create --name zoobot38_tf python==3.8 conda activate
+zoobot38_tf conda install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0 export
 LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$CONDA_PREFIX/lib/ # add this environment
-variable ### Latest features (v1.0.0) v1.0.0 recognises that most of the
-complexity in this repo is training Zoobot from scratch, but most non-GZ users
-will probably simply want to load the pretrained Zoobot and finetune it on
-their data. - Adds new finetuning interface (`finetune.run_finetuning()`),
-examples. - Refocuses docs on finetuning rather than training from scratch. -
-Rework installation process to separate CUDA from Zoobot (simpler, easier) -
-Better wandb logging throughout, to monitor training - Remove need to make
-TFRecords. Now TF directly uses images. - Refactor out augmentations and
-datasets to `galaxy-datasets` repo. TF and Torch now use identical
-augmentations (via albumentations). - Many small quality-of-life improvements
-Contributions are very welcome and will be credited in any future work. Please
-get in touch! See [CONTRIBUTING.md](https://github.com/mwalmsley/zoobot/blob/
-main/benchmarks) for more. ### Benchmarks and Replication - Training from
-Scratch The [benchmarks](https://github.com/mwalmsley/zoobot/blob/main/
-benchmarks) folder contains slurm and Python scripts to train Zoobot from
-scratch. We use these scripts to make sure new code versions work well, and
-that TensorFlow and PyTorch achieve similar performance. Training Zoobot using
-the GZ DECaLS dataset option will create models very similar to those used for
-the GZ DECaLS catalogue and shared with the early versions of this repo. The GZ
-DESI Zoobot model is trained on additional data (GZD-1, GZD-2), as the GZ Evo
-Zoobot model (GZD-1/2/5, Hubble, Candels, GZ2). ### Citing We have submitted a
-JOSS paper to describe Zoobot itself. We hope this will become the single
-point-of-reference for Zoobot. Meanwhile, please cite the [Galaxy Zoo DECaLS]
-(https://arxiv.org/abs/2102.08414), which uses the code that evolved into
-Zoobot: @article{Walmsley2022decals, author = {Mike Walmsley and Chris Lintott
-and Geron Tobias and Sandor J Kruk and Coleman Krawczyk and Kyle Willett and
-Steven Bamford and William Keel and Lee S Kelvin and Lucy Fortson and Karen
-Masters and Vihang Mehta and Brooke Simmons and Rebecca J Smethurst and
-Elisabeth M L Baeten and Christine Macmillan}, issue = {3}, journal = {Monthly
-Notices of the Royal Astronomical Society}, month = {12}, pages = {3966-3988},
-title = {Galaxy Zoo DECaLS: Detailed Visual Morphology Measurements from
-Volunteers and Deep Learning for 314,000 Galaxies}, volume = {509}, url =
-{https://arxiv.org/abs/2102.08414}, year = {2022}, } You might be interested in
-reading papers using Zoobot: - [Galaxy Zoo DECaLS](https://arxiv.org/abs/
-2102.08414) (first use at Galaxy Zoo) - [A Comparison of Deep Learning
-Architectures for Optical Galaxy Morphology Classification](https://arxiv.org/
-abs/2111.04353) - [Practical Galaxy Morphology Tools from Deep Supervised
-Representation Learning](https://arxiv.org/abs/2110.12735) - [Towards
-Foundation Models for Galaxy Morphology](https://arxiv.org/abs/2206.11927)
-(adding contrastive learning) - [Harnessing the Hubble Space Telescope
-Archives: A Catalogue of 21,926 Interacting Galaxies](https://arxiv.org/abs/
-2303.00366) Many other works use Zoobot indirectly via the [Galaxy Zoo DECaLS]
-(https://arxiv.org/abs/2102.08414) catalog.
+variable ### Latest minor features (v1.0.4) - Now supports multi-class
+finetuning. See `pytorch/examples/finetuning/
+finetune_multiclass_classification.py` - Removed `simplejpeg` dependency due to
+M1 install issue. - Pinned `timm` version to ensure MaX-ViT models load
+correctly. Models supporting the latest `timm` will follow. - (internal until
+published) GZ Evo v2 now includes Cosmic Dawn (HSC). Significant performance
+improvement on HSC finetuning. ### Latest major features (v1.0.0) v1.0.0
+recognises that most of the complexity in this repo is training Zoobot from
+scratch, but most non-GZ users will probably simply want to load the pretrained
+Zoobot and finetune it on their data. - Adds new finetuning interface
+(`finetune.run_finetuning()`), examples. - Refocuses docs on finetuning rather
+than training from scratch. - Rework installation process to separate CUDA from
+Zoobot (simpler, easier) - Better wandb logging throughout, to monitor training
+- Remove need to make TFRecords. Now TF directly uses images. - Refactor out
+augmentations and datasets to `galaxy-datasets` repo. TF and Torch now use
+identical augmentations (via albumentations). - Many small quality-of-life
+improvements Contributions are very welcome and will be credited in any future
+work. Please get in touch! See [CONTRIBUTING.md](https://github.com/mwalmsley/
+zoobot/blob/main/benchmarks) for more. ### Benchmarks and Replication -
+Training from Scratch The [benchmarks](https://github.com/mwalmsley/zoobot/
+blob/main/benchmarks) folder contains slurm and Python scripts to train Zoobot
+from scratch. We use these scripts to make sure new code versions work well,
+and that TensorFlow and PyTorch achieve similar performance. Training Zoobot
+using the GZ DECaLS dataset option will create models very similar to those
+used for the GZ DECaLS catalogue and shared with the early versions of this
+repo. The GZ DESI Zoobot model is trained on additional data (GZD-1, GZD-2), as
+the GZ Evo Zoobot model (GZD-1/2/5, Hubble, Candels, GZ2). ### Citing We have
+submitted a JOSS paper to describe Zoobot itself. We hope this will become the
+single point-of-reference for Zoobot. Meanwhile, please cite the [Galaxy Zoo
+DECaLS](https://arxiv.org/abs/2102.08414), which uses the code that evolved
+into Zoobot: @article{Walmsley2022decals, author = {Mike Walmsley and Chris
+Lintott and Geron Tobias and Sandor J Kruk and Coleman Krawczyk and Kyle
+Willett and Steven Bamford and William Keel and Lee S Kelvin and Lucy Fortson
+and Karen Masters and Vihang Mehta and Brooke Simmons and Rebecca J Smethurst
+and Elisabeth M L Baeten and Christine Macmillan}, issue = {3}, journal =
+{Monthly Notices of the Royal Astronomical Society}, month = {12}, pages =
+{3966-3988}, title = {Galaxy Zoo DECaLS: Detailed Visual Morphology
+Measurements from Volunteers and Deep Learning for 314,000 Galaxies}, volume =
+{509}, url = {https://arxiv.org/abs/2102.08414}, year = {2022}, } You might be
+interested in reading papers using Zoobot: - [Galaxy Zoo DECaLS](https://
+arxiv.org/abs/2102.08414) (first use at Galaxy Zoo) - [A Comparison of Deep
+Learning Architectures for Optical Galaxy Morphology Classification](https://
+arxiv.org/abs/2111.04353) - [Practical Galaxy Morphology Tools from Deep
+Supervised Representation Learning](https://arxiv.org/abs/2110.12735) -
+[Towards Foundation Models for Galaxy Morphology](https://arxiv.org/abs/
+2206.11927) (adding contrastive learning) - [Harnessing the Hubble Space
+Telescope Archives: A Catalogue of 21,926 Interacting Galaxies](https://
+arxiv.org/abs/2303.00366) Many other works use Zoobot indirectly via the
+[Galaxy Zoo DECaLS](https://arxiv.org/abs/2102.08414) catalog.
```

### Comparing `zoobot-1.0.3/setup.py` & `zoobot-1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="zoobot",
-    version="1.0.3",
+    version="1.0.4",
     author="Mike Walmsley",
     author_email="walmsleymk1@gmail.com",
     description="Galaxy morphology classifiers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mwalmsley/zoobot",
     classifiers=[
@@ -25,54 +25,51 @@
         'pytorch_cpu': [
             # A100 GPU currently only seems to support cuda 11.3 on manchester cluster, let's stick with this version for now
             # very latest version wants cuda 11.6
             'torch == 1.12.1+cpu',
             'torchvision == 0.13.1+cpu',
             'torchaudio == 0.12.1',
             'pytorch-lightning >= 2.0.0',
-            'simplejpeg',
+            # 'simplejpeg',
             'albumentations',
             'pyro-ppl == 1.8.0',
             'torchmetrics == 0.11.0',
-            'timm'
+            'timm == 0.6.12'
         ],
         'pytorch_m1': [
             # as above but without the +cpu (and the extra-index-url in readme has no effect)
             # all matching pytorch versions for an m1 system will be cpu
             'torch == 1.12.1',
             'torchvision == 0.13.1',
             'torchaudio == 0.12.1',
             'pytorch-lightning >= 2.0.0',
-            'simplejpeg',
             'albumentations',
             'pyro-ppl == 1.8.0',
             'torchmetrics == 0.11.0',
-            'timm'
+            'timm == 0.6.12'
         ],
         # as above but without pytorch itself
         # for GPU, you will also need e.g. cudatoolkit=11.3, 11.6
         # https://pytorch.org/get-started/previous-versions/#v1121
         'pytorch_cu113': [
             'torch == 1.12.1+cu113',
             'torchvision == 0.13.1+cu113',
             'torchaudio == 0.12.1',
             'pytorch-lightning >= 2.0.0',
-            'simplejpeg',
             'albumentations',
             'pyro-ppl == 1.8.0',
             'torchmetrics == 0.11.0',
-            'timm'
+            'timm == 0.6.12'
         ],
         'pytorch_colab': [
             'pytorch-lightning >= 2.0.0',
-            'simplejpeg',
             'albumentations',
             'pyro-ppl>=1.8.0',
             'torchmetrics==0.11.0',
-            'timm'
+            'timm == 0.6.12'
         ],
         'tensorflow': [
             'tensorflow == 2.10.0',  # 2.11.0 turns on XLA somewhere which then fails on multi-GPU...TODO
             'keras_applications',
             'tensorflow_probability == 0.18.0',  # 0.19 requires tf 2.11
             'protobuf <= 3.19'  # tensorflow incompatible above this (usually resolved by pip automatically)
         ],
@@ -101,10 +98,10 @@
         'scikit-image >= 0.19.2',
         'scikit-learn >= 1.0.2',
         'matplotlib',
         'pyarrow',  # to read parquet, which is very handy for big datasets
         # for saving metrics to weights&biases (cloud service, free within limits)
         'wandb',
         'setuptools==59.5.0',  # wandb logger incompatibility
-        'galaxy-datasets==0.0.12'  # for dataset loading in both TF and Torch (renamed from pytorch-galaxy-datasets)
+        'galaxy-datasets==0.0.14'  # for dataset loading in both TF and Torch (renamed from pytorch-galaxy-datasets)
     ]
 )
```

### Comparing `zoobot-1.0.3/tests/test_loss_equivalence.py` & `zoobot-1.0.4/tests/test_loss_equivalence.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/pytorch/estimators/custom_layers.py` & `zoobot-1.0.4/zoobot/pytorch/estimators/custom_layers.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/pytorch/estimators/define_model.py` & `zoobot-1.0.4/zoobot/pytorch/estimators/define_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,16 @@
             channels,
             use_imagenet_weights=use_imagenet_weights,
             **timm_kwargs
         )
         # bit lazy assuming 224 input size
         self.encoder_dim = get_encoder_dim(self.encoder, input_size=224, channels=channels)
         # typically encoder_dim=1280 for effnetb0
+        logging.info('encoder dim: {}'.format(self.encoder_dim))
+
 
         self.head = get_pytorch_dirichlet_head(
             self.encoder_dim,
             output_dim=output_dim,
             test_time_dropout=test_time_dropout,
             dropout_rate=dropout_rate
         )
```

### Comparing `zoobot-1.0.3/zoobot/pytorch/estimators/efficientnet_custom.py` & `zoobot-1.0.4/zoobot/pytorch/estimators/efficientnet_custom.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/pytorch/manchester.py` & `zoobot-1.0.4/zoobot/pytorch/manchester.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/pytorch/predictions/predict_on_catalog.py` & `zoobot-1.0.4/zoobot/pytorch/predictions/predict_on_catalog.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/pytorch/training/finetune.py` & `zoobot-1.0.4/zoobot/pytorch/training/finetune.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,28 +117,30 @@
         self.prog_bar = prog_bar
         self.visualize_images = visualize_images
 
     def configure_optimizers(self):
 
         if self.freeze:
             params = self.head.parameters()
-            return torch.optim.AdamW(params, lr=self.learning_rate)
+            return torch.optim.AdamW(params, betas=(0.9, 0.999), lr=self.learning_rate)
         else:
             lr = self.learning_rate
             params = [{"params": self.head.parameters(), "lr": lr}]
 
             # this bit is specific to Zoobot EffNet
+            # TODO check these are blocks not individual layers
             encoder_blocks = list(self.encoder.children())
 
             # for n, l in enumerate(encoder_blocks):
             #     print('\n')
             #     print(n)
             #     print(l)
             
             # layers with no parameters don't count
+            # TODO double-check is_tuneable
             tuneable_blocks = [b for b in encoder_blocks if is_tuneable(b)]
  
             assert self.n_layers <= len(
                 tuneable_blocks
             ), f"Network only has {len(tuneable_blocks)} tuneable blocks, {self.n_layers} specified for finetuning"
 
             # Append parameters of layers for finetuning along with decayed learning rate
@@ -248,30 +250,39 @@
         
     """
 
     def __init__(
             self,
             num_classes: int,
             label_smoothing=0.,
+            class_weights=None,
             **super_kwargs) -> None:
 
         super().__init__(**super_kwargs)
 
         logging.info('Using classification head and cross-entropy loss')
         self.head = LinearClassifier(
             input_dim=self.encoder_dim,
             output_dim=num_classes,
             dropout_prob=self.dropout_prob
         )
         self.label_smoothing = label_smoothing
         self.loss = partial(cross_entropy_loss,
+                            weight=class_weights,
                             label_smoothing=self.label_smoothing)
-        self.train_acc = tm.Accuracy(task='binary', average="micro")
-        self.val_acc = tm.Accuracy(task='binary', average="micro")
-        self.test_acc = tm.Accuracy(task='binary', average="micro")
+        logging.info(f'num_classes: {num_classes}')
+        if num_classes == 2:
+            logging.info('Using binary classification')
+            task = 'binary'
+        else:
+            logging.info('Using multi-class classification')
+            task = 'multiclass'
+        self.train_acc = tm.Accuracy(task=task, average="micro", num_classes=num_classes)
+        self.val_acc = tm.Accuracy(task=task, average="micro", num_classes=num_classes)
+        self.test_acc = tm.Accuracy(task=task, average="micro", num_classes=num_classes)
         
     def step_to_dict(self, y, y_pred, loss):
         y_class_preds = torch.argmax(y_pred, axis=1)
         return {'loss': loss.mean(), 'predictions': y_pred, 'labels': y, 'class_predictions': y_class_preds}
 
     def on_train_batch_end(self, step_output, *args):
         super().on_train_batch_end(step_output, *args)
@@ -381,20 +392,20 @@
     def forward(self, x):
         # returns logits, as recommended for CrossEntropy loss
         x = self.dropout(x)
         x = self.linear(x)
         return x
 
 
-def cross_entropy_loss(y_pred, y, label_smoothing=0.):
+def cross_entropy_loss(y_pred, y, label_smoothing=0., weight=None):
     # y should be shape (batch) and ints
     # y_pred should be shape (batch, classes)
     # returns loss of shape (batch)
     # will reduce myself
-    return F.cross_entropy(y_pred, y.long(), label_smoothing=label_smoothing, reduction='none')
+    return F.cross_entropy(y_pred, y.long(), label_smoothing=label_smoothing, weight=weight, reduction='none')
 
 
 def dirichlet_loss(y_pred, y, question_index_groups):
     # aggregation equiv. to sum(axis=1).mean(), but fewer operations
     # returns loss of shape (batch)
     # my func uses sklearn convention y, y_pred
     return losses.calculate_multiquestion_loss(y, y_pred, question_index_groups).mean()*len(question_index_groups)
@@ -477,15 +488,15 @@
         accelerator=accelerator,
         devices=devices,
         **trainer_kwargs,
     )
 
     return trainer
 
-
+# TODO check exactly which layers get FTd
 def is_tuneable(block_of_layers):
     if len(list(block_of_layers.parameters())) == 0:
         logging.info('Skipping block with no params')
         logging.info(block_of_layers)
         return False
     else:
         # currently, allowed to include batchnorm
```

### Comparing `zoobot-1.0.3/zoobot/pytorch/training/losses.py` & `zoobot-1.0.4/zoobot/pytorch/training/losses.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/pytorch/training/representations.py` & `zoobot-1.0.4/zoobot/pytorch/training/representations.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/pytorch/training/tensorboard_writers.py` & `zoobot-1.0.4/zoobot/pytorch/training/tensorboard_writers.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/pytorch/training/train_with_pytorch_lightning.py` & `zoobot-1.0.4/zoobot/pytorch/training/train_with_pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/shared/benchmark_datasets.py` & `zoobot-1.0.4/zoobot/shared/benchmark_datasets.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,25 +19,26 @@
 
     schema = schemas.decals_dr5_ortho_schema
     logging.info('Schema: {}'.format(schema))
 
     return schema, (train_catalog, val_catalog, test_catalog)
 
 
-def get_gz_evo_benchmark_dataset(data_dir, random_state, download=False, debug=False, datasets=['gz_desi', 'gz_hubble', 'gz_candels', 'gz2', 'gz_rings']):
+def get_gz_evo_benchmark_dataset(data_dir, random_state, download=False, debug=False, datasets=['gz_desi', 'gz_hubble', 'gz_candels', 'gz2', 'gz_rings', 'gz_cosmic_dawn']):
 
     from foundation.datasets import mixed  # not yet public. import will fail if you're not me.
 
     # temporarily, everything *but* hubble, for Ben
     # datasets = ['gz_desi', 'gz_candels', 'gz2', 'gz_rings']
-    datasets = ['gz_desi', 'gz_candels', 'gz_hubble', 'gz2', 'gz_rings']
 
-    _, (temp_train_catalog, temp_val_catalog, _) = mixed.everything_all_dirichlet_with_rings(data_dir, debug, download=download, use_cache=True, datasets=datasets)
+    # TODO temporarily no cache, to remake
+    direct_label_cols, (temp_train_catalog, temp_val_catalog, _) = mixed.everything_all_dirichlet_with_rings(data_dir, debug, download=download, use_cache=True, datasets=datasets)
     canonical_train_catalog = pd.concat([temp_train_catalog, temp_val_catalog], axis=0)
 
     # here I'm going to ignore the test catalog
     train_catalog, hidden_catalog = train_test_split(canonical_train_catalog, test_size=1./3., random_state=random_state)
     val_catalog, test_catalog = train_test_split(hidden_catalog, test_size=2./3., random_state=random_state)
 
     schema = mixed.mixed_schema()
+    assert len(direct_label_cols) == len(schema.label_cols), ValueError((len(direct_label_cols), len(schema)))
     logging.info('Schema: {}'.format(schema))
     return schema, (train_catalog, val_catalog,test_catalog)
```

### Comparing `zoobot-1.0.3/zoobot/shared/compress_representations.py` & `zoobot-1.0.4/zoobot/shared/compress_representations.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/shared/label_metadata.py` & `zoobot-1.0.4/zoobot/shared/label_metadata.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/shared/load_predictions.py` & `zoobot-1.0.4/zoobot/shared/load_predictions.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,31 +36,36 @@
         logging.warning('Passed a single hdf5 loc to load_hdf5s - assuming this is a single file to load, not list of files to load')
         hdf5_locs = [hdf5_locs]  # pretend user passed a list
 
     predictions = []
     prediction_metadata = []
     template_label_cols = None  # will use this var to check consistency of label_cols across each hdf5_loc
     for loc in hdf5_locs:
-        with h5py.File(loc, 'r') as f:
-            logging.debug(f.keys())
-            these_predictions = f['predictions'][:]
-            these_prediction_metadata = {
-                'id_str': f['id_str'].asstr()[:],
-                'hdf5_loc': [os.path.basename(loc) for _ in these_predictions]
-        }
-            predictions.append(these_predictions)  # will create a list where each element is 3D predictions stored in each hdf5
-            prediction_metadata.append(these_prediction_metadata)  # also track id_str, similarly
-
-            if template_label_cols is None:  # first file to load, use this as the expected template
-                template_label_cols = f['label_cols'].asstr()[:]
-                logging.info('Using label columns {} from first hdf5 {}'.format(template_label_cols, loc))
-            else:
-                these_label_cols = f['label_cols'].asstr()[:]
-                if any(these_label_cols != template_label_cols):
-                    raise ValueError('Label columns {} of hdf5 {} do not match first label columns {}'.format(loc, f['label_cols'], template_label_cols))
+        try:
+            with h5py.File(loc, 'r') as f:
+
+                    logging.debug(f.keys())
+                    these_predictions = f['predictions'][:]
+                    these_prediction_metadata = {
+                        'id_str': f['id_str'].asstr()[:],
+                        'hdf5_loc': [os.path.basename(loc) for _ in these_predictions]
+                }
+                    predictions.append(these_predictions)  # will create a list where each element is 3D predictions stored in each hdf5
+                    prediction_metadata.append(these_prediction_metadata)  # also track id_str, similarly
+
+                    if template_label_cols is None:  # first file to load, use this as the expected template
+                        template_label_cols = f['label_cols'].asstr()[:]
+                        logging.info('Using label columns {} from first hdf5 {}'.format(template_label_cols, loc))
+                    else:
+                        these_label_cols = f['label_cols'].asstr()[:]
+                        if any(these_label_cols != template_label_cols):
+                            raise ValueError('Label columns {} of hdf5 {} do not match first label columns {}'.format(loc, f['label_cols'], template_label_cols))
+        except Exception as e:
+            logging.critical('Failed to load {}'.format(loc))
+            raise e
 
 
     # there is no assumption that id_str is unique, or attempt to group predictions by id_str
     # it just maps a set of hdf5 files, each with predictions, to a df of id_str and those loaded predictions (matching row-wise)
     logging.info('All hdf5 loaded, beginning concat.')
     predictions = np.concatenate(predictions, axis=0)
     prediction_metadata = {
@@ -84,26 +89,31 @@
     
     Args:
         hdf5_loc (str): _description_
         save_loc (str): _description_
     """
     assert isinstance(hdf5_loc, str)
 
-    label_cols = schema.label_cols
 
     # concentrations will be of (galaxy, question, model, forward_pass) after going through c_group
     # may be only one model but will still have that dimension (e.g. 1000, 39, 1, 5)
     galaxy_id_df, concentrations, _ = load_hdf5s(hdf5_loc)
 
     if debug:
         logging.warning('Using debug mode of 100k only')
         concentrations = concentrations[:100000]
         galaxy_id_df = galaxy_id_df[:100000]
         save_loc = save_loc.replace('.parquet', '_debug.parquet')
 
+    label_cols = schema.label_cols
+    # TODO optionally ignore all but a subset of columns, for models without finetuning
+    # hdf5_label_cols = label_cols
+    # valid_cols = [col for col in hdf5_label_cols if col in label_col_subset]
+    # concentrations = concentrations[:, valid_cols]
+
     # applies to all questions at once
     # hopefully also supports 3D concentrations (galaxy/question/model/pass)
     logging.info('Concentrations: {}'.format(concentrations.shape))
 
     # supports (galaxy, question, distribution...) shape, no TF needed
     unmasked_fractions = stats.expected_value_of_dirichlet_mixture(concentrations, schema)
```

### Comparing `zoobot-1.0.3/zoobot/shared/save_predictions.py` & `zoobot-1.0.4/zoobot/shared/save_predictions.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/shared/schemas.py` & `zoobot-1.0.4/zoobot/shared/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,14 +264,17 @@
 decals_dr5_ortho_schema = Schema(label_metadata.decals_dr5_ortho_pairs , label_metadata.decals_ortho_dependencies)
 decals_dr8_ortho_schema = Schema(label_metadata.decals_dr8_ortho_pairs , label_metadata.decals_ortho_dependencies)
 decals_all_campaigns_ortho_schema = Schema(label_metadata.decals_all_campaigns_ortho_pairs , label_metadata.decals_ortho_dependencies)
 gz2_ortho_schema = Schema(label_metadata.gz2_ortho_pairs , label_metadata.gz2_ortho_dependencies)
 gz_candels_ortho_schema = Schema(label_metadata.candels_ortho_pairs, label_metadata.candels_ortho_dependencies)
 gz_hubble_ortho_schema = Schema(label_metadata.hubble_ortho_pairs, label_metadata.hubble_ortho_dependencies)
 cosmic_dawn_ortho_schema = Schema(label_metadata.cosmic_dawn_ortho_pairs , label_metadata.cosmic_dawn_ortho_dependencies)
+
+# schemas without orthogonal question suffix (-cd, -dr8, etc)
+cosmic_dawn_schema = Schema(label_metadata.cosmic_dawn_pairs , label_metadata.cosmic_dawn_dependencies)
 gz_rings_schema = Schema(label_metadata.rings_pairs, label_metadata.rings_dependencies)
 desi_schema = Schema(label_metadata.desi_pairs, label_metadata.desi_dependencies)  # for DESI data release prediction users, not for ML training - no -dr5, -dr8, etc
 # note that as this is a call to Schema (and Question and Answer), any logging within those will 
 # trigger basicConfig() and prevent user setting their own logging.
 # so don't log anything during Schema.__init__!
 
 # temp for debugging
```

### Comparing `zoobot-1.0.3/zoobot/shared/stats.py` & `zoobot-1.0.4/zoobot/shared/stats.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/tensorflow/estimators/alexnet_baseline.py` & `zoobot-1.0.4/zoobot/tensorflow/estimators/alexnet_baseline.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/tensorflow/estimators/custom_callbacks.py` & `zoobot-1.0.4/zoobot/tensorflow/estimators/custom_callbacks.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/tensorflow/estimators/custom_layers.py` & `zoobot-1.0.4/zoobot/tensorflow/estimators/custom_layers.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/tensorflow/estimators/define_model.py` & `zoobot-1.0.4/zoobot/tensorflow/estimators/define_model.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/tensorflow/estimators/efficientnet_custom.py` & `zoobot-1.0.4/zoobot/tensorflow/estimators/efficientnet_custom.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/tensorflow/estimators/efficientnet_standard.py` & `zoobot-1.0.4/zoobot/tensorflow/estimators/efficientnet_standard.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/tensorflow/estimators/small_cnn_baseline.py` & `zoobot-1.0.4/zoobot/tensorflow/estimators/small_cnn_baseline.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/tensorflow/predictions/predict_on_dataset.py` & `zoobot-1.0.4/zoobot/tensorflow/predictions/predict_on_dataset.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/tensorflow/predictions/visualize_dirichlet_predictions.py` & `zoobot-1.0.4/zoobot/tensorflow/predictions/visualize_dirichlet_predictions.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/tensorflow/stats/coverage.py` & `zoobot-1.0.4/zoobot/tensorflow/stats/coverage.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/tensorflow/stats/dirichlet_stats.py` & `zoobot-1.0.4/zoobot/tensorflow/stats/dirichlet_stats.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/tensorflow/stats/mixture_stats.py` & `zoobot-1.0.4/zoobot/tensorflow/stats/mixture_stats.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/tensorflow/training/custom_metrics.py` & `zoobot-1.0.4/zoobot/tensorflow/training/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/tensorflow/training/finetune.py` & `zoobot-1.0.4/zoobot/tensorflow/training/finetune.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/tensorflow/training/losses.py` & `zoobot-1.0.4/zoobot/tensorflow/training/losses.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/tensorflow/training/train_with_keras.py` & `zoobot-1.0.4/zoobot/tensorflow/training/train_with_keras.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot/tensorflow/training/training_config.py` & `zoobot-1.0.4/zoobot/tensorflow/training/training_config.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot.egg-info/PKG-INFO` & `zoobot-1.0.4/zoobot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoobot
-Version: 1.0.3
+Version: 1.0.4
 Summary: Galaxy morphology classifiers
 Home-page: https://github.com/mwalmsley/zoobot
 Author: Mike Walmsley
 Author-email: walmsleymk1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -25,25 +25,26 @@
 
 [![Downloads](https://pepy.tech/badge/zoobot)](https://pepy.tech/project/zoobot)
 [![Documentation Status](https://readthedocs.org/projects/zoobot/badge/?version=latest)](https://zoobot.readthedocs.io/)
 ![build](https://github.com/mwalmsley/zoobot/actions/workflows/run_CI.yml/badge.svg)
 ![publish](https://github.com/mwalmsley/zoobot/actions/workflows/python-publish.yml/badge.svg)
 [![PyPI](https://badge.fury.io/py/zoobot.svg)](https://badge.fury.io/py/zoobot)
 [![DOI](https://zenodo.org/badge/343787617.svg)](https://zenodo.org/badge/latestdoi/343787617)
+[![status](https://joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f/status.svg)](https://joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f)
 <a href="https://ascl.net/2203.027"><img src="https://img.shields.io/badge/ascl-2203.027-blue.svg?colorB=262255" alt="ascl:2203.027" /></a>
 
 Zoobot classifies galaxy morphology with deep learning.
 <!-- At Galaxy Zoo, we use Zoobot to help our volunteers classify the galaxies in all our recent catalogues: GZ DECaLS, GZ DESI, GZ Rings and GZ Cosmic Dawn. -->
 
 Zoobot is trained using millions of answers by Galaxy Zoo volunteers. This code will let you **retrain** Zoobot to accurately solve your own prediction task.
 
 - [Install](#installation)
 - [Quickstart](#quickstart)
 - [Worked Examples](#worked-examples)
-- [Pretrained Weights](https://zoobot.readthedocs.io/data_notes.html)
+- [Pretrained Weights](https://zoobot.readthedocs.io/en/latest/data_notes.html)
 - [Datasets](https://www.github.com/mwalmsley/galaxy-datasets)
 - [Documentation](https://zoobot.readthedocs.io/) (for understanding/reference)
 
 ## Installation
 <a name="installation"></a>
 
 You can retrain Zoobot in the cloud with a free GPU using this [Google Colab notebook](https://colab.research.google.com/drive/17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing). To install locally, keep reading.
@@ -122,15 +123,15 @@
 ## Getting Started
 <a name="getting_started"></a>
 
 I suggest starting with the [Colab notebook](https://colab.research.google.com/drive/17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) or the worked examples below, which you can copy and adapt.
 
 For context and explanation, see the [documentation](https://zoobot.readthedocs.io/).
 
-For pretrained model weights, precalculated representations, catalogues, and so forth, see the [data notes](https://zoobot.readthedocs.io/data_notes.html) in particular.
+For pretrained model weights, precalculated representations, catalogues, and so forth, see the [data notes](https://zoobot.readthedocs.io/en/latest/data_notes.html) in particular.
 
 ### Worked Examples
 <a name="worked_examples"></a>
 
 PyTorch (recommended):
 - [pytorch/examples/finetuning/finetune_binary_classification.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/finetuning/finetune_binary_classification.py)
 - [pytorch/examples/finetuning/finetune_counts_full_tree.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/finetuning/finetune_counts_full_tree.py)
@@ -141,15 +142,15 @@
 - [tensorflow/examples/train_model_on_catalog.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/tensorflow/examples/train_model_on_catalog.py) (only necessary to train from scratch)
 - [tensorflow/examples/make_predictions.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/tensorflow/examples/make_predictions.py)
 - [tensorflow/examples/finetune_minimal.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/tensorflow/examples/finetune_minimal.py)
 - [tensorflow/examples/finetune_advanced.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/tensorflow/examples/finetune_advanced.py)
 
 There is more explanation and an API reference on the [docs](https://zoobot.readthedocs.io/).
 
-I also [include](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) the scripts used to create and benchmark our pretrained models. Many pretrained models are available [already](https://zoobot.readthedocs.io/data_notes.html), but if you need one trained on e.g. different input image sizes or with a specific architecture, I can probably make it for you.
+I also [include](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) the scripts used to create and benchmark our pretrained models. Many pretrained models are available [already](https://zoobot.readthedocs.io/en/latest/data_notes.html), but if you need one trained on e.g. different input image sizes or with a specific architecture, I can probably make it for you.
 
 When trained with a decision tree head (ZoobotTree, FinetuneableZoobotTree), Zoobot can learn from volunteer labels of varying confidence and predict posteriors for what the typical volunteer might say. Specifically, this Zoobot mode predicts the parameters for distributions, not simple class labels! For a demonstration of how to interpret these predictions, see the [gz_decals_data_release_analysis_demo.ipynb](https://github.com/mwalmsley/zoobot/blob/main/gz_decals_data_release_analysis_demo.ipynb).
 
 
 
 ### (Optional) Install PyTorch or TensorFlow, with CUDA
 <a name="install_cuda"></a>
@@ -167,15 +168,22 @@
 CUDA 11.2 and CUDNN 8.1 for TensorFlow 2.10.0:
 
     conda create --name zoobot38_tf python==3.8
     conda activate zoobot38_tf
     conda install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0
     export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$CONDA_PREFIX/lib/  # add this environment variable
 
-### Latest features (v1.0.0)
+### Latest minor features (v1.0.4)
+
+- Now supports multi-class finetuning. See `pytorch/examples/finetuning/finetune_multiclass_classification.py`
+- Removed `simplejpeg` dependency due to M1 install issue. 
+- Pinned `timm` version to ensure MaX-ViT models load correctly. Models supporting the latest `timm` will follow.
+- (internal until published) GZ Evo v2 now includes Cosmic Dawn (HSC). Significant performance improvement on HSC finetuning.
+
+### Latest major features (v1.0.0)
 
 v1.0.0 recognises that most of the complexity in this repo is training Zoobot from scratch, but most non-GZ users will probably simply want to load the pretrained Zoobot and finetune it on their data.
 
 - Adds new finetuning interface (`finetune.run_finetuning()`), examples.
 - Refocuses docs on finetuning rather than training from scratch.
 - Rework installation process to separate CUDA from Zoobot (simpler, easier)
 - Better wandb logging throughout, to monitor training
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zoobot Version: 1.0.3 Summary: Galaxy morphology
+Metadata-Version: 2.1 Name: zoobot Version: 1.0.4 Summary: Galaxy morphology
 classifiers Home-page: https://github.com/mwalmsley/zoobot Author: Mike
 Walmsley Author-email: walmsleymk1@gmail.com Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: GNU General Public
 License (GPL) Classifier: Operating System :: OS Independent Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: GPU :: NVIDIA CUDA
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 pytorch_cpu Provides-Extra: pytorch_m1 Provides-Extra: pytorch_cu113 Provides-
@@ -10,24 +10,26 @@
 Provides-Extra: docs License-File: LICENSE # Zoobot [![Downloads](https://
 pepy.tech/badge/zoobot)](https://pepy.tech/project/zoobot) [![Documentation
 Status](https://readthedocs.org/projects/zoobot/badge/?version=latest)](https:/
 /zoobot.readthedocs.io/) ![build](https://github.com/mwalmsley/zoobot/actions/
 workflows/run_CI.yml/badge.svg) ![publish](https://github.com/mwalmsley/zoobot/
 actions/workflows/python-publish.yml/badge.svg) [![PyPI](https://badge.fury.io/
 py/zoobot.svg)](https://badge.fury.io/py/zoobot) [![DOI](https://zenodo.org/
-badge/343787617.svg)](https://zenodo.org/badge/latestdoi/343787617) [ascl:
+badge/343787617.svg)](https://zenodo.org/badge/latestdoi/343787617) [![status]
+(https://joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f/status.svg)]
+(https://joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f) [ascl:
 2203.027] Zoobot classifies galaxy morphology with deep learning.  Zoobot is
 trained using millions of answers by Galaxy Zoo volunteers. This code will let
 you **retrain** Zoobot to accurately solve your own prediction task. -
 [Install](#installation) - [Quickstart](#quickstart) - [Worked Examples]
-(#worked-examples) - [Pretrained Weights](https://zoobot.readthedocs.io/
-data_notes.html) - [Datasets](https://www.github.com/mwalmsley/galaxy-datasets)
-- [Documentation](https://zoobot.readthedocs.io/) (for understanding/reference)
-## Installation  You can retrain Zoobot in the cloud with a free GPU using this
-[Google Colab notebook](https://colab.research.google.com/drive/
+(#worked-examples) - [Pretrained Weights](https://zoobot.readthedocs.io/en/
+latest/data_notes.html) - [Datasets](https://www.github.com/mwalmsley/galaxy-
+datasets) - [Documentation](https://zoobot.readthedocs.io/) (for understanding/
+reference) ## Installation  You can retrain Zoobot in the cloud with a free GPU
+using this [Google Colab notebook](https://colab.research.google.com/drive/
 17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing). To install locally, keep
 reading. Download the code using git: git clone git@github.com:mwalmsley/
 zoobot.git And then pick one of the three commands below to install Zoobot and
 either PyTorch (recommended) or TensorFlow: # Zoobot with PyTorch and a GPU.
 Requires CUDA 11.3. pip install -e "zoobot[pytorch_cu113]" --extra-index-url
 https://download.pytorch.org/whl/cu113 # OR Zoobot with PyTorch and no GPU pip
 install -e "zoobot[pytorch_cpu]" --extra-index-url https://
@@ -64,16 +66,16 @@
 many guides and working examples - see the [Getting Started](#getting-started)
 section below. ## Getting Started  I suggest starting with the [Colab notebook]
 (https://colab.research.google.com/drive/
 17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) or the worked examples below,
 which you can copy and adapt. For context and explanation, see the
 [documentation](https://zoobot.readthedocs.io/). For pretrained model weights,
 precalculated representations, catalogues, and so forth, see the [data notes]
-(https://zoobot.readthedocs.io/data_notes.html) in particular. ### Worked
-Examples  PyTorch (recommended): - [pytorch/examples/finetuning/
+(https://zoobot.readthedocs.io/en/latest/data_notes.html) in particular. ###
+Worked Examples  PyTorch (recommended): - [pytorch/examples/finetuning/
 finetune_binary_classification.py](https://github.com/mwalmsley/zoobot/blob/
 main/zoobot/pytorch/examples/finetuning/finetune_binary_classification.py) -
 [pytorch/examples/finetuning/finetune_counts_full_tree.py](https://github.com/
 mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/finetuning/
 finetune_counts_full_tree.py) - [pytorch/examples/representations/
 get_representations.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/
 pytorch/examples/representations/get_representations.py) - [pytorch/examples/
@@ -87,71 +89,77 @@
 examples/finetune_minimal.py](https://github.com/mwalmsley/zoobot/blob/main/
 zoobot/tensorflow/examples/finetune_minimal.py) - [tensorflow/examples/
 finetune_advanced.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/
 tensorflow/examples/finetune_advanced.py) There is more explanation and an API
 reference on the [docs](https://zoobot.readthedocs.io/). I also [include]
 (https://github.com/mwalmsley/zoobot/blob/main/benchmarks) the scripts used to
 create and benchmark our pretrained models. Many pretrained models are
-available [already](https://zoobot.readthedocs.io/data_notes.html), but if you
-need one trained on e.g. different input image sizes or with a specific
-architecture, I can probably make it for you. When trained with a decision tree
-head (ZoobotTree, FinetuneableZoobotTree), Zoobot can learn from volunteer
-labels of varying confidence and predict posteriors for what the typical
-volunteer might say. Specifically, this Zoobot mode predicts the parameters for
-distributions, not simple class labels! For a demonstration of how to interpret
-these predictions, see the [gz_decals_data_release_analysis_demo.ipynb](https:/
-/github.com/mwalmsley/zoobot/blob/main/
-gz_decals_data_release_analysis_demo.ipynb). ### (Optional) Install PyTorch or
-TensorFlow, with CUDA  *If you're not using a GPU, skip this step. Use the
-pytorch_cpu or tensorflow_cpu options in the section below.* Install PyTorch
-1.12.1 or Tensorflow 2.10.0 and compatible CUDA drivers. I highly recommend
-using [conda](https://docs.conda.io/en/latest/miniconda.html) to do this. Conda
-will handle both creating a new virtual environment (`conda create`) and
-installing CUDA (`cudatoolkit`, `cudnn`) CUDA 11.3 for PyTorch: conda create --
-name zoobot38_torch python==3.8 conda activate zoobot38_torch conda install -
-c conda-forge cudatoolkit=11.3 CUDA 11.2 and CUDNN 8.1 for TensorFlow 2.10.0:
-conda create --name zoobot38_tf python==3.8 conda activate zoobot38_tf conda
-install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0 export
+available [already](https://zoobot.readthedocs.io/en/latest/data_notes.html),
+but if you need one trained on e.g. different input image sizes or with a
+specific architecture, I can probably make it for you. When trained with a
+decision tree head (ZoobotTree, FinetuneableZoobotTree), Zoobot can learn from
+volunteer labels of varying confidence and predict posteriors for what the
+typical volunteer might say. Specifically, this Zoobot mode predicts the
+parameters for distributions, not simple class labels! For a demonstration of
+how to interpret these predictions, see the
+[gz_decals_data_release_analysis_demo.ipynb](https://github.com/mwalmsley/
+zoobot/blob/main/gz_decals_data_release_analysis_demo.ipynb). ### (Optional)
+Install PyTorch or TensorFlow, with CUDA  *If you're not using a GPU, skip this
+step. Use the pytorch_cpu or tensorflow_cpu options in the section below.*
+Install PyTorch 1.12.1 or Tensorflow 2.10.0 and compatible CUDA drivers. I
+highly recommend using [conda](https://docs.conda.io/en/latest/miniconda.html)
+to do this. Conda will handle both creating a new virtual environment (`conda
+create`) and installing CUDA (`cudatoolkit`, `cudnn`) CUDA 11.3 for PyTorch:
+conda create --name zoobot38_torch python==3.8 conda activate zoobot38_torch
+conda install -c conda-forge cudatoolkit=11.3 CUDA 11.2 and CUDNN 8.1 for
+TensorFlow 2.10.0: conda create --name zoobot38_tf python==3.8 conda activate
+zoobot38_tf conda install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0 export
 LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$CONDA_PREFIX/lib/ # add this environment
-variable ### Latest features (v1.0.0) v1.0.0 recognises that most of the
-complexity in this repo is training Zoobot from scratch, but most non-GZ users
-will probably simply want to load the pretrained Zoobot and finetune it on
-their data. - Adds new finetuning interface (`finetune.run_finetuning()`),
-examples. - Refocuses docs on finetuning rather than training from scratch. -
-Rework installation process to separate CUDA from Zoobot (simpler, easier) -
-Better wandb logging throughout, to monitor training - Remove need to make
-TFRecords. Now TF directly uses images. - Refactor out augmentations and
-datasets to `galaxy-datasets` repo. TF and Torch now use identical
-augmentations (via albumentations). - Many small quality-of-life improvements
-Contributions are very welcome and will be credited in any future work. Please
-get in touch! See [CONTRIBUTING.md](https://github.com/mwalmsley/zoobot/blob/
-main/benchmarks) for more. ### Benchmarks and Replication - Training from
-Scratch The [benchmarks](https://github.com/mwalmsley/zoobot/blob/main/
-benchmarks) folder contains slurm and Python scripts to train Zoobot from
-scratch. We use these scripts to make sure new code versions work well, and
-that TensorFlow and PyTorch achieve similar performance. Training Zoobot using
-the GZ DECaLS dataset option will create models very similar to those used for
-the GZ DECaLS catalogue and shared with the early versions of this repo. The GZ
-DESI Zoobot model is trained on additional data (GZD-1, GZD-2), as the GZ Evo
-Zoobot model (GZD-1/2/5, Hubble, Candels, GZ2). ### Citing We have submitted a
-JOSS paper to describe Zoobot itself. We hope this will become the single
-point-of-reference for Zoobot. Meanwhile, please cite the [Galaxy Zoo DECaLS]
-(https://arxiv.org/abs/2102.08414), which uses the code that evolved into
-Zoobot: @article{Walmsley2022decals, author = {Mike Walmsley and Chris Lintott
-and Geron Tobias and Sandor J Kruk and Coleman Krawczyk and Kyle Willett and
-Steven Bamford and William Keel and Lee S Kelvin and Lucy Fortson and Karen
-Masters and Vihang Mehta and Brooke Simmons and Rebecca J Smethurst and
-Elisabeth M L Baeten and Christine Macmillan}, issue = {3}, journal = {Monthly
-Notices of the Royal Astronomical Society}, month = {12}, pages = {3966-3988},
-title = {Galaxy Zoo DECaLS: Detailed Visual Morphology Measurements from
-Volunteers and Deep Learning for 314,000 Galaxies}, volume = {509}, url =
-{https://arxiv.org/abs/2102.08414}, year = {2022}, } You might be interested in
-reading papers using Zoobot: - [Galaxy Zoo DECaLS](https://arxiv.org/abs/
-2102.08414) (first use at Galaxy Zoo) - [A Comparison of Deep Learning
-Architectures for Optical Galaxy Morphology Classification](https://arxiv.org/
-abs/2111.04353) - [Practical Galaxy Morphology Tools from Deep Supervised
-Representation Learning](https://arxiv.org/abs/2110.12735) - [Towards
-Foundation Models for Galaxy Morphology](https://arxiv.org/abs/2206.11927)
-(adding contrastive learning) - [Harnessing the Hubble Space Telescope
-Archives: A Catalogue of 21,926 Interacting Galaxies](https://arxiv.org/abs/
-2303.00366) Many other works use Zoobot indirectly via the [Galaxy Zoo DECaLS]
-(https://arxiv.org/abs/2102.08414) catalog.
+variable ### Latest minor features (v1.0.4) - Now supports multi-class
+finetuning. See `pytorch/examples/finetuning/
+finetune_multiclass_classification.py` - Removed `simplejpeg` dependency due to
+M1 install issue. - Pinned `timm` version to ensure MaX-ViT models load
+correctly. Models supporting the latest `timm` will follow. - (internal until
+published) GZ Evo v2 now includes Cosmic Dawn (HSC). Significant performance
+improvement on HSC finetuning. ### Latest major features (v1.0.0) v1.0.0
+recognises that most of the complexity in this repo is training Zoobot from
+scratch, but most non-GZ users will probably simply want to load the pretrained
+Zoobot and finetune it on their data. - Adds new finetuning interface
+(`finetune.run_finetuning()`), examples. - Refocuses docs on finetuning rather
+than training from scratch. - Rework installation process to separate CUDA from
+Zoobot (simpler, easier) - Better wandb logging throughout, to monitor training
+- Remove need to make TFRecords. Now TF directly uses images. - Refactor out
+augmentations and datasets to `galaxy-datasets` repo. TF and Torch now use
+identical augmentations (via albumentations). - Many small quality-of-life
+improvements Contributions are very welcome and will be credited in any future
+work. Please get in touch! See [CONTRIBUTING.md](https://github.com/mwalmsley/
+zoobot/blob/main/benchmarks) for more. ### Benchmarks and Replication -
+Training from Scratch The [benchmarks](https://github.com/mwalmsley/zoobot/
+blob/main/benchmarks) folder contains slurm and Python scripts to train Zoobot
+from scratch. We use these scripts to make sure new code versions work well,
+and that TensorFlow and PyTorch achieve similar performance. Training Zoobot
+using the GZ DECaLS dataset option will create models very similar to those
+used for the GZ DECaLS catalogue and shared with the early versions of this
+repo. The GZ DESI Zoobot model is trained on additional data (GZD-1, GZD-2), as
+the GZ Evo Zoobot model (GZD-1/2/5, Hubble, Candels, GZ2). ### Citing We have
+submitted a JOSS paper to describe Zoobot itself. We hope this will become the
+single point-of-reference for Zoobot. Meanwhile, please cite the [Galaxy Zoo
+DECaLS](https://arxiv.org/abs/2102.08414), which uses the code that evolved
+into Zoobot: @article{Walmsley2022decals, author = {Mike Walmsley and Chris
+Lintott and Geron Tobias and Sandor J Kruk and Coleman Krawczyk and Kyle
+Willett and Steven Bamford and William Keel and Lee S Kelvin and Lucy Fortson
+and Karen Masters and Vihang Mehta and Brooke Simmons and Rebecca J Smethurst
+and Elisabeth M L Baeten and Christine Macmillan}, issue = {3}, journal =
+{Monthly Notices of the Royal Astronomical Society}, month = {12}, pages =
+{3966-3988}, title = {Galaxy Zoo DECaLS: Detailed Visual Morphology
+Measurements from Volunteers and Deep Learning for 314,000 Galaxies}, volume =
+{509}, url = {https://arxiv.org/abs/2102.08414}, year = {2022}, } You might be
+interested in reading papers using Zoobot: - [Galaxy Zoo DECaLS](https://
+arxiv.org/abs/2102.08414) (first use at Galaxy Zoo) - [A Comparison of Deep
+Learning Architectures for Optical Galaxy Morphology Classification](https://
+arxiv.org/abs/2111.04353) - [Practical Galaxy Morphology Tools from Deep
+Supervised Representation Learning](https://arxiv.org/abs/2110.12735) -
+[Towards Foundation Models for Galaxy Morphology](https://arxiv.org/abs/
+2206.11927) (adding contrastive learning) - [Harnessing the Hubble Space
+Telescope Archives: A Catalogue of 21,926 Interacting Galaxies](https://
+arxiv.org/abs/2303.00366) Many other works use Zoobot indirectly via the
+[Galaxy Zoo DECaLS](https://arxiv.org/abs/2102.08414) catalog.
```

### Comparing `zoobot-1.0.3/zoobot.egg-info/SOURCES.txt` & `zoobot-1.0.4/zoobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.3/zoobot.egg-info/requires.txt` & `zoobot-1.0.4/zoobot.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -7,62 +7,58 @@
 astropy
 scikit-image>=0.19.2
 scikit-learn>=1.0.2
 matplotlib
 pyarrow
 wandb
 setuptools==59.5.0
-galaxy-datasets==0.0.12
+galaxy-datasets==0.0.14
 
 [docs]
 Sphinx
 sphinxcontrib-napoleon
 furo
 docutils<0.18
 
 [pytorch_colab]
 pytorch-lightning>=2.0.0
-simplejpeg
 albumentations
 pyro-ppl>=1.8.0
 torchmetrics==0.11.0
-timm
+timm==0.6.12
 
 [pytorch_cpu]
 torch==1.12.1+cpu
 torchvision==0.13.1+cpu
 torchaudio==0.12.1
 pytorch-lightning>=2.0.0
-simplejpeg
 albumentations
 pyro-ppl==1.8.0
 torchmetrics==0.11.0
-timm
+timm==0.6.12
 
 [pytorch_cu113]
 torch==1.12.1+cu113
 torchvision==0.13.1+cu113
 torchaudio==0.12.1
 pytorch-lightning>=2.0.0
-simplejpeg
 albumentations
 pyro-ppl==1.8.0
 torchmetrics==0.11.0
-timm
+timm==0.6.12
 
 [pytorch_m1]
 torch==1.12.1
 torchvision==0.13.1
 torchaudio==0.12.1
 pytorch-lightning>=2.0.0
-simplejpeg
 albumentations
 pyro-ppl==1.8.0
 torchmetrics==0.11.0
-timm
+timm==0.6.12
 
 [tensorflow]
 tensorflow==2.10.0
 keras_applications
 tensorflow_probability==0.18.0
 protobuf<=3.19
```

