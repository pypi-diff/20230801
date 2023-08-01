# Comparing `tmp/sparsify-nightly-1.6.0.20230723.tar.gz` & `tmp/sparsify-nightly-1.6.0.20230801.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sparsify-nightly-1.6.0.20230723.tar", last modified: Sun Jul 23 20:07:38 2023, max compression
+gzip compressed data, was "dist/sparsify-nightly-1.6.0.20230801.tar", last modified: Tue Aug  1 14:43:39 2023, max compression
```

## Comparing `sparsify-nightly-1.6.0.20230723.tar` & `sparsify-nightly-1.6.0.20230801.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1243 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/NOTICE
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/create/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4248 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/create/api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      728 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/create/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1817 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/create/schemas.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5235 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/login.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      674 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/cli/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      617 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/cli/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5632 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/cli/opts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5045 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/cli/run.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1490 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      825 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      760 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3325 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/nm_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2161 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/hardware_analyzer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9333 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6855 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/error_handler.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/scripts/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2385 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/scripts/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      617 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/scripts/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/transformers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      695 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/transformers/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26268 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/transformers/args.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13031 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/transformers/runner.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/deployment_instructions.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      695 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3356 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/args.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18157 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/runner.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/object_detection/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/object_detection/yolov5/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      676 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/object_detection/yolov5/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6896 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/object_detection/yolov5/args.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8349 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/object_detection/yolov5/runner.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      656 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/object_detection/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/image_classification/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      676 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/image_classification/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6146 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/image_classification/args.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8088 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/image_classification/runner.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      873 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      735 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1055 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/pathway_checks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5941 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/ort_health.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1359 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/gpu_device.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4247 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/utils/system.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      748 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3681 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/utils/task_name.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      877 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/utils/nm_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4393 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/utils/helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5067 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/utils/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      758 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/utils/exceptions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/one_shot/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3353 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/one_shot/api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      745 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/one_shot/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3758 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/schemas/tuning_hyperparameters.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11587 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/schemas/auto_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      715 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/src/sparsify/schemas/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify_nightly.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify_nightly.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      159 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify_nightly.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29051 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify_nightly.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify_nightly.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      316 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify_nightly.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2167 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/src/sparsify_nightly.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23875 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4453 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29051 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       56 2023-07-23 20:05:01.000000 sparsify-nightly-1.6.0.20230723/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      625 2023-07-23 20:07:38.000000 sparsify-nightly-1.6.0.20230723/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 14:43:39.000000 sparsify-nightly-1.6.0.20230801/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1243 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/NOTICE
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 14:43:38.000000 sparsify-nightly-1.6.0.20230801/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 14:43:38.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 14:43:39.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/create/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4248 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/create/api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      728 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/create/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1817 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/create/schemas.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5235 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/login.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      674 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 14:43:39.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/cli/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      617 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/cli/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5632 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/cli/opts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5045 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/cli/run.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1490 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 14:43:38.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      825 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 14:43:39.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      760 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3325 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/utils/nm_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2161 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/utils/hardware_analyzer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9333 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/utils/helpers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6855 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/utils/error_handler.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 14:43:38.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/scripts/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2385 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/scripts/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      617 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/scripts/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 14:43:38.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 14:43:39.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/transformers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      695 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/transformers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26268 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/transformers/args.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13031 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/transformers/runner.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3711 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/deployment_instructions.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      695 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3356 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/args.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18157 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/runner.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 14:43:39.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/object_detection/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 14:43:39.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/object_detection/yolov5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      676 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/object_detection/yolov5/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6896 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/object_detection/yolov5/args.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8349 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/object_detection/yolov5/runner.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      656 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/object_detection/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 14:43:39.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/image_classification/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      676 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/image_classification/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6146 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/image_classification/args.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8088 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/image_classification/runner.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 14:43:39.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/check_environment/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      873 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/check_environment/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      735 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/check_environment/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1055 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/check_environment/pathway_checks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5941 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/check_environment/ort_health.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1359 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/check_environment/gpu_device.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 14:43:39.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4247 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/utils/system.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      748 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3681 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/utils/task_name.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      877 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/utils/nm_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4393 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/utils/helpers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5067 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/utils/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      758 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/utils/exceptions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 14:43:39.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/one_shot/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3353 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/one_shot/api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      745 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/one_shot/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 14:43:39.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3758 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/schemas/tuning_hyperparameters.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11587 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/schemas/auto_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      715 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/src/sparsify/schemas/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 14:43:39.000000 sparsify-nightly-1.6.0.20230801/src/sparsify_nightly.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-08-01 14:43:38.000000 sparsify-nightly-1.6.0.20230801/src/sparsify_nightly.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      159 2023-08-01 14:43:38.000000 sparsify-nightly-1.6.0.20230801/src/sparsify_nightly.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29051 2023-08-01 14:43:38.000000 sparsify-nightly-1.6.0.20230801/src/sparsify_nightly.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-08-01 14:43:38.000000 sparsify-nightly-1.6.0.20230801/src/sparsify_nightly.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      316 2023-08-01 14:43:38.000000 sparsify-nightly-1.6.0.20230801/src/sparsify_nightly.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2167 2023-08-01 14:43:38.000000 sparsify-nightly-1.6.0.20230801/src/sparsify_nightly.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23875 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4453 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29051 2023-08-01 14:43:39.000000 sparsify-nightly-1.6.0.20230801/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       56 2023-08-01 14:41:02.000000 sparsify-nightly-1.6.0.20230801/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      625 2023-08-01 14:43:39.000000 sparsify-nightly-1.6.0.20230801/setup.cfg
```

### Comparing `sparsify-nightly-1.6.0.20230723/NOTICE` & `sparsify-nightly-1.6.0.20230801/NOTICE`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/create/api.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/create/api.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/create/__init__.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/create/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/create/schemas.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/create/schemas.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/login.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/login.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/__init__.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/cli/__init__.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/cli/opts.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/cli/opts.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/cli/run.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/cli/run.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/version.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/version.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/__init__.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/__init__.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/nm_api.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/utils/nm_api.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/hardware_analyzer.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/utils/hardware_analyzer.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/helpers.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/utils/error_handler.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/utils/error_handler.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/scripts/main.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/scripts/main.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/scripts/__init__.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/transformers/__init__.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/transformers/args.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/transformers/args.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/transformers/runner.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/transformers/runner.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/deployment_instructions.md` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/deployment_instructions.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 custom_pipeline = CustomTaskPipeline(
     model_path="zoo:cv/classification/resnet_v1-50/pytorch/sparseml/imagenet/pruned90_quant-none",
     process_inputs_fn=preprocess,
 )
 ​
 scores, probs = custom_pipeline("buddy.jpeg")
 ```
-(Note: Download [buddy.jpeg](https://github.com/neuralmagic/deepsparse/blob/main/tests/deepsparse/pipelines/sample_images/buddy.jpeg))
+(Note: Download [buddy.jpeg](https://raw.githubusercontent.com/neuralmagic/deepsparse/main/tests/deepsparse/pipelines/sample_images/buddy.jpeg))
 
 ​
 For more information on the available pipelines and how to create custom pipelines, see the [Pipeline Deployment Guide](https://github.com/neuralmagic/deepsparse/blob/main/docs/user-guide/deepsparse-benchmarking.md).
 ​
 ## Server Deployments
 ​
 DeepSparse additionally contains a performant server deployment for different use cases.
```

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/__init__.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/args.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/args.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/runner.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/runner.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/object_detection/yolov5/__init__.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/object_detection/yolov5/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/object_detection/yolov5/args.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/object_detection/yolov5/args.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/object_detection/yolov5/runner.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/object_detection/yolov5/runner.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/object_detection/__init__.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/image_classification/__init__.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/image_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/image_classification/args.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/image_classification/args.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/auto/tasks/image_classification/runner.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/auto/tasks/image_classification/runner.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/main.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/check_environment/main.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/__init__.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/check_environment/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/pathway_checks.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/check_environment/pathway_checks.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/ort_health.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/check_environment/ort_health.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/check_environment/gpu_device.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/check_environment/gpu_device.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/utils/system.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/utils/system.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/utils/__init__.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/utils/task_name.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/utils/task_name.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/utils/nm_api.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/utils/nm_api.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/utils/helpers.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/utils/constants.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/utils/exceptions.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/one_shot/api.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/one_shot/api.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/one_shot/__init__.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/one_shot/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/schemas/tuning_hyperparameters.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/schemas/tuning_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/schemas/auto_api.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/schemas/auto_api.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify/schemas/__init__.py` & `sparsify-nightly-1.6.0.20230801/src/sparsify/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify_nightly.egg-info/PKG-INFO` & `sparsify-nightly-1.6.0.20230801/src/sparsify_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparsify-nightly
-Version: 1.6.0.20230723
+Version: 1.6.0.20230801
 Summary: Easy-to-use UI for automatically sparsifying neural networks and creating sparsification recipes for better inference performance and a smaller footprint
 Home-page: https://github.com/neuralmagic/sparsify
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache
 Description: 
         <!--
