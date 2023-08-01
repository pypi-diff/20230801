# Comparing `tmp/sarus-0.7.4.dev2.tar.gz` & `tmp/sarus-0.7.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus-0.7.4.dev2.tar", last modified: Mon Jul  3 19:54:27 2023, max compression
+gzip compressed data, was "sarus-0.7.5rc0.tar", last modified: Tue Aug  1 13:17:33 2023, max compression
```

## Comparing `sarus-0.7.4.dev2.tar` & `sarus-0.7.5rc0.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.202402 sarus-0.7.4.dev2/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/MANIFEST.in
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1558 2023-07-03 19:54:27.202402 sarus-0.7.4.dev2/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2021-08-24 10:18:30.000000 sarus-0.7.4.dev2/README.rst
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2021-09-06 19:14:48.000000 sarus-0.7.4.dev2/pyproject.toml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.182402 sarus-0.7.4.dev2/sarus/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      549 2023-07-03 19:53:43.000000 sarus-0.7.4.dev2/sarus/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13201 2023-06-07 13:55:59.000000 sarus-0.7.4.dev2/sarus/config.yaml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.186402 sarus-0.7.4.dev2/sarus/context/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/context/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3137 2023-06-07 13:55:59.000000 sarus-0.7.4.dev2/sarus/context/local_sdk.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      345 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/context/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13990 2023-06-07 13:55:59.000000 sarus-0.7.4.dev2/sarus/dataspec_wrapper.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      743 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/debug.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.186402 sarus-0.7.4.dev2/sarus/imblearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      265 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/imblearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/imblearn/over_sampling.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/imblearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/imblearn/under_sampling.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.186402 sarus-0.7.4.dev2/sarus/legacy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/legacy/__init__.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.186402 sarus-0.7.4.dev2/sarus/legacy/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/legacy/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/legacy/tensorflow/dataset.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/legacy/tensorflow/model.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.190402 sarus-0.7.4.dev2/sarus/manager/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/manager/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5490 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/manager/arrow_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1927 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/manager/arrow_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1296 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/manager/base_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3869 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/manager/cache_scalar_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     8719 2023-06-22 14:51:31.000000 sarus-0.7.4.dev2/sarus/manager/dataspec_api.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.190402 sarus-0.7.4.dev2/sarus/manager/ops/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/manager/ops/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      688 2023-06-07 13:55:59.000000 sarus-0.7.4.dev2/sarus/manager/ops/api.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3487 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/manager/parquet_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    20367 2023-07-03 19:53:57.000000 sarus-0.7.4.dev2/sarus/manager/sdk_manager.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2650 2023-06-07 13:55:59.000000 sarus-0.7.4.dev2/sarus/manager/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4729 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/manager/value_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1573 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/manager/value_remote.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.190402 sarus-0.7.4.dev2/sarus/numpy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      337 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/numpy/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/numpy/random.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/numpy/scalars.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.190402 sarus-0.7.4.dev2/sarus/pandas/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      197 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/pandas/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      838 2023-06-07 13:55:59.000000 sarus-0.7.4.dev2/sarus/pandas/core.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4843 2023-06-07 13:55:59.000000 sarus-0.7.4.dev2/sarus/pandas/dataframe.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/pandas/io.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.190402 sarus-0.7.4.dev2/sarus/pandas_profiling/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/pandas_profiling/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      377 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/pandas_profiling/profile_report.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.190402 sarus-0.7.4.dev2/sarus/plotly/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      108 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/plotly/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      138 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/plotly/express.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    43166 2023-06-22 14:49:08.000000 sarus-0.7.4.dev2/sarus/sarus.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.190402 sarus-0.7.4.dev2/sarus/scripts/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/scripts/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4672 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/scripts/generate_op_list.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.198402 sarus-0.7.4.dev2/sarus/sklearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      680 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6604 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/cluster.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      766 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/compose.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      814 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/decomposition.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    11437 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/ensemble.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      566 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/impute.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      177 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/inspection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/linear_model.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/metrics.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1073 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/model_selection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1571 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/preprocessing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/sklearn/svm.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.198402 sarus-0.7.4.dev2/sarus/skopt/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      223 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/skopt/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      929 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/skopt/searchcv.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.202402 sarus-0.7.4.dev2/sarus/std/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      154 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/std/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1600 2023-06-07 13:55:59.000000 sarus-0.7.4.dev2/sarus/std/types.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.202402 sarus-0.7.4.dev2/sarus/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1831 2023-06-07 13:55:59.000000 sarus-0.7.4.dev2/sarus/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    10848 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/utils.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1461 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/wrapper_factory.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.202402 sarus-0.7.4.dev2/sarus/xgboost/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/xgboost/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      754 2023-05-23 10:20:26.000000 sarus-0.7.4.dev2/sarus/xgboost/xgboost.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.186402 sarus-0.7.4.dev2/sarus.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1558 2023-07-03 19:54:27.000000 sarus-0.7.4.dev2/sarus.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1965 2023-07-03 19:54:27.000000 sarus-0.7.4.dev2/sarus.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-07-03 19:54:27.000000 sarus-0.7.4.dev2/sarus.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-08-30 08:41:07.000000 sarus-0.7.4.dev2/sarus.egg-info/not-zip-safe
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      364 2023-07-03 19:54:27.000000 sarus-0.7.4.dev2/sarus.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2023-07-03 19:54:27.000000 sarus-0.7.4.dev2/sarus.egg-info/top_level.txt
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1326 2023-07-03 19:54:27.206402 sarus-0.7.4.dev2/setup.cfg
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      111 2023-07-03 19:53:24.000000 sarus-0.7.4.dev2/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-03 19:54:27.202402 sarus-0.7.4.dev2/tests/
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2021-09-06 19:14:48.000000 sarus-0.7.4.dev2/tests/test_sanity.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:17:33.023568 sarus-0.7.5rc0/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/MANIFEST.in
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1556 2023-08-01 13:17:33.023568 sarus-0.7.5rc0/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/README.rst
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/pyproject.toml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:17:33.015586 sarus-0.7.5rc0/sarus/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      548 2023-08-01 13:17:11.000000 sarus-0.7.5rc0/sarus/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13718 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/config.yaml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:17:33.015586 sarus-0.7.5rc0/sarus/context/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/context/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3136 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/context/local_sdk.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      345 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/context/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    15091 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/dataspec_wrapper.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      743 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/debug.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:17:33.019577 sarus-0.7.5rc0/sarus/imblearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      265 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/imblearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/imblearn/over_sampling.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/imblearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/imblearn/under_sampling.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:17:33.019577 sarus-0.7.5rc0/sarus/legacy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/legacy/__init__.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:17:33.019577 sarus-0.7.5rc0/sarus/legacy/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/legacy/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/legacy/tensorflow/dataset.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/legacy/tensorflow/model.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:17:33.019577 sarus-0.7.5rc0/sarus/manager/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/manager/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5684 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/manager/arrow_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1927 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/manager/arrow_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1296 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/manager/base_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3869 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/manager/cache_scalar_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     8755 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/manager/dataspec_api.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:17:33.019577 sarus-0.7.5rc0/sarus/manager/ops/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/manager/ops/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      688 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/manager/ops/api.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3487 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/manager/parquet_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    21753 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/manager/sdk_manager.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2650 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/manager/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4729 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/manager/value_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1573 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/manager/value_remote.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:17:33.019577 sarus-0.7.5rc0/sarus/numpy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      337 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/numpy/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/numpy/random.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/numpy/scalars.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:17:33.019577 sarus-0.7.5rc0/sarus/pandas/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      197 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/pandas/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      838 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/pandas/core.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4843 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/pandas/dataframe.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/pandas/io.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:17:33.019577 sarus-0.7.5rc0/sarus/pandas_profiling/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/pandas_profiling/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      377 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/pandas_profiling/profile_report.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:17:33.019577 sarus-0.7.5rc0/sarus/plotly/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      108 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/plotly/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      138 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/plotly/express.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    43166 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/sarus.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:17:33.023568 sarus-0.7.5rc0/sarus/scripts/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/scripts/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4672 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/scripts/generate_op_list.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2935 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/serialization.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:17:33.023568 sarus-0.7.5rc0/sarus/sklearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      680 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/sklearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6604 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/sklearn/cluster.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      766 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/sklearn/compose.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      814 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/sklearn/decomposition.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    11437 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/sklearn/ensemble.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      566 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/sklearn/impute.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      177 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/sklearn/inspection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/sklearn/linear_model.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/sklearn/metrics.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1073 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/sklearn/model_selection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/sklearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1571 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/sklearn/preprocessing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/sklearn/svm.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:17:33.023568 sarus-0.7.5rc0/sarus/skopt/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      223 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/skopt/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      929 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/skopt/searchcv.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:17:33.023568 sarus-0.7.5rc0/sarus/std/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      154 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/std/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2726 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/std/types.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:17:33.023568 sarus-0.7.5rc0/sarus/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2539 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13563 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/utils.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2344 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/wrapper_factory.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:17:33.023568 sarus-0.7.5rc0/sarus/xgboost/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/xgboost/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      754 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/sarus/xgboost/xgboost.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:17:33.015586 sarus-0.7.5rc0/sarus.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1556 2023-08-01 13:17:32.000000 sarus-0.7.5rc0/sarus.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1988 2023-08-01 13:17:32.000000 sarus-0.7.5rc0/sarus.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-08-01 13:17:32.000000 sarus-0.7.5rc0/sarus.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-08-01 13:17:32.000000 sarus-0.7.5rc0/sarus.egg-info/not-zip-safe
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      359 2023-08-01 13:17:32.000000 sarus-0.7.5rc0/sarus.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2023-08-01 13:17:32.000000 sarus-0.7.5rc0/sarus.egg-info/top_level.txt
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1321 2023-08-01 13:17:33.023568 sarus-0.7.5rc0/setup.cfg
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      110 2023-08-01 13:16:27.000000 sarus-0.7.5rc0/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-08-01 13:17:33.023568 sarus-0.7.5rc0/tests/
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2023-08-01 13:15:29.000000 sarus-0.7.5rc0/tests/test_sanity.py
```

### Comparing `sarus-0.7.4.dev2/PKG-INFO` & `sarus-0.7.5rc0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.7.4.dev2
+Version: 0.7.5rc0
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.7.4.dev2/README.rst` & `sarus-0.7.5rc0/README.rst`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/__init__.py` & `sarus-0.7.5rc0/sarus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         std,
         xgboost,
     )
 
     from .sarus import Client, Dataset
     from .utils import eval, eval_policy, floating, integer, length
 
-VERSION = "0.7.4.dev2"
+VERSION = "0.7.5.rc0"
 
 __all__ = [
     "Dataset",
     "Client",
     "length",
     "eval",
     "eval_policy",
```

