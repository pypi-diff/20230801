# Comparing `tmp/super-csv-3.0.1.tar.gz` & `tmp/super-csv-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "super-csv-3.0.1.tar", last modified: Mon Aug 15 14:46:31 2022, max compression
+gzip compressed data, was "super-csv-3.1.0.tar", last modified: Tue Aug  1 18:28:49 2023, max compression
```

## Comparing `super-csv-3.0.1.tar` & `super-csv-3.1.0.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 14:46:31.804106 super-csv-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     3459 2022-08-15 14:46:25.000000 super-csv-3.0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)      549 2022-08-15 14:46:25.000000 super-csv-3.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-08-15 14:46:25.000000 super-csv-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8496 2022-08-15 14:46:31.804106 super-csv-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4352 2022-08-15 14:46:25.000000 super-csv-3.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 14:46:31.800106 super-csv-3.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-08-15 14:46:25.000000 super-csv-3.0.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-08-15 14:46:31.804106 super-csv-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3080 2022-08-15 14:46:25.000000 super-csv-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 14:46:31.800106 super-csv-3.0.1/super_csv/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-08-15 14:46:25.000000 super-csv-3.0.1/super_csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-08-15 14:46:25.000000 super-csv-3.0.1/super_csv/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-08-15 14:46:25.000000 super-csv-3.0.1/super_csv/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-08-15 14:46:25.000000 super-csv-3.0.1/super_csv/common_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    11036 2022-08-15 14:46:25.000000 super-csv-3.0.1/super_csv/csv_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-08-15 14:46:25.000000 super-csv-3.0.1/super_csv/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 14:46:31.804106 super-csv-3.0.1/super_csv/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2022-08-15 14:46:25.000000 super-csv-3.0.1/super_csv/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-08-15 14:46:25.000000 super-csv-3.0.1/super_csv/migrations/0002_csvoperation_user.py
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-08-15 14:46:25.000000 super-csv-3.0.1/super_csv/migrations/0003_csvoperation_original_filename.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-15 14:46:25.000000 super-csv-3.0.1/super_csv/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7410 2022-08-15 14:46:25.000000 super-csv-3.0.1/super_csv/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)     2785 2022-08-15 14:46:25.000000 super-csv-3.0.1/super_csv/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1937 2022-08-15 14:46:25.000000 super-csv-3.0.1/super_csv/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-08-15 14:46:25.000000 super-csv-3.0.1/super_csv/signals.py
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-08-15 14:46:25.000000 super-csv-3.0.1/super_csv/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 14:46:31.800106 super-csv-3.0.1/super_csv/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 14:46:31.804106 super-csv-3.0.1/super_csv/templates/super_csv/
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-08-15 14:46:25.000000 super-csv-3.0.1/super_csv/templates/super_csv/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 14:46:31.804106 super-csv-3.0.1/super_csv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8496 2022-08-15 14:46:31.000000 super-csv-3.0.1/super_csv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-08-15 14:46:31.000000 super-csv-3.0.1/super_csv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-15 14:46:31.000000 super-csv-3.0.1/super_csv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-08-15 14:46:31.000000 super-csv-3.0.1/super_csv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-15 14:46:31.000000 super-csv-3.0.1/super_csv.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-08-15 14:46:31.000000 super-csv-3.0.1/super_csv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-15 14:46:31.000000 super-csv-3.0.1/super_csv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:28:49.759004 super-csv-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-08-01 18:28:43.000000 super-csv-3.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      549 2023-08-01 18:28:43.000000 super-csv-3.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-08-01 18:28:43.000000 super-csv-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8672 2023-08-01 18:28:49.759004 super-csv-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4253 2023-08-01 18:28:43.000000 super-csv-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:28:49.751004 super-csv-3.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      313 2023-08-01 18:28:43.000000 super-csv-3.1.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-08-01 18:28:49.759004 super-csv-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3084 2023-08-01 18:28:43.000000 super-csv-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:28:49.755004 super-csv-3.1.0/super_csv/
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      321 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/common_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11036 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/csv_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:28:49.759004 super-csv-3.1.0/super_csv/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1205 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      587 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/migrations/0002_csvoperation_user.py
+-rw-r--r--   0 runner    (1001) docker     (122)      430 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/migrations/0003_csvoperation_original_filename.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7410 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2785 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      478 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:28:49.751004 super-csv-3.1.0/super_csv/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:28:49.759004 super-csv-3.1.0/super_csv/templates/super_csv/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-08-01 18:28:43.000000 super-csv-3.1.0/super_csv/templates/super_csv/base.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:28:49.755004 super-csv-3.1.0/super_csv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8672 2023-08-01 18:28:49.000000 super-csv-3.1.0/super_csv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      846 2023-08-01 18:28:49.000000 super-csv-3.1.0/super_csv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-01 18:28:49.000000 super-csv-3.1.0/super_csv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-08-01 18:28:49.000000 super-csv-3.1.0/super_csv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-01 18:28:49.000000 super-csv-3.1.0/super_csv.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-08-01 18:28:49.000000 super-csv-3.1.0/super_csv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-08-01 18:28:49.000000 super-csv-3.1.0/super_csv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:28:49.759004 super-csv-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     9259 2023-08-01 18:28:43.000000 super-csv-3.1.0/tests/test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-08-01 18:28:43.000000 super-csv-3.1.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1416 2023-08-01 18:28:43.000000 super-csv-3.1.0/tests/test_serializers.py
```

### Comparing `super-csv-3.0.1/CHANGELOG.rst` & `super-csv-3.1.0/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,30 @@
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+
+[3.1.0] - 2023-07-31
+~~~~~~~~~~~~~~~~~~~~
+
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
+  more details.
+* Added support of Django 4.2
+
 [3.0.1] - 2022-02-17
