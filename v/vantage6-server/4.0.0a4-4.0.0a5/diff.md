# Comparing `tmp/vantage6-server-4.0.0a4.tar.gz` & `tmp/vantage6-server-4.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-server-4.0.0a4.tar", last modified: Mon Jul 24 13:22:28 2023, max compression
+gzip compressed data, was "vantage6-server-4.0.0a5.tar", last modified: Tue Aug  1 14:00:30 2023, max compression
```

## Comparing `vantage6-server-4.0.0a4.tar` & `vantage6-server-4.0.0a5.tar`

### file list

```diff
@@ -1,92 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.784588 vantage6-server-4.0.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-24 13:22:28.784588 vantage6-server-4.0.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:22:28.784588 vantage6-server-4.0.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.776587 vantage6-server-4.0.0a4/tests_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/tests_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/tests_server/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)   139499 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/tests_server/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.776587 vantage6-server-4.0.0a4/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.776587 vantage6-server-4.0.0a4/vantage6/server/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/__build__
--rw-r--r--   0 runner    (1001) docker     (123)    24701 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.776587 vantage6-server-4.0.0a4/vantage6/server/_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.780588 vantage6-server-4.0.0a4/vantage6/server/_data/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/_data/dev/fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/_data/dev/node_a.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/_data/dev/node_b.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/_data/dev/server.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/_data/example_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/_data/unittest_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/_data/unittest_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.780588 vantage6-server-4.0.0a4/vantage6/server/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/cli/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.780588 vantage6-server-4.0.0a4/vantage6/server/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/controller/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/default_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/mail_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.780588 vantage6-server-4.0.0a4/vantage6/server/model/
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/algorithm_port.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/authenticatable.py
--rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/collaboration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.780588 vantage6-server-4.0.0a4/vantage6/server/model/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/node_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/role_rule_association.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/task_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.784588 vantage6-server-4.0.0a4/vantage6/server/resource/
--rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29413 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/collaboration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.784588 vantage6-server-4.0.0a4/vantage6/server/resource/common/
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/common/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/common/input_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/common/output_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/common/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/common/swagger_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/health.py
--rw-r--r--   0 runner    (1001) docker     (123)    22412 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/port.py
--rw-r--r--   0 runner    (1001) docker     (123)    18896 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/recover.py
--rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    28270 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    22580 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    32644 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    12746 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    28822 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/vpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/websocket_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/websockets.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.784588 vantage6-server-4.0.0a4/vantage6_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-24 13:22:28.000000 vantage6-server-4.0.0a4/vantage6_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-24 13:22:28.000000 vantage6-server-4.0.0a4/vantage6_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:28.000000 vantage6-server-4.0.0a4/vantage6_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 13:22:28.000000 vantage6-server-4.0.0a4/vantage6_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-24 13:22:28.000000 vantage6-server-4.0.0a4/vantage6_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-24 13:22:28.000000 vantage6-server-4.0.0a4/vantage6_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:30.575469 vantage6-server-4.0.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-08-01 14:00:30.575469 vantage6-server-4.0.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:00:30.575469 vantage6-server-4.0.0a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:30.567469 vantage6-server-4.0.0a5/tests_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/tests_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/tests_server/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)   140588 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/tests_server/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:30.567469 vantage6-server-4.0.0a5/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:30.567469 vantage6-server-4.0.0a5/vantage6/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)    24701 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:30.567469 vantage6-server-4.0.0a5/vantage6/server/_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:30.571469 vantage6-server-4.0.0a5/vantage6/server/_data/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/_data/dev/fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/_data/dev/node_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/_data/dev/node_b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/_data/dev/server.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/_data/example_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/_data/unittest_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/_data/unittest_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:30.571469 vantage6-server-4.0.0a5/vantage6/server/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/cli/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:30.571469 vantage6-server-4.0.0a5/vantage6/server/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/controller/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/mail_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:30.571469 vantage6-server-4.0.0a5/vantage6/server/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/model/algorithm_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/model/authenticatable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/model/collaboration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:30.571469 vantage6-server-4.0.0a5/vantage6/server/model/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/model/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/model/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/model/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/model/node_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/model/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/model/role_rule_association.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/model/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/model/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/model/task_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18223 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:30.575469 vantage6-server-4.0.0a5/vantage6/server/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29413 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/collaboration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:30.575469 vantage6-server-4.0.0a5/vantage6/server/resource/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/common/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/common/input_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/common/output_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/common/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/common/swagger_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22404 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18896 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/recover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28270 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23510 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33313 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12746 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/vpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/resource/websocket_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/websockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-01 14:00:14.000000 vantage6-server-4.0.0a5/vantage6/server/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:00:30.575469 vantage6-server-4.0.0a5/vantage6_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-08-01 14:00:30.000000 vantage6-server-4.0.0a5/vantage6_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-08-01 14:00:30.000000 vantage6-server-4.0.0a5/vantage6_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:00:30.000000 vantage6-server-4.0.0a5/vantage6_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 14:00:30.000000 vantage6-server-4.0.0a5/vantage6_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-01 14:00:30.000000 vantage6-server-4.0.0a5/vantage6_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 14:00:30.000000 vantage6-server-4.0.0a5/vantage6_server.egg-info/top_level.txt
```

### Comparing `vantage6-server-4.0.0a4/PKG-INFO` & `vantage6-server-4.0.0a5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vantage6-server
-Version: 4.0.0a4
+Version: 4.0.0a5
 Summary: Vantage6 server
 Home-page: https://github.com/vantage6/vantage6
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
   <br>
   <a href="https://vantage6.ai"><img src="https://github.com/IKNL/guidelines/blob/master/resources/logos/vantage6.png?raw=true" alt="vantage6" width="350"></a>
 </h1>
