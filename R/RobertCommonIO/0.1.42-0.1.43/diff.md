# Comparing `tmp/RobertCommonIO-0.1.42.tar.gz` & `tmp/RobertCommonIO-0.1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonIO-0.1.42.tar", last modified: Fri Jun  9 09:56:56 2023, max compression
+gzip compressed data, was "RobertCommonIO-0.1.43.tar", last modified: Tue Aug  1 09:28:36 2023, max compression
```

## Comparing `RobertCommonIO-0.1.42.tar` & `RobertCommonIO-0.1.43.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:56.698934 RobertCommonIO-0.1.42/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonIO-0.1.42/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonIO-0.1.42/MANIFEST.in
--rw-rw-rw-   0        0        0      878 2023-06-09 09:56:56.698934 RobertCommonIO-0.1.42/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-06-02 07:57:14.000000 RobertCommonIO-0.1.42/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:56.653400 RobertCommonIO-0.1.42/RobertCommonIO.egg-info/
--rw-rw-rw-   0        0        0      878 2023-06-09 09:56:56.000000 RobertCommonIO-0.1.42/RobertCommonIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1703 2023-06-09 09:56:56.000000 RobertCommonIO-0.1.42/RobertCommonIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 09:56:56.000000 RobertCommonIO-0.1.42/RobertCommonIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      250 2023-06-09 09:56:56.000000 RobertCommonIO-0.1.42/RobertCommonIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-09 09:56:56.000000 RobertCommonIO-0.1.42/RobertCommonIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      275 2023-06-09 09:31:22.000000 RobertCommonIO-0.1.42/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:56.654400 RobertCommonIO-0.1.42/robertcommonio/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonIO-0.1.42/robertcommonio/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:56.655400 RobertCommonIO-0.1.42/robertcommonio/system/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonIO-0.1.42/robertcommonio/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:56.676688 RobertCommonIO-0.1.42/robertcommonio/system/io/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/__init__.py
--rw-rw-rw-   0        0        0    19281 2023-04-04 06:29:48.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/data_storage.py
--rw-rw-rw-   0        0        0     3336 2023-06-06 03:31:50.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/email.py
--rw-rw-rw-   0        0        0     7388 2023-04-19 09:38:00.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/file.py
--rw-rw-rw-   0        0        0     6347 2022-10-09 08:05:49.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/ftp.py
--rw-rw-rw-   0        0        0    10214 2023-02-21 02:59:34.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/http.py
--rw-rw-rw-   0        0        0     3334 2023-01-31 09:43:08.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/ini.py
--rw-rw-rw-   0        0        0     6566 2022-11-24 06:58:34.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/license.py
--rw-rw-rw-   0        0        0    27538 2023-06-08 15:33:06.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/mongo.py
--rw-rw-rw-   0        0        0     6883 2023-05-16 09:34:00.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/mqtt.py
--rw-rw-rw-   0        0        0     6535 2023-01-04 05:46:19.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/mysql.py
--rw-rw-rw-   0        0        0     3900 2022-11-22 07:50:13.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/oss.py
--rw-rw-rw-   0        0        0     7191 2022-11-22 07:56:12.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/rabitmq.py
--rw-rw-rw-   0        0        0    11702 2022-10-09 08:16:48.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/redis.py
--rw-rw-rw-   0        0        0     2267 2022-10-09 08:16:48.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/redis_cache.py
--rw-rw-rw-   0        0        0     9779 2023-05-25 09:55:20.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/response.py
--rw-rw-rw-   0        0        0    37639 2023-02-23 08:23:07.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/socket.py
--rw-rw-rw-   0        0        0     7249 2023-05-26 06:26:38.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/sqlalche.py
--rw-rw-rw-   0        0        0     6710 2022-11-22 07:58:41.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/transport.py
--rw-rw-rw-   0        0        0      725 2022-12-14 08:37:33.000000 RobertCommonIO-0.1.42/robertcommonio/system/io/version.py
--rw-rw-rw-   0        0        0       42 2023-06-09 09:56:56.698934 RobertCommonIO-0.1.42/setup.cfg
--rw-rw-rw-   0        0        0     3869 2023-06-09 09:33:34.000000 RobertCommonIO-0.1.42/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:56.678681 RobertCommonIO-0.1.42/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonIO-0.1.42/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:56.678681 RobertCommonIO-0.1.42/tests/test_system/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonIO-0.1.42/tests/test_system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:56:56.696911 RobertCommonIO-0.1.42/tests/test_system/test_io/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:50:10.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/__init__.py
--rw-rw-rw-   0        0        0     1322 2023-01-04 02:27:37.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test.py
--rw-rw-rw-   0        0        0     1570 2023-01-05 05:43:17.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_data_storage.py
--rw-rw-rw-   0        0        0    14345 2023-06-06 02:41:30.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_email.py
--rw-rw-rw-   0        0        0     3985 2022-07-11 02:23:20.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_file.py
--rw-rw-rw-   0        0        0      978 2022-05-25 08:49:17.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_ftp.py
--rw-rw-rw-   0        0        0      399 2022-12-14 07:23:38.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_http.py
--rw-rw-rw-   0        0        0      413 2022-01-13 06:50:54.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_ini.py
--rw-rw-rw-   0        0        0     1187 2023-03-09 08:37:11.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_license.py
--rw-rw-rw-   0        0        0     3141 2023-04-04 06:18:30.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_mongo.py
--rw-rw-rw-   0        0        0     1582 2022-04-20 08:37:11.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_mqtt.py
--rw-rw-rw-   0        0        0    10544 2021-12-24 13:47:06.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_oracle.py
--rw-rw-rw-   0        0        0     1028 2022-09-07 06:12:44.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_rabbitmq.py
--rw-rw-rw-   0        0        0     4221 2022-10-09 07:39:57.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_socket.py
--rw-rw-rw-   0        0        0     3967 2023-06-02 08:41:38.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_sqlalche.py
--rw-rw-rw-   0        0        0     1389 2022-10-13 09:07:08.000000 RobertCommonIO-0.1.42/tests/test_system/test_io/test_transport.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:28:36.958694 RobertCommonIO-0.1.43/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonIO-0.1.43/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonIO-0.1.43/MANIFEST.in
+-rw-rw-rw-   0        0        0      878 2023-08-01 09:28:36.958694 RobertCommonIO-0.1.43/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-06-02 07:57:14.000000 RobertCommonIO-0.1.43/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 09:28:36.913441 RobertCommonIO-0.1.43/RobertCommonIO.egg-info/
+-rw-rw-rw-   0        0        0      878 2023-08-01 09:28:36.000000 RobertCommonIO-0.1.43/RobertCommonIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-08-01 09:28:36.000000 RobertCommonIO-0.1.43/RobertCommonIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 09:28:36.000000 RobertCommonIO-0.1.43/RobertCommonIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      262 2023-08-01 09:28:36.000000 RobertCommonIO-0.1.43/RobertCommonIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-08-01 09:28:36.000000 RobertCommonIO-0.1.43/RobertCommonIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      288 2023-08-01 09:17:21.000000 RobertCommonIO-0.1.43/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 09:28:36.914437 RobertCommonIO-0.1.43/robertcommonio/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonIO-0.1.43/robertcommonio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:28:36.915439 RobertCommonIO-0.1.43/robertcommonio/system/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonIO-0.1.43/robertcommonio/system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:28:36.934496 RobertCommonIO-0.1.43/robertcommonio/system/io/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/__init__.py
+-rw-rw-rw-   0        0        0    19301 2023-06-13 02:16:52.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/data_storage.py
+-rw-rw-rw-   0        0        0     3380 2023-06-13 06:54:18.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/email.py
+-rw-rw-rw-   0        0        0     7388 2023-04-19 09:38:00.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/file.py
+-rw-rw-rw-   0        0        0     6347 2022-10-09 08:05:49.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/ftp.py
+-rw-rw-rw-   0        0        0    10214 2023-02-21 02:59:34.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/http.py
+-rw-rw-rw-   0        0        0     3390 2023-08-01 09:18:07.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/ini.py
+-rw-rw-rw-   0        0        0     4351 2023-08-01 09:23:18.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/job.py
+-rw-rw-rw-   0        0        0     6566 2022-11-24 06:58:34.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/license.py
+-rw-rw-rw-   0        0        0    27527 2023-06-13 02:37:00.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/mongo.py
+-rw-rw-rw-   0        0        0     7107 2023-08-01 09:27:32.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/mqtt.py
+-rw-rw-rw-   0        0        0     6535 2023-01-04 05:46:19.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/mysql.py
+-rw-rw-rw-   0        0        0     3900 2022-11-22 07:50:13.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/oss.py
+-rw-rw-rw-   0        0        0    19915 2023-06-13 09:03:21.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/rabitmq.py
+-rw-rw-rw-   0        0        0    11702 2022-10-09 08:16:48.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/redis.py
+-rw-rw-rw-   0        0        0     2267 2022-10-09 08:16:48.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/redis_cache.py
+-rw-rw-rw-   0        0        0     9779 2023-05-25 09:55:20.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/response.py
+-rw-rw-rw-   0        0        0    37671 2023-08-01 09:13:24.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/socket.py
+-rw-rw-rw-   0        0        0     7306 2023-06-13 02:14:30.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/sqlalche.py
+-rw-rw-rw-   0        0        0     6710 2022-11-22 07:58:41.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/transport.py
+-rw-rw-rw-   0        0        0      725 2022-12-14 08:37:33.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/version.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 09:28:36.958694 RobertCommonIO-0.1.43/setup.cfg
+-rw-rw-rw-   0        0        0     3869 2023-08-01 09:18:29.000000 RobertCommonIO-0.1.43/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:28:36.935446 RobertCommonIO-0.1.43/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonIO-0.1.43/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:28:36.936444 RobertCommonIO-0.1.43/tests/test_system/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonIO-0.1.43/tests/test_system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:28:36.957696 RobertCommonIO-0.1.43/tests/test_system/test_io/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:50:10.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/__init__.py
+-rw-rw-rw-   0        0        0     1322 2023-01-04 02:27:37.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test.py
+-rw-rw-rw-   0        0        0     1570 2023-01-05 05:43:17.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_data_storage.py
+-rw-rw-rw-   0        0        0    14345 2023-06-06 02:41:30.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_email.py
+-rw-rw-rw-   0        0        0     3985 2022-07-11 02:23:20.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_file.py
+-rw-rw-rw-   0        0        0      978 2022-05-25 08:49:17.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_ftp.py
+-rw-rw-rw-   0        0        0      570 2023-07-10 09:37:45.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_http.py
+-rw-rw-rw-   0        0        0      413 2022-01-13 06:50:54.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_ini.py
+-rw-rw-rw-   0        0        0      381 2023-06-13 07:55:37.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_job.py
+-rw-rw-rw-   0        0        0     1187 2023-03-09 08:37:11.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_license.py
+-rw-rw-rw-   0        0        0     3141 2023-04-04 06:18:30.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_mongo.py
+-rw-rw-rw-   0        0        0     1582 2022-04-20 08:37:11.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_mqtt.py
+-rw-rw-rw-   0        0        0    10544 2021-12-24 13:47:06.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_oracle.py
+-rw-rw-rw-   0        0        0     1028 2022-09-07 06:12:44.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_rabbitmq.py
+-rw-rw-rw-   0        0        0     4221 2022-10-09 07:39:57.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_socket.py
+-rw-rw-rw-   0        0        0     3967 2023-06-02 08:41:38.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_sqlalche.py
+-rw-rw-rw-   0        0        0     1389 2022-10-13 09:07:08.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_transport.py
```

### Comparing `RobertCommonIO-0.1.42/LICENSE` & `RobertCommonIO-0.1.43/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/PKG-INFO` & `RobertCommonIO-0.1.43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonIO
-Version: 0.1.42
+Version: 0.1.43
 Summary: Robert Common IO Library
 Home-page: https://github.com/hun0423/RobertCommonIO
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonIO-0.1.42/RobertCommonIO.egg-info/PKG-INFO` & `RobertCommonIO-0.1.43/RobertCommonIO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonIO
-Version: 0.1.42
+Version: 0.1.43
 Summary: Robert Common IO Library
 Home-page: https://github.com/hun0423/RobertCommonIO
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonIO-0.1.42/RobertCommonIO.egg-info/SOURCES.txt` & `RobertCommonIO-0.1.43/RobertCommonIO.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 robertcommonio/system/io/__init__.py
 robertcommonio/system/io/data_storage.py
 robertcommonio/system/io/email.py
 robertcommonio/system/io/file.py
 robertcommonio/system/io/ftp.py
 robertcommonio/system/io/http.py
 robertcommonio/system/io/ini.py
