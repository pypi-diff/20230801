# Comparing `tmp/huhk-1.8.9.tar.gz` & `tmp/huhk-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhk-1.8.9.tar", last modified: Wed Jul 26 08:46:36 2023, max compression
+gzip compressed data, was "huhk-1.9.1.tar", last modified: Tue Aug  1 01:44:39 2023, max compression
```

## Comparing `huhk-1.8.9.tar` & `huhk-1.9.1.tar`

### file list

```diff
@@ -1,105 +1,481 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.824959 huhk-1.8.9/
--rw-rw-rw-   0        0        0      223 2023-07-26 08:46:36.823970 huhk-1.8.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.597446 huhk-1.8.9/huhk/
--rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.8.9/huhk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.641948 huhk-1.8.9/huhk/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.8.9/huhk/case_project/__init__.py
--rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.8.9/huhk/case_project/json_coder.py
--rw-rw-rw-   0        0        0     3258 2023-07-26 08:25:43.000000 huhk-1.8.9/huhk/case_project/main_fun.py
--rw-rw-rw-   0        0        0    21410 2023-07-26 08:38:20.000000 huhk-1.8.9/huhk/case_project/project_base.py
--rw-rw-rw-   0        0        0     2099 2023-07-21 08:18:22.000000 huhk-1.8.9/huhk/case_project/project_init.py
--rw-rw-rw-   0        0        0    17878 2023-07-26 08:45:18.000000 huhk-1.8.9/huhk/case_project/project_string.py
--rw-rw-rw-   0        0        0      895 2023-07-26 08:22:28.000000 huhk-1.8.9/huhk/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-26 08:46:36.000000 huhk-1.8.9/huhk/case_project/version.py
--rw-rw-rw-   0        0        0    12802 2023-07-26 08:10:46.000000 huhk-1.8.9/huhk/init_project.py
--rw-rw-rw-   0        0        0     1267 2023-07-25 09:00:59.000000 huhk-1.8.9/huhk/main.py
--rw-rw-rw-   0        0        0      336 2023-07-25 02:56:17.000000 huhk-1.8.9/huhk/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.643947 huhk-1.8.9/huhk/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.8.9/huhk/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.693814 huhk-1.8.9/huhk/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.8.9/huhk/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.8.9/huhk/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.8.9/huhk/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.8.9/huhk/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.8.9/huhk/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.8.9/huhk/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.8.9/huhk/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.8.9/huhk/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.8.9/huhk/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.8.9/huhk/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.8.9/huhk/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.8.9/huhk/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.8.9/huhk/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.8.9/huhk/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.8.9/huhk/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.8.9/huhk/unit_encryption.py
--rw-rw-rw-   0        0        0    28433 2023-07-26 06:32:08.000000 huhk-1.8.9/huhk/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.8.9/huhk/unit_logger.py
--rw-rw-rw-   0        0        0     9960 2023-07-22 07:06:52.000000 huhk-1.8.9/huhk/unit_request.py
--rw-rw-rw-   0        0        0     2511 2023-07-24 06:56:32.000000 huhk-1.8.9/huhk/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.8.9/huhk/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.615395 huhk-1.8.9/huhk.egg-info/
--rw-rw-rw-   0        0        0      223 2023-07-26 08:46:36.000000 huhk-1.8.9/huhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2839 2023-07-26 08:46:36.000000 huhk-1.8.9/huhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 08:46:36.000000 huhk-1.8.9/huhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-26 08:46:36.000000 huhk-1.8.9/huhk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-07-26 08:46:36.000000 huhk-1.8.9/huhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-26 08:46:36.000000 huhk-1.8.9/huhk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.541837 huhk-1.8.9/service/
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.702787 huhk-1.8.9/service/app_t/
--rw-rw-rw-   0        0        0      420 2023-07-22 06:54:11.000000 huhk-1.8.9/service/app_t/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.704782 huhk-1.8.9/service/app_t/apis/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.8.9/service/app_t/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.708771 huhk-1.8.9/service/app_t/apis/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/apis/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.718752 huhk-1.8.9/service/app_t/apis/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/apis/open/haohan/__init__.py
--rw-rw-rw-   0        0        0    35088 2023-07-26 08:10:30.000000 huhk-1.8.9/service/app_t/apis/open/haohan/apis_open_haohan_relation.py
--rw-rw-rw-   0        0        0    36705 2023-07-26 08:10:30.000000 huhk-1.8.9/service/app_t/apis/open/haohan/apis_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.727721 huhk-1.8.9/service/app_t/apis/points/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/apis/points/__init__.py
--rw-rw-rw-   0        0        0    48149 2023-07-26 08:10:30.000000 huhk-1.8.9/service/app_t/apis/points/apis_points_points.py
--rw-rw-rw-   0        0        0    39604 2023-07-26 08:10:30.000000 huhk-1.8.9/service/app_t/apis/points/apis_points_pointsApp.py
--rw-rw-rw-   0        0        0      650 2023-07-22 10:57:15.000000 huhk-1.8.9/service/app_t/app_t_fun.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.730713 huhk-1.8.9/service/app_t/asserts/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.8.9/service/app_t/asserts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.733705 huhk-1.8.9/service/app_t/asserts/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/asserts/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.743759 huhk-1.8.9/service/app_t/asserts/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/asserts/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      602 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py
--rw-rw-rw-   0        0        0      590 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.753534 huhk-1.8.9/service/app_t/asserts/points/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/asserts/points/__init__.py
--rw-rw-rw-   0        0        0     1761 2023-07-22 07:08:51.000000 huhk-1.8.9/service/app_t/asserts/points/asserts_points_points.py
--rw-rw-rw-   0        0        0     1358 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/asserts/points/asserts_points_pointsApp.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.766505 huhk-1.8.9/service/app_t/funs/
--rw-rw-rw-   0        0        0        0 2023-07-24 01:53:24.000000 huhk-1.8.9/service/app_t/funs/__init__.py
--rw-rw-rw-   0        0        0      161 2023-07-24 01:53:33.000000 huhk-1.8.9/service/app_t/funs/funs_app_t.py
--rw-rw-rw-   0        0        0      118 2023-07-24 01:53:32.000000 huhk-1.8.9/service/app_t/funs/funs_open.py
--rw-rw-rw-   0        0        0      230 2023-07-24 01:53:33.000000 huhk-1.8.9/service/app_t/funs/funs_points.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.771492 huhk-1.8.9/service/app_t/funs/open/
--rw-rw-rw-   0        0        0        0 2023-07-24 01:53:27.000000 huhk-1.8.9/service/app_t/funs/open/__init__.py
--rw-rw-rw-   0        0        0      267 2023-07-24 01:53:31.000000 huhk-1.8.9/service/app_t/funs/open/funs_open_haohan.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.780068 huhk-1.8.9/service/app_t/funs/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-24 01:53:27.000000 huhk-1.8.9/service/app_t/funs/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      871 2023-07-26 08:10:30.000000 huhk-1.8.9/service/app_t/funs/open/haohan/funs_open_haohan_relation.py
--rw-rw-rw-   0        0        0      959 2023-07-26 08:10:30.000000 huhk-1.8.9/service/app_t/funs/open/haohan/funs_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.790042 huhk-1.8.9/service/app_t/funs/points/
--rw-rw-rw-   0        0        0        0 2023-07-24 01:53:32.000000 huhk-1.8.9/service/app_t/funs/points/__init__.py
--rw-rw-rw-   0        0        0     3201 2023-07-26 08:10:30.000000 huhk-1.8.9/service/app_t/funs/points/funs_points_points.py
--rw-rw-rw-   0        0        0     2040 2023-07-26 08:10:30.000000 huhk-1.8.9/service/app_t/funs/points/funs_points_pointsApp.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.792036 huhk-1.8.9/service/app_t/sqls/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.8.9/service/app_t/sqls/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.796026 huhk-1.8.9/service/app_t/sqls/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/sqls/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.806996 huhk-1.8.9/service/app_t/sqls/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/sqls/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      571 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py
--rw-rw-rw-   0        0        0      567 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.818982 huhk-1.8.9/service/app_t/sqls/points/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/sqls/points/__init__.py
--rw-rw-rw-   0        0        0     1994 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/sqls/points/sqls_points_points.py
--rw-rw-rw-   0        0        0     1529 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/sqls/points/sqls_points_pointsApp.py
--rw-rw-rw-   0        0        0       42 2023-07-26 08:46:36.824959 huhk-1.8.9/setup.cfg
--rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.8.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.852923 huhk-1.9.1/
+-rw-rw-rw-   0        0        0      223 2023-08-01 01:44:39.850899 huhk-1.9.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:37.794568 huhk-1.9.1/huhk/
+-rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.9.1/huhk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:37.891250 huhk-1.9.1/huhk/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.1/huhk/case_project/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.9.1/huhk/case_project/json_coder.py
+-rw-rw-rw-   0        0        0     3258 2023-07-26 08:25:43.000000 huhk-1.9.1/huhk/case_project/main_fun.py
+-rw-rw-rw-   0        0        0    21531 2023-07-31 07:13:40.000000 huhk-1.9.1/huhk/case_project/project_base.py
+-rw-rw-rw-   0        0        0     1332 2023-07-31 08:21:56.000000 huhk-1.9.1/huhk/case_project/project_init.py
+-rw-rw-rw-   0        0        0    18567 2023-07-31 08:18:51.000000 huhk-1.9.1/huhk/case_project/project_string.py
+-rw-rw-rw-   0        0        0      895 2023-07-26 08:22:28.000000 huhk-1.9.1/huhk/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-08-01 01:44:36.000000 huhk-1.9.1/huhk/case_project/version.py
+-rw-rw-rw-   0        0        0     9925 2023-07-31 05:34:49.000000 huhk-1.9.1/huhk/init_project.py
+-rw-rw-rw-   0        0        0     1267 2023-07-25 09:00:59.000000 huhk-1.9.1/huhk/main.py
+-rw-rw-rw-   0        0        0      336 2023-07-25 02:56:17.000000 huhk-1.9.1/huhk/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:37.896468 huhk-1.9.1/huhk/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.1/huhk/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.005378 huhk-1.9.1/huhk/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.1/huhk/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.9.1/huhk/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.9.1/huhk/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.9.1/huhk/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.9.1/huhk/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.9.1/huhk/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.9.1/huhk/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.9.1/huhk/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.9.1/huhk/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.9.1/huhk/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.9.1/huhk/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.9.1/huhk/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.9.1/huhk/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.9.1/huhk/unit_apache_beam.py
+-rw-rw-rw-   0        0        0      352 2023-07-31 09:35:09.000000 huhk-1.9.1/huhk/unit_data.py
+-rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.9.1/huhk/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.9.1/huhk/unit_encryption.py
+-rw-rw-rw-   0        0        0    29027 2023-08-01 01:43:21.000000 huhk-1.9.1/huhk/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.9.1/huhk/unit_logger.py
+-rw-rw-rw-   0        0        0     9960 2023-07-22 07:06:52.000000 huhk-1.9.1/huhk/unit_request.py
+-rw-rw-rw-   0        0        0     2511 2023-07-24 06:56:32.000000 huhk-1.9.1/huhk/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.9.1/huhk/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:37.828604 huhk-1.9.1/huhk.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-08-01 01:44:37.000000 huhk-1.9.1/huhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    19653 2023-08-01 01:44:37.000000 huhk-1.9.1/huhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 01:44:37.000000 huhk-1.9.1/huhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-08-01 01:44:37.000000 huhk-1.9.1/huhk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-08-01 01:44:37.000000 huhk-1.9.1/huhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-08-01 01:44:37.000000 huhk-1.9.1/huhk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.013357 huhk-1.9.1/service/
+-rw-rw-rw-   0        0        0        0 2023-07-28 06:59:30.000000 huhk-1.9.1/service/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.028108 huhk-1.9.1/service/app_a/
+-rw-rw-rw-   0        0        0      420 2023-07-31 05:25:05.000000 huhk-1.9.1/service/app_a/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.080965 huhk-1.9.1/service/app_a/apis/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:00:52.000000 huhk-1.9.1/service/app_a/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.126843 huhk-1.9.1/service/app_a/apis/admin/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:00:53.000000 huhk-1.9.1/service/app_a/apis/admin/__init__.py
+-rw-rw-rw-   0        0        0     1603 2023-07-31 06:00:53.000000 huhk-1.9.1/service/app_a/apis/admin/apis_admin_guc.py
+-rw-rw-rw-   0        0        0      784 2023-07-31 06:00:53.000000 huhk-1.9.1/service/app_a/apis/admin/apis_admin_spa.py
+-rw-rw-rw-   0        0        0     1105 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/apis_activitymanager.py
+-rw-rw-rw-   0        0        0     2049 2023-07-31 06:01:00.000000 huhk-1.9.1/service/app_a/apis/apis_app_a.py
+-rw-rw-rw-   0        0        0     1072 2023-07-31 06:01:00.000000 huhk-1.9.1/service/app_a/apis/apis_area.py
+-rw-rw-rw-   0        0        0      914 2023-07-31 06:00:57.000000 huhk-1.9.1/service/app_a/apis/apis_content.py
+-rw-rw-rw-   0        0        0     2511 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/apis_essay.py
+-rw-rw-rw-   0        0        0     2187 2023-07-31 06:00:55.000000 huhk-1.9.1/service/app_a/apis/apis_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.197114 huhk-1.9.1/service/app_a/apis/common/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:00:53.000000 huhk-1.9.1/service/app_a/apis/common/__init__.py
+-rw-rw-rw-   0        0        0     1422 2023-07-31 06:00:53.000000 huhk-1.9.1/service/app_a/apis/common/apis_common_clue.py
+-rw-rw-rw-   0        0        0     1071 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/common/apis_common_common.py
+-rw-rw-rw-   0        0        0     1945 2023-07-31 06:00:53.000000 huhk-1.9.1/service/app_a/apis/common/apis_common_remoteinterfacelog.py
+-rw-rw-rw-   0        0        0     2922 2023-07-31 06:00:53.000000 huhk-1.9.1/service/app_a/apis/common/apis_common_systemversion.py
+-rw-rw-rw-   0        0        0      867 2023-07-31 06:00:53.000000 huhk-1.9.1/service/app_a/apis/common/apis_common_user.py
+-rw-rw-rw-   0        0        0    25061 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/apis/common/apis_common_user4c.py
+-rw-rw-rw-   0        0        0     5938 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/apis/common/apis_common_userpointsmanage.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.360952 huhk-1.9.1/service/app_a/apis/content/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:00:52.000000 huhk-1.9.1/service/app_a/apis/content/__init__.py
+-rw-rw-rw-   0        0        0    26441 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_activitymanager.py
+-rw-rw-rw-   0        0        0    13587 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_adv.py
+-rw-rw-rw-   0        0        0     1184 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_advplace.py
+-rw-rw-rw-   0        0        0    10283 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_agreement.py
+-rw-rw-rw-   0        0        0     8389 2023-07-31 06:00:53.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_campmanager.py
+-rw-rw-rw-   0        0        0     7639 2023-07-31 06:01:00.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_comment.py
+-rw-rw-rw-   0        0        0     8748 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_commonquestion.py
+-rw-rw-rw-   0        0        0     1419 2023-07-31 06:00:58.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_contentmanager.py
+-rw-rw-rw-   0        0        0    14248 2023-07-31 06:01:00.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_essay.py
+-rw-rw-rw-   0        0        0     1317 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_essaycomment.py
+-rw-rw-rw-   0        0        0     4566 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_essayweb.py
+-rw-rw-rw-   0        0        0      859 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_hotcity.py
+-rw-rw-rw-   0        0        0     2952 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_hotsearch.py
+-rw-rw-rw-   0        0        0     6682 2023-07-31 06:01:00.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_material.py
+-rw-rw-rw-   0        0        0     9450 2023-07-31 06:00:55.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_messagemanager.py
+-rw-rw-rw-   0        0        0     3576 2023-07-31 06:00:55.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_noticemanager.py
+-rw-rw-rw-   0        0        0     5813 2023-07-31 06:01:00.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_question.py
+-rw-rw-rw-   0        0        0     2008 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_recruit.py
+-rw-rw-rw-   0        0        0     5100 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_safecode.py
+-rw-rw-rw-   0        0        0     9825 2023-07-31 06:01:00.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_subject.py
+-rw-rw-rw-   0        0        0     9388 2023-07-31 06:00:59.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_subjectweb.py
+-rw-rw-rw-   0        0        0     6365 2023-07-31 06:01:00.000000 huhk-1.9.1/service/app_a/apis/content/apis_content_topic4c.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.372918 huhk-1.9.1/service/app_a/apis/content/material/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/apis/content/material/__init__.py
+-rw-rw-rw-   0        0        0     1474 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/apis/content/material/apis_content_material_getmateriallist.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.413810 huhk-1.9.1/service/app_a/apis/goods/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:00:53.000000 huhk-1.9.1/service/app_a/apis/goods/__init__.py
+-rw-rw-rw-   0        0        0     9854 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/apis/goods/apis_goods_area.py
+-rw-rw-rw-   0        0        0    12191 2023-07-31 06:00:57.000000 huhk-1.9.1/service/app_a/apis/goods/apis_goods_carmodel.py
+-rw-rw-rw-   0        0        0    10643 2023-07-31 06:01:00.000000 huhk-1.9.1/service/app_a/apis/goods/apis_goods_configure.py
+-rw-rw-rw-   0        0        0     6170 2023-07-31 06:00:55.000000 huhk-1.9.1/service/app_a/apis/goods/apis_goods_ordermain.py
+-rw-rw-rw-   0        0        0     3147 2023-07-31 06:00:55.000000 huhk-1.9.1/service/app_a/apis/goods/apis_goods_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.419794 huhk-1.9.1/service/app_a/apis/manageapi/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/manageapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.432761 huhk-1.9.1/service/app_a/apis/manageapi/order/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/manageapi/order/__init__.py
+-rw-rw-rw-   0        0        0     8140 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/manageapi/order/apis_manageapi_order_mainorder.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.437747 huhk-1.9.1/service/app_a/apis/open/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:00:52.000000 huhk-1.9.1/service/app_a/apis/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.459687 huhk-1.9.1/service/app_a/apis/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:00:52.000000 huhk-1.9.1/service/app_a/apis/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      816 2023-07-31 06:00:52.000000 huhk-1.9.1/service/app_a/apis/open/haohan/apis_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      849 2023-07-31 06:00:52.000000 huhk-1.9.1/service/app_a/apis/open/haohan/apis_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.503827 huhk-1.9.1/service/app_a/apis/order/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:00:52.000000 huhk-1.9.1/service/app_a/apis/order/__init__.py
+-rw-rw-rw-   0        0        0     2652 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/apis/order/apis_order_freeorder.py
+-rw-rw-rw-   0        0        0    23046 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/order/apis_order_mainorder.py
+-rw-rw-rw-   0        0        0     3724 2023-07-31 06:00:55.000000 huhk-1.9.1/service/app_a/apis/order/apis_order_order.py
+-rw-rw-rw-   0        0        0    11987 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/order/apis_order_rightsorder.py
+-rw-rw-rw-   0        0        0     2582 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/apis/order/apis_order_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.518788 huhk-1.9.1/service/app_a/apis/order/mainorder/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/order/mainorder/__init__.py
+-rw-rw-rw-   0        0        0     1125 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/order/mainorder/apis_order_mainorder_scrm2app.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.541725 huhk-1.9.1/service/app_a/apis/order/rights/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/order/rights/__init__.py
+-rw-rw-rw-   0        0        0    10735 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/order/rights/apis_order_rights_rightsmanager.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.566660 huhk-1.9.1/service/app_a/apis/order/rightsorder/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/order/rightsorder/__init__.py
+-rw-rw-rw-   0        0        0     2379 2023-07-31 06:00:56.000000 huhk-1.9.1/service/app_a/apis/order/rightsorder/apis_order_rightsorder_receive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.578626 huhk-1.9.1/service/app_a/apis/pay/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:00:55.000000 huhk-1.9.1/service/app_a/apis/pay/__init__.py
+-rw-rw-rw-   0        0        0      865 2023-07-31 06:00:55.000000 huhk-1.9.1/service/app_a/apis/pay/apis_pay_orderpaybill.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.613535 huhk-1.9.1/service/app_a/apis/radarpoints/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.620515 huhk-1.9.1/service/app_a/apis/radarpoints/adjustpoints/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/adjustpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.642457 huhk-1.9.1/service/app_a/apis/radarpoints/adjustpoints/adjust/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/adjustpoints/adjust/__init__.py
+-rw-rw-rw-   0        0        0     3883 2023-07-31 06:00:55.000000 huhk-1.9.1/service/app_a/apis/radarpoints/adjustpoints/adjust/apis_radarpoints_adjustpoints_adjust_batch.py
+-rw-rw-rw-   0        0        0     1699 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/adjustpoints/adjust/apis_radarpoints_adjustpoints_adjust_single.py
+-rw-rw-rw-   0        0        0     6180 2023-07-31 06:00:55.000000 huhk-1.9.1/service/app_a/apis/radarpoints/apis_radarpoints_adjustpoints.py
+-rw-rw-rw-   0        0        0     7225 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/apis_radarpoints_pointsconfig.py
+-rw-rw-rw-   0        0        0     3763 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/apis_radarpoints_pointstask.py
+-rw-rw-rw-   0        0        0     2247 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/apis_radarpoints_summarystatistics.py
+-rw-rw-rw-   0        0        0     6270 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/apis_radarpoints_userpoints.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.665398 huhk-1.9.1/service/app_a/apis/radarpoints/userpoints/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/userpoints/__init__.py
+-rw-rw-rw-   0        0        0     1871 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/userpoints/apis_radarpoints_userpoints_exchangeinfo.py
+-rw-rw-rw-   0        0        0     2061 2023-07-31 06:00:54.000000 huhk-1.9.1/service/app_a/apis/radarpoints/userpoints/apis_radarpoints_userpoints_pointsinfo.py
+-rw-rw-rw-   0        0        0      752 2023-07-31 05:25:05.000000 huhk-1.9.1/service/app_a/app_a_fun.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.702555 huhk-1.9.1/service/app_a/asserts/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:00:52.000000 huhk-1.9.1/service/app_a/asserts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.719510 huhk-1.9.1/service/app_a/asserts/admin/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/admin/__init__.py
+-rw-rw-rw-   0        0        0      941 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/admin/asserts_admin_guc.py
+-rw-rw-rw-   0        0        0      552 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/admin/asserts_admin_spa.py
+-rw-rw-rw-   0        0        0      626 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/asserts_activitymanager.py
+-rw-rw-rw-   0        0        0      653 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/asserts_app_a.py
+-rw-rw-rw-   0        0        0      525 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/asserts_area.py
+-rw-rw-rw-   0        0        0      536 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/asserts_content.py
+-rw-rw-rw-   0        0        0     1009 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/asserts_essay.py
+-rw-rw-rw-   0        0        0      707 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/asserts_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.758403 huhk-1.9.1/service/app_a/asserts/common/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/common/__init__.py
+-rw-rw-rw-   0        0        0      587 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/common/asserts_common_clue.py
+-rw-rw-rw-   0        0        0      581 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/common/asserts_common_common.py
+-rw-rw-rw-   0        0        0      712 2023-07-31 06:09:08.000000 huhk-1.9.1/service/app_a/asserts/common/asserts_common_remoteinterfacelog.py
+-rw-rw-rw-   0        0        0     1116 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/common/asserts_common_systemversion.py
+-rw-rw-rw-   0        0        0      579 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/common/asserts_common_user.py
+-rw-rw-rw-   0        0        0     6848 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/common/asserts_common_user4c.py
+-rw-rw-rw-   0        0        0     2174 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/common/asserts_common_userpointsmanage.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.871862 huhk-1.9.1/service/app_a/asserts/content/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/content/__init__.py
+-rw-rw-rw-   0        0        0     7782 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_activitymanager.py
+-rw-rw-rw-   0        0        0     5226 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_adv.py
+-rw-rw-rw-   0        0        0      653 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_advplace.py
+-rw-rw-rw-   0        0        0     3600 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_agreement.py
+-rw-rw-rw-   0        0        0     2959 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_campmanager.py
+-rw-rw-rw-   0        0        0     2532 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_comment.py
+-rw-rw-rw-   0        0        0     4032 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_commonquestion.py
+-rw-rw-rw-   0        0        0      649 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_contentmanager.py
+-rw-rw-rw-   0        0        0     4302 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_essay.py
+-rw-rw-rw-   0        0        0      664 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_essaycomment.py
+-rw-rw-rw-   0        0        0     1937 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_essayweb.py
+-rw-rw-rw-   0        0        0      582 2023-07-31 06:01:05.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_hotcity.py
+-rw-rw-rw-   0        0        0     1432 2023-07-31 06:01:05.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_hotsearch.py
+-rw-rw-rw-   0        0        0     3121 2023-07-31 06:01:05.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_material.py
+-rw-rw-rw-   0        0        0     3611 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_messagemanager.py
+-rw-rw-rw-   0        0        0     1560 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_noticemanager.py
+-rw-rw-rw-   0        0        0     1960 2023-07-31 06:01:05.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_question.py
+-rw-rw-rw-   0        0        0      998 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_recruit.py
+-rw-rw-rw-   0        0        0     2216 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_safecode.py
+-rw-rw-rw-   0        0        0     3677 2023-07-31 06:01:05.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_subject.py
+-rw-rw-rw-   0        0        0     3368 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_subjectweb.py
+-rw-rw-rw-   0        0        0     2290 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/content/asserts_content_topic4c.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.884828 huhk-1.9.1/service/app_a/asserts/content/material/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/content/material/__init__.py
+-rw-rw-rw-   0        0        0      717 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/content/material/asserts_content_material_getmateriallist.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.918492 huhk-1.9.1/service/app_a/asserts/goods/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/goods/__init__.py
+-rw-rw-rw-   0        0        0     3466 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/goods/asserts_goods_area.py
+-rw-rw-rw-   0        0        0     3208 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/goods/asserts_goods_carmodel.py
+-rw-rw-rw-   0        0        0     2408 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/goods/asserts_goods_configure.py
+-rw-rw-rw-   0        0        0     2048 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/goods/asserts_goods_ordermain.py
+-rw-rw-rw-   0        0        0     1164 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/goods/asserts_goods_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.923480 huhk-1.9.1/service/app_a/asserts/manageapi/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/manageapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.936444 huhk-1.9.1/service/app_a/asserts/manageapi/order/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/manageapi/order/__init__.py
+-rw-rw-rw-   0        0        0     1277 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/manageapi/order/asserts_manageapi_order_mainorder.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.940433 huhk-1.9.1/service/app_a/asserts/open/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.957388 huhk-1.9.1/service/app_a/asserts/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      625 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/open/haohan/asserts_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      613 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/open/haohan/asserts_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.985313 huhk-1.9.1/service/app_a/asserts/order/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/asserts/order/__init__.py
+-rw-rw-rw-   0        0        0      824 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/order/asserts_order_freeorder.py
+-rw-rw-rw-   0        0        0     7067 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/order/asserts_order_mainorder.py
+-rw-rw-rw-   0        0        0     1428 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/order/asserts_order_order.py
+-rw-rw-rw-   0        0        0     3268 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/order/asserts_order_rightsorder.py
+-rw-rw-rw-   0        0        0     1108 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/asserts/order/asserts_order_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:38.994289 huhk-1.9.1/service/app_a/asserts/order/mainorder/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/order/mainorder/__init__.py
+-rw-rw-rw-   0        0        0      704 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/order/mainorder/asserts_order_mainorder_scrm2app.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.003920 huhk-1.9.1/service/app_a/asserts/order/rights/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/order/rights/__init__.py
+-rw-rw-rw-   0        0        0     3944 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/order/rights/asserts_order_rights_rightsmanager.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.012895 huhk-1.9.1/service/app_a/asserts/order/rightsorder/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/order/rightsorder/__init__.py
+-rw-rw-rw-   0        0        0      890 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/asserts/order/rightsorder/asserts_order_rightsorder_receive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.020873 huhk-1.9.1/service/app_a/asserts/pay/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/pay/__init__.py
+-rw-rw-rw-   0        0        0      611 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/asserts/pay/asserts_pay_orderpaybill.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.046319 huhk-1.9.1/service/app_a/asserts/radarpoints/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.051305 huhk-1.9.1/service/app_a/asserts/radarpoints/adjustpoints/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/adjustpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.067262 huhk-1.9.1/service/app_a/asserts/radarpoints/adjustpoints/adjust/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/adjustpoints/adjust/__init__.py
+-rw-rw-rw-   0        0        0     1319 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/adjustpoints/adjust/asserts_radarpoints_adjustpoints_adjust_batch.py
+-rw-rw-rw-   0        0        0      817 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/adjustpoints/adjust/asserts_radarpoints_adjustpoints_adjust_single.py
+-rw-rw-rw-   0        0        0     2203 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/asserts_radarpoints_adjustpoints.py
+-rw-rw-rw-   0        0        0     2272 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/asserts_radarpoints_pointsconfig.py
+-rw-rw-rw-   0        0        0     1275 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/asserts_radarpoints_pointstask.py
+-rw-rw-rw-   0        0        0     1163 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/asserts_radarpoints_summarystatistics.py
+-rw-rw-rw-   0        0        0     1660 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/asserts_radarpoints_userpoints.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.084221 huhk-1.9.1/service/app_a/asserts/radarpoints/userpoints/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/userpoints/__init__.py
+-rw-rw-rw-   0        0        0      807 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/userpoints/asserts_radarpoints_userpoints_exchangeinfo.py
+-rw-rw-rw-   0        0        0      783 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/asserts/radarpoints/userpoints/asserts_radarpoints_userpoints_pointsinfo.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.151282 huhk-1.9.1/service/app_a/funs/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:13:45.000000 huhk-1.9.1/service/app_a/funs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.163396 huhk-1.9.1/service/app_a/funs/admin/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/admin/__init__.py
+-rw-rw-rw-   0        0        0     1065 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/admin/funs_admin_guc.py
+-rw-rw-rw-   0        0        0      647 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/admin/funs_admin_spa.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.195342 huhk-1.9.1/service/app_a/funs/common/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/common/__init__.py
+-rw-rw-rw-   0        0        0      928 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/common/funs_common_clue.py
+-rw-rw-rw-   0        0        0      709 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/common/funs_common_common.py
+-rw-rw-rw-   0        0        0     1795 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/common/funs_common_remoteinterfacelog.py
+-rw-rw-rw-   0        0        0     2804 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/common/funs_common_systemversion.py
+-rw-rw-rw-   0        0        0      729 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/common/funs_common_user.py
+-rw-rw-rw-   0        0        0    21622 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/common/funs_common_user4c.py
+-rw-rw-rw-   0        0        0     6180 2023-07-31 07:18:02.000000 huhk-1.9.1/service/app_a/funs/common/funs_common_userpointsmanage.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.292315 huhk-1.9.1/service/app_a/funs/content/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:18:02.000000 huhk-1.9.1/service/app_a/funs/content/__init__.py
+-rw-rw-rw-   0        0        0    26429 2023-07-31 07:18:02.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_activitymanager.py
+-rw-rw-rw-   0        0        0    11631 2023-07-31 07:18:02.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_adv.py
+-rw-rw-rw-   0        0        0     1482 2023-07-31 07:18:02.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_advplace.py
+-rw-rw-rw-   0        0        0     7550 2023-07-31 07:18:02.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_agreement.py
+-rw-rw-rw-   0        0        0     8084 2023-07-31 07:18:02.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_campmanager.py
+-rw-rw-rw-   0        0        0     7904 2023-07-31 07:18:02.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_comment.py
+-rw-rw-rw-   0        0        0     7209 2023-07-31 07:18:02.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_commonquestion.py
+-rw-rw-rw-   0        0        0     1082 2023-07-31 07:18:02.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_contentmanager.py
+-rw-rw-rw-   0        0        0    13476 2023-07-31 07:18:03.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_essay.py
+-rw-rw-rw-   0        0        0     1526 2023-07-31 07:18:03.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_essaycomment.py
+-rw-rw-rw-   0        0        0     4715 2023-07-31 07:18:03.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_essayweb.py
+-rw-rw-rw-   0        0        0      694 2023-07-31 07:18:03.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_hotcity.py
+-rw-rw-rw-   0        0        0     2656 2023-07-31 07:18:03.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_hotsearch.py
+-rw-rw-rw-   0        0        0     5431 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_material.py
+-rw-rw-rw-   0        0        0    10631 2023-07-31 07:18:03.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_messagemanager.py
+-rw-rw-rw-   0        0        0     2868 2023-07-31 07:18:03.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_noticemanager.py
+-rw-rw-rw-   0        0        0     4376 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_question.py
+-rw-rw-rw-   0        0        0     1529 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_recruit.py
+-rw-rw-rw-   0        0        0     3317 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_safecode.py
+-rw-rw-rw-   0        0        0     8951 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_subject.py
+-rw-rw-rw-   0        0        0     9433 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_subjectweb.py
+-rw-rw-rw-   0        0        0     4900 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/content/funs_content_topic4c.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.302564 huhk-1.9.1/service/app_a/funs/content/material/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/content/material/__init__.py
+-rw-rw-rw-   0        0        0     1219 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/content/material/funs_content_material_getmateriallist.py
+-rw-rw-rw-   0        0        0     1130 2023-07-31 07:13:45.000000 huhk-1.9.1/service/app_a/funs/funs_activitymanager.py
+-rw-rw-rw-   0        0        0      194 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/funs_admin.py
+-rw-rw-rw-   0        0        0     3167 2023-07-31 07:18:06.000000 huhk-1.9.1/service/app_a/funs/funs_app_a.py
+-rw-rw-rw-   0        0        0      599 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/funs_area.py
+-rw-rw-rw-   0        0        0      761 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/funs_common.py
+-rw-rw-rw-   0        0        0     3101 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/funs_content.py
+-rw-rw-rw-   0        0        0     2527 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/funs_essay.py
+-rw-rw-rw-   0        0        0      506 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/funs_goods.py
+-rw-rw-rw-   0        0        0      140 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/funs_manageapi.py
+-rw-rw-rw-   0        0        0      118 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/funs_open.py
+-rw-rw-rw-   0        0        0      607 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/funs_order.py
+-rw-rw-rw-   0        0        0      131 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/funs_pay.py
+-rw-rw-rw-   0        0        0      698 2023-07-31 07:18:06.000000 huhk-1.9.1/service/app_a/funs/funs_radarpoints.py
+-rw-rw-rw-   0        0        0     2813 2023-07-31 07:18:01.000000 huhk-1.9.1/service/app_a/funs/funs_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.329491 huhk-1.9.1/service/app_a/funs/goods/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/goods/__init__.py
+-rw-rw-rw-   0        0        0     6559 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/goods/funs_goods_area.py
+-rw-rw-rw-   0        0        0    11252 2023-07-31 07:18:04.000000 huhk-1.9.1/service/app_a/funs/goods/funs_goods_carmodel.py
+-rw-rw-rw-   0        0        0    10293 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/goods/funs_goods_configure.py
+-rw-rw-rw-   0        0        0     5322 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/goods/funs_goods_ordermain.py
+-rw-rw-rw-   0        0        0     3626 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/goods/funs_goods_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.339469 huhk-1.9.1/service/app_a/funs/manageapi/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/manageapi/__init__.py
+-rw-rw-rw-   0        0        0      179 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/manageapi/funs_manageapi_order.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.348448 huhk-1.9.1/service/app_a/funs/manageapi/order/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/manageapi/order/__init__.py
+-rw-rw-rw-   0        0        0     4282 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/manageapi/order/funs_manageapi_order_mainorder.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.356421 huhk-1.9.1/service/app_a/funs/open/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/open/__init__.py
+-rw-rw-rw-   0        0        0      267 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/open/funs_open_haohan.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.368389 huhk-1.9.1/service/app_a/funs/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      869 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/open/haohan/funs_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      959 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/open/haohan/funs_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.395313 huhk-1.9.1/service/app_a/funs/order/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/__init__.py
+-rw-rw-rw-   0        0        0     3970 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/funs_order_freeorder.py
+-rw-rw-rw-   0        0        0    19335 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/funs_order_mainorder.py
+-rw-rw-rw-   0        0        0     2770 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/funs_order_order.py
+-rw-rw-rw-   0        0        0      176 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/funs_order_rights.py
+-rw-rw-rw-   0        0        0    12237 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/funs_order_rightsorder.py
+-rw-rw-rw-   0        0        0     2884 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/funs_order_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.403292 huhk-1.9.1/service/app_a/funs/order/mainorder/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/mainorder/__init__.py
+-rw-rw-rw-   0        0        0     1373 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/mainorder/funs_order_mainorder_scrm2app.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.412884 huhk-1.9.1/service/app_a/funs/order/rights/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/rights/__init__.py
+-rw-rw-rw-   0        0        0     9168 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/rights/funs_order_rights_rightsmanager.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.421088 huhk-1.9.1/service/app_a/funs/order/rightsorder/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/rightsorder/__init__.py
+-rw-rw-rw-   0        0        0     3959 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/order/rightsorder/funs_order_rightsorder_receive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.430071 huhk-1.9.1/service/app_a/funs/pay/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/pay/__init__.py
+-rw-rw-rw-   0        0        0      900 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/pay/funs_pay_orderpaybill.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.457744 huhk-1.9.1/service/app_a/funs/radarpoints/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/radarpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.467715 huhk-1.9.1/service/app_a/funs/radarpoints/adjustpoints/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/radarpoints/adjustpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.482678 huhk-1.9.1/service/app_a/funs/radarpoints/adjustpoints/adjust/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/radarpoints/adjustpoints/adjust/__init__.py
+-rw-rw-rw-   0        0        0     4080 2023-07-31 07:18:06.000000 huhk-1.9.1/service/app_a/funs/radarpoints/adjustpoints/adjust/funs_radarpoints_adjustpoints_adjust_batch.py
+-rw-rw-rw-   0        0        0     2099 2023-07-31 07:18:06.000000 huhk-1.9.1/service/app_a/funs/radarpoints/adjustpoints/adjust/funs_radarpoints_adjustpoints_adjust_single.py
+-rw-rw-rw-   0        0        0      433 2023-07-31 07:18:06.000000 huhk-1.9.1/service/app_a/funs/radarpoints/adjustpoints/funs_radarpoints_adjustpoints_adjust.py
+-rw-rw-rw-   0        0        0     5930 2023-07-31 07:18:06.000000 huhk-1.9.1/service/app_a/funs/radarpoints/funs_radarpoints_adjustpoints.py
+-rw-rw-rw-   0        0        0     8017 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/radarpoints/funs_radarpoints_pointsconfig.py
+-rw-rw-rw-   0        0        0     4126 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/radarpoints/funs_radarpoints_pointstask.py
+-rw-rw-rw-   0        0        0     2339 2023-07-31 07:18:05.000000 huhk-1.9.1/service/app_a/funs/radarpoints/funs_radarpoints_summarystatistics.py
+-rw-rw-rw-   0        0        0     7883 2023-07-31 07:18:06.000000 huhk-1.9.1/service/app_a/funs/radarpoints/funs_radarpoints_userpoints.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.501624 huhk-1.9.1/service/app_a/funs/radarpoints/userpoints/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:18:06.000000 huhk-1.9.1/service/app_a/funs/radarpoints/userpoints/__init__.py
+-rw-rw-rw-   0        0        0     2066 2023-07-31 07:18:06.000000 huhk-1.9.1/service/app_a/funs/radarpoints/userpoints/funs_radarpoints_userpoints_exchangeinfo.py
+-rw-rw-rw-   0        0        0     2169 2023-07-31 07:18:06.000000 huhk-1.9.1/service/app_a/funs/radarpoints/userpoints/funs_radarpoints_userpoints_pointsinfo.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.536537 huhk-1.9.1/service/app_a/sqls/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:00:52.000000 huhk-1.9.1/service/app_a/sqls/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.551214 huhk-1.9.1/service/app_a/sqls/admin/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/admin/__init__.py
+-rw-rw-rw-   0        0        0     1026 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/admin/sqls_admin_guc.py
+-rw-rw-rw-   0        0        0      552 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/admin/sqls_admin_spa.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.582131 huhk-1.9.1/service/app_a/sqls/common/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/common/__init__.py
+-rw-rw-rw-   0        0        0      563 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/common/sqls_common_clue.py
+-rw-rw-rw-   0        0        0      562 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/common/sqls_common_common.py
+-rw-rw-rw-   0        0        0      586 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/common/sqls_common_remoteinterfacelog.py
+-rw-rw-rw-   0        0        0     1050 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/common/sqls_common_systemversion.py
+-rw-rw-rw-   0        0        0      563 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/common/sqls_common_user.py
+-rw-rw-rw-   0        0        0     6794 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/common/sqls_common_user4c.py
+-rw-rw-rw-   0        0        0     2069 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/common/sqls_common_userpointsmanage.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.663639 huhk-1.9.1/service/app_a/sqls/content/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/content/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.672615 huhk-1.9.1/service/app_a/sqls/content/material/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/content/material/__init__.py
+-rw-rw-rw-   0        0        0      602 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/content/material/sqls_content_material_getmateriallist.py
+-rw-rw-rw-   0        0        0     7456 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_activitymanager.py
+-rw-rw-rw-   0        0        0     5815 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_adv.py
+-rw-rw-rw-   0        0        0      568 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_advplace.py
+-rw-rw-rw-   0        0        0     3943 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_agreement.py
+-rw-rw-rw-   0        0        0     2981 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_campmanager.py
+-rw-rw-rw-   0        0        0     2480 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_comment.py
+-rw-rw-rw-   0        0        0     4458 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_commonquestion.py
+-rw-rw-rw-   0        0        0      581 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_contentmanager.py
+-rw-rw-rw-   0        0        0     4379 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_essay.py
+-rw-rw-rw-   0        0        0      575 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_essaycomment.py
+-rw-rw-rw-   0        0        0     2002 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_essayweb.py
+-rw-rw-rw-   0        0        0      560 2023-07-31 06:01:05.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_hotcity.py
+-rw-rw-rw-   0        0        0     1520 2023-07-31 06:01:05.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_hotsearch.py
+-rw-rw-rw-   0        0        0     3466 2023-07-31 06:01:05.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_material.py
+-rw-rw-rw-   0        0        0     3504 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_messagemanager.py
+-rw-rw-rw-   0        0        0     1564 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_noticemanager.py
+-rw-rw-rw-   0        0        0     2022 2023-07-31 06:01:05.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_question.py
+-rw-rw-rw-   0        0        0     1037 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_recruit.py
+-rw-rw-rw-   0        0        0     2474 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_safecode.py
+-rw-rw-rw-   0        0        0     3917 2023-07-31 06:01:05.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_subject.py
+-rw-rw-rw-   0        0        0     3455 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_subjectweb.py
+-rw-rw-rw-   0        0        0     2470 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/content/sqls_content_topic4c.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.697550 huhk-1.9.1/service/app_a/sqls/goods/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/goods/__init__.py
+-rw-rw-rw-   0        0        0     3904 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/goods/sqls_goods_area.py
+-rw-rw-rw-   0        0        0     3000 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/goods/sqls_goods_carmodel.py
+-rw-rw-rw-   0        0        0     2521 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/goods/sqls_goods_configure.py
+-rw-rw-rw-   0        0        0     2016 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/goods/sqls_goods_ordermain.py
+-rw-rw-rw-   0        0        0     1043 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/goods/sqls_goods_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.702538 huhk-1.9.1/service/app_a/sqls/manageapi/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/manageapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.711513 huhk-1.9.1/service/app_a/sqls/manageapi/order/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/manageapi/order/__init__.py
+-rw-rw-rw-   0        0        0     1070 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/manageapi/order/sqls_manageapi_order_mainorder.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.716498 huhk-1.9.1/service/app_a/sqls/open/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.729856 huhk-1.9.1/service/app_a/sqls/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      571 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/open/haohan/sqls_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      567 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/open/haohan/sqls_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.754771 huhk-1.9.1/service/app_a/sqls/order/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:01.000000 huhk-1.9.1/service/app_a/sqls/order/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.764748 huhk-1.9.1/service/app_a/sqls/order/mainorder/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/order/mainorder/__init__.py
+-rw-rw-rw-   0        0        0      590 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/order/mainorder/sqls_order_mainorder_scrm2app.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.772724 huhk-1.9.1/service/app_a/sqls/order/rights/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/order/rights/__init__.py
+-rw-rw-rw-   0        0        0     4025 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/order/rights/sqls_order_rights_rightsmanager.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.779504 huhk-1.9.1/service/app_a/sqls/order/rightsorder/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/order/rightsorder/__init__.py
+-rw-rw-rw-   0        0        0      581 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/order/rightsorder/sqls_order_rightsorder_receive.py
+-rw-rw-rw-   0        0        0      564 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/order/sqls_order_freeorder.py
+-rw-rw-rw-   0        0        0     7363 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/order/sqls_order_mainorder.py
+-rw-rw-rw-   0        0        0     1511 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/order/sqls_order_order.py
+-rw-rw-rw-   0        0        0     2972 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/order/sqls_order_rightsorder.py
+-rw-rw-rw-   0        0        0     1045 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/order/sqls_order_testdrive.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.786515 huhk-1.9.1/service/app_a/sqls/pay/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/pay/__init__.py
+-rw-rw-rw-   0        0        0      569 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/pay/sqls_pay_orderpaybill.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.806530 huhk-1.9.1/service/app_a/sqls/radarpoints/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.809522 huhk-1.9.1/service/app_a/sqls/radarpoints/adjustpoints/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/adjustpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.822515 huhk-1.9.1/service/app_a/sqls/radarpoints/adjustpoints/adjust/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/adjustpoints/adjust/__init__.py
+-rw-rw-rw-   0        0        0     1101 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/adjustpoints/adjust/sqls_radarpoints_adjustpoints_adjust_batch.py
+-rw-rw-rw-   0        0        0      604 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/adjustpoints/adjust/sqls_radarpoints_adjustpoints_adjust_single.py
+-rw-rw-rw-   0        0        0     2076 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/sqls_radarpoints_adjustpoints.py
+-rw-rw-rw-   0        0        0     2046 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/sqls_radarpoints_pointsconfig.py
+-rw-rw-rw-   0        0        0     1062 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/sqls_radarpoints_pointstask.py
+-rw-rw-rw-   0        0        0     1083 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/sqls_radarpoints_summarystatistics.py
+-rw-rw-rw-   0        0        0     1062 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/sqls_radarpoints_userpoints.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.831978 huhk-1.9.1/service/app_a/sqls/radarpoints/userpoints/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/userpoints/__init__.py
+-rw-rw-rw-   0        0        0      603 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/userpoints/sqls_radarpoints_userpoints_exchangeinfo.py
+-rw-rw-rw-   0        0        0      599 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/radarpoints/userpoints/sqls_radarpoints_userpoints_pointsinfo.py
+-rw-rw-rw-   0        0        0      574 2023-07-31 06:01:02.000000 huhk-1.9.1/service/app_a/sqls/sqls_activitymanager.py
+-rw-rw-rw-   0        0        0      534 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/sqls_app_a.py
+-rw-rw-rw-   0        0        0      546 2023-07-31 06:01:06.000000 huhk-1.9.1/service/app_a/sqls/sqls_area.py
+-rw-rw-rw-   0        0        0      545 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/sqls_content.py
+-rw-rw-rw-   0        0        0     1017 2023-07-31 06:01:04.000000 huhk-1.9.1/service/app_a/sqls/sqls_essay.py
+-rw-rw-rw-   0        0        0      554 2023-07-31 06:01:03.000000 huhk-1.9.1/service/app_a/sqls/sqls_testdrive.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 01:44:39.852923 huhk-1.9.1/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.834970 huhk-1.9.1/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:02:47.000000 huhk-1.9.1/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:44:39.846910 huhk-1.9.1/testcase/app_a/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:02:47.000000 huhk-1.9.1/testcase/app_a/__init__.py
+-rw-rw-rw-   0        0        0      361 2023-07-31 06:02:47.000000 huhk-1.9.1/testcase/app_a/conftest.py
+-rw-rw-rw-   0        0        0     3184 2023-07-31 07:18:01.000000 huhk-1.9.1/testcase/app_a/test_page.py
```

### Comparing `huhk-1.8.9/huhk/__init__.py` & `huhk-1.9.1/huhk/__init__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/huhk/case_project/json_coder.py` & `huhk-1.9.1/huhk/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/huhk/case_project/main_fun.py` & `huhk-1.9.1/huhk/case_project/main_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/huhk/case_project/project_base.py` & `huhk-1.9.1/huhk/case_project/project_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,16 @@
 
     def set_service_value(self, key, value, _type=0):
         """设置项目本地变量"""
         self._set_service_value(key=key, value=value, name=self.name, _type=_type)
 
     def get_api_attribute(self, file_str, api_file):
         try:
