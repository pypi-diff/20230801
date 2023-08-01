# Comparing `tmp/yet_another_wizz_cli-1.2.5.tar.gz` & `tmp/yet_another_wizz_cli-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yet_another_wizz_cli-1.2.5.tar", last modified: Fri Jul 28 22:42:32 2023, max compression
+gzip compressed data, was "yet_another_wizz_cli-1.2.6.tar", last modified: Tue Aug  1 06:31:13 2023, max compression
```

## Comparing `yet_another_wizz_cli-1.2.5.tar` & `yet_another_wizz_cli-1.2.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:42:32.326504 yet_another_wizz_cli-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-28 22:42:32.326504 yet_another_wizz_cli-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 22:42:32.326504 yet_another_wizz_cli-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:42:32.322504 yet_another_wizz_cli-1.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:42:32.326504 yet_another_wizz_cli-1.2.5/src/yaw_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:42:32.326504 yet_another_wizz_cli-1.2.5/src/yaw_cli/commandline/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/commandline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/commandline/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    17419 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/commandline/subcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/commandline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:42:32.326504 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/default_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/directories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    16014 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15048 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    19259 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:42:32.326504 yet_another_wizz_cli-1.2.5/src/yet_another_wizz_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-28 22:42:32.000000 yet_another_wizz_cli-1.2.5/src/yet_another_wizz_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-28 22:42:32.000000 yet_another_wizz_cli-1.2.5/src/yet_another_wizz_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:42:32.000000 yet_another_wizz_cli-1.2.5/src/yet_another_wizz_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 22:42:32.000000 yet_another_wizz_cli-1.2.5/src/yet_another_wizz_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-28 22:42:32.000000 yet_another_wizz_cli-1.2.5/src/yet_another_wizz_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 22:42:32.000000 yet_another_wizz_cli-1.2.5/src/yet_another_wizz_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:31:13.566652 yet_another_wizz_cli-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-01 06:30:47.000000 yet_another_wizz_cli-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-08-01 06:31:13.566652 yet_another_wizz_cli-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-08-01 06:30:47.000000 yet_another_wizz_cli-1.2.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-01 06:30:47.000000 yet_another_wizz_cli-1.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 06:31:13.566652 yet_another_wizz_cli-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-01 06:30:47.000000 yet_another_wizz_cli-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:31:13.562652 yet_another_wizz_cli-1.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:31:13.562652 yet_another_wizz_cli-1.2.6/src/yaw_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-01 06:30:47.000000 yet_another_wizz_cli-1.2.6/src/yaw_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:31:13.562652 yet_another_wizz_cli-1.2.6/src/yaw_cli/commandline/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-01 06:30:47.000000 yet_another_wizz_cli-1.2.6/src/yaw_cli/commandline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-08-01 06:30:47.000000 yet_another_wizz_cli-1.2.6/src/yaw_cli/commandline/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17419 2023-08-01 06:30:47.000000 yet_another_wizz_cli-1.2.6/src/yaw_cli/commandline/subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-08-01 06:30:47.000000 yet_another_wizz_cli-1.2.6/src/yaw_cli/commandline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:31:13.566652 yet_another_wizz_cli-1.2.6/src/yaw_cli/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-08-01 06:30:47.000000 yet_another_wizz_cli-1.2.6/src/yaw_cli/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-08-01 06:30:47.000000 yet_another_wizz_cli-1.2.6/src/yaw_cli/pipeline/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-08-01 06:30:47.000000 yet_another_wizz_cli-1.2.6/src/yaw_cli/pipeline/default_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-08-01 06:30:47.000000 yet_another_wizz_cli-1.2.6/src/yaw_cli/pipeline/directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-08-01 06:30:47.000000 yet_another_wizz_cli-1.2.6/src/yaw_cli/pipeline/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-08-01 06:30:47.000000 yet_another_wizz_cli-1.2.6/src/yaw_cli/pipeline/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-08-01 06:30:47.000000 yet_another_wizz_cli-1.2.6/src/yaw_cli/pipeline/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16014 2023-08-01 06:30:47.000000 yet_another_wizz_cli-1.2.6/src/yaw_cli/pipeline/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15048 2023-08-01 06:30:47.000000 yet_another_wizz_cli-1.2.6/src/yaw_cli/pipeline/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19259 2023-08-01 06:30:47.000000 yet_another_wizz_cli-1.2.6/src/yaw_cli/pipeline/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:31:13.566652 yet_another_wizz_cli-1.2.6/src/yet_another_wizz_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-08-01 06:31:13.000000 yet_another_wizz_cli-1.2.6/src/yet_another_wizz_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-01 06:31:13.000000 yet_another_wizz_cli-1.2.6/src/yet_another_wizz_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:31:13.000000 yet_another_wizz_cli-1.2.6/src/yet_another_wizz_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 06:31:13.000000 yet_another_wizz_cli-1.2.6/src/yet_another_wizz_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-01 06:31:13.000000 yet_another_wizz_cli-1.2.6/src/yet_another_wizz_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 06:31:13.000000 yet_another_wizz_cli-1.2.6/src/yet_another_wizz_cli.egg-info/top_level.txt
```

### Comparing `yet_another_wizz_cli-1.2.5/LICENSE` & `yet_another_wizz_cli-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.5/PKG-INFO` & `yet_another_wizz_cli-1.2.6/src/yet_another_wizz_cli.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: yet_another_wizz_cli
-Version: 1.2.5
+Name: yet-another-wizz-cli
+Version: 1.2.6
 Summary: Command line client for yet_another_wizz.
 Home-page: https://github.com/jlvdb/yet_another_wizz_cli.git
 Author-email: Jan Luca van den Busch <jlvdb@astro.ruhr-uni-bochum.de>
 License: GPL-3.0-or-later
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Programming Language :: Python :: 3
@@ -21,32 +21,33 @@
     :width: 1000
     :alt: yet_another_wizz
 
 |
 
 .. image:: https://img.shields.io/pypi/v/yet_another_wizz_cli?logo=pypi&logoColor=blue
     :target: https://pypi.org/project/yet_another_wizz_cli/
