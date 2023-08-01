# Comparing `tmp/RSFile-3.0.tar.gz` & `tmp/RSFile-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RSFile-3.0.tar", last modified: Sun Jun 26 21:22:40 2022, max compression
+gzip compressed data, was "RSFile-3.1.tar", last modified: Tue Aug  1 19:28:57 2023, max compression
```

## Comparing `RSFile-3.0.tar` & `RSFile-3.1.tar`

### file list

```diff
@@ -1,56 +1,60 @@
-drwxrwxrwx   0        0        0        0 2022-06-26 21:22:40.182738 RSFile-3.0/
--rw-rw-rw-   0        0        0     3607 2022-06-26 11:28:51.000000 RSFile-3.0/CHANGELOG.rst
--rw-rw-rw-   0        0        0     3252 2022-06-26 12:38:04.000000 RSFile-3.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       22 2016-06-17 15:37:22.000000 RSFile-3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2929 2022-06-26 21:22:40.182738 RSFile-3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1783 2022-06-26 21:13:28.000000 RSFile-3.0/README.rst
-drwxrwxrwx   0        0        0        0 2022-06-26 21:22:40.085505 RSFile-3.0/RSFile.egg-info/
--rw-rw-rw-   0        0        0     2929 2022-06-26 21:22:39.000000 RSFile-3.0/RSFile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1484 2022-06-26 21:22:39.000000 RSFile-3.0/RSFile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-26 21:22:39.000000 RSFile-3.0/RSFile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-06-26 21:22:39.000000 RSFile-3.0/RSFile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        4 2022-06-26 11:28:54.000000 RSFile-3.0/VERSION
-drwxrwxrwx   0        0        0        0 2022-06-26 21:22:40.105497 RSFile-3.0/rsfile/
--rw-rw-rw-   0        0        0      349 2022-06-26 13:20:25.000000 RSFile-3.0/rsfile/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-26 21:22:40.130486 RSFile-3.0/rsfile/rsbackend/
--rw-rw-rw-   0        0        0       24 2022-06-26 13:20:25.000000 RSFile-3.0/rsfile/rsbackend/__init__.py
--rw-rw-rw-   0        0        0     2831 2022-06-26 13:20:25.000000 RSFile-3.0/rsfile/rsbackend/_utilities.py
--rw-rw-rw-   0        0        0      222 2022-06-26 12:43:15.000000 RSFile-3.0/rsfile/rsbackend/raw_unix_defines.py
--rw-rw-rw-   0        0        0     5560 2022-06-26 13:20:26.000000 RSFile-3.0/rsfile/rsbackend/raw_win32_ctypes.py
--rw-rw-rw-   0        0        0     1042 2022-06-22 19:16:50.000000 RSFile-3.0/rsfile/rsbackend/raw_win32_defines.py
--rw-rw-rw-   0        0        0     1401 2022-06-26 13:20:25.000000 RSFile-3.0/rsfile/rsbackend/unix_stdlib.py
--rw-rw-rw-   0        0        0     9801 2022-06-26 13:20:26.000000 RSFile-3.0/rsfile/rsbackend/windows_ctypes.py
--rw-rw-rw-   0        0        0     3441 2022-06-26 13:20:25.000000 RSFile-3.0/rsfile/rsbackend/windows_pywin32.py
--rw-rw-rw-   0        0        0     1487 2022-06-26 13:20:25.000000 RSFile-3.0/rsfile/rsfile_definitions.py
--rw-rw-rw-   0        0        0    21191 2022-06-26 13:20:26.000000 RSFile-3.0/rsfile/rsfile_factories.py
--rw-rw-rw-   0        0        0    11184 2022-06-26 13:20:26.000000 RSFile-3.0/rsfile/rsfile_registries.py
--rw-rw-rw-   0        0        0     6342 2022-06-26 13:20:25.000000 RSFile-3.0/rsfile/rsfile_streams.py
--rw-rw-rw-   0        0        0     5823 2022-06-26 17:12:29.000000 RSFile-3.0/rsfile/rsfile_utilities.py
--rw-rw-rw-   0        0        0    26354 2022-06-26 19:19:04.000000 RSFile-3.0/rsfile/rsfileio_abstract.py
--rw-rw-rw-   0        0        0    11116 2022-06-26 18:18:05.000000 RSFile-3.0/rsfile/rsfileio_unix.py
--rw-rw-rw-   0        0        0    17372 2022-06-26 13:20:26.000000 RSFile-3.0/rsfile/rsfileio_windows.py
--rw-rw-rw-   0        0        0    12357 2022-06-26 13:20:26.000000 RSFile-3.0/rsfile/rsiobase.py
-drwxrwxrwx   0        0        0        0 2022-06-26 21:22:40.155754 RSFile-3.0/rsfile/rstest/
--rw-rw-rw-   0        0        0       24 2022-06-26 13:20:26.000000 RSFile-3.0/rsfile/rstest/__init__.py
--rw-rw-rw-   0        0        0      439 2022-06-26 13:20:26.000000 RSFile-3.0/rsfile/rstest/_fd_inheritance_tester.py
--rw-rw-rw-   0        0        0     1503 2022-06-26 13:20:26.000000 RSFile-3.0/rsfile/rstest/_utilities.py
--rw-rw-rw-   0        0        0    11353 2022-06-26 13:20:26.000000 RSFile-3.0/rsfile/rstest/_worker_process.py
--rw-rw-rw-   0        0        0    10088 2022-06-26 13:20:26.000000 RSFile-3.0/rsfile/rstest/run_iobench.py
-drwxrwxrwx   0        0        0        0 2022-06-26 21:22:40.180739 RSFile-3.0/rsfile/rstest/stdlib/
--rw-rw-rw-   0        0        0       24 2022-06-26 13:20:26.000000 RSFile-3.0/rsfile/rstest/stdlib/__init__.py
--rw-rw-rw-   0        0        0    68544 2022-06-26 13:20:29.000000 RSFile-3.0/rsfile/rstest/stdlib/_pyio_py27_backup.py
--rw-rw-rw-   0        0        0    93280 2022-06-26 13:20:29.000000 RSFile-3.0/rsfile/rstest/stdlib/_pyio_py310_backup.py
--rw-rw-rw-   0        0        0    72836 2022-06-26 13:20:28.000000 RSFile-3.0/rsfile/rstest/stdlib/_pyio_py34_backup.py
--rw-rw-rw-   0        0        0    86699 2022-06-26 13:20:29.000000 RSFile-3.0/rsfile/rstest/stdlib/_pyio_py35_backup.py
--rw-rw-rw-   0        0        0    86952 2022-06-26 13:20:30.000000 RSFile-3.0/rsfile/rstest/stdlib/_pyio_py36_backup.py
--rw-rw-rw-   0        0        0    89909 2022-06-26 13:20:30.000000 RSFile-3.0/rsfile/rstest/stdlib/_pyio_py37_backup.py
--rw-rw-rw-   0        0        0    91930 2022-06-26 13:20:30.000000 RSFile-3.0/rsfile/rstest/stdlib/_pyio_py38_backup.py
--rw-rw-rw-   0        0        0    92165 2022-06-26 13:20:30.000000 RSFile-3.0/rsfile/rstest/stdlib/_pyio_py39_backup.py
--rw-rw-rw-   0        0        0    16991 2022-06-26 13:20:29.000000 RSFile-3.0/rsfile/rstest/stdlib/iobench.py
--rw-rw-rw-   0        0        0     2449 2022-06-26 13:20:29.000000 RSFile-3.0/rsfile/rstest/test_backend_utilities.py
--rw-rw-rw-   0        0        0    27152 2022-06-26 18:12:36.000000 RSFile-3.0/rsfile/rstest/test_rsfile_locking.py
--rw-rw-rw-   0        0        0    14630 2022-06-26 13:20:29.000000 RSFile-3.0/rsfile/rstest/test_rsfile_retrocompatibility.py
--rw-rw-rw-   0        0        0     6482 2022-06-26 13:20:29.000000 RSFile-3.0/rsfile/rstest/test_rsfile_stdlib.py
--rw-rw-rw-   0        0        0    45931 2022-06-26 18:21:59.000000 RSFile-3.0/rsfile/rstest/test_rsfile_streams.py
--rw-rw-rw-   0        0        0      137 2022-06-26 21:22:40.185733 RSFile-3.0/setup.cfg
--rw-rw-rw-   0        0        0     1482 2022-06-26 12:45:27.000000 RSFile-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:28:57.694974 RSFile-3.1/
+-rw-rw-rw-   0        0        0     4068 2023-08-01 17:39:38.000000 RSFile-3.1/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     2926 2023-08-01 16:01:40.000000 RSFile-3.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1069 2022-09-01 15:41:00.000000 RSFile-3.1/License.txt
+-rw-rw-rw-   0        0        0     2970 2023-08-01 19:28:57.693974 RSFile-3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1799 2023-08-01 17:45:48.000000 RSFile-3.1/README.rst
+-rw-rw-rw-   0        0        0     1596 2023-08-01 15:47:39.000000 RSFile-3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 19:28:57.694974 RSFile-3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 19:28:57.659946 RSFile-3.1/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 19:28:57.670452 RSFile-3.1/src/RSFile.egg-info/
+-rw-rw-rw-   0        0        0     2970 2023-08-01 19:28:57.000000 RSFile-3.1/src/RSFile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1818 2023-08-01 19:28:57.000000 RSFile-3.1/src/RSFile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 19:28:57.000000 RSFile-3.1/src/RSFile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-08-01 19:28:57.000000 RSFile-3.1/src/RSFile.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 19:28:57.675954 RSFile-3.1/src/rsfile/
+-rw-rw-rw-   0        0        0      349 2022-06-26 13:20:25.000000 RSFile-3.1/src/rsfile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:28:57.679957 RSFile-3.1/src/rsfile/rsbackend/
+-rw-rw-rw-   0        0        0       24 2022-06-26 13:20:25.000000 RSFile-3.1/src/rsfile/rsbackend/__init__.py
+-rw-rw-rw-   0        0        0     2831 2022-06-26 13:20:25.000000 RSFile-3.1/src/rsfile/rsbackend/_utilities.py
+-rw-rw-rw-   0        0        0      222 2022-06-26 12:43:15.000000 RSFile-3.1/src/rsfile/rsbackend/raw_unix_defines.py
+-rw-rw-rw-   0        0        0     5560 2022-06-26 13:20:26.000000 RSFile-3.1/src/rsfile/rsbackend/raw_win32_ctypes.py
+-rw-rw-rw-   0        0        0     1042 2022-06-22 19:16:50.000000 RSFile-3.1/src/rsfile/rsbackend/raw_win32_defines.py
+-rw-rw-rw-   0        0        0     1401 2022-06-26 13:20:25.000000 RSFile-3.1/src/rsfile/rsbackend/unix_stdlib.py
+-rw-rw-rw-   0        0        0     9976 2023-08-01 14:15:20.000000 RSFile-3.1/src/rsfile/rsbackend/windows_ctypes.py
+-rw-rw-rw-   0        0        0     3441 2022-06-26 13:20:25.000000 RSFile-3.1/src/rsfile/rsbackend/windows_pywin32.py
+-rw-rw-rw-   0        0        0     1573 2023-07-31 21:17:04.000000 RSFile-3.1/src/rsfile/rsfile_definitions.py
+-rw-rw-rw-   0        0        0    21191 2022-06-26 13:20:26.000000 RSFile-3.1/src/rsfile/rsfile_factories.py
+-rw-rw-rw-   0        0        0    11184 2022-06-26 13:20:26.000000 RSFile-3.1/src/rsfile/rsfile_registries.py
+-rw-rw-rw-   0        0        0     6342 2022-06-26 13:20:25.000000 RSFile-3.1/src/rsfile/rsfile_streams.py
+-rw-rw-rw-   0        0        0     5823 2022-06-26 17:12:29.000000 RSFile-3.1/src/rsfile/rsfile_utilities.py
+-rw-rw-rw-   0        0        0    26350 2023-08-01 08:56:19.000000 RSFile-3.1/src/rsfile/rsfileio_abstract.py
+-rw-rw-rw-   0        0        0    11116 2022-06-26 18:18:05.000000 RSFile-3.1/src/rsfile/rsfileio_unix.py
+-rw-rw-rw-   0        0        0    19397 2023-08-01 14:44:06.000000 RSFile-3.1/src/rsfile/rsfileio_windows.py
+-rw-rw-rw-   0        0        0    12357 2022-06-26 13:20:26.000000 RSFile-3.1/src/rsfile/rsiobase.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:28:57.685970 RSFile-3.1/src/rsfile/rstest/
+-rw-rw-rw-   0        0        0       24 2022-06-26 13:20:26.000000 RSFile-3.1/src/rsfile/rstest/__init__.py
+-rw-rw-rw-   0        0        0      439 2022-06-26 13:20:26.000000 RSFile-3.1/src/rsfile/rstest/_fd_inheritance_tester.py
+-rw-rw-rw-   0        0        0     1503 2023-08-01 14:19:39.000000 RSFile-3.1/src/rsfile/rstest/_utilities.py
+-rw-rw-rw-   0        0        0    11353 2022-06-26 13:20:26.000000 RSFile-3.1/src/rsfile/rstest/_worker_process.py
+-rw-rw-rw-   0        0        0    18127 2023-08-01 16:30:21.000000 RSFile-3.1/src/rsfile/rstest/run_iobench.py
+drwxrwxrwx   0        0        0        0 2023-08-01 19:28:57.693974 RSFile-3.1/src/rsfile/rstest/stdlib/
+-rw-rw-rw-   0        0        0       24 2022-06-26 13:20:26.000000 RSFile-3.1/src/rsfile/rstest/stdlib/__init__.py
+-rw-rw-rw-   0        0        0    68544 2022-06-26 13:20:29.000000 RSFile-3.1/src/rsfile/rstest/stdlib/_pyio_py27_backup.py
+-rw-rw-rw-   0        0        0    93280 2022-06-26 13:20:29.000000 RSFile-3.1/src/rsfile/rstest/stdlib/_pyio_py310_backup.py
+-rw-rw-rw-   0        0        0    96745 2023-02-07 15:54:22.000000 RSFile-3.1/src/rsfile/rstest/stdlib/_pyio_py311_backup.py
+-rw-rw-rw-   0        0        0    96131 2023-07-11 11:56:58.000000 RSFile-3.1/src/rsfile/rstest/stdlib/_pyio_py312_backup.py
+-rw-rw-rw-   0        0        0    72836 2022-06-26 13:20:28.000000 RSFile-3.1/src/rsfile/rstest/stdlib/_pyio_py34_backup.py
+-rw-rw-rw-   0        0        0    86699 2022-06-26 13:20:29.000000 RSFile-3.1/src/rsfile/rstest/stdlib/_pyio_py35_backup.py
+-rw-rw-rw-   0        0        0    86952 2022-06-26 13:20:30.000000 RSFile-3.1/src/rsfile/rstest/stdlib/_pyio_py36_backup.py
+-rw-rw-rw-   0        0        0    89909 2022-06-26 13:20:30.000000 RSFile-3.1/src/rsfile/rstest/stdlib/_pyio_py37_backup.py
+-rw-rw-rw-   0        0        0    91930 2022-06-26 13:20:30.000000 RSFile-3.1/src/rsfile/rstest/stdlib/_pyio_py38_backup.py
+-rw-rw-rw-   0        0        0    92165 2022-06-26 13:20:30.000000 RSFile-3.1/src/rsfile/rstest/stdlib/_pyio_py39_backup.py
+-rw-rw-rw-   0        0        0    17502 2023-07-31 21:26:04.000000 RSFile-3.1/src/rsfile/rstest/stdlib/iobench.py
+-rw-rw-rw-   0        0        0   181654 2023-02-07 15:54:22.000000 RSFile-3.1/src/rsfile/rstest/stdlib/test_io_py311.py
+-rw-rw-rw-   0        0        0   185068 2023-07-11 11:57:00.000000 RSFile-3.1/src/rsfile/rstest/stdlib/test_io_py312.py
+-rw-rw-rw-   0        0        0     2449 2022-06-26 13:20:29.000000 RSFile-3.1/src/rsfile/rstest/test_backend_utilities.py
+-rw-rw-rw-   0        0        0    27152 2022-06-26 18:12:36.000000 RSFile-3.1/src/rsfile/rstest/test_rsfile_locking.py
+-rw-rw-rw-   0        0        0    14630 2022-06-26 13:20:29.000000 RSFile-3.1/src/rsfile/rstest/test_rsfile_retrocompatibility.py
+-rw-rw-rw-   0        0        0     7017 2023-08-01 17:02:15.000000 RSFile-3.1/src/rsfile/rstest/test_rsfile_stdlib.py
+-rw-rw-rw-   0        0        0    45963 2023-07-31 21:36:49.000000 RSFile-3.1/src/rsfile/rstest/test_rsfile_streams.py
```

### Comparing `RSFile-3.0/CHANGELOG.rst` & `RSFile-3.1/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,21 @@
 
