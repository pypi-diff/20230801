# Comparing `tmp/chemprop-1.6.0.tar.gz` & `tmp/chemprop-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemprop-1.6.0.tar", last modified: Wed Jul 19 16:52:25 2023, max compression
+gzip compressed data, was "chemprop-1.6.1.tar", last modified: Tue Aug  1 20:40:28 2023, max compression
```

## Comparing `chemprop-1.6.0.tar` & `chemprop-1.6.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 kpg       (1016) kpg       (1016)        0 2023-07-19 16:52:25.217102 chemprop-1.6.0/
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     1127 2023-05-18 18:22:54.000000 chemprop-1.6.0/LICENSE.txt
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    66084 2023-07-19 16:52:25.217102 chemprop-1.6.0/PKG-INFO
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    65023 2023-07-17 20:28:44.000000 chemprop-1.6.0/README.md
-drwxrwxr-x   0 kpg       (1016) kpg       (1016)        0 2023-07-19 16:52:25.213102 chemprop-1.6.0/chemprop/
--rw-rw-r--   0 kpg       (1016) kpg       (1016)      474 2023-07-17 20:33:26.000000 chemprop-1.6.0/chemprop/__init__.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    58955 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/args.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)      233 2023-05-18 18:22:54.000000 chemprop-1.6.0/chemprop/constants.py
-drwxrwxr-x   0 kpg       (1016) kpg       (1016)        0 2023-07-19 16:52:25.213102 chemprop-1.6.0/chemprop/data/
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     1410 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/data/__init__.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    41700 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/data/data.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     7896 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/data/scaffold.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     6343 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/data/scaler.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    43137 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/data/utils.py
-drwxrwxr-x   0 kpg       (1016) kpg       (1016)        0 2023-07-19 16:52:25.213102 chemprop-1.6.0/chemprop/features/
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     1491 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/features/__init__.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     6219 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/features/features_generators.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    33729 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/features/featurization.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     4085 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/features/utils.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    14944 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/hyperopt_utils.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     8147 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/hyperparameter_optimization.py
--rwxrwxr-x   0 kpg       (1016) kpg       (1016)    13921 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/interpret.py
-drwxrwxr-x   0 kpg       (1016) kpg       (1016)        0 2023-07-19 16:52:25.213102 chemprop-1.6.0/chemprop/models/
--rw-rw-r--   0 kpg       (1016) kpg       (1016)      206 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/models/__init__.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    16096 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/models/ffn.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    15909 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/models/model.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    17948 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/models/mpn.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     3435 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/multitask_utils.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     8202 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/nn_utils.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)       27 2023-05-18 18:22:54.000000 chemprop-1.6.0/chemprop/py.typed
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     1210 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/rdkit.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     3097 2023-07-17 20:28:49.000000 chemprop-1.6.0/chemprop/sklearn_predict.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    15071 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/sklearn_train.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     5245 2023-05-18 18:22:54.000000 chemprop-1.6.0/chemprop/spectra_utils.py
-drwxrwxr-x   0 kpg       (1016) kpg       (1016)        0 2023-07-19 16:52:25.217102 chemprop-1.6.0/chemprop/train/
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     1395 2023-05-18 18:22:54.000000 chemprop-1.6.0/chemprop/train/__init__.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     8998 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/train/cross_validate.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     7022 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/train/evaluate.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    15379 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/train/loss_functions.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    21730 2023-07-17 20:28:49.000000 chemprop-1.6.0/chemprop/train/make_predictions.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    13018 2023-05-18 18:22:54.000000 chemprop-1.6.0/chemprop/train/metrics.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    10654 2023-07-17 20:28:49.000000 chemprop-1.6.0/chemprop/train/molecule_fingerprint.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    10741 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/train/predict.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    19813 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/train/run_training.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    12670 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/train/train.py
-drwxrwxr-x   0 kpg       (1016) kpg       (1016)        0 2023-07-19 16:52:25.217102 chemprop-1.6.0/chemprop/uncertainty/
--rw-rw-r--   0 kpg       (1016) kpg       (1016)      547 2023-05-18 18:22:54.000000 chemprop-1.6.0/chemprop/uncertainty/__init__.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    41156 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/uncertainty/uncertainty_calibrator.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     2480 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/uncertainty/uncertainty_estimator.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    19954 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/uncertainty/uncertainty_evaluator.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    51885 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/uncertainty/uncertainty_predictor.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    36993 2023-07-17 20:28:49.000000 chemprop-1.6.0/chemprop/utils.py
-drwxrwxr-x   0 kpg       (1016) kpg       (1016)        0 2023-07-19 16:52:25.217102 chemprop-1.6.0/chemprop/web/
--rw-rw-r--   0 kpg       (1016) kpg       (1016)       42 2023-05-18 18:22:54.000000 chemprop-1.6.0/chemprop/web/__init__.py
-drwxrwxr-x   0 kpg       (1016) kpg       (1016)        0 2023-07-19 16:52:25.217102 chemprop-1.6.0/chemprop/web/app/
--rw-rw-r--   0 kpg       (1016) kpg       (1016)      429 2023-05-18 18:22:54.000000 chemprop-1.6.0/chemprop/web/app/__init__.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     8348 2023-05-18 18:22:54.000000 chemprop-1.6.0/chemprop/web/app/db.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    21135 2023-07-17 20:28:44.000000 chemprop-1.6.0/chemprop/web/app/views.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)      351 2023-05-18 18:22:54.000000 chemprop-1.6.0/chemprop/web/config.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     1423 2023-05-18 18:22:54.000000 chemprop-1.6.0/chemprop/web/run.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     1709 2023-05-18 18:22:54.000000 chemprop-1.6.0/chemprop/web/utils.py
--rw-rw-r--   0 kpg       (1016) kpg       (1016)      670 2023-05-18 18:22:54.000000 chemprop-1.6.0/chemprop/web/wsgi.py
-drwxrwxr-x   0 kpg       (1016) kpg       (1016)        0 2023-07-19 16:52:25.213102 chemprop-1.6.0/chemprop.egg-info/
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    66084 2023-07-19 16:52:25.000000 chemprop-1.6.0/chemprop.egg-info/PKG-INFO
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     1653 2023-07-19 16:52:25.000000 chemprop-1.6.0/chemprop.egg-info/SOURCES.txt
--rw-rw-r--   0 kpg       (1016) kpg       (1016)        1 2023-07-19 16:52:25.000000 chemprop-1.6.0/chemprop.egg-info/dependency_links.txt
--rw-rw-r--   0 kpg       (1016) kpg       (1016)      466 2023-07-19 16:52:25.000000 chemprop-1.6.0/chemprop.egg-info/entry_points.txt
--rw-rw-r--   0 kpg       (1016) kpg       (1016)      301 2023-07-19 16:52:25.000000 chemprop-1.6.0/chemprop.egg-info/requires.txt
--rw-rw-r--   0 kpg       (1016) kpg       (1016)        9 2023-07-19 16:52:25.000000 chemprop-1.6.0/chemprop.egg-info/top_level.txt
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     1945 2023-07-19 16:52:25.217102 chemprop-1.6.0/setup.cfg
--rw-rw-r--   0 kpg       (1016) kpg       (1016)     2626 2023-07-17 20:33:26.000000 chemprop-1.6.0/setup.py
-drwxrwxr-x   0 kpg       (1016) kpg       (1016)        0 2023-07-19 16:52:25.217102 chemprop-1.6.0/tests/
--rw-rw-r--   0 kpg       (1016) kpg       (1016)    50552 2023-07-17 20:28:44.000000 chemprop-1.6.0/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:28.829637 chemprop-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-01 20:40:19.000000 chemprop-1.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    66319 2023-08-01 20:40:28.829637 chemprop-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    65258 2023-08-01 20:40:19.000000 chemprop-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:28.825637 chemprop-1.6.1/chemprop/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58955 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:28.825637 chemprop-1.6.1/chemprop/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41700 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/data/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/data/scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43137 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:28.825637 chemprop-1.6.1/chemprop/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/features/features_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33781 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/features/featurization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/features/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/hyperopt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/hyperparameter_optimization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13921 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/interpret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:28.825637 chemprop-1.6.1/chemprop/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16096 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/models/ffn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15909 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17948 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/models/mpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/multitask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/nn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/rdkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/sklearn_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15071 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/sklearn_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/spectra_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:28.829637 chemprop-1.6.1/chemprop/train/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/train/cross_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/train/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15379 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/train/loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21730 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/train/make_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/train/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10654 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/train/molecule_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/train/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19813 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/train/run_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12670 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/train/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:28.829637 chemprop-1.6.1/chemprop/uncertainty/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/uncertainty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41156 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/uncertainty/uncertainty_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/uncertainty/uncertainty_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19954 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/uncertainty/uncertainty_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51885 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/uncertainty/uncertainty_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36993 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:28.829637 chemprop-1.6.1/chemprop/web/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:28.829637 chemprop-1.6.1/chemprop/web/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/web/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/web/app/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21135 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/web/app/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/web/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/web/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/web/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-01 20:40:19.000000 chemprop-1.6.1/chemprop/web/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:28.825637 chemprop-1.6.1/chemprop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    66319 2023-08-01 20:40:28.000000 chemprop-1.6.1/chemprop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-08-01 20:40:28.000000 chemprop-1.6.1/chemprop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:40:28.000000 chemprop-1.6.1/chemprop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-01 20:40:28.000000 chemprop-1.6.1/chemprop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-01 20:40:28.000000 chemprop-1.6.1/chemprop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 20:40:28.000000 chemprop-1.6.1/chemprop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-08-01 20:40:28.829637 chemprop-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-08-01 20:40:19.000000 chemprop-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:28.829637 chemprop-1.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    50547 2023-08-01 20:40:19.000000 chemprop-1.6.1/tests/test_integration.py
```

### Comparing `chemprop-1.6.0/LICENSE.txt` & `chemprop-1.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/PKG-INFO` & `chemprop-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chemprop
-Version: 1.6.0
+Version: 1.6.1
 Summary: Molecular Property Prediction with Message Passing Neural Networks
 Home-page: https://github.com/chemprop/chemprop
