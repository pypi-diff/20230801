# Comparing `tmp/dagster-airflow-1.4.2.tar.gz` & `tmp/dagster-airflow-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-airflow-1.4.2.tar", last modified: Fri Jul 21 22:36:39 2023, max compression
+gzip compressed data, was "dagster-airflow-1.4.3.tar", last modified: Mon Jul 31 23:07:57 2023, max compression
```

## Comparing `dagster-airflow-1.4.2.tar` & `dagster-airflow-1.4.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:36:39.970607 dagster-airflow-1.4.2/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      105 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      599 2023-07-21 22:36:39.970607 dagster-airflow-1.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:36:39.962607 dagster-airflow-1.4.2/dagster_airflow/
--rw-r--r--   0 root         (0) root         (0)     2474 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/dagster_airflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3759 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/dagster_airflow/airflow_dag_converter.py
--rw-r--r--   0 root         (0) root         (0)     7716 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/dagster_airflow/dagster_asset_factory.py
--rw-r--r--   0 root         (0) root         (0)     8158 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/dagster_airflow/dagster_factory.py
--rw-r--r--   0 root         (0) root         (0)     3896 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/dagster_airflow/dagster_job_factory.py
--rw-r--r--   0 root         (0) root         (0)     1763 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/dagster_airflow/dagster_schedule_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:36:39.962607 dagster-airflow-1.4.2/dagster_airflow/hooks/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/dagster_airflow/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9138 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/dagster_airflow/hooks/dagster_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:36:39.966607 dagster-airflow-1.4.2/dagster_airflow/links/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/dagster_airflow/links/__init__.py
--rw-r--r--   0 root         (0) root         (0)      842 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/dagster_airflow/links/dagster_link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:36:39.966607 dagster-airflow-1.4.2/dagster_airflow/operators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/dagster_airflow/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5170 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/dagster_airflow/operators/dagster_operator.py
--rw-r--r--   0 root         (0) root         (0)      651 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/dagster_airflow/patch_airflow_example_dag.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/dagster_airflow/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:36:39.970607 dagster-airflow-1.4.2/dagster_airflow/resources/
--rw-r--r--   0 root         (0) root         (0)      324 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/dagster_airflow/resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3966 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/dagster_airflow/resources/airflow_db.py
--rw-r--r--   0 root         (0) root         (0)     3659 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/dagster_airflow/resources/airflow_ephemeral_db.py
--rw-r--r--   0 root         (0) root         (0)     4037 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/dagster_airflow/resources/airflow_persistent_db.py
--rw-r--r--   0 root         (0) root         (0)     4496 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/dagster_airflow/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/dagster_airflow/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:36:39.962607 dagster-airflow-1.4.2/dagster_airflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      599 2023-07-21 22:36:39.000000 dagster-airflow-1.4.2/dagster_airflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1041 2023-07-21 22:36:39.000000 dagster-airflow-1.4.2/dagster_airflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 22:36:39.000000 dagster-airflow-1.4.2/dagster_airflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      168 2023-07-21 22:36:39.000000 dagster-airflow-1.4.2/dagster_airflow.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      469 2023-07-21 22:36:39.000000 dagster-airflow-1.4.2/dagster_airflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-21 22:36:39.000000 dagster-airflow-1.4.2/dagster_airflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      192 2023-07-21 22:36:39.970607 dagster-airflow-1.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2588 2023-07-21 22:28:10.000000 dagster-airflow-1.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:07:57.821989 dagster-airflow-1.4.3/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      599 2023-07-31 23:07:57.821989 dagster-airflow-1.4.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:07:57.813989 dagster-airflow-1.4.3/dagster_airflow/
+-rw-r--r--   0 root         (0) root         (0)     2474 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/dagster_airflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3815 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/dagster_airflow/airflow_dag_converter.py
+-rw-r--r--   0 root         (0) root         (0)     7716 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/dagster_airflow/dagster_asset_factory.py
+-rw-r--r--   0 root         (0) root         (0)     8158 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/dagster_airflow/dagster_factory.py
+-rw-r--r--   0 root         (0) root         (0)     3896 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/dagster_airflow/dagster_job_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/dagster_airflow/dagster_schedule_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:07:57.813989 dagster-airflow-1.4.3/dagster_airflow/hooks/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/dagster_airflow/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9138 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/dagster_airflow/hooks/dagster_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:07:57.817989 dagster-airflow-1.4.3/dagster_airflow/links/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/dagster_airflow/links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      842 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/dagster_airflow/links/dagster_link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:07:57.817989 dagster-airflow-1.4.3/dagster_airflow/operators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/dagster_airflow/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5170 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/dagster_airflow/operators/dagster_operator.py
+-rw-r--r--   0 root         (0) root         (0)      651 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/dagster_airflow/patch_airflow_example_dag.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/dagster_airflow/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:07:57.821989 dagster-airflow-1.4.3/dagster_airflow/resources/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/dagster_airflow/resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3966 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/dagster_airflow/resources/airflow_db.py
+-rw-r--r--   0 root         (0) root         (0)     3659 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/dagster_airflow/resources/airflow_ephemeral_db.py
+-rw-r--r--   0 root         (0) root         (0)     4037 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/dagster_airflow/resources/airflow_persistent_db.py
+-rw-r--r--   0 root         (0) root         (0)     4496 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/dagster_airflow/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/dagster_airflow/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:07:57.813989 dagster-airflow-1.4.3/dagster_airflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      599 2023-07-31 23:07:57.000000 dagster-airflow-1.4.3/dagster_airflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-07-31 23:07:57.000000 dagster-airflow-1.4.3/dagster_airflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 23:07:57.000000 dagster-airflow-1.4.3/dagster_airflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      168 2023-07-31 23:07:57.000000 dagster-airflow-1.4.3/dagster_airflow.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      469 2023-07-31 23:07:57.000000 dagster-airflow-1.4.3/dagster_airflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-31 23:07:57.000000 dagster-airflow-1.4.3/dagster_airflow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      192 2023-07-31 23:07:57.821989 dagster-airflow-1.4.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-07-31 22:58:19.000000 dagster-airflow-1.4.3/setup.py
```

### Comparing `dagster-airflow-1.4.2/LICENSE` & `dagster-airflow-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.4.2/PKG-INFO` & `dagster-airflow-1.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airflow
-Version: 1.4.2
+Version: 1.4.3
 Summary: Airflow plugin for Dagster
 Home-page: https://github.com/dagster-io/dagster
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: project-url/documentation, https://docs.dagster.io
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-airflow-1.4.2/dagster_airflow/__init__.py` & `dagster-airflow-1.4.3/dagster_airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.4.2/dagster_airflow/airflow_dag_converter.py` & `dagster-airflow-1.4.3/dagster_airflow/airflow_dag_converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import importlib
+from typing import TYPE_CHECKING
 
 import airflow
