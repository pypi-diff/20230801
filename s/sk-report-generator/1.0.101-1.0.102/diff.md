# Comparing `tmp/sk_report_generator-1.0.101.tar.gz` & `tmp/sk_report_generator-1.0.102.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sk_report_generator-1.0.101.tar", last modified: Fri Jul 28 16:22:03 2023, max compression
+gzip compressed data, was "sk_report_generator-1.0.102.tar", last modified: Tue Aug  1 17:19:52 2023, max compression
```

## Comparing `sk_report_generator-1.0.101.tar` & `sk_report_generator-1.0.102.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 16:22:03.958986 sk_report_generator-1.0.101/
--rw-rw-rw-   0        0        0     1055 2023-07-18 15:19:22.000000 sk_report_generator-1.0.101/LICENSE.txt
--rw-rw-rw-   0        0        0     7599 2023-07-28 16:22:03.957986 sk_report_generator-1.0.101/PKG-INFO
--rw-rw-rw-   0        0        0     7117 2023-07-18 15:19:22.000000 sk_report_generator-1.0.101/README.md
--rw-rw-rw-   0        0        0       42 2023-07-28 16:22:03.958986 sk_report_generator-1.0.101/setup.cfg
--rw-rw-rw-   0        0        0      807 2023-07-28 16:21:43.000000 sk_report_generator-1.0.101/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 16:22:03.841003 sk_report_generator-1.0.101/sk_report_generator/
--rw-rw-rw-   0        0        0     1377 2023-07-21 09:56:32.000000 sk_report_generator-1.0.101/sk_report_generator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 16:22:03.863048 sk_report_generator-1.0.101/sk_report_generator/reporter/
--rw-rw-rw-   0        0        0        0 2023-07-18 15:15:10.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/__init__.py
--rw-rw-rw-   0        0        0      847 2023-07-18 15:15:10.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/base.py
--rw-rw-rw-   0        0        0      482 2023-07-18 15:15:10.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/default.py
--rw-rw-rw-   0        0        0     1268 2023-07-23 10:12:14.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/format.py
-drwxrwxrwx   0        0        0        0 2023-07-28 16:22:03.868159 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/
--rw-rw-rw-   0        0        0        0 2023-07-18 15:15:10.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/__init__.py
--rw-rw-rw-   0        0        0      624 2023-07-24 05:03:27.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/base.py
--rw-rw-rw-   0        0        0     3881 2023-07-28 14:25:35.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format.py
-drwxrwxrwx   0        0        0        0 2023-07-28 16:22:03.884387 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format_functions/
--rw-rw-rw-   0        0        0        0 2023-07-18 15:19:22.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format_functions/__init__.py
--rw-rw-rw-   0        0        0      522 2023-07-23 05:26:22.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format_functions/bool.py
--rw-rw-rw-   0        0        0     1675 2023-07-18 16:53:16.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format_functions/ceil.py
--rw-rw-rw-   0        0        0     2540 2023-07-18 16:52:42.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format_functions/currency.py
--rw-rw-rw-   0        0        0     3003 2023-07-23 14:36:22.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format_functions/datetime.py
--rw-rw-rw-   0        0        0      291 2023-07-23 10:08:44.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format_functions/default.py
--rw-rw-rw-   0        0        0     1655 2023-07-23 15:19:07.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format_functions/floor.py
--rw-rw-rw-   0        0        0     1159 2023-07-23 17:25:05.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format_functions/mask.py
--rw-rw-rw-   0        0        0      474 2023-07-18 16:55:02.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format_functions/round.py
--rw-rw-rw-   0        0        0      652 2023-07-18 16:53:26.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format_functions/str_continue.py
--rw-rw-rw-   0        0        0      742 2023-07-23 16:14:34.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format_functions/trunc.py
--rw-rw-rw-   0        0        0      547 2023-07-26 03:11:57.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/default_format_evaluate.py
--rw-rw-rw-   0        0        0      151 2023-07-23 09:57:19.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/format_default.py
--rw-rw-rw-   0        0        0      822 2023-07-23 10:05:42.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/format_evaluate.py
-drwxrwxrwx   0        0        0        0 2023-07-28 16:22:03.896031 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/json_to_format_spec/
--rw-rw-rw-   0        0        0        0 2023-07-18 15:19:22.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/json_to_format_spec/__init__.py
--rw-rw-rw-   0        0        0      806 2023-07-24 05:03:44.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/json_to_format_spec/align.py
--rw-rw-rw-   0        0        0      304 2023-07-24 05:12:11.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/json_to_format_spec/dufault.py
--rw-rw-rw-   0        0        0      594 2023-07-24 05:06:15.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/json_to_format_spec/fill.py
--rw-rw-rw-   0        0        0      605 2023-07-24 05:05:29.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/json_to_format_spec/grouping_option.py
--rw-rw-rw-   0        0        0      536 2023-07-24 05:05:36.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/json_to_format_spec/pad.py
--rw-rw-rw-   0        0        0      620 2023-07-24 05:05:44.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/json_to_format_spec/precision.py
--rw-rw-rw-   0        0        0      590 2023-07-24 05:05:50.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/json_to_format_spec/sign.py
--rw-rw-rw-   0        0        0      592 2023-07-24 05:05:57.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/json_to_format_spec/type.py
--rw-rw-rw-   0        0        0      599 2023-07-24 05:04:08.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/json_to_format_spec/width.py
-drwxrwxrwx   0        0        0        0 2023-07-28 16:22:03.910734 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/process/
--rw-rw-rw-   0        0        0        0 2023-07-18 15:19:22.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/process/__init__.py
--rw-rw-rw-   0        0        0      361 2023-07-24 07:08:50.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/process/evaluate_default_format.py
--rw-rw-rw-   0        0        0      171 2023-07-18 15:19:22.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/process/format_tag_remove.py
--rw-rw-rw-   0        0        0      405 2023-07-24 06:42:02.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/process/get_condition.py
--rw-rw-rw-   0        0        0      620 2023-07-28 14:23:12.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/process/get_format_specs.py
--rw-rw-rw-   0        0        0      754 2023-07-24 07:34:26.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/process/template_format_process.py
--rw-rw-rw-   0        0        0      572 2023-07-18 15:19:22.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/process/template_to_format_list.py
--rw-rw-rw-   0        0        0     1707 2023-07-26 03:11:57.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function.py
-drwxrwxrwx   0        0        0        0 2023-07-28 16:22:03.917549 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/
--rw-rw-rw-   0        0        0        0 2023-07-26 03:11:57.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 16:22:03.947712 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/
--rw-rw-rw-   0        0        0        0 2023-07-26 04:49:19.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/__init__.py
--rw-rw-rw-   0        0        0      638 2023-07-18 15:19:22.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/avg.py
--rw-rw-rw-   0        0        0     1073 2023-07-26 09:50:25.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/camel.py
--rw-rw-rw-   0        0        0     1008 2023-07-26 09:49:53.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/capitalize.py
--rw-rw-rw-   0        0        0     1126 2023-07-26 13:09:45.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/ceil.py
--rw-rw-rw-   0        0        0     1172 2023-07-26 12:48:30.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/count.py
--rw-rw-rw-   0        0        0      191 2023-07-18 15:19:22.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/default.py
--rw-rw-rw-   0        0        0      600 2023-07-26 12:49:19.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/distinct.py
--rw-rw-rw-   0        0        0      756 2023-07-26 12:47:41.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/filter.py
--rw-rw-rw-   0        0        0     1129 2023-07-26 12:55:44.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/floor.py
--rw-rw-rw-   0        0        0     1315 2023-07-27 09:21:49.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/foreach.py
--rw-rw-rw-   0        0        0      572 2023-07-26 12:49:52.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/len.py
--rw-rw-rw-   0        0        0      594 2023-07-26 11:08:46.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/lower.py
--rw-rw-rw-   0        0        0      577 2023-07-26 12:49:56.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/max.py
--rw-rw-rw-   0        0        0      579 2023-07-26 12:50:01.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/min.py
-drwxrwxrwx   0        0        0        0 2023-07-28 16:22:03.949860 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/modules/
--rw-rw-rw-   0        0        0        0 2023-07-26 04:49:19.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/modules/__init__.py
--rw-rw-rw-   0        0        0      385 2023-07-26 09:38:14.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/modules/check_condition.py
--rw-rw-rw-   0        0        0      526 2023-07-26 09:44:03.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/modules/get_arg.py
--rw-rw-rw-   0        0        0     2427 2023-07-26 14:03:47.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/range.py
--rw-rw-rw-   0        0        0     1177 2023-07-26 12:50:10.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/reverse.py
--rw-rw-rw-   0        0        0      737 2023-07-26 12:50:15.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/round.py
--rw-rw-rw-   0        0        0      714 2023-07-26 12:50:19.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/set.py
--rw-rw-rw-   0        0        0      554 2023-07-26 12:50:24.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/slice.py
--rw-rw-rw-   0        0        0      623 2023-07-26 12:34:31.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/snake.py
--rw-rw-rw-   0        0        0      566 2023-07-26 12:50:33.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/sum.py
--rw-rw-rw-   0        0        0      594 2023-07-26 12:45:41.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/upper_case.py
--rw-rw-rw-   0        0        0     1232 2023-07-27 08:34:29.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function_solver.py
--rw-rw-rw-   0        0        0      834 2023-07-27 08:26:47.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/get_index_value.py
--rw-rw-rw-   0        0        0      211 2023-07-26 03:11:57.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/get_obj_value.py
--rw-rw-rw-   0        0        0      207 2023-07-26 03:11:57.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/process_condition.py
--rw-rw-rw-   0        0        0      325 2023-07-28 08:04:20.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/process_function_calling.py
--rw-rw-rw-   0        0        0     3518 2023-07-27 09:26:11.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/single_function_solver.py
--rw-rw-rw-   0        0        0      979 2023-07-18 15:19:22.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/operation.py
--rw-rw-rw-   0        0        0     1311 2023-07-27 10:14:34.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/script.py
-drwxrwxrwx   0        0        0        0 2023-07-28 16:22:03.954876 sk_report_generator-1.0.101/sk_report_generator/reporter/script_evaluate/
--rw-rw-rw-   0        0        0        0 2023-07-18 15:15:10.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/script_evaluate/__init__.py
--rw-rw-rw-   0        0        0     1352 2023-07-27 10:13:16.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/script_evaluate/script_process.py
--rw-rw-rw-   0        0        0      291 2023-07-18 15:19:22.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/script_evaluate/script_replacer.py
--rw-rw-rw-   0        0        0      635 2023-07-21 05:02:00.000000 sk_report_generator-1.0.101/sk_report_generator/reporter/script_evaluate/script_runner.py
-drwxrwxrwx   0        0        0        0 2023-07-28 16:22:03.850023 sk_report_generator-1.0.101/sk_report_generator.egg-info/
--rw-rw-rw-   0        0        0     7599 2023-07-28 16:22:03.000000 sk_report_generator-1.0.101/sk_report_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5261 2023-07-28 16:22:03.000000 sk_report_generator-1.0.101/sk_report_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 16:22:03.000000 sk_report_generator-1.0.101/sk_report_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-28 16:22:03.000000 sk_report_generator-1.0.101/sk_report_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-28 16:22:03.000000 sk_report_generator-1.0.101/sk_report_generator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 17:19:52.608120 sk_report_generator-1.0.102/
+-rw-rw-rw-   0        0        0     1055 2023-07-18 15:19:22.000000 sk_report_generator-1.0.102/LICENSE.txt
+-rw-rw-rw-   0        0        0     7599 2023-08-01 17:19:52.608120 sk_report_generator-1.0.102/PKG-INFO
+-rw-rw-rw-   0        0        0     7117 2023-07-18 15:19:22.000000 sk_report_generator-1.0.102/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 17:19:52.608120 sk_report_generator-1.0.102/setup.cfg
+-rw-rw-rw-   0        0        0      807 2023-08-01 17:19:36.000000 sk_report_generator-1.0.102/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:19:52.114024 sk_report_generator-1.0.102/sk_report_generator/
+-rw-rw-rw-   0        0        0     1377 2023-07-21 09:56:32.000000 sk_report_generator-1.0.102/sk_report_generator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:19:52.179371 sk_report_generator-1.0.102/sk_report_generator/reporter/
+-rw-rw-rw-   0        0        0        0 2023-07-18 15:15:10.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/__init__.py
+-rw-rw-rw-   0        0        0      847 2023-07-18 15:15:10.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/base.py
+-rw-rw-rw-   0        0        0      482 2023-07-18 15:15:10.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/default.py
+-rw-rw-rw-   0        0        0     1268 2023-07-23 10:12:14.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/format.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:19:52.212864 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/
+-rw-rw-rw-   0        0        0        0 2023-07-18 15:15:10.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/__init__.py
+-rw-rw-rw-   0        0        0      624 2023-07-24 05:03:27.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/base.py
+-rw-rw-rw-   0        0        0     3881 2023-07-28 14:25:35.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:19:52.281236 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format_functions/
+-rw-rw-rw-   0        0        0        0 2023-07-18 15:19:22.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format_functions/__init__.py
+-rw-rw-rw-   0        0        0      522 2023-07-23 05:26:22.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format_functions/bool.py
+-rw-rw-rw-   0        0        0     1675 2023-07-18 16:53:16.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format_functions/ceil.py
+-rw-rw-rw-   0        0        0     2540 2023-07-18 16:52:42.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format_functions/currency.py
+-rw-rw-rw-   0        0        0     3003 2023-07-23 14:36:22.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format_functions/datetime.py
+-rw-rw-rw-   0        0        0      291 2023-07-23 10:08:44.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format_functions/default.py
+-rw-rw-rw-   0        0        0     1655 2023-07-23 15:19:07.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format_functions/floor.py
+-rw-rw-rw-   0        0        0     1159 2023-07-23 17:25:05.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format_functions/mask.py
+-rw-rw-rw-   0        0        0      474 2023-07-18 16:55:02.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format_functions/round.py
+-rw-rw-rw-   0        0        0      652 2023-07-18 16:53:26.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format_functions/str_continue.py
+-rw-rw-rw-   0        0        0      742 2023-07-23 16:14:34.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format_functions/trunc.py
+-rw-rw-rw-   0        0        0      556 2023-07-31 01:32:23.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/default_format_evaluate.py
+-rw-rw-rw-   0        0        0      151 2023-07-23 09:57:19.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/format_default.py
+-rw-rw-rw-   0        0        0      822 2023-07-23 10:05:42.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/format_evaluate.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:19:52.339739 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/json_to_format_spec/
+-rw-rw-rw-   0        0        0        0 2023-07-18 15:19:22.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/json_to_format_spec/__init__.py
+-rw-rw-rw-   0        0        0      806 2023-07-24 05:03:44.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/json_to_format_spec/align.py
+-rw-rw-rw-   0        0        0      304 2023-07-24 05:12:11.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/json_to_format_spec/dufault.py
+-rw-rw-rw-   0        0        0      594 2023-07-24 05:06:15.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/json_to_format_spec/fill.py
+-rw-rw-rw-   0        0        0      605 2023-07-24 05:05:29.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/json_to_format_spec/grouping_option.py
+-rw-rw-rw-   0        0        0      536 2023-07-24 05:05:36.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/json_to_format_spec/pad.py
+-rw-rw-rw-   0        0        0      620 2023-07-24 05:05:44.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/json_to_format_spec/precision.py
+-rw-rw-rw-   0        0        0      590 2023-07-24 05:05:50.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/json_to_format_spec/sign.py
+-rw-rw-rw-   0        0        0      592 2023-07-24 05:05:57.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/json_to_format_spec/type.py
+-rw-rw-rw-   0        0        0      599 2023-07-24 05:04:08.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/json_to_format_spec/width.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:19:52.381343 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/process/
+-rw-rw-rw-   0        0        0        0 2023-07-18 15:19:22.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/process/__init__.py
+-rw-rw-rw-   0        0        0      452 2023-07-31 03:14:55.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/process/evaluate_default_format.py
+-rw-rw-rw-   0        0        0      171 2023-07-18 15:19:22.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/process/format_tag_remove.py
+-rw-rw-rw-   0        0        0      494 2023-07-31 01:39:27.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/process/get_condition.py
+-rw-rw-rw-   0        0        0      620 2023-07-28 14:23:12.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/process/get_format_specs.py
+-rw-rw-rw-   0        0        0      754 2023-07-24 07:34:26.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/process/template_format_process.py
+-rw-rw-rw-   0        0        0      572 2023-07-18 15:19:22.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/process/template_to_format_list.py
+-rw-rw-rw-   0        0        0     1707 2023-07-26 03:11:57.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:19:52.423508 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/
+-rw-rw-rw-   0        0        0        0 2023-07-26 03:11:57.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:19:52.571252 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/
+-rw-rw-rw-   0        0        0        0 2023-07-26 04:49:19.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/__init__.py
+-rw-rw-rw-   0        0        0      638 2023-07-18 15:19:22.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/avg.py
+-rw-rw-rw-   0        0        0     1073 2023-07-26 09:50:25.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/camel.py
+-rw-rw-rw-   0        0        0     1008 2023-07-26 09:49:53.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/capitalize.py
+-rw-rw-rw-   0        0        0     1126 2023-07-26 13:09:45.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/ceil.py
+-rw-rw-rw-   0        0        0     1172 2023-07-26 12:48:30.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/count.py
+-rw-rw-rw-   0        0        0      191 2023-07-18 15:19:22.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/default.py
+-rw-rw-rw-   0        0        0      600 2023-07-26 12:49:19.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/distinct.py
+-rw-rw-rw-   0        0        0      756 2023-07-26 12:47:41.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/filter.py
+-rw-rw-rw-   0        0        0     1129 2023-07-26 12:55:44.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/floor.py
+-rw-rw-rw-   0        0        0     1315 2023-07-27 09:21:49.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/foreach.py
+-rw-rw-rw-   0        0        0      572 2023-07-26 12:49:52.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/len.py
+-rw-rw-rw-   0        0        0      594 2023-07-26 11:08:46.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/lower.py
+-rw-rw-rw-   0        0        0      577 2023-07-26 12:49:56.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/max.py
+-rw-rw-rw-   0        0        0      579 2023-07-26 12:50:01.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/min.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:19:52.585839 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/modules/
+-rw-rw-rw-   0        0        0        0 2023-07-26 04:49:19.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/modules/__init__.py
+-rw-rw-rw-   0        0        0      385 2023-07-26 09:38:14.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/modules/check_condition.py
+-rw-rw-rw-   0        0        0      526 2023-07-26 09:44:03.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/modules/get_arg.py
+-rw-rw-rw-   0        0        0     2427 2023-07-26 14:03:47.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/range.py
+-rw-rw-rw-   0        0        0     1177 2023-07-26 12:50:10.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/reverse.py
+-rw-rw-rw-   0        0        0      737 2023-07-26 12:50:15.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/round.py
+-rw-rw-rw-   0        0        0      714 2023-07-26 12:50:19.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/set.py
+-rw-rw-rw-   0        0        0      554 2023-07-26 12:50:24.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/slice.py
+-rw-rw-rw-   0        0        0      623 2023-07-26 12:34:31.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/snake.py
+-rw-rw-rw-   0        0        0      566 2023-07-26 12:50:33.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/sum.py
+-rw-rw-rw-   0        0        0      594 2023-07-26 12:45:41.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/upper_case.py
+-rw-rw-rw-   0        0        0     1232 2023-07-31 01:08:10.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function_solver.py
+-rw-rw-rw-   0        0        0      834 2023-07-27 08:26:47.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/get_index_value.py
+-rw-rw-rw-   0        0        0      211 2023-07-26 03:11:57.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/get_obj_value.py
+-rw-rw-rw-   0        0        0      207 2023-07-26 03:11:57.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/process_condition.py
+-rw-rw-rw-   0        0        0      325 2023-07-28 08:04:20.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/process_function_calling.py
+-rw-rw-rw-   0        0        0     3518 2023-07-27 09:26:11.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/single_function_solver.py
+-rw-rw-rw-   0        0        0      979 2023-07-18 15:19:22.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/operation.py
+-rw-rw-rw-   0        0        0     1311 2023-07-27 10:14:34.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/script.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:19:52.607119 sk_report_generator-1.0.102/sk_report_generator/reporter/script_evaluate/
+-rw-rw-rw-   0        0        0        0 2023-07-18 15:15:10.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/script_evaluate/__init__.py
+-rw-rw-rw-   0        0        0     1352 2023-07-27 10:13:16.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/script_evaluate/script_process.py
+-rw-rw-rw-   0        0        0      291 2023-07-18 15:19:22.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/script_evaluate/script_replacer.py
+-rw-rw-rw-   0        0        0      635 2023-07-21 05:02:00.000000 sk_report_generator-1.0.102/sk_report_generator/reporter/script_evaluate/script_runner.py
+drwxrwxrwx   0        0        0        0 2023-08-01 17:19:52.136340 sk_report_generator-1.0.102/sk_report_generator.egg-info/
+-rw-rw-rw-   0        0        0     7599 2023-08-01 17:19:52.000000 sk_report_generator-1.0.102/sk_report_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5261 2023-08-01 17:19:52.000000 sk_report_generator-1.0.102/sk_report_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 17:19:52.000000 sk_report_generator-1.0.102/sk_report_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-01 17:19:52.000000 sk_report_generator-1.0.102/sk_report_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-08-01 17:19:52.000000 sk_report_generator-1.0.102/sk_report_generator.egg-info/top_level.txt
```

### Comparing `sk_report_generator-1.0.101/LICENSE.txt` & `sk_report_generator-1.0.102/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/PKG-INFO` & `sk_report_generator-1.0.102/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sk_report_generator
-Version: 1.0.101
+Version: 1.0.102
 Summary: A simple Reporting program
 Author: gkibria
 Author-email: gkibria121@gmail.com
 Keywords: python,calculator,python calculator,gk calculator,advanced calculator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sk_report_generator-1.0.101/README.md` & `sk_report_generator-1.0.102/README.md`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/setup.py` & `sk_report_generator-1.0.102/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sk_report_generator',
-    version='1.0.101',
+    version='1.0.102',
     description='A simple Reporting program',
     author='gkibria',
     long_description=long_description,
     long_description_content_type="text/markdown",  # Specify the content type as Markdown
     author_email='gkibria121@gmail.com',
     packages=find_packages(),
     install_requires=['regex'],
```

