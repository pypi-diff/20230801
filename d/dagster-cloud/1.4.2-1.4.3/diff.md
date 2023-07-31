# Comparing `tmp/dagster_cloud-1.4.2.tar.gz` & `tmp/dagster_cloud-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_cloud-1.4.2.tar", last modified: Fri Jul 21 22:39:09 2023, max compression
+gzip compressed data, was "dagster_cloud-1.4.3.tar", last modified: Mon Jul 31 23:08:42 2023, max compression
```

## Comparing `dagster_cloud-1.4.2.tar` & `dagster_cloud-1.4.3.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.672773 dagster_cloud-1.4.2/
--rw-r--r--   0 root         (0) root         (0)     4537 2023-07-21 22:39:09.672773 dagster_cloud-1.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3062 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.616772 dagster_cloud-1.4.2/dagster_cloud/
--rw-r--r--   0 root         (0) root         (0)      223 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.620772 dagster_cloud-1.4.2/dagster_cloud/agent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.624772 dagster_cloud-1.4.2/dagster_cloud/agent/cli/
--rw-r--r--   0 root         (0) root         (0)     7584 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/agent/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41815 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/agent/dagster_cloud_agent.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/agent/queries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.628772 dagster_cloud-1.4.2/dagster_cloud/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16984 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/api/dagster_cloud_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.628772 dagster_cloud-1.4.2/dagster_cloud/auth/
--rw-r--r--   0 root         (0) root         (0)      248 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1242 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/auth/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.628772 dagster_cloud-1.4.2/dagster_cloud/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.628772 dagster_cloud-1.4.2/dagster_cloud/execution/cloud_run_launcher/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/execution/cloud_run_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/execution/cloud_run_launcher/k8s.py
--rw-r--r--   0 root         (0) root         (0)     3223 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/execution/cloud_run_launcher/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.628772 dagster_cloud-1.4.2/dagster_cloud/execution/monitoring/
--rw-r--r--   0 root         (0) root         (0)    14913 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/execution/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.632772 dagster_cloud-1.4.2/dagster_cloud/execution/utils/
--rw-r--r--   0 root         (0) root         (0)      254 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/execution/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/execution/utils/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.632772 dagster_cloud-1.4.2/dagster_cloud/instance/
--rw-r--r--   0 root         (0) root         (0)    18147 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/instance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.632772 dagster_cloud-1.4.2/dagster_cloud/pex/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/pex/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.636772 dagster_cloud-1.4.2/dagster_cloud/pex/grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.640772 dagster_cloud-1.4.2/dagster_cloud/pex/grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      285 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/pex/grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6822 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7786 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/pex/grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4536 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/pex/grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/pex/grpc/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.644772 dagster_cloud-1.4.2/dagster_cloud/pex/grpc/server/
--rw-r--r--   0 root         (0) root         (0)      119 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/pex/grpc/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.644772 dagster_cloud-1.4.2/dagster_cloud/pex/grpc/server/cli/
--rw-r--r--   0 root         (0) root         (0)     1781 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/pex/grpc/server/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10999 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/pex/grpc/server/manager.py
--rw-r--r--   0 root         (0) root         (0)     9826 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/pex/grpc/server/registry.py
--rw-r--r--   0 root         (0) root         (0)    12925 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/pex/grpc/server/server.py
--rw-r--r--   0 root         (0) root         (0)     2889 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/pex/grpc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.644772 dagster_cloud-1.4.2/dagster_cloud/secrets/
--rw-r--r--   0 root         (0) root         (0)       75 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.648772 dagster_cloud-1.4.2/dagster_cloud/serverless/
--rw-r--r--   0 root         (0) root         (0)       71 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/serverless/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4641 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/serverless/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.648772 dagster_cloud-1.4.2/dagster_cloud/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/storage/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.648772 dagster_cloud-1.4.2/dagster_cloud/storage/compute_logs/
--rw-r--r--   0 root         (0) root         (0)       82 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/storage/compute_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4761 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/storage/compute_logs/compute_log_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.652772 dagster_cloud-1.4.2/dagster_cloud/storage/event_logs/
--rw-r--r--   0 root         (0) root         (0)       70 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/storage/event_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12868 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/storage/event_logs/queries.py
--rw-r--r--   0 root         (0) root         (0)    34523 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/storage/event_logs/storage.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/storage/event_logs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.656772 dagster_cloud-1.4.2/dagster_cloud/storage/runs/
--rw-r--r--   0 root         (0) root         (0)       60 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6504 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/storage/runs/queries.py
--rw-r--r--   0 root         (0) root         (0)    19006 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/storage/runs/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.656772 dagster_cloud-1.4.2/dagster_cloud/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)       70 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1930 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/storage/schedules/queries.py
--rw-r--r--   0 root         (0) root         (0)     7336 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/storage/schedules/storage.py
--rw-r--r--   0 root         (0) root         (0)      280 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/storage/tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.656772 dagster_cloud-1.4.2/dagster_cloud/util/
--rw-r--r--   0 root         (0) root         (0)     2248 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.660772 dagster_cloud-1.4.2/dagster_cloud/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.660772 dagster_cloud-1.4.2/dagster_cloud/workspace/cli/
--rw-r--r--   0 root         (0) root         (0)     6943 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.660772 dagster_cloud-1.4.2/dagster_cloud/workspace/config_schema/
--rw-r--r--   0 root         (0) root         (0)     8613 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/config_schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)      967 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/config_schema/docker.py
--rw-r--r--   0 root         (0) root         (0)     6895 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/config_schema/ecs.py
--rw-r--r--   0 root         (0) root         (0)     6130 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/config_schema/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.664772 dagster_cloud-1.4.2/dagster_cloud/workspace/docker/
--rw-r--r--   0 root         (0) root         (0)    12030 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/docker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.668772 dagster_cloud-1.4.2/dagster_cloud/workspace/ecs/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/ecs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26066 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/ecs/client.py
--rw-r--r--   0 root         (0) root         (0)    23557 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/ecs/launcher.py
--rw-r--r--   0 root         (0) root         (0)      534 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/ecs/run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     4240 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/ecs/service.py
--rw-r--r--   0 root         (0) root         (0)     2766 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/ecs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.668772 dagster_cloud-1.4.2/dagster_cloud/workspace/kubernetes/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17125 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/kubernetes/launcher.py
--rw-r--r--   0 root         (0) root         (0)    11474 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/kubernetes/utils.py
--rw-r--r--   0 root         (0) root         (0)     1268 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.672773 dagster_cloud-1.4.2/dagster_cloud/workspace/user_code_launcher/
--rw-r--r--   0 root         (0) root         (0)      745 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/user_code_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12807 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/user_code_launcher/process.py
--rw-r--r--   0 root         (0) root         (0)    74335 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1209 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/dagster_cloud/workspace/user_code_launcher/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:09.616772 dagster_cloud-1.4.2/dagster_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4537 2023-07-21 22:39:09.000000 dagster_cloud-1.4.2/dagster_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3216 2023-07-21 22:39:09.000000 dagster_cloud-1.4.2/dagster_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 22:39:09.000000 dagster_cloud-1.4.2/dagster_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      409 2023-07-21 22:39:09.000000 dagster_cloud-1.4.2/dagster_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-21 22:39:09.000000 dagster_cloud-1.4.2/dagster_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 22:39:09.672773 dagster_cloud-1.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2890 2023-07-21 22:28:28.000000 dagster_cloud-1.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.370319 dagster_cloud-1.4.3/
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-07-31 23:08:42.370319 dagster_cloud-1.4.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3062 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.310318 dagster_cloud-1.4.3/dagster_cloud/
+-rw-r--r--   0 root         (0) root         (0)      223 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.314318 dagster_cloud-1.4.3/dagster_cloud/agent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.314318 dagster_cloud-1.4.3/dagster_cloud/agent/cli/
+-rw-r--r--   0 root         (0) root         (0)     7584 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/agent/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41818 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/agent/dagster_cloud_agent.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/agent/queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.314318 dagster_cloud-1.4.3/dagster_cloud/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16984 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/api/dagster_cloud_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.318318 dagster_cloud-1.4.3/dagster_cloud/auth/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/auth/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.318318 dagster_cloud-1.4.3/dagster_cloud/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.318318 dagster_cloud-1.4.3/dagster_cloud/execution/cloud_run_launcher/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/execution/cloud_run_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/execution/cloud_run_launcher/k8s.py
+-rw-r--r--   0 root         (0) root         (0)     3223 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/execution/cloud_run_launcher/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.322318 dagster_cloud-1.4.3/dagster_cloud/execution/monitoring/
+-rw-r--r--   0 root         (0) root         (0)    14915 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/execution/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.322318 dagster_cloud-1.4.3/dagster_cloud/execution/utils/
+-rw-r--r--   0 root         (0) root         (0)      254 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/execution/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/execution/utils/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.322318 dagster_cloud-1.4.3/dagster_cloud/instance/
+-rw-r--r--   0 root         (0) root         (0)    19347 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/instance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.322318 dagster_cloud-1.4.3/dagster_cloud/pex/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/pex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.326318 dagster_cloud-1.4.3/dagster_cloud/pex/grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.326318 dagster_cloud-1.4.3/dagster_cloud/pex/grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      285 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/pex/grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7786 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/pex/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4536 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/pex/grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/pex/grpc/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.330318 dagster_cloud-1.4.3/dagster_cloud/pex/grpc/server/
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/pex/grpc/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.330318 dagster_cloud-1.4.3/dagster_cloud/pex/grpc/server/cli/
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/pex/grpc/server/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10999 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/pex/grpc/server/manager.py
+-rw-r--r--   0 root         (0) root         (0)     9826 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/pex/grpc/server/registry.py
+-rw-r--r--   0 root         (0) root         (0)    12925 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/pex/grpc/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     2889 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/pex/grpc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.334318 dagster_cloud-1.4.3/dagster_cloud/secrets/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.334318 dagster_cloud-1.4.3/dagster_cloud/serverless/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/serverless/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4641 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/serverless/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.334318 dagster_cloud-1.4.3/dagster_cloud/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.338318 dagster_cloud-1.4.3/dagster_cloud/storage/compute_logs/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/storage/compute_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4761 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/storage/compute_logs/compute_log_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.346318 dagster_cloud-1.4.3/dagster_cloud/storage/event_logs/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/storage/event_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12868 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/storage/event_logs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    34523 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/storage/event_logs/storage.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/storage/event_logs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.346318 dagster_cloud-1.4.3/dagster_cloud/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/storage/runs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    19006 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/storage/runs/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.350319 dagster_cloud-1.4.3/dagster_cloud/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/storage/schedules/queries.py
+-rw-r--r--   0 root         (0) root         (0)     7336 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/storage/schedules/storage.py
+-rw-r--r--   0 root         (0) root         (0)      280 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/storage/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.350319 dagster_cloud-1.4.3/dagster_cloud/util/
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.350319 dagster_cloud-1.4.3/dagster_cloud/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.358318 dagster_cloud-1.4.3/dagster_cloud/workspace/cli/
+-rw-r--r--   0 root         (0) root         (0)     6943 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.358318 dagster_cloud-1.4.3/dagster_cloud/workspace/config_schema/
+-rw-r--r--   0 root         (0) root         (0)     8613 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/config_schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      967 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/config_schema/docker.py
+-rw-r--r--   0 root         (0) root         (0)     6895 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/config_schema/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     6130 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/config_schema/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.358318 dagster_cloud-1.4.3/dagster_cloud/workspace/docker/
+-rw-r--r--   0 root         (0) root         (0)    12030 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/docker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.362319 dagster_cloud-1.4.3/dagster_cloud/workspace/ecs/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/ecs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26066 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/ecs/client.py
+-rw-r--r--   0 root         (0) root         (0)    23557 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/ecs/launcher.py
+-rw-r--r--   0 root         (0) root         (0)      534 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/ecs/run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     4240 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/ecs/service.py
+-rw-r--r--   0 root         (0) root         (0)     2766 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/ecs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.362319 dagster_cloud-1.4.3/dagster_cloud/workspace/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17587 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/kubernetes/launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11474 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/kubernetes/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.366319 dagster_cloud-1.4.3/dagster_cloud/workspace/user_code_launcher/
+-rw-r--r--   0 root         (0) root         (0)      745 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/user_code_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12807 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/user_code_launcher/process.py
+-rw-r--r--   0 root         (0) root         (0)    74335 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/dagster_cloud/workspace/user_code_launcher/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:42.314318 dagster_cloud-1.4.3/dagster_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-07-31 23:08:42.000000 dagster_cloud-1.4.3/dagster_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-07-31 23:08:42.000000 dagster_cloud-1.4.3/dagster_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 23:08:42.000000 dagster_cloud-1.4.3/dagster_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      409 2023-07-31 23:08:42.000000 dagster_cloud-1.4.3/dagster_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-31 23:08:42.000000 dagster_cloud-1.4.3/dagster_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 23:08:42.370319 dagster_cloud-1.4.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-07-31 22:58:36.000000 dagster_cloud-1.4.3/setup.py
```

### Comparing `dagster_cloud-1.4.2/PKG-INFO` & `dagster_cloud-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster_cloud
-Version: 1.4.2
+Version: 1.4.3
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster_cloud-1.4.2/README.md` & `dagster_cloud-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/agent/cli/__init__.py` & `dagster_cloud-1.4.3/dagster_cloud/agent/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/agent/dagster_cloud_agent.py` & `dagster_cloud-1.4.3/dagster_cloud/agent/dagster_cloud_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -710,24 +710,24 @@
 
                     launcher.launch_run_from_grpc_client(
                         scoped_instance, run, server.server_endpoint.create_client()
                     )
 
                 return DagsterCloudApiSuccess()
         elif api_name == DagsterCloudApi.TERMINATE_RUN:
-            # With agent replicas enabled:
+            # With isolated agents enabled:
             # Run workers now poll for run status. We don't use the run launcher to terminate.
             # Once min agent version is bumped, we can deprecate this command.
             # For backcompat, we use the run launcher to terminate unless the user opts in.
             run = request.request_args.pipeline_run
 
             with DagsterInstance.from_ref(
                 instance.ref_for_deployment(deployment_name)
             ) as scoped_instance:
-                if instance.agent_replicas_enabled:
+                if instance.is_using_isolated_agents:
                     scoped_instance.report_engine_event(
                         f"{instance.agent_display_name} received request to mark run as canceling",
                         run,
                         cls=self.__class__,
                     )
                     scoped_instance.report_run_canceling(run)
                 else:
```

### Comparing `dagster_cloud-1.4.2/dagster_cloud/agent/queries.py` & `dagster_cloud-1.4.3/dagster_cloud/agent/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/api/dagster_cloud_api.py` & `dagster_cloud-1.4.3/dagster_cloud/api/dagster_cloud_api.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/auth/constants.py` & `dagster_cloud-1.4.3/dagster_cloud/auth/constants.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/execution/cloud_run_launcher/process.py` & `dagster_cloud-1.4.3/dagster_cloud/execution/cloud_run_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/execution/monitoring/__init__.py` & `dagster_cloud-1.4.3/dagster_cloud/execution/monitoring/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
                     launcher = scoped_instance.run_launcher
                     statuses_for_deployment.append(
                         CloudRunWorkerStatus.from_check_run_health_result(
                             run.run_id, launcher.check_run_worker_health(run)
                         )
                     )
                 else:
-                    if scoped_instance.agent_replicas_enabled:  # type: ignore  # (instance subclass)
+                    if scoped_instance.is_using_isolated_agents:  # type: ignore  # (instance subclass)
                         # Not currently supported for non isolated run monitoring
                         continue
 
                     if run.status != DagsterRunStatus.STARTED:
                         # Rely on timeout for runs in STARTING
                         continue
```

### Comparing `dagster_cloud-1.4.2/dagster_cloud/execution/utils/process.py` & `dagster_cloud-1.4.3/dagster_cloud/execution/utils/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/instance/__init__.py` & `dagster_cloud-1.4.3/dagster_cloud/instance/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 class DagsterCloudAgentInstance(DagsterCloudInstance):
     def __init__(
         self,
         *args,
         dagster_cloud_api,
         user_code_launcher=None,
         agent_replicas=None,
+        isolated_agents=None,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
         self._unprocessed_dagster_cloud_api_config = dagster_cloud_api
         self._dagster_cloud_api_config = self._get_processed_config(
             "dagster_cloud_api", dagster_cloud_api, dagster_cloud_api_config()
@@ -83,17 +84,30 @@
         self._user_code_launcher = None
         self._graphql_requests_session: Optional[Session] = None
         self._rest_requests_session: Optional[Session] = None
         self._graphql_client = None
 
         assert self.dagster_cloud_url
 
-        self._agent_replicas_config = self._get_processed_config(
-            "agent_replicas", agent_replicas, self._agent_replicas_config_schema()
-        )
+        # Handle backcompat between isolated_agents and agent_replicas
+        if isolated_agents and agent_replicas:
+            raise Exception(
+                "Cannot provide both isolated_agents and agent_replicas configuration. Please only"
+                " provide one of these."
+            )
+        if agent_replicas:
+            self._isolated_agents = self._get_processed_config(
+                "agent_replicas", agent_replicas, self._isolated_agents_config_schema()
+            )
+        elif isolated_agents:
+            self._isolated_agents = self._get_processed_config(
+                "isolated_agents", isolated_agents, self._isolated_agents_config_schema()
+            )
+        else:
+            self._isolated_agents = None
 
         self._instance_uuid = str(uuid.uuid4())
 
     def _get_processed_config(
         self, name: str, config: Optional[Dict[str, Any]], config_type: Dict[str, Any]
     ):
         config_dict = check.opt_dict_param(config, "config", key_type=str)
@@ -380,19 +394,22 @@
         return instance
 
     @classmethod
     def config_schema(cls):
         return {
             "dagster_cloud_api": Field(dagster_cloud_api_config(), is_required=True),
             "user_code_launcher": config_field_for_configurable_class(),
-            "agent_replicas": Field(cls._agent_replicas_config_schema(), is_required=False),
+            "isolated_agents": Field(cls._isolated_agents_config_schema(), is_required=False),
+            "agent_replicas": Field(
+                cls._isolated_agents_config_schema(), is_required=False
+            ),  # deprecated in favor of isolated_agents
         }
 
     @classmethod
-    def _agent_replicas_config_schema(cls):
+    def _isolated_agents_config_schema(cls):
         return {"enabled": Field(bool, is_required=False, default_value=False)}
 
     def get_required_daemon_types(self) -> Sequence[str]:
         return []
 
     @staticmethod
     def config_defaults(base_dir):
@@ -452,19 +469,24 @@
 
     def dispose(self) -> None:
         super().dispose()
         self._exit_stack.close()
 
     @property
     def should_start_background_run_thread(self) -> bool:
-        return self.agent_replicas_enabled
+        # If using isolated agents (that is, agents cannot see each other's grpc
+        # servers), TERMINATE_RUN requests can't be served by the Dagster Cloud API,
+        # which will send requests to any agent. Only the agent with the run can
+        # terminate it - so we need to start a background run thread to monitor for
+        # runs moved into a canceling state.
+        return self.is_using_isolated_agents
 
     @property
-    def agent_replicas_enabled(self) -> bool:
-        return self._agent_replicas_config.get("enabled", False)
+    def is_using_isolated_agents(self) -> bool:
+        return self._isolated_agents is not None and self._isolated_agents.get("enabled", False)
 
     @property
     def dagster_cloud_run_worker_monitoring_interval_seconds(self) -> int:
         return 30
 
 
 @lru_cache(maxsize=100)  # Scales on order of active branch deployments
```

### Comparing `dagster_cloud-1.4.2/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py` & `dagster_cloud-1.4.3/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py` & `dagster_cloud-1.4.3/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/pex/grpc/client.py` & `dagster_cloud-1.4.3/dagster_cloud/pex/grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/pex/grpc/compile.py` & `dagster_cloud-1.4.3/dagster_cloud/pex/grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/pex/grpc/server/cli/__init__.py` & `dagster_cloud-1.4.3/dagster_cloud/pex/grpc/server/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/pex/grpc/server/manager.py` & `dagster_cloud-1.4.3/dagster_cloud/pex/grpc/server/manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/pex/grpc/server/registry.py` & `dagster_cloud-1.4.3/dagster_cloud/pex/grpc/server/registry.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/pex/grpc/server/server.py` & `dagster_cloud-1.4.3/dagster_cloud/pex/grpc/server/server.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/pex/grpc/types.py` & `dagster_cloud-1.4.3/dagster_cloud/pex/grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/secrets/loader.py` & `dagster_cloud-1.4.3/dagster_cloud/secrets/loader.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/serverless/io_manager.py` & `dagster_cloud-1.4.3/dagster_cloud/serverless/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/storage/client.py` & `dagster_cloud-1.4.3/dagster_cloud/storage/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/storage/compute_logs/compute_log_manager.py` & `dagster_cloud-1.4.3/dagster_cloud/storage/compute_logs/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/storage/event_logs/queries.py` & `dagster_cloud-1.4.3/dagster_cloud/storage/event_logs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/storage/event_logs/storage.py` & `dagster_cloud-1.4.3/dagster_cloud/storage/event_logs/storage.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/storage/event_logs/utils.py` & `dagster_cloud-1.4.3/dagster_cloud/storage/event_logs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/storage/runs/queries.py` & `dagster_cloud-1.4.3/dagster_cloud/storage/runs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/storage/runs/storage.py` & `dagster_cloud-1.4.3/dagster_cloud/storage/runs/storage.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/storage/schedules/queries.py` & `dagster_cloud-1.4.3/dagster_cloud/storage/schedules/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/storage/schedules/storage.py` & `dagster_cloud-1.4.3/dagster_cloud/storage/schedules/storage.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/util/__init__.py` & `dagster_cloud-1.4.3/dagster_cloud/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/workspace/cli/__init__.py` & `dagster_cloud-1.4.3/dagster_cloud/workspace/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/workspace/config_schema/__init__.py` & `dagster_cloud-1.4.3/dagster_cloud/workspace/config_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/workspace/config_schema/docker.py` & `dagster_cloud-1.4.3/dagster_cloud/workspace/config_schema/docker.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/workspace/config_schema/ecs.py` & `dagster_cloud-1.4.3/dagster_cloud/workspace/config_schema/ecs.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/workspace/config_schema/kubernetes.py` & `dagster_cloud-1.4.3/dagster_cloud/workspace/config_schema/kubernetes.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/workspace/docker/__init__.py` & `dagster_cloud-1.4.3/dagster_cloud/workspace/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/workspace/ecs/client.py` & `dagster_cloud-1.4.3/dagster_cloud/workspace/ecs/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/workspace/ecs/launcher.py` & `dagster_cloud-1.4.3/dagster_cloud/workspace/ecs/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/workspace/ecs/run_launcher.py` & `dagster_cloud-1.4.3/dagster_cloud/workspace/ecs/run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/workspace/ecs/service.py` & `dagster_cloud-1.4.3/dagster_cloud/workspace/ecs/service.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/workspace/ecs/utils.py` & `dagster_cloud-1.4.3/dagster_cloud/workspace/ecs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/workspace/kubernetes/launcher.py` & `dagster_cloud-1.4.3/dagster_cloud/workspace/kubernetes/launcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 from collections import defaultdict
 from contextlib import contextmanager
+from pathlib import Path
 from typing import Any, Collection, Dict, List, NamedTuple, Optional, Set, Tuple, cast
 
 import kubernetes
 import kubernetes.client as client
 from dagster import (
     Field,
     IntSource,
@@ -339,14 +340,23 @@
             namespace, label_selector=f"user-deployment={k8s_deployment_name}"
         ).items
 
         return get_deployment_failure_debug_info(
             k8s_deployment_name, namespace, core_api, pod_list, self._logger
         )
 
+    def _write_liveness_sentinel(self) -> None:
+        # Write to a sentinel file to indicate that we've finished our initial
+        # reconciliation - this is used to indicate that we're ready to
+        # serve requests
+        Path("/tmp/finished_initial_reconciliation_sentinel.txt").touch(exist_ok=True)
+        self._logger.info(
+            "Wrote liveness sentinel: indicating that agent is ready to serve requests"
+        )
+
     def _wait_for_new_server_ready(
         self,
         deployment_name: str,
         location_name: str,
         metadata: CodeDeploymentMetadata,
         server_handle: K8sHandle,
         server_endpoint: ServerEndpoint,
```

### Comparing `dagster_cloud-1.4.2/dagster_cloud/workspace/kubernetes/utils.py` & `dagster_cloud-1.4.3/dagster_cloud/workspace/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/workspace/origin.py` & `dagster_cloud-1.4.3/dagster_cloud/workspace/origin.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/workspace/user_code_launcher/__init__.py` & `dagster_cloud-1.4.3/dagster_cloud/workspace/user_code_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/workspace/user_code_launcher/process.py` & `dagster_cloud-1.4.3/dagster_cloud/workspace/user_code_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py` & `dagster_cloud-1.4.3/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud/workspace/user_code_launcher/utils.py` & `dagster_cloud-1.4.3/dagster_cloud/workspace/user_code_launcher/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/dagster_cloud.egg-info/PKG-INFO` & `dagster_cloud-1.4.3/dagster_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.4.2
+Version: 1.4.3
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster_cloud-1.4.2/dagster_cloud.egg-info/SOURCES.txt` & `dagster_cloud-1.4.3/dagster_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.2/setup.py` & `dagster_cloud-1.4.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         "Slack": "https://dagster.io/slack",
         "Blog": "https://dagster.io/blog",
         "Newsletter": "https://dagster.io/newsletter-signup",
     },
     packages=find_packages(exclude=["dagster_cloud_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.4.2",
-        "dagster-cloud-cli==1.4.2",
+        "dagster==1.4.3",
+        "dagster-cloud-cli==1.4.3",
         "pex",
         "questionary",
         "requests",
         "typer[all]",
     ],
     extras_require={
         "tests": [
@@ -58,19 +58,19 @@
             "mypy",
             "paramiko",
             "pylint",
             "pytest",
             "types-PyYAML",
             "types-requests",
             "dagster-cloud-test-infra",
-            "dagster_k8s==0.20.2",
+            "dagster_k8s==0.20.3",
         ],
-        "docker": ["docker", "dagster_docker==0.20.2"],
-        "kubernetes": ["kubernetes", "dagster_k8s==0.20.2"],
-        "ecs": ["dagster_aws==0.20.2", "boto3"],
+        "docker": ["docker", "dagster_docker==0.20.3"],
+        "kubernetes": ["kubernetes", "dagster_k8s==0.20.3"],
+        "ecs": ["dagster_aws==0.20.3", "boto3"],
         "sandbox": ["supervisor"],
         "pex": ["boto3"],
         "serverless": ["boto3"],
     },
     author="Elementl",
     license="Apache-2.0",
     classifiers=[
```