-from airflow.models.baseoperator import BaseOperator
 from airflow.models.dag import DAG
 from dagster import (
     DependencyDefinition,
     In,
     MultiDependencyDefinition,
     Nothing,
     OpDefinition,
@@ -19,14 +19,17 @@
 
 from dagster_airflow.utils import (
     is_airflow_2_loaded_in_environment,
     normalized_name,
     replace_airflow_logger_handlers,
 )
 
+if TYPE_CHECKING:
+    from airflow.models.baseoperator import BaseOperator
+
 
 def get_graph_definition_args(
     dag: DAG,
 ):
     check.inst_param(dag, "dag", DAG)
 
     dependencies: dict[str, dict[str, MultiDependencyDefinition]] = {}
```

### Comparing `dagster-airflow-1.4.2/dagster_airflow/dagster_asset_factory.py` & `dagster-airflow-1.4.3/dagster_airflow/dagster_asset_factory.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.4.2/dagster_airflow/dagster_factory.py` & `dagster-airflow-1.4.3/dagster_airflow/dagster_factory.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.4.2/dagster_airflow/dagster_job_factory.py` & `dagster-airflow-1.4.3/dagster_airflow/dagster_job_factory.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.4.2/dagster_airflow/dagster_schedule_factory.py` & `dagster-airflow-1.4.3/dagster_airflow/dagster_schedule_factory.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.4.2/dagster_airflow/hooks/dagster_hook.py` & `dagster-airflow-1.4.3/dagster_airflow/hooks/dagster_hook.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.4.2/dagster_airflow/links/dagster_link.py` & `dagster-airflow-1.4.3/dagster_airflow/links/dagster_link.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.4.2/dagster_airflow/operators/dagster_operator.py` & `dagster-airflow-1.4.3/dagster_airflow/operators/dagster_operator.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.4.2/dagster_airflow/patch_airflow_example_dag.py` & `dagster-airflow-1.4.3/dagster_airflow/patch_airflow_example_dag.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.4.2/dagster_airflow/resources/airflow_db.py` & `dagster-airflow-1.4.3/dagster_airflow/resources/airflow_db.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.4.2/dagster_airflow/resources/airflow_ephemeral_db.py` & `dagster-airflow-1.4.3/dagster_airflow/resources/airflow_ephemeral_db.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.4.2/dagster_airflow/resources/airflow_persistent_db.py` & `dagster-airflow-1.4.3/dagster_airflow/resources/airflow_persistent_db.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.4.2/dagster_airflow/utils.py` & `dagster-airflow-1.4.3/dagster_airflow/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.4.2/dagster_airflow.egg-info/PKG-INFO` & `dagster-airflow-1.4.3/dagster_airflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airflow
-Version: 1.4.2
+Version: 1.4.3
 Summary: Airflow plugin for Dagster
 Home-page: https://github.com/dagster-io/dagster
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: project-url/documentation, https://docs.dagster.io
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-airflow-1.4.2/dagster_airflow.egg-info/SOURCES.txt` & `dagster-airflow-1.4.3/dagster_airflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.4.2/setup.py` & `dagster-airflow-1.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_airflow_tests*"]),
     install_requires=[
-        "dagster==1.4.2",
+        "dagster==1.4.3",
         "docker>=5.0.3,<6.0.0",
         "lazy_object_proxy",
         "pendulum",
     ],
     project_urls={
         # airflow will embed a link this in the providers page UI
         "project-url/documentation": "https://docs.dagster.io",
```

