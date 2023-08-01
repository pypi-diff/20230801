# Comparing `tmp/kedro-datasets-1.5.0.tar.gz` & `tmp/kedro-datasets-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-datasets-1.5.0.tar", last modified: Mon Jul 31 15:37:02 2023, max compression
+gzip compressed data, was "kedro-datasets-1.5.1.tar", last modified: Tue Aug  1 13:44:20 2023, max compression
```

## Comparing `kedro-datasets-1.5.0.tar` & `kedro-datasets-1.5.1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.851839 kedro-datasets-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-31 15:37:02.851839 kedro-datasets-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.835839 kedro-datasets-1.5.0/kedro_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.835839 kedro-datasets-1.5.0/kedro_datasets/api/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/api/api_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.835839 kedro-datasets-1.5.0/kedro_datasets/biosequence/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/biosequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/biosequence/biosequence_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.835839 kedro-datasets-1.5.0/kedro_datasets/dask/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/dask/parquet_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.835839 kedro-datasets-1.5.0/kedro_datasets/databricks/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/databricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/databricks/managed_table_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.839839 kedro-datasets-1.5.0/kedro_datasets/email/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/email/message_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.839839 kedro-datasets-1.5.0/kedro_datasets/geopandas/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/geopandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/geopandas/geojson_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.839839 kedro-datasets-1.5.0/kedro_datasets/holoviews/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/holoviews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/holoviews/holoviews_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.839839 kedro-datasets-1.5.0/kedro_datasets/json/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/json/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.839839 kedro-datasets-1.5.0/kedro_datasets/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/matplotlib/matplotlib_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.839839 kedro-datasets-1.5.0/kedro_datasets/networkx/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/networkx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/networkx/gml_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/networkx/graphml_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/networkx/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.843839 kedro-datasets-1.5.0/kedro_datasets/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/deltatable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/feather_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/gbq_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/generic_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/hdf_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/parquet_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21158 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/sql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/xml_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.843839 kedro-datasets-1.5.0/kedro_datasets/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pickle/pickle_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.843839 kedro-datasets-1.5.0/kedro_datasets/pillow/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pillow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pillow/image_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.843839 kedro-datasets-1.5.0/kedro_datasets/plotly/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/plotly/json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/plotly/plotly_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.843839 kedro-datasets-1.5.0/kedro_datasets/polars/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/polars/csv_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.843839 kedro-datasets-1.5.0/kedro_datasets/redis/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/redis/redis_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.847839 kedro-datasets-1.5.0/kedro_datasets/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/snowflake/snowpark_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.847839 kedro-datasets-1.5.0/kedro_datasets/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/spark/deltatable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    16216 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/spark/spark_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/spark/spark_hive_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/spark/spark_jdbc_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/spark/spark_streaming_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.847839 kedro-datasets-1.5.0/kedro_datasets/svmlight/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/svmlight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/svmlight/svmlight_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.847839 kedro-datasets-1.5.0/kedro_datasets/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/tensorflow/tensorflow_model_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.847839 kedro-datasets-1.5.0/kedro_datasets/text/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/text/text_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.847839 kedro-datasets-1.5.0/kedro_datasets/tracking/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/tracking/json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/tracking/metrics_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.847839 kedro-datasets-1.5.0/kedro_datasets/video/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12475 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/video/video_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.847839 kedro-datasets-1.5.0/kedro_datasets/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/yaml/yaml_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.835839 kedro-datasets-1.5.0/kedro_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-31 15:37:02.000000 kedro-datasets-1.5.0/kedro_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-31 15:37:02.000000 kedro-datasets-1.5.0/kedro_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 15:37:02.000000 kedro-datasets-1.5.0/kedro_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-07-31 15:37:02.000000 kedro-datasets-1.5.0/kedro_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 15:37:02.000000 kedro-datasets-1.5.0/kedro_datasets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 15:37:02.851839 kedro-datasets-1.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.851839 kedro-datasets-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/tests/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.894790 kedro-datasets-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-08-01 13:44:20.894790 kedro-datasets-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.882789 kedro-datasets-1.5.1/kedro_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.882789 kedro-datasets-1.5.1/kedro_datasets/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/api/api_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.886789 kedro-datasets-1.5.1/kedro_datasets/biosequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/biosequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/biosequence/biosequence_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.886789 kedro-datasets-1.5.1/kedro_datasets/dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/dask/parquet_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.886789 kedro-datasets-1.5.1/kedro_datasets/databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/databricks/managed_table_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.886789 kedro-datasets-1.5.1/kedro_datasets/email/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/email/message_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.886789 kedro-datasets-1.5.1/kedro_datasets/geopandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/geopandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/geopandas/geojson_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.886789 kedro-datasets-1.5.1/kedro_datasets/holoviews/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/holoviews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/holoviews/holoviews_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.886789 kedro-datasets-1.5.1/kedro_datasets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/json/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.886789 kedro-datasets-1.5.1/kedro_datasets/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/matplotlib/matplotlib_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.886789 kedro-datasets-1.5.1/kedro_datasets/networkx/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/networkx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/networkx/gml_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/networkx/graphml_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/networkx/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.890789 kedro-datasets-1.5.1/kedro_datasets/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/pandas/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/pandas/deltatable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/pandas/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/pandas/feather_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/pandas/gbq_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/pandas/generic_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/pandas/hdf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/pandas/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/pandas/parquet_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21158 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/pandas/sql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/pandas/xml_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.890789 kedro-datasets-1.5.1/kedro_datasets/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/pickle/pickle_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.890789 kedro-datasets-1.5.1/kedro_datasets/pillow/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/pillow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/pillow/image_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.890789 kedro-datasets-1.5.1/kedro_datasets/plotly/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/plotly/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/plotly/plotly_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.890789 kedro-datasets-1.5.1/kedro_datasets/polars/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/polars/csv_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.890789 kedro-datasets-1.5.1/kedro_datasets/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/redis/redis_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.890789 kedro-datasets-1.5.1/kedro_datasets/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/snowflake/snowpark_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.890789 kedro-datasets-1.5.1/kedro_datasets/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/spark/deltatable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16216 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/spark/spark_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/spark/spark_hive_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/spark/spark_jdbc_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/spark/spark_streaming_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.890789 kedro-datasets-1.5.1/kedro_datasets/svmlight/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/svmlight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/svmlight/svmlight_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.890789 kedro-datasets-1.5.1/kedro_datasets/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/tensorflow/tensorflow_model_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.894790 kedro-datasets-1.5.1/kedro_datasets/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/text/text_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.894790 kedro-datasets-1.5.1/kedro_datasets/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/tracking/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/tracking/metrics_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.894790 kedro-datasets-1.5.1/kedro_datasets/video/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12475 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/video/video_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.894790 kedro-datasets-1.5.1/kedro_datasets/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/kedro_datasets/yaml/yaml_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.882789 kedro-datasets-1.5.1/kedro_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-08-01 13:44:20.000000 kedro-datasets-1.5.1/kedro_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-08-01 13:44:20.000000 kedro-datasets-1.5.1/kedro_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:44:20.000000 kedro-datasets-1.5.1/kedro_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-08-01 13:44:20.000000 kedro-datasets-1.5.1/kedro_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 13:44:20.000000 kedro-datasets-1.5.1/kedro_datasets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 13:44:20.894790 kedro-datasets-1.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:20.894790 kedro-datasets-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-08-01 13:44:09.000000 kedro-datasets-1.5.1/tests/test_io.py
```

### Comparing `kedro-datasets-1.5.0/PKG-INFO` & `kedro-datasets-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-datasets
-Version: 1.5.0
+Version: 1.5.1
 Summary: Kedro-Datasets is where you can find all of Kedro's data connectors.
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-datasets
 Project-URL: Documentation, https://docs.kedro.org
 Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
 Requires-Python: <3.11,>=3.7