+~~~~~~~~~~~~~~~~~~~~
 
 * fix: encode the csv data before save
 
 [3.0.0] - 2022-02-17
+~~~~~~~~~~~~~~~~~~~~
 
 * Fix `dev.in` to pull from `ci.txt` rather than `travis.txt`.
 * Dropped Django22, 30 and 31 support.
 * Added Django40 support.
 
 [2.1.1] - 2021-09-01
 ~~~~~~~~~~~~~~~~~~~~
```

### Comparing `super-csv-3.0.1/LICENSE.txt` & `super-csv-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `super-csv-3.0.1/PKG-INFO` & `super-csv-3.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: super-csv
-Version: 3.0.1
+Version: 3.1.0
 Summary: CSV Processor
-Home-page: https://github.com/edx/super-csv
+Home-page: https://github.com/openedx/super-csv
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Keywords: Django edx
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -27,15 +26,15 @@
 |license-badge|
 
 Generic CSV Processing for Django Apps
 
 Overview
 ------------------------
 
-This library provides a `CSVProcessor <https://github.com/edx/super-csv/blob/master/super_csv/csv_processor.py>`_ class
+This library provides a `CSVProcessor <https://github.com/openedx/super-csv/blob/master/super_csv/csv_processor.py>`_ class
 which should be subclassed to implement your own per-row processing of CSV files.
 At minimum, override `process_row(row)`.
 
 The mixins support optional checksums of arbitrary columns, and asynchronous processing of files using Celery.
 
 Documentation
 -------------
@@ -52,15 +51,15 @@
 
     make test
 
 Runs the unit tests in local environment.
 
 Using with Docker Devstack
 --------------------------
-Prerequisite: Have your Open edX https://github.com/edx/devstack properly installed.
+Prerequisite: Have your Open edX https://github.com/openedx/devstack properly installed.
 Note: When you see "from inside the lms" below, it means that you've run ``make lms-shell`` from your devstack directory
 and are on a command prompt inside the LMS container.
 
 #. Clone this repo into ``../src/`` directory (relative to your "devstack" repo location). This will mount the directory
    in a way that is accessible to the lms container.
 
 #. Clone inside the lms, uninstall super-csv and reinstall your local copy.
@@ -89,24 +88,22 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 The pull request description template should be automatically applied if you are creating a pull request from GitHub. Otherwise you
-can find it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/super-csv/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_.
+can find it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/super-csv/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_.
 
 The issue report template should be automatically applied if you are creating an issue on GitHub as well. Otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/super-csv/blob/master/.github/ISSUE_TEMPLATE.md>`_.
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/super-csv/blob/master/.github/ISSUE_TEMPLATE.md>`_.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -118,16 +115,16 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/super-csv.svg
     :target: https://pypi.python.org/pypi/super-csv/
     :alt: PyPI
 
-.. |CI| image:: https://github.com/edx/super-csv/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/super-csv/actions?query=workflow%3A%22Python+CI%22
+.. |CI| image:: https://github.com/openedx/super-csv/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/super-csv/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/super-csv/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/super-csv?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/super-csv/badge/?version=latest
@@ -135,15 +132,15 @@
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/super-csv.svg
     :target: https://pypi.python.org/pypi/super-csv/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/super-csv.svg
-    :target: https://github.com/edx/super-csv/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/super-csv/blob/master/LICENSE.txt
     :alt: License
 
 
 Change Log
 ----------
 
 ..
@@ -154,19 +151,30 @@
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+
+[3.1.0] - 2023-07-31
+~~~~~~~~~~~~~~~~~~~~
+
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
+  more details.
+* Added support of Django 4.2
+
 [3.0.1] - 2022-02-17
+~~~~~~~~~~~~~~~~~~~~
 
 * fix: encode the csv data before save
 
 [3.0.0] - 2022-02-17
