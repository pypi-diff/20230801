# Comparing `tmp/torchtnt-nightly-2023.7.9.tar.gz` & `tmp/torchtnt-nightly-2023.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchtnt-nightly-2023.7.9.tar", last modified: Sun Jul  9 11:23:36 2023, max compression
+gzip compressed data, was "torchtnt-nightly-2023.8.1.tar", last modified: Tue Aug  1 11:27:46 2023, max compression
```

## Comparing `torchtnt-nightly-2023.7.9.tar` & `torchtnt-nightly-2023.8.1.tar`

### file list

```diff
@@ -1,75 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:23:36.100377 torchtnt-nightly-2023.7.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-09 11:23:36.100377 torchtnt-nightly-2023.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 11:23:36.100377 torchtnt-nightly-2023.7.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:23:36.092377 torchtnt-nightly-2023.7.9/torchtnt/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:23:36.092377 torchtnt-nightly-2023.7.9/torchtnt/framework/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36790 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/auto_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:23:36.096377 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/base_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/learning_rate_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/module_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/pytorch_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/system_resources_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/torchsnapshot_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/tqdm_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/train_progress_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    15355 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:23:36.096377 torchtnt-nightly-2023.7.9/torchtnt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:23:36.096377 torchtnt-nightly-2023.7.9/torchtnt/utils/data/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/data/data_prefetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/data/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/data/multi_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/data/profile_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19191 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/early_stop_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/fsspec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:23:36.096377 torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/oom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/prepare_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/rank_zero_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13242 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-09 11:22:10.000000 torchtnt-nightly-2023.7.9/torchtnt/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:23:36.100377 torchtnt-nightly-2023.7.9/torchtnt_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-09 11:23:36.000000 torchtnt-nightly-2023.7.9/torchtnt_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-09 11:23:36.000000 torchtnt-nightly-2023.7.9/torchtnt_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 11:23:36.000000 torchtnt-nightly-2023.7.9/torchtnt_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-09 11:23:36.000000 torchtnt-nightly-2023.7.9/torchtnt_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 11:23:36.000000 torchtnt-nightly-2023.7.9/torchtnt_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 11:23:36.000000 torchtnt-nightly-2023.7.9/torchtnt_nightly.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:27:46.742790 torchtnt-nightly-2023.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-01 11:27:46.742790 torchtnt-nightly-2023.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:27:46.742790 torchtnt-nightly-2023.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:27:46.710789 torchtnt-nightly-2023.8.1/torchtnt/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:27:46.718789 torchtnt-nightly-2023.8.1/torchtnt/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37488 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/auto_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:27:46.722789 torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/base_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/learning_rate_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/module_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/pytorch_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/system_resources_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/torchsnapshot_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/tqdm_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/train_progress_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16174 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:27:46.734789 torchtnt-nightly-2023.8.1/torchtnt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:27:46.738789 torchtnt-nightly-2023.8.1/torchtnt/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/data/data_prefetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/data/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/data/multi_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/data/profile_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19191 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/early_stop_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/flops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/fsspec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:27:46.742790 torchtnt-nightly-2023.8.1/torchtnt/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/loggers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/loggers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/loggers/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/loggers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/loggers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27731 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/module_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/oom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/prepare_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/rank_zero_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-01 11:24:14.000000 torchtnt-nightly-2023.8.1/torchtnt/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:27:46.742790 torchtnt-nightly-2023.8.1/torchtnt_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-01 11:27:46.000000 torchtnt-nightly-2023.8.1/torchtnt_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-08-01 11:27:46.000000 torchtnt-nightly-2023.8.1/torchtnt_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:27:46.000000 torchtnt-nightly-2023.8.1/torchtnt_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-01 11:27:46.000000 torchtnt-nightly-2023.8.1/torchtnt_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 11:27:46.000000 torchtnt-nightly-2023.8.1/torchtnt_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:27:46.000000 torchtnt-nightly-2023.8.1/torchtnt_nightly.egg-info/zip-safe
```

### Comparing `torchtnt-nightly-2023.7.9/LICENSE` & `torchtnt-nightly-2023.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/PKG-INFO` & `torchtnt-nightly-2023.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2023.7.9
+Version: 2023.8.1
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.7.9 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.8.1 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt-nightly-2023.7.9/README.md` & `torchtnt-nightly-2023.8.1/README.md`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/setup.py` & `torchtnt-nightly-2023.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/__init__.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,34 +2,30 @@
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 from .auto_unit import AutoPredictUnit, AutoUnit
 from .callback import Callback
-from .evaluate import evaluate, init_eval_state
-from .fit import fit, init_fit_state
-from .predict import init_predict_state, predict
+from .evaluate import evaluate
+from .fit import fit
+from .predict import predict
 from .state import PhaseState, State
-from .train import init_train_state, train
+from .train import train
 from .unit import EvalUnit, PredictUnit, TEvalUnit, TPredictUnit, TrainUnit, TTrainUnit
 
 __all__ = [
     "AutoPredictUnit",
     "AutoUnit",
     "Callback",
     "evaluate",
-    "init_eval_state",
     "fit",
-    "init_fit_state",
-    "init_predict_state",
     "predict",
     "PhaseState",
     "State",
-    "init_train_state",
     "train",
     "EvalUnit",
     "PredictUnit",
     "TEvalUnit",
     "TPredictUnit",
     "TrainUnit",
     "TTrainUnit",
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/_test_utils.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/_test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,39 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-from typing import Iterator, Tuple
+from typing import Any, Iterable, Iterator, Optional, Tuple
 
 import torch
 from torch import nn, Tensor
 from torch.utils.data import DataLoader, Dataset, IterableDataset, TensorDataset
-from torchtnt.framework.state import State
+from torchtnt.framework.state import EntryPoint, PhaseState, State
 from torchtnt.framework.unit import EvalUnit, PredictUnit, TrainUnit
 
 Batch = Tuple[torch.Tensor, torch.Tensor]
 
 
+# pyre-ignore
+def get_dummy_train_state(dataloader: Optional[Iterable[Any]] = None) -> State:
+    return State(
+        entry_point=EntryPoint.TRAIN,
+        train_state=PhaseState(
+            dataloader=dataloader or [1, 2, 3, 4],
+            max_epochs=1,
+            max_steps=1,
+            max_steps_per_epoch=1,
+        ),
+        timer=None,
+    )
+
+
 class DummyEvalUnit(EvalUnit[Batch]):
     def __init__(self, input_dim: int) -> None:
         super().__init__()
         # initialize module & loss_fn
         self.module = nn.Linear(input_dim, 2)
         self.loss_fn = nn.CrossEntropyLoss()
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/auto_unit.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/auto_unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,29 +21,22 @@
     apply_activation_checkpointing,
     checkpoint_wrapper,
     CheckpointImpl,
 )
 from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
 from torch.nn.parallel import DistributedDataParallel as DDP
 from torch.optim.swa_utils import AveragedModel, SWALR
-from torchtnt.framework.state import ActivePhase, State
+from torchtnt.framework.state import ActivePhase, EntryPoint, State
 from torchtnt.framework.unit import EvalUnit, PredictUnit, TPredictData, TrainUnit
-from torchtnt.framework.utils import (
-    _get_timing_context,
-    _is_fsdp_module,
-    get_current_progress,
-)
-from torchtnt.utils import (
-    init_from_env,
-    TLRScheduler,
-    transfer_batch_norm_stats,
-    transfer_weights,
-)
+from torchtnt.framework.utils import _is_fsdp_module, get_timing_context
 from torchtnt.utils.device import copy_data_to_device, record_data_in_stream
-from torchtnt.utils.prepare_model import (
+from torchtnt.utils.env import init_from_env
+from torchtnt.utils.lr_scheduler import TLRScheduler
+from torchtnt.utils.misc import transfer_batch_norm_stats, transfer_weights
+from torchtnt.utils.prepare_module import (
     DDPStrategy,
     FSDPStrategy,
     prepare_ddp,
     prepare_fsdp,
     Strategy,
 )
 from torchtnt.utils.rank_zero_log import rank_zero_warn
@@ -145,14 +138,15 @@
         self,
         *,
         module: torch.nn.Module,
         device: Optional[torch.device] = None,
         strategy: Optional[Union[Strategy, str]] = None,
         precision: Optional[Union[str, torch.dtype]] = None,
         torch_compile_params: Optional[TorchCompileParams] = None,
+        detect_anomaly: Optional[bool] = None,
     ) -> None:
         """
         AutoPredictUnit is a convenience for users who are running inference and would like to have certain features handled for them, such as:
         - Moving data to the correct device.
         - Running inference under a mixed precision context.
         - Handling data parallel replication, especially if the module cannot fit on a single device using FullyShardedDataParallel.
         - Profiling the data transfer to device and forward pass.
@@ -166,14 +160,15 @@
 
         Args:
             module: module to be used during prediction.
             device: the device to be used.
             precision: the precision to use in training, as either a string or a torch.dtype.
             strategy: the data parallelization strategy to be used. if a string, must be one of ``ddp`` or ``fsdp``.
             torch_compile_params: params for Torch compile https://pytorch.org/docs/stable/generated/torch.compile.html
+            detect_anomaly: whether to enable anomaly detection for the autograd engine https://pytorch.org/docs/stable/autograd.html#anomaly-detection
 
         Note:
             Torch compile support is only available in PyTorch 2.0 or higher.
         """
         if torch_compile_params:
             _validate_torch_compile_available()
 
@@ -213,40 +208,53 @@
                     self.device,
                     strategy,
                     self.precision,
                 )
         else:
             module = module.to(self.device)
         if torch_compile_params:
-            # use in-place compile to avoid altering the state_dict keys
-            module.compile(**asdict(torch_compile_params))
+            try:
+                # use in-place compile to avoid altering the state_dict keys
+                module.compile(**asdict(torch_compile_params))
+            except AttributeError:
+                rank_zero_warn(
+                    "Please install pytorch nightlies to use in-place compile to avoid altering the state_dict keys when checkpointing."
+                )
+                torch.compile(module, **asdict(torch_compile_params))
         self.module: torch.nn.Module = module
 
         # cuda stream to use for moving data to device
         self._prefetch_stream: Optional[torch.cuda.streams.Stream] = (
             torch.cuda.Stream() if self.device.type == "cuda" else None
         )
         # the next batch which has been prefetched and is ready to be used
         self._next_batch: Optional[TPredictData] = None
 
         # whether the next batch has been prefetched and is ready to be used
         self._prefetched: bool = False
 
+        self.detect_anomaly = detect_anomaly
+
     def predict_step(self, state: State, data: Iterator[TPredictData]) -> Any:
         batch = self._get_next_batch(state, data)
 
-        with self.maybe_autocast_precision:
-            with _get_timing_context(state, f"{self.__class__.__name__}.forward"):
+        # if detect_anomaly is true, run forward pass under detect_anomaly context
+        detect_anomaly = self.detect_anomaly
+        maybe_detect_anomaly = (
+            torch.autograd.set_detect_anomaly(detect_anomaly)
+            if detect_anomaly is not None
+            else contextlib.nullcontext()
+        )
+
+        with self.maybe_autocast_precision, maybe_detect_anomaly:
+            with get_timing_context(state, f"{self.__class__.__name__}.forward"):
                 outputs = self.module(batch)
 
-        step = get_current_progress(state).num_steps_completed
-        with _get_timing_context(
-            state, f"{self.__class__.__name__}.on_predict_step_end"
-        ):
-            self.on_predict_step_end(state, batch, step, outputs)
+        step = self.predict_progress.num_steps_completed
+        self.on_predict_step_end(state, batch, step, outputs)
         return outputs
 
     def on_predict_step_end(
         self, state: State, data: TPredictData, step: int, outputs: Any
     ) -> None:
         """
         This will be called at the end of every ``predict_step`` before returning. The user can implement this method with code to update and log their metrics,
@@ -283,26 +291,26 @@
         self, state: State, data: Iterator[TPredictData]
     ) -> TPredictData:
         if not self._prefetched:
             self._prefetch_next_batch(state, data)
             self._prefetched = True
 
         if self._prefetch_stream:
-            with _get_timing_context(state, f"{self.__class__.__name__}.wait_stream"):
+            with get_timing_context(state, f"{self.__class__.__name__}.wait_stream"):
                 # wait on the CUDA stream to complete the host to device copy
                 torch.cuda.current_stream().wait_stream(self._prefetch_stream)
 
         # get the next batch which was stored by _prefetch_next_batch
         batch = self._next_batch
         if batch is None:
             self._prefetched = False
             raise StopIteration
 
         if self._prefetch_stream:
-            with _get_timing_context(
+            with get_timing_context(
                 state, f"{self.__class__.__name__}.record_data_in_stream"
             ):
                 # record the batch in the current stream
                 record_data_in_stream(batch, torch.cuda.current_stream())
 
         # kick off prefetching the next batch
         self._prefetch_next_batch(state, data)
@@ -310,28 +318,28 @@
 
     def _prefetch_next_batch(
         self, state: State, data_iter: Iterator[TPredictData]
     ) -> None:
         """Prefetch the next batch on a separate CUDA stream."""
 
         try:
-            with _get_timing_context(
+            with get_timing_context(
                 state, f"{self.__class__.__name__}.next(data_iter)"
             ):
                 next_batch = next(data_iter)
         except StopIteration:
             self._next_batch = None
             return
 
         non_blocking = (
             True if self.device.type == "cuda" and self._prefetched else False
         )
 
         # if on cpu, self._prefetch_stream is None so the torch.cuda.stream call is a no-op
-        with torch.cuda.stream(self._prefetch_stream), _get_timing_context(
+        with torch.cuda.stream(self._prefetch_stream), get_timing_context(
             state, f"{self.__class__.__name__}.move_data_to_device"
         ):
             self._next_batch = self.move_data_to_device(
                 state, next_batch, non_blocking=non_blocking
             )
 
 
@@ -465,16 +473,22 @@
 
         if torch_compile_params:
             # pyre-ignore
             self.compute_loss = torch.compile(
                 self.compute_loss,
                 **asdict(torch_compile_params),
             )
-            # use in-place compile to avoid altering the state_dict keys
-            module.compile(**asdict(torch_compile_params))
+            try:
+                # use in-place compile to avoid altering the state_dict keys
+                module.compile(**asdict(torch_compile_params))
+            except AttributeError:
+                rank_zero_warn(
+                    "Please install pytorch nightlies to use in-place compile to avoid altering the state_dict keys when checkpointing."
+                )
+                torch.compile(module, **asdict(torch_compile_params))
 
         self.module: torch.nn.Module = module
 
         self.step_lr_interval = step_lr_interval
 
         self.gradient_accumulation_steps = gradient_accumulation_steps
 
@@ -557,15 +571,15 @@
         return copy_data_to_device(data, self.device, non_blocking=non_blocking)
 
     def _prefetch_next_batch(self, state: State, data_iter: Iterator[TData]) -> None:
         """Prefetch the next batch on a separate CUDA stream."""
 
         phase = state.active_phase.name.lower()
         try:
-            with _get_timing_context(
+            with get_timing_context(
                 state, f"{self.__class__.__name__}.{phase}.next(data_iter)"
             ):
                 next_batch = next(data_iter)
         except StopIteration:
             self._next_batch = None
             self._is_last_train_batch = True
             return
@@ -575,59 +589,57 @@
             if state.active_phase == ActivePhase.TRAIN
             and self.device.type == "cuda"
             and self._prefetched
             else False
         )
 
         # if on cpu, self._prefetch_stream is None so the torch.cuda.stream call is a no-op
-        with torch.cuda.stream(self._prefetch_stream), _get_timing_context(
+        with torch.cuda.stream(self._prefetch_stream), get_timing_context(
             state, f"{self.__class__.__name__}.{phase}.move_data_to_device"
         ):
             self._next_batch = self.move_data_to_device(
                 state, next_batch, non_blocking=non_blocking
             )
 
     def _get_next_batch(self, state: State, data: Iterator[TData]) -> TData:
         if not self._prefetched:
             self._prefetch_next_batch(state, data)
             self._prefetched = True
 
         if self._prefetch_stream:
-            with _get_timing_context(state, f"{self.__class__.__name__}.wait_stream"):
+            with get_timing_context(state, f"{self.__class__.__name__}.wait_stream"):
                 # wait on the CUDA stream to complete the host to device copy
                 torch.cuda.current_stream().wait_stream(self._prefetch_stream)
 
         # get the next batch which was stored by _prefetch_next_batch
         batch = self._next_batch
         if batch is None:
             self._prefetched = False
             self._is_last_train_batch = False
             raise StopIteration
 
         if self._prefetch_stream:
-            with _get_timing_context(
+            with get_timing_context(
                 state, f"{self.__class__.__name__}.record_data_in_stream"
             ):
                 # record the batch in the current stream
                 record_data_in_stream(batch, torch.cuda.current_stream())
 
         # prefetch the next batch
         self._prefetch_next_batch(state, data)
 
         return batch
 
     def train_step(
         self, state: State, data: Iterator[TData]
     ) -> Tuple[torch.Tensor, Any]:
-        train_state = none_throws(state.train_state)
-
         batch = self._get_next_batch(state, data)
 
         should_update_weights = (
-            train_state.progress.num_steps_completed_in_epoch + 1
+            self.train_progress.num_steps_completed_in_epoch + 1
         ) % self.gradient_accumulation_steps == 0 or self._is_last_train_batch
 
         # for pyre, assign to local variable
         module = self.module
 
         # if using gradient accumulation with either DDP or FSDP, when in a step where we will not update the weights,
         # run forward and backward in no_sync context
@@ -647,107 +659,102 @@
             if detect_anomaly is not None
             else contextlib.nullcontext()
         )
 
         grad_scaler = self.grad_scaler
         with maybe_no_sync, maybe_detect_anomaly:
             with self.maybe_autocast_precision:
-                with _get_timing_context(
+                with get_timing_context(
                     state, f"{self.__class__.__name__}.compute_loss"
                 ):
                     # Run the forward pass and compute the loss
                     loss, outputs = self.compute_loss(state, batch)
 
             # normalize loss to account for gradient accumulation
             loss = loss / self.gradient_accumulation_steps
 
             if grad_scaler:
                 scaled_loss = grad_scaler.scale(loss)
-                with _get_timing_context(state, f"{self.__class__.__name__}.backward"):
+                with get_timing_context(state, f"{self.__class__.__name__}.backward"):
                     scaled_loss.backward()
             else:
-                with _get_timing_context(state, f"{self.__class__.__name__}.backward"):
+                with get_timing_context(state, f"{self.__class__.__name__}.backward"):
                     loss.backward()
 
         if should_update_weights:
             # Run gradient clipping, optimizer step, and zero_grad
             clip_grad_norm = self.clip_grad_norm
             clip_grad_value = self.clip_grad_value
             if grad_scaler and (clip_grad_norm or clip_grad_value):
                 # unscale the gradients of optimizer's assigned params in-place in preparation for gradient clipping
-                with _get_timing_context(
+                with get_timing_context(
                     state, f"{self.__class__.__name__}.grad_unscale"
                 ):
                     grad_scaler.unscale_(self.optimizer)
 
             # gradient norm clipping
             if clip_grad_norm:
                 if _is_fsdp_module(module):
                     if isinstance(module, FSDP):
-                        with _get_timing_context(
+                        with get_timing_context(
                             state, f"{self.__class__.__name__}.clip_grad_norm"
                         ):
                             module.clip_grad_norm_(max_norm=clip_grad_norm)
                     else:
                         raise RuntimeError(
                             "Composable FSDP clip_grad_norm is not yet implemented: https://github.com/pytorch/pytorch/issues/97271"
                         )
                 else:
-                    with _get_timing_context(
+                    with get_timing_context(
                         state, f"{self.__class__.__name__}.clip_grad_norm"
                     ):
                         torch.nn.utils.clip_grad_norm_(
                             parameters=module.parameters(),
                             max_norm=clip_grad_norm,
                         )
 
             # gradient value clipping
             if clip_grad_value:
-                with _get_timing_context(
+                with get_timing_context(
                     state, f"{self.__class__.__name__}.clip_grad_value"
                 ):
                     torch.nn.utils.clip_grad_value_(
                         parameters=module.parameters(),
                         clip_value=clip_grad_value,
                     )
 
-            with _get_timing_context(
-                state, f"{self.__class__.__name__}.optimizer_step"
-            ):
+            with get_timing_context(state, f"{self.__class__.__name__}.optimizer_step"):
                 if grad_scaler:
                     grad_scaler.step(self.optimizer)
                     # update the scale for next iteration
                     grad_scaler.update()
                 else:
                     self.optimizer.step()
 
             # sets gradients to zero
-            with _get_timing_context(
+            with get_timing_context(
                 state, f"{self.__class__.__name__}.optimizer_zero_grad"
             ):
                 self.optimizer.zero_grad(set_to_none=True)
 
             # optionally step lr scheduler if SWA not in use
-            train_state = none_throws(state.train_state)
             if (
                 self.swa_params is None
-                or train_state.progress.num_epochs_completed
+                or self.train_progress.num_epochs_completed
                 < self.swa_params.epoch_start
             ):
                 lr_scheduler = self.lr_scheduler
                 if lr_scheduler and self.step_lr_interval == "step":
-                    with _get_timing_context(
+                    with get_timing_context(
                         state, f"{self.__class__.__name__}.lr_scheduler_step"
                     ):
                         lr_scheduler.step()
 
-        step = get_current_progress(state).num_steps_completed
-        # users can override this, by default this is a no-op
-        with _get_timing_context(state, f"{self.__class__.__name__}.on_train_step_end"):
-            self.on_train_step_end(state, batch, step, loss, outputs)
+        step = self.train_progress.num_steps_completed
+        self.on_train_step_end(state, batch, step, loss, outputs)
         return loss, outputs
 
     def on_train_step_end(
         self, state: State, data: TData, step: int, loss: torch.Tensor, outputs: Any
     ) -> None:
         """
         This will be called at the end of every ``train_step`` before returning. The user can implement this method with code to update and log their metrics,
@@ -762,68 +769,68 @@
         """
         pass
 
     def on_train_epoch_end(self, state: State) -> None:
         """
         Note: if overriding ``on_train_epoch_end``, remember to call ``super().on_train_epoch_end()``
         """
-        train_state = none_throws(state.train_state)
-
         if (
             self.swa_model
             and self.swa_params
-            and train_state.progress.num_epochs_completed >= self.swa_params.epoch_start
+            and self.train_progress.num_epochs_completed >= self.swa_params.epoch_start
         ):
-            with _get_timing_context(
+            with get_timing_context(
                 state, f"{self.__class__.__name__}.stochastic_weight_avg_update"
             ):
                 self.swa_model.update_parameters(self.module)
-            with _get_timing_context(
+            with get_timing_context(
                 state, f"{self.__class__.__name__}.stochastic_weight_avg_step"
             ):
                 none_throws(self.swa_scheduler).step()
         elif self.lr_scheduler and self.step_lr_interval == "epoch":
             # optionally step lr scheduler
-            with _get_timing_context(
+            with get_timing_context(
                 state, f"{self.__class__.__name__}.lr_scheduler_step"
             ):
                 self.lr_scheduler.step()
 
     def on_train_end(self, state: State) -> None:
         """
         Note that if using SWA and implementing `on_train_end()`, must call `super().on_train_end()`.
         """
         swa_model = self.swa_model
         if swa_model:
-            with _get_timing_context(
+            with get_timing_context(
                 state,
                 f"{self.__class__.__name__}.stochastic_weight_avg_transfer_weights",
             ):
                 transfer_weights(swa_model, self.module)
-            with _get_timing_context(
+            with get_timing_context(
                 state,
                 f"{self.__class__.__name__}.stochastic_weight_avg_transfer_batch_norm_stats",
             ):
                 transfer_batch_norm_stats(swa_model, self.module)
 
     def eval_step(self, state: State, data: TData) -> Tuple[torch.Tensor, Any]:
-        with _get_timing_context(
+        with get_timing_context(
             state, f"{self.__class__.__name__}.move_data_to_device"
         ):
             data = self.move_data_to_device(state, data, non_blocking=False)
 
         with self.maybe_autocast_precision:
             # users must override this
-            with _get_timing_context(state, f"{self.__class__.__name__}.compute_loss"):
+            with get_timing_context(state, f"{self.__class__.__name__}.compute_loss"):
                 loss, outputs = self.compute_loss(state, data)
 
-        step = get_current_progress(state).num_steps_completed
-        # users can override this, by default this is a no-op
-        with _get_timing_context(state, f"{self.__class__.__name__}.on_eval_step_end"):
-            self.on_eval_step_end(state, data, step, loss, outputs)
+        if state.entry_point == EntryPoint.FIT:
+            step = self.train_progress.num_steps_completed
+        else:
+            step = self.eval_progress.num_steps_completed
+
+        self.on_eval_step_end(state, data, step, loss, outputs)
         return loss, outputs
 
     def on_eval_step_end(
         self, state: State, data: TData, step: int, loss: torch.Tensor, outputs: Any
     ) -> None:
         """
         This will be called at the end of every ``eval_step`` before returning. The user can implement this method with code to update and log their metrics,
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/callback.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,17 @@
     in your `Unit <https://www.internalfb.com/intern/staticdocs/torchtnt/framework/unit.html>`_. To write your own callback,
     subclass the Callback class and add your own code into the hooks.
 
     Below is an example of a basic callback which prints a message at various points during execution.
 
     .. code-block:: python
 
