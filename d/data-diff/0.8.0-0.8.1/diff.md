# Comparing `tmp/data_diff-0.8.0.tar.gz` & `tmp/data_diff-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_diff-0.8.0.tar", max compression
+gzip compressed data, was "data_diff-0.8.1.tar", max compression
```

## Comparing `data_diff-0.8.0.tar` & `data_diff-0.8.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.8.0/LICENSE
--rw-r--r--   0        0        0     2742 2023-07-27 16:41:55.956926 data_diff-0.8.0/README.md
--rw-r--r--   0        0        0     8710 2023-05-24 18:36:17.565800 data_diff-0.8.0/data_diff/__init__.py
--rw-r--r--   0        0        0    18130 2023-07-27 15:17:08.933362 data_diff-0.8.0/data_diff/__main__.py
--rw-r--r--   0        0        0      126 2023-05-15 21:10:13.082463 data_diff-0.8.0/data_diff/cloud/__init__.py
--rw-r--r--   0        0        0    11568 2023-06-16 19:57:48.275419 data_diff-0.8.0/data_diff/cloud/data_source.py
--rw-r--r--   0        0        0    10562 2023-07-25 19:31:06.998411 data_diff-0.8.0/data_diff/cloud/datafold_api.py
--rw-r--r--   0        0        0     4044 2023-04-03 18:06:26.931568 data_diff-0.8.0/data_diff/config.py
--rw-r--r--   0        0        0      493 2023-04-21 21:58:08.194615 data_diff-0.8.0/data_diff/databases/__init__.py
--rw-r--r--   0        0        0     1353 2023-04-21 21:58:08.194720 data_diff-0.8.0/data_diff/databases/_connect.py
--rw-r--r--   0        0        0      174 2023-04-21 21:58:08.194816 data_diff-0.8.0/data_diff/databases/base.py
--rw-r--r--   0        0        0      257 2023-04-21 21:58:08.195148 data_diff-0.8.0/data_diff/databases/bigquery.py
--rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195281 data_diff-0.8.0/data_diff/databases/clickhouse.py
--rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195390 data_diff-0.8.0/data_diff/databases/databricks.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195511 data_diff-0.8.0/data_diff/databases/duckdb.py
--rw-r--r--   0        0        0      236 2023-04-21 21:58:08.195617 data_diff-0.8.0/data_diff/databases/mysql.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195713 data_diff-0.8.0/data_diff/databases/oracle.py
--rw-r--r--   0        0        0      275 2023-04-21 21:58:08.195827 data_diff-0.8.0/data_diff/databases/postgresql.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195918 data_diff-0.8.0/data_diff/databases/presto.py
--rw-r--r--   0        0        0      257 2023-04-21 21:58:08.196013 data_diff-0.8.0/data_diff/databases/redshift.py
--rw-r--r--   0        0        0      264 2023-04-21 21:58:08.196109 data_diff-0.8.0/data_diff/databases/snowflake.py
--rw-r--r--   0        0        0      236 2023-04-21 21:58:08.196196 data_diff-0.8.0/data_diff/databases/trino.py
--rw-r--r--   0        0        0      250 2023-04-21 21:58:08.196288 data_diff-0.8.0/data_diff/databases/vertica.py
--rw-r--r--   0        0        0    19863 2023-07-27 15:25:50.449603 data_diff-0.8.0/data_diff/dbt.py
--rw-r--r--   0        0        0    20292 2023-07-27 15:17:08.934005 data_diff-0.8.0/data_diff/dbt_parser.py
--rw-r--r--   0        0        0    14471 2023-07-18 16:15:04.405684 data_diff-0.8.0/data_diff/diff_tables.py
--rw-r--r--   0        0        0     2411 2023-07-25 19:31:06.998680 data_diff-0.8.0/data_diff/errors.py
--rw-r--r--   0        0        0     9098 2023-07-16 03:33:52.656293 data_diff-0.8.0/data_diff/format.py
--rw-r--r--   0        0        0     9405 2023-06-27 22:04:20.813975 data_diff-0.8.0/data_diff/hashdiff_tables.py
--rw-r--r--   0        0        0     1917 2023-06-22 19:56:54.945638 data_diff-0.8.0/data_diff/info_tree.py
--rw-r--r--   0        0        0    15377 2023-06-22 19:56:54.946004 data_diff-0.8.0/data_diff/joindiff_tables.py
--rw-r--r--   0        0        0     7557 2023-04-03 18:06:26.932827 data_diff-0.8.0/data_diff/lexicographic_space.py
--rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.8.0/data_diff/parse_time.py
--rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.197181 data_diff-0.8.0/data_diff/query_utils.py
--rw-r--r--   0        0        0       76 2023-04-21 21:58:08.197422 data_diff-0.8.0/data_diff/sqeleton/__init__.py
--rw-r--r--   0        0        0      279 2023-04-21 21:58:08.197521 data_diff-0.8.0/data_diff/sqeleton/__main__.py
--rw-r--r--   0        0        0      264 2023-05-05 21:08:17.222879 data_diff-0.8.0/data_diff/sqeleton/abcs/__init__.py
--rw-r--r--   0        0        0      409 2023-04-21 21:58:08.197743 data_diff-0.8.0/data_diff/sqeleton/abcs/compiler.py
--rw-r--r--   0        0        0    11118 2023-05-05 21:08:17.223038 data_diff-0.8.0/data_diff/sqeleton/abcs/database_types.py
--rw-r--r--   0        0        0     7029 2023-06-27 22:04:20.814299 data_diff-0.8.0/data_diff/sqeleton/abcs/mixins.py
--rw-r--r--   0        0        0     2425 2023-04-21 21:58:08.198003 data_diff-0.8.0/data_diff/sqeleton/bound_exprs.py
--rw-r--r--   0        0        0      554 2023-04-21 21:58:08.198154 data_diff-0.8.0/data_diff/sqeleton/databases/__init__.py
--rw-r--r--   0        0        0     9245 2023-06-20 20:21:00.599502 data_diff-0.8.0/data_diff/sqeleton/databases/_connect.py
--rw-r--r--   0        0        0    20140 2023-05-11 19:39:43.705453 data_diff-0.8.0/data_diff/sqeleton/databases/base.py
--rw-r--r--   0        0        0    10648 2023-06-16 19:57:48.277742 data_diff-0.8.0/data_diff/sqeleton/databases/bigquery.py
--rw-r--r--   0        0        0     6642 2023-04-21 21:58:08.198608 data_diff-0.8.0/data_diff/sqeleton/databases/clickhouse.py
--rw-r--r--   0        0        0     6959 2023-04-21 21:58:08.198702 data_diff-0.8.0/data_diff/sqeleton/databases/databricks.py
--rw-r--r--   0        0        0     6093 2023-04-21 21:58:08.198787 data_diff-0.8.0/data_diff/sqeleton/databases/duckdb.py
--rw-r--r--   0        0        0      910 2023-04-21 21:58:08.198859 data_diff-0.8.0/data_diff/sqeleton/databases/mssql.py
--rw-r--r--   0        0        0     4438 2023-04-21 21:58:08.198940 data_diff-0.8.0/data_diff/sqeleton/databases/mysql.py
--rw-r--r--   0        0        0     6550 2023-05-05 21:08:17.223666 data_diff-0.8.0/data_diff/sqeleton/databases/oracle.py
--rw-r--r--   0        0        0     5550 2023-06-27 22:04:20.814520 data_diff-0.8.0/data_diff/sqeleton/databases/postgresql.py
--rw-r--r--   0        0        0     6112 2023-04-21 21:58:08.199200 data_diff-0.8.0/data_diff/sqeleton/databases/presto.py
--rw-r--r--   0        0        0     6295 2023-06-27 22:04:20.814736 data_diff-0.8.0/data_diff/sqeleton/databases/redshift.py
--rw-r--r--   0        0        0     7742 2023-04-21 21:58:08.199375 data_diff-0.8.0/data_diff/sqeleton/databases/snowflake.py
--rw-r--r--   0        0        0     1297 2023-04-21 21:58:08.199477 data_diff-0.8.0/data_diff/sqeleton/databases/trino.py
--rw-r--r--   0        0        0     5426 2023-04-21 21:58:08.199590 data_diff-0.8.0/data_diff/sqeleton/databases/vertica.py
--rw-r--r--   0        0        0      464 2023-04-21 21:58:08.199708 data_diff-0.8.0/data_diff/sqeleton/queries/__init__.py
--rw-r--r--   0        0        0     5291 2023-04-21 21:58:08.199788 data_diff-0.8.0/data_diff/sqeleton/queries/api.py
--rw-r--r--   0        0        0    30750 2023-05-05 21:08:17.224381 data_diff-0.8.0/data_diff/sqeleton/queries/ast_classes.py
--rw-r--r--   0        0        0      367 2023-04-21 21:58:08.200018 data_diff-0.8.0/data_diff/sqeleton/queries/base.py
--rw-r--r--   0        0        0     2605 2023-04-21 21:58:08.200096 data_diff-0.8.0/data_diff/sqeleton/queries/compiler.py
--rw-r--r--   0        0        0     1985 2023-04-21 21:58:08.200163 data_diff-0.8.0/data_diff/sqeleton/queries/extras.py
--rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.200227 data_diff-0.8.0/data_diff/sqeleton/query_utils.py
--rw-r--r--   0        0        0     1981 2023-04-21 21:58:08.200332 data_diff-0.8.0/data_diff/sqeleton/repl.py
--rw-r--r--   0        0        0      737 2023-04-21 21:58:08.200391 data_diff-0.8.0/data_diff/sqeleton/schema.py
--rw-r--r--   0        0        0     8906 2023-06-27 22:04:20.814972 data_diff-0.8.0/data_diff/sqeleton/utils.py
--rw-r--r--   0        0        0    10884 2023-04-21 21:58:08.200617 data_diff-0.8.0/data_diff/table_segment.py
--rw-r--r--   0        0        0     2651 2023-04-03 18:06:26.933183 data_diff-0.8.0/data_diff/thread_utils.py
--rw-r--r--   0        0        0     5481 2023-06-16 19:57:48.278007 data_diff-0.8.0/data_diff/tracking.py
--rw-r--r--   0        0        0     7840 2023-06-27 22:04:20.815284 data_diff-0.8.0/data_diff/utils.py
--rw-r--r--   0        0        0       22 2023-07-27 16:42:35.824003 data_diff-0.8.0/data_diff/version.py
--rwxr-xr-x   0        0        0     2729 2023-07-27 16:42:16.366305 data_diff-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     5253 1970-01-01 00:00:00.000000 data_diff-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.8.1/LICENSE
+-rw-r--r--   0        0        0     7601 2023-08-01 01:08:51.526212 data_diff-0.8.1/README.md
+-rw-r--r--   0        0        0     8710 2023-05-24 18:36:17.565800 data_diff-0.8.1/data_diff/__init__.py
+-rw-r--r--   0        0        0    18130 2023-07-27 15:17:08.933362 data_diff-0.8.1/data_diff/__main__.py
+-rw-r--r--   0        0        0      126 2023-05-15 21:10:13.082463 data_diff-0.8.1/data_diff/cloud/__init__.py
+-rw-r--r--   0        0        0    11568 2023-06-16 19:57:48.275419 data_diff-0.8.1/data_diff/cloud/data_source.py
+-rw-r--r--   0        0        0    10562 2023-07-25 19:31:06.998411 data_diff-0.8.1/data_diff/cloud/datafold_api.py
+-rw-r--r--   0        0        0     4044 2023-04-03 18:06:26.931568 data_diff-0.8.1/data_diff/config.py
+-rw-r--r--   0        0        0      493 2023-04-21 21:58:08.194615 data_diff-0.8.1/data_diff/databases/__init__.py
+-rw-r--r--   0        0        0     1353 2023-04-21 21:58:08.194720 data_diff-0.8.1/data_diff/databases/_connect.py
+-rw-r--r--   0        0        0      174 2023-04-21 21:58:08.194816 data_diff-0.8.1/data_diff/databases/base.py
+-rw-r--r--   0        0        0      257 2023-04-21 21:58:08.195148 data_diff-0.8.1/data_diff/databases/bigquery.py
+-rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195281 data_diff-0.8.1/data_diff/databases/clickhouse.py
+-rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195390 data_diff-0.8.1/data_diff/databases/databricks.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195511 data_diff-0.8.1/data_diff/databases/duckdb.py
+-rw-r--r--   0        0        0      236 2023-04-21 21:58:08.195617 data_diff-0.8.1/data_diff/databases/mysql.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195713 data_diff-0.8.1/data_diff/databases/oracle.py
+-rw-r--r--   0        0        0      275 2023-04-21 21:58:08.195827 data_diff-0.8.1/data_diff/databases/postgresql.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195918 data_diff-0.8.1/data_diff/databases/presto.py
+-rw-r--r--   0        0        0      257 2023-04-21 21:58:08.196013 data_diff-0.8.1/data_diff/databases/redshift.py
+-rw-r--r--   0        0        0      264 2023-04-21 21:58:08.196109 data_diff-0.8.1/data_diff/databases/snowflake.py
+-rw-r--r--   0        0        0      236 2023-04-21 21:58:08.196196 data_diff-0.8.1/data_diff/databases/trino.py
+-rw-r--r--   0        0        0      250 2023-04-21 21:58:08.196288 data_diff-0.8.1/data_diff/databases/vertica.py
+-rw-r--r--   0        0        0    19863 2023-07-27 15:25:50.449603 data_diff-0.8.1/data_diff/dbt.py
+-rw-r--r--   0        0        0    20292 2023-08-01 01:57:36.270732 data_diff-0.8.1/data_diff/dbt_parser.py
+-rw-r--r--   0        0        0    14471 2023-07-18 16:15:04.405684 data_diff-0.8.1/data_diff/diff_tables.py
+-rw-r--r--   0        0        0     2411 2023-07-25 19:31:06.998680 data_diff-0.8.1/data_diff/errors.py
+-rw-r--r--   0        0        0     9098 2023-07-16 03:33:52.656293 data_diff-0.8.1/data_diff/format.py
+-rw-r--r--   0        0        0     9405 2023-06-27 22:04:20.813975 data_diff-0.8.1/data_diff/hashdiff_tables.py
+-rw-r--r--   0        0        0     1917 2023-06-22 19:56:54.945638 data_diff-0.8.1/data_diff/info_tree.py
+-rw-r--r--   0        0        0    15377 2023-06-22 19:56:54.946004 data_diff-0.8.1/data_diff/joindiff_tables.py
+-rw-r--r--   0        0        0     7557 2023-04-03 18:06:26.932827 data_diff-0.8.1/data_diff/lexicographic_space.py
+-rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.8.1/data_diff/parse_time.py
+-rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.197181 data_diff-0.8.1/data_diff/query_utils.py
+-rw-r--r--   0        0        0       76 2023-04-21 21:58:08.197422 data_diff-0.8.1/data_diff/sqeleton/__init__.py
+-rw-r--r--   0        0        0      279 2023-04-21 21:58:08.197521 data_diff-0.8.1/data_diff/sqeleton/__main__.py
+-rw-r--r--   0        0        0      264 2023-05-05 21:08:17.222879 data_diff-0.8.1/data_diff/sqeleton/abcs/__init__.py
+-rw-r--r--   0        0        0      409 2023-04-21 21:58:08.197743 data_diff-0.8.1/data_diff/sqeleton/abcs/compiler.py
+-rw-r--r--   0        0        0    11118 2023-05-05 21:08:17.223038 data_diff-0.8.1/data_diff/sqeleton/abcs/database_types.py
+-rw-r--r--   0        0        0     7029 2023-06-27 22:04:20.814299 data_diff-0.8.1/data_diff/sqeleton/abcs/mixins.py
+-rw-r--r--   0        0        0     2425 2023-04-21 21:58:08.198003 data_diff-0.8.1/data_diff/sqeleton/bound_exprs.py
+-rw-r--r--   0        0        0      554 2023-04-21 21:58:08.198154 data_diff-0.8.1/data_diff/sqeleton/databases/__init__.py
+-rw-r--r--   0        0        0     9245 2023-06-20 20:21:00.599502 data_diff-0.8.1/data_diff/sqeleton/databases/_connect.py
+-rw-r--r--   0        0        0    20140 2023-05-11 19:39:43.705453 data_diff-0.8.1/data_diff/sqeleton/databases/base.py
+-rw-r--r--   0        0        0    10648 2023-06-16 19:57:48.277742 data_diff-0.8.1/data_diff/sqeleton/databases/bigquery.py
+-rw-r--r--   0        0        0     6642 2023-04-21 21:58:08.198608 data_diff-0.8.1/data_diff/sqeleton/databases/clickhouse.py
+-rw-r--r--   0        0        0     6959 2023-04-21 21:58:08.198702 data_diff-0.8.1/data_diff/sqeleton/databases/databricks.py
+-rw-r--r--   0        0        0     6093 2023-04-21 21:58:08.198787 data_diff-0.8.1/data_diff/sqeleton/databases/duckdb.py
+-rw-r--r--   0        0        0      910 2023-04-21 21:58:08.198859 data_diff-0.8.1/data_diff/sqeleton/databases/mssql.py
+-rw-r--r--   0        0        0     4438 2023-04-21 21:58:08.198940 data_diff-0.8.1/data_diff/sqeleton/databases/mysql.py
+-rw-r--r--   0        0        0     6550 2023-05-05 21:08:17.223666 data_diff-0.8.1/data_diff/sqeleton/databases/oracle.py
+-rw-r--r--   0        0        0     5550 2023-06-27 22:04:20.814520 data_diff-0.8.1/data_diff/sqeleton/databases/postgresql.py
+-rw-r--r--   0        0        0     6112 2023-04-21 21:58:08.199200 data_diff-0.8.1/data_diff/sqeleton/databases/presto.py
+-rw-r--r--   0        0        0     6295 2023-06-27 22:04:20.814736 data_diff-0.8.1/data_diff/sqeleton/databases/redshift.py
+-rw-r--r--   0        0        0     7742 2023-04-21 21:58:08.199375 data_diff-0.8.1/data_diff/sqeleton/databases/snowflake.py
+-rw-r--r--   0        0        0     1297 2023-04-21 21:58:08.199477 data_diff-0.8.1/data_diff/sqeleton/databases/trino.py
+-rw-r--r--   0        0        0     5426 2023-04-21 21:58:08.199590 data_diff-0.8.1/data_diff/sqeleton/databases/vertica.py
+-rw-r--r--   0        0        0      464 2023-04-21 21:58:08.199708 data_diff-0.8.1/data_diff/sqeleton/queries/__init__.py
+-rw-r--r--   0        0        0     5291 2023-04-21 21:58:08.199788 data_diff-0.8.1/data_diff/sqeleton/queries/api.py
+-rw-r--r--   0        0        0    30750 2023-05-05 21:08:17.224381 data_diff-0.8.1/data_diff/sqeleton/queries/ast_classes.py
+-rw-r--r--   0        0        0      367 2023-04-21 21:58:08.200018 data_diff-0.8.1/data_diff/sqeleton/queries/base.py
+-rw-r--r--   0        0        0     2605 2023-04-21 21:58:08.200096 data_diff-0.8.1/data_diff/sqeleton/queries/compiler.py
+-rw-r--r--   0        0        0     1985 2023-04-21 21:58:08.200163 data_diff-0.8.1/data_diff/sqeleton/queries/extras.py
+-rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.200227 data_diff-0.8.1/data_diff/sqeleton/query_utils.py
+-rw-r--r--   0        0        0     1981 2023-04-21 21:58:08.200332 data_diff-0.8.1/data_diff/sqeleton/repl.py
+-rw-r--r--   0        0        0      737 2023-04-21 21:58:08.200391 data_diff-0.8.1/data_diff/sqeleton/schema.py
+-rw-r--r--   0        0        0     8906 2023-06-27 22:04:20.814972 data_diff-0.8.1/data_diff/sqeleton/utils.py
+-rw-r--r--   0        0        0    10884 2023-04-21 21:58:08.200617 data_diff-0.8.1/data_diff/table_segment.py
+-rw-r--r--   0        0        0     2651 2023-04-03 18:06:26.933183 data_diff-0.8.1/data_diff/thread_utils.py
+-rw-r--r--   0        0        0     5481 2023-06-16 19:57:48.278007 data_diff-0.8.1/data_diff/tracking.py
+-rw-r--r--   0        0        0     7840 2023-06-27 22:04:20.815284 data_diff-0.8.1/data_diff/utils.py
+-rw-r--r--   0        0        0       22 2023-08-01 01:57:52.763840 data_diff-0.8.1/data_diff/version.py
+-rwxr-xr-x   0        0        0     2729 2023-08-01 01:57:43.432225 data_diff-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0    10112 1970-01-01 00:00:00.000000 data_diff-0.8.1/PKG-INFO
```

### Comparing `data_diff-0.8.0/LICENSE` & `data_diff-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/__init__.py` & `data_diff-0.8.1/data_diff/__init__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/__main__.py` & `data_diff-0.8.1/data_diff/__main__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/cloud/data_source.py` & `data_diff-0.8.1/data_diff/cloud/data_source.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/cloud/datafold_api.py` & `data_diff-0.8.1/data_diff/cloud/datafold_api.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/config.py` & `data_diff-0.8.1/data_diff/config.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/databases/_connect.py` & `data_diff-0.8.1/data_diff/databases/_connect.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/dbt.py` & `data_diff-0.8.1/data_diff/dbt.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/dbt_parser.py` & `data_diff-0.8.1/data_diff/dbt_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 
 RUN_RESULTS_PATH = "target/run_results.json"
 MANIFEST_PATH = "target/manifest.json"
 PROJECT_FILE = "dbt_project.yml"
 PROFILES_FILE = "profiles.yml"
 LOWER_DBT_V = "1.0.0"
