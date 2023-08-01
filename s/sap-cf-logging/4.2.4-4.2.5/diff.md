# Comparing `tmp/sap_cf_logging-4.2.4.tar.gz` & `tmp/sap_cf_logging-4.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sap_cf_logging-4.2.4.tar", last modified: Tue Apr 26 12:50:43 2022, max compression
+gzip compressed data, was "sap_cf_logging-4.2.5.tar", last modified: Tue Aug  1 11:17:37 2023, max compression
```

## Comparing `sap_cf_logging-4.2.4.tar` & `sap_cf_logging-4.2.5.tar`

### file list

```diff
@@ -1,60 +1,65 @@
-drwxrwxrwx   0        0        0        0 2022-04-26 12:50:43.396256 sap_cf_logging-4.2.4/
--rw-rw-rw-   0        0        0     1730 2022-04-26 12:49:56.000000 sap_cf_logging-4.2.4/CHANGELOG.md
--rw-rw-rw-   0        0        0    11558 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/LICENSE
--rw-rw-rw-   0        0        0       41 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0    12286 2022-04-26 12:50:43.397254 sap_cf_logging-4.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    11057 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/README.rst
-drwxrwxrwx   0        0        0        0 2022-04-26 12:50:42.731116 sap_cf_logging-4.2.4/sap/
--rw-rw-rw-   0        0        0       89 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-26 12:50:42.754115 sap_cf_logging-4.2.4/sap/cf_logging/
--rw-rw-rw-   0        0        0     2353 2022-04-26 12:49:56.000000 sap_cf_logging-4.2.4/sap/cf_logging/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-26 12:50:42.874110 sap_cf_logging-4.2.4/sap/cf_logging/core/
--rw-rw-rw-   0        0        0        0 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/core/__init__.py
--rw-rw-rw-   0        0        0      254 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/core/constants.py
--rw-rw-rw-   0        0        0     1028 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/core/context.py
--rw-rw-rw-   0        0        0     1712 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/core/framework.py
--rw-rw-rw-   0        0        0     3368 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/core/request_reader.py
--rw-rw-rw-   0        0        0      798 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/core/response_reader.py
--rw-rw-rw-   0        0        0      296 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/defaults.py
-drwxrwxrwx   0        0        0        0 2022-04-26 12:50:42.947540 sap_cf_logging-4.2.4/sap/cf_logging/django_logging/
--rw-rw-rw-   0        0        0     2449 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/django_logging/__init__.py
--rw-rw-rw-   0        0        0      829 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/django_logging/context.py
--rw-rw-rw-   0        0        0     1094 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/django_logging/request_reader.py
--rw-rw-rw-   0        0        0      464 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/django_logging/response_reader.py
-drwxrwxrwx   0        0        0        0 2022-04-26 12:50:43.040521 sap_cf_logging-4.2.4/sap/cf_logging/falcon_logging/
--rw-rw-rw-   0        0        0     2919 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/falcon_logging/__init__.py
--rw-rw-rw-   0        0        0      582 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/falcon_logging/context.py
--rw-rw-rw-   0        0        0      951 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/falcon_logging/request_reader.py
--rw-rw-rw-   0        0        0      439 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/falcon_logging/response_reader.py
-drwxrwxrwx   0        0        0        0 2022-04-26 12:50:43.119271 sap_cf_logging-4.2.4/sap/cf_logging/flask_logging/
--rw-rw-rw-   0        0        0     2758 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/flask_logging/__init__.py
--rw-rw-rw-   0        0        0      577 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/flask_logging/context.py
--rw-rw-rw-   0        0        0      745 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/flask_logging/request_reader.py
--rw-rw-rw-   0        0        0      378 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/flask_logging/response_reader.py
-drwxrwxrwx   0        0        0        0 2022-04-26 12:50:43.163469 sap_cf_logging-4.2.4/sap/cf_logging/formatters/
--rw-rw-rw-   0        0        0        0 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/formatters/__init__.py
--rw-rw-rw-   0        0        0      808 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/formatters/json_formatter.py
--rw-rw-rw-   0        0        0     1406 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/formatters/stacktrace_formatter.py
-drwxrwxrwx   0        0        0        0 2022-04-26 12:50:43.207665 sap_cf_logging-4.2.4/sap/cf_logging/job_logging/
--rw-rw-rw-   0        0        0        0 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/job_logging/__init__.py
--rw-rw-rw-   0        0        0      527 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/job_logging/context.py
--rw-rw-rw-   0        0        0      797 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/job_logging/framework.py
-drwxrwxrwx   0        0        0        0 2022-04-26 12:50:43.293055 sap_cf_logging-4.2.4/sap/cf_logging/record/
--rw-rw-rw-   0        0        0        0 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/record/__init__.py
--rw-rw-rw-   0        0        0      570 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/record/application_info.py
--rw-rw-rw-   0        0        0     4132 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/record/request_log_record.py
--rw-rw-rw-   0        0        0     4019 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/record/simple_log_record.py
--rw-rw-rw-   0        0        0     1623 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/record/util.py
-drwxrwxrwx   0        0        0        0 2022-04-26 12:50:43.371285 sap_cf_logging-4.2.4/sap/cf_logging/sanic_logging/
--rw-rw-rw-   0        0        0     3001 2022-04-26 12:48:17.000000 sap_cf_logging-4.2.4/sap/cf_logging/sanic_logging/__init__.py
--rw-rw-rw-   0        0        0      664 2022-04-26 12:48:18.000000 sap_cf_logging-4.2.4/sap/cf_logging/sanic_logging/context.py
--rw-rw-rw-   0        0        0      581 2022-04-26 12:48:18.000000 sap_cf_logging-4.2.4/sap/cf_logging/sanic_logging/request_reader.py
--rw-rw-rw-   0        0        0      484 2022-04-26 12:48:18.000000 sap_cf_logging-4.2.4/sap/cf_logging/sanic_logging/response_reader.py
-drwxrwxrwx   0        0        0        0 2022-04-26 12:50:43.392255 sap_cf_logging-4.2.4/sap_cf_logging.egg-info/
--rw-rw-rw-   0        0        0    12286 2022-04-26 12:50:42.000000 sap_cf_logging-4.2.4/sap_cf_logging.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1681 2022-04-26 12:50:42.000000 sap_cf_logging-4.2.4/sap_cf_logging.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-26 12:50:42.000000 sap_cf_logging-4.2.4/sap_cf_logging.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-04-26 12:50:40.000000 sap_cf_logging-4.2.4/sap_cf_logging.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        4 2022-04-26 12:50:42.000000 sap_cf_logging-4.2.4/sap_cf_logging.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      239 2022-04-26 12:50:43.415152 sap_cf_logging-4.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1753 2022-04-26 12:48:18.000000 sap_cf_logging-4.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:17:37.314465 sap_cf_logging-4.2.5/
+-rw-rw-rw-   0        0        0     1844 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/CHANGELOG.md
+-rw-rw-rw-   0        0        0    11558 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/LICENSE
+-rw-rw-rw-   0        0        0       41 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    12437 2023-08-01 11:17:37.317463 sap_cf_logging-4.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    11057 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-01 11:17:36.473730 sap_cf_logging-4.2.5/sap/
+-rw-rw-rw-   0        0        0       89 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:17:36.495730 sap_cf_logging-4.2.5/sap/cf_logging/
+-rw-rw-rw-   0        0        0     2353 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:17:36.620181 sap_cf_logging-4.2.5/sap/cf_logging/core/
+-rw-rw-rw-   0        0        0        0 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/core/__init__.py
+-rw-rw-rw-   0        0        0      254 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/core/constants.py
+-rw-rw-rw-   0        0        0     1028 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/core/context.py
+-rw-rw-rw-   0        0        0     1712 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/core/framework.py
+-rw-rw-rw-   0        0        0     3368 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/core/request_reader.py
+-rw-rw-rw-   0        0        0      798 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/core/response_reader.py
+-rw-rw-rw-   0        0        0      296 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/defaults.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:17:36.691041 sap_cf_logging-4.2.5/sap/cf_logging/django_logging/
+-rw-rw-rw-   0        0        0     2449 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/django_logging/__init__.py
+-rw-rw-rw-   0        0        0      829 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/django_logging/context.py
+-rw-rw-rw-   0        0        0     1094 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/django_logging/request_reader.py
+-rw-rw-rw-   0        0        0      464 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/django_logging/response_reader.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:17:36.728740 sap_cf_logging-4.2.5/sap/cf_logging/falcon_logging/
+-rw-rw-rw-   0        0        0     2919 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/falcon_logging/__init__.py
+-rw-rw-rw-   0        0        0      582 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/falcon_logging/context.py
+-rw-rw-rw-   0        0        0      951 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/falcon_logging/request_reader.py
+-rw-rw-rw-   0        0        0      439 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/falcon_logging/response_reader.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:17:36.771772 sap_cf_logging-4.2.5/sap/cf_logging/flask_logging/
+-rw-rw-rw-   0        0        0     2758 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/flask_logging/__init__.py
+-rw-rw-rw-   0        0        0      577 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/flask_logging/context.py
+-rw-rw-rw-   0        0        0      745 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/flask_logging/request_reader.py
+-rw-rw-rw-   0        0        0      378 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/flask_logging/response_reader.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:17:36.827771 sap_cf_logging-4.2.5/sap/cf_logging/formatters/
+-rw-rw-rw-   0        0        0        0 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/formatters/__init__.py
+-rw-rw-rw-   0        0        0      808 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/formatters/json_formatter.py
+-rw-rw-rw-   0        0        0     1406 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/formatters/stacktrace_formatter.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:17:36.878984 sap_cf_logging-4.2.5/sap/cf_logging/job_logging/
+-rw-rw-rw-   0        0        0        0 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/job_logging/__init__.py
+-rw-rw-rw-   0        0        0      527 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/job_logging/context.py
+-rw-rw-rw-   0        0        0      797 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/job_logging/framework.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:17:36.990176 sap_cf_logging-4.2.5/sap/cf_logging/record/
+-rw-rw-rw-   0        0        0        0 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/record/__init__.py
+-rw-rw-rw-   0        0        0      570 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/record/application_info.py
+-rw-rw-rw-   0        0        0     4132 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/record/request_log_record.py
+-rw-rw-rw-   0        0        0     3985 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/record/simple_log_record.py
+-rw-rw-rw-   0        0        0     1623 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/record/util.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:17:37.072853 sap_cf_logging-4.2.5/sap/cf_logging/sanic_logging/
+-rw-rw-rw-   0        0        0     3001 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/sanic_logging/__init__.py
+-rw-rw-rw-   0        0        0      664 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/sanic_logging/context.py
+-rw-rw-rw-   0        0        0      581 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/sanic_logging/request_reader.py
+-rw-rw-rw-   0        0        0      484 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/sap/cf_logging/sanic_logging/response_reader.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:17:37.169541 sap_cf_logging-4.2.5/sap_cf_logging.egg-info/
+-rw-rw-rw-   0        0        0    12437 2023-08-01 11:17:36.000000 sap_cf_logging-4.2.5/sap_cf_logging.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1792 2023-08-01 11:17:36.000000 sap_cf_logging-4.2.5/sap_cf_logging.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 11:17:36.000000 sap_cf_logging-4.2.5/sap_cf_logging.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-01 11:17:34.000000 sap_cf_logging-4.2.5/sap_cf_logging.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        4 2023-08-01 11:17:36.000000 sap_cf_logging-4.2.5/sap_cf_logging.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      239 2023-08-01 11:17:37.370035 sap_cf_logging-4.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1905 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:17:37.302467 sap_cf_logging-4.2.5/tests/
+-rw-rw-rw-   0        0        0     5269 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/tests/test_falcon_logging.py
+-rw-rw-rw-   0        0        0     3677 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/tests/test_flask_logging.py
+-rw-rw-rw-   0        0        0     4057 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/tests/test_job_logging.py
+-rw-rw-rw-   0        0        0     3861 2023-08-01 11:14:27.000000 sap_cf_logging-4.2.5/tests/test_sanic_logging.py
```

### Comparing `sap_cf_logging-4.2.4/CHANGELOG.md` & `sap_cf_logging-4.2.5/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Change Log
 All notable changes to this project will be documented in this file.
 
 This project adheres to [Semantic Versioning](http://semver.org/).
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/).
 