+~~~~~~~~~~~~~~~~~~~~
 
 * Fix `dev.in` to pull from `ci.txt` rather than `travis.txt`.
 * Dropped Django22, 30 and 31 support.
 * Added Django40 support.
 
 [2.1.1] - 2021-09-01
 ~~~~~~~~~~~~~~~~~~~~
@@ -276,9 +284,7 @@
 [0.1.0] - 2019-05-15
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Added
 _____
 
 * First release on PyPI.
-
-
```

### Comparing `super-csv-3.0.1/README.rst` & `super-csv-3.1.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 |license-badge|
 
 Generic CSV Processing for Django Apps
 
 Overview
 ------------------------
 
-This library provides a `CSVProcessor <https://github.com/edx/super-csv/blob/master/super_csv/csv_processor.py>`_ class
+This library provides a `CSVProcessor <https://github.com/openedx/super-csv/blob/master/super_csv/csv_processor.py>`_ class
 which should be subclassed to implement your own per-row processing of CSV files.
 At minimum, override `process_row(row)`.
 
 The mixins support optional checksums of arbitrary columns, and asynchronous processing of files using Celery.
 
 Documentation
 -------------
@@ -30,15 +30,15 @@
 
     make test
 
 Runs the unit tests in local environment.
 
 Using with Docker Devstack
 --------------------------
-Prerequisite: Have your Open edX https://github.com/edx/devstack properly installed.
+Prerequisite: Have your Open edX https://github.com/openedx/devstack properly installed.
 Note: When you see "from inside the lms" below, it means that you've run ``make lms-shell`` from your devstack directory
 and are on a command prompt inside the LMS container.
 
 #. Clone this repo into ``../src/`` directory (relative to your "devstack" repo location). This will mount the directory
    in a way that is accessible to the lms container.
 
 #. Clone inside the lms, uninstall super-csv and reinstall your local copy.
@@ -67,24 +67,22 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 The pull request description template should be automatically applied if you are creating a pull request from GitHub. Otherwise you
-can find it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/super-csv/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_.
+can find it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/super-csv/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_.
 
 The issue report template should be automatically applied if you are creating an issue on GitHub as well. Otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/super-csv/blob/master/.github/ISSUE_TEMPLATE.md>`_.
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/super-csv/blob/master/.github/ISSUE_TEMPLATE.md>`_.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -96,16 +94,16 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/super-csv.svg
     :target: https://pypi.python.org/pypi/super-csv/
     :alt: PyPI
 
-.. |CI| image:: https://github.com/edx/super-csv/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/super-csv/actions?query=workflow%3A%22Python+CI%22
+.. |CI| image:: https://github.com/openedx/super-csv/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/super-csv/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/super-csv/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/super-csv?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/super-csv/badge/?version=latest
@@ -113,9 +111,9 @@
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/super-csv.svg
     :target: https://pypi.python.org/pypi/super-csv/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/super-csv.svg
-    :target: https://github.com/edx/super-csv/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/super-csv/blob/master/LICENSE.txt
     :alt: License
```

### Comparing `super-csv-3.0.1/setup.cfg` & `super-csv-3.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `super-csv-3.0.1/setup.py` & `super-csv-3.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     name='super-csv',
     version=VERSION,
     description="""CSV Processor""",
     long_description=README + '\n\n' + CHANGELOG,
     long_description_content_type='text/x-rst',
     author='edX',
     author_email='oscm@edx.org',
-    url='https://github.com/edx/super-csv',
+    url='https://github.com/openedx/super-csv',
     packages=[
         'super_csv',
     ],
     include_package_data=True,
     install_requires=load_requirements('requirements/base.in'),
     license="Apache 2.0",
     zip_safe=False,
```

### Comparing `super-csv-3.0.1/super_csv/csv_processor.py` & `super-csv-3.1.0/super_csv/csv_processor.py`

 * *Files identical despite different names*

### Comparing `super-csv-3.0.1/super_csv/migrations/0001_initial.py` & `super-csv-3.1.0/super_csv/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `super-csv-3.0.1/super_csv/migrations/0002_csvoperation_user.py` & `super-csv-3.1.0/super_csv/migrations/0002_csvoperation_user.py`

 * *Files identical despite different names*

### Comparing `super-csv-3.0.1/super_csv/mixins.py` & `super-csv-3.1.0/super_csv/mixins.py`

 * *Files identical despite different names*

### Comparing `super-csv-3.0.1/super_csv/models.py` & `super-csv-3.1.0/super_csv/models.py`

 * *Files identical despite different names*

### Comparing `super-csv-3.0.1/super_csv/serializers.py` & `super-csv-3.1.0/super_csv/serializers.py`

 * *Files identical despite different names*