+            if api_file == 'D:\\projects\\python_test\\huhk-common\\service\\app_a\\apis\\content\\apis_content_essay.py':
+                print()
             fun_list = re.findall(r"\ndef +([^_].+)?\((.*?)\):\s*"
                                   r"([\'\"]{3}"
                                   r"\s*(.*?)?\s*up_time=(\d+)?[\w\W]*?"
                                   r"(    params:[\w\W]*?)?(====[\w\W]*?)?"
                                   r"[\'\"]{3})?"
                                   r"[\w\W]*?_method *= *[\"\'](\S+?)[\"\']"
                                   r"[\w\W]*?_url *= *[\"\'](\S+?)[\"\']"
@@ -92,27 +94,30 @@
                 self.this_fun_list.api[fun[0]].params = fun[5]
                 self.this_fun_list.api[fun[0]].method = fun[7]
                 self.this_fun_list.api[fun[0]].url = fun[8]
         except Exception as e:
             logger.error(str(e))
 
     def get_this_fun_list(self):
-        last_time = self.get_service_value("last_time")
-        # self.set_service_value("last_time", time.time())
-        service_dir = os.path.join(self.path.dir, 'service', self.name)
-        for dirpath, dirnames, filenames in os.walk(service_dir):
-            for filename in filenames:
-                key = filename.split("_")[0]
-                if key in self.this_file_list.keys():
-                    if not (key == "api" and last_time and
-                            os.stat(os.path.join(dirpath, filename)).st_mtime < last_time):
-                        self.this_file_list[key].append(os.path.join(dirpath, filename))
-        for api_file in self.this_file_list.get('api'):
-            file_str = FunBase.read_file(api_file)
-            self.get_api_attribute(file_str, api_file)
+        try:
+            last_time = self.get_service_value("last_time")
+            # self.set_service_value("last_time", time.time())
+            service_dir = os.path.join(self.path.dir, 'service', self.name)
+            for dirpath, dirnames, filenames in os.walk(service_dir):
+                for filename in filenames:
+                    key = filename.split("_")[0]
+                    if key in self.this_file_list.keys() and filename[-3:] == ".py":
+                        if not (key == "apis" and last_time and
+                                os.stat(os.path.join(dirpath, filename)).st_mtime < last_time):
+                            self.this_file_list[key].append(os.path.join(dirpath, filename))
+            for api_file in self.this_file_list.get('apis'):
+                file_str = FunBase.read_file(api_file)
+                self.get_api_attribute(file_str, api_file)
+        except Exception as e:
+            print(e)
 
     def get_project(self):
         if self.app_key:
             project = requests.post(self.url + '/variable/variable/',
                                     json={"app_key": self.app_key, "environment": "sit"}).json()
             if project.get('project'):
                 self.name = self.name or project.get('project')[0].get('code')
@@ -148,15 +153,16 @@
                 api = Dict()
                 api.path = data.basePath + k
                 for k2, v2 in v.items():
                     api.method = k2
                     api.title = v2.get('summary', "")
                     api.up_time = int(time.time())
                     api.req_headers = [{'name': 'Content-Type', 'desc': '',
-                                        'value': v2.consumes[0] if v2.consumes else "application/x-www-form-urlencoded"}]
+                                        'value': v2.consumes[
+                                            0] if v2.consumes else "application/x-www-form-urlencoded"}]
                     api["req_params"] = []
                     api["req_query"] = []
                     api["req_body_other"] = []
                     api["res_body"] = []
                     for parameter in v2.get('parameters', []):
                         if parameter.get('in') == "body":
                             if parameter.get('name') not in ("params", "headers"):