-      from torchtnt.framework import Callback, State, TEvalUnit, TPredictUnit, TTrainUnit
+      from torchtnt.framework.callback import Callback
+      from torchtnt.framework.state import State
+      from torchtnt.framework.unit import TEvalUnit, TPredictUnit, TTrainUnit
 
       class PrintingCallback(Callback):
           def on_train_start(self, state: State, unit: TTrainUnit) -> None:
               print("Starting training")
 
           def on_train_end(self, state: State, unit: TTrainUnit) -> None:
               print("Ending training")
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/__init__.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/base_csv_writer.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/base_csv_writer.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/garbage_collector.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/garbage_collector.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,20 +43,19 @@
 
     def on_train_start(self, state: State, unit: TTrainUnit) -> None:
         gc.disable()
 
     def on_train_step_end(self, state: State, unit: TTrainUnit) -> None:
         gc.collect(generation=1)
 
-        train_state = none_throws(state.train_state)
-        total_num_steps_completed = train_state.progress.num_steps_completed
+        total_num_steps_completed = unit.train_progress.num_steps_completed
         if state.entry_point == EntryPoint.FIT:
             # if fitting, include the num eval steps completed in the total steps completed
             eval_state = none_throws(state.eval_state)
-            total_num_steps_completed += eval_state.progress.num_steps_completed
+            total_num_steps_completed += unit.eval_progress.num_steps_completed
 
         if total_num_steps_completed % self._step_interval == 0:
             gc.collect()
 
     def on_train_end(self, state: State, unit: TTrainUnit) -> None:
         gc.enable()
 
@@ -64,20 +63,18 @@
         if state.entry_point == EntryPoint.FIT:
             # if fitting, this is already handled in on_train_start
             return
         gc.disable()
 
     def on_eval_step_end(self, state: State, unit: TEvalUnit) -> None:
         gc.collect(generation=1)
-        eval_state = none_throws(state.eval_state)
-        total_num_steps_completed = eval_state.progress.num_steps_completed
+        total_num_steps_completed = unit.eval_progress.num_steps_completed
         if state.entry_point == EntryPoint.FIT:
             # if fitting, include the num train steps completed in the total steps completed
-            train_state = none_throws(state.train_state)
-            total_num_steps_completed += train_state.progress.num_steps_completed
+            total_num_steps_completed += unit.train_progress.num_steps_completed
 
         if total_num_steps_completed % self._step_interval == 0:
             gc.collect()
 
     def on_eval_end(self, state: State, unit: TEvalUnit) -> None:
         if state.entry_point == EntryPoint.FIT:
             # if fitting, this will be handled in on_train_end
@@ -85,13 +82,12 @@
         gc.enable()
 
     def on_predict_start(self, state: State, unit: TPredictUnit) -> None:
         gc.disable()
 
     def on_predict_step_end(self, state: State, unit: TPredictUnit) -> None:
         gc.collect(generation=1)
-        predict_state = none_throws(state.predict_state)
-        if predict_state.progress.num_steps_completed % self._step_interval == 0:
+        if unit.predict_progress.num_steps_completed % self._step_interval == 0:
             gc.collect()
 
     def on_predict_end(self, state: State, unit: TPredictUnit) -> None:
         gc.enable()
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/lambda_callback.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/lambda_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,22 +35,22 @@
         on_predict_step_start: function to run when each predict step starts.
         on_predict_step_end: function to run when each predict step ends.
         on_predict_epoch_end: function to run when each predict epoch ends.
         on_predict_end: function to run when predict ends.
 
     Examples::
 
-        from torchtnt.framework import evaluate
         from torchtnt.framework.callbacks import Lambda
+        from torchtnt.framework.evaluate import evaluate
 
         dataloader = MyDataLoader()
         unit = MyUnit()
 
         def print_on_step_start(state, unit) -> None:
-            print(f'starting eval step {state.eval_state.progress.num_steps_completed}')
+            print(f'starting eval step {unit.eval_progress.num_steps_completed}')
 
 
         lambda_cb = Lambda(
             on_eval_start=lambda *args, print('starting eval'),
             on_eval_step_start=print_on_step_start,
         )
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/learning_rate_monitor.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/learning_rate_monitor.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Dict, List, Union
 
-from pyre_extensions import none_throws
-
 from torch.optim.optimizer import Optimizer
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.state import State
 from torchtnt.framework.unit import TTrainUnit
 from torchtnt.utils.loggers.logger import MetricLogger
 
 
@@ -96,25 +94,21 @@
             return
 
         if self.logging_interval != "epoch":
             return
 
         lr_stats = _extract_lr(unit)
 
-        train_state = none_throws(state.train_state)
-
-        step = train_state.progress.num_steps_completed
+        step = unit.train_progress.num_steps_completed
         _write_stats(self._loggers, lr_stats, step)
 
     def on_train_step_start(self, state: State, unit: TTrainUnit) -> None:
         if not self._loggers:
             return
 
         if self.logging_interval != "step":
             return
 
         lr_stats = _extract_lr(unit)
 
-        train_state = none_throws(state.train_state)
-
-        step = train_state.progress.num_steps_completed
+        step = unit.train_progress.num_steps_completed
         _write_stats(self._loggers, lr_stats, step)
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/module_summary.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/module_summary.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,40 +2,34 @@
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Any, Callable, Dict, List, MutableMapping, Optional, Tuple
 
-try:
-    from torcheval.tools import (
-        get_module_summary,
-        get_summary_table,
-        ModuleSummary as ModuleSummaryObj,
-        prune_module_summary,
-    )
-
-    _TORCHEVAL_AVAILABLE = True
-except Exception:
-    _TORCHEVAL_AVAILABLE = False
-
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.state import EntryPoint, State
 from torchtnt.framework.unit import AppStateMixin, TEvalUnit, TPredictUnit, TTrainUnit
