# Comparing `tmp/dagster-airbyte-0.20.2.tar.gz` & `tmp/dagster-airbyte-0.20.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-airbyte-0.20.2.tar", last modified: Fri Jul 21 22:36:52 2023, max compression
+gzip compressed data, was "dagster-airbyte-0.20.3.tar", last modified: Mon Jul 31 23:06:17 2023, max compression
```

## Comparing `dagster-airbyte-0.20.2.tar` & `dagster-airbyte-0.20.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:36:52.754794 dagster-airbyte-0.20.2/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-21 22:28:10.000000 dagster-airbyte-0.20.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       67 2023-07-21 22:28:10.000000 dagster-airbyte-0.20.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      666 2023-07-21 22:36:52.754794 dagster-airbyte-0.20.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-07-21 22:28:10.000000 dagster-airbyte-0.20.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:36:52.742793 dagster-airbyte-0.20.2/dagster_airbyte/
--rw-r--r--   0 root         (0) root         (0)     1215 2023-07-21 22:28:10.000000 dagster-airbyte-0.20.2/dagster_airbyte/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44583 2023-07-21 22:28:10.000000 dagster-airbyte-0.20.2/dagster_airbyte/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)      425 2023-07-21 22:28:10.000000 dagster-airbyte-0.20.2/dagster_airbyte/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:36:52.746794 dagster-airbyte-0.20.2/dagster_airbyte/managed/
--rw-r--r--   0 root         (0) root         (0)      423 2023-07-21 22:28:10.000000 dagster-airbyte-0.20.2/dagster_airbyte/managed/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:36:52.750794 dagster-airbyte-0.20.2/dagster_airbyte/managed/generated/
--rw-r--r--   0 root         (0) root         (0)       76 2023-07-21 22:28:10.000000 dagster-airbyte-0.20.2/dagster_airbyte/managed/generated/__init__.py
--rw-r--r--   0 root         (0) root         (0)   119751 2023-07-21 22:28:10.000000 dagster-airbyte-0.20.2/dagster_airbyte/managed/generated/destinations.py
--rw-r--r--   0 root         (0) root         (0)   282784 2023-07-21 22:28:10.000000 dagster-airbyte-0.20.2/dagster_airbyte/managed/generated/sources.py
--rw-r--r--   0 root         (0) root         (0)    33752 2023-07-21 22:28:10.000000 dagster-airbyte-0.20.2/dagster_airbyte/managed/reconciliation.py
--rw-r--r--   0 root         (0) root         (0)    14161 2023-07-21 22:28:10.000000 dagster-airbyte-0.20.2/dagster_airbyte/managed/types.py
--rw-r--r--   0 root         (0) root         (0)     4128 2023-07-21 22:28:10.000000 dagster-airbyte-0.20.2/dagster_airbyte/ops.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-21 22:28:10.000000 dagster-airbyte-0.20.2/dagster_airbyte/py.typed
--rw-r--r--   0 root         (0) root         (0)    26670 2023-07-21 22:28:10.000000 dagster-airbyte-0.20.2/dagster_airbyte/resources.py
--rw-r--r--   0 root         (0) root         (0)     1434 2023-07-21 22:28:10.000000 dagster-airbyte-0.20.2/dagster_airbyte/types.py
--rw-r--r--   0 root         (0) root         (0)     2633 2023-07-21 22:28:10.000000 dagster-airbyte-0.20.2/dagster_airbyte/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-21 22:28:10.000000 dagster-airbyte-0.20.2/dagster_airbyte/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:36:52.746794 dagster-airbyte-0.20.2/dagster_airbyte.egg-info/
--rw-r--r--   0 root         (0) root         (0)      666 2023-07-21 22:36:52.000000 dagster-airbyte-0.20.2/dagster_airbyte.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      809 2023-07-21 22:36:52.000000 dagster-airbyte-0.20.2/dagster_airbyte.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 22:36:52.000000 dagster-airbyte-0.20.2/dagster_airbyte.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-07-21 22:36:52.000000 dagster-airbyte-0.20.2/dagster_airbyte.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 22:36:52.000000 dagster-airbyte-0.20.2/dagster_airbyte.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-21 22:36:52.000000 dagster-airbyte-0.20.2/dagster_airbyte.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-21 22:36:52.000000 dagster-airbyte-0.20.2/dagster_airbyte.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2023-07-21 22:36:52.754794 dagster-airbyte-0.20.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1544 2023-07-21 22:28:10.000000 dagster-airbyte-0.20.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:06:17.701247 dagster-airbyte-0.20.3/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-31 22:58:19.000000 dagster-airbyte-0.20.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       67 2023-07-31 22:58:19.000000 dagster-airbyte-0.20.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      666 2023-07-31 23:06:17.701247 dagster-airbyte-0.20.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2023-07-31 22:58:19.000000 dagster-airbyte-0.20.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:06:17.693247 dagster-airbyte-0.20.3/dagster_airbyte/
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-07-31 22:58:19.000000 dagster-airbyte-0.20.3/dagster_airbyte/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44615 2023-07-31 22:58:19.000000 dagster-airbyte-0.20.3/dagster_airbyte/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)      425 2023-07-31 22:58:19.000000 dagster-airbyte-0.20.3/dagster_airbyte/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:06:17.697247 dagster-airbyte-0.20.3/dagster_airbyte/managed/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-07-31 22:58:19.000000 dagster-airbyte-0.20.3/dagster_airbyte/managed/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:06:17.697247 dagster-airbyte-0.20.3/dagster_airbyte/managed/generated/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-07-31 22:58:19.000000 dagster-airbyte-0.20.3/dagster_airbyte/managed/generated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   119751 2023-07-31 22:58:19.000000 dagster-airbyte-0.20.3/dagster_airbyte/managed/generated/destinations.py
+-rw-r--r--   0 root         (0) root         (0)   282784 2023-07-31 22:58:19.000000 dagster-airbyte-0.20.3/dagster_airbyte/managed/generated/sources.py
+-rw-r--r--   0 root         (0) root         (0)    33752 2023-07-31 22:58:19.000000 dagster-airbyte-0.20.3/dagster_airbyte/managed/reconciliation.py
+-rw-r--r--   0 root         (0) root         (0)    14161 2023-07-31 22:58:19.000000 dagster-airbyte-0.20.3/dagster_airbyte/managed/types.py
+-rw-r--r--   0 root         (0) root         (0)     4128 2023-07-31 22:58:19.000000 dagster-airbyte-0.20.3/dagster_airbyte/ops.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-31 22:58:19.000000 dagster-airbyte-0.20.3/dagster_airbyte/py.typed
+-rw-r--r--   0 root         (0) root         (0)    26670 2023-07-31 22:58:19.000000 dagster-airbyte-0.20.3/dagster_airbyte/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1434 2023-07-31 22:58:19.000000 dagster-airbyte-0.20.3/dagster_airbyte/types.py
+-rw-r--r--   0 root         (0) root         (0)     2633 2023-07-31 22:58:19.000000 dagster-airbyte-0.20.3/dagster_airbyte/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-31 22:58:19.000000 dagster-airbyte-0.20.3/dagster_airbyte/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:06:17.693247 dagster-airbyte-0.20.3/dagster_airbyte.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      666 2023-07-31 23:06:17.000000 dagster-airbyte-0.20.3/dagster_airbyte.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      809 2023-07-31 23:06:17.000000 dagster-airbyte-0.20.3/dagster_airbyte.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 23:06:17.000000 dagster-airbyte-0.20.3/dagster_airbyte.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-31 23:06:17.000000 dagster-airbyte-0.20.3/dagster_airbyte.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 23:06:17.000000 dagster-airbyte-0.20.3/dagster_airbyte.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-31 23:06:17.000000 dagster-airbyte-0.20.3/dagster_airbyte.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-31 23:06:17.000000 dagster-airbyte-0.20.3/dagster_airbyte.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2023-07-31 23:06:17.701247 dagster-airbyte-0.20.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-07-31 22:58:19.000000 dagster-airbyte-0.20.3/setup.py
```

### Comparing `dagster-airbyte-0.20.2/LICENSE` & `dagster-airbyte-0.20.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.20.2/PKG-INFO` & `dagster-airbyte-0.20.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airbyte
-Version: 0.20.2
+Version: 0.20.3
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-airbyte-0.20.2/dagster_airbyte/__init__.py` & `dagster-airbyte-0.20.3/dagster_airbyte/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.20.2/dagster_airbyte/asset_defs.py` & `dagster-airbyte-0.20.3/dagster_airbyte/asset_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -610,15 +610,15 @@
             connection_filter=connection_filter,
             connection_to_asset_key_fn=connection_to_asset_key_fn,
             connection_to_freshness_policy_fn=connection_to_freshness_policy_fn,
             connection_to_auto_materialize_policy_fn=connection_to_auto_materialize_policy_fn,
         )
         self._workspace_id = workspace_id
         self._airbyte_instance: AirbyteResource = (
-            airbyte_resource_def
+            airbyte_resource_def.process_config_and_initialize()
             if isinstance(airbyte_resource_def, AirbyteResource)
             else airbyte_resource_def(build_init_resource_context())
         )
 
     def _get_connections(self) -> Sequence[Tuple[str, AirbyteConnectionMetadata]]:
         workspace_id = self._workspace_id
         if not workspace_id:
