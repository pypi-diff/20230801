# Comparing `tmp/meili-sdk-0.6.0.tar.gz` & `tmp/meili-sdk-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meili-sdk-0.6.0.tar", last modified: Mon Jul 24 14:07:02 2023, max compression
+gzip compressed data, was "meili-sdk-0.6.1.tar", last modified: Tue Aug  1 13:01:36 2023, max compression
```

## Comparing `meili-sdk-0.6.0.tar` & `meili-sdk-0.6.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.967427 meili-sdk-0.6.0/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     5035 2023-07-24 14:07:02.967427 meili-sdk-0.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4735 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.957427 meili-sdk-0.6.0/meili_sdk/
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.958427 meili-sdk-0.6.0/meili_sdk/clients/
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/clients/apitoken_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/clients/base.py
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/clients/persistent_token_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1002 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/clients/sdk_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.959427 meili-sdk-0.6.0/meili_sdk/config/
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/config/type.py
--rw-rw-rw-   0 root         (0) root         (0)      506 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/config/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2191 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.960427 meili-sdk-0.6.0/meili_sdk/models/
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4047 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1742 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/models/form.py
--rw-rw-rw-   0 root         (0) root         (0)      220 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/models/organization.py
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/models/ros_setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/models/task.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/models/team.py
--rw-rw-rw-   0 root         (0) root         (0)      941 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/models/trigger.py
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/models/user.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/models/vehicle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.961427 meili-sdk-0.6.0/meili_sdk/mqtt/
--rw-rw-rw-   0 root         (0) root         (0)      407 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/mqtt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1807 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/mqtt/action_client.py
--rw-rw-rw-   0 root         (0) root         (0)     8530 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/mqtt/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.962427 meili-sdk-0.6.0/meili_sdk/mqtt/models/
--rw-rw-rw-   0 root         (0) root         (0)      250 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/mqtt/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1244 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/mqtt/models/action.py
--rw-rw-rw-   0 root         (0) root         (0)     3379 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/mqtt/models/order.py
--rw-rw-rw-   0 root         (0) root         (0)     3793 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/mqtt/models/state.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/mqtt/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.963427 meili-sdk-0.6.0/meili_sdk/resources/
--rw-rw-rw-   0 root         (0) root         (0)      334 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5110 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1365 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/forms.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/maps.py
--rw-rw-rw-   0 root         (0) root         (0)      744 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/organizations.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/ros.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/teams.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/triggers.py
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/users.py
--rw-rw-rw-   0 root         (0) root         (0)      768 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/vehicles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.964427 meili-sdk-0.6.0/meili_sdk/schedules/
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/schedules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/schedules/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/schedules/loader.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/schedules/models.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/site.py
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/token.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.965427 meili-sdk-0.6.0/meili_sdk/websockets/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15825 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/client.py
--rw-rw-rw-   0 root         (0) root         (0)     1488 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.967427 meili-sdk-0.6.0/meili_sdk/websockets/models/
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/models/cancel_task_message.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/models/docking_routine_message.py
--rw-rw-rw-   0 root         (0) root         (0)     6253 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)      356 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/models/move_message.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/models/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1179 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/models/task_v2.py
--rw-rw-rw-   0 root         (0) root         (0)      204 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/models/topic.py
--rw-rw-rw-   0 root         (0) root         (0)      962 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/models/traffic_control_action_message.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/models/update_map_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.957427 meili-sdk-0.6.0/meili_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5035 2023-07-24 14:07:02.000000 meili-sdk-0.6.0/meili_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2075 2023-07-24 14:07:02.000000 meili-sdk-0.6.0/meili_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 14:07:02.000000 meili-sdk-0.6.0/meili_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       78 2023-07-24 14:07:02.000000 meili-sdk-0.6.0/meili_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-24 14:07:02.000000 meili-sdk-0.6.0/meili_sdk.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      606 2023-07-24 14:07:02.968427 meili-sdk-0.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:01:36.693670 meili-sdk-0.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     5035 2023-08-01 13:01:36.693670 meili-sdk-0.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4735 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:01:36.682670 meili-sdk-0.6.1/meili_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:01:36.684670 meili-sdk-0.6.1/meili_sdk/clients/
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/clients/apitoken_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/clients/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/clients/persistent_token_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/clients/sdk_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:01:36.684670 meili-sdk-0.6.1/meili_sdk/config/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/config/type.py
+-rw-rw-rw-   0 root         (0) root         (0)      506 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/config/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:01:36.686670 meili-sdk-0.6.1/meili_sdk/models/
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4047 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/models/form.py
+-rw-rw-rw-   0 root         (0) root         (0)      220 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/models/organization.py
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/models/ros_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/models/task.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/models/team.py
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/models/trigger.py
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/models/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/models/vehicle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:01:36.687670 meili-sdk-0.6.1/meili_sdk/mqtt/
+-rw-rw-rw-   0 root         (0) root         (0)      407 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/mqtt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1807 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/mqtt/action_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     8530 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/mqtt/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:01:36.687670 meili-sdk-0.6.1/meili_sdk/mqtt/models/
+-rw-rw-rw-   0 root         (0) root         (0)      250 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/mqtt/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/mqtt/models/action.py
+-rw-rw-rw-   0 root         (0) root         (0)     3379 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/mqtt/models/order.py
+-rw-rw-rw-   0 root         (0) root         (0)     3793 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/mqtt/models/state.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/mqtt/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:01:36.689670 meili-sdk-0.6.1/meili_sdk/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5110 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/resources/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1365 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/resources/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/resources/maps.py
+-rw-rw-rw-   0 root         (0) root         (0)      744 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/resources/organizations.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/resources/ros.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/resources/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/resources/teams.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/resources/triggers.py
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/resources/users.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/resources/vehicles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:01:36.690670 meili-sdk-0.6.1/meili_sdk/schedules/
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/schedules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/schedules/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      845 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/schedules/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/schedules/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/site.py
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/token.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:01:36.691670 meili-sdk-0.6.1/meili_sdk/websockets/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/websockets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15831 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/websockets/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/websockets/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:01:36.693670 meili-sdk-0.6.1/meili_sdk/websockets/models/
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/websockets/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/websockets/models/cancel_task_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/websockets/models/docking_routine_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     6735 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/websockets/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/websockets/models/move_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/websockets/models/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/websockets/models/task_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)      204 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/websockets/models/topic.py
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/websockets/models/traffic_control_action_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/meili_sdk/websockets/models/update_map_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:01:36.683670 meili-sdk-0.6.1/meili_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5035 2023-08-01 13:01:36.000000 meili-sdk-0.6.1/meili_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2075 2023-08-01 13:01:36.000000 meili-sdk-0.6.1/meili_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 13:01:36.000000 meili-sdk-0.6.1/meili_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-08-01 13:01:36.000000 meili-sdk-0.6.1/meili_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-08-01 13:01:36.000000 meili-sdk-0.6.1/meili_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      606 2023-08-01 13:01:36.693670 meili-sdk-0.6.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-08-01 13:01:27.000000 meili-sdk-0.6.1/setup.py
```

### Comparing `meili-sdk-0.6.0/LICENSE.txt` & `meili-sdk-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/PKG-INFO` & `meili-sdk-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meili-sdk
-Version: 0.6.0
+Version: 0.6.1
 Summary: Meili FMS SDK
 Home-page: https://gitlab.com/meilirobots/dev/meili-sdk
 Author: Rimvydas Zilinskas
 Author-email: rimvydas@meilirobots.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: MQTT
