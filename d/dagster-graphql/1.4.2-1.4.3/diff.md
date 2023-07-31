# Comparing `tmp/dagster-graphql-1.4.2.tar.gz` & `tmp/dagster-graphql-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-graphql-1.4.2.tar", last modified: Fri Jul 21 22:28:43 2023, max compression
+gzip compressed data, was "dagster-graphql-1.4.3.tar", last modified: Mon Jul 31 22:58:53 2023, max compression
```

## Comparing `dagster-graphql-1.4.2.tar` & `dagster-graphql-1.4.3.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:43.955676 dagster-graphql-1.4.2/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      604 2023-07-21 22:28:43.955676 dagster-graphql-1.4.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:43.939675 dagster-graphql-1.4.2/dagster_graphql/
--rw-r--r--   0 root         (0) root         (0)      641 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7480 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:43.943675 dagster-graphql-1.4.2/dagster_graphql/client/
--rw-r--r--   0 root         (0) root         (0)      482 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17963 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2715 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/client/client_queries.py
--rw-r--r--   0 root         (0) root         (0)     6886 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/client/query.py
--rw-r--r--   0 root         (0) root         (0)     2917 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:43.947676 dagster-graphql-1.4.2/dagster_graphql/implementation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18592 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:43.947676 dagster-graphql-1.4.2/dagster_graphql/implementation/execution/
--rw-r--r--   0 root         (0) root         (0)    11422 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9850 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     3725 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/execution/dynamic_partitions.py
--rw-r--r--   0 root         (0) root         (0)     4586 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/execution/launch_execution.py
--rw-r--r--   0 root         (0) root         (0)     4396 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/execution/run_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     7270 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/external.py
--rw-r--r--   0 root         (0) root         (0)    25530 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_assets.py
--rw-r--r--   0 root         (0) root         (0)     2369 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)     1237 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_backfills.py
--rw-r--r--   0 root         (0) root         (0)     1120 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_env_vars.py
--rw-r--r--   0 root         (0) root         (0)     4346 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_instigators.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_logs.py
--rw-r--r--   0 root         (0) root         (0)    12589 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_partition_sets.py
--rw-r--r--   0 root         (0) root         (0)     3726 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     2431 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_resources.py
--rw-r--r--   0 root         (0) root         (0)    14972 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_runs.py
--rw-r--r--   0 root         (0) root         (0)     8157 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_schedules.py
--rw-r--r--   0 root         (0) root         (0)     9554 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_sensors.py
--rw-r--r--   0 root         (0) root         (0)     2910 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_solids.py
--rw-r--r--   0 root         (0) root         (0)    21120 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/loader.py
--rw-r--r--   0 root         (0) root         (0)     3093 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)      933 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     8078 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/implementation/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:43.951676 dagster-graphql-1.4.2/dagster_graphql/schema/
--rw-r--r--   0 root         (0) root         (0)     2877 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40455 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)      385 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/asset_key.py
--rw-r--r--   0 root         (0) root         (0)     8466 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)      838 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    16867 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/backfill.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/config_type_or_error.py
--rw-r--r--   0 root         (0) root         (0)    15855 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4785 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/env_vars.py
--rw-r--r--   0 root         (0) root         (0)    18061 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/errors.py
--rw-r--r--   0 root         (0) root         (0)     5489 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/execution.py
--rw-r--r--   0 root         (0) root         (0)    16323 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/external.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    10983 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/inputs.py
--rw-r--r--   0 root         (0) root         (0)     6708 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/instance.py
--rw-r--r--   0 root         (0) root         (0)    28430 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/instigation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:43.951676 dagster-graphql-1.4.2/dagster_graphql/schema/logs/
--rw-r--r--   0 root         (0) root         (0)     3632 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2868 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/logs/compute_logs.py
--rw-r--r--   0 root         (0) root         (0)    20983 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/logs/events.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/logs/log_level.py
--rw-r--r--   0 root         (0) root         (0)     4473 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/metadata.py
--rw-r--r--   0 root         (0) root         (0)      111 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/paging.py
--rw-r--r--   0 root         (0) root         (0)    17622 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/partition_sets.py
--rw-r--r--   0 root         (0) root         (0)      748 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:43.955676 dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/
--rw-r--r--   0 root         (0) root         (0)     3263 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11058 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/config.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/config_result.py
--rw-r--r--   0 root         (0) root         (0)     1369 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/logger.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/mode.py
--rw-r--r--   0 root         (0) root         (0)    39668 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/pipeline.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/pipeline_ref.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/pipeline_run_stats.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/resource.py
--rw-r--r--   0 root         (0) root         (0)     1261 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     1621 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/status.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1658 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/repository_origin.py
--rw-r--r--   0 root         (0) root         (0)     8315 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:43.955676 dagster-graphql-1.4.2/dagster_graphql/schema/roots/
--rw-r--r--   0 root         (0) root         (0)     2094 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/roots/__init__.py
--rw-r--r--   0 root         (0) root         (0)      620 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/roots/assets.py
--rw-r--r--   0 root         (0) root         (0)      564 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/roots/execution_plan.py
--rw-r--r--   0 root         (0) root         (0)    26779 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/roots/mutation.py
--rw-r--r--   0 root         (0) root         (0)      723 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/roots/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    37803 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/roots/query.py
--rw-r--r--   0 root         (0) root         (0)     2905 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/roots/subscription.py
--rw-r--r--   0 root         (0) root         (0)     5050 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/run_config.py
--rw-r--r--   0 root         (0) root         (0)     5940 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/runs.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/schedule_dry_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:43.955676 dagster-graphql-1.4.2/dagster_graphql/schema/schedules/
--rw-r--r--   0 root         (0) root         (0)     3904 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8306 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/schedules/schedules.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/schedules/ticks.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/sensor_dry_run.py
--rw-r--r--   0 root         (0) root         (0)     7983 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/sensors.py
--rw-r--r--   0 root         (0) root         (0)    29569 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/solids.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/table.py
--rw-r--r--   0 root         (0) root         (0)     1411 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/tags.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/test.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/used_solid.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/schema/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:43.955676 dagster-graphql-1.4.2/dagster_graphql/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6751 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/test/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/dagster_graphql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:43.943675 dagster-graphql-1.4.2/dagster_graphql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      604 2023-07-21 22:28:43.000000 dagster-graphql-1.4.2/dagster_graphql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4286 2023-07-21 22:28:43.000000 dagster-graphql-1.4.2/dagster_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 22:28:43.000000 dagster-graphql-1.4.2/dagster_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-07-21 22:28:43.000000 dagster-graphql-1.4.2/dagster_graphql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2023-07-21 22:28:43.000000 dagster-graphql-1.4.2/dagster_graphql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-21 22:28:43.000000 dagster-graphql-1.4.2/dagster_graphql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      180 2023-07-21 22:28:43.955676 dagster-graphql-1.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1509 2023-07-21 22:28:09.000000 dagster-graphql-1.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.977937 dagster-graphql-1.4.3/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      604 2023-07-31 22:58:53.977937 dagster-graphql-1.4.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.957937 dagster-graphql-1.4.3/dagster_graphql/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.957937 dagster-graphql-1.4.3/dagster_graphql/client/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17966 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/client/client_queries.py
+-rw-r--r--   0 root         (0) root         (0)     6886 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/client/query.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.961937 dagster-graphql-1.4.3/dagster_graphql/implementation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18592 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.965937 dagster-graphql-1.4.3/dagster_graphql/implementation/execution/
+-rw-r--r--   0 root         (0) root         (0)    11422 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9850 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     3725 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/execution/dynamic_partitions.py
+-rw-r--r--   0 root         (0) root         (0)     4591 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/execution/launch_execution.py
+-rw-r--r--   0 root         (0) root         (0)     4396 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/execution/run_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     7244 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/external.py
+-rw-r--r--   0 root         (0) root         (0)    25530 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_assets.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_backfills.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_env_vars.py
+-rw-r--r--   0 root         (0) root         (0)     4346 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_instigators.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_logs.py
+-rw-r--r--   0 root         (0) root         (0)    12589 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     2436 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_resources.py
+-rw-r--r--   0 root         (0) root         (0)    14972 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_runs.py
+-rw-r--r--   0 root         (0) root         (0)     8157 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_schedules.py
+-rw-r--r--   0 root         (0) root         (0)     9554 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_sensors.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_solids.py
+-rw-r--r--   0 root         (0) root         (0)    21120 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/loader.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)      933 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     8042 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.969937 dagster-graphql-1.4.3/dagster_graphql/schema/
+-rw-r--r--   0 root         (0) root         (0)     2877 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40455 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)      385 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)     8754 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)      838 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16867 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/backfill.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/config_type_or_error.py
+-rw-r--r--   0 root         (0) root         (0)    15855 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     4823 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/env_vars.py
+-rw-r--r--   0 root         (0) root         (0)    18061 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5489 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/execution.py
+-rw-r--r--   0 root         (0) root         (0)    16361 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/external.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    10983 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     6708 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/instance.py
+-rw-r--r--   0 root         (0) root         (0)    28430 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/instigation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.973937 dagster-graphql-1.4.3/dagster_graphql/schema/logs/
+-rw-r--r--   0 root         (0) root         (0)     3632 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/logs/compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)    20983 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/logs/events.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/logs/log_level.py
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/metadata.py
+-rw-r--r--   0 root         (0) root         (0)      111 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/paging.py
+-rw-r--r--   0 root         (0) root         (0)    17622 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)      748 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.973937 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     3263 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11058 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/config.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/config_result.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/mode.py
+-rw-r--r--   0 root         (0) root         (0)    40083 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/pipeline_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/pipeline_run_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/status.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/repository_origin.py
+-rw-r--r--   0 root         (0) root         (0)     8353 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.977937 dagster-graphql-1.4.3/dagster_graphql/schema/roots/
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/roots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      620 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/roots/assets.py
+-rw-r--r--   0 root         (0) root         (0)      564 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/roots/execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)    26779 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/roots/mutation.py
+-rw-r--r--   0 root         (0) root         (0)      723 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/roots/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    37803 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/roots/query.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/roots/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     5088 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     5940 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/runs.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/schedule_dry_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.977937 dagster-graphql-1.4.3/dagster_graphql/schema/schedules/
+-rw-r--r--   0 root         (0) root         (0)     3904 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8306 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/schedules/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/schedules/ticks.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/sensor_dry_run.py
+-rw-r--r--   0 root         (0) root         (0)     7983 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    29569 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/solids.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/table.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/tags.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/test.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/used_solid.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.977937 dagster-graphql-1.4.3/dagster_graphql/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6751 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/test/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.957937 dagster-graphql-1.4.3/dagster_graphql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-07-31 22:58:53.000000 dagster-graphql-1.4.3/dagster_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4286 2023-07-31 22:58:53.000000 dagster-graphql-1.4.3/dagster_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 22:58:53.000000 dagster-graphql-1.4.3/dagster_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-31 22:58:53.000000 dagster-graphql-1.4.3/dagster_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-07-31 22:58:53.000000 dagster-graphql-1.4.3/dagster_graphql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-31 22:58:53.000000 dagster-graphql-1.4.3/dagster_graphql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2023-07-31 22:58:53.993937 dagster-graphql-1.4.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/setup.py
```

### Comparing `dagster-graphql-1.4.2/LICENSE` & `dagster-graphql-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/PKG-INFO` & `dagster-graphql-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.4.2
+Version: 1.4.3
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-graphql-1.4.2/dagster_graphql/__init__.py` & `dagster-graphql-1.4.3/dagster_graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/cli.py` & `dagster-graphql-1.4.3/dagster_graphql/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/client/client.py` & `dagster-graphql-1.4.3/dagster_graphql/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     .. code-block:: python
 
         client = DagsterGraphQLClient("localhost", port_number=3000)
         status = client.get_run_status(**SOME_RUN_ID**)
 
     Args:
         hostname (str): Hostname for the Dagster GraphQL API, like `localhost` or
