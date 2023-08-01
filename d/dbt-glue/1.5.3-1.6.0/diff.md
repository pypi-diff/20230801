# Comparing `tmp/dbt-glue-1.5.3.tar.gz` & `tmp/dbt-glue-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-glue-1.5.3.tar", last modified: Mon Jul 17 09:35:23 2023, max compression
+gzip compressed data, was "dbt-glue-1.6.0.tar", last modified: Tue Aug  1 11:13:14 2023, max compression
```

## Comparing `dbt-glue-1.5.3.tar` & `dbt-glue-1.6.0.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.126378 dbt-glue-1.5.3/
--rw-r--r--   0 menuetb    (504) staff       (20)    10142 2022-04-05 16:42:41.000000 dbt-glue-1.5.3/LICENSE
--rw-r--r--   0 menuetb    (504) staff       (20)       67 2022-04-05 16:42:41.000000 dbt-glue-1.5.3/NOTICE
--rw-r--r--   0 menuetb    (504) staff       (20)    44977 2023-07-17 09:35:23.126216 dbt-glue-1.5.3/PKG-INFO
--rw-r--r--   0 menuetb    (504) staff       (20)    44126 2023-07-05 15:16:41.000000 dbt-glue-1.5.3/README.md
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.118651 dbt-glue-1.5.3/dbt/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.118465 dbt-glue-1.5.3/dbt/adapters/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.121748 dbt-glue-1.5.3/dbt/adapters/glue/
--rw-r--r--   0 menuetb    (504) staff       (20)      394 2023-04-06 15:48:24.000000 dbt-glue-1.5.3/dbt/adapters/glue/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)       17 2023-07-17 09:34:17.000000 dbt-glue-1.5.3/dbt/adapters/glue/__version__.py
--rw-r--r--   0 menuetb    (504) staff       (20)     3917 2023-06-29 08:34:49.000000 dbt-glue-1.5.3/dbt/adapters/glue/connections.py
--rw-r--r--   0 menuetb    (504) staff       (20)     2585 2023-07-05 15:16:41.000000 dbt-glue-1.5.3/dbt/adapters/glue/credentials.py
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.122421 dbt-glue-1.5.3/dbt/adapters/glue/gluedbapi/
--rw-r--r--   0 menuetb    (504) staff       (20)      140 2022-04-05 16:42:41.000000 dbt-glue-1.5.3/dbt/adapters/glue/gluedbapi/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)     1216 2023-04-27 15:40:43.000000 dbt-glue-1.5.3/dbt/adapters/glue/gluedbapi/commons.py
--rw-r--r--   0 menuetb    (504) staff       (20)     9946 2023-07-17 09:33:44.000000 dbt-glue-1.5.3/dbt/adapters/glue/gluedbapi/connection.py
--rw-r--r--   0 menuetb    (504) staff       (20)     8225 2023-07-05 15:09:54.000000 dbt-glue-1.5.3/dbt/adapters/glue/gluedbapi/cursor.py
--rw-r--r--   0 menuetb    (504) staff       (20)    38602 2023-07-17 09:33:44.000000 dbt-glue-1.5.3/dbt/adapters/glue/impl.py
--rw-r--r--   0 menuetb    (504) staff       (20)     1264 2023-04-07 07:53:59.000000 dbt-glue-1.5.3/dbt/adapters/glue/relation.py
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.118709 dbt-glue-1.5.3/dbt/include/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.123015 dbt-glue-1.5.3/dbt/include/glue/
--rw-r--r--   0 menuetb    (504) staff       (20)       51 2022-04-05 16:42:41.000000 dbt-glue-1.5.3/dbt/include/glue/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)       72 2022-07-11 06:48:28.000000 dbt-glue-1.5.3/dbt/include/glue/dbt_project.yml
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.123253 dbt-glue-1.5.3/dbt/include/glue/macros/
--rw-r--r--   0 menuetb    (504) staff       (20)     5352 2023-01-17 10:30:07.000000 dbt-glue-1.5.3/dbt/include/glue/macros/adapters.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.123708 dbt-glue-1.5.3/dbt/include/glue/macros/generic_test_sql/
--rw-r--r--   0 menuetb    (504) staff       (20)      494 2022-07-11 06:48:28.000000 dbt-glue-1.5.3/dbt/include/glue/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      370 2022-07-11 06:48:28.000000 dbt-glue-1.5.3/dbt/include/glue/macros/generic_test_sql/relationships.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.124302 dbt-glue-1.5.3/dbt/include/glue/macros/materializations/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.124611 dbt-glue-1.5.3/dbt/include/glue/macros/materializations/incremental/
--rw-r--r--   0 menuetb    (504) staff       (20)     4453 2023-07-17 09:33:44.000000 dbt-glue-1.5.3/dbt/include/glue/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 menuetb    (504) staff       (20)     1689 2023-07-05 12:59:31.000000 dbt-glue-1.5.3/dbt/include/glue/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 menuetb    (504) staff       (20)     1436 2023-01-06 16:44:08.000000 dbt-glue-1.5.3/dbt/include/glue/macros/materializations/seed.sql
--rw-r--r--   0 menuetb    (504) staff       (20)    10334 2023-06-29 09:23:22.000000 dbt-glue-1.5.3/dbt/include/glue/macros/materializations/snapshot.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.124867 dbt-glue-1.5.3/dbt/include/glue/macros/materializations/table/
--rw-r--r--   0 menuetb    (504) staff       (20)     1159 2022-11-03 13:40:21.000000 dbt-glue-1.5.3/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      112 2022-07-11 06:48:28.000000 dbt-glue-1.5.3/dbt/include/glue/macros/materializations/view.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      584 2023-06-15 08:24:37.000000 dbt-glue-1.5.3/dbt/include/glue/sample_profiles.yml
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.119310 dbt-glue-1.5.3/dbt/include/glue/tests/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.125028 dbt-glue-1.5.3/dbt/include/glue/tests/generic/
--rw-r--r--   0 menuetb    (504) staff       (20)      290 2022-07-11 06:48:28.000000 dbt-glue-1.5.3/dbt/include/glue/tests/generic/builtin.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-17 09:35:23.125943 dbt-glue-1.5.3/dbt_glue.egg-info/
--rw-r--r--   0 menuetb    (504) staff       (20)    44977 2023-07-17 09:35:23.000000 dbt-glue-1.5.3/dbt_glue.egg-info/PKG-INFO
--rw-r--r--   0 menuetb    (504) staff       (20)     1230 2023-07-17 09:35:23.000000 dbt-glue-1.5.3/dbt_glue.egg-info/SOURCES.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        1 2023-07-17 09:35:23.000000 dbt-glue-1.5.3/dbt_glue.egg-info/dependency_links.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        1 2022-05-12 16:43:26.000000 dbt-glue-1.5.3/dbt_glue.egg-info/not-zip-safe
--rw-r--r--   0 menuetb    (504) staff       (20)       46 2023-07-17 09:35:23.000000 dbt-glue-1.5.3/dbt_glue.egg-info/requires.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        4 2023-07-17 09:35:23.000000 dbt-glue-1.5.3/dbt_glue.egg-info/top_level.txt
--rw-r--r--   0 menuetb    (504) staff       (20)       38 2023-07-17 09:35:23.126430 dbt-glue-1.5.3/setup.cfg
--rw-r--r--   0 menuetb    (504) staff       (20)     2857 2023-06-29 08:57:00.000000 dbt-glue-1.5.3/setup.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-08-01 11:13:14.533526 dbt-glue-1.6.0/
+-rw-r--r--   0 menuetb    (504) staff       (20)    10142 2022-04-05 16:42:41.000000 dbt-glue-1.6.0/LICENSE
+-rw-r--r--   0 menuetb    (504) staff       (20)       67 2022-04-05 16:42:41.000000 dbt-glue-1.6.0/NOTICE
+-rw-r--r--   0 menuetb    (504) staff       (20)    50814 2023-08-01 11:13:14.533342 dbt-glue-1.6.0/PKG-INFO
+-rw-r--r--   0 menuetb    (504) staff       (20)    49963 2023-08-01 11:11:00.000000 dbt-glue-1.6.0/README.md
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-08-01 11:13:14.523718 dbt-glue-1.6.0/dbt/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-08-01 11:13:14.523521 dbt-glue-1.6.0/dbt/adapters/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-08-01 11:13:14.527747 dbt-glue-1.6.0/dbt/adapters/glue/
+-rw-r--r--   0 menuetb    (504) staff       (20)      394 2023-04-06 15:48:24.000000 dbt-glue-1.6.0/dbt/adapters/glue/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)       17 2023-08-01 11:11:21.000000 dbt-glue-1.6.0/dbt/adapters/glue/__version__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     3917 2023-06-29 08:34:49.000000 dbt-glue-1.6.0/dbt/adapters/glue/connections.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     2609 2023-08-01 11:11:00.000000 dbt-glue-1.6.0/dbt/adapters/glue/credentials.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-08-01 11:13:14.528834 dbt-glue-1.6.0/dbt/adapters/glue/gluedbapi/
+-rw-r--r--   0 menuetb    (504) staff       (20)      140 2022-04-05 16:42:41.000000 dbt-glue-1.6.0/dbt/adapters/glue/gluedbapi/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     1216 2023-04-27 15:40:43.000000 dbt-glue-1.6.0/dbt/adapters/glue/gluedbapi/commons.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     9946 2023-07-17 09:33:44.000000 dbt-glue-1.6.0/dbt/adapters/glue/gluedbapi/connection.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     8225 2023-07-05 15:09:54.000000 dbt-glue-1.6.0/dbt/adapters/glue/gluedbapi/cursor.py
+-rw-r--r--   0 menuetb    (504) staff       (20)    40011 2023-08-01 11:11:00.000000 dbt-glue-1.6.0/dbt/adapters/glue/impl.py
+-rw-r--r--   0 menuetb    (504) staff       (20)    13710 2023-08-01 11:11:00.000000 dbt-glue-1.6.0/dbt/adapters/glue/lakeformation.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     1264 2023-04-07 07:53:59.000000 dbt-glue-1.6.0/dbt/adapters/glue/relation.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-08-01 11:13:14.523785 dbt-glue-1.6.0/dbt/include/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-08-01 11:13:14.529642 dbt-glue-1.6.0/dbt/include/glue/
+-rw-r--r--   0 menuetb    (504) staff       (20)       51 2022-04-05 16:42:41.000000 dbt-glue-1.6.0/dbt/include/glue/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)       72 2022-07-11 06:48:28.000000 dbt-glue-1.6.0/dbt/include/glue/dbt_project.yml
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-08-01 11:13:14.529915 dbt-glue-1.6.0/dbt/include/glue/macros/
+-rw-r--r--   0 menuetb    (504) staff       (20)     7268 2023-08-01 11:11:00.000000 dbt-glue-1.6.0/dbt/include/glue/macros/adapters.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-08-01 11:13:14.530294 dbt-glue-1.6.0/dbt/include/glue/macros/generic_test_sql/
+-rw-r--r--   0 menuetb    (504) staff       (20)      494 2022-07-11 06:48:28.000000 dbt-glue-1.6.0/dbt/include/glue/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      370 2022-07-11 06:48:28.000000 dbt-glue-1.6.0/dbt/include/glue/macros/generic_test_sql/relationships.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-08-01 11:13:14.530880 dbt-glue-1.6.0/dbt/include/glue/macros/materializations/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-08-01 11:13:14.531252 dbt-glue-1.6.0/dbt/include/glue/macros/materializations/incremental/
+-rw-r--r--   0 menuetb    (504) staff       (20)     4786 2023-08-01 11:11:00.000000 dbt-glue-1.6.0/dbt/include/glue/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)     1689 2023-07-05 12:59:31.000000 dbt-glue-1.6.0/dbt/include/glue/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)     1770 2023-08-01 11:11:00.000000 dbt-glue-1.6.0/dbt/include/glue/macros/materializations/seed.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)    10542 2023-08-01 11:12:10.000000 dbt-glue-1.6.0/dbt/include/glue/macros/materializations/snapshot.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-08-01 11:13:14.531710 dbt-glue-1.6.0/dbt/include/glue/macros/materializations/table/
+-rw-r--r--   0 menuetb    (504) staff       (20)     1496 2023-08-01 11:11:00.000000 dbt-glue-1.6.0/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)     4414 2023-08-01 11:11:00.000000 dbt-glue-1.6.0/dbt/include/glue/macros/materializations/table/table.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      112 2022-07-11 06:48:28.000000 dbt-glue-1.6.0/dbt/include/glue/macros/materializations/view.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      584 2023-06-15 08:24:37.000000 dbt-glue-1.6.0/dbt/include/glue/sample_profiles.yml
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-08-01 11:13:14.524360 dbt-glue-1.6.0/dbt/include/glue/tests/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-08-01 11:13:14.531880 dbt-glue-1.6.0/dbt/include/glue/tests/generic/
+-rw-r--r--   0 menuetb    (504) staff       (20)      290 2022-07-11 06:48:28.000000 dbt-glue-1.6.0/dbt/include/glue/tests/generic/builtin.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-08-01 11:13:14.532887 dbt-glue-1.6.0/dbt_glue.egg-info/
+-rw-r--r--   0 menuetb    (504) staff       (20)    50814 2023-08-01 11:13:14.000000 dbt-glue-1.6.0/dbt_glue.egg-info/PKG-INFO
+-rw-r--r--   0 menuetb    (504) staff       (20)     1322 2023-08-01 11:13:14.000000 dbt-glue-1.6.0/dbt_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        1 2023-08-01 11:13:14.000000 dbt-glue-1.6.0/dbt_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        1 2022-05-12 16:43:26.000000 dbt-glue-1.6.0/dbt_glue.egg-info/not-zip-safe
+-rw-r--r--   0 menuetb    (504) staff       (20)       46 2023-08-01 11:13:14.000000 dbt-glue-1.6.0/dbt_glue.egg-info/requires.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        4 2023-08-01 11:13:14.000000 dbt-glue-1.6.0/dbt_glue.egg-info/top_level.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)       38 2023-08-01 11:13:14.533583 dbt-glue-1.6.0/setup.cfg
+-rw-r--r--   0 menuetb    (504) staff       (20)     2857 2023-08-01 11:11:12.000000 dbt-glue-1.6.0/setup.py
```

### Comparing `dbt-glue-1.5.3/LICENSE` & `dbt-glue-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.3/PKG-INFO` & `dbt-glue-1.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: dbt-glue
-Version: 1.5.3
-Summary: dbt (data build tool) adapter for Aws Glue
-Home-page: https://github.com/aws-samples/dbt-glue
-Author: moshirm,menuetb,mamallem,segnina
-Author-email: moshirm@amazon.fr, menuetb@amazon.fr, mamallem@amazon.fr, segnina@amazon.fr 
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: NOTICE
-
 <p align="center">
   <img src="/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
 
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications.
 dbt is the T in ELT. Organize, cleanse, denormalize, filter, rename, and pre-aggregate the raw data in your warehouse so that it's ready for analysis.
 