### Comparing `sarus-0.7.4.dev2/sarus/config.yaml` & `sarus-0.7.5rc0/sarus/config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -29,14 +29,28 @@
         __neg__: std.NEG
         _sudo: std.SUDO
   std:
     classes:
       Dict:
         keys: std.KEYS
         values: std.VALUES
+      String:
+        casefold: std.CASEFOLD
+        center: std.CENTER
+        capitalize: std.CAPITALIZE
+        expandtabs: std.EXPANDTABS
+        join: std.JOIN
+        lower: std.LOWER
+        lstrip: std.LSTRIP
+        replace: std.REPLACE
+        rstrip: std.RSTRIP
+        split: std.SPLIT
+        splitlines: std.SPLITLINES
+        strip: std.STRIP
+        upper: std.UPPER
   pandas:
     sarus_functions:
       get_dummies: pandas.PD_GET_DUMMIES
       to_datetime: pandas.PD_TO_DATETIME
       merge: pandas.PD_MERGE
       concat: pandas.PD_CONCAT
     core:
@@ -103,14 +117,16 @@
           __eq__: pandas.PD_EQ
           __getitem__: pandas.PD_GETITEM
           abs: pandas.PD_ABS
           add: pandas.PD_ADD
           agg: pandas.PD_AGG
           any: pandas.PD_ANY
           append: pandas.PD_APPEND
