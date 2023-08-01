# Comparing `tmp/byteplus-rec-1.0.4.tar.gz` & `tmp/byteplus-rec-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byteplus-rec-1.0.4.tar", last modified: Thu Oct 27 02:31:23 2022, max compression
+gzip compressed data, was "byteplus-rec-1.0.5.tar", last modified: Tue Aug  1 03:08:10 2023, max compression
```

## Comparing `byteplus-rec-1.0.4.tar` & `byteplus-rec-1.0.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2022-10-27 02:31:23.000179 byteplus-rec-1.0.4/
--rw-r--r--   0 bytedance   (502) staff       (20)       24 2022-03-02 09:15:20.000000 byteplus-rec-1.0.4/MANIFEST.in
--rw-r--r--   0 bytedance   (502) staff       (20)     4183 2022-10-27 02:31:22.999783 byteplus-rec-1.0.4/PKG-INFO
--rw-r--r--   0 bytedance   (502) staff       (20)     3079 2022-10-26 03:43:28.000000 byteplus-rec-1.0.4/README.md
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2022-10-27 02:31:22.972913 byteplus-rec-1.0.4/byteplus_rec/
--rw-r--r--   0 bytedance   (502) staff       (20)        0 2022-03-02 09:15:20.000000 byteplus-rec-1.0.4/byteplus_rec/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)      275 2022-10-26 10:53:35.000000 byteplus-rec-1.0.4/byteplus_rec/__version__.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2022-10-27 02:31:22.978697 byteplus-rec-1.0.4/byteplus_rec/content/
--rw-r--r--   0 bytedance   (502) staff       (20)        0 2022-08-18 02:54:08.000000 byteplus-rec-1.0.4/byteplus_rec/content/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)     5250 2022-10-26 03:03:13.000000 byteplus-rec-1.0.4/byteplus_rec/content/abstract_client.py
--rw-r--r--   0 bytedance   (502) staff       (20)     1719 2022-10-26 03:06:37.000000 byteplus-rec-1.0.4/byteplus_rec/content/constant.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6780 2022-10-26 03:08:09.000000 byteplus-rec-1.0.4/byteplus_rec/content/content_client.py
--rw-r--r--   0 bytedance   (502) staff       (20)     3761 2022-08-18 03:32:00.000000 byteplus-rec-1.0.4/byteplus_rec/content/content_client_builder.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2022-10-27 02:31:22.981837 byteplus-rec-1.0.4/byteplus_rec/content/example/
--rw-r--r--   0 bytedance   (502) staff       (20)        0 2022-08-18 02:54:26.000000 byteplus-rec-1.0.4/byteplus_rec/content/example/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)    17579 2022-10-26 08:57:13.000000 byteplus-rec-1.0.4/byteplus_rec/content/example/main.py
--rw-r--r--   0 bytedance   (502) staff       (20)     7471 2022-10-26 03:26:24.000000 byteplus-rec-1.0.4/byteplus_rec/content/example/mock_helper.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2022-10-27 02:31:22.983850 byteplus-rec-1.0.4/byteplus_rec/content/protocol/
--rw-r--r--   0 bytedance   (502) staff       (20)      284 2022-10-26 03:02:25.000000 byteplus-rec-1.0.4/byteplus_rec/content/protocol/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)    21761 2022-10-26 02:54:06.000000 byteplus-rec-1.0.4/byteplus_rec/content/protocol/byteplus_saas_content_pb2.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2022-10-27 02:31:22.985728 byteplus-rec-1.0.4/byteplus_rec/region/
--rw-r--r--   0 bytedance   (502) staff       (20)        0 2022-04-14 04:57:22.000000 byteplus-rec-1.0.4/byteplus_rec/region/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)      444 2022-04-14 04:57:22.000000 byteplus-rec-1.0.4/byteplus_rec/region/region.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2022-10-27 02:31:22.990373 byteplus-rec-1.0.4/byteplus_rec/retail/
--rw-r--r--   0 bytedance   (502) staff       (20)        0 2022-03-02 09:15:20.000000 byteplus-rec-1.0.4/byteplus_rec/retail/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)     5319 2022-04-14 04:57:22.000000 byteplus-rec-1.0.4/byteplus_rec/retail/abstract_client.py
--rw-r--r--   0 bytedance   (502) staff       (20)     1707 2022-08-18 03:07:43.000000 byteplus-rec-1.0.4/byteplus_rec/retail/constant.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2022-10-27 02:31:22.995664 byteplus-rec-1.0.4/byteplus_rec/retail/example/
--rw-r--r--   0 bytedance   (502) staff       (20)        0 2022-03-02 09:15:20.000000 byteplus-rec-1.0.4/byteplus_rec/retail/example/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)    17490 2022-10-26 09:16:24.000000 byteplus-rec-1.0.4/byteplus_rec/retail/example/main.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6432 2022-04-14 04:57:22.000000 byteplus-rec-1.0.4/byteplus_rec/retail/example/mock_helper.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2022-10-27 02:31:22.998372 byteplus-rec-1.0.4/byteplus_rec/retail/protocol/
--rw-r--r--   0 bytedance   (502) staff       (20)      252 2022-04-14 04:57:22.000000 byteplus-rec-1.0.4/byteplus_rec/retail/protocol/__init__.py
--rw-r--r--   0 bytedance   (502) staff       (20)    25289 2022-10-26 02:53:01.000000 byteplus-rec-1.0.4/byteplus_rec/retail/protocol/byteplus_saas_retail_pb2.py
--rw-r--r--   0 bytedance   (502) staff       (20)     6778 2022-08-18 03:08:45.000000 byteplus-rec-1.0.4/byteplus_rec/retail/retail_client.py
--rw-r--r--   0 bytedance   (502) staff       (20)     3759 2022-08-18 03:30:04.000000 byteplus-rec-1.0.4/byteplus_rec/retail/retail_client_builder.py
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2022-10-27 02:31:22.975189 byteplus-rec-1.0.4/byteplus_rec.egg-info/
--rw-r--r--   0 bytedance   (502) staff       (20)     4183 2022-10-27 02:31:22.000000 byteplus-rec-1.0.4/byteplus_rec.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (502) staff       (20)     1158 2022-10-27 02:31:22.000000 byteplus-rec-1.0.4/byteplus_rec.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (502) staff       (20)        1 2022-10-27 02:31:22.000000 byteplus-rec-1.0.4/byteplus_rec.egg-info/dependency_links.txt
--rw-r--r--   0 bytedance   (502) staff       (20)       25 2022-10-27 02:31:22.000000 byteplus-rec-1.0.4/byteplus_rec.egg-info/requires.txt
--rw-r--r--   0 bytedance   (502) staff       (20)       13 2022-10-27 02:31:22.000000 byteplus-rec-1.0.4/byteplus_rec.egg-info/top_level.txt
--rw-r--r--   0 bytedance   (502) staff       (20)       24 2022-10-26 07:24:44.000000 byteplus-rec-1.0.4/requirements.txt
--rw-r--r--   0 bytedance   (502) staff       (20)       38 2022-10-27 02:31:23.000305 byteplus-rec-1.0.4/setup.cfg
--rw-r--r--   0 bytedance   (502) staff       (20)     1908 2022-03-02 09:15:20.000000 byteplus-rec-1.0.4/setup.py
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-08-01 03:08:10.239785 byteplus-rec-1.0.5/
+-rw-r--r--   0 bytedance   (502) staff       (20)       24 2022-03-02 09:15:20.000000 byteplus-rec-1.0.5/MANIFEST.in
+-rw-r--r--   0 bytedance   (502) staff       (20)     4183 2023-08-01 03:08:10.239365 byteplus-rec-1.0.5/PKG-INFO
+-rw-r--r--   0 bytedance   (502) staff       (20)     3079 2023-06-16 03:09:38.000000 byteplus-rec-1.0.5/README.md
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-08-01 03:08:10.207776 byteplus-rec-1.0.5/byteplus_rec/
+-rw-r--r--   0 bytedance   (502) staff       (20)        0 2022-03-02 09:15:20.000000 byteplus-rec-1.0.5/byteplus_rec/__init__.py
+-rw-r--r--   0 bytedance   (502) staff       (20)      275 2023-08-01 03:07:02.000000 byteplus-rec-1.0.5/byteplus_rec/__version__.py
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-08-01 03:08:10.220787 byteplus-rec-1.0.5/byteplus_rec/content/
+-rw-r--r--   0 bytedance   (502) staff       (20)        0 2023-06-16 03:09:38.000000 byteplus-rec-1.0.5/byteplus_rec/content/__init__.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     5250 2023-06-16 03:09:38.000000 byteplus-rec-1.0.5/byteplus_rec/content/abstract_client.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     1719 2023-06-16 03:09:38.000000 byteplus-rec-1.0.5/byteplus_rec/content/constant.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     6780 2023-06-16 03:09:38.000000 byteplus-rec-1.0.5/byteplus_rec/content/content_client.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     3761 2023-06-16 03:09:38.000000 byteplus-rec-1.0.5/byteplus_rec/content/content_client_builder.py
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-08-01 03:08:10.224291 byteplus-rec-1.0.5/byteplus_rec/content/example/
+-rw-r--r--   0 bytedance   (502) staff       (20)        0 2023-06-16 03:09:38.000000 byteplus-rec-1.0.5/byteplus_rec/content/example/__init__.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    17857 2023-06-28 07:22:27.000000 byteplus-rec-1.0.5/byteplus_rec/content/example/main.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     4235 2023-08-01 03:05:54.000000 byteplus-rec-1.0.5/byteplus_rec/content/example/mock_helper.py
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-08-01 03:08:10.225923 byteplus-rec-1.0.5/byteplus_rec/content/protocol/
+-rw-r--r--   0 bytedance   (502) staff       (20)      387 2023-08-01 03:05:54.000000 byteplus-rec-1.0.5/byteplus_rec/content/protocol/__init__.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    40005 2023-08-01 03:05:54.000000 byteplus-rec-1.0.5/byteplus_rec/content/protocol/byteplus_saas_content_pb2.py
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-08-01 03:08:10.228181 byteplus-rec-1.0.5/byteplus_rec/region/
+-rw-r--r--   0 bytedance   (502) staff       (20)        0 2022-04-14 04:57:22.000000 byteplus-rec-1.0.5/byteplus_rec/region/__init__.py
+-rw-r--r--   0 bytedance   (502) staff       (20)      444 2022-04-14 04:57:22.000000 byteplus-rec-1.0.5/byteplus_rec/region/region.py
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-08-01 03:08:10.233094 byteplus-rec-1.0.5/byteplus_rec/retail/
+-rw-r--r--   0 bytedance   (502) staff       (20)        0 2022-03-02 09:15:20.000000 byteplus-rec-1.0.5/byteplus_rec/retail/__init__.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     5319 2022-04-14 04:57:22.000000 byteplus-rec-1.0.5/byteplus_rec/retail/abstract_client.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     1707 2023-06-16 03:09:38.000000 byteplus-rec-1.0.5/byteplus_rec/retail/constant.py
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-08-01 03:08:10.237343 byteplus-rec-1.0.5/byteplus_rec/retail/example/
+-rw-r--r--   0 bytedance   (502) staff       (20)        0 2022-03-02 09:15:20.000000 byteplus-rec-1.0.5/byteplus_rec/retail/example/__init__.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    17768 2023-06-28 07:22:03.000000 byteplus-rec-1.0.5/byteplus_rec/retail/example/main.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     3973 2023-08-01 03:05:54.000000 byteplus-rec-1.0.5/byteplus_rec/retail/example/mock_helper.py
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-08-01 03:08:10.238649 byteplus-rec-1.0.5/byteplus_rec/retail/protocol/
+-rw-r--r--   0 bytedance   (502) staff       (20)      355 2023-08-01 03:05:54.000000 byteplus-rec-1.0.5/byteplus_rec/retail/protocol/__init__.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    39767 2023-08-01 03:05:54.000000 byteplus-rec-1.0.5/byteplus_rec/retail/protocol/byteplus_saas_retail_pb2.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     6778 2023-06-16 03:09:38.000000 byteplus-rec-1.0.5/byteplus_rec/retail/retail_client.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     3759 2023-06-16 03:09:38.000000 byteplus-rec-1.0.5/byteplus_rec/retail/retail_client_builder.py
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-08-01 03:08:10.213178 byteplus-rec-1.0.5/byteplus_rec.egg-info/
+-rw-r--r--   0 bytedance   (502) staff       (20)     4183 2023-08-01 03:08:09.000000 byteplus-rec-1.0.5/byteplus_rec.egg-info/PKG-INFO
+-rw-r--r--   0 bytedance   (502) staff       (20)     1158 2023-08-01 03:08:09.000000 byteplus-rec-1.0.5/byteplus_rec.egg-info/SOURCES.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)        1 2023-08-01 03:08:09.000000 byteplus-rec-1.0.5/byteplus_rec.egg-info/dependency_links.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)       25 2023-08-01 03:08:09.000000 byteplus-rec-1.0.5/byteplus_rec.egg-info/requires.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)       13 2023-08-01 03:08:09.000000 byteplus-rec-1.0.5/byteplus_rec.egg-info/top_level.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)       24 2023-06-16 03:09:38.000000 byteplus-rec-1.0.5/requirements.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)       38 2023-08-01 03:08:10.239934 byteplus-rec-1.0.5/setup.cfg
+-rw-r--r--   0 bytedance   (502) staff       (20)     1908 2022-03-02 09:15:20.000000 byteplus-rec-1.0.5/setup.py
```

### Comparing `byteplus-rec-1.0.4/PKG-INFO` & `byteplus-rec-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byteplus-rec
-Version: 1.0.4
+Version: 1.0.5
 Summary: SDK for byteplus rec
 Home-page: https://github.com/byteplus-sdk
 Author: Guowei Lei
 Author-email: leiguowei@bytedance.com
 License: Apache 2.0
 Project-URL: Documentation, https://docs.byteplus.com
 Project-URL: Source, https://github.com/byteplus-sdk/byteplus-sdk-python-rec