@@ -99,15 +78,24 @@
                 "glue:CreateDatabase",
                 "glue:BatchDeleteTableVersion",
                 "glue:BatchDeleteTable",
                 "glue:DeletePartition",
                 "glue:GetUserDefinedFunctions",
                 "lakeformation:ListResources",
                 "lakeformation:BatchGrantPermissions",
-                "lakeformation:ListPermissions"
+                "lakeformation:ListPermissions", 
+                "lakeformation:GetDataAccess",
+                "lakeformation:GrantPermissions",
+                "lakeformation:RevokePermissions",
+                "lakeformation:BatchRevokePermissions",
+                "lakeformation:AddLFTagsToResource",
+                "lakeformation:RemoveLFTagsFromResource",
+                "lakeformation:GetResourceLFTags",
+                "lakeformation:ListLFTags",
+                "lakeformation:GetLFTag",
             ],
             "Resource": [
                 "arn:aws:glue:<region>:<AWS Account>:catalog",
                 "arn:aws:glue:<region>:<AWS Account>:table/<dbt output database>/*",
                 "arn:aws:glue:<region>:<AWS Account>:database/<dbt output database>"
             ],
             "Effect": "Allow"
@@ -840,14 +828,139 @@
 `database` to exist at a higher level than `schema`. As such, you should _never_
 use or set `database` as a node config or in the target profile when running dbt-glue.
 
 If you want to control the schema/database in which dbt will materialize models,
 use the `schema` config and `generate_schema_name` macro _only_.
 For more information, check the dbt documentation about [custom schemas](https://docs.getdbt.com/docs/build/custom-schemas).
 
+## AWS Lakeformation integration
+The adapter supports AWS Lakeformation tags management enabling you to associate existing tags defined out of dbt-glue to database objects built by dbt-glue (table, view, snapshot, incremental models, seeds).
+
+- You can enable or disable lf-tags management via config, at model and dbt-project level (disabled by default)
+- If enabled, lf-tags will be updated on every dbt run. There are table level lf-tags configs and column-level lf-tags configs. 
+- You can specify that you want to drop existing table lf-tags or column lf-tags by setting the drop_existing config field to True (False by default, meaning existing tags are kept)
+- Please note that if the tag you want to associate with the table does not exist, the dbt-glue execution will throw an error
+- dbt-glue does not manage database-level lf-tags, meaning :
+  - you can't associate database lf-tags within dbt-glue
+  - if the table inherits from a database lf-tags defined outside of dbt, dbt-glue does not drop this tag.
+
+The adapter also supports AWS Lakeformation data cell filtering. 
+- You can enable or disable data-cell filtering via config, at model and dbt-project level (disabled by default)
+- If enabled, data_cell_filters will be updated on every dbt run.
+- You can specify that you want to drop existing table data-cell filters by setting the drop_existing config field to True (False by default, meaning existing filters are kept)
+- You can leverage excluded_columns_names **OR** columns config fields to perform Column level security as well. **Please note that you can use one or the other but not both**.
+- By default, if you don't specify any column or excluded_columns, dbt-glue does not perform Column level filtering and let the principal access all the columns.
+
+The below configuration let the specified principal (lf-data-scientist IAM user) access rows that have a customer_lifetime_value > 15 and all the columns specified ('customer_id', 'first_order', 'most_recent_order', 'number_of_orders')
+
+```sql
+lf_grants={
+        'data_cell_filters': {
+            'enabled': True,
+            'drop_existing' : True,
+            'filters': {
+                'the_name_of_my_filter': {
+                    'row_filter': 'customer_lifetime_value>15',
+                    'principals': ['arn:aws:iam::123456789:user/lf-data-scientist'], 
+                    'column_names': ['customer_id', 'first_order', 'most_recent_order', 'number_of_orders']
+                }
+            }, 
+        }
+    }
+```
+The below configuration let the specified principal (lf-data-scientist IAM user) access rows that have a customer_lifetime_value > 15 and all the columns *except* the one specified ('first_name')
+
+```sql
+lf_grants={
+        'data_cell_filters': {
+            'enabled': True,
+            'drop_existing' : True,
+            'filters': {
+                'the_name_of_my_filter': {
+                    'row_filter': 'customer_lifetime_value>15',
+                    'principals': ['arn:aws:iam::123456789:user/lf-data-scientist'], 
+                    'excluded_column_names': ['first_name']
+                }
+            }, 
+        }
+    }
+```
+
+See below some examples of how you can integrate LF Tags management and data cell filtering to your configurations : 
+
+#### At model level
+This way of defining your Lakeformation rules is appropriate if you want to handle the tagging and filtering policy at object level. Remember that it overrides any configuration defined at dbt-project level. 
+
+```sql
+{{ config(
+    materialized='incremental',
+    unique_key="customer_id",
+    incremental_strategy='append',
+    lf_tags_config={
+          'enabled': true,
+          'drop_existing' : False,
+          'tags': 
+          {
+            'name_of_my_lf_tag': 'value_of_my_tag'          
+            }, 
+          'tags_columns': {
+            'name_of_my_lf_tag': {
+              'value_of_my_tag': ['customer_id', 'customer_lifetime_value', 'dt']
+            }}},
+    lf_grants={
+        'data_cell_filters': {
+            'enabled': True,
+            'drop_existing' : True,
+            'filters': {
+                'the_name_of_my_filter': {
+                    'row_filter': 'customer_lifetime_value>15',
+                    'principals': ['arn:aws:iam::123456789:user/lf-data-scientist'], 
+                    'excluded_column_names': ['first_name']
+                }
+            }, 
+        }
+    }
+) }}
+
+    select
+        customers.customer_id,
+        customers.first_name,
+        customers.last_name,
+        customer_orders.first_order,
+        customer_orders.most_recent_order,
+        customer_orders.number_of_orders,
+        customer_payments.total_amount as customer_lifetime_value,
+        current_date() as dt
+        
+    from customers
+
+    left join customer_orders using (customer_id)
+
+    left join customer_payments using (customer_id)
+
+```
+
+#### At dbt-project level
+This way you can specify tags and data filtering policy for a particular path in your dbt project (eg. models, seeds, models/model_group1, etc.)
+This is especially useful for seeds, for which you can't define configuration in the file directly.
+
+```yml
+seeds:
+  +lf_tags_config:
+    enabled: true
+    tags: 
+      name_of_my_tag: 'value_of_my_tag'     
+models:
+  +lf_tags_config:
+    enabled: true
+    drop_existing: True
+    tags: 
+      name_of_my_tag: 'value_of_my_tag'
+```
+  
 ## Tests
 
 To perform a functional test:
 1. Install dev requirements:
 ```bash
 $ pip3 install -r dev-requirements.txt
 ```
```

### Comparing `dbt-glue-1.5.3/README.md` & `dbt-glue-1.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: dbt-glue
+Version: 1.6.0
+Summary: dbt (data build tool) adapter for Aws Glue
+Home-page: https://github.com/aws-samples/dbt-glue
+Author: moshirm,menuetb,mamallem,segnina
+Author-email: moshirm@amazon.fr, menuetb@amazon.fr, mamallem@amazon.fr, segnina@amazon.fr 
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: NOTICE
+
 <p align="center">
   <img src="/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
 
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications.
 dbt is the T in ELT. Organize, cleanse, denormalize, filter, rename, and pre-aggregate the raw data in your warehouse so that it's ready for analysis.
 
@@ -78,15 +99,24 @@
                 "glue:CreateDatabase",
                 "glue:BatchDeleteTableVersion",
                 "glue:BatchDeleteTable",
                 "glue:DeletePartition",
                 "glue:GetUserDefinedFunctions",
                 "lakeformation:ListResources",
                 "lakeformation:BatchGrantPermissions",
-                "lakeformation:ListPermissions"
+                "lakeformation:ListPermissions", 
+                "lakeformation:GetDataAccess",
+                "lakeformation:GrantPermissions",
+                "lakeformation:RevokePermissions",
+                "lakeformation:BatchRevokePermissions",
+                "lakeformation:AddLFTagsToResource",
+                "lakeformation:RemoveLFTagsFromResource",
+                "lakeformation:GetResourceLFTags",
+                "lakeformation:ListLFTags",
+                "lakeformation:GetLFTag",
             ],
             "Resource": [
                 "arn:aws:glue:<region>:<AWS Account>:catalog",
                 "arn:aws:glue:<region>:<AWS Account>:table/<dbt output database>/*",
                 "arn:aws:glue:<region>:<AWS Account>:database/<dbt output database>"
             ],
             "Effect": "Allow"
