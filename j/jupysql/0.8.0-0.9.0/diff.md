# Comparing `tmp/jupysql-0.8.0.tar.gz` & `tmp/jupysql-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupysql-0.8.0.tar", last modified: Tue Jul 18 14:57:10 2023, max compression
+gzip compressed data, was "jupysql-0.9.0.tar", last modified: Tue Aug  1 14:24:59 2023, max compression
```

## Comparing `jupysql-0.8.0.tar` & `jupysql-0.9.0.tar`

### file list

```diff
@@ -1,67 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.742658 jupysql-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-07-18 14:56:54.000000 jupysql-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-18 14:56:54.000000 jupysql-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-18 14:57:10.742658 jupysql-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-18 14:56:54.000000 jupysql-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-18 14:56:54.000000 jupysql-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-18 14:57:10.742658 jupysql-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-18 14:56:54.000000 jupysql-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.734658 jupysql-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.734658 jupysql-0.8.0/src/jupysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-18 14:57:10.000000 jupysql-0.8.0/src/jupysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-18 14:57:10.000000 jupysql-0.8.0/src/jupysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:57:10.000000 jupysql-0.8.0/src/jupysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:57:10.000000 jupysql-0.8.0/src/jupysql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-18 14:57:10.000000 jupysql-0.8.0/src/jupysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-18 14:57:10.000000 jupysql-0.8.0/src/jupysql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.738658 jupysql-0.8.0/src/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/_testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.738658 jupysql-0.8.0/src/sql/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/cmd/cmd_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/cmd/columns.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/cmd/explore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/cmd/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/cmd/snippets.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/cmd/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/cmd/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/column_guesser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    23034 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/error_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.738658 jupysql-0.8.0/src/sql/ggplot/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/ggplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/ggplot/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/ggplot/facet_wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.742658 jupysql-0.8.0/src/sql/ggplot/geom/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/ggplot/geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/ggplot/geom/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/ggplot/geom/geom_boxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/ggplot/geom/geom_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/ggplot/ggplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    16093 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)    21240 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/magic_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/magic_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    25369 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/query_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    24152 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/store.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.742658 jupysql-0.8.0/src/sql/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.742658 jupysql-0.8.0/src/sql/widgets/table_widget/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/widgets/table_widget/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.742658 jupysql-0.8.0/src/sql/widgets/table_widget/css/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/widgets/table_widget/css/tableWidget.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.742658 jupysql-0.8.0/src/sql/widgets/table_widget/js/
--rw-r--r--   0 runner    (1001) docker     (123)    13553 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/widgets/table_widget/js/tableWidget.js
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/widgets/table_widget/table_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/widgets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:24:59.389218 jupysql-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-08-01 14:24:37.000000 jupysql-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 14:24:37.000000 jupysql-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-08-01 14:24:59.389218 jupysql-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-08-01 14:24:37.000000 jupysql-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-08-01 14:24:37.000000 jupysql-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-01 14:24:59.389218 jupysql-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-08-01 14:24:37.000000 jupysql-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:24:59.381218 jupysql-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:24:59.381218 jupysql-0.9.0/src/jupysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-08-01 14:24:59.000000 jupysql-0.9.0/src/jupysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-08-01 14:24:59.000000 jupysql-0.9.0/src/jupysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:24:59.000000 jupysql-0.9.0/src/jupysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:24:59.000000 jupysql-0.9.0/src/jupysql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-01 14:24:59.000000 jupysql-0.9.0/src/jupysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-01 14:24:59.000000 jupysql-0.9.0/src/jupysql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:24:59.385218 jupysql-0.9.0/src/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12981 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:24:59.385218 jupysql-0.9.0/src/sql/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/cmd/cmd_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/cmd/columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/cmd/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/cmd/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/cmd/snippets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/cmd/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/cmd/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/column_guesser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:24:59.385218 jupysql-0.9.0/src/sql/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31345 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/connection/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/error_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:24:59.385218 jupysql-0.9.0/src/sql/ggplot/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/ggplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/ggplot/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/ggplot/facet_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:24:59.385218 jupysql-0.9.0/src/sql/ggplot/geom/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/ggplot/geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/ggplot/geom/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/ggplot/geom/geom_boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/ggplot/geom/geom_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/ggplot/ggplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16042 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23203 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/magic_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/magic_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26311 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/query_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:24:59.385218 jupysql-0.9.0/src/sql/run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/run/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/run/pgspecial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17146 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/run/resultset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/run/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/run/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13630 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:24:59.385218 jupysql-0.9.0/src/sql/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:24:59.385218 jupysql-0.9.0/src/sql/widgets/table_widget/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/widgets/table_widget/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:24:59.385218 jupysql-0.9.0/src/sql/widgets/table_widget/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/widgets/table_widget/css/tableWidget.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:24:59.385218 jupysql-0.9.0/src/sql/widgets/table_widget/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    13553 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/widgets/table_widget/js/tableWidget.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/widgets/table_widget/table_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-08-01 14:24:37.000000 jupysql-0.9.0/src/sql/widgets/utils.py
```

### Comparing `jupysql-0.8.0/LICENSE` & `jupysql-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupysql-0.8.0/PKG-INFO` & `jupysql-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql
-Version: 0.8.0
+Version: 0.9.0
 Summary: Better SQL in Jupyter
 Home-page: https://github.com/ploomber/jupysql
 Author: Ploomber
 Author-email: contact@ploomber.io
 Project-URL: Source, https://github.com/ploomber/jupysql
 Keywords: database ipython postgresql mysql duckdb
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupysql Version: 0.8.0 Summary: Better SQL in
+Metadata-Version: 2.1 Name: jupysql Version: 0.9.0 Summary: Better SQL in
 Jupyter Home-page: https://github.com/ploomber/jupysql Author: Ploomber Author-
 email: contact@ploomber.io Project-URL: Source, https://github.com/ploomber/
 jupysql Keywords: database ipython postgresql mysql duckdb Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Topic ::
 Database Classifier: Topic :: Database :: Front-Ends Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `jupysql-0.8.0/README.md` & `jupysql-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `jupysql-0.8.0/pyproject.toml` & `jupysql-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupysql-0.8.0/setup.py` & `jupysql-0.9.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -47,26 +47,30 @@
     "matplotlib",
     "black",
     # for %%sql --interact
     "ipywidgets",
     # for running tests for %sqlcmd explore --table
     "js2py",
     "jupysql-plugin",