-            `dagit.dagster.YOUR_ORG_HERE`.
+            `dagster.YOUR_ORG_HERE`.
         port_number (Optional[int], optional): Optional port number to connect to on the host.
             Defaults to None.
         transport (Optional[Transport], optional): A custom transport to use to connect to the
             GraphQL API with (e.g. for custom auth). Defaults to None.
         use_https (bool, optional): Whether to use https in the URL connection string for the
             GraphQL API. Defaults to False.
 
@@ -294,15 +294,15 @@
 
     @public
     def reload_repository_location(
         self, repository_location_name: str
     ) -> ReloadRepositoryLocationInfo:
         """Reloads a Dagster Repository Location, which reloads all repositories in that repository location.
 
-        This is useful in a variety of contexts, including refreshing Dagit without restarting
+        This is useful in a variety of contexts, including refreshing the Dagster UI without restarting
         the server.
 
         Args:
             repository_location_name (str): The name of the repository location
 
         Returns:
             ReloadRepositoryLocationInfo: Object with information about the result of the reload request
```

### Comparing `dagster-graphql-1.4.2/dagster_graphql/client/client_queries.py` & `dagster-graphql-1.4.3/dagster_graphql/client/client_queries.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/client/query.py` & `dagster-graphql-1.4.3/dagster_graphql/client/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/client/utils.py` & `dagster-graphql-1.4.3/dagster_graphql/client/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/events.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/execution/__init__.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/execution/backfill.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/execution/dynamic_partitions.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/execution/dynamic_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/execution/launch_execution.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/execution/launch_execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from typing import TYPE_CHECKING, cast
 
 import dagster._check as check
 from dagster._core.definitions.selector import JobSubsetSelector
 from dagster._core.execution.plan.resume_retry import ReexecutionStrategy
-from dagster._core.instance import DagsterInstance
 from dagster._core.storage.dagster_run import DagsterRun, RunsFilter
 from dagster._core.workspace.permissions import Permissions
 
 from ..external import get_external_job_or_raise
 from ..utils import (
     ExecutionMetadata,
     ExecutionParams,
     assert_permission_for_location,
 )
 from .run_lifecycle import create_valid_pipeline_run
 
 if TYPE_CHECKING:
+    from dagster._core.instance import DagsterInstance
+
     from dagster_graphql.schema.runs import GrapheneLaunchRunSuccess
     from dagster_graphql.schema.util import ResolveInfo
 
 
 def launch_pipeline_reexecution(
     graphene_info: "ResolveInfo", execution_params: ExecutionParams
 ) -> "GrapheneLaunchRunSuccess":
```

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/execution/run_lifecycle.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/execution/run_lifecycle.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/external.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/external.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 import sys
 from typing import TYPE_CHECKING, Mapping, Optional, Sequence, Union
 
 import dagster._check as check
 from dagster._config import validate_config_from_snap
 from dagster._core.definitions.selector import JobSubsetSelector, RepositorySelector
 from dagster._core.execution.plan.state import KnownExecutionState
@@ -103,15 +101,15 @@
         external_job=external_pipeline,
         run_config=run_config,
         step_keys_to_execute=step_keys_to_execute,
         known_state=known_state,
     )
 
 
-def fetch_repositories(graphene_info: "ResolveInfo") -> GrapheneRepositoryConnection:
+def fetch_repositories(graphene_info: "ResolveInfo") -> "GrapheneRepositoryConnection":
     from ..schema.external import GrapheneRepository, GrapheneRepositoryConnection
 
     return GrapheneRepositoryConnection(
         nodes=[
             GrapheneRepository(
                 instance=graphene_info.context.instance,
                 repository=repository,
@@ -121,15 +119,15 @@
             for repository in location.get_repositories().values()
         ]
     )
 
 
 def fetch_repository(
     graphene_info: "ResolveInfo", repository_selector: RepositorySelector
-) -> Union[GrapheneRepository, GrapheneRepositoryNotFoundError]:
+) -> Union["GrapheneRepository", "GrapheneRepositoryNotFoundError"]:
     from ..schema.errors import GrapheneRepositoryNotFoundError
     from ..schema.external import GrapheneRepository
 
     check.inst_param(repository_selector, "repository_selector", RepositorySelector)
 
     if graphene_info.context.has_code_location(repository_selector.location_name):
         repo_loc = graphene_info.context.get_code_location(repository_selector.location_name)
@@ -141,15 +139,15 @@
             )
 
     return GrapheneRepositoryNotFoundError(
         repository_selector.location_name, repository_selector.repository_name
     )
 
 
-def fetch_workspace(workspace_request_context: WorkspaceRequestContext) -> GrapheneWorkspace:
+def fetch_workspace(workspace_request_context: WorkspaceRequestContext) -> "GrapheneWorkspace":
     from ..schema.external import GrapheneWorkspace, GrapheneWorkspaceLocationEntry
 
     check.inst_param(
         workspace_request_context, "workspace_request_context", BaseWorkspaceRequestContext
     )
 
     nodes = [
@@ -158,15 +156,15 @@
     ]
 
     return GrapheneWorkspace(locationEntries=nodes)
 
 
 def fetch_location_statuses(
     workspace_request_context: WorkspaceRequestContext,
-) -> GrapheneWorkspaceLocationStatusEntries:
+) -> "GrapheneWorkspaceLocationStatusEntries":
     from ..schema.external import (
         GrapheneRepositoryLocationLoadStatus,
         GrapheneWorkspaceLocationStatusEntries,
         GrapheneWorkspaceLocationStatusEntry,
     )
 
     check.inst_param(
```

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_assets.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_backfills.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_backfills.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_env_vars.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_env_vars.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+from typing import TYPE_CHECKING
+
 import dagster._check as check
 from dagster._core.definitions.selector import RepositorySelector
-from dagster._core.host_representation.code_location import CodeLocation
 from graphene import ResolveInfo
 
 from dagster_graphql.schema.env_vars import (
     GrapheneEnvVarWithConsumers,
     GrapheneEnvVarWithConsumersList,
     GrapheneEnvVarWithConsumersListOrError,
 )
 
+if TYPE_CHECKING:
+    from dagster._core.host_representation.code_location import CodeLocation
+
 
 def get_utilized_env_vars_or_error(
     graphene_info, repository_selector
 ) -> GrapheneEnvVarWithConsumersListOrError:
     check.inst_param(graphene_info, "graphene_info", ResolveInfo)
     check.inst_param(repository_selector, "repository_selector", RepositorySelector)
```

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_instigators.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_instigators.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_logs.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_partition_sets.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_pipelines.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_pipelines.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_resources.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from typing import TYPE_CHECKING
 
 import dagster._check as check
 from dagster._core.definitions.selector import RepositorySelector, ResourceSelector
-from dagster._core.host_representation.code_location import CodeLocation
 from graphene import ResolveInfo
 
 from .utils import UserFacingGraphQLError
 
 if TYPE_CHECKING:
+    from dagster._core.host_representation.code_location import CodeLocation
+
     from ..schema.resources import GrapheneResourceDetails, GrapheneResourceDetailsList
 
 
 def get_top_level_resources_or_error(
     graphene_info: "ResolveInfo", repository_selector: RepositorySelector
 ) -> "GrapheneResourceDetailsList":
     from ..schema.resources import GrapheneResourceDetails, GrapheneResourceDetailsList
```

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_runs.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_schedules.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_sensors.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/fetch_solids.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/loader.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/loader.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/run_config_schema.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/telemetry.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/implementation/utils.py` & `dagster-graphql-1.4.3/dagster_graphql/implementation/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 import sys
 from contextlib import contextmanager
 from contextvars import ContextVar
 from types import TracebackType
 from typing import (
     TYPE_CHECKING,
     Any,
```

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/__init__.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/asset_graph.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/auto_materialize_asset_evaluations.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/auto_materialize_asset_evaluations.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,17 @@
 class GrapheneDownstreamFreshnessAutoMaterializeCondition(graphene.ObjectType):
     class Meta:
         name = "DownstreamFreshnessAutoMaterializeCondition"
         interfaces = (GrapheneAutoMaterializeConditionWithDecisionType,)
 
 
 class GrapheneParentMaterializedAutoMaterializeCondition(graphene.ObjectType):
+    updatedAssetKeys = graphene.List(graphene.NonNull(GrapheneAssetKey))
+    willUpdateAssetKeys = graphene.List(graphene.NonNull(GrapheneAssetKey))
+
     class Meta:
         name = "ParentMaterializedAutoMaterializeCondition"
         interfaces = (GrapheneAutoMaterializeConditionWithDecisionType,)
 
 
 class GrapheneMissingAutoMaterializeCondition(graphene.ObjectType):
     class Meta:
@@ -133,15 +136,18 @@
         )
     elif isinstance(condition, DownstreamFreshnessAutoMaterializeCondition):
         return GrapheneDownstreamFreshnessAutoMaterializeCondition(
             decisionType=condition.decision_type, partitionKeysOrError=partition_keys_or_error
         )
     elif isinstance(condition, ParentMaterializedAutoMaterializeCondition):
         return GrapheneParentMaterializedAutoMaterializeCondition(
-            decisionType=condition.decision_type, partitionKeysOrError=partition_keys_or_error
+            decisionType=condition.decision_type,
+            partitionKeysOrError=partition_keys_or_error,
+            updatedAssetKeys=condition.updated_asset_keys,
+            willUpdateAssetKeys=condition.will_update_asset_keys,
         )
     elif isinstance(condition, MissingAutoMaterializeCondition):
         return GrapheneMissingAutoMaterializeCondition(
             decisionType=condition.decision_type, partitionKeysOrError=partition_keys_or_error
         )
     elif isinstance(condition, ParentOutdatedAutoMaterializeCondition):
         return GrapheneParentOutdatedAutoMaterializeCondition(
```

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/auto_materialize_policy.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/backfill.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/config_type_or_error.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/config_type_or_error.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/config_types.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/config_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/dagster_types.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/dagster_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-from typing import Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import dagster._check as check
 import graphene
 from dagster._core.snap import JobSnapshot
-from dagster._core.snap.dagster_types import DagsterTypeSnap
 from dagster._core.types.dagster_type import DagsterTypeKind
 from typing_extensions import TypeAlias
 
 from dagster_graphql.implementation.events import iterate_metadata_entries
 from dagster_graphql.schema.metadata import GrapheneMetadataEntry
 
 from .config_types import GrapheneConfigType, GrapheneConfigTypeUnion, to_config_type
 from .errors import (
     GrapheneDagsterTypeNotFoundError,
     GraphenePipelineNotFoundError,
     GraphenePythonError,
 )
 from .util import non_null_list
 
+if TYPE_CHECKING:
+    from dagster._core.snap.dagster_types import DagsterTypeSnap
+
 GrapheneDagsterTypeUnion: TypeAlias = Union[
     "GrapheneListDagsterType", "GrapheneNullableDagsterType", "GrapheneRegularDagsterType"
 ]
 
 
 def config_type_for_schema(
     pipeline_snapshot: JobSnapshot, schema_key: Optional[str]
```

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/env_vars.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/errors.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/execution.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/external.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/external.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import asyncio
-from typing import Dict, List
+from typing import TYPE_CHECKING, Dict, List
 
 import graphene
 from dagster import (
     DagsterInstance,
     _check as check,
 )
 from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
 from dagster._core.definitions.partition import CachingDynamicPartitionsLoader
 from dagster._core.host_representation import (
     CodeLocation,
     ExternalRepository,
     GrpcServerCodeLocation,
     ManagedGrpcPythonEnvCodeLocationOrigin,
 )
-from dagster._core.host_representation.external_data import ExternalAssetNode
 from dagster._core.host_representation.grpc_server_state_subscriber import (
     LocationStateChangeEvent,
     LocationStateChangeEventType,
     LocationStateSubscriber,
 )
 from dagster._core.workspace.context import (
     WorkspaceProcessContext,
@@ -42,14 +41,17 @@
 from .repository_origin import GrapheneRepositoryMetadata, GrapheneRepositoryOrigin
 from .resources import GrapheneResourceDetails
 from .schedules import GrapheneSchedule
 from .sensors import GrapheneSensor
 from .used_solid import GrapheneUsedSolid
 from .util import ResolveInfo, non_null_list
 
+if TYPE_CHECKING:
+    from dagster._core.host_representation.external_data import ExternalAssetNode
+
 GrapheneLocationStateChangeEventType = graphene.Enum.from_enum(LocationStateChangeEventType)
 
 
 class GrapheneDagsterLibraryVersion(graphene.ObjectType):
     name = graphene.NonNull(graphene.String)
     version = graphene.NonNull(graphene.String)
```

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/freshness_policy.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/inputs.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/instance.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/instigation.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/logs/__init__.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/logs/compute_logs.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/logs/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/logs/events.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/logs/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/logs/log_level.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/logs/log_level.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/metadata.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/metadata.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/partition_sets.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/permissions.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/__init__.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/config.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/config_result.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/config_result.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/logger.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/mode.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/pipeline.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -372,14 +372,15 @@
     )
     startTime = graphene.Float()
     endTime = graphene.Float()
     updateTime = graphene.Float()
     hasReExecutePermission = graphene.NonNull(graphene.Boolean)
     hasTerminatePermission = graphene.NonNull(graphene.Boolean)
     hasDeletePermission = graphene.NonNull(graphene.Boolean)
+    hasConcurrencyKeySlots = graphene.NonNull(graphene.Boolean)
 
     class Meta:
         interfaces = (GraphenePipelineRun,)
         name = "Run"
 
     def __init__(self, record: RunRecord):
         check.inst_param(record, "record", RunRecord)
@@ -579,14 +580,22 @@
             return self._run_stats.end_time
         return run_record.end_time
 
     def resolve_updateTime(self, graphene_info: ResolveInfo):
         run_record = self._get_run_record(graphene_info.context.instance)
         return datetime_as_float(run_record.update_timestamp)
 
+    def resolve_hasConcurrencyKeySlots(self, graphene_info: ResolveInfo):
+        instance = graphene_info.context.instance
+        if not instance.event_log_storage.supports_global_concurrency_limits:
+            return False
+
+        active_run_ids = instance.event_log_storage.get_concurrency_run_ids()
+        return self.runId in active_run_ids
+
 
 class GrapheneIPipelineSnapshotMixin:
     # Mixin this class to implement IPipelineSnapshot
     #
     # Graphene has some strange properties that make it so that you cannot
     # implement ABCs nor use properties in an overridable way. So the way
     # the mixin works is that the target classes have to have a method
```

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/pipeline_ref.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/pipeline_ref.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/pipeline_run_stats.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/pipeline_run_stats.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/resource.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/snapshot.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/status.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/status.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/pipelines/subscription.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/repository_origin.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/repository_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/resources.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-from typing import List
+from typing import TYPE_CHECKING, List
 
 import dagster._check as check
 import graphene
 from dagster._core.definitions.selector import ResourceSelector
 from dagster._core.host_representation.external import ExternalRepository, ExternalResource
 from dagster._core.host_representation.external_data import (
     ExternalResourceConfigEnvVar,
     ExternalResourceValue,
     NestedResourceType,
     ResourceJobUsageEntry,
 )
-from dagster._core.workspace.workspace import IWorkspace
 
 from dagster_graphql.schema.asset_key import GrapheneAssetKey
 from dagster_graphql.schema.errors import (
     GraphenePythonError,
     GrapheneRepositoryNotFoundError,
     GrapheneResourceNotFoundError,
 )
 from dagster_graphql.schema.pipelines.pipeline import GrapheneJob
 from dagster_graphql.schema.solids import GrapheneSolidHandle, build_solid_handles
 from dagster_graphql.schema.util import non_null_list
 
 from .config_types import GrapheneConfigTypeField
 
+if TYPE_CHECKING:
+    from dagster._core.workspace.workspace import IWorkspace
+
 
 class GrapheneConfiguredValueType(graphene.Enum):
     VALUE = "VALUE"
     ENV_VAR = "ENV_VAR"
 
     class Meta:
         name = "ConfiguredValueType"
```

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/roots/__init__.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/roots/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/roots/assets.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/roots/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/roots/execution_plan.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/roots/execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/roots/mutation.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/roots/mutation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/roots/pipeline.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/roots/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/roots/query.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/roots/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/roots/subscription.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/roots/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/run_config.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/run_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from typing import Any, Optional
+from typing import TYPE_CHECKING, Any, Optional
 
 import dagster._check as check
 import graphene
-from dagster._config.snap import ConfigSchemaSnapshot
 from dagster._core.host_representation import RepresentedJob
 from dagster._core.host_representation.external_data import DEFAULT_MODE_NAME
 from dagster._core.snap.snap_to_yaml import default_values_yaml_from_type_snap
 
 from ..implementation.run_config_schema import resolve_is_run_config_valid
 from ..implementation.utils import capture_error
 from .config_types import GrapheneConfigType, to_config_type
@@ -16,14 +15,17 @@
     GraphenePipelineNotFoundError,
     GraphenePythonError,
 )
 from .pipelines.config_result import GraphenePipelineConfigValidationResult
 from .runs import GrapheneRunConfigData, parse_run_config_input
 from .util import ResolveInfo, non_null_list
 
+if TYPE_CHECKING:
+    from dagster._config.snap import ConfigSchemaSnapshot
+
 
 class GrapheneRunConfigSchema(graphene.ObjectType):
     rootConfigType = graphene.Field(
         graphene.NonNull(GrapheneConfigType),
         description="""Fetch the root environment type. Concretely this is the type that
         is in scope at the root of configuration document for a particular execution selection.
         It is the type that is in scope initially with a blank config editor.""",
```

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/runs.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/schedule_dry_run.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/schedule_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/schedules/__init__.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/schedules/schedules.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/schedules/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/schedules/ticks.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/schedules/ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/sensor_dry_run.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/sensor_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/sensors.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/solids.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/table.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/table.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/tags.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/used_solid.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/used_solid.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/schema/util.py` & `dagster-graphql-1.4.3/dagster_graphql/schema/util.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql/test/utils.py` & `dagster-graphql-1.4.3/dagster_graphql/test/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/dagster_graphql.egg-info/PKG-INFO` & `dagster-graphql-1.4.3/dagster_graphql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.4.2
+Version: 1.4.3
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-graphql-1.4.2/dagster_graphql.egg-info/SOURCES.txt` & `dagster-graphql-1.4.3/dagster_graphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.2/setup.py` & `dagster-graphql-1.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_graphql_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.4.2",
+        "dagster==1.4.3",
         "graphene>=3",
         "gql[requests]>=3.0.0",
         "requests",
         "starlette",  # used for run_in_threadpool utility fn
         "urllib3<2.0.0",  # https://github.com/psf/requests/issues/6432
     ],
     entry_points={"console_scripts": ["dagster-graphql = dagster_graphql.cli:main"]},
```

