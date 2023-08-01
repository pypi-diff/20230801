# Comparing `tmp/openlineage-airflow-0.9.0.tar.gz` & `tmp/openlineage-airflow-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openlineage-airflow-0.9.0.tar", last modified: Fri Jun  3 23:03:16 2022, max compression
+gzip compressed data, was "openlineage-airflow-1.0.0.tar", last modified: Tue Aug  1 19:51:58 2023, max compression
```

## Comparing `openlineage-airflow-0.9.0.tar` & `openlineage-airflow-1.0.0.tar`

### file list

```diff
@@ -1,39 +1,59 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11740 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9352 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage/airflow/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      669 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7317 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8844 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/dag.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      320 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2128 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1847 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/bash_extractor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3808 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/bigquery_extractor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2731 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/dbapi_utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      596 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/example_dag.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3329 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/extractors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1539 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/great_expectations_extractor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3256 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/manager.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4319 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/mysql_extractor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4282 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/postgres_extractor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2522 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/python_extractor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5621 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/snowflake_extractor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1415 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/facets.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6374 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/listener.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2170 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/macros.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      874 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/plugin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8648 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage/lineage_backend/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3428 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/lineage_backend/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage_airflow.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11740 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage_airflow.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1245 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage_airflow.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage_airflow.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       84 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage_airflow.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage_airflow.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      732 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage_airflow.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage_airflow.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      554 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2023 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:51:58.088492 openlineage-airflow-1.0.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12454 2023-08-01 19:51:58.088492 openlineage-airflow-1.0.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12173 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:51:58.080492 openlineage-airflow-1.0.0/openlineage/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:51:58.080492 openlineage-airflow-1.0.0/openlineage/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      723 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11168 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/adapter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:51:58.084492 openlineage-airflow-1.0.0/openlineage/airflow/extractors/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      381 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5404 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/athena_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4491 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2037 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/bash_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3910 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/bigquery_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1273 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/converters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5259 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/dbapi_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10165 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/dbt_cloud_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      697 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/example_dag.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8344 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/extractors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2689 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/ftp_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1419 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/gcs_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1470 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/great_expectations_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4724 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/manager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1471 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/mysql_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1762 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/postgres_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2590 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/python_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3098 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/redshift_data_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2503 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/redshift_sql_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2105 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/s3_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5794 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/sagemaker_extractors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4288 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/sftp_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3047 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/snowflake_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7187 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/sql_check_extractors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      444 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/sql_execute_query.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10715 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/sql_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1486 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/extractors/trino_extractor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2752 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/facets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8042 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/listener.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1843 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/macros.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1313 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/plugin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16069 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/airflow/version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:51:58.084492 openlineage-airflow-1.0.0/openlineage/lineage_backend/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3848 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/openlineage/lineage_backend/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:51:58.088492 openlineage-airflow-1.0.0/openlineage_airflow.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12454 2023-08-01 19:51:58.000000 openlineage-airflow-1.0.0/openlineage_airflow.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2081 2023-08-01 19:51:58.000000 openlineage-airflow-1.0.0/openlineage_airflow.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-01 19:51:58.000000 openlineage-airflow-1.0.0/openlineage_airflow.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-08-01 19:51:58.000000 openlineage-airflow-1.0.0/openlineage_airflow.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-01 19:51:58.000000 openlineage-airflow-1.0.0/openlineage_airflow.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      848 2023-08-01 19:51:58.000000 openlineage-airflow-1.0.0/openlineage_airflow.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-08-01 19:51:58.000000 openlineage-airflow-1.0.0/openlineage_airflow.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      214 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1941 2023-08-01 19:51:58.088492 openlineage-airflow-1.0.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2267 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:51:58.088492 openlineage-airflow-1.0.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3245 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/tests/test_listener.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      981 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/tests/test_location.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1599 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/tests/test_openlineage_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6774 2023-08-01 19:51:48.000000 openlineage-airflow-1.0.0/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `openlineage-airflow-0.9.0/PKG-INFO` & `openlineage-airflow-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,266 +1,292 @@
 Metadata-Version: 2.1
 Name: openlineage-airflow
-Version: 0.9.0
+Version: 1.0.0
 Summary: OpenLineage integration with Airflow
-Home-page: UNKNOWN
 Author: OpenLineage
-License: UNKNOWN
-Description: <!-- SPDX-License-Identifier: Apache-2.0 -->
-        
-        # OpenLineage Airflow Integration
-        
-        A library that integrates [Airflow `DAGs`]() with [OpenLineage](https://openlineage.io) for automatic metadata collection.
-        
-        ## Features
-        
-        **Metadata**
-        
-        * Task lifecycle
-        * Task parameters
-        * Task runs linked to **versioned** code
-        * Task inputs / outputs
-        
-        **Lineage**
-        
-        * Track inter-DAG dependencies
-        
-        **Built-in**
-        
-        * SQL parser
-        * Link to code builder (ex: **GitHub**)
-        * Metadata extractors
-        
-        ## Requirements
-        
-        - [Python 3.7](https://www.python.org/downloads)
-        - [Airflow 1.10.12+](https://pypi.org/project/apache-airflow)
-        - (experimental) [Airflow 2.1+](https://pypi.org/project/apache-airflow)
-        
-        ## Installation
-        
-        ```bash
-        $ pip3 install openlineage-airflow
-        ```
-        
-        > **Note:** You can also add `openlineage-airflow` to your `requirements.txt` for Airflow.
-        
-        To install from source, run:
-        
-        ```bash
-        $ python3 setup.py install
-        ```
-        
-        ## Setup
-        
-        ### Airflow 2.3+
-        
-        Integration automatically registers itself for Airflow 2.3 if it's installed on Airflow worker's python.
-        This means you don't have to do anything besides configuring it, which is described in Configuration section.
-        
-        ### Airflow 2.1 - 2.2
-        
-        This method has limited support: 
-        it does not support tracking failed jobs, and job starts are registered only when job ends.
-        
-        Set your LineageBackend in your [airflow.cfg](https://airflow.apache.org/docs/apache-airflow/stable/howto/set-config.html) or via environmental variable `AIRFLOW__LINEAGE__BACKEND`
-        to 
-        ```
-        openlineage.lineage_backend.OpenLineageBackend
-        ```
-        
-        In contrast to integration via subclassing `DAG`, `LineageBackend` based approach collects all metadata 
-        for task on each task completion.
-        
-        OpenLineageBackend does not take into account manually configured inlets and outlets. 
-        
-        ### Airflow 1.10+
-        
-        To begin collecting Airflow DAG metadata with OpenLineage, use:
-        
-        ```diff
-        - from airflow import DAG
-        + from openlineage.airflow import DAG
-        ```
-        
-        When enabled, the library will:
-        
-        1. On DAG **start**, collect metadata for each task using an `Extractor` if it exists for given operator.
-        2. Collect task input / output metadata (`source`, `schema`, etc)
-        3. Collect task run-level metadata (execution time, state, parameters, etc)
-        4. On DAG **complete**, also mark the task as _complete_ in OpenLineage
-        
-        ## Configuration
-        
-        ### `HTTP` Backend Environment Variables
-        
-        `openlineage-airflow` uses OpenLineage client to push data to OpenLineage backend.
-        
-        OpenLineage client depends on environment variables:
-        
-        * `OPENLINEAGE_URL` - point to service which will consume OpenLineage events
-        * `OPENLINEAGE_API_KEY` - set if consumer of OpenLineage events requires `Bearer` authentication key
-        * `OPENLINEAGE_NAMESPACE` - set if you are using something other than the `default` namespace for job namespace.
-        * `OPENLINEAGE_AIRFLOW_DISABLE_SOURCE_CODE` - set to `True` if you don't want source code of callables provided to PythonOperator to be send in OpenLineage events
-        
-        For backwards compatibility, `openlineage-airflow` also support configuration via
-        `MARQUEZ_URL`, `MARQUEZ_NAMESPACE` and `MARQUEZ_API_KEY` variables.
-        
-        ```
-        MARQUEZ_URL=http://my_hosted_marquez.example.com:5000
-        MARQUEZ_NAMESPACE=my_special_ns
-        ```
-        
-        ### Extractors : Sending the correct data from your DAGs
-        
-        If you do nothing, OpenLineage backend will receive the `Job` and the `Run` from your DAGs, but,
-        unless you use few operators for which this integration provides extractor, input and output metadata will not be send.
-        
-        `openlineage-airflow` allows you to do more than that by building "Extractors". Extractor is object
-        suited to extract metadata from particular operator (or operators). 
-        
-        1. Name : The name of the task
-        2. Inputs : List of input datasets
-        3. Outputs : List of output datasets
-        4. Context : The Airflow context for the task
-        
-        #### Bundled Extractors
-        
-        `openlineage-airflow` provides extractors for
-        
-        * `PostgresOperator`
-        * `MySqlOperator`
-        * `BigQueryOperator`
-        * `SnowflakeOperator`
-        * `GreatExpectationsOperator`
-        * `PythonOperator`
-        
-        SQL Operators utilize SQL parser. There is experimental SQL parser, activated if you install [openlineage-sql](https://pypi.org/project/openlineage-sql) on your Airflow worker.
-        
-        #### Custom Extractors
-        
-        If your DAGs contain additional operators from which you want to extract lineage data, fear not - you can always
-        provide custom extractors. They should derive from `BaseExtractor`. 
-        
-        There are two ways to register them for use in `openlineage-airflow`. 
-        
-        First one, is to add them to `OPENLINEAGE_EXTRACTORS` environment variable, separated by comma `(;)` 
-        ```
-        OPENLINEAGE_EXTRACTORS=full.path.to.ExtractorClass;full.path.to.AnotherExtractorClass
-        ```
-        
-        Second one - working in Airflow 1.10.x only - is to register all additional operator-extractor pairings by 
-        providing `lineage_custom_extractors` argument in `openlineage.airflow.DAG`.
-        
-        #### Great Expectations
-        
-        Great Expectations integration works by providing OpenLineageValidationAction. You need to include it into your `action_list` in `great_expectations.yml`.
-        
-        The following example illustrates example change in default configuration: 
-        ```diff
-        validation_operators:
-          action_list_operator:
-            # To learn how to configure sending Slack notifications during evaluation
-            # (and other customizations), read: https://docs.greatexpectations.io/en/latest/autoapi/great_expectations/validation_operators/index.html#great_expectations.validation_operators.ActionListValidationOperator
-            class_name: ActionListValidationOperator
-            action_list:
-              - name: store_validation_result
-                action:
-                  class_name: StoreValidationResultAction
-              - name: store_evaluation_params
-                action:
-                  class_name: StoreEvaluationParametersAction
-              - name: update_data_docs
-                action:
-                  class_name: UpdateDataDocsAction
-        +     - name: openlineage
-        +       action:
-        +         class_name: OpenLineageValidationAction
-        +         module_name: openlineage.common.provider.great_expectations.action
-              # - name: send_slack_notification_on_validation_result
-              #   action:
-              #     class_name: SlackNotificationAction
-              #     # put the actual webhook URL in the uncommitted/config_variables.yml file
-              #     slack_webhook: ${validation_notification_slack_webhook}
-              #     notify_on: all # possible values: "all", "failure", "success"
-              #     renderer:
-              #       module_name: great_expectations.render.renderer.slack_renderer
-              #       class_name: SlackRenderer
-        ```
-        
-        If you're using `GreatExpectationsOperator`, you need to set `validation_operator_name` to operator that includes OpenLineageValidationAction.
-        Setting it in `great_expectations.yml` files isn't enough - the operator overrides it with default name if it's not provided.
-        
-        To see example of working configuration, you can see [DAG](https://github.com/OpenLineage/OpenLineage/blob/main/integration/airflow/tests/integration/airflow/dags/greatexpectations_dag.py) and [Great Expectations configuration](https://github.com/OpenLineage/OpenLineage/tree/main/integration/airflow/tests/integration/data/great_expectations) in integration tests.
-        
-        ## Triggering Child Jobs
-        Commonly, Airflow DAGs will trigger processes on remote systems, such as an Apache Spark or Apache
-        Beam job. Those systems may have their own OpenLineage integration and report their own
-        job runs and dataset inputs/outputs. To propagate the job hierarchy, tasks must send their own run
-        id so that the downstream process can report the [ParentRunFacet](https://github.com/OpenLineage/OpenLineage/blob/main/spec/OpenLineage.json#/definitions/ParentRunFacet)
-        with the proper run id.
-        
-        The `lineage_run_id` and `lineage_parent_id` macros exists to inject the run id or whole parent run information
-        of a given task into the arguments sent to a  remote processing job's Airflow operator. The macro requires the 
-        DAG run_id and the task to access the generated run id for that task. For example, a Spark job can be triggered
-        using the `DataProcPySparkOperator` with the correct parent run id using the following configuration:
-        
-        Airflow 1.10:
-        
-        ```python
-        t1 = DataProcPySparkOperator(
-            task_id=job_name,
-            #required pyspark configuration,
-            job_name=job_name,
-            dataproc_pyspark_properties={
-                'spark.driver.extraJavaOptions':
-                    f"-javaagent:{jar}={os.environ.get('OPENLINEAGE_URL')}/api/v1/namespaces/{os.getenv('OPENLINEAGE_NAMESPACE', 'default')}/jobs/{job_name}/runs/{{{{lineage_run_id(run_id, task)}}}}?api_key={os.environ.get('OPENLINEAGE_API_KEY')}"
-                dag=dag)
-        ```
-        
-        Airflow 2.0+:
-        
-        ```python
-        t1 = DataProcPySparkOperator(
-            task_id=job_name,
-            #required pyspark configuration,
-            job_name=job_name,
-            dataproc_pyspark_properties={
-                'spark.driver.extraJavaOptions':
-                    f"-javaagent:{jar}={os.environ.get('OPENLINEAGE_URL')}/api/v1/namespaces/{os.getenv('OPENLINEAGE_NAMESPACE', 'default')}/jobs/{job_name}/runs/{{{{macros.OpenLineagePlugin.lineage_run_id(run_id, task)}}}}?api_key={os.environ.get('OPENLINEAGE_API_KEY')}"
-                dag=dag)
-        ```
-        
-        ## Development
-        
-        To install all dependencies for _local_ development:
-        
-        ```bash
-        # Bash
-        $ pip3 install -e .[dev]
-        ```
-        ```zsh
-        # escape the brackets in zsh
-        $ pip3 install -e .\[dev\]
-        ```
-        
-        To run the entire test suite, you'll first want to initialize the Airflow database:
-        
-        ```bash
-        $ airflow initdb
-        ```
-        
-        Then, run the test suite with:
-        
-        ```bash
-        $ pytest
-        ```
-        
 Keywords: openlineage
-Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: sql
 Provides-Extra: tests
-Provides-Extra: airflow-1
-Provides-Extra: airflow-2
+Provides-Extra: airflow
 Provides-Extra: dev
+
+# OpenLineage Airflow Integration
+
+A library that integrates [Airflow `DAGs`]() with [OpenLineage](https://openlineage.io) for automatic metadata collection.
+
+## Features
+
+**Metadata**
+
+* Task lifecycle
+* Task parameters
+* Task runs linked to **versioned** code
+* Task inputs / outputs
+
+**Lineage**
+
+* Track inter-DAG dependencies
+
+**Built-in**
+
+* SQL parser
+* Link to code builder (ex: **GitHub**)
+* Metadata extractors
+
+## Requirements
+
+- [Python 3.8](https://www.python.org/downloads)
+- [Airflow 2.1+](https://pypi.org/project/apache-airflow)
+
+## Installation
+
+```bash
+$ pip3 install openlineage-airflow
+```
+
+> **Note:** You can also add `openlineage-airflow` to your `requirements.txt` for Airflow.
+
+To install from source, run:
+
+```bash
+$ python3 setup.py install
+```
+
+## Setup
+
+### Airflow 2.3+
+
+The integration automatically registers itself for Airflow 2.3 if it's installed on the Airflow worker's Python.
+This means you don't have to do anything besides configuring it, which is described in the Configuration section.
+
+### Airflow 2.1 - 2.2
+
+This method has limited support: it does not support tracking failed jobs, and job starts are registered only when a job ends.
+
+Set your LineageBackend in your [airflow.cfg](https://airflow.apache.org/docs/apache-airflow/stable/howto/set-config.html) or via environmental variable `AIRFLOW__LINEAGE__BACKEND` to 
+```
+openlineage.lineage_backend.OpenLineageBackend
+```
+
+In contrast to integration via subclassing a `DAG`, a `LineageBackend`-based approach collects all metadata 
+for a task on each task's completion.
+
+The OpenLineageBackend does not take into account manually configured inlets and outlets. 
+
+When enabled, the library will:
+
+1. On DAG **start**, collect metadata for each task using an `Extractor` if it exists for a given operator.
+2. Collect task input / output metadata (`source`, `schema`, etc.)
+3. Collect task run-level metadata (execution time, state, parameters, etc.)
+4. On DAG **complete**, also mark the task as _complete_ in OpenLineage
+
+## Configuration
+
+### `HTTP` Backend Environment Variables
+
+`openlineage-airflow` uses the OpenLineage client to push data to OpenLineage backend.
+
+The OpenLineage client depends on environment variables:
+
+* `OPENLINEAGE_URL` - point to the service that will consume OpenLineage events.
+* `OPENLINEAGE_API_KEY` - set if the consumer of OpenLineage events requires a `Bearer` authentication key.
+* `OPENLINEAGE_NAMESPACE` - set if you are using something other than the `default` namespace for the job namespace.
+* `OPENLINEAGE_AIRFLOW_DISABLE_SOURCE_CODE` - set to `False` if you want the source code of callables provided in the PythonOperator to be sent in OpenLineage events.
+
+For backwards compatibility, `openlineage-airflow` also supports configuration via
+`MARQUEZ_URL`, `MARQUEZ_NAMESPACE` and `MARQUEZ_API_KEY` variables.
+
+```
+MARQUEZ_URL=http://my_hosted_marquez.example.com:5000
+MARQUEZ_NAMESPACE=my_special_ns
+```
+
+### Extractors : Sending the correct data from your DAGs
+
+If you do nothing, the OpenLineage backend will receive the `Job` and the `Run` from your DAGs, but,
+unless you use one of the few operators for which this integration provides an extractor, input and output metadata will not be sent.
+
+`openlineage-airflow` allows you to do more than that by building "Extractors." An extractor is an object
+suited to extract metadata from a particular operator (or operators). 
+
+1. Name : The name of the task
+2. Inputs : A list of input datasets
+3. Outputs : A list of output datasets
+4. Context : The Airflow context for the task
+
+#### Bundled Extractors
+
+`openlineage-airflow` provides extractors for:
+
+* `PostgresOperator`
+* `MySqlOperator`
+* `AthenaOperator`
+* `BigQueryOperator`
+* `SnowflakeOperator`
+* `TrinoOperator`
+* `GreatExpectationsOperator`
+* `SFTPOperator`
+* `FTPFileTransmitOperator`
+* `PythonOperator`
+* `RedshiftDataOperator`, `RedshiftSQLOperator`
+* `SageMakerProcessingOperator`, `SageMakerProcessingOperatorAsync`
+* `SageMakerTrainingOperator`, `SageMakerTrainingOperatorAsync`
+* `SageMakerTransformOperator`, `SageMakerTransformOperatorAsync`
+* `S3CopyObjectExtractor`, `S3FileTransformExtractor`
+* `GCSToGCSOperator`
+* `DbtCloudRunJobOperator`
+
+SQL Operators utilize the SQL parser. There is an experimental SQL parser activated if you install [openlineage-sql](https://pypi.org/project/openlineage-sql) on your Airflow worker.
+
+
+#### Custom Extractors
+
+If your DAGs contain additional operators from which you want to extract lineage data, fear not - you can always
+provide custom extractors. They should derive from `BaseExtractor`. 
+
+There are two ways to register them for use in `openlineage-airflow`. 
+
+One way is to add them to the `OPENLINEAGE_EXTRACTORS` environment variable, separated by a semi-colon `(;)`. 
+```
+OPENLINEAGE_EXTRACTORS=full.path.to.ExtractorClass;full.path.to.AnotherExtractorClass
+```
+
+To ensure OpenLineage logging propagation to custom extractors you should use `self.log` instead of creating a logger yourself.
+
+#### Default Extractor
+
+When you own operators' code this is not neccessary to provide custom extractors. You can also use Default Extractor's capability.
+
+In order to do that you should define at least one of two methods in operator:
+
+* `get_openlineage_facets_on_start()`
+
+Extracts metadata on start of task.
+
+* `get_openlineage_facets_on_complete(task_instance: TaskInstance)`
+
+Extracts metadata on complete of task. This should accept `task_instance` argument, similar to `extract_on_complete` method in base extractors.
+
+If you don't define `get_openlineage_facets_on_complete` method it would fall back to `get_openlineage_facets_on_start`.
+
+
+#### Great Expectations
+
+The Great Expectations integration works by providing an OpenLineageValidationAction. You need to include it into your `action_list` in `great_expectations.yml`.
+
+The following example illustrates a way to change the default configuration: 
+```diff
+validation_operators:
+  action_list_operator:
+    # To learn how to configure sending Slack notifications during evaluation
+    # (and other customizations), read: https://docs.greatexpectations.io/en/latest/autoapi/great_expectations/validation_operators/index.html#great_expectations.validation_operators.ActionListValidationOperator
+    class_name: ActionListValidationOperator
+    action_list:
+      - name: store_validation_result
+        action:
+          class_name: StoreValidationResultAction
+      - name: store_evaluation_params
+        action:
+          class_name: StoreEvaluationParametersAction
+      - name: update_data_docs
+        action:
+          class_name: UpdateDataDocsAction
++     - name: openlineage
++       action:
++         class_name: OpenLineageValidationAction
++         module_name: openlineage.common.provider.great_expectations.action
+      # - name: send_slack_notification_on_validation_result
+      #   action:
+      #     class_name: SlackNotificationAction
+      #     # put the actual webhook URL in the uncommitted/config_variables.yml file
+      #     slack_webhook: ${validation_notification_slack_webhook}
+      #     notify_on: all # possible values: "all", "failure", "success"
+      #     renderer:
+      #       module_name: great_expectations.render.renderer.slack_renderer
+      #       class_name: SlackRenderer
+```
+
+If you're using `GreatExpectationsOperator`, you need to set `validation_operator_name` to an operator that includes OpenLineageValidationAction.
+Setting it in `great_expectations.yml` files isn't enough - the operator overrides it with the default name if a different one is not provided.
+
+To see an example of a working configuration, see [DAG](https://github.com/OpenLineage/OpenLineage/blob/main/integration/airflow/tests/integration/airflow/dags/greatexpectations_dag.py) and [Great Expectations configuration](https://github.com/OpenLineage/OpenLineage/tree/main/integration/airflow/tests/integration/data/great_expectations) in the integration tests.
+
+### Logging
+In addition to conventional logging approaches, the `openlineage-airflow` package provides an alternative way of configuring its logging behavior. By setting the `OPENLINEAGE_AIRFLOW_LOGGING` environment variable, you can establish the logging level for the `openlineage.airflow` and its child modules.
+
+## Triggering Child Jobs
+Commonly, Airflow DAGs will trigger processes on remote systems, such as an Apache Spark or Apache
+Beam job. Those systems may have their own OpenLineage integrations and report their own
+job runs and dataset inputs/outputs. To propagate the job hierarchy, tasks must send their own run
+ids so that the downstream process can report the [ParentRunFacet](https://github.com/OpenLineage/OpenLineage/blob/main/spec/OpenLineage.json#/definitions/ParentRunFacet)
+with the proper run id.
+
+The `lineage_run_id` and `lineage_parent_id` macros exists to inject the run id or whole parent run information
+of a given task into the arguments sent to a remote processing job's Airflow operator. The macro requires the 
+DAG `run_id` and the task to access the generated `run_id` for that task. For example, a Spark job can be triggered
+using the `DataProcPySparkOperator` with the correct parent `run_id` using the following configuration:
+
+```python
+t1 = DataProcPySparkOperator(
+    task_id=job_name,
+    #required pyspark configuration,
+    job_name=job_name,
+    dataproc_pyspark_properties={
+        'spark.driver.extraJavaOptions':
+            f"-javaagent:{jar}={os.environ.get('OPENLINEAGE_URL')}/api/v1/namespaces/{os.getenv('OPENLINEAGE_NAMESPACE', 'default')}/jobs/{job_name}/runs/{{{{macros.OpenLineagePlugin.lineage_run_id(task, task_instance)}}}}?api_key={os.environ.get('OPENLINEAGE_API_KEY')}"
+        dag=dag)
+```
+
+## Secrets redaction
+The integration uses Airflow SecretsMasker to hide secrets from produced metadata events. As not all fields in the metadata should be redacted, `RedactMixin` is used to pass information about which fields should be ignored by the process. 
+
+Typically, you should subclass `RedactMixin` and use the `_skip_redact` attribute as a list of names of fields to be skipped.
+
+However, all facets inheriting from `BaseFacet` should use the `_additional_skip_redact` attribute as an addition to the regular list (`['_producer', '_schemaURL']`).
+
+## Development
+
+To install all dependencies for _local_ development:
+
+The Airflow integration depends on `openlineage.sql`, `openlineage.common` and `openlineage.client.python`. You should install them first independently or try to install them with following command:
+
+```bash
+$ pip install -r dev-requirements.txt
+```
+
+There is also a bash script that can run an arbitrary Airflow image with an OpenLineage integration built from the current branch. Additionally, it mounts OpenLineage Python packages as Docker volumes. This enables you to change your code without the need to constantly rebuild Docker images to run tests.
+Run it as:
+```bash
+$ AIRFLOW_IMAGE=<airflow_image_with_tag> ./scripts/run-dev-airflow.sh [--help]
+```
+### Unit tests
+To run the entire unit test suite, use the below command:
+```bash
+$ tox
+```
+or choose one of the environments, e.g.:
+```bash
+$ tox -e py-airflow214
+```
+You can also skip using `tox` and run `pytest` on your own dev environment.
+### Integration tests
+The integration tests require the use of _docker compose_. There are scripts prepared to make build images and run tests easier.
+
+```bash
+$ AIRFLOW_IMAGE=<name-of-airflow-image> ./tests/integration/docker/up.sh
+```
+
+```bash
+$ AIRFLOW_IMAGE=apache/airflow:2.3.1-python3.8 ./tests/integration/docker/up.sh
+```
+
+When using `run-dev-airflow.sh`, you can add the `-i` flag or `--attach-integration` flag to run integration tests in a dev environment.
+This can be helpful when you need to run arbitrary integration tests during development. For example, the following command run in the integration container...
+```bash
+python -m pytest test_integration.py::test_integration[great_expectations_validation-requests/great_expectations.json]
+```
+...runs a single test which you can repeat after changes in code.
+
+----
+SPDX-License-Identifier: Apache-2.0\
+Copyright 2018-2023 contributors to the OpenLineage project
```

### Comparing `openlineage-airflow-0.9.0/README.md` & `openlineage-airflow-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-<!-- SPDX-License-Identifier: Apache-2.0 -->
-
 # OpenLineage Airflow Integration
 
 A library that integrates [Airflow `DAGs`]() with [OpenLineage](https://openlineage.io) for automatic metadata collection.
 
 ## Features
 
 **Metadata**
@@ -21,17 +19,16 @@
 
 * SQL parser
 * Link to code builder (ex: **GitHub**)
 * Metadata extractors
 
 ## Requirements
 
-- [Python 3.7](https://www.python.org/downloads)
-- [Airflow 1.10.12+](https://pypi.org/project/apache-airflow)
-- (experimental) [Airflow 2.1+](https://pypi.org/project/apache-airflow)
+- [Python 3.8](https://www.python.org/downloads)
+- [Airflow 2.1+](https://pypi.org/project/apache-airflow)
 
 ## Installation
 
 ```bash
 $ pip3 install openlineage-airflow
 ```
 
@@ -43,116 +40,133 @@
 $ python3 setup.py install
 ```
 
 ## Setup
 
 ### Airflow 2.3+
 
-Integration automatically registers itself for Airflow 2.3 if it's installed on Airflow worker's python.
-This means you don't have to do anything besides configuring it, which is described in Configuration section.
+The integration automatically registers itself for Airflow 2.3 if it's installed on the Airflow worker's Python.
+This means you don't have to do anything besides configuring it, which is described in the Configuration section.
 
 ### Airflow 2.1 - 2.2
 
-This method has limited support: 
-it does not support tracking failed jobs, and job starts are registered only when job ends.
+This method has limited support: it does not support tracking failed jobs, and job starts are registered only when a job ends.
 
-Set your LineageBackend in your [airflow.cfg](https://airflow.apache.org/docs/apache-airflow/stable/howto/set-config.html) or via environmental variable `AIRFLOW__LINEAGE__BACKEND`
-to 
+Set your LineageBackend in your [airflow.cfg](https://airflow.apache.org/docs/apache-airflow/stable/howto/set-config.html) or via environmental variable `AIRFLOW__LINEAGE__BACKEND` to 
 ```
 openlineage.lineage_backend.OpenLineageBackend
 ```
 
-In contrast to integration via subclassing `DAG`, `LineageBackend` based approach collects all metadata 
-for task on each task completion.
-
-OpenLineageBackend does not take into account manually configured inlets and outlets. 
-
-### Airflow 1.10+
+In contrast to integration via subclassing a `DAG`, a `LineageBackend`-based approach collects all metadata 
+for a task on each task's completion.
 
-To begin collecting Airflow DAG metadata with OpenLineage, use:
-
-```diff
-- from airflow import DAG
-+ from openlineage.airflow import DAG
-```
+The OpenLineageBackend does not take into account manually configured inlets and outlets. 
 
 When enabled, the library will:
 
-1. On DAG **start**, collect metadata for each task using an `Extractor` if it exists for given operator.
-2. Collect task input / output metadata (`source`, `schema`, etc)
-3. Collect task run-level metadata (execution time, state, parameters, etc)
+1. On DAG **start**, collect metadata for each task using an `Extractor` if it exists for a given operator.
+2. Collect task input / output metadata (`source`, `schema`, etc.)
+3. Collect task run-level metadata (execution time, state, parameters, etc.)
 4. On DAG **complete**, also mark the task as _complete_ in OpenLineage
 
 ## Configuration
 
 ### `HTTP` Backend Environment Variables
 
-`openlineage-airflow` uses OpenLineage client to push data to OpenLineage backend.
+`openlineage-airflow` uses the OpenLineage client to push data to OpenLineage backend.
 
-OpenLineage client depends on environment variables:
+The OpenLineage client depends on environment variables:
 
-* `OPENLINEAGE_URL` - point to service which will consume OpenLineage events
-* `OPENLINEAGE_API_KEY` - set if consumer of OpenLineage events requires `Bearer` authentication key
-* `OPENLINEAGE_NAMESPACE` - set if you are using something other than the `default` namespace for job namespace.
-* `OPENLINEAGE_AIRFLOW_DISABLE_SOURCE_CODE` - set to `True` if you don't want source code of callables provided to PythonOperator to be send in OpenLineage events
+* `OPENLINEAGE_URL` - point to the service that will consume OpenLineage events.
+* `OPENLINEAGE_API_KEY` - set if the consumer of OpenLineage events requires a `Bearer` authentication key.
+* `OPENLINEAGE_NAMESPACE` - set if you are using something other than the `default` namespace for the job namespace.
+* `OPENLINEAGE_AIRFLOW_DISABLE_SOURCE_CODE` - set to `False` if you want the source code of callables provided in the PythonOperator to be sent in OpenLineage events.
 
-For backwards compatibility, `openlineage-airflow` also support configuration via
+For backwards compatibility, `openlineage-airflow` also supports configuration via
 `MARQUEZ_URL`, `MARQUEZ_NAMESPACE` and `MARQUEZ_API_KEY` variables.
 
 ```
 MARQUEZ_URL=http://my_hosted_marquez.example.com:5000
 MARQUEZ_NAMESPACE=my_special_ns
 ```
 
 ### Extractors : Sending the correct data from your DAGs
 
-If you do nothing, OpenLineage backend will receive the `Job` and the `Run` from your DAGs, but,
-unless you use few operators for which this integration provides extractor, input and output metadata will not be send.
+If you do nothing, the OpenLineage backend will receive the `Job` and the `Run` from your DAGs, but,
+unless you use one of the few operators for which this integration provides an extractor, input and output metadata will not be sent.
 
-`openlineage-airflow` allows you to do more than that by building "Extractors". Extractor is object
-suited to extract metadata from particular operator (or operators). 
+`openlineage-airflow` allows you to do more than that by building "Extractors." An extractor is an object
+suited to extract metadata from a particular operator (or operators). 
 
 1. Name : The name of the task
-2. Inputs : List of input datasets
-3. Outputs : List of output datasets
+2. Inputs : A list of input datasets
+3. Outputs : A list of output datasets
 4. Context : The Airflow context for the task
 
 #### Bundled Extractors
 
-`openlineage-airflow` provides extractors for
+`openlineage-airflow` provides extractors for:
 
 * `PostgresOperator`
 * `MySqlOperator`
+* `AthenaOperator`
 * `BigQueryOperator`
 * `SnowflakeOperator`
+* `TrinoOperator`
 * `GreatExpectationsOperator`
+* `SFTPOperator`
+* `FTPFileTransmitOperator`
 * `PythonOperator`
+* `RedshiftDataOperator`, `RedshiftSQLOperator`
+* `SageMakerProcessingOperator`, `SageMakerProcessingOperatorAsync`
+* `SageMakerTrainingOperator`, `SageMakerTrainingOperatorAsync`
+* `SageMakerTransformOperator`, `SageMakerTransformOperatorAsync`
+* `S3CopyObjectExtractor`, `S3FileTransformExtractor`
+* `GCSToGCSOperator`
+* `DbtCloudRunJobOperator`
+
+SQL Operators utilize the SQL parser. There is an experimental SQL parser activated if you install [openlineage-sql](https://pypi.org/project/openlineage-sql) on your Airflow worker.
 
-SQL Operators utilize SQL parser. There is experimental SQL parser, activated if you install [openlineage-sql](https://pypi.org/project/openlineage-sql) on your Airflow worker.
 
 #### Custom Extractors
 
 If your DAGs contain additional operators from which you want to extract lineage data, fear not - you can always
 provide custom extractors. They should derive from `BaseExtractor`. 
 
 There are two ways to register them for use in `openlineage-airflow`. 
 
-First one, is to add them to `OPENLINEAGE_EXTRACTORS` environment variable, separated by comma `(;)` 
+One way is to add them to the `OPENLINEAGE_EXTRACTORS` environment variable, separated by a semi-colon `(;)`. 
 ```
 OPENLINEAGE_EXTRACTORS=full.path.to.ExtractorClass;full.path.to.AnotherExtractorClass
 ```
 
-Second one - working in Airflow 1.10.x only - is to register all additional operator-extractor pairings by 
-providing `lineage_custom_extractors` argument in `openlineage.airflow.DAG`.
+To ensure OpenLineage logging propagation to custom extractors you should use `self.log` instead of creating a logger yourself.
+
+#### Default Extractor
+
+When you own operators' code this is not neccessary to provide custom extractors. You can also use Default Extractor's capability.
+
+In order to do that you should define at least one of two methods in operator:
+
+* `get_openlineage_facets_on_start()`
+
+Extracts metadata on start of task.
+
+* `get_openlineage_facets_on_complete(task_instance: TaskInstance)`
+
+Extracts metadata on complete of task. This should accept `task_instance` argument, similar to `extract_on_complete` method in base extractors.
+
+If you don't define `get_openlineage_facets_on_complete` method it would fall back to `get_openlineage_facets_on_start`.
+
 
 #### Great Expectations
 
-Great Expectations integration works by providing OpenLineageValidationAction. You need to include it into your `action_list` in `great_expectations.yml`.
+The Great Expectations integration works by providing an OpenLineageValidationAction. You need to include it into your `action_list` in `great_expectations.yml`.
 
-The following example illustrates example change in default configuration: 
+The following example illustrates a way to change the default configuration: 
 ```diff
 validation_operators:
   action_list_operator:
     # To learn how to configure sending Slack notifications during evaluation
     # (and other customizations), read: https://docs.greatexpectations.io/en/latest/autoapi/great_expectations/validation_operators/index.html#great_expectations.validation_operators.ActionListValidationOperator
     class_name: ActionListValidationOperator
     action_list:
@@ -176,74 +190,91 @@
       #     slack_webhook: ${validation_notification_slack_webhook}
       #     notify_on: all # possible values: "all", "failure", "success"
       #     renderer:
       #       module_name: great_expectations.render.renderer.slack_renderer
       #       class_name: SlackRenderer
 ```
 
-If you're using `GreatExpectationsOperator`, you need to set `validation_operator_name` to operator that includes OpenLineageValidationAction.
-Setting it in `great_expectations.yml` files isn't enough - the operator overrides it with default name if it's not provided.
+If you're using `GreatExpectationsOperator`, you need to set `validation_operator_name` to an operator that includes OpenLineageValidationAction.
+Setting it in `great_expectations.yml` files isn't enough - the operator overrides it with the default name if a different one is not provided.
+
+To see an example of a working configuration, see [DAG](https://github.com/OpenLineage/OpenLineage/blob/main/integration/airflow/tests/integration/airflow/dags/greatexpectations_dag.py) and [Great Expectations configuration](https://github.com/OpenLineage/OpenLineage/tree/main/integration/airflow/tests/integration/data/great_expectations) in the integration tests.
 
-To see example of working configuration, you can see [DAG](https://github.com/OpenLineage/OpenLineage/blob/main/integration/airflow/tests/integration/airflow/dags/greatexpectations_dag.py) and [Great Expectations configuration](https://github.com/OpenLineage/OpenLineage/tree/main/integration/airflow/tests/integration/data/great_expectations) in integration tests.
+### Logging
+In addition to conventional logging approaches, the `openlineage-airflow` package provides an alternative way of configuring its logging behavior. By setting the `OPENLINEAGE_AIRFLOW_LOGGING` environment variable, you can establish the logging level for the `openlineage.airflow` and its child modules.
 
 ## Triggering Child Jobs
 Commonly, Airflow DAGs will trigger processes on remote systems, such as an Apache Spark or Apache
-Beam job. Those systems may have their own OpenLineage integration and report their own
+Beam job. Those systems may have their own OpenLineage integrations and report their own
 job runs and dataset inputs/outputs. To propagate the job hierarchy, tasks must send their own run
-id so that the downstream process can report the [ParentRunFacet](https://github.com/OpenLineage/OpenLineage/blob/main/spec/OpenLineage.json#/definitions/ParentRunFacet)
+ids so that the downstream process can report the [ParentRunFacet](https://github.com/OpenLineage/OpenLineage/blob/main/spec/OpenLineage.json#/definitions/ParentRunFacet)
 with the proper run id.
 
 The `lineage_run_id` and `lineage_parent_id` macros exists to inject the run id or whole parent run information
-of a given task into the arguments sent to a  remote processing job's Airflow operator. The macro requires the 
-DAG run_id and the task to access the generated run id for that task. For example, a Spark job can be triggered
-using the `DataProcPySparkOperator` with the correct parent run id using the following configuration:
-
-Airflow 1.10:
+of a given task into the arguments sent to a remote processing job's Airflow operator. The macro requires the 
+DAG `run_id` and the task to access the generated `run_id` for that task. For example, a Spark job can be triggered
+using the `DataProcPySparkOperator` with the correct parent `run_id` using the following configuration:
 
 ```python
 t1 = DataProcPySparkOperator(
     task_id=job_name,
     #required pyspark configuration,
     job_name=job_name,
     dataproc_pyspark_properties={
         'spark.driver.extraJavaOptions':
-            f"-javaagent:{jar}={os.environ.get('OPENLINEAGE_URL')}/api/v1/namespaces/{os.getenv('OPENLINEAGE_NAMESPACE', 'default')}/jobs/{job_name}/runs/{{{{lineage_run_id(run_id, task)}}}}?api_key={os.environ.get('OPENLINEAGE_API_KEY')}"
+            f"-javaagent:{jar}={os.environ.get('OPENLINEAGE_URL')}/api/v1/namespaces/{os.getenv('OPENLINEAGE_NAMESPACE', 'default')}/jobs/{job_name}/runs/{{{{macros.OpenLineagePlugin.lineage_run_id(task, task_instance)}}}}?api_key={os.environ.get('OPENLINEAGE_API_KEY')}"
         dag=dag)
 ```
 
-Airflow 2.0+:
+## Secrets redaction
+The integration uses Airflow SecretsMasker to hide secrets from produced metadata events. As not all fields in the metadata should be redacted, `RedactMixin` is used to pass information about which fields should be ignored by the process. 
 
-```python
-t1 = DataProcPySparkOperator(
-    task_id=job_name,
-    #required pyspark configuration,
-    job_name=job_name,
-    dataproc_pyspark_properties={
-        'spark.driver.extraJavaOptions':
-            f"-javaagent:{jar}={os.environ.get('OPENLINEAGE_URL')}/api/v1/namespaces/{os.getenv('OPENLINEAGE_NAMESPACE', 'default')}/jobs/{job_name}/runs/{{{{macros.OpenLineagePlugin.lineage_run_id(run_id, task)}}}}?api_key={os.environ.get('OPENLINEAGE_API_KEY')}"
-        dag=dag)
-```
+Typically, you should subclass `RedactMixin` and use the `_skip_redact` attribute as a list of names of fields to be skipped.
+
+However, all facets inheriting from `BaseFacet` should use the `_additional_skip_redact` attribute as an addition to the regular list (`['_producer', '_schemaURL']`).
 
 ## Development
 
 To install all dependencies for _local_ development:
 
+The Airflow integration depends on `openlineage.sql`, `openlineage.common` and `openlineage.client.python`. You should install them first independently or try to install them with following command:
+
 ```bash
-# Bash
-$ pip3 install -e .[dev]
-```
-```zsh
-# escape the brackets in zsh
-$ pip3 install -e .\[dev\]
+$ pip install -r dev-requirements.txt
 ```
 
-To run the entire test suite, you'll first want to initialize the Airflow database:
+There is also a bash script that can run an arbitrary Airflow image with an OpenLineage integration built from the current branch. Additionally, it mounts OpenLineage Python packages as Docker volumes. This enables you to change your code without the need to constantly rebuild Docker images to run tests.
+Run it as:
+```bash
+$ AIRFLOW_IMAGE=<airflow_image_with_tag> ./scripts/run-dev-airflow.sh [--help]
+```
+### Unit tests
+To run the entire unit test suite, use the below command:
+```bash
+$ tox
+```
+or choose one of the environments, e.g.:
+```bash
+$ tox -e py-airflow214
+```
+You can also skip using `tox` and run `pytest` on your own dev environment.
+### Integration tests
+The integration tests require the use of _docker compose_. There are scripts prepared to make build images and run tests easier.
 
 ```bash
-$ airflow initdb
+$ AIRFLOW_IMAGE=<name-of-airflow-image> ./tests/integration/docker/up.sh
 ```
 
-Then, run the test suite with:
+```bash
+$ AIRFLOW_IMAGE=apache/airflow:2.3.1-python3.8 ./tests/integration/docker/up.sh
+```
 
+When using `run-dev-airflow.sh`, you can add the `-i` flag or `--attach-integration` flag to run integration tests in a dev environment.
+This can be helpful when you need to run arbitrary integration tests during development. For example, the following command run in the integration container...
 ```bash
-$ pytest
+python -m pytest test_integration.py::test_integration[great_expectations_validation-requests/great_expectations.json]
 ```
+...runs a single test which you can repeat after changes in code.
+
+----
+SPDX-License-Identifier: Apache-2.0\
+Copyright 2018-2023 contributors to the OpenLineage project
```

### Comparing `openlineage-airflow-0.9.0/openlineage/airflow/__init__.py` & `openlineage-airflow-1.0.0/openlineage/airflow/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-# SPDX-License-Identifier: Apache-2.0.
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
 #
 # -*- coding: utf-8 -*-
+import logging
+
+from openlineage.airflow.version import __version__
 from pkg_resources import parse_version
+
 from airflow.version import version as AIRFLOW_VERSION
-import logging
 
 __author__ = """OpenLineage"""
-__version__ = "0.9.0"
 
-if parse_version(AIRFLOW_VERSION) < parse_version("2.0.0"):
-    from openlineage.airflow.dag import DAG
-    __all__ = ["DAG"]
+if parse_version(AIRFLOW_VERSION) < parse_version("2.0.0"):     # type: ignore
     logging.warning(
         f'''
-        OpenLineage supprot for Airflow version {AIRFLOW_VERSION}
-        is DEPRECATED, and will be desupported on September 30, 2022.
+        OpenLineage support for Airflow version {AIRFLOW_VERSION} is REMOVED.
         Please make sure to upgrade your Airflow version to minimum of 2.0.0
         in order to continue using OpenLineage.
         '''
     )
+
+from airflow.models import DAG
+
+__all__ = ["DAG", "__version__"]
```

### Comparing `openlineage-airflow-0.9.0/openlineage/airflow/dag.py` & `openlineage-airflow-1.0.0/openlineage/airflow/listener.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,234 +1,246 @@
-# SPDX-License-Identifier: Apache-2.0.
-import time
-import os
-import copy
-import uuid
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
 
-from airflow.models import DAG as AIRFLOW_DAG
-from airflow.utils.state import State
+import copy
+import datetime
+import logging
+import threading
+from concurrent.futures import Executor, ThreadPoolExecutor
+from typing import TYPE_CHECKING, Callable, Optional
 
-from openlineage.airflow.extractors.manager import ExtractorManager
-from openlineage.airflow.macros import lineage_run_id, lineage_parent_id
+from openlineage.airflow.adapter import OpenLineageAdapter
+from openlineage.airflow.extractors import ExtractorManager
 from openlineage.airflow.utils import (
-    JobIdMapping,
     DagUtils,
+    get_airflow_run_facet,
     get_custom_facets,
-    new_lineage_run_id, get_task_location, openlineage_job_name
+    get_dagrun_start_end,
+    get_job_name,
+    get_task_location,
+    getboolean,
+    is_airflow_version_enough,
 )
 
-from openlineage.airflow.adapter import OpenLineageAdapter, _DAG_DEFAULT_NAMESPACE
+from airflow.listeners import hookimpl
 
-_DAG_NAMESPACE = os.getenv('OPENLINEAGE_NAMESPACE', None)
-if not _DAG_NAMESPACE:
-    _DAG_NAMESPACE = os.getenv(
-        'MARQUEZ_NAMESPACE', _DAG_DEFAULT_NAMESPACE
-    )
+if TYPE_CHECKING:
+    from sqlalchemy.orm import Session
+
+    from airflow.models import BaseOperator, DagRun, TaskInstance
+
+
+class TaskHolder:
+    """Class that stores run data - run_id and task in-memory. This is needed because Airflow
+    does not always pass all runtime info to on_task_instance_success and
+    on_task_instance_failed that is needed to emit events. This is not a big problem since
+    we're only running on worker - in separate process that is always spawned (or forked) on
+    execution, just like old PHP runtime model.
+    """
+
+    def __init__(self):
+        self.run_data = {}
+
+    def set_task(self, task_instance: "TaskInstance"):
+        self.run_data[self._pk(task_instance)] = task_instance.task
+
+    def get_task(self, task_instance: "TaskInstance") -> Optional["BaseOperator"]:
+        return self.run_data.get(self._pk(task_instance))
+
+    @staticmethod
+    def _pk(ti: "TaskInstance"):
+        return ti.dag_id + ti.task_id + ti.run_id
+
+
+log = logging.getLogger(__name__)
+# TODO: move task instance runs to executor
+executor: Optional[Executor] = None
+
+
+def execute_in_thread(target: Callable, kwargs=None):
+    if kwargs is None:
+        kwargs = {}
+    thread = threading.Thread(target=target, kwargs=kwargs, daemon=True)
+    thread.start()
 
-_ADAPTER = OpenLineageAdapter()
+    # Join, but ignore checking if thread stopped. If it did, then we shoudn't do anything.
+    # This basically gives this thread 5 seconds to complete work, then it can be killed,
+    # as daemon=True. We don't want to deadlock Airflow if our code hangs.
+
+    # This will hang if this timeouts, and extractor is running non-daemon thread inside,
+    # since it will never be cleaned up. Ex. SnowflakeOperator
+    thread.join(timeout=10)
+
+
+task_holder = TaskHolder()
 extractor_manager = ExtractorManager()
+adapter = OpenLineageAdapter()
+
+
+def direct_execution():
+    return is_airflow_version_enough("2.6.0") \
+        or getboolean("OPENLINEAGE_AIRFLOW_ENABLE_DIRECT_EXECUTION", False)
+
+
+def execute(_callable):
+    try:
+        if direct_execution():
+            _callable()
+        else:
+            execute_in_thread(_callable)
+    except Exception:
+        # Make sure we're not failing task, even for things we think can't happen
+        log.exception("Failed to emit OpenLineage event due to exception")
+
+
+@hookimpl
+def on_task_instance_running(previous_state, task_instance: "TaskInstance", session: "Session"):
+    if not hasattr(task_instance, 'task'):
+        log.warning(
+            f"No task set for TI object task_id: {task_instance.task_id} - dag_id: {task_instance.dag_id} - run_id {task_instance.run_id}")  # noqa
+        return
+
+    log.debug("OpenLineage listener got notification about task instance start")
+    dagrun = task_instance.dag_run
+
+    def on_running():
+        nonlocal task_instance
+        ti = copy.deepcopy(task_instance)
+        ti.render_templates()
+
+        task = ti.task
+        dag = task.dag
+        task_holder.set_task(ti)
+        # that's a workaround to detect task running from deferred state
+        # we return here because Airflow 2.3 needs task from deferred state
+        if ti.next_method is not None:
+            return
+        parent_run_id = adapter.build_dag_run_id(task.dag.dag_id, dagrun.run_id)
 
+        task_uuid = OpenLineageAdapter.build_task_instance_run_id(
+            task.task_id, ti.execution_date, ti.try_number
+        )
 
-def has_lineage_backend_setup():
-    from airflow.configuration import conf
-    return conf.get("lineage", "backend") == "openlineage.lineage_backend.OpenLineageBackend"
-
-
-class DAG(AIRFLOW_DAG):
-    def __init__(self, *args, **kwargs):
-        self.log.info("openlineage-airflow dag starting")
-        macros = {}
-        if kwargs.__contains__("user_defined_macros"):
-            macros = kwargs["user_defined_macros"]
-        macros["lineage_run_id"] = lineage_run_id
-        macros["lineage_parent_id"] = lineage_parent_id
-        kwargs["user_defined_macros"] = macros
-        if kwargs.__contains__("lineage_custom_extractors"):
-            for operator, extractor in kwargs['lineage_custom_extractors'].items():
-                extractor_manager.add_extractor(operator, extractor)
-            del kwargs['lineage_custom_extractors']
-
-        self.has_lineage_backend = has_lineage_backend_setup()
-        super().__init__(*args, **kwargs)
-
-    def add_task(self, task):
-        super().add_task(task)
-
-    def create_dagrun(self, *args, **kwargs):
-        # run Airflow's create_dagrun() first
-        dagrun = super(DAG, self).create_dagrun(*args, **kwargs)
-
-        create_dag_start_ms = self._now_ms()
-        try:
-            self._register_dagrun(
-                dagrun,
-                kwargs.get('external_trigger', False),
-                DagUtils.get_execution_date(**kwargs)
-            )
-        except Exception as e:
-            self.log.error(
-                f'Failed to record metadata: {e} '
-                f'{self._timed_log_message(create_dag_start_ms)}',
-                exc_info=True)
-
-        return dagrun
-
-    # We make the assumption that when a DAG run is created, its
-    # tasks can be safely marked as started as well.
-    # Doing it other way would require to hook up to
-    # scheduler, where tasks are actually started
-    def _register_dagrun(self, dagrun, is_external_trigger: bool, execution_date: str):
-        self.log.debug(f"self.task_dict: {self.task_dict}")
-        parent_run_id = str(uuid.uuid3(uuid.NAMESPACE_URL, f'{self.dag_id}.{dagrun.run_id}'))
-        # Register each task in the DAG
-        for task_id, task in self.task_dict.items():
-            t = self._now_ms()
-            try:
-                task_metadata = extractor_manager.extract_metadata(dagrun, task)
-
-                job_name = openlineage_job_name(task.dag_id, task.task_id)
-                run_id = new_lineage_run_id(dagrun.run_id, task_id)
-
-                task_run_id = _ADAPTER.start_task(
-                    run_id,
-                    job_name,
-                    self.description,
-                    DagUtils.to_iso_8601(self._now_ms()),
-                    self.dag_id,
-                    parent_run_id,
-                    get_task_location(task),
-                    DagUtils.get_start_time(execution_date),
-                    DagUtils.get_end_time(execution_date, self.following_schedule(execution_date)),
-                    task_metadata,
-                    {**task_metadata.run_facets, **get_custom_facets(task, is_external_trigger)}
-                )
-
-                JobIdMapping.set(
-                    job_name,
-                    dagrun.run_id,
-                    task_run_id
-                )
-            except Exception as e:
-                self.log.error(
-                    f'Failed to record task {task_id}: {e} '
-                    f'{self._timed_log_message(t)}',
-                    exc_info=True)
-
-    def handle_callback(self, *args, **kwargs):
-        self.log.debug(f"handle_callback({args}, {kwargs})")
-
-        if has_lineage_backend_setup():
-            self.log.info("lineage backend is set up; dag is skipping COMPLETE events")
-            return super(DAG, self).handle_callback(*args, **kwargs)
-
-        try:
-            dagrun = args[0]
-            self.log.debug(f"handle_callback() dagrun : {dagrun}")
-            self._report_task_instances(
-                dagrun,
-                kwargs.get('session')
-            )
-        except Exception as e:
-            self.log.error(
-                f'Failed to record dagrun callback: {e} '
-                f'dag_id={self.dag_id}',
-                exc_info=True)
-
-        return super().handle_callback(*args)
-
-    def _report_task_instances(self, dagrun, session):
-        task_instances = dagrun.get_task_instances()
-        for task_instance in task_instances:
-            try:
-                self._report_task_instance(task_instance, dagrun, session)
-            except Exception as e:
-                self.log.error(
-                    f'Failed to record task instance: {e} '
-                    f'dag_id={self.dag_id}',
-                    exc_info=True)
-
-    def _report_task_instance(self, task_instance, dagrun, session):
-        task = self.get_task(task_instance.task_id)
-
-        # Note: task_run_id could be missing if it was removed from airflow
-        # or the job could not be registered.
-        task_run_id = JobIdMapping.pop(
-            self._openlineage_job_name_from_task_instance(task_instance), dagrun.run_id, session)
+        task_metadata = extractor_manager.extract_metadata(
+            dagrun, task, task_uuid=task_uuid
+        )
+
+        ti_start_time = ti.start_date if ti.start_date else datetime.datetime.now()
+        start, end = get_dagrun_start_end(dagrun=dagrun, dag=dag)
+
+        adapter.start_task(
+            run_id=task_uuid,
+            job_name=get_job_name(task),
+            job_description=dag.description,
+            event_time=DagUtils.get_start_time(ti_start_time),
+            parent_job_name=dag.dag_id,
+            parent_run_id=parent_run_id,
+            code_location=get_task_location(task),
+            nominal_start_time=DagUtils.get_start_time(start),
+            nominal_end_time=DagUtils.to_iso_8601(end),
+            owners=dag.owner.split(", "),
+            task=task_metadata,
+            run_facets={
+                **task_metadata.run_facets,
+                **get_custom_facets(
+                    dagrun, task, dagrun.external_trigger, ti
+                ),
+                **get_airflow_run_facet(dagrun, dag, ti, task, task_uuid)
+            }
+        )
+
+    execute(on_running)
+
+
+@hookimpl
+def on_task_instance_success(previous_state, task_instance: "TaskInstance", session):
+    log.debug("OpenLineage listener got notification about task instance success")
+    task = task_holder.get_task(task_instance) or task_instance.task
+
+    dagrun = task_instance.dag_run
+
+    task_uuid = OpenLineageAdapter.build_task_instance_run_id(
+        task.task_id, task_instance.execution_date, task_instance.try_number - 1
+    )
+
+    def on_success():
         task_metadata = extractor_manager.extract_metadata(
             dagrun, task, complete=True, task_instance=task_instance
         )
+        adapter.complete_task(
+            run_id=task_uuid,
+            job_name=get_job_name(task),
+            end_time=DagUtils.to_iso_8601(task_instance.end_date),
+            task=task_metadata,
+        )
 
-        job_name = openlineage_job_name(self.dag_id, task.task_id)
-        run_id = new_lineage_run_id(dagrun.run_id, task.task_id)
+    execute(on_success)
 
-        if not task_run_id:
-            parent_run_id = str(uuid.uuid3(uuid.NAMESPACE_URL, f'{self.dag_id}.{dagrun.run_id}'))
-            task_run_id = _ADAPTER.start_task(
-                run_id,
-                job_name,
-                self.description,
-                DagUtils.to_iso_8601(task_instance.start_date),
-                self.dag_id,
-                parent_run_id,
-                get_task_location(task),
-                DagUtils.to_iso_8601(task_instance.start_date),
-                DagUtils.to_iso_8601(task_instance.end_date),
-                task_metadata,
-                {**task_metadata.run_facets, **get_custom_facets(task, False)}
-            )
-
-            if not task_run_id:
-                self.log.warning('Could not emit lineage')
-
-        self.log.debug(f'Setting task state: {task_instance.state}'
-                       f' for {task_instance.task_id}')
-        if task_instance.state in {State.SUCCESS, State.SKIPPED}:
-            _ADAPTER.complete_task(
-                task_run_id,
-                job_name,
-                DagUtils.to_iso_8601(task_instance.end_date),
-                task_metadata
-            )
-        else:
-            _ADAPTER.fail_task(
-                task_run_id,
-                job_name,
-                DagUtils.to_iso_8601(task_instance.end_date),
-                task_metadata
-            )
-
-    def __deepcopy__(self, memo):
-        """
-        Override __deepcopy__ to avoid copying the _log property,
-        which causes failure when pickling
-
-        :param memo:
-        :return:
-        """
-        cls = self.__class__
-        result = cls.__new__(cls)
-        memo[id(self)] = result
-        for k, v in list(self.__dict__.items()):
-            if k not in ('user_defined_macros', 'user_defined_filters', 'params', '_log'):
-                try:
-                    deepcopy = copy.deepcopy(v, memo)
-                    setattr(result, k, deepcopy)
-                except TypeError as e:
-                    self.log.error(f"Unable to copy property{k}")
-                    raise RuntimeError(f"Unable to copy property{k}") from e
-
-        result.user_defined_macros = self.user_defined_macros
-        result.user_defined_filters = self.user_defined_filters
-        result.params = self.params
-        return result
-
-    def _timed_log_message(self, start_time):
-        return f'airflow_dag_id={self.dag_id} ' \
-            f'duration_ms={(self._now_ms() - start_time)}'
 
-    @staticmethod
-    def _openlineage_job_name_from_task_instance(task_instance):
-        return openlineage_job_name(task_instance.dag_id, task_instance.task_id)
+@hookimpl
+def on_task_instance_failed(previous_state, task_instance: "TaskInstance", session):
+    log.debug("OpenLineage listener got notification about task instance failure")
+    task = task_holder.get_task(task_instance) or task_instance.task
 
-    @staticmethod
-    def _now_ms():
-        return int(round(time.time() * 1000))
+    dagrun = task_instance.dag_run
+
+    task_uuid = OpenLineageAdapter.build_task_instance_run_id(
+        task.task_id, task_instance.execution_date, task_instance.try_number - 1
+    )
+
+    def on_failure():
+        task_metadata = extractor_manager.extract_metadata(
+            dagrun, task, complete=True, task_instance=task_instance
+        )
+
+        end_date = task_instance.end_date if task_instance.end_date else datetime.datetime.now()
+
+        adapter.fail_task(
+            run_id=task_uuid,
+            job_name=get_job_name(task),
+            end_time=DagUtils.to_iso_8601(end_date),
+            task=task_metadata,
+        )
+
+    execute(on_failure)
+
+
+@hookimpl
+def on_starting(component):
+    global executor
+    executor = ThreadPoolExecutor(max_workers=8, thread_name_prefix="openlineage_")
+
+
+@hookimpl
+def before_stopping(component):
+    executor.shutdown(wait=False)
+
+
+@hookimpl
+def on_dag_run_running(dag_run: "DagRun", msg: str):
+    if not executor:
+        log.error("Executor have not started before `on_dag_run_running`")
+        return
+    start, end = get_dagrun_start_end(dag_run, dag_run.dag)
+    executor.submit(
+        adapter.dag_started,
+        dag_run=dag_run,
+        msg=msg,
+        nominal_start_time=DagUtils.get_start_time(start),
+        nominal_end_time=DagUtils.to_iso_8601(end),
+    )
+
+
+@hookimpl
+def on_dag_run_success(dag_run: "DagRun", msg: str):
+    if not executor:
+        log.error("Executor have not started before `on_dag_run_success`")
+        return
+    executor.submit(adapter.dag_success, dag_run=dag_run, msg=msg)
+
+
+@hookimpl
+def on_dag_run_failed(dag_run: "DagRun", msg: str):
+    if not executor:
+        log.error("Executor have not started before `on_dag_run_failed`")
+        return
+    executor.submit(adapter.dag_failed, dag_run=dag_run, msg=msg)
```

### Comparing `openlineage-airflow-0.9.0/openlineage/airflow/extractors/bash_extractor.py` & `openlineage-airflow-1.0.0/openlineage/airflow/extractors/bash_extractor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
+
 import os
-from typing import Optional, List
+from typing import Dict, List, Optional
 
 from openlineage.airflow.extractors.base import BaseExtractor, TaskMetadata
 from openlineage.airflow.facets import UnknownOperatorAttributeRunFacet, UnknownOperatorInstance
 from openlineage.client.facet import SourceCodeJobFacet
 
 
 class BashExtractor(BaseExtractor):
@@ -13,28 +16,31 @@
     datasets.
     """
     @classmethod
     def get_operator_classnames(cls) -> List[str]:
         return ["BashOperator"]
 
     def extract(self) -> Optional[TaskMetadata]:
-        if os.environ.get(
-            "OPENLINEAGE_AIRFLOW_DISABLE_SOURCE_CODE", "False"
-        ).lower() in ('true', '1', 't'):
-            return None
-
-        return TaskMetadata(
-            name=f"{self.operator.dag_id}.{self.operator.task_id}",
-            job_facets={
+        collect_source = os.environ.get(
+            "OPENLINEAGE_AIRFLOW_DISABLE_SOURCE_CODE", "True"
+        ).lower() not in ('true', '1', 't')
+
+        job_facet: Dict = {}
+        if collect_source:
+            job_facet = {
                 "sourceCode": SourceCodeJobFacet(
                     "bash",
                     # We're on worker and should have access to DAG files
                     self.operator.bash_command
                 )
-            },
+            }
+
+        return TaskMetadata(
+            name=f"{self.operator.dag_id}.{self.operator.task_id}",
+            job_facets=job_facet,
             run_facets={
 
                 # The BashOperator is recorded as an "unknownSource" even though we have an
                 # extractor, as the <i>data lineage</i> cannot be determined from the operator
                 # directly.
                 "unknownSourceAttribute": UnknownOperatorAttributeRunFacet(
                     unknownItems=[
```

### Comparing `openlineage-airflow-0.9.0/openlineage/airflow/extractors/bigquery_extractor.py` & `openlineage-airflow-1.0.0/openlineage/airflow/extractors/bigquery_extractor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,43 @@
-# SPDX-License-Identifier: Apache-2.0.
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
 
-import logging
 import traceback
-from typing import Optional, List
-from airflow.version import version as AIRFLOW_VERSION
-
-from pkg_resources import parse_version
+from typing import List, Optional
 
+from openlineage.airflow.extractors.base import BaseExtractor, TaskMetadata
+from openlineage.airflow.utils import get_job_name, try_import_from_string
 from openlineage.client.facet import SqlJobFacet
 from openlineage.common.provider.bigquery import BigQueryDatasetsProvider, BigQueryErrorRunFacet
 
-from openlineage.airflow.extractors.base import (
-    BaseExtractor,
-    TaskMetadata
-)
-from openlineage.airflow.utils import get_job_name, try_import_from_string
-from google.cloud.bigquery import Client
-
 _BIGQUERY_CONN_URL = 'bigquery'
 
-log = logging.getLogger(__name__)
-
 
 class BigQueryExtractor(BaseExtractor):
     def __init__(self, operator):
         super().__init__(operator)
 
     @classmethod
     def get_operator_classnames(cls) -> List[str]:
         return ['BigQueryOperator', 'BigQueryExecuteQueryOperator']
 
     def extract(self) -> Optional[TaskMetadata]:
         return None
 
     def extract_on_complete(self, task_instance) -> Optional[TaskMetadata]:
-        log.debug(f"extract_on_complete({task_instance})")
+        self.log.debug(f"extract_on_complete({task_instance})")
 
         try:
             bigquery_job_id = self._get_xcom_bigquery_job_id(task_instance)
             if bigquery_job_id is None:
                 raise Exception(
                     "Xcom could not resolve BigQuery job id. Job may have failed."
                 )
         except Exception as e:
-            log.error(
+            self.log.error(
                 f"Cannot retrieve job details from BigQuery.Client. {e}", exc_info=True
             )
             return TaskMetadata(
                 name=get_job_name(task=self.operator),
                 run_facets={
                     "bigQuery_error": BigQueryErrorRunFacet(
                         clientError=f"{e}: {traceback.format_exc()}",
@@ -56,52 +46,63 @@
             )
 
         client = self._get_client()
 
         stats = BigQueryDatasetsProvider(client=client).get_facets(bigquery_job_id)
         inputs = stats.inputs
         output = stats.output
+
+        for ds in inputs:
+            ds.input_facets = self._get_input_facets()
+
         run_facets = stats.run_facets
         job_facets = {
             "sql": SqlJobFacet(self.operator.sql)
         }
 
         return TaskMetadata(
             name=get_job_name(task=self.operator),
             inputs=[ds.to_openlineage_dataset() for ds in inputs],
             outputs=[output.to_openlineage_dataset()] if output else [],
             run_facets=run_facets,
             job_facets=job_facets
         )
 
     def _get_client(self):
+        # lazy-load the bigquery Client due to its slow import
+        from google.cloud.bigquery import Client
         # Get client using Airflow hook - this way we use the same credentials as Airflow
         if hasattr(self.operator, 'hook') and self.operator.hook:
             hook = self.operator.hook
             return hook.get_client(
                 project_id=hook.project_id,
                 location=hook.location
             )
-        elif parse_version(AIRFLOW_VERSION) >= parse_version("2.0.0"):
-            BigQueryHook = try_import_from_string(
-                'airflow.providers.google.cloud.operators.bigquery.BigQueryHook'
+        BigQueryHook = try_import_from_string(
+            'airflow.providers.google.cloud.operators.bigquery.BigQueryHook'
+        )
+        if BigQueryHook is not None:
+            params = {
+                "gcp_conn_id": self.operator.gcp_conn_id,
+                "use_legacy_sql": self.operator.use_legacy_sql,
+                "location": self.operator.location,
+                "impersonation_chain": self.operator.impersonation_chain,
+            }
+            if hasattr(self.operator, "delegate_to"):
+                params["delegate_to"] = self.operator.delegate_to
+
+            hook = BigQueryHook(**params)
+            return hook.get_client(
+                project_id=hook.project_id,
+                location=hook.location
             )
-            if BigQueryHook is not None:
-                hook = BigQueryHook(
-                    gcp_conn_id=self.operator.gcp_conn_id,
-                    use_legacy_sql=self.operator.use_legacy_sql,
-                    delegate_to=self.operator.delegate_to,
-                    location=self.operator.location,
-                    impersonation_chain=self.operator.impersonation_chain,
-                )
-                return hook.get_client(
-                    project_id=hook.project_id,
-                    location=hook.location
-                )
         return Client()
 
     def _get_xcom_bigquery_job_id(self, task_instance):
         bigquery_job_id = task_instance.xcom_pull(
             task_ids=task_instance.task_id, key='job_id')
 
-        log.debug(f"bigquery_job_id: {bigquery_job_id}")
+        self.log.debug(f"bigquery_job_id: {bigquery_job_id}")
         return bigquery_job_id
+
+    def _get_input_facets(self):
+        return {}
```

### Comparing `openlineage-airflow-0.9.0/openlineage/airflow/extractors/example_dag.py` & `openlineage-airflow-1.0.0/openlineage/airflow/extractors/example_dag.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
+
 import os
 from datetime import datetime
 
 from airflow import DAG
 from airflow.operators.bash_operator import BashOperator
 from airflow.operators.python_operator import PythonOperator
```

### Comparing `openlineage-airflow-0.9.0/openlineage/airflow/extractors/great_expectations_extractor.py` & `openlineage-airflow-1.0.0/openlineage/airflow/extractors/great_expectations_extractor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-# SPDX-License-Identifier: Apache-2.0.
-import logging
-from typing import Optional, List
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
 
-from openlineage.airflow.extractors.base import BaseExtractor, TaskMetadata
-
-log = logging.getLogger(__file__)
+from typing import List, Optional
 
+from openlineage.airflow.extractors.base import BaseExtractor, TaskMetadata
 
 # Great Expectations is optional dependency.
 try:
     from great_expectations_provider.operators.great_expectations import GreatExpectationsOperator
     _has_great_expectations = True
 except Exception:
     # Create placeholder for GreatExpectationsOperator
@@ -29,21 +27,18 @@
     @classmethod
     def get_operator_classnames(cls) -> List[str]:
         return [GreatExpectationsOperator.__name__] if GreatExpectationsOperator else []
 
     def extract(self) -> Optional[TaskMetadata]:
         return None
 
-    def extract_on_complete(self, task_instance) -> Optional[TaskMetadata]:
-        return None
-
 
 if _has_great_expectations:
     GreatExpectationsExtractor = GreatExpectationsExtractorImpl
 else:
-    class GreatExpectationsExtractor:
+    class GreatExpectationsExtractor:   # type: ignore
         def __init__(self):
             raise RuntimeError('Great Expectations provider not found')
 
         @classmethod
         def get_operator_classnames(cls) -> List[str]:
             return []
```

### Comparing `openlineage-airflow-0.9.0/openlineage/airflow/extractors/postgres_extractor.py` & `openlineage-airflow-1.0.0/openlineage/airflow/extractors/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,134 +1,131 @@
-# SPDX-License-Identifier: Apache-2.0.
-import logging
-from typing import List, Optional
-from urllib.parse import urlparse
-
-from openlineage.airflow.extractors.dbapi_utils import get_table_schemas
-from openlineage.airflow.utils import (
-    get_normalized_postgres_connection_uri,
-    get_connection, safe_import_airflow
-)
-from openlineage.airflow.extractors.base import (
-    BaseExtractor,
-    TaskMetadata
-)
-from openlineage.client.facet import SqlJobFacet
-from openlineage.common.sql import SqlMeta, parse, DbTableMeta
-from openlineage.common.dataset import Source
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
 
+import json
+from abc import ABC, abstractmethod
+from typing import Any, Dict, List, Optional
+from urllib.parse import parse_qsl, urlencode, urlparse, urlunparse
 
-logger = logging.getLogger(__name__)
+import attr
+from openlineage.airflow.utils import LoggingMixin, get_job_name
+from openlineage.client.facet import BaseFacet
+from openlineage.client.run import Dataset
 
 
-class PostgresExtractor(BaseExtractor):
-    default_schema = 'public'
+@attr.s
+class OperatorLineage:
+    inputs: List[Dataset] = attr.ib(factory=list)
+    outputs: List[Dataset] = attr.ib(factory=list)
+    run_facets: Dict[str, BaseFacet] = attr.ib(factory=dict)
+    job_facets: Dict[str, BaseFacet] = attr.ib(factory=dict)
+
+
+@attr.s
+class TaskMetadata:
+    name: str = attr.ib()  # deprecated
+    inputs: List[Dataset] = attr.ib(factory=list)
+    outputs: List[Dataset] = attr.ib(factory=list)
+    run_facets: Dict[str, BaseFacet] = attr.ib(factory=dict)
+    job_facets: Dict[str, BaseFacet] = attr.ib(factory=dict)
+
+
+class BaseExtractor(ABC, LoggingMixin):
+
+    _whitelist_query_params: List[str] = []
 
     def __init__(self, operator):
-        super().__init__(operator)
-        self.conn = None
+        super().__init__()
+        self.operator = operator
+        self.patch()
+        self.context: Dict[str, Any] = dict()
+
+    def patch(self):
+        # Extractor should register extension methods or patches to operator here
+        pass
+
+    def set_context(self, key, value):
+        self.context[key] = value
 
     @classmethod
     def get_operator_classnames(cls) -> List[str]:
-        return ['PostgresOperator']
-
-    def extract(self) -> TaskMetadata:
-        task_name = f"{self.operator.dag_id}.{self.operator.task_id}"
-        job_facets = {
-            'sql': SqlJobFacet(self.operator.sql)
-        }
-
-        # (1) Parse sql statement to obtain input / output tables.
-        logger.debug(f"Sending SQL to parser: {self.operator.sql}")
-        sql_meta: Optional[SqlMeta] = parse(self.operator.sql, self.default_schema)
-        logger.debug(f"Got meta {sql_meta}")
-
-        if not sql_meta:
-            return TaskMetadata(
-                name=task_name,
-                inputs=[],
-                outputs=[],
-                run_facets={},
-                job_facets=job_facets
-            )
+        """
+        Implement this method returning list of operators that extractor works for.
+        Particularly, in Airflow 2 some operators are deprecated and simply subclass the new
+        implementation, for example BigQueryOperator:
+        https://github.com/apache/airflow/blob/main/airflow/contrib/operators/bigquery_operator.py
+        The BigQueryExtractor needs to work with both of them.
+        :return:
+        """
+        raise NotImplementedError()
 
-        # (2) Get Airflow connection
-        self.conn = get_connection(self._conn_id())
+    def validate(self):
+        assert self.operator.__class__.__name__ in self.get_operator_classnames()
 
-        # (3) Construct source object
-        source = Source(
-            scheme="postgres",
-            authority=self._get_authority(),
-            connection_url=self._get_connection_uri()
-        )
+    @abstractmethod
+    def extract(self) -> Optional[TaskMetadata]:
+        pass
 
-        database = self.operator.database
-        if not database:
-            database = self._get_database()
-
-        # (4) Map input / output tables to dataset objects with source set
-        # as the current connection. We need to also fetch the schema for the
-        # input tables to format the dataset name as:
-        # {schema_name}.{table_name}
-        inputs, outputs = get_table_schemas(
-            self._get_hook(),
-            source,
-            database,
-            self._information_schema_query(sql_meta.in_tables) if sql_meta.in_tables else None,
-            self._information_schema_query(sql_meta.out_tables) if sql_meta.out_tables else None
-        )
+    def extract_on_complete(self, task_instance) -> Optional[TaskMetadata]:
+        return self.extract()
 
-        return TaskMetadata(
-            name=task_name,
-            inputs=[ds.to_openlineage_dataset() for ds in inputs],
-            outputs=[ds.to_openlineage_dataset() for ds in outputs],
-            run_facets={},
-            job_facets=job_facets
-        )
+    @classmethod
+    def get_connection_uri(cls, conn):
+        """
+        Return the connection URI for the given ID. We first attempt to lookup
+        the connection URI via AIRFLOW_CONN_<conn_id>, else fallback on querying
+        the Airflow's connection table.
+        """
 
-    def _get_connection_uri(self):
-        return get_normalized_postgres_connection_uri(self.conn)
+        conn_uri = conn.get_uri()
+        parsed = urlparse(conn_uri)
 
-    def _get_scheme(self):
-        return 'postgres'
+        # Remove username and password
+        netloc = f"{parsed.hostname}" + (f":{parsed.port}" if parsed.port else "")
+        parsed = parsed._replace(netloc=netloc)
+        if parsed.query:
+            query_dict = dict(parse_qsl(parsed.query))
+            if conn.EXTRA_KEY in query_dict:
+                query_dict = json.loads(query_dict[conn.EXTRA_KEY])
+            filtered_qs = {
+                k: v for k, v in query_dict.items() if k in cls._whitelist_query_params
+            }
+            parsed = parsed._replace(query=urlencode(filtered_qs))
+        return urlunparse(parsed)
 
-    def _get_database(self) -> str:
-        if self.conn.schema:
-            return self.conn.schema
-        else:
-            parsed = urlparse(self.conn.get_uri())
-            return f'{parsed.path}'
-
-    def _get_authority(self) -> str:
-        if self.conn.host and self.conn.port:
-            return f'{self.conn.host}:{self.conn.port}'
-        else:
-            parsed = urlparse(self.conn.get_uri())
-            return f'{parsed.hostname}:{parsed.port}'
-
-    def _conn_id(self):
-        return self.operator.postgres_conn_id
-
-    def _get_hook(self):
-        PostgresHook = safe_import_airflow(
-            airflow_1_path="airflow.hooks.postgres_hook.PostgresHook",
-            airflow_2_path="airflow.providers.postgres.hooks.postgres.PostgresHook"
-        )
-        return PostgresHook(
-            postgres_conn_id=self.operator.postgres_conn_id,
-            schema=self.operator.database
-        )
 
-    @staticmethod
-    def _information_schema_query(tables: List[DbTableMeta]) -> str:
-        table_names = ",".join(map(
-            lambda name: f"'{name.name}'", tables
-        ))
-        return f"""
-        SELECT table_schema,
-        table_name,
-        column_name,
-        ordinal_position,
-        udt_name
-        FROM information_schema.columns
-        WHERE table_name IN ({table_names});
+class DefaultExtractor(BaseExtractor):
+    @classmethod
+    def get_operator_classnames(cls) -> List[str]:
+        """
+        Default extractor is chosen not on the classname basis, but
+        by existence of get_openlineage_facets method on operator
         """
+        return []
+
+    def extract(self) -> Optional[TaskMetadata]:
+        try:
+            return self._get_openlineage_facets(
+                self.operator.get_openlineage_facets_on_start
+            )
+        except AttributeError:
+            return None
+
+    def extract_on_complete(self, task_instance) -> Optional[TaskMetadata]:
+        on_complete = getattr(self.operator, 'get_openlineage_facets_on_complete', None)
+        if on_complete and callable(on_complete):
+            return self._get_openlineage_facets(
+                on_complete, task_instance
+            )
+        return self.extract()
+
+    def _get_openlineage_facets(
+        self, get_facets_method, *args
+    ) -> Optional[TaskMetadata]:
+        facets: OperatorLineage = get_facets_method(*args)
+        return TaskMetadata(
+            name=get_job_name(task=self.operator),
+            inputs=facets.inputs,
+            outputs=facets.outputs,
+            run_facets=facets.run_facets,
+            job_facets=facets.job_facets,
+        )
```

### Comparing `openlineage-airflow-0.9.0/openlineage/airflow/extractors/python_extractor.py` & `openlineage-airflow-1.0.0/openlineage/airflow/extractors/python_extractor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-import os
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
+
 import inspect
-import logging
-from typing import Optional, List, Callable
+import os
+from typing import Callable, Dict, List, Optional
 
 from openlineage.airflow.extractors.base import BaseExtractor, TaskMetadata
 from openlineage.airflow.facets import UnknownOperatorAttributeRunFacet, UnknownOperatorInstance
 from openlineage.client.facet import SourceCodeJobFacet
 
 
-log = logging.getLogger(__name__)
-
-
 class PythonExtractor(BaseExtractor):
     """
     This extractor provides visibility on what particular task does by extracting
     executed source code and putting it into SourceCodeJobFacet. It does not extract
     datasets.
     """
     @classmethod
     def get_operator_classnames(cls) -> List[str]:
         return ["PythonOperator"]
 
     def extract(self) -> Optional[TaskMetadata]:
-        collect_source = True
-        if os.environ.get(
-            "OPENLINEAGE_AIRFLOW_DISABLE_SOURCE_CODE", "False"
-        ).lower() in ('true', '1', 't'):
-            collect_source = False
+        collect_source = os.environ.get(
+            "OPENLINEAGE_AIRFLOW_DISABLE_SOURCE_CODE", "True"
+        ).lower() not in ('true', '1', 't')
 
         source_code = self.get_source_code(self.operator.python_callable)
-        job_facet = {}
+        job_facet: Dict = {}
         if collect_source and source_code:
             job_facet = {
                 "sourceCode": SourceCodeJobFacet(
                     "python",
                     # We're on worker and should have access to DAG files
                     source_code
                 )
@@ -61,8 +58,11 @@
     def get_source_code(self, callable: Callable) -> Optional[str]:
         try:
             return inspect.getsource(callable)
         except TypeError:
             # Trying to extract source code of builtin_function_or_method
             return str(callable)
         except OSError:
-            log.exception(f"Can't get source code facet of PythonOperator {self.operator.task_id}")
+            self.log.exception(
+                f"Can't get source code facet of PythonOperator {self.operator.task_id}"
+            )
+        return None
```

### Comparing `openlineage-airflow-0.9.0/openlineage/lineage_backend/__init__.py` & `openlineage-airflow-1.0.0/openlineage/lineage_backend/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+# Copyright 2018-2023 contributors to the OpenLineage project
 # SPDX-License-Identifier: Apache-2.0
+
 import os
-import uuid
 import time
+import uuid
+from typing import Optional
 
 from pkg_resources import parse_version
 
 from airflow.lineage.backend import LineageBackend
 from airflow.version import version as AIRFLOW_VERSION
 
 
@@ -27,70 +30,82 @@
             outlets=None,
             context=None
     ):
         """
         Send_lineage ignores manually provided inlets and outlets. The data collection mechanism
         is automatic, and bases on the passed context.
         """
-        from openlineage.airflow.utils import DagUtils, get_custom_facets, \
-            get_job_name, get_task_location
+        from openlineage.airflow.adapter import OpenLineageAdapter
+        from openlineage.airflow.utils import (
+            DagUtils,
+            get_airflow_run_facet,
+            get_custom_facets,
+            get_dagrun_start_end,
+            get_job_name,
+            get_task_location,
+        )
         dag = context['dag']
         dagrun = context['dag_run']
         task_instance = context['task_instance']
-        dag_run_id = str(uuid.uuid3(uuid.NAMESPACE_URL, f'{dag.dag_id}.{dagrun.run_id}'))
+        dag_run_id = self.adapter.build_dag_run_id(dag.dag_id, dagrun.run_id)
 
         run_id = str(uuid.uuid4())
         job_name = get_job_name(operator)
 
         task_metadata = self.extractor_manager.extract_metadata(
             dagrun=dagrun,
             task=operator,
             complete=True,
             task_instance=task_instance
         )
 
-        if parse_version(AIRFLOW_VERSION) >= parse_version("2.0.0"):
-            self.adapter.start_task(
-                run_id=run_id,
-                job_name=job_name,
-                job_description=dag.description,
-                event_time=DagUtils.get_start_time(task_instance.start_date),
-                parent_job_name=dag.dag_id,
-                parent_run_id=dag_run_id,
-                code_location=get_task_location(operator),
-                nominal_start_time=DagUtils.get_start_time(dagrun.execution_date),
-                nominal_end_time=DagUtils.to_iso_8601(task_instance.end_date),
-                task=task_metadata,
-                run_facets={
-                    **task_metadata.run_facets,
-                    **get_custom_facets(operator, dagrun.external_trigger)
-                }
-            )
+        task_uuid = OpenLineageAdapter.build_task_instance_run_id(
+            operator.task_id, task_instance.execution_date, task_instance.try_number
+        )
+        start, end = get_dagrun_start_end(dagrun, dag)
+
+        self.adapter.start_task(
+            run_id=run_id,
+            job_name=job_name,
+            job_description=dag.description,
+            event_time=DagUtils.get_start_time(task_instance.start_date),
+            parent_job_name=dag.dag_id,
+            parent_run_id=dag_run_id,
+            code_location=get_task_location(operator),
+            nominal_start_time=DagUtils.get_start_time(start),
+            nominal_end_time=DagUtils.to_iso_8601(end),
+            owners=dag.owner.split(', '),
+            task=task_metadata,
+            run_facets={
+                **task_metadata.run_facets,
+                **get_custom_facets(dagrun, operator, dagrun.external_trigger),
+                **get_airflow_run_facet(dagrun, dag, task_instance, operator, task_uuid)
+            }
+        )
 
         self.adapter.complete_task(
             run_id=run_id,
             job_name=job_name,
             end_time=DagUtils.to_iso_8601(self._now_ms()),
             task=task_metadata,
         )
 
     @staticmethod
     def _now_ms():
         return int(round(time.time() * 1000))
 
 
 class OpenLineageBackend(LineageBackend):
-    # Airflow 1.10 uses send_lineage as staticmethod, so just construct class
-    # instance on first use and delegate calls to it
-    backend: Backend = None
+    # Constructing instance on first use and delegate calls to it - backwards compatible with 1.10
+    backend: Optional[Backend] = None
 
     @classmethod
     def send_lineage(cls, *args, **kwargs):
         # Do not use LineageBackend approach when we can use plugins
         if parse_version(AIRFLOW_VERSION) >= parse_version("2.3.0.dev0"):
             return
         # Make this method a noop if OPENLINEAGE_DISABLED is set to true
-        if os.getenv("OPENLINEAGE_DISABLED", None) in [True, 'true', "True"]:
+        if os.getenv("OPENLINEAGE_DISABLED", "").lower() == "true":
             return
         if not cls.backend:
             cls.backend = Backend()
         return cls.backend.send_lineage(*args, **kwargs)
```

### Comparing `openlineage-airflow-0.9.0/openlineage_airflow.egg-info/PKG-INFO` & `openlineage-airflow-1.0.0/openlineage_airflow.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,266 +1,292 @@
 Metadata-Version: 2.1
 Name: openlineage-airflow
-Version: 0.9.0
+Version: 1.0.0
 Summary: OpenLineage integration with Airflow
-Home-page: UNKNOWN
 Author: OpenLineage
-License: UNKNOWN
-Description: <!-- SPDX-License-Identifier: Apache-2.0 -->
-        
-        # OpenLineage Airflow Integration
-        
-        A library that integrates [Airflow `DAGs`]() with [OpenLineage](https://openlineage.io) for automatic metadata collection.
-        
-        ## Features
-        
-        **Metadata**
-        
-        * Task lifecycle
-        * Task parameters
-        * Task runs linked to **versioned** code
-        * Task inputs / outputs
-        
-        **Lineage**
-        
-        * Track inter-DAG dependencies
-        
-        **Built-in**
-        
-        * SQL parser
-        * Link to code builder (ex: **GitHub**)
-        * Metadata extractors
-        
-        ## Requirements
-        
-        - [Python 3.7](https://www.python.org/downloads)
-        - [Airflow 1.10.12+](https://pypi.org/project/apache-airflow)
-        - (experimental) [Airflow 2.1+](https://pypi.org/project/apache-airflow)
-        
-        ## Installation
-        
-        ```bash
-        $ pip3 install openlineage-airflow
-        ```
-        
-        > **Note:** You can also add `openlineage-airflow` to your `requirements.txt` for Airflow.
-        
-        To install from source, run:
-        
-        ```bash
-        $ python3 setup.py install
-        ```
-        
-        ## Setup
-        
-        ### Airflow 2.3+
-        
-        Integration automatically registers itself for Airflow 2.3 if it's installed on Airflow worker's python.
-        This means you don't have to do anything besides configuring it, which is described in Configuration section.
-        
-        ### Airflow 2.1 - 2.2
-        
-        This method has limited support: 
-        it does not support tracking failed jobs, and job starts are registered only when job ends.
-        
-        Set your LineageBackend in your [airflow.cfg](https://airflow.apache.org/docs/apache-airflow/stable/howto/set-config.html) or via environmental variable `AIRFLOW__LINEAGE__BACKEND`
-        to 
-        ```
-        openlineage.lineage_backend.OpenLineageBackend
-        ```
-        
-        In contrast to integration via subclassing `DAG`, `LineageBackend` based approach collects all metadata 
-        for task on each task completion.
-        
-        OpenLineageBackend does not take into account manually configured inlets and outlets. 
-        
-        ### Airflow 1.10+
-        
-        To begin collecting Airflow DAG metadata with OpenLineage, use:
-        
-        ```diff
-        - from airflow import DAG
-        + from openlineage.airflow import DAG
-        ```
-        
-        When enabled, the library will:
-        
-        1. On DAG **start**, collect metadata for each task using an `Extractor` if it exists for given operator.
-        2. Collect task input / output metadata (`source`, `schema`, etc)
-        3. Collect task run-level metadata (execution time, state, parameters, etc)
-        4. On DAG **complete**, also mark the task as _complete_ in OpenLineage
-        
-        ## Configuration
-        
-        ### `HTTP` Backend Environment Variables
-        
-        `openlineage-airflow` uses OpenLineage client to push data to OpenLineage backend.
-        
-        OpenLineage client depends on environment variables:
-        
-        * `OPENLINEAGE_URL` - point to service which will consume OpenLineage events
-        * `OPENLINEAGE_API_KEY` - set if consumer of OpenLineage events requires `Bearer` authentication key
-        * `OPENLINEAGE_NAMESPACE` - set if you are using something other than the `default` namespace for job namespace.
-        * `OPENLINEAGE_AIRFLOW_DISABLE_SOURCE_CODE` - set to `True` if you don't want source code of callables provided to PythonOperator to be send in OpenLineage events
-        
-        For backwards compatibility, `openlineage-airflow` also support configuration via
-        `MARQUEZ_URL`, `MARQUEZ_NAMESPACE` and `MARQUEZ_API_KEY` variables.
-        
-        ```
-        MARQUEZ_URL=http://my_hosted_marquez.example.com:5000
-        MARQUEZ_NAMESPACE=my_special_ns
-        ```
-        
-        ### Extractors : Sending the correct data from your DAGs
-        
-        If you do nothing, OpenLineage backend will receive the `Job` and the `Run` from your DAGs, but,
-        unless you use few operators for which this integration provides extractor, input and output metadata will not be send.
-        
-        `openlineage-airflow` allows you to do more than that by building "Extractors". Extractor is object
-        suited to extract metadata from particular operator (or operators). 
-        
-        1. Name : The name of the task
-        2. Inputs : List of input datasets
-        3. Outputs : List of output datasets
-        4. Context : The Airflow context for the task
-        
-        #### Bundled Extractors
-        
-        `openlineage-airflow` provides extractors for
-        
-        * `PostgresOperator`
-        * `MySqlOperator`
-        * `BigQueryOperator`
-        * `SnowflakeOperator`
-        * `GreatExpectationsOperator`
-        * `PythonOperator`
-        
-        SQL Operators utilize SQL parser. There is experimental SQL parser, activated if you install [openlineage-sql](https://pypi.org/project/openlineage-sql) on your Airflow worker.
-        
-        #### Custom Extractors
-        
-        If your DAGs contain additional operators from which you want to extract lineage data, fear not - you can always
-        provide custom extractors. They should derive from `BaseExtractor`. 
-        
-        There are two ways to register them for use in `openlineage-airflow`. 
-        
-        First one, is to add them to `OPENLINEAGE_EXTRACTORS` environment variable, separated by comma `(;)` 
-        ```
-        OPENLINEAGE_EXTRACTORS=full.path.to.ExtractorClass;full.path.to.AnotherExtractorClass
-        ```
-        
-        Second one - working in Airflow 1.10.x only - is to register all additional operator-extractor pairings by 
-        providing `lineage_custom_extractors` argument in `openlineage.airflow.DAG`.
-        
-        #### Great Expectations
-        
-        Great Expectations integration works by providing OpenLineageValidationAction. You need to include it into your `action_list` in `great_expectations.yml`.
-        
-        The following example illustrates example change in default configuration: 
-        ```diff
-        validation_operators:
-          action_list_operator:
-            # To learn how to configure sending Slack notifications during evaluation
-            # (and other customizations), read: https://docs.greatexpectations.io/en/latest/autoapi/great_expectations/validation_operators/index.html#great_expectations.validation_operators.ActionListValidationOperator
-            class_name: ActionListValidationOperator
-            action_list:
-              - name: store_validation_result
-                action:
-                  class_name: StoreValidationResultAction
-              - name: store_evaluation_params
-                action:
-                  class_name: StoreEvaluationParametersAction
-              - name: update_data_docs
-                action:
-                  class_name: UpdateDataDocsAction
-        +     - name: openlineage
-        +       action:
-        +         class_name: OpenLineageValidationAction
-        +         module_name: openlineage.common.provider.great_expectations.action
-              # - name: send_slack_notification_on_validation_result
-              #   action:
-              #     class_name: SlackNotificationAction
-              #     # put the actual webhook URL in the uncommitted/config_variables.yml file
-              #     slack_webhook: ${validation_notification_slack_webhook}
-              #     notify_on: all # possible values: "all", "failure", "success"
-              #     renderer:
-              #       module_name: great_expectations.render.renderer.slack_renderer
-              #       class_name: SlackRenderer
-        ```
-        
-        If you're using `GreatExpectationsOperator`, you need to set `validation_operator_name` to operator that includes OpenLineageValidationAction.
-        Setting it in `great_expectations.yml` files isn't enough - the operator overrides it with default name if it's not provided.
-        
-        To see example of working configuration, you can see [DAG](https://github.com/OpenLineage/OpenLineage/blob/main/integration/airflow/tests/integration/airflow/dags/greatexpectations_dag.py) and [Great Expectations configuration](https://github.com/OpenLineage/OpenLineage/tree/main/integration/airflow/tests/integration/data/great_expectations) in integration tests.
-        
-        ## Triggering Child Jobs
-        Commonly, Airflow DAGs will trigger processes on remote systems, such as an Apache Spark or Apache
-        Beam job. Those systems may have their own OpenLineage integration and report their own
-        job runs and dataset inputs/outputs. To propagate the job hierarchy, tasks must send their own run
-        id so that the downstream process can report the [ParentRunFacet](https://github.com/OpenLineage/OpenLineage/blob/main/spec/OpenLineage.json#/definitions/ParentRunFacet)
-        with the proper run id.
-        
-        The `lineage_run_id` and `lineage_parent_id` macros exists to inject the run id or whole parent run information
-        of a given task into the arguments sent to a  remote processing job's Airflow operator. The macro requires the 
-        DAG run_id and the task to access the generated run id for that task. For example, a Spark job can be triggered
-        using the `DataProcPySparkOperator` with the correct parent run id using the following configuration:
-        
-        Airflow 1.10:
-        
-        ```python
-        t1 = DataProcPySparkOperator(
-            task_id=job_name,
-            #required pyspark configuration,
-            job_name=job_name,
-            dataproc_pyspark_properties={
-                'spark.driver.extraJavaOptions':
-                    f"-javaagent:{jar}={os.environ.get('OPENLINEAGE_URL')}/api/v1/namespaces/{os.getenv('OPENLINEAGE_NAMESPACE', 'default')}/jobs/{job_name}/runs/{{{{lineage_run_id(run_id, task)}}}}?api_key={os.environ.get('OPENLINEAGE_API_KEY')}"
-                dag=dag)
-        ```
-        
-        Airflow 2.0+:
-        
-        ```python
-        t1 = DataProcPySparkOperator(
-            task_id=job_name,
-            #required pyspark configuration,
-            job_name=job_name,
-            dataproc_pyspark_properties={
-                'spark.driver.extraJavaOptions':
-                    f"-javaagent:{jar}={os.environ.get('OPENLINEAGE_URL')}/api/v1/namespaces/{os.getenv('OPENLINEAGE_NAMESPACE', 'default')}/jobs/{job_name}/runs/{{{{macros.OpenLineagePlugin.lineage_run_id(run_id, task)}}}}?api_key={os.environ.get('OPENLINEAGE_API_KEY')}"
-                dag=dag)
-        ```
-        
-        ## Development
-        
-        To install all dependencies for _local_ development:
-        
-        ```bash
-        # Bash
-        $ pip3 install -e .[dev]
-        ```
-        ```zsh
-        # escape the brackets in zsh
-        $ pip3 install -e .\[dev\]
-        ```
-        
-        To run the entire test suite, you'll first want to initialize the Airflow database:
-        
-        ```bash
-        $ airflow initdb
-        ```
-        
-        Then, run the test suite with:
-        
-        ```bash
-        $ pytest
-        ```
-        
 Keywords: openlineage
-Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: sql
 Provides-Extra: tests
-Provides-Extra: airflow-1
-Provides-Extra: airflow-2
+Provides-Extra: airflow
 Provides-Extra: dev
+
+# OpenLineage Airflow Integration
+
+A library that integrates [Airflow `DAGs`]() with [OpenLineage](https://openlineage.io) for automatic metadata collection.
+
+## Features
+
+**Metadata**
+
+* Task lifecycle
+* Task parameters
+* Task runs linked to **versioned** code
+* Task inputs / outputs
+
+**Lineage**
+
+* Track inter-DAG dependencies
+
+**Built-in**
+
+* SQL parser
+* Link to code builder (ex: **GitHub**)
+* Metadata extractors
+
+## Requirements
+
+- [Python 3.8](https://www.python.org/downloads)
+- [Airflow 2.1+](https://pypi.org/project/apache-airflow)
+
+## Installation
+
+```bash
+$ pip3 install openlineage-airflow
+```
+
+> **Note:** You can also add `openlineage-airflow` to your `requirements.txt` for Airflow.
+
+To install from source, run:
+
+```bash
+$ python3 setup.py install
+```
+
+## Setup
+
+### Airflow 2.3+
+
+The integration automatically registers itself for Airflow 2.3 if it's installed on the Airflow worker's Python.
+This means you don't have to do anything besides configuring it, which is described in the Configuration section.
+
+### Airflow 2.1 - 2.2
+
+This method has limited support: it does not support tracking failed jobs, and job starts are registered only when a job ends.
+
+Set your LineageBackend in your [airflow.cfg](https://airflow.apache.org/docs/apache-airflow/stable/howto/set-config.html) or via environmental variable `AIRFLOW__LINEAGE__BACKEND` to 
+```
+openlineage.lineage_backend.OpenLineageBackend
+```
+
+In contrast to integration via subclassing a `DAG`, a `LineageBackend`-based approach collects all metadata 
+for a task on each task's completion.
+
+The OpenLineageBackend does not take into account manually configured inlets and outlets. 
+
+When enabled, the library will:
+
+1. On DAG **start**, collect metadata for each task using an `Extractor` if it exists for a given operator.
+2. Collect task input / output metadata (`source`, `schema`, etc.)
+3. Collect task run-level metadata (execution time, state, parameters, etc.)
+4. On DAG **complete**, also mark the task as _complete_ in OpenLineage
+
+## Configuration
+
+### `HTTP` Backend Environment Variables
+
+`openlineage-airflow` uses the OpenLineage client to push data to OpenLineage backend.
+
+The OpenLineage client depends on environment variables:
+
+* `OPENLINEAGE_URL` - point to the service that will consume OpenLineage events.
+* `OPENLINEAGE_API_KEY` - set if the consumer of OpenLineage events requires a `Bearer` authentication key.
+* `OPENLINEAGE_NAMESPACE` - set if you are using something other than the `default` namespace for the job namespace.
+* `OPENLINEAGE_AIRFLOW_DISABLE_SOURCE_CODE` - set to `False` if you want the source code of callables provided in the PythonOperator to be sent in OpenLineage events.
+
+For backwards compatibility, `openlineage-airflow` also supports configuration via
+`MARQUEZ_URL`, `MARQUEZ_NAMESPACE` and `MARQUEZ_API_KEY` variables.
+
+```
+MARQUEZ_URL=http://my_hosted_marquez.example.com:5000
+MARQUEZ_NAMESPACE=my_special_ns
+```
+
+### Extractors : Sending the correct data from your DAGs
+
+If you do nothing, the OpenLineage backend will receive the `Job` and the `Run` from your DAGs, but,
+unless you use one of the few operators for which this integration provides an extractor, input and output metadata will not be sent.
+
+`openlineage-airflow` allows you to do more than that by building "Extractors." An extractor is an object
+suited to extract metadata from a particular operator (or operators). 
+
+1. Name : The name of the task
+2. Inputs : A list of input datasets
+3. Outputs : A list of output datasets
+4. Context : The Airflow context for the task
+
+#### Bundled Extractors
+
+`openlineage-airflow` provides extractors for:
+
+* `PostgresOperator`
+* `MySqlOperator`
+* `AthenaOperator`
+* `BigQueryOperator`
+* `SnowflakeOperator`
+* `TrinoOperator`
+* `GreatExpectationsOperator`
+* `SFTPOperator`
+* `FTPFileTransmitOperator`
+* `PythonOperator`
+* `RedshiftDataOperator`, `RedshiftSQLOperator`
+* `SageMakerProcessingOperator`, `SageMakerProcessingOperatorAsync`
+* `SageMakerTrainingOperator`, `SageMakerTrainingOperatorAsync`
+* `SageMakerTransformOperator`, `SageMakerTransformOperatorAsync`
+* `S3CopyObjectExtractor`, `S3FileTransformExtractor`
+* `GCSToGCSOperator`
+* `DbtCloudRunJobOperator`
+
+SQL Operators utilize the SQL parser. There is an experimental SQL parser activated if you install [openlineage-sql](https://pypi.org/project/openlineage-sql) on your Airflow worker.
+
+
+#### Custom Extractors
+
+If your DAGs contain additional operators from which you want to extract lineage data, fear not - you can always
+provide custom extractors. They should derive from `BaseExtractor`. 
+
+There are two ways to register them for use in `openlineage-airflow`. 
+
+One way is to add them to the `OPENLINEAGE_EXTRACTORS` environment variable, separated by a semi-colon `(;)`. 
+```
+OPENLINEAGE_EXTRACTORS=full.path.to.ExtractorClass;full.path.to.AnotherExtractorClass
+```
+
+To ensure OpenLineage logging propagation to custom extractors you should use `self.log` instead of creating a logger yourself.
+
+#### Default Extractor
+
+When you own operators' code this is not neccessary to provide custom extractors. You can also use Default Extractor's capability.
+
+In order to do that you should define at least one of two methods in operator:
+
+* `get_openlineage_facets_on_start()`
+
+Extracts metadata on start of task.
+
+* `get_openlineage_facets_on_complete(task_instance: TaskInstance)`
+
+Extracts metadata on complete of task. This should accept `task_instance` argument, similar to `extract_on_complete` method in base extractors.
+
+If you don't define `get_openlineage_facets_on_complete` method it would fall back to `get_openlineage_facets_on_start`.
+
+
+#### Great Expectations
+
+The Great Expectations integration works by providing an OpenLineageValidationAction. You need to include it into your `action_list` in `great_expectations.yml`.
+
+The following example illustrates a way to change the default configuration: 
+```diff
+validation_operators:
+  action_list_operator:
+    # To learn how to configure sending Slack notifications during evaluation
+    # (and other customizations), read: https://docs.greatexpectations.io/en/latest/autoapi/great_expectations/validation_operators/index.html#great_expectations.validation_operators.ActionListValidationOperator
+    class_name: ActionListValidationOperator
+    action_list:
+      - name: store_validation_result
+        action:
+          class_name: StoreValidationResultAction
+      - name: store_evaluation_params
+        action:
+          class_name: StoreEvaluationParametersAction
+      - name: update_data_docs
+        action:
+          class_name: UpdateDataDocsAction
++     - name: openlineage
++       action:
++         class_name: OpenLineageValidationAction
++         module_name: openlineage.common.provider.great_expectations.action
+      # - name: send_slack_notification_on_validation_result
+      #   action:
+      #     class_name: SlackNotificationAction
+      #     # put the actual webhook URL in the uncommitted/config_variables.yml file
+      #     slack_webhook: ${validation_notification_slack_webhook}
+      #     notify_on: all # possible values: "all", "failure", "success"
+      #     renderer:
+      #       module_name: great_expectations.render.renderer.slack_renderer
+      #       class_name: SlackRenderer
+```
+
+If you're using `GreatExpectationsOperator`, you need to set `validation_operator_name` to an operator that includes OpenLineageValidationAction.
+Setting it in `great_expectations.yml` files isn't enough - the operator overrides it with the default name if a different one is not provided.
+
+To see an example of a working configuration, see [DAG](https://github.com/OpenLineage/OpenLineage/blob/main/integration/airflow/tests/integration/airflow/dags/greatexpectations_dag.py) and [Great Expectations configuration](https://github.com/OpenLineage/OpenLineage/tree/main/integration/airflow/tests/integration/data/great_expectations) in the integration tests.
+
+### Logging
+In addition to conventional logging approaches, the `openlineage-airflow` package provides an alternative way of configuring its logging behavior. By setting the `OPENLINEAGE_AIRFLOW_LOGGING` environment variable, you can establish the logging level for the `openlineage.airflow` and its child modules.
+
+## Triggering Child Jobs
+Commonly, Airflow DAGs will trigger processes on remote systems, such as an Apache Spark or Apache
+Beam job. Those systems may have their own OpenLineage integrations and report their own
+job runs and dataset inputs/outputs. To propagate the job hierarchy, tasks must send their own run
+ids so that the downstream process can report the [ParentRunFacet](https://github.com/OpenLineage/OpenLineage/blob/main/spec/OpenLineage.json#/definitions/ParentRunFacet)
+with the proper run id.
+
+The `lineage_run_id` and `lineage_parent_id` macros exists to inject the run id or whole parent run information
+of a given task into the arguments sent to a remote processing job's Airflow operator. The macro requires the 
+DAG `run_id` and the task to access the generated `run_id` for that task. For example, a Spark job can be triggered
+using the `DataProcPySparkOperator` with the correct parent `run_id` using the following configuration:
+
+```python
+t1 = DataProcPySparkOperator(
+    task_id=job_name,
+    #required pyspark configuration,
+    job_name=job_name,
+    dataproc_pyspark_properties={
+        'spark.driver.extraJavaOptions':
+            f"-javaagent:{jar}={os.environ.get('OPENLINEAGE_URL')}/api/v1/namespaces/{os.getenv('OPENLINEAGE_NAMESPACE', 'default')}/jobs/{job_name}/runs/{{{{macros.OpenLineagePlugin.lineage_run_id(task, task_instance)}}}}?api_key={os.environ.get('OPENLINEAGE_API_KEY')}"
+        dag=dag)
+```
+
+## Secrets redaction
+The integration uses Airflow SecretsMasker to hide secrets from produced metadata events. As not all fields in the metadata should be redacted, `RedactMixin` is used to pass information about which fields should be ignored by the process. 
+
+Typically, you should subclass `RedactMixin` and use the `_skip_redact` attribute as a list of names of fields to be skipped.
+
+However, all facets inheriting from `BaseFacet` should use the `_additional_skip_redact` attribute as an addition to the regular list (`['_producer', '_schemaURL']`).
+
+## Development
+
+To install all dependencies for _local_ development:
+
+The Airflow integration depends on `openlineage.sql`, `openlineage.common` and `openlineage.client.python`. You should install them first independently or try to install them with following command:
+
+```bash
+$ pip install -r dev-requirements.txt
+```
+
+There is also a bash script that can run an arbitrary Airflow image with an OpenLineage integration built from the current branch. Additionally, it mounts OpenLineage Python packages as Docker volumes. This enables you to change your code without the need to constantly rebuild Docker images to run tests.
+Run it as:
+```bash
+$ AIRFLOW_IMAGE=<airflow_image_with_tag> ./scripts/run-dev-airflow.sh [--help]
+```
+### Unit tests
+To run the entire unit test suite, use the below command:
+```bash
+$ tox
+```
+or choose one of the environments, e.g.:
+```bash
+$ tox -e py-airflow214
+```
+You can also skip using `tox` and run `pytest` on your own dev environment.
+### Integration tests
+The integration tests require the use of _docker compose_. There are scripts prepared to make build images and run tests easier.
+
+```bash
+$ AIRFLOW_IMAGE=<name-of-airflow-image> ./tests/integration/docker/up.sh
+```
+
+```bash
+$ AIRFLOW_IMAGE=apache/airflow:2.3.1-python3.8 ./tests/integration/docker/up.sh
+```
+
+When using `run-dev-airflow.sh`, you can add the `-i` flag or `--attach-integration` flag to run integration tests in a dev environment.
+This can be helpful when you need to run arbitrary integration tests during development. For example, the following command run in the integration container...
+```bash
+python -m pytest test_integration.py::test_integration[great_expectations_validation-requests/great_expectations.json]
+```
+...runs a single test which you can repeat after changes in code.
+
+----
+SPDX-License-Identifier: Apache-2.0\
+Copyright 2018-2023 contributors to the OpenLineage project
```

### Comparing `openlineage-airflow-0.9.0/setup.py` & `openlineage-airflow-1.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 #!/usr/bin/env python
 #
-# SPDX-License-Identifier: Apache-2.0.
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
 #
 # -*- coding: utf-8 -*-
 
-from setuptools import setup, find_namespace_packages
+from setuptools import find_namespace_packages, setup
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
-__version__ = "0.9.0"
+__version__ = "1.0.0"
 
 requirements = [
-    "attrs>=19.3",
+    "attrs>=20.3",
     "requests>=2.20.0",
-    "sqlparse>=0.3.1",
-    f"openlineage-integration-common=={__version__}",
+    f"openlineage-integration-common[sql]=={__version__}",
     f"openlineage-python=={__version__}",
 ]
 
 extras_require = {
-    "sql": [
-        f"openlineage-integration-common[sql]=={__version__}",
-    ],
     "tests": [
+        "aiohttp",          # tox Airflow 2.3.4 does not install it by default
         "pytest",
         "pytest-cov",
+        "pytest-mock",
         "mock",
-        "flake8",
+        "ruff",
         "SQLAlchemy",       # must be set to 1.3.* for airflow tests compatibility
         "Flask-SQLAlchemy",  # must be set to 2.4.* for airflow tests compatibility
         "pandas-gbq==0.14.1",       # must be set to 0.14.* for airflow tests compatibility
-        "snowflake-connector-python"
-    ],
-    "airflow-1": [
-        "apache-airflow[gcp_api,google,postgres,mysql]==1.10.15",
-        "airflow-provider-great-expectations==0.0.8",
+        "snowflake-connector-python",
     ],
-    "airflow-2": [
-        "apache-airflow==2.1.4",
+    "airflow": [
         "apache-airflow-providers-postgres>=2.0.0",
         "apache-airflow-providers-mysql>=2.0.0",
+        "apache-airflow-providers-trino>=3.1.0",
         "apache-airflow-providers-snowflake>=2.1.0",
         "apache-airflow-providers-google>=5.0.0",
-        "airflow-provider-great-expectations>=0.0.8",
+        "apache-airflow-providers-amazon>=3.1.1",
+        "apache-airflow-providers-sftp>=2.1.1",
+        "apache-airflow-providers-ssh>=2.1.0",
+        "apache-airflow-providers-ftp>=3.3.0",
+        "apache-airflow-providers-dbt-cloud<3.2.0",
+        "airflow-provider-great-expectations==0.1.5",
+        "great-expectations<=0.15.23",
+        "protobuf>=3.20,<4.23",
     ],
 }
 
 extras_require["dev"] = extras_require["tests"]
 
 setup(
     name="openlineage-airflow",
@@ -56,14 +58,14 @@
     long_description=readme,
     long_description_content_type="text/markdown",
     author="OpenLineage",
     packages=find_namespace_packages(include=['openlineage.*']),
     include_package_data=True,
     install_requires=requirements,
     extras_require=extras_require,
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     zip_safe=False,
     keywords="openlineage",
     entry_points={
         "airflow.plugins": ["OpenLineagePlugin = openlineage.airflow.plugin:OpenLineagePlugin"]
     }
 )
```

