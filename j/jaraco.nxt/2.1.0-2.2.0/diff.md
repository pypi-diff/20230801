# Comparing `tmp/jaraco.nxt-2.1.0.tar.gz` & `tmp/jaraco.nxt-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.nxt-2.1.0.tar", last modified: Tue Feb  2 00:49:47 2021, max compression
+gzip compressed data, was "jaraco.nxt-2.2.0.tar", last modified: Tue Aug  1 01:10:04 2023, max compression
```

## Comparing `jaraco.nxt-2.1.0.tar` & `jaraco.nxt-2.2.0.tar`

### file list

```diff
@@ -1,51 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 00:49:47.416756 jaraco.nxt-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (117)       50 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (117)      136 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 00:49:47.412756 jaraco.nxt-2.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 00:49:47.412756 jaraco.nxt-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (117)      497 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/.github/workflows/automerge.yml
--rw-r--r--   0 runner    (1001) docker     (117)     1030 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (117)      175 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (117)       79 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (117)     1346 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (117)     1050 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (117)     2956 2021-02-02 00:49:47.416756 jaraco.nxt-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (117)     1934 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 00:49:47.416756 jaraco.nxt-2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (117)      756 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (117)       81 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (117)      294 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (117)     1084 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/docs/license.txt
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 00:49:47.416756 jaraco.nxt-2.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (117)      223 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/examples/cycle_motor_a.py
--rw-r--r--   0 runner    (1001) docker     (117)      224 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/examples/cycle_motor_b.py
--rw-r--r--   0 runner    (1001) docker     (117)     4215 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/examples/drive_around_table.py
--rw-r--r--   0 runner    (1001) docker     (117)      317 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/examples/get_battery_voltage.py
--rw-r--r--   0 runner    (1001) docker     (117)      174 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/examples/locate-device.py
--rw-r--r--   0 runner    (1001) docker     (117)     1398 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/examples/read_input.py
--rw-r--r--   0 runner    (1001) docker     (117)     1101 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/examples/sync_motors.py
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 00:49:47.412756 jaraco.nxt-2.1.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 00:49:47.416756 jaraco.nxt-2.1.0/jaraco/nxt/
--rw-r--r--   0 runner    (1001) docker     (117)     2663 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/jaraco/nxt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (117)     3007 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/jaraco/nxt/_enum.py
--rw-r--r--   0 runner    (1001) docker     (117)     5173 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/jaraco/nxt/controller.py
--rw-r--r--   0 runner    (1001) docker     (117)    15391 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/jaraco/nxt/messages.py
--rw-r--r--   0 runner    (1001) docker     (117)      887 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/jaraco/nxt/routine.py
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 00:49:47.416756 jaraco.nxt-2.1.0/jaraco.nxt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (117)     2956 2021-02-02 00:49:47.000000 jaraco.nxt-2.1.0/jaraco.nxt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (117)      853 2021-02-02 00:49:47.000000 jaraco.nxt-2.1.0/jaraco.nxt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (117)        1 2021-02-02 00:49:47.000000 jaraco.nxt-2.1.0/jaraco.nxt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (117)       69 2021-02-02 00:49:47.000000 jaraco.nxt-2.1.0/jaraco.nxt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (117)      276 2021-02-02 00:49:47.000000 jaraco.nxt-2.1.0/jaraco.nxt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (117)       21 2021-02-02 00:49:47.000000 jaraco.nxt-2.1.0/jaraco.nxt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (117)       37 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (117)      367 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (117)      333 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (117)      252 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/release.howto
--rw-r--r--   0 runner    (1001) docker     (117)     1137 2021-02-02 00:49:47.416756 jaraco.nxt-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (117)       92 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (117)    10139 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/skeleton.md
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 00:49:47.416756 jaraco.nxt-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (117)      323 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/tests/readme.txt
--rw-r--r--   0 runner    (1001) docker     (117)      541 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/tests/test_parse_messages.py
--rw-r--r--   0 runner    (1001) docker     (117)      719 2021-02-02 00:49:29.000000 jaraco.nxt-2.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:10:04.474887 jaraco.nxt-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:10:04.466887 jaraco.nxt-2.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:10:04.466887 jaraco.nxt-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-01 01:10:04.474887 jaraco.nxt-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:10:04.466887 jaraco.nxt-2.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/docs/license.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:10:04.470887 jaraco.nxt-2.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/examples/cycle_motor_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/examples/cycle_motor_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/examples/drive_around_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/examples/get_battery_voltage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/examples/locate-device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/examples/read_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/examples/sync_motors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:10:04.458887 jaraco.nxt-2.2.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:10:04.474887 jaraco.nxt-2.2.0/jaraco/nxt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/jaraco/nxt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/jaraco/nxt/_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/jaraco/nxt/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15391 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/jaraco/nxt/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/jaraco/nxt/routine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:10:04.470887 jaraco.nxt-2.2.0/jaraco.nxt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-01 01:10:04.000000 jaraco.nxt-2.2.0/jaraco.nxt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-01 01:10:04.000000 jaraco.nxt-2.2.0/jaraco.nxt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 01:10:04.000000 jaraco.nxt-2.2.0/jaraco.nxt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-01 01:10:04.000000 jaraco.nxt-2.2.0/jaraco.nxt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-01 01:10:04.000000 jaraco.nxt-2.2.0/jaraco.nxt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 01:10:04.000000 jaraco.nxt-2.2.0/jaraco.nxt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/release.howto
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-01 01:10:04.474887 jaraco.nxt-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:10:04.474887 jaraco.nxt-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/tests/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/tests/test_parse_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-01 01:09:44.000000 jaraco.nxt-2.2.0/tox.ini
```

### Comparing `jaraco.nxt-2.1.0/CHANGES.rst` & `jaraco.nxt-2.2.0/NEWS.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v2.2.0
+======
+
+Features
+--------
+
+- Require Python 3.8 or later.
+
+
 v2.1.0
 ======
 
 Refreshed package. Use PEP 420 for namespace package.
 
 2.0
 ===
