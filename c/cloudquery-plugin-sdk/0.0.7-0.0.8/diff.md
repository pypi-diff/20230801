# Comparing `tmp/cloudquery-plugin-sdk-0.0.7.tar.gz` & `tmp/cloudquery-plugin-sdk-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudquery-plugin-sdk-0.0.7.tar", last modified: Sat Jul 29 19:42:17 2023, max compression
+gzip compressed data, was "cloudquery-plugin-sdk-0.0.8.tar", last modified: Tue Aug  1 13:01:21 2023, max compression
```

## Comparing `cloudquery-plugin-sdk-0.0.7.tar` & `cloudquery-plugin-sdk-0.0.8.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.463659 cloudquery-plugin-sdk-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-29 19:42:17.463659 cloudquery-plugin-sdk-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.447659 cloudquery-plugin-sdk-0.0.7/cloudquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.455659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.455659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/docs/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/docs/markdown_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.455659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.455659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/memdb/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/memdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/memdb/memdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.455659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/servers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/servers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.459659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/servers/discovery_v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/servers/discovery_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/servers/discovery_v1/discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.459659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/servers/plugin_v3/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/servers/plugin_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/servers/plugin_v3/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.459659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/message/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/message/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/message/write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.459659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.463659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/date32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/date64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/int.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/scalar_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/uint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.463659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scheduler/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scheduler/table_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.463659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/schema/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/schema/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/schema/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/schema/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.463659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/serve/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/serve/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.463659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/transformers/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/transformers/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.463659 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/types/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/types/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/types/uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:42:17.463659 cloudquery-plugin-sdk-0.0.7/cloudquery_plugin_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-29 19:42:17.000000 cloudquery-plugin-sdk-0.0.7/cloudquery_plugin_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-29 19:42:17.000000 cloudquery-plugin-sdk-0.0.7/cloudquery_plugin_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 19:42:17.000000 cloudquery-plugin-sdk-0.0.7/cloudquery_plugin_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 19:42:17.000000 cloudquery-plugin-sdk-0.0.7/cloudquery_plugin_sdk.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 19:42:17.000000 cloudquery-plugin-sdk-0.0.7/cloudquery_plugin_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-29 19:42:17.000000 cloudquery-plugin-sdk-0.0.7/cloudquery_plugin_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 19:42:17.000000 cloudquery-plugin-sdk-0.0.7/cloudquery_plugin_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 19:42:17.467659 cloudquery-plugin-sdk-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-29 19:41:46.000000 cloudquery-plugin-sdk-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.102550 cloudquery-plugin-sdk-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-01 13:01:21.102550 cloudquery-plugin-sdk-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.090550 cloudquery-plugin-sdk-0.0.8/cloudquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.090550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.090550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/docs/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/docs/markdown_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.094550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.094550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/memdb/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/memdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/memdb/memdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.094550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/servers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.094550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/servers/discovery_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/servers/discovery_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/servers/discovery_v1/discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.094550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/servers/plugin_v3/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/servers/plugin_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/servers/plugin_v3/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.094550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/message/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/message/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/message/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.094550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.098550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/date32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/date64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/scalar_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/uint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.098550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scheduler/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scheduler/table_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.098550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/schema/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/schema/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/schema/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/schema/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.098550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/serve/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.098550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/transformers/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/transformers/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.098550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/types/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/types/uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.102550 cloudquery-plugin-sdk-0.0.8/cloudquery_plugin_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-01 13:01:21.000000 cloudquery-plugin-sdk-0.0.8/cloudquery_plugin_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-01 13:01:21.000000 cloudquery-plugin-sdk-0.0.8/cloudquery_plugin_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:01:21.000000 cloudquery-plugin-sdk-0.0.8/cloudquery_plugin_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 13:01:21.000000 cloudquery-plugin-sdk-0.0.8/cloudquery_plugin_sdk.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:00:57.000000 cloudquery-plugin-sdk-0.0.8/cloudquery_plugin_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-01 13:01:21.000000 cloudquery-plugin-sdk-0.0.8/cloudquery_plugin_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 13:01:21.000000 cloudquery-plugin-sdk-0.0.8/cloudquery_plugin_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 13:01:21.102550 cloudquery-plugin-sdk-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/setup.py
```

### Comparing `cloudquery-plugin-sdk-0.0.7/PKG-INFO` & `cloudquery-plugin-sdk-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudquery-plugin-sdk
-Version: 0.0.7
+Version: 0.0.8
 Summary: CloudQuery Plugin SDK for Python
 Home-page: https://github.com/cloudquery/plugin-sdk-python
 Author: CloudQuery LTD
 Author-email: pypi-packages@cloudquery.io
 License: MPL-2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Intended Audience :: Developers
