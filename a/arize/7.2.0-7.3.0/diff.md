# Comparing `tmp/arize-7.2.0.tar.gz` & `tmp/arize-7.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arize-7.2.0.tar", last modified: Fri Jul 21 22:41:29 2023, max compression
+gzip compressed data, was "arize-7.3.0.tar", last modified: Tue Aug  1 21:10:06 2023, max compression
```

## Comparing `arize-7.2.0.tar` & `arize-7.3.0.tar`

### file list

```diff
@@ -1,78 +1,77 @@
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.251542 arize-7.2.0/
--rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-06-23 05:09:35.000000 arize-7.2.0/LICENSE.md
--rw-r--r--   0 kiko       (501) staff       (20)       65 2023-06-23 05:09:35.000000 arize-7.2.0/MANIFEST.in
--rw-r--r--   0 kiko       (501) staff       (20)    12555 2023-07-21 22:41:29.251891 arize-7.2.0/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-06-23 05:09:35.000000 arize-7.2.0/README.md
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.182958 arize-7.2.0/arize/
--rw-r--r--   0 kiko       (501) staff       (20)       22 2023-07-21 22:31:43.000000 arize-7.2.0/arize/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    32195 2023-07-21 22:31:43.000000 arize-7.2.0/arize/api.py
--rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-06-23 05:09:35.000000 arize-7.2.0/arize/bounded_executor.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.200987 arize-7.2.0/arize/examples/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.2.0/arize/examples/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-06-23 05:09:35.000000 arize-7.2.0/arize/examples/bulk_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-06-23 05:09:35.000000 arize-7.2.0/arize/examples/bulk_client_shap.py
--rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-06-23 05:09:35.000000 arize-7.2.0/arize/examples/client_shap_values.py
--rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-06-23 05:09:35.000000 arize-7.2.0/arize/examples/log_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-06-23 05:09:35.000000 arize-7.2.0/arize/examples/log_pandas_dataframe.py
--rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-06-23 05:09:35.000000 arize-7.2.0/arize/examples/preproduction_client.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.202793 arize-7.2.0/arize/exporter/
--rw-r--r--   0 kiko       (501) staff       (20)      146 2023-06-23 05:09:35.000000 arize-7.2.0/arize/exporter/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.206128 arize-7.2.0/arize/exporter/core/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.2.0/arize/exporter/core/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    10940 2023-06-30 17:46:28.000000 arize-7.2.0/arize/exporter/core/client.py
--rw-r--r--   0 kiko       (501) staff       (20)     1343 2023-06-30 17:46:28.000000 arize-7.2.0/arize/exporter/core/query.py
--rw-r--r--   0 kiko       (501) staff       (20)     3464 2023-06-30 17:46:28.000000 arize-7.2.0/arize/exporter/core/session.py
--rw-r--r--   0 kiko       (501) staff       (20)     2406 2023-07-18 18:29:39.000000 arize-7.2.0/arize/exporter/publicexporter_pb2.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.210171 arize-7.2.0/arize/exporter/utils/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.2.0/arize/exporter/utils/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1422 2023-06-30 17:46:28.000000 arize-7.2.0/arize/exporter/utils/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)      727 2023-06-30 17:46:28.000000 arize-7.2.0/arize/exporter/utils/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)     5793 2023-06-30 17:46:28.000000 arize-7.2.0/arize/exporter/utils/schema_parser.py
--rw-r--r--   0 kiko       (501) staff       (20)      778 2023-06-30 17:46:28.000000 arize-7.2.0/arize/exporter/utils/validation.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.211445 arize-7.2.0/arize/pandas/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.221576 arize-7.2.0/arize/pandas/embeddings/
--rw-r--r--   0 kiko       (501) staff       (20)      124 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/embeddings/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/embeddings/auto_generator.py
--rw-r--r--   0 kiko       (501) staff       (20)     6988 2023-06-30 17:46:28.000000 arize-7.2.0/arize/pandas/embeddings/base_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      213 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/embeddings/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)     2023 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/embeddings/cv_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      753 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/embeddings/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)      571 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/embeddings/models.py
--rw-r--r--   0 kiko       (501) staff       (20)     3675 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/embeddings/nlp_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)     5853 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/embeddings/tabular_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      412 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/embeddings/usecases.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.222708 arize-7.2.0/arize/pandas/generative/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/generative/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.226607 arize-7.2.0/arize/pandas/generative/llm_evaluation/
--rw-r--r--   0 kiko       (501) staff       (20)      160 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/generative/llm_evaluation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      183 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/generative/llm_evaluation/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)    12178 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/generative/llm_evaluation/hf_metrics.py
--rw-r--r--   0 kiko       (501) staff       (20)    24029 2023-07-21 22:31:43.000000 arize-7.2.0/arize/pandas/logger.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.229801 arize-7.2.0/arize/pandas/surrogate_explainer/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/surrogate_explainer/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     5090 2023-06-30 17:46:28.000000 arize-7.2.0/arize/pandas/surrogate_explainer/mimic.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.234976 arize-7.2.0/arize/pandas/validation/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/validation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    26601 2023-07-21 00:34:26.000000 arize-7.2.0/arize/pandas/validation/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)    70724 2023-07-21 22:31:43.000000 arize-7.2.0/arize/pandas/validation/validator.py
--rw-r--r--   0 kiko       (501) staff       (20)    50975 2023-07-18 18:29:39.000000 arize-7.2.0/arize/public_pb2.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.247833 arize-7.2.0/arize/utils/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.2.0/arize/utils/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      743 2023-07-21 22:31:43.000000 arize-7.2.0/arize/utils/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)     1163 2023-07-21 22:31:43.000000 arize-7.2.0/arize/utils/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-06-23 05:09:35.000000 arize-7.2.0/arize/utils/logging.py
--rw-r--r--   0 kiko       (501) staff       (20)     5725 2023-06-23 05:09:35.000000 arize-7.2.0/arize/utils/model_mapping.json
--rw-r--r--   0 kiko       (501) staff       (20)    24659 2023-06-30 17:46:28.000000 arize-7.2.0/arize/utils/types.py
--rw-r--r--   0 kiko       (501) staff       (20)     7620 2023-06-23 05:09:35.000000 arize-7.2.0/arize/utils/utils.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.188408 arize-7.2.0/arize.egg-info/
--rw-r--r--   0 kiko       (501) staff       (20)    12555 2023-07-21 22:41:29.000000 arize-7.2.0/arize.egg-info/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)     1901 2023-07-21 22:41:29.000000 arize-7.2.0/arize.egg-info/SOURCES.txt
--rw-r--r--   0 kiko       (501) staff       (20)        1 2023-07-21 22:41:29.000000 arize-7.2.0/arize.egg-info/dependency_links.txt
--rw-r--r--   0 kiko       (501) staff       (20)      429 2023-07-21 22:41:29.000000 arize-7.2.0/arize.egg-info/requires.txt
--rw-r--r--   0 kiko       (501) staff       (20)        6 2023-07-21 22:41:29.000000 arize-7.2.0/arize.egg-info/top_level.txt
--rw-r--r--   0 kiko       (501) staff       (20)      167 2023-06-23 05:09:35.000000 arize-7.2.0/pyproject.toml
--rw-r--r--   0 kiko       (501) staff       (20)     1517 2023-07-21 22:41:29.254223 arize-7.2.0/setup.cfg
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.250500 arize-7.2.0/tests/
--rw-r--r--   0 kiko       (501) staff       (20)    61734 2023-07-21 22:31:43.000000 arize-7.2.0/tests/test_api.py
--rw-r--r--   0 kiko       (501) staff       (20)      952 2023-06-23 05:09:35.000000 arize-7.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:10:06.242458 arize-7.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-08-01 21:09:42.000000 arize-7.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-01 21:09:42.000000 arize-7.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-08-01 21:10:06.242458 arize-7.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-08-01 21:09:42.000000 arize-7.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:10:06.230459 arize-7.3.0/arize/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 21:09:42.000000 arize-7.3.0/arize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32195 2023-08-01 21:09:42.000000 arize-7.3.0/arize/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-01 21:09:42.000000 arize-7.3.0/arize/bounded_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:10:06.234459 arize-7.3.0/arize/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 21:09:42.000000 arize-7.3.0/arize/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-01 21:09:42.000000 arize-7.3.0/arize/examples/bulk_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-08-01 21:09:42.000000 arize-7.3.0/arize/examples/bulk_client_shap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-08-01 21:09:42.000000 arize-7.3.0/arize/examples/client_shap_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-08-01 21:09:42.000000 arize-7.3.0/arize/examples/log_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-08-01 21:09:42.000000 arize-7.3.0/arize/examples/log_pandas_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-08-01 21:09:42.000000 arize-7.3.0/arize/examples/preproduction_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:10:06.234459 arize-7.3.0/arize/exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-01 21:09:42.000000 arize-7.3.0/arize/exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:10:06.234459 arize-7.3.0/arize/exporter/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 21:09:42.000000 arize-7.3.0/arize/exporter/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-08-01 21:09:42.000000 arize-7.3.0/arize/exporter/core/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-08-01 21:09:42.000000 arize-7.3.0/arize/exporter/core/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-08-01 21:09:42.000000 arize-7.3.0/arize/exporter/core/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-08-01 21:09:42.000000 arize-7.3.0/arize/exporter/publicexporter_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:10:06.234459 arize-7.3.0/arize/exporter/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 21:09:42.000000 arize-7.3.0/arize/exporter/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-01 21:09:42.000000 arize-7.3.0/arize/exporter/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-01 21:09:42.000000 arize-7.3.0/arize/exporter/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-08-01 21:09:42.000000 arize-7.3.0/arize/exporter/utils/schema_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-01 21:09:42.000000 arize-7.3.0/arize/exporter/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:10:06.234459 arize-7.3.0/arize/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 21:09:42.000000 arize-7.3.0/arize/pandas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:10:06.238458 arize-7.3.0/arize/pandas/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-01 21:09:42.000000 arize-7.3.0/arize/pandas/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-08-01 21:09:42.000000 arize-7.3.0/arize/pandas/embeddings/auto_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-08-01 21:09:42.000000 arize-7.3.0/arize/pandas/embeddings/base_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-01 21:09:42.000000 arize-7.3.0/arize/pandas/embeddings/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-01 21:09:42.000000 arize-7.3.0/arize/pandas/embeddings/cv_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-01 21:09:42.000000 arize-7.3.0/arize/pandas/embeddings/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-08-01 21:09:42.000000 arize-7.3.0/arize/pandas/embeddings/nlp_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-08-01 21:09:42.000000 arize-7.3.0/arize/pandas/embeddings/tabular_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-01 21:09:42.000000 arize-7.3.0/arize/pandas/embeddings/usecases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:10:06.238458 arize-7.3.0/arize/pandas/generative/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 21:09:42.000000 arize-7.3.0/arize/pandas/generative/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:10:06.238458 arize-7.3.0/arize/pandas/generative/llm_evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-01 21:09:42.000000 arize-7.3.0/arize/pandas/generative/llm_evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-01 21:09:42.000000 arize-7.3.0/arize/pandas/generative/llm_evaluation/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12178 2023-08-01 21:09:42.000000 arize-7.3.0/arize/pandas/generative/llm_evaluation/hf_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24029 2023-08-01 21:09:42.000000 arize-7.3.0/arize/pandas/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:10:06.238458 arize-7.3.0/arize/pandas/surrogate_explainer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 21:09:42.000000 arize-7.3.0/arize/pandas/surrogate_explainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-08-01 21:09:42.000000 arize-7.3.0/arize/pandas/surrogate_explainer/mimic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:10:06.238458 arize-7.3.0/arize/pandas/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 21:09:42.000000 arize-7.3.0/arize/pandas/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26601 2023-08-01 21:09:42.000000 arize-7.3.0/arize/pandas/validation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70724 2023-08-01 21:09:42.000000 arize-7.3.0/arize/pandas/validation/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50975 2023-08-01 21:09:42.000000 arize-7.3.0/arize/public_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:10:06.242458 arize-7.3.0/arize/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 21:09:42.000000 arize-7.3.0/arize/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-01 21:09:42.000000 arize-7.3.0/arize/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-01 21:09:42.000000 arize-7.3.0/arize/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-08-01 21:09:42.000000 arize-7.3.0/arize/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-08-01 21:09:42.000000 arize-7.3.0/arize/utils/model_mapping.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24659 2023-08-01 21:09:42.000000 arize-7.3.0/arize/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-08-01 21:09:42.000000 arize-7.3.0/arize/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:10:06.230459 arize-7.3.0/arize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-08-01 21:10:06.000000 arize-7.3.0/arize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-01 21:10:06.000000 arize-7.3.0/arize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 21:10:06.000000 arize-7.3.0/arize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-01 21:10:06.000000 arize-7.3.0/arize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 21:10:06.000000 arize-7.3.0/arize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-01 21:09:42.000000 arize-7.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-01 21:10:06.242458 arize-7.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:10:06.242458 arize-7.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    61734 2023-08-01 21:09:42.000000 arize-7.3.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-01 21:09:42.000000 arize-7.3.0/tests/test_utils.py
```

### Comparing `arize-7.2.0/LICENSE.md` & `arize-7.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/PKG-INFO` & `arize-7.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.2.0
+Version: 7.3.0
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.2.0/README.md` & `arize-7.3.0/README.md`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/api.py` & `arize-7.3.0/arize/api.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/bounded_executor.py` & `arize-7.3.0/arize/bounded_executor.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/examples/bulk_client.py` & `arize-7.3.0/arize/examples/bulk_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/examples/bulk_client_shap.py` & `arize-7.3.0/arize/examples/bulk_client_shap.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/examples/client_shap_values.py` & `arize-7.3.0/arize/examples/client_shap_values.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/examples/log_client.py` & `arize-7.3.0/arize/examples/log_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/examples/log_pandas_dataframe.py` & `arize-7.3.0/arize/examples/log_pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/examples/preproduction_client.py` & `arize-7.3.0/arize/examples/preproduction_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/exporter/core/client.py` & `arize-7.3.0/arize/exporter/core/client.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/exporter/core/query.py` & `arize-7.3.0/arize/exporter/core/query.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/exporter/core/session.py` & `arize-7.3.0/arize/exporter/core/session.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/exporter/publicexporter_pb2.py` & `arize-7.3.0/arize/exporter/publicexporter_pb2.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/exporter/utils/constants.py` & `arize-7.3.0/arize/exporter/utils/constants.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/exporter/utils/errors.py` & `arize-7.3.0/arize/exporter/utils/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/exporter/utils/schema_parser.py` & `arize-7.3.0/arize/exporter/utils/schema_parser.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/exporter/utils/validation.py` & `arize-7.3.0/arize/exporter/utils/validation.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/pandas/embeddings/auto_generator.py` & `arize-7.3.0/arize/pandas/embeddings/auto_generator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 import pandas as pd
 
 from . import constants
 from .base_generators import BaseEmbeddingGenerator
-from .cv_generators import EmbeddingGeneratorForCVImageClassification
-from .models import CV_PRETRAINED_MODELS, NLP_PRETRAINED_MODELS
+from .constants import (
+    CV_PRETRAINED_MODELS,
+    DEFAULT_CV_IMAGE_CLASSIFICATION_MODEL,
+    DEFAULT_CV_OBJECT_DETECTION_MODEL,
+    DEFAULT_NLP_SEQUENCE_CLASSIFICATION_MODEL,
+    DEFAULT_NLP_SUMMARIZATION_MODEL,
+    DEFAULT_TABULAR_MODEL,
+    NLP_PRETRAINED_MODELS,
+)
+from .cv_generators import (
+    EmbeddingGeneratorForCVImageClassification,
+    EmbeddingGeneratorForCVObjectDetection,
+)
 from .nlp_generators import (
     EmbeddingGeneratorForNLPSequenceClassification,
     EmbeddingGeneratorForNLPSummarization,
 )
 from .tabular_generators import EmbeddingGeneratorForTabularFeatures
 from .usecases import UseCases
 
@@ -23,20 +34,46 @@
     def from_use_case(use_case: str, **kwargs: str) -> BaseEmbeddingGenerator:
         if use_case == UseCases.NLP.SEQUENCE_CLASSIFICATION:
             return EmbeddingGeneratorForNLPSequenceClassification(**kwargs)
         elif use_case == UseCases.NLP.SUMMARIZATION:
             return EmbeddingGeneratorForNLPSummarization(**kwargs)
         elif use_case == UseCases.CV.IMAGE_CLASSIFICATION:
             return EmbeddingGeneratorForCVImageClassification(**kwargs)
+        elif use_case == UseCases.CV.OBJECT_DETECTION:
+            return EmbeddingGeneratorForCVObjectDetection(**kwargs)
         elif use_case == UseCases.STRUCTURED.TABULAR_EMBEDDINGS:
             return EmbeddingGeneratorForTabularFeatures(**kwargs)
         else:
             raise ValueError(f"Invalid use case {use_case}")
 
     @classmethod
+    def list_default_models(cls) -> pd.DataFrame:
+        df = pd.DataFrame(
+            {
+                "Area": ["NLP", "NLP", "CV", "CV", "STRUCTURED"],
+                "Usecase": [
+                    UseCases.NLP.SEQUENCE_CLASSIFICATION.name,
+                    UseCases.NLP.SUMMARIZATION.name,
+                    UseCases.CV.IMAGE_CLASSIFICATION.name,
+                    UseCases.CV.OBJECT_DETECTION.name,
+                    UseCases.STRUCTURED.TABULAR_EMBEDDINGS.name,
+                ],
+                "Model Name": [
+                    DEFAULT_NLP_SEQUENCE_CLASSIFICATION_MODEL,
+                    DEFAULT_NLP_SUMMARIZATION_MODEL,
+                    DEFAULT_CV_IMAGE_CLASSIFICATION_MODEL,
+                    DEFAULT_CV_OBJECT_DETECTION_MODEL,
+                    DEFAULT_TABULAR_MODEL,
+                ],
+            }
+        )
+        df.sort_values(by=[col for col in df.columns], ascending=True, inplace=True)
+        return df.reset_index(drop=True)
+
+    @classmethod
     def list_pretrained_models(cls) -> pd.DataFrame:
         data = {
             "Task": ["NLP" for _ in NLP_PRETRAINED_MODELS] + ["CV" for _ in CV_PRETRAINED_MODELS],
             "Architecture": [
                 cls.__parse_model_arch(model)
                 for model in NLP_PRETRAINED_MODELS + CV_PRETRAINED_MODELS
             ],
```

