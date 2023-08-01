# Comparing `tmp/ydata-profiling-4.3.2.tar.gz` & `tmp/ydata-profiling-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydata-profiling-4.3.2.tar", last modified: Wed Jul 19 17:53:17 2023, max compression
+gzip compressed data, was "ydata-profiling-4.4.0.tar", last modified: Tue Aug  1 09:01:06 2023, max compression
```

## Comparing `ydata-profiling-4.3.2.tar` & `ydata-profiling-4.4.0.tar`

### file list

```diff
@@ -1,264 +1,267 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.451764 ydata-profiling-4.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    21088 2023-07-19 17:53:17.451764 ydata-profiling-4.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17728 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/requirements-spark.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 17:53:17.451764 ydata-profiling-4.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.399763 ydata-profiling-4.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.403763 ydata-profiling-4.3.2/src/pandas_profiling/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/pandas_profiling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.407763 ydata-profiling-4.3.2/src/ydata_profiling/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/compare_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/config_default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/config_minimal.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.407763 ydata-profiling-4.3.2/src/ydata_profiling/controller/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/controller/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/controller/pandas_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/expectations_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.411763 ydata-profiling-4.3.2/src/ydata_profiling/model/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20409 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/correlations.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/describe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/description.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/expectation_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pairwise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.419763 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/correlations_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/dataframe_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_boolean_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_categorical_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_counts_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_date_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_file_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_generic_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_image_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_numeric_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_path_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_supported_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_text_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_timeseries_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_url_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/discretize_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/duplicates_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/imbalance_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/missing_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/sample_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/summary_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/table_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/utils_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.419763 ydata-profiling-4.3.2/src/ydata_profiling/model/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/spark/correlations_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/spark/dataframe_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/spark/describe_boolean_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/spark/describe_categorical_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/spark/describe_counts_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/spark/describe_date_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/spark/describe_generic_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/spark/describe_numeric_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/spark/describe_supported_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/spark/describe_text_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/spark/duplicates_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/spark/missing_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/spark/sample_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/spark/summary_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/spark/table_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/summarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/summary_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    11595 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/typeset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/model/typeset_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)    19411 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/profile_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.419763 ydata-profiling-4.3.2/src/ydata_profiling/report/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/formatters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.419763 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.427764 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/collapse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/correlation_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/frequency_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/frequency_table_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/item_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/renderable.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/root.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/toggle_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/variable_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.427764 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/flavours.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.427764 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/collapse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/correlation_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/frequency_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/frequency_table_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/root.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.439764 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.439764 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_constant.html
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_constant_length.html
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_duplicates.html
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_empty.html
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_high_cardinality.html
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_high_correlation.html
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_imbalance.html
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_infinite.html
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_missing.html
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_non_stationary.html
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_seasonal.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_skewed.html
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_truncated.html
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_type_date.html
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_uniform.html
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_unique.html
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_unsupported.html
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_zeros.html
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts.html
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/collapse.html
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/correlation_table.html
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/diagram.html
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/duplicate.html
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table.html
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table_small.html
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/report.html
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/sample.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.439764 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/batch_grid.html
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/grid.html
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/list.html
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/named_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/sections.html
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/select.html
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/tabs.html
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/table.html
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/toggle_button.html
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/variable.html
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/variable_info.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.439764 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.443764 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    23409 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   121200 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    37045 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   125618 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/cosmo.bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   127321 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/flatly.bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    97163 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/jquery-1.12.4.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/script.js
--rw-r--r--   0 runner    (1001) docker     (123)   127551 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/simplex.bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/style.css
--rw-r--r--   0 runner    (1001) docker     (123)   122851 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/united.bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/javascript.html
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/style.html
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/toggle_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/variable_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.443764 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/collapse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/correlation_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/frequency_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/frequency_table_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/root.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/toggle_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/variable_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/frequency_table_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.443764 ydata-profiling-4.3.2/src/ydata_profiling/report/structure/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/structure/correlations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/structure/overview.py
--rw-r--r--   0 runner    (1001) docker     (123)    14934 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/structure/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.447764 ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_complex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_real.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/serialize_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.447764 ydata-profiling-4.3.2/src/ydata_profiling/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/utils/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/utils/imghdr_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/utils/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/utils/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/utils/versions.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-19 17:53:17.000000 ydata-profiling-4.3.2/src/ydata_profiling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.451764 ydata-profiling-4.3.2/src/ydata_profiling/visualisation/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/visualisation/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/visualisation/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)    29768 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/visualisation/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/src/ydata_profiling/visualisation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.407763 ydata-profiling-4.3.2/src/ydata_profiling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21088 2023-07-19 17:53:17.000000 ydata-profiling-4.3.2/src/ydata_profiling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-07-19 17:53:17.000000 ydata-profiling-4.3.2/src/ydata_profiling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 17:53:17.000000 ydata-profiling-4.3.2/src/ydata_profiling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-19 17:53:17.000000 ydata-profiling-4.3.2/src/ydata_profiling.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-19 17:53:17.000000 ydata-profiling-4.3.2/src/ydata_profiling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-19 17:53:17.000000 ydata-profiling-4.3.2/src/ydata_profiling.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:53:17.451764 ydata-profiling-4.3.2/venv/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-19 17:50:41.000000 ydata-profiling-4.3.2/venv/spark.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.834506 ydata-profiling-4.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    22068 2023-08-01 09:01:06.834506 ydata-profiling-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18625 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/requirements-spark.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 09:01:06.834506 ydata-profiling-4.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.786506 ydata-profiling-4.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.794506 ydata-profiling-4.4.0/src/pandas_profiling/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/pandas_profiling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.794506 ydata-profiling-4.4.0/src/ydata_profiling/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13111 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/compare_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/config_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/config_minimal.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.798506 ydata-profiling-4.4.0/src/ydata_profiling/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/controller/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/controller/pandas_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/expectations_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.798506 ydata-profiling-4.4.0/src/ydata_profiling/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20409 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/correlations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/describe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/expectation_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pairwise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.802506 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/correlations_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/dataframe_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_boolean_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_categorical_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_counts_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_date_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_file_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_generic_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_image_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_numeric_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_path_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_supported_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_text_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_timeseries_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_url_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/discretize_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/duplicates_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/imbalance_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/missing_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/sample_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/summary_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/table_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/timeseries_index_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/utils_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.806506 ydata-profiling-4.4.0/src/ydata_profiling/model/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/spark/correlations_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/spark/dataframe_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/spark/describe_boolean_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/spark/describe_categorical_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/spark/describe_counts_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/spark/describe_date_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/spark/describe_generic_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/spark/describe_numeric_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/spark/describe_supported_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/spark/describe_text_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/spark/duplicates_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/spark/missing_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/spark/sample_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/spark/summary_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/spark/table_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/spark/timeseries_index_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/summary_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/timeseries_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11595 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/typeset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/model/typeset_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19519 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/profile_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.806506 ydata-profiling-4.4.0/src/ydata_profiling/report/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/formatters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.806506 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.810506 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/collapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/correlation_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/frequency_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/frequency_table_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/item_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/renderable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/toggle_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/variable_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.810506 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/flavours.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.814506 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/collapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/correlation_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/frequency_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/frequency_table_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.814506 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.818506 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_constant.html
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_constant_length.html
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_duplicates.html
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_empty.html
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_high_cardinality.html
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_high_correlation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_imbalance.html
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_infinite.html
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_missing.html
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_non_stationary.html
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_seasonal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_skewed.html
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_truncated.html
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_type_date.html
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_uniform.html
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_unique.html
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_unsupported.html
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_zeros.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/collapse.html
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/correlation_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/diagram.html
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/duplicate.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table_small.html
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/sample.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.818506 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/batch_grid.html
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/grid.html
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/named_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/sections.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/tabs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/table.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/toggle_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/variable.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/variable_info.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.822506 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.822506 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    23409 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   121200 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    37045 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   125618 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/cosmo.bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   127321 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/flatly.bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    97163 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/jquery-1.12.4.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/script.js
+-rw-r--r--   0 runner    (1001) docker     (123)   127551 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/simplex.bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)   122851 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/united.bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/javascript.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/style.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/toggle_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/variable_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.826506 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/collapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/correlation_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/frequency_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/frequency_table_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/toggle_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/variable_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/frequency_table_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.826506 ydata-profiling-4.4.0/src/ydata_profiling/report/structure/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/structure/correlations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/structure/overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14934 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/structure/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.830506 ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/serialize_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.830506 ydata-profiling-4.4.0/src/ydata_profiling/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/utils/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/utils/imghdr_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/utils/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/utils/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/utils/versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 09:01:06.000000 ydata-profiling-4.4.0/src/ydata_profiling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.830506 ydata-profiling-4.4.0/src/ydata_profiling/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/visualisation/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/visualisation/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31968 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/visualisation/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/src/ydata_profiling/visualisation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.794506 ydata-profiling-4.4.0/src/ydata_profiling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22068 2023-08-01 09:01:06.000000 ydata-profiling-4.4.0/src/ydata_profiling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14364 2023-08-01 09:01:06.000000 ydata-profiling-4.4.0/src/ydata_profiling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 09:01:06.000000 ydata-profiling-4.4.0/src/ydata_profiling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 09:01:06.000000 ydata-profiling-4.4.0/src/ydata_profiling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-01 09:01:06.000000 ydata-profiling-4.4.0/src/ydata_profiling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 09:01:06.000000 ydata-profiling-4.4.0/src/ydata_profiling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:01:06.830506 ydata-profiling-4.4.0/venv/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-01 08:57:34.000000 ydata-profiling-4.4.0/venv/spark.yml
```

### Comparing `ydata-profiling-4.3.2/CONTRIBUTING.md` & `ydata-profiling-4.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/LICENSE` & `ydata-profiling-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/MANIFEST.in` & `ydata-profiling-4.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/Makefile` & `ydata-profiling-4.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/PKG-INFO` & `ydata-profiling-4.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydata-profiling
-Version: 4.3.2
+Version: 4.4.0
 Summary: Generate profile report for pandas DataFrame
 Home-page: https://github.com/ydataai/ydata-profiling
 Author: YData Labs Inc
 Author-email: opensource@ydata.ai
 License: MIT
 Description: # ydata-profiling
         
@@ -33,14 +33,16 @@
           Do you like this project? Show us your love and <a href="https://engage.ydata.ai">give feedback!</a>
         </p>
         
         `ydata-profiling` primary goal is to provide a one-line Exploratory Data Analysis (EDA) experience in a consistent and fast solution. Like pandas `df.describe()` function, that is so handy, ydata-profiling delivers an extended analysis of a DataFrame while allowing the data analysis to be exported in different formats such as **html** and **json**.
         
         The package outputs a simple and digested analysis of a dataset, including **time-series** and **text**.
         
