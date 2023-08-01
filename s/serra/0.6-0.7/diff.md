# Comparing `tmp/serra-0.6.tar.gz` & `tmp/serra-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serra-0.6.tar", last modified: Mon Jul 31 04:59:18 2023, max compression
+gzip compressed data, was "serra-0.7.tar", last modified: Tue Aug  1 20:59:29 2023, max compression
```

## Comparing `serra-0.6.tar` & `serra-0.7.tar`

### file list

```diff
@@ -1,105 +1,107 @@
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.424116 serra-0.6/
--rw-r--r--   0 alanwang   (501) staff       (20)     3860 2023-07-31 04:49:36.000000 serra-0.6/LICENSE.md
--rw-r--r--   0 alanwang   (501) staff       (20)      240 2023-07-31 04:59:18.423978 serra-0.6/PKG-INFO
--rw-r--r--   0 alanwang   (501) staff       (20)     3852 2023-07-31 04:49:36.000000 serra-0.6/README.md
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.414281 serra-0.6/serra/
--rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-07-31 04:49:36.000000 serra-0.6/serra/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2006 2023-07-31 04:49:36.000000 serra-0.6/serra/aws.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1872 2023-07-31 04:49:36.000000 serra-0.6/serra/cli.py
--rw-r--r--   0 alanwang   (501) staff       (20)      222 2023-07-31 04:49:36.000000 serra-0.6/serra/config.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1782 2023-07-31 04:49:36.000000 serra-0.6/serra/config_parser.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.411594 serra-0.6/serra/data/
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.415671 serra-0.6/serra/data/autocomplete/
--rw-r--r--   0 alanwang   (501) staff       (20)     1110 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/README.md
--rw-r--r--   0 alanwang   (501) staff       (20)     1636 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/gen_schemas.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.415783 serra-0.6/serra/data/autocomplete/inputs/
--rw-r--r--   0 alanwang   (501) staff       (20)     2249 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/inputs/specs.json
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.418356 serra-0.6/serra/data/autocomplete/output/
--rw-r--r--   0 alanwang   (501) staff       (20)      391 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/AddColumnTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      276 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/AmazonS3Reader.json
--rw-r--r--   0 alanwang   (501) staff       (20)      341 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/AmazonS3Writer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      267 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/CaseWhenTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      216 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/CastColumnTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      206 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/DatabricksReader.json
--rw-r--r--   0 alanwang   (501) staff       (20)      389 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/DatabricksWriter.json
--rw-r--r--   0 alanwang   (501) staff       (20)      213 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/DropColumnTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      274 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/GetCountTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      354 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/JoinTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      148 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/LocalReader.json
--rw-r--r--   0 alanwang   (501) staff       (20)      213 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/LocalWriter.json
--rw-r--r--   0 alanwang   (501) staff       (20)      331 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/MapTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      408 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/PivotTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      274 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/RenameColumnTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      210 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/SelectTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/SnowflakeWriter.json
--rw-r--r--   0 alanwang   (501) staff       (20)     7553 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/serra_yaml_schema.json
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.418594 serra-0.6/serra/data/autocomplete/templates/
--rw-r--r--   0 alanwang   (501) staff       (20)      326 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/templates/schema_template.json
--rw-r--r--   0 alanwang   (501) staff       (20)       95 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/templates/transformer_template.json
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.418820 serra-0.6/serra/data/workspace_example/
--rw-r--r--   0 alanwang   (501) staff       (20)      137 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/README.md
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.419206 serra-0.6/serra/data/workspace_example/examples/
--rw-r--r--   0 alanwang   (501) staff       (20)     1610 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/examples/ratings.csv
--rw-r--r--   0 alanwang   (501) staff       (20)     6706 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/examples/sales.csv
--rw-r--r--   0 alanwang   (501) staff       (20)     1124 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/examples/states_to_abbreviation.json
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.420030 serra-0.6/serra/data/workspace_example/jobs/
--rw-r--r--   0 alanwang   (501) staff       (20)     1984 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/jobs/Demo.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      415 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/jobs/LocalExample.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      220 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/jobs/ReadExample.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      456 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/jobs/ReadJoinWrite.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      393 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/jobs/ReadMapWrite.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      397 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/jobs/ReadPivotWrite.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      224 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/profiles.yml
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.420322 serra-0.6/serra/data/workspace_example/sql/
--rw-r--r--   0 alanwang   (501) staff       (20)     2603 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/sql/easy_demo.sql
--rw-r--r--   0 alanwang   (501) staff       (20)     2909 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/sql/hard_demo.sql
--rw-r--r--   0 alanwang   (501) staff       (20)     2964 2023-07-31 04:49:36.000000 serra-0.6/serra/databricks.py
--rw-r--r--   0 alanwang   (501) staff       (20)      106 2023-07-31 04:49:36.000000 serra-0.6/serra/exceptions.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1120 2023-07-31 04:49:36.000000 serra-0.6/serra/profile.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.421139 serra-0.6/serra/readers/
--rw-r--r--   0 alanwang   (501) staff       (20)      233 2023-07-31 04:49:36.000000 serra-0.6/serra/readers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1457 2023-07-31 04:49:36.000000 serra-0.6/serra/readers/amazon_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      579 2023-07-31 04:49:36.000000 serra-0.6/serra/readers/databricks_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      501 2023-07-31 04:49:36.000000 serra-0.6/serra/readers/local_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      277 2023-07-31 04:49:36.000000 serra-0.6/serra/readers/reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-07-31 04:49:36.000000 serra-0.6/serra/readers/s3_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1380 2023-07-31 04:49:36.000000 serra-0.6/serra/readers/snowflaker_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2977 2023-07-31 04:49:36.000000 serra-0.6/serra/run.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.421495 serra-0.6/serra/runners/
--rw-r--r--   0 alanwang   (501) staff       (20)     2631 2023-07-31 04:49:36.000000 serra-0.6/serra/runners/ExecutionGraph.py
--rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-07-31 04:49:36.000000 serra-0.6/serra/runners/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     3181 2023-07-31 04:49:36.000000 serra-0.6/serra/runners/graph_runner.py
--rw-r--r--   0 alanwang   (501) staff       (20)      443 2023-07-31 04:49:36.000000 serra-0.6/serra/tests.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.422957 serra-0.6/serra/transformers/
--rw-r--r--   0 alanwang   (501) staff       (20)      574 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)      928 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/add_column_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      631 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/case_when_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      460 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/cast_columns_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      601 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/drop_columns_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      637 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/get_count_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1288 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/join_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1808 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/map_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1178 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/pivot_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      700 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/rename_column_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1091 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/select_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      310 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1967 2023-07-31 04:49:36.000000 serra-0.6/serra/translate_client.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2293 2023-07-31 04:49:36.000000 serra-0.6/serra/utils.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.423775 serra-0.6/serra/writers/
--rw-r--r--   0 alanwang   (501) staff       (20)      232 2023-07-31 04:49:36.000000 serra-0.6/serra/writers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1421 2023-07-31 04:49:36.000000 serra-0.6/serra/writers/amazon_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      678 2023-07-31 04:49:36.000000 serra-0.6/serra/writers/databricks_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      508 2023-07-31 04:49:36.000000 serra-0.6/serra/writers/local_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      569 2023-07-31 04:49:36.000000 serra-0.6/serra/writers/s3_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     3048 2023-07-31 04:49:36.000000 serra-0.6/serra/writers/snowflake_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      284 2023-07-31 04:49:36.000000 serra-0.6/serra/writers/writer.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.415432 serra-0.6/serra.egg-info/
--rw-r--r--   0 alanwang   (501) staff       (20)      240 2023-07-31 04:59:18.000000 serra-0.6/serra.egg-info/PKG-INFO
--rw-r--r--   0 alanwang   (501) staff       (20)     3277 2023-07-31 04:59:18.000000 serra-0.6/serra.egg-info/SOURCES.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-07-31 04:59:18.000000 serra-0.6/serra.egg-info/dependency_links.txt
--rw-r--r--   0 alanwang   (501) staff       (20)       88 2023-07-31 04:59:18.000000 serra-0.6/serra.egg-info/entry_points.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-07-31 04:59:18.000000 serra-0.6/serra.egg-info/not-zip-safe
--rw-r--r--   0 alanwang   (501) staff       (20)       83 2023-07-31 04:59:18.000000 serra-0.6/serra.egg-info/requires.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        6 2023-07-31 04:59:18.000000 serra-0.6/serra.egg-info/top_level.txt
--rw-r--r--   0 alanwang   (501) staff       (20)       38 2023-07-31 04:59:18.424157 serra-0.6/setup.cfg
--rw-r--r--   0 alanwang   (501) staff       (20)      918 2023-07-31 04:50:45.000000 serra-0.6/setup.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.227937 serra-0.7/
+-rw-r--r--   0 alanwang   (501) staff       (20)     3860 2023-08-01 20:57:39.000000 serra-0.7/LICENSE.md
+-rw-r--r--   0 alanwang   (501) staff       (20)      240 2023-08-01 20:59:29.227796 serra-0.7/PKG-INFO
+-rw-r--r--   0 alanwang   (501) staff       (20)     4478 2023-08-01 20:57:39.000000 serra-0.7/README.md
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.215528 serra-0.7/serra/
+-rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-08-01 20:57:39.000000 serra-0.7/serra/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2006 2023-08-01 20:57:39.000000 serra-0.7/serra/aws.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1872 2023-08-01 20:57:39.000000 serra-0.7/serra/cli.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      252 2023-08-01 20:57:39.000000 serra-0.7/serra/config.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1788 2023-08-01 20:57:39.000000 serra-0.7/serra/config_parser.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.213189 serra-0.7/serra/data/
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.217335 serra-0.7/serra/data/autocomplete/
+-rw-r--r--   0 alanwang   (501) staff       (20)     1110 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/README.md
+-rw-r--r--   0 alanwang   (501) staff       (20)     1636 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/gen_schemas.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.217472 serra-0.7/serra/data/autocomplete/inputs/
+-rw-r--r--   0 alanwang   (501) staff       (20)     2249 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/inputs/specs.json
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.219812 serra-0.7/serra/data/autocomplete/output/
+-rw-r--r--   0 alanwang   (501) staff       (20)      391 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/AddColumnTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      276 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/AmazonS3Reader.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      341 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/AmazonS3Writer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      267 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/CaseWhenTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      216 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/CastColumnTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      206 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/DatabricksReader.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      389 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/DatabricksWriter.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      213 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/DropColumnTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      274 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/GetCountTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      354 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/JoinTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      148 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/LocalReader.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      213 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/LocalWriter.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      331 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/MapTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      408 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/PivotTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      274 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/RenameColumnTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      210 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/SelectTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/SnowflakeWriter.json
+-rw-r--r--   0 alanwang   (501) staff       (20)     7553 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/output/serra_yaml_schema.json
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.220044 serra-0.7/serra/data/autocomplete/templates/
+-rw-r--r--   0 alanwang   (501) staff       (20)      326 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/templates/schema_template.json
+-rw-r--r--   0 alanwang   (501) staff       (20)       95 2023-08-01 20:57:39.000000 serra-0.7/serra/data/autocomplete/templates/transformer_template.json
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.220286 serra-0.7/serra/data/workspace_example/
+-rw-r--r--   0 alanwang   (501) staff       (20)      137 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/README.md
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.220666 serra-0.7/serra/data/workspace_example/examples/
+-rw-r--r--   0 alanwang   (501) staff       (20)     1610 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/examples/ratings.csv
+-rw-r--r--   0 alanwang   (501) staff       (20)     6706 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/examples/sales.csv
+-rw-r--r--   0 alanwang   (501) staff       (20)     1124 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/examples/states_to_abbreviation.json
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.221568 serra-0.7/serra/data/workspace_example/jobs/
+-rw-r--r--   0 alanwang   (501) staff       (20)      912 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/jobs/CloudDemo.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      945 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/jobs/Demo.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      418 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/jobs/LocalExample.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      220 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/jobs/ReadExample.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      456 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/jobs/ReadJoinWrite.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      393 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/jobs/ReadMapWrite.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      397 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/jobs/ReadPivotWrite.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      323 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/profiles.yml
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.221811 serra-0.7/serra/data/workspace_example/sql/
+-rw-r--r--   0 alanwang   (501) staff       (20)     2603 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/sql/easy_demo.sql
+-rw-r--r--   0 alanwang   (501) staff       (20)     2909 2023-08-01 20:57:39.000000 serra-0.7/serra/data/workspace_example/sql/hard_demo.sql
+-rw-r--r--   0 alanwang   (501) staff       (20)     2964 2023-08-01 20:57:39.000000 serra-0.7/serra/databricks.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      106 2023-08-01 20:57:39.000000 serra-0.7/serra/exceptions.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1120 2023-08-01 20:57:39.000000 serra-0.7/serra/profile.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.222633 serra-0.7/serra/readers/
+-rw-r--r--   0 alanwang   (501) staff       (20)      233 2023-08-01 20:57:39.000000 serra-0.7/serra/readers/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1457 2023-08-01 20:57:39.000000 serra-0.7/serra/readers/amazon_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      579 2023-08-01 20:57:39.000000 serra-0.7/serra/readers/databricks_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      501 2023-08-01 20:57:39.000000 serra-0.7/serra/readers/local_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      277 2023-08-01 20:57:39.000000 serra-0.7/serra/readers/reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-08-01 20:57:39.000000 serra-0.7/serra/readers/s3_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1380 2023-08-01 20:57:39.000000 serra-0.7/serra/readers/snowflaker_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2977 2023-08-01 20:57:39.000000 serra-0.7/serra/run.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.223262 serra-0.7/serra/runners/
+-rw-r--r--   0 alanwang   (501) staff       (20)     2631 2023-08-01 20:57:39.000000 serra-0.7/serra/runners/ExecutionGraph.py
+-rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-08-01 20:57:39.000000 serra-0.7/serra/runners/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     3148 2023-08-01 20:57:39.000000 serra-0.7/serra/runners/graph_runner.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      443 2023-08-01 20:57:39.000000 serra-0.7/serra/tests.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.225819 serra-0.7/serra/transformers/
+-rw-r--r--   0 alanwang   (501) staff       (20)      624 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      928 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/add_column_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      631 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/case_when_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      460 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/cast_columns_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      601 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/drop_columns_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      623 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/filter_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      637 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/get_count_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1288 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/join_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1947 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/map_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1255 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/pivot_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      700 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/rename_column_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1091 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/select_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      310 2023-08-01 20:57:39.000000 serra-0.7/serra/transformers/transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1967 2023-08-01 20:57:39.000000 serra-0.7/serra/translate_client.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2293 2023-08-01 20:57:39.000000 serra-0.7/serra/utils.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.227557 serra-0.7/serra/writers/
+-rw-r--r--   0 alanwang   (501) staff       (20)      232 2023-08-01 20:57:39.000000 serra-0.7/serra/writers/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1421 2023-08-01 20:57:39.000000 serra-0.7/serra/writers/amazon_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      678 2023-08-01 20:57:39.000000 serra-0.7/serra/writers/databricks_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      508 2023-08-01 20:57:39.000000 serra-0.7/serra/writers/local_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      569 2023-08-01 20:57:39.000000 serra-0.7/serra/writers/s3_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     3048 2023-08-01 20:57:39.000000 serra-0.7/serra/writers/snowflake_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      284 2023-08-01 20:57:39.000000 serra-0.7/serra/writers/writer.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 20:59:29.216983 serra-0.7/serra.egg-info/
+-rw-r--r--   0 alanwang   (501) staff       (20)      240 2023-08-01 20:59:29.000000 serra-0.7/serra.egg-info/PKG-INFO
+-rw-r--r--   0 alanwang   (501) staff       (20)     3366 2023-08-01 20:59:29.000000 serra-0.7/serra.egg-info/SOURCES.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-08-01 20:59:29.000000 serra-0.7/serra.egg-info/dependency_links.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)       88 2023-08-01 20:59:29.000000 serra-0.7/serra.egg-info/entry_points.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-08-01 20:58:40.000000 serra-0.7/serra.egg-info/not-zip-safe
+-rw-r--r--   0 alanwang   (501) staff       (20)       83 2023-08-01 20:59:29.000000 serra-0.7/serra.egg-info/requires.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)        6 2023-08-01 20:59:29.000000 serra-0.7/serra.egg-info/top_level.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)       38 2023-08-01 20:59:29.227991 serra-0.7/setup.cfg
+-rw-r--r--   0 alanwang   (501) staff       (20)      918 2023-08-01 20:59:24.000000 serra-0.7/setup.py
```

### Comparing `serra-0.6/LICENSE.md` & `serra-0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `serra-0.6/README.md` & `serra-0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Serra.
 
 ```bash
