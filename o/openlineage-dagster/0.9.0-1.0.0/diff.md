# Comparing `tmp/openlineage-dagster-0.9.0.tar.gz` & `tmp/openlineage-dagster-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openlineage-dagster-0.9.0.tar", last modified: Fri Jun  3 23:03:15 2022, max compression
+gzip compressed data, was "openlineage-dagster-1.0.0.tar", last modified: Tue Aug  1 19:46:06 2023, max compression
```

## Comparing `openlineage-dagster-0.9.0.tar` & `openlineage-dagster-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,27 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5547 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4319 2022-06-03 23:03:13.000000 openlineage-dagster-0.9.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/openlineage/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/openlineage/dagster/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      566 2022-06-03 23:03:13.000000 openlineage-dagster-0.9.0/openlineage/dagster/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9528 2022-06-03 23:03:13.000000 openlineage-dagster-0.9.0/openlineage/dagster/adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      829 2022-06-03 23:03:13.000000 openlineage-dagster-0.9.0/openlineage/dagster/cursor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9738 2022-06-03 23:03:13.000000 openlineage-dagster-0.9.0/openlineage/dagster/sensor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2492 2022-06-03 23:03:13.000000 openlineage-dagster-0.9.0/openlineage/dagster/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/openlineage_dagster.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5547 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/openlineage_dagster.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      436 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/openlineage_dagster.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/openlineage_dagster.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/openlineage_dagster.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      153 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/openlineage_dagster.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/openlineage_dagster.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      554 2022-06-03 23:03:15.000000 openlineage-dagster-0.9.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1577 2022-06-03 23:03:13.000000 openlineage-dagster-0.9.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:46:06.934239 openlineage-dagster-1.0.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4890 2023-08-01 19:46:06.934239 openlineage-dagster-1.0.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4632 2023-08-01 19:46:01.000000 openlineage-dagster-1.0.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:46:06.930240 openlineage-dagster-1.0.0/openlineage/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:46:06.930240 openlineage-dagster-1.0.0/openlineage/dagster/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      123 2023-08-01 19:46:01.000000 openlineage-dagster-1.0.0/openlineage/dagster/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9129 2023-08-01 19:46:01.000000 openlineage-dagster-1.0.0/openlineage/dagster/adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      930 2023-08-01 19:46:01.000000 openlineage-dagster-1.0.0/openlineage/dagster/cursor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9330 2023-08-01 19:46:01.000000 openlineage-dagster-1.0.0/openlineage/dagster/sensor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2065 2023-08-01 19:46:01.000000 openlineage-dagster-1.0.0/openlineage/dagster/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:46:06.934239 openlineage-dagster-1.0.0/openlineage_dagster.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4890 2023-08-01 19:46:06.000000 openlineage-dagster-1.0.0/openlineage_dagster.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      618 2023-08-01 19:46:06.000000 openlineage-dagster-1.0.0/openlineage_dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-01 19:46:06.000000 openlineage-dagster-1.0.0/openlineage_dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-01 19:46:06.000000 openlineage-dagster-1.0.0/openlineage_dagster.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      207 2023-08-01 19:46:06.000000 openlineage-dagster-1.0.0/openlineage_dagster.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-08-01 19:46:06.000000 openlineage-dagster-1.0.0/openlineage_dagster.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      214 2023-08-01 19:46:01.000000 openlineage-dagster-1.0.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      618 2023-08-01 19:46:06.934239 openlineage-dagster-1.0.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1181 2023-08-01 19:46:01.000000 openlineage-dagster-1.0.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:46:06.934239 openlineage-dagster-1.0.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      493 2023-08-01 19:46:01.000000 openlineage-dagster-1.0.0/tests/test_adapter_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4509 2023-08-01 19:46:01.000000 openlineage-dagster-1.0.0/tests/test_adapter_pipeline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4885 2023-08-01 19:46:01.000000 openlineage-dagster-1.0.0/tests/test_adapter_step.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9250 2023-08-01 19:46:01.000000 openlineage-dagster-1.0.0/tests/test_sensor_cursor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8909 2023-08-01 19:46:01.000000 openlineage-dagster-1.0.0/tests/test_sensor_evaluation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1752 2023-08-01 19:46:01.000000 openlineage-dagster-1.0.0/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `openlineage-dagster-0.9.0/PKG-INFO` & `openlineage-dagster-1.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,127 +1,121 @@
-Metadata-Version: 2.1
-Name: openlineage-dagster
-Version: 0.9.0
-Summary: OpenLineage integration with Dagster
-Home-page: UNKNOWN
-Author: OpenLineage
-License: UNKNOWN
-Description: # OpenLineage Dagster Integration
-        
-        A library that integrates [Dagster](https://dagster.io/) with [OpenLineage](https://openlineage.io) for automatic metadata collection.
-        It provides an OpenLineage sensor, a Dagster sensor that tails Dagster event logs for tracking metadata.
-        On each sensor evaluation, the function processes a batch of event logs, converts Dagster events into OpenLineage events, 
-        and emits them to an OpenLineage backend.
-        
-        ## Features
-        
-        **Metadata**
-        
-        * Dagster job & op lifecycle
-        
-        ## Requirements
-        
-        - [Python 3.7](https://www.python.org/downloads)
-        - [Dagster 0.13.8+](https://dagster.io/)
-        
-        ## Installation
-        
-        ```bash
-        $ python -m pip install openlineage-dagster
-        ```
-        
-        ## Usage
-        
-        ### OpenLineage Sensor & Event Log Storage Requirements
-        
-        **Single OpenLineage sensor per Dagster instance** <br />
-        As it processes all event logs for a given Dagster instance, define and enable only a single OpenLineage sensor per instance. 
-        Running multiple will result in emitting duplicate OpenLineage job runs for Dagster steps with different OpenLineage run ids that are dynamically generated during sensor runs.
-        
-        **Non-sharded [Event Log Storage](https://docs.dagster.io/deployment/dagster-instance#event-log-storage)** <br />
-        For the sensor to handle all event logs across runs, use non-sharded event log storage.
-        If an event log storage sharded by run (i.e. default `SqliteEventLogStorage`) is used, cursor that tracks the last processed event storage id may not update properly. 
-        
-        ### OpenLineage Sensor Setup
-        
-        Get OpenLineage sensor definition from `openlineage_sensor()` factory function and add it to your Dagster repository.
-        
-        ```python
-        from dagster import repository
-        from openlineage.dagster.sensor import openlineage_sensor
-        
-        
-        @repository
-        def my_repository():
-            openlineage_sensor_def = openlineage_sensor()
-            return other_defs + [openlineage_sensor_def]
-        ```
-        
-        With parallel sensor run not supported at the time of writing, some tuning may be necessary to avoid affecting other sensors' performance.
-        
-        See Dagster's documentation on [Evaluation Interval](https://docs.dagster.io/concepts/partitions-schedules-sensors/sensors#evaluation-interval)
-        for more detail on `minimum_interval_seconds`, which defaults to 30 seconds.
-        `record_filter_limit` is the maximum number of event logs to process on each sensor evaluation, and it defaults to 30 records per evaluation.
-        Default values can be overridden as below.
-        
-        ```python
-        @repository
-        def my_repository():
-            openlineage_sensor_def = openlineage_sensor(
-                minimum_interval_seconds=60,
-                record_filter_limit=60,
-            )
-            return other_defs + [openlineage_sensor_def]
-        ```
-        
-        
-        OpenLineage sensor handles event logs in ascending order of storage id, and by default, starts with the first log.
-        Optionally, `after_storage_id` can be specified to customize the starting point.
-        This is only applicable when cursor is undefined or has been deleted.
-        
-        ```python
-        @repository
-        def my_repository():
-            openlineage_sensor_def = openlineage_sensor(
-                after_storage_id=100
-            )
-            return other_defs + [openlineage_sensor_def]
-        ```
-        
-        ### OpenLineage Adapter & Client Configuration
-        
-        The sensor uses OpenLineage adapter and client to convert and push data to an OpenLineage backend,
-        and they depend on the following environment variables.
-        
-        If using User Repository Deployments, add the variables to the repository where the sensor is defined.
-        Otherwise, add the variables to Dagster Daemon.
-        
-        * `OPENLINEAGE_URL` - point to service which will consume OpenLineage events
-        * `OPENLINEAGE_API_KEY` - set if consumer of OpenLineage events requires `Bearer` authentication key
-        * `OPENLINEAGE_NAMESPACE` - set if you are using something other than the `default` as the default namespace when Dagster repository is undefined 
-        
-        #### OpenLineage Namespace & Dagster Repository
-        
-        For Dagster jobs organized in repositories, Dagster keeps track of the repository name for each pipeline run.
-        When the repository name is present, it is always used as the OpenLineage namespace name.
-        `OPENLINEAGE_NAMESPACE` option is a way to fall back and provide some other static default value. 
-        
-        
-        ## Development
-        
-        To install all dependencies for local development:
-        
-        ```bash
-        $ python -m pip install -e .[dev]  # or python -m pip install -e .\[dev\] in zsh 
-        ```
-        
-        To run test suite:
-        
-        ```bash
-        $ pytest
-        ```
-Keywords: openlineage
-Platform: UNKNOWN
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: dev
+> **Note** </br>
+> New integration maintainers are needed! Please [open an issue](https://github.com/OpenLineage/OpenLineage/issues/new) to get started.
+
+# OpenLineage Dagster Integration
+
+A library that integrates [Dagster](https://dagster.io/) with [OpenLineage](https://openlineage.io) for automatic metadata collection.
+It provides an OpenLineage sensor, a Dagster sensor that tails Dagster event logs for tracking metadata.
+On each sensor evaluation, the function processes a batch of event logs, converts Dagster events into OpenLineage events, 
+and emits them to an OpenLineage backend.
+
+## Features
+
+**Metadata**
+
+* Dagster job & op lifecycle
+
+## Requirements
+
+- [Python 3.8](https://www.python.org/downloads)
+- [Dagster 0.13.8+](https://dagster.io/)
+
+## Installation
+
+```bash
+$ python -m pip install openlineage-dagster
+```
+
+## Usage
+
+### OpenLineage Sensor & Event Log Storage Requirements
+
+**Single OpenLineage sensor per Dagster instance** <br />
+As the OpenLineage sensor processes all event logs for a given Dagster instance, define and enable only one sensor per instance. 
+Running multiple sensors will result in duplicate OpenLineage job runs being emitted for Dagster steps with different OpenLineage run IDs. These are dynamically generated during sensor runs.
+
+**Non-sharded [Event Log Storage](https://docs.dagster.io/deployment/dagster-instance#event-log-storage)** <br />
+For the sensor to handle all event logs across runs, use non-sharded event log storage.
+If an event log storage sharded by run (i.e., the default `SqliteEventLogStorage`) is used, the cursor that tracks the last processed event storage ID may not update properly. 
+
+### OpenLineage Sensor Setup
+
+Get a OpenLineage sensor definition from the `openlineage_sensor()` factory function and add it to your Dagster repository.
+
+```python
+from dagster import repository
+from openlineage.dagster.sensor import openlineage_sensor
+
+
+@repository
+def my_repository():
+    openlineage_sensor_def = openlineage_sensor()
+    return other_defs + [openlineage_sensor_def]
+```
+
+Given that parallel sensor runs are not supported at the time of writing, some tuning may be necessary to avoid affecting other sensors' performance.
+
+See Dagster's documentation on [Evaluation Interval](https://docs.dagster.io/concepts/partitions-schedules-sensors/sensors#evaluation-interval)
+for more detail on `minimum_interval_seconds`, which defaults to 30 seconds.
+`record_filter_limit` is the maximum number of event logs to process on each sensor evaluation, and it defaults to 30 records per evaluation.
+Default values can be overridden:
+
+```python
+@repository
+def my_repository():
+    openlineage_sensor_def = openlineage_sensor(
+        minimum_interval_seconds=60,
+        record_filter_limit=60,
+    )
+    return other_defs + [openlineage_sensor_def]
+```
+
+
+The OpenLineage sensor handles event logs in ascending order of storage ID and starts with the first log by default.
+Optionally, `after_storage_id` can be specified to customize the starting point.
+This is only applicable when the cursor is undefined or has been deleted.
+
+```python
+@repository
+def my_repository():
+    openlineage_sensor_def = openlineage_sensor(
+        after_storage_id=100
+    )
+    return other_defs + [openlineage_sensor_def]
+```
+
+### OpenLineage Adapter & Client Configuration
+
+The sensor uses an OpenLineage adapter and client to convert and push data to an OpenLineage backend.
+These depend on environment variables.
+
+If using User Repository Deployments, add the below variables to the repository where the sensor is defined.
+Otherwise, add the variables to the Dagster Daemon.
+
+* `OPENLINEAGE_URL` - point to the service which will consume OpenLineage events.
+* `OPENLINEAGE_API_KEY` - set if the consumer of OpenLineage events requires a `Bearer` authentication key.
+* `OPENLINEAGE_NAMESPACE` - set if you are using something other than the `default` as the default namespace when a Dagster repository is undefined. 
+
+#### OpenLineage Namespace & Dagster Repository
+
+For Dagster jobs organized in repositories, Dagster keeps track of the repository name for each pipeline run.
+When the repository name is present, it is always used as the OpenLineage namespace name.
+`OPENLINEAGE_NAMESPACE` option is a way to fall back and provide some other static default value. 
+
+
+## Development
+
+To install all dependencies for local development:
+
+```bash
+$ python -m pip install -e .[dev]  # or python -m pip install -e .\[dev\] in zsh 
+```
+
+To run the test suite:
+
+```bash
+$ pytest
+```
+
+----
+SPDX-License-Identifier: Apache-2.0\
+Copyright 2018-2023 contributors to the OpenLineage project
```

