# Comparing `tmp/yetl-framework-2.0.5.dev3.tar.gz` & `tmp/yetl-framework-2.0.5.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-2.0.5.dev3.tar", last modified: Tue Aug  1 18:34:18 2023, max compression
+gzip compressed data, was "yetl-framework-2.0.5.dev4.tar", last modified: Tue Aug  1 18:47:48 2023, max compression
```

## Comparing `yetl-framework-2.0.5.dev3.tar` & `yetl-framework-2.0.5.dev4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 18:34:18.989667 yetl-framework-2.0.5.dev3/
--rw-r--r--   0 vsts      (1001) docker     (123)     1199 2023-08-01 18:34:18.989667 yetl-framework-2.0.5.dev3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-08-01 18:34:18.989667 yetl-framework-2.0.5.dev3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1544 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 18:34:18.985667 yetl-framework-2.0.5.dev3/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1764 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 18:34:18.985667 yetl-framework-2.0.5.dev3/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     3367 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 18:34:18.985667 yetl-framework-2.0.5.dev3/yetl/cli/metadata_provider/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/cli/metadata_provider/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17399 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/cli/metadata_provider/_xlsx.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 18:34:18.985667 yetl-framework-2.0.5.dev3/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4780 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2112 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9867 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5064 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19460 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 18:34:18.989667 yetl-framework-2.0.5.dev3/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5213 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6707 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4534 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 18:34:18.989667 yetl-framework-2.0.5.dev3/yetl/resource/
--rw-r--r--   0 vsts      (1001) docker     (123)      569 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/resource/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      299 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/resource/logging.yaml
--rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/resource/project.yaml
--rw-r--r--   0 vsts      (1001) docker     (123)    12636 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/resource/sibytes_yetl_pipeline_schema.json
--rw-r--r--   0 vsts      (1001) docker     (123)     2654 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/resource/sibytes_yetl_project_schema.json
--rw-r--r--   0 vsts      (1001) docker     (123)    14625 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/resource/sibytes_yetl_tables_schema.json
--rw-r--r--   0 vsts      (1001) docker     (123)    10012 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/resource/tables.xlsx
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 18:34:18.989667 yetl-framework-2.0.5.dev3/yetl/validation/
--rw-r--r--   0 vsts      (1001) docker     (123)      353 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/validation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1495 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/validation/_validate.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 18:34:18.989667 yetl-framework-2.0.5.dev3/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/workflow/_dlt.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-08-01 18:33:20.000000 yetl-framework-2.0.5.dev3/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 18:34:18.989667 yetl-framework-2.0.5.dev3/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     1199 2023-08-01 18:34:18.000000 yetl-framework-2.0.5.dev3/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1377 2023-08-01 18:34:18.000000 yetl-framework-2.0.5.dev3/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-01 18:34:18.000000 yetl-framework-2.0.5.dev3/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-01 18:34:18.000000 yetl-framework-2.0.5.dev3/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       76 2023-08-01 18:34:18.000000 yetl-framework-2.0.5.dev3/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-08-01 18:34:18.000000 yetl-framework-2.0.5.dev3/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 18:47:48.210127 yetl-framework-2.0.5.dev4/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1199 2023-08-01 18:47:48.210127 yetl-framework-2.0.5.dev4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-08-01 18:47:48.210127 yetl-framework-2.0.5.dev4/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1544 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 18:47:48.198126 yetl-framework-2.0.5.dev4/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1764 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 18:47:48.198126 yetl-framework-2.0.5.dev4/yetl/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3367 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/cli/_init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 18:47:48.198126 yetl-framework-2.0.5.dev4/yetl/cli/metadata_provider/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/cli/metadata_provider/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17399 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/cli/metadata_provider/_xlsx.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 18:47:48.202126 yetl-framework-2.0.5.dev4/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4780 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2112 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9867 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5064 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19653 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 18:47:48.202126 yetl-framework-2.0.5.dev4/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5213 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6707 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4534 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 18:47:48.206127 yetl-framework-2.0.5.dev4/yetl/resource/
+-rw-r--r--   0 vsts      (1001) docker     (123)      569 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/resource/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      299 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/resource/logging.yaml
+-rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/resource/project.yaml
+-rw-r--r--   0 vsts      (1001) docker     (123)    12636 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/resource/sibytes_yetl_pipeline_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     2654 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/resource/sibytes_yetl_project_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    14625 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/resource/sibytes_yetl_tables_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    10012 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/resource/tables.xlsx
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 18:47:48.206127 yetl-framework-2.0.5.dev4/yetl/validation/
+-rw-r--r--   0 vsts      (1001) docker     (123)      353 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/validation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1495 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/validation/_validate.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 18:47:48.206127 yetl-framework-2.0.5.dev4/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/workflow/_dlt.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-08-01 18:46:44.000000 yetl-framework-2.0.5.dev4/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 18:47:48.210127 yetl-framework-2.0.5.dev4/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1199 2023-08-01 18:47:48.000000 yetl-framework-2.0.5.dev4/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1377 2023-08-01 18:47:48.000000 yetl-framework-2.0.5.dev4/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-01 18:47:48.000000 yetl-framework-2.0.5.dev4/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-01 18:47:48.000000 yetl-framework-2.0.5.dev4/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       76 2023-08-01 18:47:48.000000 yetl-framework-2.0.5.dev4/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-08-01 18:47:48.000000 yetl-framework-2.0.5.dev4/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-2.0.5.dev3/PKG-INFO` & `yetl-framework-2.0.5.dev4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 2.0.5.dev3
+Version: 2.0.5.dev4
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-2.0.5.dev3/README.md` & `yetl-framework-2.0.5.dev4/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/setup.py` & `yetl-framework-2.0.5.dev4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="2.0.5.dev3",
+    version="2.0.5.dev4",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-2.0.5.dev3/yetl/__main__.py` & `yetl-framework-2.0.5.dev4/yetl/__main__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/cli/_init.py` & `yetl-framework-2.0.5.dev4/yetl/cli/_init.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/cli/metadata_provider/_xlsx.py` & `yetl-framework-2.0.5.dev4/yetl/cli/metadata_provider/_xlsx.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/config/__init__.py` & `yetl-framework-2.0.5.dev4/yetl/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/config/_config.py` & `yetl-framework-2.0.5.dev4/yetl/config/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/config/_decorators.py` & `yetl-framework-2.0.5.dev4/yetl/config/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/config/_logging_config.py` & `yetl-framework-2.0.5.dev4/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/config/_project.py` & `yetl-framework-2.0.5.dev4/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/config/_spark_context.py` & `yetl-framework-2.0.5.dev4/yetl/config/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/config/_tables.py` & `yetl-framework-2.0.5.dev4/yetl/config/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/config/_timeslice.py` & `yetl-framework-2.0.5.dev4/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/config/_utils.py` & `yetl-framework-2.0.5.dev4/yetl/config/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/config/deltalake.py` & `yetl-framework-2.0.5.dev4/yetl/config/deltalake.py`

 * *Files 2% similar despite different names*

```diff
@@ -451,36 +451,41 @@
         create_table_ddl = (
             f"`{catalog}`.`{database}`.`{table}`"
             if catalog
             else f"`{database}`.`{table}`"
         )
         create_table_ddl = f"CREATE TABLE {create_table_ddl}"
 