```

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/docs/generator.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/docs/generator.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/docs/markdown_templates.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/docs/markdown_templates.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/memdb/memdb.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/memdb/memdb.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/internal/servers/plugin_v3/plugin.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/servers/plugin_v3/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         for msg in self._plugin.sync(options):
             if isinstance(msg, SyncInsertMessage):
                 buf = arrow.record_to_bytes(msg.record)
                 yield plugin_pb2.Sync.Response(
                     insert=plugin_pb2.Sync.MessageInsert(record=buf)
                 )
             elif isinstance(msg, SyncMigrateTableMessage):
-                buf = arrow.schema_to_bytes(msg.schema)
+                buf = arrow.schema_to_bytes(msg.table)
                 yield plugin_pb2.Sync.Response(
                     migrate_table=plugin_pb2.Sync.MessageMigrateTable(table=buf)
                 )
             else:
                 # unknown sync message type
                 raise NotImplementedError()
```

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/message/write.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/message/write.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/plugin/plugin.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/binary.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/binary.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/bool.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/bool.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/date32.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/date32.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/date64.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/date64.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/float.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/float.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/int.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/int.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/json.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/json.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/list.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/list.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/scalar.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/scalar.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/scalar_factory.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/scalar_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import pyarrow as pa
-from .scalar import ScalarInvalidTypeError
+
+from cloudquery.sdk.types import UUIDType, JSONType
 from .binary import Binary
 from .bool import Bool
 from .date32 import Date32
 from .date64 import Date64
 from .float import Float
 from .int import Int
 from .list import List
+from .scalar import ScalarInvalidTypeError
 from .string import String
 from .timestamp import Timestamp
 from .uint import Uint
 from .uuid import UUID
-from cloudquery.sdk.types import UUIDType, JSONType
 
 
 class ScalarFactory:
     def __init__(self):
         pass
 
     def new_scalar(self, dt: pa.DataType):
@@ -81,13 +82,13 @@
         #     return ()
         # elif dt_id == pa.types.lib.Type_TIME32:
         #     return ()
         # elif dt_id == pa.types.lib.Type_TIME64:
         #     return ()
         elif dt_id == pa.types.lib.Type_TIMESTAMP:
             return Timestamp()
-        elif dt == UUIDType:
+        elif dt == UUIDType():
             return UUID()
-        elif dt == JSONType:
+        elif dt == JSONType():
             return String()
         else:
             raise ScalarInvalidTypeError("Invalid type {} for scalar".format(dt))
