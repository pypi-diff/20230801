# Comparing `tmp/vavacars_data_utils-1.1.2.tar.gz` & `tmp/vavacars_data_utils-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vavacars_data_utils-1.1.2.tar", last modified: Fri Jul 28 11:01:37 2023, max compression
+gzip compressed data, was "vavacars_data_utils-1.1.3.tar", last modified: Tue Aug  1 06:26:19 2023, max compression
```

## Comparing `vavacars_data_utils-1.1.2.tar` & `vavacars_data_utils-1.1.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-07-28 11:01:37.150830 vavacars_data_utils-1.1.2/
--rwxrwxrwx   0 pga       (1000) pga       (1000)     2801 2023-07-28 11:01:37.151838 vavacars_data_utils-1.1.2/PKG-INFO
--rwxrwxrwx   0 pga       (1000) pga       (1000)     2321 2023-06-15 14:28:48.000000 vavacars_data_utils-1.1.2/README.md
--rwxrwxrwx   0 pga       (1000) pga       (1000)      124 2022-03-09 12:03:29.000000 vavacars_data_utils-1.1.2/pyproject.toml
--rwxrwxrwx   0 pga       (1000) pga       (1000)      799 2023-07-28 11:01:37.161832 vavacars_data_utils-1.1.2/setup.cfg
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-07-28 11:01:35.320710 vavacars_data_utils-1.1.2/test/
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-07-28 11:01:35.573778 vavacars_data_utils-1.1.2/test/utils/
--rwxrwxrwx   0 pga       (1000) pga       (1000)        0 2022-03-09 12:03:29.000000 vavacars_data_utils-1.1.2/test/utils/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     1159 2022-03-09 12:03:29.000000 vavacars_data_utils-1.1.2/test/utils/test_strings.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-07-28 11:01:35.599980 vavacars_data_utils-1.1.2/vava_utils/
--rwxrwxrwx   0 pga       (1000) pga       (1000)        0 2022-03-09 12:03:29.000000 vavacars_data_utils-1.1.2/vava_utils/__init__.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-07-28 11:01:35.691948 vavacars_data_utils-1.1.2/vava_utils/azure/
--rwxrwxrwx   0 pga       (1000) pga       (1000)       70 2022-05-04 13:49:57.000000 vavacars_data_utils-1.1.2/vava_utils/azure/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)    10180 2023-03-06 06:57:28.000000 vavacars_data_utils-1.1.2/vava_utils/azure/az_helper.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-07-28 11:01:35.795580 vavacars_data_utils-1.1.2/vava_utils/bigquery/
--rwxrwxrwx   0 pga       (1000) pga       (1000)       43 2023-06-15 14:28:48.000000 vavacars_data_utils-1.1.2/vava_utils/bigquery/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     1187 2023-06-15 14:28:48.000000 vavacars_data_utils-1.1.2/vava_utils/bigquery/bigquery_helper.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-07-28 11:01:35.892746 vavacars_data_utils-1.1.2/vava_utils/camunda/
--rwxrwxrwx   0 pga       (1000) pga       (1000)       85 2022-03-09 12:03:29.000000 vavacars_data_utils-1.1.2/vava_utils/camunda/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     4008 2023-05-16 14:47:25.000000 vavacars_data_utils-1.1.2/vava_utils/camunda/camunda_helper.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-07-28 11:01:36.005822 vavacars_data_utils-1.1.2/vava_utils/email/
--rwxrwxrwx   0 pga       (1000) pga       (1000)       37 2023-06-15 13:04:41.000000 vavacars_data_utils-1.1.2/vava_utils/email/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     3862 2023-06-29 09:16:49.000000 vavacars_data_utils-1.1.2/vava_utils/email/email_helper.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-07-28 11:01:36.094042 vavacars_data_utils-1.1.2/vava_utils/salesforce/
--rwxrwxrwx   0 pga       (1000) pga       (1000)       47 2023-06-09 14:13:08.000000 vavacars_data_utils-1.1.2/vava_utils/salesforce/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     2136 2023-06-15 14:28:48.000000 vavacars_data_utils-1.1.2/vava_utils/salesforce/salesforce_helper.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-07-28 11:01:36.257933 vavacars_data_utils-1.1.2/vava_utils/smartiq/
--rwxrwxrwx   0 pga       (1000) pga       (1000)      205 2022-04-25 14:18:59.000000 vavacars_data_utils-1.1.2/vava_utils/smartiq/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     7909 2022-04-25 14:18:59.000000 vavacars_data_utils-1.1.2/vava_utils/smartiq/smartiq_helper.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     9856 2022-06-16 14:27:47.000000 vavacars_data_utils-1.1.2/vava_utils/smartiq/smartiq_helper_v2.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-07-28 11:01:36.344301 vavacars_data_utils-1.1.2/vava_utils/sql/
--rwxrwxrwx   0 pga       (1000) pga       (1000)      160 2022-06-21 13:02:18.000000 vavacars_data_utils-1.1.2/vava_utils/sql/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)    12978 2023-07-28 11:00:56.000000 vavacars_data_utils-1.1.2/vava_utils/sql/sql_helper.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-07-28 11:01:36.454282 vavacars_data_utils-1.1.2/vava_utils/turkey/
--rwxrwxrwx   0 pga       (1000) pga       (1000)      148 2022-03-09 12:03:29.000000 vavacars_data_utils-1.1.2/vava_utils/turkey/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)      889 2022-03-09 12:03:29.000000 vavacars_data_utils-1.1.2/vava_utils/turkey/dates.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-07-28 11:01:36.863092 vavacars_data_utils-1.1.2/vava_utils/utils/
--rwxrwxrwx   0 pga       (1000) pga       (1000)      411 2023-07-27 10:32:52.000000 vavacars_data_utils-1.1.2/vava_utils/utils/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)      369 2022-03-09 12:03:29.000000 vavacars_data_utils-1.1.2/vava_utils/utils/callables.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     1950 2022-07-04 11:26:35.000000 vavacars_data_utils-1.1.2/vava_utils/utils/comparisons.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     1168 2023-06-15 14:28:48.000000 vavacars_data_utils-1.1.2/vava_utils/utils/naming.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)      273 2022-04-25 14:18:59.000000 vavacars_data_utils-1.1.2/vava_utils/utils/singleton.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)      734 2022-03-09 12:03:29.000000 vavacars_data_utils-1.1.2/vava_utils/utils/strings.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)      636 2023-07-27 10:32:52.000000 vavacars_data_utils-1.1.2/vava_utils/utils/utils.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-07-28 11:01:36.948646 vavacars_data_utils-1.1.2/vava_utils/vavaprice/
--rwxrwxrwx   0 pga       (1000) pga       (1000)       91 2022-03-11 15:04:33.000000 vavacars_data_utils-1.1.2/vava_utils/vavaprice/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     3225 2022-10-18 14:03:18.000000 vavacars_data_utils-1.1.2/vava_utils/vavaprice/vavaprice_helper.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-07-28 11:01:37.115708 vavacars_data_utils-1.1.2/vavacars_data_utils.egg-info/
--rwxrwxrwx   0 pga       (1000) pga       (1000)     2801 2023-07-28 11:01:34.000000 vavacars_data_utils-1.1.2/vavacars_data_utils.egg-info/PKG-INFO
--rwxrwxrwx   0 pga       (1000) pga       (1000)     1213 2023-07-28 11:01:35.000000 vavacars_data_utils-1.1.2/vavacars_data_utils.egg-info/SOURCES.txt
--rwxrwxrwx   0 pga       (1000) pga       (1000)        1 2023-07-28 11:01:34.000000 vavacars_data_utils-1.1.2/vavacars_data_utils.egg-info/dependency_links.txt
--rwxrwxrwx   0 pga       (1000) pga       (1000)       97 2023-07-28 11:01:34.000000 vavacars_data_utils-1.1.2/vavacars_data_utils.egg-info/requires.txt
--rwxrwxrwx   0 pga       (1000) pga       (1000)       16 2023-07-28 11:01:34.000000 vavacars_data_utils-1.1.2/vavacars_data_utils.egg-info/top_level.txt
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-08-01 06:26:19.484146 vavacars_data_utils-1.1.3/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     2801 2023-08-01 06:26:19.486150 vavacars_data_utils-1.1.3/PKG-INFO
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     2321 2023-06-15 14:28:48.000000 vavacars_data_utils-1.1.3/README.md
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      124 2022-03-09 12:03:29.000000 vavacars_data_utils-1.1.3/pyproject.toml
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      799 2023-08-01 06:26:19.492148 vavacars_data_utils-1.1.3/setup.cfg
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-08-01 06:26:17.836557 vavacars_data_utils-1.1.3/test/
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-08-01 06:26:18.058702 vavacars_data_utils-1.1.3/test/utils/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)        0 2022-03-09 12:03:29.000000 vavacars_data_utils-1.1.3/test/utils/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     1159 2022-03-09 12:03:29.000000 vavacars_data_utils-1.1.3/test/utils/test_strings.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-08-01 06:26:18.094272 vavacars_data_utils-1.1.3/vava_utils/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)        0 2022-03-09 12:03:29.000000 vavacars_data_utils-1.1.3/vava_utils/__init__.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-08-01 06:26:18.172179 vavacars_data_utils-1.1.3/vava_utils/azure/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       70 2022-05-04 13:49:57.000000 vavacars_data_utils-1.1.3/vava_utils/azure/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)    10204 2023-08-01 06:25:53.000000 vavacars_data_utils-1.1.3/vava_utils/azure/az_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-08-01 06:26:18.260703 vavacars_data_utils-1.1.3/vava_utils/bigquery/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       43 2023-06-15 14:28:48.000000 vavacars_data_utils-1.1.3/vava_utils/bigquery/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     1187 2023-06-15 14:28:48.000000 vavacars_data_utils-1.1.3/vava_utils/bigquery/bigquery_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-08-01 06:26:18.341869 vavacars_data_utils-1.1.3/vava_utils/camunda/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       85 2022-03-09 12:03:29.000000 vavacars_data_utils-1.1.3/vava_utils/camunda/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     4008 2023-05-16 14:47:25.000000 vavacars_data_utils-1.1.3/vava_utils/camunda/camunda_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-08-01 06:26:18.412102 vavacars_data_utils-1.1.3/vava_utils/email/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       37 2023-06-15 13:04:41.000000 vavacars_data_utils-1.1.3/vava_utils/email/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     3862 2023-06-29 09:16:49.000000 vavacars_data_utils-1.1.3/vava_utils/email/email_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-08-01 06:26:18.490579 vavacars_data_utils-1.1.3/vava_utils/salesforce/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       47 2023-06-09 14:13:08.000000 vavacars_data_utils-1.1.3/vava_utils/salesforce/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     2136 2023-06-15 14:28:48.000000 vavacars_data_utils-1.1.3/vava_utils/salesforce/salesforce_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-08-01 06:26:18.611972 vavacars_data_utils-1.1.3/vava_utils/smartiq/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      205 2022-04-25 14:18:59.000000 vavacars_data_utils-1.1.3/vava_utils/smartiq/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     7909 2022-04-25 14:18:59.000000 vavacars_data_utils-1.1.3/vava_utils/smartiq/smartiq_helper.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     9856 2022-06-16 14:27:47.000000 vavacars_data_utils-1.1.3/vava_utils/smartiq/smartiq_helper_v2.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-08-01 06:26:18.714630 vavacars_data_utils-1.1.3/vava_utils/sql/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      160 2022-06-21 13:02:18.000000 vavacars_data_utils-1.1.3/vava_utils/sql/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)    12978 2023-07-28 11:00:56.000000 vavacars_data_utils-1.1.3/vava_utils/sql/sql_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-08-01 06:26:18.805162 vavacars_data_utils-1.1.3/vava_utils/turkey/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      148 2022-03-09 12:03:29.000000 vavacars_data_utils-1.1.3/vava_utils/turkey/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      889 2022-03-09 12:03:29.000000 vavacars_data_utils-1.1.3/vava_utils/turkey/dates.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-08-01 06:26:19.188847 vavacars_data_utils-1.1.3/vava_utils/utils/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      411 2023-07-27 10:32:52.000000 vavacars_data_utils-1.1.3/vava_utils/utils/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      369 2022-03-09 12:03:29.000000 vavacars_data_utils-1.1.3/vava_utils/utils/callables.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     1950 2022-07-04 11:26:35.000000 vavacars_data_utils-1.1.3/vava_utils/utils/comparisons.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     1168 2023-06-15 14:28:48.000000 vavacars_data_utils-1.1.3/vava_utils/utils/naming.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      273 2022-04-25 14:18:59.000000 vavacars_data_utils-1.1.3/vava_utils/utils/singleton.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      734 2022-03-09 12:03:29.000000 vavacars_data_utils-1.1.3/vava_utils/utils/strings.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      636 2023-07-27 10:32:52.000000 vavacars_data_utils-1.1.3/vava_utils/utils/utils.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-08-01 06:26:19.304046 vavacars_data_utils-1.1.3/vava_utils/vavaprice/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       91 2022-03-11 15:04:33.000000 vavacars_data_utils-1.1.3/vava_utils/vavaprice/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     3225 2022-10-18 14:03:18.000000 vavacars_data_utils-1.1.3/vava_utils/vavaprice/vavaprice_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-08-01 06:26:19.463633 vavacars_data_utils-1.1.3/vavacars_data_utils.egg-info/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     2801 2023-08-01 06:26:17.000000 vavacars_data_utils-1.1.3/vavacars_data_utils.egg-info/PKG-INFO
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     1213 2023-08-01 06:26:17.000000 vavacars_data_utils-1.1.3/vavacars_data_utils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 pga       (1000) pga       (1000)        1 2023-08-01 06:26:17.000000 vavacars_data_utils-1.1.3/vavacars_data_utils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       97 2023-08-01 06:26:17.000000 vavacars_data_utils-1.1.3/vavacars_data_utils.egg-info/requires.txt
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       16 2023-08-01 06:26:17.000000 vavacars_data_utils-1.1.3/vavacars_data_utils.egg-info/top_level.txt
```

### Comparing `vavacars_data_utils-1.1.2/PKG-INFO` & `vavacars_data_utils-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vavacars_data_utils
-Version: 1.1.2
+Version: 1.1.3
 Summary: Package with utils
 Home-page: https://dev.azure.com/vavacars/DataScience/_git/Data.Utils
 Author: Vavacars Data Science Team
 Author-email: acg@vava.cars
 Project-URL: Bug Tracker, https://dev.azure.com/vavacars/DataScience/_workitems/recentlyupdated/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `vavacars_data_utils-1.1.2/README.md` & `vavacars_data_utils-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.1.2/setup.cfg` & `vavacars_data_utils-1.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vavacars_data_utils