@@ -819,14 +849,139 @@
 `database` to exist at a higher level than `schema`. As such, you should _never_
 use or set `database` as a node config or in the target profile when running dbt-glue.
 
 If you want to control the schema/database in which dbt will materialize models,
 use the `schema` config and `generate_schema_name` macro _only_.
 For more information, check the dbt documentation about [custom schemas](https://docs.getdbt.com/docs/build/custom-schemas).
 
+## AWS Lakeformation integration
+The adapter supports AWS Lakeformation tags management enabling you to associate existing tags defined out of dbt-glue to database objects built by dbt-glue (table, view, snapshot, incremental models, seeds).
+
+- You can enable or disable lf-tags management via config, at model and dbt-project level (disabled by default)
+- If enabled, lf-tags will be updated on every dbt run. There are table level lf-tags configs and column-level lf-tags configs. 
+- You can specify that you want to drop existing table lf-tags or column lf-tags by setting the drop_existing config field to True (False by default, meaning existing tags are kept)
+- Please note that if the tag you want to associate with the table does not exist, the dbt-glue execution will throw an error
+- dbt-glue does not manage database-level lf-tags, meaning :
+  - you can't associate database lf-tags within dbt-glue
+  - if the table inherits from a database lf-tags defined outside of dbt, dbt-glue does not drop this tag.
+
+The adapter also supports AWS Lakeformation data cell filtering. 
+- You can enable or disable data-cell filtering via config, at model and dbt-project level (disabled by default)
+- If enabled, data_cell_filters will be updated on every dbt run.
+- You can specify that you want to drop existing table data-cell filters by setting the drop_existing config field to True (False by default, meaning existing filters are kept)
+- You can leverage excluded_columns_names **OR** columns config fields to perform Column level security as well. **Please note that you can use one or the other but not both**.
+- By default, if you don't specify any column or excluded_columns, dbt-glue does not perform Column level filtering and let the principal access all the columns.
+
+The below configuration let the specified principal (lf-data-scientist IAM user) access rows that have a customer_lifetime_value > 15 and all the columns specified ('customer_id', 'first_order', 'most_recent_order', 'number_of_orders')
+
+```sql
+lf_grants={
+        'data_cell_filters': {
+            'enabled': True,
+            'drop_existing' : True,
+            'filters': {
+                'the_name_of_my_filter': {
+                    'row_filter': 'customer_lifetime_value>15',
+                    'principals': ['arn:aws:iam::123456789:user/lf-data-scientist'], 
+                    'column_names': ['customer_id', 'first_order', 'most_recent_order', 'number_of_orders']
+                }
+            }, 
+        }
+    }
+```
+The below configuration let the specified principal (lf-data-scientist IAM user) access rows that have a customer_lifetime_value > 15 and all the columns *except* the one specified ('first_name')
+
+```sql
+lf_grants={
+        'data_cell_filters': {
+            'enabled': True,
+            'drop_existing' : True,
+            'filters': {
+                'the_name_of_my_filter': {
+                    'row_filter': 'customer_lifetime_value>15',
+                    'principals': ['arn:aws:iam::123456789:user/lf-data-scientist'], 
+                    'excluded_column_names': ['first_name']
+                }
+            }, 
+        }
+    }
+```
+
+See below some examples of how you can integrate LF Tags management and data cell filtering to your configurations : 
+
+#### At model level
+This way of defining your Lakeformation rules is appropriate if you want to handle the tagging and filtering policy at object level. Remember that it overrides any configuration defined at dbt-project level. 
+
+```sql
+{{ config(
+    materialized='incremental',
+    unique_key="customer_id",
+    incremental_strategy='append',
+    lf_tags_config={
+          'enabled': true,
+          'drop_existing' : False,
+          'tags': 
+          {
+            'name_of_my_lf_tag': 'value_of_my_tag'          
+            }, 
+          'tags_columns': {
+            'name_of_my_lf_tag': {
+              'value_of_my_tag': ['customer_id', 'customer_lifetime_value', 'dt']
+            }}},
+    lf_grants={
+        'data_cell_filters': {
+            'enabled': True,
+            'drop_existing' : True,
+            'filters': {
+                'the_name_of_my_filter': {
+                    'row_filter': 'customer_lifetime_value>15',
+                    'principals': ['arn:aws:iam::123456789:user/lf-data-scientist'], 
+                    'excluded_column_names': ['first_name']
+                }
+            }, 
+        }
+    }
+) }}
+
+    select
+        customers.customer_id,
+        customers.first_name,
+        customers.last_name,
+        customer_orders.first_order,
+        customer_orders.most_recent_order,
+        customer_orders.number_of_orders,
+        customer_payments.total_amount as customer_lifetime_value,
+        current_date() as dt
+        
+    from customers
+
+    left join customer_orders using (customer_id)
+
+    left join customer_payments using (customer_id)
+
+```
+
+#### At dbt-project level
+This way you can specify tags and data filtering policy for a particular path in your dbt project (eg. models, seeds, models/model_group1, etc.)
+This is especially useful for seeds, for which you can't define configuration in the file directly.
+
+```yml
+seeds:
+  +lf_tags_config:
+    enabled: true
+    tags: 
+      name_of_my_tag: 'value_of_my_tag'     
+models:
+  +lf_tags_config:
+    enabled: true
+    drop_existing: True
+    tags: 
+      name_of_my_tag: 'value_of_my_tag'
+```
+  
 ## Tests
 
 To perform a functional test:
 1. Install dev requirements:
 ```bash
 $ pip3 install -r dev-requirements.txt
 ```
```

### Comparing `dbt-glue-1.5.3/dbt/adapters/glue/connections.py` & `dbt-glue-1.6.0/dbt/adapters/glue/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.3/dbt/adapters/glue/credentials.py` & `dbt-glue-1.6.0/dbt/adapters/glue/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,9 +74,10 @@
             'conf',
             'extra_py_files',
             'delta_athena_prefix',
             'tags',
             'seed_format',
             'seed_mode',
             'default_arguments', 
-            'iceberg_glue_commit_lock_table'
+            'iceberg_glue_commit_lock_table', 
+            'lf_tags'
         ]
