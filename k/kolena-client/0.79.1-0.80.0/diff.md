# Comparing `tmp/kolena_client-0.79.1.tar.gz` & `tmp/kolena_client-0.80.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolena_client-0.79.1.tar", max compression
+gzip compressed data, was "kolena_client-0.80.0.tar", max compression
```

## Comparing `kolena_client-0.79.1.tar` & `kolena_client-0.80.0.tar`

### file list

```diff
@@ -1,118 +1,118 @@
--rw-r--r--   0        0        0    11346 2023-07-28 17:33:41.312480 kolena_client-0.79.1/LICENSE
--rw-r--r--   0        0        0      556 2023-07-28 17:33:41.312480 kolena_client-0.79.1/LICENSE_HEADER
--rw-r--r--   0        0        0     1948 2023-07-28 17:33:41.312480 kolena_client-0.79.1/README.md
--rw-r--r--   0        0        0     1356 2023-07-28 17:39:26.222085 kolena_client-0.79.1/kolena/__init__.py
--rw-r--r--   0        0        0      579 2023-07-28 17:33:41.368481 kolena_client-0.79.1/kolena/_api/__init__.py
--rw-r--r--   0        0        0      579 2023-07-28 17:33:41.368481 kolena_client-0.79.1/kolena/_api/v1/__init__.py
--rw-r--r--   0        0        0     1737 2023-07-28 17:33:41.368481 kolena_client-0.79.1/kolena/_api/v1/batched_load.py
--rw-r--r--   0        0        0      878 2023-07-28 17:33:41.368481 kolena_client-0.79.1/kolena/_api/v1/client_log.py
--rw-r--r--   0        0        0     5111 2023-07-28 17:33:41.368481 kolena_client-0.79.1/kolena/_api/v1/core.py
--rw-r--r--   0        0        0     5320 2023-07-28 17:33:41.368481 kolena_client-0.79.1/kolena/_api/v1/detection.py
--rw-r--r--   0        0        0     7531 2023-07-28 17:33:41.368481 kolena_client-0.79.1/kolena/_api/v1/fr.py
--rw-r--r--   0        0        0     5597 2023-07-28 17:33:41.368481 kolena_client-0.79.1/kolena/_api/v1/generic.py
--rw-r--r--   0        0        0      778 2023-07-28 17:33:41.368481 kolena_client-0.79.1/kolena/_api/v1/repository.py
--rw-r--r--   0        0        0      833 2023-07-28 17:33:41.368481 kolena_client-0.79.1/kolena/_api/v1/token.py
--rw-r--r--   0        0        0      738 2023-07-28 17:33:41.368481 kolena_client-0.79.1/kolena/_api/v1/workflow.py
--rw-r--r--   0        0        0      579 2023-07-28 17:33:41.368481 kolena_client-0.79.1/kolena/_experimental/__init__.py
--rw-r--r--   0        0        0      579 2023-07-28 17:33:41.368481 kolena_client-0.79.1/kolena/_experimental/classification/__init__.py
--rw-r--r--   0        0        0     4256 2023-07-28 17:33:41.368481 kolena_client-0.79.1/kolena/_experimental/classification/utils.py
--rw-r--r--   0        0        0     1117 2023-07-28 17:33:41.368481 kolena_client-0.79.1/kolena/_experimental/object_detection/__init__.py
--rw-r--r--   0        0        0     5654 2023-07-28 17:33:41.368481 kolena_client-0.79.1/kolena/_experimental/object_detection/evaluator.py
--rw-r--r--   0        0        0    15465 2023-07-28 17:33:41.368481 kolena_client-0.79.1/kolena/_experimental/object_detection/evaluator_multiclass.py
--rw-r--r--   0        0        0    10294 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_experimental/object_detection/evaluator_single_class.py
--rw-r--r--   0        0        0    13260 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_experimental/object_detection/utils.py
--rw-r--r--   0        0        0     5173 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_experimental/object_detection/workflow.py
--rw-r--r--   0        0        0      579 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_extras/__init__.py
--rw-r--r--   0        0        0      676 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_extras/metrics/__init__.py
--rw-r--r--   0        0        0      783 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_extras/metrics/sklearn.py
--rw-r--r--   0        0        0      579 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_utils/__init__.py
--rw-r--r--   0        0        0     1616 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_utils/asset_path_mapper.py
--rw-r--r--   0        0        0     5313 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_utils/batched_load.py
--rw-r--r--   0        0        0     5608 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_utils/cli.py
--rw-r--r--   0        0        0      921 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_utils/consts.py
--rw-r--r--   0        0        0      579 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_utils/dataframes/__init__.py
--rw-r--r--   0        0        0     2826 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_utils/dataframes/validators.py
--rw-r--r--   0        0        0     1952 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_utils/datatypes.py
--rw-r--r--   0        0        0     3403 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_utils/endpoints.py
--rw-r--r--   0        0        0     1690 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_utils/frozen.py
--rw-r--r--   0        0        0     1183 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_utils/geometry.py
--rw-r--r--   0        0        0     1087 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_utils/inference_validators.py
--rw-r--r--   0        0        0     2990 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_utils/instrumentation.py
--rw-r--r--   0        0        0     5033 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_utils/krequests.py
--rw-r--r--   0        0        0     3507 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_utils/log.py
--rw-r--r--   0        0        0     1003 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_utils/repository.py
--rw-r--r--   0        0        0     2494 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_utils/serde.py
--rw-r--r--   0        0        0      889 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_utils/serializable.py
--rw-r--r--   0        0        0     5450 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_utils/state.py
--rw-r--r--   0        0        0     1942 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_utils/uninstantiable.py
--rw-r--r--   0        0        0     1164 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/_utils/validators.py
--rw-r--r--   0        0        0     1272 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/classification/__init__.py
--rw-r--r--   0        0        0     1475 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/classification/metadata.py
--rw-r--r--   0        0        0     3512 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/classification/model.py
--rw-r--r--   0        0        0     1213 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/classification/multiclass/__init__.py
--rw-r--r--   0        0        0     3354 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/classification/multiclass/_utils.py
--rw-r--r--   0        0        0    15698 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/classification/multiclass/evaluator.py
--rw-r--r--   0        0        0     3573 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/classification/multiclass/test_run.py
--rw-r--r--   0        0        0     3185 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/classification/multiclass/workflow.py
--rw-r--r--   0        0        0     2694 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/classification/test_case.py
--rw-r--r--   0        0        0     2372 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/classification/test_config.py
--rw-r--r--   0        0        0     4480 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/classification/test_image.py
--rw-r--r--   0        0        0     6013 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/classification/test_run.py
--rw-r--r--   0        0        0     3180 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/classification/test_suite.py
--rw-r--r--   0        0        0     1477 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/__init__.py
--rw-r--r--   0        0        0     6819 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/_datatypes.py
--rw-r--r--   0        0        0     1042 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/_internal/__init__.py
--rw-r--r--   0        0        0     1922 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/_internal/datatypes.py
--rw-r--r--   0        0        0      765 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/_internal/ground_truth.py
--rw-r--r--   0        0        0     1035 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/_internal/inference.py
--rw-r--r--   0        0        0     5470 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/_internal/metadata.py
--rw-r--r--   0        0        0     8995 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/_internal/model.py
--rw-r--r--   0        0        0    14122 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/_internal/test_case.py
--rw-r--r--   0        0        0     1201 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/_internal/test_config.py
--rw-r--r--   0        0        0     1761 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/_internal/test_image.py
--rw-r--r--   0        0        0    12390 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/_internal/test_run.py
--rw-r--r--   0        0        0    13804 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/_internal/test_suite.py
--rw-r--r--   0        0        0     5867 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/ground_truth.py
--rw-r--r--   0        0        0     5435 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/inference.py
--rw-r--r--   0        0        0     1460 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/metadata.py
--rw-r--r--   0        0        0     3210 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/model.py
--rw-r--r--   0        0        0     2387 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/test_case.py
--rw-r--r--   0        0        0     3199 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/test_config.py
--rw-r--r--   0        0        0     5967 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/test_image.py
--rw-r--r--   0        0        0     5405 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/test_run.py
--rw-r--r--   0        0        0     2854 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/detection/test_suite.py
--rw-r--r--   0        0        0     2681 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/errors.py
--rw-r--r--   0        0        0     1400 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/fr/__init__.py
--rw-r--r--   0        0        0     2171 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/fr/_utils.py
--rw-r--r--   0        0        0    20960 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/fr/datatypes.py
--rw-r--r--   0        0        0    10274 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/fr/model.py
--rw-r--r--   0        0        0    14952 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/fr/test_case.py
--rw-r--r--   0        0        0    12237 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/fr/test_images.py
--rw-r--r--   0        0        0    16943 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/fr/test_run.py
--rw-r--r--   0        0        0    16329 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/fr/test_suite.py
--rw-r--r--   0        0        0     3880 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/initialize.py
--rw-r--r--   0        0        0     2493 2023-07-28 17:33:41.372481 kolena_client-0.79.1/kolena/workflow/__init__.py
--rw-r--r--   0        0        0    13948 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/_datatypes.py
--rw-r--r--   0        0        0     6281 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/_validators.py
--rw-r--r--   0        0        0    10397 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/annotation.py
--rw-r--r--   0        0        0     4926 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/asset.py
--rw-r--r--   0        0        0     3469 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/define_workflow.py
--rw-r--r--   0        0        0    13854 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/evaluator.py
--rw-r--r--   0        0        0    11232 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/evaluator_function.py
--rw-r--r--   0        0        0     4421 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/ground_truth.py
--rw-r--r--   0        0        0     4334 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/inference.py
--rw-r--r--   0        0        0     1150 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/metrics/__init__.py
--rw-r--r--   0        0        0     3931 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/metrics/_formula.py
--rw-r--r--   0        0        0    16014 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/metrics/_geometry.py
--rw-r--r--   0        0        0     8459 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/model.py
--rw-r--r--   0        0        0    10261 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/plot.py
--rw-r--r--   0        0        0    18319 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/test_case.py
--rw-r--r--   0        0        0    23730 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/test_run.py
--rw-r--r--   0        0        0    11006 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/test_sample.py
--rw-r--r--   0        0        0    15455 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/test_suite.py
--rw-r--r--   0        0        0      841 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/visualization/__init__.py
--rw-r--r--   0        0        0     6145 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/visualization/_activation_map.py
--rw-r--r--   0        0        0     1910 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/visualization/_utils.py
--rw-r--r--   0        0        0     9419 2023-07-28 17:33:41.376481 kolena_client-0.79.1/kolena/workflow/workflow.py
--rw-r--r--   0        0        0     3034 2023-07-28 17:39:26.222085 kolena_client-0.79.1/pyproject.toml
--rw-r--r--   0        0        0     4319 1970-01-01 00:00:00.000000 kolena_client-0.79.1/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-08-01 21:30:28.006610 kolena_client-0.80.0/LICENSE
+-rw-r--r--   0        0        0      556 2023-08-01 21:30:28.006610 kolena_client-0.80.0/LICENSE_HEADER
+-rw-r--r--   0        0        0     1993 2023-08-01 21:30:28.006610 kolena_client-0.80.0/README.md
+-rw-r--r--   0        0        0     1356 2023-08-01 21:38:48.892593 kolena_client-0.80.0/kolena/__init__.py
+-rw-r--r--   0        0        0      579 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/__init__.py
+-rw-r--r--   0        0        0      579 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/v1/__init__.py
+-rw-r--r--   0        0        0     1737 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/v1/batched_load.py
+-rw-r--r--   0        0        0      878 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/v1/client_log.py
+-rw-r--r--   0        0        0     5111 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/v1/core.py
+-rw-r--r--   0        0        0     5320 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/v1/detection.py
+-rw-r--r--   0        0        0     7531 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/v1/fr.py
+-rw-r--r--   0        0        0     5597 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/v1/generic.py
+-rw-r--r--   0        0        0      778 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/v1/repository.py
+-rw-r--r--   0        0        0      833 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/v1/token.py
+-rw-r--r--   0        0        0      738 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_api/v1/workflow.py
+-rw-r--r--   0        0        0      579 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_experimental/__init__.py
+-rw-r--r--   0        0        0      579 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_experimental/classification/__init__.py
+-rw-r--r--   0        0        0     9888 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_experimental/classification/utils.py
+-rw-r--r--   0        0        0     1553 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_experimental/object_detection/__init__.py
+-rw-r--r--   0        0        0     5165 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_experimental/object_detection/evaluator.py
+-rw-r--r--   0        0        0    18050 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_experimental/object_detection/evaluator_multiclass.py
+-rw-r--r--   0        0        0    11891 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_experimental/object_detection/evaluator_single_class.py
+-rw-r--r--   0        0        0    14344 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_experimental/object_detection/utils.py
+-rw-r--r--   0        0        0     7238 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_experimental/object_detection/workflow.py
+-rw-r--r--   0        0        0      579 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_extras/__init__.py
+-rw-r--r--   0        0        0      676 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_extras/metrics/__init__.py
+-rw-r--r--   0        0        0      785 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_extras/metrics/sklearn.py
+-rw-r--r--   0        0        0      579 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_utils/__init__.py
+-rw-r--r--   0        0        0     1616 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_utils/asset_path_mapper.py
+-rw-r--r--   0        0        0     5313 2023-08-01 21:30:28.086609 kolena_client-0.80.0/kolena/_utils/batched_load.py
+-rw-r--r--   0        0        0     5608 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/cli.py
+-rw-r--r--   0        0        0      921 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/consts.py
+-rw-r--r--   0        0        0      579 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0     2826 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/dataframes/validators.py
+-rw-r--r--   0        0        0     1952 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/datatypes.py
+-rw-r--r--   0        0        0     3403 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/endpoints.py
+-rw-r--r--   0        0        0     1690 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/frozen.py
+-rw-r--r--   0        0        0     1183 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/geometry.py
+-rw-r--r--   0        0        0     1087 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/inference_validators.py
+-rw-r--r--   0        0        0     2990 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/instrumentation.py
+-rw-r--r--   0        0        0     5033 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/krequests.py
+-rw-r--r--   0        0        0     3507 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/log.py
+-rw-r--r--   0        0        0     1003 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/repository.py
+-rw-r--r--   0        0        0     2494 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/serde.py
+-rw-r--r--   0        0        0      889 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/serializable.py
+-rw-r--r--   0        0        0     5450 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/state.py
+-rw-r--r--   0        0        0     1942 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/uninstantiable.py
+-rw-r--r--   0        0        0     1164 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/_utils/validators.py
+-rw-r--r--   0        0        0     1272 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/__init__.py
+-rw-r--r--   0        0        0     1475 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/metadata.py
+-rw-r--r--   0        0        0     3512 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/model.py
+-rw-r--r--   0        0        0     1213 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/multiclass/__init__.py
+-rw-r--r--   0        0        0     3354 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/multiclass/_utils.py
+-rw-r--r--   0        0        0    15698 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/multiclass/evaluator.py
+-rw-r--r--   0        0        0     3573 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/multiclass/test_run.py
+-rw-r--r--   0        0        0     3185 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/multiclass/workflow.py
+-rw-r--r--   0        0        0     2694 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/test_case.py
+-rw-r--r--   0        0        0     2372 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/test_config.py
+-rw-r--r--   0        0        0     4480 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/test_image.py
+-rw-r--r--   0        0        0     6013 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/test_run.py
+-rw-r--r--   0        0        0     3180 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/classification/test_suite.py
+-rw-r--r--   0        0        0     1477 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/__init__.py
+-rw-r--r--   0        0        0     6819 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_datatypes.py
+-rw-r--r--   0        0        0     1042 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/__init__.py
+-rw-r--r--   0        0        0     1922 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/datatypes.py
+-rw-r--r--   0        0        0      765 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/ground_truth.py
+-rw-r--r--   0        0        0     1035 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/inference.py
+-rw-r--r--   0        0        0     5470 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/metadata.py
+-rw-r--r--   0        0        0     8995 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/model.py
+-rw-r--r--   0        0        0    14122 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/test_case.py
+-rw-r--r--   0        0        0     1201 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/test_config.py
+-rw-r--r--   0        0        0     1761 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/test_image.py
+-rw-r--r--   0        0        0    12390 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/test_run.py
+-rw-r--r--   0        0        0    13804 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/_internal/test_suite.py
+-rw-r--r--   0        0        0     5867 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/ground_truth.py
+-rw-r--r--   0        0        0     5435 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/inference.py
+-rw-r--r--   0        0        0     1460 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/metadata.py
+-rw-r--r--   0        0        0     3210 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/model.py
+-rw-r--r--   0        0        0     2387 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/test_case.py
+-rw-r--r--   0        0        0     3199 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/test_config.py
+-rw-r--r--   0        0        0     5967 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/test_image.py
+-rw-r--r--   0        0        0     5405 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/test_run.py
+-rw-r--r--   0        0        0     2854 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/detection/test_suite.py
+-rw-r--r--   0        0        0     2681 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/errors.py
+-rw-r--r--   0        0        0     1400 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/fr/__init__.py
+-rw-r--r--   0        0        0     2171 2023-08-01 21:30:28.090609 kolena_client-0.80.0/kolena/fr/_utils.py
+-rw-r--r--   0        0        0    20960 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/fr/datatypes.py
+-rw-r--r--   0        0        0    10274 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/fr/model.py
+-rw-r--r--   0        0        0    14952 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/fr/test_case.py
+-rw-r--r--   0        0        0    12237 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/fr/test_images.py
+-rw-r--r--   0        0        0    16943 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/fr/test_run.py
+-rw-r--r--   0        0        0    16329 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/fr/test_suite.py
+-rw-r--r--   0        0        0     3880 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/initialize.py
+-rw-r--r--   0        0        0     2493 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/__init__.py
+-rw-r--r--   0        0        0    13948 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/_datatypes.py
+-rw-r--r--   0        0        0     6281 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/_validators.py
+-rw-r--r--   0        0        0    10397 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/annotation.py
+-rw-r--r--   0        0        0     4926 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/asset.py
+-rw-r--r--   0        0        0     3469 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/define_workflow.py
+-rw-r--r--   0        0        0    13854 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/evaluator.py
+-rw-r--r--   0        0        0    11232 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/evaluator_function.py
+-rw-r--r--   0        0        0     4421 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/ground_truth.py
+-rw-r--r--   0        0        0     4334 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/inference.py
+-rw-r--r--   0        0        0     1150 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/metrics/__init__.py
+-rw-r--r--   0        0        0     3931 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/metrics/_formula.py
+-rw-r--r--   0        0        0    16014 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/metrics/_geometry.py
+-rw-r--r--   0        0        0     8459 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/model.py
+-rw-r--r--   0        0        0    10261 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/plot.py
+-rw-r--r--   0        0        0    18319 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/test_case.py
+-rw-r--r--   0        0        0    23730 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/test_run.py
+-rw-r--r--   0        0        0    11006 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/test_sample.py
+-rw-r--r--   0        0        0    15455 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/test_suite.py
+-rw-r--r--   0        0        0      841 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/visualization/__init__.py
+-rw-r--r--   0        0        0     6145 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/visualization/_activation_map.py
+-rw-r--r--   0        0        0     1910 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/visualization/_utils.py
+-rw-r--r--   0        0        0     9419 2023-08-01 21:30:28.094609 kolena_client-0.80.0/kolena/workflow/workflow.py
+-rw-r--r--   0        0        0     3032 2023-08-01 21:38:48.892593 kolena_client-0.80.0/pyproject.toml
+-rw-r--r--   0        0        0     4364 1970-01-01 00:00:00.000000 kolena_client-0.80.0/PKG-INFO
```

### Comparing `kolena_client-0.79.1/LICENSE` & `kolena_client-0.80.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/LICENSE_HEADER` & `kolena_client-0.80.0/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/README.md` & `kolena_client-0.80.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 <p align="center">
-  <img src="https://docs.kolena.io/assets/images/kolena-banner.png" width="640" alt="Kolena" />
+  <a href="https://docs.kolena.io">
+    <img src="https://docs.kolena.io/assets/images/kolena-banner.png" width="640" alt="Kolena" />
+  </a>
 </p>
 
 <p align='center'>
   <a href="https://pypi.python.org/pypi/kolena"><img src="https://img.shields.io/pypi/v/kolena?logo=python&logoColor=white&style=flat-square" /></a>
   <a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/pypi/l/kolena?style=flat-square" /></a>
   <a href="https://github.com/kolenaIO/kolena/actions"><img src="https://img.shields.io/github/checks-status/kolenaIO/kolena/trunk?logo=circleci&logoColor=white&style=flat-square" /></a>
   <a href="https://codecov.io/gh/kolenaIO/kolena" ><img src="https://img.shields.io/codecov/c/github/kolenaIO/kolena?logo=codecov&logoColor=white&style=flat-square&token=8WOY5I8SF1" /></a>