+robertcommonio/system/io/job.py
 robertcommonio/system/io/license.py
 robertcommonio/system/io/mongo.py
 robertcommonio/system/io/mqtt.py
 robertcommonio/system/io/mysql.py
 robertcommonio/system/io/oss.py
 robertcommonio/system/io/rabitmq.py
 robertcommonio/system/io/redis.py
@@ -36,14 +37,15 @@
 tests/test_system/test_io/test.py
 tests/test_system/test_io/test_data_storage.py
 tests/test_system/test_io/test_email.py
 tests/test_system/test_io/test_file.py
 tests/test_system/test_io/test_ftp.py
 tests/test_system/test_io/test_http.py
 tests/test_system/test_io/test_ini.py
+tests/test_system/test_io/test_job.py
 tests/test_system/test_io/test_license.py
 tests/test_system/test_io/test_mongo.py
 tests/test_system/test_io/test_mqtt.py
 tests/test_system/test_io/test_oracle.py
 tests/test_system/test_io/test_rabbitmq.py
 tests/test_system/test_io/test_socket.py
 tests/test_system/test_io/test_sqlalche.py
```

### Comparing `RobertCommonIO-0.1.42/robertcommonio/system/io/data_storage.py` & `RobertCommonIO-0.1.43/robertcommonio/system/io/data_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,15 +249,15 @@
             self.accessor.write_sql_many(f'replace into {self.get_real_tb()} (name, time, value) values (%s,%s,%s)', params_list)
             return True
         return False
 
     def load_first_data_time(self) -> datetime:
         if isinstance(self.accessor, MongoAccessor):
             doc: Dict = self.accessor.mdbBb[self.get_history_tb()].find_one({}, sort=[("time", ASCENDING)])