+    # for monitoring access to files
+    "psutil",
 ]
 
 # dependencies for running integration tests
 INTEGRATION = [
     "dockerctx",
     "pyarrow",
     "psycopg2-binary",
     "pymysql",
     "pgspecial==2.0.1",
     "pyodbc",
     "snowflake-sqlalchemy",
     "oracledb",
+    "sqlalchemy-pytds",
+    "python-tds",
 ]
 
 setup(
     name="jupysql",
     version=VERSION,
     description="Better SQL in Jupyter",
     long_description=README,
```

### Comparing `jupysql-0.8.0/src/jupysql.egg-info/PKG-INFO` & `jupysql-0.9.0/src/jupysql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql
-Version: 0.8.0
+Version: 0.9.0
 Summary: Better SQL in Jupyter
 Home-page: https://github.com/ploomber/jupysql
 Author: Ploomber
 Author-email: contact@ploomber.io
 Project-URL: Source, https://github.com/ploomber/jupysql
 Keywords: database ipython postgresql mysql duckdb
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupysql Version: 0.8.0 Summary: Better SQL in
+Metadata-Version: 2.1 Name: jupysql Version: 0.9.0 Summary: Better SQL in
 Jupyter Home-page: https://github.com/ploomber/jupysql Author: Ploomber Author-
 email: contact@ploomber.io Project-URL: Source, https://github.com/ploomber/
 jupysql Keywords: database ipython postgresql mysql duckdb Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Topic ::
 Database Classifier: Topic :: Database :: Front-Ends Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `jupysql-0.8.0/src/jupysql.egg-info/SOURCES.txt` & `jupysql-0.9.0/src/jupysql.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -11,45 +11,51 @@
 src/jupysql.egg-info/requires.txt
 src/jupysql.egg-info/top_level.txt
 src/sql/__init__.py
 src/sql/_patch.py
 src/sql/_testing.py
 src/sql/column_guesser.py
 src/sql/command.py
-src/sql/connection.py
 src/sql/display.py
 src/sql/error_message.py
 src/sql/exceptions.py
 src/sql/inspect.py
 src/sql/magic.py
 src/sql/magic_cmd.py
 src/sql/magic_plot.py
 src/sql/parse.py
 src/sql/plot.py
 src/sql/query_util.py
-src/sql/run.py
 src/sql/store.py
 src/sql/telemetry.py
 src/sql/util.py
 src/sql/warnings.py
 src/sql/cmd/__init__.py
 src/sql/cmd/cmd_utils.py
 src/sql/cmd/columns.py
 src/sql/cmd/explore.py
 src/sql/cmd/profile.py
 src/sql/cmd/snippets.py
 src/sql/cmd/tables.py
 src/sql/cmd/test.py
+src/sql/connection/__init__.py
+src/sql/connection/connection.py
 src/sql/ggplot/__init__.py
 src/sql/ggplot/aes.py
 src/sql/ggplot/facet_wrap.py
 src/sql/ggplot/ggplot.py
 src/sql/ggplot/geom/__init__.py
 src/sql/ggplot/geom/geom.py
 src/sql/ggplot/geom/geom_boxplot.py
 src/sql/ggplot/geom/geom_histogram.py
+src/sql/run/__init__.py
+src/sql/run/csv.py
+src/sql/run/pgspecial.py
+src/sql/run/resultset.py
+src/sql/run/run.py
+src/sql/run/table.py
 src/sql/widgets/__init__.py
 src/sql/widgets/utils.py
 src/sql/widgets/table_widget/__init__.py
 src/sql/widgets/table_widget/table_widget.py
 src/sql/widgets/table_widget/css/tableWidget.css
 src/sql/widgets/table_widget/js/tableWidget.js
```

### Comparing `jupysql-0.8.0/src/jupysql.egg-info/requires.txt` & `jupysql-0.9.0/src/jupysql.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 duckdb-engine
 pyodbc
 matplotlib
 black
 ipywidgets
 js2py
 jupysql-plugin
+psutil
 
 [integration]
 flake8
 pytest
 pandas
 polars==0.17.2
 pyarrow
@@ -45,13 +46,16 @@
 duckdb-engine
 pyodbc
 matplotlib
 black
 ipywidgets
 js2py
 jupysql-plugin
+psutil
 dockerctx
 psycopg2-binary
 pymysql
 pgspecial==2.0.1
 snowflake-sqlalchemy
 oracledb
+sqlalchemy-pytds
+python-tds
```

### Comparing `jupysql-0.8.0/src/sql/_patch.py` & `jupysql-0.9.0/src/sql/_patch.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.8.0/src/sql/_testing.py` & `jupysql-0.9.0/src/sql/_testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+import os
 from contextlib import contextmanager
 import sys
 import time
 
 from sqlalchemy.engine import URL
-import os
 import sqlalchemy
+from IPython.core.interactiveshell import InteractiveShell
 
 from ploomber_core.dependencies import requires
 
 # SQLite and DuckDB do not require Docker, so we make docker packages optional
 # in case we want to run those tests
 
 try:
@@ -21,28 +22,62 @@
 except ModuleNotFoundError:
     docker = None
 
 
 TMP_DIR = "tmp"
 
 
+class TestingShell(InteractiveShell):
+    """
+    A custom InteractiveShell that raises exceptions instead of silently suppressing
+    them.
+    """
+
+    def run_cell(self, *args, **kwargs):
+        result = super().run_cell(*args, **kwargs)
+        result.raise_error()
+        return result
+
+
 class DatabaseConfigHelper:
     @staticmethod
     def get_database_config(database):
         return databaseConfig[database]
 
     @staticmethod
     def get_database_url(database):
         return _get_database_url(database)
 
     @staticmethod
     def get_tmp_dir():
         return TMP_DIR
 
 
+mssql_base = {
+    "username": "sa",
+    "password": "Ploomber_App@Root_Password",
+    "database": "master",
+    "host": "localhost",
+    "port": "1433",
+    "query": {
+        "driver": "ODBC Driver 18 for SQL Server",
+        "Encrypt": "yes",
+        "TrustServerCertificate": "yes",
+    },
+    "docker_ct": {
+        "name": "MSSQL",
+        "image": "mcr.microsoft.com/azure-sql-edge",
+        "ports": {1433: 1433},
+    },
+    "alias": "MSSQLTest",
+}
+
+mssql_pyobdc = {**mssql_base, "drivername": "mssql+pyodbc"}
+mssql_pytds = {**mssql_base, "drivername": "mssql+pytds"}
+
 databaseConfig = {
     "postgreSQL": {
         "drivername": "postgresql",
         "username": "ploomber_app",
         "password": "ploomber_app_password",
         "database": "db",
         "host": "localhost",
@@ -103,33 +138,16 @@
         "password": None,
         "database": "/{}/db-duckdb".format(TMP_DIR),
         "host": None,
         "port": None,
         "alias": "duckDBTest",
         "query": {},
     },
-    "MSSQL": {
-        "drivername": "mssql+pyodbc",
-        "username": "sa",
-        "password": "Ploomber_App@Root_Password",
-        "database": "master",
-        "host": "localhost",
-        "port": "1433",
-        "query": {
-            "driver": "ODBC Driver 18 for SQL Server",
-            "Encrypt": "yes",
-            "TrustServerCertificate": "yes",
-        },
-        "docker_ct": {
-            "name": "MSSQL",
-            "image": "mcr.microsoft.com/azure-sql-edge",
-            "ports": {1433: 1433},
-        },
-        "alias": "MSSQLTest",
-    },
+    "MSSQL": mssql_pyobdc,
+    "mssql_pytds": mssql_pytds,
     "Snowflake": {
         "drivername": "snowflake",
         "username": os.getenv("SF_USERNAME"),
         "password": os.getenv("SF_PASSWORD"),
         # database/schema
         "database": os.getenv("SF_DATABASE", "JUPYSQL_INTEGRATION_TESTING/GENERAL"),
         "host": "lpb17716.us-east-1",
@@ -194,14 +212,16 @@
     t0 = time.time()
     while time.time() - t0 < timeout:
         try:
             eng = sqlalchemy.create_engine(_get_database_url(database)).connect()
             eng.close()
             print(f"{database} is initialized successfully")
             return True
+        except ModuleNotFoundError:
+            raise
         except Exception as e:
             print(type(e))
             errors.append(str(e))
 
         time.sleep(poll_freq)
 
     # print all the errors so we know what's going on since failing to connect might be
```

### Comparing `jupysql-0.8.0/src/sql/cmd/columns.py` & `jupysql-0.9.0/src/sql/cmd/columns.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.8.0/src/sql/cmd/explore.py` & `jupysql-0.9.0/src/sql/cmd/explore.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.8.0/src/sql/cmd/profile.py` & `jupysql-0.9.0/src/sql/cmd/profile.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.8.0/src/sql/cmd/snippets.py` & `jupysql-0.9.0/src/sql/cmd/snippets.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.8.0/src/sql/cmd/tables.py` & `jupysql-0.9.0/src/sql/cmd/tables.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.8.0/src/sql/cmd/test.py` & `jupysql-0.9.0/src/sql/cmd/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from sql import exceptions
 import sql.connection
-from sqlalchemy import text
 from sqlglot import select, condition
 from prettytable import PrettyTable
 from sql.cmd.cmd_utils import CmdParser
 
 
 def return_test_results(args, conn, query):
+    columns = []
+
     try:
-        columns = []
-        column_data = conn.execute(text(query)).cursor.description
-        res = conn.execute(text(query)).fetchall()
+        column_data = conn.execute(query).cursor.description
+        res = conn.execute(query).fetchall()
         for column in column_data:
             columns.append(column[0])
         res = [columns, *res]
         return res
     except Exception as e:
         if "column" in str(e):
             raise exceptions.UsageError(
@@ -157,24 +157,24 @@
         )
     elif args.less_than and args.less_than_or_equal:
         return exceptions.UsageError(
             "You cannot use both less and less than "
             "or equal to arguments at the same time."
         )
 
-    conn = sql.connection.Connection.current.session
+    conn = sql.connection.ConnectionManager.current
     result_dict = run_each_individually(args, conn)
 
     if any(len(rows) > 1 for rows in list(result_dict.values())):
         for comparator, rows in result_dict.items():
             if len(rows) > 1:
                 print(f"\n{comparator}:\n")
                 _pretty = PrettyTable()
                 _pretty.field_names = rows[0]
                 for row in rows[1:]:
                     _pretty.add_row(row)
                 print(_pretty)
         raise exceptions.UsageError(
-            "The above values do not not match your test requirements."
+            "The above values do not match your test requirements."
         )
     else:
         return True
```

### Comparing `jupysql-0.8.0/src/sql/column_guesser.py` & `jupysql-0.9.0/src/sql/column_guesser.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.8.0/src/sql/command.py` & `jupysql-0.9.0/src/sql/command.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from pathlib import Path
 from IPython.core.magic_arguments import parse_argstring
 from jinja2 import Template
 
 from sqlalchemy.engine import Engine
 
-from sql import parse
+from sql import parse, exceptions
 from sql.store import store
-from sql.connection import Connection
+from sql.connection import ConnectionManager, is_pep249_compliant
 
 
 class SQLPlotCommand:
     def __init__(self, magic, line) -> None:
         self.args = parse_argstring(magic.execute, line)
 
 
@@ -24,42 +25,49 @@
         self._cell = cell
 
         self.args = parse.magic_args(magic.execute, line)
         # self.args.line (everything that appears after %sql/%%sql in the first line)
         # is split in tokens (delimited by spaces), this checks if we have one arg
         one_arg = len(self.args.line) == 1
 
-        is_dbapi_connection_ = (
-            Connection.is_dbapi_connection(user_ns.get(self.args.line[0], False))
-            if len(self.args.line) > 0
-            else False
-        )
+        # NOTE: this is only used to determine if what the user passed looks like a
+        # connection, we can simplify it
+        if len(self.args.line) > 0 and self.args.line[0] in user_ns:
+            conn = user_ns[self.args.line[0]]
+
+            is_dbapi_connection_ = is_pep249_compliant(conn)
+        else:
+            is_dbapi_connection_ = False
 
         if (
             one_arg
             and self.args.line[0] in user_ns
             and (isinstance(user_ns[self.args.line[0]], Engine) or is_dbapi_connection_)
         ):
             line_for_command = []
             add_conn = True
         else:
             line_for_command = self.args.line
             add_conn = False
 
-        if one_arg and self.args.line[0] in Connection.connections:
+        if one_arg and self.args.line[0] in ConnectionManager.connections:
             line_for_command = []
             add_alias = True
         else:
             add_alias = False
 
         self.command_text = " ".join(line_for_command) + "\n" + cell
 
         if self.args.file:
-            with open(self.args.file, "r") as infile:
-                self.command_text = infile.read() + "\n" + self.command_text
+            try:
+                file_contents = Path(self.args.file).read_text()
+            except FileNotFoundError as e:
+                raise exceptions.FileNotFoundError(str(e)) from e
+
+            self.command_text = file_contents + "\n" + self.command_text
 
         self.parsed = parse.parse(self.command_text, magic)
 
         self.parsed["sql_original"] = self.parsed["sql"] = self._var_expand(
             self.parsed["sql"], user_ns, magic
         )
```

### Comparing `jupysql-0.8.0/src/sql/display.py` & `jupysql-0.9.0/src/sql/display.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 A module to display confirmation messages and contextual information to the user
 """
 import html
 
 from prettytable import PrettyTable
-from IPython.display import display
+from IPython.display import display, HTML
 
 
 class Table:
     """Provides a txt and html representation of tabular data"""
 
     TITLE = ""
 
@@ -86,7 +86,17 @@
     """Display a generic message"""
     display(Message(message))
 
 
 def message_success(message):
     """Display a success message"""
     display(Message(message, style="color: green"))
+
+
+def message_html(message):
+    """Display a message as HTML"""
+    display(HTML(str(Message(message))))
+
+
+def table(headers, rows):
+    """Display a table"""
+    display(Table(headers, rows))
```

### Comparing `jupysql-0.8.0/src/sql/error_message.py` & `jupysql-0.9.0/src/sql/error_message.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ORIGINAL_ERROR = "\nOriginal error message from DB driver:\n"
 CTE_MSG = (
     "If using snippets, you may pass the --with argument explicitly.\n"
-    "For more details please refer : "
+    "For more details please refer: "
     "https://jupysql.ploomber.io/en/latest/compose.html#with-argument"
 )
 
 
 def _is_syntax_error(error):
     """
     Function to detect whether error message from DB driver
```

### Comparing `jupysql-0.8.0/src/sql/exceptions.py` & `jupysql-0.9.0/src/sql/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+"""
+In most scenarios, users don't care about the full Python traceback because it's
+irrelevant to them (they run SQL, not Python code). Hence, when raising errors,
+we only display the error message. This is possible via IPython.core.error.UsageError:
+IPython/Jupyter automatically detect this error and hide the traceback.
+Unfortunately, IPython.core.error.UsageError isn't the most appropriate error type for
+all scenarios, so we define our own error types here. The main caveat is that due to a
+bug in IPython (https://github.com/ipython/ipython/issues/14024), subclassing
+IPython.core.error.UsageError doesn't work, so `exception_factory` is a workaround
+to create new errors that are IPython.core.error.UsageError but with a different name.
+
+"""
 from IPython.core import error
 
 
 def exception_factory(name):
     def _error(message):
         exc = error.UsageError(message)
         exc.error_type = name
@@ -22,13 +34,19 @@
 
 # the following exceptions should be called instead of the Python built-in ones,
 # for guidelines on when to use them:
 # https://docs.python.org/3/library/exceptions.html#bltin-exceptions
 TypeError = exception_factory("TypeError")
 RuntimeError = exception_factory("RuntimeError")
 ValueError = exception_factory("ValueError")
-
+FileNotFoundError = exception_factory("FileNotFoundError")
 
 # The following are internal exceptions that should not be raised directly
 
 # raised internally when the user chooses a table that doesn't exist
 TableNotFoundError = exception_factory("TableNotFoundError")
+
+# raise it when there is an error in parsing pyproject.toml file
+ConfigurationError = exception_factory("ConfigurationError")
+
+
+InvalidQueryParameters = exception_factory("InvalidQueryParameters")
```

### Comparing `jupysql-0.8.0/src/sql/ggplot/facet_wrap.py` & `jupysql-0.9.0/src/sql/ggplot/facet_wrap.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             SELECT
             distinct ({{column}})
             FROM "{{table}}"
             """
         )
         query = template.render(table=table, column=column)
 
-        conn = sql.connection.Connection.current
+        conn = sql.connection.ConnectionManager.current
 
         values = conn.execute(query, with_).fetchall()
         # Added to make histogram more inclusive to NULLs
         # Filter out NULL values
         # If value[0] is NULL we skip it
         values = [value for value in values if value[0] is not None]
         n_plots = len(values)
```

### Comparing `jupysql-0.8.0/src/sql/ggplot/geom/geom_histogram.py` & `jupysql-0.9.0/src/sql/ggplot/geom/geom_histogram.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.8.0/src/sql/ggplot/ggplot.py` & `jupysql-0.9.0/src/sql/ggplot/ggplot.py`

 * *Files 11% similar despite different names*

```diff
@@ -66,17 +66,19 @@
                 self.table, other.facet, with_=self.with_
             )
 
             for i, value in enumerate(values):
                 ax_ = self.figure.add_subplot(n_rows, n_cols, i + 1)
                 facet_key_val = {"key": other.facet, "value": value[0]}
                 self.geom.draw(self, ax_, facet_key_val)
+                handles, labels = ax_.get_legend_handles_labels()
                 ax_.set_title(value[0])
                 ax_.tick_params(axis="both", labelsize=7)
-                ax_.legend(prop={"size": 10})
+                # reverses legend order so alphabetically first goes on top
+                ax_.legend(handles[::-1], labels[::-1], prop={"size": 10})
                 if other.legend is False:
                     plt.legend("", frameon=False)
                 self.axs.append(ax_)
 
         return self.figure
 
     def get_base(self, object) -> str:
```

### Comparing `jupysql-0.8.0/src/sql/inspect.py` & `jupysql-0.9.0/src/sql/inspect.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from sqlalchemy import inspect
 from prettytable import PrettyTable
 from ploomber_core.exceptions import modify_exceptions
-from sql.connection import Connection
+from sql.connection import ConnectionManager
 from sql.telemetry import telemetry
 from sql import exceptions
-import sql.run
 import math
 from sql import util
 from IPython.core.display import HTML
 import uuid
 
 
 def _get_inspector(conn):
     if conn:
         return inspect(conn)
 
-    if not Connection.current:
+    if not ConnectionManager.current:
         raise exceptions.RuntimeError("No active connection")
     else:
-        return inspect(Connection.current.session)
+        return inspect(ConnectionManager.current.connection_sqlalchemy)
 
 
 class DatabaseInspection:
     def __repr__(self) -> str:
         return self._table_txt
 
     def _repr_html_(self) -> str:
@@ -232,50 +231,49 @@
 
     def __init__(self, table_name, schema=None) -> None:
         util.is_table_exists(table_name, schema)
 
         if schema:
             table_name = f"{schema}.{table_name}"
 
-        columns_query_result = sql.run.raw_run(
-            Connection.current, f"SELECT * FROM {table_name} WHERE 1=0"
-        )
-        if Connection.is_dbapi_connection():
+        conn = ConnectionManager.current
+
+        columns_query_result = conn.raw_execute(f"SELECT * FROM {table_name} WHERE 1=0")
+        if ConnectionManager.current.is_dbapi_connection:
             columns = [i[0] for i in columns_query_result.description]
         else:
             columns = columns_query_result.keys()
 
         table_stats = dict({})
         columns_to_include_in_report = set()
         columns_with_styles = []
         message_check = False
 
         for i, column in enumerate(columns):
             table_stats[column] = dict()
 
             # check the datatype of a column
             try:
-                result = sql.run.raw_run(
-                    Connection.current, f"""SELECT {column} FROM {table_name} LIMIT 1"""
+                result = ConnectionManager.current.raw_execute(
+                    f"""SELECT {column} FROM {table_name} LIMIT 1"""
                 ).fetchone()
 
                 value = result[0]
                 is_numeric = isinstance(value, (int, float)) or (
                     isinstance(value, str) and _is_numeric(value)
                 )
             except ValueError:
                 is_numeric = True
 
             if _is_numeric_as_str(column, value):
                 columns_with_styles.append(i + 1)
                 message_check = True
             # Note: index is reserved word in sqlite
             try:
-                result_col_freq_values = sql.run.raw_run(
-                    Connection.current,
+                result_col_freq_values = ConnectionManager.current.raw_execute(
                     f"""SELECT DISTINCT {column} as top,
                     COUNT({column}) as frequency FROM {table_name}
                     GROUP BY top ORDER BY frequency Desc""",
                 ).fetchall()
 
                 table_stats[column]["freq"] = result_col_freq_values[0][1]
                 table_stats[column]["top"] = result_col_freq_values[0][0]
@@ -283,16 +281,15 @@
                 columns_to_include_in_report.update(["freq", "top"])
 
             except Exception:
                 pass
 
             try:
                 # get all non None values, min, max and avg.
-                result_value_values = sql.run.raw_run(
-                    Connection.current,
+                result_value_values = ConnectionManager.current.raw_execute(
                     f"""
                     SELECT MIN({column}) AS min,
                     MAX({column}) AS max,
                     COUNT({column}) AS count
                     FROM {table_name}
                     WHERE {column} IS NOT NULL
                     """,
@@ -307,31 +304,29 @@
                 columns_to_include_in_report.update(["count", "min", "max"])
 
             except Exception:
                 pass
 
             try:
                 # get unique values
-                result_value_values = sql.run.raw_run(
-                    Connection.current,
+                result_value_values = ConnectionManager.current.raw_execute(
                     f"""
                     SELECT
                     COUNT(DISTINCT {column}) AS unique_count
                     FROM {table_name}
                     WHERE {column} IS NOT NULL
                     """,
                 ).fetchall()
                 table_stats[column]["unique"] = result_value_values[0][0]
                 columns_to_include_in_report.update(["unique"])
             except Exception:
                 pass
 
             try:
-                results_avg = sql.run.raw_run(
-                    Connection.current,
+                results_avg = ConnectionManager.current.raw_execute(
                     f"""
                                 SELECT AVG({column}) AS avg
                                 FROM {table_name}
                                 WHERE {column} IS NOT NULL
                                 """,
                 ).fetchall()
 
@@ -342,16 +337,15 @@
                 table_stats[column]["mean"] = math.nan
 
             # These keys are numeric and work only on duckdb
             special_numeric_keys = ["std", "25%", "50%", "75%"]
 
             try:
                 # Note: stddev_pop and PERCENTILE_DISC will work only on DuckDB
-                result = sql.run.raw_run(
-                    Connection.current,
+                result = ConnectionManager.current.raw_execute(
                     f"""
                     SELECT
                         stddev_pop({column}) as key_std,
                         percentile_disc(0.25) WITHIN GROUP
                         (ORDER BY {column}) as key_25,
                         percentile_disc(0.50) WITHIN GROUP
                         (ORDER BY {column}) as key_50,
@@ -424,16 +418,16 @@
             warning_background = "#FFFFCC"
             warning_title = "Warning: "
         else:
             message_content = ""
             warning_background = "white"
             warning_title = ""
 
-        database = Connection.current.url
-        db_driver = Connection.current._get_curr_sqlalchemy_connection_info()["driver"]
+        database = ConnectionManager.current.url
+        db_driver = ConnectionManager.current._get_database_information()["driver"]
         if "duckdb" in database:
             db_message = ""
         else:
             db_message = f"""Following statistics are not available in
             {db_driver}: STD, 25%, 50%, 75%"""
 
         db_html = (
```

### Comparing `jupysql-0.8.0/src/sql/magic.py` & `jupysql-0.9.0/src/sql/magic.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,36 +11,43 @@
     cell_magic,
     line_magic,
     magics_class,
     needs_local_scope,
     no_var_expand,
 )
 from IPython.core.magic_arguments import argument, magic_arguments, parse_argstring
-from sqlalchemy.exc import OperationalError, ProgrammingError, DatabaseError
+from sqlalchemy.exc import (
+    OperationalError,
+    ProgrammingError,
+    DatabaseError,
+    StatementError,
+)
+from traitlets.config.configurable import Configurable
+from traitlets import Bool, Int, TraitError, Unicode, Dict, observe, validate
 
 import warnings
 import shlex
 from difflib import get_close_matches
 import sql.connection
 import sql.parse
-import sql.run
+from sql.run.run import run_statements
 from sql.parse import _option_strings_from_parser
 from sql import display, exceptions
 from sql.store import store
 from sql.command import SQLCommand
 from sql.magic_plot import SqlPlotMagic
 from sql.magic_cmd import SqlCmdMagic
 from sql._patch import patch_ipython_usage_error
-from sql import query_util
+from sql import query_util, util
 from sql.util import get_suggestions_message, pretty_print
-from ploomber_core.dependencies import check_installed
-
+from sql.exceptions import RuntimeError
 from sql.error_message import detail
-from traitlets.config.configurable import Configurable
-from traitlets import Bool, Int, TraitError, Unicode, Dict, observe, validate
+
+
+from ploomber_core.dependencies import check_installed
 
 
 try:
     from pandas.core.frame import DataFrame, Series
 except ModuleNotFoundError:
     DataFrame = None
     Series = None
@@ -146,14 +153,23 @@
         help="Path to DSN file. "
         "When the first argument is of the form [section], "
         "a sqlalchemy connection string is formed from the "
         "matching section in the DSN file.",
     )
     autocommit = Bool(True, config=True, help="Set autocommit mode")
 
+    named_parameters = Bool(
+        False,
+        config=True,
+        help=(
+            "Allow named parameters in queries "
+            "(i.e., 'SELECT * FROM foo WHERE bar = :bar')"
+        ),
+    )
+
     @telemetry.log_call("init")
     def __init__(self, shell):
         self._store = store
 
         Configurable.__init__(self, config=shell.config)
         Magics.__init__(self, shell=shell)
 
@@ -216,33 +232,31 @@
                         "Unrecognized argument(s): {}".format(check_argument)
                     )
 
     def _error_handling(self, e, query):
         detailed_msg = detail(e)
         if self.short_errors:
             if detailed_msg is not None:
-                err = exceptions.UsageError(detailed_msg)
-                raise err
+                raise exceptions.RuntimeError(detailed_msg) from e
                 # TODO: move to error_messages.py
                 # Added here due to circular dependency issue (#545)
             elif "no such table" in str(e):
                 tables = query_util.extract_tables_from_query(query)
                 for table in tables:
                     suggestions = get_close_matches(table, list(self._store))
                     err_message = f"There is no table with name {table!r}."
                     # with_message = "Alternatively, please specify table
                     # name using --with argument"
                     if len(suggestions) > 0:
                         suggestions_message = get_suggestions_message(suggestions)
                         raise exceptions.TableNotFoundError(
                             f"{err_message}{suggestions_message}"
-                        )
-                display.message(str(e))
-            else:
-                display.message(str(e))
+                        ) from e
+
+            raise RuntimeError(str(e)) from e
         else:
             if detailed_msg is not None:
                 display.message(detailed_msg)
             e.modify_exception = True
             raise e
 
     @no_var_expand