```

### Comparing `kolena_client-0.79.1/kolena/__init__.py` & `kolena_client-0.80.0/kolena/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_api/__init__.py` & `kolena_client-0.80.0/kolena/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_api/v1/__init__.py` & `kolena_client-0.80.0/kolena/_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_api/v1/batched_load.py` & `kolena_client-0.80.0/kolena/_api/v1/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_api/v1/client_log.py` & `kolena_client-0.80.0/kolena/_api/v1/client_log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_api/v1/core.py` & `kolena_client-0.80.0/kolena/_api/v1/core.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_api/v1/detection.py` & `kolena_client-0.80.0/kolena/_api/v1/detection.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_api/v1/fr.py` & `kolena_client-0.80.0/kolena/_api/v1/fr.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_api/v1/generic.py` & `kolena_client-0.80.0/kolena/_api/v1/generic.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_api/v1/repository.py` & `kolena_client-0.80.0/kolena/_api/v1/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_api/v1/token.py` & `kolena_client-0.80.0/kolena/_api/v1/token.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_api/v1/workflow.py` & `kolena_client-0.80.0/kolena/_api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_experimental/__init__.py` & `kolena_client-0.80.0/kolena/_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_experimental/classification/__init__.py` & `kolena_client-0.80.0/kolena/_experimental/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_experimental/object_detection/__init__.py` & `kolena_client-0.80.0/kolena/classification/multiclass/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,26 +11,30 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # noreorder
 from .workflow import TestSample
 from .workflow import GroundTruth