+          apply: pandas.PD_APPLY
+          applymap: pandas.PD_APPLYMAP
           astype: pandas.PD_ASTYPE
           count: pandas.PD_COUNT
           corr: pandas.PD_CORR
           describe: pandas.PD_DESCRIBE
           drop: pandas.PD_DROP
           dropna: pandas.PD_DROPNA
           drop_duplicates: pandas.PD_DROP_DUPLICATES
@@ -149,14 +165,15 @@
           __eq__: pandas.PD_EQ
           __getitem__: pandas.PD_GETITEM
           abs: pandas.PD_ABS
           add: pandas.PD_ADD
           agg: pandas.PD_AGG
           any: pandas.PD_ANY
           append: pandas.PD_APPEND
+          apply: pandas.PD_APPLY
           astype: pandas.PD_ASTYPE
           corr: pandas.PD_CORR_SERIES
           count: pandas.PD_COUNT
           describe: pandas.PD_DESCRIBE
           drop: pandas.PD_DROP
           dropna: pandas.PD_DROPNA
           drop_duplicates: pandas.PD_DROP_DUPLICATES
@@ -165,14 +182,15 @@
           groupby: pandas.PD_GROUPBY
           head: pandas.PD_HEAD
           isin: pandas.PD_ISIN
           isnull: pandas.PD_ISNULL
           join: pandas.PD_JOIN
           kurtosis: pandas.PD_KURTOSIS
           mad: pandas.PD_MAD
+          map: pandas.PD_MAP
           mask: pandas.PD_MASK
           mean: pandas.PD_MEAN
           median: pandas.PD_MEDIAN
           notnull: pandas.PD_NOTNULL
           quantile: pandas.PD_QUANTILE
           reindex: pandas.PD_REINDEX
           rename: pandas.PD_RENAME
```

### Comparing `sarus-0.7.4.dev2/sarus/context/local_sdk.py` & `sarus-0.7.5rc0/sarus/context/local_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import sarus_data_spec.protobuf as sp
 from sarus_data_spec.attribute import Attribute
 from sarus_data_spec.context.public import Public as PublicContext
 from sarus_data_spec.dataset import Dataset
 from sarus_data_spec.factory import Factory
 from sarus_data_spec.scalar import Scalar
 from sarus_data_spec.schema import Schema
-
 from sarus_data_spec.storage.local import Storage
 from sarus_data_spec.transform import Transform
 from sarus_data_spec.variant_constraint import VariantConstraint
 
 from sarus.dataspec_wrapper import MetaWrapper
 from sarus.manager.sdk_manager import SDKManager, manager
 from sarus.typing import Client
```

### Comparing `sarus-0.7.4.dev2/sarus/dataspec_wrapper.py` & `sarus-0.7.5rc0/sarus/dataspec_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     get_args,
 )
 
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 from sarus_data_spec.context import global_context
 from sarus_data_spec.dataspec_validator.typing import DataspecPrivacyPolicy
+from sarus_data_spec.transform import variable
 
 from sarus.context.typing import LocalSDKContext
 from sarus.manager.typing import SDKManager
 from sarus.typing import DataSpecVariant, SyncPolicy
 from sarus.utils import register_ops
 
 logger = logging.getLogger(__name__)