```

### Comparing `kedro-datasets-1.5.0/README.md` & `kedro-datasets-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/_io.py` & `kedro-datasets-1.5.1/kedro_datasets/_io.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/api/api_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/api/api_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/biosequence/biosequence_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/biosequence/biosequence_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/dask/parquet_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/dask/parquet_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/databricks/managed_table_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/databricks/managed_table_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/email/message_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/email/message_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/geopandas/geojson_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/geopandas/geojson_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/holoviews/holoviews_writer.py` & `kedro-datasets-1.5.1/kedro_datasets/holoviews/holoviews_writer.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/json/json_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/json/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/matplotlib/matplotlib_writer.py` & `kedro-datasets-1.5.1/kedro_datasets/matplotlib/matplotlib_writer.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/networkx/__init__.py` & `kedro-datasets-1.5.1/kedro_datasets/networkx/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/networkx/gml_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/networkx/gml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/networkx/graphml_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/networkx/graphml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/networkx/json_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/networkx/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/pandas/__init__.py` & `kedro-datasets-1.5.1/kedro_datasets/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/pandas/csv_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/pandas/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/pandas/deltatable_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/pandas/deltatable_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,17 @@
     S3, GCS), Databricks unity catalog and AWS Glue catalog respectively. It handles
     load and save using a pandas dataframe. When saving data, you can specify one of two
     modes: overwrite(default), append. If you wish to alter the schema as a part of
     overwrite, pass overwrite_schema=True. You can overwrite a specific partition by using
     mode=overwrite together with partition_filters. This will remove all files within the
     matching partition and insert your data as new files.
 