@@ -277,23 +283,21 @@
                 file_str = "if __name__ == '__main__':".join(tmp_list)
                 FunBase.write_file(assert_path.path, file_str)
         else:
             file_str = self.get_assert_header_str(assert_path.class_name, sql_path) + self.get_assert_fun_str(fun_name)
             FunBase.mkdir_file(assert_path.path)
             FunBase.write_file(assert_path.path, file_str)
 
-    def set_api_fun_header(self, fun_name, type=1):
+    def set_api_fun_header(self, fun_name):
+        fun_name = fun_name.strip(" _")
+
         def _fun_header():
-            if type == 1:
-                new_str = f"from {fun_path.import_path} import {fun_path.class_name}\n\n\n" \
-                          f"class {fun_path2.class_name}({fun_path.class_name}):\n    pass\n\n"
-            else:
-                new_str = f"from {fun_path.import_path} import {fun_path.class_name}\n\n\n" \
-                          f"class {fun_path2.class_name}({fun_path.class_name}):\n    pass\n\n"
-            return new_str
+            return f"from {fun_path.import_path} import {fun_path.class_name}\n\n\n" \
+                   f"class {fun_path2.class_name}({fun_path.class_name}):\n    pass\n\n"
+
         fun_path = self.get_path(fun_name, fun_type="funs")
         if fun_name.count('_') > 0:
             # path = fun_path.path.rsplit('_', 1)[0] + '.py'
             fun_path2 = self.get_path(fun_name.rsplit('_', 1)[0], fun_type='funs')
             path = fun_path2.path
             if os.path.exists(path):
                 old_str = FunBase.read_file(path)