@@ -459,24 +459,24 @@
         ```
         
 Keywords: inference,machine learning,neural network,computer vision,nlp,cv,deep learning,torch,pytorch,tensorflow,keras,automl,sparsity,pruning,deep learning libraries,onnx,quantization
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sparsify-nightly Version: 1.6.0.20230723 Summary:
+Metadata-Version: 2.1 Name: sparsify-nightly Version: 1.6.0.20230801 Summary:
 Easy-to-use UI for automatically sparsifying neural networks and creating
 sparsification recipes for better inference performance and a smaller footprint
 Home-page: https://github.com/neuralmagic/sparsify Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com License: Apache Description:
 ****** [Sparsify tool icon]  Sparsify [Alpha] ******
 **** ML model optimization product to accelerate inference ****
 [Documentation] [https://img.shields.io/badge/slack-purple?style=for-the-
@@ -273,18 +273,18 @@
 year={2020}, eprint={2004.14340}, archivePrefix={arXiv}, primaryClass={cs.LG} }
 ``` Keywords: inference,machine learning,neural network,computer
 vision,nlp,cv,deep
 learning,torch,pytorch,tensorflow,keras,automl,sparsity,pruning,deep learning
 libraries,onnx,quantization Platform: UNKNOWN Classifier: Development Status ::
 5 - Production/Stable Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Requires-Python: >=3.7.0