### Comparing `arize-7.2.0/arize/pandas/embeddings/base_generators.py` & `arize-7.3.0/arize/pandas/embeddings/base_generators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import os
 from abc import ABC, abstractmethod
 from enum import Enum
-from typing import Dict, List, Union
+from functools import partial
+from typing import Dict, List, Union, cast
 
 import arize.pandas.embeddings.errors as err
 import pandas as pd
 from arize.utils.logging import logger
 
 from .constants import IMPORT_ERROR_MESSAGE
-from .models import CV_PRETRAINED_MODELS, NLP_PRETRAINED_MODELS
 
 try:
     import torch
+    from datasets import Dataset
     from PIL import Image
     from transformers import (  # type: ignore
-        AutoFeatureExtractor,
+        AutoImageProcessor,
         AutoModel,
         AutoTokenizer,
         BatchEncoding,
     )
     from transformers.utils import logging as transformer_logging
 except ImportError:
     raise ImportError(IMPORT_ERROR_MESSAGE)
@@ -36,15 +37,20 @@
             logger.warning(
                 "No available GPU has been detected. The use of GPU acceleration is "
                 "strongly recommended. You can check for GPU availability by running "
                 "`torch.cuda.is_available()`"
             )
         self.__batch_size = batch_size
         logger.info(f"Downloading pre-trained model '{self.model_name}'")
