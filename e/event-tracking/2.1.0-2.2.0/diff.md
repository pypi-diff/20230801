# Comparing `tmp/event-tracking-2.1.0.tar.gz` & `tmp/event-tracking-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event-tracking-2.1.0.tar", last modified: Wed Feb 23 10:24:20 2022, max compression
+gzip compressed data, was "event-tracking-2.2.0.tar", last modified: Tue Aug  1 18:32:41 2023, max compression
```

## Comparing `event-tracking-2.1.0.tar` & `event-tracking-2.2.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:24:20.585125 event-tracking-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-02-23 10:24:16.000000 event-tracking-2.1.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)    35136 2022-02-23 10:24:16.000000 event-tracking-2.1.0/LICENSE.TXT
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-02-23 10:24:16.000000 event-tracking-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7557 2022-02-23 10:24:20.585125 event-tracking-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6646 2022-02-23 10:24:16.000000 event-tracking-2.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:24:20.581125 event-tracking-2.1.0/event_tracking.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7557 2022-02-23 10:24:20.000000 event-tracking-2.1.0/event_tracking.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-02-23 10:24:20.000000 event-tracking-2.1.0/event_tracking.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-23 10:24:20.000000 event-tracking-2.1.0/event_tracking.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-02-23 10:24:20.000000 event-tracking-2.1.0/event_tracking.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-23 10:24:20.000000 event-tracking-2.1.0/event_tracking.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:24:20.585125 event-tracking-2.1.0/eventtracking/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:24:20.585125 event-tracking-2.1.0/eventtracking/backends/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/backends/async_routing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2037 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/backends/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     2945 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/backends/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (121)     5942 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/backends/routing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3288 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/backends/segment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:24:20.585125 event-tracking-2.1.0/eventtracking/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     2521 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/backends/tests/test_async_routing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3068 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/backends/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     2491 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/backends/tests/test_logger_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1913 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/backends/tests/test_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (121)     2951 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/backends/tests/test_mongodb_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/backends/tests/test_mongodb_performance.py
--rw-r--r--   0 runner    (1001) docker     (121)    10049 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/backends/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (121)     5831 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/backends/tests/test_segment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:24:20.585125 event-tracking-2.1.0/eventtracking/django/
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/django/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     6153 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/django/django_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:24:20.585125 event-tracking-2.1.0/eventtracking/django/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/django/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/django/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     9650 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/django/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/django/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1581 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/locator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:24:20.585125 event-tracking-2.1.0/eventtracking/processors/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/processors/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2969 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/processors/regex_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:24:20.585125 event-tracking-2.1.0/eventtracking/processors/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/processors/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1861 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/processors/tests/test_regex_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3092 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/processors/tests/test_whitelist.py
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/processors/whitelist.py
--rw-r--r--   0 runner    (1001) docker     (121)     1827 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:24:20.585125 event-tracking-2.1.0/eventtracking/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2380 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/tests/test_locator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     5277 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/tests/test_track.py
--rw-r--r--   0 runner    (1001) docker     (121)     4662 2022-02-23 10:24:16.000000 event-tracking-2.1.0/eventtracking/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:24:20.585125 event-tracking-2.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-02-23 10:24:16.000000 event-tracking-2.1.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-02-23 10:24:20.585125 event-tracking-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2924 2022-02-23 10:24:16.000000 event-tracking-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:32:41.700628 event-tracking-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-08-01 18:32:33.000000 event-tracking-2.2.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-08-01 18:32:33.000000 event-tracking-2.2.0/LICENSE.TXT
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-08-01 18:32:33.000000 event-tracking-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7553 2023-08-01 18:32:41.700628 event-tracking-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6658 2023-08-01 18:32:33.000000 event-tracking-2.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:32:41.692628 event-tracking-2.2.0/event_tracking.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7553 2023-08-01 18:32:41.000000 event-tracking-2.2.0/event_tracking.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-08-01 18:32:41.000000 event-tracking-2.2.0/event_tracking.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-01 18:32:41.000000 event-tracking-2.2.0/event_tracking.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-08-01 18:32:41.000000 event-tracking-2.2.0/event_tracking.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-08-01 18:32:41.000000 event-tracking-2.2.0/event_tracking.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:32:41.692628 event-tracking-2.2.0/eventtracking/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:32:41.696628 event-tracking-2.2.0/eventtracking/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1618 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/backends/async_routing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2037 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/backends/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2945 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/backends/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5942 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/backends/routing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3288 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/backends/segment.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:32:41.696628 event-tracking-2.2.0/eventtracking/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2521 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      973 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/backends/tests/test_async_routing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3068 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/backends/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2491 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/backends/tests/test_logger_integration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1913 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/backends/tests/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2951 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/backends/tests/test_mongodb_integration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/backends/tests/test_mongodb_performance.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10049 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/backends/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5831 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/backends/tests/test_segment.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:32:41.696628 event-tracking-2.2.0/eventtracking/django/
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/django/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6153 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/django/django_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:32:41.696628 event-tracking-2.2.0/eventtracking/django/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/django/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      356 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/django/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9650 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/django/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/django/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/locator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:32:41.696628 event-tracking-2.2.0/eventtracking/processors/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      547 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/processors/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2969 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/processors/regex_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:32:41.696628 event-tracking-2.2.0/eventtracking/processors/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/processors/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1861 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/processors/tests/test_regex_filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3092 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/processors/tests/test_whitelist.py
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/processors/whitelist.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1827 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:32:41.700628 event-tracking-2.2.0/eventtracking/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/tests/test_locator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5277 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/tests/test_track.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4662 2023-08-01 18:32:33.000000 event-tracking-2.2.0/eventtracking/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:32:41.700628 event-tracking-2.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-08-01 18:32:33.000000 event-tracking-2.2.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-08-01 18:32:41.700628 event-tracking-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2928 2023-08-01 18:32:33.000000 event-tracking-2.2.0/setup.py
```

### Comparing `event-tracking-2.1.0/LICENSE.TXT` & `event-tracking-2.2.0/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/PKG-INFO` & `event-tracking-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: event-tracking
-Version: 2.1.0
+Version: 2.2.0
 Summary: A simple event tracking system.