+.. image:: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/docker-publish.yml/badge.svg
+    :target: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/docker-publish.yml
 .. image:: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/run-tests.yml/badge.svg
     :target: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/run-tests.yml
+.. image:: https://readthedocs.org/projects/yet-another-wizz/badge/?version=latest
+    :target: https://yet-another-wizz.readthedocs.io/en/latest/?badge=latest
 .. image:: https://codecov.io/gh/jlvdb/yet_another_wizz_cli/branch/main/graph/badge.svg?token=PC41ME2AR8
     :target: https://codecov.io/gh/jlvdb/yet_another_wizz_cli
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
-    :target: https://pycqa.github.io/isort/
 
 
 Commandline tool
 ================
 
 *yet_another_wizz_cli* implements a command line interface for the clustering
 redshift code `yet_another_wizz <https://github.com/jlvdb/yet_another_wizz>`_:
 
 - code: https://github.com/jlvdb/yet_another_wizz_cli.git
 - PyPI: https://pypi.org/project/yet_another_wizz_cli/
+- Docker: https://hub.docker.com/r/jlvdb/yet_another_wizz_cli/
 
 The documentation of this commandline tool is part of the official documentation
 of *yet_another_wizz* itself, including some usage examples:
 
 - docs: https://yet-another-wizz.readthedocs.io/
 
 Refer especially to the sections **User guide / Usage examples** and
```

### Comparing `yet_another_wizz_cli-1.2.5/README.rst` & `yet_another_wizz_cli-1.2.6/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -2,32 +2,33 @@
     :width: 1000
     :alt: yet_another_wizz
 
 |
 
 .. image:: https://img.shields.io/pypi/v/yet_another_wizz_cli?logo=pypi&logoColor=blue
     :target: https://pypi.org/project/yet_another_wizz_cli/
+.. image:: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/docker-publish.yml/badge.svg
+    :target: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/docker-publish.yml
 .. image:: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/run-tests.yml/badge.svg
     :target: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/run-tests.yml
+.. image:: https://readthedocs.org/projects/yet-another-wizz/badge/?version=latest
+    :target: https://yet-another-wizz.readthedocs.io/en/latest/?badge=latest
 .. image:: https://codecov.io/gh/jlvdb/yet_another_wizz_cli/branch/main/graph/badge.svg?token=PC41ME2AR8
     :target: https://codecov.io/gh/jlvdb/yet_another_wizz_cli
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
-    :target: https://pycqa.github.io/isort/
 
 
 Commandline tool
 ================
 
 *yet_another_wizz_cli* implements a command line interface for the clustering
 redshift code `yet_another_wizz <https://github.com/jlvdb/yet_another_wizz>`_:
 
 - code: https://github.com/jlvdb/yet_another_wizz_cli.git
 - PyPI: https://pypi.org/project/yet_another_wizz_cli/