@@ -306,23 +310,23 @@
                     new_str = "".join(old_str_l)
                 else:
                     new_str = _fun_header()
             else:
                 new_str = _fun_header()
             FunBase.write_file(path, new_str)
             if fun_name.count('_') > 1:
-                self.set_api_fun_header(fun_name.rsplit('_', 1)[0], type=2)
+                self.set_api_fun_header(fun_name.rsplit('_', 1)[0])
         else:
             print("Warning")
 
     def write_api_fun(self, fun_name, _update=False):
         fun_path = self.get_path(fun_name, fun_type='funs')
 
         if os.path.exists(fun_path.path):
-            file_str = FunBase.read_file(fun_path.path).replace("    pass\n", "")
+            file_str = FunBase.read_file(fun_path.path).replace("    pass\n\n", "").replace("    pass\n", "")
             ord_str = re.findall(
                 r'\n((    @allure.step\(.*\) *\n)?    def %s\(.+\)[\w\W]*?)(\n    @allure.step\(|\n    def|$)' %
                 fun_name, file_str)
             if ord_str:
                 if _update:
                     new_str = self.get_api_fun_fun_str(fun_name)
                     file_str = file_str.replace(ord_str[0][0], new_str)
```

### Comparing `huhk-1.8.9/huhk/case_project/project_string.py` & `huhk-1.9.1/huhk/case_project/project_string.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,25 @@
         value += '            return out.get("data")\n        else:\n'
         value += '            assert False, sql_str + str(out.get("msg"))\n\n\n'
         value += f"if __name__ == '__main__':\n    f = {self.name2.replace('_', '')}Fun()\n"
         value += '    out = f.faker().name()\n'
         value += '    print(out)\n\n'
         return value
 