+from torchtnt.utils.module_summary import (
+    get_module_summary,
+    get_summary_table,
+    ModuleSummary as ModuleSummaryObj,
+    prune_module_summary,
+)
 from torchtnt.utils.rank_zero_log import rank_zero_info
 
 
 def _log_module_summary_tables(module_summaries: List[ModuleSummaryObj]) -> None:
     for ms in module_summaries:
         rank_zero_info("\n" + get_summary_table(ms))
 
 
 class ModuleSummary(Callback):
     """
-    A callback which generates and logs a summary of the modules using `TorchEval <https://pytorch.org/torcheval/>`_.
+    A callback which generates and logs a summary of the modules.
 
     Args:
         max_depth: The maximum depth of module summaries to keep.
         process_fn: Function to print the module summaries. Default is to log all module summary tables.
         module_inputs: A mapping from module name to (args, kwargs) for that module. Useful when wanting FLOPS, activation sizes, etc.
 
     Raises:
@@ -50,20 +44,14 @@
             [List[ModuleSummaryObj]], None
         ] = _log_module_summary_tables,
         # pyre-ignore
         module_inputs: Optional[
             MutableMapping[str, Tuple[Tuple[Any, ...], Dict[str, Any]]]
         ] = None,
     ) -> None:
-        if not _TORCHEVAL_AVAILABLE:
-            raise RuntimeError(
-                "ModuleSummary support requires torcheval. "
-                "Please make sure ``torcheval`` is installed. "
-                "Installation: https://github.com/pytorch/torcheval#installing-torcheval"
-            )
         self._max_depth = max_depth
         self._process_fn = process_fn
         self._module_inputs = module_inputs
 
     def on_train_start(self, state: State, unit: TTrainUnit) -> None:
         self._get_and_process_summaries(unit)
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/pytorch_profiler.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/pytorch_profiler.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/system_resources_monitor.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/system_resources_monitor.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 import psutil
 import torch
-from pyre_extensions import none_throws
 from torchtnt.framework.callback import Callback
-from torchtnt.framework.state import PhaseState, State
+from torchtnt.framework.state import State
 from torchtnt.framework.unit import TEvalUnit, TPredictUnit, TTrainUnit
 from torchtnt.utils.device import collect_system_stats, get_device_from_env
 from torchtnt.utils.loggers.logger import MetricLogger
 
 
 def _write_stats(
     writers: List[MetricLogger],
@@ -65,36 +64,35 @@
         self._loggers: List[MetricLogger] = loggers
         self.logging_interval = logging_interval
         self.process = psutil.Process()
         self.max_gpu_mem_usage_b: Optional[float] = None
         self.device: torch.device = get_device_from_env()
 
     def write_system_stats(
-        self, logging_interval: Literal["epoch", "step"], state: PhaseState
+        self, logging_interval: Literal["epoch", "step"], step: int
     ) -> None:
         if not self._loggers:
             return
 
         if self.logging_interval != logging_interval:
             return
 
         system_stats = collect_system_stats(self.device)
-        step = state.progress.num_steps_completed
         _write_stats(self._loggers, system_stats, step)
 
     def on_train_epoch_start(self, state: State, unit: TTrainUnit) -> None:
-        self.write_system_stats("epoch", none_throws(state.train_state))
+        self.write_system_stats("epoch", unit.train_progress.num_steps_completed)
 
     def on_train_step_start(self, state: State, unit: TTrainUnit) -> None:
-        self.write_system_stats("step", none_throws(state.train_state))
+        self.write_system_stats("step", unit.train_progress.num_steps_completed)
 
     def on_eval_epoch_start(self, state: State, unit: TEvalUnit) -> None:
-        self.write_system_stats("epoch", none_throws(state.eval_state))
+        self.write_system_stats("epoch", unit.eval_progress.num_steps_completed)
 
     def on_eval_step_start(self, state: State, unit: TEvalUnit) -> None:
-        self.write_system_stats("step", none_throws(state.eval_state))
+        self.write_system_stats("step", unit.eval_progress.num_steps_completed)
 
     def on_predict_epoch_start(self, state: State, unit: TPredictUnit) -> None:
-        self.write_system_stats("epoch", none_throws(state.predict_state))
+        self.write_system_stats("epoch", unit.predict_progress.num_steps_completed)
 
     def on_predict_step_start(self, state: State, unit: TPredictUnit) -> None:
-        self.write_system_stats("step", none_throws(state.predict_state))
+        self.write_system_stats("step", unit.predict_progress.num_steps_completed)
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Dict, Optional, Union
 
 import torch
 
-from pyre_extensions import none_throws
-
 from torch.utils.tensorboard import SummaryWriter
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.state import State
 from torchtnt.framework.unit import TTrainUnit
 from torchtnt.utils.loggers.tensorboard import TensorBoardLogger
 
 
@@ -45,12 +43,10 @@
         self._writer: Optional[SummaryWriter] = logger
 
     def on_train_epoch_end(self, state: State, unit: TTrainUnit) -> None:
         writer = self._writer
         if not writer:
             return
 
-        train_state = none_throws(state.train_state)
-
-        step = train_state.progress.num_steps_completed
+        step = unit.train_progress.num_steps_completed
         modules = unit.tracked_modules()
         _write_histogram_parameters(writer, modules, step)
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/torchsnapshot_saver.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/torchsnapshot_saver.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,40 +2,38 @@
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 import logging
 import os
-from typing import Any, Dict, List, Optional, Set, Union
+import re
+from typing import Any, Dict, List, Optional, Pattern, Set, Union
 
 import torch.distributed as dist
 
 from pyre_extensions import none_throws
 from torchsnapshot.snapshot import PendingSnapshot, Snapshot
 
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.state import EntryPoint, State
-from torchtnt.framework.unit import (
-    _Stateful as StatefulProtocol,
-    AppStateMixin,
-    TEvalUnit,
-    TPredictUnit,
-    TTrainUnit,
-)
-from torchtnt.framework.utils import _construct_tracked_optimizers
-from torchtnt.utils import get_global_rank, rank_zero_info, rank_zero_warn
+from torchtnt.framework.unit import AppStateMixin, TEvalUnit, TPredictUnit, TTrainUnit
+from torchtnt.framework.utils import _construct_tracked_optimizers, get_timing_context
+from torchtnt.utils.distributed import get_global_rank, PGWrapper
+from torchtnt.utils.fsspec import get_filesystem
+from torchtnt.utils.rank_zero_log import rank_zero_info, rank_zero_warn
+from torchtnt.utils.stateful import Stateful
 
 try:
     import torchsnapshot
 
     _TStateful = torchsnapshot.Stateful
     _TORCHSNAPSHOT_AVAILABLE = True
 except Exception:
-    _TStateful = StatefulProtocol
+    _TStateful = Stateful
     _TORCHSNAPSHOT_AVAILABLE = False
 
 _EVAL_PROGRESS_STATE_KEY = "eval_progress"
 _RNG_STATE_KEY = "rng_state"
 _TRAIN_PROGRESS_STATE_KEY = "train_progress"
 _TRAIN_DL_STATE_KEY = "train_dataloader"
 
@@ -55,28 +53,30 @@
 
     Args:
         dirpath: Parent directory to save snapshots to.
         save_every_n_train_steps: Frequency of steps with which to save snapshots during the train epoch. If None, no intra-epoch snapshots are generated.
         save_every_n_epochs: Frequency of epochs with which to save snapshots during training. If None, no end-of-epoch snapshots are generated.
         replicated: A glob-pattern of replicated key names that indicate which application state entries have the same state across all processes.
             For more information, see https://pytorch.org/torchsnapshot/main/api_reference.html#torchsnapshot.Snapshot.take .
+        storage_options: Additional keyword options for the storage plugin to use. See each storage plugin's documentation for customizations.
 
     Note: If torch.distributed is available and default process group is initialized, the constructor will call a collective operation for rank 0 to broadcast the dirpath to all other ranks
 
     Note:
         If checkpointing FSDP model, you can set state_dict type calling `set_state_dict_type <https://pytorch.org/docs/stable/fsdp.html#torch.distributed.fsdp.FullyShardedDataParallel.set_state_dict_type>`_ prior to starting training.
     """
 
     def __init__(
         self,
         dirpath: str,
         *,
         save_every_n_train_steps: Optional[int] = None,
         save_every_n_epochs: Optional[int] = None,
         replicated: Optional[List[str]] = None,
+        storage_options: Optional[Dict[str, Any]] = None,
     ) -> None:
         _validate_snapshot_available()
         if save_every_n_train_steps is not None and save_every_n_train_steps <= 0:
             raise ValueError(
                 f"Invalid value passed for save_every_n_train_steps. Expected to receive either None or positive number, but received {save_every_n_train_steps}"
             )
         if save_every_n_epochs is not None and save_every_n_epochs <= 0:
@@ -85,14 +85,15 @@
             )
         self._save_every_n_epochs = save_every_n_epochs
         self._save_every_n_train_steps = save_every_n_train_steps
         self._sync_dirpath_to_all_ranks(dirpath)
         self._replicated: Set[str] = set(replicated or [])
 
         self._prev_snapshot: Optional[PendingSnapshot] = None
+        self._storage_options = storage_options
 
     def _sync_dirpath_to_all_ranks(self, dirpath: str) -> None:
         if not (dist.is_available() and dist.is_initialized()):
             self._dirpath: str = dirpath
             return
 
         dirpath_container = [dirpath] if get_global_rank() == 0 else [""]
@@ -111,56 +112,60 @@
 
     def on_train_start(self, state: State, unit: TTrainUnit) -> None:
         """Validate there's no key collision for the app state."""
         app_state = _app_state(unit)
         _check_app_state_collision(app_state)
 
     def on_train_step_end(self, state: State, unit: TTrainUnit) -> None:
-        train_progress = none_throws(state.train_state).progress
-
-        num_steps_completed = train_progress.num_steps_completed
+        num_steps_completed = unit.train_progress.num_steps_completed
         save_every_n_train_steps = self._save_every_n_train_steps
         if (
             save_every_n_train_steps is None
             or num_steps_completed % save_every_n_train_steps != 0
         ):
             return
 
         app_state = _get_app_state(state, unit, self._replicated, intra_epoch=True)
-        epoch = train_progress.num_epochs_completed
+        epoch = unit.train_progress.num_epochs_completed
         snapshot_path = _get_snapshot_save_path(
             self._dirpath, epoch, num_steps_completed
         )
-        self._async_snapshot(snapshot_path, app_state, wait=False)
+        with get_timing_context(
+            state, f"{self.__class__.__name__}.take_async_snapshot"
+        ):
+            self._async_snapshot(snapshot_path, app_state, wait=False)
 
     def on_train_epoch_end(self, state: State, unit: TTrainUnit) -> None:
-        train_progress = none_throws(state.train_state).progress
-
-        epoch = train_progress.num_epochs_completed
+        epoch = unit.train_progress.num_epochs_completed
         save_every_n_epochs = self._save_every_n_epochs
         if save_every_n_epochs is None or epoch % save_every_n_epochs != 0:
             return
 
         app_state = _get_app_state(state, unit, self._replicated, intra_epoch=False)
-        num_steps_completed = train_progress.num_steps_completed
+        num_steps_completed = unit.train_progress.num_steps_completed
         snapshot_path = _get_snapshot_save_path(
             self._dirpath, epoch, num_steps_completed
         )
-        self._async_snapshot(snapshot_path, app_state, wait=True)
+        with get_timing_context(
+            state, f"{self.__class__.__name__}.take_async_snapshot"
+        ):
+            self._async_snapshot(snapshot_path, app_state, wait=True)
 
     def on_train_end(self, state: State, unit: TTrainUnit) -> None:
         app_state = _get_app_state(state, unit, self._replicated, intra_epoch=False)
-        train_progress = none_throws(state.train_state).progress
-        num_steps_completed = train_progress.num_steps_completed
-        epoch = train_progress.num_epochs_completed
+        num_steps_completed = unit.train_progress.num_steps_completed
+        epoch = unit.train_progress.num_epochs_completed
         snapshot_path = _get_snapshot_save_path(
             self._dirpath, epoch, num_steps_completed
         )
-        self._async_snapshot(snapshot_path, app_state, wait=True)
-        self._wait()
+        with get_timing_context(
+            state, f"{self.__class__.__name__}.take_async_snapshot"
+        ):
+            self._async_snapshot(snapshot_path, app_state, wait=True)
+            self._wait()
 
     def on_exception(
         self,
         state: State,
         unit: Union[TTrainUnit, TEvalUnit, TPredictUnit],
         exc: BaseException,
     ) -> None:
@@ -186,68 +191,143 @@
                 rank_zero_warn(
                     f"Still writing previous snapshot, will skip this one. Consider increasing 'frequency' (current {self._save_every_n_train_steps})",
                     logger=logger,
                 )
                 return False
 
         self._prev_snapshot = Snapshot.async_take(
-            str(snapshot_path), app_state=app_state, replicated=list(self._replicated)
+            str(snapshot_path),
+            app_state=app_state,
+            replicated=list(self._replicated),
+            storage_options=self._storage_options,
         )
         rank_zero_info(f"Saving snapshot to path: {snapshot_path}", logger=logger)
         return True
 
     @staticmethod
     def restore(
         path: str,
-        state: State,
         unit: AppStateMixin,
         *,
+        train_dataloader: Optional[_TStateful] = None,
         restore_train_progress: bool = True,
-        restore_train_dataloader: bool = True,
         restore_eval_progress: bool = True,
+        storage_options: Optional[Dict[str, Any]] = None,
     ) -> None:
         """Utility method to restore snapshot state from a path.
 
         Since the class also manages saving the progress and dataloader states,
         this method handles their restoration. There are additional flags offered
         should the user want to skip loading these states. By default, the train progress,
         train dataloader, and eval progress are restored, if applicable.
         """
 
         _validate_snapshot_available()
         app_state = _app_state(unit)
         _check_app_state_collision(app_state)
 
-        snapshot = torchsnapshot.Snapshot(path)
-
-        train_state = none_throws(state.train_state)
+        snapshot = torchsnapshot.Snapshot(path, storage_options=storage_options)
 
         rng_state = torchsnapshot.RNGState()
         app_state[_RNG_STATE_KEY] = rng_state
 
-        if restore_train_progress:
-            train_progress = train_state.progress
-            app_state[_TRAIN_PROGRESS_STATE_KEY] = train_progress
+        if not restore_train_progress:
+            del app_state[_TRAIN_PROGRESS_STATE_KEY]
+
+        if not restore_eval_progress:
+            del app_state[_EVAL_PROGRESS_STATE_KEY]
 
-        if restore_train_dataloader:
+        if train_dataloader is not None:
             # request to restore the dataloader state only if
             # the persisted snapshot state includes the dataloader entry
             manifest = snapshot.get_manifest()
             for key in manifest:
                 if _TRAIN_DL_STATE_KEY in key:
-                    app_state[_TRAIN_DL_STATE_KEY] = train_state.dataloader
+                    app_state[_TRAIN_DL_STATE_KEY] = train_dataloader
                     break
 
-        if state.entry_point == EntryPoint.FIT and restore_eval_progress:
-            # include evaluation states if fitting
-            eval_state = none_throws(state.eval_state)
-            app_state[_EVAL_PROGRESS_STATE_KEY] = eval_state.progress
-
         snapshot.restore(app_state)
 