### Comparing `openlineage-dagster-0.9.0/README.md` & `openlineage-dagster-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: openlineage-dagster
+Version: 1.0.0
+Summary: OpenLineage integration with Dagster
+Author: OpenLineage
+Keywords: openlineage
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+Provides-Extra: dev
+
+> **Note** </br>
+> New integration maintainers are needed! Please [open an issue](https://github.com/OpenLineage/OpenLineage/issues/new) to get started.
+
 # OpenLineage Dagster Integration
 
 A library that integrates [Dagster](https://dagster.io/) with [OpenLineage](https://openlineage.io) for automatic metadata collection.
 It provides an OpenLineage sensor, a Dagster sensor that tails Dagster event logs for tracking metadata.
 On each sensor evaluation, the function processes a batch of event logs, converts Dagster events into OpenLineage events, 
 and emits them to an OpenLineage backend.
 
@@ -9,92 +23,92 @@
 
 **Metadata**
 
 * Dagster job & op lifecycle
 
 ## Requirements
 
-- [Python 3.7](https://www.python.org/downloads)
+- [Python 3.8](https://www.python.org/downloads)
 - [Dagster 0.13.8+](https://dagster.io/)
 
 ## Installation
 
 ```bash
 $ python -m pip install openlineage-dagster
 ```
 
 ## Usage
 
 ### OpenLineage Sensor & Event Log Storage Requirements
 
 **Single OpenLineage sensor per Dagster instance** <br />
-As it processes all event logs for a given Dagster instance, define and enable only a single OpenLineage sensor per instance. 
-Running multiple will result in emitting duplicate OpenLineage job runs for Dagster steps with different OpenLineage run ids that are dynamically generated during sensor runs.
+As the OpenLineage sensor processes all event logs for a given Dagster instance, define and enable only one sensor per instance. 
+Running multiple sensors will result in duplicate OpenLineage job runs being emitted for Dagster steps with different OpenLineage run IDs. These are dynamically generated during sensor runs.
 
 **Non-sharded [Event Log Storage](https://docs.dagster.io/deployment/dagster-instance#event-log-storage)** <br />
 For the sensor to handle all event logs across runs, use non-sharded event log storage.
-If an event log storage sharded by run (i.e. default `SqliteEventLogStorage`) is used, cursor that tracks the last processed event storage id may not update properly. 
+If an event log storage sharded by run (i.e., the default `SqliteEventLogStorage`) is used, the cursor that tracks the last processed event storage ID may not update properly. 
 
 ### OpenLineage Sensor Setup
 
-Get OpenLineage sensor definition from `openlineage_sensor()` factory function and add it to your Dagster repository.
+Get a OpenLineage sensor definition from the `openlineage_sensor()` factory function and add it to your Dagster repository.
 
 ```python
 from dagster import repository
 from openlineage.dagster.sensor import openlineage_sensor
 
 
 @repository
 def my_repository():
     openlineage_sensor_def = openlineage_sensor()
     return other_defs + [openlineage_sensor_def]
 ```
 
-With parallel sensor run not supported at the time of writing, some tuning may be necessary to avoid affecting other sensors' performance.
+Given that parallel sensor runs are not supported at the time of writing, some tuning may be necessary to avoid affecting other sensors' performance.
 
 See Dagster's documentation on [Evaluation Interval](https://docs.dagster.io/concepts/partitions-schedules-sensors/sensors#evaluation-interval)
 for more detail on `minimum_interval_seconds`, which defaults to 30 seconds.
 `record_filter_limit` is the maximum number of event logs to process on each sensor evaluation, and it defaults to 30 records per evaluation.
-Default values can be overridden as below.
+Default values can be overridden:
 
 ```python
 @repository
 def my_repository():
     openlineage_sensor_def = openlineage_sensor(
         minimum_interval_seconds=60,
         record_filter_limit=60,
     )
     return other_defs + [openlineage_sensor_def]
 ```
 
 
-OpenLineage sensor handles event logs in ascending order of storage id, and by default, starts with the first log.
+The OpenLineage sensor handles event logs in ascending order of storage ID and starts with the first log by default.
 Optionally, `after_storage_id` can be specified to customize the starting point.
-This is only applicable when cursor is undefined or has been deleted.
+This is only applicable when the cursor is undefined or has been deleted.
 
 ```python
 @repository
 def my_repository():
     openlineage_sensor_def = openlineage_sensor(
         after_storage_id=100
     )
     return other_defs + [openlineage_sensor_def]
 ```
 
 ### OpenLineage Adapter & Client Configuration
 
-The sensor uses OpenLineage adapter and client to convert and push data to an OpenLineage backend,
-and they depend on the following environment variables.
+The sensor uses an OpenLineage adapter and client to convert and push data to an OpenLineage backend.
+These depend on environment variables.
 
-If using User Repository Deployments, add the variables to the repository where the sensor is defined.
-Otherwise, add the variables to Dagster Daemon.
+If using User Repository Deployments, add the below variables to the repository where the sensor is defined.
+Otherwise, add the variables to the Dagster Daemon.
 
-* `OPENLINEAGE_URL` - point to service which will consume OpenLineage events
-* `OPENLINEAGE_API_KEY` - set if consumer of OpenLineage events requires `Bearer` authentication key
-* `OPENLINEAGE_NAMESPACE` - set if you are using something other than the `default` as the default namespace when Dagster repository is undefined 
+* `OPENLINEAGE_URL` - point to the service which will consume OpenLineage events.
+* `OPENLINEAGE_API_KEY` - set if the consumer of OpenLineage events requires a `Bearer` authentication key.
+* `OPENLINEAGE_NAMESPACE` - set if you are using something other than the `default` as the default namespace when a Dagster repository is undefined. 
 
 #### OpenLineage Namespace & Dagster Repository
 
 For Dagster jobs organized in repositories, Dagster keeps track of the repository name for each pipeline run.
 When the repository name is present, it is always used as the OpenLineage namespace name.
 `OPENLINEAGE_NAMESPACE` option is a way to fall back and provide some other static default value. 
 
@@ -103,12 +117,16 @@
 
 To install all dependencies for local development:
 
 ```bash
 $ python -m pip install -e .[dev]  # or python -m pip install -e .\[dev\] in zsh 
 ```
 
-To run test suite:
+To run the test suite:
 
 ```bash
 $ pytest
-```
+```
+
+----
+SPDX-License-Identifier: Apache-2.0\
+Copyright 2018-2023 contributors to the OpenLineage project
```

### Comparing `openlineage-dagster-0.9.0/openlineage/dagster/adapter.py` & `openlineage-dagster-1.0.0/openlineage/dagster/adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,18 @@
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
+
 import logging
 import os
-from typing import Optional
+from typing import Dict, Optional
 
 from openlineage.client import OpenLineageClient, set_producer
 from openlineage.client.constants import DEFAULT_NAMESPACE_NAME
 from openlineage.client.facet import ParentRunFacet
-from openlineage.client.run import RunEvent, RunState, Run, Job
-
+from openlineage.client.run import Job, Run, RunEvent, RunState
 from openlineage.dagster import __version__ as OPENLINEAGE_DAGSTER_VERSION
 from openlineage.dagster.utils import make_step_job_name, to_utc_iso_8601
 
 _DEFAULT_NAMESPACE_NAME = os.getenv("OPENLINEAGE_NAMESPACE", DEFAULT_NAMESPACE_NAME)
 _PRODUCER = f"https://github.com/OpenLineage/OpenLineage/tree/" \
             f"{OPENLINEAGE_DAGSTER_VERSION}/integration/dagster"
 
@@ -32,15 +23,15 @@
 
 class OpenLineageAdapter:
     """Adapter to translate Dagster metadata to OpenLineage events
     and emit them to OpenLineage backend
     """
 
     def __init__(self):
-        self._client = OpenLineageClient.from_environment()
+        self._client = OpenLineageClient()
 
     def start_pipeline(
             self,
             pipeline_name: str,
             pipeline_run_id: str,
             timestamp: float,
             repository_name: Optional[str] = None
@@ -230,21 +221,21 @@
     @staticmethod
     def _build_run(
             namespace: str,
             run_id: str,
             parent_run_id: Optional[str] = None,
             parent_job_name: Optional[str] = None
     ) -> Run:
-        facets = {}
-        if parent_run_id:
+        facets: Dict = {}
+        if parent_run_id is not None and parent_job_name is not None:
             facets.update({
                 "parent": ParentRunFacet.create(parent_run_id, namespace, parent_job_name)
             })
         return Run(run_id, facets)
 
     @staticmethod
     def _build_job(
             namespace: str,
             job_name: str
     ) -> Job:
-        facets = {}
+        facets: Dict = {}
         return Job(namespace, job_name, facets)
```

### Comparing `openlineage-dagster-0.9.0/openlineage/dagster/cursor.py` & `openlineage-dagster-1.0.0/openlineage/dagster/cursor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
+
 import json
-from typing import Optional, Dict, List
+from typing import Dict, List, Optional
 
 import attr
 import cattr
 from openlineage.client.run import InputDataset, OutputDataset
 
 
 @attr.s
```

### Comparing `openlineage-dagster-0.9.0/openlineage/dagster/sensor.py` & `openlineage-dagster-1.0.0/openlineage/dagster/sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,27 @@
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
+
 import logging
-from typing import Optional, Dict
+from typing import Dict, Optional
 
-from dagster import (
+from openlineage.dagster.adapter import OpenLineageAdapter
+from openlineage.dagster.cursor import OpenLineageCursor, RunningPipeline, RunningStep
+from openlineage.dagster.utils import get_event_log_records, get_repository_name, make_step_run_id
+
+from dagster import (  # type: ignore
     DagsterEventType,
-    sensor,
     SensorDefinition,
     SensorEvaluationContext,
-    SkipReason
+    SkipReason,
+    sensor,
 )
 from dagster.core.definitions.sensor_definition import DEFAULT_SENSOR_DAEMON_INTERVAL
 from dagster.core.events import PIPELINE_EVENTS, STEP_EVENTS
 
-from openlineage.dagster.adapter import OpenLineageAdapter
-from openlineage.dagster.cursor import OpenLineageCursor, RunningPipeline, RunningStep
-from openlineage.dagster.utils import make_step_run_id, get_event_log_records, get_repository_name
-
 _ADAPTER = OpenLineageAdapter()
 
 log = logging.getLogger(__name__)
 
 
 def openlineage_sensor(
         name: Optional[str] = "openlineage_sensor",
@@ -44,15 +36,15 @@
     :param name: sensor name
     :param description: sensor description
     :param minimum_interval_seconds: minimum number of seconds that will elapse between evaluations
     :param record_filter_limit: maximum number of event logs to process on each evaluation
     :param after_storage_id: storage id to use as the initial after cursor when getting event logs
     :return: OpenLineage sensor definition
     """
-    @sensor(
+    @sensor(    # type: ignore
         name=name,
         minimum_interval_seconds=minimum_interval_seconds,
         description=description,
     )
     def _openlineage_sensor(context: SensorEvaluationContext):
         # cursor keeps track of the last_storage_id checkpoint and running_pipelines, a map of
         # pipeline run ids to dynamically generated/extracted metadata for running pipelines
@@ -125,16 +117,16 @@
         running_pipelines: Dict[str, RunningPipeline],
         dagster_event_type: DagsterEventType,
         pipeline_name: str,
         pipeline_run_id: str,
         timestamp: float,
         repository_name: Optional[str]
 ):
-    """Handles pipeline events that are of type RUN_START, RUN_SUCCESS, RUN_FAILURE, and RUN_CANCELED.
-    Assumes event type is always in the order of RUN_START
+    """Handles pipeline events that are of type RUN_START, RUN_SUCCESS, RUN_FAILURE,
+    and RUN_CANCELED. Assumes event type is always in the order of RUN_START
     followed by RUN_SUCCESS, RUN_FAILURE, or RUN_CANCELED.
 
     :param running_pipelines: map of pipeline run ids to dynamically generated metadata
                               for pipelines that are in progress between sensor evaluations.
     :param dagster_event_type: Dagster pipeline event type
     :param pipeline_name: Dagster pipeline name
     :param pipeline_run_id: Dagster-generated unique identifier for a pipeline run
```

### Comparing `openlineage-dagster-0.9.0/openlineage/dagster/utils.py` & `openlineage-dagster-1.0.0/openlineage/dagster/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,15 @@
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
+
 import uuid
 from datetime import datetime
 from typing import Iterable, Optional
 
-from dagster import DagsterInstance, EventLogRecord, EventRecordsFilter
+from dagster import DagsterInstance, EventLogRecord, EventRecordsFilter  # type: ignore
 
 NOMINAL_TIME_FORMAT = "%Y-%m-%dT%H:%M:%S.%fZ"
 
 
 def to_utc_iso_8601(timestamp: float) -> str:
     return datetime.utcfromtimestamp(timestamp).strftime(NOMINAL_TIME_FORMAT)
```

### Comparing `openlineage-dagster-0.9.0/openlineage_dagster.egg-info/PKG-INFO` & `openlineage-dagster-1.0.0/openlineage_dagster.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,127 +1,132 @@
 Metadata-Version: 2.1
 Name: openlineage-dagster
-Version: 0.9.0
+Version: 1.0.0
 Summary: OpenLineage integration with Dagster
-Home-page: UNKNOWN
 Author: OpenLineage
-License: UNKNOWN
-Description: # OpenLineage Dagster Integration
-        
-        A library that integrates [Dagster](https://dagster.io/) with [OpenLineage](https://openlineage.io) for automatic metadata collection.
-        It provides an OpenLineage sensor, a Dagster sensor that tails Dagster event logs for tracking metadata.
-        On each sensor evaluation, the function processes a batch of event logs, converts Dagster events into OpenLineage events, 
-        and emits them to an OpenLineage backend.
-        
-        ## Features
-        
-        **Metadata**
-        
-        * Dagster job & op lifecycle
-        
-        ## Requirements
-        
-        - [Python 3.7](https://www.python.org/downloads)
-        - [Dagster 0.13.8+](https://dagster.io/)
-        
-        ## Installation
-        
-        ```bash
-        $ python -m pip install openlineage-dagster
-        ```
-        
-        ## Usage
-        
-        ### OpenLineage Sensor & Event Log Storage Requirements
-        
-        **Single OpenLineage sensor per Dagster instance** <br />
-        As it processes all event logs for a given Dagster instance, define and enable only a single OpenLineage sensor per instance. 
-        Running multiple will result in emitting duplicate OpenLineage job runs for Dagster steps with different OpenLineage run ids that are dynamically generated during sensor runs.
-        
-        **Non-sharded [Event Log Storage](https://docs.dagster.io/deployment/dagster-instance#event-log-storage)** <br />
-        For the sensor to handle all event logs across runs, use non-sharded event log storage.
-        If an event log storage sharded by run (i.e. default `SqliteEventLogStorage`) is used, cursor that tracks the last processed event storage id may not update properly. 
-        
-        ### OpenLineage Sensor Setup
-        
-        Get OpenLineage sensor definition from `openlineage_sensor()` factory function and add it to your Dagster repository.
-        
-        ```python
-        from dagster import repository
-        from openlineage.dagster.sensor import openlineage_sensor
-        
-        
-        @repository
-        def my_repository():
-            openlineage_sensor_def = openlineage_sensor()
-            return other_defs + [openlineage_sensor_def]
-        ```
-        
-        With parallel sensor run not supported at the time of writing, some tuning may be necessary to avoid affecting other sensors' performance.
-        
-        See Dagster's documentation on [Evaluation Interval](https://docs.dagster.io/concepts/partitions-schedules-sensors/sensors#evaluation-interval)
-        for more detail on `minimum_interval_seconds`, which defaults to 30 seconds.
-        `record_filter_limit` is the maximum number of event logs to process on each sensor evaluation, and it defaults to 30 records per evaluation.
-        Default values can be overridden as below.
-        
-        ```python
-        @repository
-        def my_repository():
-            openlineage_sensor_def = openlineage_sensor(
-                minimum_interval_seconds=60,
-                record_filter_limit=60,
-            )
-            return other_defs + [openlineage_sensor_def]
-        ```
-        
-        
-        OpenLineage sensor handles event logs in ascending order of storage id, and by default, starts with the first log.
-        Optionally, `after_storage_id` can be specified to customize the starting point.
-        This is only applicable when cursor is undefined or has been deleted.
-        
-        ```python
-        @repository
-        def my_repository():
-            openlineage_sensor_def = openlineage_sensor(
-                after_storage_id=100
-            )
-            return other_defs + [openlineage_sensor_def]
-        ```
-        
-        ### OpenLineage Adapter & Client Configuration
-        
-        The sensor uses OpenLineage adapter and client to convert and push data to an OpenLineage backend,
-        and they depend on the following environment variables.
-        
-        If using User Repository Deployments, add the variables to the repository where the sensor is defined.
-        Otherwise, add the variables to Dagster Daemon.
-        
-        * `OPENLINEAGE_URL` - point to service which will consume OpenLineage events
-        * `OPENLINEAGE_API_KEY` - set if consumer of OpenLineage events requires `Bearer` authentication key
-        * `OPENLINEAGE_NAMESPACE` - set if you are using something other than the `default` as the default namespace when Dagster repository is undefined 
-        
-        #### OpenLineage Namespace & Dagster Repository
-        
-        For Dagster jobs organized in repositories, Dagster keeps track of the repository name for each pipeline run.
-        When the repository name is present, it is always used as the OpenLineage namespace name.
-        `OPENLINEAGE_NAMESPACE` option is a way to fall back and provide some other static default value. 
-        
-        
-        ## Development
-        
-        To install all dependencies for local development:
-        
-        ```bash
-        $ python -m pip install -e .[dev]  # or python -m pip install -e .\[dev\] in zsh 
-        ```
-        
-        To run test suite:
-        
-        ```bash
-        $ pytest
-        ```
 Keywords: openlineage
-Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: dev
+
+> **Note** </br>
+> New integration maintainers are needed! Please [open an issue](https://github.com/OpenLineage/OpenLineage/issues/new) to get started.
+
+# OpenLineage Dagster Integration
+
+A library that integrates [Dagster](https://dagster.io/) with [OpenLineage](https://openlineage.io) for automatic metadata collection.
+It provides an OpenLineage sensor, a Dagster sensor that tails Dagster event logs for tracking metadata.
+On each sensor evaluation, the function processes a batch of event logs, converts Dagster events into OpenLineage events, 
+and emits them to an OpenLineage backend.
+
+## Features
+
+**Metadata**
+
+* Dagster job & op lifecycle
+
+## Requirements
+
+- [Python 3.8](https://www.python.org/downloads)
+- [Dagster 0.13.8+](https://dagster.io/)
+
+## Installation
+
+```bash
+$ python -m pip install openlineage-dagster
+```
+
+## Usage
+
+### OpenLineage Sensor & Event Log Storage Requirements
+
+**Single OpenLineage sensor per Dagster instance** <br />
+As the OpenLineage sensor processes all event logs for a given Dagster instance, define and enable only one sensor per instance. 
+Running multiple sensors will result in duplicate OpenLineage job runs being emitted for Dagster steps with different OpenLineage run IDs. These are dynamically generated during sensor runs.
+
+**Non-sharded [Event Log Storage](https://docs.dagster.io/deployment/dagster-instance#event-log-storage)** <br />
+For the sensor to handle all event logs across runs, use non-sharded event log storage.
+If an event log storage sharded by run (i.e., the default `SqliteEventLogStorage`) is used, the cursor that tracks the last processed event storage ID may not update properly. 
+
+### OpenLineage Sensor Setup
+
+Get a OpenLineage sensor definition from the `openlineage_sensor()` factory function and add it to your Dagster repository.
+
+```python
+from dagster import repository
+from openlineage.dagster.sensor import openlineage_sensor
+
+
+@repository
+def my_repository():
+    openlineage_sensor_def = openlineage_sensor()
+    return other_defs + [openlineage_sensor_def]
+```
+
+Given that parallel sensor runs are not supported at the time of writing, some tuning may be necessary to avoid affecting other sensors' performance.
+
+See Dagster's documentation on [Evaluation Interval](https://docs.dagster.io/concepts/partitions-schedules-sensors/sensors#evaluation-interval)
+for more detail on `minimum_interval_seconds`, which defaults to 30 seconds.
+`record_filter_limit` is the maximum number of event logs to process on each sensor evaluation, and it defaults to 30 records per evaluation.
+Default values can be overridden:
+
+```python
+@repository
+def my_repository():
+    openlineage_sensor_def = openlineage_sensor(
+        minimum_interval_seconds=60,
+        record_filter_limit=60,
+    )
+    return other_defs + [openlineage_sensor_def]
+```
+
+
+The OpenLineage sensor handles event logs in ascending order of storage ID and starts with the first log by default.
+Optionally, `after_storage_id` can be specified to customize the starting point.
+This is only applicable when the cursor is undefined or has been deleted.
+
+```python
+@repository
+def my_repository():
+    openlineage_sensor_def = openlineage_sensor(
+        after_storage_id=100
+    )
+    return other_defs + [openlineage_sensor_def]
+```
+
+### OpenLineage Adapter & Client Configuration
+
+The sensor uses an OpenLineage adapter and client to convert and push data to an OpenLineage backend.
+These depend on environment variables.
+
+If using User Repository Deployments, add the below variables to the repository where the sensor is defined.
+Otherwise, add the variables to the Dagster Daemon.
+
+* `OPENLINEAGE_URL` - point to the service which will consume OpenLineage events.
+* `OPENLINEAGE_API_KEY` - set if the consumer of OpenLineage events requires a `Bearer` authentication key.
+* `OPENLINEAGE_NAMESPACE` - set if you are using something other than the `default` as the default namespace when a Dagster repository is undefined. 
+
+#### OpenLineage Namespace & Dagster Repository
+
+For Dagster jobs organized in repositories, Dagster keeps track of the repository name for each pipeline run.
+When the repository name is present, it is always used as the OpenLineage namespace name.
+`OPENLINEAGE_NAMESPACE` option is a way to fall back and provide some other static default value. 
+
+
+## Development
+
+To install all dependencies for local development:
+
+```bash
+$ python -m pip install -e .[dev]  # or python -m pip install -e .\[dev\] in zsh 
+```
+
+To run the test suite:
+
+```bash
+$ pytest
+```
+
+----
+SPDX-License-Identifier: Apache-2.0\
+Copyright 2018-2023 contributors to the OpenLineage project
```

### Comparing `openlineage-dagster-0.9.0/setup.cfg` & `openlineage-dagster-1.0.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.9.0
+current_version = 1.0.0
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<rc>.*)
 serialize = 
 	{major}.{minor}.{patch}{rc}
 	{major}.{minor}.{patch}
 
@@ -17,11 +17,15 @@
 
 [flake8]
 max-line-length = 99
 
 [tool:pytest]
 addopts = -p no:warnings
 
+[mypy]
+ignore_missing_imports = True
+implicit_reexport = False
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