```

### Comparing `meili-sdk-0.6.0/README.md` & `meili-sdk-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/clients/__init__.py` & `meili-sdk-0.6.1/meili_sdk/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/clients/apitoken_client.py` & `meili-sdk-0.6.1/meili_sdk/clients/apitoken_client.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/clients/base.py` & `meili-sdk-0.6.1/meili_sdk/clients/base.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/clients/sdk_client.py` & `meili-sdk-0.6.1/meili_sdk/clients/sdk_client.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/exceptions.py` & `meili-sdk-0.6.1/meili_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/models/base.py` & `meili-sdk-0.6.1/meili_sdk/models/base.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/models/form.py` & `meili-sdk-0.6.1/meili_sdk/models/form.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/models/task.py` & `meili-sdk-0.6.1/meili_sdk/models/task.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/models/team.py` & `meili-sdk-0.6.1/meili_sdk/models/team.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/models/trigger.py` & `meili-sdk-0.6.1/meili_sdk/models/trigger.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/models/vehicle.py` & `meili-sdk-0.6.1/meili_sdk/models/vehicle.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/mqtt/action_client.py` & `meili-sdk-0.6.1/meili_sdk/mqtt/action_client.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/mqtt/client.py` & `meili-sdk-0.6.1/meili_sdk/mqtt/client.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/mqtt/models/action.py` & `meili-sdk-0.6.1/meili_sdk/mqtt/models/action.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/mqtt/models/order.py` & `meili-sdk-0.6.1/meili_sdk/mqtt/models/order.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/mqtt/models/state.py` & `meili-sdk-0.6.1/meili_sdk/mqtt/models/state.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/mqtt/site.py` & `meili-sdk-0.6.1/meili_sdk/mqtt/site.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/resources/base.py` & `meili-sdk-0.6.1/meili_sdk/resources/base.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/resources/forms.py` & `meili-sdk-0.6.1/meili_sdk/resources/forms.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/resources/organizations.py` & `meili-sdk-0.6.1/meili_sdk/resources/organizations.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/resources/tasks.py` & `meili-sdk-0.6.1/meili_sdk/resources/tasks.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/resources/teams.py` & `meili-sdk-0.6.1/meili_sdk/resources/teams.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/resources/triggers.py` & `meili-sdk-0.6.1/meili_sdk/resources/triggers.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/resources/vehicles.py` & `meili-sdk-0.6.1/meili_sdk/resources/vehicles.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/schedules/loader.py` & `meili-sdk-0.6.1/meili_sdk/schedules/loader.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/schedules/models.py` & `meili-sdk-0.6.1/meili_sdk/schedules/models.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/site.py` & `meili-sdk-0.6.1/meili_sdk/site.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/websockets/client.py` & `meili-sdk-0.6.1/meili_sdk/websockets/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,33 +230,35 @@
             constants.ACTION_MOVE: self.process_move,
             constants.ACTION_MOVE_TO_CHARGING_POINT: self.process_move,
             constants.ACTION_SLOW_DOWN: self.process_slow_down,
             constants.ACTION_PATH_REROUTING: self.process_path_rerouting,
             constants.ACTION_COLLISION_CLEARANCE: self.process_collision_clearance,
             constants.ACTION_TOPIC_LIST: self.process_request_for_topics,
             constants.ACTION_TOPIC_INITIALIZATION: self.process_topic_list,