-pip install serra==0.5
+pip install serra==0.6
 ```
 
 # Setup
 
 Setup your virtual environment below.
 
 ```bash
@@ -34,22 +34,50 @@
 or
 
 ```bash
 source run.sh
 ```
 
 # Getting Started
-Navigate to the workspace_example folder and try out a couple of jobs!
+Run `serra create` to create a workspace folder. 
 
 ```bash
-cd workspace_example
-serra run LocalExample
+serra create
 ```
+
+Navigate to the workspace folder and run your first job!
+
+```bash
+cd workspace
+serra run Demo
+```
+
 Other jobs available can be found in the **workspace_example/jobs** folder.
 
+# Connector Credentials
+Update your credentials for AWS, Databricks, and Snowflake in `workspace/profiles.yml`
+
+```
+AWS Access Key ID: [YOUR ACCESS KEY]
+AWS Secret Access Key: [YOUR SECRET ACCESS KEY]
+
+AWS_CONFIG_BUCKET: ENTER_HERE # Bucket to use to place job config files (not needed for quickstart)
+
+DATABRICKS_HOST: ENTER_HERE
+DATABRICKS_TOKEN: ENTER_HERE
+DATABRICKS_CLUSTER_ID: ENTER_HERE
+
+SNOWFLAKE:
+  USER: ENTER_HERE
+  PASSWORD: ENTER_HERE
+  ACCOUNT: ENTER_HERE (Organization-Account)
+```
+
+Now your jobs can connect between AWS, Databricks, and Snowflake data sources!
+
 # SQL to Serra LLM (Beta)
 Translate monolithic SQL scripts to low-code, Serra spark configuration files with one line.
 
 ```bash
 cd workspace_example
 serra translate hard_demo.sql
 ```
