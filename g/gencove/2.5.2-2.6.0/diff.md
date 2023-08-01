# Comparing `tmp/gencove-2.5.2.tar.gz` & `tmp/gencove-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gencove-2.5.2.tar", last modified: Mon Jul 10 17:42:33 2023, max compression
+gzip compressed data, was "dist/gencove-2.6.0.tar", last modified: Tue Aug  1 20:10:46 2023, max compression
```

## Comparing `gencove-2.5.2.tar` & `gencove-2.6.0.tar`

### file list

```diff
@@ -1,301 +1,301 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/
--rw-r--r--   0 root         (0) root         (0)     2387 2023-07-10 17:42:33.000000 gencove-2.5.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2085 2023-07-10 17:41:58.000000 gencove-2.5.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    32627 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6009 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/basespace/
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/basespace/autoimports/
--rw-rw-rw-   0 root         (0) root         (0)       92 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/autoimports/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/basespace/autoimports/autoimport_list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/autoimports/autoimport_list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/autoimports/autoimport_list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1966 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/autoimports/autoimport_list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/autoimports/autoimport_list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      343 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/autoimports/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/basespace/autoimports/create/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/autoimports/create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1883 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/autoimports/create/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/autoimports/create/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2398 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/autoimports/create/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/basespace/biosamples/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/biosamples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/basespace/biosamples/biosamples_list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/biosamples/biosamples_list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      897 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/biosamples/biosamples_list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2212 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/biosamples/biosamples_list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/biosamples/biosamples_list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/biosamples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/basespace/projects/
--rw-rw-rw-   0 root         (0) root         (0)       86 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/projects/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/basespace/projects/basespace_import/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/projects/basespace_import/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2031 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/projects/basespace_import/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/projects/basespace_import/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2151 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/projects/basespace_import/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/basespace/projects/basespace_list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/projects/basespace_list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/projects/basespace_list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1987 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/projects/basespace_list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      571 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/projects/basespace_list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      358 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/basespace/projects/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/common_cli_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/download/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/download/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4611 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/download/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2104 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/download/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/download/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    14731 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/download/main.py
--rw-rw-rw-   0 root         (0) root         (0)    10579 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/download/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/files/
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/files/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/files/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/files/main.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/files/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/projects/
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1682 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/projects/create/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/create/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1439 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/create/main.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/create/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/projects/create_batch/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/create_batch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1316 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/create_batch/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/create_batch/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/projects/create_merged_vcf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/create_merged_vcf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      687 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/create_merged_vcf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1436 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/create_merged_vcf/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/projects/delete_samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/delete_samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1030 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/delete_samples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1931 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/delete_samples/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/projects/get_batch/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/get_batch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      936 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/get_batch/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2769 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/get_batch/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/projects/get_merged_vcf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/get_merged_vcf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/get_merged_vcf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2147 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/get_merged_vcf/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/projects/import_existing_samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/import_existing_samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1880 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/import_existing_samples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/import_existing_samples/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2191 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/import_existing_samples/main.py
--rw-rw-rw-   0 root         (0) root         (0)      442 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/import_existing_samples/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/projects/list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      469 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2859 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/list/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/projects/list_batch_types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/list_batch_types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      688 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/list_batch_types/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/list_batch_types/main.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/list_batch_types/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/projects/list_batches/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/list_batches/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      666 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/list_batches/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2182 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/list_batches/main.py
--rw-rw-rw-   0 root         (0) root         (0)      499 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/list_batches/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/projects/list_pipeline_capabilities/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/list_pipeline_capabilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      744 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/list_pipeline_capabilities/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1668 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/list_pipeline_capabilities/main.py
--rw-rw-rw-   0 root         (0) root         (0)      448 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/list_pipeline_capabilities/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/projects/list_pipelines/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/list_pipelines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/list_pipelines/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1842 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/list_pipelines/main.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/list_pipelines/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/projects/restore_samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/restore_samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1116 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/restore_samples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1823 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/restore_samples/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/projects/run_prefix/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/run_prefix/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1953 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/run_prefix/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/run_prefix/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     4918 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/run_prefix/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/projects/samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1603 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/samples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      343 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/samples/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2454 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/samples/main.py
--rw-rw-rw-   0 root         (0) root         (0)      735 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/samples/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/projects/status_merged_vcf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/status_merged_vcf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      705 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/status_merged_vcf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1813 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/status_merged_vcf/main.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/projects/status_merged_vcf/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/s3_imports/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/s3_imports/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/s3_imports/autoimports/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/s3_imports/autoimports/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/s3_imports/autoimports/autoimport_list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/s3_imports/autoimports/autoimport_list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/s3_imports/autoimports/autoimport_list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/s3_imports/autoimports/autoimport_list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/s3_imports/autoimports/autoimport_list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      336 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/s3_imports/autoimports/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/s3_imports/autoimports/create/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/s3_imports/autoimports/create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1585 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/s3_imports/autoimports/create/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      226 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/s3_imports/autoimports/create/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2314 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/s3_imports/autoimports/create/main.py
--rw-rw-rw-   0 root         (0) root         (0)      392 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/s3_imports/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/s3_imports/s3_import/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/s3_imports/s3_import/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1434 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/s3_imports/s3_import/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/s3_imports/s3_import/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1916 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/s3_imports/s3_import/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/samples/
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/samples/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/samples/download_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/samples/download_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3262 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/samples/download_file/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/samples/download_file/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     5345 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/samples/download_file/main.py
--rw-rw-rw-   0 root         (0) root         (0)     3051 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/samples/download_file/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/samples/get_metadata/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/samples/get_metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      810 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/samples/get_metadata/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2348 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/samples/get_metadata/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/samples/set_metadata/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/samples/set_metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      758 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/samples/set_metadata/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1981 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/samples/set_metadata/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/upload/
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/upload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2760 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/upload/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1529 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/upload/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/upload/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    17222 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/upload/main.py
--rw-rw-rw-   0 root         (0) root         (0)     3028 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/upload/multi_file_reader.py
--rw-rw-rw-   0 root         (0) root         (0)     9443 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/upload/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/uploads/
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/uploads/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/uploads/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/uploads/list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/uploads/list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      934 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/uploads/list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/uploads/list/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/uploads/list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/uploads/list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3462 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/webhook/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/webhook/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/webhook/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/command/webhook/verify/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/webhook/verify/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1011 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/webhook/verify/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      999 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/command/webhook/verify/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3731 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/description/
--rw-rw-rw-   0 root         (0) root         (0)     1811 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/description/pypi_readme.md
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3205 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     7984 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/tests/
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/tests/basespace/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/basespace/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6374 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/basespace/test_basespace_autoimports_create.py
--rw-rw-rw-   0 root         (0) root         (0)     4249 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/basespace/test_basespace_autoimports_list.py
--rw-rw-rw-   0 root         (0) root         (0)     7257 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/basespace/test_basespace_biosamples_list.py
--rw-rw-rw-   0 root         (0) root         (0)     6334 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/basespace/test_basespace_projects_import.py
--rw-rw-rw-   0 root         (0) root         (0)     5955 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/basespace/test_basespace_projects_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/tests/basespace/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/basespace/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4675 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3328 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/tests/download/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/download/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    36754 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/download/test_cli_download.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/tests/download/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/download/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/download/vcr/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/tests/files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/files/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4371 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/files/test_file_types_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/tests/files/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/files/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4942 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/tests/projects/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/projects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6781 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/projects/test_projects_batch_get.py
--rw-rw-rw-   0 root         (0) root         (0)     4502 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/projects/test_projects_batch_types_list.py
--rw-rw-rw-   0 root         (0) root         (0)     8945 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/projects/test_projects_batches_create.py
--rw-rw-rw-   0 root         (0) root         (0)     4601 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/projects/test_projects_batches_list.py
--rw-rw-rw-   0 root         (0) root         (0)     4380 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/projects/test_projects_create.py
--rw-rw-rw-   0 root         (0) root         (0)     9108 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/projects/test_projects_create_merged_vcf.py
--rw-rw-rw-   0 root         (0) root         (0)     8901 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/projects/test_projects_delete_samples.py
--rw-rw-rw-   0 root         (0) root         (0)    12016 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/projects/test_projects_get_merged_vcf.py
--rw-rw-rw-   0 root         (0) root         (0)     6286 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/projects/test_projects_import_existing_samples.py
--rw-rw-rw-   0 root         (0) root         (0)    10605 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/projects/test_projects_list.py
--rw-rw-rw-   0 root         (0) root         (0)     6511 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/projects/test_projects_pipeline_capabilities_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3899 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/projects/test_projects_pipelines_list.py
--rw-rw-rw-   0 root         (0) root         (0)     7212 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/projects/test_projects_restore_samples.py
--rw-rw-rw-   0 root         (0) root         (0)    13390 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/projects/test_projects_run_prefix.py
--rw-rw-rw-   0 root         (0) root         (0)     7184 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/projects/test_projects_samples_list.py
--rw-rw-rw-   0 root         (0) root         (0)     6468 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/projects/test_projects_status_merged_vcf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/tests/projects/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/projects/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11910 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/projects/vcr/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/tests/s3_imports/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/s3_imports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6422 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/s3_imports/test_s3_autoimports_create.py
--rw-rw-rw-   0 root         (0) root         (0)     4163 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/s3_imports/test_s3_autoimports_list.py
--rw-rw-rw-   0 root         (0) root         (0)     5269 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/s3_imports/test_s3_uri_import.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/tests/s3_imports/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/s3_imports/vcr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/tests/samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10756 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/samples/test_samples_download_file.py
--rw-rw-rw-   0 root         (0) root         (0)     7024 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/samples/test_samples_get_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     3433 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/samples/test_samples_set_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/tests/samples/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/samples/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      700 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/samples/vcr/filters.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/test_logger.py
--rw-rw-rw-   0 root         (0) root         (0)    24076 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/tests/upload/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/upload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    44376 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/upload/test_cli_upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/tests/upload/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/upload/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5281 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/upload/vcr/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/tests/uploads/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/uploads/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4357 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/uploads/test_uploads_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/tests/uploads/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/uploads/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      971 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/tests/webhook/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/webhook/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3430 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/tests/webhook/test_webhook_verify.py
--rw-rw-rw-   0 root         (0) root         (0)     5174 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove/version/
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/version/A-major
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/version/B-minor
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/version/C-patch
--rw-rw-rw-   0 root         (0) root         (0)      400 2023-07-10 17:41:58.000000 gencove-2.5.2/gencove/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2387 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10251 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      127 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-10 17:42:33.000000 gencove-2.5.2/gencove.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-07-10 17:42:33.000000 gencove-2.5.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1866 2023-07-10 17:41:58.000000 gencove-2.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/
+-rw-r--r--   0 root         (0) root         (0)     2387 2023-08-01 20:10:46.000000 gencove-2.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2085 2023-08-01 20:10:12.000000 gencove-2.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-08-01 20:10:12.000000 gencove-2.6.0/gencove/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-08-01 20:10:12.000000 gencove-2.6.0/gencove/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    32627 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6009 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/basespace/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/basespace/autoimports/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/autoimports/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/basespace/autoimports/autoimport_list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/autoimports/autoimport_list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/autoimports/autoimport_list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/autoimports/autoimport_list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/autoimports/autoimport_list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      343 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/autoimports/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/basespace/autoimports/create/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/autoimports/create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1883 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/autoimports/create/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/autoimports/create/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2398 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/autoimports/create/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/basespace/biosamples/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/biosamples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/basespace/biosamples/biosamples_list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/biosamples/biosamples_list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      897 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/biosamples/biosamples_list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2212 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/biosamples/biosamples_list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/biosamples/biosamples_list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/biosamples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/basespace/projects/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/projects/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/basespace/projects/basespace_import/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/projects/basespace_import/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/projects/basespace_import/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/projects/basespace_import/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2151 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/projects/basespace_import/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/basespace/projects/basespace_list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/projects/basespace_list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/projects/basespace_list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/projects/basespace_list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      571 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/projects/basespace_list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      358 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/basespace/projects/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/common_cli_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/download/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/download/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4611 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/download/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2104 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/download/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/download/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    14731 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/download/main.py
+-rw-rw-rw-   0 root         (0) root         (0)    10579 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/download/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/files/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/files/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/files/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/files/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/files/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/projects/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1682 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/projects/create/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/create/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1439 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/create/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/create/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/projects/create_batch/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/create_batch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1316 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/create_batch/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/create_batch/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/projects/create_merged_vcf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/create_merged_vcf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      687 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/create_merged_vcf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/create_merged_vcf/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/projects/delete_samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/delete_samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/delete_samples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/delete_samples/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/projects/get_batch/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/get_batch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      936 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/get_batch/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2769 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/get_batch/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/projects/get_merged_vcf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/get_merged_vcf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/get_merged_vcf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2147 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/get_merged_vcf/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/projects/import_existing_samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/import_existing_samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1880 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/import_existing_samples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/import_existing_samples/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/import_existing_samples/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      442 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/import_existing_samples/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/projects/list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     3051 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      699 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/list/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/projects/list_batch_types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/list_batch_types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      688 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/list_batch_types/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/list_batch_types/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/list_batch_types/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/projects/list_batches/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/list_batches/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      666 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/list_batches/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2182 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/list_batches/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      499 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/list_batches/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/projects/list_pipeline_capabilities/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/list_pipeline_capabilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      744 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/list_pipeline_capabilities/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1668 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/list_pipeline_capabilities/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      448 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/list_pipeline_capabilities/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/projects/list_pipelines/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/list_pipelines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/list_pipelines/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1842 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/list_pipelines/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/list_pipelines/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/projects/restore_samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/restore_samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/restore_samples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1823 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/restore_samples/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/projects/run_prefix/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/run_prefix/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1953 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/run_prefix/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/run_prefix/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     4918 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/run_prefix/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/projects/samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1603 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/samples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      343 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/samples/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2454 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/samples/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      735 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/samples/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/projects/status_merged_vcf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/status_merged_vcf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      705 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/status_merged_vcf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1813 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/status_merged_vcf/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/projects/status_merged_vcf/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/s3_imports/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/s3_imports/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/s3_imports/autoimports/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/s3_imports/autoimports/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/s3_imports/autoimports/autoimport_list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/s3_imports/autoimports/autoimport_list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/s3_imports/autoimports/autoimport_list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/s3_imports/autoimports/autoimport_list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/s3_imports/autoimports/autoimport_list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      336 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/s3_imports/autoimports/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/s3_imports/autoimports/create/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/s3_imports/autoimports/create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/s3_imports/autoimports/create/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      226 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/s3_imports/autoimports/create/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2314 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/s3_imports/autoimports/create/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      392 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/s3_imports/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/s3_imports/s3_import/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/s3_imports/s3_import/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1434 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/s3_imports/s3_import/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/s3_imports/s3_import/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1916 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/s3_imports/s3_import/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/samples/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/samples/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/samples/download_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/samples/download_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3262 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/samples/download_file/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      141 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/samples/download_file/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     5345 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/samples/download_file/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3051 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/samples/download_file/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/samples/get_metadata/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/samples/get_metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      810 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/samples/get_metadata/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/samples/get_metadata/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/samples/set_metadata/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/samples/set_metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      758 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/samples/set_metadata/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/samples/set_metadata/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/upload/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/upload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/upload/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/upload/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/upload/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    17222 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/upload/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3028 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/upload/multi_file_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     9443 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/upload/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/uploads/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/uploads/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/uploads/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/uploads/list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/uploads/list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      934 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/uploads/list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/uploads/list/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/uploads/list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/uploads/list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3462 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/webhook/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/webhook/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/webhook/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/command/webhook/verify/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/webhook/verify/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/webhook/verify/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      999 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/command/webhook/verify/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3731 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/description/
+-rw-rw-rw-   0 root         (0) root         (0)     1811 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/description/pypi_readme.md
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3205 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     8020 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/tests/basespace/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/basespace/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6374 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/basespace/test_basespace_autoimports_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     4249 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/basespace/test_basespace_autoimports_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     7257 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/basespace/test_basespace_biosamples_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     6334 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/basespace/test_basespace_projects_import.py
+-rw-rw-rw-   0 root         (0) root         (0)     5955 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/basespace/test_basespace_projects_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/tests/basespace/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/basespace/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4675 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3328 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/tests/download/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/download/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    36754 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/download/test_cli_download.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/tests/download/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/download/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/download/vcr/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/tests/files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/files/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4371 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/files/test_file_types_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/tests/files/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/files/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4942 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/tests/projects/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/projects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6781 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/projects/test_projects_batch_get.py
+-rw-rw-rw-   0 root         (0) root         (0)     4502 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/projects/test_projects_batch_types_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     8945 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/projects/test_projects_batches_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     4601 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/projects/test_projects_batches_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     4380 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/projects/test_projects_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     9108 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/projects/test_projects_create_merged_vcf.py
+-rw-rw-rw-   0 root         (0) root         (0)     8901 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/projects/test_projects_delete_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)    12016 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/projects/test_projects_get_merged_vcf.py
+-rw-rw-rw-   0 root         (0) root         (0)     6286 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/projects/test_projects_import_existing_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)    12079 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/projects/test_projects_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     6511 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/projects/test_projects_pipeline_capabilities_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3899 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/projects/test_projects_pipelines_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     7212 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/projects/test_projects_restore_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)    13390 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/projects/test_projects_run_prefix.py
+-rw-rw-rw-   0 root         (0) root         (0)     7184 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/projects/test_projects_samples_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     6468 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/projects/test_projects_status_merged_vcf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/tests/projects/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/projects/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11910 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/projects/vcr/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/tests/s3_imports/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/s3_imports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6422 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/s3_imports/test_s3_autoimports_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     4163 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/s3_imports/test_s3_autoimports_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     5269 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/s3_imports/test_s3_uri_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/tests/s3_imports/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/s3_imports/vcr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/tests/samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10756 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/samples/test_samples_download_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     7024 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/samples/test_samples_get_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/samples/test_samples_set_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/tests/samples/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/samples/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      700 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/samples/vcr/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/test_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)    24076 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/tests/upload/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/upload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    44376 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/upload/test_cli_upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/tests/upload/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/upload/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5281 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/upload/vcr/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/tests/uploads/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/uploads/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4357 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/uploads/test_uploads_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/tests/uploads/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/uploads/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      971 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/tests/webhook/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/webhook/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3430 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/tests/webhook/test_webhook_verify.py
+-rw-rw-rw-   0 root         (0) root         (0)     5174 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove/version/
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/version/A-major
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/version/B-minor
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/version/C-patch
+-rw-rw-rw-   0 root         (0) root         (0)      400 2023-08-01 20:10:13.000000 gencove-2.6.0/gencove/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2387 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10251 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      127 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-01 20:10:46.000000 gencove-2.6.0/gencove.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-08-01 20:10:46.000000 gencove-2.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1866 2023-08-01 20:10:13.000000 gencove-2.6.0/setup.py
```

### Comparing `gencove-2.5.2/PKG-INFO` & `gencove-2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gencove
-Version: 2.5.2
+Version: 2.6.0
 Summary: Gencove API and CLI tool
 Home-page: http://docs.gencove.com
 Author: Tomaz Berisa
 License: Apache 2.0
 Description: # The Gencove CLI
         
         [![PyPI Latest Release](https://img.shields.io/pypi/v/gencove.svg)](https://pypi.org/project/gencove/)
```

### Comparing `gencove-2.5.2/README.md` & `gencove-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/cli.py` & `gencove-2.6.0/gencove/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/client.py` & `gencove-2.6.0/gencove/client.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/base.py` & `gencove-2.6.0/gencove/command/base.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/basespace/autoimports/autoimport_list/cli.py` & `gencove-2.6.0/gencove/command/basespace/autoimports/autoimport_list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/basespace/autoimports/autoimport_list/main.py` & `gencove-2.6.0/gencove/command/basespace/autoimports/autoimport_list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/basespace/autoimports/autoimport_list/utils.py` & `gencove-2.6.0/gencove/command/basespace/autoimports/autoimport_list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/basespace/autoimports/create/cli.py` & `gencove-2.6.0/gencove/command/basespace/autoimports/create/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/basespace/autoimports/create/main.py` & `gencove-2.6.0/gencove/command/basespace/autoimports/create/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/basespace/biosamples/biosamples_list/cli.py` & `gencove-2.6.0/gencove/command/basespace/biosamples/biosamples_list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/basespace/biosamples/biosamples_list/main.py` & `gencove-2.6.0/gencove/command/basespace/biosamples/biosamples_list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/basespace/biosamples/biosamples_list/utils.py` & `gencove-2.6.0/gencove/command/basespace/biosamples/biosamples_list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/basespace/projects/basespace_import/cli.py` & `gencove-2.6.0/gencove/command/basespace/projects/basespace_import/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/basespace/projects/basespace_import/main.py` & `gencove-2.6.0/gencove/command/basespace/projects/basespace_import/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/basespace/projects/basespace_list/cli.py` & `gencove-2.6.0/gencove/command/basespace/projects/basespace_list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/basespace/projects/basespace_list/main.py` & `gencove-2.6.0/gencove/command/basespace/projects/basespace_list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/basespace/projects/basespace_list/utils.py` & `gencove-2.6.0/gencove/command/basespace/projects/basespace_list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/common_cli_options.py` & `gencove-2.6.0/gencove/command/common_cli_options.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/download/cli.py` & `gencove-2.6.0/gencove/command/download/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/download/constants.py` & `gencove-2.6.0/gencove/command/download/constants.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/download/main.py` & `gencove-2.6.0/gencove/command/download/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/download/utils.py` & `gencove-2.6.0/gencove/command/download/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/files/cli.py` & `gencove-2.6.0/gencove/command/files/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/files/main.py` & `gencove-2.6.0/gencove/command/files/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/cli.py` & `gencove-2.6.0/gencove/command/projects/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/create/cli.py` & `gencove-2.6.0/gencove/command/projects/create/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/create/main.py` & `gencove-2.6.0/gencove/command/projects/create/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/create_batch/cli.py` & `gencove-2.6.0/gencove/command/projects/create_batch/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/create_batch/main.py` & `gencove-2.6.0/gencove/command/projects/create_batch/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/create_merged_vcf/cli.py` & `gencove-2.6.0/gencove/command/projects/create_merged_vcf/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/create_merged_vcf/main.py` & `gencove-2.6.0/gencove/command/projects/create_merged_vcf/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/delete_samples/cli.py` & `gencove-2.6.0/gencove/command/projects/delete_samples/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/delete_samples/main.py` & `gencove-2.6.0/gencove/command/projects/delete_samples/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/get_batch/cli.py` & `gencove-2.6.0/gencove/command/projects/get_batch/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/get_batch/main.py` & `gencove-2.6.0/gencove/command/projects/get_batch/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/get_merged_vcf/cli.py` & `gencove-2.6.0/gencove/command/projects/get_merged_vcf/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/get_merged_vcf/main.py` & `gencove-2.6.0/gencove/command/projects/get_merged_vcf/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/import_existing_samples/cli.py` & `gencove-2.6.0/gencove/command/projects/import_existing_samples/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/import_existing_samples/main.py` & `gencove-2.6.0/gencove/command/projects/import_existing_samples/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/list/main.py` & `gencove-2.6.0/gencove/command/projects/list/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 from .utils import get_line
 
 
 class List(Command):
     """List projects command executor."""
 
+    def __init__(self, include_capability, credentials, options):
+        super().__init__(credentials, options)
+        self.include_capability = include_capability
+
     def initialize(self):
         """Initialize list subcommand."""
         self.login()
 
     def validate(self):
         """Validate command input."""
 
@@ -31,15 +35,15 @@
                 augmented_projects = (
                     self.augment_projects_with_pipeline_capabilities(  # noqa: E501
                         projects
                     )
                 )
 
                 for project in augmented_projects:
-                    self.echo_data(get_line(project))
+                    self.echo_data(get_line(project, self.include_capability))
         except APIClientError as err:
             if err.status_code == 404:
                 self.echo_error("No projects found.")
             raise
 
     def get_paginated_projects(self):
         """Paginate over all projects.
```

### Comparing `gencove-2.5.2/gencove/command/projects/list_batch_types/cli.py` & `gencove-2.6.0/gencove/command/projects/list_batch_types/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/list_batch_types/main.py` & `gencove-2.6.0/gencove/command/projects/list_batch_types/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/list_batches/cli.py` & `gencove-2.6.0/gencove/command/projects/list_batches/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/list_batches/main.py` & `gencove-2.6.0/gencove/command/projects/list_batches/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/list_pipeline_capabilities/cli.py` & `gencove-2.6.0/gencove/command/projects/list_pipeline_capabilities/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/list_pipeline_capabilities/main.py` & `gencove-2.6.0/gencove/command/projects/list_pipeline_capabilities/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/list_pipelines/cli.py` & `gencove-2.6.0/gencove/command/projects/list_pipelines/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/list_pipelines/main.py` & `gencove-2.6.0/gencove/command/projects/list_pipelines/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/restore_samples/cli.py` & `gencove-2.6.0/gencove/command/projects/restore_samples/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/restore_samples/main.py` & `gencove-2.6.0/gencove/command/projects/restore_samples/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/run_prefix/cli.py` & `gencove-2.6.0/gencove/command/projects/run_prefix/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/run_prefix/main.py` & `gencove-2.6.0/gencove/command/projects/run_prefix/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/samples/cli.py` & `gencove-2.6.0/gencove/command/projects/samples/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/samples/main.py` & `gencove-2.6.0/gencove/command/projects/samples/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/samples/utils.py` & `gencove-2.6.0/gencove/command/projects/samples/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/status_merged_vcf/cli.py` & `gencove-2.6.0/gencove/command/projects/status_merged_vcf/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/projects/status_merged_vcf/main.py` & `gencove-2.6.0/gencove/command/projects/status_merged_vcf/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/s3_imports/autoimports/autoimport_list/cli.py` & `gencove-2.6.0/gencove/command/s3_imports/autoimports/autoimport_list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/s3_imports/autoimports/autoimport_list/main.py` & `gencove-2.6.0/gencove/command/s3_imports/autoimports/autoimport_list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/s3_imports/autoimports/create/cli.py` & `gencove-2.6.0/gencove/command/s3_imports/autoimports/create/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/s3_imports/autoimports/create/main.py` & `gencove-2.6.0/gencove/command/s3_imports/autoimports/create/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/s3_imports/s3_import/cli.py` & `gencove-2.6.0/gencove/command/s3_imports/s3_import/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/s3_imports/s3_import/main.py` & `gencove-2.6.0/gencove/command/s3_imports/s3_import/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/samples/download_file/cli.py` & `gencove-2.6.0/gencove/command/samples/download_file/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/samples/download_file/main.py` & `gencove-2.6.0/gencove/command/samples/download_file/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/samples/download_file/utils.py` & `gencove-2.6.0/gencove/command/samples/download_file/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/samples/get_metadata/cli.py` & `gencove-2.6.0/gencove/command/samples/get_metadata/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/samples/get_metadata/main.py` & `gencove-2.6.0/gencove/command/samples/get_metadata/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/samples/set_metadata/cli.py` & `gencove-2.6.0/gencove/command/samples/set_metadata/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/samples/set_metadata/main.py` & `gencove-2.6.0/gencove/command/samples/set_metadata/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/upload/cli.py` & `gencove-2.6.0/gencove/command/upload/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/upload/constants.py` & `gencove-2.6.0/gencove/command/upload/constants.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/upload/main.py` & `gencove-2.6.0/gencove/command/upload/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/upload/multi_file_reader.py` & `gencove-2.6.0/gencove/command/upload/multi_file_reader.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/upload/utils.py` & `gencove-2.6.0/gencove/command/upload/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/uploads/list/cli.py` & `gencove-2.6.0/gencove/command/uploads/list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/uploads/list/main.py` & `gencove-2.6.0/gencove/command/uploads/list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/uploads/list/utils.py` & `gencove-2.6.0/gencove/command/uploads/list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/utils.py` & `gencove-2.6.0/gencove/command/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/webhook/verify/cli.py` & `gencove-2.6.0/gencove/command/webhook/verify/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/command/webhook/verify/utils.py` & `gencove-2.6.0/gencove/command/webhook/verify/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/constants.py` & `gencove-2.6.0/gencove/constants.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/description/pypi_readme.md` & `gencove-2.6.0/gencove/description/pypi_readme.md`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/logger.py` & `gencove-2.6.0/gencove/logger.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/models.py` & `gencove-2.6.0/gencove/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,17 @@
     previous: Optional[str]
 
 
 # pylint: disable=too-few-public-methods
 class PipelineCapabilities(GencoveBaseModel):
     """Pipeline Capabilities record"""
 
+    id: UUID
     name: Optional[str]
+    key: Optional[str]
 
 
 class SampleFile(GencoveBaseModel):
     """SampleFile model"""
 
     s3_path: Optional[str]
     size: Optional[int]
```

### Comparing `gencove-2.5.2/gencove/tests/basespace/test_basespace_autoimports_create.py` & `gencove-2.6.0/gencove/tests/basespace/test_basespace_autoimports_create.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/basespace/test_basespace_autoimports_list.py` & `gencove-2.6.0/gencove/tests/basespace/test_basespace_autoimports_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/basespace/test_basespace_biosamples_list.py` & `gencove-2.6.0/gencove/tests/basespace/test_basespace_biosamples_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/basespace/test_basespace_projects_import.py` & `gencove-2.6.0/gencove/tests/basespace/test_basespace_projects_import.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/basespace/test_basespace_projects_list.py` & `gencove-2.6.0/gencove/tests/basespace/test_basespace_projects_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/conftest.py` & `gencove-2.6.0/gencove/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/decorators.py` & `gencove-2.6.0/gencove/tests/decorators.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/download/test_cli_download.py` & `gencove-2.6.0/gencove/tests/download/test_cli_download.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/download/vcr/filters.py` & `gencove-2.6.0/gencove/tests/download/vcr/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/files/test_file_types_list.py` & `gencove-2.6.0/gencove/tests/files/test_file_types_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/filters.py` & `gencove-2.6.0/gencove/tests/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/projects/test_projects_batch_get.py` & `gencove-2.6.0/gencove/tests/projects/test_projects_batch_get.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/projects/test_projects_batch_types_list.py` & `gencove-2.6.0/gencove/tests/projects/test_projects_batch_types_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/projects/test_projects_batches_create.py` & `gencove-2.6.0/gencove/tests/projects/test_projects_batches_create.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/projects/test_projects_batches_list.py` & `gencove-2.6.0/gencove/tests/projects/test_projects_batches_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/projects/test_projects_create.py` & `gencove-2.6.0/gencove/tests/projects/test_projects_create.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/projects/test_projects_create_merged_vcf.py` & `gencove-2.6.0/gencove/tests/projects/test_projects_create_merged_vcf.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/projects/test_projects_delete_samples.py` & `gencove-2.6.0/gencove/tests/projects/test_projects_delete_samples.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/projects/test_projects_get_merged_vcf.py` & `gencove-2.6.0/gencove/tests/projects/test_projects_get_merged_vcf.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/projects/test_projects_import_existing_samples.py` & `gencove-2.6.0/gencove/tests/projects/test_projects_import_existing_samples.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/projects/test_projects_list.py` & `gencove-2.6.0/gencove/tests/projects/test_projects_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -255,14 +255,49 @@
                         get_pipeline_capabilities_response["name"],
                     ]
                 )
             )
         assert output_line.getvalue() == res.output.encode()
 
 
+@pytest.mark.vcr
+@assert_authorization
+def test_list_projects_with_capabilities(mocker, credentials, recording, vcr):
+    """Test projects being outputed to the shell."""
+    runner = CliRunner()
+    if not recording:
+        # Mock list_projects only if using the cassettes, since we mock the
+        # return value.
+        list_projects_response = get_vcr_response("/api/v2/projects/", vcr)
+        mocked_get_projects = mocker.patch.object(
+            APIClient,
+            "list_projects",
+            return_value=Projects(**list_projects_response),
+        )
+        get_pipeline_capabilities_response = get_vcr_response(
+            "/api/v2/pipeline-capabilities/", vcr, operator.contains
+        )
+        mocked_get_pipeline_capabilities = mocker.patch.object(
+            APIClient,
+            "get_pipeline_capabilities",
+            return_value=PipelineCapabilities(**get_pipeline_capabilities_response),
+        )
+    res = runner.invoke(list_projects, ["--include-capability", *credentials])
+    assert res.exit_code == 0
+    if not recording:
+        mocked_get_projects.assert_called_once()
+        projects = list_projects_response["results"]
+        assert mocked_get_pipeline_capabilities.call_count == len(projects)
+        assert "key" in get_pipeline_capabilities_response
+        projects = res.output.splitlines()
+        for project in projects:
+            # Confirm # of columns is correct
+            assert len(project.split("\t")) == 6
+
+
 # API responses may return new keys and values eventually
 MOCKED_PROJECTS_WITH_UNEXPECTED_KEYS = dict(
     meta=dict(next=None),
     results=[
         {
             "id": str(uuid4()),
             "name": "test\tproject",
```

### Comparing `gencove-2.5.2/gencove/tests/projects/test_projects_pipeline_capabilities_list.py` & `gencove-2.6.0/gencove/tests/projects/test_projects_pipeline_capabilities_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/projects/test_projects_pipelines_list.py` & `gencove-2.6.0/gencove/tests/projects/test_projects_pipelines_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/projects/test_projects_restore_samples.py` & `gencove-2.6.0/gencove/tests/projects/test_projects_restore_samples.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/projects/test_projects_run_prefix.py` & `gencove-2.6.0/gencove/tests/projects/test_projects_run_prefix.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/projects/test_projects_samples_list.py` & `gencove-2.6.0/gencove/tests/projects/test_projects_samples_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/projects/test_projects_status_merged_vcf.py` & `gencove-2.6.0/gencove/tests/projects/test_projects_status_merged_vcf.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/projects/vcr/filters.py` & `gencove-2.6.0/gencove/tests/projects/vcr/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/s3_imports/test_s3_autoimports_create.py` & `gencove-2.6.0/gencove/tests/s3_imports/test_s3_autoimports_create.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/s3_imports/test_s3_autoimports_list.py` & `gencove-2.6.0/gencove/tests/s3_imports/test_s3_autoimports_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/s3_imports/test_s3_uri_import.py` & `gencove-2.6.0/gencove/tests/s3_imports/test_s3_uri_import.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/samples/test_samples_download_file.py` & `gencove-2.6.0/gencove/tests/samples/test_samples_download_file.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/samples/test_samples_get_metadata.py` & `gencove-2.6.0/gencove/tests/samples/test_samples_get_metadata.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/samples/test_samples_set_metadata.py` & `gencove-2.6.0/gencove/tests/samples/test_samples_set_metadata.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/samples/vcr/filters.py` & `gencove-2.6.0/gencove/tests/samples/vcr/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/test_logger.py` & `gencove-2.6.0/gencove/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/test_utils.py` & `gencove-2.6.0/gencove/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/upload/test_cli_upload.py` & `gencove-2.6.0/gencove/tests/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/upload/vcr/filters.py` & `gencove-2.6.0/gencove/tests/upload/vcr/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/uploads/test_uploads_list.py` & `gencove-2.6.0/gencove/tests/uploads/test_uploads_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/utils.py` & `gencove-2.6.0/gencove/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/tests/webhook/test_webhook_verify.py` & `gencove-2.6.0/gencove/tests/webhook/test_webhook_verify.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove/utils.py` & `gencove-2.6.0/gencove/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/gencove.egg-info/PKG-INFO` & `gencove-2.6.0/gencove.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gencove
-Version: 2.5.2
+Version: 2.6.0
 Summary: Gencove API and CLI tool
 Home-page: http://docs.gencove.com
 Author: Tomaz Berisa
 License: Apache 2.0
 Description: # The Gencove CLI
         
         [![PyPI Latest Release](https://img.shields.io/pypi/v/gencove.svg)](https://pypi.org/project/gencove/)
```

### Comparing `gencove-2.5.2/gencove.egg-info/SOURCES.txt` & `gencove-2.6.0/gencove.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gencove-2.5.2/setup.py` & `gencove-2.6.0/setup.py`

 * *Files identical despite different names*

