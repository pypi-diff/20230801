# Comparing `tmp/serra-0.7.tar.gz` & `tmp/serra-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serra-0.7.tar", last modified: Tue Aug  1 20:59:29 2023, max compression
+gzip compressed data, was "serra-0.7.1.tar", last modified: Tue Aug  1 21:22:37 2023, max compression
```

## Comparing `serra-0.7.tar` & `serra-0.7.1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.227937 serra-0.7/
--rw-r--r--   0 alanwang   (501) staff       (20)     3860 2023-08-01 20:57:39.000000 serra-0.7/LICENSE.md
--rw-r--r--   0 alanwang   (501) staff       (20)      240 2023-08-01 20:59:29.227796 serra-0.7/PKG-INFO
--rw-r--r--   0 alanwang   (501) staff       (20)     4478 2023-08-01 20:57:39.000000 serra-0.7/README.md
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.215528 serra-0.7/serra/
--rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-08-01 20:57:39.000000 serra-0.7/serra/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2006 2023-08-01 20:57:39.000000 serra-0.7/serra/aws.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1872 2023-08-01 20:57:39.000000 serra-0.7/serra/cli.py
--rw-r--r--   0 alanwang   (501) staff       (20)      252 2023-08-01 20:57:39.000000 serra-0.7/serra/config.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1788 2023-08-01 20:57:39.000000 serra-0.7/serra/config_parser.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.213189 serra-0.7/serra/data/
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.217335 serra-0.7/serra/data/autocomplete/
--rw-r--r--   0 alanwang   (501) staff       (20)     1110 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/README.md
--rw-r--r--   0 alanwang   (501) staff       (20)     1636 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/gen_schemas.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.217472 serra-0.7/serra/data/autocomplete/inputs/
--rw-r--r--   0 alanwang   (501) staff       (20)     2249 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/inputs/specs.json
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.219812 serra-0.7/serra/data/autocomplete/output/
--rw-r--r--   0 alanwang   (501) staff       (20)      391 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/AddColumnTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      276 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/AmazonS3Reader.json
--rw-r--r--   0 alanwang   (501) staff       (20)      341 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/AmazonS3Writer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      267 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/CaseWhenTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      216 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/CastColumnTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      206 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/DatabricksReader.json
--rw-r--r--   0 alanwang   (501) staff       (20)      389 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/DatabricksWriter.json
--rw-r--r--   0 alanwang   (501) staff       (20)      213 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/DropColumnTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      274 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/GetCountTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      354 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/JoinTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      148 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/LocalReader.json
--rw-r--r--   0 alanwang   (501) staff       (20)      213 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/LocalWriter.json
--rw-r--r--   0 alanwang   (501) staff       (20)      331 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/MapTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      408 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/PivotTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      274 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/RenameColumnTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      210 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/SelectTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/SnowflakeWriter.json
--rw-r--r--   0 alanwang   (501) staff       (20)     7553 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/serra_yaml_schema.json
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.220044 serra-0.7/serra/data/autocomplete/templates/
--rw-r--r--   0 alanwang   (501) staff       (20)      326 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/templates/schema_template.json
--rw-r--r--   0 alanwang   (501) staff       (20)       95 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/templates/transformer_template.json
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.220286 serra-0.7/serra/data/workspace_example/
--rw-r--r--   0 alanwang   (501) staff       (20)      137 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/README.md
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.220666 serra-0.7/serra/data/workspace_example/examples/
--rw-r--r--   0 alanwang   (501) staff       (20)     1610 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/examples/ratings.csv
--rw-r--r--   0 alanwang   (501) staff       (20)     6706 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/examples/sales.csv
--rw-r--r--   0 alanwang   (501) staff       (20)     1124 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/examples/states_to_abbreviation.json
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.221568 serra-0.7/serra/data/workspace_example/jobs/
--rw-r--r--   0 alanwang   (501) staff       (20)      912 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/jobs/CloudDemo.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      945 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/jobs/Demo.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      418 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/jobs/LocalExample.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      220 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/jobs/ReadExample.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      456 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/jobs/ReadJoinWrite.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      393 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/jobs/ReadMapWrite.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      397 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/jobs/ReadPivotWrite.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      323 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/profiles.yml
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.221811 serra-0.7/serra/data/workspace_example/sql/
--rw-r--r--   0 alanwang   (501) staff       (20)     2603 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/sql/easy_demo.sql
--rw-r--r--   0 alanwang   (501) staff       (20)     2909 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/sql/hard_demo.sql
--rw-r--r--   0 alanwang   (501) staff       (20)     2964 2023-08-01 20:57:39.000000 serra-0.7/serra/databricks.py
--rw-r--r--   0 alanwang   (501) staff       (20)      106 2023-08-01 20:57:39.000000 serra-0.7/serra/exceptions.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1120 2023-08-01 20:57:39.000000 serra-0.7/serra/profile.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.222633 serra-0.7/serra/readers/
--rw-r--r--   0 alanwang   (501) staff       (20)      233 2023-08-01 20:57:39.000000 serra-0.7/serra/readers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1457 2023-08-01 20:57:39.000000 serra-0.7/serra/readers/amazon_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      579 2023-08-01 20:57:39.000000 serra-0.7/serra/readers/databricks_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      501 2023-08-01 20:57:39.000000 serra-0.7/serra/readers/local_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      277 2023-08-01 20:57:39.000000 serra-0.7/serra/readers/reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-08-01 20:57:39.000000 serra-0.7/serra/readers/s3_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1380 2023-08-01 20:57:39.000000 serra-0.7/serra/readers/snowflaker_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2977 2023-08-01 20:57:39.000000 serra-0.7/serra/run.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.223262 serra-0.7/serra/runners/
--rw-r--r--   0 alanwang   (501) staff       (20)     2631 2023-08-01 20:57:39.000000 serra-0.7/serra/runners/ExecutionGraph.py
--rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-08-01 20:57:39.000000 serra-0.7/serra/runners/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     3148 2023-08-01 20:57:39.000000 serra-0.7/serra/runners/graph_runner.py
--rw-r--r--   0 alanwang   (501) staff       (20)      443 2023-08-01 20:57:39.000000 serra-0.7/serra/tests.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.225819 serra-0.7/serra/transformers/
--rw-r--r--   0 alanwang   (501) staff       (20)      624 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)      928 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/add_column_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      631 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/case_when_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      460 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/cast_columns_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      601 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/drop_columns_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      623 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/filter_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      637 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/get_count_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1288 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/join_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1947 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/map_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1255 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/pivot_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      700 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/rename_column_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1091 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/select_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      310 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1967 2023-08-01 20:57:39.000000 serra-0.7/serra/translate_client.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2293 2023-08-01 20:57:39.000000 serra-0.7/serra/utils.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.227557 serra-0.7/serra/writers/
--rw-r--r--   0 alanwang   (501) staff       (20)      232 2023-08-01 20:57:39.000000 serra-0.7/serra/writers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1421 2023-08-01 20:57:39.000000 serra-0.7/serra/writers/amazon_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      678 2023-08-01 20:57:39.000000 serra-0.7/serra/writers/databricks_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      508 2023-08-01 20:57:39.000000 serra-0.7/serra/writers/local_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      569 2023-08-01 20:57:39.000000 serra-0.7/serra/writers/s3_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     3048 2023-08-01 20:57:39.000000 serra-0.7/serra/writers/snowflake_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      284 2023-08-01 20:57:39.000000 serra-0.7/serra/writers/writer.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.216983 serra-0.7/serra.egg-info/
--rw-r--r--   0 alanwang   (501) staff       (20)      240 2023-08-01 20:59:29.000000 serra-0.7/serra.egg-info/PKG-INFO
--rw-r--r--   0 alanwang   (501) staff       (20)     3366 2023-08-01 20:59:29.000000 serra-0.7/serra.egg-info/SOURCES.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-08-01 20:59:29.000000 serra-0.7/serra.egg-info/dependency_links.txt
--rw-r--r--   0 alanwang   (501) staff       (20)       88 2023-08-01 20:59:29.000000 serra-0.7/serra.egg-info/entry_points.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-08-01 20:58:40.000000 serra-0.7/serra.egg-info/not-zip-safe
--rw-r--r--   0 alanwang   (501) staff       (20)       83 2023-08-01 20:59:29.000000 serra-0.7/serra.egg-info/requires.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        6 2023-08-01 20:59:29.000000 serra-0.7/serra.egg-info/top_level.txt
--rw-r--r--   0 alanwang   (501) staff       (20)       38 2023-08-01 20:59:29.227991 serra-0.7/setup.cfg
--rw-r--r--   0 alanwang   (501) staff       (20)      918 2023-08-01 20:59:24.000000 serra-0.7/setup.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.706422 serra-0.7.1/
+-rw-r--r--   0 alanwang   (501) staff       (20)     3860 2023-08-01 20:57:39.000000 serra-0.7.1/LICENSE.md
+-rw-r--r--   0 alanwang   (501) staff       (20)      242 2023-08-01 21:22:37.706051 serra-0.7.1/PKG-INFO
+-rw-r--r--   0 alanwang   (501) staff       (20)     4478 2023-08-01 20:57:39.000000 serra-0.7.1/README.md
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.694127 serra-0.7.1/serra/
+-rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-08-01 20:57:39.000000 serra-0.7.1/serra/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2006 2023-08-01 20:57:39.000000 serra-0.7.1/serra/aws.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1872 2023-08-01 20:57:39.000000 serra-0.7.1/serra/cli.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      252 2023-08-01 20:57:39.000000 serra-0.7.1/serra/config.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1788 2023-08-01 20:57:39.000000 serra-0.7.1/serra/config_parser.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.691014 serra-0.7.1/serra/data/
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.695679 serra-0.7.1/serra/data/autocomplete/
+-rw-r--r--   0 alanwang   (501) staff       (20)     1110 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/README.md
+-rw-r--r--   0 alanwang   (501) staff       (20)     1636 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/gen_schemas.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.695809 serra-0.7.1/serra/data/autocomplete/inputs/
+-rw-r--r--   0 alanwang   (501) staff       (20)     2249 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/inputs/specs.json
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.698058 serra-0.7.1/serra/data/autocomplete/output/
+-rw-r--r--   0 alanwang   (501) staff       (20)      391 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/AddColumnTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      276 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/AmazonS3Reader.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      341 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/AmazonS3Writer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      267 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/CaseWhenTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      216 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/CastColumnTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      206 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/DatabricksReader.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      389 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/DatabricksWriter.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      213 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/DropColumnTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      274 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/GetCountTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      354 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/JoinTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      148 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/LocalReader.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      213 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/LocalWriter.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      331 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/MapTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      408 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/PivotTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      274 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/RenameColumnTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      210 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/SelectTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/SnowflakeWriter.json
+-rw-r--r--   0 alanwang   (501) staff       (20)     7553 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/serra_yaml_schema.json
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.698540 serra-0.7.1/serra/data/autocomplete/templates/
+-rw-r--r--   0 alanwang   (501) staff       (20)      326 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/templates/schema_template.json
+-rw-r--r--   0 alanwang   (501) staff       (20)       95 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/templates/transformer_template.json
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.698911 serra-0.7.1/serra/data/workspace_example/
+-rw-r--r--   0 alanwang   (501) staff       (20)      137 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/README.md
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.699464 serra-0.7.1/serra/data/workspace_example/examples/
+-rw-r--r--   0 alanwang   (501) staff       (20)     1610 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/examples/ratings.csv
+-rw-r--r--   0 alanwang   (501) staff       (20)     6706 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/examples/sales.csv
+-rw-r--r--   0 alanwang   (501) staff       (20)     1124 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/examples/states_to_abbreviation.json
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.700328 serra-0.7.1/serra/data/workspace_example/jobs/
+-rw-r--r--   0 alanwang   (501) staff       (20)      912 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/jobs/CloudDemo.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      945 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/jobs/Demo.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      418 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/jobs/LocalExample.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      220 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/jobs/ReadExample.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      456 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/jobs/ReadJoinWrite.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      393 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/jobs/ReadMapWrite.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      397 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/jobs/ReadPivotWrite.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      323 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/profiles.yml
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.700591 serra-0.7.1/serra/data/workspace_example/sql/
+-rw-r--r--   0 alanwang   (501) staff       (20)     2603 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/sql/easy_demo.sql
+-rw-r--r--   0 alanwang   (501) staff       (20)     2909 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/sql/hard_demo.sql
+-rw-r--r--   0 alanwang   (501) staff       (20)     2964 2023-08-01 20:57:39.000000 serra-0.7.1/serra/databricks.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      106 2023-08-01 20:57:39.000000 serra-0.7.1/serra/exceptions.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1120 2023-08-01 20:57:39.000000 serra-0.7.1/serra/profile.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.701647 serra-0.7.1/serra/readers/
+-rw-r--r--   0 alanwang   (501) staff       (20)      233 2023-08-01 20:57:39.000000 serra-0.7.1/serra/readers/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1457 2023-08-01 20:57:39.000000 serra-0.7.1/serra/readers/amazon_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      579 2023-08-01 20:57:39.000000 serra-0.7.1/serra/readers/databricks_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      501 2023-08-01 20:57:39.000000 serra-0.7.1/serra/readers/local_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      277 2023-08-01 20:57:39.000000 serra-0.7.1/serra/readers/reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-08-01 20:57:39.000000 serra-0.7.1/serra/readers/s3_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1380 2023-08-01 20:57:39.000000 serra-0.7.1/serra/readers/snowflaker_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2977 2023-08-01 20:57:39.000000 serra-0.7.1/serra/run.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.702033 serra-0.7.1/serra/runners/
+-rw-r--r--   0 alanwang   (501) staff       (20)     2631 2023-08-01 20:57:39.000000 serra-0.7.1/serra/runners/ExecutionGraph.py
+-rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-08-01 20:57:39.000000 serra-0.7.1/serra/runners/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     3148 2023-08-01 20:57:39.000000 serra-0.7.1/serra/runners/graph_runner.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      443 2023-08-01 20:57:39.000000 serra-0.7.1/serra/tests.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.704734 serra-0.7.1/serra/transformers/
+-rw-r--r--   0 alanwang   (501) staff       (20)      624 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      928 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/add_column_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      631 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/case_when_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      460 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/cast_columns_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      601 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/drop_columns_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      623 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/filter_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      637 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/get_count_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1288 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/join_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1947 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/map_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1255 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/pivot_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      700 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/rename_column_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1091 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/select_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      310 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1967 2023-08-01 20:57:39.000000 serra-0.7.1/serra/translate_client.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2293 2023-08-01 20:57:39.000000 serra-0.7.1/serra/utils.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.705824 serra-0.7.1/serra/writers/
+-rw-r--r--   0 alanwang   (501) staff       (20)      232 2023-08-01 20:57:39.000000 serra-0.7.1/serra/writers/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1421 2023-08-01 20:57:39.000000 serra-0.7.1/serra/writers/amazon_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      678 2023-08-01 20:57:39.000000 serra-0.7.1/serra/writers/databricks_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      508 2023-08-01 20:57:39.000000 serra-0.7.1/serra/writers/local_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      569 2023-08-01 20:57:39.000000 serra-0.7.1/serra/writers/s3_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     3048 2023-08-01 20:57:39.000000 serra-0.7.1/serra/writers/snowflake_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      284 2023-08-01 20:57:39.000000 serra-0.7.1/serra/writers/writer.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.695289 serra-0.7.1/serra.egg-info/
+-rw-r--r--   0 alanwang   (501) staff       (20)      242 2023-08-01 21:22:37.000000 serra-0.7.1/serra.egg-info/PKG-INFO
+-rw-r--r--   0 alanwang   (501) staff       (20)     3366 2023-08-01 21:22:37.000000 serra-0.7.1/serra.egg-info/SOURCES.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-08-01 21:22:37.000000 serra-0.7.1/serra.egg-info/dependency_links.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)       88 2023-08-01 21:22:37.000000 serra-0.7.1/serra.egg-info/entry_points.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-08-01 20:58:40.000000 serra-0.7.1/serra.egg-info/not-zip-safe
+-rw-r--r--   0 alanwang   (501) staff       (20)       83 2023-08-01 21:22:37.000000 serra-0.7.1/serra.egg-info/requires.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)        6 2023-08-01 21:22:37.000000 serra-0.7.1/serra.egg-info/top_level.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)       38 2023-08-01 21:22:37.706525 serra-0.7.1/setup.cfg
+-rw-r--r--   0 alanwang   (501) staff       (20)      920 2023-08-01 21:22:33.000000 serra-0.7.1/setup.py
```

### Comparing `serra-0.7/LICENSE.md` & `serra-0.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `serra-0.7/README.md` & `serra-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/aws.py` & `serra-0.7.1/serra/aws.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/cli.py` & `serra-0.7.1/serra/cli.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/config_parser.py` & `serra-0.7.1/serra/config_parser.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/data/autocomplete/README.md` & `serra-0.7.1/serra/data/autocomplete/README.md`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/data/autocomplete/gen_schemas.py` & `serra-0.7.1/serra/data/autocomplete/gen_schemas.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/data/autocomplete/inputs/specs.json` & `serra-0.7.1/serra/data/autocomplete/inputs/specs.json`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/data/autocomplete/output/serra_yaml_schema.json` & `serra-0.7.1/serra/data/autocomplete/output/serra_yaml_schema.json`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/data/workspace_example/examples/ratings.csv` & `serra-0.7.1/serra/data/workspace_example/examples/ratings.csv`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/data/workspace_example/examples/sales.csv` & `serra-0.7.1/serra/data/workspace_example/examples/sales.csv`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/data/workspace_example/examples/states_to_abbreviation.json` & `serra-0.7.1/serra/data/workspace_example/examples/states_to_abbreviation.json`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/data/workspace_example/jobs/CloudDemo.yml` & `serra-0.7.1/serra/data/workspace_example/jobs/CloudDemo.yml`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/data/workspace_example/jobs/Demo.yml` & `serra-0.7.1/serra/data/workspace_example/jobs/Demo.yml`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/data/workspace_example/sql/easy_demo.sql` & `serra-0.7.1/serra/data/workspace_example/sql/easy_demo.sql`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/data/workspace_example/sql/hard_demo.sql` & `serra-0.7.1/serra/data/workspace_example/sql/hard_demo.sql`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/databricks.py` & `serra-0.7.1/serra/databricks.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/profile.py` & `serra-0.7.1/serra/profile.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/readers/amazon_reader.py` & `serra-0.7.1/serra/readers/amazon_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/readers/databricks_reader.py` & `serra-0.7.1/serra/readers/databricks_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/readers/snowflaker_reader.py` & `serra-0.7.1/serra/readers/snowflaker_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/run.py` & `serra-0.7.1/serra/run.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/runners/ExecutionGraph.py` & `serra-0.7.1/serra/runners/ExecutionGraph.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/runners/graph_runner.py` & `serra-0.7.1/serra/runners/graph_runner.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/transformers/__init__.py` & `serra-0.7.1/serra/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/transformers/add_column_transformer.py` & `serra-0.7.1/serra/transformers/add_column_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/transformers/case_when_transformer.py` & `serra-0.7.1/serra/transformers/case_when_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/transformers/drop_columns_transformer.py` & `serra-0.7.1/serra/transformers/drop_columns_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/transformers/filter_transformer.py` & `serra-0.7.1/serra/transformers/filter_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/transformers/get_count_transformer.py` & `serra-0.7.1/serra/transformers/get_count_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/transformers/join_transformer.py` & `serra-0.7.1/serra/transformers/join_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/transformers/map_transformer.py` & `serra-0.7.1/serra/transformers/map_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/transformers/pivot_transformer.py` & `serra-0.7.1/serra/transformers/pivot_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/transformers/rename_column_transformer.py` & `serra-0.7.1/serra/transformers/rename_column_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/transformers/select_transformer.py` & `serra-0.7.1/serra/transformers/select_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/translate_client.py` & `serra-0.7.1/serra/translate_client.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/utils.py` & `serra-0.7.1/serra/utils.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/writers/amazon_writer.py` & `serra-0.7.1/serra/writers/amazon_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/writers/databricks_writer.py` & `serra-0.7.1/serra/writers/databricks_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/writers/s3_writer.py` & `serra-0.7.1/serra/writers/s3_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra/writers/snowflake_writer.py` & `serra-0.7.1/serra/writers/snowflake_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7/serra.egg-info/SOURCES.txt` & `serra-0.7.1/serra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serra-0.7/setup.py` & `serra-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 from setuptools import setup
 
 setup(name='serra',
-      version='0.7',
+      version='0.7.1',
       description='Simplified Data Pipelines',
       url='http://github.com',
       author='Serra Technologies',
       author_email='founders@serra.io',
       packages=setuptools.find_packages(),
       package_data={"serra": ["data/workspace_example/*",
                               "data/workspace_example/*/*",
```