+from .workflow import InferenceLabel
 from .workflow import Inference
 from .workflow import TestCase
 from .workflow import TestSuite
 from .workflow import Model
-from .workflow import ThresholdStrategy
 from .workflow import ThresholdConfiguration
-from .evaluator import ObjectDetectionEvaluator
+from .evaluator import MulticlassClassificationEvaluator
+from .test_run import TestRun
+from .test_run import test
 
 __all__ = [
     "TestSample",
     "GroundTruth",
+    "InferenceLabel",
     "Inference",
     "TestCase",
     "TestSuite",
     "Model",
-    "ThresholdStrategy",
     "ThresholdConfiguration",
-    "ObjectDetectionEvaluator",
+    "MulticlassClassificationEvaluator",
+    "TestRun",
+    "test",
 ]
```

### Comparing `kolena_client-0.79.1/kolena/_experimental/object_detection/evaluator.py` & `kolena_client-0.80.0/kolena/_experimental/object_detection/evaluator.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,39 +12,35 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
+from kolena._experimental.object_detection import GroundTruth
+from kolena._experimental.object_detection import Inference
+from kolena._experimental.object_detection import TestCase
+from kolena._experimental.object_detection import TestCaseMetrics
+from kolena._experimental.object_detection import TestCaseMetricsSingleClass
+from kolena._experimental.object_detection import TestSample
+from kolena._experimental.object_detection import TestSampleMetrics
+from kolena._experimental.object_detection import TestSampleMetricsSingleClass
+from kolena._experimental.object_detection import TestSuite
+from kolena._experimental.object_detection import TestSuiteMetrics
+from kolena._experimental.object_detection import ThresholdConfiguration
 from kolena._experimental.object_detection.evaluator_multiclass import MulticlassObjectDetectionEvaluator
 from kolena._experimental.object_detection.evaluator_single_class import SingleClassObjectDetectionEvaluator
-from kolena._experimental.object_detection.workflow import GroundTruth
-from kolena._experimental.object_detection.workflow import Inference
-from kolena._experimental.object_detection.workflow import TestCase
-from kolena._experimental.object_detection.workflow import TestCaseMetrics
-from kolena._experimental.object_detection.workflow import TestCaseMetricsSingleClass
-from kolena._experimental.object_detection.workflow import TestSample
-from kolena._experimental.object_detection.workflow import TestSampleMetrics
-from kolena._experimental.object_detection.workflow import TestSampleMetricsSingleClass
-from kolena._experimental.object_detection.workflow import TestSuite
-from kolena._experimental.object_detection.workflow import TestSuiteMetrics
-from kolena._experimental.object_detection.workflow import ThresholdConfiguration
 from kolena.workflow import Evaluator
 from kolena.workflow import Plot
 
 
 class ObjectDetectionEvaluator(Evaluator):
     """
     This `ObjectDetectionEvaluator` transforms inferences into metrics for the object detection workflow for a
-    single class or multiple classes. The `ObjectDetectionEvaluator` uses the [`SingleClassObjectDetectionEvaluator`]
-    [kolena._experimental.object_detection.evaluator_single_class.SingleClassObjectDetectionEvaluator] for single
-    class evaluation, and [`MulticlassObjectDetectionEvaluator`]
-    [kolena._experimental.object_detection.evaluator_multiclass.MulticlassObjectDetectionEvaluator] for multiclass
-    evaluation.
+    single class or multiple classes.
 
     When a [`ThresholdConfiguration`][kolena._experimental.object_detection.workflow.ThresholdConfiguration] is
     configured to use an F1-Optimal threshold strategy, the evaluator requires that the first test case retrieved for
     a test suite contains the complete sample set.
 
     For additional functionality, see the associated [base class documentation][kolena.workflow.evaluator.Evaluator].
     """
```

### Comparing `kolena_client-0.79.1/kolena/_experimental/object_detection/evaluator_multiclass.py` & `kolena_client-0.80.0/kolena/_experimental/object_detection/evaluator_multiclass.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,35 +11,37 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from collections import defaultdict
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import Set
 from typing import Tuple
 
 import numpy as np
 
+from kolena._experimental.object_detection import ClassMetricsPerTestCase
+from kolena._experimental.object_detection import GroundTruth
+from kolena._experimental.object_detection import Inference
+from kolena._experimental.object_detection import TestCase
+from kolena._experimental.object_detection import TestCaseMetrics
+from kolena._experimental.object_detection import TestSample
+from kolena._experimental.object_detection import TestSampleMetrics
+from kolena._experimental.object_detection import TestSuite
+from kolena._experimental.object_detection import TestSuiteMetrics
+from kolena._experimental.object_detection import ThresholdConfiguration
+from kolena._experimental.object_detection import ThresholdStrategy
 from kolena._experimental.object_detection.utils import compute_average_precision
 from kolena._experimental.object_detection.utils import compute_confusion_matrix_plot
 from kolena._experimental.object_detection.utils import compute_f1_plot_multiclass
 from kolena._experimental.object_detection.utils import compute_optimal_f1_threshold_multiclass
 from kolena._experimental.object_detection.utils import compute_pr_curve
 from kolena._experimental.object_detection.utils import compute_pr_plot_multiclass