-            constants.ACTION_UPDATE_MAP : self.process_update_map,
+            constants.ACTION_UPDATE_MAP: self.process_update_map,
         }
         try:
             processor = processors[action]
         except KeyError:
             logger.warning(
                 f"Cannot handle action {action}. Maybe you are using an outdated library?"
             )
             return
 
         if processor and callable(processor):
             processor(message, vehicle)
+
     def process_update_map(
-        self, message: dict, vehicle: t.Optional[str] = None
+            self, message: dict, vehicle: t.Optional[str] = None
     ):
         update_map_message = UpdateMapMessage(**message["data"])
 
         if self.__update_map_handler and callable(self.__update_map_handler):
-            self.__update_map_handler(update_map_message,vehicle)
+            self.__update_map_handler(update_map_message, vehicle)
+
     def process_docking_routine_request(
             self, message: dict, vehicle: t.Optional[str] = None
     ):
         dock_message = DockingRoutineMessage(**message["data"])
         if self.__docking_routine_request_handler and callable(
                 self.__docking_routine_request_handler
         ):
```

### Comparing `meili-sdk-0.6.0/meili_sdk/websockets/constants.py` & `meili-sdk-0.6.1/meili_sdk/websockets/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 EVENT_SPEED = "speed"
 EVENT_BATTERY = "batteryStatus"
 EVENT_GOAL_STATUS = "goalStatus"
 EVENT_NOTIFICATION = "notification"
 EVENT_TOPICS_LIST = "topics"
 EVENT_TOPIC_DATA = "topic_data"
 EVENT_PATH_DATA = "path_data"