```

### Comparing `byteplus-rec-1.0.4/README.md` & `byteplus-rec-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `byteplus-rec-1.0.4/byteplus_rec/content/abstract_client.py` & `byteplus-rec-1.0.5/byteplus_rec/content/abstract_client.py`

 * *Files identical despite different names*

### Comparing `byteplus-rec-1.0.4/byteplus_rec/content/constant.py` & `byteplus-rec-1.0.5/byteplus_rec/content/constant.py`

 * *Files identical despite different names*

### Comparing `byteplus-rec-1.0.4/byteplus_rec/content/content_client.py` & `byteplus-rec-1.0.5/byteplus_rec/content/content_client.py`

 * *Files identical despite different names*

### Comparing `byteplus-rec-1.0.4/byteplus_rec/content/content_client_builder.py` & `byteplus-rec-1.0.5/byteplus_rec/content/content_client_builder.py`

 * *Files identical despite different names*

### Comparing `byteplus-rec-1.0.4/byteplus_rec/content/example/main.py` & `byteplus-rec-1.0.5/byteplus_rec/content/example/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,17 @@
 # metrics_config: MetricsCfg = MetricsCfg(enable_metrics=True, enable_metrics_log=True, report_interval_seconds=15)
 #
 # try:
 #     client: Client = ClientBuilder() \
 #         .account_id("***********") \
 #         .region(Region.SG) \
 #         .project_id(PROJECT_ID) \