-    Example usage for the `YAML API`_:
+    Example usage for the
+    `YAML API <https://kedro.readthedocs.io/en/stable/data/\
+    data_catalog.html#use-the-data-catalog-with-the-yaml-api>`_:
 
     .. code-block:: yaml
 
         boats_filesystem:
           type: pandas.DeltaTableDataSet
           filepath: data/01_raw/boats
           credentials: dev_creds
@@ -49,15 +51,17 @@
           catalog_type: AWS
           catalog_name: main
           database: db_schema
           table: db_table
           save_args:
             mode: overwrite
 
-    Example usage for the `Python API`_:
+    Example usage for the
+    `Python API <https://kedro.readthedocs.io/en/stable/data/\
+    data_catalog.html#use-the-data-catalog-with-the-code-api>`_:
     ::
 
         >>> from kedro_datasets.pandas import DeltaTableDataSet
         >>> import pandas as pd
         >>>
         >>> data = pd.DataFrame({'col1': [1, 2], 'col2': [4, 5], 'col3': [5, 6]})
         >>> data_set = DeltaTableDataSet(filepath="test")
@@ -90,46 +94,42 @@
         credentials: Optional[Dict[str, Any]] = None,
         fs_args: Optional[Dict[str, Any]] = None,
     ) -> None:
         """Creates a new instance of ``DeltaTableDataSet``
 
         Args:
             filepath (str): Filepath to a delta lake file with the following accepted protocol:
-                ``S3``:
-                    `s3://<bucket>/<path>`
-                    `s3a://<bucket>/<path>`
-                ``Azure``:
-                    `az://<container>/<path>`
-                    `adl://<container>/<path>`
-                    `abfs://<container>/<path>`
-                ``GCS``:
-                    `gs://<bucket>/<path>`
+                ``S3``: `s3://<bucket>/<path>`, `s3a://<bucket>/<path>`
+                ``Azure``: `az://<container>/<path>`, `adl://<container>/<path>`,
+                `abfs://<container>/<path>`
+                ``GCS``: `gs://<bucket>/<path>`
                 If any of the prefix above is not provided, `file` protocol (local filesystem)
                 will be used.
-            catalog_type (DataCatalog, optional): `AWS` or `UNITY` if filepath is not provided.
+            catalog_type (DataCatalog, Optional): `AWS` or `UNITY` if filepath is not provided.
                 Defaults to None.
-            catalog_name (str, optional): the name of catalog in AWS Glue or Databricks Unity.
+            catalog_name (str, Optional): the name of catalog in AWS Glue or Databricks Unity.
                 Defaults to None.
-            database (str, optional): the name of the database (also referred to as schema).
+            database (str, Optional): the name of the database (also referred to as schema).
                 Defaults to None.
-            table (str, optional): the name of the table.
-            load_args (Dict[str, Any], optional): Additional options for loading file(s)
+            table (str, Optional): the name of the table.
+            load_args (Dict[str, Any], Optional): Additional options for loading file(s)
                 into DeltaTableDataSet. `load_args` accepts `version` to load the appropriate
-                 version when loading from a filesystem.
-            save_args (Dict[str, Any], optional): Additional saving options for saving into
+                version when loading from a filesystem.
+            save_args (Dict[str, Any], Optional): Additional saving options for saving into
                 Delta lake. Here you can find all available arguments:
                 https://delta-io.github.io/delta-rs/python/api_reference.html#writing-deltatables
-            credentials (Dict[str, Any], optional): Credentials required to get access to
+            credentials (Dict[str, Any], Optional): Credentials required to get access to
                 the underlying filesystem. E.g. for ``GCSFileSystem`` it should look like
                 `{"token": None}`.
-            fs_args (Dict[str, Any], optional): Extra arguments to pass into underlying
+            fs_args (Dict[str, Any], Optional): Extra arguments to pass into underlying
                 filesystem class constructor.
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``).
         Raises:
             DataSetError: Invalid configuration supplied (through DeltaTableDataSet validation)
+
         """
         self._filepath = filepath
         self._catalog_type = catalog_type
         self._catalog_name = catalog_name
         self._database = database
         self._table = table
         self._fs_args = deepcopy(fs_args) or {}