```

### Comparing `dbt-glue-1.5.3/dbt/adapters/glue/gluedbapi/commons.py` & `dbt-glue-1.6.0/dbt/adapters/glue/gluedbapi/commons.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.3/dbt/adapters/glue/gluedbapi/connection.py` & `dbt-glue-1.6.0/dbt/adapters/glue/gluedbapi/connection.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.3/dbt/adapters/glue/gluedbapi/cursor.py` & `dbt-glue-1.6.0/dbt/adapters/glue/gluedbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.3/dbt/adapters/glue/impl.py` & `dbt-glue-1.6.0/dbt/adapters/glue/impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 import io
 import os
 import re
 import uuid
 import boto3
-from typing import List
+from typing import Dict, List, Any
 
 import dbt
 import agate
 from concurrent.futures import Future
 
 from dbt.adapters.base import available
 from dbt.adapters.base.relation import BaseRelation
 from dbt.adapters.base.column import Column
 from dbt.adapters.sql import SQLAdapter
 from dbt.adapters.glue import GlueConnectionManager
 from dbt.adapters.glue.gluedbapi import GlueConnection
 from dbt.adapters.glue.relation import SparkRelation
+from dbt.adapters.glue.lakeformation import (
+    LfGrantsConfig,
+    LfPermissions,
+    LfTagsConfig,
+    LfTagsManager,
+)
 from dbt.exceptions import DbtDatabaseError
 from dbt.adapters.base.impl import catch_as_completed
 from dbt.utils import executor
 from dbt.events import AdapterLogger
 
 logger = AdapterLogger("Glue")
 