-#         .auth_ak("***********") \
-#         .auth_sk("***********") \
+#         .auth_ak("***********") \ # Access Key, used to generate request signature. Saas Standard projects should use.
+#         .auth_sk("***********") \ # Secure Key, used to generate request signature. Saas Standard projects should use.
+# #         .air_auth_token("***********") \ # The token of this project. Saas Premium projects should use.
 #         .keep_alive(True) \
 #         .caller_config(caller_config) \
 #         .metrics_config(metrics_config) \
 #         .build()
 # except BizException as clientE:
 #     log.error("fail to create byteplus rec client, msg:%s", clientE)
```

### Comparing `byteplus-rec-1.0.4/byteplus_rec/retail/abstract_client.py` & `byteplus-rec-1.0.5/byteplus_rec/retail/abstract_client.py`

 * *Files identical despite different names*

### Comparing `byteplus-rec-1.0.4/byteplus_rec/retail/constant.py` & `byteplus-rec-1.0.5/byteplus_rec/retail/constant.py`

 * *Files identical despite different names*

### Comparing `byteplus-rec-1.0.4/byteplus_rec/retail/example/main.py` & `byteplus-rec-1.0.5/byteplus_rec/retail/example/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,17 @@
 # metrics_config: MetricsCfg = MetricsCfg(enable_metrics=True, enable_metrics_log=True, report_interval_seconds=15)
 #
 # try:
 #     client: Client = ClientBuilder() \
 #         .account_id("***********") \
 #         .region(Region.SG) \
 #         .project_id(PROJECT_ID) \
