# Comparing `tmp/yetl-framework-2.0.5.dev1.tar.gz` & `tmp/yetl-framework-2.0.5.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-2.0.5.dev1.tar", last modified: Tue Aug  1 07:24:06 2023, max compression
+gzip compressed data, was "yetl-framework-2.0.5.dev2.tar", last modified: Tue Aug  1 08:25:22 2023, max compression
```

## Comparing `yetl-framework-2.0.5.dev1.tar` & `yetl-framework-2.0.5.dev2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 07:24:06.019963 yetl-framework-2.0.5.dev1/
--rw-r--r--   0 vsts      (1001) docker     (123)     1199 2023-08-01 07:24:06.019963 yetl-framework-2.0.5.dev1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-08-01 07:24:06.019963 yetl-framework-2.0.5.dev1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1544 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 07:24:06.011963 yetl-framework-2.0.5.dev1/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1764 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 07:24:06.011963 yetl-framework-2.0.5.dev1/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     3367 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 07:24:06.011963 yetl-framework-2.0.5.dev1/yetl/cli/metadata_provider/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/cli/metadata_provider/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17399 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/cli/metadata_provider/_xlsx.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 07:24:06.015963 yetl-framework-2.0.5.dev1/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4780 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2112 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9867 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5064 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18293 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 07:24:06.015963 yetl-framework-2.0.5.dev1/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5013 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6707 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4534 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 07:24:06.015963 yetl-framework-2.0.5.dev1/yetl/resource/
--rw-r--r--   0 vsts      (1001) docker     (123)      569 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/resource/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      299 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/resource/logging.yaml
--rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/resource/project.yaml
--rw-r--r--   0 vsts      (1001) docker     (123)    12636 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/resource/sibytes_yetl_pipeline_schema.json
--rw-r--r--   0 vsts      (1001) docker     (123)     2654 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/resource/sibytes_yetl_project_schema.json
--rw-r--r--   0 vsts      (1001) docker     (123)    14625 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/resource/sibytes_yetl_tables_schema.json
--rw-r--r--   0 vsts      (1001) docker     (123)    10012 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/resource/tables.xlsx
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 07:24:06.015963 yetl-framework-2.0.5.dev1/yetl/validation/
--rw-r--r--   0 vsts      (1001) docker     (123)      353 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/validation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1495 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/validation/_validate.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 07:24:06.015963 yetl-framework-2.0.5.dev1/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/workflow/_dlt.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-08-01 07:22:58.000000 yetl-framework-2.0.5.dev1/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 07:24:06.019963 yetl-framework-2.0.5.dev1/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     1199 2023-08-01 07:24:05.000000 yetl-framework-2.0.5.dev1/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1377 2023-08-01 07:24:05.000000 yetl-framework-2.0.5.dev1/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-01 07:24:05.000000 yetl-framework-2.0.5.dev1/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-01 07:24:05.000000 yetl-framework-2.0.5.dev1/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       76 2023-08-01 07:24:05.000000 yetl-framework-2.0.5.dev1/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-08-01 07:24:05.000000 yetl-framework-2.0.5.dev1/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 08:25:22.581145 yetl-framework-2.0.5.dev2/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1199 2023-08-01 08:25:22.581145 yetl-framework-2.0.5.dev2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-08-01 08:25:22.581145 yetl-framework-2.0.5.dev2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1544 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 08:25:22.573145 yetl-framework-2.0.5.dev2/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1764 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 08:25:22.573145 yetl-framework-2.0.5.dev2/yetl/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3367 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/cli/_init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 08:25:22.573145 yetl-framework-2.0.5.dev2/yetl/cli/metadata_provider/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/cli/metadata_provider/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17399 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/cli/metadata_provider/_xlsx.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 08:25:22.577145 yetl-framework-2.0.5.dev2/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4780 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2112 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9867 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5064 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19355 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 08:25:22.577145 yetl-framework-2.0.5.dev2/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5213 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6707 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4534 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 08:25:22.577145 yetl-framework-2.0.5.dev2/yetl/resource/
+-rw-r--r--   0 vsts      (1001) docker     (123)      569 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/resource/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      299 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/resource/logging.yaml
+-rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/resource/project.yaml
+-rw-r--r--   0 vsts      (1001) docker     (123)    12636 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/resource/sibytes_yetl_pipeline_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     2654 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/resource/sibytes_yetl_project_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    14625 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/resource/sibytes_yetl_tables_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    10012 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/resource/tables.xlsx
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 08:25:22.577145 yetl-framework-2.0.5.dev2/yetl/validation/
+-rw-r--r--   0 vsts      (1001) docker     (123)      353 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/validation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1495 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/validation/_validate.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 08:25:22.577145 yetl-framework-2.0.5.dev2/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/workflow/_dlt.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-08-01 08:24:11.000000 yetl-framework-2.0.5.dev2/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 08:25:22.581145 yetl-framework-2.0.5.dev2/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1199 2023-08-01 08:25:22.000000 yetl-framework-2.0.5.dev2/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1377 2023-08-01 08:25:22.000000 yetl-framework-2.0.5.dev2/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-01 08:25:22.000000 yetl-framework-2.0.5.dev2/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-01 08:25:22.000000 yetl-framework-2.0.5.dev2/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       76 2023-08-01 08:25:22.000000 yetl-framework-2.0.5.dev2/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-08-01 08:25:22.000000 yetl-framework-2.0.5.dev2/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-2.0.5.dev1/PKG-INFO` & `yetl-framework-2.0.5.dev2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 2.0.5.dev1
+Version: 2.0.5.dev2
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-2.0.5.dev1/README.md` & `yetl-framework-2.0.5.dev2/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/setup.py` & `yetl-framework-2.0.5.dev2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="2.0.5.dev1",
+    version="2.0.5.dev2",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-2.0.5.dev1/yetl/__main__.py` & `yetl-framework-2.0.5.dev2/yetl/__main__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/cli/_init.py` & `yetl-framework-2.0.5.dev2/yetl/cli/_init.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/cli/metadata_provider/_xlsx.py` & `yetl-framework-2.0.5.dev2/yetl/cli/metadata_provider/_xlsx.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/config/__init__.py` & `yetl-framework-2.0.5.dev2/yetl/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/config/_config.py` & `yetl-framework-2.0.5.dev2/yetl/config/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/config/_decorators.py` & `yetl-framework-2.0.5.dev2/yetl/config/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/config/_logging_config.py` & `yetl-framework-2.0.5.dev2/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/config/_project.py` & `yetl-framework-2.0.5.dev2/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/config/_spark_context.py` & `yetl-framework-2.0.5.dev2/yetl/config/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/config/_tables.py` & `yetl-framework-2.0.5.dev2/yetl/config/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/config/_timeslice.py` & `yetl-framework-2.0.5.dev2/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/config/_utils.py` & `yetl-framework-2.0.5.dev2/yetl/config/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/config/deltalake.py` & `yetl-framework-2.0.5.dev2/yetl/config/deltalake.py`

 * *Files 5% similar despite different names*

```diff
@@ -235,35 +235,36 @@
         return sql_properties
 
     def create_table(
         self,
         database: str,
         table: str,
         path: str = None,
-        delta_properties: List[str] = None,
+        delta_properties: Optional[List[str]] = None,
         sql: str = None,
         catalog: str = None,
+        schema: Optional[StructType] = None,
+        always_identity_column: Optional[str] = None,
+        partition_by: Optional[List[str]] = None,
+        cluster_by: Optional[List[str]] = None,
     ):