-from kolena._experimental.object_detection.workflow import ClassMetricsPerTestCase
-from kolena._experimental.object_detection.workflow import GroundTruth
-from kolena._experimental.object_detection.workflow import Inference
-from kolena._experimental.object_detection.workflow import TestCase
-from kolena._experimental.object_detection.workflow import TestCaseMetrics
-from kolena._experimental.object_detection.workflow import TestSample
-from kolena._experimental.object_detection.workflow import TestSampleMetrics
-from kolena._experimental.object_detection.workflow import TestSuite
-from kolena._experimental.object_detection.workflow import TestSuiteMetrics
-from kolena._experimental.object_detection.workflow import ThresholdConfiguration
-from kolena._experimental.object_detection.workflow import ThresholdStrategy
+from kolena._experimental.object_detection.utils import filter_inferences
 from kolena.workflow import Evaluator
 from kolena.workflow import Plot
 from kolena.workflow.annotation import ScoredClassificationLabel
 from kolena.workflow.metrics import f1_score as compute_f1_score
 from kolena.workflow.metrics import match_inferences_multiclass
 from kolena.workflow.metrics import MulticlassInferenceMatches
 from kolena.workflow.metrics import precision as compute_precision
@@ -71,46 +73,63 @@
     """
 
     matchings_by_test_case: Dict[str, List[MulticlassInferenceMatches]] = defaultdict(list)
     """
     Caches matchings per test case for test case metrics and test case plots.
     """
 
-    def compute_image_metrics(
+    def test_sample_metrics_ignored(
         self,
-        ground_truth: GroundTruth,
-        inference: Inference,
-        configuration: ThresholdConfiguration,
-        test_case_name: str,
     ) -> TestSampleMetrics:
-        assert configuration is not None, "must specify configuration"
-        thresholds = self.get_confidence_thresholds(configuration)
-        bbox_matches: MulticlassInferenceMatches = match_inferences_multiclass(
-            ground_truth.bboxes,
-            [inf for inf in inference.bboxes if inf.score >= configuration.min_confidence_score],
-            ignored_ground_truths=ground_truth.ignored_bboxes,
-            mode="pascal",
-            iou_threshold=configuration.iou_threshold,
+        return TestSampleMetrics(
+            TP_labels=[],
+            TP=[],
+            FP_labels=[],
+            FP=[],
+            FN_labels=[],
+            FN=[],
+            Confused_labels=[],
+            Confused=[],
+            count_TP=0,
+            count_FP=0,
+            count_FN=0,
+            count_Confused=0,
+            has_TP=False,
+            has_FP=False,
+            has_FN=False,
+            has_Confused=False,
+            ignored=True,
+            max_confidence_above_t=None,
+            min_confidence_above_t=None,
+            thresholds=[],
+            inference_labels=[],
         )
-        self.matchings_by_test_case[test_case_name].append(bbox_matches)
+
+    def test_sample_metrics(
+        self,
+        bbox_matches: MulticlassInferenceMatches,
+        thresholds: Dict[str, float],
+    ) -> TestSampleMetrics:
         tp = [inf for _, inf in bbox_matches.matched if inf.score >= thresholds[inf.label]]
         fp = [inf for inf in bbox_matches.unmatched_inf if inf.score >= thresholds[inf.label]]
         fn = [gt for gt, _ in bbox_matches.unmatched_gt] + [
             gt for gt, inf in bbox_matches.matched if inf.score < thresholds[inf.label]
         ]
         confused = [
             inf for _, inf in bbox_matches.unmatched_gt if inf is not None and inf.score >= thresholds[inf.label]
         ]
         non_ignored_inferences = tp + fp
         scores = [inf.score for inf in non_ignored_inferences]
-        image_labels = {gt.label for gt in ground_truth.bboxes}
+        inference_labels = {inf.label for _, inf in bbox_matches.matched} | {
+            inf.label for inf in bbox_matches.unmatched_inf
+        }
         fields = [
             ScoredClassificationLabel(label=label, score=thresholds[label])
-            for label in thresholds.keys()
-            if label in image_labels
+            for label in sorted(thresholds.keys())
+            if label in inference_labels
         ]
         return TestSampleMetrics(
             TP_labels=sorted({inf.label for inf in tp}),
             TP=tp,
             FP_labels=sorted({inf.label for inf in fp}),
             FP=fp,
             FN_labels=sorted({inf.label for inf in fn}),
@@ -121,40 +140,69 @@
             count_FP=len(fp),
             count_FN=len(fn),
             count_Confused=len(confused),
             has_TP=len(tp) > 0,
             has_FP=len(fp) > 0,
             has_FN=len(fn) > 0,
             has_Confused=len(confused) > 0,
+            ignored=False,
             max_confidence_above_t=max(scores) if len(scores) > 0 else None,
             min_confidence_above_t=min(scores) if len(scores) > 0 else None,
             thresholds=fields,
-            inference_labels=sorted({inf.label for inf in inference.bboxes}),
+            inference_labels=sorted(inference_labels),
         )
 
+    def compute_image_metrics(
+        self,
+        ground_truth: GroundTruth,
+        inference: Inference,
+        configuration: ThresholdConfiguration,
+        test_case_name: str,
+    ) -> TestSampleMetrics:
+        assert configuration is not None, "must specify configuration"
+        thresholds = self.get_confidence_thresholds(configuration)
+        if inference.ignored:
+            return self.test_sample_metrics_ignored()
+
+        filtered_inferences = filter_inferences(
+            inferences=inference.bboxes,
+            confidence_score=configuration.min_confidence_score,
+        )
+        bbox_matches: MulticlassInferenceMatches = match_inferences_multiclass(
+            ground_truth.bboxes,
+            filtered_inferences,
+            ignored_ground_truths=ground_truth.ignored_bboxes,
+            mode="pascal",
+            iou_threshold=configuration.iou_threshold,
+        )
+        self.matchings_by_test_case[test_case_name].append(bbox_matches)
+
+        return self.test_sample_metrics(bbox_matches, thresholds)
+
     def compute_and_cache_f1_optimal_thresholds(
         self,
         configuration: ThresholdConfiguration,
         inferences: List[Tuple[TestSample, GroundTruth, Inference]],
     ) -> None:
         if configuration.threshold_strategy != ThresholdStrategy.F1_OPTIMAL:
             return
 
         if configuration.display_name() in self.threshold_cache.keys():
             return
 
         all_bbox_matches = [
             match_inferences_multiclass(
                 ground_truth.bboxes,
-                [inf for inf in inference.bboxes if inf.score >= configuration.min_confidence_score],
+                filter_inferences(inferences=inference.bboxes, confidence_score=configuration.min_confidence_score),
                 ignored_ground_truths=ground_truth.ignored_bboxes,
                 mode="pascal",
                 iou_threshold=configuration.iou_threshold,
             )
             for _, ground_truth, inference in inferences
+            if not inference.ignored
         ]
         optimal_thresholds = compute_optimal_f1_threshold_multiclass(all_bbox_matches)
         self.threshold_cache[configuration.display_name()] = defaultdict(
             lambda: configuration.min_confidence_score,
             optimal_thresholds,
         )
 
@@ -165,24 +213,23 @@
         configuration: Optional[ThresholdConfiguration] = None,
     ) -> List[Tuple[TestSample, TestSampleMetrics]]:
         assert configuration is not None, "must specify configuration"
         # compute thresholds to cache values for subsequent steps
         self.compute_and_cache_f1_optimal_thresholds(configuration, inferences)
         return [(ts, self.compute_image_metrics(gt, inf, configuration, test_case.name)) for ts, gt, inf in inferences]
 
-    def compute_aggregate_label_metrics(
+    def bbox_matches_for_one_label(
         self,
         matchings: List[MulticlassInferenceMatches],
         label: str,
-        thresholds: Dict[str, float],
-    ) -> ClassMetricsPerTestCase:
+    ) -> Tuple[MulticlassInferenceMatches, int]:
         match_matched = []
         match_unmatched_gt = []
         match_unmatched_inf = []
-        samples_with_label = 0
+        samples_count = 0
         # filter the matching to only consider one class
         for match in matchings:
             sample_flag = False
             for gt, inf in match.matched:
                 if gt.label == label:
                     sample_flag = True
                     match_matched.append((gt, inf))
@@ -191,95 +238,121 @@
                     sample_flag = True
                     match_unmatched_gt.append((gt, inf))
             for inf in match.unmatched_inf:
                 if inf.label == label:
                     sample_flag = True
                     match_unmatched_inf.append(inf)
             if sample_flag:
-                samples_with_label += 1
+                samples_count += 1
 
-        all_bbox_matches_for_one_label = [
-            MulticlassInferenceMatches(
-                matched=match_matched,
-                unmatched_gt=match_unmatched_gt,
-                unmatched_inf=match_unmatched_inf,
-            ),
-        ]
+        bbox_matches_for_one_label = MulticlassInferenceMatches(
+            matched=match_matched,
+            unmatched_gt=match_unmatched_gt,
+            unmatched_inf=match_unmatched_inf,
+        )
 
-        tp = [inf for _, inf in match_matched if inf.score >= thresholds[inf.label]]
-        fp = [inf for inf in match_unmatched_inf if inf.score >= thresholds[inf.label]]
-        fn = [gt for gt, _ in match_unmatched_gt] + [
-            gt for gt, inf in match_matched if inf.score < thresholds[inf.label]
-        ]
-        confused = [inf for _, inf in match_unmatched_gt if inf is not None and inf.score >= thresholds[inf.label]]
+        return bbox_matches_for_one_label, samples_count
+
+    def class_metrics_per_test_case(
+        self,
+        label: str,
+        thresholds: Dict[str, float],
+        class_matches: MulticlassInferenceMatches,
+        samples_count: int,
+        average_precision: float,
+    ) -> ClassMetricsPerTestCase:
+        matched = class_matches.matched
+        unmatched_gt = class_matches.unmatched_gt
+        unmatched_inf = class_matches.unmatched_inf
+
+        tp = [inf for _, inf in matched if inf.score >= thresholds[inf.label]]
+        fp = [inf for inf in unmatched_inf if inf.score >= thresholds[inf.label]]
+        fn = [gt for gt, _ in unmatched_gt] + [gt for gt, inf in matched if inf.score < thresholds[inf.label]]
         tp_count = len(tp)
         fp_count = len(fp)
         fn_count = len(fn)
-        confused_count = len(confused)
         precision = compute_precision(tp_count, fp_count)
         recall = compute_recall(tp_count, fn_count)
         f1_score = compute_f1_score(tp_count, fp_count, fn_count)
 
-        average_precision = 0.0
-        if precision > 0:
-            baseline_pr_curve = compute_pr_curve(all_bbox_matches_for_one_label)
-            if baseline_pr_curve is not None:
-                average_precision = compute_average_precision(baseline_pr_curve.y, baseline_pr_curve.x)
-
         return ClassMetricsPerTestCase(
             Class=label,
-            nImages=samples_with_label,
+            nImages=samples_count,
             Threshold=thresholds[label],
             Objects=tp_count + fn_count,
             Inferences=tp_count + fp_count,
             TP=tp_count,
             FN=fn_count,
             FP=fp_count,
-            Confused=confused_count,
             Precision=precision,
             Recall=recall,
             F1=f1_score,
             AP=average_precision,
         )
 
+    def compute_aggregate_label_metrics(
+        self,
+        matchings: List[MulticlassInferenceMatches],
+        label: str,
+        thresholds: Dict[str, float],
+    ) -> ClassMetricsPerTestCase:
+        match_and_count: Tuple[MulticlassInferenceMatches, int] = self.bbox_matches_for_one_label(matchings, label)
+        class_matches: MulticlassInferenceMatches = match_and_count[0]
+        samples_count: int = match_and_count[1]
+
+        average_precision = 0.0
+        baseline_pr_curve = compute_pr_curve([class_matches])
+        if baseline_pr_curve is not None:
+            average_precision = compute_average_precision(baseline_pr_curve.y, baseline_pr_curve.x)
+
+        return self.class_metrics_per_test_case(label, thresholds, class_matches, samples_count, average_precision)
+
+    def test_case_metrics(
+        self,
+        per_class_metrics: List[ClassMetricsPerTestCase],
+        metrics: List[TestSampleMetrics],
+    ) -> TestCaseMetrics:
+        tp_count = sum(im.count_TP for im in metrics)
+        fp_count = sum(im.count_FP for im in metrics)
+        fn_count = sum(im.count_FN for im in metrics)
+        ignored_count = sum(1 if im.ignored else 0 for im in metrics)
+        return TestCaseMetrics(
+            PerClass=per_class_metrics,
+            Objects=tp_count + fn_count,
+            Inferences=tp_count + fp_count,
+            TP=tp_count,
+            FN=fn_count,
+            FP=fp_count,
+            nIgnored=ignored_count,
+            macro_Precision=np.mean([data.Precision for data in per_class_metrics]) if per_class_metrics else 0.0,
+            macro_Recall=np.mean([data.Recall for data in per_class_metrics]) if per_class_metrics else 0.0,
+            macro_F1=np.mean([data.F1 for data in per_class_metrics]) if per_class_metrics else 0.0,
+            mean_AP=np.mean([data.AP for data in per_class_metrics]) if per_class_metrics else 0.0,
+        )
+
     def compute_test_case_metrics(
         self,
         test_case: TestCase,
         inferences: List[Tuple[TestSample, GroundTruth, Inference]],
         metrics: List[TestSampleMetrics],
         configuration: Optional[ThresholdConfiguration] = None,
     ) -> TestCaseMetrics:
         assert configuration is not None, "must specify configuration"
         thresholds = self.get_confidence_thresholds(configuration)
-        labels = {gt.label for _, gts, _ in inferences for gt in gts.bboxes}
         all_bbox_matches = self.matchings_by_test_case[test_case.name]
+        self.locators_by_test_case[test_case.name] = [ts.locator for ts, _, _ in inferences]
 
         # compute nested metrics per class
+        labels = {gt.label for _, gts, _ in inferences for gt in gts.bboxes}
         per_class_metrics: List[ClassMetricsPerTestCase] = []
         for label in sorted(labels):
             metrics_per_class = self.compute_aggregate_label_metrics(all_bbox_matches, label, thresholds)
             per_class_metrics.append(metrics_per_class)
 
-        self.locators_by_test_case[test_case.name] = [ts.locator for ts, _, _ in inferences]
-        tp_count = sum(im.count_TP for im in metrics)
-        fp_count = sum(im.count_FP for im in metrics)
-        fn_count = sum(im.count_FN for im in metrics)
-
-        return TestCaseMetrics(
-            PerClass=per_class_metrics,
-            Objects=tp_count + fn_count,
-            Inferences=tp_count + fp_count,
-            TP=tp_count,
-            FN=fn_count,
-            FP=fp_count,
-            macro_Precision=np.mean([class_metrics.Precision for class_metrics in per_class_metrics]),
-            macro_Recall=np.mean([class_metrics.Recall for class_metrics in per_class_metrics]),
-            macro_F1=np.mean([class_metrics.F1 for class_metrics in per_class_metrics]),
-            mean_AP=np.mean([class_metrics.AP for class_metrics in per_class_metrics]),
-        )
+        return self.test_case_metrics(per_class_metrics, metrics)
 
     def compute_test_case_plots(
         self,
         test_case: TestCase,
         inferences: List[Tuple[TestSample, GroundTruth, Inference]],
         metrics: List[TestSampleMetrics],
         configuration: Optional[ThresholdConfiguration] = None,
@@ -316,25 +389,30 @@
                     compute_confusion_matrix_plot(confusion_matrix_matchings),
                 ],
             ),
         )
 
         return plots
 
+    def test_suite_metrics(self, unique_locators: Set[str], average_precisions: List[float]) -> TestSuiteMetrics:
+        return TestSuiteMetrics(
+            n_images=len(unique_locators),
+            mean_AP=np.mean(average_precisions) if average_precisions else 0.0,
+        )
+
     def compute_test_suite_metrics(
         self,
         test_suite: TestSuite,
         metrics: List[Tuple[TestCase, TestCaseMetrics]],
         configuration: Optional[ThresholdConfiguration] = None,
     ) -> TestSuiteMetrics:
         assert configuration is not None, "must specify configuration"
-        return TestSuiteMetrics(
-            n_images=len({locator for tc, _ in metrics for locator in self.locators_by_test_case[tc.name]}),
-            mean_AP=np.average([tcm.mean_AP for _, tcm in metrics]),
-        )
+        unique_locators = {locator for tc, _ in metrics for locator in self.locators_by_test_case[tc.name]}
+        average_precisions = [tcm.mean_AP for _, tcm in metrics]
+        return self.test_suite_metrics(unique_locators, average_precisions)
 
     def get_confidence_thresholds(self, configuration: ThresholdConfiguration) -> Dict[str, float]:
         if configuration.threshold_strategy == ThresholdStrategy.FIXED_03:
             return defaultdict(lambda: 0.3)
         if configuration.threshold_strategy == ThresholdStrategy.FIXED_05:
             return defaultdict(lambda: 0.5)
         if configuration.threshold_strategy == ThresholdStrategy.FIXED_075:
```

### Comparing `kolena_client-0.79.1/kolena/_experimental/object_detection/evaluator_single_class.py` & `kolena_client-0.80.0/kolena/_experimental/object_detection/evaluator_single_class.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,33 +11,35 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from collections import defaultdict
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import Set
 from typing import Tuple
 
 import numpy as np
 
+from kolena._experimental.object_detection import GroundTruth
+from kolena._experimental.object_detection import Inference
+from kolena._experimental.object_detection import TestCase
+from kolena._experimental.object_detection import TestCaseMetricsSingleClass
+from kolena._experimental.object_detection import TestSample
+from kolena._experimental.object_detection import TestSampleMetricsSingleClass
+from kolena._experimental.object_detection import TestSuite
+from kolena._experimental.object_detection import TestSuiteMetrics
+from kolena._experimental.object_detection import ThresholdConfiguration
+from kolena._experimental.object_detection import ThresholdStrategy
 from kolena._experimental.object_detection.utils import compute_average_precision
 from kolena._experimental.object_detection.utils import compute_f1_plot
 from kolena._experimental.object_detection.utils import compute_optimal_f1_threshold
 from kolena._experimental.object_detection.utils import compute_pr_curve
 from kolena._experimental.object_detection.utils import compute_pr_plot
-from kolena._experimental.object_detection.workflow import GroundTruth
-from kolena._experimental.object_detection.workflow import Inference
-from kolena._experimental.object_detection.workflow import TestCase
-from kolena._experimental.object_detection.workflow import TestCaseMetricsSingleClass
-from kolena._experimental.object_detection.workflow import TestSample
-from kolena._experimental.object_detection.workflow import TestSampleMetricsSingleClass
-from kolena._experimental.object_detection.workflow import TestSuite
-from kolena._experimental.object_detection.workflow import TestSuiteMetrics
-from kolena._experimental.object_detection.workflow import ThresholdConfiguration
-from kolena._experimental.object_detection.workflow import ThresholdStrategy
+from kolena._experimental.object_detection.utils import filter_inferences
 from kolena.workflow import Evaluator
 from kolena.workflow import Plot
 from kolena.workflow.metrics import f1_score as compute_f1_score
 from kolena.workflow.metrics import InferenceMatches
 from kolena.workflow.metrics import match_inferences
 from kolena.workflow.metrics import precision as compute_precision
 from kolena.workflow.metrics import recall as compute_recall
@@ -68,31 +70,39 @@
     """
 
     matchings_by_test_case: Dict[str, List[InferenceMatches]] = defaultdict(list)
     """
     Caches matchings per test case for test case metrics and test case plots.
     """
 