```

### Comparing `serra-0.6/serra/aws.py` & `serra-0.7/serra/aws.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/cli.py` & `serra-0.7/serra/cli.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/config_parser.py` & `serra-0.7/serra/config_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,19 +40,19 @@
         return keys[0]
     
     def get_config_for_step(self, block_name):
         step = self.get_step(block_name)
         return step.get("config")
     
     def get_blocks(self):
-        blocks = [name for name in self.config.keys() if name != 'debug']
+        blocks = [name for name in self.config.keys() if name != 'show_all']
         return blocks
     
     def get_config_for_block(self, block_name):
         class_name = self.get_class_name_for_step(block_name)
         return self.config.get(block_name).get(class_name)
     
     def get_tests_for_block(self, block_name):
         return self.config.get(block_name).get("tests")
     
-    def get_test(self):
-        return self.config.get('debug')
+    def show_all(self):
+        return self.config.get('show_all')
```

### Comparing `serra-0.6/serra/data/autocomplete/README.md` & `serra-0.7/serra/data/autocomplete/README.md`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/data/autocomplete/gen_schemas.py` & `serra-0.7/serra/data/autocomplete/gen_schemas.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/data/autocomplete/inputs/specs.json` & `serra-0.7/serra/data/autocomplete/inputs/specs.json`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/data/autocomplete/output/serra_yaml_schema.json` & `serra-0.7/serra/data/autocomplete/output/serra_yaml_schema.json`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/data/workspace_example/examples/ratings.csv` & `serra-0.7/serra/data/workspace_example/examples/ratings.csv`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/data/workspace_example/examples/sales.csv` & `serra-0.7/serra/data/workspace_example/examples/sales.csv`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/data/workspace_example/examples/states_to_abbreviation.json` & `serra-0.7/serra/data/workspace_example/examples/states_to_abbreviation.json`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/data/workspace_example/sql/easy_demo.sql` & `serra-0.7/serra/data/workspace_example/sql/easy_demo.sql`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/data/workspace_example/sql/hard_demo.sql` & `serra-0.7/serra/data/workspace_example/sql/hard_demo.sql`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/databricks.py` & `serra-0.7/serra/databricks.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/profile.py` & `serra-0.7/serra/profile.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/readers/amazon_reader.py` & `serra-0.7/serra/readers/amazon_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/readers/databricks_reader.py` & `serra-0.7/serra/readers/databricks_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/readers/snowflaker_reader.py` & `serra-0.7/serra/readers/snowflaker_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/run.py` & `serra-0.7/serra/run.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/runners/ExecutionGraph.py` & `serra-0.7/serra/runners/ExecutionGraph.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/runners/graph_runner.py` & `serra-0.7/serra/runners/graph_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
         if is_reader(block_name, cf):
             df = block_obj.read()
             df_map[block_name] = df
         elif is_writer(block_name, cf):
             assert len(block_obj.dependencies) == 1
             dependency = block_obj.dependencies[0]