@@ -104,29 +105,48 @@
         We don't use the __init__ method because the __new__ method may be
         overwritten by the `sarus.utils.init_wrapped` decorator.
         """
         wrapper = object.__new__(cls)
         wrapper._set_dataspec(dataspec)
         return wrapper
 
+    @classmethod
+    def from_value(cls, value: T) -> DataSpecWrapper(Generic[T]):
+        """Construct a DataSpecWrapper by wrapping a Python value."""
+        return cls(value)
+
     def _set_dataspec(self, dataspec: st.DataSpec) -> None:
         self._dataspec = dataspec
         self._alt_dataspec = None
         self._alt_policy = None  # The alternative Dataspec's privacy policy
+        self._traced_transform = None
 
         # This class only works with a LocalSDKContext
         context: LocalSDKContext = global_context()
         assert isinstance(context, LocalSDKContext)
         self._manager = context.manager()
         if context.sync_policy() == SyncPolicy.SEND_ON_INIT:
             self.alternative_dataspec(launch=True)
 
         # Register wrapper instance
         DataSpecWrapper.instances[dataspec.uuid()] = id(self)
 
+    def _set_variable(self, name: str, position: int):
+        """Used to trace callables."""
+        self._traced_transform = variable(name=name, position=position)
+
+    def traced_transform(self) -> Optional[st.Transform]:
+        """Return the wrapper's composed transform or variable when tracing."""
+        return self._traced_transform
+
+    def _set_traced_transform(
+        self, traced_transform: Optional[st.Transform]
+    ) -> None:
+        self._traced_transform = traced_transform
+
     def manager(self) -> SDKManager:
         return self._manager
 
     def python_type(self) -> Optional[str]:
         """Return the value's Python type name.
 
         The SDKManager registers an attribute holding the MOCK value's
@@ -367,20 +387,27 @@
                 message = f"{message} (epsilon={epsilon:.2f})"
 
             print(message)
 
         return value
 
     def __getattr__(self, name: str) -> Any:
+        """Called when trying to access an attribute of the
+        DataSpecWrapper or calling a non-bound method."""
         if name not in IGNORE_WARNING:
             logger.info(
                 f"`{name}` not supported on {type(self)}, "
                 "object has been evaluated for this method. "
                 "See Sarus documentation."
             )
+            if self.traced_transform() is not None:
+                raise NotImplementedError(
+                    f"Cannot trace `{name}`. "
+                    f"Not supported on type {self.__wraps__}"
+                )
             return self.__sarus_eval__().__getattribute__(name)
         else:
             return object.__getattribute__(self, name)
 
     def _ipython_display_(self) -> None:
         display(self.__sarus_eval__())  # noqa: F821
```

### Comparing `sarus-0.7.4.dev2/sarus/debug.py` & `sarus-0.7.5rc0/sarus/debug.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/imblearn/over_sampling.py` & `sarus-0.7.5rc0/sarus/imblearn/over_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/imblearn/pipeline.py` & `sarus-0.7.5rc0/sarus/imblearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/imblearn/under_sampling.py` & `sarus-0.7.5rc0/sarus/imblearn/under_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/legacy/tensorflow/dataset.py` & `sarus-0.7.5rc0/sarus/legacy/tensorflow/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/legacy/tensorflow/model.py` & `sarus-0.7.5rc0/sarus/legacy/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/manager/arrow_local.py` & `sarus-0.7.5rc0/sarus/manager/arrow_local.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 from sarus_data_spec.manager.computations.local.base import LocalComputation
 
 from sarus.manager.arrow_remote import ToArrowComputationOnServer
 from sarus.manager.parquet_local import ToParquetComputation
 
 logger = logging.getLogger(__name__)
 
+# TODO: in SDS some of the default batch_size is 1 and it slows down the SDK by dozen of secondes for large tables
+# to remove when the default batch_size is changes in SDS.
+BATCH_SIZE = 10000
+
 
 class ToArrowComputation(LocalComputation[t.AsyncIterator[pa.RecordBatch]]):
     task_name = ARROW_TASK
 
     def __init__(
         self,
         computing_manager: Base,
@@ -104,15 +108,15 @@
                 await self.parquet_computation.result_from_stage_properties(
                     dataspec, stage.properties()
                 )
             )
             try:
                 ait = async_iter(
                     pq.read_table(source=cache_path).to_batches(
-                        max_chunksize=batch_size
+                        max_chunksize=BATCH_SIZE
                     )
                 )
             except Exception as e:
                 stt.error(
                     dataspec=dataspec,
                     manager=self.computing_manager(),
                     task=self.task_name,
@@ -133,17 +137,17 @@
                 raise stt.DataSpecErrorStatus(
                     (True, traceback.format_exc())
                 ) from e
         elif self.is_computation_remote(dataspec):
             status = self.remote_arrow.status(dataspec)
             ait = await self.remote_arrow.result_from_stage_properties(
                 dataspec,
-                batch_size=batch_size,
+                batch_size=BATCH_SIZE,
                 properties=status.task(
                     self.remote_arrow.task_name
                 ).properties(),
             )
         else:
             ait = await self.computing_manager().async_to_arrow_op(
-                dataset=t.cast(Dataset, dataspec), batch_size=batch_size
+                dataset=t.cast(Dataset, dataspec), batch_size=BATCH_SIZE
             )
         return ErrorCatchingAsyncIterator(ait, dataspec, self)
```

### Comparing `sarus-0.7.4.dev2/sarus/manager/arrow_remote.py` & `sarus-0.7.5rc0/sarus/manager/arrow_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/manager/base_remote.py` & `sarus-0.7.5rc0/sarus/manager/base_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/manager/cache_scalar_local.py` & `sarus-0.7.5rc0/sarus/manager/cache_scalar_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/manager/dataspec_api.py` & `sarus-0.7.5rc0/sarus/manager/dataspec_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 from sarus_data_spec.manager.async_utils import async_iter
 from sarus_data_spec.protobuf.utilities import dict_deserialize, dict_serialize
 
 from sarus.typing import Client
 
 logger = logging.getLogger(__name__)
 
+CHUNK_SIZE = 1024 * 1024
+
 
 def raise_response(resp: Response) -> None:
     """Raise exception with message encapsulated in the response JSON data."""
     if resp.status_code >= HTTPStatus.INTERNAL_SERVER_ERROR:
         resp.raise_for_status()
     if resp.status_code >= HTTPStatus.BAD_REQUEST:
         try:
@@ -249,15 +251,15 @@
     client: Client, uuid: str, batch_size: int
 ) -> t.AsyncIterator[pa.RecordBatch]:
     """Return the dataset's value as a RecordBatch async iterator."""
     resp = dataspec_result_response(client, uuid, batch_size)
     if resp.headers.get("Content-Type") == "application/parquet":
         # Recieving Parquet file
         buffer = io.BytesIO()
-        for data in resp.iter_content():
+        for data in resp.iter_content(CHUNK_SIZE):
             buffer.write(data)
         buffer.seek(0)
         return async_iter(
             pq.read_table(buffer).to_batches(max_chunksize=batch_size)
         )
     else:
         # Recieving serialized streamed record batches
```

### Comparing `sarus-0.7.4.dev2/sarus/manager/ops/api.py` & `sarus-0.7.5rc0/sarus/manager/ops/api.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/manager/parquet_local.py` & `sarus-0.7.5rc0/sarus/manager/parquet_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/manager/sdk_manager.py` & `sarus-0.7.5rc0/sarus/manager/sdk_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 import os
 import tempfile
 import typing as t
 
 import pyarrow as pa
-import requests
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.status as stt
 import sarus_data_spec.storage.typing as storage_typing
 import sarus_data_spec.type as sdt
 import sarus_data_spec.typing as st
 from sarus_data_spec.arrow.type import type_from_arrow
 from sarus_data_spec.attribute import attach_properties
@@ -27,15 +26,14 @@
     TransformedDataset,
     TransformedScalar,
 )
 from sarus_data_spec.manager.ops.source.routing import SourceScalar
 from sarus_data_spec.schema import schema as schema_builder
 
 import sarus.manager.dataspec_api as api
-import sarus.manager.ops.api as api_ops
 from sarus.typing import ADMIN_DS, MOCK, PYTHON_TYPE, Client
 
 from .arrow_local import ToArrowComputation
 from .arrow_remote import ToArrowComputationOnServer
 from .cache_scalar_local import CacheScalarComputation
 from .parquet_local import ToParquetComputation
 from .value_local import ValueComputation
@@ -244,17 +242,18 @@
         """Retreive all items necessary to compute a DataSpec.
 
         This function is used intensively to post DataSpecs, draw dot
         representationss, fetch statuses, and so on.
         """
         storage = self.storage()
 
-        class ComputationGraphVisitor(st.Visitor):
+        class ComputationGraphVisitor(st.Visitor, st.TransformVisitor):
             dataspecs: t.List[st.DataSpec] = list()
             transforms: t.Set[st.Transform] = set()
+            lambdas: t.Set[st.Transform] = set()
             edges: t.Set[
                 t.Tuple[st.DataSpec, st.DataSpec, st.Transform]
             ] = set()
             attributes: t.Set[st.Attribute] = set()
             variant_constraints: t.Set[st.VariantConstraint] = set()
             graph: t.Dict[str, t.Set[str]] = dict()
 