+## 4.2.5 - 2023-07-28
+
+### Fixed
+
+- Include stacktrace also for non-error log level if exc_info is present
+
 ## 4.2.4 - 2022-04-26
 
 ### Update
 
  - Update django version => 2.2.28
 
 ## 4.2.3 - 2022-03-23
```

### Comparing `sap_cf_logging-4.2.4/LICENSE` & `sap_cf_logging-4.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/PKG-INFO` & `sap_cf_logging-4.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sap_cf_logging
-Version: 4.2.4
+Version: 4.2.5
 Summary: Python logging library to emit JSON logs in a SAP CloudFoundry environment
 Home-page: https://github.com/SAP/cf-python-logging-support
 Author: SAP
 License: Apache License, Version 2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Flask
@@ -17,14 +17,17 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Logging
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
@@ -370,9 +373,7 @@
 See `CHANGELOG file <https://github.com/SAP/cf-python-logging-support/blob/master/CHANGELOG.md>`__.
 
 License
 -------
 
 Copyright (c) 2017-2021 SAP SE or an SAP affiliate company and cf-python-logging-support contributors.  Please see our `LICENSE file <https://github.com/SAP/cf-python-logging-support/blob/master/LICENSE>`__ for copyright and license information. Detailed information including third-party components and their licensing/copyright information is available `via the REUSE tool <https://api.reuse.software/info/github.com/SAP/cf-python-logging-support>`__.
 