-UPPER_DBT_V = "1.6.0"
+UPPER_DBT_V = "1.7.0"
 
 
 # https://github.com/dbt-labs/dbt-core/blob/c952d44ec5c2506995fbad75320acbae49125d3d/core/dbt/cli/resolvers.py#L6
 def default_project_dir() -> Path:
     paths = list(Path.cwd().parents)
     paths.insert(0, Path.cwd())
     return next((x for x in paths if (x / PROJECT_FILE).exists()), Path.cwd())
```

### Comparing `data_diff-0.8.0/data_diff/diff_tables.py` & `data_diff-0.8.1/data_diff/diff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/errors.py` & `data_diff-0.8.1/data_diff/errors.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/format.py` & `data_diff-0.8.1/data_diff/format.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/hashdiff_tables.py` & `data_diff-0.8.1/data_diff/hashdiff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/info_tree.py` & `data_diff-0.8.1/data_diff/info_tree.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/joindiff_tables.py` & `data_diff-0.8.1/data_diff/joindiff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/lexicographic_space.py` & `data_diff-0.8.1/data_diff/lexicographic_space.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/parse_time.py` & `data_diff-0.8.1/data_diff/parse_time.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/query_utils.py` & `data_diff-0.8.1/data_diff/query_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/abcs/database_types.py` & `data_diff-0.8.1/data_diff/sqeleton/abcs/database_types.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/abcs/mixins.py` & `data_diff-0.8.1/data_diff/sqeleton/abcs/mixins.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/bound_exprs.py` & `data_diff-0.8.1/data_diff/sqeleton/bound_exprs.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/databases/__init__.py` & `data_diff-0.8.1/data_diff/sqeleton/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/databases/_connect.py` & `data_diff-0.8.1/data_diff/sqeleton/databases/_connect.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/databases/base.py` & `data_diff-0.8.1/data_diff/sqeleton/databases/base.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/databases/bigquery.py` & `data_diff-0.8.1/data_diff/sqeleton/databases/bigquery.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/databases/clickhouse.py` & `data_diff-0.8.1/data_diff/sqeleton/databases/clickhouse.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/databases/databricks.py` & `data_diff-0.8.1/data_diff/sqeleton/databases/databricks.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/databases/duckdb.py` & `data_diff-0.8.1/data_diff/sqeleton/databases/duckdb.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/databases/mssql.py` & `data_diff-0.8.1/data_diff/sqeleton/databases/mssql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/databases/mysql.py` & `data_diff-0.8.1/data_diff/sqeleton/databases/mysql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/databases/oracle.py` & `data_diff-0.8.1/data_diff/sqeleton/databases/oracle.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/databases/postgresql.py` & `data_diff-0.8.1/data_diff/sqeleton/databases/postgresql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/databases/presto.py` & `data_diff-0.8.1/data_diff/sqeleton/databases/presto.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/databases/redshift.py` & `data_diff-0.8.1/data_diff/sqeleton/databases/redshift.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/databases/snowflake.py` & `data_diff-0.8.1/data_diff/sqeleton/databases/snowflake.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/databases/trino.py` & `data_diff-0.8.1/data_diff/sqeleton/databases/trino.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/databases/vertica.py` & `data_diff-0.8.1/data_diff/sqeleton/databases/vertica.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/queries/api.py` & `data_diff-0.8.1/data_diff/sqeleton/queries/api.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/queries/ast_classes.py` & `data_diff-0.8.1/data_diff/sqeleton/queries/ast_classes.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/queries/compiler.py` & `data_diff-0.8.1/data_diff/sqeleton/queries/compiler.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/queries/extras.py` & `data_diff-0.8.1/data_diff/sqeleton/queries/extras.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/query_utils.py` & `data_diff-0.8.1/data_diff/sqeleton/query_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/repl.py` & `data_diff-0.8.1/data_diff/sqeleton/repl.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/schema.py` & `data_diff-0.8.1/data_diff/sqeleton/schema.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/sqeleton/utils.py` & `data_diff-0.8.1/data_diff/sqeleton/utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/table_segment.py` & `data_diff-0.8.1/data_diff/table_segment.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/thread_utils.py` & `data_diff-0.8.1/data_diff/thread_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/tracking.py` & `data_diff-0.8.1/data_diff/tracking.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/data_diff/utils.py` & `data_diff-0.8.1/data_diff/utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.8.0/pyproject.toml` & `data_diff-0.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-diff"
-version = "0.8.0"
+version = "0.8.1"
 description = "Command-line tool and Python library to efficiently diff rows across two different databases."
 authors = ["Datafold <data-diff@datafold.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/datafold/data-diff"
 documentation = ""
 classifiers = [
@@ -33,15 +33,15 @@
 psycopg2 = {version="*", optional=true}
 snowflake-connector-python = {version = ">=3.0.2,<4.0.0", optional=true}
 cryptography = {version="*", optional=true}
 trino = {version="^0.314.0", optional=true}
 presto-python-client = {version="*", optional=true}
 clickhouse-driver = {version="*", optional=true}
 duckdb = {version="^0.7.0", optional=true}
-dbt-artifacts-parser = {version="^0.3.0"}
+dbt-artifacts-parser = {version="^0.4.0"}
 dbt-core = {version="^1.0.0"}
 keyring = "*"
 tabulate = "^0.9.0"
 preql = {version="^0.2.19", optional=true}
 cx_Oracle = {version="*", optional=true}
 vertica-python = {version="*", optional=true}
 urllib3 = "<2"
@@ -55,15 +55,15 @@
 snowflake-connector-python = ">=3.0.2,<4.0.0"
 cryptography = "*"
 trino = "^0.314.0"
 presto-python-client = "*"
 clickhouse-driver = "*"
 vertica-python = "*"
 duckdb = "^0.7.0"
-dbt-artifacts-parser = "^0.3.0"
+dbt-artifacts-parser = "^0.4.0"
 dbt-core = "^1.0.0"
 # google-cloud-bigquery = "*"
 # databricks-sql-connector = "*"
 
 [tool.poetry.extras]
 # When adding, update also: README + dev deps just above
 preql = ["preql"]
```