+        > **Looking for a scalable solution that can fully integrate with your database systems?**<br>
+        > Leverage YData Fabric Data Catalog to connect to different databases and storages (Oracle, snowflake, PostGreSQL, GCS, S3, etc.) and leverage an interactive and guided profiling experience in Fabric. Check out the [Community Version](https://ydata.ai/ydata-fabric-free-trial).
         
         ## ▶️ Quickstart
         
         ### Install
         ```cmd
         pip install ydata-profiling
         ```
@@ -102,15 +104,15 @@
         |----------|---------------------------------------------------------------------------------------------|
         | [Comparing datasets](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/comparing_datasets.html )                        | Comparing multiple version of the same dataset                                              |
         | [Profiling a Time-Series dataset](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/time_series_datasets.html)               | Generating a report for a time-series dataset with a single line of code                    |
         |[Profiling large datasets](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/big_data.html )                            | Tips on how to prepare data and configure `ydata-profiling` for working with large datasets |
         | [Handling sensitive data](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/sensitive_data.html )                       | Generating reports which are mindful about sensitive data in the input dataset              |
         | [Dataset metadata and data dictionaries](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/metadata.html)               | Complementing the report with dataset details and column-specific data dictionaries         |
         | [Customizing the report's appearance](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/custom_report_appearance.html ) | Changing the appearance of the report's page and of the contained visualizations            |
-        
+        | [Profiling Databases](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/profiling_databases.html) | For a seamless profiling experience in your organization's databases, check [Fabric Data Catalog](https://ydata.ai/products/data_catalog), which allows to consume data from different types of storages such as RDBMs (Azure SQL, PostGreSQL, Oracle, etc.) and object storages (Google Cloud Storage, AWS S3, Snowflake, etc.), among others. |
         ### Using inside Jupyter Notebooks
         
         There are two interfaces to consume the report inside a Jupyter notebook: through widgets and through an embedded HTML report.
         
         <img alt="Notebook Widgets" src="https://ydata-profiling.ydata.ai/docs/master/assets/widgets.gif" width="800" />
         
         The above is achieved by simply displaying the report as a set of widgets. In a Jupyter Notebook, run:
@@ -143,18 +145,18 @@
         
         # As a file
         profile.to_file("your_report.json")
         ```
         
         ### Using in the command line
         
-        For standard formatted CSV files (which can be read directly by pandas without additional settings), the `pandas_profiling` executable can be used in the command line. The example below generates a report named _Example Profiling Report_, using a configuration file called `default.yaml`, in the file `report.html` by processing a `data.csv` dataset.
+        For standard formatted CSV files (which can be read directly by pandas without additional settings), the `ydata_profiling` executable can be used in the command line. The example below generates a report named *Example Profiling Report*, using a configuration file called `default.yaml`, in the file `report.html` by processing a `data.csv` dataset.
         
         ```sh
-        pandas_profiling --title "Example Profiling Report" --config_file default.yaml data.csv report.html
+        ydata_profiling --title "Example Profiling Report" --config_file default.yaml data.csv report.html
         ```
         
         Additional details on the CLI are available [on the documentation](https://ydata-profiling.ydata.ai/docs/master/pages/getting_started/quickstart.html#command-line-usage).
         
         ## 👀 Examples
         
         The following example reports showcase the potentialities of the package across a wide range of dataset and data types:
@@ -233,32 +235,34 @@
         | [requirements.txt](https://github.com/ydataai/pandas-profiling/blob/master/requirements.txt) | Package requirements|
         | [requirements-dev.txt](https://github.com/ydataai/pandas-profiling/blob/master/requirements-dev.txt)  |  Requirements for development|
         | [requirements-test.txt](https://github.com/ydataai/pandas-profiling/blob/master/requirements-test.txt) | Requirements for testing|
         | [setup.py](https://github.com/ydataai/pandas-profiling/blob/master/setup.py) | Requirements for widgets etc. |
         
         ## 🔗 Integrations
         
-        To maximize its usefulness in real world contexts, `pandas-profiling` has a set of implicit and explicit integrations with a variety of other actors in the Data Science ecosystem: 
+        To maximize its usefulness in real world contexts, `ydata-profiling` has a set of implicit and explicit integrations with a variety of other actors in the Data Science ecosystem: 
         
         | Integration type | Description |
         |---|---|
         | [Other DataFrame libraries](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/other_dataframe_libraries.html) | How to compute the profiling of data stored in libraries other than pandas |
         | [Great Expectations](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/great_expectations.html) | Generating [Great Expectations](https://greatexpectations.io) expectations suites directly from a profiling report |
         | [Interactive applications](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/data_apps.html) | Embedding profiling reports in [Streamlit](http://streamlit.io), [Dash](http://dash.plotly.com) or [Panel](https://panel.holoviz.org) applications |
         | [Pipelines](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/pipelines.html) | Integration with DAG workflow execution tools like [Airflow](https://airflow.apache.org) or [Kedro](https://kedro.org) |
-        | [Cloud services](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/cloud_services.html) | Using `pandas-profiling` in hosted computation services like [Lambda](https://lambdalabs.com), [Google Cloud](https://github.com/GoogleCloudPlatform/analytics-componentized-patterns/blob/master/retail/propensity-model/bqml/bqml_kfp_retail_propensity_to_purchase.ipynb) or [Kaggle](https://www.kaggle.com/code) |
-        | [IDEs](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/ides.html) | Using `pandas-profiling` directly from integrated development environments such as [PyCharm](https://www.jetbrains.com/pycharm/) |
+        | [Cloud services](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/cloud_services.html) | Using `ydata-profiling` in hosted computation services like [Lambda](https://lambdalabs.com), [Google Cloud](https://github.com/GoogleCloudPlatform/analytics-componentized-patterns/blob/master/retail/propensity-model/bqml/bqml_kfp_retail_propensity_to_purchase.ipynb) or [Kaggle](https://www.kaggle.com/code) |
+        | [IDEs](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/ides.html) | Using `ydata-profiling` directly from integrated development environments such as [PyCharm](https://www.jetbrains.com/pycharm/) |
         
         ## 🙋 Support
         Need help? Want to share a perspective? Report a bug? Ideas for collaborations? Reach out via the following channels:
         
         - [Stack Overflow](https://stackoverflow.com/questions/tagged/pandas-profiling+or+ydata-profiling): ideal for asking questions on how to use the package
         - [GitHub Issues](https://github.com/ydataai/ydata-profiling/issues): bugs, proposals for changes, feature requests
         - [Discord](https://tiny.ydata.ai/dcai-ydata-profiling): ideal for projects discussions, ask questions, collaborations, general chat
-        - [Email](mailto:developers@ydata.ai): project collaborations or sponsoring
+        
+        > **Need Help?**<br>
+        > Get your questions answered with a product owner by [booking a Pawsome chat](https://meetings.hubspot.com/fabiana-clemente)! 🐼
         
         > ❗ Before reporting an issue on GitHub, check out [Common Issues](https://ydata-profiling.ydata.ai/docs/master/pages/support_contrib/common_issues.html).
         
         ## 🤝🏽 Contributing
         Learn how to get involved in the [Contribution Guide](https://ydata-profiling.ydata.ai/docs/master/pages/support_contrib/contribution_guidelines.html).
         
         A low-threshold place to ask questions or start contributing is the [Data Centric AI Community's Discord](https://tiny.ydata.ai/dcai-ydata-profiling).
@@ -286,11 +290,12 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Framework :: IPython
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: notebook
 Provides-Extra: unicode
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ydata-profiling Version: 4.3.2 Summary: Generate
+Metadata-Version: 2.1 Name: ydata-profiling Version: 4.4.0 Summary: Generate
 profile report for pandas DataFrame Home-page: https://github.com/ydataai/
 ydata-profiling Author: YData Labs Inc Author-email: opensource@ydata.ai
 License: MIT Description: # ydata-profiling [![Build Status](https://
 github.com/ydataai/pandas-profiling/actions/workflows/tests.yml/
 badge.svg?branch=master)](https://github.com/ydataai/pandas-profiling/actions/
 workflows/tests.yml) [![PyPI download month](https://img.shields.io/pypi/dm/
 ydata-profiling.svg)](https://pypi.python.org/pypi/ydata-profiling/) [![]
@@ -20,51 +20,57 @@
         Do you like this project? Show us your love and give_feedback!
 `ydata-profiling` primary goal is to provide a one-line Exploratory Data
 Analysis (EDA) experience in a consistent and fast solution. Like pandas
 `df.describe()` function, that is so handy, ydata-profiling delivers an
 extended analysis of a DataFrame while allowing the data analysis to be
 exported in different formats such as **html** and **json**. The package
 outputs a simple and digested analysis of a dataset, including **time-series**
-and **text**. ## â¶ï¸ Quickstart ### Install ```cmd pip install ydata-
-profiling ``` or ```cmd conda install -c conda-forge ydata-profiling ``` ###
-Start profiling Start by loading your pandas `DataFrame` as you normally would,
-e.g. by using: ```python import numpy as np import pandas as pd from
-ydata_profiling import ProfileReport df = pd.DataFrame(np.random.rand(100, 5),
-columns=["a", "b", "c", "d", "e"]) ``` To generate the standard profiling
-report, merely run: ```python profile = ProfileReport(df, title="Profiling
-Report") ``` ## Key features - **Type inference**: automatic detection of
-columns' data types (*Categorical*, *Numerical*, *Date*, etc.) - **Warnings**:
-A summary of the problems/challenges in the data that you might need to work on
-(*missing data*, *inaccuracies*, *skewness*, etc.) - **Univariate analysis**:
-including descriptive statistics (mean, median, mode, etc) and informative
-visualizations such as distribution histograms - **Multivariate analysis**:
-including correlations, a detailed analysis of missing data, duplicate rows,
-and visual support for variables pairwise interaction - **Time-Series**:
-including different statistical information relative to time dependent data
-such as auto-correlation and seasonality, along ACF and PACF plots. - **Text
-analysis**: most common categories (uppercase, lowercase, separator), scripts
-(Latin, Cyrillic) and blocks (ASCII, Cyrilic) - **File and Image analysis**:
-file sizes, creation dates, dimensions, indication of truncated images and
-existence of EXIF metadata - **Compare datasets**: one-line solution to enable
-a fast and complete report on the comparison of datasets - **Flexible output
-formats**: all analysis can be exported to an HTML report that can be easily
-shared with different parties, as JSON for an easy integration in automated
-systems and as a widget in a Jupyter Notebook. The report contains three
-additional sections: - **Overview**: mostly global details about the dataset
-(number of records, number of variables, overall missigness and duplicates,
-memory footprint) - **Alerts**: a comprehensive and automatic list of potential
-data quality issues (high correlation, skewness, uniformity, zeros, missing
-values, constant values, between others) - **Reproduction**: technical details
-about the analysis (time, version and configuration) ### ð Latest features -
-Want to scale? Check the latest release with â­â¡[Spark support](https://
-ydata-profiling.ydata.ai/docs/master/pages/integrations/pypspark.html)! -
-Looking for how you can do an EDA for Time-Series ð ? Check [this blogpost]
-(https://towardsdatascience.com/how-to-do-an-eda-for-time-series-cbb92b3b1913).
-- You want to compare 2 datasets and get a report? Check [this blogpost](https:
-//medium.com/towards-artificial-intelligence/how-to-compare-2-dataset-with-
+and **text**. > **Looking for a scalable solution that can fully integrate with
+your database systems?**
+> Leverage YData Fabric Data Catalog to connect to different databases and
+storages (Oracle, snowflake, PostGreSQL, GCS, S3, etc.) and leverage an
+interactive and guided profiling experience in Fabric. Check out the [Community
+Version](https://ydata.ai/ydata-fabric-free-trial). ## â¶ï¸ Quickstart ###
+Install ```cmd pip install ydata-profiling ``` or ```cmd conda install -
+c conda-forge ydata-profiling ``` ### Start profiling Start by loading your
+pandas `DataFrame` as you normally would, e.g. by using: ```python import numpy
+as np import pandas as pd from ydata_profiling import ProfileReport df =
+pd.DataFrame(np.random.rand(100, 5), columns=["a", "b", "c", "d", "e"]) ``` To
+generate the standard profiling report, merely run: ```python profile =
+ProfileReport(df, title="Profiling Report") ``` ## Key features - **Type
+inference**: automatic detection of columns' data types (*Categorical*,
+*Numerical*, *Date*, etc.) - **Warnings**: A summary of the problems/challenges
+in the data that you might need to work on (*missing data*, *inaccuracies*,
+*skewness*, etc.) - **Univariate analysis**: including descriptive statistics
+(mean, median, mode, etc) and informative visualizations such as distribution
+histograms - **Multivariate analysis**: including correlations, a detailed
+analysis of missing data, duplicate rows, and visual support for variables
+pairwise interaction - **Time-Series**: including different statistical
+information relative to time dependent data such as auto-correlation and
+seasonality, along ACF and PACF plots. - **Text analysis**: most common
+categories (uppercase, lowercase, separator), scripts (Latin, Cyrillic) and
+blocks (ASCII, Cyrilic) - **File and Image analysis**: file sizes, creation
+dates, dimensions, indication of truncated images and existence of EXIF
+metadata - **Compare datasets**: one-line solution to enable a fast and
+complete report on the comparison of datasets - **Flexible output formats**:
+all analysis can be exported to an HTML report that can be easily shared with
+different parties, as JSON for an easy integration in automated systems and as
+a widget in a Jupyter Notebook. The report contains three additional sections:
+- **Overview**: mostly global details about the dataset (number of records,
+number of variables, overall missigness and duplicates, memory footprint) -
+**Alerts**: a comprehensive and automatic list of potential data quality issues
+(high correlation, skewness, uniformity, zeros, missing values, constant
+values, between others) - **Reproduction**: technical details about the
+analysis (time, version and configuration) ### ð Latest features - Want to
+scale? Check the latest release with â­â¡[Spark support](https://ydata-
+profiling.ydata.ai/docs/master/pages/integrations/pypspark.html)! - Looking for
+how you can do an EDA for Time-Series ð ? Check [this blogpost](https://
+towardsdatascience.com/how-to-do-an-eda-for-time-series-cbb92b3b1913). - You
+want to compare 2 datasets and get a report? Check [this blogpost](https://
+medium.com/towards-artificial-intelligence/how-to-compare-2-dataset-with-
 pandas-profiling-2ae3a9d7695e) ### â¡ Spark Spark support has been released,
 but we are always looking for an extra pair of hands ð. [Check current work
 in progress!](https://github.com/ydataai/ydata-profiling/projects/3). ## ð
 Use cases YData-profiling can be used to deliver a variety of different use-
 case. The documentation includes guides, tips and tricks for tackling them: |
 Use case | Description | |----------|------------------------------------------
 ---------------------------------------------------| | [Comparing datasets]
@@ -79,42 +85,47 @@
 master/pages/use_cases/sensitive_data.html ) | Generating reports which are
 mindful about sensitive data in the input dataset | | [Dataset metadata and
 data dictionaries](https://ydata-profiling.ydata.ai/docs/master/pages/
 use_cases/metadata.html) | Complementing the report with dataset details and
 column-specific data dictionaries | | [Customizing the report's appearance]
 (https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/
 custom_report_appearance.html ) | Changing the appearance of the report's page
-and of the contained visualizations | ### Using inside Jupyter Notebooks There
-are two interfaces to consume the report inside a Jupyter notebook: through
-widgets and through an embedded HTML report. [Notebook Widgets] The above is
-achieved by simply displaying the report as a set of widgets. In a Jupyter
-Notebook, run: ```python profile.to_widgets() ``` The HTML report can be
-directly embedded in a cell in a similar fashion: ```python
-profile.to_notebook_iframe() ``` [HTML] ### Exporting the report to a file To
-generate a HTML report file, save the `ProfileReport` to an object and use the
-`to_file()` function: ```python profile.to_file("your_report.html") ```
-Alternatively, the report's data can be obtained as a JSON file: ```python # As
-a JSON string json_data = profile.to_json() # As a file profile.to_file
-("your_report.json") ``` ### Using in the command line For standard formatted
-CSV files (which can be read directly by pandas without additional settings),
-the `pandas_profiling` executable can be used in the command line. The example
-below generates a report named _Example Profiling Report_, using a
-configuration file called `default.yaml`, in the file `report.html` by
-processing a `data.csv` dataset. ```sh pandas_profiling --title "Example
-Profiling Report" --config_file default.yaml data.csv report.html ```
-Additional details on the CLI are available [on the documentation](https://
-ydata-profiling.ydata.ai/docs/master/pages/getting_started/
-quickstart.html#command-line-usage). ## ð Examples The following example
-reports showcase the potentialities of the package across a wide range of
-dataset and data types: * [Census Income](https://ydata-profiling.ydata.ai/
-examples/master/census/census_report.html) (US Adult Census data relating
-income with other demographic properties) * [NASA Meteorites](https://ydata-
-profiling.ydata.ai/examples/master/meteorites/meteorites_report.html)
-(comprehensive set of meteorite landing - object properties and locations) [!
-[Open In Colab](https://camo.githubusercontent.com/
+and of the contained visualizations | | [Profiling Databases](https://ydata-
+profiling.ydata.ai/docs/master/pages/use_cases/profiling_databases.html) | For
+a seamless profiling experience in your organization's databases, check [Fabric
+Data Catalog](https://ydata.ai/products/data_catalog), which allows to consume
+data from different types of storages such as RDBMs (Azure SQL, PostGreSQL,
+Oracle, etc.) and object storages (Google Cloud Storage, AWS S3, Snowflake,
+etc.), among others. | ### Using inside Jupyter Notebooks There are two
+interfaces to consume the report inside a Jupyter notebook: through widgets and
+through an embedded HTML report. [Notebook Widgets] The above is achieved by
+simply displaying the report as a set of widgets. In a Jupyter Notebook, run:
+```python profile.to_widgets() ``` The HTML report can be directly embedded in
+a cell in a similar fashion: ```python profile.to_notebook_iframe() ``` [HTML]
+### Exporting the report to a file To generate a HTML report file, save the
+`ProfileReport` to an object and use the `to_file()` function: ```python
+profile.to_file("your_report.html") ``` Alternatively, the report's data can be
+obtained as a JSON file: ```python # As a JSON string json_data =
+profile.to_json() # As a file profile.to_file("your_report.json") ``` ### Using
+in the command line For standard formatted CSV files (which can be read
+directly by pandas without additional settings), the `ydata_profiling`
+executable can be used in the command line. The example below generates a
+report named *Example Profiling Report*, using a configuration file called
+`default.yaml`, in the file `report.html` by processing a `data.csv` dataset.
+```sh ydata_profiling --title "Example Profiling Report" --config_file
+default.yaml data.csv report.html ``` Additional details on the CLI are
+available [on the documentation](https://ydata-profiling.ydata.ai/docs/master/
+pages/getting_started/quickstart.html#command-line-usage). ## ð Examples The
+following example reports showcase the potentialities of the package across a
+wide range of dataset and data types: * [Census Income](https://ydata-
+profiling.ydata.ai/examples/master/census/census_report.html) (US Adult Census
+data relating income with other demographic properties) * [NASA Meteorites]
+(https://ydata-profiling.ydata.ai/examples/master/meteorites/
+meteorites_report.html) (comprehensive set of meteorite landing - object
+properties and locations) [![Open In Colab](https://camo.githubusercontent.com/
 52feade06f2fecbf006889a904d221e6a730c194/
 68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)]
 (https://colab.research.google.com/github/ydataai/pandas-profiling/blob/master/
 examples/meteorites/meteorites_cloud.ipynb) [![Binder](https://
 camo.githubusercontent.com/483bae47a175c24dfbfc57390edd8b6982ac5fb3/
 68747470733a2f2f6d7962696e6465722e6f72672f62616467655f6c6f676f2e737667)](https:
 //mybinder.org/v2/gh/ydataai/pandas-profiling/
@@ -181,15 +192,15 @@
 github.com/ydataai/pandas-profiling/blob/master/requirements.txt) | Package
 requirements| | [requirements-dev.txt](https://github.com/ydataai/pandas-
 profiling/blob/master/requirements-dev.txt) | Requirements for development| |
 [requirements-test.txt](https://github.com/ydataai/pandas-profiling/blob/
 master/requirements-test.txt) | Requirements for testing| | [setup.py](https://
 github.com/ydataai/pandas-profiling/blob/master/setup.py) | Requirements for
 widgets etc. | ## ð Integrations To maximize its usefulness in real world
-contexts, `pandas-profiling` has a set of implicit and explicit integrations
+contexts, `ydata-profiling` has a set of implicit and explicit integrations
 with a variety of other actors in the Data Science ecosystem: | Integration
 type | Description | |---|---| | [Other DataFrame libraries](https://ydata-
 profiling.ydata.ai/docs/master/pages/integrations/
 other_dataframe_libraries.html) | How to compute the profiling of data stored
 in libraries other than pandas | | [Great Expectations](https://ydata-
 profiling.ydata.ai/docs/master/pages/integrations/great_expectations.html) |
 Generating [Great Expectations](https://greatexpectations.io) expectations
@@ -197,34 +208,35 @@
 ydata-profiling.ydata.ai/docs/master/pages/integrations/data_apps.html) |
 Embedding profiling reports in [Streamlit](http://streamlit.io), [Dash](http://
 dash.plotly.com) or [Panel](https://panel.holoviz.org) applications | |
 [Pipelines](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/
 pipelines.html) | Integration with DAG workflow execution tools like [Airflow]
 (https://airflow.apache.org) or [Kedro](https://kedro.org) | | [Cloud services]
 (https://ydata-profiling.ydata.ai/docs/master/pages/integrations/
-cloud_services.html) | Using `pandas-profiling` in hosted computation services
+cloud_services.html) | Using `ydata-profiling` in hosted computation services
 like [Lambda](https://lambdalabs.com), [Google Cloud](https://github.com/
 GoogleCloudPlatform/analytics-componentized-patterns/blob/master/retail/
 propensity-model/bqml/bqml_kfp_retail_propensity_to_purchase.ipynb) or [Kaggle]
 (https://www.kaggle.com/code) | | [IDEs](https://ydata-profiling.ydata.ai/docs/
-master/pages/integrations/ides.html) | Using `pandas-profiling` directly from
+master/pages/integrations/ides.html) | Using `ydata-profiling` directly from
 integrated development environments such as [PyCharm](https://
 www.jetbrains.com/pycharm/) | ## ð Support Need help? Want to share a
 perspective? Report a bug? Ideas for collaborations? Reach out via the
 following channels: - [Stack Overflow](https://stackoverflow.com/questions/
 tagged/pandas-profiling+or+ydata-profiling): ideal for asking questions on how
 to use the package - [GitHub Issues](https://github.com/ydataai/ydata-
 profiling/issues): bugs, proposals for changes, feature requests - [Discord]
 (https://tiny.ydata.ai/dcai-ydata-profiling): ideal for projects discussions,
-ask questions, collaborations, general chat - [Email](mailto:
-developers@ydata.ai): project collaborations or sponsoring > â Before
-reporting an issue on GitHub, check out [Common Issues](https://ydata-
-profiling.ydata.ai/docs/master/pages/support_contrib/common_issues.html). ##
-ð¤ð½ Contributing Learn how to get involved in the [Contribution Guide]
-(https://ydata-profiling.ydata.ai/docs/master/pages/support_contrib/
+ask questions, collaborations, general chat > **Need Help?**
+> Get your questions answered with a product owner by [booking a Pawsome chat]
+(https://meetings.hubspot.com/fabiana-clemente)! ð¼ > â Before reporting an
+issue on GitHub, check out [Common Issues](https://ydata-profiling.ydata.ai/
+docs/master/pages/support_contrib/common_issues.html). ## ð¤ð½ Contributing
+Learn how to get involved in the [Contribution Guide](https://ydata-
+profiling.ydata.ai/docs/master/pages/support_contrib/
 contribution_guidelines.html). A low-threshold place to ask questions or start
 contributing is the [Data Centric AI Community's Discord](https://
 tiny.ydata.ai/dcai-ydata-profiling). A big thank you to all our amazing
 contributors! [https://contrib.rocks/image?repo=ydataai/ydata-profiling]
 Contributors wall made with [contrib.rocks](https://contrib.rocks). Keywords:
 pandas data-science data-analysis python jupyter ipython Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable Classifier: Topic ::
@@ -233,9 +245,10 @@
 Independent Classifier: Intended Audience :: Science/Research Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Financial and
 Insurance Industry Classifier: Intended Audience :: Healthcare Industry
 Classifier: Topic :: Scientific/Engineering Classifier: Framework :: IPython
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Requires-Python: >=3.7, <3.12 Description-Content-
-Type: text/markdown Provides-Extra: notebook Provides-Extra: unicode
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7, <3.12 Description-Content-Type: text/markdown Provides-
+Extra: notebook Provides-Extra: unicode
```

### Comparing `ydata-profiling-4.3.2/README.md` & `ydata-profiling-4.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,16 @@
   Do you like this project? Show us your love and <a href="https://engage.ydata.ai">give feedback!</a>
 </p>
 
 `ydata-profiling` primary goal is to provide a one-line Exploratory Data Analysis (EDA) experience in a consistent and fast solution. Like pandas `df.describe()` function, that is so handy, ydata-profiling delivers an extended analysis of a DataFrame while allowing the data analysis to be exported in different formats such as **html** and **json**.
 
 The package outputs a simple and digested analysis of a dataset, including **time-series** and **text**.
 
+> **Looking for a scalable solution that can fully integrate with your database systems?**<br>
+> Leverage YData Fabric Data Catalog to connect to different databases and storages (Oracle, snowflake, PostGreSQL, GCS, S3, etc.) and leverage an interactive and guided profiling experience in Fabric. Check out the [Community Version](https://ydata.ai/ydata-fabric-free-trial).
 
 ## ▶️ Quickstart
 
 ### Install
 ```cmd
 pip install ydata-profiling
 ```
@@ -94,15 +96,15 @@
 |----------|---------------------------------------------------------------------------------------------|
 | [Comparing datasets](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/comparing_datasets.html )                        | Comparing multiple version of the same dataset                                              |
 | [Profiling a Time-Series dataset](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/time_series_datasets.html)               | Generating a report for a time-series dataset with a single line of code                    |
 |[Profiling large datasets](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/big_data.html )                            | Tips on how to prepare data and configure `ydata-profiling` for working with large datasets |
 | [Handling sensitive data](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/sensitive_data.html )                       | Generating reports which are mindful about sensitive data in the input dataset              |
 | [Dataset metadata and data dictionaries](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/metadata.html)               | Complementing the report with dataset details and column-specific data dictionaries         |
 | [Customizing the report's appearance](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/custom_report_appearance.html ) | Changing the appearance of the report's page and of the contained visualizations            |
-
+| [Profiling Databases](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/profiling_databases.html) | For a seamless profiling experience in your organization's databases, check [Fabric Data Catalog](https://ydata.ai/products/data_catalog), which allows to consume data from different types of storages such as RDBMs (Azure SQL, PostGreSQL, Oracle, etc.) and object storages (Google Cloud Storage, AWS S3, Snowflake, etc.), among others. |
 ### Using inside Jupyter Notebooks
 
 There are two interfaces to consume the report inside a Jupyter notebook: through widgets and through an embedded HTML report.
 
 <img alt="Notebook Widgets" src="https://ydata-profiling.ydata.ai/docs/master/assets/widgets.gif" width="800" />
 
 The above is achieved by simply displaying the report as a set of widgets. In a Jupyter Notebook, run:
@@ -135,18 +137,18 @@
 
 # As a file
 profile.to_file("your_report.json")
 ```
 
 ### Using in the command line
 
-For standard formatted CSV files (which can be read directly by pandas without additional settings), the `pandas_profiling` executable can be used in the command line. The example below generates a report named _Example Profiling Report_, using a configuration file called `default.yaml`, in the file `report.html` by processing a `data.csv` dataset.
+For standard formatted CSV files (which can be read directly by pandas without additional settings), the `ydata_profiling` executable can be used in the command line. The example below generates a report named *Example Profiling Report*, using a configuration file called `default.yaml`, in the file `report.html` by processing a `data.csv` dataset.
 
 ```sh
-pandas_profiling --title "Example Profiling Report" --config_file default.yaml data.csv report.html
+ydata_profiling --title "Example Profiling Report" --config_file default.yaml data.csv report.html
 ```
 
 Additional details on the CLI are available [on the documentation](https://ydata-profiling.ydata.ai/docs/master/pages/getting_started/quickstart.html#command-line-usage).
 
 ## 👀 Examples
 
 The following example reports showcase the potentialities of the package across a wide range of dataset and data types:
@@ -225,32 +227,34 @@
 | [requirements.txt](https://github.com/ydataai/pandas-profiling/blob/master/requirements.txt) | Package requirements|
 | [requirements-dev.txt](https://github.com/ydataai/pandas-profiling/blob/master/requirements-dev.txt)  |  Requirements for development|
 | [requirements-test.txt](https://github.com/ydataai/pandas-profiling/blob/master/requirements-test.txt) | Requirements for testing|
 | [setup.py](https://github.com/ydataai/pandas-profiling/blob/master/setup.py) | Requirements for widgets etc. |
 
 ## 🔗 Integrations
 
-To maximize its usefulness in real world contexts, `pandas-profiling` has a set of implicit and explicit integrations with a variety of other actors in the Data Science ecosystem: 
+To maximize its usefulness in real world contexts, `ydata-profiling` has a set of implicit and explicit integrations with a variety of other actors in the Data Science ecosystem: 
 
 | Integration type | Description |
 |---|---|
 | [Other DataFrame libraries](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/other_dataframe_libraries.html) | How to compute the profiling of data stored in libraries other than pandas |
 | [Great Expectations](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/great_expectations.html) | Generating [Great Expectations](https://greatexpectations.io) expectations suites directly from a profiling report |
 | [Interactive applications](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/data_apps.html) | Embedding profiling reports in [Streamlit](http://streamlit.io), [Dash](http://dash.plotly.com) or [Panel](https://panel.holoviz.org) applications |
 | [Pipelines](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/pipelines.html) | Integration with DAG workflow execution tools like [Airflow](https://airflow.apache.org) or [Kedro](https://kedro.org) |
-| [Cloud services](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/cloud_services.html) | Using `pandas-profiling` in hosted computation services like [Lambda](https://lambdalabs.com), [Google Cloud](https://github.com/GoogleCloudPlatform/analytics-componentized-patterns/blob/master/retail/propensity-model/bqml/bqml_kfp_retail_propensity_to_purchase.ipynb) or [Kaggle](https://www.kaggle.com/code) |
-| [IDEs](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/ides.html) | Using `pandas-profiling` directly from integrated development environments such as [PyCharm](https://www.jetbrains.com/pycharm/) |
+| [Cloud services](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/cloud_services.html) | Using `ydata-profiling` in hosted computation services like [Lambda](https://lambdalabs.com), [Google Cloud](https://github.com/GoogleCloudPlatform/analytics-componentized-patterns/blob/master/retail/propensity-model/bqml/bqml_kfp_retail_propensity_to_purchase.ipynb) or [Kaggle](https://www.kaggle.com/code) |
+| [IDEs](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/ides.html) | Using `ydata-profiling` directly from integrated development environments such as [PyCharm](https://www.jetbrains.com/pycharm/) |
 
 ## 🙋 Support
 Need help? Want to share a perspective? Report a bug? Ideas for collaborations? Reach out via the following channels:
 
 - [Stack Overflow](https://stackoverflow.com/questions/tagged/pandas-profiling+or+ydata-profiling): ideal for asking questions on how to use the package
 - [GitHub Issues](https://github.com/ydataai/ydata-profiling/issues): bugs, proposals for changes, feature requests
 - [Discord](https://tiny.ydata.ai/dcai-ydata-profiling): ideal for projects discussions, ask questions, collaborations, general chat
-- [Email](mailto:developers@ydata.ai): project collaborations or sponsoring
+
+> **Need Help?**<br>
+> Get your questions answered with a product owner by [booking a Pawsome chat](https://meetings.hubspot.com/fabiana-clemente)! 🐼
 
 > ❗ Before reporting an issue on GitHub, check out [Common Issues](https://ydata-profiling.ydata.ai/docs/master/pages/support_contrib/common_issues.html).
 
 ## 🤝🏽 Contributing
 Learn how to get involved in the [Contribution Guide](https://ydata-profiling.ydata.ai/docs/master/pages/support_contrib/contribution_guidelines.html).
 
 A low-threshold place to ask questions or start contributing is the [Data Centric AI Community's Discord](https://tiny.ydata.ai/dcai-ydata-profiling).
```

#### html2text {}

```diff
@@ -16,51 +16,57 @@
         Do you like this project? Show us your love and give_feedback!
 `ydata-profiling` primary goal is to provide a one-line Exploratory Data
 Analysis (EDA) experience in a consistent and fast solution. Like pandas
 `df.describe()` function, that is so handy, ydata-profiling delivers an
 extended analysis of a DataFrame while allowing the data analysis to be
 exported in different formats such as **html** and **json**. The package
 outputs a simple and digested analysis of a dataset, including **time-series**
-and **text**. ## â¶ï¸ Quickstart ### Install ```cmd pip install ydata-
-profiling ``` or ```cmd conda install -c conda-forge ydata-profiling ``` ###
-Start profiling Start by loading your pandas `DataFrame` as you normally would,
-e.g. by using: ```python import numpy as np import pandas as pd from
-ydata_profiling import ProfileReport df = pd.DataFrame(np.random.rand(100, 5),
-columns=["a", "b", "c", "d", "e"]) ``` To generate the standard profiling
-report, merely run: ```python profile = ProfileReport(df, title="Profiling
-Report") ``` ## Key features - **Type inference**: automatic detection of
-columns' data types (*Categorical*, *Numerical*, *Date*, etc.) - **Warnings**:
-A summary of the problems/challenges in the data that you might need to work on
-(*missing data*, *inaccuracies*, *skewness*, etc.) - **Univariate analysis**:
-including descriptive statistics (mean, median, mode, etc) and informative
-visualizations such as distribution histograms - **Multivariate analysis**:
-including correlations, a detailed analysis of missing data, duplicate rows,
-and visual support for variables pairwise interaction - **Time-Series**:
-including different statistical information relative to time dependent data
-such as auto-correlation and seasonality, along ACF and PACF plots. - **Text
-analysis**: most common categories (uppercase, lowercase, separator), scripts
-(Latin, Cyrillic) and blocks (ASCII, Cyrilic) - **File and Image analysis**:
-file sizes, creation dates, dimensions, indication of truncated images and
-existence of EXIF metadata - **Compare datasets**: one-line solution to enable
-a fast and complete report on the comparison of datasets - **Flexible output
-formats**: all analysis can be exported to an HTML report that can be easily
-shared with different parties, as JSON for an easy integration in automated
-systems and as a widget in a Jupyter Notebook. The report contains three
-additional sections: - **Overview**: mostly global details about the dataset
-(number of records, number of variables, overall missigness and duplicates,
-memory footprint) - **Alerts**: a comprehensive and automatic list of potential
-data quality issues (high correlation, skewness, uniformity, zeros, missing
-values, constant values, between others) - **Reproduction**: technical details
-about the analysis (time, version and configuration) ### ð Latest features -
-Want to scale? Check the latest release with â­â¡[Spark support](https://
-ydata-profiling.ydata.ai/docs/master/pages/integrations/pypspark.html)! -
-Looking for how you can do an EDA for Time-Series ð ? Check [this blogpost]
-(https://towardsdatascience.com/how-to-do-an-eda-for-time-series-cbb92b3b1913).
-- You want to compare 2 datasets and get a report? Check [this blogpost](https:
-//medium.com/towards-artificial-intelligence/how-to-compare-2-dataset-with-
+and **text**. > **Looking for a scalable solution that can fully integrate with
+your database systems?**
+> Leverage YData Fabric Data Catalog to connect to different databases and
+storages (Oracle, snowflake, PostGreSQL, GCS, S3, etc.) and leverage an
+interactive and guided profiling experience in Fabric. Check out the [Community
+Version](https://ydata.ai/ydata-fabric-free-trial). ## â¶ï¸ Quickstart ###
+Install ```cmd pip install ydata-profiling ``` or ```cmd conda install -
+c conda-forge ydata-profiling ``` ### Start profiling Start by loading your
+pandas `DataFrame` as you normally would, e.g. by using: ```python import numpy
+as np import pandas as pd from ydata_profiling import ProfileReport df =
+pd.DataFrame(np.random.rand(100, 5), columns=["a", "b", "c", "d", "e"]) ``` To
+generate the standard profiling report, merely run: ```python profile =
+ProfileReport(df, title="Profiling Report") ``` ## Key features - **Type
+inference**: automatic detection of columns' data types (*Categorical*,
+*Numerical*, *Date*, etc.) - **Warnings**: A summary of the problems/challenges
+in the data that you might need to work on (*missing data*, *inaccuracies*,
+*skewness*, etc.) - **Univariate analysis**: including descriptive statistics
+(mean, median, mode, etc) and informative visualizations such as distribution
+histograms - **Multivariate analysis**: including correlations, a detailed
+analysis of missing data, duplicate rows, and visual support for variables
+pairwise interaction - **Time-Series**: including different statistical
+information relative to time dependent data such as auto-correlation and
+seasonality, along ACF and PACF plots. - **Text analysis**: most common
+categories (uppercase, lowercase, separator), scripts (Latin, Cyrillic) and
+blocks (ASCII, Cyrilic) - **File and Image analysis**: file sizes, creation
+dates, dimensions, indication of truncated images and existence of EXIF
+metadata - **Compare datasets**: one-line solution to enable a fast and
+complete report on the comparison of datasets - **Flexible output formats**:
+all analysis can be exported to an HTML report that can be easily shared with
+different parties, as JSON for an easy integration in automated systems and as
+a widget in a Jupyter Notebook. The report contains three additional sections:
+- **Overview**: mostly global details about the dataset (number of records,
+number of variables, overall missigness and duplicates, memory footprint) -
+**Alerts**: a comprehensive and automatic list of potential data quality issues
+(high correlation, skewness, uniformity, zeros, missing values, constant
+values, between others) - **Reproduction**: technical details about the
+analysis (time, version and configuration) ### ð Latest features - Want to
+scale? Check the latest release with â­â¡[Spark support](https://ydata-
+profiling.ydata.ai/docs/master/pages/integrations/pypspark.html)! - Looking for
+how you can do an EDA for Time-Series ð ? Check [this blogpost](https://
+towardsdatascience.com/how-to-do-an-eda-for-time-series-cbb92b3b1913). - You
+want to compare 2 datasets and get a report? Check [this blogpost](https://
+medium.com/towards-artificial-intelligence/how-to-compare-2-dataset-with-
 pandas-profiling-2ae3a9d7695e) ### â¡ Spark Spark support has been released,
 but we are always looking for an extra pair of hands ð. [Check current work
 in progress!](https://github.com/ydataai/ydata-profiling/projects/3). ## ð
 Use cases YData-profiling can be used to deliver a variety of different use-
 case. The documentation includes guides, tips and tricks for tackling them: |
 Use case | Description | |----------|------------------------------------------
 ---------------------------------------------------| | [Comparing datasets]
@@ -75,42 +81,47 @@
 master/pages/use_cases/sensitive_data.html ) | Generating reports which are
 mindful about sensitive data in the input dataset | | [Dataset metadata and
 data dictionaries](https://ydata-profiling.ydata.ai/docs/master/pages/
 use_cases/metadata.html) | Complementing the report with dataset details and
 column-specific data dictionaries | | [Customizing the report's appearance]
 (https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/
 custom_report_appearance.html ) | Changing the appearance of the report's page
-and of the contained visualizations | ### Using inside Jupyter Notebooks There
-are two interfaces to consume the report inside a Jupyter notebook: through
-widgets and through an embedded HTML report. [Notebook Widgets] The above is
-achieved by simply displaying the report as a set of widgets. In a Jupyter
-Notebook, run: ```python profile.to_widgets() ``` The HTML report can be
-directly embedded in a cell in a similar fashion: ```python
-profile.to_notebook_iframe() ``` [HTML] ### Exporting the report to a file To
-generate a HTML report file, save the `ProfileReport` to an object and use the
-`to_file()` function: ```python profile.to_file("your_report.html") ```
-Alternatively, the report's data can be obtained as a JSON file: ```python # As
-a JSON string json_data = profile.to_json() # As a file profile.to_file
-("your_report.json") ``` ### Using in the command line For standard formatted
-CSV files (which can be read directly by pandas without additional settings),
-the `pandas_profiling` executable can be used in the command line. The example
-below generates a report named _Example Profiling Report_, using a
-configuration file called `default.yaml`, in the file `report.html` by
-processing a `data.csv` dataset. ```sh pandas_profiling --title "Example
-Profiling Report" --config_file default.yaml data.csv report.html ```
-Additional details on the CLI are available [on the documentation](https://
-ydata-profiling.ydata.ai/docs/master/pages/getting_started/
-quickstart.html#command-line-usage). ## ð Examples The following example
-reports showcase the potentialities of the package across a wide range of
-dataset and data types: * [Census Income](https://ydata-profiling.ydata.ai/
-examples/master/census/census_report.html) (US Adult Census data relating
-income with other demographic properties) * [NASA Meteorites](https://ydata-
-profiling.ydata.ai/examples/master/meteorites/meteorites_report.html)
-(comprehensive set of meteorite landing - object properties and locations) [!
-[Open In Colab](https://camo.githubusercontent.com/
+and of the contained visualizations | | [Profiling Databases](https://ydata-
+profiling.ydata.ai/docs/master/pages/use_cases/profiling_databases.html) | For
+a seamless profiling experience in your organization's databases, check [Fabric
+Data Catalog](https://ydata.ai/products/data_catalog), which allows to consume
+data from different types of storages such as RDBMs (Azure SQL, PostGreSQL,
+Oracle, etc.) and object storages (Google Cloud Storage, AWS S3, Snowflake,
+etc.), among others. | ### Using inside Jupyter Notebooks There are two
+interfaces to consume the report inside a Jupyter notebook: through widgets and
+through an embedded HTML report. [Notebook Widgets] The above is achieved by
+simply displaying the report as a set of widgets. In a Jupyter Notebook, run:
+```python profile.to_widgets() ``` The HTML report can be directly embedded in
+a cell in a similar fashion: ```python profile.to_notebook_iframe() ``` [HTML]
+### Exporting the report to a file To generate a HTML report file, save the
+`ProfileReport` to an object and use the `to_file()` function: ```python
+profile.to_file("your_report.html") ``` Alternatively, the report's data can be
+obtained as a JSON file: ```python # As a JSON string json_data =
+profile.to_json() # As a file profile.to_file("your_report.json") ``` ### Using
+in the command line For standard formatted CSV files (which can be read
+directly by pandas without additional settings), the `ydata_profiling`
+executable can be used in the command line. The example below generates a
+report named *Example Profiling Report*, using a configuration file called
+`default.yaml`, in the file `report.html` by processing a `data.csv` dataset.
+```sh ydata_profiling --title "Example Profiling Report" --config_file
+default.yaml data.csv report.html ``` Additional details on the CLI are
+available [on the documentation](https://ydata-profiling.ydata.ai/docs/master/
+pages/getting_started/quickstart.html#command-line-usage). ## ð Examples The
+following example reports showcase the potentialities of the package across a
+wide range of dataset and data types: * [Census Income](https://ydata-
+profiling.ydata.ai/examples/master/census/census_report.html) (US Adult Census
+data relating income with other demographic properties) * [NASA Meteorites]
+(https://ydata-profiling.ydata.ai/examples/master/meteorites/
+meteorites_report.html) (comprehensive set of meteorite landing - object
+properties and locations) [![Open In Colab](https://camo.githubusercontent.com/
 52feade06f2fecbf006889a904d221e6a730c194/
 68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)]
 (https://colab.research.google.com/github/ydataai/pandas-profiling/blob/master/
 examples/meteorites/meteorites_cloud.ipynb) [![Binder](https://
 camo.githubusercontent.com/483bae47a175c24dfbfc57390edd8b6982ac5fb3/
 68747470733a2f2f6d7962696e6465722e6f72672f62616467655f6c6f676f2e737667)](https:
 //mybinder.org/v2/gh/ydataai/pandas-profiling/
@@ -177,15 +188,15 @@
 github.com/ydataai/pandas-profiling/blob/master/requirements.txt) | Package
 requirements| | [requirements-dev.txt](https://github.com/ydataai/pandas-
 profiling/blob/master/requirements-dev.txt) | Requirements for development| |
 [requirements-test.txt](https://github.com/ydataai/pandas-profiling/blob/
 master/requirements-test.txt) | Requirements for testing| | [setup.py](https://
 github.com/ydataai/pandas-profiling/blob/master/setup.py) | Requirements for
 widgets etc. | ## ð Integrations To maximize its usefulness in real world
-contexts, `pandas-profiling` has a set of implicit and explicit integrations
+contexts, `ydata-profiling` has a set of implicit and explicit integrations
 with a variety of other actors in the Data Science ecosystem: | Integration
 type | Description | |---|---| | [Other DataFrame libraries](https://ydata-
 profiling.ydata.ai/docs/master/pages/integrations/
 other_dataframe_libraries.html) | How to compute the profiling of data stored
 in libraries other than pandas | | [Great Expectations](https://ydata-
 profiling.ydata.ai/docs/master/pages/integrations/great_expectations.html) |
 Generating [Great Expectations](https://greatexpectations.io) expectations
@@ -193,32 +204,33 @@
 ydata-profiling.ydata.ai/docs/master/pages/integrations/data_apps.html) |
 Embedding profiling reports in [Streamlit](http://streamlit.io), [Dash](http://
 dash.plotly.com) or [Panel](https://panel.holoviz.org) applications | |
 [Pipelines](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/
 pipelines.html) | Integration with DAG workflow execution tools like [Airflow]
 (https://airflow.apache.org) or [Kedro](https://kedro.org) | | [Cloud services]
 (https://ydata-profiling.ydata.ai/docs/master/pages/integrations/
-cloud_services.html) | Using `pandas-profiling` in hosted computation services
+cloud_services.html) | Using `ydata-profiling` in hosted computation services
 like [Lambda](https://lambdalabs.com), [Google Cloud](https://github.com/
 GoogleCloudPlatform/analytics-componentized-patterns/blob/master/retail/
 propensity-model/bqml/bqml_kfp_retail_propensity_to_purchase.ipynb) or [Kaggle]
 (https://www.kaggle.com/code) | | [IDEs](https://ydata-profiling.ydata.ai/docs/
-master/pages/integrations/ides.html) | Using `pandas-profiling` directly from
+master/pages/integrations/ides.html) | Using `ydata-profiling` directly from
 integrated development environments such as [PyCharm](https://
 www.jetbrains.com/pycharm/) | ## ð Support Need help? Want to share a
 perspective? Report a bug? Ideas for collaborations? Reach out via the
 following channels: - [Stack Overflow](https://stackoverflow.com/questions/
 tagged/pandas-profiling+or+ydata-profiling): ideal for asking questions on how
 to use the package - [GitHub Issues](https://github.com/ydataai/ydata-
 profiling/issues): bugs, proposals for changes, feature requests - [Discord]
 (https://tiny.ydata.ai/dcai-ydata-profiling): ideal for projects discussions,
-ask questions, collaborations, general chat - [Email](mailto:
-developers@ydata.ai): project collaborations or sponsoring > â Before
-reporting an issue on GitHub, check out [Common Issues](https://ydata-
-profiling.ydata.ai/docs/master/pages/support_contrib/common_issues.html). ##
-ð¤ð½ Contributing Learn how to get involved in the [Contribution Guide]
-(https://ydata-profiling.ydata.ai/docs/master/pages/support_contrib/
+ask questions, collaborations, general chat > **Need Help?**
+> Get your questions answered with a product owner by [booking a Pawsome chat]
+(https://meetings.hubspot.com/fabiana-clemente)! ð¼ > â Before reporting an
+issue on GitHub, check out [Common Issues](https://ydata-profiling.ydata.ai/
+docs/master/pages/support_contrib/common_issues.html). ## ð¤ð½ Contributing
+Learn how to get involved in the [Contribution Guide](https://ydata-
+profiling.ydata.ai/docs/master/pages/support_contrib/
 contribution_guidelines.html). A low-threshold place to ask questions or start
 contributing is the [Data Centric AI Community's Discord](https://
 tiny.ydata.ai/dcai-ydata-profiling). A big thank you to all our amazing
 contributors! [https://contrib.rocks/image?repo=ydataai/ydata-profiling]
 Contributors wall made with [contrib.rocks](https://contrib.rocks).
```

### Comparing `ydata-profiling-4.3.2/make.bat` & `ydata-profiling-4.4.0/make.bat`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/setup.py` & `ydata-profiling-4.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         "Topic :: Scientific/Engineering",
         "Framework :: IPython",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     keywords="pandas data-science data-analysis python jupyter ipython",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         "console_scripts": [
             "ydata_profiling = ydata_profiling.controller.console:main",
```

### Comparing `ydata-profiling-4.3.2/src/pandas_profiling/__init__.py` & `ydata-profiling-4.4.0/src/pandas_profiling/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/__init__.py` & `ydata-profiling-4.4.0/src/ydata_profiling/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/compare_reports.py` & `ydata-profiling-4.4.0/src/ydata_profiling/compare_reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -352,10 +352,12 @@
 
     res: dict = _update_merge(None, descriptions_dict[0])
     for r in descriptions_dict[1:]:
         res = _update_merge(res, r)
 
     res["analysis"]["title"] = _compare_title(res["analysis"]["title"])
     res["alerts"] = _create_placehoder_alerts(res["alerts"])
+    if not any(res["time_index_analysis"]):
+        res["time_index_analysis"] = None
     profile = ProfileReport(None, config=_config)
     profile._description_set = from_dict(data_class=BaseDescription, data=res)
     return profile
```

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/config.py` & `ydata-profiling-4.4.0/src/ydata_profiling/config.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/config_default.yaml` & `ydata-profiling-4.4.0/src/ydata_profiling/config_default.yaml`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/config_minimal.yaml` & `ydata-profiling-4.4.0/src/ydata_profiling/config_minimal.yaml`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/controller/console.py` & `ydata-profiling-4.4.0/src/ydata_profiling/controller/console.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/expectations_report.py` & `ydata-profiling-4.4.0/src/ydata_profiling/expectations_report.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/alerts.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/alerts.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/correlations.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/correlations.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/describe.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/describe.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 from ydata_profiling.model import BaseAnalysis, BaseDescription
 from ydata_profiling.model.alerts import get_alerts
 from ydata_profiling.model.correlations import (
     calculate_correlation,
     get_active_correlations,
 )
 from ydata_profiling.model.dataframe import check_dataframe, preprocess
+from ydata_profiling.model.description import TimeIndexAnalysis
 from ydata_profiling.model.duplicates import get_duplicates
 from ydata_profiling.model.missing import get_missing_active, get_missing_diagram
 from ydata_profiling.model.pairwise import get_scatter_plot, get_scatter_tasks
 from ydata_profiling.model.sample import get_custom_sample, get_sample
 from ydata_profiling.model.summarizer import BaseSummarizer
 from ydata_profiling.model.summary import get_series_descriptions
 from ydata_profiling.model.table import get_table_stats
+from ydata_profiling.model.timeseries_index import get_time_index_description
 from ydata_profiling.utils.progress_bar import progress
 from ydata_profiling.version import __version__
 
 
 def describe(
     config: Settings,
     df: pd.DataFrame,
@@ -154,29 +156,36 @@
         )
         table_stats.update(metrics)
 
         alerts = progress(get_alerts, pbar, "Get alerts")(
             config, table_stats, series_description, correlations
         )
 
+        if config.vars.timeseries.active:
+            tsindex_description = get_time_index_description(config, df, table_stats)
+
         pbar.set_postfix_str("Get reproduction details")
         package = {
             "ydata_profiling_version": __version__,
             "ydata_profiling_config": config.json(),
         }
         pbar.update()
 
         pbar.set_postfix_str("Completed")
 
         date_end = datetime.utcnow()
 
     analysis = BaseAnalysis(config.title, date_start, date_end)
+    time_index_analysis = None
+    if config.vars.timeseries.active and tsindex_description:
+        time_index_analysis = TimeIndexAnalysis(**tsindex_description)
 
     description = BaseDescription(
         analysis=analysis,
+        time_index_analysis=time_index_analysis,
         table=table_stats,
         variables=series_description,
         scatter=scatter_matrix,
         correlations=correlations,
         missing=missing,
         alerts=alerts,
         package=package,
```

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/expectation_algorithms.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/expectation_algorithms.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/handler.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/handler.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/missing.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/missing.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pairwise.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pairwise.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/__init__.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     describe_timeseries_pandas,
     describe_url_pandas,
     duplicates_pandas,
     missing_pandas,
     sample_pandas,
     summary_pandas,
     table_pandas,
+    timeseries_index_pandas,
 )
 
 __all__ = [
     "correlations_pandas",
     "dataframe_pandas",
     "describe_boolean_pandas",
     "describe_categorical_pandas",
@@ -39,8 +40,9 @@
     "describe_url_pandas",
     "duplicates_pandas",
     "missing_pandas",
     "sample_pandas",
     "sample_pandas",
     "summary_pandas",
     "table_pandas",
+    "timeseries_index_pandas",
 ]
```

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/correlations_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/correlations_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/dataframe_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/dataframe_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_boolean_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_boolean_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_categorical_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_categorical_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_counts_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_counts_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_date_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_date_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_file_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_file_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_generic_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_generic_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_image_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_image_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_numeric_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_numeric_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_path_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_path_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_supported_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_supported_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_text_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_text_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_timeseries_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_timeseries_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/describe_url_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/describe_url_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/discretize_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/discretize_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/duplicates_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/duplicates_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/imbalance_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/imbalance_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/missing_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/missing_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/sample_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/sample_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/summary_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/summary_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/table_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/table_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/pandas/utils_pandas.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/pandas/utils_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/sample.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/sample.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/spark/__init__.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/spark/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     describe_numeric_spark,
     describe_supported_spark,
     duplicates_spark,
     missing_spark,
     sample_spark,
     summary_spark,
     table_spark,
+    timeseries_index_spark,
 )
 
 __all__ = [
     "correlations_spark",
     "dataframe_spark",
     "describe_boolean_spark",
     "describe_categorical_spark",
@@ -27,8 +28,9 @@
     "describe_supported_spark",
     "duplicates_spark",
     "missing_spark",
     "sample_spark",
     "sample_spark",
     "summary_spark",
     "table_spark",
+    "timeseries_index_spark",
 ]
```

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/spark/correlations_spark.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/spark/correlations_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/spark/dataframe_spark.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/spark/dataframe_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/spark/describe_boolean_spark.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/spark/describe_boolean_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/spark/describe_categorical_spark.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/spark/describe_categorical_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/spark/describe_counts_spark.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/spark/describe_counts_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/spark/describe_date_spark.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/spark/describe_date_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/spark/describe_generic_spark.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/spark/describe_generic_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/spark/describe_numeric_spark.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/spark/describe_numeric_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/spark/describe_supported_spark.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/spark/describe_supported_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/spark/describe_text_spark.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/spark/describe_text_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/spark/duplicates_spark.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/spark/duplicates_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/spark/missing_spark.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/spark/missing_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/spark/sample_spark.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/spark/sample_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/spark/summary_spark.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/spark/summary_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/spark/table_spark.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/spark/table_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/summarizer.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/summarizer.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/summary.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/summary.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/summary_algorithms.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/summary_algorithms.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/typeset.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/typeset.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/model/typeset_relations.py` & `ydata-profiling-4.4.0/src/ydata_profiling/model/typeset_relations.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/profile_report.py` & `ydata-profiling-4.4.0/src/ydata_profiling/profile_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,21 +193,23 @@
     def __initialize_dataframe(
         df: Optional[Union[pd.DataFrame, sDataFrame]], report_config: Settings
     ) -> Optional[Union[pd.DataFrame, sDataFrame]]:
         if (
             df is not None
             and isinstance(df, pd.DataFrame)
             and report_config.vars.timeseries.active
-            and report_config.vars.timeseries.sortby
         ):
-            return df.sort_values(by=report_config.vars.timeseries.sortby).reset_index(
-                drop=True
-            )
-        else:
-            return df
+            if report_config.vars.timeseries.sortby:
+                df = df.sort_values(by=report_config.vars.timeseries.sortby)
+                df = df.set_index(report_config.vars.timeseries.sortby, drop=False)
+                df.index.name = None
+            else:
+                df = df.sort_index()
+
+        return df
 
     def invalidate_cache(self, subset: Optional[str] = None) -> None:
         """Invalidate report cache. Useful after changing setting.
 
         Args:
             subset:
             - "rendering" to invalidate the html, json and widget report rendering
```

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/formatters.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/formatters.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/__init__.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/alerts.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/alerts.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/collapse.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/collapse.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/container.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/container.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/correlation_table.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/correlation_table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/dropdown.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/dropdown.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/image.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/image.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/renderable.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/renderable.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/root.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/root.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/sample.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/sample.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/table.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/variable.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/variable.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/core/variable_info.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/core/variable_info.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/flavours.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/flavours.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/__init__.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/alerts.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/alerts.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/container.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/container.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/correlation_table.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/correlation_table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/duplicate.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/duplicate.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/frequency_table.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/frequency_table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/frequency_table_small.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/frequency_table_small.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts.html` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table.html` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table_small.html` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table_small.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/report.html` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/report.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/batch_grid.html` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/batch_grid.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/grid.html` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/grid.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/sections.html` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/sections.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/select.html` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/select.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/tabs.html` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/tabs.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/table.html` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/table.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/toggle_button.html` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/toggle_button.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/variable_info.html` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/variable_info.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap-theme.min.css` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.css` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.js` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/cosmo.bootstrap.min.css` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/cosmo.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/flatly.bootstrap.min.css` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/flatly.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/jquery-1.12.4.min.js` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/jquery-1.12.4.min.js`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/script.js` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/script.js`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/simplex.bootstrap.min.css` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/simplex.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/style.css` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/style.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/united.bootstrap.min.css` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/united.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/javascript.html` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/javascript.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/navigation.html` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/navigation.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/style.html` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/style.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/html/templates.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/html/templates.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/__init__.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/alerts.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/alerts.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/collapse.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/collapse.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/container.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/container.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/dropdown.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/dropdown.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/frequency_table.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/frequency_table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/frequency_table_small.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/frequency_table_small.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/image.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/image.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/notebook.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/notebook.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/table.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/flavours/widget/toggle_button.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/flavours/widget/toggle_button.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/presentation/frequency_table_utils.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/presentation/frequency_table_utils.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/structure/correlations.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/structure/correlations.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/structure/overview.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/structure/overview.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-from typing import List
+from datetime import datetime
+from typing import Any, List
 from urllib.parse import quote
 
 from ydata_profiling.config import Settings
 from ydata_profiling.model import BaseDescription
 from ydata_profiling.model.alerts import AlertType
+from ydata_profiling.model.description import TimeIndexAnalysis
 from ydata_profiling.report.formatters import (
     fmt,
     fmt_bytesize,
     fmt_number,
     fmt_numeric,
     fmt_percent,
     fmt_timespan,
     list_args,
 )
-from ydata_profiling.report.presentation.core import Alerts, Container, Table
+from ydata_profiling.report.presentation.core import Alerts, Container
+from ydata_profiling.report.presentation.core import Image as ImageWidget
+from ydata_profiling.report.presentation.core import Table
 from ydata_profiling.report.presentation.core.renderable import Renderable
+from ydata_profiling.visualisation.plot import plot_overview_timeseries
 
 
 def get_dataset_overview(config: Settings, summary: BaseDescription) -> Renderable:
     table_metrics = [
         {
             "name": "Number of variables",
             "value": fmt_number(summary.table["n_var"]),
@@ -262,14 +267,84 @@
         alerts=alerts,
         name=f"Alerts ({count})",
         anchor_id="alerts",
         style=config.html.style,
     )
 
 
+def get_timeseries_items(config: Settings, summary: BaseDescription) -> Container:
+    def format_tsindex_limit(limit: Any) -> str:
+        if isinstance(limit, datetime):
+            return limit.strftime("%Y-%m-%d %H:%M:%S")
+        else:
+            return fmt_number(limit)
+
+    assert isinstance(summary.time_index_analysis, TimeIndexAnalysis)
+    table_stats = [
+        {
+            "name": "Number of series",
+            "value": fmt_number(summary.time_index_analysis.n_series),
+        },
+        {
+            "name": "Time series length",
+            "value": fmt_number(summary.time_index_analysis.length),
+        },
+        {
+            "name": "Starting point",
+            "value": format_tsindex_limit(summary.time_index_analysis.start),
+        },
+        {
+            "name": "Ending point",
+            "value": format_tsindex_limit(summary.time_index_analysis.end),
+        },
+        {
+            "name": "Period",
+            "value": fmt_number(summary.time_index_analysis.period),
+        },
+    ]
+
+    if summary.time_index_analysis.frequency:
+        table_stats.append(
+            {
+                "name": "Frequency",
+                "value": summary.time_index_analysis.frequency,
+            }
+        )
+
+    ts_info = Table(table_stats, name="Timeseries statistics", style=config.html.style)
+
+    timeseries = ImageWidget(
+        plot_overview_timeseries(config, summary.variables),
+        image_format=config.plot.image_format,
+        alt="ts_plot",
+        name="preview",
+        anchor_id="ts_plot_overview",
+    )
+    timeseries_scaled = ImageWidget(
+        plot_overview_timeseries(config, summary.variables, scale=True),
+        image_format=config.plot.image_format,
+        alt="ts_plot_scaled",
+        name="scaled",
+        anchor_id="ts_plot_scaled_overview",
+    )
+    ts_tab = Container(
+        [timeseries, timeseries_scaled],
+        anchor_id="ts_plot_overview",
+        name="",
+        sequence_type="tabs",
+    )
+
+    return Container(
+        [ts_info, ts_tab],
+        anchor_id="timeseries_overview",
+        name="Time Series",
+        sequence_type="grid",
+    )
+
+
 def get_dataset_items(config: Settings, summary: BaseDescription, alerts: list) -> list:
     """Returns the dataset overview (at the top of the report)
 
     Args:
         config: settings object
         summary: the calculated summary
         alerts: the alerts
@@ -289,13 +364,16 @@
         key: config.variables.descriptions[key]
         for key in config.variables.descriptions.keys()
     }
 
     if len(column_details) > 0:
         items.append(get_dataset_column_definitions(config, column_details))
 
+    if summary.time_index_analysis:
+        items.append(get_timeseries_items(config, summary))
+
     if alerts:
         items.append(get_dataset_alerts(config, alerts))
 
     items.append(get_dataset_reproduction(config, summary))
 
     return items
```

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/structure/report.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/structure/report.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/__init__.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_boolean.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_boolean.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_categorical.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_categorical.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_common.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_common.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_complex.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_complex.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_count.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_count.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_date.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_date.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_file.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_file.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_generic.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_generic.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_image.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_image.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_path.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_path.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_real.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_real.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_text.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_text.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_timeseries.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,14 +277,22 @@
         image_format=image_format,
         alt="Autocorrelation",
         caption="<strong>ACF and PACF</strong>",
         name="Autocorrelation",
         anchor_id=f"{varid}acf_pacf",
     )
 
+    ts_plot = Image(
+        mini_ts_plot(config, summary["series"], figsize=(7, 3)),
+        image_format=image_format,
+        alt="Time-series plot",
+        name="Time-series",
+        anchor_id=f"{varid}_ts_plot",
+    )
+
     template_variables["bottom"] = Container(
-        [statistics, hist, fq, evs, acf_pacf],
+        [statistics, hist, ts_plot, fq, evs, acf_pacf],
         sequence_type="tabs",
         anchor_id=f"{varid}bottom",
     )
 
     return template_variables
```

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/report/structure/variables/render_url.py` & `ydata-profiling-4.4.0/src/ydata_profiling/report/structure/variables/render_url.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/serialize_report.py` & `ydata-profiling-4.4.0/src/ydata_profiling/serialize_report.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/utils/cache.py` & `ydata-profiling-4.4.0/src/ydata_profiling/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/utils/common.py` & `ydata-profiling-4.4.0/src/ydata_profiling/utils/common.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/utils/dataframe.py` & `ydata-profiling-4.4.0/src/ydata_profiling/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/utils/imghdr_patch.py` & `ydata-profiling-4.4.0/src/ydata_profiling/utils/imghdr_patch.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/utils/paths.py` & `ydata-profiling-4.4.0/src/ydata_profiling/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/visualisation/context.py` & `ydata-profiling-4.4.0/src/ydata_profiling/visualisation/context.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/visualisation/missing.py` & `ydata-profiling-4.4.0/src/ydata_profiling/visualisation/missing.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/visualisation/plot.py` & `ydata-profiling-4.4.0/src/ydata_profiling/visualisation/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import matplotlib
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from matplotlib import pyplot as plt
 from matplotlib.collections import PolyCollection
 from matplotlib.colors import Colormap, LinearSegmentedColormap, ListedColormap, rgb2hex
+from matplotlib.dates import AutoDateLocator, ConciseDateFormatter
 from matplotlib.patches import Patch
 from matplotlib.ticker import FuncFormatter
 from statsmodels.graphics.tsaplots import plot_acf, plot_pacf
 from typeguard import typechecked
 from wordcloud import WordCloud
 
 from ydata_profiling.config import Settings
@@ -540,14 +541,69 @@
         init = colors[0]
         end = colors[1] if len(colors) >= 2 else "#000000"
         cmap = LinearSegmentedColormap.from_list("ts_leg", [init, end], len(labels))
         colors = [rgb2hex(cmap(i)) for i in range(cmap.N)]
     return colors
 
 
+def _format_ts_date_axis(
+    series: pd.Series,
+    axis: matplotlib.axis.Axis,
+) -> matplotlib.axis.Axis:
+    if isinstance(series.index, pd.DatetimeIndex):
+        locator = AutoDateLocator()
+        axis.xaxis.set_major_locator(locator)
+        axis.xaxis.set_major_formatter(ConciseDateFormatter(locator))
+
+    return axis
+
+
+@manage_matplotlib_context()
+def plot_overview_timeseries(
+    config: Settings,
+    variables: Any,
+    figsize: tuple = (6, 4),
+    scale: bool = False,
+) -> matplotlib.figure.Figure:
+    """Plot an line plot from the data and return the AxesSubplot object.
+    Args:
+        variables: The data to plot.
+        figsize: The size of the figure (width, height) in inches, default (6,4).
+        scale: Scale series values between [0,1]. Defaults to False.
+    Returns:
+        The TimeSeries lineplot.
+    """
+    fig = plt.figure(figsize=figsize)
+    ax = fig.add_subplot(111)
+
+    col = next(iter(variables))
+    if isinstance(variables[col]["type"], list):
+        colors = create_comparison_color_list(config)
+        line_styles = ["-", "--"]
+        for col, data in variables.items():
+            if all(iter([t == "TimeSeries" for t in data["type"]])):
+                for i, series in enumerate(data["series"]):
+                    if scale:
+                        series = (series - series.min()) / (series.max() - series.min())
+                    series.plot(
+                        ax=ax,
+                        label=col,
+                        linestyle=line_styles[i],
+                        color=colors[i],
+                        alpha=0.65,
+                    )
+    else:
+        for col, data in variables.items():
+            if data["type"] == "TimeSeries":
+                data["series"].plot(ax=ax, label=col)
+
+    plt.legend(loc="upper right")
+    return plot_360_n0sc0pe(config)
+
+
 def _plot_timeseries(
     config: Settings,
     series: Union[list, pd.Series],
     figsize: tuple = (6, 4),
 ) -> matplotlib.figure.Figure:
     """Plot an line plot from the data and return the AxesSubplot object.
     Args:
@@ -560,31 +616,39 @@
     plot = fig.add_subplot(111)
 
     if isinstance(series, list):
         labels = config.html.style._labels
         colors = create_comparison_color_list(config)
 
         for serie, color, label in zip(series, colors, labels):
-            serie.plot(color=color, label=label)
+            ax = serie.plot(color=color, label=label, alpha=0.75)
+            _format_ts_date_axis(serie, ax)
 
     else:
-        series.plot(color=config.html.style.primary_colors[0])
+        ax = series.plot(color=config.html.style.primary_colors[0])
+        _format_ts_date_axis(series, ax)
 
     return plot
 
 
 @manage_matplotlib_context()
-def mini_ts_plot(config: Settings, series: Union[list, pd.Series]) -> str:
+def mini_ts_plot(
+    config: Settings,
+    series: Union[list, pd.Series],
+    figsize: Tuple[float, float] = (3, 2.25),
+) -> str:
     """Plot an time-series plot of the data.
     Args:
-      series: The data to plot.
+        config: profiling settings.
+        series: The data to plot.
+        figsize: The size of the figure (width, height) in inches, default (3, 2.25)
     Returns:
-      The resulting timeseries plot encoded as a string.
+        The resulting timeseries plot encoded as a string.
     """
-    plot = _plot_timeseries(config, series, figsize=(3, 2.25))
+    plot = _plot_timeseries(config, series, figsize=figsize)
     plot.xaxis.set_tick_params(rotation=45)
     plt.rc("ytick", labelsize=3)
 
     for tick in plot.xaxis.get_major_ticks():
         if isinstance(series.index, pd.DatetimeIndex):
             tick.label1.set_fontsize(6)
         else:
```

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling/visualisation/utils.py` & `ydata-profiling-4.4.0/src/ydata_profiling/visualisation/utils.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling.egg-info/PKG-INFO` & `ydata-profiling-4.4.0/src/ydata_profiling.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydata-profiling
-Version: 4.3.2
+Version: 4.4.0
 Summary: Generate profile report for pandas DataFrame
 Home-page: https://github.com/ydataai/ydata-profiling
 Author: YData Labs Inc
 Author-email: opensource@ydata.ai
 License: MIT
 Description: # ydata-profiling
         
@@ -33,14 +33,16 @@
           Do you like this project? Show us your love and <a href="https://engage.ydata.ai">give feedback!</a>
         </p>
         
         `ydata-profiling` primary goal is to provide a one-line Exploratory Data Analysis (EDA) experience in a consistent and fast solution. Like pandas `df.describe()` function, that is so handy, ydata-profiling delivers an extended analysis of a DataFrame while allowing the data analysis to be exported in different formats such as **html** and **json**.
         
         The package outputs a simple and digested analysis of a dataset, including **time-series** and **text**.
         
+        > **Looking for a scalable solution that can fully integrate with your database systems?**<br>
+        > Leverage YData Fabric Data Catalog to connect to different databases and storages (Oracle, snowflake, PostGreSQL, GCS, S3, etc.) and leverage an interactive and guided profiling experience in Fabric. Check out the [Community Version](https://ydata.ai/ydata-fabric-free-trial).
         
         ## ▶️ Quickstart
         
         ### Install
         ```cmd
         pip install ydata-profiling
         ```
@@ -102,15 +104,15 @@
         |----------|---------------------------------------------------------------------------------------------|
         | [Comparing datasets](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/comparing_datasets.html )                        | Comparing multiple version of the same dataset                                              |
         | [Profiling a Time-Series dataset](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/time_series_datasets.html)               | Generating a report for a time-series dataset with a single line of code                    |
         |[Profiling large datasets](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/big_data.html )                            | Tips on how to prepare data and configure `ydata-profiling` for working with large datasets |
         | [Handling sensitive data](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/sensitive_data.html )                       | Generating reports which are mindful about sensitive data in the input dataset              |
         | [Dataset metadata and data dictionaries](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/metadata.html)               | Complementing the report with dataset details and column-specific data dictionaries         |
         | [Customizing the report's appearance](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/custom_report_appearance.html ) | Changing the appearance of the report's page and of the contained visualizations            |
-        
+        | [Profiling Databases](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/profiling_databases.html) | For a seamless profiling experience in your organization's databases, check [Fabric Data Catalog](https://ydata.ai/products/data_catalog), which allows to consume data from different types of storages such as RDBMs (Azure SQL, PostGreSQL, Oracle, etc.) and object storages (Google Cloud Storage, AWS S3, Snowflake, etc.), among others. |
         ### Using inside Jupyter Notebooks
         
         There are two interfaces to consume the report inside a Jupyter notebook: through widgets and through an embedded HTML report.
         
         <img alt="Notebook Widgets" src="https://ydata-profiling.ydata.ai/docs/master/assets/widgets.gif" width="800" />
         
         The above is achieved by simply displaying the report as a set of widgets. In a Jupyter Notebook, run:
@@ -143,18 +145,18 @@
         
         # As a file
         profile.to_file("your_report.json")
         ```
         
         ### Using in the command line
         
-        For standard formatted CSV files (which can be read directly by pandas without additional settings), the `pandas_profiling` executable can be used in the command line. The example below generates a report named _Example Profiling Report_, using a configuration file called `default.yaml`, in the file `report.html` by processing a `data.csv` dataset.
+        For standard formatted CSV files (which can be read directly by pandas without additional settings), the `ydata_profiling` executable can be used in the command line. The example below generates a report named *Example Profiling Report*, using a configuration file called `default.yaml`, in the file `report.html` by processing a `data.csv` dataset.
         
         ```sh
-        pandas_profiling --title "Example Profiling Report" --config_file default.yaml data.csv report.html
+        ydata_profiling --title "Example Profiling Report" --config_file default.yaml data.csv report.html
         ```
         
         Additional details on the CLI are available [on the documentation](https://ydata-profiling.ydata.ai/docs/master/pages/getting_started/quickstart.html#command-line-usage).
         
         ## 👀 Examples
         
         The following example reports showcase the potentialities of the package across a wide range of dataset and data types:
@@ -233,32 +235,34 @@
         | [requirements.txt](https://github.com/ydataai/pandas-profiling/blob/master/requirements.txt) | Package requirements|
         | [requirements-dev.txt](https://github.com/ydataai/pandas-profiling/blob/master/requirements-dev.txt)  |  Requirements for development|
         | [requirements-test.txt](https://github.com/ydataai/pandas-profiling/blob/master/requirements-test.txt) | Requirements for testing|
         | [setup.py](https://github.com/ydataai/pandas-profiling/blob/master/setup.py) | Requirements for widgets etc. |
         
         ## 🔗 Integrations
         
-        To maximize its usefulness in real world contexts, `pandas-profiling` has a set of implicit and explicit integrations with a variety of other actors in the Data Science ecosystem: 
+        To maximize its usefulness in real world contexts, `ydata-profiling` has a set of implicit and explicit integrations with a variety of other actors in the Data Science ecosystem: 
         
         | Integration type | Description |
         |---|---|
         | [Other DataFrame libraries](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/other_dataframe_libraries.html) | How to compute the profiling of data stored in libraries other than pandas |
         | [Great Expectations](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/great_expectations.html) | Generating [Great Expectations](https://greatexpectations.io) expectations suites directly from a profiling report |
         | [Interactive applications](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/data_apps.html) | Embedding profiling reports in [Streamlit](http://streamlit.io), [Dash](http://dash.plotly.com) or [Panel](https://panel.holoviz.org) applications |
         | [Pipelines](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/pipelines.html) | Integration with DAG workflow execution tools like [Airflow](https://airflow.apache.org) or [Kedro](https://kedro.org) |
-        | [Cloud services](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/cloud_services.html) | Using `pandas-profiling` in hosted computation services like [Lambda](https://lambdalabs.com), [Google Cloud](https://github.com/GoogleCloudPlatform/analytics-componentized-patterns/blob/master/retail/propensity-model/bqml/bqml_kfp_retail_propensity_to_purchase.ipynb) or [Kaggle](https://www.kaggle.com/code) |
-        | [IDEs](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/ides.html) | Using `pandas-profiling` directly from integrated development environments such as [PyCharm](https://www.jetbrains.com/pycharm/) |
+        | [Cloud services](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/cloud_services.html) | Using `ydata-profiling` in hosted computation services like [Lambda](https://lambdalabs.com), [Google Cloud](https://github.com/GoogleCloudPlatform/analytics-componentized-patterns/blob/master/retail/propensity-model/bqml/bqml_kfp_retail_propensity_to_purchase.ipynb) or [Kaggle](https://www.kaggle.com/code) |
+        | [IDEs](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/ides.html) | Using `ydata-profiling` directly from integrated development environments such as [PyCharm](https://www.jetbrains.com/pycharm/) |
         
         ## 🙋 Support
         Need help? Want to share a perspective? Report a bug? Ideas for collaborations? Reach out via the following channels:
         
         - [Stack Overflow](https://stackoverflow.com/questions/tagged/pandas-profiling+or+ydata-profiling): ideal for asking questions on how to use the package
         - [GitHub Issues](https://github.com/ydataai/ydata-profiling/issues): bugs, proposals for changes, feature requests
         - [Discord](https://tiny.ydata.ai/dcai-ydata-profiling): ideal for projects discussions, ask questions, collaborations, general chat
-        - [Email](mailto:developers@ydata.ai): project collaborations or sponsoring
+        
+        > **Need Help?**<br>
+        > Get your questions answered with a product owner by [booking a Pawsome chat](https://meetings.hubspot.com/fabiana-clemente)! 🐼
         
         > ❗ Before reporting an issue on GitHub, check out [Common Issues](https://ydata-profiling.ydata.ai/docs/master/pages/support_contrib/common_issues.html).
         
         ## 🤝🏽 Contributing
         Learn how to get involved in the [Contribution Guide](https://ydata-profiling.ydata.ai/docs/master/pages/support_contrib/contribution_guidelines.html).
         
         A low-threshold place to ask questions or start contributing is the [Data Centric AI Community's Discord](https://tiny.ydata.ai/dcai-ydata-profiling).
@@ -286,11 +290,12 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Framework :: IPython
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: notebook
 Provides-Extra: unicode
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ydata-profiling Version: 4.3.2 Summary: Generate
+Metadata-Version: 2.1 Name: ydata-profiling Version: 4.4.0 Summary: Generate
 profile report for pandas DataFrame Home-page: https://github.com/ydataai/
 ydata-profiling Author: YData Labs Inc Author-email: opensource@ydata.ai
 License: MIT Description: # ydata-profiling [![Build Status](https://
 github.com/ydataai/pandas-profiling/actions/workflows/tests.yml/
 badge.svg?branch=master)](https://github.com/ydataai/pandas-profiling/actions/
 workflows/tests.yml) [![PyPI download month](https://img.shields.io/pypi/dm/
 ydata-profiling.svg)](https://pypi.python.org/pypi/ydata-profiling/) [![]
@@ -20,51 +20,57 @@
         Do you like this project? Show us your love and give_feedback!
 `ydata-profiling` primary goal is to provide a one-line Exploratory Data
 Analysis (EDA) experience in a consistent and fast solution. Like pandas
 `df.describe()` function, that is so handy, ydata-profiling delivers an
 extended analysis of a DataFrame while allowing the data analysis to be
 exported in different formats such as **html** and **json**. The package
 outputs a simple and digested analysis of a dataset, including **time-series**
-and **text**. ## â¶ï¸ Quickstart ### Install ```cmd pip install ydata-
-profiling ``` or ```cmd conda install -c conda-forge ydata-profiling ``` ###
-Start profiling Start by loading your pandas `DataFrame` as you normally would,
-e.g. by using: ```python import numpy as np import pandas as pd from
-ydata_profiling import ProfileReport df = pd.DataFrame(np.random.rand(100, 5),
-columns=["a", "b", "c", "d", "e"]) ``` To generate the standard profiling
-report, merely run: ```python profile = ProfileReport(df, title="Profiling
-Report") ``` ## Key features - **Type inference**: automatic detection of
-columns' data types (*Categorical*, *Numerical*, *Date*, etc.) - **Warnings**:
-A summary of the problems/challenges in the data that you might need to work on
-(*missing data*, *inaccuracies*, *skewness*, etc.) - **Univariate analysis**:
-including descriptive statistics (mean, median, mode, etc) and informative
-visualizations such as distribution histograms - **Multivariate analysis**:
-including correlations, a detailed analysis of missing data, duplicate rows,
-and visual support for variables pairwise interaction - **Time-Series**:
-including different statistical information relative to time dependent data
-such as auto-correlation and seasonality, along ACF and PACF plots. - **Text
-analysis**: most common categories (uppercase, lowercase, separator), scripts
-(Latin, Cyrillic) and blocks (ASCII, Cyrilic) - **File and Image analysis**:
-file sizes, creation dates, dimensions, indication of truncated images and
-existence of EXIF metadata - **Compare datasets**: one-line solution to enable
-a fast and complete report on the comparison of datasets - **Flexible output
-formats**: all analysis can be exported to an HTML report that can be easily
-shared with different parties, as JSON for an easy integration in automated
-systems and as a widget in a Jupyter Notebook. The report contains three
-additional sections: - **Overview**: mostly global details about the dataset
-(number of records, number of variables, overall missigness and duplicates,
-memory footprint) - **Alerts**: a comprehensive and automatic list of potential
-data quality issues (high correlation, skewness, uniformity, zeros, missing
-values, constant values, between others) - **Reproduction**: technical details
-about the analysis (time, version and configuration) ### ð Latest features -
-Want to scale? Check the latest release with â­â¡[Spark support](https://
-ydata-profiling.ydata.ai/docs/master/pages/integrations/pypspark.html)! -
-Looking for how you can do an EDA for Time-Series ð ? Check [this blogpost]
-(https://towardsdatascience.com/how-to-do-an-eda-for-time-series-cbb92b3b1913).
-- You want to compare 2 datasets and get a report? Check [this blogpost](https:
-//medium.com/towards-artificial-intelligence/how-to-compare-2-dataset-with-
+and **text**. > **Looking for a scalable solution that can fully integrate with
+your database systems?**
+> Leverage YData Fabric Data Catalog to connect to different databases and
+storages (Oracle, snowflake, PostGreSQL, GCS, S3, etc.) and leverage an
+interactive and guided profiling experience in Fabric. Check out the [Community
+Version](https://ydata.ai/ydata-fabric-free-trial). ## â¶ï¸ Quickstart ###
+Install ```cmd pip install ydata-profiling ``` or ```cmd conda install -
+c conda-forge ydata-profiling ``` ### Start profiling Start by loading your
+pandas `DataFrame` as you normally would, e.g. by using: ```python import numpy
+as np import pandas as pd from ydata_profiling import ProfileReport df =
+pd.DataFrame(np.random.rand(100, 5), columns=["a", "b", "c", "d", "e"]) ``` To
+generate the standard profiling report, merely run: ```python profile =
+ProfileReport(df, title="Profiling Report") ``` ## Key features - **Type
+inference**: automatic detection of columns' data types (*Categorical*,
+*Numerical*, *Date*, etc.) - **Warnings**: A summary of the problems/challenges
+in the data that you might need to work on (*missing data*, *inaccuracies*,
+*skewness*, etc.) - **Univariate analysis**: including descriptive statistics
+(mean, median, mode, etc) and informative visualizations such as distribution
+histograms - **Multivariate analysis**: including correlations, a detailed
+analysis of missing data, duplicate rows, and visual support for variables
+pairwise interaction - **Time-Series**: including different statistical
+information relative to time dependent data such as auto-correlation and
+seasonality, along ACF and PACF plots. - **Text analysis**: most common
+categories (uppercase, lowercase, separator), scripts (Latin, Cyrillic) and
+blocks (ASCII, Cyrilic) - **File and Image analysis**: file sizes, creation
+dates, dimensions, indication of truncated images and existence of EXIF
+metadata - **Compare datasets**: one-line solution to enable a fast and
+complete report on the comparison of datasets - **Flexible output formats**:
+all analysis can be exported to an HTML report that can be easily shared with
+different parties, as JSON for an easy integration in automated systems and as
+a widget in a Jupyter Notebook. The report contains three additional sections:
+- **Overview**: mostly global details about the dataset (number of records,
+number of variables, overall missigness and duplicates, memory footprint) -
+**Alerts**: a comprehensive and automatic list of potential data quality issues
+(high correlation, skewness, uniformity, zeros, missing values, constant
+values, between others) - **Reproduction**: technical details about the
+analysis (time, version and configuration) ### ð Latest features - Want to
+scale? Check the latest release with â­â¡[Spark support](https://ydata-
+profiling.ydata.ai/docs/master/pages/integrations/pypspark.html)! - Looking for
+how you can do an EDA for Time-Series ð ? Check [this blogpost](https://
+towardsdatascience.com/how-to-do-an-eda-for-time-series-cbb92b3b1913). - You
+want to compare 2 datasets and get a report? Check [this blogpost](https://
+medium.com/towards-artificial-intelligence/how-to-compare-2-dataset-with-
 pandas-profiling-2ae3a9d7695e) ### â¡ Spark Spark support has been released,
 but we are always looking for an extra pair of hands ð. [Check current work
 in progress!](https://github.com/ydataai/ydata-profiling/projects/3). ## ð
 Use cases YData-profiling can be used to deliver a variety of different use-
 case. The documentation includes guides, tips and tricks for tackling them: |
 Use case | Description | |----------|------------------------------------------
 ---------------------------------------------------| | [Comparing datasets]
@@ -79,42 +85,47 @@
 master/pages/use_cases/sensitive_data.html ) | Generating reports which are
 mindful about sensitive data in the input dataset | | [Dataset metadata and
 data dictionaries](https://ydata-profiling.ydata.ai/docs/master/pages/
 use_cases/metadata.html) | Complementing the report with dataset details and
 column-specific data dictionaries | | [Customizing the report's appearance]
 (https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/
 custom_report_appearance.html ) | Changing the appearance of the report's page
-and of the contained visualizations | ### Using inside Jupyter Notebooks There
-are two interfaces to consume the report inside a Jupyter notebook: through
-widgets and through an embedded HTML report. [Notebook Widgets] The above is
-achieved by simply displaying the report as a set of widgets. In a Jupyter
-Notebook, run: ```python profile.to_widgets() ``` The HTML report can be
-directly embedded in a cell in a similar fashion: ```python
-profile.to_notebook_iframe() ``` [HTML] ### Exporting the report to a file To
-generate a HTML report file, save the `ProfileReport` to an object and use the
-`to_file()` function: ```python profile.to_file("your_report.html") ```
-Alternatively, the report's data can be obtained as a JSON file: ```python # As
-a JSON string json_data = profile.to_json() # As a file profile.to_file
-("your_report.json") ``` ### Using in the command line For standard formatted
-CSV files (which can be read directly by pandas without additional settings),
-the `pandas_profiling` executable can be used in the command line. The example
-below generates a report named _Example Profiling Report_, using a
-configuration file called `default.yaml`, in the file `report.html` by
-processing a `data.csv` dataset. ```sh pandas_profiling --title "Example
-Profiling Report" --config_file default.yaml data.csv report.html ```
-Additional details on the CLI are available [on the documentation](https://
-ydata-profiling.ydata.ai/docs/master/pages/getting_started/
-quickstart.html#command-line-usage). ## ð Examples The following example
-reports showcase the potentialities of the package across a wide range of
-dataset and data types: * [Census Income](https://ydata-profiling.ydata.ai/
-examples/master/census/census_report.html) (US Adult Census data relating
-income with other demographic properties) * [NASA Meteorites](https://ydata-
-profiling.ydata.ai/examples/master/meteorites/meteorites_report.html)
-(comprehensive set of meteorite landing - object properties and locations) [!
-[Open In Colab](https://camo.githubusercontent.com/
+and of the contained visualizations | | [Profiling Databases](https://ydata-
+profiling.ydata.ai/docs/master/pages/use_cases/profiling_databases.html) | For
+a seamless profiling experience in your organization's databases, check [Fabric
+Data Catalog](https://ydata.ai/products/data_catalog), which allows to consume
+data from different types of storages such as RDBMs (Azure SQL, PostGreSQL,
+Oracle, etc.) and object storages (Google Cloud Storage, AWS S3, Snowflake,
+etc.), among others. | ### Using inside Jupyter Notebooks There are two
+interfaces to consume the report inside a Jupyter notebook: through widgets and
+through an embedded HTML report. [Notebook Widgets] The above is achieved by
+simply displaying the report as a set of widgets. In a Jupyter Notebook, run:
+```python profile.to_widgets() ``` The HTML report can be directly embedded in
+a cell in a similar fashion: ```python profile.to_notebook_iframe() ``` [HTML]
+### Exporting the report to a file To generate a HTML report file, save the
+`ProfileReport` to an object and use the `to_file()` function: ```python
+profile.to_file("your_report.html") ``` Alternatively, the report's data can be
+obtained as a JSON file: ```python # As a JSON string json_data =
+profile.to_json() # As a file profile.to_file("your_report.json") ``` ### Using
+in the command line For standard formatted CSV files (which can be read
+directly by pandas without additional settings), the `ydata_profiling`
+executable can be used in the command line. The example below generates a
+report named *Example Profiling Report*, using a configuration file called
+`default.yaml`, in the file `report.html` by processing a `data.csv` dataset.
+```sh ydata_profiling --title "Example Profiling Report" --config_file
+default.yaml data.csv report.html ``` Additional details on the CLI are
+available [on the documentation](https://ydata-profiling.ydata.ai/docs/master/
+pages/getting_started/quickstart.html#command-line-usage). ## ð Examples The
+following example reports showcase the potentialities of the package across a
+wide range of dataset and data types: * [Census Income](https://ydata-
+profiling.ydata.ai/examples/master/census/census_report.html) (US Adult Census
+data relating income with other demographic properties) * [NASA Meteorites]
+(https://ydata-profiling.ydata.ai/examples/master/meteorites/
+meteorites_report.html) (comprehensive set of meteorite landing - object
+properties and locations) [![Open In Colab](https://camo.githubusercontent.com/
 52feade06f2fecbf006889a904d221e6a730c194/
 68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)]
 (https://colab.research.google.com/github/ydataai/pandas-profiling/blob/master/
 examples/meteorites/meteorites_cloud.ipynb) [![Binder](https://
 camo.githubusercontent.com/483bae47a175c24dfbfc57390edd8b6982ac5fb3/
 68747470733a2f2f6d7962696e6465722e6f72672f62616467655f6c6f676f2e737667)](https:
 //mybinder.org/v2/gh/ydataai/pandas-profiling/
@@ -181,15 +192,15 @@
 github.com/ydataai/pandas-profiling/blob/master/requirements.txt) | Package
 requirements| | [requirements-dev.txt](https://github.com/ydataai/pandas-
 profiling/blob/master/requirements-dev.txt) | Requirements for development| |
 [requirements-test.txt](https://github.com/ydataai/pandas-profiling/blob/
 master/requirements-test.txt) | Requirements for testing| | [setup.py](https://
 github.com/ydataai/pandas-profiling/blob/master/setup.py) | Requirements for
 widgets etc. | ## ð Integrations To maximize its usefulness in real world
-contexts, `pandas-profiling` has a set of implicit and explicit integrations
+contexts, `ydata-profiling` has a set of implicit and explicit integrations
 with a variety of other actors in the Data Science ecosystem: | Integration
 type | Description | |---|---| | [Other DataFrame libraries](https://ydata-
 profiling.ydata.ai/docs/master/pages/integrations/
 other_dataframe_libraries.html) | How to compute the profiling of data stored
 in libraries other than pandas | | [Great Expectations](https://ydata-
 profiling.ydata.ai/docs/master/pages/integrations/great_expectations.html) |
 Generating [Great Expectations](https://greatexpectations.io) expectations
@@ -197,34 +208,35 @@
 ydata-profiling.ydata.ai/docs/master/pages/integrations/data_apps.html) |
 Embedding profiling reports in [Streamlit](http://streamlit.io), [Dash](http://
 dash.plotly.com) or [Panel](https://panel.holoviz.org) applications | |
 [Pipelines](https://ydata-profiling.ydata.ai/docs/master/pages/integrations/
 pipelines.html) | Integration with DAG workflow execution tools like [Airflow]
 (https://airflow.apache.org) or [Kedro](https://kedro.org) | | [Cloud services]
 (https://ydata-profiling.ydata.ai/docs/master/pages/integrations/
-cloud_services.html) | Using `pandas-profiling` in hosted computation services
+cloud_services.html) | Using `ydata-profiling` in hosted computation services
 like [Lambda](https://lambdalabs.com), [Google Cloud](https://github.com/
 GoogleCloudPlatform/analytics-componentized-patterns/blob/master/retail/
 propensity-model/bqml/bqml_kfp_retail_propensity_to_purchase.ipynb) or [Kaggle]
 (https://www.kaggle.com/code) | | [IDEs](https://ydata-profiling.ydata.ai/docs/
-master/pages/integrations/ides.html) | Using `pandas-profiling` directly from
+master/pages/integrations/ides.html) | Using `ydata-profiling` directly from
 integrated development environments such as [PyCharm](https://
 www.jetbrains.com/pycharm/) | ## ð Support Need help? Want to share a
 perspective? Report a bug? Ideas for collaborations? Reach out via the
 following channels: - [Stack Overflow](https://stackoverflow.com/questions/
 tagged/pandas-profiling+or+ydata-profiling): ideal for asking questions on how
 to use the package - [GitHub Issues](https://github.com/ydataai/ydata-
 profiling/issues): bugs, proposals for changes, feature requests - [Discord]
 (https://tiny.ydata.ai/dcai-ydata-profiling): ideal for projects discussions,
-ask questions, collaborations, general chat - [Email](mailto:
-developers@ydata.ai): project collaborations or sponsoring > â Before
-reporting an issue on GitHub, check out [Common Issues](https://ydata-
-profiling.ydata.ai/docs/master/pages/support_contrib/common_issues.html). ##
-ð¤ð½ Contributing Learn how to get involved in the [Contribution Guide]
-(https://ydata-profiling.ydata.ai/docs/master/pages/support_contrib/
+ask questions, collaborations, general chat > **Need Help?**
+> Get your questions answered with a product owner by [booking a Pawsome chat]
+(https://meetings.hubspot.com/fabiana-clemente)! ð¼ > â Before reporting an
+issue on GitHub, check out [Common Issues](https://ydata-profiling.ydata.ai/
+docs/master/pages/support_contrib/common_issues.html). ## ð¤ð½ Contributing
+Learn how to get involved in the [Contribution Guide](https://ydata-
+profiling.ydata.ai/docs/master/pages/support_contrib/
 contribution_guidelines.html). A low-threshold place to ask questions or start
 contributing is the [Data Centric AI Community's Discord](https://
 tiny.ydata.ai/dcai-ydata-profiling). A big thank you to all our amazing
 contributors! [https://contrib.rocks/image?repo=ydataai/ydata-profiling]
 Contributors wall made with [contrib.rocks](https://contrib.rocks). Keywords:
 pandas data-science data-analysis python jupyter ipython Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable Classifier: Topic ::
@@ -233,9 +245,10 @@
 Independent Classifier: Intended Audience :: Science/Research Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Financial and
 Insurance Industry Classifier: Intended Audience :: Healthcare Industry
 Classifier: Topic :: Scientific/Engineering Classifier: Framework :: IPython
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Requires-Python: >=3.7, <3.12 Description-Content-
-Type: text/markdown Provides-Extra: notebook Provides-Extra: unicode
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7, <3.12 Description-Content-Type: text/markdown Provides-
+Extra: notebook Provides-Extra: unicode
```

### Comparing `ydata-profiling-4.3.2/src/ydata_profiling.egg-info/SOURCES.txt` & `ydata-profiling-4.4.0/src/ydata_profiling.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 src/ydata_profiling/model/missing.py
 src/ydata_profiling/model/pairwise.py
 src/ydata_profiling/model/sample.py
 src/ydata_profiling/model/summarizer.py
 src/ydata_profiling/model/summary.py
 src/ydata_profiling/model/summary_algorithms.py
 src/ydata_profiling/model/table.py
+src/ydata_profiling/model/timeseries_index.py
 src/ydata_profiling/model/typeset.py
 src/ydata_profiling/model/typeset_relations.py
 src/ydata_profiling/model/pandas/__init__.py
 src/ydata_profiling/model/pandas/correlations_pandas.py
 src/ydata_profiling/model/pandas/dataframe_pandas.py
 src/ydata_profiling/model/pandas/describe_boolean_pandas.py
 src/ydata_profiling/model/pandas/describe_categorical_pandas.py
@@ -65,14 +66,15 @@
 src/ydata_profiling/model/pandas/discretize_pandas.py
 src/ydata_profiling/model/pandas/duplicates_pandas.py
 src/ydata_profiling/model/pandas/imbalance_pandas.py
 src/ydata_profiling/model/pandas/missing_pandas.py
 src/ydata_profiling/model/pandas/sample_pandas.py
 src/ydata_profiling/model/pandas/summary_pandas.py
 src/ydata_profiling/model/pandas/table_pandas.py
+src/ydata_profiling/model/pandas/timeseries_index_pandas.py
 src/ydata_profiling/model/pandas/utils_pandas.py
 src/ydata_profiling/model/spark/__init__.py
 src/ydata_profiling/model/spark/correlations_spark.py
 src/ydata_profiling/model/spark/dataframe_spark.py
 src/ydata_profiling/model/spark/describe_boolean_spark.py
 src/ydata_profiling/model/spark/describe_categorical_spark.py
 src/ydata_profiling/model/spark/describe_counts_spark.py
@@ -82,14 +84,15 @@
 src/ydata_profiling/model/spark/describe_supported_spark.py
 src/ydata_profiling/model/spark/describe_text_spark.py
 src/ydata_profiling/model/spark/duplicates_spark.py
 src/ydata_profiling/model/spark/missing_spark.py
 src/ydata_profiling/model/spark/sample_spark.py
 src/ydata_profiling/model/spark/summary_spark.py
 src/ydata_profiling/model/spark/table_spark.py
+src/ydata_profiling/model/spark/timeseries_index_spark.py
 src/ydata_profiling/report/__init__.py
 src/ydata_profiling/report/formatters.py
 src/ydata_profiling/report/presentation/__init__.py
 src/ydata_profiling/report/presentation/frequency_table_utils.py
 src/ydata_profiling/report/presentation/core/__init__.py
 src/ydata_profiling/report/presentation/core/alerts.py
 src/ydata_profiling/report/presentation/core/collapse.py
```