```

### Comparing `jaraco.nxt-2.1.0/LICENSE` & `jaraco.nxt-2.2.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jaraco.nxt-2.1.0/PKG-INFO` & `jaraco.nxt-2.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,73 +1,74 @@
 Metadata-Version: 2.1
 Name: jaraco.nxt
-Version: 2.1.0
+Version: 2.2.0
 Summary: Logo Mindstorms NXT Routines
 Home-page: https://github.com/jaraco/jaraco.nxt
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
-License: UNKNOWN
-Description: .. image:: https://img.shields.io/pypi/v/jaraco.nxt.svg
-           :target: `PyPI link`_
-        
-        .. image:: https://img.shields.io/pypi/pyversions/jaraco.nxt.svg
-           :target: `PyPI link`_
-        
-        .. _PyPI link: https://pypi.org/project/jaraco.nxt
-        
-        .. image:: https://github.com/jaraco/jaraco.nxt/workflows/tests/badge.svg
-           :target: https://github.com/jaraco/jaraco.nxt/actions?query=workflow%3A%22tests%22
-           :alt: tests
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-           :target: https://github.com/psf/black
-           :alt: Code style: Black
-        
-        .. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-        ..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
-        
-        .. -*- restructuredtext -*-
-        
-        LEGO Mindstorms NXT Bluetooth API in Python
-        
-        Overview
-        --------
-        
-        ``jaraco.nxt`` implements the LEGO Mindstorms NXT Bluetooth API in Python.
-        
-        The ``jaraco.nxt`` library also can take advantage of the `jaraco input
-        <https://pypi.org/project/jaraco.input>`_
-        package.  To include it as part of the install, use the command
-        ``pip install jaraco.nxt[input]``.
-        
-        Getting Started
-        ---------------
-        
-        ``jaraco.nxt`` provides a message class for sending and receiving messages
-        with the Lego NXT device.  First pair the device with your PC by following
-        the instructions included with the device.  Then, determine the COM port
-        to which it is connected.  The `hello world example
-        <https://github.com/jaraco/jaraco.nxt/tree/master/examples/get_battery_voltage.py>`_
-        is to retrieve the battery
-        voltage.  `Browse the other examples
-        <https://github.com/jaraco/jaraco.nxt/tree/master/examples/>`_ for
-        more inspiration.
-        
-        For more information, read the docstrings of the modules in the packages.
-        
-        Modules of interest are
-        
-        * jaraco.nxt.messages: implements the messages defined by
-          the NXT Bluetooth protocol.
-        * jaraco.nxt.controller: demonstrates how to link input from
-          a joystick to messages controlling the motors.  Uses jaraco.input.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 Provides-Extra: input
+License-File: LICENSE
+
+.. image:: https://img.shields.io/pypi/v/jaraco.nxt.svg
+   :target: https://pypi.org/project/jaraco.nxt
+
+.. image:: https://img.shields.io/pypi/pyversions/jaraco.nxt.svg
+
+.. image:: https://github.com/jaraco/jaraco.nxt/workflows/tests/badge.svg
+   :target: https://github.com/jaraco/jaraco.nxt/actions?query=workflow%3A%22tests%22
+   :alt: tests
+
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Code style: Black
+
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
+
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
+   :target: https://blog.jaraco.com/skeleton
+
+LEGO Mindstorms NXT Bluetooth API in Python
+
+Overview
+--------
+
+``jaraco.nxt`` implements the LEGO Mindstorms NXT Bluetooth API in Python.
+
+The ``jaraco.nxt`` library also can take advantage of the `jaraco input
+<https://pypi.org/project/jaraco.input>`_
+package.  To include it as part of the install, use the command
+``pip install jaraco.nxt[input]``.
+
+Getting Started
+---------------
+
+``jaraco.nxt`` provides a message class for sending and receiving messages
+with the Lego NXT device.  First pair the device with your PC by following
+the instructions included with the device.  Then, determine the COM port
+to which it is connected.  The `hello world example
+<https://github.com/jaraco/jaraco.nxt/tree/master/examples/get_battery_voltage.py>`_
+is to retrieve the battery
+voltage.  `Browse the other examples
+<https://github.com/jaraco/jaraco.nxt/tree/master/examples/>`_ for
+more inspiration.
+
+For more information, read the docstrings of the modules in the packages.
+
+Modules of interest are
+
+* jaraco.nxt.messages: implements the messages defined by
+  the NXT Bluetooth protocol.
+* jaraco.nxt.controller: demonstrates how to link input from
+  a joystick to messages controlling the motors.  Uses jaraco.input.
```

### Comparing `jaraco.nxt-2.1.0/README.rst` & `jaraco.nxt-2.2.0/jaraco.nxt.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,47 @@
+Metadata-Version: 2.1
+Name: jaraco.nxt
+Version: 2.2.0
+Summary: Logo Mindstorms NXT Routines
+Home-page: https://github.com/jaraco/jaraco.nxt
+Author: Jason R. Coombs
+Author-email: jaraco@jaraco.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8
+Provides-Extra: testing
+Provides-Extra: docs
+Provides-Extra: input
+License-File: LICENSE
+
 .. image:: https://img.shields.io/pypi/v/jaraco.nxt.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/jaraco.nxt
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.nxt.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/jaraco.nxt
 
 .. image:: https://github.com/jaraco/jaraco.nxt/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.nxt/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. -*- restructuredtext -*-
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
+   :target: https://blog.jaraco.com/skeleton
 
 LEGO Mindstorms NXT Bluetooth API in Python
 
 Overview
 --------
 
 ``jaraco.nxt`` implements the LEGO Mindstorms NXT Bluetooth API in Python.
