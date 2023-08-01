# Comparing `tmp/awswrangler-3.2.1.tar.gz` & `tmp/awswrangler-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awswrangler-3.2.1.tar", max compression
+gzip compressed data, was "awswrangler-3.3.0.tar", max compression
```

## Comparing `awswrangler-3.2.1.tar` & `awswrangler-3.3.0.tar`

### file list

```diff
@@ -1,153 +1,157 @@
--rw-r--r--   0        0        0    10142 2022-08-02 16:44:38.861100 awswrangler-3.2.1/LICENSE.txt
--rw-r--r--   0        0        0       92 2022-09-01 20:50:36.683640 awswrangler-3.2.1/NOTICE.txt
--rw-r--r--   0        0        0    19946 2023-06-14 21:39:23.380775 awswrangler-3.2.1/README.md
--rw-r--r--   0        0        0    17494 2022-08-02 16:44:38.861401 awswrangler-3.2.1/THIRD_PARTY.txt
--rw-r--r--   0        0        0     1445 2023-06-13 21:15:14.188495 awswrangler-3.2.1/awswrangler/__init__.py
--rw-r--r--   0        0        0      276 2023-06-14 21:39:23.381455 awswrangler-3.2.1/awswrangler/__metadata__.py
--rw-r--r--   0        0        0     4351 2023-06-13 21:15:14.189071 awswrangler-3.2.1/awswrangler/_arrow.py
--rw-r--r--   0        0        0    28922 2023-06-13 21:15:14.189395 awswrangler-3.2.1/awswrangler/_config.py
--rw-r--r--   0        0        0    32498 2023-06-13 21:15:14.189750 awswrangler-3.2.1/awswrangler/_data_types.py
--rw-r--r--   0        0        0    13918 2023-06-13 21:15:14.190038 awswrangler-3.2.1/awswrangler/_databases.py
--rw-r--r--   0        0        0     6254 2023-06-13 21:15:14.190280 awswrangler-3.2.1/awswrangler/_distributed.py
--rw-r--r--   0        0        0     2063 2023-04-21 16:06:31.388005 awswrangler-3.2.1/awswrangler/_executor.py
--rw-r--r--   0        0        0     5780 2023-06-13 21:15:14.190528 awswrangler-3.2.1/awswrangler/_sql_formatter.py
--rw-r--r--   0        0        0    29441 2023-06-13 21:15:14.190851 awswrangler-3.2.1/awswrangler/_utils.py
--rw-r--r--   0        0        0     1701 2023-04-21 16:06:31.390428 awswrangler-3.2.1/awswrangler/annotations.py
--rw-r--r--   0        0        0     1329 2023-06-14 21:39:23.381802 awswrangler-3.2.1/awswrangler/athena/__init__.py
--rw-r--r--   0        0        0     9602 2023-06-13 21:15:14.191569 awswrangler-3.2.1/awswrangler/athena/_cache.py
--rw-r--r--   0        0        0     9681 2023-06-14 21:39:23.382168 awswrangler-3.2.1/awswrangler/athena/_executions.py
--rw-r--r--   0        0        0     2148 2023-06-14 21:39:23.382413 awswrangler-3.2.1/awswrangler/athena/_executions.pyi
--rw-r--r--   0        0        0    57298 2023-06-14 21:39:23.382977 awswrangler-3.2.1/awswrangler/athena/_read.py
--rw-r--r--   0        0        0    12408 2023-06-14 21:39:23.383292 awswrangler-3.2.1/awswrangler/athena/_read.pyi
--rw-r--r--   0        0        0     8661 2023-06-13 21:15:14.193473 awswrangler-3.2.1/awswrangler/athena/_spark.py
--rw-r--r--   0        0        0    42079 2023-06-14 21:39:23.383659 awswrangler-3.2.1/awswrangler/athena/_utils.py
--rw-r--r--   0        0        0     8398 2023-06-13 21:15:14.194522 awswrangler-3.2.1/awswrangler/athena/_write_iceberg.py
--rw-r--r--   0        0        0     2531 2023-06-13 21:15:14.194795 awswrangler-3.2.1/awswrangler/catalog/__init__.py
--rw-r--r--   0        0        0    17109 2023-06-13 21:15:14.195033 awswrangler-3.2.1/awswrangler/catalog/_add.py
--rw-r--r--   0        0        0    60168 2023-06-13 21:15:14.195357 awswrangler-3.2.1/awswrangler/catalog/_create.py
--rw-r--r--   0        0        0    14525 2023-06-13 21:15:14.195595 awswrangler-3.2.1/awswrangler/catalog/_definitions.py
--rw-r--r--   0        0        0     8236 2023-04-21 16:06:31.394534 awswrangler-3.2.1/awswrangler/catalog/_delete.py
--rw-r--r--   0        0        0    36053 2023-05-26 15:59:19.165550 awswrangler-3.2.1/awswrangler/catalog/_get.py
--rw-r--r--   0        0        0    11233 2023-04-21 16:06:31.395700 awswrangler-3.2.1/awswrangler/catalog/_utils.py
--rw-r--r--   0        0        0     1199 2023-06-07 15:18:15.458044 awswrangler-3.2.1/awswrangler/chime.py
--rw-r--r--   0        0        0    16592 2023-04-21 16:06:31.396720 awswrangler-3.2.1/awswrangler/cloudwatch.py
--rw-r--r--   0        0        0      141 2022-08-02 16:44:38.863831 awswrangler-3.2.1/awswrangler/data_api/__init__.py
--rw-r--r--   0        0        0     5367 2023-06-13 21:15:14.196073 awswrangler-3.2.1/awswrangler/data_api/_connector.py
--rw-r--r--   0        0        0    16265 2023-06-13 21:15:14.196358 awswrangler-3.2.1/awswrangler/data_api/rds.py
--rw-r--r--   0        0        0    11152 2023-06-13 21:15:14.196599 awswrangler-3.2.1/awswrangler/data_api/redshift.py
--rw-r--r--   0        0        0      377 2023-01-17 17:33:17.179381 awswrangler-3.2.1/awswrangler/data_quality/__init__.py
--rw-r--r--   0        0        0    13403 2023-05-24 14:22:08.634079 awswrangler-3.2.1/awswrangler/data_quality/_create.py
--rw-r--r--   0        0        0     1404 2023-04-21 16:06:31.398990 awswrangler-3.2.1/awswrangler/data_quality/_get.py
--rw-r--r--   0        0        0     6762 2023-06-13 21:15:14.196842 awswrangler-3.2.1/awswrangler/data_quality/_utils.py
--rw-r--r--   0        0        0       26 2023-04-21 16:06:31.399991 awswrangler-3.2.1/awswrangler/distributed/__init__.py
--rw-r--r--   0        0        0      237 2023-04-21 16:06:31.400247 awswrangler-3.2.1/awswrangler/distributed/ray/__init__.py
--rw-r--r--   0        0        0     6334 2023-06-13 21:15:14.199735 awswrangler-3.2.1/awswrangler/distributed/ray/_core.py
--rw-r--r--   0        0        0      931 2023-04-21 16:06:31.400648 awswrangler-3.2.1/awswrangler/distributed/ray/_core.pyi
--rw-r--r--   0        0        0     2151 2023-06-14 18:23:54.169183 awswrangler-3.2.1/awswrangler/distributed/ray/_executor.py
--rw-r--r--   0        0        0     4971 2023-06-13 21:15:14.200016 awswrangler-3.2.1/awswrangler/distributed/ray/_register.py
--rw-r--r--   0        0        0     2503 2023-06-14 18:23:54.170071 awswrangler-3.2.1/awswrangler/distributed/ray/_utils.py
--rw-r--r--   0        0        0     1131 2023-06-13 21:15:14.200645 awswrangler-3.2.1/awswrangler/distributed/ray/datasources/__init__.py
--rw-r--r--   0        0        0     2186 2023-06-14 18:23:54.171486 awswrangler-3.2.1/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py
--rw-r--r--   0        0        0     1273 2023-04-21 16:06:31.402074 awswrangler-3.2.1/awswrangler/distributed/ray/datasources/arrow_json_datasource.py
--rw-r--r--   0        0        0     2036 2023-06-14 21:46:19.742499 awswrangler-3.2.1/awswrangler/distributed/ray/datasources/arrow_orc_datasource.py
--rw-r--r--   0        0        0     3318 2023-06-14 18:23:54.173362 awswrangler-3.2.1/awswrangler/distributed/ray/datasources/arrow_parquet_base_datasource.py
--rw-r--r--   0        0        0    19694 2023-06-14 18:23:54.174400 awswrangler-3.2.1/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py
--rw-r--r--   0        0        0     8953 2023-06-14 18:23:54.175332 awswrangler-3.2.1/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py
--rw-r--r--   0        0        0     5891 2023-06-14 18:23:54.175963 awswrangler-3.2.1/awswrangler/distributed/ray/datasources/pandas_text_datasource.py
--rw-r--r--   0        0        0      135 2023-04-21 16:06:31.402995 awswrangler-3.2.1/awswrangler/distributed/ray/modin/__init__.py
--rw-r--r--   0        0        0     2524 2023-04-21 16:06:31.403517 awswrangler-3.2.1/awswrangler/distributed/ray/modin/_core.py
--rw-r--r--   0        0        0      929 2023-06-12 14:16:31.031863 awswrangler-3.2.1/awswrangler/distributed/ray/modin/_data_types.py
--rw-r--r--   0        0        0     4068 2023-06-14 18:23:54.177267 awswrangler-3.2.1/awswrangler/distributed/ray/modin/_utils.py
--rw-r--r--   0        0        0       27 2023-04-21 16:06:31.403997 awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/__init__.py
--rw-r--r--   0        0        0     1484 2023-06-13 21:15:14.202375 awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_read_orc.py
--rw-r--r--   0        0        0     1871 2023-06-13 21:15:14.202754 awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_read_parquet.py
--rw-r--r--   0        0        0     5507 2023-06-13 21:15:14.203222 awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_read_text.py
--rw-r--r--   0        0        0     7306 2023-04-21 16:06:31.405287 awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_write_dataset.py
--rw-r--r--   0        0        0     3043 2023-06-13 21:15:14.203325 awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_write_orc.py
--rw-r--r--   0        0        0     3065 2023-06-05 20:19:19.920635 awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_write_parquet.py
--rw-r--r--   0        0        0     5479 2023-06-13 21:15:14.203788 awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_write_text.py
--rw-r--r--   0        0        0       21 2023-04-21 16:06:31.405975 awswrangler-3.2.1/awswrangler/distributed/ray/s3/__init__.py
--rw-r--r--   0        0        0     2413 2023-04-21 16:06:31.406055 awswrangler-3.2.1/awswrangler/distributed/ray/s3/_list.py
--rw-r--r--   0        0        0      850 2023-06-13 21:15:14.203888 awswrangler-3.2.1/awswrangler/distributed/ray/s3/_read_orc.py
--rw-r--r--   0        0        0     1005 2023-05-24 14:22:08.638085 awswrangler-3.2.1/awswrangler/distributed/ray/s3/_read_parquet.py
--rw-r--r--   0        0        0      484 2023-05-04 22:03:58.498637 awswrangler-3.2.1/awswrangler/dynamodb/__init__.py
--rw-r--r--   0        0        0     1545 2023-04-21 16:06:31.406985 awswrangler-3.2.1/awswrangler/dynamodb/_delete.py
--rw-r--r--   0        0        0    25553 2023-06-13 21:15:14.204147 awswrangler-3.2.1/awswrangler/dynamodb/_read.py
--rw-r--r--   0        0        0     9612 2023-06-13 21:15:14.204271 awswrangler-3.2.1/awswrangler/dynamodb/_read.pyi
--rw-r--r--   0        0        0     6918 2023-06-13 21:15:14.204966 awswrangler-3.2.1/awswrangler/dynamodb/_utils.py
--rw-r--r--   0        0        0     8406 2023-04-21 16:06:31.408377 awswrangler-3.2.1/awswrangler/dynamodb/_write.py
--rw-r--r--   0        0        0    44390 2023-06-13 21:15:14.206293 awswrangler-3.2.1/awswrangler/emr.py
--rw-r--r--   0        0        0    10247 2023-06-13 21:15:14.206475 awswrangler-3.2.1/awswrangler/emr_serverless.py
--rw-r--r--   0        0        0     2977 2023-06-13 21:15:14.207077 awswrangler-3.2.1/awswrangler/exceptions.py
--rw-r--r--   0        0        0      682 2023-04-13 20:06:09.276287 awswrangler-3.2.1/awswrangler/lakeformation/__init__.py
--rw-r--r--   0        0        0    12069 2023-06-13 21:15:14.207817 awswrangler-3.2.1/awswrangler/lakeformation/_read.py
--rw-r--r--   0        0        0    13151 2023-04-21 16:06:31.411661 awswrangler-3.2.1/awswrangler/lakeformation/_utils.py
--rw-r--r--   0        0        0    21739 2023-06-13 21:15:14.208458 awswrangler-3.2.1/awswrangler/mysql.py
--rw-r--r--   0        0        0      673 2023-06-13 21:15:14.208796 awswrangler-3.2.1/awswrangler/neptune/__init__.py
--rw-r--r--   0        0        0    16117 2023-06-13 21:15:14.210053 awswrangler-3.2.1/awswrangler/neptune/_client.py
--rw-r--r--   0        0        0      923 2023-04-21 16:06:31.412767 awswrangler-3.2.1/awswrangler/neptune/_gremlin_init.py
--rw-r--r--   0        0        0     2708 2023-06-13 21:15:14.210311 awswrangler-3.2.1/awswrangler/neptune/_gremlin_parser.py
--rw-r--r--   0        0        0    25013 2023-06-13 21:15:14.211352 awswrangler-3.2.1/awswrangler/neptune/_neptune.py
--rw-r--r--   0        0        0     3752 2023-06-13 21:15:14.212053 awswrangler-3.2.1/awswrangler/neptune/_utils.py
--rw-r--r--   0        0        0      502 2023-01-30 20:05:15.832378 awswrangler-3.2.1/awswrangler/opensearch/__init__.py
--rw-r--r--   0        0        0     6480 2023-06-13 21:13:23.797325 awswrangler-3.2.1/awswrangler/opensearch/_read.py
--rw-r--r--   0        0        0    13764 2023-06-13 21:13:23.797629 awswrangler-3.2.1/awswrangler/opensearch/_utils.py
--rw-r--r--   0        0        0    23823 2023-06-13 21:15:14.212648 awswrangler-3.2.1/awswrangler/opensearch/_write.py
--rw-r--r--   0        0        0    22400 2023-06-13 21:15:14.212930 awswrangler-3.2.1/awswrangler/oracle.py
--rw-r--r--   0        0        0     1282 2023-06-13 21:15:14.213188 awswrangler-3.2.1/awswrangler/pandas/__init__.py
--rw-r--r--   0        0        0    22222 2023-06-13 21:15:14.214956 awswrangler-3.2.1/awswrangler/postgresql.py
--rw-r--r--   0        0        0       27 2022-08-02 16:44:38.866284 awswrangler-3.2.1/awswrangler/py.typed
--rw-r--r--   0        0        0     2219 2023-01-17 17:33:17.208660 awswrangler-3.2.1/awswrangler/quicksight/__init__.py
--rw-r--r--   0        0        0     1906 2023-04-21 16:06:31.416913 awswrangler-3.2.1/awswrangler/quicksight/_cancel.py
--rw-r--r--   0        0        0    19228 2023-06-13 21:15:14.218977 awswrangler-3.2.1/awswrangler/quicksight/_create.py
--rw-r--r--   0        0        0    11710 2023-04-21 16:06:31.417954 awswrangler-3.2.1/awswrangler/quicksight/_delete.py
--rw-r--r--   0        0        0     8660 2023-04-21 16:06:31.418387 awswrangler-3.2.1/awswrangler/quicksight/_describe.py
--rw-r--r--   0        0        0    23657 2023-05-15 14:19:50.276077 awswrangler-3.2.1/awswrangler/quicksight/_get_list.py
--rw-r--r--   0        0        0     2096 2023-06-13 21:15:14.220205 awswrangler-3.2.1/awswrangler/quicksight/_utils.py
--rw-r--r--   0        0        0      440 2023-06-13 21:15:14.220549 awswrangler-3.2.1/awswrangler/redshift/__init__.py
--rw-r--r--   0        0        0     8809 2023-06-13 21:15:14.220661 awswrangler-3.2.1/awswrangler/redshift/_connect.py
--rw-r--r--   0        0        0    20832 2023-06-13 21:15:14.220795 awswrangler-3.2.1/awswrangler/redshift/_read.py
--rw-r--r--   0        0        0     6716 2023-06-13 21:15:14.220904 awswrangler-3.2.1/awswrangler/redshift/_read.pyi
--rw-r--r--   0        0        0    15681 2023-06-13 21:15:14.221067 awswrangler-3.2.1/awswrangler/redshift/_utils.py
--rw-r--r--   0        0        0    28318 2023-06-13 21:15:14.221202 awswrangler-3.2.1/awswrangler/redshift/_write.py
--rw-r--r--   0        0        0     2008 2023-06-13 21:15:14.221574 awswrangler-3.2.1/awswrangler/s3/__init__.py
--rw-r--r--   0        0        0    10594 2023-05-24 14:22:08.646591 awswrangler-3.2.1/awswrangler/s3/_copy.py
--rw-r--r--   0        0        0     5289 2023-04-21 16:06:31.421784 awswrangler-3.2.1/awswrangler/s3/_delete.py
--rw-r--r--   0        0        0     9327 2023-04-21 16:06:31.422180 awswrangler-3.2.1/awswrangler/s3/_describe.py
--rw-r--r--   0        0        0     2633 2023-01-30 20:05:15.841405 awswrangler-3.2.1/awswrangler/s3/_download.py
--rw-r--r--   0        0        0    23146 2023-04-21 16:06:31.422841 awswrangler-3.2.1/awswrangler/s3/_fs.py
--rw-r--r--   0        0        0    15683 2023-04-21 16:06:31.423159 awswrangler-3.2.1/awswrangler/s3/_list.py
--rw-r--r--   0        0        0     4158 2023-06-13 21:15:14.221765 awswrangler-3.2.1/awswrangler/s3/_list.pyi
--rw-r--r--   0        0        0    15344 2023-06-13 21:15:14.222716 awswrangler-3.2.1/awswrangler/s3/_read.py
--rw-r--r--   0        0        0     4167 2023-06-13 21:15:14.222974 awswrangler-3.2.1/awswrangler/s3/_read_deltalake.py
--rw-r--r--   0        0        0     3277 2023-06-13 21:13:23.801300 awswrangler-3.2.1/awswrangler/s3/_read_excel.py
--rw-r--r--   0        0        0    23265 2023-06-14 20:26:54.837101 awswrangler-3.2.1/awswrangler/s3/_read_orc.py
--rw-r--r--   0        0        0    33869 2023-06-14 21:39:23.384240 awswrangler-3.2.1/awswrangler/s3/_read_parquet.py
--rw-r--r--   0        0        0    10040 2023-06-13 21:15:14.225352 awswrangler-3.2.1/awswrangler/s3/_read_parquet.pyi
--rw-r--r--   0        0        0    27928 2023-06-14 21:39:23.384699 awswrangler-3.2.1/awswrangler/s3/_read_text.py
--rw-r--r--   0        0        0     7993 2023-06-13 21:15:14.226169 awswrangler-3.2.1/awswrangler/s3/_read_text.pyi
--rw-r--r--   0        0        0     4108 2023-05-22 20:51:56.860472 awswrangler-3.2.1/awswrangler/s3/_read_text_core.py
--rw-r--r--   0        0        0    12569 2023-06-13 21:15:14.226577 awswrangler-3.2.1/awswrangler/s3/_select.py
--rw-r--r--   0        0        0     2465 2023-04-21 16:06:31.426801 awswrangler-3.2.1/awswrangler/s3/_upload.py
--rw-r--r--   0        0        0     6205 2023-04-21 16:06:31.427634 awswrangler-3.2.1/awswrangler/s3/_wait.py
--rw-r--r--   0        0        0    18407 2023-06-13 21:15:14.227190 awswrangler-3.2.1/awswrangler/s3/_write.py
--rw-r--r--   0        0        0     1840 2023-04-21 16:06:31.428436 awswrangler-3.2.1/awswrangler/s3/_write_concurrent.py
--rw-r--r--   0        0        0    12740 2023-06-13 21:15:14.227436 awswrangler-3.2.1/awswrangler/s3/_write_dataset.py
--rw-r--r--   0        0        0     4144 2023-06-13 21:15:14.227527 awswrangler-3.2.1/awswrangler/s3/_write_deltalake.py
--rw-r--r--   0        0        0     3196 2023-06-13 21:13:23.801521 awswrangler-3.2.1/awswrangler/s3/_write_excel.py
--rw-r--r--   0        0        0    26700 2023-06-14 20:26:54.837927 awswrangler-3.2.1/awswrangler/s3/_write_orc.py
--rw-r--r--   0        0        0    39437 2023-06-14 21:39:23.386060 awswrangler-3.2.1/awswrangler/s3/_write_parquet.py
--rw-r--r--   0        0        0    48588 2023-06-14 21:39:23.386613 awswrangler-3.2.1/awswrangler/s3/_write_text.py
--rw-r--r--   0        0        0     2018 2023-04-21 16:06:31.431108 awswrangler-3.2.1/awswrangler/secretsmanager.py
--rw-r--r--   0        0        0    19421 2023-06-13 21:15:14.231127 awswrangler-3.2.1/awswrangler/sqlserver.py
--rw-r--r--   0        0        0     1853 2023-04-21 16:06:31.432014 awswrangler-3.2.1/awswrangler/sts.py
--rw-r--r--   0        0        0      727 2023-06-13 21:15:14.231474 awswrangler-3.2.1/awswrangler/timestream/__init__.py
--rw-r--r--   0        0        0     4512 2023-06-13 21:15:14.231567 awswrangler-3.2.1/awswrangler/timestream/_create.py
--rw-r--r--   0        0        0     2491 2023-06-13 21:15:14.231639 awswrangler-3.2.1/awswrangler/timestream/_delete.py
--rw-r--r--   0        0        0     2603 2023-06-13 21:15:14.231709 awswrangler-3.2.1/awswrangler/timestream/_list.py
--rw-r--r--   0        0        0    16998 2023-06-13 21:15:14.231817 awswrangler-3.2.1/awswrangler/timestream/_read.py
--rw-r--r--   0        0        0     1910 2023-06-13 21:15:14.231911 awswrangler-3.2.1/awswrangler/timestream/_read.pyi
--rw-r--r--   0        0        0    26397 2023-06-13 21:15:14.232051 awswrangler-3.2.1/awswrangler/timestream/_write.py
--rw-r--r--   0        0        0     9355 2023-06-13 21:15:14.233372 awswrangler-3.2.1/awswrangler/typing.py
--rw-r--r--   0        0        0     4854 2023-06-14 21:39:23.387816 awswrangler-3.2.1/pyproject.toml
--rw-r--r--   0        0        0    22585 1970-01-01 00:00:00.000000 awswrangler-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0    10142 2021-01-13 17:42:05.000000 awswrangler-3.3.0/LICENSE.txt
+-rw-r--r--   0        0        0       92 2022-09-07 12:05:27.255553 awswrangler-3.3.0/NOTICE.txt
+-rw-r--r--   0        0        0    20583 2023-08-01 07:18:46.949430 awswrangler-3.3.0/README.md
+-rw-r--r--   0        0        0    17494 2021-01-13 17:42:05.000000 awswrangler-3.3.0/THIRD_PARTY.txt
+-rw-r--r--   0        0        0     1479 2023-06-27 10:04:34.491148 awswrangler-3.3.0/awswrangler/__init__.py
+-rw-r--r--   0        0        0      276 2023-08-01 07:18:46.951358 awswrangler-3.3.0/awswrangler/__metadata__.py
+-rw-r--r--   0        0        0     4472 2023-08-01 11:53:36.754589 awswrangler-3.3.0/awswrangler/_arrow.py
+-rw-r--r--   0        0        0    28922 2023-06-26 08:59:53.033237 awswrangler-3.3.0/awswrangler/_config.py
+-rw-r--r--   0        0        0    32498 2023-06-26 08:59:53.034315 awswrangler-3.3.0/awswrangler/_data_types.py
+-rw-r--r--   0        0        0    13918 2023-06-26 08:59:53.035261 awswrangler-3.3.0/awswrangler/_databases.py
+-rw-r--r--   0        0        0     6254 2023-06-26 08:59:53.035856 awswrangler-3.3.0/awswrangler/_distributed.py
+-rw-r--r--   0        0        0     2063 2023-06-26 08:59:53.036086 awswrangler-3.3.0/awswrangler/_executor.py
+-rw-r--r--   0        0        0     5780 2023-06-26 08:59:53.036469 awswrangler-3.3.0/awswrangler/_sql_formatter.py
+-rw-r--r--   0        0        0    29770 2023-07-21 13:12:51.766538 awswrangler-3.3.0/awswrangler/_utils.py
+-rw-r--r--   0        0        0     1701 2023-06-26 08:59:53.037442 awswrangler-3.3.0/awswrangler/annotations.py
+-rw-r--r--   0        0        0     1566 2023-06-26 08:59:53.037794 awswrangler-3.3.0/awswrangler/athena/__init__.py
+-rw-r--r--   0        0        0     9602 2023-06-26 08:59:53.038624 awswrangler-3.3.0/awswrangler/athena/_cache.py
+-rw-r--r--   0        0        0    10445 2023-06-26 08:59:53.039025 awswrangler-3.3.0/awswrangler/athena/_executions.py
+-rw-r--r--   0        0        0     2347 2023-06-26 08:59:53.039185 awswrangler-3.3.0/awswrangler/athena/_executions.pyi
+-rw-r--r--   0        0        0    59251 2023-08-01 07:18:46.952976 awswrangler-3.3.0/awswrangler/athena/_read.py
+-rw-r--r--   0        0        0    12786 2023-06-26 08:59:53.040279 awswrangler-3.3.0/awswrangler/athena/_read.pyi
+-rw-r--r--   0        0        0     8661 2023-06-26 08:59:53.041107 awswrangler-3.3.0/awswrangler/athena/_spark.py
+-rw-r--r--   0        0        0     5466 2023-06-26 08:59:53.041279 awswrangler-3.3.0/awswrangler/athena/_statements.py
+-rw-r--r--   0        0        0    44213 2023-07-21 13:12:51.767861 awswrangler-3.3.0/awswrangler/athena/_utils.py
+-rw-r--r--   0        0        0     8793 2023-06-30 15:47:34.374063 awswrangler-3.3.0/awswrangler/athena/_write_iceberg.py
+-rw-r--r--   0        0        0     2531 2023-06-26 08:59:53.042702 awswrangler-3.3.0/awswrangler/catalog/__init__.py
+-rw-r--r--   0        0        0    17109 2023-06-26 08:59:53.043636 awswrangler-3.3.0/awswrangler/catalog/_add.py
+-rw-r--r--   0        0        0    60168 2023-06-26 08:59:53.044047 awswrangler-3.3.0/awswrangler/catalog/_create.py
+-rw-r--r--   0        0        0    14525 2023-06-26 08:59:53.044693 awswrangler-3.3.0/awswrangler/catalog/_definitions.py
+-rw-r--r--   0        0        0     8236 2023-06-26 08:59:53.045041 awswrangler-3.3.0/awswrangler/catalog/_delete.py
+-rw-r--r--   0        0        0    36053 2023-06-26 08:59:53.045827 awswrangler-3.3.0/awswrangler/catalog/_get.py
+-rw-r--r--   0        0        0    11233 2023-06-26 08:59:53.046203 awswrangler-3.3.0/awswrangler/catalog/_utils.py
+-rw-r--r--   0        0        0     1199 2022-10-08 10:37:42.800465 awswrangler-3.3.0/awswrangler/chime.py
+-rw-r--r--   0        0        0      198 2023-06-27 10:04:34.492953 awswrangler-3.3.0/awswrangler/cleanrooms/__init__.py
+-rw-r--r--   0        0        0     4758 2023-07-06 08:25:39.047037 awswrangler-3.3.0/awswrangler/cleanrooms/_read.py
+-rw-r--r--   0        0        0     1914 2023-06-27 10:04:34.494264 awswrangler-3.3.0/awswrangler/cleanrooms/_utils.py
+-rw-r--r--   0        0        0    16592 2023-06-26 08:59:53.046570 awswrangler-3.3.0/awswrangler/cloudwatch.py
+-rw-r--r--   0        0        0      141 2022-10-08 10:37:42.802168 awswrangler-3.3.0/awswrangler/data_api/__init__.py
+-rw-r--r--   0        0        0     5367 2023-06-26 08:59:53.047474 awswrangler-3.3.0/awswrangler/data_api/_connector.py
+-rw-r--r--   0        0        0    17142 2023-07-21 13:12:51.768918 awswrangler-3.3.0/awswrangler/data_api/rds.py
+-rw-r--r--   0        0        0    11152 2023-06-26 08:59:53.048966 awswrangler-3.3.0/awswrangler/data_api/redshift.py
+-rw-r--r--   0        0        0      377 2023-03-24 17:26:04.723684 awswrangler-3.3.0/awswrangler/data_quality/__init__.py
+-rw-r--r--   0        0        0    13403 2023-06-26 08:59:53.049405 awswrangler-3.3.0/awswrangler/data_quality/_create.py
+-rw-r--r--   0        0        0     1404 2023-06-26 08:59:53.049745 awswrangler-3.3.0/awswrangler/data_quality/_get.py
+-rw-r--r--   0        0        0     6762 2023-06-26 08:59:53.050395 awswrangler-3.3.0/awswrangler/data_quality/_utils.py
+-rw-r--r--   0        0        0       26 2023-04-17 10:44:07.342942 awswrangler-3.3.0/awswrangler/distributed/__init__.py
+-rw-r--r--   0        0        0      237 2023-04-17 10:44:07.343785 awswrangler-3.3.0/awswrangler/distributed/ray/__init__.py
+-rw-r--r--   0        0        0     6334 2023-07-25 10:08:13.250996 awswrangler-3.3.0/awswrangler/distributed/ray/_core.py
+-rw-r--r--   0        0        0      931 2023-04-17 10:44:07.344596 awswrangler-3.3.0/awswrangler/distributed/ray/_core.pyi
+-rw-r--r--   0        0        0     2121 2023-07-31 18:52:13.842867 awswrangler-3.3.0/awswrangler/distributed/ray/_executor.py
+-rw-r--r--   0        0        0     4971 2023-06-26 08:59:53.051204 awswrangler-3.3.0/awswrangler/distributed/ray/_register.py
+-rw-r--r--   0        0        0     2443 2023-07-31 18:52:13.843572 awswrangler-3.3.0/awswrangler/distributed/ray/_utils.py
+-rw-r--r--   0        0        0     1131 2023-06-26 08:59:53.051765 awswrangler-3.3.0/awswrangler/distributed/ray/datasources/__init__.py
+-rw-r--r--   0        0        0     2186 2023-06-26 08:59:53.052325 awswrangler-3.3.0/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py
+-rw-r--r--   0        0        0     1273 2023-06-26 08:59:53.052525 awswrangler-3.3.0/awswrangler/distributed/ray/datasources/arrow_json_datasource.py
+-rw-r--r--   0        0        0     2036 2023-06-26 08:59:53.052933 awswrangler-3.3.0/awswrangler/distributed/ray/datasources/arrow_orc_datasource.py
+-rw-r--r--   0        0        0     3318 2023-06-26 08:59:53.053087 awswrangler-3.3.0/awswrangler/distributed/ray/datasources/arrow_parquet_base_datasource.py
+-rw-r--r--   0        0        0    19636 2023-07-31 18:52:13.844939 awswrangler-3.3.0/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py
+-rw-r--r--   0        0        0     8953 2023-07-21 12:08:55.149251 awswrangler-3.3.0/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py
+-rw-r--r--   0        0        0     5891 2023-06-26 08:59:53.054666 awswrangler-3.3.0/awswrangler/distributed/ray/datasources/pandas_text_datasource.py
+-rw-r--r--   0        0        0      135 2023-04-17 10:44:07.351791 awswrangler-3.3.0/awswrangler/distributed/ray/modin/__init__.py
+-rw-r--r--   0        0        0     2524 2023-06-26 08:59:53.055076 awswrangler-3.3.0/awswrangler/distributed/ray/modin/_core.py
+-rw-r--r--   0        0        0      929 2023-06-26 08:59:53.055406 awswrangler-3.3.0/awswrangler/distributed/ray/modin/_data_types.py
+-rw-r--r--   0        0        0     4098 2023-07-31 21:12:24.247736 awswrangler-3.3.0/awswrangler/distributed/ray/modin/_utils.py
+-rw-r--r--   0        0        0       27 2023-04-17 10:44:07.354121 awswrangler-3.3.0/awswrangler/distributed/ray/modin/s3/__init__.py
+-rw-r--r--   0        0        0     1484 2023-06-26 08:59:53.055908 awswrangler-3.3.0/awswrangler/distributed/ray/modin/s3/_read_orc.py
+-rw-r--r--   0        0        0     1871 2023-06-26 08:59:53.056281 awswrangler-3.3.0/awswrangler/distributed/ray/modin/s3/_read_parquet.py
+-rw-r--r--   0        0        0     5507 2023-06-26 08:59:53.056721 awswrangler-3.3.0/awswrangler/distributed/ray/modin/s3/_read_text.py
+-rw-r--r--   0        0        0     7306 2023-06-26 08:59:53.057246 awswrangler-3.3.0/awswrangler/distributed/ray/modin/s3/_write_dataset.py
+-rw-r--r--   0        0        0     3043 2023-06-26 08:59:53.057450 awswrangler-3.3.0/awswrangler/distributed/ray/modin/s3/_write_orc.py
+-rw-r--r--   0        0        0     3065 2023-06-26 08:59:53.057835 awswrangler-3.3.0/awswrangler/distributed/ray/modin/s3/_write_parquet.py
+-rw-r--r--   0        0        0     5479 2023-06-26 08:59:53.058860 awswrangler-3.3.0/awswrangler/distributed/ray/modin/s3/_write_text.py
+-rw-r--r--   0        0        0       21 2023-06-26 08:59:53.059041 awswrangler-3.3.0/awswrangler/distributed/ray/s3/__init__.py
+-rw-r--r--   0        0        0     2413 2023-06-26 08:59:53.059199 awswrangler-3.3.0/awswrangler/distributed/ray/s3/_list.py
+-rw-r--r--   0        0        0      850 2023-06-26 08:59:53.059387 awswrangler-3.3.0/awswrangler/distributed/ray/s3/_read_orc.py
+-rw-r--r--   0        0        0     1005 2023-06-26 08:59:53.059573 awswrangler-3.3.0/awswrangler/distributed/ray/s3/_read_parquet.py
+-rw-r--r--   0        0        0      484 2023-06-26 08:59:53.060031 awswrangler-3.3.0/awswrangler/dynamodb/__init__.py
+-rw-r--r--   0        0        0     1545 2023-06-26 08:59:53.060439 awswrangler-3.3.0/awswrangler/dynamodb/_delete.py
+-rw-r--r--   0        0        0    27117 2023-07-31 13:59:53.959187 awswrangler-3.3.0/awswrangler/dynamodb/_read.py
+-rw-r--r--   0        0        0     9612 2023-06-26 08:59:53.061460 awswrangler-3.3.0/awswrangler/dynamodb/_read.pyi
+-rw-r--r--   0        0        0     6918 2023-06-26 08:59:53.061886 awswrangler-3.3.0/awswrangler/dynamodb/_utils.py
+-rw-r--r--   0        0        0     8406 2023-06-26 08:59:53.062344 awswrangler-3.3.0/awswrangler/dynamodb/_write.py
+-rw-r--r--   0        0        0    44390 2023-06-26 08:59:53.063796 awswrangler-3.3.0/awswrangler/emr.py
+-rw-r--r--   0        0        0    10247 2023-06-26 08:59:53.064059 awswrangler-3.3.0/awswrangler/emr_serverless.py
+-rw-r--r--   0        0        0     2977 2023-06-26 08:59:53.064766 awswrangler-3.3.0/awswrangler/exceptions.py
+-rw-r--r--   0        0        0      682 2023-04-12 09:10:27.080012 awswrangler-3.3.0/awswrangler/lakeformation/__init__.py
+-rw-r--r--   0        0        0    12069 2023-06-26 08:59:53.065142 awswrangler-3.3.0/awswrangler/lakeformation/_read.py
+-rw-r--r--   0        0        0    13151 2023-06-26 08:59:53.065607 awswrangler-3.3.0/awswrangler/lakeformation/_utils.py
+-rw-r--r--   0        0        0    21739 2023-06-26 08:59:53.066311 awswrangler-3.3.0/awswrangler/mysql.py
+-rw-r--r--   0        0        0      673 2023-06-26 08:59:53.067261 awswrangler-3.3.0/awswrangler/neptune/__init__.py
+-rw-r--r--   0        0        0    16117 2023-06-26 08:59:53.067577 awswrangler-3.3.0/awswrangler/neptune/_client.py
+-rw-r--r--   0        0        0      923 2023-06-26 08:59:53.067808 awswrangler-3.3.0/awswrangler/neptune/_gremlin_init.py
+-rw-r--r--   0        0        0     2708 2023-06-26 08:59:53.068051 awswrangler-3.3.0/awswrangler/neptune/_gremlin_parser.py
+-rw-r--r--   0        0        0    25013 2023-06-26 08:59:53.068826 awswrangler-3.3.0/awswrangler/neptune/_neptune.py
+-rw-r--r--   0        0        0     3752 2023-06-26 08:59:53.069402 awswrangler-3.3.0/awswrangler/neptune/_utils.py
+-rw-r--r--   0        0        0      502 2023-03-24 17:26:04.718775 awswrangler-3.3.0/awswrangler/opensearch/__init__.py
+-rw-r--r--   0        0        0     6480 2023-06-26 08:59:53.070130 awswrangler-3.3.0/awswrangler/opensearch/_read.py
+-rw-r--r--   0        0        0    13764 2023-06-26 08:59:53.070626 awswrangler-3.3.0/awswrangler/opensearch/_utils.py
+-rw-r--r--   0        0        0    23823 2023-06-26 08:59:53.071984 awswrangler-3.3.0/awswrangler/opensearch/_write.py
+-rw-r--r--   0        0        0    22400 2023-06-26 08:59:53.072852 awswrangler-3.3.0/awswrangler/oracle.py
+-rw-r--r--   0        0        0     1282 2023-06-26 08:59:53.073119 awswrangler-3.3.0/awswrangler/pandas/__init__.py
+-rw-r--r--   0        0        0    22740 2023-07-17 17:12:26.344181 awswrangler-3.3.0/awswrangler/postgresql.py
+-rw-r--r--   0        0        0       27 2022-10-08 10:37:42.809867 awswrangler-3.3.0/awswrangler/py.typed
+-rw-r--r--   0        0        0     2219 2023-03-24 17:26:04.717923 awswrangler-3.3.0/awswrangler/quicksight/__init__.py
+-rw-r--r--   0        0        0     1906 2023-06-26 08:59:53.074031 awswrangler-3.3.0/awswrangler/quicksight/_cancel.py
+-rw-r--r--   0        0        0    19228 2023-06-26 08:59:53.074531 awswrangler-3.3.0/awswrangler/quicksight/_create.py
+-rw-r--r--   0        0        0    11710 2023-06-26 08:59:53.074979 awswrangler-3.3.0/awswrangler/quicksight/_delete.py
+-rw-r--r--   0        0        0     8660 2023-06-26 08:59:53.075432 awswrangler-3.3.0/awswrangler/quicksight/_describe.py
+-rw-r--r--   0        0        0    23657 2023-06-26 08:59:53.075967 awswrangler-3.3.0/awswrangler/quicksight/_get_list.py
+-rw-r--r--   0        0        0     2096 2023-06-26 08:59:53.076634 awswrangler-3.3.0/awswrangler/quicksight/_utils.py
+-rw-r--r--   0        0        0      440 2023-06-26 08:59:53.077131 awswrangler-3.3.0/awswrangler/redshift/__init__.py
+-rw-r--r--   0        0        0     8809 2023-06-26 08:59:53.077916 awswrangler-3.3.0/awswrangler/redshift/_connect.py
+-rw-r--r--   0        0        0    20832 2023-06-26 08:59:53.078211 awswrangler-3.3.0/awswrangler/redshift/_read.py
+-rw-r--r--   0        0        0     6716 2023-06-26 08:59:53.078396 awswrangler-3.3.0/awswrangler/redshift/_read.pyi
+-rw-r--r--   0        0        0    15730 2023-06-30 15:47:34.374632 awswrangler-3.3.0/awswrangler/redshift/_utils.py
+-rw-r--r--   0        0        0    28318 2023-06-26 08:59:53.079190 awswrangler-3.3.0/awswrangler/redshift/_write.py
+-rw-r--r--   0        0        0     2008 2023-06-26 08:59:53.079544 awswrangler-3.3.0/awswrangler/s3/__init__.py
+-rw-r--r--   0        0        0    10594 2023-06-26 08:59:53.079992 awswrangler-3.3.0/awswrangler/s3/_copy.py
+-rw-r--r--   0        0        0     5289 2023-06-26 08:59:53.080477 awswrangler-3.3.0/awswrangler/s3/_delete.py
+-rw-r--r--   0        0        0     9327 2023-06-26 08:59:53.080955 awswrangler-3.3.0/awswrangler/s3/_describe.py
+-rw-r--r--   0        0        0     2633 2023-06-26 08:59:53.081466 awswrangler-3.3.0/awswrangler/s3/_download.py
+-rw-r--r--   0        0        0    23146 2023-06-26 08:59:53.082068 awswrangler-3.3.0/awswrangler/s3/_fs.py
+-rw-r--r--   0        0        0    15683 2023-06-26 08:59:53.082538 awswrangler-3.3.0/awswrangler/s3/_list.py
+-rw-r--r--   0        0        0     4158 2023-06-26 08:59:53.083356 awswrangler-3.3.0/awswrangler/s3/_list.pyi
+-rw-r--r--   0        0        0    15344 2023-06-26 08:59:53.083733 awswrangler-3.3.0/awswrangler/s3/_read.py
+-rw-r--r--   0        0        0     4140 2023-07-31 18:52:13.846238 awswrangler-3.3.0/awswrangler/s3/_read_deltalake.py
+-rw-r--r--   0        0        0     3277 2023-06-26 08:59:53.084466 awswrangler-3.3.0/awswrangler/s3/_read_excel.py
+-rw-r--r--   0        0        0    23265 2023-06-26 08:59:53.084726 awswrangler-3.3.0/awswrangler/s3/_read_orc.py
+-rw-r--r--   0        0        0    33910 2023-08-01 07:18:46.954341 awswrangler-3.3.0/awswrangler/s3/_read_parquet.py
+-rw-r--r--   0        0        0    10040 2023-06-26 08:59:53.085485 awswrangler-3.3.0/awswrangler/s3/_read_parquet.pyi
+-rw-r--r--   0        0        0    27928 2023-08-01 07:18:46.956263 awswrangler-3.3.0/awswrangler/s3/_read_text.py
+-rw-r--r--   0        0        0     7993 2023-06-26 08:59:53.086278 awswrangler-3.3.0/awswrangler/s3/_read_text.pyi
+-rw-r--r--   0        0        0     4108 2023-06-26 08:59:53.086656 awswrangler-3.3.0/awswrangler/s3/_read_text_core.py
+-rw-r--r--   0        0        0    12569 2023-07-21 13:12:51.771650 awswrangler-3.3.0/awswrangler/s3/_select.py
+-rw-r--r--   0        0        0     2465 2023-06-26 08:59:53.087459 awswrangler-3.3.0/awswrangler/s3/_upload.py
+-rw-r--r--   0        0        0     6205 2023-06-26 08:59:53.088085 awswrangler-3.3.0/awswrangler/s3/_wait.py
+-rw-r--r--   0        0        0    18399 2023-07-06 13:00:08.512133 awswrangler-3.3.0/awswrangler/s3/_write.py
+-rw-r--r--   0        0        0     1840 2023-06-26 08:59:53.088974 awswrangler-3.3.0/awswrangler/s3/_write_concurrent.py
+-rw-r--r--   0        0        0    12740 2023-06-26 08:59:53.090201 awswrangler-3.3.0/awswrangler/s3/_write_dataset.py
+-rw-r--r--   0        0        0     4144 2023-06-26 08:59:53.090692 awswrangler-3.3.0/awswrangler/s3/_write_deltalake.py
+-rw-r--r--   0        0        0     3196 2023-06-26 08:59:53.090990 awswrangler-3.3.0/awswrangler/s3/_write_excel.py
+-rw-r--r--   0        0        0    26700 2023-06-26 08:59:53.091218 awswrangler-3.3.0/awswrangler/s3/_write_orc.py
+-rw-r--r--   0        0        0    39437 2023-08-01 07:18:46.957510 awswrangler-3.3.0/awswrangler/s3/_write_parquet.py
+-rw-r--r--   0        0        0    48588 2023-08-01 07:18:46.958923 awswrangler-3.3.0/awswrangler/s3/_write_text.py
+-rw-r--r--   0        0        0     2018 2023-06-26 08:59:53.092788 awswrangler-3.3.0/awswrangler/secretsmanager.py
+-rw-r--r--   0        0        0    19421 2023-06-26 08:59:53.093180 awswrangler-3.3.0/awswrangler/sqlserver.py
+-rw-r--r--   0        0        0     1853 2023-06-26 08:59:53.093618 awswrangler-3.3.0/awswrangler/sts.py
+-rw-r--r--   0        0        0      727 2023-06-26 08:59:53.094380 awswrangler-3.3.0/awswrangler/timestream/__init__.py
+-rw-r--r--   0        0        0     4512 2023-06-26 08:59:53.094973 awswrangler-3.3.0/awswrangler/timestream/_create.py
+-rw-r--r--   0        0        0     2491 2023-06-26 08:59:53.095125 awswrangler-3.3.0/awswrangler/timestream/_delete.py
+-rw-r--r--   0        0        0     2603 2023-06-26 08:59:53.095533 awswrangler-3.3.0/awswrangler/timestream/_list.py
+-rw-r--r--   0        0        0    16998 2023-06-26 08:59:53.096081 awswrangler-3.3.0/awswrangler/timestream/_read.py
+-rw-r--r--   0        0        0     1910 2023-06-26 08:59:53.096727 awswrangler-3.3.0/awswrangler/timestream/_read.pyi
+-rw-r--r--   0        0        0    26397 2023-06-26 08:59:53.097213 awswrangler-3.3.0/awswrangler/timestream/_write.py
+-rw-r--r--   0        0        0     9355 2023-06-26 08:59:53.097404 awswrangler-3.3.0/awswrangler/typing.py
+-rw-r--r--   0        0        0     4803 2023-08-01 07:18:46.961758 awswrangler-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0    23012 1970-01-01 00:00:00.000000 awswrangler-3.3.0/PKG-INFO
```

### Comparing `awswrangler-3.2.1/LICENSE.txt` & `awswrangler-3.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/README.md` & `awswrangler-3.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 Easy integration with Athena, Glue, Redshift, Timestream, OpenSearch, Neptune, QuickSight, Chime, CloudWatchLogs, DynamoDB, EMR, SecretManager, PostgreSQL, MySQL, SQLServer and S3 (Parquet, CSV, JSON and EXCEL).
 
 ![AWS SDK for pandas](docs/source/_static/logo2.png?raw=true "AWS SDK for pandas")
 ![tracker](https://d3tiqpr4kkkomd.cloudfront.net/img/pixel.png?asset=GVOYN2BOOQ573LTVIHEW)
 
 > An [AWS Professional Service](https://aws.amazon.com/professional-services/) open source initiative | aws-proserve-opensource@amazon.com
 
-[![Release](https://img.shields.io/badge/3.2.1-brightgreen.svg)](https://pypi.org/project/awswrangler/)
-[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.8%20%7C%203.9%20%7C%203.10-brightgreen.svg)](https://anaconda.org/conda-forge/awswrangler)
+[![Release](https://img.shields.io/badge/3.3.0-brightgreen.svg)](https://pypi.org/project/awswrangler/)
+[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-brightgreen.svg)](https://anaconda.org/conda-forge/awswrangler)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 ![Static Checking](https://github.com/aws/aws-sdk-pandas/workflows/Static%20Checking/badge.svg?branch=main)
 [![Documentation Status](https://readthedocs.org/projects/aws-sdk-pandas/badge/?version=latest)](https://aws-sdk-pandas.readthedocs.io/?badge=latest)
 
@@ -95,33 +95,33 @@
 """)
 
 ```
 
 ## At scale
 AWS SDK for pandas can also run your workflows at scale by leveraging [Modin](https://modin.readthedocs.io/en/stable/) and [Ray](https://www.ray.io/). Both projects aim to speed up data workloads by distributing processing over a cluster of workers.
 
-The quickest way to get started is to use AWS Glue with Ray. Read our [docs](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/scale.html), our [blog](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/), or head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials) to discover even more features.
+The quickest way to get started is to use AWS Glue with Ray. Read our [docs](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/scale.html), our blogs ([1](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/)/[2](https://aws.amazon.com/blogs/big-data/advanced-patterns-with-aws-sdk-for-pandas-on-aws-glue-for-ray/)), or head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials) to discover even more features.
 
 ## [Read The Docs](https://aws-sdk-pandas.readthedocs.io/)
 
-- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/about.html)
-- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html)
-  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#pypi-pip)
-  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#conda)
-  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#aws-lambda-layer)
-  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#aws-glue-python-shell-jobs)
-  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#aws-glue-pyspark-jobs)
-  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#amazon-sagemaker-notebook)
-  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#amazon-sagemaker-notebook-lifecycle)
-  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#emr)
-  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#from-source)
-- [**At scale**](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/scale.html)
-  - [Getting Started](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/scale.html#getting-started)
-  - [Supported APIs](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/scale.html#supported-apis)
-  - [Resources](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/scale.html#resources)
+- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/about.html)
+- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/install.html)
+  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/install.html#pypi-pip)
+  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/install.html#conda)
+  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/install.html#aws-lambda-layer)
+  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/install.html#aws-glue-python-shell-jobs)
+  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/install.html#aws-glue-pyspark-jobs)
+  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/install.html#amazon-sagemaker-notebook)
+  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/install.html#amazon-sagemaker-notebook-lifecycle)
+  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/install.html#emr)
+  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/install.html#from-source)
+- [**At scale**](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/scale.html)
+  - [Getting Started](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/scale.html#getting-started)
+  - [Supported APIs](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/scale.html#supported-apis)
+  - [Resources](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/scale.html#resources)
 - [**Tutorials**](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials)
   - [001 - Introduction](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/001%20-%20Introduction.ipynb)
   - [002 - Sessions](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/002%20-%20Sessions.ipynb)
   - [003 - Amazon S3](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/003%20-%20Amazon%20S3.ipynb)
   - [004 - Parquet Datasets](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/004%20-%20Parquet%20Datasets.ipynb)
   - [005 - Glue Catalog](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/005%20-%20Glue%20Catalog.ipynb)
   - [006 - Amazon Athena](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/006%20-%20Amazon%20Athena.ipynb)
@@ -154,39 +154,41 @@
   - [033 - Amazon Neptune](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/033%20-%20Amazon%20Neptune.ipynb)
   - [034 - Distributing Calls Using Ray](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/034%20-%20Distributing%20Calls%20using%20Ray.ipynb)
   - [035 - Distributing Calls on Ray Remote Cluster](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/035%20-%20Distributing%20Calls%20on%20Ray%20Remote%20Cluster.ipynb)
   - [036 - Distributing Calls with Glue Interactive Sessions on Ray](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/036%20-%20Distributing%20Calls%20with%20Glue%20Interactive%20Sessions%20on%20Ray.ipynb)
   - [037 - Glue Data Quality](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/037%20-%20Glue%20Data%20Quality.ipynb)
   - [038 - OpenSearch Serverless](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/038%20-%20OpenSearch%20Serverless.ipynb)
   - [039 - Athena Iceberg](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/039%20-%20Athena%20Iceberg.ipynb)
-- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html)
-  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-s3)
-  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#aws-glue-catalog)
-  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-athena)
-  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#aws-lake-formation)
-  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-redshift)
-  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#postgresql)
-  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#mysql)
-  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#sqlserver)
-  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#oracle)
-  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#data-api-redshift)
-  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#data-api-rds)
-  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#opensearch)
-  - [AWS Glue Data Quality](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#aws-glue-data-quality)
-  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-neptune)
-  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#dynamodb)
-  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-timestream)
-  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-emr)
-  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-cloudwatch-logs)
-  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-chime)
-  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-quicksight)
-  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#aws-sts)
-  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#aws-secrets-manager)
-  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#global-configurations)
-  - [Distributed - Ray](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#distributed-ray)
+  - [040 - EMR Serverless](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/040%20-%20EMR%20Serverless.ipynb)
+  - [041 - Apache Spark on Amazon Athena](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/041%20-%20Apache%20Spark%20on%20Amazon%20Athena.ipynb)
+- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html)
+  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#amazon-s3)
+  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#aws-glue-catalog)
+  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#amazon-athena)
+  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#aws-lake-formation)
+  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#amazon-redshift)
+  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#postgresql)
+  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#mysql)
+  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#sqlserver)
+  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#oracle)
+  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#data-api-redshift)
+  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#data-api-rds)
+  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#opensearch)
+  - [AWS Glue Data Quality](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#aws-glue-data-quality)
+  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#amazon-neptune)
+  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#dynamodb)
+  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#amazon-timestream)
+  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#amazon-emr)
+  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#amazon-cloudwatch-logs)
+  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#amazon-chime)
+  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#amazon-quicksight)
+  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#aws-sts)
+  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#aws-secrets-manager)
+  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#global-configurations)
+  - [Distributed - Ray](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#distributed-ray)
 - [**License**](https://github.com/aws/aws-sdk-pandas/blob/main/LICENSE.txt)
 - [**Contributing**](https://github.com/aws/aws-sdk-pandas/blob/main/CONTRIBUTING.md)
 
 ## Getting Help
 
 The best way to interact with our team is through GitHub. You can open an [issue](https://github.com/aws/aws-sdk-pandas/issues/new/choose) and choose from one of our templates for bug reports, feature requests...
 You may also find help on these community resources:
@@ -195,14 +197,15 @@
   and tag it with `awswrangler`
 * [Runbook](https://github.com/aws/aws-sdk-pandas/discussions/1815) for AWS SDK for pandas with Ray
 
 ## Community Resources
 
 Please [send a Pull Request](https://github.com/aws/aws-sdk-pandas/edit/main/README.md) with your resource reference and @githubhandle.
 
+- [YouTube channel](https://www.youtube.com/playlist?list=PL7bE4nSzLSWdDdlfRgfKo2JBplB4p_v5O) [[@AdrianoNicolucci](https://github.com/AdrianoNicolucci)]
 - [Optimize Python ETL by extending Pandas with AWS SDK for pandas](https://aws.amazon.com/blogs/big-data/optimize-python-etl-by-extending-pandas-with-aws-data-wrangler/) [[@igorborgest](https://github.com/igorborgest)]
 - [Reading Parquet Files With AWS Lambda](https://aprakash.wordpress.com/2020/04/14/reading-parquet-files-with-aws-lambda/) [[@anand086](https://github.com/anand086)]
 - [Transform AWS CloudTrail data using AWS SDK for pandas](https://aprakash.wordpress.com/2020/09/17/transform-aws-cloudtrail-data-using-aws-data-wrangler/) [[@anand086](https://github.com/anand086)]
 - [Rename Glue Tables using AWS SDK for pandas](https://ananddatastories.com/rename-glue-tables-using-aws-sdk-pandas/) [[@anand086](https://github.com/anand086)]
 - [Getting started on AWS SDK for pandas and Athena](https://medium.com/@dheerajsharmainampudi/getting-started-on-aws-sdk-pandas-and-athena-7b446c834076) [[@dheerajsharma21](https://github.com/dheerajsharma21)]
 - [Simplifying Pandas integration with AWS data related services](https://medium.com/@bv_subhash/aws-sdk-pandas-simplifying-pandas-integration-with-aws-data-related-services-2b3325c12188) [[@bvsubhash](https://github.com/bvsubhash)]
 - [Build an ETL pipeline using AWS S3, Glue and Athena](https://www.linkedin.com/pulse/build-etl-pipeline-using-aws-s3-glue-athena-data-wrangler-tom-reid/) [[@taupirho](https://github.com/taupirho)]
@@ -238,14 +241,15 @@
 - [DNX](https://www.dnx.solutions/) [[@DNXLabs](https://github.com/DNXLabs)]
 - [Fortescue Future Industries](https://ffi.com.au/) [[@spencervoorend](https://github.com/spencervoorend)]
 - [Funcional Health Tech](https://www.funcionalcorp.com.br/) [[@webysther](https://github.com/webysther)]
 - [Funding Circle](https://www.fundingcircle.com/) [[@pfig](https://github.com/pfig)]
 - [Infomach](https://www.infomach.com.br/)
 - [Informa Markets](https://www.informamarkets.com/en/home.html) [[@mateusmorato]](http://github.com/mateusmorato)
 - [LINE TV](https://www.linetv.tw/) [[@bryanyang0528](https://github.com/bryanyang0528)]
+- [LogicalCube](https://www.logicalcube.com) [[@zolabud](https://github.com/zolabud)]
 - [Magnataur](https://magnataur.com) [[@brianmingus2](https://github.com/brianmingus2)]
 - [M4U](https://www.m4u.com.br/) [[@Thiago-Dantas](https://github.com/Thiago-Dantas)]
 - [NBCUniversal](https://www.nbcuniversal.com/) [[@vibe](https://github.com/vibe)]
 - [nrd.io](https://nrd.io/) [[@mrtns](https://github.com/mrtns)]
 - [OKRA Technologies](https://okra.ai) [[@JPFrancoia](https://github.com/JPFrancoia), [@schot](https://github.com/schot)]
 - [Pier](https://www.pier.digital/) [[@flaviomax](https://github.com/flaviomax)]
 - [Pismo](https://www.pismo.io/) [[@msantino](https://github.com/msantino)]
```

### Comparing `awswrangler-3.2.1/THIRD_PARTY.txt` & `awswrangler-3.3.0/THIRD_PARTY.txt`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/__init__.py` & `awswrangler-3.3.0/awswrangler/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import logging as _logging
 
 from awswrangler import (  # noqa
     athena,
     catalog,
     chime,
+    cleanrooms,
     cloudwatch,
     data_api,
     data_quality,
     dynamodb,
     emr,
     emr_serverless,
     exceptions,
@@ -39,14 +40,15 @@
 
 engine.register()
 
 __all__ = [
     "athena",
     "catalog",
     "chime",
+    "cleanrooms",
     "cloudwatch",
     "emr",
     "emr_serverless",
     "data_api",
     "data_quality",
     "dynamodb",
     "exceptions",
```

### Comparing `awswrangler-3.2.1/awswrangler/_arrow.py` & `awswrangler-3.3.0/awswrangler/_arrow.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import datetime
 import json
 import logging
 from typing import Any, Dict, Optional, Tuple, cast
 
 import pyarrow as pa
+import pytz
 
 import awswrangler.pandas as pd
 from awswrangler._data_types import athena2pyarrow
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
@@ -67,15 +68,16 @@
         else:
             continue
         if col_name in df.columns and c["pandas_type"] == "datetimetz":
             timezone: datetime.tzinfo = pa.lib.string_to_tzinfo(c["metadata"]["timezone"])
             _logger.debug("applying timezone (%s) on column %s", timezone, col_name)
             if hasattr(df[col_name].dtype, "tz") is False:
                 df[col_name] = df[col_name].dt.tz_localize(tz="UTC")
-            df[col_name] = df[col_name].dt.tz_convert(tz=timezone)
+            if timezone is not None and timezone != pytz.UTC and hasattr(df[col_name].dt, "tz_convert"):
+                df[col_name] = df[col_name].dt.tz_convert(tz=timezone)
     return df
 
 
 def _table_to_df(
     table: pa.Table,
     kwargs: Dict[str, Any],
 ) -> pd.DataFrame:
```

### Comparing `awswrangler-3.2.1/awswrangler/_config.py` & `awswrangler-3.3.0/awswrangler/_config.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/_data_types.py` & `awswrangler-3.3.0/awswrangler/_data_types.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/_databases.py` & `awswrangler-3.3.0/awswrangler/_databases.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/_distributed.py` & `awswrangler-3.3.0/awswrangler/_distributed.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/_executor.py` & `awswrangler-3.3.0/awswrangler/_executor.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/_sql_formatter.py` & `awswrangler-3.3.0/awswrangler/_sql_formatter.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/_utils.py` & `awswrangler-3.3.0/awswrangler/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 from awswrangler._config import _insert_str, apply_configs
 from awswrangler._distributed import EngineEnum, engine
 
 if TYPE_CHECKING:
     from boto3.resources.base import ServiceResource
     from botocore.client import BaseClient
     from mypy_boto3_athena import AthenaClient
+    from mypy_boto3_cleanrooms import CleanRoomsServiceClient
     from mypy_boto3_dynamodb import DynamoDBClient, DynamoDBServiceResource
     from mypy_boto3_ec2 import EC2Client
     from mypy_boto3_emr.client import EMRClient
     from mypy_boto3_emr_serverless import EMRServerlessClient
     from mypy_boto3_glue import GlueClient
     from mypy_boto3_kms.client import KMSClient
     from mypy_boto3_lakeformation.client import LakeFormationClient
@@ -64,14 +65,15 @@
     from mypy_boto3_sts.client import STSClient
     from mypy_boto3_timestream_query.client import TimestreamQueryClient
     from mypy_boto3_timestream_write.client import TimestreamWriteClient
     from typing_extensions import Literal
 
     ServiceName = Literal[
         "athena",
+        "cleanrooms",
         "dynamodb",
         "ec2",
         "emr",
         "emr-serverless",
         "glue",
         "kms",
         "lakeformation",
@@ -284,14 +286,24 @@
     verify: Optional[Union[str, bool]] = None,
 ) -> "AthenaClient":
     ...
 
 
 @overload
 def client(
+    service_name: 'Literal["cleanrooms"]',
+    session: Optional[boto3.Session] = None,
+    botocore_config: Optional[Config] = None,
+    verify: Optional[Union[str, bool]] = None,
+) -> "CleanRoomsServiceClient":
+    ...
+
+
+@overload
+def client(
     service_name: 'Literal["lakeformation"]',
     session: Optional[boto3.Session] = None,
     botocore_config: Optional[Config] = None,
     verify: Optional[Union[str, bool]] = None,
 ) -> "LakeFormationClient":
     ...
```

### Comparing `awswrangler-3.2.1/awswrangler/annotations.py` & `awswrangler-3.3.0/awswrangler/annotations.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/athena/__init__.py` & `awswrangler-3.3.0/awswrangler/athena/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 from awswrangler.athena._executions import (  # noqa
     get_query_execution,
     stop_query_execution,
     start_query_execution,
     wait_query,
 )
 from awswrangler.athena._spark import create_spark_session, run_spark_calculation
+from awswrangler.athena._statements import (
+    create_prepared_statement,
+    delete_prepared_statement,
+    list_prepared_statements,
+)
 from awswrangler.athena._read import (  # noqa
     get_query_results,
     read_sql_query,
     read_sql_table,
     unload,
 )
 from awswrangler.athena._utils import (  # noqa
@@ -47,9 +52,12 @@
     "run_spark_calculation",
     "create_ctas_table",
     "show_create_table",
     "start_query_execution",
     "stop_query_execution",
     "unload",
     "wait_query",
+    "create_prepared_statement",
+    "list_prepared_statements",
+    "delete_prepared_statement",
     "to_iceberg",
 ]
```

### Comparing `awswrangler-3.2.1/awswrangler/athena/_cache.py` & `awswrangler-3.3.0/awswrangler/athena/_cache.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/athena/_executions.py` & `awswrangler-3.3.0/awswrangler/athena/_executions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """Query executions Module for Amazon Athena."""
 import logging
 import time
 from typing import (
     Any,
     Dict,
+    List,
     Optional,
     Union,
     cast,
 )
 
 import boto3
 import botocore
+from typing_extensions import Literal
 
 from awswrangler import _utils, exceptions, typing
 from awswrangler._config import apply_configs
-from awswrangler._sql_formatter import _process_sql_params
 
 from ._cache import _cache_manager, _CacheInfo, _check_for_cached_results
 from ._utils import (
     _QUERY_FINAL_STATES,
     _QUERY_WAIT_POLLING_DELAY,
+    _apply_formatter,
     _get_workgroup_config,
     _start_query_execution,
     _WorkGroupConfig,
 )
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
@@ -32,15 +34,16 @@
 def start_query_execution(
     sql: str,
     database: Optional[str] = None,
     s3_output: Optional[str] = None,
     workgroup: Optional[str] = None,
     encryption: Optional[str] = None,
     kms_key: Optional[str] = None,
-    params: Optional[Dict[str, Any]] = None,
+    params: Union[Dict[str, Any], List[str], None] = None,
+    paramstyle: Literal["qmark", "named"] = "named",
     boto3_session: Optional[boto3.Session] = None,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = None,
     athena_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY,
     data_source: Optional[str] = None,
     wait: bool = False,
 ) -> Union[str, Dict[str, Any]]:
     """Start a SQL Query against AWS Athena.
@@ -60,18 +63,33 @@
         AWS S3 path.
     workgroup : str, optional
         Athena workgroup.
     encryption : str, optional
         None, 'SSE_S3', 'SSE_KMS', 'CSE_KMS'.
     kms_key : str, optional
         For SSE-KMS and CSE-KMS , this is the KMS key ARN or ID.
-    params: Dict[str, any], optional
-        Dict of parameters that will be used for constructing the SQL query. Only named parameters are supported.
-        The dict needs to contain the information in the form {'name': 'value'} and the SQL query needs to contain
-        `:name`. Note that for varchar columns and similar, you must surround the value in single quotes.
+    params: Dict[str, any] | List[str], optional
+        Parameters that will be used for constructing the SQL query.
+        Only named or question mark parameters are supported.
+        The parameter style needs to be specified in the ``paramstyle`` parameter.
+
+        For ``paramstyle="named"``, this value needs to be a dictionary.
+        The dict needs to contain the information in the form ``{'name': 'value'}`` and the SQL query needs to contain
+        ``:name``.
+        The formatter will be applied client-side in this scenario.
+
+        For ``paramstyle="qmark"``, this value needs to be a list of strings.
+        The formatter will be applied server-side.
+        The values are applied sequentially to the parameters in the query in the order in which the parameters occur.
+    paramstyle: str, optional
+        Determines the style of ``params``.
+        Possible values are:
+
+        - ``named``
+        - ``qmark``
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
     athena_cache_settings: typing.AthenaCacheSettings, optional
         Parameters of the Athena cache settings such as max_cache_seconds, max_cache_query_inspections,
         max_remote_cache_entries, and max_local_cache_entries.
         AthenaCacheSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
         instance of AthenaCacheSettings or as a regular Python dict.
@@ -99,15 +117,16 @@
 
     Querying into another data source (PostgreSQL, Redshift, etc)
 
     >>> import awswrangler as wr
     >>> query_exec_id = wr.athena.start_query_execution(sql='...', database='...', data_source='...')
 
     """
-    sql = _process_sql_params(sql, params)
+    # Substitute query parameters if applicable
+    sql, execution_params = _apply_formatter(sql, params, paramstyle)
     _logger.debug("Executing query:\n%s", sql)
 
     athena_cache_settings = athena_cache_settings if athena_cache_settings else {}
     max_cache_seconds = athena_cache_settings.get("max_cache_seconds", 0)
     max_cache_query_inspections = athena_cache_settings.get("max_cache_query_inspections", 50)
     max_remote_cache_entries = athena_cache_settings.get("max_remote_cache_entries", 50)
     max_local_cache_entries = athena_cache_settings.get("max_local_cache_entries", 100)
@@ -135,14 +154,15 @@
             wg_config=wg_config,
             database=database,
             data_source=data_source,
             s3_output=s3_output,
             workgroup=workgroup,
             encryption=encryption,
             kms_key=kms_key,
+            execution_params=execution_params,
             boto3_session=boto3_session,
         )
     if wait:
         return wait_query(
             query_execution_id=query_execution_id,
             boto3_session=boto3_session,
             athena_query_wait_polling_delay=athena_query_wait_polling_delay,
```

### Comparing `awswrangler-3.2.1/awswrangler/athena/_executions.pyi` & `awswrangler-3.3.0/awswrangler/athena/_executions.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import (
     Any,
     Dict,
+    List,
     Literal,
     Optional,
     Union,
     overload,
 )
 
 import boto3
@@ -15,15 +16,16 @@
 def start_query_execution(
     sql: str,
     database: Optional[str] = ...,
     s3_output: Optional[str] = ...,
     workgroup: Optional[str] = ...,
     encryption: Optional[str] = ...,
     kms_key: Optional[str] = ...,
-    params: Optional[Dict[str, Any]] = ...,
+    params: Union[Dict[str, Any], List[str], None] = ...,
+    paramstyle: Literal["qmark", "named"] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
     athena_query_wait_polling_delay: float = ...,
     data_source: Optional[str] = ...,
     wait: Literal[False] = ...,
 ) -> str: ...
 @overload
@@ -31,15 +33,16 @@
     sql: str,
     *,
     database: Optional[str] = ...,
     s3_output: Optional[str] = ...,
     workgroup: Optional[str] = ...,
     encryption: Optional[str] = ...,
     kms_key: Optional[str] = ...,
-    params: Optional[Dict[str, Any]] = ...,
+    params: Union[Dict[str, Any], List[str], None] = ...,
+    paramstyle: Literal["qmark", "named"] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
     athena_query_wait_polling_delay: float = ...,
     data_source: Optional[str] = ...,
     wait: Literal[True],
 ) -> Dict[str, Any]: ...
 @overload
@@ -47,15 +50,16 @@
     sql: str,
     *,
     database: Optional[str] = ...,
     s3_output: Optional[str] = ...,
     workgroup: Optional[str] = ...,
     encryption: Optional[str] = ...,
     kms_key: Optional[str] = ...,
-    params: Optional[Dict[str, Any]] = ...,
+    params: Union[Dict[str, Any], List[str], None] = ...,
+    paramstyle: Literal["qmark", "named"] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
     athena_query_wait_polling_delay: float = ...,
     data_source: Optional[str] = ...,
     wait: bool,
 ) -> Union[str, Dict[str, Any]]: ...
 def stop_query_execution(query_execution_id: str, boto3_session: Optional[boto3.Session] = ...) -> None: ...
```

### Comparing `awswrangler-3.2.1/awswrangler/athena/_read.py` & `awswrangler-3.3.0/awswrangler/athena/_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 import botocore.exceptions
 import pandas as pd
 from typing_extensions import Literal
 
 from awswrangler import _utils, catalog, exceptions, s3, typing
 from awswrangler._config import apply_configs
 from awswrangler._data_types import cast_pandas_with_athena_types
-from awswrangler._sql_formatter import _process_sql_params
 from awswrangler.athena._utils import (
     _QUERY_WAIT_POLLING_DELAY,
+    _apply_formatter,
     _apply_query_metadata,
     _empty_dataframe_response,
     _get_query_metadata,
     _get_s3_output,
     _get_workgroup_config,
     _QueryMetadata,
     _start_query_execution,
@@ -283,14 +283,15 @@
     ctas_bucketing_info: Optional[typing.BucketingInfoTuple],
     ctas_write_compression: Optional[str],
     athena_query_wait_polling_delay: float,
     use_threads: Union[bool, int],
     s3_additional_kwargs: Optional[Dict[str, Any]],
     boto3_session: Optional[boto3.Session],
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
+    execution_params: Optional[List[str]] = None,
     dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     ctas_query_info: Dict[str, Union[str, _QueryMetadata]] = create_ctas_table(
         sql=sql,
         database=database,
         ctas_table=name,
         ctas_database=alt_database,
@@ -300,14 +301,15 @@
         workgroup=workgroup,
         encryption=encryption,
         write_compression=ctas_write_compression,
         kms_key=kms_key,
         wait=True,
         athena_query_wait_polling_delay=athena_query_wait_polling_delay,
         boto3_session=boto3_session,
+        execution_params=execution_params,
     )
     fully_qualified_name: str = f'"{ctas_query_info["ctas_database"]}"."{ctas_query_info["ctas_table"]}"'
     ctas_query_metadata = cast(_QueryMetadata, ctas_query_info["ctas_query_metadata"])
     _logger.debug("CTAS query metadata: %s", ctas_query_metadata)
     return _fetch_parquet_result(
         query_metadata=ctas_query_metadata,
         keep_files=keep_files,
@@ -338,14 +340,15 @@
     kms_key: Optional[str],
     workgroup: Optional[str],
     use_threads: Union[bool, int],
     athena_query_wait_polling_delay: float,
     s3_additional_kwargs: Optional[Dict[str, Any]],
     boto3_session: Optional[boto3.Session],
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
+    execution_params: Optional[List[str]] = None,
     dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     query_metadata = _unload(
         sql=sql,
         path=s3_output,
         file_format=file_format,
         compression=compression,
@@ -354,14 +357,15 @@
         workgroup=workgroup,
         database=database,
         encryption=encryption,
         kms_key=kms_key,
         boto3_session=boto3_session,
         data_source=data_source,
         athena_query_wait_polling_delay=athena_query_wait_polling_delay,
+        execution_params=execution_params,
     )
     if file_format == "PARQUET":
         return _fetch_parquet_result(
             query_metadata=query_metadata,
             keep_files=keep_files,
             categories=categories,
             chunksize=chunksize,
@@ -385,14 +389,15 @@
     encryption: Optional[str],
     workgroup: Optional[str],
     kms_key: Optional[str],
     use_threads: Union[bool, int],
     athena_query_wait_polling_delay: float,
     s3_additional_kwargs: Optional[Dict[str, Any]],
     boto3_session: Optional[boto3.Session],
+    execution_params: Optional[List[str]] = None,
     dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     wg_config: _WorkGroupConfig = _get_workgroup_config(session=boto3_session, workgroup=workgroup)
     s3_output = _get_s3_output(s3_output=s3_output, wg_config=wg_config, boto3_session=boto3_session)
     s3_output = s3_output[:-1] if s3_output[-1] == "/" else s3_output
     _logger.debug("Executing sql: %s", sql)
     query_id: str = _start_query_execution(
@@ -400,14 +405,15 @@
         wg_config=wg_config,
         database=database,
         data_source=data_source,
         s3_output=s3_output,
         workgroup=workgroup,
         encryption=encryption,
         kms_key=kms_key,
+        execution_params=execution_params,
         boto3_session=boto3_session,
     )
     _logger.debug("Query id: %s", query_id)
     query_metadata: _QueryMetadata = _get_query_metadata(
         query_execution_id=query_id,
         boto3_session=boto3_session,
         categories=categories,
@@ -446,14 +452,15 @@
     ctas_bucketing_info: Optional[typing.BucketingInfoTuple],
     ctas_write_compression: Optional[str],
     athena_query_wait_polling_delay: float,
     use_threads: Union[bool, int],
     s3_additional_kwargs: Optional[Dict[str, Any]],
     boto3_session: Optional[boto3.Session],
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
+    execution_params: Optional[List[str]] = None,
     dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """
     Execute a query in Athena and returns results as DataFrame, back to `read_sql_query`.
 
     Usually called by `read_sql_query` when using cache is not possible.
     """
@@ -479,14 +486,15 @@
                 ctas_bucketing_info=ctas_bucketing_info,
                 ctas_write_compression=ctas_write_compression,
                 athena_query_wait_polling_delay=athena_query_wait_polling_delay,
                 use_threads=use_threads,
                 s3_additional_kwargs=s3_additional_kwargs,
                 boto3_session=boto3_session,
                 pyarrow_additional_kwargs=pyarrow_additional_kwargs,
+                execution_params=execution_params,
                 dtype_backend=dtype_backend,
             )
         finally:
             catalog.delete_table_if_exists(database=ctas_database or database, table=name, boto3_session=boto3_session)
     elif unload_approach is True:
         if unload_parameters is None:
             unload_parameters = {}
@@ -506,14 +514,15 @@
             kms_key=kms_key,
             workgroup=workgroup,
             use_threads=use_threads,
             athena_query_wait_polling_delay=athena_query_wait_polling_delay,
             s3_additional_kwargs=s3_additional_kwargs,
             boto3_session=boto3_session,
             pyarrow_additional_kwargs=pyarrow_additional_kwargs,
+            execution_params=execution_params,
             dtype_backend=dtype_backend,
         )
     return _resolve_query_without_cache_regular(
         sql=sql,
         database=database,
         data_source=data_source,
         s3_output=s3_output,
@@ -523,14 +532,15 @@
         encryption=encryption,
         workgroup=workgroup,
         kms_key=kms_key,
         use_threads=use_threads,
         athena_query_wait_polling_delay=athena_query_wait_polling_delay,
         s3_additional_kwargs=s3_additional_kwargs,
         boto3_session=boto3_session,
+        execution_params=execution_params,
         dtype_backend=dtype_backend,
     )
 
 
 def _unload(
     sql: str,
     path: Optional[str],
@@ -541,14 +551,15 @@
     workgroup: Optional[str],
     database: Optional[str],
     encryption: Optional[str],
     kms_key: Optional[str],
     boto3_session: Optional[boto3.Session],
     data_source: Optional[str],
     athena_query_wait_polling_delay: float,
+    execution_params: Optional[List[str]],
 ) -> _QueryMetadata:
     wg_config: _WorkGroupConfig = _get_workgroup_config(session=boto3_session, workgroup=workgroup)
     s3_output: str = _get_s3_output(s3_output=path, wg_config=wg_config, boto3_session=boto3_session)
     s3_output = s3_output[:-1] if s3_output[-1] == "/" else s3_output
     # Athena does not enforce a Query Result Location for UNLOAD. Thus, the workgroup output location
     # is only used if no path is supplied.
     if not path:
@@ -572,14 +583,15 @@
             wg_config=wg_config,
             database=database,
             data_source=data_source,
             s3_output=s3_output,
             encryption=encryption,
             kms_key=kms_key,
             boto3_session=boto3_session,
+            execution_params=execution_params,
         )
     except botocore.exceptions.ClientError as ex:
         msg: str = str(ex)
         error = ex.response["Error"]
         if error["Code"] == "InvalidRequestException":
             raise exceptions.InvalidArgumentValue(f"Exception parsing query. Root error message: {msg}")
         raise ex
@@ -731,28 +743,29 @@
     kms_key: Optional[str] = None,
     keep_files: bool = True,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = None,
     data_source: Optional[str] = None,
     athena_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY,
-    params: Optional[Dict[str, Any]] = None,
+    params: Union[Dict[str, Any], List[str], None] = None,
+    paramstyle: Literal["qmark", "named"] = "named",
     dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Execute any SQL query on AWS Athena and return the results as a Pandas DataFrame.
 
     **Related tutorial:**
 
-    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.2.1/
+    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.3.0/
       tutorials/006%20-%20Amazon%20Athena.html>`_
-    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.2.1/
+    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.3.0/
       tutorials/019%20-%20Athena%20Cache.html>`_
-    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.2.1/
+    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.3.0/
       tutorials/021%20-%20Global%20Configurations.html>`_
 
     **There are three approaches available through ctas_approach and unload_approach parameters:**
 
     **1** - ctas_approach=True (Default):
 
     Wrap the query with a CTAS and then reads the table data as parquet directly from s3.
@@ -808,15 +821,15 @@
     ----
     The resulting DataFrame (or every DataFrame in the returned Iterator for chunked queries) have a
     `query_metadata` attribute, which brings the query result metadata returned by
     `Boto3/Athena <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services
     /athena.html#Athena.Client.get_query_execution>`_ .
 
     For a practical example check out the
-    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.2.1/
+    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.3.0/
     tutorials/024%20-%20Athena%20Query%20Metadata.html>`_!
 
 
     Note
     ----
     Valid encryption modes: [None, 'SSE_S3', 'SSE_KMS'].
 
@@ -901,18 +914,33 @@
         If cached results are valid, awswrangler ignores the `ctas_approach`, `s3_output`, `encryption`, `kms_key`,
         `keep_files` and `ctas_temp_table_name` params.
         If reading cached data fails for any reason, execution falls back to the usual query run path.
     data_source : str, optional
         Data Source / Catalog name. If None, 'AwsDataCatalog' will be used by default.
     athena_query_wait_polling_delay: float, default: 0.25 seconds
         Interval in seconds for how often the function will check if the Athena query has completed.
-    params: Dict[str, any], optional
-        Dict of parameters that will be used for constructing the SQL query. Only named parameters are supported.
-        The dict needs to contain the information in the form {'name': 'value'} and the SQL query needs to contain
-        `:name`. Note that for varchar columns and similar, you must surround the value in single quotes.
+    params: Dict[str, any] | List[str], optional
+        Parameters that will be used for constructing the SQL query.
+        Only named or question mark parameters are supported.
+        The parameter style needs to be specified in the ``paramstyle`` parameter.
+
+        For ``paramstyle="named"``, this value needs to be a dictionary.
+        The dict needs to contain the information in the form ``{'name': 'value'}`` and the SQL query needs to contain
+        ``:name``.
+        The formatter will be applied client-side in this scenario.
+
+        For ``paramstyle="qmark"``, this value needs to be a list of strings.
+        The formatter will be applied server-side.
+        The values are applied sequentially to the parameters in the query in the order in which the parameters occur.
+    paramstyle: str, optional
+        Determines the style of ``params``.
+        Possible values are:
+
+        - ``named``
+        - ``qmark``
     dtype_backend: str, optional
         Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
         nullable dtypes are used for all dtypes that have a nullable implementation when
         “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
 
         The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
     s3_additional_kwargs : Optional[Dict[str, Any]]
@@ -960,23 +988,23 @@
         )
     if ctas_approach and unload_approach:
         raise exceptions.InvalidArgumentCombination("Only one of ctas_approach=True or unload_approach=True is allowed")
     if unload_parameters and unload_parameters.get("file_format") not in (None, "PARQUET"):
         raise exceptions.InvalidArgumentCombination("Only PARQUET file format is supported if unload_approach=True")
     chunksize = sys.maxsize if ctas_approach is False and chunksize is True else chunksize
 
+    # Substitute query parameters if applicable
+    sql, execution_params = _apply_formatter(sql, params, paramstyle)
+
     athena_cache_settings = athena_cache_settings if athena_cache_settings else {}
     max_cache_seconds = athena_cache_settings.get("max_cache_seconds", 0)
     max_cache_query_inspections = athena_cache_settings.get("max_cache_query_inspections", 50)
     max_remote_cache_entries = athena_cache_settings.get("max_remote_cache_entries", 50)
     max_local_cache_entries = athena_cache_settings.get("max_local_cache_entries", 100)
 
-    # Substitute query parameters
-    sql = _process_sql_params(sql, params)
-
     max_remote_cache_entries = min(max_remote_cache_entries, max_local_cache_entries)
 
     _cache_manager.max_cache_size = max_local_cache_entries
     cache_info: _CacheInfo = _check_for_cached_results(
         sql=sql,
         boto3_session=boto3_session,
         workgroup=workgroup,
@@ -1028,14 +1056,15 @@
         ctas_bucketing_info=ctas_bucketing_info,
         ctas_write_compression=ctas_write_compression,
         athena_query_wait_polling_delay=athena_query_wait_polling_delay,
         use_threads=use_threads,
         s3_additional_kwargs=s3_additional_kwargs,
         boto3_session=boto3_session,
         pyarrow_additional_kwargs=pyarrow_additional_kwargs,
+        execution_params=execution_params,
         dtype_backend=dtype_backend,
     )
 
 
 @apply_configs
 @_utils.validate_distributed_kwargs(
     unsupported_kwargs=["boto3_session", "s3_additional_kwargs"],
@@ -1062,19 +1091,19 @@
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Extract the full table AWS Athena and return the results as a Pandas DataFrame.
 
     **Related tutorial:**
 
-    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.2.1/
+    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.3.0/
       tutorials/006%20-%20Amazon%20Athena.html>`_
-    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.2.1/
+    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.3.0/
       tutorials/019%20-%20Athena%20Cache.html>`_
-    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.2.1/
+    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.3.0/
       tutorials/021%20-%20Global%20Configurations.html>`_
 
     **There are three approaches available through ctas_approach and unload_approach parameters:**
 
     **1** - ctas_approach=True (Default):
 
     Wrap the query with a CTAS and then reads the table data as parquet directly from s3.
@@ -1130,15 +1159,15 @@
     ----
     The resulting DataFrame (or every DataFrame in the returned Iterator for chunked queries) have a
     `query_metadata` attribute, which brings the query result metadata returned by
     `Boto3/Athena <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services
     /athena.html#Athena.Client.get_query_execution>`_ .
 
     For a practical example check out the
-    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.2.1/
+    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.3.0/
     tutorials/024%20-%20Athena%20Query%20Metadata.html>`_!
 
 
     Note
     ----
     Valid encryption modes: [None, 'SSE_S3', 'SSE_KMS'].
 
@@ -1284,15 +1313,16 @@
     field_delimiter: Optional[str] = None,
     partitioned_by: Optional[List[str]] = None,
     workgroup: Optional[str] = None,
     encryption: Optional[str] = None,
     kms_key: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
     data_source: Optional[str] = None,
-    params: Optional[Dict[str, Any]] = None,
+    params: Union[Dict[str, Any], List[str], None] = None,
+    paramstyle: Literal["qmark", "named"] = "named",
     athena_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY,
 ) -> _QueryMetadata:
     """Write query results from a SELECT statement to the specified data format using UNLOAD.
 
     https://docs.aws.amazon.com/athena/latest/ug/unload.html
 
     Parameters
@@ -1321,18 +1351,33 @@
         Valid values: [None, 'SSE_S3', 'SSE_KMS']. Notice: 'CSE_KMS' is not supported.
     kms_key : str, optional
         For SSE-KMS, this is the KMS key ARN or ID.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
     data_source : str, optional
         Data Source / Catalog name. If None, 'AwsDataCatalog' will be used by default.
-    params: Dict[str, any], optional
-        Dict of parameters that will be used for constructing the SQL query. Only named parameters are supported.
-        The dict needs to contain the information in the form {'name': 'value'} and the SQL query needs to contain
-        `:name`. Note that for varchar columns and similar, you must surround the value in single quotes.
+    params: Dict[str, any] | List[str], optional
+        Parameters that will be used for constructing the SQL query.
+        Only named or question mark parameters are supported.
+        The parameter style needs to be specified in the ``paramstyle`` parameter.
+
+        For ``paramstyle="named"``, this value needs to be a dictionary.
+        The dict needs to contain the information in the form ``{'name': 'value'}`` and the SQL query needs to contain
+        ``:name``.
+        The formatter will be applied client-side in this scenario.
+
+        For ``paramstyle="qmark"``, this value needs to be a list of strings.
+        The formatter will be applied server-side.
+        The values are applied sequentially to the parameters in the query in the order in which the parameters occur.
+    paramstyle: str, optional
+        Determines the style of ``params``.
+        Possible values are:
+
+        - ``named``
+        - ``qmark``
     athena_query_wait_polling_delay: float, default: 0.25 seconds
         Interval in seconds for how often the function will check if the Athena query has completed.
 
     Returns
     -------
     _QueryMetadata
         Query metadata including query execution id, dtypes, manifest & output location.
@@ -1342,24 +1387,25 @@
     >>> import awswrangler as wr
     >>> res = wr.athena.unload(
     ...     sql="SELECT * FROM my_table WHERE name=:name AND city=:city",
     ...     params={"name": "filtered_name", "city": "filtered_city"}
     ... )
 
     """
-    # Substitute query parameters
-    sql = _process_sql_params(sql, params)
+    # Substitute query parameters if applicable
+    sql, execution_params = _apply_formatter(sql, params, paramstyle)
     return _unload(
         sql=sql,
         path=path,
         file_format=file_format,
         compression=compression,
         field_delimiter=field_delimiter,
         partitioned_by=partitioned_by,
         workgroup=workgroup,
         database=database,
         encryption=encryption,
         kms_key=kms_key,
         athena_query_wait_polling_delay=athena_query_wait_polling_delay,
         boto3_session=boto3_session,
         data_source=data_source,
+        execution_params=execution_params,
     )
```

### Comparing `awswrangler-3.2.1/awswrangler/athena/_read.pyi` & `awswrangler-3.3.0/awswrangler/athena/_read.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -69,15 +69,16 @@
     kms_key: Optional[str] = ...,
     keep_files: bool = ...,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
     data_source: Optional[str] = ...,
     athena_query_wait_polling_delay: float = ...,
-    params: Optional[Dict[str, Any]] = ...,
+    params: Union[Dict[str, Any], List[str], None] = ...,
+    paramstyle: Literal["qmark", "named"] = ...,
     dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> pd.DataFrame: ...
 @overload
 def read_sql_query(
     sql: str,
@@ -95,15 +96,16 @@
     kms_key: Optional[str] = ...,
     keep_files: bool = ...,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
     data_source: Optional[str] = ...,
     athena_query_wait_polling_delay: float = ...,
-    params: Optional[Dict[str, Any]] = ...,
+    params: Union[Dict[str, Any], List[str], None] = ...,
+    paramstyle: Literal["qmark", "named"] = ...,
     dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Iterator[pd.DataFrame]: ...
 @overload
 def read_sql_query(
     sql: str,
@@ -121,15 +123,16 @@
     kms_key: Optional[str] = ...,
     keep_files: bool = ...,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
     data_source: Optional[str] = ...,
     athena_query_wait_polling_delay: float = ...,
-    params: Optional[Dict[str, Any]] = ...,
+    params: Union[Dict[str, Any], List[str], None] = ...,
+    paramstyle: Literal["qmark", "named"] = ...,
     dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]: ...
 @overload
 def read_sql_query(
     sql: str,
@@ -147,15 +150,16 @@
     kms_key: Optional[str] = ...,
     keep_files: bool = ...,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
     data_source: Optional[str] = ...,
     athena_query_wait_polling_delay: float = ...,
-    params: Optional[Dict[str, Any]] = ...,
+    params: Union[Dict[str, Any], List[str], None] = ...,
+    paramstyle: Literal["qmark", "named"] = ...,
     dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Iterator[pd.DataFrame]: ...
 @overload
 def read_sql_query(
     sql: str,
@@ -173,15 +177,16 @@
     kms_key: Optional[str] = ...,
     keep_files: bool = ...,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
     data_source: Optional[str] = ...,
     athena_query_wait_polling_delay: float = ...,
-    params: Optional[Dict[str, Any]] = ...,
+    params: Union[Dict[str, Any], List[str], None] = ...,
+    paramstyle: Literal["qmark", "named"] = ...,
     dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]: ...
 @overload
 def read_sql_table(
     table: str,
@@ -311,10 +316,11 @@
     field_delimiter: Optional[str] = ...,
     partitioned_by: Optional[List[str]] = ...,
     workgroup: Optional[str] = ...,
     encryption: Optional[str] = ...,
     kms_key: Optional[str] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     data_source: Optional[str] = ...,
-    params: Optional[Dict[str, Any]] = ...,
+    params: Union[Dict[str, Any], List[str], None] = ...,
+    paramstyle: Literal["qmark", "named"] = ...,
     athena_query_wait_polling_delay: float = ...,
 ) -> _QueryMetadata: ...
```

### Comparing `awswrangler-3.2.1/awswrangler/athena/_spark.py` & `awswrangler-3.3.0/awswrangler/athena/_spark.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/athena/_utils.py` & `awswrangler-3.3.0/awswrangler/athena/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,27 @@
     Dict,
     Generator,
     List,
     NamedTuple,
     Optional,
     Sequence,
     Tuple,
+    TypedDict,
     Union,
     cast,
 )
 
 import boto3
 import botocore.exceptions
 import pandas as pd
 from typing_extensions import Literal
 
 from awswrangler import _data_types, _utils, catalog, exceptions, s3, sts, typing
 from awswrangler._config import apply_configs
+from awswrangler._sql_formatter import _process_sql_params
 from awswrangler.catalog._utils import _catalog_id, _transaction_id
 
 from . import _executions
 from ._cache import _cache_manager, _LocalMetadataCacheManager
 
 if TYPE_CHECKING:
     from mypy_boto3_glue.type_defs import ColumnTypeDef
@@ -78,14 +80,15 @@
     wg_config: _WorkGroupConfig,
     database: Optional[str] = None,
     data_source: Optional[str] = None,
     s3_output: Optional[str] = None,
     workgroup: Optional[str] = None,
     encryption: Optional[str] = None,
     kms_key: Optional[str] = None,
+    execution_params: Optional[List[str]] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> str:
     args: Dict[str, Any] = {"QueryString": sql}
 
     # s3_output
     args["ResultConfiguration"] = {
         "OutputLocation": _get_s3_output(s3_output=s3_output, wg_config=wg_config, boto3_session=boto3_session)
@@ -108,14 +111,17 @@
         if data_source is not None:
             args["QueryExecutionContext"]["Catalog"] = data_source
 
     # workgroup
     if workgroup is not None:
         args["WorkGroup"] = workgroup
 
+    if execution_params:
+        args["ExecutionParameters"] = execution_params
+
     client_athena = _utils.client(service_name="athena", session=boto3_session)
     _logger.debug("Starting query execution with args: \n%s", pprint.pformat(args))
     response = _utils.try_it(
         f=client_athena.start_query_execution,
         ex=botocore.exceptions.ClientError,
         ex_code="ThrottlingException",
         max_num_tries=5,
@@ -203,14 +209,15 @@
 def _get_query_metadata(  # pylint: disable=too-many-statements
     query_execution_id: str,
     boto3_session: Optional[boto3.Session] = None,
     categories: Optional[List[str]] = None,
     query_execution_payload: Optional[Dict[str, Any]] = None,
     metadata_cache_manager: Optional[_LocalMetadataCacheManager] = None,
     athena_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY,
+    execution_params: Optional[List[str]] = None,
     dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> _QueryMetadata:
     """Get query metadata."""
     if (query_execution_payload is not None) and (query_execution_payload["Status"]["State"] in _QUERY_FINAL_STATES):
         if query_execution_payload["Status"]["State"] != "SUCCEEDED":
             reason: str = query_execution_payload["Status"]["StateChangeReason"]
             raise exceptions.QueryFailed(f"Query error: {reason}")
@@ -286,14 +293,78 @@
 def _apply_query_metadata(df: pd.DataFrame, query_metadata: _QueryMetadata) -> pd.DataFrame:
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", category=UserWarning)
         df.query_metadata = query_metadata.raw_payload
     return df
 
 
+class _FormatterTypeQMark(TypedDict):
+    params: List[str]
+    paramstyle: Literal["qmark"]
+
+
+class _FormatterTypeNamed(TypedDict):
+    params: Dict[str, Any]
+    paramstyle: Literal["named"]
+
+
+_FormatterType = Union[_FormatterTypeQMark, _FormatterTypeNamed, None]
+
+
+def _verify_formatter(
+    params: Union[Dict[str, Any], List[str], None],
+    paramstyle: Literal["qmark", "named"],
+) -> _FormatterType:
+    if params is None:
+        return None
+
+    if paramstyle == "named":
+        if not isinstance(params, dict):
+            raise exceptions.InvalidArgumentCombination(
+                f"`params` must be a dict when paramstyle is `named`. Instead, found type {type(params)}."
+            )
+
+        return {
+            "paramstyle": "named",
+            "params": params,
+        }
+
+    if paramstyle == "qmark":
+        if not isinstance(params, list):
+            raise exceptions.InvalidArgumentCombination(
+                f"`params` must be a list when paramstyle is `qmark`. Instead, found type {type(params)}."
+            )
+
+        return {
+            "paramstyle": "qmark",
+            "params": params,
+        }
+
+    raise exceptions.InvalidArgumentValue(f"`paramstyle` must be either `qmark` or `named`. Found: {paramstyle}.")
+
+
+def _apply_formatter(
+    sql: str,
+    params: Union[Dict[str, Any], List[str], None],
+    paramstyle: Literal["qmark", "named"],
+) -> Tuple[str, Optional[List[str]]]:
+    formatter_settings = _verify_formatter(params, paramstyle)
+
+    if formatter_settings is None:
+        return sql, None
+
+    if formatter_settings["paramstyle"] == "named":
+        # Substitute query parameters]
+        sql = _process_sql_params(sql, formatter_settings["params"])
+
+        return sql, None
+
+    return sql, formatter_settings["params"]
+
+
 def get_named_query_statement(
     named_query_id: str,
     boto3_session: Optional[boto3.Session] = None,
 ) -> str:
     """
     Get the named query statement string from a query ID.
 
@@ -564,14 +635,15 @@
     workgroup: Optional[str] = None,
     data_source: Optional[str] = None,
     encryption: Optional[str] = None,
     kms_key: Optional[str] = None,
     categories: Optional[List[str]] = None,
     wait: bool = False,
     athena_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY,
+    execution_params: Optional[List[str]] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> Dict[str, Union[str, _QueryMetadata]]:
     """Create a new table populated with the results of a SELECT query.
 
     https://docs.aws.amazon.com/athena/latest/ug/create-table-as.html
 
     Parameters
@@ -717,14 +789,15 @@
             database=database,
             data_source=data_source,
             s3_output=s3_output,
             workgroup=workgroup,
             encryption=encryption,
             kms_key=kms_key,
             boto3_session=boto3_session,
+            execution_params=execution_params,
         )
     except botocore.exceptions.ClientError as ex:
         error = ex.response["Error"]
         if error["Code"] == "InvalidRequestException" and "Exception parsing query" in error["Message"]:
             raise exceptions.InvalidCtasApproachQuery(
                 f"It is not possible to wrap this query into a CTAS statement. Root error message: {error['Message']}"
             )
```

### Comparing `awswrangler-3.2.1/awswrangler/athena/_write_iceberg.py` & `awswrangler-3.3.0/awswrangler/athena/_write_iceberg.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,19 +29,20 @@
     additional_table_properties: Optional[Dict[str, Any]],
     index: bool = False,
     data_source: Optional[str] = None,
     workgroup: Optional[str] = None,
     encryption: Optional[str] = None,
     kms_key: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
+    dtype: Optional[Dict[str, str]] = None,
 ) -> None:
     if not path:
         raise exceptions.InvalidArgumentValue("Must specify table location to create the table.")
 
-    columns_types, _ = catalog.extract_athena_types(df=df, index=index)
+    columns_types, _ = catalog.extract_athena_types(df=df, index=index, dtype=dtype)
     cols_str: str = ", ".join([f"{k} {v}" for k, v in columns_types.items()])
     partition_cols_str: str = f"PARTITIONED BY ({', '.join([col for col in partition_cols])})" if partition_cols else ""
     table_properties_str: str = (
         ", " + ", ".join([f"'{key}'='{value}'" for key, value in additional_table_properties.items()])
         if additional_table_properties
         else ""
     )
@@ -82,14 +83,15 @@
     data_source: Optional[str] = None,
     workgroup: Optional[str] = None,
     encryption: Optional[str] = None,
     kms_key: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     additional_table_properties: Optional[Dict[str, Any]] = None,
+    dtype: Optional[Dict[str, str]] = None,
 ) -> None:
     """
     Insert into Athena Iceberg table using INSERT INTO ... SELECT. Will create Iceberg table if it does not exist.
 
     Creates temporary external table, writes staged files and inserts via INSERT INTO ... SELECT.
 
     Parameters
@@ -129,14 +131,18 @@
         Forwarded to botocore requests.
         e.g. s3_additional_kwargs={'RequestPayer': 'requester'}
     additional_table_properties : Optional[Dict[str, Any]]
         Additional table properties.
         e.g. additional_table_properties={'write_target_data_file_size_bytes': '536870912'}
 
         https://docs.aws.amazon.com/athena/latest/ug/querying-iceberg-creating-tables.html#querying-iceberg-table-properties
+    dtype: Optional[Dict[str, str]]
+        Dictionary of columns names and Athena/Glue types to be casted.
+        Useful when you have columns with undetermined or mixed data types.
+        e.g. {'col name': 'bigint', 'col2 name': 'int'}
 
     Returns
     -------
     None
 
     Examples
     --------
@@ -188,25 +194,27 @@
                 additional_table_properties=additional_table_properties,
                 index=index,
                 data_source=data_source,
                 workgroup=workgroup,
                 encryption=encryption,
                 kms_key=kms_key,
                 boto3_session=boto3_session,
+                dtype=dtype,
             )
 
         # Create temporary external table, write the results
         s3.to_parquet(
             df=df,
             path=temp_path or wg_config.s3_output,
             dataset=True,
             database=database,
             table=temp_table,
             boto3_session=boto3_session,
             s3_additional_kwargs=s3_additional_kwargs,
+            dtype=dtype,
         )
 
         # Insert into iceberg table
         query_id: str = _start_query_execution(
             sql=f'INSERT INTO "{database}"."{table}" SELECT * FROM "{database}"."{temp_table}"',
             workgroup=workgroup,
             wg_config=wg_config,
```

### Comparing `awswrangler-3.2.1/awswrangler/catalog/__init__.py` & `awswrangler-3.3.0/awswrangler/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/catalog/_add.py` & `awswrangler-3.3.0/awswrangler/catalog/_add.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/catalog/_create.py` & `awswrangler-3.3.0/awswrangler/catalog/_create.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/catalog/_definitions.py` & `awswrangler-3.3.0/awswrangler/catalog/_definitions.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/catalog/_delete.py` & `awswrangler-3.3.0/awswrangler/catalog/_delete.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/catalog/_get.py` & `awswrangler-3.3.0/awswrangler/catalog/_get.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/catalog/_utils.py` & `awswrangler-3.3.0/awswrangler/catalog/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/chime.py` & `awswrangler-3.3.0/awswrangler/chime.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/cloudwatch.py` & `awswrangler-3.3.0/awswrangler/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/data_api/_connector.py` & `awswrangler-3.3.0/awswrangler/data_api/_connector.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/data_api/rds.py` & `awswrangler-3.3.0/awswrangler/data_api/rds.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """RDS Data API Connector."""
 import datetime as dt
 import logging
+import re
 import time
 import uuid
 from decimal import Decimal
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, TypeVar, Union, cast
 
 import boto3
 from typing_extensions import Literal
@@ -223,14 +224,27 @@
             rows.append(row)
 
         column_names: List[str] = [column["name"] for column in result["columnMetadata"]]
         dataframe = pd.DataFrame(rows, columns=column_names)
         return dataframe
 
 
+def escape_identifier(identifier: str, sql_mode: str = "mysql") -> str:
+    """Escape identifiers. Uses MySQL-compatible backticks by default."""
+    if not isinstance(identifier, str):
+        raise TypeError("SQL identifier must be a string")
+    if re.search(r"\W", identifier):
+        raise TypeError(f"SQL identifier contains invalid characters: {identifier}")
+    if sql_mode == "mysql":
+        return f"`{identifier}`"
+    elif sql_mode == "ansi":
+        return f'"{identifier}"'
+    raise ValueError(f"Unknown SQL MODE: {sql_mode}")
+
+
 def connect(
     resource_arn: str, database: str, secret_arn: str = "", boto3_session: Optional[boto3.Session] = None, **kwargs: Any
 ) -> RdsDataApi:
     """Create a RDS Data API connection.
 
     Parameters
     ----------
@@ -267,16 +281,16 @@
     Returns
     -------
     A Pandas DataFrame containing the query results.
     """
     return con.execute(sql, database=database)
 
 
-def _drop_table(con: RdsDataApi, table: str, database: str, transaction_id: str) -> None:
-    sql = f"DROP TABLE IF EXISTS `{table}`"
+def _drop_table(con: RdsDataApi, table: str, database: str, transaction_id: str, sql_mode: str) -> None:
+    sql = f"DROP TABLE IF EXISTS {escape_identifier(table, sql_mode=sql_mode)}"
     _logger.debug("Drop table query:\n%s", sql)
     con.execute(sql, database=database, transaction_id=transaction_id)
 
 
 def _does_table_exist(con: RdsDataApi, table: str, database: str, transaction_id: str) -> bool:
     res = con.execute(f"SELECT * FROM INFORMATION_SCHEMA.TABLES WHERE TABLE_NAME = '{table}'")
     return not res.empty
@@ -288,30 +302,31 @@
     table: str,
     database: str,
     transaction_id: str,
     mode: str,
     index: bool,
     dtype: Optional[Dict[str, str]],
     varchar_lengths: Optional[Dict[str, int]],
+    sql_mode: str,
 ) -> None:
     if mode == "overwrite":
-        _drop_table(con=con, table=table, database=database, transaction_id=transaction_id)
+        _drop_table(con=con, table=table, database=database, transaction_id=transaction_id, sql_mode=sql_mode)
     elif _does_table_exist(con=con, table=table, database=database, transaction_id=transaction_id):
         return
 
     mysql_types: Dict[str, str] = _data_types.database_types_from_pandas(
         df=df,
         index=index,
         dtype=dtype,
         varchar_lengths_default="TEXT",
         varchar_lengths=varchar_lengths,
         converter_func=_data_types.pyarrow2mysql,
     )
-    cols_str: str = "".join([f"`{k}` {v},\n" for k, v in mysql_types.items()])[:-2]
-    sql = f"CREATE TABLE IF NOT EXISTS `{table}` (\n{cols_str})"
+    cols_str: str = "".join([f"{escape_identifier(k, sql_mode=sql_mode)} {v},\n" for k, v in mysql_types.items()])[:-2]
+    sql = f"CREATE TABLE IF NOT EXISTS {escape_identifier(table, sql_mode=sql_mode)} (\n{cols_str})"
 
     _logger.debug("Create table query:\n%s", sql)
     con.execute(sql, database=database, transaction_id=transaction_id)
 
 
 def _create_value_dict(  # pylint: disable=too-many-return-statements
     value: Any,
@@ -384,14 +399,15 @@
     database: str,
     mode: Literal["append", "overwrite"] = "append",
     index: bool = False,
     dtype: Optional[Dict[str, str]] = None,
     varchar_lengths: Optional[Dict[str, int]] = None,
     use_column_names: bool = False,
     chunksize: int = 200,
+    sql_mode: str = "mysql",
 ) -> None:
     """
     Insert data using an SQL query on a Data API connection.
 
     Parameters
     ----------
     df: pandas.DataFrame
@@ -435,27 +451,30 @@
             table=table,
             database=database,
             transaction_id=transaction_id,
             mode=mode,
             index=index,
             dtype=dtype,
             varchar_lengths=varchar_lengths,
+            sql_mode=sql_mode,
         )
 
         if index:
             df = df.reset_index(level=df.index.names)
 
         if use_column_names:
-            insertion_columns = "(" + ", ".join([f"`{col}`" for col in df.columns]) + ")"
+            insertion_columns = (
+                "(" + ", ".join([f"{escape_identifier(col, sql_mode=sql_mode)}" for col in df.columns]) + ")"
+            )
         else:
             insertion_columns = ""
 
         placeholders = ", ".join([f":{col}" for col in df.columns])
 
-        sql = f"""INSERT INTO `{table}` {insertion_columns} VALUES ({placeholders})"""
+        sql = f"INSERT INTO {escape_identifier(table, sql_mode=sql_mode)} {insertion_columns} VALUES ({placeholders})"
         parameter_sets = _generate_parameter_sets(df)
 
         for parameter_sets_chunk in _utils.chunkify(parameter_sets, max_length=chunksize):
             con.batch_execute(
                 sql=sql,
                 database=database,
                 transaction_id=transaction_id,
```

### Comparing `awswrangler-3.2.1/awswrangler/data_api/redshift.py` & `awswrangler-3.3.0/awswrangler/data_api/redshift.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/data_quality/_create.py` & `awswrangler-3.3.0/awswrangler/data_quality/_create.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/data_quality/_get.py` & `awswrangler-3.3.0/awswrangler/data_quality/_get.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/data_quality/_utils.py` & `awswrangler-3.3.0/awswrangler/data_quality/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/_core.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/_core.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/_core.pyi` & `awswrangler-3.3.0/awswrangler/distributed/ray/_core.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/_executor.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def map(self, func: Callable[..., MapOutputType], _: Optional["BaseClient"], *args: Any) -> List[MapOutputType]:
         """Map func and return ray futures."""
         _logger.debug("Ray map: %s", func)
         # Discard boto3 client
         return list(func(*arg) for arg in zip(itertools.repeat(None), *args))
 
 
-@ray.remote  # type: ignore[attr-defined]
+@ray.remote
 class AsyncActor:
     async def run_concurrent(self, func: Callable[..., MapOutputType], *args: Any) -> MapOutputType:
         return func(*args)
 
 
 class _RayMaxConcurrencyExecutor(_BaseExecutor):
     def __init__(self, max_concurrency: int) -> None:
```

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/_register.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/_register.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/_utils.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     If we aren't in a placement group, this is trivially the number of CPUs in the
     cluster. Otherwise, we try to calculate how large the placement group is relative
     to the size of the cluster.
 
     Args:
         cur_pg: The current placement group, if any.
     """
-    cluster_cpus = int(ray.cluster_resources().get("CPU", 1))  # type: ignore[attr-defined]
-    cluster_gpus = int(ray.cluster_resources().get("GPU", 0))  # type: ignore[attr-defined]
+    cluster_cpus = int(ray.cluster_resources().get("CPU", 1))
+    cluster_gpus = int(ray.cluster_resources().get("GPU", 0))
 
     # If we're in a placement group, we shouldn't assume the entire cluster's
     # resources are available for us to use. Estimate an upper bound on what's
     # reasonable to assume is available for datasets to use.
     if cur_pg:
         pg_cpus = 0
         for bundle in cur_pg.bundle_specs:
```

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/datasources/__init__.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/datasources/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/datasources/arrow_json_datasource.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/datasources/arrow_json_datasource.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/datasources/arrow_orc_datasource.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/datasources/arrow_orc_datasource.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/datasources/arrow_parquet_base_datasource.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/datasources/arrow_parquet_base_datasource.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
             paths = paths[0]
 
         self._local_scheduling = None
         if local_uri:
             import ray
             from ray.util.scheduling_strategies import NodeAffinitySchedulingStrategy
 
-            self._local_scheduling = NodeAffinitySchedulingStrategy(ray.get_runtime_context().get_node_id(), soft=False)  # type: ignore[attr-defined]
+            self._local_scheduling = NodeAffinitySchedulingStrategy(ray.get_runtime_context().get_node_id(), soft=False)
 
         dataset_kwargs = reader_args.pop("dataset_kwargs", {})
         try:
             pq_ds = pq.ParquetDataset(paths, **dataset_kwargs, filesystem=filesystem, use_legacy_dataset=False)
         except OSError as e:
             _handle_read_os_error(e, paths)
         if schema is None:
@@ -221,15 +221,15 @@
         if columns:
             schema = pa.schema([schema.field(column) for column in columns], schema.metadata)
 
         if _block_udf is not None:
             # Try to infer dataset schema by passing dummy table through UDF.
             dummy_table = schema.empty_table()
             try:
-                inferred_schema = _block_udf(dummy_table).schema  # type: ignore[union-attr]
+                inferred_schema = _block_udf(dummy_table).schema
                 inferred_schema = inferred_schema.with_metadata(schema.metadata)
             except Exception:  # pylint: disable=broad-except
                 _logger.debug(
                     "Failed to infer schema of dataset by passing dummy table "
                     "through UDF due to the following exception:",
                     exc_info=True,
                 )
```

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/datasources/pandas_text_datasource.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/datasources/pandas_text_datasource.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/modin/_core.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/modin/_core.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/modin/_data_types.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/modin/_data_types.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/modin/_utils.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/modin/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,16 @@
     @ray_remote()
     def _is_not_empty(table: pa.Table) -> Any:
         return table.num_rows > 0 or table.num_columns > 0
 
     ref_rows: List[bool] = ray_get([_is_not_empty(arrow_ref) for arrow_ref in arrow_refs])
     refs: List[Callable[..., Any]] = [ref for ref_rows, ref in zip(ref_rows, arrow_refs) if ref_rows]
     return _to_modin(
-        dataset=ray.data.from_arrow_refs(refs if len(refs) > 0 else [pa.Table.from_arrays([])]), to_pandas_kwargs=kwargs
+        dataset=ray.data.from_arrow_refs(refs) if len(refs) > 0 else ray.data.from_arrow([pa.Table.from_arrays([])]),
+        to_pandas_kwargs=kwargs,
     )
 
 
 def _is_pandas_or_modin_frame(obj: Any) -> bool:
     return isinstance(obj, (pd.DataFrame, modin_pd.DataFrame))
```

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_read_orc.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/modin/s3/_read_orc.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_read_parquet.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/modin/s3/_read_parquet.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_read_text.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/modin/s3/_read_text.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_write_dataset.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/modin/s3/_write_dataset.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_write_orc.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/modin/s3/_write_orc.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_write_parquet.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/modin/s3/_write_parquet.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_write_text.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/modin/s3/_write_text.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/s3/_list.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/s3/_list.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/s3/_read_orc.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/s3/_read_orc.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/distributed/ray/s3/_read_parquet.py` & `awswrangler-3.3.0/awswrangler/distributed/ray/s3/_read_parquet.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/dynamodb/_delete.py` & `awswrangler-3.3.0/awswrangler/dynamodb/_delete.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/dynamodb/_read.py` & `awswrangler-3.3.0/awswrangler/dynamodb/_read.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Amazon DynamoDB Read Module (PRIVATE)."""
 
 import itertools
 import logging
+import warnings
 from functools import wraps
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterator,
@@ -160,15 +161,16 @@
         _utils.table_refs_to_df(
             [
                 _utils.list_to_arrow_table(
                     # Convert DynamoDB "Binary" type to native Python data type
                     mapping=[
                         {k: v.value if isinstance(v, Binary) else v for k, v in d.items()}  # type: ignore[attr-defined]
                         for d in items
-                    ]
+                    ],
+                    schema=arrow_kwargs.pop("schema", None),
                 )
             ],
             arrow_kwargs,
         )
         if as_dataframe
         else items
     )
@@ -183,36 +185,42 @@
         yield _convert_items(items, as_dataframe, arrow_kwargs)
 
 
 def _read_scan_chunked(
     dynamodb_client: Optional["DynamoDBClient"],
     as_dataframe: bool,
     kwargs: Dict[str, Any],
+    schema: Optional[pa.Schema] = None,
     segment: Optional[int] = None,
 ) -> Union[Iterator[pa.Table], Iterator[_ItemsListType]]:
     # SEE: https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Scan.html#Scan.ParallelScan
     client_dynamodb = dynamodb_client if dynamodb_client else _utils.client(service_name="dynamodb")
 
     deserializer = boto3.dynamodb.types.TypeDeserializer()
     next_token = "init_token"  # Dummy token
+    total_items = 0
 
     kwargs = dict(kwargs)
     if segment is not None:
         kwargs["Segment"] = segment
 
     while next_token:
         response = _handle_reserved_keyword_error(client_dynamodb.scan)(**kwargs)
         # Unlike a resource, the DynamoDB client returns serialized results, so they must be deserialized
         # Additionally, the DynamoDB "Binary" type is converted to a native Python data type
         # SEE: https://boto3.amazonaws.com/v1/documentation/api/latest/_modules/boto3/dynamodb/types.html
         items = [
             {k: v["B"] if list(v.keys())[0] == "B" else deserializer.deserialize(v) for k, v in d.items()}
             for d in response.get("Items", [])
         ]
-        yield _utils.list_to_arrow_table(mapping=items) if as_dataframe else items
+        total_items += len(items)
+        yield _utils.list_to_arrow_table(mapping=items, schema=schema) if as_dataframe else items
+
+        if ("Limit" in kwargs) and (total_items >= kwargs["Limit"]):
+            break
 
         next_token = response.get("LastEvaluatedKey", None)  # type: ignore[assignment]
         if next_token:
             kwargs["ExclusiveStartKey"] = next_token
 
 
 @engine.dispatch_on_engine
@@ -220,35 +228,44 @@
     ex=ClientError,
     ex_code="ProvisionedThroughputExceededException",
 )
 def _read_scan(
     dynamodb_client: Optional["DynamoDBClient"],
     as_dataframe: bool,
     kwargs: Dict[str, Any],
+    schema: Optional[pa.Schema],
     segment: int,
 ) -> Union[pa.Table, _ItemsListType]:
-    items_iterator: Iterator[_ItemsListType] = _read_scan_chunked(dynamodb_client, False, kwargs, segment)
+    items_iterator: Iterator[_ItemsListType] = _read_scan_chunked(dynamodb_client, False, kwargs, None, segment)
 
     items = list(itertools.chain.from_iterable(items_iterator))
 
-    return _utils.list_to_arrow_table(mapping=items) if as_dataframe else items
+    return _utils.list_to_arrow_table(mapping=items, schema=schema) if as_dataframe else items
 
 
 def _read_query_chunked(
     table_name: str, boto3_session: Optional[boto3.Session] = None, **kwargs: Any
 ) -> Iterator[_ItemsListType]:
     table = get_table(table_name=table_name, boto3_session=boto3_session)
-    response = table.query(**kwargs)
-    yield response.get("Items", [])
+    next_token = "init_token"  # Dummy token
+    total_items = 0
 
     # Handle pagination
-    while "LastEvaluatedKey" in response:
-        kwargs["ExclusiveStartKey"] = response["LastEvaluatedKey"]
+    while next_token:
         response = table.query(**kwargs)
-        yield response.get("Items", [])
+        items = response.get("Items", [])
+        total_items += len(items)
+        yield items
+
+        if ("Limit" in kwargs) and (total_items >= kwargs["Limit"]):
+            break
+
+        next_token = response.get("LastEvaluatedKey", None)  # type: ignore[assignment]
+        if next_token:
+            kwargs["ExclusiveStartKey"] = next_token
 
 
 @_handle_reserved_keyword_error
 def _read_query(
     table_name: str, chunked: bool, boto3_session: Optional[boto3.Session] = None, **kwargs: Any
 ) -> Union[_ItemsListType, Iterator[_ItemsListType]]:
     items_iterator = _read_query_chunked(table_name, boto3_session, **kwargs)
@@ -309,18 +326,19 @@
     boto3_session: Optional[boto3.Session] = None,
     **kwargs: Any,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame], _ItemsListType, Iterator[_ItemsListType]]:
     dynamodb_client = _utils.client(service_name="dynamodb", session=boto3_session)
 
     kwargs = _serialize_kwargs(kwargs)
     kwargs["TableName"] = table_name
+    schema = arrow_kwargs.pop("schema", None)
 
     if chunked:
         _logger.debug("Scanning DynamoDB table %s and returning results in an iterator", table_name)
-        scan_iterator = _read_scan_chunked(dynamodb_client, as_dataframe, kwargs)
+        scan_iterator = _read_scan_chunked(dynamodb_client, as_dataframe, kwargs, schema)
         if as_dataframe:
             return (_utils.table_refs_to_df([items], arrow_kwargs) for items in scan_iterator)
 
         return scan_iterator
 
     # Use Parallel Scan
     executor: _BaseExecutor = _get_executor(use_threads=use_threads)
@@ -330,14 +348,15 @@
     _logger.debug("Scanning DynamoDB table %s with %d segments", table_name, total_segments)
 
     items = executor.map(
         _read_scan,
         dynamodb_client,
         itertools.repeat(as_dataframe),
         itertools.repeat(kwargs),
+        itertools.repeat(schema),
         range(total_segments),
     )
 
     if as_dataframe:
         return _utils.table_refs_to_df(items, arrow_kwargs)
 
     return list(itertools.chain(*ray_get(items)))
@@ -348,17 +367,18 @@
     as_dataframe: bool,
     arrow_kwargs: Dict[str, Any],
     use_threads: Union[bool, int],
     chunked: bool,
     boto3_session: Optional[boto3.Session] = None,
     **kwargs: Any,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame], _ItemsListType, Iterator[_ItemsListType]]:
-    # Extract 'Keys' and 'IndexName' from provided kwargs: if needed, will be reinserted later on
+    # Extract 'Keys', 'IndexName' and 'Limit' from provided kwargs: if needed, will be reinserted later on
     keys = kwargs.pop("Keys", None)
     index = kwargs.pop("IndexName", None)
+    limit = kwargs.pop("Limit", None)
 
     # Conditionally define optimal reading strategy
     use_get_item = (keys is not None) and (len(keys) == 1)
     use_batch_get_item = (keys is not None) and (len(keys) > 1)
     use_query = (keys is None) and ("KeyConditionExpression" in kwargs)
 
     # Single Item
@@ -368,23 +388,32 @@
 
     # Batch of Items
     elif use_batch_get_item:
         kwargs["Keys"] = keys
         items = _read_batch_items(table_name, chunked, boto3_session, **kwargs)
 
     else:
+        if limit:
+            kwargs["Limit"] = limit
+            _logger.debug("`max_items_evaluated` argument detected, setting use_threads to False")
+            use_threads = False
+
         if index:
             kwargs["IndexName"] = index
 
         if use_query:
             # Query
             _logger.debug("Query DynamoDB table %s", table_name)
             items = _read_query(table_name, chunked, boto3_session, **kwargs)
         else:
             # Last resort use Scan
+            warnings.warn(
+                f"Attempting DynamoDB Scan operation with arguments:\n{kwargs}",
+                UserWarning,
+            )
             return _read_items_scan(
                 table_name=table_name,
                 as_dataframe=as_dataframe,
                 arrow_kwargs=arrow_kwargs,
                 use_threads=use_threads,
                 chunked=chunked,
                 boto3_session=boto3_session,
@@ -427,21 +456,31 @@
     This function aims to gracefully handle (some of) the complexity of read actions
     available in Boto3 towards a DynamoDB table, abstracting it away while providing
     a single, unified entry point.
 
     Under the hood, it wraps all the four available read actions: `get_item`, `batch_get_item`,
     `query` and `scan`.
 
+    Warning
+    -------
+    To avoid a potentially costly Scan operation, please make sure to pass arguments such as
+    `partition_values` or `max_items_evaluated`. Note that `filter_expression` is applied AFTER a Scan
+
     Note
     ----
     Number of Parallel Scan segments is based on the `use_threads` argument.
     A parallel scan with a large number of workers could consume all the provisioned throughput
     of the table or index.
     See: https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Scan.html#Scan.ParallelScan
 
+    Note
+    ----
+    If `max_items_evaluated` is specified, then `use_threads=False` is enforced. This is because
+    it's not possible to limit the number of items in a Query/Scan operation across threads.
+
     Parameters
     ----------
     table_name : str
         DynamoDB table name.
     index_name : str, optional
         Name of the secondary global or local index on the table. Defaults to None.
     partition_values : Sequence[Any], optional
@@ -462,14 +501,15 @@
         Defaults to False.
     columns : Sequence[str], optional
         Attributes to retain in the returned items. Defaults to None (all attributes).
     allow_full_scan : bool
         If True, allow full table scan without any filtering. Defaults to False.
     max_items_evaluated : int, optional
         Limit the number of items evaluated in case of query or scan operations. Defaults to None (all matching items).
+        When set, `use_threads` is enforced to False.
     dtype_backend: str, optional
         Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
         nullable dtypes are used for all dtypes that have a nullable implementation when
         “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
 
         The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
     as_dataframe : bool
@@ -552,14 +592,15 @@
     >>> df = wr.dynamodb.read_items(
     ...     table_name='my-table',
     ...     key_condition_expression='key_1 = :v1 and key_2 = :v2',
     ...     expression_attribute_values={':v1': 'val_1', ':v2': 'val_2'},
     ... )
 
     Reading items matching a FilterExpression expressed with boto3.dynamodb.conditions.Attr
+    Note that FilterExpression is applied AFTER a Scan operation
 
     >>> import awswrangler as wr
     >>> from boto3.dynamodb.conditions import Attr
     >>> df = wr.dynamodb.read_items(
     ...     table_name='my-table',
     ...     filter_expression=Attr('my_attr').eq('this-value')
     ... )
```

### Comparing `awswrangler-3.2.1/awswrangler/dynamodb/_read.pyi` & `awswrangler-3.3.0/awswrangler/dynamodb/_read.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/dynamodb/_utils.py` & `awswrangler-3.3.0/awswrangler/dynamodb/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/dynamodb/_write.py` & `awswrangler-3.3.0/awswrangler/dynamodb/_write.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/emr.py` & `awswrangler-3.3.0/awswrangler/emr.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/emr_serverless.py` & `awswrangler-3.3.0/awswrangler/emr_serverless.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/exceptions.py` & `awswrangler-3.3.0/awswrangler/exceptions.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/lakeformation/__init__.py` & `awswrangler-3.3.0/awswrangler/lakeformation/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/lakeformation/_read.py` & `awswrangler-3.3.0/awswrangler/lakeformation/_read.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/lakeformation/_utils.py` & `awswrangler-3.3.0/awswrangler/lakeformation/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/mysql.py` & `awswrangler-3.3.0/awswrangler/mysql.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/neptune/__init__.py` & `awswrangler-3.3.0/awswrangler/neptune/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/neptune/_client.py` & `awswrangler-3.3.0/awswrangler/neptune/_client.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/neptune/_gremlin_init.py` & `awswrangler-3.3.0/awswrangler/neptune/_gremlin_init.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/neptune/_gremlin_parser.py` & `awswrangler-3.3.0/awswrangler/neptune/_gremlin_parser.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/neptune/_neptune.py` & `awswrangler-3.3.0/awswrangler/neptune/_neptune.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/neptune/_utils.py` & `awswrangler-3.3.0/awswrangler/neptune/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/opensearch/_read.py` & `awswrangler-3.3.0/awswrangler/opensearch/_read.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/opensearch/_utils.py` & `awswrangler-3.3.0/awswrangler/opensearch/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/opensearch/_write.py` & `awswrangler-3.3.0/awswrangler/opensearch/_write.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/oracle.py` & `awswrangler-3.3.0/awswrangler/oracle.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/pandas/__init__.py` & `awswrangler-3.3.0/awswrangler/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/postgresql.py` & `awswrangler-3.3.0/awswrangler/postgresql.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,40 +11,41 @@
 
 import awswrangler.pandas as pd
 from awswrangler import _data_types, _utils, exceptions
 from awswrangler import _databases as _db_utils
 from awswrangler._config import apply_configs
 
 pg8000 = _utils.import_optional_dependency("pg8000")
+pg8000_native = _utils.import_optional_dependency("pg8000.native")
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 def _validate_connection(con: "pg8000.Connection") -> None:
     if not isinstance(con, pg8000.Connection):
         raise exceptions.InvalidConnection(
             "Invalid 'conn' argument, please pass a "
             "pg8000.Connection object. Use pg8000.connect() to use "
             "credentials directly or wr.postgresql.connect() to fetch it from the Glue Catalog."
         )
 
 
 def _drop_table(cursor: "pg8000.Cursor", schema: Optional[str], table: str) -> None:
-    schema_str = f'"{schema}".' if schema else ""
-    sql = f'DROP TABLE IF EXISTS {schema_str}"{table}"'
+    schema_str = f"{pg8000_native.identifier(schema)}." if schema else ""
+    sql = f"DROP TABLE IF EXISTS {schema_str}{pg8000_native.identifier(table)}"
     _logger.debug("Drop table query:\n%s", sql)
     cursor.execute(sql)
 
 
 def _does_table_exist(cursor: "pg8000.Cursor", schema: Optional[str], table: str) -> bool:
-    schema_str = f"TABLE_SCHEMA = '{schema}' AND" if schema else ""
+    schema_str = f"TABLE_SCHEMA = {pg8000_native.literal(schema)} AND" if schema else ""
     cursor.execute(
         f"SELECT true WHERE EXISTS ("
         f"SELECT * FROM INFORMATION_SCHEMA.TABLES WHERE "
-        f"{schema_str} TABLE_NAME = '{table}'"
+        f"{schema_str} TABLE_NAME = {pg8000_native.literal(table)}"
         f");"
     )
     return len(cursor.fetchall()) > 0
 
 
 def _create_table(
     df: pd.DataFrame,
@@ -65,15 +66,15 @@
         index=index,
         dtype=dtype,
         varchar_lengths_default="TEXT",
         varchar_lengths=varchar_lengths,
         converter_func=_data_types.pyarrow2postgresql,
     )
     cols_str: str = "".join([f'"{k}" {v},\n' for k, v in postgresql_types.items()])[:-2]
-    sql = f'CREATE TABLE IF NOT EXISTS "{schema}"."{table}" (\n{cols_str})'
+    sql = f"CREATE TABLE IF NOT EXISTS {pg8000_native.identifier(schema)}.{pg8000_native.identifier(table)} (\n{cols_str})"
     _logger.debug("Create table query:\n%s", sql)
     cursor.execute(sql)
 
 
 def _iterate_server_side_cursor(
     sql: str,
     con: Any,
@@ -90,20 +91,24 @@
 
     Note: Pg8000 is not fully DB API 2.0 - compliant with fetchmany() fetching all result set. Using server-side cursor
     allows fetching only specific amount of results reducing memory impact. Ultimately we'd like pg8000 to add full
     support for fetchmany() or add SSCursor implementation similar to MySQL and revise this implementation in the future.
     """
     with con.cursor() as cursor:
         sscursor_name: str = f"c_{uuid.uuid4().hex}"
-        cursor_args = _db_utils._convert_params(f"DECLARE {sscursor_name} CURSOR FOR {sql}", params)
+        cursor_args = _db_utils._convert_params(
+            f"DECLARE {pg8000_native.identifier(sscursor_name)} CURSOR FOR {sql}", params
+        )
         cursor.execute(*cursor_args)
 
         try:
             while True:
-                cursor.execute(f"FETCH FORWARD {chunksize} FROM {sscursor_name}")
+                cursor.execute(
+                    f"FETCH FORWARD {pg8000_native.literal(chunksize)} FROM {pg8000_native.identifier(sscursor_name)}"
+                )
                 records = cursor.fetchall()
 
                 if not records:
                     break
 
                 yield _db_utils._records2df(
                     records=records,
@@ -111,15 +116,15 @@
                     index=index_col,
                     safe=safe,
                     dtype=dtype,
                     timestamp_as_object=timestamp_as_object,
                     dtype_backend=dtype_backend,
                 )
         finally:
-            cursor.execute(f"CLOSE {sscursor_name}")
+            cursor.execute(f"CLOSE {pg8000_native.identifier(sscursor_name)}")
 
 
 @_utils.check_optional_dependency(pg8000, "pg8000")
 def connect(
     connection: Optional[str] = None,
     secret_id: Optional[str] = None,
     catalog_id: Optional[str] = None,
@@ -454,15 +459,19 @@
     ...     table="my_table",
     ...     schema="public",
     ...     con=con
     ... )
     >>> con.close()
 
     """
-    sql: str = f'SELECT * FROM "{table}"' if schema is None else f'SELECT * FROM "{schema}"."{table}"'
+    sql: str = (
+        f"SELECT * FROM {pg8000_native.identifier(table)}"
+        if schema is None
+        else f"SELECT * FROM {pg8000_native.identifier(schema)}.{pg8000_native.identifier(table)}"
+    )
     return read_sql_query(
         sql=sql,
         con=con,
         index_col=index_col,
         params=params,
         chunksize=chunksize,
         dtype=dtype,
@@ -587,15 +596,15 @@
             if mode == "append" and insert_conflict_columns:
                 conflict_columns = ", ".join(insert_conflict_columns)
                 upsert_str = f" ON CONFLICT ({conflict_columns}) DO NOTHING"
             placeholder_parameter_pair_generator = _db_utils.generate_placeholder_parameter_pairs(
                 df=df, column_placeholders=column_placeholders, chunksize=chunksize
             )
             for placeholders, parameters in placeholder_parameter_pair_generator:
-                sql: str = f'INSERT INTO "{schema}"."{table}" {insertion_columns} VALUES {placeholders}{upsert_str}'
+                sql: str = f"INSERT INTO {pg8000_native.identifier(schema)}.{pg8000_native.identifier(table)} {insertion_columns} VALUES {placeholders}{upsert_str}"
                 _logger.debug("sql: %s", sql)
                 cursor.executemany(sql, (parameters,))
             con.commit()
     except Exception as ex:
         con.rollback()
         _logger.error(ex)
         raise
```

### Comparing `awswrangler-3.2.1/awswrangler/quicksight/__init__.py` & `awswrangler-3.3.0/awswrangler/quicksight/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/quicksight/_cancel.py` & `awswrangler-3.3.0/awswrangler/quicksight/_cancel.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/quicksight/_create.py` & `awswrangler-3.3.0/awswrangler/quicksight/_create.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/quicksight/_delete.py` & `awswrangler-3.3.0/awswrangler/quicksight/_delete.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/quicksight/_describe.py` & `awswrangler-3.3.0/awswrangler/quicksight/_describe.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/quicksight/_get_list.py` & `awswrangler-3.3.0/awswrangler/quicksight/_get_list.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/quicksight/_utils.py` & `awswrangler-3.3.0/awswrangler/quicksight/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/redshift/_connect.py` & `awswrangler-3.3.0/awswrangler/redshift/_connect.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/redshift/_read.py` & `awswrangler-3.3.0/awswrangler/redshift/_read.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/redshift/_read.pyi` & `awswrangler-3.3.0/awswrangler/redshift/_read.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/redshift/_utils.py` & `awswrangler-3.3.0/awswrangler/redshift/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,15 +345,17 @@
         diststyle=diststyle,
         distkey=distkey,
         sortstyle=sortstyle,
         sortkey=sortkey,
         primary_keys=primary_keys,
     )
     cols_str: str = "".join([f'"{k}" {v},\n' for k, v in redshift_types.items()])[:-2]
-    primary_keys_str: str = f",\nPRIMARY KEY ({', '.join(primary_keys)})" if primary_keys else ""
+    primary_keys_str: str = (
+        ",\nPRIMARY KEY ({})".format(", ".join('"' + pk + '"' for pk in primary_keys)) if primary_keys else ""
+    )
     distkey_str: str = f"\nDISTKEY({distkey})" if distkey and diststyle == "KEY" else ""
     sortkey_str: str = f"\n{sortstyle} SORTKEY({','.join(sortkey)})" if sortkey else ""
     sql = (
         f'CREATE TABLE IF NOT EXISTS "{schema}"."{table}" (\n'
         f"{cols_str}"
         f"{primary_keys_str}"
         f")\nDISTSTYLE {diststyle}"
```

### Comparing `awswrangler-3.2.1/awswrangler/redshift/_write.py` & `awswrangler-3.3.0/awswrangler/redshift/_write.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/__init__.py` & `awswrangler-3.3.0/awswrangler/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_copy.py` & `awswrangler-3.3.0/awswrangler/s3/_copy.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_delete.py` & `awswrangler-3.3.0/awswrangler/s3/_delete.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_describe.py` & `awswrangler-3.3.0/awswrangler/s3/_describe.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_download.py` & `awswrangler-3.3.0/awswrangler/s3/_download.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_fs.py` & `awswrangler-3.3.0/awswrangler/s3/_fs.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_list.py` & `awswrangler-3.3.0/awswrangler/s3/_list.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_list.pyi` & `awswrangler-3.3.0/awswrangler/s3/_list.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_read.py` & `awswrangler-3.3.0/awswrangler/s3/_read.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_read_deltalake.py` & `awswrangler-3.3.0/awswrangler/s3/_read_deltalake.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         **s3_additional_kwargs,
     }
 
 
 @_utils.check_optional_dependency(deltalake, "deltalake")
 @apply_configs
 def read_deltalake(
-    path: Optional[str] = None,
+    path: str,
     version: Optional[int] = None,
     partitions: Optional[List[Tuple[str, str, Any]]] = None,
     columns: Optional[List[str]] = None,
     without_files: bool = False,
     dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
     use_threads: bool = True,
     boto3_session: Optional[boto3.Session] = None,
@@ -50,15 +50,15 @@
     <https://delta-io.github.io/delta-rs/python>`__.
     See the `How to load a Delta table
     <https://delta-io.github.io/delta-rs/python/usage.html#loading-a-delta-table>`__
     guide for loading instructions.
 
     Parameters
     ----------
-    path: Optional[str]
+    path: str
         The path of the DeltaTable.
     version: Optional[int]
         The version of the DeltaTable.
     partitions: Optional[List[Tuple[str, str, Any]]
         A list of partition filters, see help(DeltaTable.files_by_partitions)
         for filter syntax.
     columns: Optional[List[str]]
```

### Comparing `awswrangler-3.2.1/awswrangler/s3/_read_excel.py` & `awswrangler-3.3.0/awswrangler/s3/_read_excel.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_read_orc.py` & `awswrangler-3.3.0/awswrangler/s3/_read_orc.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_read_parquet.py` & `awswrangler-3.3.0/awswrangler/s3/_read_parquet.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
                 continue
 
             use_threads_flag: bool = use_threads if isinstance(use_threads, bool) else bool(use_threads > 1)
             chunks = pq_file.iter_batches(
                 batch_size=batch_size, columns=columns, use_threads=use_threads_flag, use_pandas_metadata=False
             )
             table = _add_table_partitions(
-                table=pa.Table.from_batches(chunks),
+                table=pa.Table.from_batches(chunks, schema=pq_file.schema.to_arrow_schema()),
                 path=path,
                 path_root=path_root,
             )
             df = _table_to_df(table=table, kwargs=arrow_kwargs)
             if chunked is True:
                 yield df
             else:
@@ -374,15 +374,15 @@
     partition_filter : Callable[[Dict[str, str]], bool], optional
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function must receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values must be strings and the function
         must return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-data-wrangler.readthedocs.io/en/3.2.1/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-data-wrangler.readthedocs.io/en/3.3.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     columns : List[str], optional
         List of columns to read from the file(s).
     validate_schema : bool, default False
         Check that the schema is consistent across individual files.
     coerce_int96_timestamp_unit : str, optional
         Cast timestamps that are stored in INT96 format to a particular resolution (e.g. "ms").
         Setting to None is equivalent to "ns" and therefore INT96 timestamps are inferred as in nanoseconds.
@@ -601,15 +601,15 @@
     partition_filter: Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function must receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values must be strings and the function
         must return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.3.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     columns : List[str], optional
         List of columns to read from the file(s).
     validate_schema : bool, default False
         Check that the schema is consistent across individual files.
     coerce_int96_timestamp_unit : str, optional
         Cast timestamps that are stored in INT96 format to a particular resolution (e.g. "ms").
         Setting to None is equivalent to "ns" and therefore INT96 timestamps are inferred as in nanoseconds.
```

### Comparing `awswrangler-3.2.1/awswrangler/s3/_read_parquet.pyi` & `awswrangler-3.3.0/awswrangler/s3/_read_parquet.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_read_text.py` & `awswrangler-3.3.0/awswrangler/s3/_read_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,15 +229,15 @@
     partition_filter : Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function MUST receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values will be always strings extracted from S3.
         This function MUST return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.3.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     ray_args: typing.RaySettings, optional
         Parameters of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
     pandas_kwargs :
         KEYWORD arguments forwarded to pandas.read_csv(). You can NOT pass `pandas_kwargs` explicitly, just add valid
         Pandas arguments in the function call and awswrangler will accept it.
         e.g. wr.s3.read_csv('s3://bucket/prefix/', sep='|', na_values=['null', 'none'], skip_blank_lines=True)
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html
@@ -389,15 +389,15 @@
     partition_filter: Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function MUST receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values will be always strings extracted from S3.
         This function MUST return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.3.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     ray_args: typing.RaySettings, optional
         Parameters of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
     pandas_kwargs:
         KEYWORD arguments forwarded to pandas.read_fwf(). You can NOT pass `pandas_kwargs` explicit, just add valid
         Pandas arguments in the function call and awswrangler will accept it.
         e.g. wr.s3.read_fwf(path='s3://bucket/prefix/', widths=[1, 3], names=["c0", "c1"])
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_fwf.html
@@ -556,15 +556,15 @@
     partition_filter: Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function MUST receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values will be always strings extracted from S3.
         This function MUST return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.3.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     ray_args: typing.RaySettings, optional
         Parameters of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
     pandas_kwargs:
         KEYWORD arguments forwarded to pandas.read_json(). You can NOT pass `pandas_kwargs` explicit, just add valid
         Pandas arguments in the function call and awswrangler will accept it.
         e.g. wr.s3.read_json('s3://bucket/prefix/', lines=True, keep_default_dates=True)
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_json.html
```

### Comparing `awswrangler-3.2.1/awswrangler/s3/_read_text.pyi` & `awswrangler-3.3.0/awswrangler/s3/_read_text.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_read_text_core.py` & `awswrangler-3.3.0/awswrangler/s3/_read_text_core.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_select.py` & `awswrangler-3.3.0/awswrangler/s3/_select.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_upload.py` & `awswrangler-3.3.0/awswrangler/s3/_upload.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_wait.py` & `awswrangler-3.3.0/awswrangler/s3/_wait.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_write.py` & `awswrangler-3.3.0/awswrangler/s3/_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 ) -> _SanitizeResult:
     df = catalog.sanitize_dataframe_columns_names(df=df)
     partition_cols = [catalog.sanitize_column_name(p) for p in partition_cols]
     if bucketing_info:
         bucketing_info = [
             catalog.sanitize_column_name(bucketing_col) for bucketing_col in bucketing_info[0]
         ], bucketing_info[1]
-    dtype = {catalog.sanitize_column_name(k): v.lower() for k, v in dtype.items()}
+    dtype = {catalog.sanitize_column_name(k): v for k, v in dtype.items()}
     _utils.check_duplicated_columns(df=df)
     return _SanitizeResult(df, dtype, partition_cols, bucketing_info)
 
 
 def _get_chunk_file_path(file_counter: int, file_path: str) -> str:
     slash_index: int = file_path.rfind("/")
     dot_index: int = file_path.find(".", slash_index)
```

### Comparing `awswrangler-3.2.1/awswrangler/s3/_write_concurrent.py` & `awswrangler-3.3.0/awswrangler/s3/_write_concurrent.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_write_dataset.py` & `awswrangler-3.3.0/awswrangler/s3/_write_dataset.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_write_deltalake.py` & `awswrangler-3.3.0/awswrangler/s3/_write_deltalake.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_write_excel.py` & `awswrangler-3.3.0/awswrangler/s3/_write_excel.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_write_orc.py` & `awswrangler-3.3.0/awswrangler/s3/_write_orc.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/s3/_write_parquet.py` & `awswrangler-3.3.0/awswrangler/s3/_write_parquet.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,26 +405,26 @@
     bucketing_info: Tuple[List[str], int], optional
         Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
         second element.
         Only `str`, `int` and `bool` are supported as column data types for bucketing.
     concurrent_partitioning: bool
         If True will increase the parallelism level during the partitions writing. It will decrease the
         writing time and increase the memory usage.
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.3.0/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
     mode: str, optional
         ``append`` (Default), ``overwrite``, ``overwrite_partitions``. Only takes effect if dataset=True.
         For details check the related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/004%20-%20Parquet%20Datasets.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.3.0/tutorials/004%20-%20Parquet%20Datasets.html
     catalog_versioning : bool
         If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
     schema_evolution : bool
         If True allows schema evolution (new or missing columns), otherwise a exception will be raised. True by default.
         (Only considered if dataset=True and mode in ("append", "overwrite_partitions"))
         Related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/014%20-%20Schema%20Evolution.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.3.0/tutorials/014%20-%20Schema%20Evolution.html
     database : str, optional
         Glue/Athena catalog: Database name.
     table : str, optional
         Glue/Athena catalog: Table name.
     glue_table_settings: dict (GlueTableSettings), optional
         Settings for writing to the Glue table.
     dtype : Dict[str, str], optional
```

### Comparing `awswrangler-3.2.1/awswrangler/s3/_write_text.py` & `awswrangler-3.3.0/awswrangler/s3/_write_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,26 +165,26 @@
     bucketing_info: Tuple[List[str], int], optional
         Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
         second element.
         Only `str`, `int` and `bool` are supported as column data types for bucketing.
     concurrent_partitioning: bool
         If True will increase the parallelism level during the partitions writing. It will decrease the
         writing time and increase the memory usage.
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.3.0/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
     mode : str, optional
         ``append`` (Default), ``overwrite``, ``overwrite_partitions``. Only takes effect if dataset=True.
         For details check the related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
+        https://aws-sdk-pandas.readthedocs.io/en/3.3.0/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
     catalog_versioning : bool
         If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
     schema_evolution : bool
         If True allows schema evolution (new or missing columns), otherwise a exception will be raised.
         (Only considered if dataset=True and mode in ("append", "overwrite_partitions")). False by default.
         Related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/014%20-%20Schema%20Evolution.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.3.0/tutorials/014%20-%20Schema%20Evolution.html
     database : str, optional
         Glue/Athena catalog: Database name.
     table : str, optional
         Glue/Athena catalog: Table name.
     glue_table_settings: dict (GlueTableSettings), optional
         Settings for writing to the Glue table.
     dtype : Dict[str, str], optional
@@ -769,26 +769,26 @@
     bucketing_info: Tuple[List[str], int], optional
         Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
         second element.
         Only `str`, `int` and `bool` are supported as column data types for bucketing.
     concurrent_partitioning: bool
         If True will increase the parallelism level during the partitions writing. It will decrease the
         writing time and increase the memory usage.
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.3.0/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
     mode : str, optional
         ``append`` (Default), ``overwrite``, ``overwrite_partitions``. Only takes effect if dataset=True.
         For details check the related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
+        https://aws-sdk-pandas.readthedocs.io/en/3.3.0/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
     catalog_versioning : bool
         If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
     schema_evolution : bool
         If True allows schema evolution (new or missing columns), otherwise a exception will be raised.
         (Only considered if dataset=True and mode in ("append", "overwrite_partitions"))
         Related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/014%20-%20Schema%20Evolution.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.3.0/tutorials/014%20-%20Schema%20Evolution.html
     database : str, optional
         Glue/Athena catalog: Database name.
     table : str, optional
         Glue/Athena catalog: Table name.
     glue_table_settings: dict (GlueTableSettings), optional
         Settings for writing to the Glue table.
     dtype : Dict[str, str], optional
```

### Comparing `awswrangler-3.2.1/awswrangler/secretsmanager.py` & `awswrangler-3.3.0/awswrangler/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/sqlserver.py` & `awswrangler-3.3.0/awswrangler/sqlserver.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/sts.py` & `awswrangler-3.3.0/awswrangler/sts.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/timestream/__init__.py` & `awswrangler-3.3.0/awswrangler/timestream/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/timestream/_create.py` & `awswrangler-3.3.0/awswrangler/timestream/_create.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/timestream/_delete.py` & `awswrangler-3.3.0/awswrangler/timestream/_delete.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/timestream/_list.py` & `awswrangler-3.3.0/awswrangler/timestream/_list.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/timestream/_read.py` & `awswrangler-3.3.0/awswrangler/timestream/_read.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/timestream/_read.pyi` & `awswrangler-3.3.0/awswrangler/timestream/_read.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/timestream/_write.py` & `awswrangler-3.3.0/awswrangler/timestream/_write.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/awswrangler/typing.py` & `awswrangler-3.3.0/awswrangler/typing.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.1/pyproject.toml` & `awswrangler-3.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "awswrangler"
-version = "3.2.1"
+version = "3.3.0"
 description = "Pandas on AWS."
 authors = ["Amazon Web Services"]
 license = "Apache License 2.0"
 
 readme = "README.md"
 
 include = ["README.md", "LICENSE.txt", "NOTICE.txt", "THIRD_PARTY.txt", "awswrangler/py.typed"]
@@ -26,15 +26,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8, <4.0"
 
 # Required
 boto3 = "^1.20.32"
 botocore = "^1.23.32"
-pandas = ">=1.2.0,!=1.5.0,<3.0.0" # Exclusion per: https://github.com/aws/aws-sdk-pandas/issues/1678
+pandas = ">=1.2.0,<3.0.0"
 numpy = "^1.18"
 pyarrow = ">=7.0.0"
 typing-extensions = "^4.4.0"
 packaging = ">=21.1,<24.0"
 
 # Databases
 redshift-connector = { version = "^2.0.0", optional = true }
@@ -52,19 +52,19 @@
 opensearch-py = { version = "^2.0.0", optional = true }
 requests-aws4auth = { version = "^1.1.1", optional = true }
 jsonpath-ng = { version = "^1.5.3", optional = true }
 
 # Other
 openpyxl = { version = "^3.0.0", optional = true }
 progressbar2 = { version = "^4.0.0", optional = true }
-deltalake = { version = ">=0.6.4,<0.10.0", optional = true }
+deltalake = { version = ">=0.6.4,<0.11.0", optional = true }
 
 # Distributed
-modin = { version = "^0.20.1", optional = true }
-ray = { version = ">=2.0.0,<2.6.0", extras = ["default", "data"], optional = true }
+modin = { version = "^0.23.0", optional = true }
+ray = { version = ">=2.0.0,<2.7.0", extras = ["default", "data"], optional = true }
 
 [tool.poetry.extras]
 redshift = ["redshift-connector"]
 mysql = ["pymysql"]
 postgres = ["pg8000"]
 sqlserver = ["pyodbc"]
 oracle = ["oracledb"]
@@ -81,15 +81,15 @@
 [tool.poetry.dev-dependencies]
 # Build
 setuptools = "*"
 wheel = "^0.38.1"
 
 # Lint
 black = "^23.1.0"
-boto3-stubs = {version = "1.26.151", extras = ["athena", "chime", "cloudwatch", "dynamodb", "ec2", "emr", "emr-serverless", "glue", "kms", "lakeformation", "logs", "neptune", "opensearch", "opensearchserverless", "quicksight", "rds", "rds-data", "redshift", "redshift-data", "s3", "secretsmanager", "ssm", "sts", "timestream-query", "timestream-write"]}
+boto3-stubs = {version = "^1.26.151", extras = ["athena", "cleanrooms", "chime", "cloudwatch", "dynamodb", "ec2", "emr", "emr-serverless", "glue", "kms", "lakeformation", "logs", "neptune", "opensearch", "opensearchserverless", "quicksight", "rds", "rds-data", "redshift", "redshift-data", "s3", "secretsmanager", "ssm", "sts", "timestream-query", "timestream-write"]}
 doc8 = "^1.0"
 mypy = "^1.0"
 pylint = "^2.17"
 ruff = "^0.0.270"
 isort = "^5.9.2"
 flake8 = "^5.0.1"
 pydocstyle = "^6.1.1"
@@ -120,15 +120,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
-target-version = ["py38", "py39", "py310"]
+target-version = ["py38", "py39", "py310", "py311"]
 extend_exclude = '''
 /(
     \.eggs
   | \.git
   | \.hg
   | \.mypy_cache
   | \.tox
```

### Comparing `awswrangler-3.2.1/PKG-INFO` & `awswrangler-3.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 Metadata-Version: 2.1
 Name: awswrangler
-Version: 3.2.1
+Version: 3.3.0
 Summary: Pandas on AWS.
 Home-page: https://aws-sdk-pandas.readthedocs.io/
 License: Apache-2.0
 Keywords: pandas,aws
 Author: Amazon Web Services
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: deltalake
 Provides-Extra: gremlin
 Provides-Extra: modin
 Provides-Extra: mysql
 Provides-Extra: opencypher
 Provides-Extra: openpyxl
 Provides-Extra: opensearch
@@ -30,30 +26,30 @@
 Provides-Extra: ray
 Provides-Extra: redshift
 Provides-Extra: sparql
 Provides-Extra: sqlserver
 Requires-Dist: SPARQLWrapper (>=2.0.0,<3.0.0) ; extra == "sparql"
 Requires-Dist: boto3 (>=1.20.32,<2.0.0)
 Requires-Dist: botocore (>=1.23.32,<2.0.0)
-Requires-Dist: deltalake (>=0.6.4,<0.10.0) ; extra == "deltalake"
+Requires-Dist: deltalake (>=0.6.4,<0.11.0) ; extra == "deltalake"
 Requires-Dist: gremlinpython (>=3.6.2,<4.0.0) ; extra == "gremlin"
 Requires-Dist: jsonpath-ng (>=1.5.3,<2.0.0) ; extra == "opensearch"
-Requires-Dist: modin (>=0.20.1,<0.21.0) ; extra == "modin"
+Requires-Dist: modin (>=0.23.0,<0.24.0) ; extra == "modin"
 Requires-Dist: numpy (>=1.18,<2.0)
 Requires-Dist: openpyxl (>=3.0.0,<4.0.0) ; extra == "openpyxl"
 Requires-Dist: opensearch-py (>=2.0.0,<3.0.0) ; extra == "opensearch"
 Requires-Dist: oracledb (>=1.0.0,<2.0.0) ; extra == "oracle"
 Requires-Dist: packaging (>=21.1,<24.0)
-Requires-Dist: pandas (>=1.2.0,!=1.5.0,<3.0.0)
+Requires-Dist: pandas (>=1.2.0,<3.0.0)
 Requires-Dist: pg8000 (>=1.29.0,<2.0.0) ; extra == "postgres"
 Requires-Dist: progressbar2 (>=4.0.0,<5.0.0) ; extra == "progressbar"
 Requires-Dist: pyarrow (>=7.0.0)
 Requires-Dist: pymysql (>=1.0.0,<2.0.0) ; extra == "mysql"
 Requires-Dist: pyodbc (>=4.0.0,<5.0.0) ; extra == "sqlserver"
-Requires-Dist: ray[data,default] (>=2.0.0,<2.6.0) ; extra == "ray"
+Requires-Dist: ray[data,default] (>=2.0.0,<2.7.0) ; extra == "ray"
 Requires-Dist: redshift-connector (>=2.0.0,<3.0.0) ; extra == "redshift"
 Requires-Dist: requests (>=2.0.0,<3.0.0) ; extra == "gremlin" or extra == "sparql" or extra == "opencypher"
 Requires-Dist: requests-aws4auth (>=1.1.1,<2.0.0) ; extra == "opensearch"
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Project-URL: Documentation, https://aws-sdk-pandas.readthedocs.io/
 Project-URL: Repository, https://github.com/aws/aws-sdk-pandas
 Description-Content-Type: text/markdown
@@ -67,16 +63,16 @@
 Easy integration with Athena, Glue, Redshift, Timestream, OpenSearch, Neptune, QuickSight, Chime, CloudWatchLogs, DynamoDB, EMR, SecretManager, PostgreSQL, MySQL, SQLServer and S3 (Parquet, CSV, JSON and EXCEL).
 
 ![AWS SDK for pandas](docs/source/_static/logo2.png?raw=true "AWS SDK for pandas")
 ![tracker](https://d3tiqpr4kkkomd.cloudfront.net/img/pixel.png?asset=GVOYN2BOOQ573LTVIHEW)
 
 > An [AWS Professional Service](https://aws.amazon.com/professional-services/) open source initiative | aws-proserve-opensource@amazon.com
 
-[![Release](https://img.shields.io/badge/3.2.1-brightgreen.svg)](https://pypi.org/project/awswrangler/)
-[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.8%20%7C%203.9%20%7C%203.10-brightgreen.svg)](https://anaconda.org/conda-forge/awswrangler)
+[![Release](https://img.shields.io/badge/3.3.0-brightgreen.svg)](https://pypi.org/project/awswrangler/)
+[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-brightgreen.svg)](https://anaconda.org/conda-forge/awswrangler)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 ![Static Checking](https://github.com/aws/aws-sdk-pandas/workflows/Static%20Checking/badge.svg?branch=main)
 [![Documentation Status](https://readthedocs.org/projects/aws-sdk-pandas/badge/?version=latest)](https://aws-sdk-pandas.readthedocs.io/?badge=latest)
 
@@ -155,33 +151,33 @@
 """)
 
 ```
 
 ## At scale
 AWS SDK for pandas can also run your workflows at scale by leveraging [Modin](https://modin.readthedocs.io/en/stable/) and [Ray](https://www.ray.io/). Both projects aim to speed up data workloads by distributing processing over a cluster of workers.
 
-The quickest way to get started is to use AWS Glue with Ray. Read our [docs](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/scale.html), our [blog](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/), or head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials) to discover even more features.
+The quickest way to get started is to use AWS Glue with Ray. Read our [docs](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/scale.html), our blogs ([1](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/)/[2](https://aws.amazon.com/blogs/big-data/advanced-patterns-with-aws-sdk-for-pandas-on-aws-glue-for-ray/)), or head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials) to discover even more features.
 
 ## [Read The Docs](https://aws-sdk-pandas.readthedocs.io/)
 
-- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/about.html)
-- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html)
-  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#pypi-pip)
-  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#conda)
-  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#aws-lambda-layer)
-  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#aws-glue-python-shell-jobs)
-  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#aws-glue-pyspark-jobs)
-  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#amazon-sagemaker-notebook)
-  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#amazon-sagemaker-notebook-lifecycle)
-  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#emr)
-  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#from-source)
-- [**At scale**](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/scale.html)
-  - [Getting Started](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/scale.html#getting-started)
-  - [Supported APIs](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/scale.html#supported-apis)
-  - [Resources](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/scale.html#resources)
+- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/about.html)
+- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/install.html)
+  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/install.html#pypi-pip)
+  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/install.html#conda)
+  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/install.html#aws-lambda-layer)
+  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/install.html#aws-glue-python-shell-jobs)
+  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/install.html#aws-glue-pyspark-jobs)
+  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/install.html#amazon-sagemaker-notebook)
+  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/install.html#amazon-sagemaker-notebook-lifecycle)
+  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/install.html#emr)
+  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/install.html#from-source)
+- [**At scale**](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/scale.html)
+  - [Getting Started](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/scale.html#getting-started)
+  - [Supported APIs](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/scale.html#supported-apis)
+  - [Resources](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/scale.html#resources)
 - [**Tutorials**](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials)
   - [001 - Introduction](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/001%20-%20Introduction.ipynb)
   - [002 - Sessions](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/002%20-%20Sessions.ipynb)
   - [003 - Amazon S3](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/003%20-%20Amazon%20S3.ipynb)
   - [004 - Parquet Datasets](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/004%20-%20Parquet%20Datasets.ipynb)
   - [005 - Glue Catalog](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/005%20-%20Glue%20Catalog.ipynb)
   - [006 - Amazon Athena](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/006%20-%20Amazon%20Athena.ipynb)
@@ -214,39 +210,41 @@
   - [033 - Amazon Neptune](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/033%20-%20Amazon%20Neptune.ipynb)
   - [034 - Distributing Calls Using Ray](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/034%20-%20Distributing%20Calls%20using%20Ray.ipynb)
   - [035 - Distributing Calls on Ray Remote Cluster](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/035%20-%20Distributing%20Calls%20on%20Ray%20Remote%20Cluster.ipynb)
   - [036 - Distributing Calls with Glue Interactive Sessions on Ray](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/036%20-%20Distributing%20Calls%20with%20Glue%20Interactive%20Sessions%20on%20Ray.ipynb)
   - [037 - Glue Data Quality](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/037%20-%20Glue%20Data%20Quality.ipynb)
   - [038 - OpenSearch Serverless](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/038%20-%20OpenSearch%20Serverless.ipynb)
   - [039 - Athena Iceberg](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/039%20-%20Athena%20Iceberg.ipynb)
-- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html)
-  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-s3)
-  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#aws-glue-catalog)
-  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-athena)
-  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#aws-lake-formation)
-  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-redshift)
-  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#postgresql)
-  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#mysql)
-  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#sqlserver)
-  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#oracle)
-  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#data-api-redshift)
-  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#data-api-rds)
-  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#opensearch)
-  - [AWS Glue Data Quality](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#aws-glue-data-quality)
-  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-neptune)
-  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#dynamodb)
-  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-timestream)
-  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-emr)
-  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-cloudwatch-logs)
-  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-chime)
-  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-quicksight)
-  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#aws-sts)
-  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#aws-secrets-manager)
-  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#global-configurations)
-  - [Distributed - Ray](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#distributed-ray)
+  - [040 - EMR Serverless](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/040%20-%20EMR%20Serverless.ipynb)
+  - [041 - Apache Spark on Amazon Athena](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/041%20-%20Apache%20Spark%20on%20Amazon%20Athena.ipynb)
+- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html)
+  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#amazon-s3)
+  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#aws-glue-catalog)
+  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#amazon-athena)
+  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#aws-lake-formation)
+  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#amazon-redshift)
+  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#postgresql)
+  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#mysql)
+  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#sqlserver)
+  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#oracle)
+  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#data-api-redshift)
+  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#data-api-rds)
+  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#opensearch)
+  - [AWS Glue Data Quality](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#aws-glue-data-quality)
+  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#amazon-neptune)
+  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#dynamodb)
+  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#amazon-timestream)
+  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#amazon-emr)
+  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#amazon-cloudwatch-logs)
+  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#amazon-chime)
+  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#amazon-quicksight)
+  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#aws-sts)
+  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#aws-secrets-manager)
+  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#global-configurations)
+  - [Distributed - Ray](https://aws-sdk-pandas.readthedocs.io/en/3.3.0/api.html#distributed-ray)
 - [**License**](https://github.com/aws/aws-sdk-pandas/blob/main/LICENSE.txt)
 - [**Contributing**](https://github.com/aws/aws-sdk-pandas/blob/main/CONTRIBUTING.md)
 
 ## Getting Help
 
 The best way to interact with our team is through GitHub. You can open an [issue](https://github.com/aws/aws-sdk-pandas/issues/new/choose) and choose from one of our templates for bug reports, feature requests...
 You may also find help on these community resources:
@@ -255,14 +253,15 @@
   and tag it with `awswrangler`
 * [Runbook](https://github.com/aws/aws-sdk-pandas/discussions/1815) for AWS SDK for pandas with Ray
 
 ## Community Resources
 
 Please [send a Pull Request](https://github.com/aws/aws-sdk-pandas/edit/main/README.md) with your resource reference and @githubhandle.
 
+- [YouTube channel](https://www.youtube.com/playlist?list=PL7bE4nSzLSWdDdlfRgfKo2JBplB4p_v5O) [[@AdrianoNicolucci](https://github.com/AdrianoNicolucci)]
 - [Optimize Python ETL by extending Pandas with AWS SDK for pandas](https://aws.amazon.com/blogs/big-data/optimize-python-etl-by-extending-pandas-with-aws-data-wrangler/) [[@igorborgest](https://github.com/igorborgest)]
 - [Reading Parquet Files With AWS Lambda](https://aprakash.wordpress.com/2020/04/14/reading-parquet-files-with-aws-lambda/) [[@anand086](https://github.com/anand086)]
 - [Transform AWS CloudTrail data using AWS SDK for pandas](https://aprakash.wordpress.com/2020/09/17/transform-aws-cloudtrail-data-using-aws-data-wrangler/) [[@anand086](https://github.com/anand086)]
 - [Rename Glue Tables using AWS SDK for pandas](https://ananddatastories.com/rename-glue-tables-using-aws-sdk-pandas/) [[@anand086](https://github.com/anand086)]
 - [Getting started on AWS SDK for pandas and Athena](https://medium.com/@dheerajsharmainampudi/getting-started-on-aws-sdk-pandas-and-athena-7b446c834076) [[@dheerajsharma21](https://github.com/dheerajsharma21)]
 - [Simplifying Pandas integration with AWS data related services](https://medium.com/@bv_subhash/aws-sdk-pandas-simplifying-pandas-integration-with-aws-data-related-services-2b3325c12188) [[@bvsubhash](https://github.com/bvsubhash)]
 - [Build an ETL pipeline using AWS S3, Glue and Athena](https://www.linkedin.com/pulse/build-etl-pipeline-using-aws-s3-glue-athena-data-wrangler-tom-reid/) [[@taupirho](https://github.com/taupirho)]
@@ -298,14 +297,15 @@
 - [DNX](https://www.dnx.solutions/) [[@DNXLabs](https://github.com/DNXLabs)]
 - [Fortescue Future Industries](https://ffi.com.au/) [[@spencervoorend](https://github.com/spencervoorend)]
 - [Funcional Health Tech](https://www.funcionalcorp.com.br/) [[@webysther](https://github.com/webysther)]
 - [Funding Circle](https://www.fundingcircle.com/) [[@pfig](https://github.com/pfig)]
 - [Infomach](https://www.infomach.com.br/)
 - [Informa Markets](https://www.informamarkets.com/en/home.html) [[@mateusmorato]](http://github.com/mateusmorato)
 - [LINE TV](https://www.linetv.tw/) [[@bryanyang0528](https://github.com/bryanyang0528)]
+- [LogicalCube](https://www.logicalcube.com) [[@zolabud](https://github.com/zolabud)]
 - [Magnataur](https://magnataur.com) [[@brianmingus2](https://github.com/brianmingus2)]
 - [M4U](https://www.m4u.com.br/) [[@Thiago-Dantas](https://github.com/Thiago-Dantas)]
 - [NBCUniversal](https://www.nbcuniversal.com/) [[@vibe](https://github.com/vibe)]
 - [nrd.io](https://nrd.io/) [[@mrtns](https://github.com/mrtns)]
 - [OKRA Technologies](https://okra.ai) [[@JPFrancoia](https://github.com/JPFrancoia), [@schot](https://github.com/schot)]
 - [Pier](https://www.pier.digital/) [[@flaviomax](https://github.com/flaviomax)]
 - [Pismo](https://www.pismo.io/) [[@msantino](https://github.com/msantino)]
```