-        self.__model = AutoModel.from_pretrained(self.model_name, **kwargs).to(self.device)
+        try:
+            self.__model = AutoModel.from_pretrained(self.model_name, **kwargs).to(self.device)
+        except OSError:
+            raise err.HuggingFaceRepositoryNotFound(model_name)
+        except Exception as e:
+            raise e
 
     @property
     def use_case(self) -> str:
         return self.__use_case
 
     @property
     def model_name(self) -> str:
@@ -87,15 +93,15 @@
         # (batch_size, seq_length/or/num_tokens, hidden_size)
         if method == "cls_token":  # Select CLS token vector
             embeddings = outputs.last_hidden_state[:, 0, :]
         elif method == "avg_token":  # Select avg token vector
             embeddings = torch.mean(outputs.last_hidden_state, 1)
         else:
             raise ValueError(f"Invalid method = {method}")
-        return {"embedding_vector": embeddings.cpu().numpy()}
+        return {"embedding_vector": embeddings.cpu().numpy().astype(float)}
 
     @staticmethod
     def check_invalid_index(field: Union[pd.Series, pd.DataFrame]) -> None:
         if (field.index != field.reset_index(drop=True).index).any():
             if isinstance(field, pd.DataFrame):
                 raise err.InvalidIndexError("DataFrame")
             else:
@@ -116,23 +122,20 @@
             f"  tokenizer={self.tokenizer.__class__},\n"
             f"  model={self.model.__class__},\n"
             f"  batch_size={self.batch_size},\n"
             f")"
         )
 
     def __init__(self, use_case: Enum, model_name: str, tokenizer_max_length: int = 512, **kwargs):
-        if model_name not in NLP_PRETRAINED_MODELS:
-            raise ValueError(
-                "model_name not supported. Check supported models with "
-                "`AutoEmbeddingGenerator.list_pretrained_models()`"
-            )
         super(NLPEmbeddingGenerator, self).__init__(
             use_case=use_case, model_name=model_name, **kwargs
         )
         self.__tokenizer_max_length = tokenizer_max_length
+        # We don't check for the tokenizer's existence since it is coupled with the corresponding model
+        # We check the model's existence in `BaseEmbeddingGenerator`
         logger.info(f"Downloading tokenizer for '{self.model_name}'")
         self.__tokenizer = AutoTokenizer.from_pretrained(
             self.model_name, model_max_length=self.tokenizer_max_length
         )
 
     @property
     def tokenizer(self):
@@ -154,40 +157,68 @@
 
 class CVEmbeddingGenerator(BaseEmbeddingGenerator):
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}(\n"
             f"  use_case={self.use_case},\n"
             f"  model_name='{self.model_name}',\n"
-            f"  feature_extractor={self.feature_extractor.__class__},\n"
+            f"  image_processor={self.image_processor.__class__},\n"
             f"  model={self.model.__class__},\n"
             f"  batch_size={self.batch_size},\n"
             f")"
         )
 
     def __init__(self, use_case: Enum, model_name: str, **kwargs):