-        database = f"`{catalog}`.`{database}`" if catalog else f"`{database}`"
-        table = f"`{table}`"
-        self._logger.info(f"Creating table if not exists {database}.{table} at {path}")
-        if not sql:
-            sql = f"CREATE TABLE IF NOT EXISTS {database}.{table}"
 
-            # add in the delta properties if there are any
-            sql_properties = ""
-            if delta_properties:
-                sql_properties = self.get_delta_properties_sql(delta_properties)
-                sql_properties = f"TBLPROPERTIES({sql_properties})"
-
-            sql_path = ""
-            if path:
-                sql_path = f"USING DELTA LOCATION '{path}'"
-
-                sql = f"{sql}\n{sql_path}\n{sql_properties};"
+        self._logger.info(f"Creating table if not exists {catalog}.{database}.{table} at {path}")
+        if not sql:
+            sql = self.create_table_dll(
+                database=database,
+                table=table,
+                catalog=catalog,
+                schema=schema,
+                always_identity_column=always_identity_column,
+                partition_by=partition_by,
+                cluster_by=cluster_by,
+                delta_properties=delta_properties,
+                location=path,
+            )
 
         self._logger.info(f"{sql}")
         self.spark.sql(sql)
 
         return sql
 
     def create_database(
@@ -412,58 +413,86 @@
             fields = ",".join(fields)
             ddl: str = template_cluster_by.render(fields=fields)
         else:
             ddl = ""
 
         return ddl
 
+    def field_ddl(
+        self, schema: StructType, always_identity_column: Optional[str] = None
+    ):
+        if schema is not None:
+            ddl = [self.create_column_ddl(f) for f in schema.fields]
+            if always_identity_column:
+                always_identity_column = (
+                    f"\t`{always_identity_column}` GENERATED ALWAYS AS IDENTITY"
+                )
+                ddl = [always_identity_column] + ddl
+
+            ddl = ",\n".join(ddl)
+
+            return ddl
+        else:
+            return ""
+
     def create_table_dll(
         self,
-        schema: StructType,
-        partition_fields: list = [],
-        cluster_by_fields: list = [],
+        database: str,
+        table: str,
+        catalog: Optional[str] = None,
+        schema: Optional[StructType] = None,
+        always_identity_column: Optional[str] = None,
+        partition_by: Optional[List[str]] = None,
+        cluster_by: Optional[List[str]] = None,
+        delta_properties: Optional[List[str]] = None,
         format: str = "DELTA",
-        always_identity_column: str = None,
+        location: Optional[str] = None,
     ):
-        field_ddl = [self.create_column_ddl(f) for f in schema.fields]
-        if always_identity_column:
-            always_identity_column = (
-                f"\t`{always_identity_column}` GENERATED ALWAYS AS IDENTITY"
-            )
-            field_ddl = [always_identity_column] + field_ddl
+        create_table_ddl = (
+            f"`{catalog}`.`{database}`.`{table}`"
+            if catalog
+            else f"`{database}`.`{table}`"
+        )
+        create_table_ddl = f"CREATE TABLE {create_table_ddl}"
 
-        field_ddl = ",\n".join(field_ddl)
+        field_ddl = self.field_ddl(schema, always_identity_column)
+        if delta_properties:
+            delta_properties_ddl = self.get_delta_properties_sql(delta_properties)
+            delta_properties_ddl = f"TBLPROPERTIES({delta_properties_ddl})"
 
-        template_ddl = jinja2.Template(
-            """CREATE TABLE {{database_name}}.{{table_name}}
-    (
-    {{field_ddl}}
-    )
-    USING {{format}} LOCATION '{{path}}'
-    {{partition_ddl}}
-    {{cluster_by_ddl}}""",
-            undefined=jinja2.DebugUndefined,
-        )
+        location_ddl = f"LOCATION '{location}'" if location else ""
 
         partition_ddl = ""
         cluster_by_ddl = ""
-        if cluster_by_fields:
-            cluster_by_ddl = self.partition_by_ddl(
-                cluster_by_fields, PartitionType.CLUSTER
-            )
-        elif partition_fields:
+        if cluster_by:
+            cluster_by_ddl = self.partition_by_ddl(cluster_by, PartitionType.CLUSTER)
+        elif partition_by:
             partition_ddl = self.partition_by_ddl(
-                partition_fields, PartitionType.PARTITIONED
+                partition_by, PartitionType.PARTITIONED
             )
 
+        template_ddl = jinja2.Template(
+            """{{create_table_ddl}}
+    {{field_ddl}}
+    {{partition_ddl}}
+    {{cluster_by_ddl}}
+    USING {{format}}
+    {{location_ddl}}
+    {{delta_properties_ddl}}""",
+            undefined=jinja2.DebugUndefined,
+        )
+
         replace = {
+            "create_table_ddl": create_table_ddl,
             "field_ddl": field_ddl,
             "partition_ddl": partition_ddl,
             "cluster_by_ddl": cluster_by_ddl,
             "format": format,
+            "location_ddl": location_ddl,
+            "delta_properties_ddl": delta_properties_ddl,
         }
 
         table_ddl = template_ddl.render(replace)
         table_ddl = f"{table_ddl};"
 
         return table_ddl
```

### Comparing `yetl-framework-2.0.5.dev1/yetl/config/table/_deltalake.py` & `yetl-framework-2.0.5.dev2/yetl/config/table/_deltalake.py`

 * *Files 9% similar despite different names*

```diff
@@ -108,23 +108,27 @@
             if self.managed:
                 self._spark.create_table(
                     database=self.database,
                     table=self.table,
                     delta_properties=self.delta_properties,
                     sql=self.sql,
                     catalog=self.catalog,
+                    cluster_by=self.cluster_by,
+                    partition_by=self.partition_by,
                 )
             else:
                 self._spark.create_table(
                     database=self.database,
                     table=self.table,
                     delta_properties=self.delta_properties,
                     path=self.location,
                     sql=self.sql,
                     catalog=self.catalog,
+                    cluster_by=self.cluster_by,
+                    partition_by=self.partition_by,
                 )
 
     def qualified_table_name(self):
         name = f"`{self.database}`.`{self.table}`"
         if self.catalog:
             name = f"`{self.catalog}`.{name}"
         return name
```

### Comparing `yetl-framework-2.0.5.dev1/yetl/config/table/_factory.py` & `yetl-framework-2.0.5.dev2/yetl/config/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/config/table/_read.py` & `yetl-framework-2.0.5.dev2/yetl/config/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/config/table/_table.py` & `yetl-framework-2.0.5.dev2/yetl/config/table/_table.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/resource/__init__.py` & `yetl-framework-2.0.5.dev2/yetl/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/resource/sibytes_yetl_pipeline_schema.json` & `yetl-framework-2.0.5.dev2/yetl/resource/sibytes_yetl_pipeline_schema.json`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/resource/sibytes_yetl_project_schema.json` & `yetl-framework-2.0.5.dev2/yetl/resource/sibytes_yetl_project_schema.json`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/resource/sibytes_yetl_tables_schema.json` & `yetl-framework-2.0.5.dev2/yetl/resource/sibytes_yetl_tables_schema.json`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/resource/tables.xlsx` & `yetl-framework-2.0.5.dev2/yetl/resource/tables.xlsx`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/validation/_validate.py` & `yetl-framework-2.0.5.dev2/yetl/validation/_validate.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/workflow/_dlt.py` & `yetl-framework-2.0.5.dev2/yetl/workflow/_dlt.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl/workflow/_multi_threaded.py` & `yetl-framework-2.0.5.dev2/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev1/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-2.0.5.dev2/yetl_framework.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 2.0.5.dev1
+Version: 2.0.5.dev2
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-2.0.5.dev1/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-2.0.5.dev2/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