+- Docker: https://hub.docker.com/r/jlvdb/yet_another_wizz_cli/
 
 The documentation of this commandline tool is part of the official documentation
 of *yet_another_wizz* itself, including some usage examples:
 
 - docs: https://yet-another-wizz.readthedocs.io/
 
 Refer especially to the sections **User guide / Usage examples** and
```

### Comparing `yet_another_wizz_cli-1.2.5/pyproject.toml` & `yet_another_wizz_cli-1.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.5/src/yaw_cli/commandline/main.py` & `yet_another_wizz_cli-1.2.6/src/yaw_cli/commandline/main.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.5/src/yaw_cli/commandline/subcommands.py` & `yet_another_wizz_cli-1.2.6/src/yaw_cli/commandline/subcommands.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.5/src/yaw_cli/commandline/utils.py` & `yet_another_wizz_cli-1.2.6/src/yaw_cli/commandline/utils.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/__init__.py` & `yet_another_wizz_cli-1.2.6/src/yaw_cli/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/data.py` & `yet_another_wizz_cli-1.2.6/src/yaw_cli/pipeline/data.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/default_setup.py` & `yet_another_wizz_cli-1.2.6/src/yaw_cli/pipeline/default_setup.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/directories.py` & `yet_another_wizz_cli-1.2.6/src/yaw_cli/pipeline/directories.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/logger.py` & `yet_another_wizz_cli-1.2.6/src/yaw_cli/pipeline/logger.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/merge.py` & `yet_another_wizz_cli-1.2.6/src/yaw_cli/pipeline/merge.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/plot.py` & `yet_another_wizz_cli-1.2.6/src/yaw_cli/pipeline/plot.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/processing.py` & `yet_another_wizz_cli-1.2.6/src/yaw_cli/pipeline/processing.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/project.py` & `yet_another_wizz_cli-1.2.6/src/yaw_cli/pipeline/project.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/tasks.py` & `yet_another_wizz_cli-1.2.6/src/yaw_cli/pipeline/tasks.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.5/src/yet_another_wizz_cli.egg-info/PKG-INFO` & `yet_another_wizz_cli-1.2.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: yet-another-wizz-cli
-Version: 1.2.5
+Name: yet_another_wizz_cli
+Version: 1.2.6
 Summary: Command line client for yet_another_wizz.
 Home-page: https://github.com/jlvdb/yet_another_wizz_cli.git
 Author-email: Jan Luca van den Busch <jlvdb@astro.ruhr-uni-bochum.de>
 License: GPL-3.0-or-later
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Programming Language :: Python :: 3
@@ -21,32 +21,33 @@
     :width: 1000
     :alt: yet_another_wizz
 
 |
 
 .. image:: https://img.shields.io/pypi/v/yet_another_wizz_cli?logo=pypi&logoColor=blue
     :target: https://pypi.org/project/yet_another_wizz_cli/
+.. image:: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/docker-publish.yml/badge.svg
+    :target: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/docker-publish.yml
 .. image:: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/run-tests.yml/badge.svg
     :target: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/run-tests.yml
+.. image:: https://readthedocs.org/projects/yet-another-wizz/badge/?version=latest
+    :target: https://yet-another-wizz.readthedocs.io/en/latest/?badge=latest
 .. image:: https://codecov.io/gh/jlvdb/yet_another_wizz_cli/branch/main/graph/badge.svg?token=PC41ME2AR8
     :target: https://codecov.io/gh/jlvdb/yet_another_wizz_cli
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
-    :target: https://pycqa.github.io/isort/
 
 
 Commandline tool
 ================
 
 *yet_another_wizz_cli* implements a command line interface for the clustering
 redshift code `yet_another_wizz <https://github.com/jlvdb/yet_another_wizz>`_:
 
 - code: https://github.com/jlvdb/yet_another_wizz_cli.git
 - PyPI: https://pypi.org/project/yet_another_wizz_cli/
+- Docker: https://hub.docker.com/r/jlvdb/yet_another_wizz_cli/
 
 The documentation of this commandline tool is part of the official documentation
 of *yet_another_wizz* itself, including some usage examples:
 
 - docs: https://yet-another-wizz.readthedocs.io/
 
 Refer especially to the sections **User guide / Usage examples** and
```

### Comparing `yet_another_wizz_cli-1.2.5/src/yet_another_wizz_cli.egg-info/SOURCES.txt` & `yet_another_wizz_cli-1.2.6/src/yet_another_wizz_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