### Comparing `sk_report_generator-1.0.101/sk_report_generator/__init__.py` & `sk_report_generator-1.0.102/sk_report_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/base.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/base.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/format.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/format.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/base.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/base.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format_functions/bool.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format_functions/bool.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format_functions/ceil.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format_functions/ceil.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format_functions/currency.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format_functions/currency.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format_functions/datetime.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format_functions/datetime.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format_functions/floor.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format_functions/floor.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format_functions/mask.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format_functions/mask.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format_functions/str_continue.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format_functions/str_continue.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/custom_format_functions/trunc.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/custom_format_functions/trunc.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/default_format_evaluate.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/default_format_evaluate.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 class DefaultFormat:
 
     def run(self,value,format_spec,format_class_list):
         if len(format_class_list) ==0:
             value = str(value)
             digit = re.sub(r'[,.e\+\-]','',value).isdigit()
             if digit:
-                f_value = value
+                f_value = eval(value)
             else:
                 f_value = f'"{value}"'
 
-            value =eval("format(f_value,format_spec)")
+            value =eval(f"format({f_value},format_spec)")
 
         return self.go_next.run(value,format_spec,format_class_list)
 
     def set_next(self,go_next):
 
         self.go_next = go_next
```

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/format_evaluate.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/format_evaluate.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/json_to_format_spec/align.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/json_to_format_spec/align.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/json_to_format_spec/fill.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/json_to_format_spec/fill.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/json_to_format_spec/grouping_option.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/json_to_format_spec/grouping_option.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/json_to_format_spec/pad.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/json_to_format_spec/pad.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/json_to_format_spec/precision.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/json_to_format_spec/precision.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/json_to_format_spec/sign.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/json_to_format_spec/sign.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/json_to_format_spec/type.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/json_to_format_spec/type.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/json_to_format_spec/width.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/json_to_format_spec/width.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/process/get_format_specs.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/process/get_format_specs.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/process/template_format_process.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/process/template_format_process.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/formatter/process/template_to_format_list.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/formatter/process/template_to_format_list.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/avg.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/avg.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/camel.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/camel.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/capitalize.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/capitalize.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/ceil.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/ceil.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/count.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/count.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/distinct.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/distinct.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/filter.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/filter.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/floor.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/floor.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/foreach.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/foreach.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/len.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/len.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/lower.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/lower.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/max.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/max.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/min.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/min.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/modules/get_arg.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/modules/get_arg.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/range.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/range.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/reverse.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/reverse.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/round.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/round.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/set.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/set.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/slice.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/slice.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/snake.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/snake.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/sum.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/sum.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function/upper_case.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function/upper_case.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/function_solver.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/function_solver.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         function_calling = self.process_function_calling.run(function_calling)
         single_object_pattern = r'((\$\w+)((?:\.\w+(\(((?:[^()])|(?4))*\)))|(?:(?:\[\W?\w+\W?\])+))*)'
         single_boject_list = re.findall(single_object_pattern, function_calling)
 
         for single_object in single_boject_list:
 
-            reslut = self.single_obj_solver.run(single_object[1],single_object[2])
+            reslut = self.single_obj_solver.run(single_object[1],single_object[0])
 
             function_calling = re.sub(re.escape(single_object[0]) + r'(?=\s|\b|$)', str(reslut), function_calling)
 
         result = function_calling
         return result
 
     def set_data(self, data):
```

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/get_index_value.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/get_index_value.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/function_solver/single_function_solver.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/function_solver/single_function_solver.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/operation.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/operation.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/script.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/script.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/script_evaluate/script_process.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/script_evaluate/script_process.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator/reporter/script_evaluate/script_runner.py` & `sk_report_generator-1.0.102/sk_report_generator/reporter/script_evaluate/script_runner.py`

 * *Files identical despite different names*

### Comparing `sk_report_generator-1.0.101/sk_report_generator.egg-info/PKG-INFO` & `sk_report_generator-1.0.102/sk_report_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sk-report-generator
-Version: 1.0.101
+Version: 1.0.102
 Summary: A simple Reporting program
 Author: gkibria
 Author-email: gkibria121@gmail.com
 Keywords: python,calculator,python calculator,gk calculator,advanced calculator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sk_report_generator-1.0.101/sk_report_generator.egg-info/SOURCES.txt` & `sk_report_generator-1.0.102/sk_report_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

