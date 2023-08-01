# Comparing `tmp/shrike-2.0.0.dev6.tar.gz` & `tmp/shrike-2.0.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shrike-2.0.0.dev6.tar", last modified: Fri Jul 28 16:54:45 2023, max compression
+gzip compressed data, was "shrike-2.0.0.dev7.tar", last modified: Tue Aug  1 20:47:15 2023, max compression
```

## Comparing `shrike-2.0.0.dev6.tar` & `shrike-2.0.0.dev7.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:54:45.828761 shrike-2.0.0.dev6/
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)   252717 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     8629 2023-07-28 16:54:45.828761 shrike-2.0.0.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6977 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-28 16:54:45.828761 shrike-2.0.0.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2318 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:54:45.816761 shrike-2.0.0.dev6/shrike/
--rw-r--r--   0 runner    (1001) docker     (122)      399 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:54:45.816761 shrike-2.0.0.dev6/shrike/_core/
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4102 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/_core/eyesoff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/_core/testing.py
--rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:54:45.816761 shrike-2.0.0.dev6/shrike/build/
--rw-r--r--   0 runner    (1001) docker     (122)      427 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:54:45.816761 shrike-2.0.0.dev6/shrike/build/commands/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/build/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    59472 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/build/commands/prepare.py
--rw-r--r--   0 runner    (1001) docker     (122)     7756 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/build/commands/register.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:54:45.816761 shrike-2.0.0.dev6/shrike/build/core/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/build/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14964 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/build/core/command_line.py
--rw-r--r--   0 runner    (1001) docker     (122)     8463 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/build/core/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:54:45.816761 shrike-2.0.0.dev6/shrike/build/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/build/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5526 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/build/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:54:45.820761 shrike-2.0.0.dev6/shrike/compliant_logging/
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/compliant_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6036 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/compliant_logging/argparser_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/compliant_logging/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    10327 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/compliant_logging/data_conversions.py
--rw-r--r--   0 runner    (1001) docker     (122)    16169 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/compliant_logging/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    41143 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/compliant_logging/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)    10311 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/compliant_logging/progress.py
--rw-r--r--   0 runner    (1001) docker     (122)     4875 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/compliant_logging/stack_trace_extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/compliant_logging/system_info.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:54:45.820761 shrike-2.0.0.dev6/shrike/distributed/
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9037 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/distributed/cluster_auto_setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     9829 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/distributed/dask.py
--rw-r--r--   0 runner    (1001) docker     (122)     4130 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/distributed/mpi_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)     5414 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/distributed/ray.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:54:45.820761 shrike-2.0.0.dev6/shrike/pipeline/
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/aml_connect.py
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/argparser_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7223 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/canary_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:54:45.812761 shrike-2.0.0.dev6/shrike/pipeline/components/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:54:45.824761 shrike-2.0.0.dev6/shrike/pipeline/components/fedavg/
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/components/fedavg/env.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/components/fedavg/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     3131 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/components/fedavg/spec.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    38725 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/federated_learning.py
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/module_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    20048 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/module_helper_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    20768 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/pipeline_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/pipeline_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    42859 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/pipeline_helper_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/ray_actor.py
--rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/telemetry_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:54:45.824761 shrike-2.0.0.dev6/shrike/pipeline/testing/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24460 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/testing/components.py
--rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/testing/importer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1837 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/testing/module_run_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     7894 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/testing/pipeline_class_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     7520 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/testing/pipeline_class_test_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:54:45.824761 shrike-2.0.0.dev6/shrike/pipeline/v1/
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5039 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/v1/aml_connect.py
--rw-r--r--   0 runner    (1001) docker     (122)     3565 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/v1/module_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    75663 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/v1/pipeline_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:54:45.824761 shrike-2.0.0.dev6/shrike/pipeline/v2/
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/v2/aml_connect.py
--rw-r--r--   0 runner    (1001) docker     (122)     3839 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/v2/module_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    67952 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/pipeline/v2/pipeline_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:54:45.824761 shrike-2.0.0.dev6/shrike/spark/
--rw-r--r--   0 runner    (1001) docker     (122)      187 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5221 2023-07-28 16:50:44.000000 shrike-2.0.0.dev6/shrike/spark/spark_net.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 16:54:45.816761 shrike-2.0.0.dev6/shrike.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8629 2023-07-28 16:54:45.000000 shrike-2.0.0.dev6/shrike.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-07-28 16:54:45.000000 shrike-2.0.0.dev6/shrike.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-28 16:54:45.000000 shrike-2.0.0.dev6/shrike.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1280 2023-07-28 16:54:45.000000 shrike-2.0.0.dev6/shrike.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-28 16:54:45.000000 shrike-2.0.0.dev6/shrike.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 20:47:15.947624 shrike-2.0.0.dev7/
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)   252717 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8629 2023-08-01 20:47:15.947624 shrike-2.0.0.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6977 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-01 20:47:15.947624 shrike-2.0.0.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2318 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 20:47:15.927624 shrike-2.0.0.dev7/shrike/
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 20:47:15.931624 shrike-2.0.0.dev7/shrike/_core/
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4102 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/_core/eyesoff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/_core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 20:47:15.931624 shrike-2.0.0.dev7/shrike/build/
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 20:47:15.931624 shrike-2.0.0.dev7/shrike/build/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/build/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    61132 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/build/commands/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7843 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/build/commands/register.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 20:47:15.931624 shrike-2.0.0.dev7/shrike/build/core/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/build/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14964 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/build/core/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8463 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/build/core/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 20:47:15.935624 shrike-2.0.0.dev7/shrike/build/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/build/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5526 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/build/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 20:47:15.935624 shrike-2.0.0.dev7/shrike/compliant_logging/
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/compliant_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6036 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/compliant_logging/argparser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/compliant_logging/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10327 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/compliant_logging/data_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16169 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/compliant_logging/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41143 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/compliant_logging/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10311 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/compliant_logging/progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4875 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/compliant_logging/stack_trace_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/compliant_logging/system_info.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 20:47:15.939624 shrike-2.0.0.dev7/shrike/distributed/
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9037 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/distributed/cluster_auto_setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9829 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/distributed/dask.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4130 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/distributed/mpi_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5414 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/distributed/ray.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 20:47:15.939624 shrike-2.0.0.dev7/shrike/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/aml_connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/argparser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7223 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/canary_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 20:47:15.923624 shrike-2.0.0.dev7/shrike/pipeline/components/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 20:47:15.943624 shrike-2.0.0.dev7/shrike/pipeline/components/fedavg/
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/components/fedavg/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/components/fedavg/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3131 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/components/fedavg/spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    38725 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/federated_learning.py
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/module_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20048 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/module_helper_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20768 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/pipeline_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/pipeline_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42859 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/pipeline_helper_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/ray_actor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/telemetry_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 20:47:15.943624 shrike-2.0.0.dev7/shrike/pipeline/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24460 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/testing/components.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/testing/importer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1837 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/testing/module_run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7894 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/testing/pipeline_class_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7520 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/testing/pipeline_class_test_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 20:47:15.943624 shrike-2.0.0.dev7/shrike/pipeline/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5039 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/v1/aml_connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3565 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/v1/module_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    75663 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/v1/pipeline_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 20:47:15.947624 shrike-2.0.0.dev7/shrike/pipeline/v2/
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/v2/aml_connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3839 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/v2/module_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    67952 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/pipeline/v2/pipeline_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 20:47:15.947624 shrike-2.0.0.dev7/shrike/spark/
+-rw-r--r--   0 runner    (1001) docker     (122)      187 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5221 2023-08-01 20:41:56.000000 shrike-2.0.0.dev7/shrike/spark/spark_net.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 20:47:15.931624 shrike-2.0.0.dev7/shrike.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8629 2023-08-01 20:47:15.000000 shrike-2.0.0.dev7/shrike.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-08-01 20:47:15.000000 shrike-2.0.0.dev7/shrike.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-01 20:47:15.000000 shrike-2.0.0.dev7/shrike.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1280 2023-08-01 20:47:15.000000 shrike-2.0.0.dev7/shrike.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-08-01 20:47:15.000000 shrike-2.0.0.dev7/shrike.egg-info/top_level.txt
```

### Comparing `shrike-2.0.0.dev6/LICENSE` & `shrike-2.0.0.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/NOTICE.txt` & `shrike-2.0.0.dev7/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/PKG-INFO` & `shrike-2.0.0.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shrike
-Version: 2.0.0.dev6
+Version: 2.0.0.dev7
 Summary: Python utilities for compliant Azure machine learning
 Home-page: https://github.com/ai-platform-ml-platform/shrike
 Author: AML Data Science
 Author-email: aml-ds@microsoft.com
 License: MIT
 Description: # Shrike: incubation for Azure ML