@@ -200,15 +200,15 @@
         Metadata contains the following:
         1. A unique id
         2. A name, if provided
         3. A description, if provided
         4. The list of partition_columns.
         5. The created_time of the table
         6. A map of table configuration. This includes fields such as delta.appendOnly,
-            which if true indicates the table is not meant to have data deleted from it.
+        which if true indicates the table is not meant to have data deleted from it.
 
         Returns: Metadata object containing the above metadata attributes.
         """
         return self._delta_table.metadata()
 
     @property
     def history(self) -> List[Dict[str, Any]]:
```

### Comparing `kedro-datasets-1.5.0/kedro_datasets/pandas/excel_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/pandas/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/pandas/feather_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/pandas/feather_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/pandas/gbq_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/pandas/gbq_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/pandas/generic_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/pandas/generic_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/pandas/hdf_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/pandas/hdf_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/pandas/json_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/pandas/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/pandas/parquet_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/pandas/parquet_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/pandas/sql_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/pandas/sql_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/pandas/xml_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/pandas/xml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/pickle/pickle_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/pickle/pickle_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/pillow/image_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/pillow/image_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/plotly/json_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/plotly/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/plotly/plotly_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/plotly/plotly_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/polars/csv_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/polars/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/redis/redis_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/redis/redis_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/snowflake/snowpark_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/snowflake/snowpark_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/spark/__init__.py` & `kedro-datasets-1.5.1/kedro_datasets/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/spark/deltatable_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/spark/deltatable_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/spark/spark_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/spark/spark_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/spark/spark_hive_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/spark/spark_hive_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/spark/spark_jdbc_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/spark/spark_jdbc_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/spark/spark_streaming_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/spark/spark_streaming_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/svmlight/svmlight_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/svmlight/svmlight_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/tensorflow/tensorflow_model_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/tensorflow/tensorflow_model_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/text/text_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/text/text_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/tracking/json_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/tracking/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/tracking/metrics_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/tracking/metrics_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/video/video_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/video/video_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets/yaml/yaml_dataset.py` & `kedro-datasets-1.5.1/kedro_datasets/yaml/yaml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets.egg-info/PKG-INFO` & `kedro-datasets-1.5.1/kedro_datasets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-datasets
-Version: 1.5.0
+Version: 1.5.1
 Summary: Kedro-Datasets is where you can find all of Kedro's data connectors.
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-datasets
 Project-URL: Documentation, https://docs.kedro.org
 Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
 Requires-Python: <3.11,>=3.7
```

### Comparing `kedro-datasets-1.5.0/kedro_datasets.egg-info/SOURCES.txt` & `kedro-datasets-1.5.1/kedro_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/kedro_datasets.egg-info/requires.txt` & `kedro-datasets-1.5.1/kedro_datasets.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/pyproject.toml` & `kedro-datasets-1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.5.0/tests/test_io.py` & `kedro-datasets-1.5.1/tests/test_io.py`

 * *Files identical despite different names*