+    @staticmethod
+    def get_latest_checkpoint_path(dirpath: str) -> Optional[str]:
+        """Given a parent directory where checkpoints are saved, return the latest checkpoint subdirectory."""
+
+        ret = None
+        rank = get_global_rank()
+        # Do all filesystem reads from rank 0 only
+        if rank == 0:
+            ret = _latest_checkpoint_path(dirpath)
+
+        # If not running in a distributed setting, return as is
+        if not (dist.is_available() and dist.is_initialized()):
+            return ret
+
+        # Otherwise, broadcast result from rank 0 to all ranks
+        pg = PGWrapper(dist.group.WORLD)
+        path_container = [ret] if rank == 0 else [None]
+        pg.broadcast_object_list(path_container, 0)
+        val = path_container[0]
+        return val
+
+
+def _latest_checkpoint_path(dirpath: str) -> Optional[str]:
+    fs = get_filesystem(dirpath)
+
+    if not fs.exists(dirpath):
+        logger.warning(f"Input dirpath doesn't exist: {dirpath}")
+        return None
+
+    contents = fs.ls(dirpath, detail=True)
+    contents = [item["name"] for item in contents if item["type"] == "directory"]
+    if len(contents) == 0:
+        logger.warning(f"Input dirpath doesn't contain any subdirectories: {dirpath}")
+        return None
+
+    # Define the regex pattern to match the directory names
+    pattern = rf"^{dirpath}/epoch_\d+_step_\d+"
+    snapshot_dirpath_pattern: Pattern[str] = re.compile(pattern)
+    candidate_dirpaths = list(filter(snapshot_dirpath_pattern.match, contents))
+
+    if len(candidate_dirpaths) == 0:
+        logger.warning(
+            f"No valid checkpoint directories were found in input dirpath: {dirpath}"
+        )
+        return None
+
+    # Initialize variables to store the largest epoch and step numbers
+    largest_subdirectory = None
+    largest_epoch = -1
+    largest_step = -1
+
+    # Iterate through all files and directories in the specified directory
+    for candidate in candidate_dirpaths:
+        # Extract the epoch and step numbers from the directory name
+        dirname = os.path.basename(candidate)
+
+        # dirname will be of the format epoch_N_step_M
+        # where N is the epoch number and M is the step number as integers
+        split = dirname.split("_")
+        if len(split) != 4:
+            raise AssertionError(
+                f"Expected exactly 4 elements for pattern of epoch_N_step_M, but received {split})"
+            )
+
+        epoch_num, step_num = int(split[1]), int(split[3])
+        # Check if the current epoch and step numbers are larger than the largest ones found so far
+        if epoch_num > largest_epoch:
+            largest_epoch = epoch_num
+            largest_step = step_num
+            largest_subdirectory = dirname
+        elif largest_epoch == epoch_num and step_num > largest_step:
+            largest_step = step_num
+            largest_subdirectory = dirname
+
+    # Rejoin with the parent directory path and return the largest subdirectory
+    return os.path.join(dirpath, none_throws(largest_subdirectory))
+
 
 def _validate_snapshot_available() -> None:
     if not _TORCHSNAPSHOT_AVAILABLE:
         raise RuntimeError(
             "TorchSnapshotSaver support requires torchsnapshot. "
             "Please make sure ``torchsnapshot`` is installed. "
             "Installation: https://github.com/pytorch/torchsnapshot#install"
@@ -267,45 +347,38 @@
     return app_state
 
 
 def _get_app_state(
     state: State, unit: AppStateMixin, replicated: Set[str], *, intra_epoch: bool
 ) -> Dict[str, _TStateful]:
     train_state = none_throws(state.train_state)
-
-    train_progress = train_state.progress
     app_state = _app_state(unit)
 
     rng_state = torchsnapshot.RNGState()
     app_state[_RNG_STATE_KEY] = rng_state
-    app_state[_TRAIN_PROGRESS_STATE_KEY] = train_progress
-    train_prog_glob = f"{_TRAIN_PROGRESS_STATE_KEY}/*"
-    replicated.add(train_prog_glob)
 
     # for intra-epoch checkpointing, include dataloader states
     train_dl = train_state.dataloader
     if intra_epoch and isinstance(train_dl, _TStateful):
         app_state[_TRAIN_DL_STATE_KEY] = train_dl
 
-    if state.entry_point == EntryPoint.FIT:
-        # include evaluation states if fitting
-        eval_state = none_throws(state.eval_state)
+    # add progress to replicated
+    train_prog_glob = f"{_TRAIN_PROGRESS_STATE_KEY}/*"
+    replicated.add(train_prog_glob)
 
-        app_state[_EVAL_PROGRESS_STATE_KEY] = eval_state.progress
+    if state.entry_point == EntryPoint.FIT:
         eval_prog_glob = f"{_EVAL_PROGRESS_STATE_KEY}/*"
         replicated.add(eval_prog_glob)
 
     return app_state
 
 
 def _check_app_state_collision(app_state: Dict[str, _TStateful]) -> None:
     keys_to_check = (
-        _TRAIN_PROGRESS_STATE_KEY,
         _TRAIN_DL_STATE_KEY,
         _RNG_STATE_KEY,
-        _EVAL_PROGRESS_STATE_KEY,
     )
     for key in keys_to_check:
         if key in app_state:
             raise RuntimeError(
                 f"Detected collision for key in app state: {key}. TorchSnapshotSaver expects to save and load this key."
             )
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/tqdm_progress_bar.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/tqdm_progress_bar.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,96 +38,90 @@
 
     def on_train_epoch_start(self, state: State, unit: TTrainUnit) -> None:
         train_state = none_throws(state.train_state)
         if get_global_rank() == 0:
             self._train_progress_bar = create_progress_bar(
                 train_state.dataloader,
                 desc="Train Epoch",
-                num_epochs_completed=train_state.progress.num_epochs_completed,
-                num_steps_completed=train_state.progress.num_steps_completed_in_epoch,
+                num_epochs_completed=unit.train_progress.num_epochs_completed,
+                num_steps_completed=unit.train_progress.num_steps_completed_in_epoch,
                 max_steps=train_state.max_steps,
                 max_steps_per_epoch=train_state.max_steps_per_epoch,
             )
 
     def on_train_step_end(self, state: State, unit: TTrainUnit) -> None:
-        train_state = none_throws(state.train_state)
         pbar = self._train_progress_bar
         if pbar is not None:
             update_progress_bar(
                 pbar,
-                train_state.progress.num_steps_completed_in_epoch,
+                unit.train_progress.num_steps_completed_in_epoch,
                 self._refresh_rate,
             )
 
     def on_train_epoch_end(self, state: State, unit: TTrainUnit) -> None:
-        train_state = none_throws(state.train_state)
         pbar = self._train_progress_bar
         if pbar is not None:
             close_progress_bar(
                 pbar,
-                train_state.progress.num_steps_completed_in_epoch,
+                unit.train_progress.num_steps_completed_in_epoch,
                 self._refresh_rate,
             )
 
     def on_eval_epoch_start(self, state: State, unit: TEvalUnit) -> None:
         eval_state = none_throws(state.eval_state)
         if get_global_rank() == 0:
             self._eval_progress_bar = create_progress_bar(
                 eval_state.dataloader,
                 desc="Eval Epoch",
-                num_epochs_completed=eval_state.progress.num_epochs_completed,
-                num_steps_completed=eval_state.progress.num_steps_completed_in_epoch,
+                num_epochs_completed=unit.eval_progress.num_epochs_completed,
+                num_steps_completed=unit.eval_progress.num_steps_completed_in_epoch,
                 max_steps=eval_state.max_steps,
                 max_steps_per_epoch=eval_state.max_steps_per_epoch,
             )
 
     def on_eval_step_end(self, state: State, unit: TEvalUnit) -> None:
-        eval_state = none_throws(state.eval_state)
         pbar = self._eval_progress_bar
         if pbar is not None:
             update_progress_bar(
                 pbar,
-                eval_state.progress.num_steps_completed_in_epoch,
+                unit.eval_progress.num_steps_completed_in_epoch,
                 self._refresh_rate,
             )
 
     def on_eval_epoch_end(self, state: State, unit: TEvalUnit) -> None:
-        eval_state = none_throws(state.eval_state)
         pbar = self._eval_progress_bar
         if pbar is not None and state.eval_state:
             close_progress_bar(
                 pbar,
-                eval_state.progress.num_steps_completed_in_epoch,
+                unit.eval_progress.num_steps_completed_in_epoch,
                 self._refresh_rate,
             )
 
     def on_predict_epoch_start(self, state: State, unit: TPredictUnit) -> None:
         predict_state = none_throws(state.predict_state)
         if get_global_rank() == 0:
             self._predict_progress_bar = create_progress_bar(
                 predict_state.dataloader,
                 desc="Predict Epoch",
-                num_epochs_completed=predict_state.progress.num_epochs_completed,
-                num_steps_completed=predict_state.progress.num_steps_completed,
+                num_epochs_completed=unit.predict_progress.num_epochs_completed,
+                num_steps_completed=unit.predict_progress.num_steps_completed,
                 max_steps=predict_state.max_steps,
                 max_steps_per_epoch=predict_state.max_steps_per_epoch,
             )
 
     def on_predict_step_end(self, state: State, unit: TPredictUnit) -> None:
-        predict_state = none_throws(state.predict_state)
         pbar = self._predict_progress_bar
         if pbar is not None:
             update_progress_bar(
                 pbar,
-                predict_state.progress.num_steps_completed_in_epoch,
+                unit.predict_progress.num_steps_completed_in_epoch,
                 self._refresh_rate,
             )
 
     def on_predict_epoch_end(self, state: State, unit: TPredictUnit) -> None:
-        predict_state = none_throws(state.predict_state)
         pbar = self._predict_progress_bar
         if pbar is not None:
             close_progress_bar(
                 pbar,
-                predict_state.progress.num_steps_completed_in_epoch,
+                unit.predict_progress.num_steps_completed_in_epoch,
                 self._refresh_rate,
             )
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/callbacks/train_progress_monitor.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/callbacks/train_progress_monitor.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,30 +2,29 @@
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import List, Union
 
-from pyre_extensions import none_throws
-
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.state import State
 from torchtnt.framework.unit import TTrainUnit
 from torchtnt.utils.loggers.logger import MetricLogger
+from torchtnt.utils.progress import Progress
 
 
-def _write_training_progress(state: State, loggers: List[MetricLogger]) -> None:
+def _write_training_progress(
+    train_progress: Progress, loggers: List[MetricLogger]
+) -> None:
     if not loggers:
         return
 
-    train_state = none_throws(state.train_state)
-
-    step = train_state.progress.num_steps_completed
-    epoch = train_state.progress.num_epochs_completed
+    step = train_progress.num_steps_completed
+    epoch = train_progress.num_epochs_completed
     for logger in loggers:
         logger.log("Training steps completed vs epochs", step, epoch)
 
 
 class TrainProgressMonitor(Callback):
     """
     A callback which logs training progress in terms of steps vs epochs. This is helpful to visualize when the end of data occurs across epochs, especially for iterable datasets.
@@ -41,11 +40,11 @@
         loggers: Union[MetricLogger, List[MetricLogger]],
     ) -> None:
         if not isinstance(loggers, list):
             loggers = [loggers]
         self._loggers: List[MetricLogger] = loggers
 
     def on_train_start(self, state: State, unit: TTrainUnit) -> None:
-        _write_training_progress(state, self._loggers)
+        _write_training_progress(unit.train_progress, self._loggers)
 
     def on_train_epoch_end(self, state: State, unit: TTrainUnit) -> None:
-        _write_training_progress(state, self._loggers)
+        _write_training_progress(unit.train_progress, self._loggers)
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/evaluate.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/evaluate.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,98 +5,61 @@
 # LICENSE file in the root directory of this source tree.
 
 import logging
 from typing import Iterable, List, Optional
 
 import torch
 from pyre_extensions import none_throws
-from torchtnt.framework import AutoUnit
+from torchtnt.framework._callback_handler import CallbackHandler
 from torchtnt.framework.callback import Callback
 
 from torchtnt.framework.state import ActivePhase, EntryPoint, PhaseState, State
 from torchtnt.framework.unit import TEvalData, TEvalUnit
 from torchtnt.framework.utils import (
-    _get_timing_context,
     _is_epoch_done,
     _reset_module_training_mode,
-    _run_callback_fn,
     _set_module_training_mode,
     _step_requires_iterator,
+    get_timing_context,
     log_api_usage,
 )
-from torchtnt.utils.timer import get_timer_summary, Timer
+from torchtnt.utils.timer import get_timer_summary, TimerProtocol
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-def init_eval_state(
-    *,
-    dataloader: Iterable[TEvalData],
-    max_steps_per_epoch: Optional[int] = None,
-    auto_timing: bool = False,
-) -> State:
-    """
-    ``init_eval_state`` is a helper function that initializes a :class:`~torchtnt.framework.State` object for evaluation. This :class:`~torchtnt.framework.State` object
-    can then be passed to the :func:`~torchtnt.framework.evaluate` entry point.
-
-    Args:
-        dataloader: dataloader to be used during evaluation, which can be *any* iterable, including PyTorch DataLoader, DataLoader2, etc.
-        max_steps_per_epoch: the max number of steps to run per epoch. None means evaluate until the dataloader is exhausted.
-        auto_timing: whether to automatically time the evaluation loop, using the state's timer (enabling auto_timing may degrade performance).
-
-    Returns:
-        An initialized state object containing metadata.
-
-    Below is an example of calling :py:func:`~torchtnt.framework.init_eval_state` and :py:func:`~torchtnt.framework.evaluate` together.
-
-    .. code-block:: python
-
-        from torchtnt.framework import init_eval_state, evaluate
-
-        eval_unit = MyEvalUnit(module=..., optimizer=..., lr_scheduler=...)
-        dataloader = torch.utils.data.DataLoader(...)
-        state = init_eval_state(dataloader=dataloader, max_steps_per_epoch=20)
-        evaluate(state, eval_unit)
-    """
-
-    return State(
-        entry_point=EntryPoint.EVALUATE,
-        eval_state=PhaseState(
-            dataloader=dataloader,
-            max_steps_per_epoch=max_steps_per_epoch,
-        ),
-        timer=None if not auto_timing else Timer(),
-    )
-
-
 def evaluate(
-    state: State,
     eval_unit: TEvalUnit,
+    eval_dataloader: Iterable[TEvalData],
     *,
+    max_steps_per_epoch: Optional[int] = None,
     callbacks: Optional[List[Callback]] = None,
+    timer: Optional[TimerProtocol] = None,
 ) -> None:
     """
-    The ``evaluate`` entry point takes in a :class:`~torchtnt.framework.State` object, a :class:`~torchtnt.framework.EvalUnit` object, and an optional list of :class:`~torchtnt.framework.Callback` s,
-    and runs the evaluation loop. The :class:`~torchtnt.framework.State` object can be initialized with :func:`~torchtnt.framework.init_eval_state`.
+    The ``evaluate`` entry point takes in a :class:`~torchtnt.framework.EvalUnit` object, a train dataloader (any Iterable), optional arguments to modify loop execution,
+    and runs the evaluation loop.
 
     Args:
-        state: a :class:`~torchtnt.framework.State` object containing metadata about the evaluation run.
         eval_unit: an instance of :class:`~torchtnt.framework.EvalUnit` which implements `eval_step`.
-        callbacks: an optional list of callbacks.
+        eval_dataloader: dataloader to be used during evaluation, which can be *any* iterable, including PyTorch DataLoader, DataLoader2, etc.
+        max_steps_per_epoch: the max number of steps to run per epoch. None means evaluate until the dataloader is exhausted.
+        callbacks: an optional list of :class:`~torchtnt.framework.Callback` s.
+        timer: an optional Timer which will be used to time key events (using a Timer with CUDA synchronization may degrade performance).
 
-    Below is an example of calling :py:func:`~torchtnt.framework.init_eval_state` and :py:func:`~torchtnt.framework.evaluate` together.
+
+    Below is an example of calling :py:func:`~torchtnt.framework.evaluate`.
 
     .. code-block:: python
 
-        from torchtnt.framework import init_eval_state, evaluate
+        from torchtnt.framework.evaluate import evaluate
 
         eval_unit = MyEvalUnit(module=..., optimizer=..., lr_scheduler=...)
-        dataloader = torch.utils.data.DataLoader(...)
-        state = init_eval_state(dataloader=dataloader, max_steps_per_epoch=20)
-        evaluate(state, eval_unit)
+        eval_dataloader = torch.utils.data.DataLoader(...)
+        evaluate(eval_unit, eval_dataloader, max_steps_per_epoch=20)
 
     Below is pseudocode of what the :py:func:`~torchtnt.framework.evaluate` entry point does.
 
     .. code-block:: text
 
         set unit's tracked modules to eval mode
         call on_eval_start on unit first and then callbacks
@@ -111,118 +74,110 @@
             except StopIteration:
                 break
         increment epoch counter
         call on_eval_epoch_end on unit first and then callbacks
         call on_eval_end on unit first and then callbacks
     """
     log_api_usage("evaluate")
-    callbacks = callbacks or []
+    callback_handler = CallbackHandler(callbacks or [])
+    state = State(
+        entry_point=EntryPoint.EVALUATE,
+        eval_state=PhaseState(
+            dataloader=eval_dataloader,
+            max_steps_per_epoch=max_steps_per_epoch,
+        ),
+        timer=timer,
+    )
     try:
-        state._entry_point = EntryPoint.EVALUATE
-        _evaluate_impl(state, eval_unit, callbacks)
+        _evaluate_impl(state, eval_unit, callback_handler)
         logger.info("Finished evaluation")
         if state.timer:
             logger.info(get_timer_summary(state.timer))
     except Exception as e:
         # TODO: log for diagnostics
         logger.info(e)
         eval_unit.on_exception(state, e)
-        _run_callback_fn(callbacks, "on_exception", state, eval_unit, e)
+        callback_handler.on_exception(state, eval_unit, e)
         raise e
 
 
 @torch.no_grad()
 def _evaluate_impl(
     state: State,
     eval_unit: TEvalUnit,
-    callbacks: List[Callback],
+    callback_handler: CallbackHandler,
 ) -> None:
     # input validation
     eval_state = none_throws(state.eval_state)
 
     state._active_phase = ActivePhase.EVALUATE
     logger.info(
         f"Started evaluate with max_steps_per_epoch={eval_state.max_steps_per_epoch}"
     )
 
     # Set all modules to eval mode
-    # access modules made available through _AppStateMixin
+    # access modules made available through AppStateMixin
     tracked_modules = eval_unit.tracked_modules()
     prior_module_train_states = _set_module_training_mode(tracked_modules, False)
 
-    with _get_timing_context(state, f"{eval_unit.__class__.__name__}.on_eval_start"):
-        eval_unit.on_eval_start(state)
-    _run_callback_fn(callbacks, "on_eval_start", state, eval_unit)
+    eval_unit.on_eval_start(state)
+    callback_handler.on_eval_start(state, eval_unit)
 
     # Conditionally run this to avoid running this multiple times
     # in the case of resuming from a checkpoint mid-epoch
-    if eval_state.progress.num_steps_completed_in_epoch == 0:
-        with _get_timing_context(
-            state, f"{eval_unit.__class__.__name__}.on_eval_epoch_start"
-        ):
-            eval_unit.on_eval_epoch_start(state)
-        _run_callback_fn(callbacks, "on_eval_epoch_start", state, eval_unit)
+    if eval_unit.eval_progress.num_steps_completed_in_epoch == 0:
+        eval_unit.on_eval_epoch_start(state)
+        callback_handler.on_eval_epoch_start(state, eval_unit)
 
-    with _get_timing_context(state, "evaluate.iter(dataloader)"):
+    with get_timing_context(state, "evaluate.iter(dataloader)"):
         data_iter = iter(eval_state.dataloader)
     step_input = data_iter
 
     pass_data_iter_to_step = _step_requires_iterator(eval_unit.eval_step)
-    is_auto_unit = isinstance(eval_unit, AutoUnit)
-    prev_steps_in_epoch = eval_state.progress.num_steps_completed_in_epoch
+    prev_steps_in_epoch = eval_unit.eval_progress.num_steps_completed_in_epoch
 
     while not (
         state.should_stop
         or _is_epoch_done(
-            eval_state.progress, eval_state.max_steps_per_epoch, eval_state.max_steps
+            eval_unit.eval_progress,
+            eval_state.max_steps_per_epoch,
+            eval_state.max_steps,
         )
     ):
         try:
             if not pass_data_iter_to_step:
                 # get the next batch from the data iterator
-                with _get_timing_context(state, "evaluate.next(data_iter)"):
+                with get_timing_context(state, "evaluate.next(data_iter)"):
                     step_input = next(data_iter)
-            _run_callback_fn(callbacks, "on_eval_step_start", state, eval_unit)
-            with _get_timing_context(
-                state,
-                f"{eval_unit.__class__.__name__}.eval_step",
-                skip_timer=is_auto_unit,
-                # skip timer if eval_unit is a subclass of AutoUnit because we have additional timing in the AutoUnit and all timing should be mutually exclusive
-            ):
-                eval_state._step_output = eval_unit.eval_step(state, step_input)
-
-            eval_state.progress.increment_step()
-            _run_callback_fn(
-                callbacks,
-                "on_eval_step_end",
-                state,
-                eval_unit,
-            )
+
+            callback_handler.on_eval_step_start(state, eval_unit)
+            eval_state._step_output = eval_unit.eval_step(state, step_input)
+
+            eval_unit.eval_progress.increment_step()
+            callback_handler.on_eval_step_end(state, eval_unit)
+
             # clear step_output to avoid retaining extra memory
             eval_state._step_output = None
         except StopIteration:
             break
 
     # Possibly warn about an empty dataloader
     any_steps_completed = (
-        abs(eval_state.progress.num_steps_completed_in_epoch - prev_steps_in_epoch) > 0
+        abs(eval_unit.eval_progress.num_steps_completed_in_epoch - prev_steps_in_epoch)
+        > 0
     )
     if not any_steps_completed:
         logger.warning("No steps completed during evaluate epoch!")
 
     # set progress counters for the next epoch
-    eval_state.progress.increment_epoch()
+    eval_unit.eval_progress.increment_epoch()
 
-    with _get_timing_context(
-        state, f"{eval_unit.__class__.__name__}.on_eval_epoch_end"
-    ):
-        eval_unit.on_eval_epoch_end(state)
-    _run_callback_fn(callbacks, "on_eval_epoch_end", state, eval_unit)
+    eval_unit.on_eval_epoch_end(state)
+    callback_handler.on_eval_epoch_end(state, eval_unit)
 
-    with _get_timing_context(state, f"{eval_unit.__class__.__name__}.on_eval_end"):
-        eval_unit.on_eval_end(state)
-    _run_callback_fn(callbacks, "on_eval_end", state, eval_unit)
+    eval_unit.on_eval_end(state)
+    callback_handler.on_eval_end(state, eval_unit)
 
     # Reset training mode for modules at the end of the epoch
     # This ensures that side-effects made by the loop are reset before
     # returning back to the user
     _reset_module_training_mode(tracked_modules, prior_module_train_states)
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/fit.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/train.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,195 +3,257 @@
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 import logging
 from typing import Iterable, List, Optional
 
+import torch
 from pyre_extensions import none_throws
+from torchtnt.framework._callback_handler import CallbackHandler
 from torchtnt.framework.callback import Callback
-from torchtnt.framework.state import EntryPoint, PhaseState, State
-from torchtnt.framework.train import _train_epoch_impl
-from torchtnt.framework.unit import (
-    EvalUnit,
-    TEvalData,
-    TrainUnit,
-    TTrainData,
-    TTrainUnit,
-)
+from torchtnt.framework.evaluate import _evaluate_impl
+from torchtnt.framework.state import ActivePhase, EntryPoint, PhaseState, State
+from torchtnt.framework.unit import TTrainData, TTrainUnit
 from torchtnt.framework.utils import (
-    _get_timing_context,
     _is_done,
-    _run_callback_fn,
+    _is_epoch_done,
+    _maybe_set_distributed_sampler_epoch,
+    _reset_module_training_mode,
+    _set_module_training_mode,
+    _step_requires_iterator,
+    get_timing_context,
     log_api_usage,
 )
-from torchtnt.utils.timer import get_timer_summary, Timer
+from torchtnt.utils.timer import get_timer_summary, TimerProtocol
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-def init_fit_state(
+@torch.enable_grad()
+def train(
+    train_unit: TTrainUnit,
     train_dataloader: Iterable[TTrainData],
-    eval_dataloader: Iterable[TEvalData],
+    *,
     max_epochs: Optional[int] = None,
     max_steps: Optional[int] = None,
-    max_train_steps_per_epoch: Optional[int] = None,
-    max_eval_steps_per_epoch: Optional[int] = None,
-    evaluate_every_n_steps: Optional[int] = None,
-    evaluate_every_n_epochs: Optional[int] = 1,
-    auto_timing: bool = False,
-) -> State:
-    """
-    ``init_fit_state`` is a helper function that initializes a :class:`~torchtnt.framework.State` object for fitting. This :class:`~torchtnt.framework.State` object
-    can then be passed to the :func:`~torchtnt.framework.fit` entry point.
-
-    Args:
-        train_dataloader: dataloader to be used during training, which can be *any* iterable, including PyTorch DataLoader, DataLoader2, etc.
-        eval_dataloader: dataloader to be used during evaluation, which can be *any* iterable, including PyTorch DataLoader, DataLoader2, etc.
-        max_epochs: the max number of epochs to run for training. ``None`` means no limit (infinite training) unless stopped by max_steps.
-        max_steps: the max number of steps to run for training. ``None`` means no limit (infinite training) unless stopped by max_epochs.
-        max_train_steps_per_epoch: the max number of steps to run per epoch for training. None means train until ``train_dataloader`` is exhausted.
-        max_eval_steps_per_epoch: the max number of steps to run per epoch for evaluation. None means evaluate until ``eval_dataloader`` is exhausted.
-        evaluate_every_n_steps: how often to run the evaluation loop in terms of training steps.
-        evaluate_every_n_epochs: how often to run the evaluation loop in terms of training epochs.
-        auto_timing: whether to automatically time the training and evaluation loop, using the state's timer (enabling auto_timing may degrade performance).
-
-    Returns:
-        An initialized state object containing metadata.
-
-    Below is an example of calling :py:func:`~torchtnt.framework.init_fit_state` and :py:func:`~torchtnt.framework.fit` together.
-
-    .. code-block:: python
-
-        from torchtnt.framework import fit, init_fit_state
-
-        fit_unit = MyFitUnit(module=..., optimizer=..., lr_scheduler=...)
-        train_dataloader = torch.utils.data.DataLoader(...)
-        eval_dataloader = torch.utils.data.DataLoader(...)
-        state = init_fit_state(train_dataloader=train_dataloader, eval_dataloader=eval_dataloader, max_epochs=4)
-        fit(state, fit_unit)
-    """
-
-    return State(
-        entry_point=EntryPoint.FIT,
-        train_state=PhaseState(
-            dataloader=train_dataloader,
-            max_epochs=max_epochs,
-            max_steps=max_steps,
-            max_steps_per_epoch=max_train_steps_per_epoch,
-        ),
-        eval_state=PhaseState(
-            dataloader=eval_dataloader,
-            max_steps_per_epoch=max_eval_steps_per_epoch,
-            evaluate_every_n_steps=evaluate_every_n_steps,
-            evaluate_every_n_epochs=evaluate_every_n_epochs,
-        ),
-        timer=None if not auto_timing else Timer(),
-    )
-
-
-def fit(
-    state: State,
-    unit: TTrainUnit,
-    *,
+    max_steps_per_epoch: Optional[int] = None,
     callbacks: Optional[List[Callback]] = None,
+    timer: Optional[TimerProtocol] = None,
 ) -> None:
     """
-    The ``fit`` entry point interleaves training and evaluation loops.  It takes in a :class:`~torchtnt.framework.State` object, an object which subclasses both :class:`~torchtnt.framework.TrainUnit` and :class:`~torchtnt.framework.EvalUnit`,
-    and an optional list of :class:`~torchtnt.framework.Callback` s, and runs the fit loop. The :class:`~torchtnt.framework.State` object can be initialized with :func:`~torchtnt.framework.init_fit_state`.
+    The ``train`` entry point takes in a :class:`~torchtnt.framework.TrainUnit` object, a train dataloader (any Iterable), optional arguments to modify loop execution,
+    and runs the training loop.
 
     Args:
-        state: a :class:`~torchtnt.framework.State` object containing metadata about the fitting run.
-         :func:`~torchtnt.framework.init_fit_state` can be used to initialize a state object.
-        unit: an instance that subclasses both :class:`~torchtnt.framework.unit.TrainUnit` and :class:`~torchtnt.framework.unit.EvalUnit`,
-         implementing :meth:`~torchtnt.framework.TrainUnit.train_step` and :meth:`~torchtnt.framework.EvalUnit.eval_step`.
-        callbacks: an optional list of callbacks.
+        train_unit: an instance of :class:`~torchtnt.framework.TrainUnit` which implements `train_step`.
+        train_dataloader: dataloader to be used during training, which can be *any* iterable, including PyTorch DataLoader, DataLoader2, etc.
+        max_epochs: the max number of epochs to run. ``None`` means no limit (infinite training) unless stopped by max_steps.
+        max_steps: the max number of steps to run. ``None`` means no limit (infinite training) unless stopped by max_epochs.
+        max_steps_per_epoch: the max number of steps to run per epoch. None means train until the dataloader is exhausted.
+        callbacks: an optional list of :class:`~torchtnt.framework.Callback` s.
+        timer: an optional Timer which will be used to time key events (using a Timer with CUDA synchronization may degrade performance).
+
 
-    Below is an example of calling :py:func:`~torchtnt.framework.init_fit_state` and :py:func:`~torchtnt.framework.fit` together.
+    Below is an example of calling :py:func:`~torchtnt.framework.train`.
 
     .. code-block:: python
 
-        from torchtnt.framework import fit, init_fit_state
+        from torchtnt.framework.train import train
 
-        fit_unit = MyFitUnit(module=..., optimizer=..., lr_scheduler=...)
+        train_unit = MyTrainUnit(module=..., optimizer=..., lr_scheduler=...)
         train_dataloader = torch.utils.data.DataLoader(...)
-        eval_dataloader = torch.utils.data.DataLoader(...)
-        state = init_fit_state(train_dataloader=train_dataloader, eval_dataloader=eval_dataloader, max_epochs=4)
-        fit(state, fit_unit)
+        train(train_unit, train_dataloader, max_epochs=4)
 
-    Below is pseudocode of what the :py:func:`~torchtnt.framework.fit` entry point does.
+    Below is pseudocode of what the :py:func:`~torchtnt.framework.train` entry point does.
 
     .. code-block:: text
 
         set unit's tracked modules to train mode
         call on_train_start on unit first and then callbacks
         while training is not done:
             while epoch is not done:
                 call on_train_epoch_start on unit first and then callbacks
                 try:
                     data = next(dataloader)
                     call on_train_step_start on callbacks
                     call train_step on unit
                     increment step counter
                     call on_train_step_end on callbacks
-                    if should evaluate after this step:
-                        run eval loops
                 except StopIteration:
                     break
             increment epoch counter
             call on_train_epoch_end on unit first and then callbacks
-            if should evaluate after this epoch:
-                run eval loop
         call on_train_end on unit first and then callbacks
     """
-    log_api_usage("fit")
-    callbacks = callbacks or []
-
+    log_api_usage("train")
+    callback_handler = CallbackHandler(callbacks or [])
+    state = State(
+        entry_point=EntryPoint.TRAIN,
+        train_state=PhaseState(
+            dataloader=train_dataloader,
+            max_epochs=max_epochs,
+            max_steps=max_steps,
+            max_steps_per_epoch=max_steps_per_epoch,
+        ),
+        timer=timer,
+    )
     try:
-        state._entry_point = EntryPoint.FIT
-        _fit_impl(state, unit, callbacks)
+        _train_impl(state, train_unit, callback_handler)
+        logger.info("Finished train")
         if state.timer:
             logger.info(get_timer_summary(state.timer))
     except Exception as e:
         # TODO: log for diagnostics
-        logger.info(e)
-        unit.on_exception(state, e)
-        _run_callback_fn(callbacks, "on_exception", state, unit, e)
+        logger.info(f"Exception during train\n: {e}")
+        train_unit.on_exception(state, e)
+        callback_handler.on_exception(state, train_unit, e)
         raise e
 
 
-def _fit_impl(
+def _train_impl(
     state: State,
-    unit: TTrainUnit,
-    callbacks: List[Callback],
+    train_unit: TTrainUnit,
+    callback_handler: CallbackHandler,
 ) -> None:
-    # input validation
-    if not isinstance(unit, TrainUnit):
-        raise TypeError("Expected unit to implement TrainUnit interface.")
-    if not isinstance(unit, EvalUnit):
-        raise TypeError("Expected unit to implement EvalUnit interface.")
-
     train_state = none_throws(state.train_state)
-    eval_state = none_throws(state.eval_state)
 
     logger.info(
-        f"Started fit with max_epochs={train_state.max_epochs} "
-        f"max_steps={train_state.max_steps} "
-        f"max_train_steps_per_epoch={train_state.max_steps_per_epoch} "
-        f"max_eval_steps_per_epoch={eval_state.max_steps_per_epoch} "
-        f"evaluate_every_n_steps={eval_state.evaluate_every_n_steps} "
-        f"evaluate_every_n_epochs={eval_state.evaluate_every_n_epochs} "
+        f"Started train with max_epochs={train_state.max_epochs}, max_steps={train_state.max_steps}, max_steps_per_epoch={train_state.max_steps_per_epoch}"
     )
+    if train_state.max_epochs is None and train_state.max_steps is None:
+        logger.warning(
+            "Will run infinite training, since both max_epochs and max_steps were not set."
+        )
+    state._active_phase = ActivePhase.TRAIN
+
+    # Set all modules to train() mode
+    # access modules made available through AppStateMixin
+    tracked_modules = train_unit.tracked_modules()
+    prior_module_train_states = _set_module_training_mode(tracked_modules, True)
 
-    with _get_timing_context(state, f"{unit.__class__.__name__}.on_train_start"):
-        unit.on_train_start(state)
-    _run_callback_fn(callbacks, "on_train_start", state, unit)
+    train_unit.on_train_start(state)
+    callback_handler.on_train_start(state, train_unit)
 
     while not (
         state.should_stop
-        or _is_done(train_state.progress, train_state.max_epochs, train_state.max_steps)
+        or _is_done(
+            train_unit.train_progress, train_state.max_epochs, train_state.max_steps
+        )
+    ):
+        _train_epoch_impl(state, train_unit, callback_handler)
+
+    train_unit.on_train_end(state)
+    callback_handler.on_train_end(state, train_unit)
+
+    # Reset training mode for modules at the end of the epoch
+    # This ensures that side-effects made by the loop are reset before
+    # returning back to the user
+    _reset_module_training_mode(tracked_modules, prior_module_train_states)
+
+
+def _train_epoch_impl(
+    state: State,
+    train_unit: TTrainUnit,
+    callback_handler: CallbackHandler,
+) -> None:
+    logger.info("Started train epoch")
+    state._active_phase = ActivePhase.TRAIN
+
+    train_state = none_throws(state.train_state)
+
+    evaluate_every_n_steps = None
+    evaluate_every_n_epochs = None
+    if state.eval_state:
+        if state.eval_state.evaluate_every_n_steps:
+            evaluate_every_n_steps = state.eval_state.evaluate_every_n_steps
+        if state.eval_state.evaluate_every_n_epochs:
+            evaluate_every_n_epochs = state.eval_state.evaluate_every_n_epochs
+
+    # Check the progress to conditionally run this
+    # to avoid running this multiple times
+    # in the case of resuming from a checkpoint mid-epoch
+    if train_unit.train_progress.num_steps_completed_in_epoch == 0:
+        train_unit.on_train_epoch_start(state)
+        callback_handler.on_train_epoch_start(state, train_unit)
+
+    _maybe_set_distributed_sampler_epoch(
+        train_state.dataloader, train_unit.train_progress.num_epochs_completed
+    )
+
+    with get_timing_context(state, "train.iter(dataloader)"):
+        data_iter = iter(train_state.dataloader)
+    step_input = data_iter
+
+    pass_data_iter_to_step = _step_requires_iterator(train_unit.train_step)
+    prev_steps_in_epoch = train_unit.train_progress.num_steps_completed_in_epoch
+
+    while not (
+        state.should_stop
+        or _is_epoch_done(
+            train_unit.train_progress,
+            train_state.max_steps_per_epoch,
+            train_state.max_steps,
+        )
+    ):
+        try:
+            if not pass_data_iter_to_step:
+                # get the next batch from the data iterator
+                with get_timing_context(state, "train.next(data_iter)"):
+                    step_input = next(data_iter)
+
+            callback_handler.on_train_step_start(state, train_unit)
+            train_state._step_output = train_unit.train_step(state, step_input)
+            train_unit.train_progress.increment_step()
+            callback_handler.on_train_step_end(state, train_unit)
+
+            # clear step_output to avoid retaining extra memory
+            train_state._step_output = None
+
+            if (
+                evaluate_every_n_steps
+                and train_unit.train_progress.num_steps_completed
+                % evaluate_every_n_steps
+                == 0
+            ):
+                _evaluate_impl(
+                    state,
+                    # pyre-ignore: Incompatible parameter type [6]
+                    train_unit,
+                    callback_handler,
+                )
+                logger.info("Finished evaluation. Resuming training epoch")
+                state._active_phase = ActivePhase.TRAIN
+
+        except StopIteration:
+            break
+
+    # Possibly warn about an empty dataloader
+    any_steps_completed = (
+        abs(
+            train_unit.train_progress.num_steps_completed_in_epoch - prev_steps_in_epoch
+        )
+        > 0
+    )
+    if not any_steps_completed:
+        logger.warning("No steps completed during train epoch!")
+
+    # set progress counters for the next epoch
+    train_unit.train_progress.increment_epoch()
+
+    train_unit.on_train_epoch_end(state)
+    callback_handler.on_train_epoch_end(state, train_unit)
+
+    if (
+        evaluate_every_n_epochs
+        and train_unit.train_progress.num_epochs_completed % evaluate_every_n_epochs
+        == 0
     ):
-        _train_epoch_impl(state, unit, callbacks)
+        _evaluate_impl(
+            state,
+            # pyre-ignore: Incompatible parameter type [6]
+            train_unit,
+            callback_handler,
+        )
+        state._active_phase = ActivePhase.TRAIN
 
-    with _get_timing_context(state, f"{unit.__class__.__name__}.on_train_end"):
-        unit.on_train_end(state)
-    _run_callback_fn(callbacks, "on_train_end", state, unit)
+    logger.info("Ended train epoch")
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/predict.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/predict.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,99 +5,61 @@
 # LICENSE file in the root directory of this source tree.
 
 import logging
 from typing import Iterable, List, Optional
 
 import torch
 from pyre_extensions import none_throws
-from torchtnt.framework.auto_unit import AutoPredictUnit, AutoUnit
-from torchtnt.framework.callback import Callback
 
+from torchtnt.framework._callback_handler import CallbackHandler
+from torchtnt.framework.callback import Callback
 from torchtnt.framework.state import ActivePhase, EntryPoint, PhaseState, State
 from torchtnt.framework.unit import TPredictData, TPredictUnit
 from torchtnt.framework.utils import (
-    _get_timing_context,
     _is_epoch_done,
     _reset_module_training_mode,
-    _run_callback_fn,
     _set_module_training_mode,
     _step_requires_iterator,
+    get_timing_context,
     log_api_usage,
 )
-from torchtnt.utils.timer import get_timer_summary, Timer
+from torchtnt.utils.timer import get_timer_summary, TimerProtocol
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-def init_predict_state(
-    *,
-    dataloader: Iterable[TPredictData],
-    max_steps_per_epoch: Optional[int] = None,
-    auto_timing: bool = False,
-) -> State:
-    """
-    ``init_predict_state`` is a helper function that initializes a :class:`~torchtnt.framework.State` object for prediction. This :class:`~torchtnt.framework.State` object
-    can then be passed to the :func:`~torchtnt.framework.predict` entry point.
-
-    Args:
-        dataloader: dataloader to be used during prediction, which can be *any* iterable, including PyTorch DataLoader, DataLoader2, etc.
-        max_steps_per_epoch: the max number of steps to run per epoch. None means predict until the dataloader is exhausted.
-        auto_timing: whether to automatically time the prediction loop, using the state's timer (enabling auto_timing may degrade performance).
-
-    Returns:
-        An initialized state object containing metadata.
-
-    Below is an example of calling :py:func:`~torchtnt.framework.init_predict_state` and :py:func:`~torchtnt.framework.predict` together.
-
-    .. code-block:: python
-
-        from torchtnt.framework import init_predict_state, predict
-
-        predict_unit = MyPredictUnit(module=..., optimizer=..., lr_scheduler=...)
-        dataloader = torch.utils.data.DataLoader(...)
-        state = init_predict_state(dataloader=dataloader, max_steps_per_epoch=20)
-        predict(state, predict_unit)
-
-    """
-
-    return State(
-        entry_point=EntryPoint.PREDICT,
-        predict_state=PhaseState(
-            dataloader=dataloader,
-            max_steps_per_epoch=max_steps_per_epoch,
-        ),
-        timer=None if not auto_timing else Timer(),
-    )
-
-
 def predict(
-    state: State,
     predict_unit: TPredictUnit,
+    predict_dataloader: Iterable[TPredictData],
     *,
+    max_steps_per_epoch: Optional[int] = None,
     callbacks: Optional[List[Callback]] = None,
+    timer: Optional[TimerProtocol] = None,
 ) -> None:
     """
-    The ``predict`` entry point takes in a :class:`~torchtnt.framework.State` object, a :class:`~torchtnt.framework.PredictUnit` object, and an optional list of :class:`~torchtnt.framework.Callback` s,
-    and runs the prediction loop. The :class:`~torchtnt.framework.State` object can be initialized with :func:`~torchtnt.framework.init_predict_state`.
+    The ``predict`` entry point takes in a :class:`~torchtnt.framework.PredictUnit` object, a train dataloader (any Iterable), optional arguments to modify loop execution,
+    and runs the prediction loop.
 
     Args:
-        state: a State object containing metadata about the prediction run. This can be initialized using :func:`~torchtnt.framework.init_predict_state`.
         predict_unit: an instance of :class:`~torchtnt.framework.PredictUnit` which implements `predict_step`.
-        callbacks: an optional list of callbacks.
+        predict_dataloader: dataloader to be used during prediction, which can be *any* iterable, including PyTorch DataLoader, DataLoader2, etc.
+        max_steps_per_epoch: the max number of steps to run per epoch. None means predict until the dataloader is exhausted.
+        callbacks: an optional list of :class:`~torchtnt.framework.Callback` s.
+        timer: an optional Timer which will be used to time key events (using a Timer with CUDA synchronization may degrade performance).
+
 
-    Below is an example of calling :py:func:`~torchtnt.framework.init_predict_state` and :py:func:`~torchtnt.framework.predict` together.
+    Below is an example of calling :py:func:`~torchtnt.framework.predict`.
 
     .. code-block:: python
 
-        from torchtnt.framework import init_predict_state, predict
+        from torchtnt.framework.predict import predict
 
         predict_unit = MyPredictUnit(module=..., optimizer=..., lr_scheduler=...)
-        dataloader = torch.utils.data.DataLoader(...)
-        state = init_predict_state(dataloader=dataloader, max_steps_per_epoch=20)
-        predict(state, predict_unit)
+        predict_dataloader = torch.utils.data.DataLoader(...)
+        predict(predict_unit, predict_dataloader, max_steps_per_epoch=20)
 
     Below is pseudocode of what the :py:func:`~torchtnt.framework.predict` entry point does.
 
     .. code-block:: text
 
         set unit's tracked modules to eval mode
         call on_predict_start on unit first and then callbacks
@@ -112,123 +74,119 @@
             except StopIteration:
                 break
         increment epoch counter
         call on_predict_epoch_end on unit first and then callbacks
         call on_predict_end on unit first and then callbacks
     """
     log_api_usage("predict")
-    callbacks = callbacks or []
+    callback_handler = CallbackHandler(callbacks or [])
+    state = State(
+        entry_point=EntryPoint.PREDICT,
+        predict_state=PhaseState(
+            dataloader=predict_dataloader,
+            max_steps_per_epoch=max_steps_per_epoch,
+        ),
+        timer=timer,
+    )
     try:
-        state._entry_point = EntryPoint.PREDICT
-        _predict_impl(state, predict_unit, callbacks)
+        _predict_impl(state, predict_unit, callback_handler)
         logger.info("Finished predict")
         if state.timer:
             logger.info(get_timer_summary(state.timer))
     except Exception as e:
         # TODO: log for diagnostics
         logger.info(e)
         predict_unit.on_exception(state, e)
-        _run_callback_fn(callbacks, "on_exception", state, predict_unit, e)
+        callback_handler.on_exception(state, predict_unit, e)
         raise e
 
 
 @torch.inference_mode()
 def _predict_impl(
     state: State,
     predict_unit: TPredictUnit,
-    callbacks: List[Callback],
+    callback_handler: CallbackHandler,
 ) -> None:
     # input validation
     predict_state = none_throws(state.predict_state)
 
     state._active_phase = ActivePhase.PREDICT
     logger.info(
         f"Started predict with max_steps_per_epoch={predict_state.max_steps_per_epoch}"
     )
 
     # Set all modules to eval mode
-    # access modules made available through _AppStateMixin
+    # access modules made available through AppStateMixin
     tracked_modules = predict_unit.tracked_modules()
     prior_module_train_states = _set_module_training_mode(tracked_modules, False)
 
-    with _get_timing_context(
+    with get_timing_context(
         state, f"{predict_unit.__class__.__name__}.on_predict_start"
     ):
         predict_unit.on_predict_start(state)
-    _run_callback_fn(callbacks, "on_predict_start", state, predict_unit)
+    callback_handler.on_predict_start(state, predict_unit)
 
     # Conditionally run this to avoid running this multiple times
     # in the case of resuming from a checkpoint mid-epoch
-    if predict_state.progress.num_steps_completed_in_epoch == 0:
-        with _get_timing_context(
+    if predict_unit.predict_progress.num_steps_completed_in_epoch == 0:
+        with get_timing_context(
             state, f"{predict_unit.__class__.__name__}.on_predict_epoch_start"
         ):
             predict_unit.on_predict_epoch_start(state)
-        _run_callback_fn(callbacks, "on_predict_epoch_start", state, predict_unit)
+        callback_handler.on_predict_epoch_start(state, predict_unit)
 
-    with _get_timing_context(state, "predict.iter(dataloader)"):
+    with get_timing_context(state, "predict.iter(dataloader)"):
         data_iter = iter(predict_state.dataloader)
     step_input = data_iter
 
     pass_data_iter_to_step = _step_requires_iterator(predict_unit.predict_step)
-    is_auto_unit = isinstance(predict_unit, (AutoUnit, AutoPredictUnit))
-    prev_steps_in_epoch = predict_state.progress.num_steps_completed_in_epoch
+    prev_steps_in_epoch = predict_unit.predict_progress.num_steps_completed_in_epoch
 
     while not (
         state.should_stop
         or _is_epoch_done(
-            predict_state.progress,
+            predict_unit.predict_progress,
             predict_state.max_steps_per_epoch,
             predict_state.max_steps,
         )
     ):
         try:
             if not pass_data_iter_to_step:
                 # get the next batch from the data iterator
-                with _get_timing_context(state, "predict.next(data_iter)"):
+                with get_timing_context(state, "predict.next(data_iter)"):
                     step_input = next(data_iter)
 
-            _run_callback_fn(callbacks, "on_predict_step_start", state, predict_unit)
-            with _get_timing_context(
-                state,
-                f"{predict_unit.__class__.__name__}.predict_step",
-                skip_timer=is_auto_unit,
-                # skip timer if predict_unit is a subclass of AutoUnit because we have additional timing in the AutoUnit and all timing should be mutually exclusive
-            ):
-                predict_state._step_output = predict_unit.predict_step(
-                    state, step_input
-                )
-            predict_state.progress.increment_step()
-            _run_callback_fn(callbacks, "on_predict_step_end", state, predict_unit)
+            callback_handler.on_predict_step_start(state, predict_unit)
+            predict_state._step_output = predict_unit.predict_step(state, step_input)
+
+            predict_unit.predict_progress.increment_step()
+            callback_handler.on_predict_step_end(state, predict_unit)
 
             # clear step_output to avoid retaining extra memory
             predict_state._step_output = None
         except StopIteration:
             break
 
     # Possibly warn about an empty dataloader
     any_steps_completed = (
-        abs(predict_state.progress.num_steps_completed_in_epoch - prev_steps_in_epoch)
+        abs(
+            predict_unit.predict_progress.num_steps_completed_in_epoch
+            - prev_steps_in_epoch
+        )
         > 0
     )
     if not any_steps_completed:
         logger.warning("No steps completed during predict epoch!")
 
     # set progress counters for the next epoch
-    predict_state.progress.increment_epoch()
+    predict_unit.predict_progress.increment_epoch()
 
-    with _get_timing_context(
-        state, f"{predict_unit.__class__.__name__}.on_predict_epoch_end"
-    ):
-        predict_unit.on_predict_epoch_end(state)
-    _run_callback_fn(callbacks, "on_predict_epoch_end", state, predict_unit)
+    predict_unit.on_predict_epoch_end(state)
+    callback_handler.on_predict_epoch_end(state, predict_unit)
 
-    with _get_timing_context(
-        state, f"{predict_unit.__class__.__name__}.on_predict_end"
-    ):
-        predict_unit.on_predict_end(state)
-    _run_callback_fn(callbacks, "on_predict_end", state, predict_unit)
+    predict_unit.on_predict_end(state)
+    callback_handler.on_predict_end(state, predict_unit)
 
     # Reset training mode for modules at the end of the epoch
     # This ensures that side-effects made by the loop are reset before
     # returning back to the user
     _reset_module_training_mode(tracked_modules, prior_module_train_states)
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/state.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/state.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 # pyre-ignore-all-errors[3]
 # pyre-ignore-all-errors[4]
 
 import logging
 from enum import auto, Enum
 from typing import Any, Iterable, Optional
 
-from torchtnt.utils.progress import Progress
-from torchtnt.utils.timer import Timer
+from torchtnt.utils.timer import TimerProtocol
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 def _check_loop_condition(name: str, val: Optional[int]) -> None:
     if val is not None and val < 0:
         raise ValueError(
@@ -65,48 +64,41 @@
     Modified by the framework, read-only for the user.
     """
 
     def __init__(
         self,
         *,
         dataloader: Iterable[Any],
-        progress: Optional[Progress] = None,
         max_epochs: Optional[int] = None,  # used only for train
         max_steps: Optional[int] = None,  # used only for train
         max_steps_per_epoch: Optional[int] = None,
         evaluate_every_n_steps: Optional[int] = None,  # used only for evaluate
         evaluate_every_n_epochs: Optional[int] = None,  # used only for evaluate
     ) -> None:
         _check_loop_condition("max_epochs", max_epochs)
         _check_loop_condition("max_steps", max_steps)
         _check_loop_condition("max_steps_per_epoch", max_steps_per_epoch)
         _check_loop_condition("evaluate_every_n_steps", evaluate_every_n_steps)
         _check_loop_condition("evaluate_every_n_epochs", evaluate_every_n_epochs)
 
         self._dataloader: Iterable[Any] = dataloader
-        self._progress: Progress = progress or Progress()
         self._max_epochs = max_epochs
         self._max_steps = max_steps
         self._max_steps_per_epoch = max_steps_per_epoch
         self._evaluate_every_n_steps = evaluate_every_n_steps
         self._evaluate_every_n_epochs = evaluate_every_n_epochs
 
         self._step_output: Any = None
 
     @property
     def dataloader(self) -> Iterable[Any]:
         """Dataloader defined by the user."""
         return self._dataloader
 
     @property
-    def progress(self) -> Progress:
-        """An instance of :class:`~torchtnt.framework.Progress` which contains information about the current progress of the loop."""
-        return self._progress
-
-    @property
     def max_epochs(self) -> Optional[int]:
         """Maximum number of epochs to train, defined by the user."""
         return self._max_epochs
 
     @property
     def max_steps(self) -> Optional[int]:
         """Maximum number of steps to train, defined by the user."""
@@ -138,15 +130,15 @@
     Modified by the framework, read-only for the user.
     """
 
     def __init__(
         self,
         *,
         entry_point: EntryPoint,
-        timer: Optional[Timer] = None,
+        timer: Optional[TimerProtocol] = None,
         train_state: Optional[PhaseState] = None,
         eval_state: Optional[PhaseState] = None,
         predict_state: Optional[PhaseState] = None,
     ) -> None:
         self._entry_point = entry_point
         self._timer = timer
         self._train_state = train_state
@@ -162,16 +154,16 @@
 
     @property
     def active_phase(self) -> ActivePhase:
         """Current active phase of the loop. (One of TRAIN, EVALUATE, PREDICT)."""
         return self._active_phase
 
     @property
-    def timer(self) -> Optional[Timer]:
-        """A :class:`~torchtnt.framework.Timer` object which can be used for debugging to record latencies of key events during loop execution."""
+    def timer(self) -> Optional[TimerProtocol]:
+        """A :class:`~torchtnt.utils.TimerProtocol` object which can be used for debugging to record latencies of key events during loop execution."""
         return self._timer
 
     @property
     def train_state(self) -> Optional[PhaseState]:
         """A :class:`~torchtnt.framework.PhaseState` object which contains meta information about the train phase."""
         return self._train_state
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/unit.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/unit.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,31 +10,23 @@
 
 from abc import ABC, abstractmethod
 from typing import Any, Dict, Generic, TypeVar
 
 import torch
 
 from torchtnt.framework.state import State
-from torchtnt.utils import TLRScheduler
-from typing_extensions import Protocol, runtime_checkable
+from torchtnt.utils.lr_scheduler import TLRScheduler
+from torchtnt.utils.progress import Progress
+from torchtnt.utils.stateful import Stateful
 
 """
 This file defines mixins and interfaces for users to customize hooks in training, evaluation, and prediction loops.
 """
 
 
-@runtime_checkable
-class _Stateful(Protocol):
-    def state_dict(self) -> Dict[str, Any]:
-        ...
-
-    def load_state_dict(self, state_dict: Dict[str, Any]) -> None:
-        ...
-
-
 def _remove_from_dicts(name_to_remove: str, *dicts: Dict[str, Any]) -> None:
     for d in dicts:
         if name_to_remove in d:
             del d[name_to_remove]
 
 
 class AppStateMixin:
@@ -44,28 +36,30 @@
     The logic here is adapted from torch.nn.Module's handling to register states for buffers, parameters, and modules.
     """
 
     def __init__(self) -> None:
         self._modules: Dict[str, torch.nn.Module] = {}
         self._optimizers: Dict[str, torch.optim.Optimizer] = {}
         self._lr_schedulers: Dict[str, TLRScheduler] = {}
+        self._progress: Dict[str, Progress] = {}
         # catch-all for miscellaneous statefuls
         self._misc_statefuls: Dict[str, Any] = {}
         # TODO: include other known statefuls
 
     def app_state(self) -> Dict[str, Any]:
         """Join together all of the tracked stateful entities to simplify registration of snapshottable states"""
         # TODO: refine with Stateful typehint
         # TODO: Should we split this into app_state_to_load and app_state_to_save
         # in order to let users customize the saving & loading paths independently?
         # or should we assume this is done outside of the loop framework entirely?
         app_state = {
             **self.tracked_modules(),
             **self.tracked_optimizers(),
             **self.tracked_lr_schedulers(),
+            **self.tracked_progress(),
             **self.tracked_misc_statefuls(),
         }
         return app_state
 
     def tracked_modules(self) -> Dict[str, torch.nn.Module]:
         return self._modules
 
@@ -73,14 +67,17 @@
         return self._optimizers
 
     def tracked_lr_schedulers(
         self,
     ) -> Dict[str, TLRScheduler]:
         return self._lr_schedulers
 
+    def tracked_progress(self) -> Dict[str, Progress]:
+        return self._progress
+
     def tracked_misc_statefuls(self) -> Dict[str, Any]:
         return self._misc_statefuls
 
     def __getattr__(self, name: str) -> Any:
         if "_modules" in self.__dict__:
             _modules = self.__dict__["_modules"]
             if name in _modules:
@@ -89,14 +86,18 @@
             _optimizers = self.__dict__["_optimizers"]
             if name in _optimizers:
                 return _optimizers[name]
         if "_lr_schedulers" in self.__dict__:
             _lr_schedulers = self.__dict__["_lr_schedulers"]
             if name in _lr_schedulers:
                 return _lr_schedulers[name]
+        if "_progress" in self.__dict__:
+            _progress = self.__dict__["_progress"]
+            if name in _progress:
+                return _progress[name]
         if "_misc_statefuls" in self.__dict__:
             _misc_statefuls = self.__dict__["_misc_statefuls"]
             if name in _misc_statefuls:
                 return _misc_statefuls[name]
 
         return self.__getattribute__(name)
 
@@ -112,14 +113,15 @@
             )
         _remove_from_dicts(
             name,
             self.__dict__,
             self._modules,
             self._optimizers,
             self._lr_schedulers,
+            self._progress,
             self._misc_statefuls,
         )
         tracked_objects[name] = value
 
     def __setattr__(self, name: str, value: Any) -> None:
         if isinstance(value, torch.nn.Module):
             self._update_attr(name, value, self.__dict__.get("_modules"))
