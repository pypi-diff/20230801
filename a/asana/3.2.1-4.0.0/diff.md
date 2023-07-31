# Comparing `tmp/asana-3.2.1.tar.gz` & `tmp/asana-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/python-asana/python-asana/dist/.tmp-tepx3kjb/asana-3.2.1.tar", last modified: Thu Apr 13 16:54:49 2023, max compression
+gzip compressed data, was "/home/runner/work/python-asana/python-asana/dist/.tmp-_jv5cclr/asana-4.0.0.tar", last modified: Mon Jul 31 23:40:33 2023, max compression
```

## Comparing `asana-3.2.1.tar` & `asana-4.0.0.tar`

### file list

```diff
@@ -1,115 +1,917 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:54:49.000000 asana-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:54:39.000000 asana-3.2.1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:54:39.000000 asana-3.2.1/CONTRIBUTORS
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-13 16:54:39.000000 asana-3.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 16:54:39.000000 asana-3.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-04-13 16:54:49.000000 asana-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-04-13 16:54:39.000000 asana-3.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:54:49.000000 asana-3.2.1/asana/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-13 16:54:39.000000 asana-3.2.1/asana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-04-13 16:54:39.000000 asana-3.2.1/asana/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-13 16:54:39.000000 asana-3.2.1/asana/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-04-13 16:54:39.000000 asana-3.2.1/asana/page_iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:54:49.000000 asana-3.2.1/asana/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/audit_log_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/batch_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/custom_field_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:54:49.000000 asana-3.2.1/asana/resources/gen/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/audit_log_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/batch_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/custom_field_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12487 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/goal_relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)    14536 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/goals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/organization_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/portfolio_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)    16355 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/project_briefs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/project_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/project_statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/project_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    27462 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/status_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/stories.py
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    43387 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/team_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/time_periods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/typeahead.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/user_task_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/workspace_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/goal_relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/goals.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/organization_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/portfolio_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/project_briefs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/project_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/project_statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/project_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/status_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/stories.py
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    20218 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/team_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/time_periods.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/typeahead.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/user_task_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/workspace_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-13 16:54:39.000000 asana-3.2.1/asana/session.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 16:54:39.000000 asana-3.2.1/asana/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:54:49.000000 asana-3.2.1/asana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-04-13 16:54:49.000000 asana-3.2.1/asana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-13 16:54:49.000000 asana-3.2.1/asana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:54:49.000000 asana-3.2.1/asana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 16:54:49.000000 asana-3.2.1/asana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 16:54:49.000000 asana-3.2.1/asana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:54:49.000000 asana-3.2.1/asana.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 16:54:49.000000 asana-3.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1321 2023-04-13 16:54:39.000000 asana-3.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:54:49.000000 asana-3.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18990 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_audit_log_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_custom_field_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_organization_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_portfolio_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_stories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_user_task_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:40:33.000000 asana-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-31 23:40:21.000000 asana-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    62194 2023-07-31 23:40:33.000000 asana-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    61965 2023-07-31 23:40:21.000000 asana-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:40:33.000000 asana-4.0.0/asana/
+-rw-r--r--   0 runner    (1001) docker     (123)    32590 2023-07-31 23:40:21.000000 asana-4.0.0/asana/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:40:33.000000 asana-4.0.0/asana/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23638 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/audit_log_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/batch_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/custom_field_settings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45237 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/custom_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28584 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/goal_relationships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52939 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/goals_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14709 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/organization_exports_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/portfolio_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63742 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/portfolios_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20925 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/project_briefs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/project_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21905 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/project_statuses_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28285 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/project_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106576 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/rules_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35829 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/sections_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/status_updates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26060 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/stories_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42172 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   163533 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24345 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/team_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37627 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/time_periods_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28122 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/time_tracking_entries_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/typeahead_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/user_task_lists_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30129 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29476 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18363 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/workspace_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27455 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api/workspaces_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25558 2023-07-31 23:40:21.000000 asana-4.0.0/asana/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-07-31 23:40:21.000000 asana-4.0.0/asana/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:40:33.000000 asana-4.0.0/asana/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    30621 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/add_custom_field_setting_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/add_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/add_members_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/all_of_project_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/all_of_project_template_base_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/all_of_project_template_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/all_of_story_response_new_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/all_of_story_response_old_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/all_of_user_task_list_base_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/all_of_user_task_list_base_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/all_of_user_task_list_compact_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/all_of_user_task_list_compact_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/all_of_user_task_list_request_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/all_of_user_task_list_request_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/all_of_user_task_list_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/all_of_user_task_list_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/all_of_workspace_membership_response_user_task_list_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/all_of_workspace_membership_response_user_task_list_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/asana_named_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/asana_named_resource_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/asana_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/attachment_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/attachment_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/attachment_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14064 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/attachment_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/attachment_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/attachment_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/audit_log_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/audit_log_event_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/audit_log_event_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/audit_log_event_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/audit_log_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/audit_log_event_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/batch_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/batch_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/batch_request_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/batch_request_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/batch_request_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/batch_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/create_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/create_time_tracking_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30420 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_field_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_field_base_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_field_base_enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_field_base_enum_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_field_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_field_gid_enum_options_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_field_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33924 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_field_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_field_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_field_response_created_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_field_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_field_response_people_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_field_setting_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_field_setting_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_field_setting_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_field_setting_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35868 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_field_setting_response_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_field_setting_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_field_setting_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_field_setting_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_fields_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/custom_fields_custom_field_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/date_variable_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/date_variable_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/empty_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/empty_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/enum_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/enum_option_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/enum_option_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/enum_option_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/enum_option_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/enum_options_enum_option_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/enum_options_insert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/error_response_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/event_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/event_response_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/event_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/event_response_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/event_response_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_add_subgoal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_add_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_add_supporting_work_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_gid_add_supporting_relationship_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_gid_remove_supporting_relationship_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_gid_set_metric_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_gid_set_metric_current_value_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_membership_base_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_metric_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_metric_current_value_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_metric_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_relationship_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_relationship_base_supported_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_relationship_base_supporting_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_relationship_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_relationship_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_relationship_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_relationship_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_relationships_goal_relationship_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_remove_subgoal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_remove_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_request_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18927 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_response_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_response_likes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_response_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_response_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_response_time_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goal_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goals_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/goals_goal_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/inline_response412.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/inline_response412_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/job_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/job_base_new_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/job_base_new_project_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/job_base_new_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/job_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/job_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/like.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/member_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/memberships_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/modify_dependencies_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/modify_dependents_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/next_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/organization_export_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/organization_export_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/organization_export_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/organization_export_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/organization_export_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/organization_exports_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_add_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_gid_add_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_gid_add_item_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_gid_add_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_gid_remove_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_gid_remove_item_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_gid_remove_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_membership_base_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_remove_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_response_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_response_custom_field_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17399 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_response_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolio_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolios_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/portfolios_portfolio_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20495 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_base_current_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_base_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_base_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_brief_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_brief_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_brief_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_brief_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_brief_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_brief_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_briefs_project_brief_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_duplicate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_duplicate_request_schedule_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_gid_add_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_gid_add_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_gid_duplicate_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_gid_project_briefs_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_gid_project_statuses_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_gid_remove_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_gid_remove_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_gid_save_as_template_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_gid_sections_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_membership_response_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24286 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31095 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_response_completed_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_response_created_from_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_response_project_brief.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_response_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_save_as_template_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_section_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_status_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_status_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_status_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_status_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_template_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_template_base_requested_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_template_base_requested_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_template_base_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_template_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_template_gid_instantiate_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_template_instantiate_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_template_instantiate_project_request_requested_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_template_instantiate_project_request_requested_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_template_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_template_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/project_template_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/projects_project_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/remove_custom_field_setting_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/remove_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/remove_members_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/requested_role_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/rule_trigger_gid_run_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/rule_trigger_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/rule_trigger_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/rule_trigger_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/section_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/section_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/section_gid_add_task_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/section_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/section_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/section_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/section_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/section_task_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/sections_insert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/sections_section_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/status_update_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/status_update_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/status_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/status_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/status_update_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/status_update_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/status_update_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/status_updates_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/stories_story_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/story_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/story_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/story_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48927 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/story_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/story_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/story_response_assignee.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17099 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/story_response_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/story_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/story_response_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/story_response_old_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/story_response_old_enum_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/story_response_old_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/story_response_previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/story_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/story_response_story.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/story_response_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/story_response_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/story_response_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/tag_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/tag_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/tag_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/tag_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_add_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_add_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_add_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35097 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_base_completed_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_base_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_base_external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_base_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_base_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_count_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_duplicate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_gid_add_dependencies_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_gid_add_dependents_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_gid_add_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_gid_add_tag_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_gid_duplicate_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_gid_remove_dependencies_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_gid_remove_dependents_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_gid_remove_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_gid_remove_tag_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_gid_set_parent_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_gid_stories_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_gid_subtasks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_gid_time_tracking_entries_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_remove_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_remove_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_remove_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43510 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44565 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_response_assignee_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34464 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_response_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_response_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/task_set_parent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/tasks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/tasks_task_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/team_add_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/team_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/team_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/team_gid_add_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/team_gid_projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/team_gid_remove_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/team_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/team_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/team_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/team_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/team_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/team_remove_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19673 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/team_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/team_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/team_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/team_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/team_response_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/teams_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/teams_team_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/template_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/time_period_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/time_period_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/time_period_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/time_period_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/time_period_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/time_tracking_entries_time_tracking_entry_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/time_tracking_entry_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/time_tracking_entry_base_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/time_tracking_entry_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/time_tracking_entry_compact_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/update_time_tracking_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/user_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/user_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/user_base_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/user_base_response_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/user_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/user_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/user_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/user_task_list_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/user_task_list_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/user_task_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/user_task_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/user_task_list_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/webhook_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/webhook_compact_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/webhook_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/webhook_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/webhook_request_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/webhook_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/webhook_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/webhook_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/webhooks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/webhooks_webhook_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/workspace_add_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/workspace_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/workspace_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/workspace_gid_add_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/workspace_gid_projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/workspace_gid_remove_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/workspace_gid_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/workspace_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/workspace_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/workspace_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/workspace_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/workspace_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/workspace_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/workspace_membership_response_user_task_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/workspace_membership_response_vacation_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/workspace_remove_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/workspace_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/workspace_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-31 23:40:21.000000 asana-4.0.0/asana/models/workspaces_workspace_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-07-31 23:40:21.000000 asana-4.0.0/asana/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:40:33.000000 asana-4.0.0/asana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    62194 2023-07-31 23:40:33.000000 asana-4.0.0/asana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35232 2023-07-31 23:40:33.000000 asana-4.0.0/asana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 23:40:33.000000 asana-4.0.0/asana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-31 23:40:33.000000 asana-4.0.0/asana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-31 23:40:33.000000 asana-4.0.0/asana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 23:40:33.000000 asana-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-31 23:40:21.000000 asana-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:40:33.000000 asana-4.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 23:40:21.000000 asana-4.0.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_add_custom_field_setting_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_add_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_add_members_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_all_of_project_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_all_of_project_template_base_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_all_of_project_template_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_all_of_story_response_new_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_all_of_story_response_old_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_all_of_user_task_list_base_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_all_of_user_task_list_base_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_all_of_user_task_list_compact_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_all_of_user_task_list_compact_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_all_of_user_task_list_request_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_all_of_user_task_list_request_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_all_of_user_task_list_response_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_all_of_user_task_list_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_all_of_workspace_membership_response_user_task_list_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_all_of_workspace_membership_response_user_task_list_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_asana_named_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_asana_named_resource_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_asana_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_attachment_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_attachment_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_attachment_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_attachment_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_attachment_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_attachment_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_audit_log_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_audit_log_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_audit_log_event_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_audit_log_event_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_audit_log_event_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_audit_log_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_audit_log_event_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_batch_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_batch_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_batch_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_batch_request_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_batch_request_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_batch_request_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_batch_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_create_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_create_time_tracking_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_field_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_field_base_date_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_field_base_enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_field_base_enum_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_field_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_field_gid_enum_options_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_field_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_field_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_field_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_field_response_created_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_field_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_field_response_people_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_field_setting_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_field_setting_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_field_setting_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_field_setting_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_field_setting_response_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_field_setting_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_field_setting_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_field_setting_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_field_settings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_fields_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_custom_fields_custom_field_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_date_variable_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_date_variable_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_empty_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_empty_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_enum_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_enum_option_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_enum_option_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_enum_option_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_enum_option_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_enum_options_enum_option_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_enum_options_insert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_error_response_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_event_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_event_response_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_event_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_event_response_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_event_response_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_add_subgoal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_add_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_add_supporting_work_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_gid_add_supporting_relationship_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_gid_remove_supporting_relationship_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_gid_set_metric_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_gid_set_metric_current_value_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_membership_base_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_metric_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_metric_current_value_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_metric_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_relationship_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_relationship_base_supported_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_relationship_base_supporting_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_relationship_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_relationship_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_relationship_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_relationship_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_relationships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_relationships_goal_relationship_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_remove_subgoal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_remove_supporting_relationship_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_request_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_response_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_response_likes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_response_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_response_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_response_time_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goal_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goals_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goals_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_goals_goal_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_inline_response412.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_inline_response412_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_job_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_job_base_new_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_job_base_new_project_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_job_base_new_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_job_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_job_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_member_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_memberships_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_modify_dependencies_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_modify_dependents_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_next_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_organization_export_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_organization_export_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_organization_export_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_organization_export_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_organization_export_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_organization_exports_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_organization_exports_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_add_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_gid_add_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_gid_add_item_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_gid_add_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_gid_remove_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_gid_remove_item_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_gid_remove_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_membership_base_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_remove_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_response_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_response_custom_field_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_response_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolio_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolios_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolios_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_portfolios_portfolio_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_base_current_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_base_current_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_base_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_brief_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_brief_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_brief_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_brief_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_brief_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_brief_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_briefs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_briefs_project_brief_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_duplicate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_duplicate_request_schedule_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_gid_add_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_gid_add_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_gid_duplicate_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_gid_project_briefs_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_gid_project_statuses_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_gid_remove_custom_field_setting_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_gid_remove_members_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_gid_save_as_template_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_gid_sections_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_membership_response_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_response_completed_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_response_created_from_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_response_project_brief.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_response_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_save_as_template_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_section_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_status_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_status_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_status_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_status_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_statuses_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_template_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_template_base_requested_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_template_base_requested_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_template_base_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_template_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_template_gid_instantiate_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_template_instantiate_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_template_instantiate_project_request_requested_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_template_instantiate_project_request_requested_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_template_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_template_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_template_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_project_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_projects_project_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_remove_custom_field_setting_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_remove_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_remove_members_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_requested_role_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_rule_trigger_gid_run_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_rule_trigger_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_rule_trigger_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_rule_trigger_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_rules_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_section_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_section_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_section_gid_add_task_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_section_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_section_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_section_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_section_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_section_task_insert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_sections_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_sections_insert_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_sections_section_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_status_update_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_status_update_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_status_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_status_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_status_update_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_status_update_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_status_update_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_status_updates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_status_updates_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_stories_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_stories_story_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_story_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_story_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_story_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_story_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_story_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_story_response_assignee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_story_response_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_story_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_story_response_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_story_response_old_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_story_response_old_enum_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_story_response_old_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_story_response_previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_story_response_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_story_response_story.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_story_response_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_story_response_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_story_response_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_tag_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_tag_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_tag_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_tag_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_task_add_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_task_add_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_task_add_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_task_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_task_base_completed_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_task_base_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_task_base_external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_task_base_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_task_base_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_task_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_task_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_task_count_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_task_duplicate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_task_gid_add_dependencies_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-31 23:40:21.000000 asana-4.0.0/test/test_task_gid_add_dependents_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_gid_add_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_gid_add_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_gid_add_tag_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_gid_duplicate_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_gid_remove_dependencies_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_gid_remove_dependents_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_gid_remove_followers_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_gid_remove_project_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_gid_remove_tag_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_gid_set_parent_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_gid_stories_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_gid_subtasks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_gid_time_tracking_entries_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_remove_followers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_remove_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_remove_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_response_assignee_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_response_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_response_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_response_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_response_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_task_set_parent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_tasks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_tasks_task_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_team_add_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_team_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_team_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_team_gid_add_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_team_gid_projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_team_gid_remove_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_team_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_team_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_team_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_team_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_team_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_team_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_team_remove_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_team_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_team_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_team_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_team_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_team_response_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_teams_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_teams_team_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_template_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_time_period_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_time_period_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_time_period_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_time_period_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_time_period_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_time_periods_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_time_tracking_entries_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_time_tracking_entries_time_tracking_entry_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_time_tracking_entry_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_time_tracking_entry_base_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_time_tracking_entry_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_time_tracking_entry_compact_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_typeahead_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_update_time_tracking_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_user_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_user_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_user_base_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_user_base_response_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_user_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_user_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_user_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_user_task_list_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_user_task_list_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_user_task_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_user_task_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_user_task_list_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_user_task_lists_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_webhook_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_webhook_compact_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_webhook_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_webhook_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_webhook_request_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_webhook_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_webhook_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_webhook_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_webhooks_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_webhooks_webhook_gid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspace_add_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspace_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspace_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspace_gid_add_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspace_gid_projects_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspace_gid_remove_user_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspace_gid_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspace_membership_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspace_membership_compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspace_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspace_membership_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspace_membership_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspace_membership_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspace_membership_response_user_task_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspace_membership_response_vacation_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspace_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspace_remove_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspace_response_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspace_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspaces_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 23:40:22.000000 asana-4.0.0/test/test_workspaces_workspace_gid_body.py
```

### Comparing `asana-3.2.1/LICENSE` & `asana-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asana-3.2.1/asana/resources/sections.py` & `asana-4.0.0/asana/models/project_section_insert_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,119 +1,169 @@
-from .gen.sections import _Sections
+# coding: utf-8
 