-            block_obj.write(df_map[dependency]) # Get the 
+            block_obj.write(df_map[dependency])
         elif is_Transformer(block_name, cf):
             assert len(block_obj.dependencies) >= 1
             input_dfs = [df_map[dep] for dep in block_obj.dependencies]
             df = block_obj.transform(*input_dfs)
             df_map[block_name] = df
 
         if cf.get_tests_for_block(block_name) is not None:
@@ -74,13 +74,13 @@
                 logger.info(f"\tRunning test {test_name}")
                 if test_name == 'nulls':
                     df = df_map[block_name]
                     nulls_test(df)
                 if test_name == 'duplicates':
                     df = df_map[block_name]
                     duplicates_test(df)
-    
-    df_map[dependency].show()
 
-    if cf.get_test():
-        logger.info("Debug is true—printing out rows.")
+    if cf.show_all():
+        logger.info("Showing 500 rows...")
         df.show(500)
+    else:
+        df.show()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `serra-0.6/serra/transformers/__init__.py` & `serra-0.7/serra/transformers/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,8 +4,9 @@
 from .drop_columns_transformer import DropColumnTransformer
 from .get_count_transformer import GetCountTransformer
 from .join_transformer import JoinTransformer
 from .map_transformer import MapTransformer
 from .pivot_transformer import PivotTransformer
 from .rename_column_transformer import RenameColumnTransformer
 from .select_transformer import SelectTransformer
+from .filter_transformer import FilterTransformer
 from .transformer import Transformer
```