+Development :: Libraries :: Python Modules Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown Provides-Extra: dev
```

### Comparing `sparsify-nightly-1.6.0.20230723/src/sparsify_nightly.egg-info/SOURCES.txt` & `sparsify-nightly-1.6.0.20230801/src/sparsify_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/README.md` & `sparsify-nightly-1.6.0.20230801/README.md`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/LICENSE` & `sparsify-nightly-1.6.0.20230801/LICENSE`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230723/setup.py` & `sparsify-nightly-1.6.0.20230801/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,20 +110,20 @@
     url="https://github.com/neuralmagic/sparsify",
     include_package_data=True,
     package_dir=_setup_package_dir(),
     packages=_setup_packages(),
     install_requires=_setup_install_requires(),
     extras_require=_setup_extras(),
     entry_points=_setup_entry_points(),
-    python_requires=">=3.7.0",
+    python_requires=">=3.8.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
```

### Comparing `sparsify-nightly-1.6.0.20230723/PKG-INFO` & `sparsify-nightly-1.6.0.20230801/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparsify-nightly
-Version: 1.6.0.20230723
+Version: 1.6.0.20230801
 Summary: Easy-to-use UI for automatically sparsifying neural networks and creating sparsification recipes for better inference performance and a smaller footprint
 Home-page: https://github.com/neuralmagic/sparsify
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache
 Description: 
         <!--
@@ -459,24 +459,24 @@
         ```
         
 Keywords: inference,machine learning,neural network,computer vision,nlp,cv,deep learning,torch,pytorch,tensorflow,keras,automl,sparsity,pruning,deep learning libraries,onnx,quantization
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sparsify-nightly Version: 1.6.0.20230723 Summary:
+Metadata-Version: 2.1 Name: sparsify-nightly Version: 1.6.0.20230801 Summary:
 Easy-to-use UI for automatically sparsifying neural networks and creating
 sparsification recipes for better inference performance and a smaller footprint
 Home-page: https://github.com/neuralmagic/sparsify Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com License: Apache Description:
 ****** [Sparsify tool icon]  Sparsify [Alpha] ******
 **** ML model optimization product to accelerate inference ****
 [Documentation] [https://img.shields.io/badge/slack-purple?style=for-the-
@@ -273,18 +273,18 @@
 year={2020}, eprint={2004.14340}, archivePrefix={arXiv}, primaryClass={cs.LG} }
 ``` Keywords: inference,machine learning,neural network,computer
 vision,nlp,cv,deep
 learning,torch,pytorch,tensorflow,keras,automl,sparsity,pruning,deep learning
 libraries,onnx,quantization Platform: UNKNOWN Classifier: Development Status ::
 5 - Production/Stable Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Requires-Python: >=3.7.0
+Development :: Libraries :: Python Modules Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown Provides-Extra: dev
```

### Comparing `sparsify-nightly-1.6.0.20230723/setup.cfg` & `sparsify-nightly-1.6.0.20230801/setup.cfg`

 * *Files identical despite different names*