+    def get_conftest_value(self):
+        """生成标签文件"""
+        value = ("import pytest\n\n\ndef pytest_configure(config):\n"
+                 '    config.addinivalue_line("markers", "smoke:冒烟用例")\n'
+                 '    config.addinivalue_line("markers", "success:正向用例")\n'
+                 '    config.addinivalue_line("markers", "failed:逆向用例")\n'
+                 '    config.addinivalue_line("markers", "get:查询用例")\n'
+                 '    config.addinivalue_line("markers", "fun:功能用例")\n\n')
+
+        return value
+
     @staticmethod
     def get_params_string(req_all, res_body):
         """方法描述生成"""
         def get_str(l):
             _str = ""
             for p in l:
                 _str += f'    params: {p.get("name", "")} : {p.get("type", "")} : {p.get("desc", "")}\n'
@@ -125,15 +136,15 @@
                 '"%s"' % p.get("value", "") if value else p.get("name", "")) + ","
             json_str += ("  # " + p.get("desc").replace('\n', ' ') if p.get("desc") else "") + '\n'
         json_str += '    }'
         return json_str
 
     @staticmethod
     def get_fun_name(name):
-        name = re.sub(r'\W', '_', name.split('{')[0]).strip().lstrip('_')
+        name = re.sub(r'\W', '_', name.split('{')[0]).strip().lstrip('_').lower()
         return name
 
     def get_path(self, name, fun_type="apis"):
         name_l = [i for i in name.split('_') if i]
         out = Dict()
         if fun_type == "api" and self.this_fun_list.api[name]:
             filename = self.this_fun_list.api[name].path