@@ -891,15 +897,41 @@
             """)
         try:
             session.cursor().execute(code)
         except DbtDatabaseError as e:
             raise DbtDatabaseError(msg="GlueIcebergExpireSnapshotsFailed") from e
         except Exception as e:
             logger.error(e)
-
+    
+    @available
+    def add_lf_tags(self, relation: SparkRelation, lf_tags_config: Dict[str, Any]) -> None:
+        config = LfTagsConfig(**lf_tags_config)
+        if config.enabled:
+            conn = self.connections.get_thread_connection()
+            client = conn.handle
+            lf = boto3.client("lakeformation", region_name=client.credentials.region)
+            manager = LfTagsManager(lf, relation, config)
+            manager.process_lf_tags()
+            return
+        logger.debug(f"Lakeformation is disabled for {relation}")
+
+    @available
+    def apply_lf_grants(self, relation: SparkRelation, lf_grants_config: Dict[str, Any]) -> None:
+        lf_config = LfGrantsConfig(**lf_grants_config)
+        if lf_config.data_cell_filters.enabled:
+            conn = self.connections.get_thread_connection()
+            client = conn.handle
+            lf = boto3.client("lakeformation", region_name=client.credentials.region)
+            sts = boto3.client("sts")
+            identity = sts.get_caller_identity()
+            account = identity.get("Account")
+            lf_permissions = LfPermissions(account, relation, lf)  # type: ignore
+            lf_permissions.process_filters(lf_config)
+            lf_permissions.process_permissions(lf_config)
+    
     @available
     def execute_pyspark(self, codeblock):
         session, client = self.get_connection()
 
         code = f"""
 custom_glue_code_for_dbt_adapter
 {codeblock}
```

### Comparing `dbt-glue-1.5.3/dbt/adapters/glue/relation.py` & `dbt-glue-1.6.0/dbt/adapters/glue/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.3/dbt/include/glue/macros/adapters.sql` & `dbt-glue-1.6.0/dbt/include/glue/macros/adapters.sql`

 * *Files 19% similar despite different names*

```diff
@@ -126,17 +126,25 @@
     dbt_next_query
     create view {{ relation }}
         as
     {{ sql }}
 {% endmacro %}
 
 {% macro glue__create_view(relation, sql) -%}
+  {%- set lf_tags_config = config.get('lf_tags_config') -%}
+  {%- set lf_grants = config.get('lf_grants') -%}
   {% call statement("create_view(", fetch_result=false, auto_begin=false) %}
     {{ create_view_as(relation, sql) }}
   {% endcall %}