### Comparing `super-csv-3.0.1/super_csv/signals.py` & `super-csv-3.1.0/super_csv/signals.py`

 * *Files identical despite different names*

### Comparing `super-csv-3.0.1/super_csv/templates/super_csv/base.html` & `super-csv-3.1.0/super_csv/templates/super_csv/base.html`

 * *Files identical despite different names*

### Comparing `super-csv-3.0.1/super_csv.egg-info/PKG-INFO` & `super-csv-3.1.0/super_csv.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: super-csv
-Version: 3.0.1
+Version: 3.1.0
 Summary: CSV Processor
-Home-page: https://github.com/edx/super-csv
+Home-page: https://github.com/openedx/super-csv
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Keywords: Django edx
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -27,15 +26,15 @@
 |license-badge|
 
 Generic CSV Processing for Django Apps
 
 Overview
 ------------------------
 
-This library provides a `CSVProcessor <https://github.com/edx/super-csv/blob/master/super_csv/csv_processor.py>`_ class
+This library provides a `CSVProcessor <https://github.com/openedx/super-csv/blob/master/super_csv/csv_processor.py>`_ class
 which should be subclassed to implement your own per-row processing of CSV files.
 At minimum, override `process_row(row)`.
 
 The mixins support optional checksums of arbitrary columns, and asynchronous processing of files using Celery.
 
 Documentation
 -------------
@@ -52,15 +51,15 @@
 
     make test
 
 Runs the unit tests in local environment.
 
 Using with Docker Devstack
 --------------------------
-Prerequisite: Have your Open edX https://github.com/edx/devstack properly installed.
+Prerequisite: Have your Open edX https://github.com/openedx/devstack properly installed.
 Note: When you see "from inside the lms" below, it means that you've run ``make lms-shell`` from your devstack directory
 and are on a command prompt inside the LMS container.
 
 #. Clone this repo into ``../src/`` directory (relative to your "devstack" repo location). This will mount the directory
    in a way that is accessible to the lms container.
 
 #. Clone inside the lms, uninstall super-csv and reinstall your local copy.
@@ -89,24 +88,22 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 The pull request description template should be automatically applied if you are creating a pull request from GitHub. Otherwise you
-can find it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/super-csv/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_.
+can find it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/super-csv/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_.
 
 The issue report template should be automatically applied if you are creating an issue on GitHub as well. Otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/super-csv/blob/master/.github/ISSUE_TEMPLATE.md>`_.
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/super-csv/blob/master/.github/ISSUE_TEMPLATE.md>`_.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -118,16 +115,16 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/super-csv.svg
     :target: https://pypi.python.org/pypi/super-csv/
     :alt: PyPI
 
-.. |CI| image:: https://github.com/edx/super-csv/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/super-csv/actions?query=workflow%3A%22Python+CI%22
+.. |CI| image:: https://github.com/openedx/super-csv/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/super-csv/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/super-csv/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/super-csv?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/super-csv/badge/?version=latest
@@ -135,15 +132,15 @@
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/super-csv.svg
     :target: https://pypi.python.org/pypi/super-csv/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/super-csv.svg
-    :target: https://github.com/edx/super-csv/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/super-csv/blob/master/LICENSE.txt
     :alt: License
 
 
 Change Log
 ----------
 
 ..
@@ -154,19 +151,30 @@
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+
+[3.1.0] - 2023-07-31
+~~~~~~~~~~~~~~~~~~~~
+
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
+  more details.
+* Added support of Django 4.2
+
 [3.0.1] - 2022-02-17
+~~~~~~~~~~~~~~~~~~~~
 
 * fix: encode the csv data before save
 
 [3.0.0] - 2022-02-17
+~~~~~~~~~~~~~~~~~~~~
 
 * Fix `dev.in` to pull from `ci.txt` rather than `travis.txt`.
 * Dropped Django22, 30 and 31 support.
 * Added Django40 support.
 
 [2.1.1] - 2021-09-01
 ~~~~~~~~~~~~~~~~~~~~
@@ -276,9 +284,7 @@
 [0.1.0] - 2019-05-15
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Added
 _____
 
 * First release on PyPI.
-
-
```

### Comparing `super-csv-3.0.1/super_csv.egg-info/SOURCES.txt` & `super-csv-3.1.0/super_csv.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -23,8 +23,11 @@
 super_csv.egg-info/not-zip-safe
 super_csv.egg-info/requires.txt
 super_csv.egg-info/top_level.txt
 super_csv/migrations/0001_initial.py
 super_csv/migrations/0002_csvoperation_user.py
 super_csv/migrations/0003_csvoperation_original_filename.py
 super_csv/migrations/__init__.py
-super_csv/templates/super_csv/base.html
+super_csv/templates/super_csv/base.html
+tests/test_csv.py
+tests/test_models.py
+tests/test_serializers.py
```