@@ -287,31 +286,59 @@
                         [vc for vc in variant_constraints]
                     )
 
                     self.transforms.add(transform)
                     for argument in arguments:
                         argument.accept(self)
                         self.edges.add((argument, visited, transform))
+                        if isinstance(argument, st.Transform):
+                            self.lambdas.add(argument)
                     for _, argument in named_arguments.items():
                         argument.accept(self)
                         self.edges.add((argument, visited, transform))
+                        if isinstance(argument, st.Transform):
+                            self.lambdas.add(argument)
 
             def other(self, visited: st.DataSpec) -> None:
                 if visited not in self.dataspecs:
+                    assert isinstance(visited, st.DataSpec)
                     self.dataspecs.append(visited)
 
+            def composed(
+                self,
+                visited: st.Transform,
+                transform: st.Transform,
+                *arguments: st.Transform,
+                **named_arguments: st.Transform,
+            ) -> None:
+                self.transforms.add(visited)
+                self.transforms.add(transform)
+                for argument in arguments:
+                    argument.accept(self)
+                for _, argument in named_arguments.items():
+                    argument.accept(self)
+
+            def variable(
+                self,
+                visited: st.Transform,
+                name: str,
+                position: int,
+            ) -> None:
+                self.transforms.add(visited)
+
         visitor = ComputationGraphVisitor()
         dataspec.accept(visitor)
 
         return {
-            "dataspecs": visitor.dataspecs[::-1],
+            "dataspecs": visitor.dataspecs,
             "transforms": visitor.transforms,
             "attributes": visitor.attributes,
             "variant_constraints": visitor.variant_constraints,
             "edges": visitor.edges,
+            "lambdas": visitor.lambdas,
         }
 
     def _delete_local(self, uuid: str) -> None:
         """Delete a DataSpec locally. MOCKs also have to be deleted."""
         would_delete = self.storage().all_referrings(uuid)
         additional_cleanup = []
         for uuid in would_delete:
@@ -339,15 +366,14 @@
         """Graphviz dot language representation of the graph.
 
         Statuses are represented with a color code. The symbols are the
         caller's symbol for the DataSpec wrapper
         (see DataSpecWrapper.dataspec_wrapper_symbols).
         """
         graph = self.computation_graph(dataspec)
-        dataspecs = graph["dataspecs"]
         TASK = (
             ARROW_TASK if dataspec.prototype() == sp.Dataset else SCALAR_TASK
         )
 
         # Get statuses wether remote or local
         if remote:
             statuses_proto = api.pull_dataspec_status_graph(
@@ -355,33 +381,42 @@
             )
             statuses = {
                 proto.dataspec: stt.Status(proto, store=False)
                 for proto in statuses_proto
             }
         else:
             statuses = {
-                ds.uuid(): stt.last_status(ds, task=TASK) for ds in dataspecs
+                ds.uuid(): stt.last_status(ds, task=TASK)
+                for ds in graph["dataspecs"]
             }
 
-        edges, nodes, props = [], [], []
-        for dataspec in dataspecs:
+        edges, nodes, props, lambdas = [], [], [], []
+        for dataspec in graph["dataspecs"]:
             status = statuses.get(dataspec.uuid())
-            nodes.append(self.node_repr(dataspec, status, symbols))
+            nodes.append(self.dataspec_repr(dataspec, status, symbols))
         for parent, child, transform in graph["edges"]:
             edges.append(
                 f'"{parent.uuid()}" -> "{child.uuid()}"'
                 f'[label="{transform.name()}"];'
             )
+        for i, transform in enumerate(graph["lambdas"]):
+            lambdas.append(
+                transform.dot().replace(
+                    'digraph {',
+                    f'subgraph cluster_{i} {{\ncolor=black;\nlabel="Traced function";',
+                )
+            )
+
         props = [
             'node [style="rounded,filled"]',
         ]
-        dot = ["digraph {"] + props + nodes + edges + ["}"]
+        dot = ["digraph {"] + props + nodes + edges + lambdas + ["}"]
         return "\n".join(dot)
 
