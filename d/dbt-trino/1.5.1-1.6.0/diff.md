# Comparing `tmp/dbt-trino-1.5.1.tar.gz` & `tmp/dbt-trino-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-trino-1.5.1.tar", last modified: Mon Jul 17 19:17:02 2023, max compression
+gzip compressed data, was "dbt-trino-1.6.0.tar", last modified: Tue Aug  1 14:12:15 2023, max compression
```

## Comparing `dbt-trino-1.5.1.tar` & `dbt-trino-1.6.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.616028 dbt-trino-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-07-17 19:17:02.616028 dbt-trino-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.608027 dbt-trino-1.5.1/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.608027 dbt-trino-1.5.1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.612027 dbt-trino-1.5.1/dbt/adapters/trino/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/adapters/trino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/adapters/trino/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/adapters/trino/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    16345 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/adapters/trino/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/adapters/trino/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/adapters/trino/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.608027 dbt-trino-1.5.1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.612027 dbt-trino-1.5.1/dbt/include/trino/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.612027 dbt-trino-1.5.1/dbt/include/trino/macros/
--rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.612027 dbt-trino-1.5.1/dbt/include/trino/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/materializations/materialized_view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.612027 dbt-trino-1.5.1/dbt/include/trino/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.612027 dbt-trino-1.5.1/dbt/include/trino/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/datatypes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/dbt/include/trino/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:17:02.616028 dbt-trino-1.5.1/dbt_trino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-07-17 19:17:02.000000 dbt-trino-1.5.1/dbt_trino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-17 19:17:02.000000 dbt-trino-1.5.1/dbt_trino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:17:02.000000 dbt-trino-1.5.1/dbt_trino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:17:02.000000 dbt-trino-1.5.1/dbt_trino.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 19:17:02.000000 dbt-trino-1.5.1/dbt_trino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-17 19:17:02.000000 dbt-trino-1.5.1/dbt_trino.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 19:17:02.616028 dbt-trino-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-17 19:16:21.000000 dbt-trino-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:12:15.313283 dbt-trino-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-08-01 14:12:15.313283 dbt-trino-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:12:15.305283 dbt-trino-1.6.0/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:12:15.305283 dbt-trino-1.6.0/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:12:15.309283 dbt-trino-1.6.0/dbt/adapters/trino/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/adapters/trino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/adapters/trino/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/adapters/trino/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16035 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/adapters/trino/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/adapters/trino/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/adapters/trino/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:12:15.305283 dbt-trino-1.6.0/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:12:15.309283 dbt-trino-1.6.0/dbt/include/trino/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:12:15.309283 dbt-trino-1.6.0/dbt/include/trino/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    10507 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:12:15.309283 dbt-trino-1.6.0/dbt/include/trino/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/materializations/materialized_view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:12:15.309283 dbt-trino-1.6.0/dbt/include/trino/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:12:15.313283 dbt-trino-1.6.0/dbt/include/trino/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/utils/datatypes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/dbt/include/trino/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:12:15.313283 dbt-trino-1.6.0/dbt_trino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-08-01 14:12:15.000000 dbt-trino-1.6.0/dbt_trino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-08-01 14:12:15.000000 dbt-trino-1.6.0/dbt_trino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:12:15.000000 dbt-trino-1.6.0/dbt_trino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:12:15.000000 dbt-trino-1.6.0/dbt_trino.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 14:12:15.000000 dbt-trino-1.6.0/dbt_trino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-01 14:12:15.000000 dbt-trino-1.6.0/dbt_trino.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:12:15.313283 dbt-trino-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-08-01 14:11:42.000000 dbt-trino-1.6.0/setup.py
```

### Comparing `dbt-trino-1.5.1/LICENSE.txt` & `dbt-trino-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.1/PKG-INFO` & `dbt-trino-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: dbt-trino
-Version: 1.5.1
+Version: 1.6.0
 Summary: The trino adapter plugin for dbt (data build tool)
 Home-page: https://github.com/starburstdata/dbt-trino
 Author: Starburst Data
 Author-email: info@starburstdata.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # dbt-trino
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/Starburst_Logo_White%2BBlue.svg" width="98%">
```

### Comparing `dbt-trino-1.5.1/README.md` & `dbt-trino-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.1/dbt/adapters/trino/__init__.py` & `dbt-trino-1.6.0/dbt/adapters/trino/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.1/dbt/adapters/trino/column.py` & `dbt-trino-1.6.0/dbt/adapters/trino/column.py`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.1/dbt/adapters/trino/connections.py` & `dbt-trino-1.6.0/dbt/adapters/trino/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -478,16 +478,14 @@
             without_comments = re.sub(
                 re.compile("^.*(--.*)$", re.MULTILINE), "", individual_query
             ).strip()
 
             if without_comments == "":
                 continue
 
-            individual_query = self._add_query_comment(individual_query)
-
             parent = super(TrinoConnectionManager, self)
             connection, cursor = parent.add_query(
                 individual_query, auto_begin, bindings, abridge_sql_log
             )
 
         if cursor is None:
             conn = self.get_thread_connection()
@@ -501,16 +499,10 @@
                 "conditionally running\nsql, eg. in a model hook, make "
                 "sure your `else` clause contains valid sql!\n\n"
                 "Provided SQL:\n{}".format(conn_name, sql)
             )
 
         return connection, cursor
 
-    def execute(self, sql, auto_begin=False, fetch=False):
-        _, cursor = self.add_query(sql, auto_begin)
-        status = self.get_response(cursor)
-        table = self.get_result_from_cursor(cursor)
-        return status, table
-
     @classmethod
     def data_type_code_to_name(cls, type_code) -> str:
         return type_code.split("(")[0].upper()
```