-            result = None
+            result: Optional[datetime] = None
             if doc:
                 result = doc['time']
                 time_group = list(self.accessor.mdbBb[self.get_history_tb()].find({"time": result}))
                 min_item = min(time_group, key=lambda i: min(map(int, i["value"].keys())))
                 min_hour = min(min_item["value"].keys(), key=lambda i: int(i))
                 min_minute = min(min_item['value'][min_hour].keys(), key=lambda i: int(i))
                 result += timedelta(hours=float(min_hour), minutes=float(min_minute))
```

### Comparing `RobertCommonIO-0.1.42/robertcommonio/system/io/email.py` & `RobertCommonIO-0.1.43/robertcommonio/system/io/email.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,24 @@
 
 class EmailConfig(NamedTuple):
     HOST: str
     PORT: int
     USER: str
     PSW: str
     FROM: str
+    TIMEOUT: int = 60
 
 
 class EmailAccessor:
 
     def __init__(self, config: EmailConfig):
         self.config = config
 
     def _send(self, recipients: str, smtp_msg: Any):
-        with SMTP(self.config.HOST, self.config.PORT) as smtp_handle:
+        with SMTP(self.config.HOST, self.config.PORT, self.config.TIMEOUT) as smtp_handle:
             smtp_handle.starttls()
             smtp_handle.login(self.config.USER, self.config.PSW)
             smtp_handle.sendmail(self.config.FROM, recipients.split(','), smtp_msg.as_string())
             smtp_handle.quit()
         return True
 
     def crate_email(self, sender: str, recipients: str, datas: list, title: str = '', ccs: str = ''):