-Home-page: https://github.com/edx/event-tracking
+Home-page: https://github.com/openedx/event-tracking
 Author: edX
 Author-email: oscm@edx.org
 License: AGPLv3 License
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -201,26 +200,24 @@
 
 
 How to Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/wiki/How-To-Contribute>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/edx-platform/wiki/How-To-Contribute>`_ for details.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org
 
 Mailing List and IRC Channel
 ----------------------------
 
 You can discuss this code on the `edx-code Google Group`__ or in the
 ``edx-code`` IRC channel on Freenode.
 
 __ https://groups.google.com/forum/#!forum/edx-code
 
-.. |build-status| image:: https://github.com/edx/event-tracking/workflows/Python%20CI/badge.svg?branch=master
-   :target: https://github.com/edx/event-tracking/actions?query=workflow%3A%22Python+CI%22
-
-
+.. |build-status| image:: https://github.com/openedx/event-tracking/workflows/Python%20CI/badge.svg?branch=master
+   :target: https://github.com/openedx/event-tracking/actions?query=workflow%3A%22Python+CI%22
```

### Comparing `event-tracking-2.1.0/README.rst` & `event-tracking-2.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -176,24 +176,24 @@
 
 
 How to Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/wiki/How-To-Contribute>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/edx-platform/wiki/How-To-Contribute>`_ for details.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org
 
 Mailing List and IRC Channel
 ----------------------------
 
 You can discuss this code on the `edx-code Google Group`__ or in the
 ``edx-code`` IRC channel on Freenode.
 
 __ https://groups.google.com/forum/#!forum/edx-code
 
-.. |build-status| image:: https://github.com/edx/event-tracking/workflows/Python%20CI/badge.svg?branch=master
-   :target: https://github.com/edx/event-tracking/actions?query=workflow%3A%22Python+CI%22
+.. |build-status| image:: https://github.com/openedx/event-tracking/workflows/Python%20CI/badge.svg?branch=master
+   :target: https://github.com/openedx/event-tracking/actions?query=workflow%3A%22Python+CI%22
```

### Comparing `event-tracking-2.1.0/event_tracking.egg-info/PKG-INFO` & `event-tracking-2.2.0/event_tracking.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: event-tracking
-Version: 2.1.0
+Version: 2.2.0
 Summary: A simple event tracking system.