@@ -154,15 +165,15 @@
 
     def get_api_header_str(self):
         api_header_str = f"import allure\n\nfrom service.{self.name} import http_requester\n" \
                          f"from huhk.unit_request import get_url\n\n\n"
         return api_header_str
 
     def get_api_fun_str(self, name, row):
-        if self.api_type == 1:
+        if self.yapi_url and self.yapi_token:
             data = {"token": self.yapi_token, "id": row.get('_id')}
             res = requests.get(self.yapi_url + "/api/interface/get", data=data)
             row = Dict(json.loads(res.text)).get('data')
         api_str = '@allure.step(title="调接口：%s")\n' % row.get("path").split('{')[0]
         api_str += "def " + name + "("
         req_params = row.get('req_params', [])
         req_query = row.get('req_query', [])
@@ -236,14 +247,15 @@
         api_path = self.get_path(fun_name, fun_type='apis')
         header_str = "import allure\n"
         if header_str not in file_str:
             file_str = header_str + file_str
         header_str = f"from {assert_path.import_path} import {assert_path.class_name}\n"
         if header_str not in file_str:
             file_str = header_str + file_str
+            file_str = file_str.replace("):", f", {assert_path.class_name}):", 1)
         header_str = f"from {api_path.import_path.rsplit('.', 1)[0]} import {api_path.import_path.rsplit('.', 1)[1]}\n"
         if header_str not in file_str:
             file_str = header_str + file_str
         return file_str
 
     def get_api_fun_fun_str(self, fun_name):
         api_path = self.get_path(fun_name, fun_type='apis')
```

### Comparing `huhk-1.8.9/huhk/case_project/setup_set.py` & `huhk-1.9.1/huhk/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/huhk/init_project.py` & `huhk-1.9.1/huhk/init_project.py`

 * *Files 19% similar despite different names*

```diff
@@ -37,14 +37,16 @@
         if not os.path.exists(os.path.join(self.path.service_dir, "__init__.py")) or \
                 not FunBase.read_file(os.path.join(self.path.service_dir, "__init__.py")):
             FunBase.write_file(os.path.join(self.path.service_dir, "__init__.py"), value=self.get_init_value())
         if not os.path.exists(os.path.join(self.path.service_dir, f"{self.name}_fun.py")):
             FunBase.write_file(os.path.join(self.path.service_dir, f"{self.name}_fun.py"), value=self.get_fun_value())
         if not os.path.exists(os.path.join(self.path.service_dir, f"setting.json")):
             FunBase.write_file(os.path.join(self.path.service_dir, f"setting.json"), value="{}")
+        if not os.path.exists(os.path.join(self.path.testcase_dir, f"conftest.py")):
+            FunBase.write_file(os.path.join(self.path.testcase_dir, f"conftest.py"), value=self.get_conftest_value())
 
     def get_api_fun_list(self):
         """获取已维护方法列表，无则创建demo文件"""
         self.path.fun_file_path = os.path.join(self.path.service_dir, self.name + "_fun.py")
         if os.path.exists(self.path.fun_file_path):
             self.fun_file_str = FunBase.read_file(self.path.fun_file_path)
         else:
@@ -124,64 +126,14 @@
             self.write_api(row)
         for fun_name in self.this_fun_list.api.keys():
             self.write_sql(fun_name, _update=_update)
             self.write_assert(fun_name, _update=_update)
             self.write_api_fun(fun_name, _update=_update)
             self.write_testcase(fun_name, _update=_update)
 
-
-    def write_api_fun2(self):
-        for row in self.api_list:
-            fun_name = self.get_fun_name(row.get('path'))
-            if fun_name in self.api_list_old:
-                ord_str = re.findall(r'(def %s\(.+\)[\w\W]*?)(def|$)' % fun_name, self.api_file_str)
-                up_time = re.findall(r'up_time=(\d+)([\w\W]+)', ord_str[0][0])
-                if up_time and int(up_time[0][0]) < row.get('up_time'):
-                    new_str = self.get_api_fun_str(fun_name, row)
-                    self.api_file_str = self.api_file_str.replace(ord_str[0][0], new_str)
-            else:
-                self.api_list_old.append(fun_name)
-                self.api_file_str += self.get_api_fun_str(fun_name, row)
-        if not self.api_list_old:
-            self.api_list_old.append("demo")
-            self.api_file_str += """@allure.step(title="调接口：/demo")\ndef demo(mobile=None, headers=None, **kwargs):
-    \"""\n    发送手机验证码\n    up_time=1657087679\n\n    params: mobile :  : 用户电话号码
-    params: headers : 请求\n    ====================返回======================
-    params: code : number : \n    params: msg : string : \n    params: data : null : 
-    \"""\n    _method = "GET"\n    _url = "/common/common/sendSmsCode"\n
-    _headers = {\n        "Content-Type": "application/x-www-form-urlencoded",\n    }
-    _headers.update({"headers": headers})\n\n    _data = {\n        "mobile": mobile,  # 用户电话号码\n    }\n
-    _params = {\n    }\n
-    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)\n\n"""
-        for fun_name in self.api_list_old:
-            if fun_name not in self.api_fun_fun_list:
-                self.api_fun_fun_list.append(fun_name)
-                self.get_api_fun_fun_str(fun_name)
-        for fun_name in self.api_fun_fun_list:
-            if "assert_" + fun_name not in self.assert_fun_list and "self.assert_" + fun_name + '(' in self.api_fun_file_str:
-                self.assert_fun_list.append("assert_" + fun_name)
-                self.get_assert_fun_str(fun_name)
-        for fun_name in self.assert_fun_list:
-            fun_name = fun_name[7:]
-            if "sql_" + fun_name not in self.sql_fun_list and "self.sql_" + fun_name + '(' in self.assert_file_str:
-                self.sql_fun_list.append("sql_" + fun_name)
-                self.get_sql_fun_str(fun_name)
-        for fun_name in self.api_fun_fun_list:
-            if fun_name not in self.api_testcase_list:
-                self.api_testcase_list.append("test_" + fun_name)
-                self.get_api_testcase_str(fun_name)
-
-        FunBase.write_file(self.path.api_file_path, self.api_file_str)
-        FunBase.write_file(self.path.fun_file_path, self.fun_file_str)
-        FunBase.write_file(self.path.sql_file_path, self.sql_file_str)
-        FunBase.write_file(self.path.assert_file_path, self.assert_file_str)
-        FunBase.write_file(self.path.api_fun_file_path, self.api_fun_file_str)
-        FunBase.write_file(self.path.api_testcase_file_path, self.api_testcase_file_str)
-
-
     def sub_hz(self, _id, _str):
         if re.findall(r'[^\da-zA-Z_\ (=,*):]', re.findall(r"def .*?\):", _str)[0]):
             api = self.get_api(_id)
             tmp2 = api.get('data', {}).get('req_params', [])
             for tmp3 in tmp2:
                 name = tmp3.get('name', "")
                 desc = tmp3.get('desc', "")
```

### Comparing `huhk-1.8.9/huhk/main.py` & `huhk-1.9.1/huhk/main.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/huhk/testcase/apache/beam_class.py` & `huhk-1.9.1/huhk/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/huhk/testcase/apache/data.py` & `huhk-1.9.1/huhk/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/huhk/testcase/apache/par_do.py` & `huhk-1.9.1/huhk/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/huhk/testcase/apache/test_cogroupbykey.py` & `huhk-1.9.1/huhk/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/huhk/testcase/apache/test_fiter.py` & `huhk-1.9.1/huhk/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/huhk/testcase/apache/test_flatmap.py` & `huhk-1.9.1/huhk/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/huhk/testcase/apache/test_map.py` & `huhk-1.9.1/huhk/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/huhk/testcase/apache/test_par_do.py` & `huhk-1.9.1/huhk/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/huhk/testcase/apache/test_regex.py` & `huhk-1.9.1/huhk/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/huhk/testcase/apache/test_time.py` & `huhk-1.9.1/huhk/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/huhk/unit_apache_beam.py` & `huhk-1.9.1/huhk/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/huhk/unit_dict.py` & `huhk-1.9.1/huhk/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/huhk/unit_encryption.py` & `huhk-1.9.1/huhk/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/huhk/unit_fun.py` & `huhk-1.9.1/huhk/unit_fun.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # import pymysql
 from pandas import DataFrame, ExcelWriter
 from typing import List
 from faker import Faker
 
 from huhk.unit_dict import Dict
 from huhk.unit_logger import logger