+
+Rsfile 3.1
+============
+
+* Add support for python 3.11 and 3.12b
+* Drop compatibility for Python 3.6 included
+* Remove support for "U" open() mode in Python>=3.11
+* Fix bugs regarding non-blocking pipes (see current troubles on https://github.com/python/cpython/issues/57531)
+* Switch to pyproject.toml package configuration and new "src/" layout
+* Switch to Alabaster sphinx doc template
+* Add .readthedocs.yaml configuration for Read The Docs
+
+
 Rsfile 3.0
 ============
 
 * Drop compatibility for Python 2.7 to 3.5 included
 * Add support for python 3.8, 3.9, and 3.10
```

### Comparing `RSFile-3.0/CONTRIBUTING.rst` & `RSFile-3.1/CONTRIBUTING.rst`

 * *Files 12% similar despite different names*

```diff
@@ -4,47 +4,43 @@
 RSFile welcomes contributions like Reporting Bugs and Pull Requests.
 
 
 TESTING
 ++++++++++
 
 
-The test suites of RSFile can be run against any compatible python2/3 interpreter installed on your system.
+The test suites of RSFile can be run against any compatible python3 interpreter installed on your system.
 Since they reuse many stdlib testcases, you must have the "python test suite" installed for the selected interpreter version, else only a subset of RSFile tests will be run.
 On Windows this test suite must have been selected during install, on Linux you must install separate packages like "libpythonX.Y-testsuite", etc.
 
 .. note::
-    Some tests, like those concerning open() mode equivalences, or locking, are very long to execute,
-    so as long as the test process consumes CPU, they're probably still working normally. Some tests, mainly
+    Some tests, like those concerning open() mode equivalences, or locking, are long to execute,
+    so as long as the test process consumes CPU, they're probably still working normally. Other tests, mainly
     concerning large files, are disabled by default and must be manually enabled by editing flags in test
-    files.
+    files (see ENABLE_LARGE_FILE_TESTS variable).
 
 
 
 Testing using TOX
 ---------------------
 
-- install the latest versions of pip, virtualenv and tox
-- run tox from the folder containing setup.py (possibly with "-e pyXY" or "-e doc" to select a specific environement):
+- Pnstall the latest versions of pip, virtualenv and tox
+- Run tox from the root folder (possibly with "-e pyXY" or "-e doc" to select a specific environment):
 
 $ tox
 
 This will install RSFile into a virtual environment, and launch the test suites.
 
-If tox fails when creating py35 environment on windows ("The program can't start because VCRUNTIME140.dll is missing from your computer."), you might need to use "virtualenv-rewrite" instead of "virtualenv", for details see https://github.com/pypa/virtualenv/issues/796
-
 
 Testing manually
 -----------------
 
-To manually launch the test suites against a specific "python" interpreter, use the different commands visible in the "tox.ini", in the form **python -m rsfile.rstest.xxxxxxx**
-
-Note that these *.py test files can't all be executed inside the same runner process, since they monkey-patch their python environment differently.
+To manually launch the test suites against a specific "python" interpreter, use the different commands visible in the "tox.ini", in the form **python -m rsfile.rstest.xxxxxxx**. The "src/" folder must be in your current python paths (ex. by using PYTHONPATH environment variable, or by pip-installing the repository in "editable" mode).
 
-Also, double-check that the "rsfile" package imported is well the one you meant, since the current working directory is usually automatically added by python to your "sys.path" on launch.
+Note that these *.py test files can't all be executed inside the same runner process (ex. using pytest), since they monkey-patch their python environment differently.
 
 If you have installed python-tabulate (https://pypi.python.org/pypi/tabulate), the retrocompatibility test will display a table listing the different file opening modes, and their features.
 
 
 Checking code coverage
 ------------------------
 
@@ -59,20 +55,16 @@
 +++++++++++++
 
 To launch performance benchmarks, tweak the flags in rsfile/rstest/run_iobench.py to your liking,
 maybe modify rsfileio_win32.py to force a specific low-level backend (if on Windows), and then run:
 
     $ python -m  rsfile.rstest.run_iobench
 
-Again, be aware of possible confusion between an installed and a "current dir" rsfile packages.
-
 
 BUILDING
 ++++++++++
 
-To build the rsfile package:
-
-    $ python setup.py sdist --formats=gztar,zip
+To build the rsfile package, use the standard setuptools "build" command: https://setuptools.pypa.io/en/latest/userguide/quickstart.html
 
-No need for `bdist_msi` or the weaker `bdist_wininst`: rsfile is pure-python
+Rsfile is pure-python, so buildings wheels is not necessary.
```

### Comparing `RSFile-3.0/PKG-INFO` & `RSFile-3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: RSFile
-Version: 3.0
+Version: 3.1
 Summary: Advanced I/O file streams with fine-grained locking and creation options
-Home-page: https://github.com/pakal/rsfile
-Author: Pascal Chambon
-Author-email: pythoniks@gmail.com
-License: http://www.opensource.org/licenses/mit-license.php
-Platform: any
+Author-email: Pascal Chambon <pythoniks@gmail.com>
+License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: License.txt
 
 RSFILE
 ================
 
 .. image:: https://ci.appveyor.com/api/projects/status/x002hlal3qwiavsa/branch/master
     :target: https://ci.appveyor.com/project/pakal/rsfile
 
@@ -35,15 +36,15 @@
 
 Locking is performed using actual file record locking capabilities of the OS, not by using separate files/directories as locking markers, or other fragile gimmicks.
 
 .. END OF PART KINDA SHARED WITH SPHINX DOC INDEX ..
 
 Possible use cases for this library: concurrently writing to logs without ending up with garbled data, manipulating sensitive data like disk-based databases, synchronizing heterogeneous producer/consumer processes when multiprocessing semaphores aren't an option, etc.
 
-Tested on Python 3.6+, on windows and unix-like systems. *Should* work with IronPython/Jython/PyPy too, since it uses stdlib utilities and ctypes bridges.
+Tested on CPython3, on windows and unix-like systems. *Should* work with IronPython/Jython/PyPy too, since it uses stdlib utilities and ctypes bridges.
 
 **Read the documentation here: http://rsfile.readthedocs.io/**
 
 
 INSTALL
 ------------
 
@@ -51,21 +52,19 @@
 
     $ pip install rsfile
 
 
 QUICKSTART
 ------------
 
-::
+.. code-block:: python
 
     from rsfile import rsopen
 
     with rsopen("myfile.txt", "w") as f:
-        f.write(u"This string will be veeeeeryyyyy safely written to file.")
+        f.write("This string will be veeeeeryyyyy safely written to file.")
 
     with rsopen("myfile.txt", "WANISB", locking=False, thread_safe=False) as f:
         f.write(b"See the docs for info on these cool new modes and parameters.")
 
 
 See CONTRIBUTING.rst for development advice (testing, benchmarking...)
-
-
```

### Comparing `RSFile-3.0/README.rst` & `RSFile-3.1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Locking is performed using actual file record locking capabilities of the OS, not by using separate files/directories as locking markers, or other fragile gimmicks.
 
 .. END OF PART KINDA SHARED WITH SPHINX DOC INDEX ..
 
 Possible use cases for this library: concurrently writing to logs without ending up with garbled data, manipulating sensitive data like disk-based databases, synchronizing heterogeneous producer/consumer processes when multiprocessing semaphores aren't an option, etc.
 
-Tested on Python 3.6+, on windows and unix-like systems. *Should* work with IronPython/Jython/PyPy too, since it uses stdlib utilities and ctypes bridges.
+Tested on CPython3, on windows and unix-like systems. *Should* work with IronPython/Jython/PyPy too, since it uses stdlib utilities and ctypes bridges.
 
 **Read the documentation here: http://rsfile.readthedocs.io/**
 
 
 INSTALL
 ------------
 
@@ -26,19 +26,19 @@
 
     $ pip install rsfile
 
 
 QUICKSTART
 ------------
 
-::
+.. code-block:: python
 
     from rsfile import rsopen
 
     with rsopen("myfile.txt", "w") as f:
-        f.write(u"This string will be veeeeeryyyyy safely written to file.")
+        f.write("This string will be veeeeeryyyyy safely written to file.")
 
     with rsopen("myfile.txt", "WANISB", locking=False, thread_safe=False) as f:
         f.write(b"See the docs for info on these cool new modes and parameters.")
 
 
 See CONTRIBUTING.rst for development advice (testing, benchmarking...)
```

### Comparing `RSFile-3.0/RSFile.egg-info/PKG-INFO` & `RSFile-3.1/src/RSFile.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: RSFile
-Version: 3.0
+Version: 3.1
 Summary: Advanced I/O file streams with fine-grained locking and creation options
-Home-page: https://github.com/pakal/rsfile
-Author: Pascal Chambon
-Author-email: pythoniks@gmail.com
-License: http://www.opensource.org/licenses/mit-license.php
-Platform: any
+Author-email: Pascal Chambon <pythoniks@gmail.com>
+License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: License.txt
 
 RSFILE
 ================
 
 .. image:: https://ci.appveyor.com/api/projects/status/x002hlal3qwiavsa/branch/master
     :target: https://ci.appveyor.com/project/pakal/rsfile
 
@@ -35,15 +36,15 @@
 
 Locking is performed using actual file record locking capabilities of the OS, not by using separate files/directories as locking markers, or other fragile gimmicks.
 
 .. END OF PART KINDA SHARED WITH SPHINX DOC INDEX ..
 
 Possible use cases for this library: concurrently writing to logs without ending up with garbled data, manipulating sensitive data like disk-based databases, synchronizing heterogeneous producer/consumer processes when multiprocessing semaphores aren't an option, etc.
 
-Tested on Python 3.6+, on windows and unix-like systems. *Should* work with IronPython/Jython/PyPy too, since it uses stdlib utilities and ctypes bridges.
+Tested on CPython3, on windows and unix-like systems. *Should* work with IronPython/Jython/PyPy too, since it uses stdlib utilities and ctypes bridges.
 
 **Read the documentation here: http://rsfile.readthedocs.io/**
 
 
 INSTALL
 ------------
 
@@ -51,21 +52,19 @@
 
     $ pip install rsfile
 
 
 QUICKSTART
 ------------
 
-::
+.. code-block:: python
 
     from rsfile import rsopen
 
     with rsopen("myfile.txt", "w") as f:
-        f.write(u"This string will be veeeeeryyyyy safely written to file.")
+        f.write("This string will be veeeeeryyyyy safely written to file.")
 
     with rsopen("myfile.txt", "WANISB", locking=False, thread_safe=False) as f:
         f.write(b"See the docs for info on these cool new modes and parameters.")
 
 
 See CONTRIBUTING.rst for development advice (testing, benchmarking...)
-
-
```

### Comparing `RSFile-3.0/rsfile/rsbackend/_utilities.py` & `RSFile-3.1/src/rsfile/rsbackend/_utilities.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rsbackend/raw_win32_ctypes.py` & `RSFile-3.1/src/rsfile/rsbackend/raw_win32_ctypes.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rsbackend/raw_win32_defines.py` & `RSFile-3.1/src/rsfile/rsbackend/raw_win32_defines.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rsbackend/unix_stdlib.py` & `RSFile-3.1/src/rsfile/rsbackend/unix_stdlib.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rsbackend/windows_ctypes.py` & `RSFile-3.1/src/rsfile/rsbackend/windows_ctypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,17 +185,19 @@
 
     address = data_to_write  # ctypes.addressof(data_to_write)
 
     bytes_written = wintypes.DWORD(0)
 
     # no need to use WriteFileEx here...
     res = win32api.WriteFile(handle, address, len(data), ctypes.byref(bytes_written), overlapped)
-
+    #err_ = win32api.GetLastError()
+    #print(">> WRITE RES IS", res, bytes_written.value, err_, overlapped)
     if not res:
         err = ctypes.GetLastError()
+        #print(">> SAW WRITE ERROR", err, "vs", ERROR_IO_PENDING)
         if err != ERROR_IO_PENDING:
             raise ctypes.WinError(err)
     else:
         err = 0
 
     return (err, bytes_written.value)
```

### Comparing `RSFile-3.0/rsfile/rsbackend/windows_pywin32.py` & `RSFile-3.1/src/rsfile/rsbackend/windows_pywin32.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rsfile_definitions.py` & `RSFile-3.1/src/rsfile/rsfile_definitions.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 if sys.platform == "win32":  # even on 64bits windows OS
     RSFILE_IMPLEMENTATION = "windows"
 else:
     RSFILE_IMPLEMENTATION = "unix"
 
 HAS_X_OPEN_FLAG = sys.version_info >= (3, 3)
 
-STDLIB_OPEN_FLAGS = set("xarw+btU")
+STDLIB_OPEN_FLAGS = set("xarw+bt" + ("U" if sys.version_info < (3, 11) else ""))  # Universal newline got removed in 3.11
 ADVANCED_OPEN_FLAGS = set("RAW+-CNSIEBT")  # + and - are only left for retrocompatibility
 
 # beware, using C-backed IO doesn't work ATM because of class layout conflicts
 import _pyio as io_module
 
 
 class BadValueTypeError(ValueError, TypeError):
```

### Comparing `RSFile-3.0/rsfile/rsfile_factories.py` & `RSFile-3.1/src/rsfile/rsfile_factories.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rsfile_registries.py` & `RSFile-3.1/src/rsfile/rsfile_registries.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rsfile_streams.py` & `RSFile-3.1/src/rsfile/rsfile_streams.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rsfile_utilities.py` & `RSFile-3.1/src/rsfile/rsfile_utilities.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rsfileio_abstract.py` & `RSFile-3.1/src/rsfile/rsfileio_abstract.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         # BEWARE, also called if __init__() itself raised an exception!
         try:
             self.close()
         except:
             pass
 
     def __reduce__(self):
-        raise defs.BadValueTypeError("RSFileIO is not pickleable")
+        raise defs.BadValueTypeError("cannot pickle RSFileIO")
 
     def isatty(self):
         """On OSX the fileio.c implementation fails to recognized /dev/tty as a terminal,
         when using custom rsfile classes, so let's use this '_pyio.py' implementation instead"""
         return os.isatty(self.fileno())
 
     def seekable(self):
```

### Comparing `RSFile-3.0/rsfile/rsfileio_unix.py` & `RSFile-3.1/src/rsfile/rsfileio_unix.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rsfileio_windows.py` & `RSFile-3.1/src/rsfile/rsfileio_windows.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 try:
     from .rsbackend import windows_pywin32 as win32
 except ImportError:
     from .rsbackend import windows_ctypes as win32
 
 WIN32_MSG_ENCODING = locale.getpreferredencoding()
 
+BLOCKING_MODES_ENABLED = hasattr(os, "set_blocking")  # New in python 3.12 for Windows
+
 
 class RSFileIO(rsfileio_abstract.RSFileIOAbstract):
     __POSITION_REFERENCES = {
         defs.SEEK_SET: win32.FILE_BEGIN,
         defs.SEEK_CUR: win32.FILE_CURRENT,
         defs.SEEK_END: win32.FILE_END,
     }
@@ -100,15 +102,14 @@
             # print "FILE OPENED VIA HANDLE ", handle
 
         elif fileno is not None:
             assert handle is None
             self._fileno = fileno
             # print "FILE OPENED VIA FILENO ", fileno
             import msvcrt
-
             assert msvcrt.get_osfhandle == win32._get_osfhandle
             self._handle = win32._get_osfhandle(fileno)  # required immediately
 
         else:  # we open the file with CreateFile
             # print "FILE OPENED VIA PATH ", path
             desiredAccess = 0
             if read:  # we mimic the POSIX behaviour : we must have at least read or write
@@ -170,14 +171,26 @@
             handle = win32.CreateFile(*args)  # should raise if it's a DIRECTORY
             # print ">>>File opened : ", path
 
             self._handle = int(handle)
             if hasattr(handle, "Detach"):  # pywin32
                 handle.Detach()
 
+        self._use_nonblocking_pipe_write_hack = False
+        #print(">>> Detecting _use_nonblocking_pipe_write_hack!", write, BLOCKING_MODES_ENABLED)
+        if write and BLOCKING_MODES_ENABLED:
+            _fileno = win32._open_osfhandle(self._handle, (int(append) and os.O_APPEND))
+            try:
+                if not os.get_blocking(_fileno):
+                    #print(">>> We want to use _use_nonblocking_pipe_write_hack!")
+                    self._fileno = _fileno
+                    self._use_nonblocking_pipe_write_hack = True
+            except OSError:
+                pass  # probably not a PIPE
+
         # WHATEVER the origin of the stream, we initialize these fields:
         self._lock_registry_inode = self._handle  # we don't care about real inode unique_id, since win32 already
         # distinguishes which handle owns a lock
         self._lock_registry_descriptor = self._handle
 
     @_win32_error_converter
     def _inner_close_streams(self):
@@ -338,16 +351,25 @@
         reference = self.__POSITION_REFERENCES[whence]
         new_offset = win32.SetFilePointer(self._handle, offset, reference)
         return new_offset
 
     @_broken_pipe_ignorer
     @_win32_error_converter
     def _inner_read(self, n):
-        (res, mybytes) = win32.ReadFile(self._handle, n)  # returns bytes
-        return mybytes
+        #print(">> WIN32 READING BYTES", n)
+        try:
+            (res, mybytes) = win32.ReadFile(self._handle, n)  # returns bytes
+            #print(">> WIN32 READ BYTES", len(mybytes))
+            return mybytes
+        except win32.error as e:
+            # ERROR_NO_DATA in non-blocking mode, wrongly reported as "the pipe is being closed"
+            if e.winerror == 232:
+                #print(">> WIN32 READ RETURNS NONE")
+                return None
+            raise
 
     '''
     @_win32_error_converter  # abandoned for now
     def _inner_readinto(self, buffer):
         """ Warning - this method is currently inefficient since it converts C string into
             python str and then into bytearray, but this will be optimized later by rewriting in C module
         """
@@ -362,26 +384,46 @@
             buffer[0:len(mybytes)] = mybytes
         return len(mybytes)
     '''
 
     @_win32_error_converter
     def _inner_write(self, buffer):
 
+        #print(">> WIN32 WRITING BYTES", len(buffer))
+
         if self._append:  # yep, no atomicity around here, as in truncate(), since FILE_APPEND_DATA can't be used
             self._inner_seek(0, defs.SEEK_END)
 
         cur_pos = self._inner_tell()
         if cur_pos > self._inner_size():
             # we extend the file with zeros until current file pointer position
             self._inner_extend(cur_pos, zero_fill=True)
 
-        (res, bytes_written) = win32.WriteFile(self._handle, buffer)
-        # nothing to do with res, for files, it seems
+        if self._use_nonblocking_pipe_write_hack:
+            # Non-blocking pipes have horrendous behaviour on Windows
+            # See https://github.com/python/cpython/issues/101881
+            # So we rely on CPython hacks to force-write data into pipe
+            assert self._fileno, self._fileno
+            try:
+                bytes_written = os.write(self._fileno, buffer)
+            except BlockingIOError:
+                bytes_written = 0
+            errCode = None
+        else:
+            (errCode, bytes_written) = win32.WriteFile(self._handle, buffer)
+
+        # Nothing special for to do with errCode, for files, it seems
+        # see https://learn.microsoft.com/en-us/windows/win32/api/fileapi/nf-fileapi-writefile
+        #print(">> WIN32 WRITE RETURNED", errCode, bytes_written)
+        if not bytes_written:
+            #print(">> WIN32 WRITE FALLBACK TO NONE")
+            return None  # We mimick effects of EAGAIN on Unix
 
         # we let the file pointer where it is, even if we're in append mode (no come-back to previous reading position)
+        #print(">> WIN32 WRITTEN BYTES", bytes_written)
         return bytes_written
 
     # no need for @_win32_error_converter
     def _win32_convert_file_range_arguments(self, length, abs_offset):
 
         if abs_offset is None:
             abs_offset = 0
```

### Comparing `RSFile-3.0/rsfile/rsiobase.py` & `RSFile-3.1/src/rsfile/rsiobase.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rstest/_utilities.py` & `RSFile-3.1/src/rsfile/rstest/_utilities.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rstest/_worker_process.py` & `RSFile-3.1/src/rsfile/rstest/_worker_process.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rstest/stdlib/_pyio_py27_backup.py` & `RSFile-3.1/src/rsfile/rstest/stdlib/_pyio_py27_backup.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rstest/stdlib/_pyio_py310_backup.py` & `RSFile-3.1/src/rsfile/rstest/stdlib/_pyio_py310_backup.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rstest/stdlib/_pyio_py34_backup.py` & `RSFile-3.1/src/rsfile/rstest/stdlib/_pyio_py34_backup.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rstest/stdlib/_pyio_py35_backup.py` & `RSFile-3.1/src/rsfile/rstest/stdlib/_pyio_py35_backup.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rstest/stdlib/_pyio_py36_backup.py` & `RSFile-3.1/src/rsfile/rstest/stdlib/_pyio_py36_backup.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rstest/stdlib/_pyio_py37_backup.py` & `RSFile-3.1/src/rsfile/rstest/stdlib/_pyio_py37_backup.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rstest/stdlib/_pyio_py38_backup.py` & `RSFile-3.1/src/rsfile/rstest/stdlib/_pyio_py38_backup.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rstest/stdlib/_pyio_py39_backup.py` & `RSFile-3.1/src/rsfile/rstest/stdlib/_pyio_py39_backup.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rstest/stdlib/iobench.py` & `RSFile-3.1/src/rsfile/rstest/stdlib/iobench.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,286 +1,265 @@
 # -*- coding: utf-8 -*-
 # This file should be kept compatible with both Python 2.6 and Python >= 3.0.
 # GRABBED FROM http://svn.python.org/projects/python/trunk/Tools/iobench/, last checked 2016-05-20 #
 
 import itertools
 import os
+import platform
 import re
 import sys
 import time
 from optparse import OptionParser
 
 out = sys.stdout
 
-TEXT_ENCODING = "utf8"
-NEWLINES = "lf"
-
-# Compatibility
-try:
-    xrange
-except NameError:
-    xrange = range
+TEXT_ENCODING = 'utf8'
+NEWLINES = 'lf'
 
 
 def text_open(fn, mode, encoding=None):
     try:
         return open(fn, mode, encoding=encoding or TEXT_ENCODING)
     except TypeError:
         return open(fn, mode)
 
 
 def get_file_sizes():
-    for s in ["20 KB", "400 KB", "10 MB"]:
+    for s in ['20 KiB', '400 KiB', '10 MiB']:
         size, unit = s.split()
-        size = int(size) * {"KB": 1024, "MB": 1024**2}[unit]
-        yield s.replace(" ", ""), size
+        size = int(size) * {'KiB': 1024, 'MiB': 1024 ** 2}[unit]
+        yield s.replace(' ', ''), size
 
 
 def get_binary_files():
     return ((name + ".bin", size) for name, size in get_file_sizes())
 
 
 def get_text_files():
-    return (("%s-%s-%s.txt" % (name, TEXT_ENCODING, NEWLINES), size) for name, size in get_file_sizes())
+    return ((f"{name}-{TEXT_ENCODING}-{NEWLINES}.txt", size)
+        for name, size in get_file_sizes())
 
 
 def with_open_mode(mode):
     def decorate(f):
         f.file_open_mode = mode
         return f
-
     return decorate
 
 
 def with_sizes(*sizes):
     def decorate(f):
         f.file_sizes = sizes
         return f
-
     return decorate
 
 
 # Here begin the tests
 
-
 @with_open_mode("r")
 @with_sizes("medium")
 def read_bytewise(f):
-    """read one unit at a time"""
+    """ read one unit at a time """
     f.seek(0)
     while f.read(1):
         pass
 
 
 @with_open_mode("r")
 @with_sizes("medium")
 def read_small_chunks(f):
-    """read 20 units at a time"""
+    """ read 20 units at a time """
     f.seek(0)
     while f.read(20):
         pass
 
 
 @with_open_mode("r")
 @with_sizes("medium")
 def read_big_chunks(f):
-    """read 4096 units at a time"""
+    """ read 4096 units at a time """
     f.seek(0)
     while f.read(4096):
         pass
 
 
 @with_open_mode("r")
 @with_sizes("small", "medium", "large")
 def read_whole_file(f):
-    """read whole contents at once"""
+    """ read whole contents at once """
     f.seek(0)
     while f.read():
         pass
 
 
 @with_open_mode("rt")
 @with_sizes("medium")
 def read_lines(f):
-    """read one line at a time"""
+    """ read one line at a time """
     f.seek(0)
     for line in f:
         pass
 
 
 @with_open_mode("r")
 @with_sizes("medium")
 def seek_forward_bytewise(f):
-    """seek forward one unit at a time"""
+    """ seek forward one unit at a time """
     f.seek(0, 2)
     size = f.tell()
     f.seek(0, 0)
     for i in range(0, size - 1):
         f.seek(i, 0)
 
 
 @with_open_mode("r")
 @with_sizes("medium")
 def seek_forward_blockwise(f):
-    """seek forward 1000 units at a time"""
+    """ seek forward 1000 units at a time """
     f.seek(0, 2)
     size = f.tell()
     f.seek(0, 0)
     for i in range(0, size - 1, 1000):
         f.seek(i, 0)
 
 
 @with_open_mode("rb")
 @with_sizes("medium")
 def read_seek_bytewise(f):
-    """alternate read & seek one unit"""
+    """ alternate read & seek one unit """
     f.seek(0)
     while f.read(1):
         f.seek(1, 1)
 
 
 @with_open_mode("rb")
 @with_sizes("medium")
 def read_seek_blockwise(f):
-    """alternate read & seek 1000 units"""
+    """ alternate read & seek 1000 units """
     f.seek(0)
     while f.read(1000):
         f.seek(1000, 1)
 
 
 @with_open_mode("w")
 @with_sizes("small")
 def write_bytewise(f, source):
-    """write one unit at a time"""
+    """ write one unit at a time """
     for i in range(0, len(source)):
-        f.write(source[i : i + 1])
+        f.write(source[i:i+1])
 
 
 @with_open_mode("w")
 @with_sizes("medium")
 def write_small_chunks(f, source):
-    """write 20 units at a time"""
+    """ write 20 units at a time """
     for i in range(0, len(source), 20):
-        f.write(source[i : i + 20])
+        f.write(source[i:i+20])
 
 
 @with_open_mode("w")
 @with_sizes("medium")
 def write_medium_chunks(f, source):
-    """write 4096 units at a time"""
+    """ write 4096 units at a time """
     for i in range(0, len(source), 4096):
-        f.write(source[i : i + 4096])
+        f.write(source[i:i+4096])
 
 
 @with_open_mode("w")
 @with_sizes("large")
 def write_large_chunks(f, source):
-    """write 1e6 units at a time"""
+    """ write 1e6 units at a time """
     for i in range(0, len(source), 1000000):
-        f.write(source[i : i + 1000000])
+        f.write(source[i:i+1000000])
 
 
 @with_open_mode("w+")
 @with_sizes("small")
 def modify_bytewise(f, source):
-    """modify one unit at a time"""
+    """ modify one unit at a time """
     f.seek(0)
     for i in range(0, len(source)):
-        f.write(source[i : i + 1])
+        f.write(source[i:i+1])
 
 
 @with_open_mode("w+")
 @with_sizes("medium")
 def modify_small_chunks(f, source):
-    """modify 20 units at a time"""
+    """ modify 20 units at a time """
     f.seek(0)
     for i in range(0, len(source), 20):
-        f.write(source[i : i + 20])
+        f.write(source[i:i+20])
 
 
 @with_open_mode("w+")
 @with_sizes("medium")
 def modify_medium_chunks(f, source):
-    """modify 4096 units at a time"""
+    """ modify 4096 units at a time """
     f.seek(0)
     for i in range(0, len(source), 4096):
-        f.write(source[i : i + 4096])
+        f.write(source[i:i+4096])
 
 
 @with_open_mode("wb+")
 @with_sizes("medium")
 def modify_seek_forward_bytewise(f, source):
-    """alternate write & seek one unit"""
+    """ alternate write & seek one unit """
     f.seek(0)
     for i in range(0, len(source), 2):
-        f.write(source[i : i + 1])
-        f.seek(i + 2)
+        f.write(source[i:i+1])
+        f.seek(i+2)
 
 
 @with_open_mode("wb+")
 @with_sizes("medium")
 def modify_seek_forward_blockwise(f, source):
-    """alternate write & seek 1000 units"""
+    """ alternate write & seek 1000 units """
     f.seek(0)
     for i in range(0, len(source), 2000):
-        f.write(source[i : i + 1000])
-        f.seek(i + 2000)
+        f.write(source[i:i+1000])
+        f.seek(i+2000)
 
 
 # XXX the 2 following tests don't work with py3k's text IO
 @with_open_mode("wb+")
 @with_sizes("medium")
 def read_modify_bytewise(f, source):
-    """alternate read & write one unit"""
+    """ alternate read & write one unit """
     f.seek(0)
     for i in range(0, len(source), 2):
         f.read(1)
-        f.write(source[i + 1 : i + 2])
+        f.write(source[i+1:i+2])
 
 
 @with_open_mode("wb+")
 @with_sizes("medium")
 def read_modify_blockwise(f, source):
-    """alternate read & write 1000 units"""
+    """ alternate read & write 1000 units """
     f.seek(0)
     for i in range(0, len(source), 2000):
         f.read(1000)
-        f.write(source[i + 1000 : i + 2000])
+        f.write(source[i+1000:i+2000])
 
 
 read_tests = [
-    read_bytewise,
-    read_small_chunks,
-    read_lines,
-    read_big_chunks,
-    None,
-    read_whole_file,
-    None,
-    seek_forward_bytewise,
-    seek_forward_blockwise,
-    read_seek_bytewise,
-    read_seek_blockwise,
+    read_bytewise, read_small_chunks, read_lines, read_big_chunks,
+    None, read_whole_file, None,
+    seek_forward_bytewise, seek_forward_blockwise,
+    read_seek_bytewise, read_seek_blockwise,
 ]
 
 write_tests = [
-    write_bytewise,
-    write_small_chunks,
-    write_medium_chunks,
-    write_large_chunks,
+    write_bytewise, write_small_chunks, write_medium_chunks, write_large_chunks,
 ]
 
 modify_tests = [
-    modify_bytewise,
-    modify_small_chunks,
-    modify_medium_chunks,
+    modify_bytewise, modify_small_chunks, modify_medium_chunks,
     None,
-    modify_seek_forward_bytewise,
-    modify_seek_forward_blockwise,
-    read_modify_bytewise,
-    read_modify_blockwise,
+    modify_seek_forward_bytewise, modify_seek_forward_blockwise,
+    read_modify_bytewise, read_modify_blockwise,
 ]
 
 
 def run_during(duration, func):
     _t = time.time
     n = 0
     start = os.times()
@@ -299,24 +278,27 @@
 def warm_cache(filename):
     with open(filename, "rb") as f:
         f.read()
 
 
 def run_all_tests(options):
     def print_label(filename, func):
-        name = re.split(r"[-.]", filename)[0]
-        out.write(("[%s] %s... " % (name.center(7), func.__doc__.strip())).ljust(52))
+        name = re.split(r'[-.]', filename)[0]
+        out.write(
+            f"[{name.center(7)}] {func.__doc__.strip()}... ".ljust(52))
         out.flush()
 
     def print_results(size, n, real, cpu):
-        bw = n * float(size) / 1024**2 / real
-        bw = ("%4d MB/s" if bw > 100 else "%.3g MB/s") % bw
+        bw = n * float(size) / 1024 ** 2 / real
+        bw = ("%4d MiB/s" if bw > 100 else "%.3g MiB/s") % bw
         out.write(bw.rjust(12) + "\n")
         if cpu < 0.90 * real:
-            out.write("   warning: test above used only %d%% CPU, " "result may be flawed!\n" % (100.0 * cpu / real))
+            out.write("   warning: test above used only "
+                      f"{cpu / real:%} CPU, "
+                      "result may be flawed!\n")
 
     def run_one_test(name, size, open_func, test_func, *args):
         mode = test_func.file_open_mode
         print_label(name, test_func)
         if "w" not in mode or "+" in mode:
             warm_cache(name)
         with open_func(name) as f:
@@ -328,30 +310,34 @@
             if test_func is None:
                 out.write("\n")
                 continue
             if mode_filter in test_func.file_open_mode:
                 continue
             for s in test_func.file_sizes:
                 name, size = files[size_names[s]]
-                # name += file_ext
+                #name += file_ext
                 args = tuple(f(name, size) for f in make_args)
-                run_one_test(name, size, open_func, test_func, *args)
+                run_one_test(name, size,
+                    open_func, test_func, *args)
 
     size_names = {
         "small": 0,
         "medium": 1,
         "large": 2,
     }
 
+    print(f"Python {sys.version}")
+    print("Unicode: PEP 393")
+    print(platform.platform())
     binary_files = list(get_binary_files())
     text_files = list(get_text_files())
     if "b" in options:
         print("Binary unit = one byte")
     if "t" in options:
-        print(("Text unit = one character (%s-decoded)" % TEXT_ENCODING))
+        print(f"Text unit = one character ({TEXT_ENCODING}-decoded)")
 
     # Binary reads
     if "b" in options and "r" in options:
         print("\n** Binary input **\n")
         run_test_family(read_tests, "t", binary_files, lambda fn: open(fn, "rb"))
 
     # Text reads
@@ -362,78 +348,79 @@
     # Binary writes
     if "b" in options and "w" in options:
         print("\n** Binary append **\n")
 
         def make_test_source(name, size):
             with open(name, "rb") as f:
                 return f.read()
-
-        run_test_family(write_tests, "t", binary_files, lambda fn: open(os.devnull, "wb"), make_test_source)
+        run_test_family(write_tests, "t", binary_files,
+            lambda fn: open(os.devnull, "wb"), make_test_source)
 
     # Text writes
     if "t" in options and "w" in options:
         print("\n** Text append **\n")
 
         def make_test_source(name, size):
             with text_open(name, "r") as f:
                 return f.read()
-
-        run_test_family(write_tests, "b", text_files, lambda fn: text_open(os.devnull, "w"), make_test_source)
+        run_test_family(write_tests, "b", text_files,
+            lambda fn: text_open(os.devnull, "w"), make_test_source)
 
     # Binary overwrites
     if "b" in options and "w" in options:
         print("\n** Binary overwrite **\n")
 
         def make_test_source(name, size):
             with open(name, "rb") as f:
                 return f.read()
-
-        run_test_family(modify_tests, "t", binary_files, lambda fn: open(fn, "r+b"), make_test_source)
+        run_test_family(modify_tests, "t", binary_files,
+            lambda fn: open(fn, "r+b"), make_test_source)
 
     # Text overwrites
     if "t" in options and "w" in options:
         print("\n** Text overwrite **\n")
 
         def make_test_source(name, size):
             with text_open(name, "r") as f:
                 return f.read()
-
-        run_test_family(modify_tests, "b", text_files, lambda fn: open(fn, "r+"), make_test_source)
+        run_test_family(modify_tests, "b", text_files,
+            lambda fn: text_open(fn, "r+"), make_test_source)
 
 
 def prepare_files():
     print("Preparing files...")
     # Binary files
     for name, size in get_binary_files():
         if os.path.isfile(name) and os.path.getsize(name) == size:
             continue
         with open(name, "wb") as f:
             f.write(os.urandom(size))
     # Text files
     chunk = []
-    # print(">> Opening %s to look for chunk markers" % __file__)
-    with text_open(__file__, "rU", encoding="utf8") as f:
+    with text_open(__file__, "r", encoding='utf8') as f:
         for line in f:
             if line.startswith("# <iobench text chunk marker>"):
                 break
         else:
-            raise RuntimeError("Couldn't find chunk marker in %s !" % __file__)
+            raise RuntimeError(
+                f"Couldn't find chunk marker in {__file__} !")
         if NEWLINES == "all":
             it = itertools.cycle(["\n", "\r", "\r\n"])
         else:
-            it = itertools.repeat({"cr": "\r", "lf": "\n", "crlf": "\r\n"}[NEWLINES])
+            it = itertools.repeat(
+                {"cr": "\r", "lf": "\n", "crlf": "\r\n"}[NEWLINES])
         chunk = "".join(line.replace("\n", next(it)) for line in f)
         if isinstance(chunk, bytes):
-            chunk = chunk.decode("utf8")
+            chunk = chunk.decode('utf8')
         chunk = chunk.encode(TEXT_ENCODING)
     for name, size in get_text_files():
         if os.path.isfile(name) and os.path.getsize(name) == size:
             continue
         head = chunk * (size // len(chunk))
-        tail = chunk[: size % len(chunk)]
+        tail = chunk[:size % len(chunk)]
         # Adjust tail to end on a character boundary
         while True:
             try:
                 tail.decode(TEXT_ENCODING)
                 break
             except UnicodeDecodeError:
                 tail = tail[:-1]
@@ -443,42 +430,42 @@
 
 
 def main():
     global TEXT_ENCODING, NEWLINES
 
     usage = "usage: %prog [-h|--help] [options]"
     parser = OptionParser(usage=usage)
-    parser.add_option("-b", "--binary", action="store_true", dest="binary", default=False, help="run binary I/O tests")
-    parser.add_option("-t", "--text", action="store_true", dest="text", default=False, help="run text I/O tests")
-    parser.add_option("-r", "--read", action="store_true", dest="read", default=False, help="run read tests")
-    parser.add_option(
-        "-w", "--write", action="store_true", dest="write", default=False, help="run write & modify tests"
-    )
-    parser.add_option(
-        "-E",
-        "--encoding",
-        action="store",
-        dest="encoding",
-        default=None,
-        help="encoding for text tests (default: %s)" % TEXT_ENCODING,
-    )
-    parser.add_option(
-        "-N",
-        "--newlines",
-        action="store",
-        dest="newlines",
-        default="lf",
-        help="line endings for text tests " "(one of: {lf (default), cr, crlf, all})",
-    )
+    parser.add_option("-b", "--binary",
+                      action="store_true", dest="binary", default=False,
+                      help="run binary I/O tests")
+    parser.add_option("-t", "--text",
+                      action="store_true", dest="text", default=False,
+                      help="run text I/O tests")
+    parser.add_option("-r", "--read",
+                      action="store_true", dest="read", default=False,
+                      help="run read tests")
+    parser.add_option("-w", "--write",
+                      action="store_true", dest="write", default=False,
+                      help="run write & modify tests")
+    parser.add_option("-E", "--encoding",
+                      action="store", dest="encoding", default=None,
+                      help=f"encoding for text tests (default: {TEXT_ENCODING})")
+    parser.add_option("-N", "--newlines",
+                      action="store", dest="newlines", default='lf',
+                      help="line endings for text tests "
+                           "(one of: {lf (default), cr, crlf, all})")
+    parser.add_option("-m", "--io-module",
+                      action="store", dest="io_module", default=None,
+                      help="io module to test (default: builtin open())")
     options, args = parser.parse_args()
     if args:
         parser.error("unexpected arguments")
     NEWLINES = options.newlines.lower()
-    if NEWLINES not in ("lf", "cr", "crlf", "all"):
-        parser.error("invalid 'newlines' option: %r" % NEWLINES)
+    if NEWLINES not in ('lf', 'cr', 'crlf', 'all'):
+        parser.error(f"invalid 'newlines' option: {NEWLINES!r}")
 
     test_options = ""
     if options.read:
         test_options += "r"
     if options.write:
         test_options += "w"
     elif not options.read:
@@ -489,21 +476,25 @@
         test_options += "b"
     elif not options.text:
         test_options += "tb"
 
     if options.encoding:
         TEXT_ENCODING = options.encoding
 
+    if options.io_module:
+        globals()['open'] = __import__(options.io_module, {}, {}, ['open']).open
+
     prepare_files()
     run_all_tests(test_options)
 
 
 if __name__ == "__main__":
     main()
 
+
 # -- This part to exercise text reading. Don't change anything! --
 # <iobench text chunk marker>
 
 """
 1.
 Gáttir allar,
 áðr gangi fram,
@@ -570,32 +561,12 @@
 lof ok líknstafi;
 ódælla er við þat,
 er maðr eiga skal
 annars brjóstum í.
 """
 
 """
-C'est revenir tard, je le sens, sur un sujet trop rebattu et déjà presque oublié. Mon état, qui ne me permet plus
-aucun travail suivi, mon aversion pour le genre polémique, ont causé ma lenteur à écrire et ma répugnance à publier.
-J'aurais même tout à fait supprimé ces Lettres, ou plutôt je lie les aurais point écrites, s'il n'eût été question
-que de moi : Mais ma patrie ne m'est pas tellement devenue étrangère que je puisse voir tranquillement opprimer ses
-citoyens, surtout lorsqu'ils n'ont compromis leurs droits qu'en défendant ma cause. Je serais le dernier des hommes
-si dans une telle occasion j'écoutais un sentiment qui n'est plus ni douceur ni patience, mais faiblesse et lâcheté,
-dans celui qu'il empêche de remplir son devoir.
-Rien de moins important pour le public, j'en conviens, que la matière de ces lettres. La constitution d'une petite
-République, le sort d'un petit particulier, l'exposé de quelques injustices, la réfutation de quelques sophismes ;
-tout cela n'a rien en soi d'assez considérable pour mériter beaucoup de lecteurs : mais si mes sujets sont petits mes
-objets sont grands, et dignes de l'attention de tout honnête homme. Laissons Genève à sa place, et Rousseau dans sa
-dépression ; mais la religion, mais la liberté, la justice ! voilà, qui que vous soyez, ce qui n'est pas au-dessous
-de vous.
-Qu'on ne cherche pas même ici dans le style le dédommagement de l'aridité de la matière. Ceux que quelques traits
-heureux de ma plume ont si fort irrités trouveront de quoi s'apaiser dans ces lettres, L'honneur de défendre un
-opprimé eût enflammé mon coeur si j'avais parlé pour un autre. Réduit au triste emploi de me défendre moi-même,
-j'ai dû me borner à raisonner ; m'échauffer eût été m'avilir. J'aurai donc trouvé grâce en ce point devant ceux qui
-s'imaginent qu'il est essentiel à la vérité d'être dite froidement ; opinion que pourtant j'ai peine à comprendre.
-Lorsqu'une vive persuasion nous anime, le moyen d'employer un langage glacé ? Quand Archimède tout transporté courait
-nu dans les rues de Syracuse, en avait-il moins trouvé la vérité parce qu'il se passionnait pour elle ? Tout au
-contraire, celui qui la sent ne peut s'abstenir de l'adorer ; celui qui demeure froid ne l'a pas vue.
-Quoi qu'il en soit, je prie les lecteurs de vouloir bien mettre à part mon beau style, et d'examiner seulement si je
-raisonne bien ou mal ; car enfin, de cela seul qu'un auteur s'exprime en bons termes, je ne vois pas comment il peut
-s'ensuivre que cet auteur ne sait ce qu'il dit.
+C'est revenir tard, je le sens, sur un sujet trop rebattu et déjà presque oublié. Mon état, qui ne me permet plus aucun travail suivi, mon aversion pour le genre polémique, ont causé ma lenteur à écrire et ma répugnance à publier. J'aurais même tout à fait supprimé ces Lettres, ou plutôt je lie les aurais point écrites, s'il n'eût été question que de moi : Mais ma patrie ne m'est pas tellement devenue étrangère que je puisse voir tranquillement opprimer ses citoyens, surtout lorsqu'ils n'ont compromis leurs droits qu'en défendant ma cause. Je serais le dernier des hommes si dans une telle occasion j'écoutais un sentiment qui n'est plus ni douceur ni patience, mais faiblesse et lâcheté, dans celui qu'il empêche de remplir son devoir.
+Rien de moins important pour le public, j'en conviens, que la matière de ces lettres. La constitution d'une petite République, le sort d'un petit particulier, l'exposé de quelques injustices, la réfutation de quelques sophismes ; tout cela n'a rien en soi d'assez considérable pour mériter beaucoup de lecteurs : mais si mes sujets sont petits mes objets sont grands, et dignes de l'attention de tout honnête homme. Laissons Genève à sa place, et Rousseau dans sa dépression ; mais la religion, mais la liberté, la justice ! voilà, qui que vous soyez, ce qui n'est pas au-dessous de vous.
+Qu'on ne cherche pas même ici dans le style le dédommagement de l'aridité de la matière. Ceux que quelques traits heureux de ma plume ont si fort irrités trouveront de quoi s'apaiser dans ces lettres, L'honneur de défendre un opprimé eût enflammé mon coeur si j'avais parlé pour un autre. Réduit au triste emploi de me défendre moi-même, j'ai dû me borner à raisonner ; m'échauffer eût été m'avilir. J'aurai donc trouvé grâce en ce point devant ceux qui s'imaginent qu'il est essentiel à la vérité d'être dite froidement ; opinion que pourtant j'ai peine à comprendre. Lorsqu'une vive persuasion nous anime, le moyen d'employer un langage glacé ? Quand Archimède tout transporté courait nu dans les rues de Syracuse, en avait-il moins trouvé la vérité parce qu'il se passionnait pour elle ? Tout au contraire, celui qui la sent ne peut s'abstenir de l'adorer ; celui qui demeure froid ne l'a pas vue.
+Quoi qu'il en soit, je prie les lecteurs de vouloir bien mettre à part mon beau style, et d'examiner seulement si je raisonne bien ou mal ; car enfin, de cela seul qu'un auteur s'exprime en bons termes, je ne vois pas comment il peut s'ensuivre que cet auteur ne sait ce qu'il dit.
 """
```

### Comparing `RSFile-3.0/rsfile/rstest/test_backend_utilities.py` & `RSFile-3.1/src/rsfile/rstest/test_backend_utilities.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rstest/test_rsfile_locking.py` & `RSFile-3.1/src/rsfile/rstest/test_rsfile_locking.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rstest/test_rsfile_retrocompatibility.py` & `RSFile-3.1/src/rsfile/rstest/test_rsfile_retrocompatibility.py`

 * *Files identical despite different names*

### Comparing `RSFile-3.0/rsfile/rstest/test_rsfile_stdlib.py` & `RSFile-3.1/src/rsfile/rstest/test_rsfile_stdlib.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 
-
 from rsfile.rstest import _utilities
 
 _utilities.patch_test_supports()
 
 import sys
 import os
 import unittest
@@ -87,14 +86,19 @@
 
     test_io.IOTest.test_garbage_collection = dummyfunc  # cyclic GC can't work with python classes having __del__()
     # method
     test_io.PyIOTest.test_garbage_collection = dummyfunc  # idem
     test_io.PyIOTest.test_large_file_ops = dummyfunc  # we just skip because HEAVY AND LONG
     test_io.TextIOWrapperTest.test_repr = dummyfunc  # repr() of streams changes of course
 
+    # Skip tests dealing with details of C implementation
+    if hasattr(test_io, "TestIOCTypes"):
+        test_io.TestIOCTypes.test_immutable_types = dummyfunc
+        test_io.TestIOCTypes.test_class_hierarchy = dummyfunc
+
     # like in _pyio implementation, in rsfile, we do not detect reentrant access, nor raise RuntimeError to avoid
     # deadlocks
     test_io.PySignalsTest.test_reentrant_write_buffered = dummyfunc
     test_io.PySignalsTest.test_reentrant_write_text = dummyfunc
     test_io.CSignalsTest.test_reentrant_write_buffered = dummyfunc
     test_io.CSignalsTest.test_reentrant_write_text = dummyfunc
 
@@ -135,18 +139,27 @@
     test_memoryio.CStringIOPickleTest = dummyklass
     test_memoryio.CBytesIOTest = dummyklass
     test_memoryio.CStringIOTest = dummyklass
 
     # Skip C-oriented tests
     test_file.CAutoFileTests = dummyklass
 
-    ## To launch a single test ##
-    # mytest = test_io.PyIOTest('test_invalid_newline')
-    # res = mytest.run()
-    # print(res)
+    ## Use this to launch a single test ##
+    '''
+    from unittest import TextTestResult
+	from unittest.runner import _WritelnDecorator
+	from rsfile import rsopen
+    mytest = test_io.PyMiscIOTest('test_nonblock_pipe_write_smallbuf')
+    mytest.open = rsopen
+    mytest.BlockingIOError = BlockingIOError
+    res = mytest.run(result=TextTestResult(_WritelnDecorator(sys.stdout), "", 1))
+    print(res)
+    res.printErrors()
+    return
+    '''
 
     all_test_suites = []
 
     test_modules = [test_io, test_file, test_fileio, test_bufio, test_memoryio]
 
     if ENABLE_LARGE_FILE_TESTS:
         # BEWARE - heavy test, activate it it wisely
```

### Comparing `RSFile-3.0/rsfile/rstest/test_rsfile_streams.py` & `RSFile-3.1/src/rsfile/rstest/test_rsfile_streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -973,31 +973,31 @@
                 for i in range(N):
                     f.write(b"a")
                     f.flush()
                 b = time.time()
                 res1 = b - a
 
                 # LIGHTEST SYNC
-                a = time.time()
+                a = time.perf_counter()
                 for i in range(N):
                     f.write(b"b")
                     f.sync(metadata=False, full_flush=False)
-                b = time.time()
+                b = time.perf_counter()
                 res2 = b - a
 
                 assert res2 > 1.05 * res1, (res1, res2)  # it takes time to datasync()
 
                 # HEAVIEST SYNC
-                a = time.time()
+                a = time.perf_counter()
                 for i in range(N):
                     f.write(b"c")
                     # print("We issue full sync")
                     f.sync(metadata=True, full_flush=True)
                     # print("STOP")
-                b = time.time()
+                b = time.perf_counter()
                 res3 = b - a
 
                 if defs.RSFILE_IMPLEMENTATION == "windows":
                     assert res3 > 1.05 * res1, (res1, res3)  # same as datasync
                 else:
                     assert res3 > 1.05 * res2, (res2, res3)  # full sync heavier than datasync, on linux/osx
```