-    def compute_image_metrics(
+    def test_sample_metrics_ignored(
         self,
-        ground_truth: GroundTruth,
-        inference: Inference,
-        configuration: ThresholdConfiguration,
-        test_case_name: str,
+        thresholds: float,
     ) -> TestSampleMetricsSingleClass:
-        assert configuration is not None, "must specify configuration"
-        thresholds = self.get_confidence_thresholds(configuration)
-        bbox_matches: InferenceMatches = match_inferences(
-            ground_truth.bboxes,
-            [inf for inf in inference.bboxes if inf.score >= configuration.min_confidence_score],
-            ignored_ground_truths=ground_truth.ignored_bboxes,
-            mode="pascal",
-            iou_threshold=configuration.iou_threshold,
+        return TestSampleMetricsSingleClass(
+            TP=[],
+            FP=[],
+            FN=[],
+            count_TP=0,
+            count_FP=0,
+            count_FN=0,
+            has_TP=False,
+            has_FP=False,
+            has_FN=False,
+            ignored=True,
+            max_confidence_above_t=None,
+            min_confidence_above_t=None,
+            thresholds=thresholds,
         )
-        self.matchings_by_test_case[test_case_name].append(bbox_matches)
+
+    def test_sample_metrics_single_class(
+        self,
+        bbox_matches: InferenceMatches,
+        thresholds: float,
+    ) -> TestSampleMetricsSingleClass:
         tp = [inf for _, inf in bbox_matches.matched if inf.score >= thresholds]
         fp = [inf for inf in bbox_matches.unmatched_inf if inf.score >= thresholds]
         fn = bbox_matches.unmatched_gt + [gt for gt, inf in bbox_matches.matched if inf.score < thresholds]
         non_ignored_inferences = tp + fp
         scores = [inf.score for inf in non_ignored_inferences]
         return TestSampleMetricsSingleClass(
             TP=tp,
@@ -100,39 +110,64 @@
             FN=fn,
             count_TP=len(tp),
             count_FP=len(fp),
             count_FN=len(fn),
             has_TP=len(tp) > 0,
             has_FP=len(fp) > 0,
             has_FN=len(fn) > 0,
+            ignored=False,
             max_confidence_above_t=max(scores) if len(scores) > 0 else None,
             min_confidence_above_t=min(scores) if len(scores) > 0 else None,
             thresholds=thresholds,
         )
 
+    def compute_image_metrics(
+        self,
+        ground_truth: GroundTruth,
+        inference: Inference,
+        configuration: ThresholdConfiguration,
+        test_case_name: str,
+    ) -> TestSampleMetricsSingleClass:
+        assert configuration is not None, "must specify configuration"
+        thresholds = self.get_confidence_thresholds(configuration)
+        if inference.ignored:
+            return self.test_sample_metrics_ignored(thresholds)
+
+        bbox_matches: InferenceMatches = match_inferences(
+            ground_truth.bboxes,
+            filter_inferences(inferences=inference.bboxes, confidence_score=configuration.min_confidence_score),
+            ignored_ground_truths=ground_truth.ignored_bboxes,
+            mode="pascal",
+            iou_threshold=configuration.iou_threshold,
+        )
+        self.matchings_by_test_case[test_case_name].append(bbox_matches)
+
+        return self.test_sample_metrics_single_class(bbox_matches, thresholds)
+
     def compute_and_cache_f1_optimal_thresholds(
         self,
         configuration: ThresholdConfiguration,
         inferences: List[Tuple[TestSample, GroundTruth, Inference]],
     ) -> None:
         if configuration.threshold_strategy != ThresholdStrategy.F1_OPTIMAL:
             return
 
         if configuration.display_name() in self.threshold_cache.keys():
             return
 
         all_bbox_matches = [
             match_inferences(
                 ground_truth.bboxes,
-                [inf for inf in inference.bboxes if inf.score >= configuration.min_confidence_score],
+                filter_inferences(inferences=inference.bboxes, confidence_score=configuration.min_confidence_score),
                 ignored_ground_truths=ground_truth.ignored_bboxes,
                 mode="pascal",
                 iou_threshold=configuration.iou_threshold,
             )
             for _, ground_truth, inference in inferences
+            if not inference.ignored
         ]
         optimal_thresholds = compute_optimal_f1_threshold(all_bbox_matches)
         self.threshold_cache[configuration.display_name()] = max(configuration.min_confidence_score, optimal_thresholds)
 
     def compute_test_sample_metrics(
         self,
         test_case: TestCase,
@@ -140,51 +175,59 @@
         configuration: Optional[ThresholdConfiguration] = None,
     ) -> List[Tuple[TestSample, TestSampleMetricsSingleClass]]:
         assert configuration is not None, "must specify configuration"
         # compute thresholds to cache values for subsequent steps
         self.compute_and_cache_f1_optimal_thresholds(configuration, inferences)
         return [(ts, self.compute_image_metrics(gt, inf, configuration, test_case.name)) for ts, gt, inf in inferences]
 
-    def compute_test_case_metrics(
+    def test_case_metrics_single_class(
         self,
-        test_case: TestCase,
-        inferences: List[Tuple[TestSample, GroundTruth, Inference]],
         metrics: List[TestSampleMetricsSingleClass],
-        configuration: Optional[ThresholdConfiguration] = None,
+        average_precision: float,
     ) -> TestCaseMetricsSingleClass:
-        assert configuration is not None, "must specify configuration"
-        all_bbox_matches = self.matchings_by_test_case[test_case.name]
-
-        self.locators_by_test_case[test_case.name] = [ts.locator for ts, _, _ in inferences]
         tp_count = sum(im.count_TP for im in metrics)
         fp_count = sum(im.count_FP for im in metrics)
         fn_count = sum(im.count_FN for im in metrics)
+        ignored_count = sum(1 if im.ignored else 0 for im in metrics)
 
         precision = compute_precision(tp_count, fp_count)
         recall = compute_recall(tp_count, fn_count)
         f1_score = compute_f1_score(tp_count, fp_count, fn_count)
 
-        average_precision = 0.0
-        if precision > 0:
-            baseline_pr_curve = compute_pr_curve(all_bbox_matches)
-            if baseline_pr_curve is not None:
-                average_precision = compute_average_precision(baseline_pr_curve.y, baseline_pr_curve.x)
-
         return TestCaseMetricsSingleClass(
             Objects=tp_count + fn_count,
             Inferences=tp_count + fp_count,
             TP=tp_count,
             FN=fn_count,
             FP=fp_count,
+            nIgnored=ignored_count,
             Precision=precision,
             Recall=recall,
             F1=f1_score,
             AP=average_precision,
         )
 
+    def compute_test_case_metrics(
+        self,
+        test_case: TestCase,
+        inferences: List[Tuple[TestSample, GroundTruth, Inference]],
+        metrics: List[TestSampleMetricsSingleClass],
+        configuration: Optional[ThresholdConfiguration] = None,
+    ) -> TestCaseMetricsSingleClass:
+        assert configuration is not None, "must specify configuration"
+        all_bbox_matches = self.matchings_by_test_case[test_case.name]
+        self.locators_by_test_case[test_case.name] = [ts.locator for ts, _, _ in inferences]
+
+        average_precision = 0.0
+        baseline_pr_curve = compute_pr_curve(all_bbox_matches)
+        if baseline_pr_curve is not None:
+            average_precision = compute_average_precision(baseline_pr_curve.y, baseline_pr_curve.x)
+
+        return self.test_case_metrics_single_class(metrics, average_precision)
+
     def compute_test_case_plots(
         self,
         test_case: TestCase,
         inferences: List[Tuple[TestSample, GroundTruth, Inference]],
         metrics: List[TestSampleMetricsSingleClass],
         configuration: Optional[ThresholdConfiguration] = None,
     ) -> Optional[List[Plot]]:
@@ -200,25 +243,30 @@
                     compute_f1_plot(all_bbox_matches),
                 ],
             ),
         )
 
         return plots
 