```

### Comparing `shrike-2.0.0.dev6/README.md` & `shrike-2.0.0.dev7/README.md`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/setup.py` & `shrike-2.0.0.dev7/setup.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/_core/eyesoff.py` & `shrike-2.0.0.dev7/shrike/_core/eyesoff.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/_core/testing.py` & `shrike-2.0.0.dev7/shrike/_core/testing.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/_core/utils.py` & `shrike-2.0.0.dev7/shrike/_core/utils.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/build/commands/prepare.py` & `shrike-2.0.0.dev7/shrike/build/commands/prepare.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,39 +132,68 @@
                     pool.map(self.validate_each_components, files)
                 pool.close()
                 pool.join()
             return rv  # type: ignore
 
     def build_each_components(self, component):
         """
-        For one of component specification file, run `az ml component build`,
+        For one of component specification file, run `mldesigner compile`,
         and register the status (+ register error if build failed).
         """
         path = Path(component)
-        res = subprocess.run(
-            args=f"mldesigner compile --source {component} --output {path.parent}/.build".split(), 
-            cwd = self.config.working_directory,
-            stdout = subprocess.PIPE,
-            stderr = subprocess.PIPE
-        )
-        stderr = str(res.stderr, encoding="utf-8", errors="ignore")
-        success_log = "Mldesigner has compiled 1 components from 1 files."
-        build_component_success = res.returncode == 0 and success_log in stderr
+        with open(component, "r") as spec_file:
+            spec = YAML(typ="safe").load(spec_file)
+        if isinstance(spec, dict) and spec.get("type") in ["spark", "SparkComponent"]:
+            build_component_success, stderr = self.build_spark_component(spec, path)
+        else:
+            res = subprocess.run(
+                args=f"mldesigner compile --source {component} --output {path.parent}/.build".split(), 
+                cwd = self.config.working_directory,
+                stdout = subprocess.PIPE,
+                stderr = subprocess.PIPE
+            )
+            stderr = str(res.stderr, encoding="utf-8", errors="ignore")
+            success_log = "Mldesigner has compiled 1 components from 1 files."
+            build_component_success = res.returncode == 0 and success_log in stderr
 
         if build_component_success:
             log.info(f"Component {component} is built.")
-            with open(component, "r") as spec_file:
-                spec = YAML(typ="safe").load(spec_file)
             component_name = spec.get("name")
             log.info(f"component_name {component_name}")
-            return str(path.parent / ".build" / component_name /path.name)
+            return str(path.parent / ".build" / component_name /path.name)  # type: ignore
         else:
             # if build fails, the path above won't exist, so no return
             self.register_error(f"Error when building component {component}. Logs: {stderr}")
 
+    def build_spark_component(self, spec, path_to_component_spec):
+        """
+        Manually compile spark component, workaround since `mldesigner compile`
+        does not support spark component for now.
+        """
+        try:
+            code = spec.get("code", ".")
+            component_name = spec.get("name")
+            compiled_folder = os.path.join(path_to_component_spec.parent, ".build", component_name)
+            shutil.copytree(path_to_component_spec.parent, compiled_folder)
+            if code not in [".", "./"]:
+                code_paths = [code] if isinstance(code, str) else code
+                for code_path in code_paths:
+                    source_path = os.path.join(path_to_component_spec.parent, code_path)
+                    if os.path.isdir(source_path):
+                        shutil.copytree(source_path, os.path.join(compiled_folder, Path(code_path).name))
+                    else:
+                        shutil.copy2(source_path, os.path.join(compiled_folder, Path(code_path).name))
+                spec["code"] = "./"
+            with open(os.path.join(compiled_folder, path_to_component_spec.name), "w") as f:
+                yaml.dump(spec, f)
+            return True, ""
+        except Exception as e:
+            return False, e
+
+
     def create_catalog_files(self, files: List[str]):
         """
         Create the appropriate kind of catalog file(s), using the configured
         method ("aml" or "aether").
         """
         signing_mode = self.config.signing_mode
 
@@ -983,16 +1012,19 @@
 
     def validate_each_components(self, component) -> None:
         """
         For one of component specification file, run `az ml component validate`,
         run compliance and customized validation if enabled,
         and register the status (+ register error if validation failed).
         """
+        validate_command = f"ml component validate --file {component}"
+        if self.config.verbose:
+            validate_command +=  " --debug"
         validate_component_success = self.execute_azure_cli_command(
-            f"ml component validate --file {component}", stderr_is_failure=False, check_stdout_result=True, ignore_blowfish=True
+            validate_command, stderr_is_failure=False, check_stdout_result=True, ignore_blowfish=True
         )
         compliance_validation_success = True
         customized_validation_success = True
         if self.config.enable_component_validation:
             log.info(f"Running compliance validation on {component}")
             compliance_validation_success = self.compliance_validation(component)
             if len(self.config.component_validation) > 0:
```