@@ -127,15 +129,21 @@
             self._update_attr(name, value, self.__dict__.get("_optimizers"))
         elif isinstance(value, TLRScheduler):
             self._update_attr(
                 name,
                 value,
                 self.__dict__.get("_lr_schedulers"),
             )
-        elif isinstance(value, _Stateful):
+        elif isinstance(value, Progress):
+            self._update_attr(
+                name,
+                value,
+                self.__dict__.get("_progress"),
+            )
+        elif isinstance(value, Stateful):
             self._update_attr(
                 name,
                 value,
                 self.__dict__.get("_misc_statefuls"),
             )
         else:
             if value is None:
@@ -152,14 +160,16 @@
     def __delattr__(self, name: str) -> None:
         if name in self._modules:
             del self._modules[name]
         elif name in self._optimizers:
             del self._optimizers[name]
         elif name in self._lr_schedulers:
             del self._lr_schedulers[name]
+        elif name in self._progress:
+            del self._progress[name]
         elif name in self._misc_statefuls:
             del self._misc_statefuls[name]
         else:
             super().__delattr__(name)
 
 
 class _OnExceptionMixin:
@@ -180,15 +190,15 @@
     To use the TrainUnit, create a class which subclasses TrainUnit. Then implement the ``train_step`` method on your class, and optionally
     implement any of the hooks, which allow you to control the behavior of the loop at different points.
 
     Below is a simple example of a user's subclass of TrainUnit that implements a basic ``train_step``, and the ``on_train_epoch_end`` hook.
 
     .. code-block:: python
 