+from unit_data import page_and_size, before_and_end, before_and_end_re_str
 
 
 class FunBase:
     def __init__(self):
         self._time2 = 0
         self._time1 = 0
         self.sql_str = ""
@@ -96,17 +97,17 @@
                 f.write(value)
         else:
             with open(file_path, mode, encoding=encoding, **kwargs) as f:
                 f.write(value)
 
 
     @staticmethod
-    def read_file(file_path, mode="r"):
+    def read_file(file_path, mode="r", encoding='utf-8', **kwargs):
         """读文件"""
-        with open(file_path, mode, encoding='utf-8') as f:
+        with open(file_path, mode, encoding=encoding, **kwargs) as f:
             value = f.read()
         return value
 
     @staticmethod
     def log_info(msg):
         logger.info(str(msg))
 
@@ -476,15 +477,16 @@
             if self.res.status_code == 200 and self.res.rsp and isinstance(self.res.rsp, dict):
                 for key, value in self.res.rsp.items():
                     if isinstance(value, list):
                         return [i.get(name) for i in value]
                     elif isinstance(value, dict):
                         for key2, value2 in value.items():
                             if isinstance(value2, list):
-                                return [i.get(name) for i in value2 if i.get(name)]
+                                return [i.get(name) or i.get(name.lower()) or
+                                        i.get(name[0].lower()+name[1:]) for i in value2 if i.get(name)]
             return []
 
     @staticmethod
     def _to_excel(f, data, sheet_name="sheet", set_column=[], header_format=None, column_header=[],
                   column_default=[], isdigitl=True):
         if data and isinstance(data[0], (list, tuple)):
             h = data[0]
@@ -614,24 +616,30 @@
         with open("huhk/case_project/version.py", "w", encoding="utf-8") as f:
             f.write("version='%s'\n" % version)
         return version
 
     def set_value(self, value_dict):
         caller = inspect.getframeinfo(inspect.currentframe().f_back)
         for k, v in value_dict.items():
-            self.input_value[caller.function][k] = v
+            if k not in page_and_size:
+                self.input_value[caller.function][k] = v
 
     def set_output_value(self, key_list):
         if isinstance(key_list, dict):
-            key_list = [key_list.keys()]
+            key_list = list(key_list.keys())
         elif isinstance(key_list, str):
             key_list = [key_list]
         caller = inspect.getframeinfo(inspect.currentframe().f_back)
+        key_list = [n for n in key_list if n not in page_and_size and n != 'headers']
         for key in key_list:
-            self.output_list[caller.function][key] = self.get_res_value_list(key)
+            values = self.get_res_value_list(key)
+            self.output_list[caller.function][key] = values
+            if (not values) and re.findall(before_and_end_re_str, key):
+                key2 = re.sub(before_and_end_re_str, "", key)
+                self.output_list[caller.function][key] = self.get_res_value_list(key2)
 
     def get_value(self, name):
         name_list = name.split('.')
         if len(name_list) == 1:
             caller = inspect.getframeinfo(inspect.currentframe().f_back)
             return self.input_value[caller.function][name_list[-1]]
         elif len(name_list) > 1:
```

### Comparing `huhk-1.8.9/huhk/unit_logger.py` & `huhk-1.9.1/huhk/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/huhk/unit_request.py` & `huhk-1.9.1/huhk/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/huhk/unit_tasks.py` & `huhk-1.9.1/huhk/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/huhk/常用命令.py` & `huhk-1.9.1/huhk/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.9/service/app_t/app_t_fun.py` & `huhk-1.9.1/service/app_a/app_a_fun.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import requests
 
 from huhk.unit_fun import FunBase
+from huhk.unit_dict import Dict
 from huhk import admin_host
 
 
-class AppTFun(FunBase):
+class AppAFun(FunBase):
     def __init__(self):
         super().__init__()
         self.res = None
-
+        self.output_list = Dict()
+        self.input_value = Dict()
     @staticmethod
-    def run_mysql(sql_str, db_id=1):
+    def run_mysql( sql_str, db_id=1):
         # 根据后台数据库配置id查询
         out = requests.post(admin_host + "/sql/running_sql/", json={"id": db_id, "sql_str": sql_str}).json()
         if out.get("code") == "0000":
             return out.get("data")
         else:
             assert False, sql_str + str(out.get("msg"))
 
 
 if __name__ == '__main__':
-    f = AppTFun()
+    f = AppAFun()
     out = f.faker().name()
     print(out)
```

### Comparing `huhk-1.8.9/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py` & `huhk-1.9.1/service/app_a/asserts/open/haohan/asserts_open_haohan_rights.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import allure
 
-from service.app_t import unit_request
-from service.app_t.sqls.open.haohan.sqls_open_haohan_relation import SqlsOpenHaohanRelation
+from service.app_a import unit_request
+from service.app_a.sqls.open.haohan.sqls_open_haohan_rights import SqlsOpenHaohanRights
 
 
-class AssertsOpenHaohanRelation(SqlsOpenHaohanRelation):
+class AssertsOpenHaohanRights(SqlsOpenHaohanRights):
     @allure.step(title="接口返回结果校验")
-    def assert_open_haohan_relation_update(self, **kwargs):
-        assert unit_request.is_assert_true(self.res), "校验接口返回，缺少成功标识"
-        # out = self.sql_open_haohan_relation_update(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["userId"])
+    def assert_open_haohan_rights_update(self, _assert=True, **kwargs):
+        assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
+        # out = self.sql_open_haohan_rights_update(**kwargs)
+        # flag = self.compare_json_list(self.res, out, ["params"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.8.9/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py` & `huhk-1.9.1/service/app_a/asserts/asserts_content.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import allure
 
-from service.app_t import unit_request
-from service.app_t.sqls.open.haohan.sqls_open_haohan_rights import SqlsOpenHaohanRights
+from service.app_a import unit_request
+from service.app_a.sqls.sqls_content import SqlsContent
 
 
-class AssertsOpenHaohanRights(SqlsOpenHaohanRights):
+class AssertsContent(SqlsContent):
     @allure.step(title="接口返回结果校验")
-    def assert_open_haohan_rights_update(self, **kwargs):
-        assert unit_request.is_assert_true(self.res), "校验接口返回，缺少成功标识"
-        # out = self.sql_open_haohan_rights_update(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["params"])
+    def assert_content_adv_(self, _assert=True, **kwargs):
+        assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
+        # out = self.sql_content_adv_(**kwargs)
+        # flag = self.compare_json_list(self.res, out, ["advId"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.8.9/service/app_t/asserts/points/asserts_points_points.py` & `huhk-1.9.1/service/app_a/asserts/radarpoints/asserts_radarpoints_adjustpoints.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import allure
 
-from service.app_t import unit_request
-from service.app_t.sqls.points.sqls_points_points import SqlsPointsPoints
+from service.app_a import unit_request
+from service.app_a.sqls.radarpoints.sqls_radarpoints_adjustpoints import SqlsRadarpointsAdjustpoints
 
 
-class AssertsPointsPoints(SqlsPointsPoints):
+class AssertsRadarpointsAdjustpoints(SqlsRadarpointsAdjustpoints):
     @allure.step(title="接口返回结果校验")
-    def assert_points_points_flowDetail(self, _assert=True, **kwargs):
+    def assert_radarpoints_adjustpoints_pagelist(self, _assert=True, **kwargs):
         assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
-        # out = self.sql_points_points_flowDetail(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["userId"])
+        # out = self.sql_radarpoints_adjustpoints_pagelist(**kwargs)
+        # flag = self.compare_json_list(self.res, out, ["optAbility", "adjustTimeEnd", "mobile", "nickName", "userId", "optAbilityName", "adjustNotes", "adjustTimeBefore"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
-    def assert_points_points_page(self, **kwargs):
-        assert unit_request.is_assert_true(self.res), "校验接口返回，缺少成功标识"
-        # out = self.sql_points_points_page(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["endTime", "beforeTime"])
+    def assert_radarpoints_adjustpoints_getuserpointsqtybyuserid(self, _assert=True, **kwargs):
+        assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
+        # out = self.sql_radarpoints_adjustpoints_getuserpointsqtybyuserid(**kwargs)
+        # flag = self.compare_json_list(self.res, out, ["userId"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
-    def assert_points_points_download(self, **kwargs):
-        assert unit_request.is_assert_true(self.res), "校验接口返回，缺少成功标识"
-        # out = self.sql_points_points_download(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["endTime", "beforeTime"])
+    def assert_radarpoints_adjustpoints_getuserpointsqtybymobile(self, _assert=True, **kwargs):
+        assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
+        # out = self.sql_radarpoints_adjustpoints_getuserpointsqtybymobile(**kwargs)
+        # flag = self.compare_json_list(self.res, out, ["mobile"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
-    def assert_points_points_convertDetail(self, **kwargs):
-        assert unit_request.is_assert_true(self.res), "校验接口返回，缺少成功标识"
-        # out = self.sql_points_points_convertDetail(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["userId"])
+    def assert_radarpoints_adjustpoints_export(self, _assert=True, **kwargs):
+        assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
+        # out = self.sql_radarpoints_adjustpoints_export(**kwargs)
+        # flag = self.compare_json_list(self.res, out, ["optAbility", "adjustTimeEnd", "mobile", "nickName", "userId", "optAbilityName", "adjustNotes", "adjustTimeBefore"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.8.9/service/app_t/asserts/points/asserts_points_pointsApp.py` & `huhk-1.9.1/service/app_a/asserts/content/asserts_content_hotsearch.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import allure
 
-from service.app_t import unit_request
-from service.app_t.sqls.points.sqls_points_pointsApp import SqlsPointsPointsapp
+from service.app_a import unit_request
+from service.app_a.sqls.content.sqls_content_hotsearch import SqlsContentHotsearch
 
 
-class AssertsPointsPointsapp(SqlsPointsPointsapp):
+class AssertsContentHotsearch(SqlsContentHotsearch):
     @allure.step(title="接口返回结果校验")