-Download-URL: https://github.com/chemprop/chemprop/v_1.6.0.tar.gz
+Download-URL: https://github.com/chemprop/chemprop/v_1.6.1.tar.gz
 Author: Kyle Swanson, Kevin Yang, Wengong Jin, Lior Hirschfeld, Allison Tam
 Author-email: chemprop@mit.edu
 License: MIT
 Project-URL: Documentation, https://chemprop.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/chemprop/chemprop
 Project-URL: PyPi, https://pypi.org/project/chemprop/
 Project-URL: Demo, http://chemprop.csail.mit.edu/
@@ -25,15 +25,15 @@
 ![ChemProp Logo](docs/source/_static/images/chemprop_logo.svg)
 # Molecular Property Prediction
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/chemprop)](https://badge.fury.io/py/chemprop)
 [![PyPI version](https://badge.fury.io/py/chemprop.svg)](https://badge.fury.io/py/chemprop)
 [![Build Status](https://github.com/chemprop/chemprop/workflows/tests/badge.svg)](https://github.com/chemprop/chemprop)
 
-This repository contains message passing neural networks for molecular property prediction as described in the paper [Analyzing Learned Molecular Representations for Property Prediction](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.9b00237) and as used in the paper [A Deep Learning Approach to Antibiotic Discovery](https://www.cell.com/cell/fulltext/S0092-8674(20)30102-1) for molecules and [Machine Learning of Reaction Properties via Learned Representations of the Condensed Graph of Reaction](https://doi.org/10.1021/acs.jcim.1c00975) for reactions.
+This repository contains message passing neural networks for molecular property prediction as initially described in the paper [Analyzing Learned Molecular Representations for Property Prediction](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.9b00237) and as used in the paper [A Deep Learning Approach to Antibiotic Discovery](https://www.cell.com/cell/fulltext/S0092-8674(20)30102-1) for molecules and [Machine Learning of Reaction Properties via Learned Representations of the Condensed Graph of Reaction](https://doi.org/10.1021/acs.jcim.1c00975) for reactions. Chemprop now also has its own dedicated manuscript: [Chemprop: Machine Learning Package for Chemical Property Prediction](https://doi.org/10.26434/chemrxiv-2023-3zcfl). Please cite us if Chemprop is helpful to your research.
 
 **Documentation:** Full documentation of Chemprop is available at https://chemprop.readthedocs.io/en/latest/.
 
 **Website:** A web prediction interface with some trained Chemprop models is available at [chemprop.csail.mit.edu](http://chemprop.csail.mit.edu).
 
 **Tutorial:** These [slides](https://docs.google.com/presentation/d/14pbd9LTXzfPSJHyXYkfLxnK8Q80LhVnjImg8a3WqCRM/edit?usp=sharing) provide a Chemprop tutorial and highlight recent additions as of April 28th, 2020.
```

### Comparing `chemprop-1.6.0/README.md` & `chemprop-1.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ![ChemProp Logo](docs/source/_static/images/chemprop_logo.svg)
 # Molecular Property Prediction
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/chemprop)](https://badge.fury.io/py/chemprop)
 [![PyPI version](https://badge.fury.io/py/chemprop.svg)](https://badge.fury.io/py/chemprop)
 [![Build Status](https://github.com/chemprop/chemprop/workflows/tests/badge.svg)](https://github.com/chemprop/chemprop)
 
-This repository contains message passing neural networks for molecular property prediction as described in the paper [Analyzing Learned Molecular Representations for Property Prediction](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.9b00237) and as used in the paper [A Deep Learning Approach to Antibiotic Discovery](https://www.cell.com/cell/fulltext/S0092-8674(20)30102-1) for molecules and [Machine Learning of Reaction Properties via Learned Representations of the Condensed Graph of Reaction](https://doi.org/10.1021/acs.jcim.1c00975) for reactions.
+This repository contains message passing neural networks for molecular property prediction as initially described in the paper [Analyzing Learned Molecular Representations for Property Prediction](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.9b00237) and as used in the paper [A Deep Learning Approach to Antibiotic Discovery](https://www.cell.com/cell/fulltext/S0092-8674(20)30102-1) for molecules and [Machine Learning of Reaction Properties via Learned Representations of the Condensed Graph of Reaction](https://doi.org/10.1021/acs.jcim.1c00975) for reactions. Chemprop now also has its own dedicated manuscript: [Chemprop: Machine Learning Package for Chemical Property Prediction](https://doi.org/10.26434/chemrxiv-2023-3zcfl). Please cite us if Chemprop is helpful to your research.
 
 **Documentation:** Full documentation of Chemprop is available at https://chemprop.readthedocs.io/en/latest/.
 
 **Website:** A web prediction interface with some trained Chemprop models is available at [chemprop.csail.mit.edu](http://chemprop.csail.mit.edu).
 
 **Tutorial:** These [slides](https://docs.google.com/presentation/d/14pbd9LTXzfPSJHyXYkfLxnK8Q80LhVnjImg8a3WqCRM/edit?usp=sharing) provide a Chemprop tutorial and highlight recent additions as of April 28th, 2020.
```

### Comparing `chemprop-1.6.0/chemprop/args.py` & `chemprop-1.6.1/chemprop/args.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/data/__init__.py` & `chemprop-1.6.1/chemprop/data/__init__.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/data/data.py` & `chemprop-1.6.1/chemprop/data/data.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/data/scaffold.py` & `chemprop-1.6.1/chemprop/data/scaffold.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections import defaultdict
 import logging
 from random import Random
 from typing import Dict, List, Set, Tuple, Union
 import warnings
+import copy
 
 from rdkit import Chem
 from rdkit.Chem.Scaffolds import MurckoScaffold
 from tqdm import tqdm
 import numpy as np
 
 from .data import MoleculeDataset, make_mol
@@ -19,15 +20,17 @@
     :param mol: A SMILES or an RDKit molecule.
     :param include_chirality: Whether to include chirality in the computed scaffold..
     :return: The Bemis-Murcko scaffold for the molecule.
     """
     if isinstance(mol, str):
         mol = make_mol(mol, keep_h = False, add_h = False, keep_atom_map = False)
     if isinstance(mol, tuple):
-        mol = mol[0]
+        mol = copy.deepcopy(mol[0])
+        for atom in mol.GetAtoms():
+            atom.SetAtomMapNum(0)
     scaffold = MurckoScaffold.MurckoScaffoldSmiles(mol = mol, includeChirality = include_chirality)
 
     return scaffold
 
 
 def scaffold_to_smiles(mols: Union[List[str], List[Chem.Mol], List[Tuple[Chem.Mol, Chem.Mol]]],
                        use_indices: bool = False) -> Dict[str, Union[Set[str], Set[int]]]:
```

### Comparing `chemprop-1.6.0/chemprop/data/scaler.py` & `chemprop-1.6.1/chemprop/data/scaler.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/data/utils.py` & `chemprop-1.6.1/chemprop/data/utils.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/features/__init__.py` & `chemprop-1.6.1/chemprop/features/__init__.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/features/features_generators.py` & `chemprop-1.6.1/chemprop/features/features_generators.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/features/featurization.py` & `chemprop-1.6.1/chemprop/features/featurization.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     return False
 
 
 def is_keeping_atom_map(is_mol: bool = True) -> bool:
     r"""Returns whether to keep the original atom mapping (not for reactions)"""
     if is_mol:
         return PARAMS.KEEP_ATOM_MAP
-    return False
+    return True
 
 
 def is_reaction(is_mol: bool = True) -> bool:
     r"""Returns whether to use reactions as input"""
     if is_mol:
         return False
     if PARAMS.REACTION: #(and not is_mol, checked above)
@@ -333,22 +333,23 @@
         :param overwrite_default_atom_features: Boolean to overwrite default atom features by atom_features instead of concatenating.
         :param overwrite_default_bond_features: Boolean to overwrite default bond features by bond_features instead of concatenating.
         """
         self.is_mol = is_mol(mol)
         self.is_reaction = is_reaction(self.is_mol)
         self.is_explicit_h = is_explicit_h(self.is_mol)
         self.is_adding_hs = is_adding_hs(self.is_mol)
+        self.is_keeping_atom_map = is_keeping_atom_map(self.is_mol)
         self.reaction_mode = reaction_mode()
         
         # Convert SMILES to RDKit molecule if necessary
         if type(mol) == str:
             if self.is_reaction:
-                mol = (make_mol(mol.split(">")[0], self.is_explicit_h, self.is_adding_hs, self.is_keeping_atom_map_list), make_mol(mol.split(">")[-1], self.is_explicit_h, self.is_adding_hs, self.is_keeping_atom_map_list)) 
+                mol = (make_mol(mol.split(">")[0], self.is_explicit_h, self.is_adding_hs, self.is_keeping_atom_map), make_mol(mol.split(">")[-1], self.is_explicit_h, self.is_adding_hs, self.is_keeping_atom_map)) 
             else:
-                mol = make_mol(mol, self.is_explicit_h, self.is_adding_hs, self.is_keeping_atom_map_list)
+                mol = make_mol(mol, self.is_explicit_h, self.is_adding_hs, self.is_keeping_atom_map)
 
         self.n_atoms = 0  # number of atoms
         self.n_bonds = 0  # number of bonds
         self.f_atoms = []  # mapping from atom index to atom features
         self.f_bonds = []  # mapping from bond index to concat(in_atom, bond) features
         self.a2b = []  # mapping from atom index to incoming bond indices
         self.b2a = []  # mapping from bond index to the index of the atom the bond is coming from
```

### Comparing `chemprop-1.6.0/chemprop/features/utils.py` & `chemprop-1.6.1/chemprop/features/utils.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/hyperopt_utils.py` & `chemprop-1.6.1/chemprop/hyperopt_utils.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/hyperparameter_optimization.py` & `chemprop-1.6.1/chemprop/hyperparameter_optimization.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/interpret.py` & `chemprop-1.6.1/chemprop/interpret.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/models/ffn.py` & `chemprop-1.6.1/chemprop/models/ffn.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/models/model.py` & `chemprop-1.6.1/chemprop/models/model.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/models/mpn.py` & `chemprop-1.6.1/chemprop/models/mpn.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/multitask_utils.py` & `chemprop-1.6.1/chemprop/multitask_utils.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/nn_utils.py` & `chemprop-1.6.1/chemprop/nn_utils.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/rdkit.py` & `chemprop-1.6.1/chemprop/rdkit.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     :param s: SMILES string.
     :param keep_h: Boolean whether to keep hydrogens in the input smiles. This does not add hydrogens, it only keeps them if they are specified.
     :param add_h: Boolean whether to add hydrogens to the input smiles.
     :param keep_atom_map: Boolean whether to keep the original atom mapping.
     :return: RDKit molecule.
     """
     params = Chem.SmilesParserParams()
-    params.removeHs = not keep_h if not keep_atom_map else False
+    params.removeHs = not keep_h
     mol = Chem.MolFromSmiles(s, params)
 
     if add_h:
         mol = Chem.AddHs(mol)
 
     if keep_atom_map and mol is not None:
         atom_map_numbers = tuple(atom.GetAtomMapNum() for atom in mol.GetAtoms())
```

### Comparing `chemprop-1.6.0/chemprop/sklearn_predict.py` & `chemprop-1.6.1/chemprop/sklearn_predict.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/sklearn_train.py` & `chemprop-1.6.1/chemprop/sklearn_train.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/spectra_utils.py` & `chemprop-1.6.1/chemprop/spectra_utils.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/train/__init__.py` & `chemprop-1.6.1/chemprop/train/__init__.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/train/cross_validate.py` & `chemprop-1.6.1/chemprop/train/cross_validate.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/train/evaluate.py` & `chemprop-1.6.1/chemprop/train/evaluate.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/train/loss_functions.py` & `chemprop-1.6.1/chemprop/train/loss_functions.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/train/make_predictions.py` & `chemprop-1.6.1/chemprop/train/make_predictions.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/train/metrics.py` & `chemprop-1.6.1/chemprop/train/metrics.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/train/molecule_fingerprint.py` & `chemprop-1.6.1/chemprop/train/molecule_fingerprint.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/train/predict.py` & `chemprop-1.6.1/chemprop/train/predict.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/train/run_training.py` & `chemprop-1.6.1/chemprop/train/run_training.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/train/train.py` & `chemprop-1.6.1/chemprop/train/train.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/uncertainty/__init__.py` & `chemprop-1.6.1/chemprop/uncertainty/__init__.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/uncertainty/uncertainty_calibrator.py` & `chemprop-1.6.1/chemprop/uncertainty/uncertainty_calibrator.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/uncertainty/uncertainty_estimator.py` & `chemprop-1.6.1/chemprop/uncertainty/uncertainty_estimator.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/uncertainty/uncertainty_evaluator.py` & `chemprop-1.6.1/chemprop/uncertainty/uncertainty_evaluator.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/uncertainty/uncertainty_predictor.py` & `chemprop-1.6.1/chemprop/uncertainty/uncertainty_predictor.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/utils.py` & `chemprop-1.6.1/chemprop/utils.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/web/app/db.py` & `chemprop-1.6.1/chemprop/web/app/db.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/web/app/views.py` & `chemprop-1.6.1/chemprop/web/app/views.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/web/run.py` & `chemprop-1.6.1/chemprop/web/run.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/web/utils.py` & `chemprop-1.6.1/chemprop/web/utils.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop/web/wsgi.py` & `chemprop-1.6.1/chemprop/web/wsgi.py`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/chemprop.egg-info/PKG-INFO` & `chemprop-1.6.1/chemprop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chemprop
-Version: 1.6.0
+Version: 1.6.1
 Summary: Molecular Property Prediction with Message Passing Neural Networks
 Home-page: https://github.com/chemprop/chemprop
-Download-URL: https://github.com/chemprop/chemprop/v_1.6.0.tar.gz
+Download-URL: https://github.com/chemprop/chemprop/v_1.6.1.tar.gz
 Author: Kyle Swanson, Kevin Yang, Wengong Jin, Lior Hirschfeld, Allison Tam
 Author-email: chemprop@mit.edu
 License: MIT
 Project-URL: Documentation, https://chemprop.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/chemprop/chemprop
 Project-URL: PyPi, https://pypi.org/project/chemprop/
 Project-URL: Demo, http://chemprop.csail.mit.edu/
@@ -25,15 +25,15 @@
 ![ChemProp Logo](docs/source/_static/images/chemprop_logo.svg)
 # Molecular Property Prediction
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/chemprop)](https://badge.fury.io/py/chemprop)
 [![PyPI version](https://badge.fury.io/py/chemprop.svg)](https://badge.fury.io/py/chemprop)
 [![Build Status](https://github.com/chemprop/chemprop/workflows/tests/badge.svg)](https://github.com/chemprop/chemprop)
 
-This repository contains message passing neural networks for molecular property prediction as described in the paper [Analyzing Learned Molecular Representations for Property Prediction](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.9b00237) and as used in the paper [A Deep Learning Approach to Antibiotic Discovery](https://www.cell.com/cell/fulltext/S0092-8674(20)30102-1) for molecules and [Machine Learning of Reaction Properties via Learned Representations of the Condensed Graph of Reaction](https://doi.org/10.1021/acs.jcim.1c00975) for reactions.
+This repository contains message passing neural networks for molecular property prediction as initially described in the paper [Analyzing Learned Molecular Representations for Property Prediction](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.9b00237) and as used in the paper [A Deep Learning Approach to Antibiotic Discovery](https://www.cell.com/cell/fulltext/S0092-8674(20)30102-1) for molecules and [Machine Learning of Reaction Properties via Learned Representations of the Condensed Graph of Reaction](https://doi.org/10.1021/acs.jcim.1c00975) for reactions. Chemprop now also has its own dedicated manuscript: [Chemprop: Machine Learning Package for Chemical Property Prediction](https://doi.org/10.26434/chemrxiv-2023-3zcfl). Please cite us if Chemprop is helpful to your research.
 
 **Documentation:** Full documentation of Chemprop is available at https://chemprop.readthedocs.io/en/latest/.
 
 **Website:** A web prediction interface with some trained Chemprop models is available at [chemprop.csail.mit.edu](http://chemprop.csail.mit.edu).
 
 **Tutorial:** These [slides](https://docs.google.com/presentation/d/14pbd9LTXzfPSJHyXYkfLxnK8Q80LhVnjImg8a3WqCRM/edit?usp=sharing) provide a Chemprop tutorial and highlight recent additions as of April 28th, 2020.
```

### Comparing `chemprop-1.6.0/chemprop.egg-info/SOURCES.txt` & `chemprop-1.6.1/chemprop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chemprop-1.6.0/setup.cfg` & `chemprop-1.6.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [metadata]
 name = chemprop
-version = 1.6.0
+version = 1.6.1
 author = Kyle Swanson, Kevin Yang, Wengong Jin, Lior Hirschfeld, Allison Tam
 author_email = chemprop@mit.edu
 license = MIT
 description = Molecular Property Prediction with Message Passing Neural Networks
 keywords = 
 	chemistry
 	machine learning
 	property prediction
 	message passing neural network
 	graph neural network
 url = https://github.com/chemprop/chemprop
-download_url = https://github.com/chemprop/chemprop/v_1.6.0.tar.gz
+download_url = https://github.com/chemprop/chemprop/v_1.6.1.tar.gz
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	License :: OSI Approved :: MIT License
@@ -33,18 +33,18 @@
 	flask>=1.1.2
 	hyperopt>=0.2.3
 	matplotlib>=3.1.3
 	numpy>=1.18.1
 	pandas>=1.0.3
 	pandas-flavor>=0.2.0
 	scikit-learn>=0.22.2.post1
-	scipy>=1.6.0
+	scipy>=1.4.1
 	sphinx>=3.1.2
 	tensorboardX>=2.0
-	torch>=1.6.0
+	torch>=1.4.0
 	tqdm>=4.45.0
 	typed-argument-parser>=1.6.1
 	rdkit>=2020.03.1.0
 	descriptastorus
 python_requires = >=3.7
 
 [options.entry_points]
```

### Comparing `chemprop-1.6.0/setup.py` & `chemprop-1.6.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,74 @@
 from setuptools import find_packages, setup
 
-__version__ = "1.6.0"
+__version__ = "1.6.1"
 
 # Load README
-with open('README.md', encoding='utf-8') as f:
+with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-    name='chemprop',
-    author='Kyle Swanson, Kevin Yang, Wengong Jin, Lior Hirschfeld, Allison Tam',
-    author_email='chemprop@mit.edu',
-    description='Molecular Property Prediction with Message Passing Neural Networks',
+    name="chemprop",
+    author="Kyle Swanson, Kevin Yang, Wengong Jin, Lior Hirschfeld, Allison Tam",
+    author_email="chemprop@mit.edu",
+    description="Molecular Property Prediction with Message Passing Neural Networks",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/chemprop/chemprop',
-    download_url=f'https://github.com/chemprop/chemprop/v_{__version__}.tar.gz',
+    long_description_content_type="text/markdown",
+    url="https://github.com/chemprop/chemprop",
+    download_url=f"https://github.com/chemprop/chemprop/v_{__version__}.tar.gz",
     project_urls={
-        'Documentation': 'https://chemprop.readthedocs.io/en/latest/',
-        'Source': 'https://github.com/chemprop/chemprop',
-        'PyPi': 'https://pypi.org/project/chemprop/',
-        'Demo': 'http://chemprop.csail.mit.edu/',
+        "Documentation": "https://chemprop.readthedocs.io/en/latest/",
+        "Source": "https://github.com/chemprop/chemprop",
+        "PyPi": "https://pypi.org/project/chemprop/",
+        "Demo": "http://chemprop.csail.mit.edu/",
     },
-    license='MIT',
+    license="MIT",
     packages=find_packages(),
-    package_data={'chemprop': ['py.typed']},
+    package_data={"chemprop": ["py.typed"]},
     entry_points={
-        'console_scripts': [
-            'chemprop_train=chemprop.train:chemprop_train',
-            'chemprop_predict=chemprop.train:chemprop_predict',
-            'chemprop_fingerprint=chemprop.train:chemprop_fingerprint',
-            'chemprop_hyperopt=chemprop.hyperparameter_optimization:chemprop_hyperopt',
-            'chemprop_interpret=chemprop.interpret:chemprop_interpret',
-            'chemprop_web=chemprop.web.run:chemprop_web',
-            'sklearn_train=chemprop.sklearn_train:sklearn_train',
-            'sklearn_predict=chemprop.sklearn_predict:sklearn_predict',
+        "console_scripts": [
+            "chemprop_train=chemprop.train:chemprop_train",
+            "chemprop_predict=chemprop.train:chemprop_predict",
+            "chemprop_fingerprint=chemprop.train:chemprop_fingerprint",
+            "chemprop_hyperopt=chemprop.hyperparameter_optimization:chemprop_hyperopt",
+            "chemprop_interpret=chemprop.interpret:chemprop_interpret",
+            "chemprop_web=chemprop.web.run:chemprop_web",
+            "sklearn_train=chemprop.sklearn_train:sklearn_train",
+            "sklearn_predict=chemprop.sklearn_predict:sklearn_predict",
         ]
     },
     install_requires=[
-        'flask>=1.1.2',
-        'hyperopt>=0.2.3',
-        'matplotlib>=3.1.3',
-        'numpy>=1.18.1',
-        'pandas>=1.0.3',
-        'pandas-flavor>=0.2.0',
-        'scikit-learn>=0.22.2.post1',
-        'scipy>=1.6.0',
-        'sphinx>=3.1.2',
-        'tensorboardX>=2.0',
-        'torch>=1.6.0',
-        'tqdm>=4.45.0',
-        'typed-argument-parser>=1.6.1',
-        'rdkit>=2020.03.1.0',
-        'descriptastorus'
+        "flask>=1.1.2",
+        "hyperopt>=0.2.3",
+        "matplotlib>=3.1.3",
+        "numpy>=1.18.1",
+        "pandas>=1.0.3",
+        "pandas-flavor>=0.2.0",
+        "scikit-learn>=0.22.2.post1",
+        "sphinx>=3.1.2",
+        "tensorboardX>=2.0",
+        "torch>=1.4.0",
+        "tqdm>=4.45.0",
+        "typed-argument-parser>=1.6.1",
+        "rdkit>=2020.03.1.0",
+        "scipy<1.11 ; python_version=='3.7'",
+        "descriptastorus<2.6.1 ; python_version=='3.7'",
+        "scipy>=1.9 ; python_version=='3.8'",
+        "descriptastorus>=2.6.1 ; python_version=='3.8'",
     ],
-    extras_require={
-        'test': [
-            'pytest>=6.2.2',
-            'parameterized>=0.8.1'
-        ]
-    },
-    python_requires='>=3.7',
+    extras_require={"test": ["pytest>=6.2.2", "parameterized>=0.8.1"]},
+    python_requires=">=3.7",
     classifiers=[
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent'
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
     ],
     keywords=[
-        'chemistry',
-        'machine learning',
-        'property prediction',
-        'message passing neural network',
-        'graph neural network'
-    ]
+        "chemistry",
+        "machine learning",
+        "property prediction",
+        "message passing neural network",
+        "graph neural network",
+    ],
 )
```

### Comparing `chemprop-1.6.0/tests/test_integration.py` & `chemprop-1.6.1/tests/test_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -813,15 +813,15 @@
                 'chemprop',
                 2.3338595,
                 ['--reaction', '--data_path', os.path.join(TEST_DATA_DIR, 'reaction_regression.csv')]
         ),
         (
                 'chemprop_scaffold_split',
                 'chemprop',
-                2.11470476,
+                2.095871,
                 ['--reaction', '--data_path', os.path.join(TEST_DATA_DIR, 'reaction_regression.csv'),'--split_type', 'scaffold_balanced']
         ),
         (
                 'chemprop_morgan_features_generator',
                 'chemprop',
                 3.122113679,
                 ['--reaction', '--data_path', os.path.join(TEST_DATA_DIR, 'reaction_regression.csv'),'--features_generator', 'morgan']
@@ -1028,15 +1028,15 @@
                 2.984292677,
                 ['--reaction_solvent', '--number_of_molecules', '2',
                  '--data_path', os.path.join(TEST_DATA_DIR, 'reaction_solvent_regression.csv'), '--explicit_h', '--adding_h']
         ),
         (
                 'chemprop_reaction_solvent_diff_mpn_size',
                 'chemprop',
-                2.899513794,
+                2.734318,
                 ['--reaction_solvent', '--number_of_molecules', '2',
                  '--data_path', os.path.join(TEST_DATA_DIR, 'reaction_solvent_regression.csv'), '--hidden_size', '500',
                  '--hidden_size_solvent', '250']
         )
     ])
     def test_train_single_task_regression_reaction_solvent(self,
                                           name: str,
```

