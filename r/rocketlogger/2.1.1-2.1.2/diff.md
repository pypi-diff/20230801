# Comparing `tmp/rocketlogger-2.1.1.tar.gz` & `tmp/rocketlogger-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocketlogger-2.1.1.tar", last modified: Sat Jul 15 10:11:08 2023, max compression
+gzip compressed data, was "rocketlogger-2.1.2.tar", last modified: Tue Aug  1 12:28:05 2023, max compression
```

## Comparing `rocketlogger-2.1.1.tar` & `rocketlogger-2.1.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-07-15 10:11:08.909980 rocketlogger-2.1.1/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      295 2021-08-07 16:51:48.000000 rocketlogger-2.1.1/.gitignore
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1583 2023-02-21 22:31:56.000000 rocketlogger-2.1.1/LICENSE
--rw-r--r--   0 lukas     (1000) lukas     (1000)      268 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/MANIFEST.in
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3494 2023-07-15 10:11:08.909980 rocketlogger-2.1.1/PKG-INFO
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2099 2023-02-21 22:31:56.000000 rocketlogger-2.1.1/README.md
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)     5107 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/bug57_recover.py
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)     3383 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/convert_calibration.py
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)     2963 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/create_calibration.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-07-15 10:11:08.903313 rocketlogger-2.1.1/data/
--rw-r--r--   0 lukas     (1000) lukas     (1000)        6 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/.gitignore
--rw-r--r--   0 lukas     (1000) lukas     (1000)   180516 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_analog_only.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)   586468 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_calibration_i1l.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)   554340 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_calibration_i2l.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)   562372 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_calibration_ih.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)  1058300 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_calibration_v.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)      104 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_calibration_v1.dat
--rw-r--r--   0 lukas     (1000) lukas     (1000)      124 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_calibration_v2.dat
--rw-r--r--   0 lukas     (1000) lukas     (1000)   180684 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_full.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)     4119 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_header_unaligned.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)   701348 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_high_current.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)      300 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_min_block_size.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/data/test_non_split.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/data/test_non_split_p1.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)     4120 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_single_block.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_split.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_split_p1.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_split_p2.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_split_truncated.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)  4608584 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_split_truncated_p1.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)  1621964 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_steps.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)    20260 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_truncated.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)  4196685 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_unsupported.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)    20264 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_v3_only.rld
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-07-15 10:11:08.909980 rocketlogger-2.1.1/docs/
--rw-r--r--   0 lukas     (1000) lukas     (1000)        7 2021-08-07 16:51:49.000000 rocketlogger-2.1.1/docs/.gitignore
--rw-r--r--   0 lukas     (1000) lukas     (1000)      634 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/docs/Makefile
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2653 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/docs/calibration.rst
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2206 2023-07-15 09:43:40.000000 rocketlogger-2.1.1/docs/conf.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1463 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/docs/data.rst
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1677 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/docs/index.rst
--rw-r--r--   0 lukas     (1000) lukas     (1000)      795 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/docs/make.bat
--rw-r--r--   0 lukas     (1000) lukas     (1000)      325 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/docs/rocketlogger.calibration.rst
--rw-r--r--   0 lukas     (1000) lukas     (1000)      218 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/docs/rocketlogger.data.rst
--rw-r--r--   0 lukas     (1000) lukas     (1000)      254 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/docs/rocketlogger.rst
--rw-r--r--   0 lukas     (1000) lukas     (1000)      799 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/docs/tests.rst
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)     2249 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/process_data.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      105 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/pyproject.toml
--rw-r--r--   0 lukas     (1000) lukas     (1000)       59 2023-07-12 21:05:07.000000 rocketlogger-2.1.1/requirements.txt
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-07-15 10:11:08.909980 rocketlogger-2.1.1/rocketlogger/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1559 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/rocketlogger/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    30148 2023-02-21 22:31:56.000000 rocketlogger-2.1.1/rocketlogger/calibration.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    53158 2023-02-19 16:35:04.000000 rocketlogger-2.1.1/rocketlogger/data.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-07-15 10:11:08.909980 rocketlogger-2.1.1/rocketlogger.egg-info/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3494 2023-07-15 10:11:08.000000 rocketlogger-2.1.1/rocketlogger.egg-info/PKG-INFO
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1347 2023-07-15 10:11:08.000000 rocketlogger-2.1.1/rocketlogger.egg-info/SOURCES.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)        1 2023-07-15 10:11:08.000000 rocketlogger-2.1.1/rocketlogger.egg-info/dependency_links.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)      107 2023-07-15 10:11:08.000000 rocketlogger-2.1.1/rocketlogger.egg-info/requires.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)       13 2023-07-15 10:11:08.000000 rocketlogger-2.1.1/rocketlogger.egg-info/top_level.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)       38 2023-07-15 10:11:08.909980 rocketlogger-2.1.1/setup.cfg
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3403 2023-07-15 09:43:40.000000 rocketlogger-2.1.1/setup.py
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)     1846 2023-02-21 22:31:56.000000 rocketlogger-2.1.1/test_coverage.sh
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)     4428 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/test_performance.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-07-15 10:11:08.909980 rocketlogger-2.1.1/tests/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1758 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/tests/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    18293 2023-02-21 22:31:56.000000 rocketlogger-2.1.1/tests/test_calibration.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    56921 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/tests/test_data.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1622 2023-02-21 22:31:56.000000 rocketlogger-2.1.1/tox.ini
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-08-01 12:28:05.775272 rocketlogger-2.1.2/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      295 2021-08-07 16:51:48.000000 rocketlogger-2.1.2/.gitignore
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1583 2023-07-27 20:28:17.000000 rocketlogger-2.1.2/LICENSE
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      268 2022-03-27 19:27:07.000000 rocketlogger-2.1.2/MANIFEST.in
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3494 2023-08-01 12:28:05.775272 rocketlogger-2.1.2/PKG-INFO
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2099 2023-08-01 12:08:26.000000 rocketlogger-2.1.2/README.md
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)     5107 2022-03-27 19:27:07.000000 rocketlogger-2.1.2/bug57_recover.py
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)     3383 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/convert_calibration.py
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)     2963 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/create_calibration.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-08-01 12:28:05.771938 rocketlogger-2.1.2/data/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        6 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/.gitignore
+-rw-r--r--   0 lukas     (1000) lukas     (1000)   180516 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/test_analog_only.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)   586468 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/test_calibration_i1l.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)   554340 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/test_calibration_i2l.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)   562372 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/test_calibration_ih.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)  1058300 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/test_calibration_v.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      104 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/test_calibration_v1.dat
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      124 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/test_calibration_v2.dat
+-rw-r--r--   0 lukas     (1000) lukas     (1000)   180684 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/test_full.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     4119 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/test_header_unaligned.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)   701348 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/test_high_current.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      300 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/test_min_block_size.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2022-03-27 19:27:07.000000 rocketlogger-2.1.2/data/test_non_split.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2022-03-27 19:27:07.000000 rocketlogger-2.1.2/data/test_non_split_p1.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     4120 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/test_single_block.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/test_split.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/test_split_p1.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/test_split_p2.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/test_split_truncated.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)  4608584 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/test_split_truncated_p1.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)  1621964 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/test_steps.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    20260 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/test_truncated.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)  4196685 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/test_unsupported.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    20264 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/data/test_v3_only.rld
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-08-01 12:28:05.775272 rocketlogger-2.1.2/docs/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        7 2021-08-07 16:51:49.000000 rocketlogger-2.1.2/docs/.gitignore
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      634 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/docs/Makefile
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2653 2022-03-27 19:27:07.000000 rocketlogger-2.1.2/docs/calibration.rst
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2172 2023-08-01 12:08:26.000000 rocketlogger-2.1.2/docs/conf.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1463 2022-03-27 19:27:07.000000 rocketlogger-2.1.2/docs/data.rst
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1677 2023-07-15 13:27:49.000000 rocketlogger-2.1.2/docs/index.rst
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      795 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/docs/make.bat
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      325 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/docs/rocketlogger.calibration.rst
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      218 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/docs/rocketlogger.data.rst
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      254 2022-03-27 19:27:07.000000 rocketlogger-2.1.2/docs/rocketlogger.rst
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      799 2022-03-27 19:27:07.000000 rocketlogger-2.1.2/docs/tests.rst
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)     2249 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/process_data.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      105 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/pyproject.toml
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       59 2023-07-12 21:05:07.000000 rocketlogger-2.1.2/requirements.txt
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-08-01 12:28:05.775272 rocketlogger-2.1.2/rocketlogger/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1559 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/rocketlogger/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    30148 2023-02-21 22:31:56.000000 rocketlogger-2.1.2/rocketlogger/calibration.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    53158 2023-02-19 16:35:04.000000 rocketlogger-2.1.2/rocketlogger/data.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-08-01 12:28:05.775272 rocketlogger-2.1.2/rocketlogger.egg-info/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3494 2023-08-01 12:28:05.000000 rocketlogger-2.1.2/rocketlogger.egg-info/PKG-INFO
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1347 2023-08-01 12:28:05.000000 rocketlogger-2.1.2/rocketlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        1 2023-08-01 12:28:05.000000 rocketlogger-2.1.2/rocketlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      107 2023-08-01 12:28:05.000000 rocketlogger-2.1.2/rocketlogger.egg-info/requires.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       13 2023-08-01 12:28:05.000000 rocketlogger-2.1.2/rocketlogger.egg-info/top_level.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       38 2023-08-01 12:28:05.775272 rocketlogger-2.1.2/setup.cfg
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3403 2023-08-01 12:08:26.000000 rocketlogger-2.1.2/setup.py
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)     1846 2023-02-21 22:31:56.000000 rocketlogger-2.1.2/test_coverage.sh
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)     4428 2021-10-30 16:36:36.000000 rocketlogger-2.1.2/test_performance.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-08-01 12:28:05.775272 rocketlogger-2.1.2/tests/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1758 2022-03-27 19:27:07.000000 rocketlogger-2.1.2/tests/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    18293 2023-02-21 22:31:56.000000 rocketlogger-2.1.2/tests/test_calibration.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    56921 2022-03-27 19:27:07.000000 rocketlogger-2.1.2/tests/test_data.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1714 2023-08-01 12:08:26.000000 rocketlogger-2.1.2/tox.ini
```

### Comparing `rocketlogger-2.1.1/LICENSE` & `rocketlogger-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/PKG-INFO` & `rocketlogger-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocketlogger
-Version: 2.1.1
+Version: 2.1.2
 Summary: RocketLogger Python Support
 Home-page: https://github.com/ETHZ-TEC/RocketLogger#readme
 Author: ETH Zurich, Computer Engineering Group
 License: BSD 3-Clause
 Project-URL: Documentation, https://github.com/ETHZ-TEC/RocketLogger/wiki/python
 Project-URL: Source, https://github.com/ETHZ-TEC/RocketLogger
 Project-URL: Tracker, https://github.com/ETHZ-TEC/RocketLogger/issues
