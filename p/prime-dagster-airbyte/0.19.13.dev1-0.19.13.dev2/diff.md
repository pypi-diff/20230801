# Comparing `tmp/prime-dagster-airbyte-0.19.13.dev1.tar.gz` & `tmp/prime-dagster-airbyte-0.19.13.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prime-dagster-airbyte-0.19.13.dev1.tar", last modified: Thu Jul 27 07:44:01 2023, max compression
+gzip compressed data, was "prime-dagster-airbyte-0.19.13.dev2.tar", last modified: Tue Aug  1 04:43:04 2023, max compression
```

## Comparing `prime-dagster-airbyte-0.19.13.dev1.tar` & `prime-dagster-airbyte-0.19.13.dev2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 huy        (503) staff       (20)        0 2023-07-27 07:44:01.213167 prime-dagster-airbyte-0.19.13.dev1/
--rw-r--r--   0 huy        (503) staff       (20)    11344 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev1/LICENSE
--rw-r--r--   0 huy        (503) staff       (20)       67 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev1/MANIFEST.in
--rw-r--r--   0 huy        (503) staff       (20)      730 2023-07-27 07:44:01.213280 prime-dagster-airbyte-0.19.13.dev1/PKG-INFO
--rw-r--r--   0 huy        (503) staff       (20)      131 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev1/README.md
-drwxr-xr-x   0 huy        (503) staff       (20)        0 2023-07-27 07:44:01.208435 prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/
--rw-r--r--   0 huy        (503) staff       (20)     1215 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/__init__.py
--rw-r--r--   0 huy        (503) staff       (20)    44337 2023-07-12 08:21:37.000000 prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/asset_defs.py
--rw-r--r--   0 huy        (503) staff       (20)      425 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/cli.py
-drwxr-xr-x   0 huy        (503) staff       (20)        0 2023-07-27 07:44:01.209235 prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/managed/
--rw-r--r--   0 huy        (503) staff       (20)      423 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/managed/__init__.py
-drwxr-xr-x   0 huy        (503) staff       (20)        0 2023-07-27 07:44:01.210838 prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/managed/generated/
--rw-r--r--   0 huy        (503) staff       (20)       76 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/managed/generated/__init__.py
--rw-r--r--   0 huy        (503) staff       (20)   119751 2023-07-17 04:04:28.000000 prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/managed/generated/destinations.py
--rw-r--r--   0 huy        (503) staff       (20)   282784 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/managed/generated/sources.py
--rw-r--r--   0 huy        (503) staff       (20)    34033 2023-07-27 07:09:00.000000 prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/managed/reconciliation.py
--rw-r--r--   0 huy        (503) staff       (20)    14161 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/managed/types.py
--rw-r--r--   0 huy        (503) staff       (20)     4128 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/ops.py
--rw-r--r--   0 huy        (503) staff       (20)        8 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/py.typed
--rw-r--r--   0 huy        (503) staff       (20)    26816 2023-07-17 03:32:27.000000 prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/resources.py
--rw-r--r--   0 huy        (503) staff       (20)     1434 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/types.py
--rw-r--r--   0 huy        (503) staff       (20)     2633 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/utils.py
--rw-r--r--   0 huy        (503) staff       (20)       28 2023-07-27 07:32:21.000000 prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/version.py
-drwxr-xr-x   0 huy        (503) staff       (20)        0 2023-07-27 07:44:01.213051 prime-dagster-airbyte-0.19.13.dev1/prime_dagster_airbyte.egg-info/
--rw-r--r--   0 huy        (503) staff       (20)      730 2023-07-27 07:44:01.000000 prime-dagster-airbyte-0.19.13.dev1/prime_dagster_airbyte.egg-info/PKG-INFO
--rw-r--r--   0 huy        (503) staff       (20)      851 2023-07-27 07:44:01.000000 prime-dagster-airbyte-0.19.13.dev1/prime_dagster_airbyte.egg-info/SOURCES.txt
--rw-r--r--   0 huy        (503) staff       (20)        1 2023-07-27 07:44:01.000000 prime-dagster-airbyte-0.19.13.dev1/prime_dagster_airbyte.egg-info/dependency_links.txt
--rw-r--r--   0 huy        (503) staff       (20)       61 2023-07-27 07:44:01.000000 prime-dagster-airbyte-0.19.13.dev1/prime_dagster_airbyte.egg-info/entry_points.txt
--rw-r--r--   0 huy        (503) staff       (20)        1 2023-07-27 07:42:56.000000 prime-dagster-airbyte-0.19.13.dev1/prime_dagster_airbyte.egg-info/not-zip-safe
--rw-r--r--   0 huy        (503) staff       (20)       89 2023-07-27 07:44:01.000000 prime-dagster-airbyte-0.19.13.dev1/prime_dagster_airbyte.egg-info/requires.txt
--rw-r--r--   0 huy        (503) staff       (20)       16 2023-07-27 07:44:01.000000 prime-dagster-airbyte-0.19.13.dev1/prime_dagster_airbyte.egg-info/top_level.txt
--rw-r--r--   0 huy        (503) staff       (20)      162 2023-07-27 07:44:01.213611 prime-dagster-airbyte-0.19.13.dev1/setup.cfg
--rw-r--r--   0 huy        (503) staff       (20)     1617 2023-07-27 07:42:41.000000 prime-dagster-airbyte-0.19.13.dev1/setup.py
+drwxr-xr-x   0 huy        (503) staff       (20)        0 2023-08-01 04:43:04.280694 prime-dagster-airbyte-0.19.13.dev2/
+-rw-r--r--   0 huy        (503) staff       (20)    11344 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev2/LICENSE
+-rw-r--r--   0 huy        (503) staff       (20)       67 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev2/MANIFEST.in
+-rw-r--r--   0 huy        (503) staff       (20)      730 2023-08-01 04:43:04.280773 prime-dagster-airbyte-0.19.13.dev2/PKG-INFO
+-rw-r--r--   0 huy        (503) staff       (20)      131 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev2/README.md
+drwxr-xr-x   0 huy        (503) staff       (20)        0 2023-08-01 04:43:04.273658 prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/
+-rw-r--r--   0 huy        (503) staff       (20)     1215 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/__init__.py
+-rw-r--r--   0 huy        (503) staff       (20)    44337 2023-07-12 08:21:37.000000 prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/asset_defs.py
+-rw-r--r--   0 huy        (503) staff       (20)      425 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/cli.py
+drwxr-xr-x   0 huy        (503) staff       (20)        0 2023-08-01 04:43:04.275594 prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/managed/
+-rw-r--r--   0 huy        (503) staff       (20)      423 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/managed/__init__.py
+drwxr-xr-x   0 huy        (503) staff       (20)        0 2023-08-01 04:43:04.278027 prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/managed/generated/
+-rw-r--r--   0 huy        (503) staff       (20)       76 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/managed/generated/__init__.py
+-rw-r--r--   0 huy        (503) staff       (20)   119751 2023-07-17 04:04:28.000000 prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/managed/generated/destinations.py
+-rw-r--r--   0 huy        (503) staff       (20)   282784 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/managed/generated/sources.py
+-rw-r--r--   0 huy        (503) staff       (20)    34030 2023-08-01 04:41:17.000000 prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/managed/reconciliation.py
+-rw-r--r--   0 huy        (503) staff       (20)    14161 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/managed/types.py
+-rw-r--r--   0 huy        (503) staff       (20)     4128 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/ops.py
+-rw-r--r--   0 huy        (503) staff       (20)        8 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/py.typed
+-rw-r--r--   0 huy        (503) staff       (20)    26816 2023-07-17 03:32:27.000000 prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/resources.py
+-rw-r--r--   0 huy        (503) staff       (20)     1434 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/types.py
+-rw-r--r--   0 huy        (503) staff       (20)     2633 2023-07-12 08:14:59.000000 prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/utils.py
+-rw-r--r--   0 huy        (503) staff       (20)       28 2023-08-01 04:42:55.000000 prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/version.py
+drwxr-xr-x   0 huy        (503) staff       (20)        0 2023-08-01 04:43:04.280581 prime-dagster-airbyte-0.19.13.dev2/prime_dagster_airbyte.egg-info/
+-rw-r--r--   0 huy        (503) staff       (20)      730 2023-08-01 04:43:04.000000 prime-dagster-airbyte-0.19.13.dev2/prime_dagster_airbyte.egg-info/PKG-INFO
+-rw-r--r--   0 huy        (503) staff       (20)      851 2023-08-01 04:43:04.000000 prime-dagster-airbyte-0.19.13.dev2/prime_dagster_airbyte.egg-info/SOURCES.txt
+-rw-r--r--   0 huy        (503) staff       (20)        1 2023-08-01 04:43:04.000000 prime-dagster-airbyte-0.19.13.dev2/prime_dagster_airbyte.egg-info/dependency_links.txt
+-rw-r--r--   0 huy        (503) staff       (20)       61 2023-08-01 04:43:04.000000 prime-dagster-airbyte-0.19.13.dev2/prime_dagster_airbyte.egg-info/entry_points.txt
+-rw-r--r--   0 huy        (503) staff       (20)        1 2023-07-27 07:42:56.000000 prime-dagster-airbyte-0.19.13.dev2/prime_dagster_airbyte.egg-info/not-zip-safe
+-rw-r--r--   0 huy        (503) staff       (20)       89 2023-08-01 04:43:04.000000 prime-dagster-airbyte-0.19.13.dev2/prime_dagster_airbyte.egg-info/requires.txt
+-rw-r--r--   0 huy        (503) staff       (20)       16 2023-08-01 04:43:04.000000 prime-dagster-airbyte-0.19.13.dev2/prime_dagster_airbyte.egg-info/top_level.txt
+-rw-r--r--   0 huy        (503) staff       (20)      162 2023-08-01 04:43:04.281043 prime-dagster-airbyte-0.19.13.dev2/setup.cfg
+-rw-r--r--   0 huy        (503) staff       (20)     1617 2023-07-27 07:42:41.000000 prime-dagster-airbyte-0.19.13.dev2/setup.py
```

### Comparing `prime-dagster-airbyte-0.19.13.dev1/LICENSE` & `prime-dagster-airbyte-0.19.13.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `prime-dagster-airbyte-0.19.13.dev1/PKG-INFO` & `prime-dagster-airbyte-0.19.13.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prime-dagster-airbyte
-Version: 0.19.13.dev1
+Version: 0.19.13.dev2
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/huylenq/dagster/tree/master/python_modules/libraries/dagster-airbyte
 Author: Elementl, Huy
 Author-email: huy.lenq@gmail.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/__init__.py` & `prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/__init__.py`

 * *Files identical despite different names*