+EVENT_STATUS = "status"
 
 ALL = (
     EVENT_DOCKING_ROUTINE,
     EVENT_REGISTER,
     EVENT_LOCATION,
     EVENT_SPEED,
     EVENT_BATTERY,
     EVENT_GOAL_STATUS,
     EVENT_NOTIFICATION,
     EVENT_TOPIC_DATA,
     EVENT_TOPICS_LIST,
     EVENT_PATH_DATA,
+    EVENT_STATUS,
 )
 
 # Incoming actions
 ACTION_DOCKING_ROUTINE_REQUEST = "docking_routine_request"
 ACTION_DOCKING_ROUTINE_FINALIZE = "docking_routine_finalize_request"
 ACTION_TASK = "task"
 ACTION_TASK_V2 = "taskv2"
```

### Comparing `meili-sdk-0.6.0/meili_sdk/websockets/models/message.py` & `meili-sdk-0.6.1/meili_sdk/websockets/models/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     EVENT_LOCATION,
     EVENT_NOTIFICATION,
     EVENT_PATH_DATA,
     EVENT_REGISTER,
     EVENT_SPEED,
     EVENT_TOPIC_DATA,
     EVENT_TOPICS_LIST,
+    EVENT_STATUS,
 )
 
 __all__ = ("Message",)
 
 
 class Message(BaseModel):
     """
@@ -59,14 +60,15 @@
             EVENT_SPEED: self._validate_value_for_speed,
             EVENT_BATTERY: self._validate_value_for_battery,
             EVENT_GOAL_STATUS: self._validate_value_for_goal_status,
             EVENT_NOTIFICATION: self._validate_value_for_notification,
             EVENT_TOPICS_LIST: self._validate_value_for_topics_list,
             EVENT_TOPIC_DATA: self._validate_value_for_topic_data,
             EVENT_PATH_DATA: self._validate_value_for_path_data,
+            EVENT_STATUS: self._validate_value_for_status,
         }[event](value)
         return value
 
     @staticmethod
     def _validate_value_for_docking_routine(value):
         try:
             path = value["path"]
@@ -176,7 +178,20 @@
             raise ValidationError(f"Missing properties: message")
 
         if not isinstance(message, str):
             raise ValidationError("message needs to be a string")
 
         if len(message) > 255:
             raise ValidationError("message needs to be less than 255 characters")
+
+    def _validate_value_for_status(self, value):
+        try:
+            self._validate_value_for_location(value["location"])
+            self._validate_value_for_speed(value["speed"])
+            if 'battery' in value:
+                self._validate_value_for_battery(value["battery"])
+
+        except Exception as e:
+            raise ValidationError("Missing property location, battery or speed")
+
+
+
```

### Comparing `meili-sdk-0.6.0/meili_sdk/websockets/models/task.py` & `meili-sdk-0.6.1/meili_sdk/websockets/models/task.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/websockets/models/task_v2.py` & `meili-sdk-0.6.1/meili_sdk/websockets/models/task_v2.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk/websockets/models/traffic_control_action_message.py` & `meili-sdk-0.6.1/meili_sdk/websockets/models/traffic_control_action_message.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/meili_sdk.egg-info/PKG-INFO` & `meili-sdk-0.6.1/meili_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meili-sdk
-Version: 0.6.0
+Version: 0.6.1
 Summary: Meili FMS SDK
 Home-page: https://gitlab.com/meilirobots/dev/meili-sdk
 Author: Rimvydas Zilinskas
 Author-email: rimvydas@meilirobots.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: MQTT
```

### Comparing `meili-sdk-0.6.0/meili_sdk.egg-info/SOURCES.txt` & `meili-sdk-0.6.1/meili_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.0/setup.cfg` & `meili-sdk-0.6.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = meili-sdk
 description = Meili FMS SDK
-version = 0.6.0
+version = 0.6.1
 license = MIT
 license_files = LICENSE.txt
 description_file = README.md
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Rimvydas Zilinskas
 author_email = rimvydas@meilirobots.com
```

