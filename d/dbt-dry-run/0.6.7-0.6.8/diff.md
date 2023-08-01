# Comparing `tmp/dbt_dry_run-0.6.7.tar.gz` & `tmp/dbt_dry_run-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_dry_run-0.6.7.tar", max compression
+gzip compressed data, was "dbt_dry_run-0.6.8.tar", max compression
```

## Comparing `dbt_dry_run-0.6.7.tar` & `dbt_dry_run-0.6.8.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0    11356 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/LICENSE
--rw-r--r--   0        0        0    12394 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/README.md
--rw-r--r--   0        0        0        0 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/__init__.py
--rw-r--r--   0        0        0      110 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/__main__.py
--rw-r--r--   0        0        0        0 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/adapter/__init__.py
--rw-r--r--   0        0        0     1994 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/adapter/service.py
--rw-r--r--   0        0        0      122 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/adapter/utils.py
--rw-r--r--   0        0        0     4072 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/cli.py
--rw-r--r--   0        0        0     3691 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/columns_metadata.py
--rw-r--r--   0        0        0     1327 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/exception.py
--rw-r--r--   0        0        0     5018 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/execution.py
--rw-r--r--   0        0        0      595 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/flags.py
--rw-r--r--   0        0        0        0 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/linting/__init__.py
--rw-r--r--   0        0        0     1783 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/linting/column_linting.py
--rw-r--r--   0        0        0     4967 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/literals.py
--rw-r--r--   0        0        0      264 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/models/__init__.py
--rw-r--r--   0        0        0     4471 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/models/manifest.py
--rw-r--r--   0        0        0     2491 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/models/profile.py
--rw-r--r--   0        0        0      692 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/models/report.py
--rw-r--r--   0        0        0     2176 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/models/table.py
--rw-r--r--   0        0        0     1757 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/node_runner/__init__.py
--rw-r--r--   0        0        0     4671 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/node_runner/model_runner.py
--rw-r--r--   0        0        0      759 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/node_runner/node_test_runner.py
--rw-r--r--   0        0        0     1564 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/node_runner/seed_runner.py
--rw-r--r--   0        0        0     3861 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/node_runner/snapshot_runner.py
--rw-r--r--   0        0        0     1521 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/node_runner/source_runner.py
--rw-r--r--   0        0        0     4679 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/result_reporter.py
--rw-r--r--   0        0        0     2468 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/results.py
--rw-r--r--   0        0        0     4899 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/scheduler.py
--rw-r--r--   0        0        0      620 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/sql_runner/__init__.py
--rw-r--r--   0        0        0     3487 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/sql_runner/big_query_sql_runner.py
--rw-r--r--   0        0        0        0 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/__init__.py
--rw-r--r--   0        0        0      231 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/conftest.py
--rw-r--r--   0        0        0        0 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/linting/__init__.py
--rw-r--r--   0        0        0     1846 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/linting/test_column_linting.py
--rw-r--r--   0        0        0     1691 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/models/test_manifest.py
--rw-r--r--   0        0        0     2761 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/models/test_profile.py
--rw-r--r--   0        0        0        0 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/__init__.py
--rw-r--r--   0        0        0    15828 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/test_model_runner.py
--rw-r--r--   0        0        0     1019 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/test_node_runner.py
--rw-r--r--   0        0        0     2482 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/test_seed_runner.py
--rw-r--r--   0        0        0     9693 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/test_snapshot_runner.py
--rw-r--r--   0        0        0     2938 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/test_test_runner.py
--rw-r--r--   0        0        0        0 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/sql_runner/__init__.py
--rw-r--r--   0        0        0     4436 2023-05-02 09:26:54.669686 dbt_dry_run-0.6.7/dbt_dry_run/test/sql_runner/test_big_query_sql_runner.py
--rw-r--r--   0        0        0     5503 2023-05-02 09:26:54.669686 dbt_dry_run-0.6.7/dbt_dry_run/test/test_columns_metadata.py
--rw-r--r--   0        0        0     2678 2023-05-02 09:26:54.669686 dbt_dry_run-0.6.7/dbt_dry_run/test/test_execution.py
--rw-r--r--   0        0        0     8855 2023-05-02 09:26:54.669686 dbt_dry_run-0.6.7/dbt_dry_run/test/test_literals.py
--rw-r--r--   0        0        0     2337 2023-05-02 09:26:54.669686 dbt_dry_run-0.6.7/dbt_dry_run/test/test_result_reporter.py
--rw-r--r--   0        0        0     3831 2023-05-02 09:26:54.669686 dbt_dry_run-0.6.7/dbt_dry_run/test/test_scheduler.py
--rw-r--r--   0        0        0     1879 2023-05-02 09:26:54.669686 dbt_dry_run-0.6.7/dbt_dry_run/test/utils.py
--rw-r--r--   0        0        0      167 2023-05-02 09:26:54.669686 dbt_dry_run-0.6.7/dbt_dry_run/version.py
--rw-r--r--   0        0        0     2057 2023-05-02 09:26:54.673686 dbt_dry_run-0.6.7/pyproject.toml
--rw-r--r--   0        0        0    13340 1970-01-01 00:00:00.000000 dbt_dry_run-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/LICENSE
+-rw-r--r--   0        0        0    12394 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/README.md
+-rw-r--r--   0        0        0        0 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/__init__.py
+-rw-r--r--   0        0        0      110 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/adapter/__init__.py
+-rw-r--r--   0        0        0     1994 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/adapter/service.py
+-rw-r--r--   0        0        0      122 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/adapter/utils.py
+-rw-r--r--   0        0        0     4072 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/cli.py
+-rw-r--r--   0        0        0     3691 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/columns_metadata.py
+-rw-r--r--   0        0        0     1327 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/exception.py
+-rw-r--r--   0        0        0     5018 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/execution.py
+-rw-r--r--   0        0        0      595 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/flags.py
+-rw-r--r--   0        0        0        0 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/linting/__init__.py
+-rw-r--r--   0        0        0     1783 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/linting/column_linting.py
+-rw-r--r--   0        0        0     4967 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/literals.py
+-rw-r--r--   0        0        0      264 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/models/__init__.py
+-rw-r--r--   0        0        0     4471 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/models/manifest.py
+-rw-r--r--   0        0        0     2491 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/models/profile.py
+-rw-r--r--   0        0        0      692 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/models/report.py
+-rw-r--r--   0        0        0     2176 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/models/table.py
+-rw-r--r--   0        0        0     1757 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/node_runner/__init__.py
+-rw-r--r--   0        0        0     4671 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/node_runner/model_runner.py
+-rw-r--r--   0        0        0      759 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/node_runner/node_test_runner.py
+-rw-r--r--   0        0        0     1564 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/node_runner/seed_runner.py
+-rw-r--r--   0        0        0     3861 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/node_runner/snapshot_runner.py
+-rw-r--r--   0        0        0     1521 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/node_runner/source_runner.py
+-rw-r--r--   0        0        0     4679 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/result_reporter.py
+-rw-r--r--   0        0        0     2468 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/results.py
+-rw-r--r--   0        0        0     4899 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/scheduler.py
+-rw-r--r--   0        0        0      620 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/sql_runner/__init__.py
+-rw-r--r--   0        0        0     3487 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/sql_runner/big_query_sql_runner.py
+-rw-r--r--   0        0        0        0 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/test/__init__.py
+-rw-r--r--   0        0        0      231 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/test/conftest.py
+-rw-r--r--   0        0        0        0 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/test/linting/__init__.py
+-rw-r--r--   0        0        0     1846 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/test/linting/test_column_linting.py
+-rw-r--r--   0        0        0     1691 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/test/models/test_manifest.py
+-rw-r--r--   0        0        0     2761 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/test/models/test_profile.py
+-rw-r--r--   0        0        0        0 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/test/node_runner/__init__.py
+-rw-r--r--   0        0        0    15828 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/test/node_runner/test_model_runner.py
+-rw-r--r--   0        0        0     1019 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/test/node_runner/test_node_runner.py
+-rw-r--r--   0        0        0     2482 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/test/node_runner/test_seed_runner.py
+-rw-r--r--   0        0        0     9693 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/test/node_runner/test_snapshot_runner.py
+-rw-r--r--   0        0        0     2938 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/test/node_runner/test_test_runner.py
+-rw-r--r--   0        0        0        0 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/test/sql_runner/__init__.py
+-rw-r--r--   0        0        0     4436 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/test/sql_runner/test_big_query_sql_runner.py
+-rw-r--r--   0        0        0     5503 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/test/test_columns_metadata.py
+-rw-r--r--   0        0        0     2678 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/test/test_execution.py
+-rw-r--r--   0        0        0     8855 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/test/test_literals.py
+-rw-r--r--   0        0        0     2337 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/test/test_result_reporter.py
+-rw-r--r--   0        0        0     3831 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/test/test_scheduler.py
+-rw-r--r--   0        0        0     1879 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/test/utils.py
+-rw-r--r--   0        0        0      167 2023-08-01 10:04:53.749679 dbt_dry_run-0.6.8/dbt_dry_run/version.py
+-rw-r--r--   0        0        0     2133 2023-08-01 10:04:53.757679 dbt_dry_run-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0    13340 1970-01-01 00:00:00.000000 dbt_dry_run-0.6.8/PKG-INFO
```

### Comparing `dbt_dry_run-0.6.7/LICENSE` & `dbt_dry_run-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/README.md` & `dbt_dry_run-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/adapter/service.py` & `dbt_dry_run-0.6.8/dbt_dry_run/adapter/service.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/cli.py` & `dbt_dry_run-0.6.8/dbt_dry_run/cli.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/columns_metadata.py` & `dbt_dry_run-0.6.8/dbt_dry_run/columns_metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/exception.py` & `dbt_dry_run-0.6.8/dbt_dry_run/exception.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/execution.py` & `dbt_dry_run-0.6.8/dbt_dry_run/execution.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/flags.py` & `dbt_dry_run-0.6.8/dbt_dry_run/flags.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/linting/column_linting.py` & `dbt_dry_run-0.6.8/dbt_dry_run/linting/column_linting.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/literals.py` & `dbt_dry_run-0.6.8/dbt_dry_run/literals.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/models/manifest.py` & `dbt_dry_run-0.6.8/dbt_dry_run/models/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/models/profile.py` & `dbt_dry_run-0.6.8/dbt_dry_run/models/profile.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/models/report.py` & `dbt_dry_run-0.6.8/dbt_dry_run/models/report.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/models/table.py` & `dbt_dry_run-0.6.8/dbt_dry_run/models/table.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/node_runner/__init__.py` & `dbt_dry_run-0.6.8/dbt_dry_run/node_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/node_runner/model_runner.py` & `dbt_dry_run-0.6.8/dbt_dry_run/node_runner/model_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/node_runner/node_test_runner.py` & `dbt_dry_run-0.6.8/dbt_dry_run/node_runner/node_test_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/node_runner/seed_runner.py` & `dbt_dry_run-0.6.8/dbt_dry_run/node_runner/seed_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/node_runner/snapshot_runner.py` & `dbt_dry_run-0.6.8/dbt_dry_run/node_runner/snapshot_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/node_runner/source_runner.py` & `dbt_dry_run-0.6.8/dbt_dry_run/node_runner/source_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/result_reporter.py` & `dbt_dry_run-0.6.8/dbt_dry_run/result_reporter.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/results.py` & `dbt_dry_run-0.6.8/dbt_dry_run/results.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/scheduler.py` & `dbt_dry_run-0.6.8/dbt_dry_run/scheduler.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/sql_runner/__init__.py` & `dbt_dry_run-0.6.8/dbt_dry_run/sql_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/sql_runner/big_query_sql_runner.py` & `dbt_dry_run-0.6.8/dbt_dry_run/sql_runner/big_query_sql_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/test/linting/test_column_linting.py` & `dbt_dry_run-0.6.8/dbt_dry_run/test/linting/test_column_linting.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/test/models/test_manifest.py` & `dbt_dry_run-0.6.8/dbt_dry_run/test/models/test_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/test/models/test_profile.py` & `dbt_dry_run-0.6.8/dbt_dry_run/test/models/test_profile.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/test_model_runner.py` & `dbt_dry_run-0.6.8/dbt_dry_run/test/node_runner/test_model_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/test_node_runner.py` & `dbt_dry_run-0.6.8/dbt_dry_run/test/node_runner/test_node_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/test_seed_runner.py` & `dbt_dry_run-0.6.8/dbt_dry_run/test/node_runner/test_seed_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/test_snapshot_runner.py` & `dbt_dry_run-0.6.8/dbt_dry_run/test/node_runner/test_snapshot_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/test_test_runner.py` & `dbt_dry_run-0.6.8/dbt_dry_run/test/node_runner/test_test_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/test/sql_runner/test_big_query_sql_runner.py` & `dbt_dry_run-0.6.8/dbt_dry_run/test/sql_runner/test_big_query_sql_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/test/test_columns_metadata.py` & `dbt_dry_run-0.6.8/dbt_dry_run/test/test_columns_metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/test/test_execution.py` & `dbt_dry_run-0.6.8/dbt_dry_run/test/test_execution.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/test/test_literals.py` & `dbt_dry_run-0.6.8/dbt_dry_run/test/test_literals.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/test/test_result_reporter.py` & `dbt_dry_run-0.6.8/dbt_dry_run/test/test_result_reporter.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/test/test_scheduler.py` & `dbt_dry_run-0.6.8/dbt_dry_run/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/dbt_dry_run/test/utils.py` & `dbt_dry_run-0.6.8/dbt_dry_run/test/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.7/pyproject.toml` & `dbt_dry_run-0.6.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-dry-run"
-version = "0.6.7"
+version = "0.6.8"
 description = "Dry run dbt projects"
 authors = ["Connor Charles <connor.charles@autotrader.co.uk>",
            "Phil hope <philip.hope@autotrader.co.uk>",
            "Angelos Georgiadis <angelos.georgiadis@autotrader.co.uk>",
            "Richard Wilmer <richard.wilmer@autotrader.co.uk>"]
 readme = "README.md"
 license = "Apache-2.0"