-    def assert_points_pointsApp_signIn(self, **kwargs):
-        assert unit_request.is_assert_true(self.res), "校验接口返回，缺少成功标识"
-        # out = self.sql_points_pointsApp_signIn(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["userId"])
+    def assert_content_hotsearch_rank(self, _assert=True, **kwargs):
+        assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
+        # out = self.sql_content_hotsearch_rank(**kwargs)
+        # flag = self.compare_json_list(self.res, out, ["kId", "rank"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
-    def assert_points_pointsApp_myPoints(self, **kwargs):
-        assert unit_request.is_assert_true(self.res), "校验接口返回，缺少成功标识"
-        # out = self.sql_points_pointsApp_myPoints(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["userId"])
+    def assert_content_hotsearch_list(self, _assert=True, **kwargs):
+        assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
+        # out = self.sql_content_hotsearch_list(**kwargs)
+        # flag = self.compare_json_list(self.res, out, ["kId", "rank"])
         assert True, "数据比较不一致"
 
     @allure.step(title="接口返回结果校验")
-    def assert_points_pointsApp_myPointsTotal(self, **kwargs):
-        assert unit_request.is_assert_true(self.res), "校验接口返回，缺少成功标识"
-        # out = self.sql_points_pointsApp_myPointsTotal(**kwargs)
-        # flag = self.compare_json_list(self.res, out, ["userId"])
+    def assert_content_hotsearch_insert(self, _assert=True, **kwargs):
+        assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"
+        # out = self.sql_content_hotsearch_insert(**kwargs)
+        # flag = self.compare_json_list(self.res, out, ["keyWord", "point"])
         assert True, "数据比较不一致"
```

### Comparing `huhk-1.8.9/service/app_t/funs/open/haohan/funs_open_haohan_relation.py` & `huhk-1.9.1/service/app_a/funs/open/haohan/funs_open_haohan_relation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import allure
 
-from service.app_t.asserts.open.haohan.asserts_open_haohan_relation import AssertsOpenHaohanRelation
-from service.app_t.apis.open.haohan import apis_open_haohan_relation
+from service.app_a.asserts.open.haohan.asserts_open_haohan_relation import AssertsOpenHaohanRelation
+from service.app_a.apis.open.haohan import apis_open_haohan_relation
 
 
 class FunsOpenHaohanRelation(AssertsOpenHaohanRelation):
     @allure.step(title="浩瀚模块-关联关系-Y")
     def open_haohan_relation_update(self, userId="$None$", _assert=True,  **kwargs):
         """
             url=/open/haohan/relation/update
@@ -17,8 +17,7 @@
         self.res = apis_open_haohan_relation.open_haohan_relation_update(**_kwargs)
 
         self.assert_open_haohan_relation_update(_assert, **_kwargs)
         self.set_output_value(_kwargs)
         self.set_value(_kwargs)
 
 
-
```

### Comparing `huhk-1.8.9/service/app_t/funs/open/haohan/funs_open_haohan_rights.py` & `huhk-1.9.1/service/app_a/funs/open/haohan/funs_open_haohan_rights.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import allure
 
-from service.app_t.asserts.open.haohan.asserts_open_haohan_rights import AssertsOpenHaohanRights
-from service.app_t.apis.open.haohan import apis_open_haohan_rights
+from service.app_a.asserts.open.haohan.asserts_open_haohan_rights import AssertsOpenHaohanRights
+from service.app_a.apis.open.haohan import apis_open_haohan_rights
 
 
 class FunsOpenHaohanRights(AssertsOpenHaohanRights):
     @allure.step(title="浩瀚模块 - 更改充电桩权益状态-Y")
     def open_haohan_rights_update(self, params="$None$", _assert=True, _all_is_None=False,  **kwargs):
         """
             url=/open/haohan/rights/update
                 params: params : object :
                 data : string : 加密数据
                 params: headers : 请求头
         """
         params = self.get_value_choice(params, list_or_dict=None, key=None, _all_is_None=_all_is_None)
+
         _kwargs = self.get_kwargs(locals())
         self.res = apis_open_haohan_rights.open_haohan_rights_update(**_kwargs)
 
         self.assert_open_haohan_rights_update(_assert, **_kwargs)
         self.set_value(_kwargs)
 
 
-
```

### Comparing `huhk-1.8.9/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py` & `huhk-1.9.1/service/app_a/sqls/open/haohan/sqls_open_haohan_relation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from service.app_t.app_t_fun import AppTFun
+from service.app_a.app_a_fun import AppAFun
 
 
-class SqlsOpenHaohanRelation(AppTFun):
+class SqlsOpenHaohanRelation(AppAFun):
     def sql_open_haohan_relation_update(self, **kwargs):
         # name = self.kwargs_pop(kwargs, 'name')  # 单独处理字段
         # self.kwargs_replace(kwargs, likes=[], ins=[], before_end=[])  # 模糊查询字段，数组包含查询字段，区间字段处理
         # kwargs["order_by"] = None  # 排序
         sql_str = self.get_sql_str("table_name", **kwargs)  # 生成sql语句
         # out = self.run_mysql(sql_str)  # 执行sql语句
         # return out
```

### Comparing `huhk-1.8.9/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py` & `huhk-1.9.1/service/app_a/sqls/content/sqls_content_advplace.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from service.app_t.app_t_fun import AppTFun
+from service.app_a.app_a_fun import AppAFun
 
 
-class SqlsOpenHaohanRights(AppTFun):
-    def sql_open_haohan_rights_update(self, **kwargs):
+class SqlsContentAdvplace(AppAFun):
+    def sql_content_advplace_updatename(self, **kwargs):
         # name = self.kwargs_pop(kwargs, 'name')  # 单独处理字段
         # self.kwargs_replace(kwargs, likes=[], ins=[], before_end=[])  # 模糊查询字段，数组包含查询字段，区间字段处理
         # kwargs["order_by"] = None  # 排序
         sql_str = self.get_sql_str("table_name", **kwargs)  # 生成sql语句
         # out = self.run_mysql(sql_str)  # 执行sql语句
         # return out
```

### Comparing `huhk-1.8.9/service/app_t/sqls/points/sqls_points_points.py` & `huhk-1.9.1/service/app_a/sqls/order/sqls_order_order.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,28 @@
-from service.app_t.app_t_fun import AppTFun
+from service.app_a.app_a_fun import AppAFun
 
 
-class SqlsPointsPoints(AppTFun):
-    def sql_points_points_flowDetail(self, **kwargs):
+class SqlsOrderOrder(AppAFun):
+    def sql_order_order_orderdetail(self, **kwargs):
         # name = self.kwargs_pop(kwargs, 'name')  # 单独处理字段
         # self.kwargs_replace(kwargs, likes=[], ins=[], before_end=[])  # 模糊查询字段，数组包含查询字段，区间字段处理
         # kwargs["order_by"] = None  # 排序
         sql_str = self.get_sql_str("table_name", **kwargs)  # 生成sql语句
         # out = self.run_mysql(sql_str)  # 执行sql语句
         # return out
 
-    def sql_points_points_page(self, **kwargs):
+    def sql_order_order_finish(self, **kwargs):
         # name = self.kwargs_pop(kwargs, 'name')  # 单独处理字段
         # self.kwargs_replace(kwargs, likes=[], ins=[], before_end=[])  # 模糊查询字段，数组包含查询字段，区间字段处理
         # kwargs["order_by"] = None  # 排序
         sql_str = self.get_sql_str("table_name", **kwargs)  # 生成sql语句
         # out = self.run_mysql(sql_str)  # 执行sql语句
         # return out
 
-    def sql_points_points_download(self, **kwargs):
-        # name = self.kwargs_pop(kwargs, 'name')  # 单独处理字段
-        # self.kwargs_replace(kwargs, likes=[], ins=[], before_end=[])  # 模糊查询字段，数组包含查询字段，区间字段处理
-        # kwargs["order_by"] = None  # 排序
-        sql_str = self.get_sql_str("table_name", **kwargs)  # 生成sql语句
-        # out = self.run_mysql(sql_str)  # 执行sql语句
-        # return out
-
-    def sql_points_points_convertDetail(self, **kwargs):
+    def sql_order_order_refundreject(self, **kwargs):
         # name = self.kwargs_pop(kwargs, 'name')  # 单独处理字段
         # self.kwargs_replace(kwargs, likes=[], ins=[], before_end=[])  # 模糊查询字段，数组包含查询字段，区间字段处理
         # kwargs["order_by"] = None  # 排序
         sql_str = self.get_sql_str("table_name", **kwargs)  # 生成sql语句
         # out = self.run_mysql(sql_str)  # 执行sql语句
         # return out
```

### Comparing `huhk-1.8.9/service/app_t/sqls/points/sqls_points_pointsApp.py` & `huhk-1.9.1/service/app_a/sqls/content/sqls_content_essayweb.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,36 @@
-from service.app_t.app_t_fun import AppTFun
+from service.app_a.app_a_fun import AppAFun
 
 
-class SqlsPointsPointsapp(AppTFun):
-    def sql_points_pointsApp_signIn(self, **kwargs):
+class SqlsContentEssayweb(AppAFun):
+    def sql_content_essayweb_add(self, **kwargs):
         # name = self.kwargs_pop(kwargs, 'name')  # 单独处理字段
         # self.kwargs_replace(kwargs, likes=[], ins=[], before_end=[])  # 模糊查询字段，数组包含查询字段，区间字段处理
         # kwargs["order_by"] = None  # 排序
         sql_str = self.get_sql_str("table_name", **kwargs)  # 生成sql语句
         # out = self.run_mysql(sql_str)  # 执行sql语句
         # return out
 
-    def sql_points_pointsApp_myPoints(self, **kwargs):
+    def sql_content_essayweb_searchbykey(self, **kwargs):
         # name = self.kwargs_pop(kwargs, 'name')  # 单独处理字段
         # self.kwargs_replace(kwargs, likes=[], ins=[], before_end=[])  # 模糊查询字段，数组包含查询字段，区间字段处理
         # kwargs["order_by"] = None  # 排序
         sql_str = self.get_sql_str("table_name", **kwargs)  # 生成sql语句
         # out = self.run_mysql(sql_str)  # 执行sql语句
         # return out
 
-    def sql_points_pointsApp_myPointsTotal(self, **kwargs):
+    def sql_content_essayweb_delete_(self, **kwargs):
+        # name = self.kwargs_pop(kwargs, 'name')  # 单独处理字段
+        # self.kwargs_replace(kwargs, likes=[], ins=[], before_end=[])  # 模糊查询字段，数组包含查询字段，区间字段处理
+        # kwargs["order_by"] = None  # 排序
+        sql_str = self.get_sql_str("table_name", **kwargs)  # 生成sql语句
+        # out = self.run_mysql(sql_str)  # 执行sql语句
+        # return out
+
+    def sql_content_essayweb_getbyid(self, **kwargs):
         # name = self.kwargs_pop(kwargs, 'name')  # 单独处理字段
         # self.kwargs_replace(kwargs, likes=[], ins=[], before_end=[])  # 模糊查询字段，数组包含查询字段，区间字段处理
         # kwargs["order_by"] = None  # 排序
         sql_str = self.get_sql_str("table_name", **kwargs)  # 生成sql语句
         # out = self.run_mysql(sql_str)  # 执行sql语句
         # return out
```