+  {% if lf_tags_config is not none %}
+    {{ adapter.add_lf_tags(target_relation, lf_tags_config) }}
+  {% endif %}
+  {% if lf_grants is not none %}
+    {{ adapter.apply_lf_grants(target_relation, lf_grants) }}
+  {% endif %}
 {% endmacro %}
 
 {% macro glue_exec_query(sql) %}
   {% call statement("run_query_statement", fetch_result=false, auto_begin=false) %}
     {{ sql }}
   {% endcall %}
 {% endmacro %}
@@ -156,7 +164,47 @@
   {% if table_properties_formatted|length > 0 %}
   	{%- set table_properties_csv= table_properties_formatted | join(', ') -%}
 		TBLPROPERTIES (
 			{{table_properties_csv}}
 		)
   {%- endif %}
 {%- endmacro %}
+
+{% macro create_or_replace_view() %}
+  {%- set identifier = model['alias'] -%}
+
+  {%- set old_relation = adapter.get_relation(database=database, schema=schema, identifier=identifier) -%}
+  {%- set exists_as_view = (old_relation is not none and old_relation.is_view) -%}
+  {%- set lf_tags_config = config.get('lf_tags_config') -%}
+  {%- set lf_grants = config.get('lf_grants') -%}
+  {%- set target_relation = api.Relation.create(
+      identifier=identifier, schema=schema, database=database,
+      type='view') -%}
+  {% set grant_config = config.get('grants') %}
+
+  {{ run_hooks(pre_hooks) }}
+
+  -- If there's a table with the same name and we weren't told to full refresh,
+  -- that's an error. If we were told to full refresh, drop it. This behavior differs
+  -- for Snowflake and BigQuery, so multiple dispatch is used.
+  {%- if old_relation is not none and old_relation.is_table -%}
+    {{ handle_existing_table(should_full_refresh(), old_relation) }}
+  {%- endif -%}
+
+  -- build model
+  {% call statement('main') -%}
+    {{ get_create_view_as_sql(target_relation, sql) }}
+  {%- endcall %}
+
+  {% set should_revoke = should_revoke(exists_as_view, full_refresh_mode=True) %}
+  {% do apply_grants(target_relation, grant_config, should_revoke=should_revoke) %}
+  {% if lf_tags_config is not none %}
+    {{ adapter.add_lf_tags(target_relation, lf_tags_config) }}
+  {% endif %}
+  {% if lf_grants is not none %}
+    {{ adapter.apply_lf_grants(target_relation, lf_grants) }}
+  {% endif %}
+  {{ run_hooks(post_hooks) }}
+
+  {{ return({'relations': [target_relation]}) }}
+
+{% endmacro %}
```

### Comparing `dbt-glue-1.5.3/dbt/include/glue/macros/materializations/incremental/incremental.sql` & `dbt-glue-1.6.0/dbt/include/glue/macros/materializations/incremental/incremental.sql`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,16 @@
   {%- set full_refresh_config = config.get('full_refresh', default=False) -%}
   {%- set full_refresh_mode = (flags.FULL_REFRESH == 'True' or full_refresh_config == 'True') -%}
 
   {% set target_relation = this %}
   {% set existing_relation_type = adapter.get_table_type(target_relation)  %}
   {% set tmp_relation = make_temp_relation(target_relation, '_tmp') %}
   {% set is_incremental = 'False' %}
-
+  {% set lf_tags_config = config.get('lf_tags_config') %}
+  {% set lf_grants = config.get('lf_grants') %}
   {% call statement() %}
     set spark.sql.autoBroadcastJoinThreshold=-1
   {% endcall %}
 
   {{ run_hooks(pre_hooks) }}
   {%- set substitute_variables = config.get('substitute_variables', default=[]) -%}
 
@@ -76,14 +77,22 @@
 
   {%- call statement('main') -%}
      {{ build_sql }}
   {%- endcall -%}
 
   {{ run_hooks(post_hooks) }}
 
+  {% if lf_tags_config is not none %}
+    {{ adapter.add_lf_tags(target_relation, lf_tags_config) }}
+  {% endif %}
+
+  {% if lf_grants is not none %}
+    {{ adapter.apply_lf_grants(target_relation, lf_grants) }}
+  {% endif %}
+  
   {% if is_incremental == 'True' %}
     {{ glue__drop_relation(tmp_relation) }}
     {% if file_format == 'delta' %}
         {{ adapter.delta_update_manifest(target_relation, custom_location) }}
     {% endif %}
   {% endif %}
```

### Comparing `dbt-glue-1.5.3/dbt/include/glue/macros/materializations/incremental/strategies.sql` & `dbt-glue-1.6.0/dbt/include/glue/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.3/dbt/include/glue/macros/materializations/seed.sql` & `dbt-glue-1.6.0/dbt/include/glue/macros/materializations/seed.sql`

 * *Files 27% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 {% materialization seed, adapter='glue' %}
 
   {%- set identifier = model['alias'] -%}
   {%- set old_relation = adapter.get_relation(database=database, schema=schema, identifier=identifier) -%}
   {%- set target_relation = api.Relation.create(database=database, schema=schema, identifier=identifier,
                                                type='table') -%}
   {%- set agate_table = load_agate_table() -%}
+  {%- set lf_tags_config = config.get('lf_tags_config') -%}
+  {%- set lf_grants = config.get('lf_grants') -%}
   {%- do store_result('agate_table', response='OK', agate_table=agate_table) -%}
 
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
 
   -- `BEGIN` happens here:
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
@@ -25,15 +27,21 @@
   {% set sql = load_csv_rows(model, agate_table) %}
 
   {% call noop_statement('main', status ~ ' ' ~ num_rows) %}
     {{ create_table_sql }}
     -- dbt seed --
     {{ sql }}
   {% endcall %}
-
+  {% if lf_tags_config is not none %}
+    {{ adapter.add_lf_tags(target_relation, lf_tags_config) }}
+  {% endif %}
+
+  {% if lf_grants is not none %}
+    {{ adapter.apply_lf_grants(target_relation, lf_grants) }}
+  {% endif %}
   {{ run_hooks(post_hooks, inside_transaction=True) }}
   -- `COMMIT` happens here
   {{ adapter.commit() }}
   {{ run_hooks(post_hooks, inside_transaction=False) }}
 
   {{ return({'relations': [target_relation]}) }}
```

### Comparing `dbt-glue-1.5.3/dbt/include/glue/macros/materializations/snapshot.sql` & `dbt-glue-1.6.0/dbt/include/glue/macros/materializations/snapshot.sql`

 * *Files 2% similar despite different names*

```diff
@@ -183,15 +183,16 @@
 
     {%- if file_format == 'hudi' -%}
       {%- set partition_by = None -%}
       {%- set custom_location = 'empty' -%}
       {%- set unique_key = 'dbt_scd_id' -%}
       {% set build_sql = build_snapshot_table(strategy, sql) %}
       {%- set hudi_options = config.get('hudi_options') -%}