-    def node_repr(
+    def dataspec_repr(
         self,
         dataspec: st.DataSpec,
         status: t.Optional[st.Status],
         symbols: t.Dict[str, t.Optional[str]],
     ) -> str:
         """Style a graph node depending on its status and symbol."""
         shape = "box"
```

### Comparing `sarus-0.7.4.dev2/sarus/manager/typing.py` & `sarus-0.7.5rc0/sarus/manager/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/manager/value_local.py` & `sarus-0.7.5rc0/sarus/manager/value_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/manager/value_remote.py` & `sarus-0.7.5rc0/sarus/manager/value_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/numpy/scalars.py` & `sarus-0.7.5rc0/sarus/numpy/scalars.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/pandas/core.py` & `sarus-0.7.5rc0/sarus/pandas/core.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/pandas/dataframe.py` & `sarus-0.7.5rc0/sarus/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/sarus.py` & `sarus-0.7.5rc0/sarus/sarus.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -27,20 +27,20 @@
 import getpass
 import hashlib
 import http
 import io
 import json
 import logging
 import os
+import pprint
 import re
 import sys
 import tarfile
 import tempfile
 import textwrap
-import pprint
 import time
 import typing as t
 import warnings
 import webbrowser
 from dataclasses import dataclass
 from io import BytesIO
 from typing import Any, Dict, List, Optional
```

### Comparing `sarus-0.7.4.dev2/sarus/scripts/generate_op_list.py` & `sarus-0.7.5rc0/sarus/scripts/generate_op_list.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/sklearn/__init__.py` & `sarus-0.7.5rc0/sarus/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/sklearn/cluster.py` & `sarus-0.7.5rc0/sarus/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/sklearn/compose.py` & `sarus-0.7.5rc0/sarus/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/sklearn/decomposition.py` & `sarus-0.7.5rc0/sarus/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/sklearn/ensemble.py` & `sarus-0.7.5rc0/sarus/sklearn/ensemble.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/sklearn/impute.py` & `sarus-0.7.5rc0/sarus/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/sklearn/linear_model.py` & `sarus-0.7.5rc0/sarus/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/sklearn/model_selection.py` & `sarus-0.7.5rc0/sarus/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/sklearn/pipeline.py` & `sarus-0.7.5rc0/sarus/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/sklearn/preprocessing.py` & `sarus-0.7.5rc0/sarus/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/sklearn/svm.py` & `sarus-0.7.5rc0/sarus/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/skopt/searchcv.py` & `sarus-0.7.5rc0/sarus/skopt/searchcv.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus/std/types.py` & `sarus-0.7.5rc0/sarus/std/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,51 @@
+from __future__ import annotations
+
 from sarus.dataspec_wrapper import DataSpecWrapper
 from sarus.utils import sarus_init
 
 
 class Slice(DataSpecWrapper[slice]):
     @sarus_init("std.SLICE")
     def __init__(self, *args, **kwargs) -> None:
         ...
 
+    @classmethod
+    def from_value(cls, value: slice) -> Slice:
+        elems = [
+            value.start,
+            value.stop,
+            value.step,
+        ]
+        return Slice(*elems)
+
 
 class Set(DataSpecWrapper[set]):
     @sarus_init("std.SET")
     def __init__(self, *args, **kwargs) -> None:
         """Need to pass all arguments Set(*args)."""
         ...
 
+    @classmethod
+    def from_value(cls, value: set) -> Set:
+        elems = [e for e in value]
+        return Set(*elems)
+
 
 class Dict(DataSpecWrapper[dict]):
     @sarus_init("std.DICT")
     def __init__(self, *args, **kwargs) -> None:
         """Need to pass all arguments Dict(**kwargs)."""
         ...
 
+    @classmethod
+    def from_value(cls, value: dict) -> Dict:
+        elems = {k: v for k, v in value.items()}
+        return Dict(**elems)
+
 
 class List(DataSpecWrapper[list]):
     @sarus_init("std.LIST")
     def __init__(self, *args, **kwargs) -> None:
         """Need to pass all arguments List(*args)."""
 
     def __iter__(self):
@@ -35,14 +56,19 @@
         try:
             idx = self.__sarus_idx__
             self.__sarus_idx__ += 1
             return self[idx]
         except IndexError:
             raise StopIteration
 
+    @classmethod
+    def from_value(cls, value: list) -> List:
+        elems = [e for e in value]
+        return List(*elems)
+
 
 class Tuple(DataSpecWrapper[tuple]):
     @sarus_init("std.TUPLE")
     def __init__(self, *args, **kwargs) -> None:
         """Need to pass all arguments Tuple(*args)."""
 
     def __iter__(self):
@@ -53,18 +79,35 @@
         try:
             idx = self.__sarus_idx__
             self.__sarus_idx__ += 1
             return self[idx]
         except IndexError:
             raise StopIteration
 
+    @classmethod
+    def from_value(cls, value: tuple) -> Tuple:
+        elems = [e for e in value]
+        return Tuple(*elems)
+
 
 class Int(DataSpecWrapper[int]):
-    ...
+    @sarus_init("std.INT")
+    def __init__(self, *args, **kwargs) -> None:
+        ...
 
 
 class Float(DataSpecWrapper[float]):
-    ...
+    @sarus_init("std.FLOAT")
+    def __init__(self, *args, **kwargs) -> None:
+        ...
 
 
 class String(DataSpecWrapper[str]):
-    ...
+    @sarus_init("std.STRING")
+    def __init__(self, *args, **kwargs) -> None:
+        ...
+
+
+class Bool(DataSpecWrapper[bool]):
+    @sarus_init("std.BOOL")
+    def __init__(self, *args, **kwargs) -> None:
+        ...
```

### Comparing `sarus-0.7.4.dev2/sarus/utils.py` & `sarus-0.7.5rc0/sarus/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import inspect
 import logging
 import os
+from datetime import date, datetime, time, timedelta, timezone
 from functools import partial, wraps
-from typing import Any, Callable, Dict, Optional, Type
+from typing import Any, Callable, Dict, Optional, Type, Union
 
+import numpy as np
+import pandas as pd
 import sarus_data_spec.typing as st
 import yaml
 from sarus_data_spec.context import global_context
 from sarus_data_spec.transform import external
 
 from .context.typing import LocalSDKContext
-from .typing import DataSpecVariant, DataSpecWrapper
+from .typing import DataSpecVariant, DataSpecWrapper, TracedFunction
 
 logger = logging.getLogger(__name__)
 
 config_file = os.path.join(os.path.dirname(__file__), "config.yaml")
 with open(config_file) as f:
     config = yaml.load(f.read(), Loader=yaml.Loader)
 
@@ -56,55 +59,92 @@
 
 
 def save(dw: DataSpecWrapper, path: str) -> None:
     """Save a DataSpecWrapper for loading in another notebook."""
     dw.sarus_save(path)
 
 
-def convert_container(x: Any) -> Any:
+def is_specific_type_iterable(iterable):
+    types = (
+        pd.Timestamp,
+        datetime,
+        timedelta,
+        timezone,
+        time,
+        date,
+        np.generic,
+        pd.Period,
+        pd.Timedelta,
+        pd.Interval,
+        type,
+        pd.api.extensions.ExtensionDtype,
+        slice,
+        str,
+        int,
+        float,
+        bool,
+        type(None),
+    )
+    return all(isinstance(x, types) for x in iterable)
+
+
+def convert_container(x):
     """Recursively convert containers in DataSpecWrappers if one
     element is a DataSpecWrapper."""
     from sarus.std import Dict, List, Set, Slice, Tuple
 
-    if isinstance(x, DataSpecWrapper):
+    sarus_types = (DataSpecWrapper, TracedFunction)
+    all_container_types = (list, set, tuple, dict, slice)
+    some_container_types = (list, set, tuple)
+
+    if isinstance(x, sarus_types):
         return x
-    elif isinstance(x, list):
-        elems = [convert_container(e) for e in x]
-        if any(isinstance(e, DataSpecWrapper) for e in elems):
-            return List(*elems)
-        else:
-            return x
-    elif isinstance(x, set):
-        elems = [convert_container(e) for e in x]
-        if any(isinstance(e, DataSpecWrapper) for e in elems):
-            return Set(*elems)
-        else:
-            return x
-    elif isinstance(x, tuple):
-        elems = [convert_container(e) for e in x]
-        if any(isinstance(e, DataSpecWrapper) for e in elems):
-            return Tuple(*elems)
-        else:
-            return x
-    elif isinstance(x, dict):
-        elems = {k: convert_container(v) for k, v in x.items()}
-        if any(isinstance(e, DataSpecWrapper) for e in elems.values()):
-            return Dict(**elems)
-        else:
-            return x
-    elif isinstance(x, slice):
-        elems = [
-            x.start,
-            x.stop,
-            x.step,
-        ]
-        if any([isinstance(e, DataSpecWrapper) for e in elems]):
-            return Slice(*elems)
-        else:
+    elif isinstance(x, all_container_types):
+        if isinstance(x, some_container_types) and is_specific_type_iterable(
+            x
+        ):
             return x
+
+        if isinstance(x, list):
+            elems = [convert_container(e) for e in x]
+            if any(isinstance(e, sarus_types) for e in elems):
+                return List(*elems)
+            else:
+                return x
+        elif isinstance(x, set):
+            elems = [convert_container(e) for e in x]
+            if any(isinstance(e, sarus_types) for e in elems):
+                return Set(*elems)
+            else:
+                return x
+        elif isinstance(x, tuple):
+            elems = [convert_container(e) for e in x]
+            if any(isinstance(e, sarus_types) for e in elems):
+                return Tuple(*elems)
+            else:
+                return x
+        elif isinstance(x, dict):
+            if is_specific_type_iterable(x.values()):
+                return x
+
+            elems = {k: convert_container(v) for k, v in x.items()}
+            if any(isinstance(e, sarus_types) for e in elems.values()):
+                return Dict(**elems)
+            else:
+                return x
+        elif isinstance(x, slice):
+            elems = [
+                x.start,
+                x.stop,
+                x.step,
+            ]
+            if any([isinstance(e, sarus_types) for e in elems]):
+                return Slice(*elems)
+            else:
+                return x
     else:
         return eval(x)
 
 
 def eval_policy(x: Any) -> Optional[str]:
     """The alternative dataspec's privacy policy."""
     if isinstance(x, DataSpecWrapper):
@@ -182,87 +222,127 @@
                 create_method(
                     mth_code_name, module_name, class_name, mth_name
                 ),
             )
 
 
 def serialize_external(
-    code_name: str, *args: Any, **kwargs: Any
+    code_name: str,
+    *args: Union[DataSpecWrapper, Any],
+    **kwargs: Union[DataSpecWrapper, Any],
 ) -> st.DataSpec:
     """Some arguments are instances of DataSpecWrapper and others are
     just Python object. This function registers a new dataspec."""
     args = [convert_container(arg) for arg in args]
     kwargs = {
         eval(name): convert_container(arg) for name, arg in kwargs.items()
     }