@@ -35,15 +35,15 @@
 
 This package provides RocketLogger data file handling support, as well as
 basic processing and plotting of the data. Further, it provides the necessary
 support to generate calibration data from measurements.
 
 **Dependencies**
 * Python 3: version 3.6-3.11
-* NumPy: version 1.13-1.23
+* NumPy: version 1.13-1.25
 
 **Optional dependencies**
 * Matplotlib: for plotting data overview
 * pandas: for pandas DataFrame export
 
 **Compatibility**
 * Data processing: supports all officially specified RLD file version (versions 2-4)
```

### Comparing `rocketlogger-2.1.1/README.md` & `rocketlogger-2.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This package provides RocketLogger data file handling support, as well as
 basic processing and plotting of the data. Further, it provides the necessary
 support to generate calibration data from measurements.
 
 **Dependencies**
 * Python 3: version 3.6-3.11
-* NumPy: version 1.13-1.23
+* NumPy: version 1.13-1.25
 
 **Optional dependencies**
 * Matplotlib: for plotting data overview
 * pandas: for pandas DataFrame export
 
 **Compatibility**
 * Data processing: supports all officially specified RLD file version (versions 2-4)
```

### Comparing `rocketlogger-2.1.1/bug57_recover.py` & `rocketlogger-2.1.2/bug57_recover.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/convert_calibration.py` & `rocketlogger-2.1.2/convert_calibration.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/create_calibration.py` & `rocketlogger-2.1.2/create_calibration.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/data/test_analog_only.rld` & `rocketlogger-2.1.2/data/test_analog_only.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/data/test_calibration_i1l.rld` & `rocketlogger-2.1.2/data/test_calibration_i1l.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/data/test_calibration_i2l.rld` & `rocketlogger-2.1.2/data/test_calibration_i2l.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/data/test_calibration_ih.rld` & `rocketlogger-2.1.2/data/test_calibration_ih.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/data/test_calibration_v.rld` & `rocketlogger-2.1.2/data/test_calibration_v.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/data/test_full.rld` & `rocketlogger-2.1.2/data/test_full.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/data/test_header_unaligned.rld` & `rocketlogger-2.1.2/data/test_header_unaligned.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/data/test_high_current.rld` & `rocketlogger-2.1.2/data/test_high_current.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/data/test_non_split.rld` & `rocketlogger-2.1.2/data/test_non_split.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/data/test_non_split_p1.rld` & `rocketlogger-2.1.2/data/test_non_split_p1.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/data/test_single_block.rld` & `rocketlogger-2.1.2/data/test_single_block.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/data/test_split.rld` & `rocketlogger-2.1.2/data/test_split.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/data/test_split_p1.rld` & `rocketlogger-2.1.2/data/test_split_p1.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/data/test_split_p2.rld` & `rocketlogger-2.1.2/data/test_split_p2.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/data/test_split_truncated.rld` & `rocketlogger-2.1.2/data/test_split_truncated.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/data/test_split_truncated_p1.rld` & `rocketlogger-2.1.2/data/test_split_truncated_p1.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/data/test_steps.rld` & `rocketlogger-2.1.2/data/test_steps.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/data/test_truncated.rld` & `rocketlogger-2.1.2/data/test_truncated.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/data/test_unsupported.rld` & `rocketlogger-2.1.2/data/test_unsupported.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/data/test_v3_only.rld` & `rocketlogger-2.1.2/data/test_v3_only.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/docs/Makefile` & `rocketlogger-2.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/docs/calibration.rst` & `rocketlogger-2.1.2/docs/calibration.rst`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/docs/conf.py` & `rocketlogger-2.1.2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,40 +8,40 @@
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
-sys.path.insert(0, os.path.abspath('../rocketlogger'))
+sys.path.insert(0, os.path.abspath('..'))
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'RocketLogger Python Support Library'
 copyright = '2021, ETH Zurich, Computer Engineering Group'
 author = 'ETH Zurich, Computer Engineering Group'
 
 # The full version, including alpha/beta/rc tags
-release = '2.1.1'
+release = '2.1.2'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.coverage',
     'sphinx.ext.viewcode',
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = []
 
 # The suffix(es) of source filenames.
 source_suffix = {
     '.rst': 'restructuredtext',
     '.md': 'markdown',
 }
 
@@ -57,8 +57,8 @@
 # a list of builtin themes.
 #
 html_theme = 'alabaster'
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = []
```