@@ -356,25 +370,26 @@
         return self._execute(
             line=line, cell=cell, local_ns=local_ns, is_interactive_mode=False
         )
 
     @telemetry.log_call("execute", payload=True)
     @modify_exceptions
     def _execute(self, payload, line, cell, local_ns, is_interactive_mode=False):
-        def interactive_execute_wrapper(**kwargs):
-            for key, value in kwargs.items():
-                local_ns[key] = value
-            return self._execute(line, cell, local_ns, is_interactive_mode=True)
-
         """
         This function implements the cell logic; we create this private
         method so we can control how the function is called. Otherwise,
         decorating ``SqlMagic.execute`` will break when adding the ``@log_call``
         decorator with ``payload=True``
         """
+
+        def interactive_execute_wrapper(**kwargs):
+            for key, value in kwargs.items():
+                local_ns[key] = value
+            return self._execute(line, cell, local_ns, is_interactive_mode=True)
+
         # line is the text after the magic, cell is the cell's body
 
         # Examples
 
         # %sql {line}
         # note that line magic has no body
 
@@ -398,15 +413,15 @@
         if args.with_:
             with_ = args.with_
         else:
             with_ = self._store.infer_dependencies(command.sql_original, args.save)
             if with_:
                 command.set_sql_with(with_)
                 display.message(
-                    f"Generating CTE with stored snippets : {pretty_print(with_)}"
+                    f"Generating CTE with stored snippets: {pretty_print(with_)}"
                 )
             else:
                 with_ = None
 
         # Create the interactive slider
         if args.interact and not is_interactive_mode:
             check_installed(["ipywidgets"], "--interactive argument")