-      {{ adapter.hudi_merge_table(target_relation, build_sql, unique_key, partition_by, custom_location, hudi_options) }}
+      {%- set substitute_variables = config.get('substitute_variables', '[]') -%}
+      {{ adapter.hudi_merge_table(target_relation, build_sql, unique_key, partition_by, custom_location, hudi_options, substitute_variables) }}
       {% set final_sql = "select * from " + target_relation.schema + "." + target_relation.identifier %}
     {% elif file_format == 'iceberg'%}
       {%- set partition_by = None -%}
       {%- set custom_location = 'empty' -%}
       {%- set unique_key = 'dbt_scd_id' -%}
       {% set build_sql = build_snapshot_table(strategy, sql | replace("from ", "from glue_catalog.")) %}
       {{ adapter.iceberg_write(target_relation, build_sql, unique_key, partition_by, custom_location, 'insert_overwrite', table_properties) }}
@@ -232,15 +233,16 @@
 
     {%- if file_format == 'hudi' -%}
         {%- set partition_by = None -%}
         {%- set custom_location = 'empty' -%}
         {%- set build_sql = "select * from " + staging_table.schema + "." + staging_table.identifier -%}
         {%- set unique_key = 'dbt_scd_id' -%}
         {%- set hudi_options = config.get('hudi_options') -%}
-        {{ adapter.hudi_merge_table(target_relation, build_sql, unique_key, partition_by, custom_location, hudi_options) }}
+      {%- set substitute_variables = config.get('substitute_variables', '[]') -%}
+        {{ adapter.hudi_merge_table(target_relation, build_sql, unique_key, partition_by, custom_location, hudi_options, substitute_variables) }}
         {% set final_sql = "select * from " + target_relation.schema + "." + target_relation.identifier %}
       {% elif file_format == 'iceberg' %}
         {%- set partition_by = None -%}
         {%- set custom_location = 'empty' -%}
         {%- set build_sql = "select * from " + staging_table.schema + "." + staging_table.identifier -%}
         {%- set unique_key = 'dbt_scd_id' -%}
         {{ adapter.iceberg_write(target_relation, build_sql, unique_key, partition_by, custom_location, 'insert_overwrite', table_properties) }}
```

### Comparing `dbt-glue-1.5.3/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql` & `dbt-glue-1.6.0/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 {% materialization iceberg_table_replace, adapter='glue' -%}
   {%- set default_catalog = 'iceberg_catalog' -%}
   {%- set partition_by = config.get('partition_by', none) -%}
   {%- set expire_snapshots = config.get('expire_snapshots', default=true) -%}
   {%- set table_properties = config.get('table_properties', default={}) -%}
+  {% set lf_tags_config = config.get('lf_tags_config') -%}
+  {%- set lf_grants = config.get('lf_grants') -%}
   {%- set target_relation = this -%}
   {%- set build_sql = create_or_replace(default_catalog, target_relation, table_properties) -%}
 
 	{{ run_hooks(pre_hooks) }}
 
   {%- call statement('main') -%}
     {{ build_sql }}
   {%- endcall -%}
 
   {%- if expire_snapshots == true -%}
   	{%- set result = adapter.iceberg_expire_snapshots(default_catalog, target_relation) -%}
   {%- endif -%}
+  
+  {% if lf_tags_config is not none %}
+    {{ adapter.add_lf_tags(target_relation, lf_tags_config) }}
+  {% endif %}
+
+  {% if lf_grants is not none %}
+    {{ adapter.apply_lf_grants(target_relation, lf_grants) }}
+  {% endif %}
 
 	{{ run_hooks(post_hooks) }}
 
 	{{ return({'relations': [target_relation]}) }}
 
 {%- endmaterialization %}
```

### Comparing `dbt-glue-1.5.3/dbt/include/glue/sample_profiles.yml` & `dbt-glue-1.6.0/dbt/include/glue/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.3/dbt_glue.egg-info/PKG-INFO` & `dbt-glue-1.6.0/dbt_glue.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-glue
-Version: 1.5.3
+Version: 1.6.0
 Summary: dbt (data build tool) adapter for Aws Glue
 Home-page: https://github.com/aws-samples/dbt-glue
 Author: moshirm,menuetb,mamallem,segnina
 Author-email: moshirm@amazon.fr, menuetb@amazon.fr, mamallem@amazon.fr, segnina@amazon.fr 
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -99,15 +99,24 @@
                 "glue:CreateDatabase",
                 "glue:BatchDeleteTableVersion",
                 "glue:BatchDeleteTable",
                 "glue:DeletePartition",
                 "glue:GetUserDefinedFunctions",
                 "lakeformation:ListResources",
                 "lakeformation:BatchGrantPermissions",
-                "lakeformation:ListPermissions"
+                "lakeformation:ListPermissions", 
+                "lakeformation:GetDataAccess",
+                "lakeformation:GrantPermissions",
+                "lakeformation:RevokePermissions",
+                "lakeformation:BatchRevokePermissions",
+                "lakeformation:AddLFTagsToResource",
+                "lakeformation:RemoveLFTagsFromResource",
+                "lakeformation:GetResourceLFTags",
+                "lakeformation:ListLFTags",
+                "lakeformation:GetLFTag",
             ],
             "Resource": [
                 "arn:aws:glue:<region>:<AWS Account>:catalog",
                 "arn:aws:glue:<region>:<AWS Account>:table/<dbt output database>/*",
                 "arn:aws:glue:<region>:<AWS Account>:database/<dbt output database>"
             ],
             "Effect": "Allow"