```

### Comparing `dagster-airbyte-0.20.2/dagster_airbyte/managed/generated/destinations.py` & `dagster-airbyte-0.20.3/dagster_airbyte/managed/generated/destinations.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.20.2/dagster_airbyte/managed/generated/sources.py` & `dagster-airbyte-0.20.3/dagster_airbyte/managed/generated/sources.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.20.2/dagster_airbyte/managed/reconciliation.py` & `dagster-airbyte-0.20.3/dagster_airbyte/managed/reconciliation.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.20.2/dagster_airbyte/managed/types.py` & `dagster-airbyte-0.20.3/dagster_airbyte/managed/types.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.20.2/dagster_airbyte/ops.py` & `dagster-airbyte-0.20.3/dagster_airbyte/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.20.2/dagster_airbyte/resources.py` & `dagster-airbyte-0.20.3/dagster_airbyte/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.20.2/dagster_airbyte/types.py` & `dagster-airbyte-0.20.3/dagster_airbyte/types.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.20.2/dagster_airbyte/utils.py` & `dagster-airbyte-0.20.3/dagster_airbyte/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.20.2/dagster_airbyte.egg-info/PKG-INFO` & `dagster-airbyte-0.20.3/dagster_airbyte.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airbyte
-Version: 0.20.2
+Version: 0.20.3
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-airbyte-0.20.2/dagster_airbyte.egg-info/SOURCES.txt` & `dagster-airbyte-0.20.3/dagster_airbyte.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.20.2/setup.py` & `dagster-airbyte-0.20.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,25 +31,25 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_airbyte_tests*"]),
     install_requires=[
-        "dagster==1.4.2",
+        "dagster==1.4.3",
         "requests",
     ],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "dagster-airbyte = dagster_airbyte.cli:main",
         ]
     },
     extras_require={
         "test": [
             "requests-mock",
         ],
         "managed": [
-            "dagster-managed-elements==0.20.2",
+            "dagster-managed-elements==0.20.3",
         ],
     },
 )
```