@@ -416,17 +431,19 @@
             display.message(
                 "Interactive mode, please interact with below "
                 "widget(s) to control the variable"
             )
             interact(interactive_execute_wrapper, **interactive_dict)
             return
         if args.connections:
-            return sql.connection.Connection.connections_table()
+            return sql.connection.ConnectionManager.connections_table()
         elif args.close:
-            return sql.connection.Connection.close(args.close)
+            return sql.connection.ConnectionManager.close_connection_with_descriptor(
+                args.close
+            )
 
         connect_arg = command.connection
 
         if args.section:
             connect_arg = sql.parse.connection_from_dsn_section(args.section, self)
 
         if args.connection_arguments:
@@ -437,31 +454,31 @@
                     targets = ['"', "'"]
                     head = raw_args[0]
                     tail = raw_args[-1]
                     if head in targets and head == tail:
                         raw_args = raw_args[1:-1]
                 args.connection_arguments = json.loads(raw_args)
             except Exception as e:
-                display.message(str(e))
-                raise e
+                raise exceptions.ValueError(str(e)) from e
         else:
             args.connection_arguments = {}
         if args.creator:
             args.creator = user_ns[args.creator]
 
         # this creates a new connection or use an existing one
         # depending on the connect_arg value
-        conn = sql.connection.Connection.set(
+        conn = sql.connection.ConnectionManager.set(
             connect_arg,
             displaycon=self.displaycon,
             connect_args=args.connection_arguments,
             creator=args.creator,
             alias=args.alias,
+            config=self,
         )
-        payload["connection_info"] = conn._get_curr_sqlalchemy_connection_info()
+        payload["connection_info"] = conn._get_database_information()
 
         if args.persist_replace and args.append:
             raise exceptions.UsageError(
                 """You cannot simultaneously persist and append data to a dataframe;
                   please choose to utilize either one or the other."""
             )
         if args.persist and args.persist_replace:
@@ -508,15 +525,20 @@
             self._store.store(args.save, command.sql_original, with_=with_)
 
         if args.no_execute:
             display.message("Skipping execution...")
             return
 
         try:
-            result = sql.run.run(conn, command.sql, self)
+            result = run_statements(
+                conn,
+                command.sql,
+                self,
+                parameters=user_ns if self.named_parameters else None,
+            )
 
             if (
                 result is not None
                 and not isinstance(result, str)
                 and self.column_local_vars
             ):
                 # Instead of returning values, set variables directly in the
@@ -543,15 +565,21 @@
                         return result
                     return None
 
                 # Return results into the default ipython _ variable
                 return result
 
         # JA: added DatabaseError for MySQL
-        except (ProgrammingError, OperationalError, DatabaseError) as e:
+        except (
+            ProgrammingError,
+            OperationalError,
+            DatabaseError,
+            # raised when they query has :parameters but no parameters are given
+            StatementError,
+        ) as e:
             # Sqlite apparently return all errors as OperationalError :/
             self._error_handling(e, command.sql)
         except Exception as e:
             # handle DuckDB exceptions
             if "Catalog Error" in str(e):
                 self._error_handling(e, command.sql)
             else:
@@ -605,31 +633,68 @@
             if_exists = "replace"
         elif append:
             if_exists = "append"
         else:
             if_exists = "fail"
 
         try:
-            frame.to_sql(table_name, conn.session, if_exists=if_exists, index=index)
+            frame.to_sql(
+                table_name, conn.connection_sqlalchemy, if_exists=if_exists, index=index
+            )
         except ValueError:
             raise exceptions.ValueError(
                 f"""Table {table_name!r} already exists. Consider using \
 --persist-replace to drop the table before persisting the data frame"""
             )
 
         display.message_success(f"Success! Persisted {table_name} to the database.")
 
 
+def set_configs(ip, file_path):
+    """Set user defined SqlMagic configuration settings"""
+    sql = ip.find_cell_magic("sql").__self__
+    user_configs = util.get_user_configs(file_path, ["tool", "jupysql", "SqlMagic"])
+    default_configs = util.get_default_configs(sql)
+    table_rows = []
+    for config, value in user_configs.items():
+        if config in default_configs.keys():
+            default_type = type(default_configs[config])
+            if isinstance(value, default_type):
+                setattr(sql, config, value)
+                table_rows.append([config, value])
+            else:
+                display.message(
+                    f"'{value}' is an invalid value for '{config}'. "
+                    f"Please use {default_type.__name__} value instead."
+                )
+        else:
+            util.find_close_match_config(config, default_configs.keys())
+
+    return table_rows
+
+
+def load_SqlMagic_configs(ip):
+    """Loads saved SqlMagic configs in pyproject.toml"""
+    file_path = util.find_path_from_root("pyproject.toml")
+    if file_path:
+        table_rows = set_configs(ip, file_path)
+        if table_rows:
+            display.message("Settings changed:")
+            display.table(["Config", "value"], table_rows)
+
+
 def load_ipython_extension(ip):
     """Load the extension in IPython."""
 
     # this fails in both Firefox and Chrome for OS X.
     # I get the error: TypeError: IPython.CodeCell.config_defaults is undefined
 
     # js = "IPython.CodeCell.config_defaults.highlight_modes['magic_sql'] = {'reg':[/^%%sql/]};" # noqa
     # display_javascript(js, raw=True)
     ip.register_magics(SqlMagic)
     ip.register_magics(RenderMagic)
     ip.register_magics(SqlPlotMagic)
     ip.register_magics(SqlCmdMagic)
 
     patch_ipython_usage_error(ip)
+
+    load_SqlMagic_configs(ip)
```

### Comparing `jupysql-0.8.0/src/sql/magic_cmd.py` & `jupysql-0.9.0/src/sql/magic_cmd.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.8.0/src/sql/magic_plot.py` & `jupysql-0.9.0/src/sql/magic_plot.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.8.0/src/sql/plot.py` & `jupysql-0.9.0/src/sql/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 from sql import util
 
 
 def _summary_stats(conn, table, column, with_=None):
     """Compute percentiles and mean for boxplot"""
 
     if not conn:
-        conn = sql.connection.Connection.current
-    driver = conn._get_curr_sqlalchemy_connection_info()["driver"]
+        conn = sql.connection.ConnectionManager.current
+    driver = conn._get_database_information()["driver"]
 
     template = Template(
         """
     SELECT
     percentile_disc([0.25, 0.50, 0.75]) WITHIN GROUP \
     (ORDER BY "{{column}}") AS percentiles,
     AVG("{{column}}") AS mean,
@@ -59,15 +59,15 @@
 
     keys = ["q1", "med", "q3", "mean", "N"]
     return {k: float(v) for k, v in zip(keys, flatten(values))}
 
 
 def _whishi(conn, table, column, hival, with_=None):
     if not conn:
-        conn = sql.connection.Connection.current
+        conn = sql.connection.ConnectionManager.current
     template = Template(
         """
 SELECT COUNT(*), MAX("{{column}}")
 FROM (
     SELECT "{{column}}"
     FROM "{{table}}"
     WHERE "{{column}}" <= {{hival}}
@@ -80,15 +80,15 @@
     values = conn.execute(query, with_).fetchone()
     keys = ["N", "wiskhi_max"]
     return {k: float(v) for k, v in zip(keys, values)}
 
 
 def _whislo(conn, table, column, loval, with_=None):
     if not conn:
-        conn = sql.connection.Connection.current
+        conn = sql.connection.ConnectionManager.current
     template = Template(
         """
 SELECT COUNT(*), MIN("{{column}}")
 FROM (
     SELECT "{{column}}"
     FROM "{{table}}"
     WHERE "{{column}}" >= {{loval}}
@@ -101,15 +101,15 @@
     values = conn.execute(query, with_).fetchone()
     keys = ["N", "wisklo_min"]
     return {k: float(v) for k, v in zip(keys, values)}
 
 
 def _percentile(conn, table, column, pct, with_=None):
     if not conn:
-        conn = sql.connection.Connection.current.session
+        conn = sql.connection.ConnectionManager.current.connection
     template = Template(
         """
 SELECT
 percentile_disc({{pct}}) WITHIN GROUP (ORDER BY "{{column}}") AS pct,
 FROM "{{table}}"
 """
     )
@@ -135,15 +135,15 @@
 
 
 # https://github.com/matplotlib/matplotlib/blob/b5ac96a8980fdb9e59c9fb649e0714d776e26701/lib/matplotlib/cbook/__init__.py
 @modify_exceptions
 def _boxplot_stats(conn, table, column, whis=1.5, autorange=False, with_=None):
     """Compute statistics required to create a boxplot"""
     if not conn:
-        conn = sql.connection.Connection.current
+        conn = sql.connection.ConnectionManager.current
 
     # calculating stats might fail on other DBs (percentile_disc)
     util.support_only_sql_alchemy_connection("boxplot")
 
     def _compute_conf_interval(N, med, iqr):
         notch_min = med - 1.57 * iqr / np.sqrt(N)
         notch_max = med + 1.57 * iqr / np.sqrt(N)
@@ -254,17 +254,17 @@
     .. plot:: ../examples/plot_boxplot_horizontal.py
 
     **Plot multiple columns from the same table:**
 
     .. plot:: ../examples/plot_boxplot_many.py
     """
     if not conn:
-        conn = sql.connection.Connection.current
+        conn = sql.connection.ConnectionManager.current
 
-    payload["connection_info"] = conn._get_curr_sqlalchemy_connection_info()
+    payload["connection_info"] = conn._get_database_information()
 
     ax = plt.gca()
     vert = orient == "v"
 
     set_ticklabels = ax.set_xticklabels if vert else ax.set_yticklabels
     set_label = ax.set_ylabel if vert else ax.set_xlabel
 
@@ -281,15 +281,15 @@
         set_ticklabels(column)
 
     return ax
 
 
 def _min_max(con, table, column, with_=None, use_backticks=False):
     if not con:
-        con = sql.connection.Connection.current
+        con = sql.connection.ConnectionManager.current
     template_ = """
 SELECT
     MIN("{{column}}"),
     MAX("{{column}}")
 FROM "{{table}}"
 """
     if use_backticks:
@@ -302,22 +302,38 @@
     return min_, max_
 
 
 def _are_numeric_values(*values):
     return all([isinstance(value, (int, float)) for value in values])
 
 
-def _get_bar_width(ax, bins):
+def _get_bar_width(ax, bins, bin_size):
     """
     Return a single bar width based on number of bins
     If bins values are str, calculate value based on figure size.
+
+    Parameters
+    ----------
+    ax : matplotlib.Axes
+        Generated plot
+
+    bins : tuple
+        Contains bins' midpoints as float
+
+    bin_size : int or None
+        Calculated bin_size from the _histogram function
+
+    Returns
+    -------
+    width : float
+        A single bar width
     """
 
-    if _are_numeric_values(bins[-1], bins[-2]):
-        width = bins[-1] - bins[-2]
+    if _are_numeric_values(bin_size):
+        width = bin_size
     else:
         fig = plt.gcf()
         bbox = ax.get_window_extent()
         width_inch = bbox.width / fig.dpi
         width = width_inch / len(bins)
 
     return width
@@ -375,18 +391,18 @@
     .. plot:: ../examples/plot_histogram.py
 
     **Plot multiple columns from the same table**:
 
     .. plot:: ../examples/plot_histogram_many.py
     """
     if not conn:
-        conn = sql.connection.Connection.current
+        conn = sql.connection.ConnectionManager.current
 
     ax = ax or plt.gca()
-    payload["connection_info"] = conn._get_curr_sqlalchemy_connection_info()
+    payload["connection_info"] = conn._get_database_information()
     if category:
         if isinstance(column, list):
             if len(column) > 1:
                 raise ValueError(
                     f"""Columns given : {column}.
                     When using a stacked histogram,
                     please ensure that you specify only one column."""
@@ -394,15 +410,15 @@
             else:
                 column = " ".join(column)
 
         if column is None or len(column) == 0:
             raise ValueError("Column name has not been specified")
 
         bin_, height, bin_size = _histogram(table, column, bins, with_=with_, conn=conn)
-        width = _get_bar_width(ax, bin_)
+        width = _get_bar_width(ax, bin_, bin_size)
         data = _histogram_stacked(
             table, column, category, bin_, bin_size, with_=with_, conn=conn, facet=facet
         )
         cmap = plt.get_cmap(cmap or "viridis")
         norm = Normalize(vmin=0, vmax=len(data))
 
         bottom = np.zeros(len(bin_))
@@ -435,20 +451,22 @@
                 bottom=bottom,
                 edgecolor=edgecolor_,
                 color=color_,
             )
             bottom += values_
 
         ax.set_title(f"Histogram from {table!r}")
-        ax.legend()
+        # reverses legend order so alphabetically first goes on top
+        handles, labels = ax.get_legend_handles_labels()
+        ax.legend(handles[::-1], labels[::-1])
     elif isinstance(column, str):
-        bin_, height, _ = _histogram(
+        bin_, height, bin_size = _histogram(
             table, column, bins, with_=with_, conn=conn, facet=facet
         )
-        width = _get_bar_width(ax, bin_)
+        width = _get_bar_width(ax, bin_, bin_size)
 
         ax.bar(
             bin_,
             height,
             align="center",
             width=width,
             color=color,
@@ -456,18 +474,18 @@
             label=column,
         )
         ax.set_title(f"{column!r} from {table!r}")
         ax.set_xlabel(column)
 
     else:
         for i, col in enumerate(column):
-            bin_, height, _ = _histogram(
+            bin_, height, bin_size = _histogram(
                 table, col, bins, with_=with_, conn=conn, facet=facet
             )
-            width = _get_bar_width(ax, bin_)
+            width = _get_bar_width(ax, bin_, bin_size)
 
             if isinstance(color, list):
                 color_ = color[i]
             else:
                 color_ = color
 
             if isinstance(edgecolor, list):
@@ -493,15 +511,15 @@
     return ax
 
 
 @modify_exceptions
 def _histogram(table, column, bins, with_=None, conn=None, facet=None):
     """Compute bins and heights"""
     if not conn:
-        conn = sql.connection.Connection.current
+        conn = sql.connection.ConnectionManager.current
     use_backticks = conn.is_use_backtick_template()
 
     # FIXME: we're computing all the with elements twice
     min_, max_ = _min_max(conn, table, column, with_=with_, use_backticks=use_backticks)
 
     # Define all relevant filters here
     filter_query_1 = f'"{column}" IS NOT NULL'
@@ -514,20 +532,21 @@
 
     if _are_numeric_values(min_, max_):
         if not isinstance(bins, int):
             raise ValueError(
                 f"bins are '{bins}'. Please specify a valid number of bins."
             )
 
+        # Use bins - 1 instead of bins and round half down instead of floor
+        # to mimic right-closed histogram intervals in R ggplot
         range_ = max_ - min_
-        bin_size = range_ / bins
-
+        bin_size = range_ / (bins - 1)
         template_ = """
             select
-            floor("{{column}}"/{{bin_size}})*{{bin_size}} as bin,
+            ceiling("{{column}}"/{{bin_size}} - 0.5)*{{bin_size}} as bin,
             count(*) as count
             from "{{table}}"
             {{filter_query}}
             group by bin
             order by bin;
             """
 
@@ -572,20 +591,25 @@
     bin_size,
     with_=None,
     conn=None,
     facet=None,
 ):
     """Compute the corresponding heights of each bin based on the category"""
     if not conn:
-        conn = sql.connection.Connection.current
+        conn = sql.connection.ConnectionManager.current
 
     cases = []
+    tolerance = bin_size / 1000  # Use to avoid floating point error
     for bin in bins:
-        case = f'SUM(CASE WHEN FLOOR({column}/{bin_size})*{bin_size} = {bin} \
-                 THEN 1 ELSE 0 END) AS "{bin}",'
+        # Use round half down instead of floor to mimic
+        # right-closed histogram intervals in R ggplot
+        case = (
+            f"SUM(CASE WHEN ABS(CEILING({column}/{bin_size} - 0.5)*{bin_size} "
+            f"- {bin}) <= {tolerance} THEN 1 ELSE 0 END) AS '{bin}',"
+        )
         cases.append(case)
 
     cases = " ".join(cases)
 
     filter_query_1 = f'"{column}" IS NOT NULL'
 
     filter_query_2 = f"{facet['key']} == '{facet['value']}'" if facet else None
@@ -594,15 +618,16 @@
 
     template = Template(
         """
         SELECT {{category}},
         {{cases}}
         FROM "{{table}}"
         {{filter_query}}
-        GROUP BY {{category}};
+        GROUP BY {{category}}
+        ORDER BY {{category}} DESC;
         """
     )
     query = template.render(
         table=table,
         column=column,
         bin_size=bin_size,
         category=category,
@@ -647,15 +672,15 @@
     return final_filter
 
 
 @modify_exceptions
 def _bar(table, column, with_=None, conn=None):
     """get x and height for bar plot"""
     if not conn:
-        conn = sql.connection.Connection.current
+        conn = sql.connection.ConnectionManager.current
     use_backticks = conn.is_use_backtick_template()
 
     if isinstance(column, list):
         if len(column) > 2:
             raise exceptions.UsageError(
                 f"Passed columns: {column}\n"
                 "Bar chart currently supports, either a single column"
@@ -756,18 +781,18 @@
     -------
     ax : matplotlib.Axes
         Generated plot
 
     """
 
     if not conn:
-        conn = sql.connection.Connection.current
+        conn = sql.connection.ConnectionManager.current
 
     ax = ax or plt.gca()
-    payload["connection_info"] = conn._get_curr_sqlalchemy_connection_info()
+    payload["connection_info"] = conn._get_database_information()
 
     if column is None:
         raise exceptions.UsageError("Column name has not been specified")
 
     x, height_, xlabel, ylabel = _bar(table, column, with_=with_, conn=conn)
 
     if color and cmap:
@@ -831,15 +856,15 @@
     return ax
 
 
 @modify_exceptions
 def _pie(table, column, with_=None, conn=None):
     """get x and height for pie chart"""
     if not conn:
-        conn = sql.connection.Connection.current
+        conn = sql.connection.ConnectionManager.current
     use_backticks = conn.is_use_backtick_template()
 
     if isinstance(column, list):
         if len(column) > 2:
             raise exceptions.UsageError(
                 f"Passed columns: {column}\n"
                 "Pie chart currently supports, either a single column"
@@ -928,18 +953,18 @@
     Returns
     -------
     ax : matplotlib.Axes
         Generated plot
     """
 
     if not conn:
-        conn = sql.connection.Connection.current
+        conn = sql.connection.ConnectionManager.current
 
     ax = ax or plt.gca()
-    payload["connection_info"] = conn._get_curr_sqlalchemy_connection_info()
+    payload["connection_info"] = conn._get_database_information()
 
     if column is None:
         raise exceptions.UsageError("Column name has not been specified")
 
     labels, size_ = _pie(table, column, with_=with_, conn=conn)
 
     if color and cmap:
```

### Comparing `jupysql-0.8.0/src/sql/query_util.py` & `jupysql-0.9.0/src/sql/query_util.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.8.0/src/sql/run.py` & `jupysql-0.9.0/src/sql/run/resultset.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,185 +1,132 @@
-import codecs
-import csv
-import operator
-import os.path
 import re
+import operator
 from functools import reduce
 from io import StringIO
 import html
-
-import prettytable
-import sqlalchemy
-import sqlparse
-from sql.connection import Connection
-from sqlalchemy.exc import ResourceClosedError
-from sql import exceptions, display
-from .column_guesser import ColumnGuesserMixin
-from sql.warnings import JupySQLDataFramePerformanceWarning
-
-try:
-    from pgspecial.main import PGSpecial
-except ModuleNotFoundError:
-    PGSpecial = None
-from sqlalchemy.orm import Session
-
-from sql.telemetry import telemetry
-import logging
-import warnings
 from collections.abc import Iterable
+from collections import defaultdict
 
 
-def unduplicate_field_names(field_names):
-    """Append a number to duplicate field names to make them unique."""
-    res = []
-    for k in field_names:
-        if k in res:
-            i = 1
-            while k + "_" + str(i) in res:
-                i += 1
-            k += "_" + str(i)
-        res.append(k)
-    return res
-
-
-class UnicodeWriter(object):
-    """
-    A CSV writer which will write rows to CSV file "f",
-    which is encoded in the given encoding.
-    """
-
-    def __init__(self, f, dialect=csv.excel, encoding="utf-8", **kwds):
-        # Redirect output to a queue
-        self.queue = StringIO()
-        self.writer = csv.writer(self.queue, dialect=dialect, **kwds)
-        self.stream = f
-        self.encoder = codecs.getincrementalencoder(encoding)()
-
-    def writerow(self, row):
-        _row = row
-        self.writer.writerow(_row)
-        # Fetch UTF-8 output from the queue ...
-        data = self.queue.getvalue()
-        # write to the target stream
-        self.stream.write(data)
-        # empty queue
-        self.queue.truncate(0)
-        self.queue.seek(0)
-
-    def writerows(self, rows):
-        for row in rows:
-            self.writerow(row)
+import prettytable
 
+from sql.column_guesser import ColumnGuesserMixin
+from sql.run.csv import CSVWriter, CSVResultDescriptor
+from sql.telemetry import telemetry
+from sql.run.table import CustomPrettyTable
 
-class CsvResultDescriptor(object):
-    """
-    Provides IPython Notebook-friendly output for the
-    feedback after a ``.csv`` called.
-    """
 
-    def __init__(self, file_path):
-        self.file_path = file_path
+class ResultSetsManager:
+    def __init__(self) -> None:
+        self._results = defaultdict(list)
 
-    def __repr__(self):
-        return "CSV results at %s" % os.path.join(os.path.abspath("."), self.file_path)
+    def append_to_key(self, key, result):
+        """
+        Append object to a given key, if it already exists, it doesn't add
+        a duplicate but moves it to the end
+        """
+        results_for_key = self._results[key]
 
-    def _repr_html_(self):
-        return '<a href="%s">CSV results</a>' % os.path.join(
-            ".", "files", self.file_path
-        )
+        if result in results_for_key:
+            results_for_key.remove(result)
 
+        results_for_key.append(result)
 
-def _nonbreaking_spaces(match_obj):
-    """
-    Make spaces visible in HTML by replacing all `` `` with ``&nbsp;``
-
-    Call with a ``re`` match object.  Retain group 1, replace group 2
-    with nonbreaking spaces.
-    """
-    spaces = "&nbsp;" * len(match_obj.group(2))
-    return "%s%s" % (match_obj.group(1), spaces)
+    def is_last_for_key(self, key, result):
+        """
+        Check if the passed result is the last one for the given key,
+        returns True if there are no results for the key
+        """
+        results_for_key = self._results[key]
 
+        # if there are no results, return True to prevent triggering
+        # a query in the database
+        if not len(results_for_key):
+            return True
 
-_cell_with_spaces_pattern = re.compile(r"(<td>)( {2,})")
+        return results_for_key[-1] is result
 
 
 class ResultSet(ColumnGuesserMixin):
     """
     Results of a SQL query. Fetches rows lazily (only the necessary rows to show the
     preview based on the current configuration)
     """
 
-    # user to overcome a duckdb-engine limitation, see @sqlaproxy for details
-    LAST_BY_CONNECTION = {}
+    # user to overcome drivers limitations, see @sqlaproxy for details
+    BY_CONNECTION = ResultSetsManager()
 
     def __init__(self, sqlaproxy, config, statement=None, conn=None):
-        ResultSet.LAST_BY_CONNECTION[conn] = self
-
-        self.config = config
-        self.truncated = False
-        self.statement = statement
-
+        self._config = config
+        self._statement = statement
         self._sqlaproxy = sqlaproxy
         self._conn = conn
-        self._dialect = conn._get_curr_sqlglot_dialect()
+        self._dialect = conn._get_sqlglot_dialect()
         self._keys = None
         self._field_names = None
         self._results = []
-
         # https://peps.python.org/pep-0249/#description
-        self.is_dbapi_results = hasattr(sqlaproxy, "description")
+        self._is_dbapi_results = hasattr(sqlaproxy, "description")
 
         # note that calling this will fetch the keys
-        self.pretty_table = self._init_table()
+        self._pretty_table = self._init_table()
 
         self._mark_fetching_as_done = False
 
-        if self.config.autolimit == 1:
+        if self._config.autolimit == 1:
             # if autolimit is 1, we only want to fetch one row
             self.fetchmany(size=1)
             self._done_fetching()
         else:
             # in all other cases, 2 allows us to know if there are more rows
             # for example when creating a table, the results contains one row, in
             # such case, fetching 2 rows will tell us that there are no more rows
             # and can set the _mark_fetching_as_done flag to True
             self.fetchmany(size=2)
 
         self._finished_init = True
 
+        # TODO: clean up, this is redundant
+        if conn:
+            conn._result_sets.append(self)
+
+        ResultSet.BY_CONNECTION.append_to_key(conn, self)
+
     @property
     def sqlaproxy(self):
         # there is a problem when using duckdb + sqlalchemy: duckdb-engine doesn't
         # create separate cursors, so whenever we have >1 ResultSet, the old ones
         # become outdated and fetching their results will return the results from
         # the last ResultSet. To fix this, we have to re-issue the query
-        is_last_result = ResultSet.LAST_BY_CONNECTION.get(self._conn) is self
+        is_last_result = ResultSet.BY_CONNECTION.is_last_for_key(self._conn, self)
         is_duckdb_sqlalchemy = (
-            self._dialect == "duckdb" and not self._conn.is_dbapi_connection()
+            self._dialect == "duckdb" and not self._conn.is_dbapi_connection
         )
 
+        # TODO: re-open it if closed
+
         if (
             # skip this if we're initializing the object (we're running __init__)
             hasattr(self, "_finished_init")
             # this only applies to duckdb + sqlalchemy with outdated results
             and is_duckdb_sqlalchemy
             and not is_last_result
         ):
-            self._sqlaproxy = self._conn.session.execute(self.statement)
+            self._sqlaproxy = self._conn.raw_execute(self._statement)
             self._sqlaproxy.fetchmany(size=len(self._results))
 
-            ResultSet.LAST_BY_CONNECTION[self._conn] = self
+            ResultSet.BY_CONNECTION.append_to_key(self._conn, self)
 
         return self._sqlaproxy
 
     def _extend_results(self, elements):
         """Store the DB fetched results into the internal list of results"""
-        to_add = self.config.displaylimit - len(self._results)
+        to_add = self._config.displaylimit - len(self._results)
         self._results.extend(elements)
-        self.pretty_table.add_rows(elements[:to_add])
+        self._pretty_table.add_rows(elements[:to_add])
 
     def mark_fetching_as_done(self):
         self._mark_fetching_as_done = True
         # NOTE: don't close the connection here (self.sqlaproxy.close()),
         # because we need to keep it open for the next query
 
     def _done_fetching(self):
@@ -196,20 +143,22 @@
     def keys(self):
         """
         Return the keys of the results (the column names)
         """
         if self._keys is not None:
             return self._keys
 
-        if not self.is_dbapi_results:
+        if not self._is_dbapi_results:
             try:
                 self._keys = self.sqlaproxy.keys()
-            # sqlite raises this error when running a script that doesn't return rows
-            # e.g, 'CREATE TABLE' but others don't (e.g., duckdb)
-            except ResourceClosedError:
+            # sqlite with sqlalchemy raises sqlalchemy.exc.ResourceClosedError,
+            # psycopg2 raises psycopg2.ProgrammingError error when running a script
+            # that doesn't return rows e.g, 'CREATE TABLE' but others don't
+            # (e.g., duckdb), so here we catch all
+            except Exception:
                 self._keys = []
                 return self._keys
 
         elif isinstance(self.sqlaproxy.description, Iterable):
             self._keys = [i[0] for i in self.sqlaproxy.description]
         else:
             self._keys = []
@@ -217,15 +166,15 @@
         return self._keys
 
     def _repr_html_(self):
         self.fetch_for_repr_if_needed()
 
         _cell_with_spaces_pattern = re.compile(r"(<td>)( {2,})")
 
-        result = self.pretty_table.get_html_string()
+        result = self._pretty_table.get_html_string()
 
         HTML = (
             "%s\n<span style='font-style:italic;font-size:11px'>"
             "<code>ResultSet</code> : to convert to pandas, call <a href="
             "'https://jupysql.ploomber.io/en/latest/integrations/pandas.html'>"
             "<code>.DataFrame()</code></a> or to polars, call <a href="
             "'https://jupysql.ploomber.io/en/latest/integrations/polars.html'>"
@@ -233,25 +182,25 @@
         )
         result = HTML % (result)
 
         # to create clickable links
         result = html.unescape(result)
         result = _cell_with_spaces_pattern.sub(_nonbreaking_spaces, result)
 
-        if self.config.displaylimit != 0 and not self._done_fetching():
+        if self._config.displaylimit != 0 and not self._done_fetching():
             HTML = (
                 '%s\n<span style="font-style:italic;text-align:center;">'
                 "Truncated to displaylimit of %d</span>"
                 "<br>"
                 '<span style="font-style:italic;text-align:center;">'
                 "If you want to see more, please visit "
                 '<a href="https://jupysql.ploomber.io/en/latest/api/configuration.html#displaylimit">displaylimit</a>'  # noqa: E501
                 " configuration</span>"
             )
-            result = HTML % (result, self.config.displaylimit)
+            result = HTML % (result, self._config.displaylimit)
         return result
 
     def __len__(self):
         self.fetchall()
 
         return len(self._results)
 
@@ -259,15 +208,15 @@
         self.fetchall()
 
         for result in self._results:
             yield result
 
     def __str__(self):
         self.fetch_for_repr_if_needed()
-        return str(self.pretty_table)
+        return str(self._pretty_table)
 
     def __repr__(self) -> str:
         return str(self)
 
     def __eq__(self, another: object) -> bool:
         return self._results == another
 
@@ -304,15 +253,15 @@
         "Iterator yielding a dict for each row"
         for row in self:
             yield dict(zip(self.keys, row))
 
     @telemetry.log_call("data-frame", payload=True)
     def DataFrame(self, payload):
         """Returns a Pandas DataFrame instance built from the result set."""
-        payload["connection_info"] = self._conn._get_curr_sqlalchemy_connection_info()
+        payload["connection_info"] = self._conn._get_database_information()
         import pandas as pd
 
         kwargs = {"columns": (self and self.keys) or []}
         return _convert_to_data_frame(self, "df", pd.DataFrame, kwargs)
 
     @telemetry.log_call("polars-data-frame")
     def PolarsDataFrame(self, **polars_dataframe_kwargs):
@@ -433,312 +382,132 @@
         Any other parameters will be passed on to csv.writer."""
         if filename:
             encoding = format_params.get("encoding", "utf-8")
             outfile = open(filename, "w", newline="", encoding=encoding)
         else:
             outfile = StringIO()
 
-        writer = UnicodeWriter(outfile, **format_params)
+        writer = CSVWriter(outfile, **format_params)
         writer.writerow(self.field_names)
         for row in self:
             writer.writerow(row)
         if filename:
             outfile.close()
-            return CsvResultDescriptor(filename)
+            return CSVResultDescriptor(filename)
         else:
             return outfile.getvalue()
 
     def fetchmany(self, size):
         """Fetch n results and add it to the results"""
         if not self._done_fetching():
             try:
                 returned = self.sqlaproxy.fetchmany(size=size)
-            # sqlite raises this error when running a script that doesn't return rows
-            # e.g, 'CREATE TABLE' but others don't (e.g., duckdb)
-            except ResourceClosedError:
+            # sqlite with sqlalchemy raises sqlalchemy.exc.ResourceClosedError,
+            # psycopg2 raises psycopg2.ProgrammingError error when running a script
+            # that doesn't return rows e.g, 'CREATE TABLE' but others don't
+            # (e.g., duckdb), so here we catch all
+            except Exception:
                 self.mark_fetching_as_done()
                 return
 
             self._extend_results(returned)
 
             if len(returned) < size:
                 self.mark_fetching_as_done()
 
             if (
-                self.config.autolimit is not None
-                and self.config.autolimit != 0
-                and len(self._results) >= self.config.autolimit
+                self._config.autolimit is not None
+                and self._config.autolimit != 0
+                and len(self._results) >= self._config.autolimit
             ):
                 self.mark_fetching_as_done()
 
     def fetch_for_repr_if_needed(self):
-        if self.config.displaylimit == 0:
+        if self._config.displaylimit == 0:
             self.fetchall()
 
-        missing = self.config.displaylimit - len(self._results)
+        missing = self._config.displaylimit - len(self._results)
 
         if missing > 0:
             self.fetchmany(missing)
 
     def fetchall(self):
         if not self._done_fetching():
             self._extend_results(self.sqlaproxy.fetchall())
             self.mark_fetching_as_done()
 
     def _init_table(self):
         pretty = CustomPrettyTable(self.field_names)
 
-        if isinstance(self.config.style, str):
-            _style = prettytable.__dict__[self.config.style.upper()]
+        if isinstance(self._config.style, str):
+            _style = prettytable.__dict__[self._config.style.upper()]
             pretty.set_style(_style)
 
         return pretty
 
 
-def display_affected_rowcount(rowcount):
-    if rowcount > 0:
-        display.message_success(f"{rowcount} rows affected.")
-
-
-class FakeResultProxy(object):
-    """A fake class that pretends to behave like the ResultProxy from
-    SqlAlchemy.
-    """
-
-    def __init__(self, cursor, headers):
-        if cursor is None:
-            cursor = []
-            headers = []
-        if isinstance(cursor, list):
-            self.from_list(source_list=cursor)
-        else:
-            self.fetchall = cursor.fetchall
-            self.fetchmany = cursor.fetchmany
-            self.rowcount = cursor.rowcount
-        self.keys = lambda: headers
-        self.returns_rows = True
-
-    def from_list(self, source_list):
-        "Simulates SQLA ResultProxy from a list."
-
-        self.fetchall = lambda: source_list
-        self.rowcount = len(source_list)
-
-        def fetchmany(size):
-            pos = 0
-            while pos < len(source_list):
-                yield source_list[pos : pos + size]
-                pos += size
-
-        self.fetchmany = fetchmany
-
-
-# some dialects have autocommit
-# specific dialects break when commit is used:
-
-_COMMIT_BLACKLIST_DIALECTS = (
-    "athena",
-    "bigquery",
-    "clickhouse",
-    "ingres",
-    "mssql",
-    "teradata",
-    "vertica",
-)
-
-
-def _commit(conn, config, manual_commit):
-    """Issues a commit, if appropriate for current config and dialect"""
-
-    _should_commit = (
-        config.autocommit
-        and all(
-            dialect not in str(conn.dialect) for dialect in _COMMIT_BLACKLIST_DIALECTS
-        )
-        and manual_commit
-    )
-
-    if _should_commit:
-        try:
-            with Session(conn.session) as session:
-                session.commit()
-        except sqlalchemy.exc.OperationalError:
-            display.message("The database does not support the COMMIT command")
-
-
-def is_postgres_or_redshift(dialect):
-    """Checks if dialect is postgres or redshift"""
-    return "postgres" in str(dialect) or "redshift" in str(dialect)
-
-
-def is_pytds(dialect):
-    """Checks if driver is pytds"""
-    return "pytds" in str(dialect)
-
-
-def handle_postgres_special(conn, statement):
-    """Execute a PostgreSQL special statement using PGSpecial module."""
-    if not PGSpecial:
-        raise exceptions.MissingPackageError("pgspecial not installed")
-
-    pgspecial = PGSpecial()
-    _, cur, headers, _ = pgspecial.execute(conn.session.connection.cursor(), statement)[
-        0
-    ]
-    return FakeResultProxy(cur, headers)
-
-
-def set_autocommit(conn, config):
-    """Sets the autocommit setting for a database connection."""
-    if is_pytds(conn.dialect):
-        warnings.warn(
-            "Autocommit is not supported for pytds, thus is automatically disabled"
-        )
-        return False
-    if config.autocommit:
-        try:
-            conn.session.execution_options(isolation_level="AUTOCOMMIT")
-        except Exception as e:
-            logging.debug(
-                f"The database driver doesn't support such "
-                f"AUTOCOMMIT execution option"
-                f"\nPerhaps you can try running a manual COMMIT command"
-                f"\nMessage from the database driver\n\t"
-                f"Exception:  {e}\n",  # noqa: F841
-            )
-            return True
-    return False
-
-
-def select_df_type(resultset, config):
-    """
-    Converts the input resultset to either a Pandas DataFrame
-    or Polars DataFrame based on the config settings.
-    """
-    if config.autopandas:
-        return resultset.DataFrame()
-    elif config.autopolars:
-        return resultset.PolarsDataFrame(**config.polars_dataframe_kwargs)
-    else:
-        return resultset
-    # returning only last result, intentionally
-
-
-def run(conn, sql, config):
-    """Run a SQL query with the given connection
-
-    Parameters
-    ----------
-    conn : sql.connection.Connection
-        The connection to use
-
-    sql : str
-        SQL query to execution
-
-    config
-        Configuration object
-    """
-    if not sql.strip():
-        # returning only when sql is empty string
-        return "Connected: %s" % conn.name
-
-    for statement in sqlparse.split(sql):
-        first_word = sql.strip().split()[0].lower()
-        manual_commit = False
-
-        # attempting to run a transaction
-        if first_word == "begin":
-            raise exceptions.RuntimeError("JupySQL does not support transactions")
-
-        # postgres metacommand
-        if first_word.startswith("\\") and is_postgres_or_redshift(conn.dialect):
-            result = handle_postgres_special(conn, statement)
-
-        # regular query
-        else:
-            manual_commit = set_autocommit(conn, config)
-            is_dbapi_connection = Connection.is_dbapi_connection(conn)
-
-            # if regular sqlalchemy, pass a text object
-            if not is_dbapi_connection:
-                statement = sqlalchemy.sql.text(statement)
-
-            result = conn.session.execute(statement)
-            _commit(conn=conn, config=config, manual_commit=manual_commit)
-
-            if result and config.feedback:
-                if hasattr(result, "rowcount"):
-                    display_affected_rowcount(result.rowcount)
-
-    resultset = ResultSet(result, config, statement, conn)
-    return select_df_type(resultset, config)
-
-
-def raw_run(conn, sql):
-    return conn.session.execute(sqlalchemy.sql.text(sql))
-
-
-class CustomPrettyTable(prettytable.PrettyTable):
-    def add_rows(self, data):
-        for row in data:
-            formatted_row = []
-            for cell in row:
-                if isinstance(cell, str) and cell.startswith("http"):
-                    formatted_row.append("<a href={}>{}</a>".format(cell, cell))
-                else:
-                    formatted_row.append(cell)
-            self.add_row(formatted_row)
-
-
-def _statement_is_select(statement):
-    statement_ = statement.lower().strip()
-    # duckdb also allows FROM without SELECT
-    return statement_.startswith("select") or statement_.startswith("from")
+def unduplicate_field_names(field_names):
+    """Append a number to duplicate field names to make them unique."""
+    res = []
+    for k in field_names:
+        if k in res:
+            i = 1
+            while k + "_" + str(i) in res:
+                i += 1
+            k += "_" + str(i)
+        res.append(k)
+    return res
 
 
 def _convert_to_data_frame(
     result_set, converter_name, constructor, constructor_kwargs=None
 ):
+    """
+    Convert the result set to a pandas DataFrame, using native DuckDB methods if
+    possible
+    """
     constructor_kwargs = constructor_kwargs or {}
-    has_converter_method = hasattr(result_set.sqlaproxy, converter_name)
+
+    # maybe create accessors in the connection objects?
+    if result_set._conn.is_dbapi_connection:
+        native_connection = result_set.sqlaproxy
+    else:
+        native_connection = result_set._conn._connection.connection
+
+    has_converter_method = hasattr(native_connection, converter_name)
 
     # native duckdb connection
-    if hasattr(result_set.sqlaproxy, converter_name):
+    if has_converter_method:
         # we need to re-execute the statement because if we fetched some rows
         # already, .df() will return None. But only if it's a select statement
         # otherwise we might end up re-execute INSERT INTO or CREATE TABLE
         # statements
-        is_select = _statement_is_select(result_set.statement)
+        is_select = _statement_is_select(result_set._statement)
 
         if is_select:
-            result_set.sqlaproxy.execute(result_set.statement)
+            native_connection.execute(result_set._statement)
 
-        return getattr(result_set.sqlaproxy, converter_name)()
+        return getattr(native_connection, converter_name)()
     else:
         frame = constructor(
             (tuple(row) for row in result_set),
             **constructor_kwargs,
         )
 
-        # NOTE: in JupySQL 0.7.9, we were opening a raw new connection so people
-        # using SQLALchemy still had the native performance to convert to data frames
-        # but this led to other problems because the native connection didn't
-        # have the same state as the SQLAlchemy connection, yielding confusing
-        # errors. So we decided to remove this and just warn the user that
-        # performance might be slow and they could use a native connection
-        if (
-            result_set._dialect == "duckdb"
-            and not has_converter_method
-            and len(frame) >= 1_000
-        ):
-            DOCS = "https://jupysql.ploomber.io/en/latest/integrations/duckdb.html"
-            WARNINGS = "https://jupysql.ploomber.io/en/latest/tutorials/duckdb-native-sqlalchemy.html#supress-warnings"  # noqa: E501
+        return frame
 
-            warnings.warn(
-                "It looks like you're using DuckDB with SQLAlchemy. "
-                "For faster conversions, use "
-                f" a DuckDB native connection. Docs: {DOCS}."
-                f" to suppress this warning, see: {WARNINGS}",
-                category=JupySQLDataFramePerformanceWarning,
-            )
 
-        return frame
+def _nonbreaking_spaces(match_obj):
+    """
+    Make spaces visible in HTML by replacing all `` `` with ``&nbsp;``
+
+    Call with a ``re`` match object.  Retain group 1, replace group 2
+    with nonbreaking spaces.
+    """
+    spaces = "&nbsp;" * len(match_obj.group(2))
+    return "%s%s" % (match_obj.group(1), spaces)
+
+
+def _statement_is_select(statement):
+    statement_ = statement.lower().strip()
+    # duckdb also allows FROM without SELECT
+    return statement_.startswith("select") or statement_.startswith("from")
```

### Comparing `jupysql-0.8.0/src/sql/store.py` & `jupysql-0.9.0/src/sql/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,14 @@
     def __init__(self):
         self._data = dict()
 
     def __setitem__(self, key: str, value: str) -> None:
         self._data[key] = value
 
     def __getitem__(self, key) -> str:
-        if not self._data:
-            raise exceptions.UsageError("No saved SQL")
         if key not in self._data:
             matches = difflib.get_close_matches(key, self._data)
             error = f'"{key}" is not a valid snippet identifier.'
             if matches:
                 raise exceptions.UsageError(error + f' Did you mean "{matches[0]}"?')
             else:
                 valid = ", ".join(f'"{key}"' for key in self._data.keys())
@@ -121,15 +119,17 @@
             """WITH{% for name in with_ %} {{name}} AS ({{rts(saved[name]._query)}})\
 {{ "," if not loop.last }}{% endfor %}{{query}}"""
         )
         with_clause_template_backtick = Template(
             """WITH{% for name in with_ %} `{{name}}` AS ({{rts(saved[name]._query)}})\
 {{ "," if not loop.last }}{% endfor %}{{query}}"""
         )
-        is_use_backtick = sql.connection.Connection.current.is_use_backtick_template()
+        is_use_backtick = (
+            sql.connection.ConnectionManager.current.is_use_backtick_template()
+        )
         with_all = _get_dependencies(self._store, self._with_)
         template = (
             with_clause_template_backtick if is_use_backtick else with_clause_template
         )
         # return query without 'with' when no dependency exists
         if len(with_all) == 0:
             return self._query.strip()
```

### Comparing `jupysql-0.8.0/src/sql/widgets/table_widget/js/tableWidget.js` & `jupysql-0.9.0/src/sql/widgets/table_widget/js/tableWidget.js`

 * *Files identical despite different names*

### Comparing `jupysql-0.8.0/src/sql/widgets/table_widget/table_widget.py` & `jupysql-0.9.0/src/sql/widgets/table_widget/table_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from sql.connection import Connection
+from sql.connection import ConnectionManager
 from IPython import get_ipython
 import math
-import sqlalchemy
 import time
 from sql.util import (
     fetch_sql_with_pagination,
     parse_sql_results_to_json,
     is_table_exists,
 )
 
@@ -58,17 +57,15 @@
         Creates an HTML table with default data
         """
         rows_per_page = 10
         rows, columns = fetch_sql_with_pagination(table, 0, rows_per_page)
         rows = parse_sql_results_to_json(rows, columns)
 
         query = f"SELECT count(*) FROM {table}"
-        n_total = Connection.current.session.execute(
-            sqlalchemy.sql.text(query)
-        ).fetchone()[0]
+        n_total = ConnectionManager.current.raw_execute(query).fetchone()[0]
         table_name = table.strip('"').strip("'")
 
         n_pages = math.ceil(n_total / rows_per_page)
 
         unique_id = str(int(time.time()))
         table_container_id = f"tableContainer_{unique_id}"
```

### Comparing `jupysql-0.8.0/src/sql/widgets/utils.py` & `jupysql-0.9.0/src/sql/widgets/utils.py`

 * *Files identical despite different names*

