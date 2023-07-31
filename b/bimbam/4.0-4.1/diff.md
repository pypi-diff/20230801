# Comparing `tmp/bimbam-4.0.tar.gz` & `tmp/bimbam-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bimbam-4.0.tar", last modified: Sun Jul 30 12:30:12 2023, max compression
+gzip compressed data, was "bimbam-4.1.tar", last modified: Mon Jul 31 22:23:57 2023, max compression
```

## Comparing `bimbam-4.0.tar` & `bimbam-4.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.320661 bimbam-4.0/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-07-30 12:30:12.320661 bimbam-4.0/PKG-INFO
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.308660 bimbam-4.0/bimbam.egg-info/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-07-30 12:30:12.000000 bimbam-4.0/bimbam.egg-info/PKG-INFO
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2648 2023-07-30 12:30:12.000000 bimbam-4.0/bimbam.egg-info/SOURCES.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-30 12:30:12.000000 bimbam-4.0/bimbam.egg-info/dependency_links.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-07-30 12:30:12.000000 bimbam-4.0/bimbam.egg-info/requires.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-07-30 12:30:12.000000 bimbam-4.0/bimbam.egg-info/top_level.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-07-30 12:30:12.320661 bimbam-4.0/setup.cfg
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1961 2023-07-30 12:30:06.000000 bimbam-4.0/setup.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.308660 bimbam-4.0/thonnycontrib/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1804 2023-07-26 19:04:33.000000 bimbam-4.0/thonnycontrib/ThonnyLogsGenerator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.312661 bimbam-4.0/thonnycontrib/backend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/backend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17887 2023-07-27 19:37:17.000000 bimbam-4.0/thonnycontrib/backend/ast_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35564 2023-07-23 17:34:08.000000 bimbam-4.0/thonnycontrib/backend/doctest_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5015 2023-07-27 19:30:14.000000 bimbam-4.0/thonnycontrib/backend/evaluator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4508 2023-07-27 19:33:34.000000 bimbam-4.0/thonnycontrib/backend/l1test_backend.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7164 2023-07-27 19:31:40.000000 bimbam-4.0/thonnycontrib/backend/test_finder.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.312661 bimbam-4.0/thonnycontrib/backend/verdicts/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2379 2023-07-22 13:45:44.000000 bimbam-4.0/thonnycontrib/backend/verdicts/ExampleVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      475 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/backend/verdicts/ExceptionVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      735 2023-07-23 18:54:56.000000 bimbam-4.0/thonnycontrib/backend/verdicts/FailedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      644 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      371 2023-07-22 11:09:20.000000 bimbam-4.0/thonnycontrib/backend/verdicts/PassedSetupVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      429 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/backend/verdicts/PassedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/backend/verdicts/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.312661 bimbam-4.0/thonnycontrib/docs/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.316661 bimbam-4.0/thonnycontrib/docs/res/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/res/error_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1778 2023-07-27 18:28:42.000000 bimbam-4.0/thonnycontrib/docs/res/exception_red_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-07-27 19:02:02.000000 bimbam-4.0/thonnycontrib/docs/res/failed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1647 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/res/failed_red_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/res/l1test_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/res/l1test_icon_old.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/res/outline_class.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/res/outline_method.gif
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-07-27 19:01:55.000000 bimbam-4.0/thonnycontrib/docs/res/passed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/res/pending_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/res/restart_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1625 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/res/success_green_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/res/warning.png
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.316661 bimbam-4.0/thonnycontrib/docstring_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      585 2023-07-29 21:42:29.000000 bimbam-4.0/thonnycontrib/docstring_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16159 2023-07-30 12:26:59.000000 bimbam-4.0/thonnycontrib/docstring_generator/doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7054 2023-07-22 09:12:15.000000 bimbam-4.0/thonnycontrib/docstring_generator/doc_template.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1058 2023-07-23 10:37:34.000000 bimbam-4.0/thonnycontrib/environement_vars.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3712 2023-07-27 21:16:38.000000 bimbam-4.0/thonnycontrib/exceptions.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.316661 bimbam-4.0/thonnycontrib/l1test_configuration/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/l1test_configuration/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2991 2023-07-23 10:41:36.000000 bimbam-4.0/thonnycontrib/l1test_configuration/l1test_options.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.316661 bimbam-4.0/thonnycontrib/l1test_frontend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      754 2023-07-23 12:01:22.000000 bimbam-4.0/thonnycontrib/l1test_frontend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2847 2023-07-20 20:39:26.000000 bimbam-4.0/thonnycontrib/l1test_frontend/l1test_error_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3986 2023-07-23 12:06:57.000000 bimbam-4.0/thonnycontrib/l1test_frontend/l1test_outliner_menu.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2749 2023-07-23 16:34:32.000000 bimbam-4.0/thonnycontrib/l1test_frontend/l1test_reporter.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    23084 2023-07-27 21:21:22.000000 bimbam-4.0/thonnycontrib/l1test_frontend/l1test_runner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    41416 2023-07-28 15:24:19.000000 bimbam-4.0/thonnycontrib/l1test_frontend/l1test_treeview.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.320661 bimbam-4.0/thonnycontrib/main_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-22 08:21:17.000000 bimbam-4.0/thonnycontrib/main_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5301 2023-07-28 14:35:18.000000 bimbam-4.0/thonnycontrib/main_generator/main_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5469 2023-07-30 12:01:10.000000 bimbam-4.0/thonnycontrib/plugin_loader.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2962 2023-07-27 19:06:48.000000 bimbam-4.0/thonnycontrib/properties.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.320661 bimbam-4.0/thonnycontrib/tests/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/tests/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.320661 bimbam-4.0/thonnycontrib/tests/fixtures/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-24 19:06:13.000000 bimbam-4.0/thonnycontrib/tests/fixtures/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/tests/fixtures/backend_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1767 2023-07-22 09:17:05.000000 bimbam-4.0/thonnycontrib/tests/fixtures/workbench_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2306 2023-07-29 22:32:55.000000 bimbam-4.0/thonnycontrib/tests/tests_doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5767 2023-07-27 19:30:14.000000 bimbam-4.0/thonnycontrib/tests/tests_example_no_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16504 2023-07-27 19:30:14.000000 bimbam-4.0/thonnycontrib/tests/tests_example_with_exception.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21862 2023-07-27 19:30:14.000000 bimbam-4.0/thonnycontrib/tests/tests_example_with_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7935 2023-07-27 19:56:06.000000 bimbam-4.0/thonnycontrib/tests/tests_l1TestRunner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2030 2023-07-26 07:37:26.000000 bimbam-4.0/thonnycontrib/tests/tests_main_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6202 2023-07-27 19:30:14.000000 bimbam-4.0/thonnycontrib/tests/tests_test_finder.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14861 2023-07-24 19:26:54.000000 bimbam-4.0/thonnycontrib/tests/tests_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    20009 2023-07-30 12:00:21.000000 bimbam-4.0/thonnycontrib/utils.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.036693 bimbam-4.1/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-07-31 22:23:57.036693 bimbam-4.1/PKG-INFO
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.020693 bimbam-4.1/bimbam.egg-info/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-07-31 22:23:56.000000 bimbam-4.1/bimbam.egg-info/PKG-INFO
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2648 2023-07-31 22:23:56.000000 bimbam-4.1/bimbam.egg-info/SOURCES.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-31 22:23:56.000000 bimbam-4.1/bimbam.egg-info/dependency_links.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-07-31 22:23:56.000000 bimbam-4.1/bimbam.egg-info/requires.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-07-31 22:23:56.000000 bimbam-4.1/bimbam.egg-info/top_level.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-07-31 22:23:57.036693 bimbam-4.1/setup.cfg
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1961 2023-07-31 22:23:51.000000 bimbam-4.1/setup.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.024693 bimbam-4.1/thonnycontrib/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1805 2023-07-31 21:50:25.000000 bimbam-4.1/thonnycontrib/ThonnyLogsGenerator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.024693 bimbam-4.1/thonnycontrib/backend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/backend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17227 2023-07-31 21:56:01.000000 bimbam-4.1/thonnycontrib/backend/ast_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35564 2023-07-23 17:34:08.000000 bimbam-4.1/thonnycontrib/backend/doctest_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5015 2023-07-31 20:39:03.000000 bimbam-4.1/thonnycontrib/backend/evaluator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4508 2023-07-27 19:33:34.000000 bimbam-4.1/thonnycontrib/backend/l1test_backend.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5653 2023-07-31 20:57:44.000000 bimbam-4.1/thonnycontrib/backend/test_finder.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.028693 bimbam-4.1/thonnycontrib/backend/verdicts/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2379 2023-07-22 13:45:44.000000 bimbam-4.1/thonnycontrib/backend/verdicts/ExampleVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      475 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/backend/verdicts/ExceptionVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      735 2023-07-23 18:54:56.000000 bimbam-4.1/thonnycontrib/backend/verdicts/FailedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      644 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      371 2023-07-22 11:09:20.000000 bimbam-4.1/thonnycontrib/backend/verdicts/PassedSetupVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      429 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/backend/verdicts/PassedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/backend/verdicts/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.028693 bimbam-4.1/thonnycontrib/docs/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.028693 bimbam-4.1/thonnycontrib/docs/res/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/res/error_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1778 2023-07-27 18:28:42.000000 bimbam-4.1/thonnycontrib/docs/res/exception_red_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-07-27 19:02:02.000000 bimbam-4.1/thonnycontrib/docs/res/failed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1647 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/res/failed_red_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/res/l1test_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/res/l1test_icon_old.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/res/outline_class.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/res/outline_method.gif
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-07-27 19:01:55.000000 bimbam-4.1/thonnycontrib/docs/res/passed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/res/pending_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/res/restart_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1625 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/res/success_green_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/res/warning.png
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.032693 bimbam-4.1/thonnycontrib/docstring_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      585 2023-07-29 21:42:29.000000 bimbam-4.1/thonnycontrib/docstring_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16157 2023-07-31 21:17:00.000000 bimbam-4.1/thonnycontrib/docstring_generator/doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7054 2023-07-22 09:12:15.000000 bimbam-4.1/thonnycontrib/docstring_generator/doc_template.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1058 2023-07-23 10:37:34.000000 bimbam-4.1/thonnycontrib/environement_vars.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3712 2023-07-27 21:16:38.000000 bimbam-4.1/thonnycontrib/exceptions.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.032693 bimbam-4.1/thonnycontrib/l1test_configuration/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/l1test_configuration/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2991 2023-07-23 10:41:36.000000 bimbam-4.1/thonnycontrib/l1test_configuration/l1test_options.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.032693 bimbam-4.1/thonnycontrib/l1test_frontend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      754 2023-07-23 12:01:22.000000 bimbam-4.1/thonnycontrib/l1test_frontend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2847 2023-07-20 20:39:26.000000 bimbam-4.1/thonnycontrib/l1test_frontend/l1test_error_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3986 2023-07-23 12:06:57.000000 bimbam-4.1/thonnycontrib/l1test_frontend/l1test_outliner_menu.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2749 2023-07-23 16:34:32.000000 bimbam-4.1/thonnycontrib/l1test_frontend/l1test_reporter.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    22870 2023-07-31 22:23:02.000000 bimbam-4.1/thonnycontrib/l1test_frontend/l1test_runner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    41365 2023-07-31 22:23:02.000000 bimbam-4.1/thonnycontrib/l1test_frontend/l1test_treeview.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.032693 bimbam-4.1/thonnycontrib/main_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-22 08:21:17.000000 bimbam-4.1/thonnycontrib/main_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5301 2023-07-28 14:35:18.000000 bimbam-4.1/thonnycontrib/main_generator/main_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5453 2023-07-30 12:38:45.000000 bimbam-4.1/thonnycontrib/plugin_loader.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2962 2023-07-27 19:06:48.000000 bimbam-4.1/thonnycontrib/properties.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.036693 bimbam-4.1/thonnycontrib/tests/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/tests/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.036693 bimbam-4.1/thonnycontrib/tests/fixtures/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-24 19:06:13.000000 bimbam-4.1/thonnycontrib/tests/fixtures/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/tests/fixtures/backend_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1767 2023-07-22 09:17:05.000000 bimbam-4.1/thonnycontrib/tests/fixtures/workbench_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2505 2023-07-30 12:46:52.000000 bimbam-4.1/thonnycontrib/tests/tests_doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5767 2023-07-27 19:30:14.000000 bimbam-4.1/thonnycontrib/tests/tests_example_no_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16504 2023-07-27 19:30:14.000000 bimbam-4.1/thonnycontrib/tests/tests_example_with_exception.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21862 2023-07-27 19:30:14.000000 bimbam-4.1/thonnycontrib/tests/tests_example_with_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7935 2023-07-27 19:56:06.000000 bimbam-4.1/thonnycontrib/tests/tests_l1TestRunner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2030 2023-07-26 07:37:26.000000 bimbam-4.1/thonnycontrib/tests/tests_main_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6202 2023-07-27 19:30:14.000000 bimbam-4.1/thonnycontrib/tests/tests_test_finder.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14861 2023-07-24 19:26:54.000000 bimbam-4.1/thonnycontrib/tests/tests_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17914 2023-07-30 12:41:56.000000 bimbam-4.1/thonnycontrib/utils.py
```

### Comparing `bimbam-4.0/PKG-INFO` & `bimbam-4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimbam
-Version: 4.0
+Version: 4.1
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests
 Author: idtaleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `bimbam-4.0/bimbam.egg-info/PKG-INFO` & `bimbam-4.1/bimbam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimbam
-Version: 4.0
+Version: 4.1
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests
 Author: idtaleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `bimbam-4.0/bimbam.egg-info/SOURCES.txt` & `bimbam-4.1/bimbam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/setup.py` & `bimbam-4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     return py_packs | other_packs
 
 setupdir = os.path.dirname(__file__)
 
 
 setup(
     name="bimbam",
-    version="4.0",
+    version="4.1",
     author="idtaleb",
     description="A plug-in which adds a test framework",
     long_description="""A plug-in for Thonny which allows you to test your doc examples
  
 More info: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests""",
     url="https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests",
 #    keywords="IDE education programming tests in documentation",
```

### Comparing `bimbam-4.0/thonnycontrib/ThonnyLogsGenerator.py` & `bimbam-4.1/thonnycontrib/ThonnyLogsGenerator.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 NOM_EVENT_TEST = "l1Tests"
 NOM_EVENT_DOC = "l1Tests.DocGenerator"
 wb = get_workbench() 
 
 # Modifié par Mathieu Bachelet, PJI 2022-2023, mais sur la V2 de L1test
 # Modifié par Mirabelle pour adaptation à la V3 de L1test
 def log_in_thonny(test_results: List[L1DocTest], selected):
-    if test_results != []:
-        filename = test_results[0].get_filename()
+    filename = test_results[0].get_filename() if test_results != [] else None
     tests_data = []
     for l1doctest in test_results:
         for example in l1doctest.get_examples():
             # test:Example
             verdict = example.get_verdict() # type ExampleVerdict
             res = vars(verdict).copy() # pour récupérer les attributs filename, lineno, tested_line, expected_results, details
             res['details'] = str(res['details']) # sinon on peut récupérer un entier
```

### Comparing `bimbam-4.0/thonnycontrib/backend/ast_parser.py` & `bimbam-4.1/thonnycontrib/backend/ast_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ast
-from enum import Enum 
+from enum import Enum
 from .verdicts.ExceptionVerdict import ExceptionVerdict
 from .verdicts.FailedVerdict import FailedVerdict
 from .verdicts.ExampleVerdict import ExampleVerdict
-from ..properties import EXECUTED_STATE, PENDING_STATE
+from ..properties import PENDING_STATE
 from ..utils import create_node_representation, send_current_state
 from .doctest_parser import DocTestParser, Example
 from typing import List, Tuple
 
 # Only these types can have a docstring 
 # according to ast's module documentation
 SUPPORTED_TYPES = (ast.FunctionDef, 
@@ -325,119 +325,102 @@
         self.__type = type
 
 
 ## The L1DocTestParser class 
 class L1TestAstParser():
     """
     The L1DocTestParser is responsible for parsing the source and extracts the L1DocTests.
-    The main method is `get_l1doctests()` which takes a list of AST nodes and returns a list of L1DocTest.
+    The main method is `parse()` that returns a generator of L1DocTests. The generator 
+    yields all the L1DocTests found in the source. 
+    
+    Note: generators are used to avoid to load all the L1DocTests in memory. This
+    is useful when the source is big. The L1DocTests are yielded one by one while parsing.
+    Finally, the use of generators allows better performances and less memory consumption.
+    
+    The `L1DocTestParser`doesn't evaluate the created L1Doctests. Each yielded L1DocTest
+    is initially unevaluated. It's the responsibility of the `Evaluator` to evaluate each 
+    received L1DocTest.
     
     Example of use:
-        - You could parse the source by invoking the get_supported_nodes() method, then pass 
-        the returned list of AST nodes to the get_l1doctests() method.
-        
-        >>> parser = L1TestAstParser("filename.py")
-        >>> list_nodes = parser.get_supported_nodes()
-        >>> l1doctests = parser.get_l1doctests(list_nodes)
-        
-        - You could also get all the L1Doctests by invoking directly the get_l1doctests() method, without 
-        parameters. In this case, the source will be firstly parsed then the L1Doctests will be extracted.
-        
-        >>> parser = L1TestAstParser("filename.py")
-        >>> l1doctests = parser.get_l1doctests()
+    >>> parser = L1DocTestParser("source", "filename.py")
+    >>> generator:  = parser.parse()
+    >>> 
     """
     def __init__(self, source:str="", filename:str="", mode="exec") -> None:
         self._filename = filename
         self._source = source
         self._mode = mode
 
-    def extract_l1doctests(self, list_nodes: List[ast.AST]=None) -> List[L1DocTest]:
+    def parse(self, lineno:int=None):
         """
-        Takes a list of supported nodes and returns a list of L1DocTest. 
-        Each L1DocTest represents an AST node. 
+        Parse the source and yields all the l1doctest.
+        If the line number is not None, only the l1doctest that has 
+        the given line number is yielded.
+        
+        Args:
+            lineno (int): the line number of the l1doctest to yield. If None, 
+            all the l1doctests are yielded.
+        Returns:
+            generator: a generator of l1doctests.
+        
+        Raises: 
+            Error: A compilation error raised by the AST module.
         """
-        list_nodes = list_nodes or self.parse()
-        l1doctests: List[L1DocTest] = []
-        doctest_parser = DocTestParser()        
+        body = self.__get_ast_body(self._source)
+        yield from self.__recursive_walking(body, lineno)
+    
+    def __get_ast_body(self, source) -> List[ast.AST]:
+        """
+        Returns the body(list of nodes) of the root node of the AST tree.
+        
+        Raises: 
+            Error: A compilation error raised by the AST module.
+        """
+        return ast.parse(source, self._filename, mode=self._mode).body
+    
+    def __recursive_walking(self, list_nodes: list, lineno: int = None):
+        """
+        Search all the supported nodes in the AST tree. Even sub-nodes are visited.
+        This is a recursive function, so all the visited nodes are added in the ~all_nodes~
+        parameter.
+        """
+        doctest_parser = DocTestParser()
         for node in list_nodes:
             if isinstance(node, SUPPORTED_TYPES):
                 type = node.__class__.__name__
                 l1doctest = L1DocTest(self._filename, create_node_representation(node), type, node.lineno)
                 if node.body:
                     first_stmt = node.body[0]
                     if isinstance(first_stmt, ast.Expr) and isinstance(first_stmt.value, ast.Str):
                         l1doctest.set_start_lineno(first_stmt.lineno)
                         l1doctest.set_end_lineno(first_stmt.end_lineno)
-                
+
                 docstring = ast.get_docstring(node, False) or ""
                 parsed_doc = doctest_parser.parse(docstring, name=self._filename)
 
                 l1doctest.set_examples(self.__filter_example_instances(l1doctest, parsed_doc))
-                l1doctests.append(l1doctest)
-        return l1doctests
+                # Check if the current node matches the given lineno
+                if lineno is None or (l1doctest.get_node_lineno() == lineno):
+                    yield l1doctest
 
-    def extract_l1doctest(self, node:ast.AST):
-        """
-        Returns the corresponding L1DocTest for the given node.
-        
-        Args: 
-            node (ast) : the ast node.  
-            This parameter cannot be None and should be a supported type. See `SUPPORTED_TYPES`.
-        """
-        assert node != None and isinstance(node, SUPPORTED_TYPES)
-        return self.extract_l1doctests([node])
+                yield from self.__recursive_walking(ast.iter_child_nodes(node), lineno)
 
-    def parse(self):
-        """
-        Get only the nodes that can have a docstring. 
-        The supported nodes are repported to ~SUPPORTED_TYPES~ constant.
-        
-        Returns:
-            generator: a generator of supported AST nodes.
-        
-        Raises: 
-            Error: A compilation error raised by the AST module.
-        """
-        source_nodes = (node for node in self.__get_ast_body() if isinstance(node, SUPPORTED_TYPES))
-        # get all the supported nodes from a source content
-        yield from self.__recursive_walking(source_nodes)
-             
-    
     def __filter_example_instances(self, l1_doctest:L1DocTest, parsed_doc:list) -> List[Example]:
         """
         The filter can return an empty list if there's no example 
         in the parsed docstring. Otherwise, it will return a list of the `Example` instances 
         matching the given l1doctest.
         """
         examples = []
         for test in parsed_doc:
             if isinstance(test, Example):
                 test.lineno = test.lineno + l1_doctest.get_start_lineno() - 1
                 examples.append(test)
-        return examples
-    
-    def __get_ast_body(self):
-        """
-        Returns the body(list of nodes) of the root node of the AST tree.
+        return examples    
         
-        Raises: 
-            Error: A compilation error raised by the AST module.
-        """
-        return ast.parse(self._source, self._filename, mode=self._mode).body
-    
-    def __recursive_walking(self, list_nodes:list):
-        """
-        Search all the supported nodes in the AST tree. Even sub-nodes are visited.
-        This is a recursive function, so all the visited nodes are added in the ~all_nodes~
-        parameter.
-        """
-        for node in list_nodes:
-            if isinstance(node, SUPPORTED_TYPES):
-                yield from ast.walk(node)
-            
     def get_filename(self):
         return self._filename
     
     def set_filename(self, filename: str):
         self._filename = filename
     
     def get_source(self):
```

### Comparing `bimbam-4.0/thonnycontrib/backend/doctest_parser.py` & `bimbam-4.1/thonnycontrib/backend/doctest_parser.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/backend/evaluator.py` & `bimbam-4.1/thonnycontrib/backend/evaluator.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/backend/l1test_backend.py` & `bimbam-4.1/thonnycontrib/backend/l1test_backend.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/backend/test_finder.py` & `bimbam-4.1/thonnycontrib/backend/test_finder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import Any, Generator, List
 from abc import *
 from thonnycontrib.exceptions import NoFunctionSelectedToTestException
 from .ast_parser import L1DocTest, L1TestAstParser
 import ast
 
 class TestFinderStrategy(ABC):
     """
@@ -15,50 +15,29 @@
     and all supported nodes are revealed, then each concrete strategy can find 
     its suitable nodes as needed. 
     """
     def __init__(self, filename="", source="", ast_parser:L1TestAstParser=None) -> None:
         self._ast_parser = L1TestAstParser(filename, source) if not ast_parser else ast_parser
     
     # ###### MAIN METHOD ###### #
-    def find_l1doctests(self) -> List[L1DocTest]:
+    
+    def find_l1doctests(self) -> Generator[L1DocTest, Any, None]:
         """Invoke this method to get the docstrings depending of the strategy.
         
         This method follows the Template Method pattern. It defines the common 
         algorithm for all concrete strategies. Then, it invokes the `_find_docstring()` 
         abstract method.
-        
-        Args:
-            test_finder (TestFinder): The testFinder fo which the docstring 
-            will be retrived.
 
         Returns:
-            List[L1DocTest]: Returns a list of the L1DocTest. Each of L1DocTest 
-            represents an AST node.
+            Generator[L1DocTest, Any, None]: A generator of L1DocTest.
         """
-        ast_nodes = self._ast_parser.parse()
-        return self._find_l1doctests(ast_nodes)
+        return self._find_l1doctests()
     
     @abstractmethod
-    def _find_l1doctests(self, ast_nodes: List[ast.AST]=[]) -> List[L1DocTest]:
-        """Gets the docstrings from the source detained by the test_finder.
-
-        Args:
-            test_finder (TestFinder): An instance of TestFinder. The finder is used 
-            to acces it's method to parse the content of the source.
-            ast_nodes (List[ast.AST]): The source that is parsed by the TestFinder. 
-            Default to empty list.
-            
-        Returns:
-            (List[L1DocTest]): Returns a list of the L1DocTest. Each of L1DocTest 
-            represents an AST node.
-            
-        Raises:
-            The overriden methods could throw an exception. For each case, the raised 
-            exceptions should be specified and explained into the docstrings.
-        """
+    def _find_l1doctests(self) -> Generator[L1DocTest, Any, None]:
         pass
 
     def get_ast_nodes(self):
         return self._ast_nodes 
     
     def set_ast_nodes(self, ast_nodes):
         self._ast_nodes = ast_nodes
@@ -67,62 +46,44 @@
         self._ast_parser.set_filename(filename)
     
     def set_source(self, source):
         self._ast_parser.set_source(source)
     
     
 class FindAllL1DoctestsStrategy(TestFinderStrategy):
-    def _find_l1doctests(self, ast_nodes):
-        return self._ast_parser.extract_l1doctests(ast_nodes)
+    def _find_l1doctests(self):
+        return self._ast_parser.parse()
 
 
 class FindSelectedL1DoctestStrategy(TestFinderStrategy):
     def __init__(self, selected_line) -> None:
         super().__init__()
         self._selected_line = selected_line
     
-    def _find_l1doctests(self, ast_nodes):
+    def _find_l1doctests(self):
         """
         Note: The following docstring specifies only the raised excpetion.
         @See the docstring of the superclass to see the full docstring. 
             
         Raises:
             NoFunctionSelectedToTestException: When the selected line doesn' correspond to a 
             function or a class declaration.
         """
-        selected_node = self.__find_node(self._selected_line, next(ast_nodes, None))
-        return self._ast_parser.extract_l1doctest(selected_node)
-    
-    def __find_node(self, line, node: ast.AST):
-        """ Returns a node by its line number.
-
-        Args:
-            line (int): The number of the selected line.
-            node (ast.AST): an ast node to be tested. Should be one of the supported types.
-            
-        Returns:
-            ast.AST : Returns an AST node if the node was found for the line number
-        
-        Raises:
-            NoFunctionSelectedToTestException: When no node was found for the line number
-        """
-        from .ast_parser import SUPPORTED_TYPES
-        if node.lineno == line and isinstance(node, SUPPORTED_TYPES) :
-            return node
-        else: 
+        selected_node = next(self._ast_parser.parse(self._selected_line), None)
+        if not selected_node :
             msg = "%s\n\n%s" %  ("No function is selected to test !", 
                                  "The selected line must have a function or a class declaration.")
             raise NoFunctionSelectedToTestException(msg)
+        yield selected_node
     
     def get_selected_line(self):
         return self._selected_line    
     
     def set_selected_line(self, selected_line):
         self._selected_line = selected_line   
-        
 
 class L1TestFinder:
     """
         The `TestFinder` relies on the `AST` module to parse the script and extracts 
         the nodes with their docstrings. 
         
         For each node, it invokes the `DoctestParser` to parse its docstring. Then, 
@@ -148,16 +109,20 @@
         Each L1DocTest has it's list of `Example`
         
         Raises: 
             NoFunctionSelectedToTestException: when the selected line desn't refer to a 
             function/class signature.
             Error: A compilation error raised by the AST module.
             SpaceMissingAfterPromptException: when a space is missing after the prompt.
-        """                
-        return self._strategy.find_l1doctests()
+        """   
+        generator = self._strategy.find_l1doctests()
+        l1doctests: List[L1DocTest] = []
+        while (l1doctest := next(generator, None)) is not None: 
+            l1doctests.append(l1doctest)            
+        return l1doctests
         
     def get_filename(self):
         return self._filename
     
     def set_filename(self, filename: str):
         self._filename = filename
         self._strategy.set_filename(filename)
```

### Comparing `bimbam-4.0/thonnycontrib/backend/verdicts/ExampleVerdict.py` & `bimbam-4.1/thonnycontrib/backend/verdicts/ExampleVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/backend/verdicts/FailedVerdict.py` & `bimbam-4.1/thonnycontrib/backend/verdicts/FailedVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py` & `bimbam-4.1/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/docs/res/error_icon.png` & `bimbam-4.1/thonnycontrib/docs/res/error_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/docs/res/exception_red_chip.png` & `bimbam-4.1/thonnycontrib/docs/res/exception_red_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/docs/res/failed.png` & `bimbam-4.1/thonnycontrib/docs/res/failed.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/docs/res/failed_red_chip.png` & `bimbam-4.1/thonnycontrib/docs/res/failed_red_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/docs/res/l1test_icon.png` & `bimbam-4.1/thonnycontrib/docs/res/l1test_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/docs/res/l1test_icon_old.png` & `bimbam-4.1/thonnycontrib/docs/res/l1test_icon_old.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/docs/res/outline_class.png` & `bimbam-4.1/thonnycontrib/docs/res/outline_class.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/docs/res/outline_method.gif` & `bimbam-4.1/thonnycontrib/docs/res/outline_method.gif`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/docs/res/passed.png` & `bimbam-4.1/thonnycontrib/docs/res/passed.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/docs/res/pending_icon.png` & `bimbam-4.1/thonnycontrib/docs/res/pending_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/docs/res/restart_icon.png` & `bimbam-4.1/thonnycontrib/docs/res/restart_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/docs/res/success_green_chip.png` & `bimbam-4.1/thonnycontrib/docs/res/success_green_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/docs/res/warning.png` & `bimbam-4.1/thonnycontrib/docs/res/warning.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/docstring_generator/__init__.py` & `bimbam-4.1/thonnycontrib/docstring_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/docstring_generator/doc_generator.py` & `bimbam-4.1/thonnycontrib/docstring_generator/doc_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,19 +38,17 @@
 in the `edit menu` ~Generate Docstring~ button. You can also select the short cut 
 Alt+d after putting the cursor on the function(or a class) declaration.
 
 - Just a return on a function declaration will generate its docstring.
 """
 
 class DocParser:
-    def __init__(self, filename="", source="", ast_parser:L1TestAstParser=None):
+    def __init__(self, filename="", source=""):
         self._filename = filename
         self._source = source
-        self._ast_parser = L1TestAstParser(self._filename, self._source, mode="single") \
-                            if not ast_parser else ast_parser
     
     def parse_source(self, error_line:int=None):
         """
         Parses the given `source` and returns a list of 
         AST nodes that may contains a doctsring.
         
         As the AST python module stated in its documentation, the AST nodes that can 
@@ -61,32 +59,31 @@
             the raised exception. If `None`, so the error line mentioned in the error will 
             be kept. 
         
         Raises:
             DocGeneratorParserException: if the ast parser is failed.
         """
         try :
-            return next(self._ast_parser.parse(), None)
+            parsed = ast.parse(self._source, self._filename, mode="single").body
+            return parsed[0] if len(parsed) == 1 else None
         except Exception as e: # if a compilation error occurs during the parsing
             error_info = sys.exc_info()
             last_exception = get_last_exception(error_info)
             if error_line:
                 last_exception = replace_error_line(last_exception, error_line)
             raise DocGeneratorParserException(last_exception)    
     
     def get_filename(self):
         return self._filename
     
     def set_filename(self, filename: str):
         self._filename = filename
-        self._ast_parser.set_filename(filename)
     
     def set_source(self, source: str):
         self._source = source
-        self._ast_parser.set_source(source)
         
     def get_source(self):
         return self._source 
     
     def set_ast_parser(self, parser) :
         self._ast_parser = parser
 
@@ -196,14 +193,16 @@
         python_indent = 4
         sig_indent = len(space_match.group(1)) if space_match else 0
         return " " * (sig_indent + python_indent)
     
     def _create_custom_body(self, signature:str):
         signature = signature.strip()
         # on supprime tous ce qu'il vient après les ":" dans la signature. Car, on veut juste la signature.
+        # En python on peut avoir une syntaxe comme : def foo(): pass, cela pose problème pour l'ast parser
+        # il faut donc qu'on ait juste la signature sans le corps de la fonction.
         signature = re.sub(r"\s*(?P<id>def|class)(?P<signature>\s*.*\s*:)(?P<body>\s*.*)$", r"\g<id>\g<signature>", signature)
         indent = " " * 4
         return signature + "\n" + indent + "pass"
     
     def set_parser(self, parser: DocParser):
         self._parser = parser
```

### Comparing `bimbam-4.0/thonnycontrib/docstring_generator/doc_template.py` & `bimbam-4.1/thonnycontrib/docstring_generator/doc_template.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/environement_vars.py` & `bimbam-4.1/thonnycontrib/environement_vars.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/exceptions.py` & `bimbam-4.1/thonnycontrib/exceptions.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/l1test_configuration/l1test_options.py` & `bimbam-4.1/thonnycontrib/l1test_configuration/l1test_options.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/l1test_frontend/__init__.py` & `bimbam-4.1/thonnycontrib/l1test_frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/l1test_frontend/l1test_error_view.py` & `bimbam-4.1/thonnycontrib/l1test_frontend/l1test_error_view.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/l1test_frontend/l1test_outliner_menu.py` & `bimbam-4.1/thonnycontrib/l1test_frontend/l1test_outliner_menu.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/l1test_frontend/l1test_reporter.py` & `bimbam-4.1/thonnycontrib/l1test_frontend/l1test_reporter.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/l1test_frontend/l1test_runner.py` & `bimbam-4.1/thonnycontrib/l1test_frontend/l1test_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,17 +111,14 @@
         backend to be executed by the thonny's runner. 
         2. if the `L1test` is invoked a lot of times (lot of clicks), then we only
         consider the first invocation (first click) of the `L1test` command. While 
         the l1test still running, the other clicks are ignored.
 
         Args:
             selected_line (int): The number of the selected line.
-        Raises:
-            AlreadyRunningException: If the l1test is already running. This is raised 
-            when the user clicks on the `Run` button while the l1test is still running.
         """
         if not self.is_running(): # si l1test n'est est pas déjà en cours d'execution
             try:
                 self.set_is_running()
                 self.__request_backend(selected_line=selected_line)
             except:
                 self.set_is_running(False)
@@ -198,15 +195,16 @@
         Note: The data is deserialized before displaying it on the view.
         """   
        
         # On vérifie si le TopLevelRespone reçu est envoyé par le l1test_backend 
         if self._is_relevant_response(msg):
             verdicts, error_msg = self.__get_verdicts_and_error(msg)
             if not self.has_exception(): 
-                self.show_treeview(verdicts) 
+                if verdicts:
+                    self.show_treeview(verdicts) 
             else: 
                 self.clean_treeview()
                 self.show_error_view(error_msg.msg, error_msg.title)
         else:
             # Le TopLevelReponse reçu ne nous intéresse pas.
             return 
         # On indique l'état de l'execution du la commande comme terminée
@@ -227,15 +225,14 @@
         """
         l1doctests, error_msg = None, ErrorMsg(title=None, msg=None)
         self.clean_error_view()
         if msg.get(L1TEST_EXCEPTION):
             error_msg = self.__handle_raised_exception(msg.get(L1TEST_EXCEPTION))
         if not self.is_pending() and self.is_running(): # si le plugin est en cours d'execution et n'est pas en attente (càd pas de tests en cours d'execution)
             self.clean_treeview()
-            self._reporter.get_treeview().enable_menu()
             received_verdicts = msg.get(VERDICTS)
             if received_verdicts:
                 self.set_has_exception(False)
                 # deserialize the verdicts
                 l1doctests: List[L1DocTest] = pickle.loads(received_verdicts)
                 # log in thonny                    
                 log_in_thonny(l1doctests, os.environ.get(SELECTED_LINE_VAR) != None)
```

### Comparing `bimbam-4.0/thonnycontrib/l1test_frontend/l1test_treeview.py` & `bimbam-4.1/thonnycontrib/l1test_frontend/l1test_treeview.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         ttk.Frame.__init__(self, master, borderwidth=0, relief="flat")
         self.workbench = thonny.get_workbench()
         self._origin_l1doctests: List[L1DocTest] = dict()
         self._copy_l1doctests = self._origin_l1doctests.copy()
         
         self.__init_treeview()
         self.__init_workbench_bindings()
+        self.__init_special_attributes()
     
     def __init_workbench_bindings(self):
         """
         Binds the events to the workbench.
         """
         # Le binding est censé augmenter/diminuer automatiquement la taille de la treeview
         self.workbench.bind("<Control-plus>", self.observe_font_changing, True)
@@ -125,22 +126,20 @@
         self.treeview.tag_bind("nonClickable", "<<TreeviewSelect>>", self._remove_highlight_selection_effect)
         self.treeview.bind("<Motion>", self._on_hover_exception_test)
         self.treeview.bind("<Configure>", self.__wrap_tree_content) # Here we handle the motion event of the treeview 
         
         # add a menu to the treeview 
         self.menu = tk.Menu(self.treeview, name="menu", tearoff=False)        
         self.init_header(row=0, column=0)
-
-        self.__init_special_attributes()
         
     def __init_special_attributes(self):
         """
         Initializes the special attributes of the treeview.
         """
-        self.__old_height = -1 # utilisé pour savoir si la hauteur de la treeview a changé
+        self.__old_width = -1 # utilisé pour savoir si la hauteur de la treeview a changé
         self.__max_lines = 1 # le nombre de lignes du texte le plus long de la treeview
         self.__hovered_exception = None # l'exception test sur laquelle le curseur est en train de passer
      
     def _on_hover_exception_test(self, event):
         """
         Handles the motion event of the treeview. When the cursor is hovering over an exception test, 
         the font of the test is changed to bold and underlined. The cursor is also changed to "hand".
@@ -466,28 +465,27 @@
         """
         widget = event.widget if event else self.treeview
         if (isinstance(widget, ttk.Treeview)): 
             view = self.workbench.get_view(self.__class__.__name__)
             if view.winfo_ismapped() :  
                 if not self.is_empty():
                     width = view.winfo_width()
-                    height = view.winfo_height() 
-                    if self.__width_is_changed(height): # on ne met à jour que si la hauteur de la treeview n'a pas changé
+                    if self.__width_is_changed(width): # on ne met à jour que si la hauteur de la treeview n'a pas changé        
                         chars_per_pixels = width // get_font_size_option() 
                         visible_nodes = self.get_all_tree_childrens()
                         longest_length = self.__update_wrapped_texts(visible_nodes, chars_per_pixels)
                         new_rowheight = self.__compute_optimal_height(longest_length, margin)
                         self.update_row_height(new_rowheight)
-                    self.__old_height = height
+                    self.__old_width = width
     
-    def __width_is_changed(self, height):
+    def __width_is_changed(self, width):
         """
         Returns True if the height of the treeview hasn't changed.
         """
-        return self.__old_height == height
+        return self.__old_width != width
     
     def get_all_tree_childrens(self):
         """
         Gets recursivly all the childrens of the given node of the treeview. 
         
         Note: This function is a generator. It yields the childrens of the given node 
         one by one. This is useful to not load all the childrens in memory at once after
@@ -496,17 +494,18 @@
         Keep this method as a generator to avoid performance issues on th GUI. 
         It's observed that thonny's IDE is more faster when the treeview is 
         updated with a generator.
         """
         def _all_childrens(treeview: ttk.Treeview, node: str = None):
             child = treeview.get_children(node)
             for sub_child in child: 
-                yield sub_child  
                 if treeview.item(sub_child)["open"]:
                     yield from _all_childrens(self.treeview, sub_child)
+                yield sub_child  
+
         yield from _all_childrens(self.treeview)
 
     def __update_wrapped_texts(self, nodes, chars_per_pixels:int) -> int:
         """
         Met à jour le wrapping des textes des nœuds spécifiés dans la Treeview.
         Return the longest wrapped line of the treeview.
         Returns the number of lines of the longest wrapped line of the treeview.
@@ -538,15 +537,15 @@
         opt_height = max_lines * (row_height * margin) if max_lines else row_height
         return round(opt_height)
     
     def update_tree_contents(self, l1doctests:List[L1DocTest], parent="", clear_errorview=True, clear_header=True):
         """
             This function contructs and inserts the rows into the treeview.
         """
-        self.__old_height = self.workbench.get_view("L1TestTreeView", False).winfo_height() if self.__old_height > 0 else -1
+        self.__old_width = self.workbench.get_view("L1TestTreeView", False).winfo_width() if self.__old_width > 0 else -1
         
         self._restore_row_selection_effect() 
         self.clear_tree(clear_all=clear_header, clear_errorview=clear_errorview)
     
         if not self.__check_if_editor_is_open():
             return
 
@@ -853,8 +852,8 @@
         """
         if ref_name in self.image_references:
             return self.image_references[ref_name]
         return None
     
     def get_max_lines(self):
         """Returns the maximum number of lines of the longest wrapped line of the treeview."""
-        return self.__max_lines
+        return self.__max_lines
```

### Comparing `bimbam-4.0/thonnycontrib/main_generator/main_generator.py` & `bimbam-4.1/thonnycontrib/main_generator/main_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/plugin_loader.py` & `bimbam-4.1/thonnycontrib/plugin_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     Args:
         auto (bool):  Si True, alors la docstring sera générée automatiquement après un saut de ligne. 
         Sinon, la docstring sera générée quand le button `doc_generator` est cliqué.
         event (Any, optional): Si event est différent de None, alors un saut de ligne a été réalisé. 
         et donc la docstring sera générée automatiquement.
         Defaults to None.
     """
-    print("ed")
     if _writable_text_is_focused(): # on vérifie si la zone séléctionnée est une zone de l'éditeur
         text_widget = get_focused_writable_text()
         selected_line = get_selected_line(text_widget) 
         docGenerator = get_doc_generator(auto)  
         docGenerator.run(selected_line - 1 if auto else selected_line, text_widget)
 
 def generate_main():
```

### Comparing `bimbam-4.0/thonnycontrib/properties.py` & `bimbam-4.1/thonnycontrib/properties.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/tests/fixtures/workbench_mock.py` & `bimbam-4.1/thonnycontrib/tests/fixtures/workbench_mock.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/tests/tests_doc_generator.py` & `bimbam-4.1/thonnycontrib/tests/tests_doc_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,12 +63,16 @@
         
         raised_exception = e.exception      
         self.assertTrue(SyntaxError.__name__ in str(raised_exception))
         
     def test_doc_generator_when_signature_doesnt_finish_with_colon(self):
         signature = "def func()"
         
-        with self.assertRaises(NoFunctionSelectedToDocumentException) as e:
+        with self.assertRaises(DocGeneratorParserException) as e:
             self.docGenerationStrategy._generate(signature)
-            
+        
+        raised_exception = e.exception      
+        self.assertTrue(SyntaxError.__name__ in str(raised_exception))
+        self.assertTrue(SyntaxError.__name__+": expected ':'" in str(raised_exception))
+        
 if __name__ == '__main__':
     ut.main(verbosity=2)
```

### Comparing `bimbam-4.0/thonnycontrib/tests/tests_example_no_expected.py` & `bimbam-4.1/thonnycontrib/tests/tests_example_no_expected.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/tests/tests_example_with_exception.py` & `bimbam-4.1/thonnycontrib/tests/tests_example_with_exception.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/tests/tests_example_with_expected.py` & `bimbam-4.1/thonnycontrib/tests/tests_example_with_expected.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/tests/tests_l1TestRunner.py` & `bimbam-4.1/thonnycontrib/tests/tests_l1TestRunner.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/tests/tests_main_generator.py` & `bimbam-4.1/thonnycontrib/tests/tests_main_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/tests/tests_test_finder.py` & `bimbam-4.1/thonnycontrib/tests/tests_test_finder.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/tests/tests_view.py` & `bimbam-4.1/thonnycontrib/tests/tests_view.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.0/thonnycontrib/utils.py` & `bimbam-4.1/thonnycontrib/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,73 +130,14 @@
          .replace("..", "\\..")
     )
 
 import traceback
 import re
 from io import StringIO
 
-def get_last_exception(exc_info: tuple):
-    """
-    Formats exception information provided by ~exc_info~.
-    Extracts the last exception located in the last frame.
-
-    Args:
-        exc_info (tuple): The tuple must contain three elements:
-                        (type, value, traceback) as returned by sys.exc_info().
-
-    Returns:
-        str: Returns a string containing a traceback message for the given ~exc_info~.
-    """
-    exc_type, exc_val, exc_tb = exc_info
-
-    # Get a traceback message.
-    excout = StringIO()
-    traceback.print_exception(exc_type, exc_val, exc_tb, file=excout)
-
-    # Extract the last exception from the traceback frames.
-    content = excout.getvalue()
-    excout.close()
-    last_exception = extract_last_exception(content.rstrip("\n"))
-
-    # Remove multiple empty lines and preceding frames.
-    #last_exception = re.sub(r"\n+", "\n", last_exception)
-
-    return last_exception.strip()
-
-def extract_last_exception(traceback_content: str):
-    """
-    Extract the last exception from the traceback frames.
-
-    Args:
-        traceback_content (str): The returned traceback as a string.
-
-    Returns:
-        str: The lines representing the compilation error.
-    """
-   # Split the traceback into lines.
-    splitted = traceback_content.splitlines()
-
-    # Reverse the traceback frames and find the last frame containing the keyword "File."
-    last_frame_index = next((i for i, frame in enumerate(reversed(splitted)) if "File" in frame), 0)
-
-    # Get the last frame and its file name.
-    last_frame = splitted[-last_frame_index:]
-
-    # We don't want to display frames from the backend on thonny, as they are unnecessary and clutter the output.
-    frames_to_exclude = ["cpython_backend", os.path.join("thonny", "backend")]
-
-    for frame in last_frame:
-        if any(exclude in frame for exclude in frames_to_exclude):
-            last_frame_index = 0
-            break
-
-    # Get the error message from the last frame.
-    return "\n".join(last_frame[-last_frame_index:]).strip()
-
-
 def get_last_exception(exc_info:tuple):
     """
     Formats exception information provided by ~exc_info~.
     Extracts the last exception located in the last frame.
     
     Args:
         exc_info (tuple): The tuple must contain three elements: 
@@ -426,15 +367,14 @@
     return lineno if only_lineno else (lineno, column)
 
 def assert_one_line_is_selected() -> bool:
     """
     Returns True if only one line is selected, otherwise an exception is raised.
     """
     text = get_focused_writable_text()
-    print("selected = ", text.tag_ranges("sel") if text else None)
     if text :
         return len(text.tag_ranges("sel")) == 0
     return False
         
 def add_random_suffix(word):
     """Add a random suffix to the given word.
```