### Comparing `shrike-2.0.0.dev6/shrike/build/commands/register.py` & `shrike-2.0.0.dev7/shrike/build/commands/register.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,17 @@
             component_raw_version = self.config.all_component_version
             log.info(
                 f"Overwrite the component version with the specified value {self.config.all_component_version}"
             )
 
         if registry:
             register_command += f" --registry-name {registry}"
+        
+        if self.config.verbose:
+            register_command += " --debug"
 
         log.info(f"Register command is {register_command}")
         return register_command
 
     def read_component_version(self, yaml_file: str):
         yaml = YAML(typ="safe")
         with open(yaml_file, "r") as file:
```

### Comparing `shrike-2.0.0.dev6/shrike/build/core/command_line.py` & `shrike-2.0.0.dev7/shrike/build/core/command_line.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/build/core/configuration.py` & `shrike-2.0.0.dev7/shrike/build/core/configuration.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/build/utils/utils.py` & `shrike-2.0.0.dev7/shrike/build/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/compliant_logging/__init__.py` & `shrike-2.0.0.dev7/shrike/compliant_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/compliant_logging/argparser_utils.py` & `shrike-2.0.0.dev7/shrike/compliant_logging/argparser_utils.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/compliant_logging/data_conversions.py` & `shrike-2.0.0.dev7/shrike/compliant_logging/data_conversions.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/compliant_logging/exceptions.py` & `shrike-2.0.0.dev7/shrike/compliant_logging/exceptions.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/compliant_logging/logging.py` & `shrike-2.0.0.dev7/shrike/compliant_logging/logging.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/compliant_logging/progress.py` & `shrike-2.0.0.dev7/shrike/compliant_logging/progress.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/compliant_logging/stack_trace_extractor.py` & `shrike-2.0.0.dev7/shrike/compliant_logging/stack_trace_extractor.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/compliant_logging/system_info.py` & `shrike-2.0.0.dev7/shrike/compliant_logging/system_info.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/distributed/cluster_auto_setup.py` & `shrike-2.0.0.dev7/shrike/distributed/cluster_auto_setup.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/distributed/dask.py` & `shrike-2.0.0.dev7/shrike/distributed/dask.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/distributed/mpi_driver.py` & `shrike-2.0.0.dev7/shrike/distributed/mpi_driver.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/distributed/ray.py` & `shrike-2.0.0.dev7/shrike/distributed/ray.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/pipeline/__init__.py` & `shrike-2.0.0.dev7/shrike/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/pipeline/canary_helper.py` & `shrike-2.0.0.dev7/shrike/pipeline/canary_helper.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/pipeline/components/fedavg/run.py` & `shrike-2.0.0.dev7/shrike/pipeline/components/fedavg/run.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/pipeline/components/fedavg/spec.yaml` & `shrike-2.0.0.dev7/shrike/pipeline/components/fedavg/spec.yaml`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/pipeline/federated_learning.py` & `shrike-2.0.0.dev7/shrike/pipeline/federated_learning.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/pipeline/module_helper_base.py` & `shrike-2.0.0.dev7/shrike/pipeline/module_helper_base.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/pipeline/pipeline_config.py` & `shrike-2.0.0.dev7/shrike/pipeline/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/pipeline/pipeline_helper_base.py` & `shrike-2.0.0.dev7/shrike/pipeline/pipeline_helper_base.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/pipeline/ray_actor.py` & `shrike-2.0.0.dev7/shrike/pipeline/ray_actor.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/pipeline/telemetry_utils.py` & `shrike-2.0.0.dev7/shrike/pipeline/telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/pipeline/testing/components.py` & `shrike-2.0.0.dev7/shrike/pipeline/testing/components.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/pipeline/testing/importer.py` & `shrike-2.0.0.dev7/shrike/pipeline/testing/importer.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/pipeline/testing/module_run_tests.py` & `shrike-2.0.0.dev7/shrike/pipeline/testing/module_run_tests.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/pipeline/testing/pipeline_class_test.py` & `shrike-2.0.0.dev7/shrike/pipeline/testing/pipeline_class_test.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/pipeline/testing/pipeline_class_test_v2.py` & `shrike-2.0.0.dev7/shrike/pipeline/testing/pipeline_class_test_v2.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/pipeline/v1/aml_connect.py` & `shrike-2.0.0.dev7/shrike/pipeline/v1/aml_connect.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/pipeline/v1/module_helper.py` & `shrike-2.0.0.dev7/shrike/pipeline/v1/module_helper.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/pipeline/v1/pipeline_helper.py` & `shrike-2.0.0.dev7/shrike/pipeline/v1/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/pipeline/v2/aml_connect.py` & `shrike-2.0.0.dev7/shrike/pipeline/v2/aml_connect.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/pipeline/v2/module_helper.py` & `shrike-2.0.0.dev7/shrike/pipeline/v2/module_helper.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/pipeline/v2/pipeline_helper.py` & `shrike-2.0.0.dev7/shrike/pipeline/v2/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike/spark/spark_net.py` & `shrike-2.0.0.dev7/shrike/spark/spark_net.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike.egg-info/PKG-INFO` & `shrike-2.0.0.dev7/shrike.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shrike
-Version: 2.0.0.dev6
+Version: 2.0.0.dev7
 Summary: Python utilities for compliant Azure machine learning
 Home-page: https://github.com/ai-platform-ml-platform/shrike
 Author: AML Data Science
 Author-email: aml-ds@microsoft.com
 License: MIT
 Description: # Shrike: incubation for Azure ML
```

### Comparing `shrike-2.0.0.dev6/shrike.egg-info/SOURCES.txt` & `shrike-2.0.0.dev7/shrike.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev6/shrike.egg-info/requires.txt` & `shrike-2.0.0.dev7/shrike.egg-info/requires.txt`

 * *Files identical despite different names*