```

### Comparing `jaraco.nxt-2.1.0/docs/license.txt` & `jaraco.nxt-2.2.0/docs/license.txt`

 * *Files identical despite different names*

### Comparing `jaraco.nxt-2.1.0/examples/drive_around_table.py` & `jaraco.nxt-2.2.0/examples/drive_around_table.py`

 * *Files identical despite different names*

### Comparing `jaraco.nxt-2.1.0/examples/read_input.py` & `jaraco.nxt-2.2.0/examples/read_input.py`

 * *Files identical despite different names*

### Comparing `jaraco.nxt-2.1.0/examples/sync_motors.py` & `jaraco.nxt-2.2.0/examples/sync_motors.py`

 * *Files identical despite different names*

### Comparing `jaraco.nxt-2.1.0/jaraco/nxt/__init__.py` & `jaraco.nxt-2.2.0/jaraco/nxt/__init__.py`

 * *Files identical despite different names*

### Comparing `jaraco.nxt-2.1.0/jaraco/nxt/_enum.py` & `jaraco.nxt-2.2.0/jaraco/nxt/_enum.py`

 * *Files identical despite different names*

### Comparing `jaraco.nxt-2.1.0/jaraco/nxt/controller.py` & `jaraco.nxt-2.2.0/jaraco/nxt/controller.py`

 * *Files identical despite different names*

### Comparing `jaraco.nxt-2.1.0/jaraco/nxt/messages.py` & `jaraco.nxt-2.2.0/jaraco/nxt/messages.py`

 * *Files identical despite different names*

### Comparing `jaraco.nxt-2.1.0/jaraco/nxt/routine.py` & `jaraco.nxt-2.2.0/jaraco/nxt/routine.py`

 * *Files identical despite different names*

### Comparing `jaraco.nxt-2.1.0/jaraco.nxt.egg-info/PKG-INFO` & `jaraco.nxt-2.2.0/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,56 @@
-Metadata-Version: 2.1
-Name: jaraco.nxt
-Version: 2.1.0
-Summary: Logo Mindstorms NXT Routines
-Home-page: https://github.com/jaraco/jaraco.nxt
-Author: Jason R. Coombs
-Author-email: jaraco@jaraco.com
-License: UNKNOWN
-Description: .. image:: https://img.shields.io/pypi/v/jaraco.nxt.svg
-           :target: `PyPI link`_
-        
-        .. image:: https://img.shields.io/pypi/pyversions/jaraco.nxt.svg
-           :target: `PyPI link`_
-        
-        .. _PyPI link: https://pypi.org/project/jaraco.nxt
-        
-        .. image:: https://github.com/jaraco/jaraco.nxt/workflows/tests/badge.svg
-           :target: https://github.com/jaraco/jaraco.nxt/actions?query=workflow%3A%22tests%22
-           :alt: tests
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-           :target: https://github.com/psf/black
-           :alt: Code style: Black
-        
-        .. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-        ..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
-        
-        .. -*- restructuredtext -*-
-        
-        LEGO Mindstorms NXT Bluetooth API in Python
-        
-        Overview
-        --------
-        
-        ``jaraco.nxt`` implements the LEGO Mindstorms NXT Bluetooth API in Python.
-        
-        The ``jaraco.nxt`` library also can take advantage of the `jaraco input
-        <https://pypi.org/project/jaraco.input>`_
-        package.  To include it as part of the install, use the command
-        ``pip install jaraco.nxt[input]``.
-        
-        Getting Started
-        ---------------
-        
-        ``jaraco.nxt`` provides a message class for sending and receiving messages
-        with the Lego NXT device.  First pair the device with your PC by following
-        the instructions included with the device.  Then, determine the COM port
-        to which it is connected.  The `hello world example
-        <https://github.com/jaraco/jaraco.nxt/tree/master/examples/get_battery_voltage.py>`_
-        is to retrieve the battery
-        voltage.  `Browse the other examples
-        <https://github.com/jaraco/jaraco.nxt/tree/master/examples/>`_ for
-        more inspiration.
-        
-        For more information, read the docstrings of the modules in the packages.
-        
-        Modules of interest are
-        
-        * jaraco.nxt.messages: implements the messages defined by
-          the NXT Bluetooth protocol.
-        * jaraco.nxt.controller: demonstrates how to link input from
-          a joystick to messages controlling the motors.  Uses jaraco.input.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
-Provides-Extra: testing
-Provides-Extra: docs
-Provides-Extra: input
+.. image:: https://img.shields.io/pypi/v/jaraco.nxt.svg
+   :target: https://pypi.org/project/jaraco.nxt
+
+.. image:: https://img.shields.io/pypi/pyversions/jaraco.nxt.svg
+
+.. image:: https://github.com/jaraco/jaraco.nxt/workflows/tests/badge.svg
+   :target: https://github.com/jaraco/jaraco.nxt/actions?query=workflow%3A%22tests%22
+   :alt: tests
+
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Code style: Black
+
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
+
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
+   :target: https://blog.jaraco.com/skeleton
+
+LEGO Mindstorms NXT Bluetooth API in Python
+
+Overview
+--------
+
+``jaraco.nxt`` implements the LEGO Mindstorms NXT Bluetooth API in Python.
+
+The ``jaraco.nxt`` library also can take advantage of the `jaraco input
+<https://pypi.org/project/jaraco.input>`_
+package.  To include it as part of the install, use the command
+``pip install jaraco.nxt[input]``.
+
+Getting Started
+---------------
+
+``jaraco.nxt`` provides a message class for sending and receiving messages
+with the Lego NXT device.  First pair the device with your PC by following
+the instructions included with the device.  Then, determine the COM port
+to which it is connected.  The `hello world example
+<https://github.com/jaraco/jaraco.nxt/tree/master/examples/get_battery_voltage.py>`_
+is to retrieve the battery
+voltage.  `Browse the other examples
+<https://github.com/jaraco/jaraco.nxt/tree/master/examples/>`_ for
+more inspiration.
+
+For more information, read the docstrings of the modules in the packages.
+
+Modules of interest are
+
+* jaraco.nxt.messages: implements the messages defined by
+  the NXT Bluetooth protocol.
+* jaraco.nxt.controller: demonstrates how to link input from
+  a joystick to messages controlling the motors.  Uses jaraco.input.
```

### Comparing `jaraco.nxt-2.1.0/jaraco.nxt.egg-info/SOURCES.txt` & `jaraco.nxt-2.2.0/jaraco.nxt.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 .coveragerc
-.flake8
+.editorconfig
 .pre-commit-config.yaml