-        field_ddl = self.field_ddl(schema, always_identity_column)
         if delta_properties:
             delta_properties_ddl = self.get_delta_properties_sql(delta_properties)
             delta_properties_ddl = f"\nTBLPROPERTIES({delta_properties_ddl})"
 
         location_ddl = f"\nLOCATION '{location}'" if location else ""
 
         partition_ddl = ""
         cluster_by_ddl = ""
-        if cluster_by:
-            cluster_by_ddl = self.partition_by_ddl(cluster_by, PartitionType.CLUSTER)
-            cluster_by_ddl = f"\n{cluster_by_ddl}"
-        elif partition_by:
-            partition_ddl = self.partition_by_ddl(
-                partition_by, PartitionType.PARTITIONED
-            )
-            partition_ddl = f"\n{partition_ddl}"
 
+        field_ddl = self.field_ddl(schema, always_identity_column)
+        if field_ddl:
+            field_ddl = f"\n{field_ddl}"
+            if cluster_by:
+                cluster_by_ddl = self.partition_by_ddl(
+                    cluster_by, PartitionType.CLUSTER
+                )
+                cluster_by_ddl = f"\n{cluster_by_ddl}"
+            elif partition_by:
+                partition_ddl = self.partition_by_ddl(
+                    partition_by, PartitionType.PARTITIONED
+                )
+                partition_ddl = f"\n{partition_ddl}"
+            field_ddl = f"{field_ddl}{cluster_by_ddl}{partition_ddl}"
+
+        template_ddl = "{{create_table_ddl}}{{field_ddl}}\nUSING {{format}}{{location_ddl}}{{delta_properties_ddl}}"
         template_ddl = jinja2.Template(
-            """{{create_table_ddl}}
-    {{field_ddl}}{{partition_ddl}}{{cluster_by_ddl}}
-    USING {{format}}{{location_ddl}}{{delta_properties_ddl}}""",
+            template_ddl,
             undefined=jinja2.DebugUndefined,
         )
 
         replace = {
             "create_table_ddl": create_table_ddl,
             "field_ddl": field_ddl,
             "partition_ddl": partition_ddl,
```

### Comparing `yetl-framework-2.0.5.dev3/yetl/config/table/_deltalake.py` & `yetl-framework-2.0.5.dev4/yetl/config/table/_deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/config/table/_factory.py` & `yetl-framework-2.0.5.dev4/yetl/config/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/config/table/_read.py` & `yetl-framework-2.0.5.dev4/yetl/config/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/config/table/_table.py` & `yetl-framework-2.0.5.dev4/yetl/config/table/_table.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/resource/__init__.py` & `yetl-framework-2.0.5.dev4/yetl/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/resource/sibytes_yetl_pipeline_schema.json` & `yetl-framework-2.0.5.dev4/yetl/resource/sibytes_yetl_pipeline_schema.json`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/resource/sibytes_yetl_project_schema.json` & `yetl-framework-2.0.5.dev4/yetl/resource/sibytes_yetl_project_schema.json`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/resource/sibytes_yetl_tables_schema.json` & `yetl-framework-2.0.5.dev4/yetl/resource/sibytes_yetl_tables_schema.json`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/resource/tables.xlsx` & `yetl-framework-2.0.5.dev4/yetl/resource/tables.xlsx`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/validation/_validate.py` & `yetl-framework-2.0.5.dev4/yetl/validation/_validate.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/workflow/_dlt.py` & `yetl-framework-2.0.5.dev4/yetl/workflow/_dlt.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl/workflow/_multi_threaded.py` & `yetl-framework-2.0.5.dev4/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.5.dev3/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-2.0.5.dev4/yetl_framework.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 2.0.5.dev3
+Version: 2.0.5.dev4
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-2.0.5.dev3/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-2.0.5.dev4/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