-#         .auth_ak("***********") \
-#         .auth_sk("***********") \
+#         .auth_ak("***********") \ # Access Key, used to generate request signature. Saas Standard projects should use.
+#         .auth_sk("***********") \ # Secure Key, used to generate request signature. Saas Standard projects should use.
+# #         .air_auth_token("***********") \ # The token of this project. Saas Premium projects should use.
 #         .keep_alive(True) \
 #         .caller_config(caller_config) \
 #         .metrics_config(metrics_config) \
 #         .build()
 # except BizException as clientE:
 #     log.error("fail to create byteplus rec client, msg:%s", clientE)
```

### Comparing `byteplus-rec-1.0.4/byteplus_rec/retail/retail_client.py` & `byteplus-rec-1.0.5/byteplus_rec/retail/retail_client.py`

 * *Files identical despite different names*

### Comparing `byteplus-rec-1.0.4/byteplus_rec/retail/retail_client_builder.py` & `byteplus-rec-1.0.5/byteplus_rec/retail/retail_client_builder.py`

 * *Files identical despite different names*

### Comparing `byteplus-rec-1.0.4/byteplus_rec.egg-info/PKG-INFO` & `byteplus-rec-1.0.5/byteplus_rec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byteplus-rec
-Version: 1.0.4
+Version: 1.0.5
 Summary: SDK for byteplus rec
 Home-page: https://github.com/byteplus-sdk
 Author: Guowei Lei
 Author-email: leiguowei@bytedance.com
 License: Apache 2.0
 Project-URL: Documentation, https://docs.byteplus.com
 Project-URL: Source, https://github.com/byteplus-sdk/byteplus-sdk-python-rec
```

### Comparing `byteplus-rec-1.0.4/byteplus_rec.egg-info/SOURCES.txt` & `byteplus-rec-1.0.5/byteplus_rec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `byteplus-rec-1.0.4/setup.py` & `byteplus-rec-1.0.5/setup.py`

 * *Files identical despite different names*