-.readthedocs.yml
-CHANGES.rst
+.readthedocs.yaml
 LICENSE
+NEWS.rst
 README.rst
 mypy.ini
 pyproject.toml
 pytest.ini
 release.howto
 setup.cfg
-setup.py
-skeleton.md
+towncrier.toml
 tox.ini
-.github/workflows/automerge.yml
+.github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
 docs/license.txt
 examples/cycle_motor_a.py
 examples/cycle_motor_b.py
```

### Comparing `jaraco.nxt-2.1.0/setup.cfg` & `jaraco.nxt-2.2.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 [metadata]
-license_files = 
-	LICENSE
 name = jaraco.nxt
 author = Jason R. Coombs
 author_email = jaraco@jaraco.com
 description = Logo Mindstorms NXT Routines
 long_description = file:README.rst
 url = https://github.com/jaraco/jaraco.nxt
 classifiers = 
@@ -13,38 +11,42 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.6
+python_requires = >=3.8
 install_requires = 
 	pyserial>=2.4
-setup_requires = setuptools_scm[toml] >= 3.4.1
 
 [options.packages.find]
 exclude = 
 	build*
+	dist*
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
-	pytest >= 3.5, !=3.7.3
-	pytest-checkdocs >= 1.2.3
-	pytest-flake8
-	pytest-black >= 0.3.7; python_implementation != "PyPy"
+	pytest >= 6
+	pytest-checkdocs >= 2.4
+	pytest-black >= 0.3.7; \
+	python_implementation != "PyPy"
 	pytest-cov
-	pytest-mypy; python_implementation != "PyPy"
-	pytest-enabler
+	pytest-mypy >= 0.9.1; \
+	python_implementation != "PyPy"
+	pytest-enabler >= 2.2
+	pytest-ruff
 docs = 
-	sphinx
-	jaraco.packaging >= 8.2
+	sphinx >= 3.5
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
 input = 
 	jaraco.input>=1.1dev
 
 [options.entry_points]
 console_scripts = 
 	nxt-control = jaraco.nxt.controller:serve_forever
```

### Comparing `jaraco.nxt-2.1.0/tests/test_parse_messages.py` & `jaraco.nxt-2.2.0/tests/test_parse_messages.py`

 * *Files identical despite different names*