```

### Comparing `RobertCommonIO-0.1.42/robertcommonio/system/io/file.py` & `RobertCommonIO-0.1.43/robertcommonio/system/io/file.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/robertcommonio/system/io/ftp.py` & `RobertCommonIO-0.1.43/robertcommonio/system/io/ftp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/robertcommonio/system/io/http.py` & `RobertCommonIO-0.1.43/robertcommonio/system/io/http.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/robertcommonio/system/io/ini.py` & `RobertCommonIO-0.1.43/robertcommonio/system/io/ini.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from configparser import ConfigParser
 from typing import NamedTuple, Any, Optional
 
+from robertcommonbasic.basic.file.ini import SensitiveConfigParser
 from robertcommonbasic.basic.os.file import get_file_folder
 from robertcommonbasic.basic.os.path import create_dir_if_not_exist
 from robertcommonbasic.basic.validation import input as input_checker
 
 
 class INIConfig(NamedTuple):
     PATH: str
@@ -26,28 +26,28 @@
         self.read_file()
 
     def ini_file(self):
         folder = get_file_folder(self.file_path)
         if len(folder) > 0:
             create_dir_if_not_exist(folder)
 
-        config = ConfigParser()
+        config = SensitiveConfigParser()
         config.read(self.file_path)
 
         for section_key in self.default_params.keys():
             for param_key in self.default_params.get(section_key).keys():
                 if config.has_section(section_key) is False:
                     config.add_section(section_key)
                 if config.has_option(section_key, param_key.lower()) is False:
                     config.set(section_key, param_key.lower(), input_checker.ensure_str(param_key, self.default_params.get(section_key)))
 
         config.write(open(self.file_path, 'w'))
 
     def read_file(self):