-        if model_name not in CV_PRETRAINED_MODELS:
-            raise ValueError(
-                "model_name not supported. Check supported models with "
-                "`AutoEmbeddingGenerator.list_pretrained_models()`"
-            )
         super(CVEmbeddingGenerator, self).__init__(
             use_case=use_case, model_name=model_name, **kwargs
         )
-        logger.info("Downloading feature extractor")
-        self.__feature_extractor = AutoFeatureExtractor.from_pretrained(self.model_name)
+        logger.info("Downloading image processor")
+        # We don't check for the image processor's existence since it is coupled with the corresponding model
+        # We check the model's existence in `BaseEmbeddingGenerator`
+        self.__image_processor = AutoImageProcessor.from_pretrained(self.model_name)
 
     @property
-    def feature_extractor(self):
-        return self.__feature_extractor
+    def image_processor(self):
+        return self.__image_processor
 
     @staticmethod
     def open_image(image_path: str) -> Image.Image:
         if not os.path.exists(image_path):
             raise ValueError(f"Cannot find image {image_path}")
         return Image.open(image_path).convert("RGB")
 
-    def extract_image_features(self, batch: Dict[str, List[str]], local_image_feat_name: str):
-        return self.feature_extractor(
+    def preprocess_image(self, batch: Dict[str, List[str]], local_image_feat_name: str):
+        return self.image_processor(
             [self.open_image(image_path) for image_path in batch[local_image_feat_name]],
             return_tensors="pt",
         ).to(self.device)
+
+    def generate_embeddings(self, local_image_path_col: pd.Series) -> pd.Series:
+        """
+        Obtain embedding vectors from your image data using pre-trained image models.
+
+        :param local_image_path_col: a pandas Series containing the local path to the images to
+        be used to generate the embedding vectors.
+        :return: a pandas Series containing the embedding vectors.
+        """
+        if not isinstance(local_image_path_col, pd.Series):
+            raise TypeError("local_image_path_col_name must be pandas Series object")
+        self.check_invalid_index(field=local_image_path_col)
+
+        # Validate that there are no null image paths
+        if local_image_path_col.isnull().any():
+            raise ValueError("There can't be any null values in the local_image_path_col series")
+
+        ds = Dataset.from_dict({"local_path": local_image_path_col})
+        ds.set_transform(
+            partial(
+                self.preprocess_image,
+                local_image_feat_name="local_path",
+            )
+        )
+        logger.info("Generating embedding vectors")
+        ds = ds.map(
+            lambda batch: self._get_embedding_vector(batch, "avg_token"),
+            batched=True,
+            batch_size=self.batch_size,
+        )
+        return cast(pd.DataFrame, ds.to_pandas())["embedding_vector"]
```

### Comparing `arize-7.2.0/arize/pandas/embeddings/nlp_generators.py` & `arize-7.3.0/arize/pandas/embeddings/nlp_generators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from functools import partial
 from typing import Optional, cast
 
 import pandas as pd
 from arize.utils.logging import logger
 
 from .base_generators import NLPEmbeddingGenerator
-from .constants import IMPORT_ERROR_MESSAGE
+from .constants import (
+    DEFAULT_NLP_SEQUENCE_CLASSIFICATION_MODEL,
+    DEFAULT_NLP_SUMMARIZATION_MODEL,
+    IMPORT_ERROR_MESSAGE,
+)
 from .usecases import UseCases
 
 try:
     from datasets import Dataset
 except ImportError:
     raise ImportError(IMPORT_ERROR_MESSAGE)
 
 
 class EmbeddingGeneratorForNLPSequenceClassification(NLPEmbeddingGenerator):
-    def __init__(self, model_name: str = "distilbert-base-uncased", **kwargs):
+    def __init__(self, model_name: str = DEFAULT_NLP_SEQUENCE_CLASSIFICATION_MODEL, **kwargs):
         super(EmbeddingGeneratorForNLPSequenceClassification, self).__init__(
             use_case=UseCases.NLP.SEQUENCE_CLASSIFICATION,
             model_name=model_name,
             **kwargs,
         )
 
     def generate_embeddings(
@@ -59,15 +63,15 @@
             batched=True,
             batch_size=self.batch_size,
         )
         return cast(pd.DataFrame, ds.to_pandas())["embedding_vector"]
 
 
 class EmbeddingGeneratorForNLPSummarization(NLPEmbeddingGenerator):
-    def __init__(self, model_name: str = "distilbert-base-uncased", **kwargs):
+    def __init__(self, model_name: str = DEFAULT_NLP_SUMMARIZATION_MODEL, **kwargs):
         super(EmbeddingGeneratorForNLPSummarization, self).__init__(
             use_case=UseCases.NLP.SUMMARIZATION,
             model_name=model_name,
             **kwargs,
         )
 
     def generate_embeddings(
```

### Comparing `arize-7.2.0/arize/pandas/embeddings/tabular_generators.py` & `arize-7.3.0/arize/pandas/embeddings/tabular_generators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,65 +1,54 @@
-from dataclasses import dataclass
-from enum import Enum, auto, unique
 from functools import partial
 from typing import Dict, List, Tuple, Union, cast
 
 import pandas as pd
 from arize.utils.logging import logger
 from arize.utils.types import is_list_of
 
 from .base_generators import NLPEmbeddingGenerator
-from .constants import IMPORT_ERROR_MESSAGE
+from .constants import DEFAULT_TABULAR_MODEL, IMPORT_ERROR_MESSAGE
+from .usecases import UseCases
 
 try:
     from datasets import Dataset
 except ImportError:
     raise ImportError(IMPORT_ERROR_MESSAGE)
 
 TABULAR_PRETRAINED_MODELS = [
     "bert-base-uncased",
     "distilbert-base-uncased",
     "xlm-roberta-base",
 ]
 
 
-@unique
-class StructuredUseCases(Enum):
-    TABULAR_FEATURES = auto()
-
-
-@dataclass
-class UseCases:
-    STRUCTURED = StructuredUseCases
-
-
 class EmbeddingGeneratorForTabularFeatures(NLPEmbeddingGenerator):
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}(\n"
             f"  use_case={self.use_case},\n"
             f"  model_name={self.model_name},\n"
             f"  tokenizer_max_length={self.tokenizer_max_length},\n"
             f"  tokenizer={self.tokenizer.__class__},\n"
             f"  model={self.model.__class__},\n"
             f")"
         )
 
     def __init__(
         self,
-        model_name: str = "distilbert-base-uncased",
+        model_name: str = DEFAULT_TABULAR_MODEL,
         **kwargs,
     ):
         if model_name not in TABULAR_PRETRAINED_MODELS:
             raise ValueError(
                 "model_name not supported. Check supported models with "
                 "`EmbeddingGeneratorForTabularFeatures.list_pretrained_models()`"
             )
         super(EmbeddingGeneratorForTabularFeatures, self).__init__(
-            use_case=UseCases.STRUCTURED.TABULAR_FEATURES,
+            use_case=UseCases.STRUCTURED.TABULAR_EMBEDDINGS,
             model_name=model_name,
             **kwargs,
         )
 
     def generate_embeddings(
         self,
         df: pd.DataFrame,
```

### Comparing `arize-7.2.0/arize/pandas/generative/llm_evaluation/hf_metrics.py` & `arize-7.3.0/arize/pandas/generative/llm_evaluation/hf_metrics.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/pandas/logger.py` & `arize-7.3.0/arize/pandas/logger.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/pandas/surrogate_explainer/mimic.py` & `arize-7.3.0/arize/pandas/surrogate_explainer/mimic.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/pandas/validation/errors.py` & `arize-7.3.0/arize/pandas/validation/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/pandas/validation/validator.py` & `arize-7.3.0/arize/pandas/validation/validator.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/public_pb2.py` & `arize-7.3.0/arize/public_pb2.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/utils/constants.py` & `arize-7.3.0/arize/utils/constants.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/utils/errors.py` & `arize-7.3.0/arize/utils/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/utils/logging.py` & `arize-7.3.0/arize/utils/logging.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/utils/model_mapping.json` & `arize-7.3.0/arize/utils/model_mapping.json`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/utils/types.py` & `arize-7.3.0/arize/utils/types.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize/utils/utils.py` & `arize-7.3.0/arize/utils/utils.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/arize.egg-info/PKG-INFO` & `arize-7.3.0/arize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.2.0
+Version: 7.3.0
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.2.0/arize.egg-info/SOURCES.txt` & `arize-7.3.0/arize.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 arize/pandas/logger.py
 arize/pandas/embeddings/__init__.py
 arize/pandas/embeddings/auto_generator.py
 arize/pandas/embeddings/base_generators.py
 arize/pandas/embeddings/constants.py
 arize/pandas/embeddings/cv_generators.py
 arize/pandas/embeddings/errors.py
-arize/pandas/embeddings/models.py
 arize/pandas/embeddings/nlp_generators.py
 arize/pandas/embeddings/tabular_generators.py
 arize/pandas/embeddings/usecases.py
 arize/pandas/generative/__init__.py
 arize/pandas/generative/llm_evaluation/__init__.py
 arize/pandas/generative/llm_evaluation/constants.py
 arize/pandas/generative/llm_evaluation/hf_metrics.py
```

### Comparing `arize-7.2.0/setup.cfg` & `arize-7.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/tests/test_api.py` & `arize-7.3.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `arize-7.2.0/tests/test_utils.py` & `arize-7.3.0/tests/test_utils.py`

 * *Files identical despite different names*