+"""
+    Asana
 
-class Sections(_Sections):
-    """The :class:`Sections` object, which represents the resource of the same
-    name in Asana's API.
+    This is the interface for interacting with the [Asana Platform](https://developers.asana.com). Our API reference is generated from our [OpenAPI spec] (https://raw.githubusercontent.com/Asana/openapi/master/defs/asana_oas.yaml).  # noqa: E501
 
+    OpenAPI spec version: 1.0
+    
+    Generated by: https://github.com/swagger-api/swagger-codegen.git
+"""
+
+import pprint
+import re  # noqa: F401
+
+import six
+
+class ProjectSectionInsertRequest(object):
+    """NOTE: This class is auto generated by the swagger code generator program.
+
+    Do not edit the class manually.
+    """
     """
-    def create_in_project(self, project, params={}, **options):
-        """Creates a new section in a project.
+    Attributes:
+      swagger_types (dict): The key is attribute name
+                            and the value is attribute type.
+      attribute_map (dict): The key is attribute name
+                            and the value is json key in definition.
+    """
+    swagger_types = {
+        'section': 'str',
+        'before_section': 'str',
+        'after_section': 'str'
+    }
 
-        Returns the full record of the newly created section.
+    attribute_map = {
+        'section': 'section',
+        'before_section': 'before_section',
+        'after_section': 'after_section'
+    }
 
-        Parameters
-        ----------
-        project : {Gid} The project to create the section in
-        [data] : {Object} Data for the request
-          - name : {String} The text to be displayed as the section name. This cannot be an empty string.
-        """
-        path = "/projects/%s/sections" % (project)
-        return self.client.post(path, params, **options)
+    def __init__(self, section=None, before_section=None, after_section=None):  # noqa: E501
+        """ProjectSectionInsertRequest - a model defined in Swagger"""  # noqa: E501
+        self._section = None
+        self._before_section = None
+        self._after_section = None
+        self.discriminator = None
+        self.section = section
+        if before_section is not None:
+            self.before_section = before_section
+        if after_section is not None:
+            self.after_section = after_section
 
-    def find_by_project(self, project, params={}, **options):
-        """Returns the compact records for all sections in the specified project.
+    @property
+    def section(self):
+        """Gets the section of this ProjectSectionInsertRequest.  # noqa: E501
 
-        Parameters
-        ----------
-        project : {Gid} The project to get sections from.
-        [params] : {Object} Parameters for the request
+        The section to reorder.  # noqa: E501
+
+        :return: The section of this ProjectSectionInsertRequest.  # noqa: E501
+        :rtype: str
         """
-        path = "/projects/%s/sections" % (project)
-        return self.client.get_collection(path, params, **options)
+        return self._section
+
+    @section.setter
+    def section(self, section):
+        """Sets the section of this ProjectSectionInsertRequest.
 
-    def find_by_id(self, section, params={}, **options):
-        """Returns the complete record for a single section.
+        The section to reorder.  # noqa: E501
 
-        Parameters
-        ----------
-        section : {Gid} The section to get.
-        [params] : {Object} Parameters for the request
+        :param section: The section of this ProjectSectionInsertRequest.  # noqa: E501
+        :type: str
         """
-        path = "/sections/%s" % (section)
-        return self.client.get(path, params, **options)
+        if section is None:
+            raise ValueError("Invalid value for `section`, must not be `None`")  # noqa: E501
 
-    def update(self, section, params={}, **options):
-        """A specific, existing section can be updated by making a PUT request on
-        the URL for that project. Only the fields provided in the `data` block
-        will be updated; any unspecified fields will remain unchanged. (note that
-        at this time, the only field that can be updated is the `name` field.)
+        self._section = section
 
-        When using this method, it is best to specify only those fields you wish
-        to change, or else you may overwrite changes made by another user since
-        you last retrieved the task.
+    @property
+    def before_section(self):
+        """Gets the before_section of this ProjectSectionInsertRequest.  # noqa: E501
 
-        Returns the complete updated section record.
+        Insert the given section immediately before the section specified by this parameter.  # noqa: E501
 
-        Parameters
-        ----------
-        section : {Gid} The section to update.
-        [data] : {Object} Data for the request
+        :return: The before_section of this ProjectSectionInsertRequest.  # noqa: E501
+        :rtype: str
         """
-        path = "/sections/%s" % (section)
-        return self.client.put(path, params, **options)
+        return self._before_section
 
-    def delete(self, section, params={}, **options):
-        """A specific, existing section can be deleted by making a DELETE request
-        on the URL for that section.
+    @before_section.setter
+    def before_section(self, before_section):
+        """Sets the before_section of this ProjectSectionInsertRequest.
 
-        Note that sections must be empty to be deleted.
+        Insert the given section immediately before the section specified by this parameter.  # noqa: E501
 
-        The last remaining section in a board view cannot be deleted.
+        :param before_section: The before_section of this ProjectSectionInsertRequest.  # noqa: E501
+        :type: str
+        """
 
-        Returns an empty data block.
+        self._before_section = before_section
 
-        Parameters
-        ----------
-        section : {Gid} The section to delete.
-        """
-        path = "/sections/%s" % (section)
-        return self.client.delete(path, params, **options)
+    @property
+    def after_section(self):
+        """Gets the after_section of this ProjectSectionInsertRequest.  # noqa: E501
 
-    def add_task(self, section, params={}, **options):
-        """Add a task to a specific, existing section. This will remove the task from other sections of the project.
+        Insert the given section immediately after the section specified by this parameter.  # noqa: E501
 
-        The task will be inserted at the top of a section unless an `insert_before` or `insert_after` parameter is declared.
+        :return: The after_section of this ProjectSectionInsertRequest.  # noqa: E501
+        :rtype: str
+        """
+        return self._after_section
 
-        This does not work for separators (tasks with the `resource_subtype` of section).
+    @after_section.setter
+    def after_section(self, after_section):
+        """Sets the after_section of this ProjectSectionInsertRequest.
 
-        Parameters
-        ----------
-        section : {Gid} The section to add a task to
-        [data] : {Object} Data for the request
-          - task : {Gid} The task to add to this section
-          - [insert_before] : {Gid} Insert the given task immediately before the task specified by this parameter. Cannot be provided together with `insert_after`.
-          - [insert_after] : {Gid} Insert the given task immediately after the task specified by this parameter. Cannot be provided together with `insert_before`.
+        Insert the given section immediately after the section specified by this parameter.  # noqa: E501
+
+        :param after_section: The after_section of this ProjectSectionInsertRequest.  # noqa: E501
+        :type: str
         """
-        path = "/sections/%s/addTask" % (section)
-        return self.client.post(path, params, **options)
 
-    def insert_in_project(self, project, params={}, **options):
-        """Move sections relative to each other in a board view. One of
-        `before_section` or `after_section` is required.
+        self._after_section = after_section
 
-        Sections cannot be moved between projects.
+    def to_dict(self):
+        """Returns the model properties as a dict"""
+        result = {}
 
-        At this point in time, moving sections is not supported in list views, only board views.
+        for attr, _ in six.iteritems(self.swagger_types):
+            value = getattr(self, attr)
+            if isinstance(value, list):
+                result[attr] = list(map(
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
+                    value
+                ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
+            elif isinstance(value, dict):
+                result[attr] = dict(map(
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
+                    value.items()
+                ))
+            else:
+                result[attr] = value
+        if issubclass(ProjectSectionInsertRequest, dict):
+            for key, value in self.items():
+                result[key] = value
 
-        Returns an empty data block.
+        return result
 
-        Parameters
-        ----------
-        project : {Gid} The project in which to reorder the given section
-        [data] : {Object} Data for the request
-          - section : {Gid} The section to reorder
-          - [before_section] : {Gid} Insert the given section immediately before the section specified by this parameter.
-          - [after_section] : {Gid} Insert the given section immediately after the section specified by this parameter.
-        """
-        path = "/projects/%s/sections/insert" % (project)
-        return self.client.post(path, params, **options)
+    def to_str(self):
+        """Returns the string representation of the model"""
+        return pprint.pformat(self.to_dict())
+
+    def __repr__(self):
+        """For `print` and `pprint`"""
+        return self.to_str()
+
+    def __eq__(self, other):
+        """Returns true if both objects are equal"""
+        if not isinstance(other, ProjectSectionInsertRequest):
+            return False
+
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        """Returns true if both objects are not equal"""
+        return not self == other
```