### Comparing `rocketlogger-2.1.1/docs/data.rst` & `rocketlogger-2.1.2/docs/data.rst`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/docs/index.rst` & `rocketlogger-2.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/docs/make.bat` & `rocketlogger-2.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/docs/tests.rst` & `rocketlogger-2.1.2/docs/tests.rst`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/process_data.py` & `rocketlogger-2.1.2/process_data.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/rocketlogger/__init__.py` & `rocketlogger-2.1.2/rocketlogger/__init__.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/rocketlogger/calibration.py` & `rocketlogger-2.1.2/rocketlogger/calibration.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/rocketlogger/data.py` & `rocketlogger-2.1.2/rocketlogger/data.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/rocketlogger.egg-info/PKG-INFO` & `rocketlogger-2.1.2/rocketlogger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocketlogger
-Version: 2.1.1
+Version: 2.1.2
 Summary: RocketLogger Python Support
 Home-page: https://github.com/ETHZ-TEC/RocketLogger#readme
 Author: ETH Zurich, Computer Engineering Group
 License: BSD 3-Clause
 Project-URL: Documentation, https://github.com/ETHZ-TEC/RocketLogger/wiki/python
 Project-URL: Source, https://github.com/ETHZ-TEC/RocketLogger
 Project-URL: Tracker, https://github.com/ETHZ-TEC/RocketLogger/issues