-        config = ConfigParser()
+        config = SensitiveConfigParser()
         config.read(self.file_path)
 
         for section in config.sections():
             for option in config.options(section):
                 self.config_sections[option] = section
                 self.config_params[option] = config.get(section, option)
 
@@ -66,15 +66,15 @@
         else:
             return input_checker.ensure_not_none(param_key, self.config_params)
 
     def set(self, param_key: str, param_value: Any, section_key: Optional[str] = None):
         param_key = param_key.lower()
         self.config_params[param_key] = param_value
 
-        config = ConfigParser()
+        config = SensitiveConfigParser()
         config.read(self.file_path)
 
         if section_key is not None:
             if config.has_section(section_key) is False:
                 config.add_section(section_key)
             config.set(section_key, param_key, param_value)
             config.write(open(self.file_path, 'w'))
```

### Comparing `RobertCommonIO-0.1.42/robertcommonio/system/io/license.py` & `RobertCommonIO-0.1.43/robertcommonio/system/io/license.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/robertcommonio/system/io/mongo.py` & `RobertCommonIO-0.1.43/robertcommonio/system/io/mongo.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
             kwargs['sort'] = sort
         if session:
             kwargs['session'] = session
         with coll.find(filter=query, **kwargs) as cursor:
             for doc in cursor:
                 yield doc
 
-    def count(self, coll_name: str, query: dict, projection: Optional[dict] = None, tz_info: Optional[str] = None) -> Iterator[dict]:
+    def count(self, coll_name: str, query: dict, projection: Optional[dict] = None, tz_info: Optional[str] = None) -> int:
         coll = self._get_coll(coll_name, tz_info)
         kwargs = {}
         if projection:
             kwargs['projection'] = projection
         return coll.count_documents(filter=query, **kwargs)
 
     def aggr(self, coll_name: str, pipeline: List, allow_disk_use: bool = False, session: Optional[ClientSession] = None, tz_info: Optional[str] = None) -> Iterator[dict]:
```

### Comparing `RobertCommonIO-0.1.42/robertcommonio/system/io/mqtt.py` & `RobertCommonIO-0.1.43/robertcommonio/system/io/mqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,42 +81,45 @@
                 self.client.loop_stop()
                 self.set_call_result('debug_log', content=f"close success")
         finally:
             self.client = None
 
     def get_client(self, client_mode='sub'):
         if self.client is None:
-            clean_session = self.config.SHORT_CONNECT  # False表示要建立一个持久性会话
-            if self.config.CLIENT_ID is None or len(self.config.CLIENT_ID) == 0:
-                client = mqtt.Client(client_id='', clean_session=True)
-            else:
-                client = mqtt.Client(self.config.CLIENT_ID, clean_session=clean_session)
-            if self.config.USER is not None and self.config.PSW is not None and len(self.config.USER) > 0:
-                client.username_pw_set(self.config.USER, self.config.PSW)
-            client.on_connect = self.on_connect
-            client.on_message = self.on_message
-            client.on_subscribe = self.on_subscribe
-            client.on_disconnect = self.on_disconnect
-            client.on_publish = self.on_publish
-            client.on_log = self.on_log
-            client.connect(self.config.HOST, self.config.PORT, self.config.KEEP_ALIVE)
-            client.reconnect_delay_set(self.config.MIN_RECONNECT_DELAY, self.config.MAX_RECONNECT_DELAY)
-            if client_mode == 'pub':
-                client.loop_start()
+            try:
+                clean_session = self.config.SHORT_CONNECT  # False表示要建立一个持久性会话
+                if self.config.CLIENT_ID is None or len(self.config.CLIENT_ID) == 0:
+                    client = mqtt.Client(client_id='', clean_session=True)
+                else:
+                    client = mqtt.Client(self.config.CLIENT_ID, clean_session=clean_session)
+                if self.config.USER is not None and self.config.PSW is not None and len(self.config.USER) > 0:
+                    client.username_pw_set(self.config.USER, self.config.PSW)
+                client.on_connect = self.on_connect
+                client.on_message = self.on_message
+                client.on_subscribe = self.on_subscribe
+                client.on_disconnect = self.on_disconnect
+                client.on_publish = self.on_publish
+                client.on_log = self.on_log
+                client.connect(self.config.HOST, self.config.PORT, self.config.KEEP_ALIVE)
+                client.reconnect_delay_set(self.config.MIN_RECONNECT_DELAY, self.config.MAX_RECONNECT_DELAY)
+                if client_mode == 'pub':
+                    client.loop_start()
 
-                wait = 5
-                while not client.is_connected() and wait > 0:    # 等待连接
-                    time.sleep(1)
-                    wait = wait - 1
+                    wait = 5
+                    while not client.is_connected() and wait > 0:    # 等待连接
+                        time.sleep(1)
+                        wait = wait - 1
 
-                if client.is_connected() is False:
-                    client.disconnect()
-                    client.loop_stop()
-                    raise Exception(f"connect fail")
-            self.client = client
+                    if client.is_connected() is False:
+                        client.disconnect()
+                        client.loop_stop()
+                        raise Exception(f"not connected")
+                self.client = client
+            except Exception as e:
+                raise Exception(f"connect fail({e.__str__()})")
         return self.client
 
     def publish_topic(self, topic: str, message: str, qos: int = 0) -> bool:
         client = self.get_client('pub')
         if client is not None:
             connect_status = False
             if client._state != 2:
```

### Comparing `RobertCommonIO-0.1.42/robertcommonio/system/io/mysql.py` & `RobertCommonIO-0.1.43/robertcommonio/system/io/mysql.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/robertcommonio/system/io/oss.py` & `RobertCommonIO-0.1.43/robertcommonio/system/io/oss.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/robertcommonio/system/io/redis.py` & `RobertCommonIO-0.1.43/robertcommonio/system/io/redis.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/robertcommonio/system/io/redis_cache.py` & `RobertCommonIO-0.1.43/robertcommonio/system/io/redis_cache.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/robertcommonio/system/io/response.py` & `RobertCommonIO-0.1.43/robertcommonio/system/io/response.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/robertcommonio/system/io/socket.py` & `RobertCommonIO-0.1.43/robertcommonio/system/io/socket.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,16 +403,16 @@
             self.config.CALL_BACK['handle_error'](self, e)
         else:
             logging.error(f"handle_error({self})({e.__str__()})")
             
     def recv_bytes(self, length: int) -> Optional[bytes]:
         data = b''
         while self.check_invalid() is True and len(data) < length:
-            rec_length = min(self.config.BUFFER, length - len(data))
-            rec_data = self.sock.recv(rec_length)
+            #rec_length = min(self.config.BUFFER, length - len(data))
+            rec_data = self.sock.recv(length - len(data))   # 加快接收速度
             if rec_data is None or len(rec_data) == 0:
                 raise CloseException(f"remote close")
             data += rec_data
         if len(data) != length:
             raise NormalException(f"recv length fail({len(data)}/{length})")
         return data
```

### Comparing `RobertCommonIO-0.1.42/robertcommonio/system/io/sqlalche.py` & `RobertCommonIO-0.1.43/robertcommonio/system/io/sqlalche.py`

 * *Files 7% similar despite different names*

```diff
@@ -108,22 +108,23 @@
             # 获取原表建表语句
             crate_sql = str(CreateTable(old_table))
             base.metadata.clear()
             return crate_sql
         return None
 
     def generate_sql_format(self, table_name: str, action: str = 'replace', colums: Optional[list] = None, filter_column: Optional[list] = None, add_syntax: bool = False):