-
-
```

### Comparing `sap_cf_logging-4.2.4/README.rst` & `sap_cf_logging-4.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/__init__.py` & `sap_cf_logging-4.2.5/sap/cf_logging/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from sap.cf_logging.core.constants import REQUEST_KEY, RESPONSE_KEY
 from sap.cf_logging.core.framework import Framework
 from sap.cf_logging.formatters.json_formatter import JsonFormatter
 from sap.cf_logging.job_logging.framework import JobFramework
 from sap.cf_logging.record.request_log_record import RequestWebRecord
 from sap.cf_logging.record.simple_log_record import SimpleLogRecord
 
-__version__ = '4.2.4'
+__version__ = '4.2.5'
 
 _SETUP_DONE = False
 FRAMEWORK = None
 
 
 class CfLogger(logging.Logger):
     """ CfLogger class inherits from logging.Logger and makes custom
```

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/core/context.py` & `sap_cf_logging-4.2.5/sap/cf_logging/core/context.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/core/framework.py` & `sap_cf_logging-4.2.5/sap/cf_logging/core/framework.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/core/request_reader.py` & `sap_cf_logging-4.2.5/sap/cf_logging/core/request_reader.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/core/response_reader.py` & `sap_cf_logging-4.2.5/sap/cf_logging/core/response_reader.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/django_logging/__init__.py` & `sap_cf_logging-4.2.5/sap/cf_logging/django_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/django_logging/context.py` & `sap_cf_logging-4.2.5/sap/cf_logging/django_logging/context.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/django_logging/request_reader.py` & `sap_cf_logging-4.2.5/sap/cf_logging/django_logging/request_reader.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/falcon_logging/__init__.py` & `sap_cf_logging-4.2.5/sap/cf_logging/falcon_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/falcon_logging/context.py` & `sap_cf_logging-4.2.5/sap/cf_logging/falcon_logging/context.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/falcon_logging/request_reader.py` & `sap_cf_logging-4.2.5/sap/cf_logging/falcon_logging/request_reader.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/flask_logging/__init__.py` & `sap_cf_logging-4.2.5/sap/cf_logging/flask_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/flask_logging/context.py` & `sap_cf_logging-4.2.5/sap/cf_logging/flask_logging/context.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/flask_logging/request_reader.py` & `sap_cf_logging-4.2.5/sap/cf_logging/flask_logging/request_reader.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/formatters/json_formatter.py` & `sap_cf_logging-4.2.5/sap/cf_logging/formatters/json_formatter.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/formatters/stacktrace_formatter.py` & `sap_cf_logging-4.2.5/sap/cf_logging/formatters/stacktrace_formatter.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/job_logging/context.py` & `sap_cf_logging-4.2.5/sap/cf_logging/job_logging/context.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/job_logging/framework.py` & `sap_cf_logging-4.2.5/sap/cf_logging/job_logging/framework.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/record/application_info.py` & `sap_cf_logging-4.2.5/sap/cf_logging/record/application_info.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/record/request_log_record.py` & `sap_cf_logging-4.2.5/sap/cf_logging/record/request_log_record.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/record/simple_log_record.py` & `sap_cf_logging-4.2.5/sap/cf_logging/record/simple_log_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             'type': 'log',
             'logger': self.name,
             'thread': self.threadName,
             'level': self.levelname,
             'msg': self.getMessage(),
         })
 
-        if self.levelno == logging.ERROR and self.exc_info:
+        if self.exc_info:
             stacktrace = ''.join(traceback.format_exception(*self.exc_info))
             stacktrace = format_stacktrace(stacktrace)
             record['stacktrace'] = stacktrace.split('\n')
             record['msg'] += "\n"
             record['msg'] += stacktrace
```

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/record/util.py` & `sap_cf_logging-4.2.5/sap/cf_logging/record/util.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/sanic_logging/__init__.py` & `sap_cf_logging-4.2.5/sap/cf_logging/sanic_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/sanic_logging/context.py` & `sap_cf_logging-4.2.5/sap/cf_logging/sanic_logging/context.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap/cf_logging/sanic_logging/request_reader.py` & `sap_cf_logging-4.2.5/sap/cf_logging/sanic_logging/request_reader.py`

 * *Files identical despite different names*

### Comparing `sap_cf_logging-4.2.4/sap_cf_logging.egg-info/PKG-INFO` & `sap_cf_logging-4.2.5/sap_cf_logging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sap-cf-logging
-Version: 4.2.4
+Version: 4.2.5
 Summary: Python logging library to emit JSON logs in a SAP CloudFoundry environment
 Home-page: https://github.com/SAP/cf-python-logging-support
 Author: SAP
 License: Apache License, Version 2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Flask
@@ -17,14 +17,17 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Logging
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
@@ -370,9 +373,7 @@
 See `CHANGELOG file <https://github.com/SAP/cf-python-logging-support/blob/master/CHANGELOG.md>`__.
 
 License
 -------
 
 Copyright (c) 2017-2021 SAP SE or an SAP affiliate company and cf-python-logging-support contributors.  Please see our `LICENSE file <https://github.com/SAP/cf-python-logging-support/blob/master/LICENSE>`__ for copyright and license information. Detailed information including third-party components and their licensing/copyright information is available `via the REUSE tool <https://api.reuse.software/info/github.com/SAP/cf-python-logging-support>`__.
 
-
-
```

### Comparing `sap_cf_logging-4.2.4/sap_cf_logging.egg-info/SOURCES.txt` & `sap_cf_logging-4.2.5/sap_cf_logging.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -40,8 +40,12 @@
 sap/cf_logging/sanic_logging/context.py
 sap/cf_logging/sanic_logging/request_reader.py
 sap/cf_logging/sanic_logging/response_reader.py
 sap_cf_logging.egg-info/PKG-INFO
 sap_cf_logging.egg-info/SOURCES.txt
 sap_cf_logging.egg-info/dependency_links.txt
 sap_cf_logging.egg-info/not-zip-safe
-sap_cf_logging.egg-info/top_level.txt
+sap_cf_logging.egg-info/top_level.txt
+tests/test_falcon_logging.py
+tests/test_flask_logging.py
+tests/test_job_logging.py
+tests/test_sanic_logging.py
```

### Comparing `sap_cf_logging-4.2.4/setup.py` & `sap_cf_logging-4.2.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,12 +34,15 @@
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Software Development',
         'Topic :: System :: Logging',
     ]
 )
```