@@ -29,29 +29,30 @@
 pytest = "^7.2.0"
 mypy = "^0.931"
 types-PyYAML = "^6.0.4"
 pytest-cov = "^4.0.0"
 twine = "^3.8.0"
 types-setuptools = "^57.4.9"
 pytest-mock = "^3.7.0"
-dbt-bigquery = "^1.5.0"
+dbt-bigquery = "^1.6.0"
 
 [build-system]
 requires = ["poetry-core>=1.5.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = "dbt_dry_run/test"
 filterwarnings = [
     "error",
     "ignore:Deprecated call to",
     "ignore:pkg_resources is deprecated as an API",
     "ignore:invalid escape sequence",
     "ignore:unclosed",
-    "ignore:'cgi' is deprecated and slated for removal"
+    "ignore:'cgi' is deprecated and slated for removal",
+    "ignore:Your application has authenticated using end user credentials"
 ]
 pythonpath = [
   "."
 ]
 
 [tool.coverage.run]
 source = ["dbt_dry_run"]
```

### Comparing `dbt_dry_run-0.6.7/PKG-INFO` & `dbt_dry_run-0.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-dry-run
-Version: 0.6.7
+Version: 0.6.8
 Summary: Dry run dbt projects
 Home-page: https://github.com/autotraderuk/dbt-dry-run
 License: Apache-2.0
 Author: Connor Charles
 Author-email: connor.charles@autotrader.co.uk
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