-        filed_format = '{}' if add_syntax is False else '`{}`'
-        filed_format1 = '{} = :{}' if add_syntax is False else '`{}` = :{}'
+        insert_fmt = '{}' if add_syntax is False else '`{}`'
+        insert_value_fmt = ':{}'
+        updte_value_fmt = '{} = :{}' if add_syntax is False else '`{}` = :{}'
         if action in ['replace', 'append']:
-            return f"insert into {table_name} ({', '.join(filed_format.format(k) for k in colums)}) VALUES ({', '.join(':{}'.format(k) for k in colums)})"
+            return f"insert into {table_name} ({', '.join(insert_fmt.format(k) for k in colums)}) VALUES ({', '.join(insert_value_fmt.format(k) for k in colums)})"
         elif action == 'update':
-            return f"update {table_name} set {', '.join(filed_format1.format(k, k) for k in colums)} where {', '.join(filed_format1.format(k, k) for k in filter_column)}"
+            return f"update {table_name} set {', '.join(updte_value_fmt.format(k, k) for k in colums)} where {', and '.join(updte_value_fmt.format(k, k) for k in filter_column)}"
         elif action == 'delete':
-            return f"delete from {table_name} where {', '.join(filed_format1.format(k, k) for k in filter_column)}"
+            return f"delete from {table_name} where {', and '.join(updte_value_fmt.format(k, k) for k in filter_column)}"
 
     def generate_sql_cmds(self, table_name: str, records: list, action: str = 'replace', colums: list = None, filter_column: list = None, add_syntax: bool = False):
         cmds = []
         if len(records) > 0:
             if action == 'replace':
                 if filter_column is None:
                     cmds.append((f"delete from {table_name}", None))
```

### Comparing `RobertCommonIO-0.1.42/robertcommonio/system/io/transport.py` & `RobertCommonIO-0.1.43/robertcommonio/system/io/transport.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/robertcommonio/system/io/version.py` & `RobertCommonIO-0.1.43/robertcommonio/system/io/version.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/setup.py` & `RobertCommonIO-0.1.43/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonIO'
 DESCRIPTION = 'Robert Common IO Library'
 URL = 'https://github.com/hun0423/RobertCommonIO'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.42'
-DATE = '2023-06-09'
+VERSION = '0.1.43'
+DATE = '2023-08-01'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

### Comparing `RobertCommonIO-0.1.42/tests/test_system/test_io/test.py` & `RobertCommonIO-0.1.43/tests/test_system/test_io/test.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/tests/test_system/test_io/test_data_storage.py` & `RobertCommonIO-0.1.43/tests/test_system/test_io/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/tests/test_system/test_io/test_email.py` & `RobertCommonIO-0.1.43/tests/test_system/test_io/test_email.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/tests/test_system/test_io/test_file.py` & `RobertCommonIO-0.1.43/tests/test_system/test_io/test_file.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/tests/test_system/test_io/test_ftp.py` & `RobertCommonIO-0.1.43/tests/test_system/test_io/test_ftp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/tests/test_system/test_io/test_license.py` & `RobertCommonIO-0.1.43/tests/test_system/test_io/test_license.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/tests/test_system/test_io/test_mongo.py` & `RobertCommonIO-0.1.43/tests/test_system/test_io/test_mongo.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/tests/test_system/test_io/test_mqtt.py` & `RobertCommonIO-0.1.43/tests/test_system/test_io/test_mqtt.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/tests/test_system/test_io/test_oracle.py` & `RobertCommonIO-0.1.43/tests/test_system/test_io/test_oracle.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/tests/test_system/test_io/test_rabbitmq.py` & `RobertCommonIO-0.1.43/tests/test_system/test_io/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/tests/test_system/test_io/test_socket.py` & `RobertCommonIO-0.1.43/tests/test_system/test_io/test_socket.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/tests/test_system/test_io/test_sqlalche.py` & `RobertCommonIO-0.1.43/tests/test_system/test_io/test_sqlalche.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.42/tests/test_system/test_io/test_transport.py` & `RobertCommonIO-0.1.43/tests/test_system/test_io/test_transport.py`

 * *Files identical despite different names*