@@ -32,20 +32,22 @@
 
 
 
 -----------------------------------------------------------------------------------------------------
 This repository is part of **vantage6**, our **privacy preserving federated learning infrastructure for secure insight exchange**, and contains all the **vantage6** infrastructure source/ code. Please visit our [website (vantage6.ai)](https://vantage6.ai) to learn more!
 
 ## :books: Documentation
-This repository is home to 4 PyPi packages:
+This repository is home to 6 PyPi packages:
 
 * [vantage6](https://pypi.org/project/vantage6) -> _CLI for managing node and server instances_
 * [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client for interacting with the vantage6-server_
+* [vantage6-algorithm-tools](https://pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate algorithm development_
 * [vantage6-node](https://pypi.org/project/vantage6-node) -> _Node application package_
 * [vantage6-server](https://pypi.org/project/vantage6-server) -> _Server application package_
+* [vantage6-common](https://pypi.org/project/vantage6-common) -> _Server application package_
 
 **Note that when using vantage6 you do not install the _server_ and _node_ packages. These are delivered to you in Docker images.**
 
 Two docker images are published which contain the Node and Server applications:
 
 * `harbor2.vantage6.ai/infrastructure/node:VERSION`
 * `harbor2.vantage6.ai/infrastructure/server:VERSION`
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: vantage6-server Version: 4.0.0a4 Summary: Vantage6
-server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
+Metadata-Version: 2.1 Name: vantage6-server Version: 4.0.0a5 Summary: Vantage6
+server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml) [![PyPI vantage6](https://badge.fury.io/py/vantage6.svg)](https://
@@ -19,32 +19,35 @@
    10.5281/zenodo.7382602.svg)](https://doi.org/10.5281/zenodo.7382602) ****
                  Documentation â¢ Contributing â¢ References
 -------------------------------------------------------------------------------
 ---------------------- This repository is part of **vantage6**, our **privacy
 preserving federated learning infrastructure for secure insight exchange**, and
 contains all the **vantage6** infrastructure source/ code. Please visit our
 [website (vantage6.ai)](https://vantage6.ai) to learn more! ## :books:
-Documentation This repository is home to 4 PyPi packages: * [vantage6](https://
+Documentation This repository is home to 6 PyPi packages: * [vantage6](https://
 pypi.org/project/vantage6) -> _CLI for managing node and server instances_ *
 [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client
-for interacting with the vantage6-server_ * [vantage6-node](https://pypi.org/
-project/vantage6-node) -> _Node application package_ * [vantage6-server](https:
-//pypi.org/project/vantage6-server) -> _Server application package_ **Note that
-when using vantage6 you do not install the _server_ and _node_ packages. These
-are delivered to you in Docker images.** Two docker images are published which
-contain the Node and Server applications: * `harbor2.vantage6.ai/
-infrastructure/node:VERSION` * `harbor2.vantage6.ai/infrastructure/server:
-VERSION` These docker images are used by the _vantage6 CLI_ package, which can
-be installed by running: `pip install vantage6` This will install the CLI which
-enables you to use the commands: * `vnode CMD [OPTIONS]` * `vserver CMD
-[OPTIONS]` You can find more (user) documentation at [Gitbook
-(docs.vantage6.ai)](https://docs.vantage6.ai). If you have any questions,
-suggestions or just want to chat about federated learning: join our [Dircord
-(https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel. ## :
-gift_heart: Contributing We hope to continue developing, improving, and
+for interacting with the vantage6-server_ * [vantage6-algorithm-tools](https://
+pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate
+algorithm development_ * [vantage6-node](https://pypi.org/project/vantage6-
+node) -> _Node application package_ * [vantage6-server](https://pypi.org/
+project/vantage6-server) -> _Server application package_ * [vantage6-common]
+(https://pypi.org/project/vantage6-common) -> _Server application package_
+**Note that when using vantage6 you do not install the _server_ and _node_
+packages. These are delivered to you in Docker images.** Two docker images are
+published which contain the Node and Server applications: *
+`harbor2.vantage6.ai/infrastructure/node:VERSION` * `harbor2.vantage6.ai/
+infrastructure/server:VERSION` These docker images are used by the _vantage6
+CLI_ package, which can be installed by running: `pip install vantage6` This
+will install the CLI which enables you to use the commands: * `vnode CMD
+[OPTIONS]` * `vserver CMD [OPTIONS]` You can find more (user) documentation at
+[Gitbook (docs.vantage6.ai)](https://docs.vantage6.ai). If you have any
+questions, suggestions or just want to chat about federated learning: join our
+[Dircord (https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel. ##
+:gift_heart: Contributing We hope to continue developing, improving, and
 supporting **vantage6** with the help of the federated learning community. If
 you are interested in contributing, first of all, thank you! Second, please
 take a look at our [contributing guidelines](https://docs.vantage6.ai/en/main/
 devops/contribute.html) ## :black_nib: References If you are using
 **vantage6**, please cite this repository as well as the accompanying papers as
 follows: > * F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6. Available at
 https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX. > * A.
```

### Comparing `vantage6-server-4.0.0a4/setup.py` & `vantage6-server-4.0.0a5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     name='vantage6-server',
     version=version_ns['__version__'],
     description='Vantage6 server',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/vantage6/vantage6',
     packages=find_namespace_packages(),
-    python_requires='>=3.6',
+    python_requires='>=3.10',
     install_requires=[
         'bcrypt==4.0.1',
         'flasgger==0.9.5',
         'flask==2.2.5',
         'Flask-Cors==3.0.10',
         'Flask-JWT-Extended==4.4.4',
         'Flask-Mail==0.9.1',
```

### Comparing `vantage6-server-4.0.0a4/tests_server/test_models.py` & `vantage6-server-4.0.0a5/tests_server/test_models.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/tests_server/test_resources.py` & `vantage6-server-4.0.0a5/tests_server/test_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1064,18 +1064,24 @@
         # you can edit other organizations with the global permission
         rule = Rule.get_by_("role", Scope.GLOBAL, Operation.EDIT)
         headers = self.create_user_and_login(rules=[rule])
         result = self.app.post(f'/api/role/{role.id}/rule/{rule.id}',
                                headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.CREATED)
 
-        # however you can only assign rules that you own
+        # you can only rules that are lower in hierarchy than the ones you own
         rule = Rule.get_by_("role", Scope.ORGANIZATION, Operation.EDIT)
         result = self.app.post(f'/api/role/{role.id}/rule/{rule.id}',
                                headers=headers)
+        self.assertEqual(result.status_code, HTTPStatus.CREATED)
+
+        # you can't assign rules you don't own
+        rule = Rule.get_by_("node", Scope.ORGANIZATION, Operation.EDIT)
+        result = self.app.post(f'/api/role/{role.id}/rule/{rule.id}',
+                               headers=headers)
         self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
 
         # test inside the collaboration
         org2 = Organization()
         org2.save()
         col = Collaboration(organizations=[org, org2])
         col.save()
@@ -1477,20 +1483,34 @@
         self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
 
         # test that you cannot assign role that has rules that you do not own
         role = Role(name="somename", rules=[not_owning_rule],
                     organization=org)
         role.save()
         result = self.app.patch(f'/api/user/{user.id}', headers=headers, json={
-            'rules': [role.id]
+            'roles': [role.id]
         })
         self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
 
-        # test that you cannot assign rules if you don't have all the rules
-        # that the other user has
+        # test that you CAN assign rules if you have higher permissions than
+        # the user you are assigning rules to. In this case, the user being
+        # changed only has permission to edit their own user, while the actor
+        # has global permission for that
+        headers = self.create_user_and_login(rules=[rule, not_owning_rule])
+        result = self.app.patch(f'/api/user/{user.id}', headers=headers, json={
+            'rules': [not_owning_rule.id, rule.id]
+        })
+        self.assertEqual(result.status_code, HTTPStatus.OK)
+
+        # test that you cannot assign rules to users if they have permissions
+        # that you don't have yourself
+        second_not_owning_rule = Rule.get_by_("node", Scope.ORGANIZATION,
+                                              Operation.EDIT)
+        user.rules.append(second_not_owning_rule)
+        user.save()
         headers = self.create_user_and_login(rules=[rule, not_owning_rule])
         result = self.app.patch(f'/api/user/{user.id}', headers=headers, json={
             'rules': [not_owning_rule.id, rule.id]
         })
         self.assertEqual(result.status_code, HTTPStatus.UNAUTHORIZED)
 
         # test that you CAN change the rules. To do so, a user is generated
```

### Comparing `vantage6-server-4.0.0a4/vantage6/server/__init__.py` & `vantage6-server-4.0.0a5/vantage6/server/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/_data/dev/fixtures.yaml` & `vantage6-server-4.0.0a5/vantage6/server/_data/dev/fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/_data/dev/node_a.yaml` & `vantage6-server-4.0.0a5/vantage6/server/_data/dev/node_a.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/_data/dev/node_b.yaml` & `vantage6-server-4.0.0a5/vantage6/server/_data/dev/node_b.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/_data/dev/server.yaml` & `vantage6-server-4.0.0a5/vantage6/server/_data/dev/server.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/_data/example_fixtures.yaml` & `vantage6-server-4.0.0a5/vantage6/server/_data/example_fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/_data/unittest_config.yaml` & `vantage6-server-4.0.0a5/vantage6/server/_data/unittest_config.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/_data/unittest_fixtures.yaml` & `vantage6-server-4.0.0a5/vantage6/server/_data/unittest_fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/_version.py` & `vantage6-server-4.0.0a5/vantage6/server/_version.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/cli/server.py` & `vantage6-server-4.0.0a5/vantage6/server/cli/server.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/context.py` & `vantage6-server-4.0.0a5/vantage6/server/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/controller/fixture.py` & `vantage6-server-4.0.0a5/vantage6/server/controller/fixture.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/db.py` & `vantage6-server-4.0.0a5/vantage6/server/db.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/default_roles.py` & `vantage6-server-4.0.0a5/vantage6/server/default_roles.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/globals.py` & `vantage6-server-4.0.0a5/vantage6/server/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/mail_service.py` & `vantage6-server-4.0.0a5/vantage6/server/mail_service.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/model/__init__.py` & `vantage6-server-4.0.0a5/vantage6/server/model/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/model/algorithm_port.py` & `vantage6-server-4.0.0a5/vantage6/server/model/algorithm_port.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/model/authenticatable.py` & `vantage6-server-4.0.0a5/vantage6/server/model/authenticatable.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/model/base.py` & `vantage6-server-4.0.0a5/vantage6/server/model/base.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/model/collaboration.py` & `vantage6-server-4.0.0a5/vantage6/server/model/collaboration.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/model/common/utils.py` & `vantage6-server-4.0.0a5/vantage6/server/model/common/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/model/member.py` & `vantage6-server-4.0.0a5/vantage6/server/model/member.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/model/node.py` & `vantage6-server-4.0.0a5/vantage6/server/model/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/model/node_config.py` & `vantage6-server-4.0.0a5/vantage6/server/model/node_config.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/model/organization.py` & `vantage6-server-4.0.0a5/vantage6/server/model/organization.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/model/permission.py` & `vantage6-server-4.0.0a5/vantage6/server/model/permission.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/model/role.py` & `vantage6-server-4.0.0a5/vantage6/server/model/role.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from sqlalchemy.orm import relationship
 from sqlalchemy.orm.exc import NoResultFound
 
 from vantage6.server.model.base import Base, DatabaseSessionManager
 
 
 class Role(Base):
-    """Collection of :class:`.~vantage6.server.model.rule.Rule`s
+    """Collection of :class:`.~vantage6.server.model.rule.Rule` permissions
 
     Attributes
     ----------
     name : str
         Name of the role
     description : str
         Description of the role
```

### Comparing `vantage6-server-4.0.0a4/vantage6/server/model/rule.py` & `vantage6-server-4.0.0a5/vantage6/server/model/rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/model/run.py` & `vantage6-server-4.0.0a5/vantage6/server/model/run.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/model/task.py` & `vantage6-server-4.0.0a5/vantage6/server/model/task.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/model/task_database.py` & `vantage6-server-4.0.0a5/vantage6/server/model/task_database.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/model/user.py` & `vantage6-server-4.0.0a5/vantage6/server/model/user.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/permission.py` & `vantage6-server-4.0.0a5/vantage6/server/permission.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,83 @@
 
 module_name = logger_name(__name__)
 log = logging.getLogger(module_name)
 
 RuleNeed = namedtuple("RuleNeed", ["name", "scope", "operation"])
 
 
+# TODO BvB 2023-07-27 this utility is a bit superfluous with the definition
+# of the operation and scope enums. We should remove it but then add longer
+# values to the enums, which leads to many other changes
+def print_operation(operation: Operation) -> str:
+    """
+    String representation of the operation, that is readable by humans.
+
+    Parameters
+    ----------
+    operation : Operation
+        Operation to be printed
+
+    Returns
+    -------
+    str
+        String representation of the operation
+
+    Raises
+    ------
+    ValueError
+        If the operation is not known
+    """
+    if operation.VIEW:
+        return "view"
+    elif operation.EDIT:
+        return "edit"
+    elif operation.CREATE:
+        return "create"
+    elif operation.DELETE:
+        return "delete"
+    elif operation.SEND:
+        return "send"
+    elif operation.RECEIVE:
+        return "receive"
+    else:
+        raise ValueError(f"Unknown operation {operation}")
+
+
+def print_scope(scope: Scope) -> str:
+    """
+    String representation of the scope, that is readable by humans.
+
+    Parameters
+    ----------
+    scope : Scope
+        Scope to be printed
+
+    Returns
+    -------
+    str
+        String representation of the scope
+
+    Raises
+    ------
+    ValueError
+        If the scope is not known
+    """
+    if scope.ORGANIZATION:
+        return "organization"
+    elif scope.COLLABORATION:
+        return "collaboration"
+    elif scope.GLOBAL:
+        return "global"
+    elif scope.OWN:
+        return "own"
+    else:
+        raise ValueError(f"Unknown scope {scope}")
+
+
 class RuleCollection(dict):
     """
     Class that tracks a set of all rules for a certain resource name
 
     Parameters
     ----------
     name: str
@@ -44,31 +113,36 @@
             Scope within which to apply the rule
         operation: Operation
             What operation the rule applies to
         """
         permission = Permission(RuleNeed(self.name, scope, operation))
         self.__setattr__(f'{operation}_{scope}', permission)
 
-    def can_for_org(self, operation: Operation, subject_org_id: int) -> bool:
+    def can_for_org(self, operation: Operation,
+                    subject_org_id: int | str) -> bool:
         """
         Check if an operation is allowed on a certain organization
 
         Parameters
         ----------
         operation: Operation
             Operation to check if allowed
-        subject_org_id: int
-            Organization id on which the operation should be allowed
+        subject_org_id: int | str
+            Organization id on which the operation should be allowed. If a
+            string is given, it will be converted to an int
 
         Returns
         -------
         bool
             True if the operation is allowed on the organization, False
             otherwise
         """
+        if isinstance(subject_org_id, str):
+            subject_org_id = int(subject_org_id)
+
         auth_org = obtain_auth_organization()
 
         # check if the entity has global permission
         global_perm = getattr(self, f'{operation}_{Scope.GLOBAL}')
         if global_perm and global_perm.can():
             return True
 
@@ -85,26 +159,31 @@
             for col in auth_org.collaborations:
                 if subject_org_id in [org.id for org in col.organizations]:
                     return True
 
         # no permission found
         return False
 
-    def can_for_col(self, operation: Operation, collaboration_id: int) -> bool:
+    def can_for_col(self, operation: Operation,
+                    collaboration_id: int | str) -> bool:
         """
         Check if the user or node can perform the operation on a certain
         collaboration
 
         Parameters
         ----------
         operation: Operation
             Operation to check if allowed
-        collaboration_id: int
-            Collaboration id on which the operation should be allowed
+        collaboration_id: int | str
+            Collaboration id on which the operation should be allowed. If a
+            string is given, it will be converted to an int
         """
+        if isinstance(collaboration_id, str):
+            collaboration_id = int(collaboration_id)
+
         auth_collabs = obtain_auth_collaborations()
 
         # check if the entity has global permission
         global_perm = getattr(self, f'{operation}_{Scope.GLOBAL}')
         if global_perm and global_perm.can():
             return True
 
@@ -221,15 +300,15 @@
 class PermissionManager:
     """
     Loads the permissions and syncs rules in database with rules defined in
     the code
     """
 
     def __init__(self) -> None:
-        self.collections = {}
+        self.collections: dict[str, RuleCollection] = {}
         log.info("Loading permission system...")
         self.load_rules_from_resources()
 
     def load_rules_from_resources(self) -> None:
         """
         Collect all permission rules from all registered API resources
         """
@@ -463,30 +542,29 @@
             name=name,
             operation=operation,
             scope=scope
         ).scalar()
         session.commit()
         return result
 
-    @staticmethod
-    def check_user_rules(rules: list[Rule]) -> dict | bool:
+    def check_user_rules(self, rules: list[Rule]) -> dict | None:
         """
         Check if a user, node or container has all the `rules` in a list
 
         Parameters
         ----------
         rules: list[:class:`~vantage6.server.model.rule.Rule`]
             List of rules that user is checked to have
 
         Returns
         -------
-        dict | bool
+        dict | None
             Dict with a message which rule is missing, else None
         """
         for rule in rules:
-            requires = RuleNeed(rule.name, rule.scope, rule.operation)
-            try:
-                Permission(requires).test()
-            except PermissionDenied:
+            if not self.collections[rule.name].has_at_least_scope(
+                rule.scope, rule.operation
+            ):
                 return {"msg": f"You don't have the rule ({rule.name}, "
-                        f"{rule.scope}, {rule.operation})"}
+                        f"{print_scope(rule.scope)}, "
+                        f"{print_operation(rule.operation)})"}
         return None
```

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/__init__.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/collaboration.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/collaboration.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/common/auth_helper.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/common/auth_helper.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/common/input_schema.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/common/input_schema.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/common/output_schema.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/common/output_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from marshmallow import fields
 from marshmallow_sqlalchemy import SQLAlchemyAutoSchema
 from flask import url_for
 
 from vantage6.server import db
 from vantage6.common import logger_name
 from vantage6.common.globals import STRING_ENCODING
-from vantage6.server.model import Base
+from vantage6.server.model import Base, User
 from vantage6.server.resource.common.pagination import Pagination
 
 log = logging.getLogger(logger_name(__name__))
 
 
 def create_one_to_many_link(obj: Base, link_to: str, link_from: str) -> str:
     """
@@ -344,14 +344,57 @@
     rules = fields.Function(lambda obj: create_one_to_many_link(
         obj, link_to='rule', link_from='user_id'
     ))
 
     organization = fields.Method("organization")
 
 
+class UserWithPermissionDetailsSchema(UserSchema):
+    """
+    A schema for API responses that contains regular user details plus
+    additional permission details for the user to be used by the UI.
+    """
+    permissions = fields.Method("permissions_")
+
+    @staticmethod
+    def permissions_(obj: User) -> dict:
+        """
+        Returns a dictionary containing permission details for the user to be
+        used by the UI.
+
+        Parameters
+        ----------
+        obj : User
+            The user to get permission details for.
+
+        Returns
+        -------
+        dict
+            A dictionary containing permission details for the user.
+        """
+        role_ids = [role.id for role in obj.roles]
+        rule_ids = list(set(
+            [rule.id for rule in obj.rules] + \
+            [rule.id for role in obj.roles for rule in role.rules]
+        ))
+        # Return which organizations the user is in collaboration with so that
+        # UI knows which organizations user has access to if they have
+        # collaboration scope permissions
+        orgs_in_collabs = list(set([
+            org.id
+            for collab in obj.organization.collaborations
+            for org in collab.organizations
+        ]))
+        return {
+            "roles": role_ids,
+            "rules": rule_ids,
+            "orgs_in_collabs": orgs_in_collabs
+        }
+
+
 class RoleSchema(HATEOASModelSchema):
 
     rules = fields.Function(lambda obj: create_one_to_many_link(
         obj, link_to='rule', link_from='role_id'
     ))
     users = fields.Function(lambda obj: create_one_to_many_link(
         obj, link_to='user', link_from='role_id'
```

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/common/pagination.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/common/pagination.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/common/swagger_templates.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/common/swagger_templates.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/event.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/event.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/health.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/health.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/node.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,20 +212,21 @@
                 return {
                     'msg': 'You lack the permission view nodes from the '
                     f'organization with id {args["organization_id"]}!'
                 }, HTTPStatus.UNAUTHORIZED
             q = q.filter(db.Node.organization_id == args['organization_id'])
 
         if 'collaboration_id' in args:
-            if not self.r.can_for_col(P.VIEW, int(args['collaboration_id'])):
+            collaboration_id = int(args['collaboration_id'])
+            if not self.r.can_for_col(P.VIEW, collaboration_id):
                 return {
                     'msg': 'You lack the permission view nodes from the '
-                    f'collaboration with id {args["collaboration_id"]}!'
+                    f'collaboration with id {collaboration_id}!'
                 }, HTTPStatus.UNAUTHORIZED
-            q = q.filter(db.Node.collaboration_id == args['collaboration_id'])
+            q = q.filter(db.Node.collaboration_id == collaboration_id)
 
         for param in ['status', 'ip']:
             if param in args:
                 q = q.filter(getattr(db.Node, param) == args[param])
         if 'name' in args:
             q = q.filter(db.Node.name.like(args['name']))
 
@@ -595,18 +596,18 @@
                         'not found!'}, HTTPStatus.NOT_FOUND
             node.organization = organization
 
         auth = self.obtain_auth()
         col_id = data.get('collaboration_id')
         updated_col = col_id and col_id != node.collaboration.id
         if updated_col:
-            collaboration = db.Collaboration.get(data['collaboration_id'])
+            collaboration = db.Collaboration.get(col_id)
             if not collaboration:
-                return {'msg': f'collaboration id={data["collaboration_id"]}'
-                        'not found!'}, HTTPStatus.NOT_FOUND
+                return {'msg': f'collaboration id={col_id} not found!'}, \
+                    HTTPStatus.NOT_FOUND
 
             if not self.r.e_glo.can():
                 if auth.organization not in collaboration.organizations:
                     return {'msg': f'Organization id={auth.organization.id} '
                             'of this node is not part of this collaboration id'
                             f'={collaboration.id}'}
```

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/organization.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/organization.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/port.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/port.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/recover.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/recover.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/result.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/token.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,421 +1,389 @@
 # -*- coding: utf-8 -*-
+"""
+Resources below '/<api_base>/token'
+"""
 import logging
+import pyotp
 
-from flask import g, request
+from flask import request, g
+from flask_jwt_extended import (
+    jwt_required,
+    create_access_token,
+    create_refresh_token,
+    get_jwt_identity
+)
 from flask_restful import Api
 from http import HTTPStatus
-from sqlalchemy import desc
 
-from vantage6.common import logger_name
+from vantage6 import server
+from vantage6.common.task_status import has_task_finished
 from vantage6.server import db
-from vantage6.server.permission import (
-    PermissionManager,
-    Scope as S,
-    Operation as P
-)
+from vantage6.server.model.user import User
 from vantage6.server.resource import (
     with_node,
-    only_for,
-    parse_datetime,
     ServicesResources
 )
-from vantage6.server.resource.common.pagination import Pagination
-from vantage6.server.resource.common.output_schema import (
-    ResultSchema,
-    ResultTaskIncludedSchema
+from vantage6.server.resource.common.auth_helper import (
+  user_login, create_qr_uri
 )
-from vantage6.server.model import (
-    Result as db_Result,
-    Node,
-    Task,
-    Collaboration,
-    Organization
+from vantage6.server.resource.common.input_schema import (
+    TokenAlgorithmInputSchema,
+    TokenNodeInputSchema,
+    TokenUserInputSchema
 )
 
-module_name = logger_name(__name__)
+module_name = __name__.split('.')[-1]
 log = logging.getLogger(module_name)
 
 
 def setup(api: Api, api_base: str, services: dict) -> None:
     """
-    Setup the result resource.
+    Setup the token resource.
 
     Parameters
     ----------
     api : Api
         Flask restful api instance
     api_base : str
         Base url of the api
     services : dict
         Dictionary with services required for the resource endpoints
     """
     path = "/".join([api_base, module_name])
-    log.info(f'Setting up "{path}" and subdirectories')
+    log.info('Setting up "{}" and subdirectories'.format(path))
 
     api.add_resource(
-        Results,
-        path,
-        endpoint='result_without_id',
-        methods=('GET',),
+        UserToken,
+        path+'/user',
+        endpoint='user_token',
+        methods=('POST',),
         resource_class_kwargs=services
     )
+
     api.add_resource(
-        Result,
-        path + '/<int:id>',
-        endpoint='result_with_id',
-        methods=('GET', 'PATCH'),
+        NodeToken,
+        path+'/node',
+        endpoint='node_token',
+        methods=('POST',),
         resource_class_kwargs=services
     )
 
+    api.add_resource(
+        ContainerToken,
+        path+'/container',
+        endpoint='container_token',
+        methods=('POST',),
+        resource_class_kwargs=services
+    )
 
-# Schemas
-result_schema = ResultSchema()
-result_inc_schema = ResultTaskIncludedSchema()
-
-
-# -----------------------------------------------------------------------------
-# Permissions
-# -----------------------------------------------------------------------------
-def permissions(permissions: PermissionManager) -> None:
-    """
-    Define the permissions for this resource.
+    api.add_resource(
+        RefreshToken,
+        path+'/refresh',
+        endpoint='refresh_token',
+        methods=('POST',),
+        resource_class_kwargs=services
+    )
 
-    Parameters
-    ----------
-    permissions : PermissionManager
-        Permission manager instance to which permissions are added
-    """
-    add = permissions.appender(module_name)
 
-    add(scope=S.GLOBAL, operation=P.VIEW,
-        description="view any result")
-    add(scope=S.ORGANIZATION, operation=P.VIEW, assign_to_container=True,
-        assign_to_node=True, description="view results of your organizations "
-        "collaborations")
+user_token_input_schema = TokenUserInputSchema()
+node_token_input_schema = TokenNodeInputSchema()
+algorithm_token_input_schema = TokenAlgorithmInputSchema()
 
 
 # ------------------------------------------------------------------------------
 # Resources / API's
 # ------------------------------------------------------------------------------
-class ResultBase(ServicesResources):
-
-    def __init__(self, socketio, mail, api, permissions, config):
-        super().__init__(socketio, mail, api, permissions, config)
-        self.r = getattr(self.permissions, module_name)
-
-
-class Results(ResultBase):
+class UserToken(ServicesResources):
+    """resource for api/token"""
 
-    @only_for(('node', 'user', 'container'))
-    def get(self):
-        """ Returns a list of results
+    def post(self):
+        """Login user
         ---
-
         description: >-
-            Returns a list of all results you are allowed to see.\n
+          Allow user to sign in by supplying a username and password. When MFA
+          is enabled on the server, a code is also required
 
-            ### Permission Table\n
-            |Rule name|Scope|Operation|Assigned to node|Assigned to container|
-            Description|\n
-            |--|--|--|--|--|--|\n
-            |Result|Global|View|❌|❌|View any result|\n
-            |Result|Organization|View|✅|✅|View the results of your
-            organization's collaborations|\n
-
-            Accessible to users.
-
-        parameters:
-            - in: query
-              name: task_id
-              schema:
-                type: integer
-              description: Task id
-            - in: query
-              name: organization_id
-              schema:
-                type: integer
-              description: Organization id
-            - in: query
-              name: assigned_from
-              schema:
-                type: date (yyyy-mm-dd)
-              description: Show only task assigned from this date
-            - in: query
-              name: started_from
-              schema:
-                type: date (yyyy-mm-dd)
-              description: Show only task started from this date
-            - in: query
-              name: finished_from
-              schema:
-                type: date (yyyy-mm-dd)
-              description: Show only task finished from this date
-            - in: query
-              name: assigned_till
-              schema:
-                type: date (yyyy-mm-dd)
-              description: Show only task assigned till this date
-            - in: query
-              name: started_till
-              schema:
-                type: date (yyyy-mm-dd)
-              description: Show only task started till this date
-            - in: query
-              name: finished_till
-              schema:
-                type: date (yyyy-mm-dd)
-              description: Show only task finished till this date
-            - in: query
-              name: state
-              schema:
-                type: string
-              description: The state of the task ('open')
-            - in: query
-              name: node_id
-              schema:
-                type: integer
-              description: Node id
-            - in: query
-              name: port
-              schema:
-                type: integer
-              description: Port number
-            - in: query
-              name: include
-              schema:
-                type: string (can be multiple)
-              description: Include 'task' to include task data.
-            - in: query
-              name: page
-              schema:
-                type: integer
-              description: Page number for pagination (default=1)
-            - in: query
-              name: per_page
-              schema:
-                type: integer
-              description: Number of items per page (default=10)
-            - in: query
-              name: sort
+        requestBody:
+          content:
+            application/json:
               schema:
-                type: string
-              description: >-
-                Sort by one or more fields, separated by a comma. Use a minus
-                sign (-) in front of the field to sort in descending order.
+                properties:
+                  username:
+                    type: string
+                    description: Username of user that is logging in
+                  password:
+                    type: string
+                    description: User password
+                  mfa_code:
+                    type: string
+                    description: Two-factor authentication code. Only required
+                      if two-factor authentication is mandatory.
 
         responses:
           200:
-            description: Ok
-          401:
-            description: Unauthorized
+            description: Ok, authenticated
           400:
-            description: Improper values for pagination or sorting parameters
-
-        security:
-        - bearerAuth: []
+            description: Username/password combination unknown, or missing from
+              request body.
+          401:
+            description: Password and/or two-factor authentication token
+              incorrect.
 
-        tags: ["Result"]
+        tags: ["Authentication"]
         """
-        auth_org = self.obtain_auth_organization()
-        args = request.args
+        log.debug("Authenticate user using username and password")
 
-        q = g.session.query(db_Result)
+        body = request.get_json()
+        # validate request body
+        errors = user_token_input_schema.validate(body)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
 
-        # relation filters
-        for param in ['task_id', 'organization_id', 'port']:
-            if param in args:
-                q = q.filter(getattr(db_Result, param) == args[param])
-
-        # date selections
-        for param in ['assigned', 'started', 'finished']:
-            if f'{param}_till' in args:
-                q = q.filter(getattr(db_Result, f'{param}_at')
-                             <= args[f'{param}_till'])
-            if f'{param}_from' in args:
-                q = q.filter(db_Result.assigned_at >= args[f'{param}_from'])
-
-        # custom filters
-        if args.get('state') == 'open':
-            q = q.filter(db_Result.finished_at.is_(None))
-
-        q = q.join(Organization).join(Node).join(Task, db_Result.task)\
-            .join(Collaboration)
-
-        if args.get('node_id'):
-            q = q.filter(db.Node.id == args.get('node_id'))\
-                .filter(db.Collaboration.id == db.Node.collaboration_id)
-
-        # filter based on permissions
-        if not self.r.v_glo.can():
-            if self.r.v_org.can():
-                col_ids = [col.id for col in auth_org.collaborations]
-                q = q.filter(Collaboration.id.in_(col_ids))
+        # Check JSON body
+        username = body.get('username')
+        password = body.get('password')
+
+        user, code = user_login(self.config, username, password, self.mail)
+        if code != HTTPStatus.OK:  # login failed
+            log.error(f"Failed to login for user='{username}'")
+            return user, code
+
+        is_mfa_enabled = self.config.get('two_factor_auth', False)
+        if is_mfa_enabled:
+            if user.otp_secret is None:
+                # server requires mfa but user hasn't set it up yet. Return
+                # an URI to generate a QR code
+                log.info(f'Redirecting user {username} to setup MFA')
+                return create_qr_uri(user), HTTPStatus.OK
             else:
-                return {'msg': 'You lack the permission to do that!'}, \
-                    HTTPStatus.UNAUTHORIZED
+                # 2nd authentication factor: check the OTP secret of the user
+                mfa_code = body.get('mfa_code')
+                if not mfa_code:
+                    # note: this is not treated as error, but simply guide
+                    # user to also fill in second factor
+                    return {"msg": "Please include your two-factor "
+                            "authentication code"}, HTTPStatus.OK
+                elif not self.validate_2fa_token(user, mfa_code):
+                    return {
+                        "msg": "Your two-factor authentication code is "
+                               "incorrect!"
+                    }, HTTPStatus.UNAUTHORIZED
 
-        # query the DB and paginate
-        q = q.order_by(desc(db_Result.id))
-        try:
-            page = Pagination.from_query(query=q, request=request)
-        except ValueError as e:
-            return {'msg': str(e)}, HTTPStatus.BAD_REQUEST
+        token = _get_token_dict(user, self.api)
 
-        # serialization of the models
-        s = result_inc_schema if self.is_included('task') else result_schema
+        log.info(f"Succesfull login from {username}")
+        return token, HTTPStatus.OK, {'jwt-token': token['access_token']}
 
-        return self.response(page, s)
+    @staticmethod
+    def validate_2fa_token(user: User, mfa_code: int | str) -> bool:
+        """
+        Check whether the 6-digit two-factor authentication code is valid
 
+        Parameters
+        ----------
+        user: User
+            The SQLAlchemy model of the user who is authenticating
+        mfa_code: int | str
+            A six-digit TOTP code from an authenticator app
+
+        Returns
+        -------
+        bool
+          Whether six-digit code is valid or not
+        """
+        # the option `valid_window=1` means the code from 1 time window (30s)
+        # ago, is also valid. This prevents that users around the edge of
+        # the time window can still login successfully if server is a bit slow
+        return pyotp.TOTP(user.otp_secret).verify(str(mfa_code),
+                                                  valid_window=1)
 
-class Result(ResultBase):
-    """Resource for /api/result"""
 
-    @only_for(('node', 'user', 'container'))
-    def get(self, id):
-        """ Get a single result
-        ---
+class NodeToken(ServicesResources):
 
+    def post(self):
+        """Login node
+        ---
         description: >-
-            Returns a result from a task specified by an id. \n
+          Allows node to sign in using a unique API key. If the login is
+          successful this returns a dictionary with access and refresh tokens
+          for the node as well as a node_url and a refresh_url.
 
-            ### Permission Table\n
-            |Rule name|Scope|Operation|Assigned to node|Assigned to container|
-            Description|\n
-            |--|--|--|--|--|--|\n
-            |Result|Global|View|❌|❌|View any result|\n
-            |Result|Organization|View|✅|✅|View the results of your
-            organizations collaborations|\n
-
-            Accessible to users.
-
-        parameters:
-          - in: path
-            name: id
-            schema:
-              type: integer
-            minimum: 1
-            description: Task id
-            required: true
-          - in: query
-            name: include
-            schema:
-              type: string
-            description: what to include ('task')
+        requestBody:
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/Node'
 
         responses:
           200:
-              description: Ok
+            description: Ok, authenticated
+          400:
+            description: No API key provided in request body.
           401:
-              description: Unauthorized
-          404:
-              description: Result id not found
+            description: Invalid API key
 
-        security:
-          - bearerAuth: []
-
-        tags: ["Result"]
+        tags: ["Authentication"]
         """
+        log.debug("Authenticate Node using api key")
+
+        body = request.get_json()
+        # validate request body
+        errors = node_token_input_schema.validate(body)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
+
+        # Check JSON body
+        api_key = request.json.get('api_key')
+        node = db.Node.get_by_api_key(api_key)
+        if not node:  # login failed
+            log.error("Api key is not recognized")
+            return {"msg": "Api key is not recognized!"}, \
+                HTTPStatus.UNAUTHORIZED
 
-        auth_org = self.obtain_auth_organization()
+        token = _get_token_dict(node, self.api)
 
-        result = db_Result.get(id)
-        if not result:
-            return {'msg': f'Result id={id} not found!'}, \
-                HTTPStatus.NOT_FOUND
-        if not self.r.v_glo.can():
-            c_orgs = result.task.collaboration.organizations
-            if not (self.r.v_org.can() and auth_org in c_orgs):
-                return {'msg': 'You lack the permission to do that!'}, \
-                    HTTPStatus.UNAUTHORIZED
+        log.info(f"Succesfull login as node '{node.id}' ({node.name})")
+        return token, HTTPStatus.OK, {'jwt-token': token['access_token']}
 
-        s = result_inc_schema if request.args.get('include') == 'task' \
-            else result_schema
 
-        return s.dump(result, many=False), HTTPStatus.OK
+class ContainerToken(ServicesResources):
 
     @with_node
-    def patch(self, id):
-        """Update results
+    def post(self):
+        """Algorithm container login
         ---
         description: >-
-          Update results from the node. Only done if the request comes from the
-          correct, authenticated node.\n
-
-          The user cannot access this endpoint so they cannot tamper with any
-          results.
+          Generate token for the algorithm container of a specific task.\n
 
-        parameters:
-          - in: path
-            name: id
-            schema:
-              type: integer
-              minimum: 1
-            description: Task id
-            required: tr
+          Not available to users; only for authenticated nodes.
 
         requestBody:
           content:
             application/json:
               schema:
-                properties:
-                  started_at:
-                    type: string
-                    description: Time at which task was started
-                  finished_at:
-                    type: string
-                    description: Time at which task was completed
-                  result:
-                    type: string
-                    description: (Encrypted) result of the task
-                  log:
-                    type: string
-                    description: Task log messages
+                $ref: '#/components/schemas/ContainerToken'
 
         responses:
           200:
-            description: Ok
+            description: Container token generated
           400:
-            description: Results already posted
+            description: Task does not exist or is already completed
           401:
-            description: Unauthorized
-          404:
-            description: Result id not found
+            description: Key request for invalid image or task
+
+        tags: ["Authentication"]
+        """
+        log.debug("Creating a token for a container running on a node")
+
+        body = request.get_json()
+        # validate request body
+        errors = algorithm_token_input_schema.validate(body)
+        if errors:
+            return {'msg': 'Request body is incorrect', 'errors': errors}, \
+                HTTPStatus.BAD_REQUEST
+
+        task_id = body.get("task_id")
+        claim_image = body.get("image")
+
+        db_task = db.Task.get(task_id)
+        if not db_task:
+            log.warning(f"Node {g.node.id} attempts to generate key for task "
+                        f"{task_id} that does not exist")
+            return {"msg": "Parent task does not exist!"}, \
+                HTTPStatus.BAD_REQUEST
+
+        # verify that task the token is requested for exists
+        if claim_image != db_task.image:
+            log.warning(
+                f"Node {g.node.id} attempts to generate key for image "
+                f"{claim_image} that does not belong to task {task_id}."
+            )
+            return {"msg": "Image and task do no match"}, \
+                HTTPStatus.UNAUTHORIZED
+
+        # check if the node is in the collaboration to which the task is
+        # enlisted
+        if g.node.collaboration_id != db_task.collaboration_id:
+            log.warning(
+                f"Node {g.node.id} attempts to generate key for task {task_id}"
+                f" which is outside its collaboration "
+                f"({g.node.collaboration_id}/{db_task.collaboration_id})."
+            )
+            return {"msg": "You are not within the collaboration"}, \
+                HTTPStatus.UNAUTHORIZED
+
+        # validate that the task not has been finished yet
+        if has_task_finished(db_task.status):
+            log.warning(f"Node {g.node.id} attempts to generate a key for "
+                        f"completed task {task_id}")
+            return {"msg": "Task is already finished!"}, HTTPStatus.BAD_REQUEST
+
+        # container identity consists of its node_id,
+        # task_id, collaboration_id and image_id
+        container = {
+            "client_type": "container",
+            "node_id": g.node.id,
+            "organization_id": g.node.organization_id,
+            "collaboration_id": g.node.collaboration_id,
+            "task_id": task_id,
+            "image": claim_image,
+            "databases": [db_entry.database for db_entry in db_task.databases]
+        }
+        token = create_access_token(container, expires_delta=False)
+
+        return {'container_token': token}, HTTPStatus.OK
+
+
+class RefreshToken(ServicesResources):
+
+    @jwt_required(refresh=True)
+    def post(self):
+        """Refresh token
+        ---
+        description: >-
+          Refresh access token if the previous one is expired.\n
+
+          Your refresh token must be present in the request headers to use
+          this endpoint.
+
+        responses:
+          200:
+            description: Token refreshed
 
         security:
           - bearerAuth: []
 
-        tags: ["Result"]
+        tags: ["Authentication"]
         """
-        result = db_Result.get(id)
-        if not result:
-            return {'msg': f'Result id={id} not found!'}, HTTPStatus.NOT_FOUND
-
-        data = request.get_json()
-
-        if result.organization_id != g.node.organization_id:
-            log.warn(
-                f"{g.node.name} tries to update a result that does not belong "
-                f"to him. ({result.organization_id}/{g.node.organization_id})"
-            )
-            return {"msg": "This is not your result to PATCH!"}, \
-                HTTPStatus.UNAUTHORIZED
+        user_or_node_id = get_jwt_identity()
+        log.info(f'Refreshing token for user or node "{user_or_node_id}"')
+        user_or_node = db.Authenticatable.get(user_or_node_id)
 
-        if result.finished_at is not None:
-            return {"msg": "Cannot update an already finished result!"}, \
-                HTTPStatus.BAD_REQUEST
+        return _get_token_dict(user_or_node, self.api), HTTPStatus.OK
 
-        # notify collaboration nodes/users that the task has an update
-        self.socketio.emit(
-            "status_update", {'result_id': id}, namespace='/tasks',
-            room=f'collaboration_{result.task.collaboration.id}'
-        )
-
-        result.started_at = parse_datetime(data.get("started_at"),
-                                           result.started_at)
-        result.finished_at = parse_datetime(data.get("finished_at"))
-        result.result = data.get("result")
-        result.log = data.get("log")
-        result.status = data.get("status", result.status)
-        result.save()
 
-        return result_schema.dump(result, many=False), HTTPStatus.OK
+def _get_token_dict(user_or_node: db.Authenticatable, api: Api) -> dict:
+    """
+    Create a dictionary with the tokens and urls for the user or node.
+
+    Parameters
+    ----------
+    user_or_node : db.Authenticatable
+        The user or node to create the tokens for.
+    api : Api
+        The api to create the urls for.
+    """
+    token_dict = {
+        'access_token': create_access_token(user_or_node),
+        'refresh_token': create_refresh_token(user_or_node),
+        'refresh_url': api.url_for(RefreshToken),
+    }
+    if isinstance(user_or_node, db.User):
+        token_dict['user_url'] = api.url_for(server.resource.user.User,
+                                             id=user_or_node.id)
+    else:
+        token_dict['node_url'] = api.url_for(server.resource.node.Node,
+                                             id=user_or_node.id)
+    return token_dict
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/role.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/role.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/rule.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,22 +139,32 @@
         # filter by any field of this endpoint
         for param in ['name', 'operation', 'scope']:
             if param in args:
                 q = q.filter(getattr(db.Rule, param) == args[param])
 
         # find roles containing a specific rule
         if 'role_id' in args:
+            role = db.Role.get(args['role_id'])
+            if not role:
+                return {
+                    'msg': f'Role with id={args["role_id"]} does not exist!'
+                }, HTTPStatus.BAD_REQUEST
             q = q.join(db.role_rule_association).join(db.Role)\
                  .filter(db.Role.id == args['role_id'])
 
         # find all rules of a specific user. This is done by first joining all
         # tables to find all rules originating from a user's roles. Then, we
         # do an outer join to find all rules that are directly assigned to the
         # user.
         if 'user_id' in args:
+            user = db.User.get(args['user_id'])
+            if not user:
+                return {
+                    'msg': f'User with id={args["user_id"]} does not exist!'
+                }, HTTPStatus.BAD_REQUEST
             q = q.join(db.role_rule_association).join(db.Role)\
                  .join(db.Permission).join(db.User)\
                  .outerjoin(db.UserPermission,
                             db.Rule.id == db.UserPermission.c.rule_id)\
                  .filter(or_(
                     db.User.id == args['user_id'],
                     db.UserPermission.c.user_id == args['user_id']
```

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/run.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 import logging
 from typing import Union
 import sqlalchemy as sa
 
 from flask import g, request
+from flask_restful import Api
 from http import HTTPStatus
 from sqlalchemy import desc
 
 from vantage6.common import logger_name
 from vantage6.server import db
 from vantage6.server.permission import (
     RuleCollection,
@@ -35,16 +36,27 @@
 )
 
 
 module_name = logger_name(__name__)
 log = logging.getLogger(module_name)
 
 
-def setup(api, api_base, services):
-
+def setup(api: Api, api_base: str, services: dict) -> None:
+    """
+    Setup the run resource.
+
+    Parameters
+    ----------
+    api : Api
+        Flask restful api instance
+    api_base : str
+        Base url of the api
+    services : dict
+        Dictionary with services required for the resource endpoints
+    """
     path = "/".join([api_base, module_name])
     log.info(f'Setting up "{path}" and subdirectories')
 
     api.add_resource(
         Runs,
         path,
         endpoint='run_without_id',
@@ -83,14 +95,22 @@
 run_input_schema = RunInputSchema()
 
 
 # -----------------------------------------------------------------------------
 # Permissions
 # -----------------------------------------------------------------------------
 def permissions(permissions: PermissionManager):
+    """
+    Define the permissions for this resource.
+    
+    Parameters
+    ----------
+    permissions : PermissionManager
+        Permission manager instance to which permissions are added
+    """
     add = permissions.appender(module_name)
 
     add(scope=S.GLOBAL, operation=P.VIEW, description="view any run")
     add(scope=S.COLLABORATION, operation=P.VIEW, assign_to_container=True,
         assign_to_node=True, description="view runs of your organizations "
         "collaborations")
     add(scope=S.ORGANIZATION, operation=P.VIEW,
@@ -99,15 +119,15 @@
         description="view any run of a task created by you")
 
 
 # ------------------------------------------------------------------------------
 # Resources / API's
 # ------------------------------------------------------------------------------
 class RunBase(ServicesResources):
-
+    """Base class for run resources"""
     def __init__(self, socketio, mail, api, permissions, config):
         super().__init__(socketio, mail, api, permissions, config)
         self.r: RuleCollection = getattr(self.permissions, module_name)
 
 
 class MultiRunBase(RunBase):
     """Base class for resources that return multiple runs or results"""
@@ -199,15 +219,15 @@
         # query the DB and paginate
         q = q.order_by(desc(db_Run.id))
         return q
 
 
 class Runs(MultiRunBase):
 
-    @only_for(['node', 'user', 'container'])
+    @only_for(('node', 'user', 'container'))
     def get(self):
         """ Returns a list of runs
         ---
 
         description: >-
             Returns a list of all runs you are allowed to see.\n
 
@@ -285,56 +305,66 @@
               schema:
                 type: integer
               description: Port number
             - in: query
               name: include
               schema:
                 type: string (can be multiple)
-              description: Include 'task' to include task data. Include
-                'metadata' to get pagination metadata. Note that this will put
-                the actual data in an envelope.
+              description: Include 'task' to include task data.
             - in: query
               name: page
               schema:
                 type: integer
-              description: Page number for pagination
+              description: Page number for pagination (default 1)
             - in: query
               name: per_page
               schema:
                 type: integer
-              description: Number of items per page
+              description: Number of items per page (default 10)
+            - in: query
+              name: sort
+              schema:
+                type: string
+              description: >-
+                Sort by one or more fields, separated by a comma. Use a minus
+                sign (-) in front of the field to sort in descending order.
 
         responses:
-            200:
-                description: Ok
-            401:
-                description: Unauthorized
-
+          200:
+            description: Ok
+          401:
+            description: Unauthorized
+          400:
+            description: Improper values for pagination or sorting parameters
+                
         security:
         - bearerAuth: []
 
         tags: ["Algorithm"]
         """
         query = self.get_query_multiple_runs()
 
         # If no query is returned, we should return message and error code
         if not isinstance(query, sa.orm.query.Query):
             return query
 
-        page = Pagination.from_query(query=query, request=request)
+        try:
+            page = Pagination.from_query(query=query, request=request)
+        except ValueError as e:
+            return {'msg': str(e)}, HTTPStatus.BAD_REQUEST
 
         # serialization of the models
         s = run_inc_schema if self.is_included('task') else run_schema
 
         return self.response(page, s)
 
 
 class Results(MultiRunBase):
 
-    @only_for(['node', 'user', 'container'])
+    @only_for(('node', 'user', 'container'))
     def get(self):
         """ Returns a list of results
         ---
 
         description: >-
             Returns a list of all results you are allowed to see.\n
 
@@ -482,15 +512,15 @@
                     HTTPStatus.UNAUTHORIZED
         return run
 
 
 class Run(SingleRunBase):
     """Resource for /api/run"""
 
-    @only_for(['node', 'user', 'container'])
+    @only_for(('node', 'user', 'container'))
     def get(self, id):
         """ Get a single run's data
         ---
 
         description: >-
             Returns a run from a task specified by an id. \n
```

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/stats.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/stats.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/task.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import json
 
 from flask import g, request, url_for
 from flask_restful import Api
 from http import HTTPStatus
 from sqlalchemy import desc
+from sqlalchemy.sql import visitors
 
 from vantage6.common.globals import STRING_ENCODING
 from vantage6.common.task_status import TaskStatus, has_task_finished
 from vantage6.server import db
 from vantage6.server.permission import (
     RuleCollection,
     Scope as S,
@@ -290,81 +291,95 @@
                 return {
                     'msg': 'You cannot view the results of all tasks, as you '
                     f'are allowed to view tasks with scope {max_scope_task} '
                     f'but you can only view results with scope {max_scope_run}'
                 }, HTTPStatus.UNAUTHORIZED
 
         if 'collaboration_id' in args:
-            if not self.r.can_for_col(P.VIEW, args['collaboration_id']):
+            collaboration_id = int(args['collaboration_id'])
+            if not self.r.can_for_col(P.VIEW, collaboration_id):
                 return {'msg': 'You lack the permission to view tasks '
-                        f'from collaboration {args["collaboration_id"]}!'}, \
+                        f'from collaboration {collaboration_id}!'}, \
                     HTTPStatus.UNAUTHORIZED
-            q = q.join(db.Collaboration).filter(
-                db.Collaboration.id == args['collaboration_id'])
+            # dont join collaboration table if it is already joined
+            # FIXME refactor this after moving to SQLAlchemy 2.0
+            has_already_joined_collab = False
+            for visitor in visitors.iterate(q.statement):
+                if visitor.__visit_name__ == 'table' and \
+                        visitor.name == 'collaboration':
+                    has_already_joined_collab = True
+            if not has_already_joined_collab:
+                q = q.join(db.Collaboration)
+            q = q.filter(db.Collaboration.id == collaboration_id)
 
         if 'init_org_id' in args:
-            if not self.r.can_for_org(P.VIEW, args['init_org_id']):
+            init_org_id = int(args['init_org_id'])
+            if not self.r.can_for_org(P.VIEW, init_org_id):
                 return {'msg': 'You lack the permission to view tasks '
-                        f'from organization id={args["init_org_id"]}!'}, \
+                        f'from organization id={init_org_id}!'}, \
                     HTTPStatus.UNAUTHORIZED
-            q = q.filter(db.Task.init_org_id == args['init_org_id'])
+            q = q.filter(db.Task.init_org_id == init_org_id)
 
         if 'init_user_id' in args:
-            init_user = db.User.get(args['init_user_id'])
+            init_user_id = int(args['init_user_id'])
+            init_user = db.User.get(init_user_id)
             if not init_user:
-                return {'msg': f'User id={args["init_user_id"]} does not '
+                return {'msg': f'User id={init_user_id} does not '
                         'exist!'}, HTTPStatus.BAD_REQUEST
             elif not self.r.can_for_org(P.VIEW, init_user.organization_id) \
                     and not (self.r.v_own.can() and g.user and
                              init_user.id == g.user.id):
                 return {'msg': 'You lack the permission to view tasks '
-                        f'from user id={args["init_user_id"]}!'}, \
+                        f'from user id={init_user_id}!'}, \
                     HTTPStatus.UNAUTHORIZED
-            q = q.filter(db.Task.init_user_id == args['init_user_id'])
+            q = q.filter(db.Task.init_user_id == init_user_id)
 
         if 'parent_id' in args:
-            parent = db.Task.get(args['parent_id'])
+            parent_id = int(args['parent_id'])
+            parent = db.Task.get(parent_id)
             if not parent:
                 return {'msg': f'Parent task id={args["parent_id"]} does not '
                         'exist!'}, HTTPStatus.BAD_REQUEST
             elif not self.r.can_for_col(P.VIEW, parent.collaboration_id):
                 return {'msg': 'You lack the permission to view tasks '
                         'from the collaboration that the task with parent_id='
                         f'{parent.collaboration_id} belongs to!'}, \
                     HTTPStatus.UNAUTHORIZED
-            q = q.filter(db.Task.parent_id == args['parent_id'])
+            q = q.filter(db.Task.parent_id == int(parent_id))
 
         if 'job_id' in args:
+            job_id = int(args['job_id'])
             task_in_job = q.session.query(db.Task).filter(
-                db.Task.job_id == args['job_id']).first()
+                db.Task.job_id == job_id).first()
             if not task_in_job:
                 return {'msg': f'Job id={args["job_id"]} does not exist!'}, \
                     HTTPStatus.BAD_REQUEST
             elif not self.r.can_for_col(P.VIEW, task_in_job.collaboration_id):
                 return {'msg': 'You lack the permission to view tasks '
                         'from the collaboration that the task with job_id='
                         f'{task_in_job.collaboration_id} belongs to!'}, \
                     HTTPStatus.UNAUTHORIZED
-            q = q.filter(db.Task.job_id == args['job_id'])
+            q = q.filter(db.Task.job_id == job_id)
 
         for param in ['name', 'image', 'description', 'status']:
             if param in args:
                 q = q.filter(getattr(db.Task, param).like(args[param]))
 
         if 'run_id' in args:
-            run = db.Run.get(args['run_id'])
+            run_id = int(args['run_id'])
+            run = db.Run.get(run_id)
             if not run:
                 return {'msg': f'Run id={args["run_id"]} does not exist!'}, \
                     HTTPStatus.BAD_REQUEST
             elif not self.r.can_for_col(P.VIEW, run.collaboration_id):
                 return {'msg': 'You lack the permission to view tasks '
                         'from the collaboration that the run with id='
                         f'{run.collaboration_id} belongs to!'}, \
                     HTTPStatus.UNAUTHORIZED
-            q = q.join(db.Run).filter(db.Run.id == args['run_id'])
+            q = q.join(db.Run).filter(db.Run.id == run_id)
 
         if 'database' in args:
             q = q.join(db.TaskDatabase)\
                  .filter(db.TaskDatabase.database == args['database'])
 
         if 'is_user_created' in args:
             try:
@@ -616,15 +631,15 @@
         # add some logging
         log.info(f"New task for collaboration '{task.collaboration.name}'")
         if g.user:
             log.debug(f" created by: '{g.user.username}'")
         else:
             log.debug(f" created by container on node_id="
                       f"{g.container['node_id']}"
-                      f" for (master) task_id={g.container['task_id']}")
+                      f" for (parent) task_id={g.container['task_id']}")
 
         log.debug(f" url: '{url_for('task_with_id', id=task.id)}'")
         log.debug(f" name: '{task.name}'")
         log.debug(f" image: '{task.image}'")
 
         return task_schema.dump(task, many=False), HTTPStatus.CREATED
 
@@ -637,15 +652,15 @@
         if not image.endswith(container["image"]):
             log.warning((f"Container from node={container['node_id']} "
                         f"attempts to post a task using illegal image!?"))
             log.warning(f"  task image: {image}")
             log.warning(f"  container image: {container['image']}")
             return False
 
-        # check master task is not completed yet
+        # check that parent task is not completed yet
         if has_task_finished(db.Task.get(container["task_id"]).status):
             log.warning(
                 f"Container from node={container['node_id']} "
                 f"attempts to start sub-task for a completed "
                 f"task={container['task_id']}"
             )
             return False
```

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/user.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 from vantage6.server.resource import (
     get_org_ids_from_collabs,
     with_user,
     ServicesResources
 )
 from vantage6.server.resource.common.input_schema import UserInputSchema
 from vantage6.server.resource.common.pagination import Pagination
-from vantage6.server.resource.common.output_schema import UserSchema
+from vantage6.server.resource.common.output_schema import (
+    UserSchema, UserWithPermissionDetailsSchema
+)
 
 
 module_name = logger_name(__name__)
 log = logging.getLogger(module_name)
 
 
 def setup(api: Api, api_base: str, services: dict) -> None:
@@ -103,15 +105,15 @@
 
 
 # ------------------------------------------------------------------------------
 # Resources / API's
 # ------------------------------------------------------------------------------
 user_schema = UserSchema()
 user_input_schema = UserInputSchema()
-
+user_schema_with_permissions = UserWithPermissionDetailsSchema()
 
 class UserBase(ServicesResources):
 
     def __init__(self, socketio, mail, api, permissions, config):
         super().__init__(socketio, mail, api, permissions, config)
         self.r: RuleCollection = getattr(self.permissions, module_name)
 
@@ -256,15 +258,18 @@
         # find users with a particulare role or rule assigned
         if 'role_id' in args:
             role = db.Role.get(args['role_id'])
             if not role:
                 return {
                     'msg': f'Role with id={args["role_id"]} does not exist!'
                 }, HTTPStatus.BAD_REQUEST
-            elif not self.r.can_for_org(P.VIEW, role.organization_id):
+            # note: We check if role has organization to ensure that users
+            # with limited permissions can still see who have default roles
+            elif not self.r.can_for_org(P.VIEW, role.organization_id) and \
+                    role.organization:
                 return {
                     'msg': 'You lack the permission view users from the '
                     f'organization that role with id={role.organization_id} '
                     'belongs to!'
                 }, HTTPStatus.UNAUTHORIZED
             q = q.join(db.Permission).join(db.Role)\
                  .filter(db.Role.id == args['role_id'])
@@ -491,14 +496,20 @@
         parameters:
             - in: path
               name: id
               schema:
                 type: integer
               description: User id
               required: true
+            - in: path
+              name: include_permissions
+              schema:
+                type: boolean
+              description: Whether or not to include extra permission info for
+                the user. By default false.
 
         responses:
             200:
                 description: Ok
             404:
                 description: User not found
             401:
@@ -509,21 +520,25 @@
 
         tags: ["User"]
         """
         user = db.User.get(id)
         if not user:
             return {"msg": f"user id={id} is not found"}, HTTPStatus.NOT_FOUND
 
-        same_user = g.user.id == user.id
+        schema = user_schema
+
+        if request.args.get('include_permissions', False):
+              schema = user_schema_with_permissions
 
         # allow user to be returned if authenticated user can view users from
         # that organization or if the user is the same as the authenticated
         # user.
+        same_user = g.user.id == user.id
         if (same_user or self.r.can_for_org(P.VIEW, user.organization_id)):
-            return user_schema.dump(user, many=False), HTTPStatus.OK
+            return schema.dump(user, many=False), HTTPStatus.OK
         else:
             return {'msg': 'You lack the permission to do that!'}, \
                     HTTPStatus.UNAUTHORIZED
 
     @with_user
     def patch(self, id):
         """Update user
```

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/version.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/version.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/vpn.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/vpn.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/resource/websocket_test.py` & `vantage6-server-4.0.0a5/vantage6/server/resource/websocket_test.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/utils.py` & `vantage6-server-4.0.0a5/vantage6/server/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a4/vantage6/server/websockets.py` & `vantage6-server-4.0.0a5/vantage6/server/websockets.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,24 +216,26 @@
 
         Parameters
         ----------
         data: Dict
             Dictionary containing parameters on the updated algorithm status.
             It should look as follows:
 
-            {
-                # node_id where algorithm container was running
-                "node_id": 1,
-                # new status of algorithm container
-                "status": "active",
-                # result_id for which the algorithm was running
-                "result_id": 1,
-                # collaboration_id for which the algorithm was running
-                "collaboration_id": 1
-            }
+            .. code:: python
+
+                {
+                    # node_id where algorithm container was running
+                    "node_id": 1,
+                    # new status of algorithm container
+                    "status": "active",
+                    # result_id for which the algorithm was running
+                    "result_id": 1,
+                    # collaboration_id for which the algorithm was running
+                    "collaboration_id": 1
+                }
         """
         # only allow nodes to send this event
         if session.type != 'node':
             self.log.warn('Only nodes can send algorithm status changes! '
                           f'{session.type} {session.auth_id} is not allowed.')
             return
```

### Comparing `vantage6-server-4.0.0a4/vantage6_server.egg-info/PKG-INFO` & `vantage6-server-4.0.0a5/vantage6_server.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vantage6-server
-Version: 4.0.0a4
+Version: 4.0.0a5
 Summary: Vantage6 server
 Home-page: https://github.com/vantage6/vantage6
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
   <br>
   <a href="https://vantage6.ai"><img src="https://github.com/IKNL/guidelines/blob/master/resources/logos/vantage6.png?raw=true" alt="vantage6" width="350"></a>
 </h1>
@@ -32,20 +32,22 @@
 
 
 
 -----------------------------------------------------------------------------------------------------
 This repository is part of **vantage6**, our **privacy preserving federated learning infrastructure for secure insight exchange**, and contains all the **vantage6** infrastructure source/ code. Please visit our [website (vantage6.ai)](https://vantage6.ai) to learn more!
 
 ## :books: Documentation
-This repository is home to 4 PyPi packages:
+This repository is home to 6 PyPi packages:
 
 * [vantage6](https://pypi.org/project/vantage6) -> _CLI for managing node and server instances_
 * [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client for interacting with the vantage6-server_
+* [vantage6-algorithm-tools](https://pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate algorithm development_
 * [vantage6-node](https://pypi.org/project/vantage6-node) -> _Node application package_
 * [vantage6-server](https://pypi.org/project/vantage6-server) -> _Server application package_
+* [vantage6-common](https://pypi.org/project/vantage6-common) -> _Server application package_
 
 **Note that when using vantage6 you do not install the _server_ and _node_ packages. These are delivered to you in Docker images.**
 
 Two docker images are published which contain the Node and Server applications:
 
 * `harbor2.vantage6.ai/infrastructure/node:VERSION`
 * `harbor2.vantage6.ai/infrastructure/server:VERSION`
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: vantage6-server Version: 4.0.0a4 Summary: Vantage6
-server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
+Metadata-Version: 2.1 Name: vantage6-server Version: 4.0.0a5 Summary: Vantage6
+server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml) [![PyPI vantage6](https://badge.fury.io/py/vantage6.svg)](https://
@@ -19,32 +19,35 @@
    10.5281/zenodo.7382602.svg)](https://doi.org/10.5281/zenodo.7382602) ****
                  Documentation â¢ Contributing â¢ References
 -------------------------------------------------------------------------------
 ---------------------- This repository is part of **vantage6**, our **privacy
 preserving federated learning infrastructure for secure insight exchange**, and
 contains all the **vantage6** infrastructure source/ code. Please visit our
 [website (vantage6.ai)](https://vantage6.ai) to learn more! ## :books:
-Documentation This repository is home to 4 PyPi packages: * [vantage6](https://
+Documentation This repository is home to 6 PyPi packages: * [vantage6](https://
 pypi.org/project/vantage6) -> _CLI for managing node and server instances_ *
 [vantage6-client](https://pypi.org/project/vantage6-client) -> _Python client
-for interacting with the vantage6-server_ * [vantage6-node](https://pypi.org/
-project/vantage6-node) -> _Node application package_ * [vantage6-server](https:
-//pypi.org/project/vantage6-server) -> _Server application package_ **Note that
-when using vantage6 you do not install the _server_ and _node_ packages. These
-are delivered to you in Docker images.** Two docker images are published which
-contain the Node and Server applications: * `harbor2.vantage6.ai/
-infrastructure/node:VERSION` * `harbor2.vantage6.ai/infrastructure/server:
-VERSION` These docker images are used by the _vantage6 CLI_ package, which can
-be installed by running: `pip install vantage6` This will install the CLI which
-enables you to use the commands: * `vnode CMD [OPTIONS]` * `vserver CMD
-[OPTIONS]` You can find more (user) documentation at [Gitbook
-(docs.vantage6.ai)](https://docs.vantage6.ai). If you have any questions,
-suggestions or just want to chat about federated learning: join our [Dircord
-(https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel. ## :
-gift_heart: Contributing We hope to continue developing, improving, and
+for interacting with the vantage6-server_ * [vantage6-algorithm-tools](https://
+pypi.org/project/vantage6-algorithm-tools) -> _Python tools to facilitate
+algorithm development_ * [vantage6-node](https://pypi.org/project/vantage6-
+node) -> _Node application package_ * [vantage6-server](https://pypi.org/
+project/vantage6-server) -> _Server application package_ * [vantage6-common]
+(https://pypi.org/project/vantage6-common) -> _Server application package_
+**Note that when using vantage6 you do not install the _server_ and _node_
+packages. These are delivered to you in Docker images.** Two docker images are
+published which contain the Node and Server applications: *
+`harbor2.vantage6.ai/infrastructure/node:VERSION` * `harbor2.vantage6.ai/
+infrastructure/server:VERSION` These docker images are used by the _vantage6
+CLI_ package, which can be installed by running: `pip install vantage6` This
+will install the CLI which enables you to use the commands: * `vnode CMD
+[OPTIONS]` * `vserver CMD [OPTIONS]` You can find more (user) documentation at
+[Gitbook (docs.vantage6.ai)](https://docs.vantage6.ai). If you have any
+questions, suggestions or just want to chat about federated learning: join our
+[Dircord (https://discord.gg/yAyFf6Y)](https://discord.gg/yAyFf6Y) channel. ##
+:gift_heart: Contributing We hope to continue developing, improving, and
 supporting **vantage6** with the help of the federated learning community. If
 you are interested in contributing, first of all, thank you! Second, please
 take a look at our [contributing guidelines](https://docs.vantage6.ai/en/main/
 devops/contribute.html) ## :black_nib: References If you are using
 **vantage6**, please cite this repository as well as the accompanying papers as
 follows: > * F. Martin, M. Sieswerda, H. Alradhi, et al. vantage6. Available at
 https://doi.org/10.5281/zenodo.7221216. Accessed on MONTH, 20XX. > * A.
```

### Comparing `vantage6-server-4.0.0a4/vantage6_server.egg-info/SOURCES.txt` & `vantage6-server-4.0.0a5/vantage6_server.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 vantage6/server/resource/collaboration.py
 vantage6/server/resource/event.py
 vantage6/server/resource/health.py
 vantage6/server/resource/node.py
 vantage6/server/resource/organization.py
 vantage6/server/resource/port.py
 vantage6/server/resource/recover.py
-vantage6/server/resource/result.py
 vantage6/server/resource/role.py
 vantage6/server/resource/rule.py
 vantage6/server/resource/run.py
 vantage6/server/resource/stats.py
 vantage6/server/resource/task.py
 vantage6/server/resource/token.py
 vantage6/server/resource/user.py
```