@@ -840,14 +849,139 @@
 `database` to exist at a higher level than `schema`. As such, you should _never_
 use or set `database` as a node config or in the target profile when running dbt-glue.
 
 If you want to control the schema/database in which dbt will materialize models,
 use the `schema` config and `generate_schema_name` macro _only_.
 For more information, check the dbt documentation about [custom schemas](https://docs.getdbt.com/docs/build/custom-schemas).
 
+## AWS Lakeformation integration
+The adapter supports AWS Lakeformation tags management enabling you to associate existing tags defined out of dbt-glue to database objects built by dbt-glue (table, view, snapshot, incremental models, seeds).
+
+- You can enable or disable lf-tags management via config, at model and dbt-project level (disabled by default)
+- If enabled, lf-tags will be updated on every dbt run. There are table level lf-tags configs and column-level lf-tags configs. 
+- You can specify that you want to drop existing table lf-tags or column lf-tags by setting the drop_existing config field to True (False by default, meaning existing tags are kept)
+- Please note that if the tag you want to associate with the table does not exist, the dbt-glue execution will throw an error
+- dbt-glue does not manage database-level lf-tags, meaning :
+  - you can't associate database lf-tags within dbt-glue
+  - if the table inherits from a database lf-tags defined outside of dbt, dbt-glue does not drop this tag.
+
+The adapter also supports AWS Lakeformation data cell filtering. 
+- You can enable or disable data-cell filtering via config, at model and dbt-project level (disabled by default)
+- If enabled, data_cell_filters will be updated on every dbt run.
+- You can specify that you want to drop existing table data-cell filters by setting the drop_existing config field to True (False by default, meaning existing filters are kept)
+- You can leverage excluded_columns_names **OR** columns config fields to perform Column level security as well. **Please note that you can use one or the other but not both**.
+- By default, if you don't specify any column or excluded_columns, dbt-glue does not perform Column level filtering and let the principal access all the columns.
+
+The below configuration let the specified principal (lf-data-scientist IAM user) access rows that have a customer_lifetime_value > 15 and all the columns specified ('customer_id', 'first_order', 'most_recent_order', 'number_of_orders')
+
+```sql
+lf_grants={
+        'data_cell_filters': {
+            'enabled': True,
+            'drop_existing' : True,
+            'filters': {
+                'the_name_of_my_filter': {
+                    'row_filter': 'customer_lifetime_value>15',
+                    'principals': ['arn:aws:iam::123456789:user/lf-data-scientist'], 
+                    'column_names': ['customer_id', 'first_order', 'most_recent_order', 'number_of_orders']
+                }
+            }, 
+        }
+    }
+```
+The below configuration let the specified principal (lf-data-scientist IAM user) access rows that have a customer_lifetime_value > 15 and all the columns *except* the one specified ('first_name')
+
+```sql
+lf_grants={
+        'data_cell_filters': {
+            'enabled': True,
+            'drop_existing' : True,
+            'filters': {
+                'the_name_of_my_filter': {
+                    'row_filter': 'customer_lifetime_value>15',
+                    'principals': ['arn:aws:iam::123456789:user/lf-data-scientist'], 
+                    'excluded_column_names': ['first_name']
+                }
+            }, 
+        }
+    }
+```
+
+See below some examples of how you can integrate LF Tags management and data cell filtering to your configurations : 
+
+#### At model level
+This way of defining your Lakeformation rules is appropriate if you want to handle the tagging and filtering policy at object level. Remember that it overrides any configuration defined at dbt-project level. 
+
+```sql
+{{ config(
+    materialized='incremental',
+    unique_key="customer_id",
+    incremental_strategy='append',
+    lf_tags_config={
+          'enabled': true,
+          'drop_existing' : False,
+          'tags': 
+          {
+            'name_of_my_lf_tag': 'value_of_my_tag'          
+            }, 
+          'tags_columns': {
+            'name_of_my_lf_tag': {
+              'value_of_my_tag': ['customer_id', 'customer_lifetime_value', 'dt']
+            }}},
+    lf_grants={
+        'data_cell_filters': {
+            'enabled': True,
+            'drop_existing' : True,
+            'filters': {
+                'the_name_of_my_filter': {
+                    'row_filter': 'customer_lifetime_value>15',
+                    'principals': ['arn:aws:iam::123456789:user/lf-data-scientist'], 
+                    'excluded_column_names': ['first_name']
+                }
+            }, 
+        }
+    }
+) }}
+
+    select
+        customers.customer_id,
+        customers.first_name,
+        customers.last_name,
+        customer_orders.first_order,
+        customer_orders.most_recent_order,
+        customer_orders.number_of_orders,
+        customer_payments.total_amount as customer_lifetime_value,
+        current_date() as dt
+        
+    from customers
+
+    left join customer_orders using (customer_id)
+
+    left join customer_payments using (customer_id)
+
+```
+
+#### At dbt-project level
+This way you can specify tags and data filtering policy for a particular path in your dbt project (eg. models, seeds, models/model_group1, etc.)
+This is especially useful for seeds, for which you can't define configuration in the file directly.
+
+```yml
+seeds:
+  +lf_tags_config:
+    enabled: true
+    tags: 
+      name_of_my_tag: 'value_of_my_tag'     
+models:
+  +lf_tags_config:
+    enabled: true
+    drop_existing: True
+    tags: 
+      name_of_my_tag: 'value_of_my_tag'
+```
+  
 ## Tests
 
 To perform a functional test:
 1. Install dev requirements:
 ```bash
 $ pip3 install -r dev-requirements.txt
 ```
```

### Comparing `dbt-glue-1.5.3/dbt_glue.egg-info/SOURCES.txt` & `dbt-glue-1.6.0/dbt_glue.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 setup.py
 dbt/adapters/glue/__init__.py
 dbt/adapters/glue/__version__.py
 dbt/adapters/glue/connections.py
 dbt/adapters/glue/credentials.py
 dbt/adapters/glue/impl.py
+dbt/adapters/glue/lakeformation.py
 dbt/adapters/glue/relation.py
 dbt/adapters/glue/gluedbapi/__init__.py
 dbt/adapters/glue/gluedbapi/commons.py
 dbt/adapters/glue/gluedbapi/connection.py
 dbt/adapters/glue/gluedbapi/cursor.py
 dbt/include/glue/__init__.py
 dbt/include/glue/dbt_project.yml
@@ -20,14 +21,15 @@
 dbt/include/glue/macros/generic_test_sql/relationships.sql
 dbt/include/glue/macros/materializations/seed.sql
 dbt/include/glue/macros/materializations/snapshot.sql
 dbt/include/glue/macros/materializations/view.sql
 dbt/include/glue/macros/materializations/incremental/incremental.sql
 dbt/include/glue/macros/materializations/incremental/strategies.sql
 dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql
+dbt/include/glue/macros/materializations/table/table.sql
 dbt/include/glue/tests/generic/builtin.sql
 dbt_glue.egg-info/PKG-INFO
 dbt_glue.egg-info/SOURCES.txt
 dbt_glue.egg-info/dependency_links.txt
 dbt_glue.egg-info/not-zip-safe
 dbt_glue.egg-info/requires.txt
 dbt_glue.egg-info/top_level.txt
```

### Comparing `dbt-glue-1.5.3/setup.py` & `dbt-glue-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,16 @@
             return line.split(delim)[1]
     else:
         raise RuntimeError("Unable to find version string.")
 
 
 package_name = "dbt-glue"
 package_version = get_version("dbt/adapters/glue/__version__.py")
-dbt_version = "1.5.2"
-dbt_spark_version = "1.5.0"
+dbt_version = "1.6.0"
+dbt_spark_version = "1.6.0"
 description = """dbt (data build tool) adapter for Aws Glue"""
 long_description = read('README.md')
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=long_description,
```