-version = 1.1.2
+version = 1.1.3
 author = Vavacars Data Science Team
 author_email = acg@vava.cars
 description = Package with utils
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://dev.azure.com/vavacars/DataScience/_git/Data.Utils
 project_urls =
```

### Comparing `vavacars_data_utils-1.1.2/test/utils/test_strings.py` & `vavacars_data_utils-1.1.3/test/utils/test_strings.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.1.2/vava_utils/azure/az_helper.py` & `vavacars_data_utils-1.1.3/vava_utils/azure/az_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,30 +230,31 @@
             version (string): Dataset version
 
         Returns:
             pd.DataFrame
         """
         return Dataset.get_by_name(self.ws, name, version).to_pandas_dataframe()
 
-    def write_dataset(self, df, datastore, ds_path, name=None, tags={}, date_tag=True,**kwargs):
+    def write_dataset(self, df, datastore, ds_path, name=None, tags={}, date_tag=True, **kwargs):
         """
         Writes Pandas DF to Azure Dataset
 
         Parameters:
             df (pd.DataFrame): data to write
             datastore (string): Azure Datastore name
             ds_path (string): path for file in Datastore
             name (string): Dataset name, if None will take ds_path as name
-            tags (dict): 
+            tags (dict):
 
         Returns:
             pd.DataFrame
         """
 
         if date_tag:
-            tags['date'] = datetime.datetime.today().strftime('%Y-%m-%d'), 
+            tags["date"] = (datetime.datetime.today().strftime("%Y-%m-%d"),)
         return Dataset.Tabular.register_pandas_dataframe(
             dataframe=df,
             target=(Datastore.get(self.ws, datastore), ds_path),
             name=ds_path if name is None else name,
+            tags=tags,
             **kwargs,
         )
```

### Comparing `vavacars_data_utils-1.1.2/vava_utils/bigquery/bigquery_helper.py` & `vavacars_data_utils-1.1.3/vava_utils/bigquery/bigquery_helper.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.1.2/vava_utils/camunda/camunda_helper.py` & `vavacars_data_utils-1.1.3/vava_utils/camunda/camunda_helper.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.1.2/vava_utils/email/email_helper.py` & `vavacars_data_utils-1.1.3/vava_utils/email/email_helper.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.1.2/vava_utils/salesforce/salesforce_helper.py` & `vavacars_data_utils-1.1.3/vava_utils/salesforce/salesforce_helper.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.1.2/vava_utils/smartiq/smartiq_helper.py` & `vavacars_data_utils-1.1.3/vava_utils/smartiq/smartiq_helper.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.1.2/vava_utils/smartiq/smartiq_helper_v2.py` & `vavacars_data_utils-1.1.3/vava_utils/smartiq/smartiq_helper_v2.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.1.2/vava_utils/sql/sql_helper.py` & `vavacars_data_utils-1.1.3/vava_utils/sql/sql_helper.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.1.2/vava_utils/turkey/dates.py` & `vavacars_data_utils-1.1.3/vava_utils/turkey/dates.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.1.2/vava_utils/utils/comparisons.py` & `vavacars_data_utils-1.1.3/vava_utils/utils/comparisons.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.1.2/vava_utils/utils/naming.py` & `vavacars_data_utils-1.1.3/vava_utils/utils/naming.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.1.2/vava_utils/utils/strings.py` & `vavacars_data_utils-1.1.3/vava_utils/utils/strings.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.1.2/vava_utils/utils/utils.py` & `vavacars_data_utils-1.1.3/vava_utils/utils/utils.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.1.2/vava_utils/vavaprice/vavaprice_helper.py` & `vavacars_data_utils-1.1.3/vava_utils/vavaprice/vavaprice_helper.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.1.2/vavacars_data_utils.egg-info/PKG-INFO` & `vavacars_data_utils-1.1.3/vavacars_data_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vavacars-data-utils
-Version: 1.1.2
+Version: 1.1.3
 Summary: Package with utils
 Home-page: https://dev.azure.com/vavacars/DataScience/_git/Data.Utils
 Author: Vavacars Data Science Team
 Author-email: acg@vava.cars
 Project-URL: Bug Tracker, https://dev.azure.com/vavacars/DataScience/_workitems/recentlyupdated/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `vavacars_data_utils-1.1.2/vavacars_data_utils.egg-info/SOURCES.txt` & `vavacars_data_utils-1.1.3/vavacars_data_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