+    sarus_types = (DataSpecWrapper, TracedFunction)
     py_args = {
         i: arg
         for i, arg in enumerate(args)
-        if not isinstance(arg, DataSpecWrapper)
+        if not isinstance(arg, sarus_types)
     }
     ds_args_pos = [
-        i for i, arg in enumerate(args) if isinstance(arg, DataSpecWrapper)
+        i for i, arg in enumerate(args) if isinstance(arg, sarus_types)
     ]
     ds_arg_types = {
         i: str(arg.__wraps__)
-        for i, arg in enumerate(args)
         if isinstance(arg, DataSpecWrapper)
+        else "TracedFunction"
+        for i, arg in enumerate(args)
+        if isinstance(arg, sarus_types)
     }
     ds_args = [
         arg.dataspec(DataSpecVariant.USER_DEFINED)
-        for arg in args
         if isinstance(arg, DataSpecWrapper)
+        else arg.transform()
+        for arg in args
+        if isinstance(arg, sarus_types)
     ]
     py_kwargs = {
         name: arg
         for name, arg in kwargs.items()
-        if not isinstance(arg, DataSpecWrapper)
+        if not isinstance(arg, sarus_types)
     }
     ds_kwargs = {
         name: arg.dataspec(DataSpecVariant.USER_DEFINED)
-        for name, arg in kwargs.items()
         if isinstance(arg, DataSpecWrapper)
+        else arg.transform()
+        for name, arg in kwargs.items()
+        if isinstance(arg, sarus_types)
     }
     ds_kwargs_types = {
         name: str(arg.__wraps__)
-        for name, arg in kwargs.items()
         if isinstance(arg, DataSpecWrapper)
+        else "TracedFunction"
+        for name, arg in kwargs.items()
+        if isinstance(arg, sarus_types)
     }
     transform = external(
         id=code_name,
         py_args=py_args,
         py_kwargs=py_kwargs,
         ds_args_pos=ds_args_pos,
         ds_types={**ds_arg_types, **ds_kwargs_types},
     )
     new_dataspec = transform(*ds_args, **ds_kwargs)
-    return new_dataspec
+
+    # Compute the traced transform if tracing
+    tr_args = [
+        arg.traced_transform()
+        for arg in args
+        if isinstance(arg, DataSpecWrapper)
+    ]
+    tr_kwargs = {
+        name: arg.traced_transform()
+        for name, arg in kwargs.items()
+        if isinstance(arg, DataSpecWrapper)
+    }
+    is_not_traced = [tr is None for tr in tr_args] + [
+        tr is None for tr in tr_kwargs.values()
+    ]
+    if all(is_not_traced):
+        traced_transform = None
+    elif any(is_not_traced):
+        raise ValueError("Some inputs are traced and other are not.")
+    else:
+        traced_transform = transform(*tr_args, **tr_kwargs)
+
+    return new_dataspec, traced_transform
 
 
 def _sarus_op(
     code_name: str,
     inplace: bool = False,
     register: bool = False,
     is_property: bool = False,
-):
+) -> Callable:
     """Parametrized decorator to register a Sarus external op."""
 
-    def parametrized_wrapper(ops_fn):
+    def parametrized_wrapper(ops_fn: Callable) -> Callable:
         @wraps(ops_fn)