-      from torchtnt.framework import TrainUnit
+      from torchtnt.framework.unit import TrainUnit
 
       Batch = Tuple[torch.tensor, torch.tensor]
       # specify type of the data in each batch of the dataloader to allow for typechecking
 
       class MyTrainUnit(TrainUnit[Batch]):
           def __init__(
               self,
@@ -213,14 +223,18 @@
           def on_train_epoch_end(self, state: State) -> None:
               # step the learning rate scheduler
               self.lr_scheduler.step()
 
       train_unit = MyTrainUnit(module=..., optimizer=..., lr_scheduler=...)
     """
 
+    def __init__(self) -> None:
+        super().__init__()
+        self.train_progress = Progress()
+
     def on_train_start(self, state: State) -> None:
         """Hook called before training starts.
 
         Args:
             state: a :class:`~torchtnt.framework.State` object containing metadata about the training run.
         """
         pass
@@ -268,15 +282,15 @@
 
     To use the EvalUnit, create a class which subclasses :class:`~torchtnt.framework.unit.EvalUnit`.
     Then implement the ``eval_step`` method on your class, and then you can optionally implement any of the hooks which allow you to control the behavior of the loop at different points.
     Below is a simple example of a user's subclass of :class:`~torchtnt.framework.unit.EvalUnit` that implements a basic ``eval_step``.
 
     .. code-block:: python
 
-      from torchtnt.framework import EvalUnit
+      from torchtnt.framework.unit import EvalUnit
 
       Batch = Tuple[torch.tensor, torch.tensor]
       # specify type of the data in each batch of the dataloader to allow for typechecking
 
       class MyEvalUnit(EvalUnit[Batch]):
           def __init__(
               self,
@@ -289,14 +303,18 @@
               inputs, targets = data
               outputs = self.module(inputs)
               loss = torch.nn.functional.binary_cross_entropy_with_logits(outputs, targets)
 
       eval_unit = MyEvalUnit(module=...)
     """
 
+    def __init__(self) -> None:
+        super().__init__()
+        self.eval_progress = Progress()
+
     def on_eval_start(self, state: State) -> None:
         """Hook called before evaluation starts.
 
         Args:
             state: a :class:`~torchtnt.framework.State` object containing metadata about the evaluation run.
         """
         pass
@@ -335,26 +353,31 @@
 
         Args:
             state: a :class:`~torchtnt.framework.State` object containing metadata about the evaluation run.
         """
         pass
 
 
-class PredictUnit(AppStateMixin, _OnExceptionMixin, Generic[TPredictData], ABC):
+class PredictUnit(
+    AppStateMixin,
+    _OnExceptionMixin,
+    Generic[TPredictData],
+    ABC,
+):
     """
     The PredictUnit is an interface that can be used to organize your prediction logic. The core of it is the ``predict_step`` which
     is an abstract method where you can define the code you want to run each iteration of the dataloader.
 
     To use the PredictUnit, create a class which subclasses :class:`~torchtnt.framework.unit.PredictUnit`.
     Then implement the ``predict_step`` method on your class, and then you can optionally implement any of the hooks which allow you to control the behavior of the loop at different points.
     Below is a simple example of a user's subclass of :class:`~torchtnt.framework.unit.PredictUnit` that implements a basic ``predict_step``.
 
     .. code-block:: python
 
-      from torchtnt.framework import PredictUnit
+      from torchtnt.framework.unit import PredictUnit
 
       Batch = Tuple[torch.tensor, torch.tensor]
       # specify type of the data in each batch of the dataloader to allow for typechecking
 
       class MyPredictUnit(PredictUnit[Batch]):
           def __init__(
               self,
@@ -367,14 +390,18 @@
               inputs, targets = data
               outputs = self.module(inputs)
               return outputs
 
       predict_unit = MyPredictUnit(module=...)
     """
 
+    def __init__(self) -> None:
+        super().__init__()
+        self.predict_progress = Progress()
+
     def on_predict_start(self, state: State) -> None:
         """Hook called before prediction starts.
 
         Args:
             state: a :class:`~torchtnt.framework.State` object containing metadata about the prediction run.
         """
         pass
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/framework/utils.py` & `torchtnt-nightly-2023.8.1/torchtnt/framework/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,22 +21,20 @@
 from torch.profiler import record_function
 from torchtnt.utils.version import is_torch_version_geq_2_0
 
 if is_torch_version_geq_2_0():
     from torch.distributed._composable_state import _get_module_state
     from torch.distributed.fsdp._common_utils import _FSDPState
 
-
-from pyre_extensions import none_throws
-from torchtnt.framework.callback import Callback
-from torchtnt.framework.state import ActivePhase, EntryPoint, State
+from torchtnt.framework.state import State
 from torchtnt.framework.unit import AppStateMixin
 from torchtnt.utils.lr_scheduler import TLRScheduler
 from torchtnt.utils.progress import Progress
 
+
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 # Helper functions common across the loops
 def _is_done(
     progress: Progress, max_epochs: Optional[int], max_steps: Optional[int]
 ) -> bool:
@@ -90,41 +88,32 @@
     for name, module in modules.items():
         if name in prior_modes:
             module.train(prior_modes[name])
 
 
 @contextmanager
 # pyre-fixme[3]: Return type must be annotated.
-def _get_timing_context(state: State, event_name: str, skip_timer: bool = False):
-    """Returns a context manager that records an event to a :class:`~torchtnt.utils.timer.Timer` and to PyTorch Profiler."""
+def get_timing_context(state: State, event_name: str):
+    """
+    Returns a context manager that records an event to a :class:`~torchtnt.utils.timer.Timer` and to PyTorch Profiler.
+
+    Args:
+        state: an instance of :class:`~torchtnt.framework.State`
+        event_name: string identifier to use for timing
+    """
     timer_context = (
         state.timer.time(event_name)
-        if state.timer and not skip_timer
+        if state.timer is not None
         else contextlib.nullcontext()
     )
     profiler_context = record_function(event_name)
     with timer_context, profiler_context:
         yield (timer_context, profiler_context)
 
 
-def _run_callback_fn(
-    callbacks: List[Callback],
-    fn_name: str,
-    state: State,
-    *args: Any,
-    **kwargs: Any,
-) -> None:
-    for cb in callbacks:
-        fn = getattr(cb, fn_name)
-        if not callable(fn):
-            raise ValueError(f"Invalid callback method name provided: {fn_name}")
-        with _get_timing_context(state, f"{cb.name}.{fn_name}"):
-            fn(state, *args, **kwargs)
-
-
 def log_api_usage(entry_point: str) -> None:
     torch._C._log_api_usage_once(f"torchtnt.framework.{entry_point}")
 
 
 def _step_requires_iterator(step_func: Callable[[State, object], object]) -> bool:
     """
     Helper function to evaluate whether the loops should pass the data iterator to the `_step`
@@ -243,21 +232,7 @@
     for optim_name, optimizer in optimizers.items():
         optimizer_params = [
             param.data_ptr() for param in optimizer.param_groups[0]["params"]
         ]
         if all(module_param in optimizer_params for module_param in module_params):
             optimizer_list.append((optim_name, optimizer))
     return optimizer_list
-
-
-def get_current_progress(state: State) -> Progress:
-    """
-    If state's entry point is fit, returns train progress. During fit, we want to return training progress even during eval, so that metrics can be compared easily across train and eval.
-    Otherwise, checks the active phase, and returns the corresponding progress class.
-    """
-    if state.entry_point == EntryPoint.FIT or state.active_phase == ActivePhase.TRAIN:
-        return none_throws(state.train_state).progress
-
-    if state.active_phase == ActivePhase.EVALUATE:
-        return none_throws(state.eval_state).progress
-    else:
-        return none_throws(state.predict_state).progress
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/__init__.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,35 +22,43 @@
     get_process_group_backend_from_device,
     get_world_size,
     PGWrapper,
     sync_bool,
 )
 from .early_stop_checker import EarlyStopChecker
 from .env import init_from_env, seed
+from .flops import FlopTensorDispatchMode
 from .fsspec import get_filesystem
 from .lr_scheduler import TLRScheduler
 from .memory import get_tensor_size_bytes_map, measure_rss_deltas, RSSProfiler
 from .misc import days_to_secs, transfer_batch_norm_stats, transfer_weights
+from .module_summary import (
+    get_module_summary,
+    get_summary_table,
+    ModuleSummary,
+    prune_module_summary,
+)
 from .oom import (
     attach_oom_observer,
     is_out_of_cpu_memory,
     is_out_of_cuda_memory,
     is_out_of_memory_error,
     log_memory_snapshot,
 )
-from .prepare_model import DDPStrategy, FSDPStrategy, prepare_ddp, prepare_fsdp
+from .prepare_module import DDPStrategy, FSDPStrategy, prepare_ddp, prepare_fsdp
 from .progress import Progress
 from .rank_zero_log import (
     rank_zero_critical,
     rank_zero_debug,
     rank_zero_error,
     rank_zero_info,
     rank_zero_print,
     rank_zero_warn,
 )
+from .stateful import Stateful
 from .timer import FullSyncPeriodicTimer, get_timer_summary, Timer
 from .tqdm import close_progress_bar, create_progress_bar, update_progress_bar
 from .version import (
     get_python_version,
     get_torch_version,
     is_torch_version_ge_1_13_1,
     is_torch_version_geq_1_10,
@@ -80,14 +88,15 @@
     "get_process_group_backend_from_device",
     "get_world_size",
     "PGWrapper",
     "sync_bool",
     "EarlyStopChecker",
     "init_from_env",
     "seed",
+    "FlopTensorDispatchMode",
     "get_filesystem",
     "get_tensor_size_bytes_map",
     "measure_rss_deltas",
     "RSSProfiler",
     "days_to_secs",
     "attach_oom_observer",
     "is_out_of_cpu_memory",
@@ -101,18 +110,23 @@
     "Progress",
     "rank_zero_critical",
     "rank_zero_debug",
     "rank_zero_error",
     "rank_zero_info",
     "rank_zero_print",
     "rank_zero_warn",
+    "Stateful",
     "FullSyncPeriodicTimer",
     "get_timer_summary",
     "transfer_batch_norm_stats",
     "transfer_weights",
+    "get_module_summary",
+    "get_summary_table",
+    "ModuleSummary",
+    "prune_module_summary",
     "Timer",
     "create_progress_bar",
     "close_progress_bar",
     "update_progress_bar",
     "TLRScheduler",
     "get_python_version",
     "get_torch_version",
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/data/__init__.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/data/data_prefetcher.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/data/data_prefetcher.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/data/iterators.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/data/iterators.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/data/multi_dataloader.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/data/multi_dataloader.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from typing import Any, Dict, Iterable, Iterator, Optional, Type, TYPE_CHECKING, Union
 
 from torchtnt.utils.data.iterators import (
     DataIterationStrategy,
     DataIterationStrategyRegistry,
     MultiIterator,
 )
+from torchtnt.utils.stateful import Stateful
 
 if TYPE_CHECKING:
     from torch.utils.data import DataLoader
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
@@ -60,15 +61,15 @@
                 else:
                     logger.warning(
                         f"Dataloader '{name}' which contains no data. "
                         "You might have empty dataloaders in the input dict."
                     )
 
     def __iter__(self) -> Iterator[Dict[str, Any]]:
-        """Iterator functions for the collection of dataloaders
+        """Iterator functions for the collection of dataloaders.
 
         Returns:
             a newly created iterator based on DataIterationStrategy
 
         """
         iterator_cls = self.iterator_cls
         if iterator_cls is None:
@@ -76,7 +77,40 @@
         # pyre-fixme[16]: `MultiDataLoader` has no attribute `iterator`.
         # pyre-fixme[45]: Cannot instantiate abstract class `MultiIterator`.
         self.iterator = iterator_cls(
             individual_dataloaders=self.individual_dataloaders,
             iteration_strategy=self.iteration_strategy,
         )
         return self.iterator
+
+    def state_dict(self) -> Dict[str, Any]:
+        """Return an aggregated state dict based on individual dataloaders.
+
+        The state dict is keyed off the names provided by ``individual_dataloaders``.
+
+        Note:
+            Only states from dataloaders that implement the :class:`~torchtnt.utils.stateful.Stateful` protocol are included in the returned state dict.
+        """
+        state_dict = {}
+        for name, dl in self.individual_dataloaders.items():
+            if isinstance(dl, Stateful):
+                state_dict[name] = dl.state_dict()
+
+        return state_dict
+
+    def load_state_dict(self, state_dict: Dict[str, Any]) -> None:
+        """Loads aggregated state dict based on individual dataloaders.
+
+        The provided state dict should be keyed off the names provided by ``individual_dataloaders``.
+
+        Note:
+            Only states from dataloaders that implement the :class:`~torchtnt.utils.stateful.Stateful` protocol are loaded.
+        """
+        for name, dl in self.individual_dataloaders.items():
+            if isinstance(dl, Stateful):
+                contents = state_dict.get(name, None)
+                if contents is None:
+                    logger.warning(
+                        f"Skipping loading state dict for dataloader {name} as there is no corresponding entry in the state dict"
+                    )
+                    continue
+                dl.load_state_dict(contents)
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/data/profile_dataloader.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/data/profile_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/device.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/device.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/distributed.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/early_stop_checker.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/early_stop_checker.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/env.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/env.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/fsspec.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/fsspec.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/__init__.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/csv.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/loggers/csv.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/file.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/loggers/file.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/in_memory.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/loggers/in_memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/json.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/loggers/json.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/logger.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/tensorboard.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/loggers/tensorboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,28 +89,28 @@
         return self._path
 
     def log_dict(self, payload: Mapping[str, Scalar], step: int) -> None:
         """Add multiple scalar values to TensorBoard.
 
         Args:
             payload (dict): dictionary of tag name and scalar value
-            step (int, Optional): step value to record
+            step (int): step value to record
         """
 
         if self._writer:
             for k, v in payload.items():
                 self.log(k, v, step)
 
     def log(self, name: str, data: Scalar, step: int) -> None:
         """Add scalar data to TensorBoard.
 
         Args:
             name (string): tag name used to group scalars
             data (float/int/Tensor): scalar data to log
-            step (int, optional): step value to record
+            step (int): step value to record
         """
 
         if self._writer:
             self._writer.add_scalar(name, data, global_step=step, new_style=True)
 
     def log_text(self, name: str, data: str, step: int) -> None:
         """Add text data to summary.
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/loggers/utils.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/loggers/utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/memory.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/misc.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/misc.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/oom.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/oom.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/prepare_model.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/prepare_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,19 +63,19 @@
 class FSDPStrategy(Strategy):
     """Dataclass representing the `FullyShardedDataParallel <https://pytorch.org/docs/stable/fsdp.html>`_ strategy"""
 
     process_group: Optional[ProcessGroup] = None
     sharding_strategy: Optional[ShardingStrategy] = None
     cpu_offload: Optional[CPUOffload] = None
     auto_wrap_policy: Optional[Callable[[torch.nn.Module, bool, int], bool]] = None
-    backward_prefetch: Optional[BackwardPrefetch] = None
+    backward_prefetch: Optional[BackwardPrefetch] = BackwardPrefetch.BACKWARD_PRE
     ignored_modules: Optional[Iterable[torch.nn.Module]] = None
     sync_module_states: bool = False
     forward_prefetch: bool = False
-    limit_all_gathers: bool = False
+    limit_all_gathers: bool = True
     use_orig_params: bool = False
 
     # FSDP set_state_dict_type params: https://pytorch.org/docs/stable/fsdp.html#torch.distributed.fsdp.FullyShardedDataParallel.set_state_dict_type
     # for setting type of state dict for checkpointing
     state_dict_type: Optional[StateDictType] = None
     state_dict_config: Optional[StateDictConfig] = None
     optim_state_dict_config: Optional[OptimStateDictConfig] = None
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/progress.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/progress.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/rank_zero_log.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/rank_zero_log.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/test_utils.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/timer.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/timer.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,149 +4,160 @@
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 import datetime
 import logging
 import os
-import warnings
 from collections import defaultdict
 from contextlib import contextmanager
 from time import perf_counter
-from typing import Dict, Generator, List, Optional, Sequence, Tuple, TypeVar
+from typing import (
+    Dict,
+    Generator,
+    List,
+    Optional,
+    Protocol,
+    runtime_checkable,
+    Sequence,
+    Tuple,
+    TypeVar,
+)
 
 import numpy as np
 
 import torch
 import torch.distributed as dist
 from torchtnt.utils.distributed import PGWrapper
 
+logger: logging.Logger = logging.getLogger(__name__)
 
 AsyncOperator = TypeVar("AsyncOperator")
 
 
 _TABLE_ROW = Tuple[str, float, int, float, float]
 _TABLE_DATA = List[_TABLE_ROW]
 
 
-class Timer:
+@runtime_checkable
+class TimerProtocol(Protocol):
     """
-    A timer which records intervals between starts and stops, as well as cumulative time in seconds.
+    Defines a Timer Protocol with `time` and `reset` methods and an attribute `recorded_durations` for storing timings.
     """
 
-    def __init__(self) -> None:
-        self.recorded_durations: Dict[str, List[float]] = defaultdict(list)
-        self.reset()
-
-    def reset(self) -> None:
-        """Reset timer state."""
-        self._paused: bool = True
-        self._interval_start_time: float = 0.0
-        self._interval_stop_time: float = 0.0
-        self._total_time_seconds: float = 0.0
-
-    def start(self) -> None:
-        """Start timer interval."""
-        if not self.paused:
-            warnings.warn("Cannot start timer while timer is running.")
-            return
-        self._paused = False
-        if torch.cuda.is_available():
-            torch.cuda.synchronize()
-        self._interval_start_time = perf_counter()
-
-    def stop(self) -> None:
-        """Stop timer interval. Interval time will be added to the total."""
-        if self.paused:
-            warnings.warn("Cannot stop timer while timer is paused.")
-            return
-        if torch.cuda.is_available():
-            torch.cuda.synchronize()
-        self._interval_stop_time = perf_counter()
-        self._paused = True
-        self._total_time_seconds += self.interval_time_seconds
+    recorded_durations: Dict[str, List[float]]
 
     @contextmanager
     def time(self, action_name: str) -> Generator[None, None, None]:
-        """Yields a context manager to encapsulate the scope of a timed action.
+        """
+        A context manager for timing a code block.
 
         Args:
-            action_name: the name under which to store the timing of what is enclosed in the context manager
+            action_name: the name under which to store the timing of what is enclosed in the context manager.
         """
-        try:
-            self.start()
-            yield
-        finally:
-            self.stop()
-        self.recorded_durations[action_name].append(self.interval_time_seconds)
+        ...
+
+    def reset(self) -> None:
+        """
+        A method to reset the state of the Timer.
+        """
+        ...
 
-    @property
-    def paused(self) -> bool:
-        return self._paused
 
-    @property
-    def interval_time_seconds(self) -> float:
+class Timer(TimerProtocol):
+    def __init__(
+        self,
+        *,
+        cuda_sync: Optional[bool] = None,
+        verbose: bool = False,
+    ) -> None:
         """
-        Interval between most recent stop and start in seconds.
-        If timer is still running, return interval between most recent start and now.
+        A Timer class which implements TimerProtocol and stores timings in a dictionary `recorded_durations`.
+
+        Args:
+            cuda_sync: whether to call torch.cuda.synchronize() before and after timing. Defaults to True if CUDA is available.
+            verbose: whether to enable verbose logging.
+
+        Note:
+            Enabling cuda_sync will incur a performance hit, but will ensure accurate timings on GPUs.
+
+        Raises:
+            ValueError: If cuda_sync is set to True but CUDA is not available.
+
         """
-        if self._interval_start_time == 0.0:
-            return 0.0
-        interval_stop_time = self._interval_stop_time if self.paused else perf_counter()
-        return interval_stop_time - self._interval_start_time
-
-    @property
-    def total_time_seconds(self) -> float:
-        """Sum of all interval times in seconds since the last reset.
-        If timer is still running, include the current interval time in the total.
+        if cuda_sync and not torch.cuda.is_available():
+            raise ValueError(
+                "CUDA must be available in order to enable CUDA synchronization."
+            )
+        self.cuda_sync: bool = (
+            cuda_sync if cuda_sync is not None else torch.cuda.is_available()
+        )
+        self.verbose = verbose
+        self.recorded_durations: Dict[str, List[float]] = defaultdict(list)
+
+    @contextmanager
+    def time(
+        self,
+        action_name: str,
+    ) -> Generator[None, None, None]:
         """
-        running_interval = 0 if self.paused else self.interval_time_seconds
-        return self._total_time_seconds + running_interval
+        A context manager for timing a code block, with optional cuda synchronization and verbose timing.
 
-    def state_dict(self) -> Dict[str, float]:
+        Args:
+            action_name: the name under which to store the timing of what is enclosed in the context manager.
         """
-        Pause timer and export state_dict for checkpointing.
+        try:
+            if self.cuda_sync:
+                torch.cuda.synchronize()
+            start_time: float = perf_counter()
+            yield
+        finally:
+            if self.cuda_sync:
+                torch.cuda.synchronize()
+            interval_time: float = perf_counter() - start_time
+            if self.verbose:
+                logger.info(f"{action_name} took {interval_time} seconds.")
+        self.recorded_durations[action_name].append(interval_time)
 
-        Raises:
-            Exception:
-                If state_dict is called while timer is still running.
+    def reset(self) -> None:
+        """
+        Reset the recorded_durations to an empty list
         """
-        if not self.paused:
-            raise Exception("Timer must be paused before creating state_dict.")
-        return {
-            "interval_start_time": self._interval_start_time,
-            "interval_stop_time": self._interval_stop_time,
-            "total_time_seconds": self._total_time_seconds,
-        }
-
-    def load_state_dict(self, state_dict: Dict[str, float]) -> None:
-        """Load timer state from state dict."""
-        self._interval_start_time = state_dict["interval_start_time"]
-        self._interval_stop_time = state_dict["interval_stop_time"]
-        self._total_time_seconds = state_dict["total_time_seconds"]
+        self.recorded_durations = defaultdict(list)
+
 
+def _get_total_time(timer: TimerProtocol) -> float:
+    total_time = 0.0
+    for _, durations in timer.recorded_durations.items():
+        array_value = np.array(durations)
+        array_sum = np.sum(array_value)
+        total_time += array_sum
 
-def _make_report(timer: Timer) -> Tuple[_TABLE_DATA, float, float]:
+    return total_time
+
+
+def _make_report(timer: TimerProtocol) -> Tuple[_TABLE_DATA, float, float]:
+    total_time = _get_total_time(timer)
     report = [
         (
             a,
             np.mean(d),
             len(d),
             np.sum(d),
-            100.0 * np.sum(d) / timer._total_time_seconds,
+            100.0 * np.sum(d) / total_time,
         )
         for a, d in timer.recorded_durations.items()
     ]
     report.sort(key=lambda x: x[4], reverse=True)
     total_calls = sum(x[2] for x in report)
-    return report, total_calls, timer._total_time_seconds
+    return report, total_calls, total_time
 
 
-def get_timer_summary(timer: Timer) -> str:
-    """Given a Timer, generate a summary of all the recorded actions.
+def get_timer_summary(timer: TimerProtocol) -> str:
+    """Given a timer, generate a summary of all the recorded actions.
 
     Args:
         timer: the Timer object for which to generate a summary
 
     Raises:
         ValueError
             If the input Timer has no recorded actions
@@ -325,36 +336,14 @@
 
 def _validate_percentiles(percentiles: Sequence[float]) -> None:
     for p in percentiles:
         if p < 0 or p > 100:
             raise ValueError(f"Percentile must be between 0 and 100. Got {p}")
 
 
-class VerboseTimer(Timer):
-    """Timer that is more verbose - prints information upon start/stop.
-    Requires a customizable logger.
-    """
-
-    @contextmanager
-    def time(
-        self, action_name: str, logger: logging.Logger
-    ) -> Generator[None, None, None]:
-        try:
-            logger.info(f"Starting {action_name}")
-            self.start()
-            yield
-        finally:
-            self.stop()
-            logger.info(
-                f"Stopping {action_name}. Took {self.interval_time_seconds} seconds"
-            )
-
-        self.recorded_durations[action_name].append(self.interval_time_seconds)
-
-
 class FullSyncPeriodicTimer:
     """
     Measures time (resets if given interval elapses) on rank 0
     and propagates result to other ranks.
     Propagation is done asynchronously from previous step
     in order to avoid blocking of a training process.
     """
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/tqdm.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/tqdm.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt/utils/version.py` & `torchtnt-nightly-2023.8.1/torchtnt/utils/version.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.9/torchtnt_nightly.egg-info/PKG-INFO` & `torchtnt-nightly-2023.8.1/torchtnt_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2023.7.9
+Version: 2023.8.1
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.7.9 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.8.1 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt-nightly-2023.7.9/torchtnt_nightly.egg-info/SOURCES.txt` & `torchtnt-nightly-2023.8.1/torchtnt_nightly.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 torchtnt/__init__.py
 torchtnt/py.typed
 torchtnt/framework/__init__.py
+torchtnt/framework/_callback_handler.py
 torchtnt/framework/_test_utils.py
 torchtnt/framework/auto_unit.py
 torchtnt/framework/callback.py
 torchtnt/framework/evaluate.py
 torchtnt/framework/fit.py
 torchtnt/framework/predict.py
 torchtnt/framework/state.py
@@ -28,22 +29,25 @@
 torchtnt/framework/callbacks/tqdm_progress_bar.py
 torchtnt/framework/callbacks/train_progress_monitor.py
 torchtnt/utils/__init__.py
 torchtnt/utils/device.py
 torchtnt/utils/distributed.py
 torchtnt/utils/early_stop_checker.py
 torchtnt/utils/env.py
+torchtnt/utils/flops.py
 torchtnt/utils/fsspec.py
 torchtnt/utils/lr_scheduler.py
 torchtnt/utils/memory.py
 torchtnt/utils/misc.py
+torchtnt/utils/module_summary.py
 torchtnt/utils/oom.py
-torchtnt/utils/prepare_model.py
+torchtnt/utils/prepare_module.py
 torchtnt/utils/progress.py
 torchtnt/utils/rank_zero_log.py
+torchtnt/utils/stateful.py
 torchtnt/utils/test_utils.py
 torchtnt/utils/timer.py
 torchtnt/utils/tqdm.py
 torchtnt/utils/version.py
 torchtnt/utils/data/__init__.py
 torchtnt/utils/data/data_prefetcher.py
 torchtnt/utils/data/iterators.py
```