@@ -35,15 +35,15 @@
 
 This package provides RocketLogger data file handling support, as well as
 basic processing and plotting of the data. Further, it provides the necessary
 support to generate calibration data from measurements.
 
 **Dependencies**
 * Python 3: version 3.6-3.11
-* NumPy: version 1.13-1.23
+* NumPy: version 1.13-1.25
 
 **Optional dependencies**
 * Matplotlib: for plotting data overview
 * pandas: for pandas DataFrame export
 
 **Compatibility**
 * Data processing: supports all officially specified RLD file version (versions 2-4)
```

### Comparing `rocketlogger-2.1.1/rocketlogger.egg-info/SOURCES.txt` & `rocketlogger-2.1.2/rocketlogger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/setup.py` & `rocketlogger-2.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="rocketlogger",
-    version="2.1.1",
+    version="2.1.2",
     author="ETH Zurich, Computer Engineering Group",
     description="RocketLogger Python Support",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="BSD 3-Clause",
     url="https://github.com/ETHZ-TEC/RocketLogger#readme",
     classifiers=[
@@ -62,15 +62,15 @@
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
     keywords="rocketlogger, data analysis, calibration",
     packages=find_packages(exclude=["contrib", "docs", "tests"]),
     python_requires=">=3.6, <4",
     install_requires=[
-        "numpy>=1.13,<1.24",
+        "numpy>=1.13,<1.26",
     ],
     extras_require={
         "dataframe": ["pandas"],
         "plot": ["matplotlib"],
         "dev": ["black", "sphinx"],
         "test": ["pytest", "pytest-cov", "tox"],
     },
```

### Comparing `rocketlogger-2.1.1/test_coverage.sh` & `rocketlogger-2.1.2/test_coverage.sh`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/test_performance.py` & `rocketlogger-2.1.2/test_performance.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/tests/__init__.py` & `rocketlogger-2.1.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/tests/test_calibration.py` & `rocketlogger-2.1.2/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/tests/test_data.py` & `rocketlogger-2.1.2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.1/tox.ini` & `rocketlogger-2.1.2/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 # numpy release notes: https://docs.scipy.org/doc/numpy/release.html
 # matplotlib release notes: https://matplotlib.org/users/whats_new.html
 # pandas release notes: https://pandas.pydata.org/pandas-docs/stable/whatsnew/index.html
 [tox]
 envlist =
     py36-numpy{113,114,115,116,117,118,119}-{with,without}_plot-{with,without}_dataframe
     py37-numpy{115,116,117,118,119,120,121}-{with,without}_plot-{with,without}_dataframe
-    py38-numpy{117,118,119,120,121,122,123}-{with,without}_plot-{with,without}_dataframe
-    py39-numpy{120,121,122,123}-{with,without}_plot-{with,without}_dataframe
-    py310-numpy{121,122,123}-{with,without}_plot-{with,without}_dataframe
-    py311-numpy{123}-{with,without}_plot-{with,without}_dataframe
+    py38-numpy{117,118,119,120,121,122,123,124}-{with,without}_plot-{with,without}_dataframe
+    py39-numpy{120,121,122,123,124,125}-{with,without}_plot-{with,without}_dataframe
+    py310-numpy{121,122,123,124,125}-{with,without}_plot-{with,without}_dataframe
+    py311-numpy{123,124,125}-{with,without}_plot-{with,without}_dataframe
 skipsdist = True
 
 [testenv]
 commands = pytest {posargs}
 deps =
     pytest
     numpy113: numpy>=1.13,<1.14
@@ -28,12 +28,14 @@
     numpy117: numpy>=1.17,<1.18
     numpy118: numpy>=1.18,<1.19
     numpy119: numpy>=1.19,<1.20
     numpy120: numpy>=1.20,<1.21
     numpy121: numpy>=1.21,<1.22
     numpy122: numpy>=1.22,<1.23
     numpy123: numpy>=1.23,<1.24
+    numpy124: numpy>=1.24,<1.25
+    numpy125: numpy>=1.25,<1.26
     with_plot: matplotlib
     with_dataframe: pandas
 setenv =
     with_plot: MATPLOTLIB_AVAILABLE = true
     with_dataframe: PANDAS_AVAILABLE = true
```