-        def wrapper_fn(*args, **kwargs):
-            new_dataspec = serialize_external(code_name, *args, **kwargs)
+        def wrapper_fn(
+            *args: Union[DataSpecWrapper, Any],
+            **kwargs: Union[DataSpecWrapper, Any],
+        ) -> DataSpecWrapper:
+            new_dataspec, traced_transform = serialize_external(
+                code_name, *args, **kwargs
+            )
             context: LocalSDKContext = global_context()
 
             new_dataspec_wrapper = context.wrapper_factory().create(
                 new_dataspec
             )
+            new_dataspec_wrapper._set_traced_transform(traced_transform)
 
             if inplace:
                 self: DataSpecWrapper = args[0]  # TODO check semantic
                 self._set_dataspec(new_dataspec)
+                self._set_traced_transform(traced_transform)
 
             return new_dataspec_wrapper
 
         if is_property:
             wrapper_fn = property(wrapper_fn)
 
         if register:
@@ -273,26 +353,33 @@
     return parametrized_wrapper
 
 
 sarus_method = partial(_sarus_op, register=True, is_property=False)
 sarus_property = partial(_sarus_op, register=True, is_property=True)
 
 
-def sarus_init(code_name):
+def sarus_init(code_name: str) -> Callable:
     """Decorator to initialize DataSpecWrapper classes from ops."""
 
-    def parametrized_wrapper(ops_fn):
+    def parametrized_wrapper(ops_fn: Callable) -> Callable:
         @wraps(ops_fn)
-        def wrapper_fn(self, *args, **kwargs):
-            new_dataspec = serialize_external(code_name, *args, **kwargs)
+        def init_fn(
+            self: DataSpecWrapper,
+            *args: Union[DataSpecWrapper, Any],
+            **kwargs: Union[DataSpecWrapper, Any],
+        ) -> None:
+            new_dataspec, traced_transform = serialize_external(
+                code_name, *args, **kwargs
+            )
             self._set_dataspec(new_dataspec)
+            self._set_traced_transform(traced_transform)
 
-        wrapper_fn = register_method(wrapper_fn, code_name)
+        init_fn = register_method(init_fn, code_name)
 
-        return wrapper_fn
+        return init_fn
 
     return parametrized_wrapper
 
 
 def create_function(
     code_name: str, module_name: str, fn_name: str, inplace: bool = False
 ) -> Callable:
```

### Comparing `sarus-0.7.4.dev2/sarus/wrapper_factory.py` & `sarus-0.7.5rc0/sarus/wrapper_factory.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,66 @@
-from typing import Any, Union, cast
+from typing import Any, Dict, Type, Union, cast
 
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 from sarus_data_spec.context import global_context
 
 from sarus.dataspec_wrapper import DataSpecWrapper
 from sarus.manager.typing import SDKManager
+from sarus.utils import convert_container
 
 
 class DataSpecWrapperFactory:
     def __init__(self):
-        self.registry = {}
+        self._registry = {}
 
     def register(
         self,
         python_classname: str,
-        sarus_wrapper_class: DataSpecWrapper,
+        sarus_wrapper_class: Type[DataSpecWrapper],
     ) -> None:
-        self.registry[python_classname] = sarus_wrapper_class
+        self._registry[python_classname] = sarus_wrapper_class
 
     def create(self, dataspec: st.DataSpec) -> Union[DataSpecWrapper, Any]:
         """Create a wrapper class from a DataSpec.
 
         If the dataspec's python value is not managed by the SDK, returns an
         unwrapped Python object.
         """
         context = global_context()
         manager: SDKManager = context.manager()
         python_type = manager.python_type(dataspec)
-        SarusWrapperClass = self.registry.get(python_type)
+        SarusWrapperClass = self._registry.get(python_type)
         if SarusWrapperClass:
             return SarusWrapperClass.from_dataspec(dataspec)
         else:
             # Datasets are either pd.DataFrame or pd.Series
             if dataspec.prototype() != sp.Scalar:
                 raise TypeError(f"Expected a Scalar {dataspec}")
             scalar = cast(st.Scalar, dataspec)
             alt_scalar = scalar.variant(
                 kind=st.ConstraintKind.SYNTHETIC, public_context=[]
             )
             return alt_scalar.value()
+
+    def from_value(self, value: Any) -> DataSpecWrapper:
+        """Creates a wrapper class from a Python object.
+
+        The Python object can be a container, in which wase it might contain a
+        DataSpecWrapper nested deeper. Such containers will be converted to
+        DataSpecWrappers.
+        """
+        value = convert_container(value)
+        if isinstance(value, DataSpecWrapper):
+            return value
+
+        python_type = str(type(value))
+        SarusWrapperClass = self.registry().get(python_type)
+        if SarusWrapperClass is None:
+            raise TypeError(
+                f"Cannot convert type {python_type} to DataSpecWrapper."
+            )
+
+        return SarusWrapperClass.from_value(value)
+
+    def registry(self) -> Dict[str, Type[DataSpecWrapper]]:
+        return self._registry
```

### Comparing `sarus-0.7.4.dev2/sarus/xgboost/xgboost.py` & `sarus-0.7.5rc0/sarus/xgboost/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.4.dev2/sarus.egg-info/PKG-INFO` & `sarus-0.7.5rc0/sarus.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.7.4.dev2
+Version: 0.7.5rc0
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.7.4.dev2/sarus.egg-info/SOURCES.txt` & `sarus-0.7.5rc0/sarus.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.cfg
 setup.py
 sarus/__init__.py
 sarus/config.yaml
 sarus/dataspec_wrapper.py
 sarus/debug.py
 sarus/sarus.py
+sarus/serialization.py
 sarus/typing.py
 sarus/utils.py
 sarus/wrapper_factory.py
 sarus.egg-info/PKG-INFO
 sarus.egg-info/SOURCES.txt
 sarus.egg-info/dependency_links.txt
 sarus.egg-info/not-zip-safe
```

### Comparing `sarus-0.7.4.dev2/setup.cfg` & `sarus-0.7.5rc0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 [options]
 zip_safe = False
 python_requires = >=3.7, <3.11
 packages = find:
 include_package_data = True
 install_requires = 
-	sarus-data-spec-public==3.5.8.dev1
+	sarus-data-spec-public==3.5.8
 	cloudpickle>=1.2, <2.1
 	pyarrow >= 11.0
 	protobuf >= 3.20.3
 
 [options.extras_require]
 sklearn = 
 	scikit-learn==1.2.2
```

