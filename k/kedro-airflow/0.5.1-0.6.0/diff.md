# Comparing `tmp/kedro-airflow-0.5.1.tar.gz` & `tmp/kedro-airflow-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-airflow-0.5.1.tar", last modified: Thu Nov 24 18:01:29 2022, max compression
+gzip compressed data, was "kedro-airflow-0.6.0.tar", last modified: Tue Aug  1 12:38:20 2023, max compression
```

## Comparing `kedro-airflow-0.5.1.tar` & `kedro-airflow-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-24 18:01:29.963145 kedro-airflow-0.5.1/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      108 2022-11-24 17:59:45.000000 kedro-airflow-0.5.1/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3594 2022-11-24 18:01:29.963145 kedro-airflow-0.5.1/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3255 2022-11-24 17:59:45.000000 kedro-airflow-0.5.1/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-24 18:01:29.963145 kedro-airflow-0.5.1/kedro_airflow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       79 2022-11-24 17:59:45.000000 kedro-airflow-0.5.1/kedro_airflow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2565 2022-11-24 17:59:45.000000 kedro-airflow-0.5.1/kedro_airflow/airflow_dag_template.j2
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3030 2022-11-24 17:59:45.000000 kedro-airflow-0.5.1/kedro_airflow/plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-24 18:01:29.963145 kedro-airflow-0.5.1/kedro_airflow.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3594 2022-11-24 18:01:29.000000 kedro-airflow-0.5.1/kedro_airflow.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      420 2022-11-24 18:01:29.000000 kedro-airflow-0.5.1/kedro_airflow.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2022-11-24 18:01:29.000000 kedro-airflow-0.5.1/kedro_airflow.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       65 2022-11-24 18:01:29.000000 kedro-airflow-0.5.1/kedro_airflow.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2022-11-24 18:01:29.000000 kedro-airflow-0.5.1/kedro_airflow.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       47 2022-11-24 18:01:29.000000 kedro-airflow-0.5.1/kedro_airflow.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       14 2022-11-24 18:01:29.000000 kedro-airflow-0.5.1/kedro_airflow.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       37 2022-11-24 17:59:45.000000 kedro-airflow-0.5.1/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      102 2022-11-24 17:59:45.000000 kedro-airflow-0.5.1/requirements.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      218 2022-11-24 18:01:29.963145 kedro-airflow-0.5.1/setup.cfg
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1343 2022-11-24 17:59:45.000000 kedro-airflow-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:38:20.483524 kedro-airflow-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-01 12:38:08.000000 kedro-airflow-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-08-01 12:38:20.483524 kedro-airflow-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-08-01 12:38:08.000000 kedro-airflow-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:38:20.479524 kedro-airflow-0.6.0/kedro_airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 12:38:08.000000 kedro-airflow-0.6.0/kedro_airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-08-01 12:38:08.000000 kedro-airflow-0.6.0/kedro_airflow/airflow_dag_template.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-08-01 12:38:08.000000 kedro-airflow-0.6.0/kedro_airflow/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:38:20.483524 kedro-airflow-0.6.0/kedro_airflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-08-01 12:38:20.000000 kedro-airflow-0.6.0/kedro_airflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-01 12:38:20.000000 kedro-airflow-0.6.0/kedro_airflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:38:20.000000 kedro-airflow-0.6.0/kedro_airflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-01 12:38:20.000000 kedro-airflow-0.6.0/kedro_airflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:38:20.000000 kedro-airflow-0.6.0/kedro_airflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-01 12:38:20.000000 kedro-airflow-0.6.0/kedro_airflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 12:38:20.000000 kedro-airflow-0.6.0/kedro_airflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-08-01 12:38:08.000000 kedro-airflow-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 12:38:20.483524 kedro-airflow-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:38:20.483524 kedro-airflow-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-08-01 12:38:08.000000 kedro-airflow-0.6.0/tests/test_plugin.py
```

### Comparing `kedro-airflow-0.5.1/kedro_airflow/airflow_dag_template.j2` & `kedro-airflow-0.6.0/kedro_airflow/airflow_dag_template.j2`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,27 @@
-from collections import defaultdict
-
+from __future__ import annotations
+from datetime import datetime, timedelta
 from pathlib import Path
 
 from airflow import DAG
 from airflow.models import BaseOperator
 from airflow.utils.decorators import apply_defaults
-from airflow.version import version
-from datetime import datetime, timedelta
 
 from kedro.framework.session import KedroSession
 from kedro.framework.project import configure_project
 
 
 class KedroOperator(BaseOperator):
-
     @apply_defaults
     def __init__(
         self,
         package_name: str,
         pipeline_name: str,
         node_name: str,
-        project_path: str,
+        project_path: str | Path,
         env: str,
         *args, **kwargs
     ) -> None:
         super().__init__(*args, **kwargs)
         self.package_name = package_name
         self.pipeline_name = pipeline_name
         self.node_name = node_name
@@ -34,50 +31,47 @@
     def execute(self, context):
         configure_project(self.package_name)
         with KedroSession.create(self.package_name,
                                  self.project_path,
                                  env=self.env) as session:
             session.run(self.pipeline_name, node_names=[self.node_name])
 
+
 # Kedro settings required to run your pipeline
 env = "{{ env }}"
 pipeline_name = "{{ pipeline_name }}"
 project_path = Path.cwd()
 package_name = "{{ package_name }}"
 
-# Default settings applied to all tasks
-default_args = {
-    'owner': 'airflow',
-    'depends_on_past': False,
-    'email_on_failure': False,
-    'email_on_retry': False,
-    'retries': 1,
-    'retry_delay': timedelta(minutes=5)
-}
-
 # Using a DAG context manager, you don't have to specify the dag property of each task
 with DAG(
-    "{{ dag_name | safe | slugify }}",
-    start_date=datetime(2019, 1, 1),
-    max_active_runs=3,
-    schedule_interval=timedelta(minutes=30),  # https://airflow.apache.org/docs/stable/scheduler.html#dag-runs
-    default_args=default_args,
-    catchup=False # enable if you don't want historical dag runs to run
-) as dag:
-
-    tasks = {}
-    {% for node in pipeline.nodes %}
-    tasks["{{ node.name | safe | slugify }}"] = KedroOperator(
-        task_id="{{ node.name | safe | slugify  }}",
-        package_name=package_name,
-        pipeline_name=pipeline_name,
-        node_name="{{ node.name | safe }}",
-        project_path=project_path,
-        env=env,
+    dag_id="{{ dag_name | safe | slugify }}",
+    start_date=datetime({{ start_date | default([2023, 1, 1]) | join(",")}}),
+    max_active_runs={{ max_active_runs | default(3) }},
+    # https://airflow.apache.org/docs/stable/scheduler.html#dag-runs
+    schedule_interval="{{ schedule_interval | default('@once') }}",
+    catchup={{ catchup | default(False) }},
+    # Default settings applied to all tasks
+    default_args=dict(
+        owner="{{ owner | default('airflow') }}",
+        depends_on_past={{ depends_on_past | default(False) }},
+        email_on_failure={{ email_on_failure | default(False) }},
+        email_on_retry={{ email_on_retry | default(False) }},
+        retries={{ retries | default(1) }},
+        retry_delay=timedelta(minutes={{ retry_delay | default(5) }})
     )
-    {% endfor %}
+) as dag:
+    tasks = {
+    {% for node in pipeline.nodes %}        "{{ node.name | safe | slugify }}": KedroOperator(
+            task_id="{{ node.name | safe | slugify  }}",
+            package_name=package_name,
+            pipeline_name=pipeline_name,
+            node_name="{{ node.name | safe }}",
+            project_path=project_path,
+            env=env,
+        ),
+{% endfor %}    }
 
     {% for parent_node, child_nodes in dependencies.items() -%}
-    {% for child in child_nodes %}
-    tasks["{{ parent_node.name | safe | slugify }}"] >> tasks["{{ child.name | safe | slugify }}"]
+    {% for child in child_nodes %}    tasks["{{ parent_node.name | safe | slugify }}"] >> tasks["{{ child.name | safe | slugify }}"]
     {% endfor %}
     {%- endfor %}
```