### Comparing `prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/asset_defs.py` & `prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/asset_defs.py`

 * *Files identical despite different names*

### Comparing `prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/managed/generated/destinations.py` & `prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/managed/generated/destinations.py`

 * *Files identical despite different names*

### Comparing `prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/managed/generated/sources.py` & `prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/managed/generated/sources.py`

 * *Files identical despite different names*

### Comparing `prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/managed/reconciliation.py` & `prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/managed/reconciliation.py`

 * *Files 0% similar despite different names*

```diff
@@ -725,15 +725,15 @@
             upstream_assets=upstream_assets,
         )
         self._connections: List[AirbyteConnection] = list(connections)
 
     def _get_connections(self) -> Sequence[Tuple[str, AirbyteConnectionMetadata]]:
         diff = reconcile_config(self._airbyte_instance, self._connections, dry_run=True)
         if isinstance(diff, ManagedElementDiff) and not diff.is_empty():
-            print('>>> ⚠️ BY PASSING CONNETION SYNCING CHECK!')
+            print("⚠️ ️BY PASSING CONNECTION SYNC CHECK!")
             # raise ValueError(
             #     "Airbyte connections are not in sync with provided configuration, diff:\n{}".format(
             #         str(diff)
             #     )
             # )
         elif isinstance(diff, ManagedElementError):
             raise ValueError(f"Error checking Airbyte connections: {diff}")
```