### Comparing `dbt-trino-1.5.1/dbt/adapters/trino/impl.py` & `dbt-trino-1.6.0/dbt/adapters/trino/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.1/dbt/adapters/trino/relation.py` & `dbt-trino-1.6.0/dbt/adapters/trino/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.1/dbt/include/trino/macros/adapters.sql` & `dbt-trino-1.6.0/dbt/include/trino/macros/adapters.sql`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 {% macro trino__list_relations_without_caching(relation) %}
   {% call statement('list_relations_without_caching', fetch_result=True) -%}
     select
       t.table_catalog as database,
       t.table_name as name,
       t.table_schema as schema,
-      case when mv.name is not null then 'materializedview'
+      case when mv.name is not null then 'materialized_view'
            when t.table_type = 'BASE TABLE' then 'table'
            when t.table_type = 'VIEW' then 'view'
            else t.table_type
       end as table_type
     from {{ relation.information_schema() }}.tables t
     left join system.metadata.materialized_views mv
           on mv.catalog_name = t.table_catalog and mv.schema_name = t.table_schema and mv.name = t.table_name
@@ -145,15 +145,15 @@
   as
     {{ sql }}
   ;
 {% endmacro %}
 
 
 {% macro trino__drop_relation(relation) -%}
-  {% set relation_type = 'materialized view' if relation.type == 'materializedview' else relation.type %}
+  {% set relation_type = relation.type|replace("_", " ") %}
   {% call statement('drop_relation', auto_begin=False) -%}
     drop {{ relation_type }} if exists {{ relation }}
   {%- endcall %}
 {% endmacro %}
 
 
 {# see this issue: https://github.com/dbt-labs/dbt/issues/2267 #}
@@ -179,15 +179,15 @@
   {%- call statement('drop_schema') -%}
     drop schema if exists {{ relation }}
   {% endcall %}
 {% endmacro %}
 
 
 {% macro trino__rename_relation(from_relation, to_relation) -%}
-  {% set from_relation_type = 'materialized view' if from_relation.type == 'materializedview' else from_relation.type %}
+  {% set from_relation_type = from_relation.type|replace("_", " ") %}
   {% call statement('rename_relation') -%}
     alter {{ from_relation_type }} {{ from_relation }} rename to {{ to_relation }}
   {%- endcall %}
 {% endmacro %}
 
 
 {% macro trino__alter_relation_comment(relation, relation_comment) -%}
```

### Comparing `dbt-trino-1.5.1/dbt/include/trino/macros/apply_grants.sql` & `dbt-trino-1.6.0/dbt/include/trino/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.1/dbt/include/trino/macros/catalog.sql` & `dbt-trino-1.6.0/dbt/include/trino/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.1/dbt/include/trino/macros/materializations/incremental.sql` & `dbt-trino-1.6.0/dbt/include/trino/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.1/dbt/include/trino/macros/materializations/seeds/helpers.sql` & `dbt-trino-1.6.0/dbt/include/trino/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.1/dbt/include/trino/macros/materializations/snapshot.sql` & `dbt-trino-1.6.0/dbt/include/trino/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.1/dbt/include/trino/macros/materializations/table.sql` & `dbt-trino-1.6.0/dbt/include/trino/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.1/dbt/include/trino/macros/utils/datediff.sql` & `dbt-trino-1.6.0/dbt/include/trino/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.1/dbt/include/trino/sample_profiles.yml` & `dbt-trino-1.6.0/dbt/include/trino/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.1/dbt_trino.egg-info/PKG-INFO` & `dbt-trino-1.6.0/dbt_trino.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: dbt-trino
-Version: 1.5.1
+Version: 1.6.0
 Summary: The trino adapter plugin for dbt (data build tool)
 Home-page: https://github.com/starburstdata/dbt-trino
 Author: Starburst Data
 Author-email: info@starburstdata.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # dbt-trino
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/starburstdata/dbt-trino/master/assets/images/Starburst_Logo_White%2BBlue.svg" width="98%">
```

### Comparing `dbt-trino-1.5.1/dbt_trino.egg-info/SOURCES.txt` & `dbt-trino-1.6.0/dbt_trino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.5.1/setup.py` & `dbt-trino-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python
 import os
 import re
 import sys
 
-# require python 3.7 or newer
-if sys.version_info < (3, 7):
+# require python 3.8 or newer
+if sys.version_info < (3, 8):
     print("Error: dbt does not support this version of Python.")
-    print("Please upgrade to Python 3.7 or higher.")
+    print("Please upgrade to Python 3.8 or higher.")
     sys.exit(1)
 
 
 # require version of setuptools that supports find_namespace_packages
 from setuptools import setup
 
 try:
@@ -91,15 +91,14 @@
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
 )
```

