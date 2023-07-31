# Comparing `tmp/bimbam-4.1.tar.gz` & `tmp/bimbam-4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bimbam-4.1.tar", last modified: Mon Jul 31 22:23:57 2023, max compression
+gzip compressed data, was "bimbam-4.2.tar", last modified: Mon Jul 31 22:27:43 2023, max compression
```

## Comparing `bimbam-4.1.tar` & `bimbam-4.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.036693 bimbam-4.1/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-07-31 22:23:57.036693 bimbam-4.1/PKG-INFO
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.020693 bimbam-4.1/bimbam.egg-info/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-07-31 22:23:56.000000 bimbam-4.1/bimbam.egg-info/PKG-INFO
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2648 2023-07-31 22:23:56.000000 bimbam-4.1/bimbam.egg-info/SOURCES.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-31 22:23:56.000000 bimbam-4.1/bimbam.egg-info/dependency_links.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-07-31 22:23:56.000000 bimbam-4.1/bimbam.egg-info/requires.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-07-31 22:23:56.000000 bimbam-4.1/bimbam.egg-info/top_level.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-07-31 22:23:57.036693 bimbam-4.1/setup.cfg
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1961 2023-07-31 22:23:51.000000 bimbam-4.1/setup.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.024693 bimbam-4.1/thonnycontrib/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1805 2023-07-31 21:50:25.000000 bimbam-4.1/thonnycontrib/ThonnyLogsGenerator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.024693 bimbam-4.1/thonnycontrib/backend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/backend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17227 2023-07-31 21:56:01.000000 bimbam-4.1/thonnycontrib/backend/ast_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35564 2023-07-23 17:34:08.000000 bimbam-4.1/thonnycontrib/backend/doctest_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5015 2023-07-31 20:39:03.000000 bimbam-4.1/thonnycontrib/backend/evaluator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4508 2023-07-27 19:33:34.000000 bimbam-4.1/thonnycontrib/backend/l1test_backend.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5653 2023-07-31 20:57:44.000000 bimbam-4.1/thonnycontrib/backend/test_finder.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.028693 bimbam-4.1/thonnycontrib/backend/verdicts/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2379 2023-07-22 13:45:44.000000 bimbam-4.1/thonnycontrib/backend/verdicts/ExampleVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      475 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/backend/verdicts/ExceptionVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      735 2023-07-23 18:54:56.000000 bimbam-4.1/thonnycontrib/backend/verdicts/FailedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      644 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      371 2023-07-22 11:09:20.000000 bimbam-4.1/thonnycontrib/backend/verdicts/PassedSetupVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      429 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/backend/verdicts/PassedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/backend/verdicts/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.028693 bimbam-4.1/thonnycontrib/docs/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.028693 bimbam-4.1/thonnycontrib/docs/res/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/res/error_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1778 2023-07-27 18:28:42.000000 bimbam-4.1/thonnycontrib/docs/res/exception_red_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-07-27 19:02:02.000000 bimbam-4.1/thonnycontrib/docs/res/failed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1647 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/res/failed_red_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/res/l1test_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/res/l1test_icon_old.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/res/outline_class.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/res/outline_method.gif
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-07-27 19:01:55.000000 bimbam-4.1/thonnycontrib/docs/res/passed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/res/pending_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/res/restart_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1625 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/res/success_green_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/docs/res/warning.png
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.032693 bimbam-4.1/thonnycontrib/docstring_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      585 2023-07-29 21:42:29.000000 bimbam-4.1/thonnycontrib/docstring_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16157 2023-07-31 21:17:00.000000 bimbam-4.1/thonnycontrib/docstring_generator/doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7054 2023-07-22 09:12:15.000000 bimbam-4.1/thonnycontrib/docstring_generator/doc_template.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1058 2023-07-23 10:37:34.000000 bimbam-4.1/thonnycontrib/environement_vars.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3712 2023-07-27 21:16:38.000000 bimbam-4.1/thonnycontrib/exceptions.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.032693 bimbam-4.1/thonnycontrib/l1test_configuration/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/l1test_configuration/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2991 2023-07-23 10:41:36.000000 bimbam-4.1/thonnycontrib/l1test_configuration/l1test_options.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.032693 bimbam-4.1/thonnycontrib/l1test_frontend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      754 2023-07-23 12:01:22.000000 bimbam-4.1/thonnycontrib/l1test_frontend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2847 2023-07-20 20:39:26.000000 bimbam-4.1/thonnycontrib/l1test_frontend/l1test_error_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3986 2023-07-23 12:06:57.000000 bimbam-4.1/thonnycontrib/l1test_frontend/l1test_outliner_menu.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2749 2023-07-23 16:34:32.000000 bimbam-4.1/thonnycontrib/l1test_frontend/l1test_reporter.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    22870 2023-07-31 22:23:02.000000 bimbam-4.1/thonnycontrib/l1test_frontend/l1test_runner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    41365 2023-07-31 22:23:02.000000 bimbam-4.1/thonnycontrib/l1test_frontend/l1test_treeview.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.032693 bimbam-4.1/thonnycontrib/main_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-22 08:21:17.000000 bimbam-4.1/thonnycontrib/main_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5301 2023-07-28 14:35:18.000000 bimbam-4.1/thonnycontrib/main_generator/main_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5453 2023-07-30 12:38:45.000000 bimbam-4.1/thonnycontrib/plugin_loader.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2962 2023-07-27 19:06:48.000000 bimbam-4.1/thonnycontrib/properties.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.036693 bimbam-4.1/thonnycontrib/tests/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/tests/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:23:57.036693 bimbam-4.1/thonnycontrib/tests/fixtures/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-24 19:06:13.000000 bimbam-4.1/thonnycontrib/tests/fixtures/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-07-20 20:20:05.000000 bimbam-4.1/thonnycontrib/tests/fixtures/backend_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1767 2023-07-22 09:17:05.000000 bimbam-4.1/thonnycontrib/tests/fixtures/workbench_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2505 2023-07-30 12:46:52.000000 bimbam-4.1/thonnycontrib/tests/tests_doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5767 2023-07-27 19:30:14.000000 bimbam-4.1/thonnycontrib/tests/tests_example_no_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16504 2023-07-27 19:30:14.000000 bimbam-4.1/thonnycontrib/tests/tests_example_with_exception.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21862 2023-07-27 19:30:14.000000 bimbam-4.1/thonnycontrib/tests/tests_example_with_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7935 2023-07-27 19:56:06.000000 bimbam-4.1/thonnycontrib/tests/tests_l1TestRunner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2030 2023-07-26 07:37:26.000000 bimbam-4.1/thonnycontrib/tests/tests_main_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6202 2023-07-27 19:30:14.000000 bimbam-4.1/thonnycontrib/tests/tests_test_finder.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14861 2023-07-24 19:26:54.000000 bimbam-4.1/thonnycontrib/tests/tests_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17914 2023-07-30 12:41:56.000000 bimbam-4.1/thonnycontrib/utils.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.789517 bimbam-4.2/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-07-31 22:27:43.789517 bimbam-4.2/PKG-INFO
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.773517 bimbam-4.2/bimbam.egg-info/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-07-31 22:27:43.000000 bimbam-4.2/bimbam.egg-info/PKG-INFO
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2648 2023-07-31 22:27:43.000000 bimbam-4.2/bimbam.egg-info/SOURCES.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-31 22:27:43.000000 bimbam-4.2/bimbam.egg-info/dependency_links.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-07-31 22:27:43.000000 bimbam-4.2/bimbam.egg-info/requires.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-07-31 22:27:43.000000 bimbam-4.2/bimbam.egg-info/top_level.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-07-31 22:27:43.789517 bimbam-4.2/setup.cfg
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1961 2023-07-31 22:27:33.000000 bimbam-4.2/setup.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.777517 bimbam-4.2/thonnycontrib/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1805 2023-07-31 21:50:25.000000 bimbam-4.2/thonnycontrib/ThonnyLogsGenerator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.777517 bimbam-4.2/thonnycontrib/backend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/backend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17227 2023-07-31 21:56:01.000000 bimbam-4.2/thonnycontrib/backend/ast_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35564 2023-07-23 17:34:08.000000 bimbam-4.2/thonnycontrib/backend/doctest_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5015 2023-07-31 20:39:03.000000 bimbam-4.2/thonnycontrib/backend/evaluator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4508 2023-07-27 19:33:34.000000 bimbam-4.2/thonnycontrib/backend/l1test_backend.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5653 2023-07-31 20:57:44.000000 bimbam-4.2/thonnycontrib/backend/test_finder.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.781517 bimbam-4.2/thonnycontrib/backend/verdicts/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2379 2023-07-22 13:45:44.000000 bimbam-4.2/thonnycontrib/backend/verdicts/ExampleVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      475 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/backend/verdicts/ExceptionVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      735 2023-07-23 18:54:56.000000 bimbam-4.2/thonnycontrib/backend/verdicts/FailedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      644 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      371 2023-07-22 11:09:20.000000 bimbam-4.2/thonnycontrib/backend/verdicts/PassedSetupVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      429 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/backend/verdicts/PassedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/backend/verdicts/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.781517 bimbam-4.2/thonnycontrib/docs/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.781517 bimbam-4.2/thonnycontrib/docs/res/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/res/error_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1778 2023-07-27 18:28:42.000000 bimbam-4.2/thonnycontrib/docs/res/exception_red_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-07-27 19:02:02.000000 bimbam-4.2/thonnycontrib/docs/res/failed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1647 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/res/failed_red_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/res/l1test_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/res/l1test_icon_old.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/res/outline_class.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/res/outline_method.gif
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-07-27 19:01:55.000000 bimbam-4.2/thonnycontrib/docs/res/passed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/res/pending_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/res/restart_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1625 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/res/success_green_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/docs/res/warning.png
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.785517 bimbam-4.2/thonnycontrib/docstring_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      585 2023-07-29 21:42:29.000000 bimbam-4.2/thonnycontrib/docstring_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16157 2023-07-31 21:17:00.000000 bimbam-4.2/thonnycontrib/docstring_generator/doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7054 2023-07-22 09:12:15.000000 bimbam-4.2/thonnycontrib/docstring_generator/doc_template.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1058 2023-07-23 10:37:34.000000 bimbam-4.2/thonnycontrib/environement_vars.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3712 2023-07-27 21:16:38.000000 bimbam-4.2/thonnycontrib/exceptions.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.785517 bimbam-4.2/thonnycontrib/l1test_configuration/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/l1test_configuration/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2991 2023-07-23 10:41:36.000000 bimbam-4.2/thonnycontrib/l1test_configuration/l1test_options.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.785517 bimbam-4.2/thonnycontrib/l1test_frontend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      754 2023-07-23 12:01:22.000000 bimbam-4.2/thonnycontrib/l1test_frontend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2847 2023-07-20 20:39:26.000000 bimbam-4.2/thonnycontrib/l1test_frontend/l1test_error_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3986 2023-07-23 12:06:57.000000 bimbam-4.2/thonnycontrib/l1test_frontend/l1test_outliner_menu.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2749 2023-07-23 16:34:32.000000 bimbam-4.2/thonnycontrib/l1test_frontend/l1test_reporter.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    23062 2023-07-31 22:27:12.000000 bimbam-4.2/thonnycontrib/l1test_frontend/l1test_runner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    41365 2023-07-31 19:30:41.000000 bimbam-4.2/thonnycontrib/l1test_frontend/l1test_treeview.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.785517 bimbam-4.2/thonnycontrib/main_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-22 08:21:17.000000 bimbam-4.2/thonnycontrib/main_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5301 2023-07-28 14:35:18.000000 bimbam-4.2/thonnycontrib/main_generator/main_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5453 2023-07-30 12:38:45.000000 bimbam-4.2/thonnycontrib/plugin_loader.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2962 2023-07-27 19:06:48.000000 bimbam-4.2/thonnycontrib/properties.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.789517 bimbam-4.2/thonnycontrib/tests/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/tests/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-31 22:27:43.789517 bimbam-4.2/thonnycontrib/tests/fixtures/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-24 19:06:13.000000 bimbam-4.2/thonnycontrib/tests/fixtures/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-07-20 20:20:05.000000 bimbam-4.2/thonnycontrib/tests/fixtures/backend_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1767 2023-07-22 09:17:05.000000 bimbam-4.2/thonnycontrib/tests/fixtures/workbench_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2505 2023-07-30 12:46:52.000000 bimbam-4.2/thonnycontrib/tests/tests_doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5767 2023-07-27 19:30:14.000000 bimbam-4.2/thonnycontrib/tests/tests_example_no_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16504 2023-07-27 19:30:14.000000 bimbam-4.2/thonnycontrib/tests/tests_example_with_exception.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21862 2023-07-27 19:30:14.000000 bimbam-4.2/thonnycontrib/tests/tests_example_with_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7935 2023-07-27 19:56:06.000000 bimbam-4.2/thonnycontrib/tests/tests_l1TestRunner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2030 2023-07-26 07:37:26.000000 bimbam-4.2/thonnycontrib/tests/tests_main_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6202 2023-07-27 19:30:14.000000 bimbam-4.2/thonnycontrib/tests/tests_test_finder.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14861 2023-07-24 19:26:54.000000 bimbam-4.2/thonnycontrib/tests/tests_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17914 2023-07-30 12:41:56.000000 bimbam-4.2/thonnycontrib/utils.py
```

### Comparing `bimbam-4.1/PKG-INFO` & `bimbam-4.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimbam
-Version: 4.1
+Version: 4.2
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests
 Author: idtaleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `bimbam-4.1/bimbam.egg-info/PKG-INFO` & `bimbam-4.2/bimbam.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimbam
-Version: 4.1
+Version: 4.2
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests
 Author: idtaleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `bimbam-4.1/bimbam.egg-info/SOURCES.txt` & `bimbam-4.2/bimbam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/setup.py` & `bimbam-4.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     return py_packs | other_packs
 
 setupdir = os.path.dirname(__file__)
 
 
 setup(
     name="bimbam",
-    version="4.1",
+    version="4.2",
     author="idtaleb",
     description="A plug-in which adds a test framework",
     long_description="""A plug-in for Thonny which allows you to test your doc examples
  
 More info: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests""",
     url="https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests",
 #    keywords="IDE education programming tests in documentation",
```

### Comparing `bimbam-4.1/thonnycontrib/ThonnyLogsGenerator.py` & `bimbam-4.2/thonnycontrib/ThonnyLogsGenerator.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/backend/ast_parser.py` & `bimbam-4.2/thonnycontrib/backend/ast_parser.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/backend/doctest_parser.py` & `bimbam-4.2/thonnycontrib/backend/doctest_parser.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/backend/evaluator.py` & `bimbam-4.2/thonnycontrib/backend/evaluator.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/backend/l1test_backend.py` & `bimbam-4.2/thonnycontrib/backend/l1test_backend.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/backend/test_finder.py` & `bimbam-4.2/thonnycontrib/backend/test_finder.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/backend/verdicts/ExampleVerdict.py` & `bimbam-4.2/thonnycontrib/backend/verdicts/ExampleVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/backend/verdicts/FailedVerdict.py` & `bimbam-4.2/thonnycontrib/backend/verdicts/FailedVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py` & `bimbam-4.2/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/docs/res/error_icon.png` & `bimbam-4.2/thonnycontrib/docs/res/error_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/docs/res/exception_red_chip.png` & `bimbam-4.2/thonnycontrib/docs/res/exception_red_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/docs/res/failed.png` & `bimbam-4.2/thonnycontrib/docs/res/failed.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/docs/res/failed_red_chip.png` & `bimbam-4.2/thonnycontrib/docs/res/failed_red_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/docs/res/l1test_icon.png` & `bimbam-4.2/thonnycontrib/docs/res/l1test_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/docs/res/l1test_icon_old.png` & `bimbam-4.2/thonnycontrib/docs/res/l1test_icon_old.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/docs/res/outline_class.png` & `bimbam-4.2/thonnycontrib/docs/res/outline_class.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/docs/res/outline_method.gif` & `bimbam-4.2/thonnycontrib/docs/res/outline_method.gif`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/docs/res/passed.png` & `bimbam-4.2/thonnycontrib/docs/res/passed.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/docs/res/pending_icon.png` & `bimbam-4.2/thonnycontrib/docs/res/pending_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/docs/res/restart_icon.png` & `bimbam-4.2/thonnycontrib/docs/res/restart_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/docs/res/success_green_chip.png` & `bimbam-4.2/thonnycontrib/docs/res/success_green_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/docs/res/warning.png` & `bimbam-4.2/thonnycontrib/docs/res/warning.png`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/docstring_generator/__init__.py` & `bimbam-4.2/thonnycontrib/docstring_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/docstring_generator/doc_generator.py` & `bimbam-4.2/thonnycontrib/docstring_generator/doc_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/docstring_generator/doc_template.py` & `bimbam-4.2/thonnycontrib/docstring_generator/doc_template.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/environement_vars.py` & `bimbam-4.2/thonnycontrib/environement_vars.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/exceptions.py` & `bimbam-4.2/thonnycontrib/exceptions.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/l1test_configuration/l1test_options.py` & `bimbam-4.2/thonnycontrib/l1test_configuration/l1test_options.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/l1test_frontend/__init__.py` & `bimbam-4.2/thonnycontrib/l1test_frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/l1test_frontend/l1test_error_view.py` & `bimbam-4.2/thonnycontrib/l1test_frontend/l1test_error_view.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/l1test_frontend/l1test_outliner_menu.py` & `bimbam-4.2/thonnycontrib/l1test_frontend/l1test_outliner_menu.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/l1test_frontend/l1test_reporter.py` & `bimbam-4.2/thonnycontrib/l1test_frontend/l1test_reporter.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/l1test_frontend/l1test_runner.py` & `bimbam-4.2/thonnycontrib/l1test_frontend/l1test_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,17 @@
         backend to be executed by the thonny's runner. 
         2. if the `L1test` is invoked a lot of times (lot of clicks), then we only
         consider the first invocation (first click) of the `L1test` command. While 
         the l1test still running, the other clicks are ignored.
 
         Args:
             selected_line (int): The number of the selected line.
+        Raises:
+            AlreadyRunningException: If the l1test is already running. This is raised 
+            when the user clicks on the `Run` button while the l1test is still running.
         """
         if not self.is_running(): # si l1test n'est est pas déjà en cours d'execution
             try:
                 self.set_is_running()
                 self.__request_backend(selected_line=selected_line)
             except:
                 self.set_is_running(False)
@@ -351,15 +354,15 @@
         """
         if self._is_relevant_response(msg):
             state:str = msg.get("state")
             if state == PENDING_STATE:
                 lineno = msg.get("lineno") # la ligne en cours d'execution est récupéré seulement si le state == PENDING_STATE
                 status_msg = L1TEST_IN_PROGRESS + ": line " + str(lineno) 
                 # you can comment the following line if you don't want to show the status message
-                self._reporter.get_treeview().insert_in_header(status_msg, clear=True, tags="blue", image=PENDING_ICON)
+                #self._reporter.get_treeview().insert_in_header(status_msg, clear=True, tags="blue", image=PENDING_ICON)
                 self.set_pending(True)
             else: # si le state == FINISHED_STATE
                 self.set_pending(False) 
     
     def show_error_view(self, error_msg=None, error_title=None, force=False, show_treeview=False):
         if self._has_exception or force:
             self.show_errors(exception_msg=error_msg, title=error_title)
```

### Comparing `bimbam-4.1/thonnycontrib/l1test_frontend/l1test_treeview.py` & `bimbam-4.2/thonnycontrib/l1test_frontend/l1test_treeview.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
         ttk.Frame.__init__(self, master, borderwidth=0, relief="flat")
         self.workbench = thonny.get_workbench()
         self._origin_l1doctests: List[L1DocTest] = dict()
         self._copy_l1doctests = self._origin_l1doctests.copy()
         
         self.__init_treeview()
         self.__init_workbench_bindings()
-        self.__init_special_attributes()
     
     def __init_workbench_bindings(self):
         """
         Binds the events to the workbench.
         """
         # Le binding est censé augmenter/diminuer automatiquement la taille de la treeview
         self.workbench.bind("<Control-plus>", self.observe_font_changing, True)
@@ -126,14 +125,16 @@
         self.treeview.tag_bind("nonClickable", "<<TreeviewSelect>>", self._remove_highlight_selection_effect)
         self.treeview.bind("<Motion>", self._on_hover_exception_test)
         self.treeview.bind("<Configure>", self.__wrap_tree_content) # Here we handle the motion event of the treeview 
         
         # add a menu to the treeview 
         self.menu = tk.Menu(self.treeview, name="menu", tearoff=False)        
         self.init_header(row=0, column=0)
+
+        self.__init_special_attributes()
         
     def __init_special_attributes(self):
         """
         Initializes the special attributes of the treeview.
         """
         self.__old_width = -1 # utilisé pour savoir si la hauteur de la treeview a changé
         self.__max_lines = 1 # le nombre de lignes du texte le plus long de la treeview
@@ -852,8 +853,8 @@
         """
         if ref_name in self.image_references:
             return self.image_references[ref_name]
         return None
     
     def get_max_lines(self):
         """Returns the maximum number of lines of the longest wrapped line of the treeview."""
-        return self.__max_lines
+        return self.__max_lines
```

### Comparing `bimbam-4.1/thonnycontrib/main_generator/main_generator.py` & `bimbam-4.2/thonnycontrib/main_generator/main_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/plugin_loader.py` & `bimbam-4.2/thonnycontrib/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/properties.py` & `bimbam-4.2/thonnycontrib/properties.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/tests/fixtures/workbench_mock.py` & `bimbam-4.2/thonnycontrib/tests/fixtures/workbench_mock.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/tests/tests_doc_generator.py` & `bimbam-4.2/thonnycontrib/tests/tests_doc_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/tests/tests_example_no_expected.py` & `bimbam-4.2/thonnycontrib/tests/tests_example_no_expected.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/tests/tests_example_with_exception.py` & `bimbam-4.2/thonnycontrib/tests/tests_example_with_exception.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/tests/tests_example_with_expected.py` & `bimbam-4.2/thonnycontrib/tests/tests_example_with_expected.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/tests/tests_l1TestRunner.py` & `bimbam-4.2/thonnycontrib/tests/tests_l1TestRunner.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/tests/tests_main_generator.py` & `bimbam-4.2/thonnycontrib/tests/tests_main_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/tests/tests_test_finder.py` & `bimbam-4.2/thonnycontrib/tests/tests_test_finder.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/tests/tests_view.py` & `bimbam-4.2/thonnycontrib/tests/tests_view.py`

 * *Files identical despite different names*

### Comparing `bimbam-4.1/thonnycontrib/utils.py` & `bimbam-4.2/thonnycontrib/utils.py`

 * *Files identical despite different names*