+    def test_suite_metrics(self, unique_locators: Set[str], average_precisions: List[float]) -> TestSuiteMetrics:
+        return TestSuiteMetrics(
+            n_images=len(unique_locators),
+            mean_AP=np.mean(average_precisions) if average_precisions else 0.0,
+        )
+
     def compute_test_suite_metrics(
         self,
         test_suite: TestSuite,
         metrics: List[Tuple[TestCase, TestCaseMetricsSingleClass]],
         configuration: Optional[ThresholdConfiguration] = None,
     ) -> TestSuiteMetrics:
         assert configuration is not None, "must specify configuration"
-        return TestSuiteMetrics(
-            n_images=len({locator for tc, _ in metrics for locator in self.locators_by_test_case[tc.name]}),
-            mean_AP=np.average([tcm.AP for _, tcm in metrics]),
-        )
+        unique_locators = {locator for tc, _ in metrics for locator in self.locators_by_test_case[tc.name]}
+        average_precisions = [tcm.AP for _, tcm in metrics]
+        return self.test_suite_metrics(unique_locators, average_precisions)
 
     def get_confidence_thresholds(self, configuration: ThresholdConfiguration) -> float:
         if configuration.threshold_strategy == ThresholdStrategy.FIXED_03:
             return 0.3
         if configuration.threshold_strategy == ThresholdStrategy.FIXED_05:
             return 0.5
         if configuration.threshold_strategy == ThresholdStrategy.FIXED_075:
```

### Comparing `kolena_client-0.79.1/kolena/_experimental/object_detection/utils.py` & `kolena_client-0.80.0/kolena/_experimental/object_detection/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Tuple
 from typing import Union
 
+from kolena.workflow.annotation import ScoredLabeledBoundingBox
+
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 import numpy as np
 
@@ -31,14 +33,27 @@
 from kolena.workflow import ConfusionMatrix
 from kolena.workflow import Curve
 from kolena.workflow import CurvePlot
 from kolena.workflow.metrics import InferenceMatches
 from kolena.workflow.metrics import MulticlassInferenceMatches
 
 
+def filter_inferences(
+    inferences: List[ScoredLabeledBoundingBox],
+    confidence_score: Optional[float] = None,
+    labels: Optional[Set[str]] = None,
+) -> List[ScoredLabeledBoundingBox]:
+    filtered_by_confidence = (
+        [inf for inf in inferences if inf.score >= confidence_score] if confidence_score else inferences
+    )
+    if labels is None:
+        return filtered_by_confidence
+    return [inf for inf in filtered_by_confidence if inf.label in labels]
+
+
 def _compute_sklearn_arrays(
     all_matches: List[Union[MulticlassInferenceMatches, InferenceMatches]],
 ) -> Tuple[np.ndarray, np.ndarray]:
     y_true: List[int] = []
     y_score: List[float] = []
     for image_bbox_matches in all_matches:
         for _, bbox_inf in image_bbox_matches.matched:  # TP (if above threshold)
@@ -75,26 +90,36 @@
         precision, recall, f1, _ = sklearn_metrics.precision_recall_fscore_support(
             y_true,
             y_pred,
             average="binary",
             zero_division=0,
         )
 
-        precisions.append(precision)
-        recalls.append(recall)
+        # avoid curves with one x-value and two y-values
+        if recall in recalls:
+            idx = recalls.index(recall)
+            precisions[idx] = max(precisions[idx], precision)
+        else:
+            precisions.append(precision)
+            recalls.append(recall)
         f1s.append(f1)
 
-    # Omit curves with only one point
-    if len(f1s) < 2:
+    # omit curves with no points
+    if len(f1s) == 0 or len(precisions) == 0 or len(recalls) == 0:
         return None
 
     if curve_type == "f1":
-        return Curve(x=thresholds, y=f1s, label=curve_label)
+        return Curve(x=thresholds, y=f1s, label=curve_label) if len(f1s) >= 2 else None
     else:
-        return Curve(x=recalls, y=precisions, label=curve_label)
+        # add a point to start the PR curve on the vertical axis if needed
+        if 0.0 not in recalls:
+            minpos = recalls.index(min(recalls))
+            precisions.append(precisions[minpos])
+            recalls.append(0.0)
+        return Curve(x=recalls, y=precisions, label=curve_label) if len(recalls) >= 2 else None
 
 
 def _compute_multiclass_curves(
     all_matches: List[MulticlassInferenceMatches],
     curve_type: Literal["pr", "f1"],
 ) -> Optional[List[Curve]]:
     curves: List[Curve] = []
```

### Comparing `kolena_client-0.79.1/kolena/_extras/__init__.py` & `kolena_client-0.80.0/kolena/_extras/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_extras/metrics/__init__.py` & `kolena_client-0.80.0/kolena/_extras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_extras/metrics/sklearn.py` & `kolena_client-0.80.0/kolena/_extras/metrics/sklearn.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 try:
     import sklearn.metrics as sklearn_metrics  # noqa: F401
 
 except ImportError:
-    raise ImportError("Package 'scikit-learn' not found; install 'metrics' extra with `pip install kolena[metrics]`")
+    raise ImportError("Package 'scikit-learn' not found; install 'metrics' extra with `pip install 'kolena[metrics]'`")
```

### Comparing `kolena_client-0.79.1/kolena/_utils/__init__.py` & `kolena_client-0.80.0/kolena/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_utils/asset_path_mapper.py` & `kolena_client-0.80.0/kolena/_utils/asset_path_mapper.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_utils/batched_load.py` & `kolena_client-0.80.0/kolena/_utils/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_utils/cli.py` & `kolena_client-0.80.0/kolena/_utils/cli.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_utils/consts.py` & `kolena_client-0.80.0/kolena/_utils/consts.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_utils/dataframes/__init__.py` & `kolena_client-0.80.0/kolena/_utils/dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_utils/dataframes/validators.py` & `kolena_client-0.80.0/kolena/_utils/dataframes/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_utils/datatypes.py` & `kolena_client-0.80.0/kolena/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_utils/endpoints.py` & `kolena_client-0.80.0/kolena/_utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_utils/frozen.py` & `kolena_client-0.80.0/kolena/_utils/frozen.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_utils/geometry.py` & `kolena_client-0.80.0/kolena/_utils/geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_utils/inference_validators.py` & `kolena_client-0.80.0/kolena/_utils/inference_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_utils/instrumentation.py` & `kolena_client-0.80.0/kolena/_utils/instrumentation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_utils/krequests.py` & `kolena_client-0.80.0/kolena/_utils/krequests.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_utils/log.py` & `kolena_client-0.80.0/kolena/_utils/log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_utils/repository.py` & `kolena_client-0.80.0/kolena/_utils/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_utils/serde.py` & `kolena_client-0.80.0/kolena/_utils/serde.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_utils/serializable.py` & `kolena_client-0.80.0/kolena/_utils/serializable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_utils/state.py` & `kolena_client-0.80.0/kolena/_utils/state.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_utils/uninstantiable.py` & `kolena_client-0.80.0/kolena/_utils/uninstantiable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/_utils/validators.py` & `kolena_client-0.80.0/kolena/_utils/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/classification/__init__.py` & `kolena_client-0.80.0/kolena/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/classification/metadata.py` & `kolena_client-0.80.0/kolena/classification/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/classification/model.py` & `kolena_client-0.80.0/kolena/classification/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/classification/multiclass/__init__.py` & `kolena_client-0.80.0/kolena/detection/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,32 +9,42 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # noreorder
-from .workflow import TestSample
-from .workflow import GroundTruth
-from .workflow import InferenceLabel
-from .workflow import Inference
-from .workflow import TestCase
-from .workflow import TestSuite
-from .workflow import Model
-from .workflow import ThresholdConfiguration
-from .evaluator import MulticlassClassificationEvaluator
+from kolena._api.v1.detection import CustomMetrics
+from .ground_truth import GroundTruth
+from .inference import Inference
+from .test_config import TestConfig
+from .test_config import FixedGlobalThreshold
+from .test_config import F1Optimal
+from .test_image import TestImage
+from .test_image import iter_images
+from .test_image import load_images
+from .test_case import TestCase
+from .test_suite import TestSuite
+from .model import Model
+from .model import InferenceModel
+from .test_run import CustomMetricsCallback
 from .test_run import TestRun
 from .test_run import test
 
 __all__ = [
-    "TestSample",
     "GroundTruth",
-    "InferenceLabel",
     "Inference",
+    "TestConfig",
+    "FixedGlobalThreshold",
+    "F1Optimal",
+    "TestImage",
+    "iter_images",
+    "load_images",
     "TestCase",
     "TestSuite",
+    "InferenceModel",
     "Model",
-    "ThresholdConfiguration",
-    "MulticlassClassificationEvaluator",
+    "CustomMetrics",
+    "CustomMetricsCallback",
     "TestRun",
     "test",
 ]
