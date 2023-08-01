# Comparing `tmp/huhk-1.9.2.tar.gz` & `tmp/huhk-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhk-1.9.2.tar", last modified: Tue Aug  1 01:48:15 2023, max compression
+gzip compressed data, was "huhk-1.9.3.tar", last modified: Tue Aug  1 01:54:01 2023, max compression
```

## Comparing `huhk-1.9.2.tar` & `huhk-1.9.3.tar`

### file list

```diff
@@ -1,50 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 01:48:15.396827 huhk-1.9.2/
--rw-rw-rw-   0        0        0      223 2023-08-01 01:48:15.395812 huhk-1.9.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 01:48:15.324786 huhk-1.9.2/huhk/
--rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.9.2/huhk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:48:15.355665 huhk-1.9.2/huhk/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.2/huhk/case_project/__init__.py
--rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.9.2/huhk/case_project/json_coder.py
--rw-rw-rw-   0        0        0     3258 2023-07-26 08:25:43.000000 huhk-1.9.2/huhk/case_project/main_fun.py
--rw-rw-rw-   0        0        0    21531 2023-07-31 07:13:40.000000 huhk-1.9.2/huhk/case_project/project_base.py
--rw-rw-rw-   0        0        0     1337 2023-08-01 01:47:29.000000 huhk-1.9.2/huhk/case_project/project_init.py
--rw-rw-rw-   0        0        0    18567 2023-07-31 08:18:51.000000 huhk-1.9.2/huhk/case_project/project_string.py
--rw-rw-rw-   0        0        0      895 2023-07-26 08:22:28.000000 huhk-1.9.2/huhk/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-08-01 01:48:13.000000 huhk-1.9.2/huhk/case_project/version.py
--rw-rw-rw-   0        0        0     9925 2023-07-31 05:34:49.000000 huhk-1.9.2/huhk/init_project.py
--rw-rw-rw-   0        0        0     1267 2023-07-25 09:00:59.000000 huhk-1.9.2/huhk/main.py
--rw-rw-rw-   0        0        0      338 2023-08-01 01:48:08.000000 huhk-1.9.2/huhk/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:48:15.356664 huhk-1.9.2/huhk/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.2/huhk/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:48:15.392820 huhk-1.9.2/huhk/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.2/huhk/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.9.2/huhk/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.9.2/huhk/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.9.2/huhk/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.9.2/huhk/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.9.2/huhk/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.9.2/huhk/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.9.2/huhk/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.9.2/huhk/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.9.2/huhk/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.9.2/huhk/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.9.2/huhk/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.9.2/huhk/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.9.2/huhk/unit_apache_beam.py
--rw-rw-rw-   0        0        0      352 2023-07-31 09:35:09.000000 huhk-1.9.2/huhk/unit_data.py
--rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.9.2/huhk/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.9.2/huhk/unit_encryption.py
--rw-rw-rw-   0        0        0    28964 2023-08-01 01:47:59.000000 huhk-1.9.2/huhk/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.9.2/huhk/unit_logger.py
--rw-rw-rw-   0        0        0     9960 2023-07-22 07:06:52.000000 huhk-1.9.2/huhk/unit_request.py
--rw-rw-rw-   0        0        0     2511 2023-07-24 06:56:32.000000 huhk-1.9.2/huhk/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.9.2/huhk/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:48:15.336715 huhk-1.9.2/huhk.egg-info/
--rw-rw-rw-   0        0        0      223 2023-08-01 01:48:14.000000 huhk-1.9.2/huhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1165 2023-08-01 01:48:14.000000 huhk-1.9.2/huhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 01:48:14.000000 huhk-1.9.2/huhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-08-01 01:48:14.000000 huhk-1.9.2/huhk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-08-01 01:48:14.000000 huhk-1.9.2/huhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-08-01 01:48:14.000000 huhk-1.9.2/huhk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 01:48:15.396827 huhk-1.9.2/setup.cfg
--rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:54:01.012658 huhk-1.9.3/
+-rw-rw-rw-   0        0        0      223 2023-08-01 01:54:01.011661 huhk-1.9.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 01:54:00.893448 huhk-1.9.3/huhk/
+-rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.9.3/huhk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:54:00.932310 huhk-1.9.3/huhk/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.3/huhk/case_project/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.9.3/huhk/case_project/json_coder.py
+-rw-rw-rw-   0        0        0     3258 2023-07-26 08:25:43.000000 huhk-1.9.3/huhk/case_project/main_fun.py
+-rw-rw-rw-   0        0        0    21531 2023-07-31 07:13:40.000000 huhk-1.9.3/huhk/case_project/project_base.py
+-rw-rw-rw-   0        0        0     1337 2023-08-01 01:47:29.000000 huhk-1.9.3/huhk/case_project/project_init.py
+-rw-rw-rw-   0        0        0    18567 2023-07-31 08:18:51.000000 huhk-1.9.3/huhk/case_project/project_string.py
+-rw-rw-rw-   0        0        0      895 2023-07-26 08:22:28.000000 huhk-1.9.3/huhk/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-08-01 01:54:00.000000 huhk-1.9.3/huhk/case_project/version.py
+-rw-rw-rw-   0        0        0     9925 2023-07-31 05:34:49.000000 huhk-1.9.3/huhk/init_project.py
+-rw-rw-rw-   0        0        0     1267 2023-07-25 09:00:59.000000 huhk-1.9.3/huhk/main.py
+-rw-rw-rw-   0        0        0      338 2023-08-01 01:48:08.000000 huhk-1.9.3/huhk/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:54:00.934304 huhk-1.9.3/huhk/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.3/huhk/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:54:00.979747 huhk-1.9.3/huhk/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.3/huhk/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.9.3/huhk/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.9.3/huhk/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.9.3/huhk/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.9.3/huhk/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.9.3/huhk/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.9.3/huhk/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.9.3/huhk/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.9.3/huhk/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.9.3/huhk/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.9.3/huhk/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.9.3/huhk/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.9.3/huhk/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.9.3/huhk/unit_apache_beam.py
+-rw-rw-rw-   0        0        0      352 2023-07-31 09:35:09.000000 huhk-1.9.3/huhk/unit_data.py
+-rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.9.3/huhk/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.9.3/huhk/unit_encryption.py
+-rw-rw-rw-   0        0        0    28964 2023-08-01 01:47:59.000000 huhk-1.9.3/huhk/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.9.3/huhk/unit_logger.py
+-rw-rw-rw-   0        0        0     9960 2023-07-22 07:06:52.000000 huhk-1.9.3/huhk/unit_request.py
+-rw-rw-rw-   0        0        0     2511 2023-07-24 06:56:32.000000 huhk-1.9.3/huhk/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.9.3/huhk/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:54:00.907376 huhk-1.9.3/huhk.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-08-01 01:54:00.000000 huhk-1.9.3/huhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1440 2023-08-01 01:54:00.000000 huhk-1.9.3/huhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 01:54:00.000000 huhk-1.9.3/huhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-08-01 01:54:00.000000 huhk-1.9.3/huhk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-08-01 01:54:00.000000 huhk-1.9.3/huhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-08-01 01:54:00.000000 huhk-1.9.3/huhk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 01:54:00.982739 huhk-1.9.3/service/
+-rw-rw-rw-   0        0        0        0 2023-08-01 01:48:49.000000 huhk-1.9.3/service/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:54:00.988725 huhk-1.9.3/service/app_a/
+-rw-rw-rw-   0        0        0      420 2023-08-01 01:48:49.000000 huhk-1.9.3/service/app_a/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:54:00.990718 huhk-1.9.3/service/app_a/apis/
+-rw-rw-rw-   0        0        0        0 2023-08-01 01:48:49.000000 huhk-1.9.3/service/app_a/apis/__init__.py
+-rw-rw-rw-   0        0        0      752 2023-08-01 01:48:49.000000 huhk-1.9.3/service/app_a/app_a_fun.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:54:00.993709 huhk-1.9.3/service/app_a/asserts/
+-rw-rw-rw-   0        0        0        0 2023-08-01 01:48:49.000000 huhk-1.9.3/service/app_a/asserts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:54:00.996701 huhk-1.9.3/service/app_a/funs/
+-rw-rw-rw-   0        0        0        0 2023-08-01 01:48:49.000000 huhk-1.9.3/service/app_a/funs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:54:00.999693 huhk-1.9.3/service/app_a/sqls/
+-rw-rw-rw-   0        0        0        0 2023-08-01 01:48:49.000000 huhk-1.9.3/service/app_a/sqls/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 01:54:01.012658 huhk-1.9.3/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:54:01.002685 huhk-1.9.3/testcase/
+-rw-rw-rw-   0        0        0        0 2023-08-01 01:48:49.000000 huhk-1.9.3/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 01:54:01.009667 huhk-1.9.3/testcase/app_a/
+-rw-rw-rw-   0        0        0        0 2023-08-01 01:48:49.000000 huhk-1.9.3/testcase/app_a/__init__.py
+-rw-rw-rw-   0        0        0      361 2023-08-01 01:48:49.000000 huhk-1.9.3/testcase/app_a/conftest.py
```

### Comparing `huhk-1.9.2/huhk/__init__.py` & `huhk-1.9.3/huhk/__init__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/case_project/json_coder.py` & `huhk-1.9.3/huhk/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/case_project/main_fun.py` & `huhk-1.9.3/huhk/case_project/main_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/case_project/project_base.py` & `huhk-1.9.3/huhk/case_project/project_base.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/case_project/project_init.py` & `huhk-1.9.3/huhk/case_project/project_init.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/case_project/project_string.py` & `huhk-1.9.3/huhk/case_project/project_string.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/case_project/setup_set.py` & `huhk-1.9.3/huhk/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/init_project.py` & `huhk-1.9.3/huhk/init_project.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/main.py` & `huhk-1.9.3/huhk/main.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/testcase/apache/beam_class.py` & `huhk-1.9.3/huhk/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/testcase/apache/data.py` & `huhk-1.9.3/huhk/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/testcase/apache/par_do.py` & `huhk-1.9.3/huhk/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/testcase/apache/test_cogroupbykey.py` & `huhk-1.9.3/huhk/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/testcase/apache/test_fiter.py` & `huhk-1.9.3/huhk/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/testcase/apache/test_flatmap.py` & `huhk-1.9.3/huhk/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/testcase/apache/test_map.py` & `huhk-1.9.3/huhk/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/testcase/apache/test_par_do.py` & `huhk-1.9.3/huhk/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/testcase/apache/test_regex.py` & `huhk-1.9.3/huhk/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/testcase/apache/test_time.py` & `huhk-1.9.3/huhk/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/unit_apache_beam.py` & `huhk-1.9.3/huhk/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/unit_dict.py` & `huhk-1.9.3/huhk/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/unit_encryption.py` & `huhk-1.9.3/huhk/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/unit_fun.py` & `huhk-1.9.3/huhk/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/unit_logger.py` & `huhk-1.9.3/huhk/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/unit_request.py` & `huhk-1.9.3/huhk/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/unit_tasks.py` & `huhk-1.9.3/huhk/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk/常用命令.py` & `huhk-1.9.3/huhk/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.2/huhk.egg-info/SOURCES.txt` & `huhk-1.9.3/huhk.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -35,8 +35,18 @@
 huhk/testcase/apache/test_file.py
 huhk/testcase/apache/test_fiter.py
 huhk/testcase/apache/test_flatmap.py
 huhk/testcase/apache/test_map.py
 huhk/testcase/apache/test_par_do.py
 huhk/testcase/apache/test_regex.py
 huhk/testcase/apache/test_time.py
-huhk/testcase/apache/test_to_string.py
+huhk/testcase/apache/test_to_string.py
+service/__init__.py
+service/app_a/__init__.py
+service/app_a/app_a_fun.py
+service/app_a/apis/__init__.py
+service/app_a/asserts/__init__.py
+service/app_a/funs/__init__.py
+service/app_a/sqls/__init__.py
+testcase/__init__.py
+testcase/app_a/__init__.py
+testcase/app_a/conftest.py
```