-Home-page: https://github.com/edx/event-tracking
+Home-page: https://github.com/openedx/event-tracking
 Author: edX
 Author-email: oscm@edx.org
 License: AGPLv3 License
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -201,26 +200,24 @@
 
 
 How to Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/wiki/How-To-Contribute>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/edx-platform/wiki/How-To-Contribute>`_ for details.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org
 
 Mailing List and IRC Channel
 ----------------------------
 
 You can discuss this code on the `edx-code Google Group`__ or in the
 ``edx-code`` IRC channel on Freenode.
 
 __ https://groups.google.com/forum/#!forum/edx-code
 
-.. |build-status| image:: https://github.com/edx/event-tracking/workflows/Python%20CI/badge.svg?branch=master
-   :target: https://github.com/edx/event-tracking/actions?query=workflow%3A%22Python+CI%22
-
-
+.. |build-status| image:: https://github.com/openedx/event-tracking/workflows/Python%20CI/badge.svg?branch=master
+   :target: https://github.com/openedx/event-tracking/actions?query=workflow%3A%22Python+CI%22
```

### Comparing `event-tracking-2.1.0/event_tracking.egg-info/SOURCES.txt` & `event-tracking-2.2.0/event_tracking.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/backends/async_routing.py` & `event-tracking-2.2.0/eventtracking/backends/async_routing.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/backends/logger.py` & `event-tracking-2.2.0/eventtracking/backends/logger.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/backends/mongodb.py` & `event-tracking-2.2.0/eventtracking/backends/mongodb.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/backends/routing.py` & `event-tracking-2.2.0/eventtracking/backends/routing.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/backends/segment.py` & `event-tracking-2.2.0/eventtracking/backends/segment.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/backends/tests/__init__.py` & `event-tracking-2.2.0/eventtracking/backends/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/backends/tests/test_async_routing.py` & `event-tracking-2.2.0/eventtracking/backends/tests/test_async_routing.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/backends/tests/test_logger.py` & `event-tracking-2.2.0/eventtracking/backends/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/backends/tests/test_logger_integration.py` & `event-tracking-2.2.0/eventtracking/backends/tests/test_logger_integration.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/backends/tests/test_mongodb.py` & `event-tracking-2.2.0/eventtracking/backends/tests/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/backends/tests/test_mongodb_integration.py` & `event-tracking-2.2.0/eventtracking/backends/tests/test_mongodb_integration.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/backends/tests/test_mongodb_performance.py` & `event-tracking-2.2.0/eventtracking/backends/tests/test_mongodb_performance.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/backends/tests/test_routing.py` & `event-tracking-2.2.0/eventtracking/backends/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/backends/tests/test_segment.py` & `event-tracking-2.2.0/eventtracking/backends/tests/test_segment.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/django/apps.py` & `event-tracking-2.2.0/eventtracking/django/apps.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/django/django_tracker.py` & `event-tracking-2.2.0/eventtracking/django/django_tracker.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/django/tests/test_configuration.py` & `event-tracking-2.2.0/eventtracking/django/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/locator.py` & `event-tracking-2.2.0/eventtracking/locator.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/processors/exceptions.py` & `event-tracking-2.2.0/eventtracking/processors/exceptions.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/processors/regex_filter.py` & `event-tracking-2.2.0/eventtracking/processors/regex_filter.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/processors/tests/test_regex_filter.py` & `event-tracking-2.2.0/eventtracking/processors/tests/test_regex_filter.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/processors/tests/test_whitelist.py` & `event-tracking-2.2.0/eventtracking/processors/tests/test_whitelist.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/processors/whitelist.py` & `event-tracking-2.2.0/eventtracking/processors/whitelist.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/tasks.py` & `event-tracking-2.2.0/eventtracking/tasks.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/tests/test_locator.py` & `event-tracking-2.2.0/eventtracking/tests/test_locator.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/tests/test_tasks.py` & `event-tracking-2.2.0/eventtracking/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/tests/test_track.py` & `event-tracking-2.2.0/eventtracking/tests/test_track.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/eventtracking/tracker.py` & `event-tracking-2.2.0/eventtracking/tracker.py`

 * *Files identical despite different names*

### Comparing `event-tracking-2.1.0/setup.py` & `event-tracking-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     version=VERSION,
     packages=find_packages(),
     include_package_data=True,
     license='AGPLv3 License',
     description='A simple event tracking system.',
     long_description=README,
     install_requires=REQUIREMENTS,
-    url='https://github.com/edx/event-tracking',
+    url='https://github.com/openedx/event-tracking',
     author='edX',
     author_email='oscm@edx.org',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
```