```

### Comparing `kolena_client-0.79.1/kolena/classification/multiclass/_utils.py` & `kolena_client-0.80.0/kolena/classification/multiclass/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/classification/multiclass/evaluator.py` & `kolena_client-0.80.0/kolena/classification/multiclass/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/classification/multiclass/test_run.py` & `kolena_client-0.80.0/kolena/classification/multiclass/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/classification/multiclass/workflow.py` & `kolena_client-0.80.0/kolena/classification/multiclass/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/classification/test_case.py` & `kolena_client-0.80.0/kolena/classification/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/classification/test_config.py` & `kolena_client-0.80.0/kolena/classification/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/classification/test_image.py` & `kolena_client-0.80.0/kolena/classification/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/classification/test_run.py` & `kolena_client-0.80.0/kolena/classification/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/classification/test_suite.py` & `kolena_client-0.80.0/kolena/classification/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/detection/_datatypes.py` & `kolena_client-0.80.0/kolena/detection/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/detection/_internal/__init__.py` & `kolena_client-0.80.0/kolena/detection/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/detection/_internal/datatypes.py` & `kolena_client-0.80.0/kolena/detection/_internal/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/detection/_internal/ground_truth.py` & `kolena_client-0.80.0/kolena/detection/_internal/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/detection/_internal/inference.py` & `kolena_client-0.80.0/kolena/detection/_internal/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/detection/_internal/metadata.py` & `kolena_client-0.80.0/kolena/detection/_internal/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/detection/_internal/model.py` & `kolena_client-0.80.0/kolena/detection/_internal/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/detection/_internal/test_case.py` & `kolena_client-0.80.0/kolena/detection/_internal/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/detection/_internal/test_config.py` & `kolena_client-0.80.0/kolena/detection/_internal/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/detection/_internal/test_image.py` & `kolena_client-0.80.0/kolena/detection/_internal/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/detection/_internal/test_run.py` & `kolena_client-0.80.0/kolena/detection/_internal/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/detection/_internal/test_suite.py` & `kolena_client-0.80.0/kolena/detection/_internal/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/detection/ground_truth.py` & `kolena_client-0.80.0/kolena/detection/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/detection/inference.py` & `kolena_client-0.80.0/kolena/detection/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/detection/metadata.py` & `kolena_client-0.80.0/kolena/detection/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/detection/model.py` & `kolena_client-0.80.0/kolena/detection/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/detection/test_case.py` & `kolena_client-0.80.0/kolena/detection/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/detection/test_config.py` & `kolena_client-0.80.0/kolena/detection/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/detection/test_image.py` & `kolena_client-0.80.0/kolena/detection/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/detection/test_run.py` & `kolena_client-0.80.0/kolena/detection/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/detection/test_suite.py` & `kolena_client-0.80.0/kolena/detection/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/errors.py` & `kolena_client-0.80.0/kolena/errors.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/fr/__init__.py` & `kolena_client-0.80.0/kolena/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/fr/_utils.py` & `kolena_client-0.80.0/kolena/fr/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/fr/datatypes.py` & `kolena_client-0.80.0/kolena/fr/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/fr/model.py` & `kolena_client-0.80.0/kolena/fr/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/fr/test_case.py` & `kolena_client-0.80.0/kolena/fr/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/fr/test_images.py` & `kolena_client-0.80.0/kolena/fr/test_images.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/fr/test_run.py` & `kolena_client-0.80.0/kolena/fr/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/fr/test_suite.py` & `kolena_client-0.80.0/kolena/fr/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/initialize.py` & `kolena_client-0.80.0/kolena/initialize.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/__init__.py` & `kolena_client-0.80.0/kolena/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/_datatypes.py` & `kolena_client-0.80.0/kolena/workflow/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/_validators.py` & `kolena_client-0.80.0/kolena/workflow/_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/annotation.py` & `kolena_client-0.80.0/kolena/workflow/annotation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/asset.py` & `kolena_client-0.80.0/kolena/workflow/asset.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/define_workflow.py` & `kolena_client-0.80.0/kolena/workflow/define_workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/evaluator.py` & `kolena_client-0.80.0/kolena/workflow/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/evaluator_function.py` & `kolena_client-0.80.0/kolena/workflow/evaluator_function.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/ground_truth.py` & `kolena_client-0.80.0/kolena/workflow/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/inference.py` & `kolena_client-0.80.0/kolena/workflow/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/metrics/__init__.py` & `kolena_client-0.80.0/kolena/workflow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/metrics/_formula.py` & `kolena_client-0.80.0/kolena/workflow/metrics/_formula.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/metrics/_geometry.py` & `kolena_client-0.80.0/kolena/workflow/metrics/_geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/model.py` & `kolena_client-0.80.0/kolena/workflow/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/plot.py` & `kolena_client-0.80.0/kolena/workflow/plot.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/test_case.py` & `kolena_client-0.80.0/kolena/workflow/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/test_run.py` & `kolena_client-0.80.0/kolena/workflow/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/test_sample.py` & `kolena_client-0.80.0/kolena/workflow/test_sample.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/test_suite.py` & `kolena_client-0.80.0/kolena/workflow/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/visualization/__init__.py` & `kolena_client-0.80.0/kolena/workflow/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/visualization/_activation_map.py` & `kolena_client-0.80.0/kolena/workflow/visualization/_activation_map.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/visualization/_utils.py` & `kolena_client-0.80.0/kolena/workflow/visualization/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/kolena/workflow/workflow.py` & `kolena_client-0.80.0/kolena/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.79.1/pyproject.toml` & `kolena_client-0.80.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kolena-client"
-version = "0.79.1"  # version is automatically set to latest git tag during release process
+version = "0.80.0"  # version is automatically set to latest git tag during release process
 description = "Client for Kolena's machine learning testing platform."
 authors = ["Kolena Engineering <eng@kolena.io>"]
 homepage = "https://kolena.io"
 documentation = "https://docs.kolena.io"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["Kolena", "ML", "testing"]
@@ -70,15 +70,15 @@
 mkdocs-git-committers-plugin-2 = "^1.1.2"
 mkdocs-git-revision-date-localized-plugin = "^1.2.0"
 
 [tool.poetry.scripts]
 kolena = 'kolena._utils.cli:run'
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 # do not scan 'kolena' for tests, as there are many functions/classes that look like tests
 norecursedirs = "kolena"
 # explicitly disable test classes such that e.g. TestRun is not interpreted as a test
 python_classes = []
```

### Comparing `kolena_client-0.79.1/PKG-INFO` & `kolena_client-0.80.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolena-client
-Version: 0.79.1
+Version: 0.80.0
 Summary: Client for Kolena's machine learning testing platform.
 Home-page: https://kolena.io
 License: Apache-2.0
 Keywords: Kolena,ML,testing
 Author: Kolena Engineering
 Author-email: eng@kolena.io
 Requires-Python: >=3.7.1,<3.12
@@ -46,15 +46,17 @@
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Requires-Dist: tqdm (>=4,<5)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; python_version < "3.8"
 Project-URL: Documentation, https://docs.kolena.io
 Description-Content-Type: text/markdown
 
 <p align="center">
-  <img src="https://docs.kolena.io/assets/images/kolena-banner.png" width="640" alt="Kolena" />
+  <a href="https://docs.kolena.io">
+    <img src="https://docs.kolena.io/assets/images/kolena-banner.png" width="640" alt="Kolena" />
+  </a>
 </p>
 
 <p align='center'>
   <a href="https://pypi.python.org/pypi/kolena"><img src="https://img.shields.io/pypi/v/kolena?logo=python&logoColor=white&style=flat-square" /></a>
   <a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/pypi/l/kolena?style=flat-square" /></a>
   <a href="https://github.com/kolenaIO/kolena/actions"><img src="https://img.shields.io/github/checks-status/kolenaIO/kolena/trunk?logo=circleci&logoColor=white&style=flat-square" /></a>
   <a href="https://codecov.io/gh/kolenaIO/kolena" ><img src="https://img.shields.io/codecov/c/github/kolenaIO/kolena?logo=codecov&logoColor=white&style=flat-square&token=8WOY5I8SF1" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kolena-client Version: 0.79.1 Summary: Client for
+Metadata-Version: 2.1 Name: kolena-client Version: 0.80.0 Summary: Client for
 Kolena's machine learning testing platform. Home-page: https://kolena.io
 License: Apache-2.0 Keywords: Kolena,ML,testing Author: Kolena Engineering
 Author-email: eng@kolena.io Requires-Python: >=3.7.1,<3.12 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