### Comparing `prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/managed/types.py` & `prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/managed/types.py`

 * *Files identical despite different names*

### Comparing `prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/ops.py` & `prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/ops.py`

 * *Files identical despite different names*

### Comparing `prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/resources.py` & `prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/resources.py`

 * *Files identical despite different names*

### Comparing `prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/types.py` & `prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/types.py`

 * *Files identical despite different names*

### Comparing `prime-dagster-airbyte-0.19.13.dev1/dagster_airbyte/utils.py` & `prime-dagster-airbyte-0.19.13.dev2/dagster_airbyte/utils.py`

 * *Files identical despite different names*

### Comparing `prime-dagster-airbyte-0.19.13.dev1/prime_dagster_airbyte.egg-info/PKG-INFO` & `prime-dagster-airbyte-0.19.13.dev2/prime_dagster_airbyte.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prime-dagster-airbyte
-Version: 0.19.13.dev1
+Version: 0.19.13.dev2
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/huylenq/dagster/tree/master/python_modules/libraries/dagster-airbyte
 Author: Elementl, Huy
 Author-email: huy.lenq@gmail.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `prime-dagster-airbyte-0.19.13.dev1/prime_dagster_airbyte.egg-info/SOURCES.txt` & `prime-dagster-airbyte-0.19.13.dev2/prime_dagster_airbyte.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prime-dagster-airbyte-0.19.13.dev1/setup.py` & `prime-dagster-airbyte-0.19.13.dev2/setup.py`

 * *Files identical despite different names*