### Comparing `serra-0.6/serra/transformers/add_column_transformer.py` & `serra-0.7/serra/transformers/add_column_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/transformers/case_when_transformer.py` & `serra-0.7/serra/transformers/case_when_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/transformers/drop_columns_transformer.py` & `serra-0.7/serra/transformers/drop_columns_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/transformers/get_count_transformer.py` & `serra-0.7/serra/transformers/get_count_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/transformers/join_transformer.py` & `serra-0.7/serra/transformers/join_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/transformers/map_transformer.py` & `serra-0.7/serra/transformers/map_transformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pyspark.sql import functions as F
-
+import json
 from serra.transformers.transformer import Transformer
 from serra.exceptions import SerraRunException
 
 class MapTransformer(Transformer):
     """
     Test transformer to add a column to dataframe
     :param config: Holds column value
@@ -26,14 +26,18 @@
         
         if not self.map_dict and not self.map_dict_path:
             raise SerraRunException("Either 'map_dict' or 'map_dict_path' must be provided in the config.")
 
         if self.col_key not in df.columns:
             raise SerraRunException(f"Column '{self.col_key}' specified as col_key does not exist in the DataFrame.")
 
+        if self.map_dict is None:
+            with open(self.map_dict_path) as f:
+                self.map_dict = json.load(f)
+
         try:
             for key, value in self.map_dict.items():
                 df = df.withColumn(f'{self.name}_{key}', F.when(F.col(self.col_key) == key, value))
 
             # Select the first non-null value from the generated columns
             # create list, then unpack *
             df = df.withColumn(self.name, F.coalesce(*[F.col(f'{self.name}_{key}') for key in self.map_dict]))
```

### Comparing `serra-0.6/serra/transformers/pivot_transformer.py` & `serra-0.7/serra/transformers/pivot_transformer.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,17 +19,18 @@
         self.aggregate_type = config.get("aggregate_type")
 
     def transform(self, df):
         """
         Add column with col_value to dataframe
         :return; Dataframe w/ new column containing col_value
         """
-
-        df = df.groupBy(self.row_level).pivot(self.column_level)
         
+        df = df.withColumn(self.sum_col, F.col(self.sum_col).cast("double"))
+        df = df.groupBy(self.row_level).pivot(self.column_level)
+
         # Perform aggregation
         if self.aggregate_type == "avg":
             df = df.avg(self.sum_col)
         elif self.aggregate_type == "sum":
             df = df.sum(self.sum_col)
         else:
             raise SerraRunException("Invalid Pivot Aggregation type")
```

### Comparing `serra-0.6/serra/transformers/rename_column_transformer.py` & `serra-0.7/serra/transformers/rename_column_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/transformers/select_transformer.py` & `serra-0.7/serra/transformers/select_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/translate_client.py` & `serra-0.7/serra/translate_client.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/utils.py` & `serra-0.7/serra/utils.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/writers/amazon_writer.py` & `serra-0.7/serra/writers/amazon_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/writers/databricks_writer.py` & `serra-0.7/serra/writers/databricks_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/writers/s3_writer.py` & `serra-0.7/serra/writers/s3_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra/writers/snowflake_writer.py` & `serra-0.7/serra/writers/snowflake_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.6/serra.egg-info/SOURCES.txt` & `serra-0.7/serra.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 serra/data/autocomplete/templates/schema_template.json
 serra/data/autocomplete/templates/transformer_template.json
 serra/data/workspace_example/README.md
 serra/data/workspace_example/profiles.yml
 serra/data/workspace_example/examples/ratings.csv
 serra/data/workspace_example/examples/sales.csv
 serra/data/workspace_example/examples/states_to_abbreviation.json
+serra/data/workspace_example/jobs/CloudDemo.yml
 serra/data/workspace_example/jobs/Demo.yml
 serra/data/workspace_example/jobs/LocalExample.yml
 serra/data/workspace_example/jobs/ReadExample.yml
 serra/data/workspace_example/jobs/ReadJoinWrite.yml
 serra/data/workspace_example/jobs/ReadMapWrite.yml
 serra/data/workspace_example/jobs/ReadPivotWrite.yml
 serra/data/workspace_example/sql/easy_demo.sql
@@ -67,14 +68,15 @@
 serra/runners/__init__.py
 serra/runners/graph_runner.py
 serra/transformers/__init__.py
 serra/transformers/add_column_transformer.py
 serra/transformers/case_when_transformer.py
 serra/transformers/cast_columns_transformer.py
 serra/transformers/drop_columns_transformer.py
+serra/transformers/filter_transformer.py
 serra/transformers/get_count_transformer.py
 serra/transformers/join_transformer.py
 serra/transformers/map_transformer.py
 serra/transformers/pivot_transformer.py
 serra/transformers/rename_column_transformer.py
 serra/transformers/select_transformer.py
 serra/transformers/transformer.py
```

### Comparing `serra-0.6/setup.py` & `serra-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 from setuptools import setup
 
 setup(name='serra',
-      version='0.6',
+      version='0.7',
       description='Simplified Data Pipelines',
       url='http://github.com',
       author='Serra Technologies',
       author_email='founders@serra.io',
       packages=setuptools.find_packages(),
       package_data={"serra": ["data/workspace_example/*",
                               "data/workspace_example/*/*",
```