```

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/string.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/string.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/timestamp.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/timestamp.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/uint.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/uint.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/uuid.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/uuid.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scalar/vector.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/vector.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scheduler/scheduler.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scheduler/scheduler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-from typing import List, Generator, Any
 import queue
-import time
+from concurrent import futures
+from typing import List, Generator, Any
+
 import structlog
-from enum import Enum
-from cloudquery.sdk.schema import Table, Resource
+
 from cloudquery.sdk.message import (
     SyncMessage,
     SyncInsertMessage,
     SyncMigrateTableMessage,
 )
-from concurrent import futures
-from typing import Generator
+from cloudquery.sdk.schema import Resource
 from .table_resolver import TableResolver
-import traceback
 
 QUEUE_PER_WORKER = 100
 
 
 class ThreadPoolExecutorWithQueueSizeLimit(futures.ThreadPoolExecutor):
     def __init__(self, maxsize, *args, **kwargs):
         super(ThreadPoolExecutorWithQueueSizeLimit, self).__init__(*args, **kwargs)
@@ -170,15 +168,15 @@
             res.put(TableResolverStarted(total_table_resolvers))
 
     def sync(
         self, client, resolvers: List[TableResolver], deterministic_cq_id=False
     ) -> Generator[SyncMessage, None, None]:
         res = queue.Queue()
         for resolver in resolvers:
-            yield SyncMigrateTableMessage(schema=resolver.table.to_arrow_schema())
+            yield SyncMigrateTableMessage(table=resolver.table.to_arrow_schema())
         thread = futures.ThreadPoolExecutor()
         thread.submit(self._sync, client, resolvers, res, deterministic_cq_id)
         total_table_resolvers = 0
         finished_table_resolvers = 0
         while True:
             message = res.get()
             if type(message) == TableResolverStarted:
@@ -188,8 +186,8 @@
                 continue
             elif type(message) == TableResolverFinished:
                 finished_table_resolvers += 1
                 if total_table_resolvers == finished_table_resolvers:
                     break
                 continue
             yield message
-        thread.shutdown()
+        thread.shutdown(wait=True)
```

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/scheduler/table_resolver.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scheduler/table_resolver.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/schema/column.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/schema/column.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/schema/resource.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/schema/resource.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/schema/table.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/schema/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,17 +32,14 @@
         self.parent = parent
         self.relations = relations
         self.is_incremental = is_incremental
 
     def multiplex(self, client) -> List[Table]:
         raise [client]
 
-    def resolver(self, client: Client, parent=None) -> Generator[Any]:
-        raise NotImplementedError()
-
     def index_column(self, column_name: str) -> int:
         for i, column in enumerate(self.columns):
             if column.name == column_name:
                 return i
         raise ValueError(f"Column {column_name} not found")
 
     @property
```

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/serve/plugin.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/serve/plugin.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/transformers/openapi.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/transformers/openapi.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/types/json.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/types/json.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery/sdk/types/uuid.py` & `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/types/uuid.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery_plugin_sdk.egg-info/PKG-INFO` & `cloudquery-plugin-sdk-0.0.8/cloudquery_plugin_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudquery-plugin-sdk
-Version: 0.0.7
+Version: 0.0.8
 Summary: CloudQuery Plugin SDK for Python
 Home-page: https://github.com/cloudquery/plugin-sdk-python
 Author: CloudQuery LTD
 Author-email: pypi-packages@cloudquery.io
 License: MPL-2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Intended Audience :: Developers
```

### Comparing `cloudquery-plugin-sdk-0.0.7/cloudquery_plugin_sdk.egg-info/SOURCES.txt` & `cloudquery-plugin-sdk-0.0.8/cloudquery_plugin_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.7/setup.py` & `cloudquery-plugin-sdk-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,34 @@
 
 name = "cloudquery-plugin-sdk"
 
 description = "CloudQuery Plugin SDK for Python"
 
 dependencies = [
     "cloudquery-plugin-pb==0.0.14",
-    "pyarrow==12.0.1",
+    "exceptiongroup==1.1.2",
+    "black==23.7.0",
+    "grpcio==1.56.2",
+    "grpcio-tools==1.56.2",
+    "iniconfig==2.0.0",
     "Jinja2==3.1.2",
+    "MarkupSafe==2.1.3",
+    "numpy==1.25.2",
+    "packaging==23.1",
+    "pandas==2.0.3",
+    "pluggy==1.2.0",
+    "protobuf==4.23.4",
+    "pyarrow==12.0.1",
+    "pytest==7.4.0",
+    "python-dateutil==2.8.2",
+    "pytz==2023.3",
+    "six==1.16.0",
     "structlog==23.1.0",
+    "tomli==2.0.1",
+    "tzdata==2023.3",
 ]
 url = "https://github.com/cloudquery/plugin-sdk-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 long_description = """
 CloudQuery Plugin SDK for Python
@@ -32,15 +49,15 @@
 packages = [
     package
     for package in setuptools.PEP420PackageFinder.find()
     if package.startswith("cloudquery")
 ]
 setuptools.setup(
     name=name,
-    version="0.0.7",
+    version="0.0.8",
     description=description,
     long_description=long_description,
     author="CloudQuery LTD",
     author_email="pypi-packages@cloudquery.io",
     license="MPL-2.0",
     url=url,
     classifiers=[
```

