# Comparing `tmp/boto3-helpers-1.4.0.tar.gz` & `tmp/boto3-helpers-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boto3-helpers-1.4.0.tar", last modified: Mon May 15 16:15:33 2023, max compression
+gzip compressed data, was "boto3-helpers-2.0.0.tar", last modified: Tue Aug  1 15:33:00 2023, max compression
```

## Comparing `boto3-helpers-1.4.0.tar` & `boto3-helpers-2.0.0.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2023-05-15 16:15:33.809904 boto3-helpers-1.4.0/
--rw-r--r--   0 bo.bayles   (501) staff       (20)    10174 2022-08-24 20:40:12.000000 boto3-helpers-1.4.0/LICENSE
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2578 2023-05-15 16:15:33.810172 boto3-helpers-1.4.0/PKG-INFO
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2099 2022-09-22 19:00:18.000000 boto3-helpers-1.4.0/README.rst
-drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2023-05-15 16:15:33.790717 boto3-helpers-1.4.0/boto3_helpers/
--rw-r--r--   0 bo.bayles   (501) staff       (20)        0 2022-12-15 15:18:48.000000 boto3-helpers-1.4.0/boto3_helpers/__init__.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     3851 2022-09-22 21:23:05.000000 boto3-helpers-1.4.0/boto3_helpers/arn.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     1792 2022-09-22 19:00:18.000000 boto3-helpers-1.4.0/boto3_helpers/awslambda.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     3217 2022-09-23 13:50:11.000000 boto3-helpers-1.4.0/boto3_helpers/cloudwatch.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     4713 2023-05-15 15:59:52.000000 boto3-helpers-1.4.0/boto3_helpers/dynamodb.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     6306 2023-01-11 18:57:17.000000 boto3-helpers-1.4.0/boto3_helpers/events.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     1810 2022-09-22 19:00:18.000000 boto3-helpers-1.4.0/boto3_helpers/mediatailor.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2213 2023-05-15 15:59:52.000000 boto3-helpers-1.4.0/boto3_helpers/pagination.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2861 2022-10-17 19:48:22.000000 boto3-helpers-1.4.0/boto3_helpers/s3.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     3271 2023-04-06 15:28:10.000000 boto3-helpers-1.4.0/boto3_helpers/signed_requests.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     7087 2022-09-23 13:50:11.000000 boto3-helpers-1.4.0/boto3_helpers/sqs.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     4469 2022-09-01 20:24:17.000000 boto3-helpers-1.4.0/boto3_helpers/sts.py
-drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2023-05-15 16:15:33.795251 boto3-helpers-1.4.0/boto3_helpers.egg-info/
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2578 2023-05-15 16:15:33.000000 boto3-helpers-1.4.0/boto3_helpers.egg-info/PKG-INFO
--rw-r--r--   0 bo.bayles   (501) staff       (20)      785 2023-05-15 16:15:33.000000 boto3-helpers-1.4.0/boto3_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 bo.bayles   (501) staff       (20)        1 2023-05-15 16:15:33.000000 boto3-helpers-1.4.0/boto3_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 bo.bayles   (501) staff       (20)       15 2023-05-15 16:15:33.000000 boto3-helpers-1.4.0/boto3_helpers.egg-info/requires.txt
--rw-r--r--   0 bo.bayles   (501) staff       (20)       14 2023-05-15 16:15:33.000000 boto3-helpers-1.4.0/boto3_helpers.egg-info/top_level.txt
--rw-r--r--   0 bo.bayles   (501) staff       (20)      171 2022-09-01 20:18:16.000000 boto3-helpers-1.4.0/pyproject.toml
--rw-r--r--   0 bo.bayles   (501) staff       (20)      689 2023-05-15 16:15:33.811583 boto3-helpers-1.4.0/setup.cfg
--rw-r--r--   0 bo.bayles   (501) staff       (20)       38 2022-09-01 20:23:34.000000 boto3-helpers-1.4.0/setup.py
-drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2023-05-15 16:15:33.808873 boto3-helpers-1.4.0/tests/
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2075 2022-09-22 21:23:05.000000 boto3-helpers-1.4.0/tests/test_arn.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     1806 2022-09-22 19:00:18.000000 boto3-helpers-1.4.0/tests/test_awslambda.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     3749 2022-09-23 13:50:11.000000 boto3-helpers-1.4.0/tests/test_cloudwatch.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     5664 2023-05-15 15:59:52.000000 boto3-helpers-1.4.0/tests/test_dynamodb.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     9813 2022-09-22 19:00:18.000000 boto3-helpers-1.4.0/tests/test_events.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     3468 2022-09-01 21:00:54.000000 boto3-helpers-1.4.0/tests/test_mediatailor.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2200 2023-04-28 15:58:17.000000 boto3-helpers-1.4.0/tests/test_pagination.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     2369 2022-10-17 19:48:22.000000 boto3-helpers-1.4.0/tests/test_s3.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     1997 2023-04-06 15:28:10.000000 boto3-helpers-1.4.0/tests/test_signed_requests.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     6180 2022-09-22 19:00:18.000000 boto3-helpers-1.4.0/tests/test_sqs.py
--rw-r--r--   0 bo.bayles   (501) staff       (20)     4106 2022-08-25 21:06:36.000000 boto3-helpers-1.4.0/tests/test_sts.py
+drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2023-08-01 15:33:00.746611 boto3-helpers-2.0.0/
+-rw-r--r--   0 bo.bayles   (501) staff       (20)    10174 2022-08-24 20:40:12.000000 boto3-helpers-2.0.0/LICENSE
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2578 2023-08-01 15:33:00.746884 boto3-helpers-2.0.0/PKG-INFO
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2099 2022-09-22 19:00:18.000000 boto3-helpers-2.0.0/README.rst
+drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2023-08-01 15:33:00.726453 boto3-helpers-2.0.0/boto3_helpers/
+-rw-r--r--   0 bo.bayles   (501) staff       (20)        0 2022-12-15 15:18:48.000000 boto3-helpers-2.0.0/boto3_helpers/__init__.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     3851 2022-09-22 21:23:05.000000 boto3-helpers-2.0.0/boto3_helpers/arn.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     1792 2022-09-22 19:00:18.000000 boto3-helpers-2.0.0/boto3_helpers/awslambda.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     3217 2022-09-23 13:50:11.000000 boto3-helpers-2.0.0/boto3_helpers/cloudwatch.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     4713 2023-05-15 15:59:52.000000 boto3-helpers-2.0.0/boto3_helpers/dynamodb.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     6306 2023-01-11 18:57:17.000000 boto3-helpers-2.0.0/boto3_helpers/events.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2518 2023-08-01 15:31:17.000000 boto3-helpers-2.0.0/boto3_helpers/medialive.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     1810 2023-08-01 15:31:17.000000 boto3-helpers-2.0.0/boto3_helpers/mediatailor.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2213 2023-05-15 15:59:52.000000 boto3-helpers-2.0.0/boto3_helpers/pagination.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2861 2022-10-17 19:48:22.000000 boto3-helpers-2.0.0/boto3_helpers/s3.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     3271 2023-04-06 15:28:10.000000 boto3-helpers-2.0.0/boto3_helpers/signed_requests.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     7087 2022-09-23 13:50:11.000000 boto3-helpers-2.0.0/boto3_helpers/sqs.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     4469 2022-09-01 20:24:17.000000 boto3-helpers-2.0.0/boto3_helpers/sts.py
+drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2023-08-01 15:33:00.730908 boto3-helpers-2.0.0/boto3_helpers.egg-info/
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2578 2023-08-01 15:33:00.000000 boto3-helpers-2.0.0/boto3_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 bo.bayles   (501) staff       (20)      836 2023-08-01 15:33:00.000000 boto3-helpers-2.0.0/boto3_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 bo.bayles   (501) staff       (20)        1 2023-08-01 15:33:00.000000 boto3-helpers-2.0.0/boto3_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 bo.bayles   (501) staff       (20)       15 2023-08-01 15:33:00.000000 boto3-helpers-2.0.0/boto3_helpers.egg-info/requires.txt
+-rw-r--r--   0 bo.bayles   (501) staff       (20)       14 2023-08-01 15:33:00.000000 boto3-helpers-2.0.0/boto3_helpers.egg-info/top_level.txt
+-rw-r--r--   0 bo.bayles   (501) staff       (20)      171 2022-09-01 20:18:16.000000 boto3-helpers-2.0.0/pyproject.toml
+-rw-r--r--   0 bo.bayles   (501) staff       (20)      689 2023-08-01 15:33:00.748178 boto3-helpers-2.0.0/setup.cfg
+-rw-r--r--   0 bo.bayles   (501) staff       (20)       38 2022-09-01 20:23:34.000000 boto3-helpers-2.0.0/setup.py
+drwxr-xr-x   0 bo.bayles   (501) staff       (20)        0 2023-08-01 15:33:00.745721 boto3-helpers-2.0.0/tests/
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2075 2022-09-22 21:23:05.000000 boto3-helpers-2.0.0/tests/test_arn.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     1806 2022-09-22 19:00:18.000000 boto3-helpers-2.0.0/tests/test_awslambda.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     3749 2022-09-23 13:50:11.000000 boto3-helpers-2.0.0/tests/test_cloudwatch.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     5664 2023-05-15 15:59:52.000000 boto3-helpers-2.0.0/tests/test_dynamodb.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     9813 2022-09-22 19:00:18.000000 boto3-helpers-2.0.0/tests/test_events.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     4246 2023-08-01 15:31:17.000000 boto3-helpers-2.0.0/tests/test_medialive.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     3468 2022-09-01 21:00:54.000000 boto3-helpers-2.0.0/tests/test_mediatailor.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2200 2023-04-28 15:58:17.000000 boto3-helpers-2.0.0/tests/test_pagination.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     2369 2022-10-17 19:48:22.000000 boto3-helpers-2.0.0/tests/test_s3.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     1997 2023-04-06 15:28:10.000000 boto3-helpers-2.0.0/tests/test_signed_requests.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     6180 2022-09-22 19:00:18.000000 boto3-helpers-2.0.0/tests/test_sqs.py
+-rw-r--r--   0 bo.bayles   (501) staff       (20)     4106 2022-08-25 21:06:36.000000 boto3-helpers-2.0.0/tests/test_sts.py
```

### Comparing `boto3-helpers-1.4.0/LICENSE` & `boto3-helpers-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/PKG-INFO` & `boto3-helpers-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: boto3-helpers
-Version: 1.4.0
+Version: 2.0.0
 Summary: Helper utilities for boto3
 Author: Bo Bayles
 Author-email: bo.bayles@wurl.com
 License: Apache 2.0
 Project-URL: homepage, https://github.com/openwurl/boto3-helpers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 boto3-helpers
 =============
 
 ``boto3_helpers`` is a Python library that aims to provide a smoother interface for
```

### Comparing `boto3-helpers-1.4.0/README.rst` & `boto3-helpers-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/boto3_helpers/arn.py` & `boto3-helpers-2.0.0/boto3_helpers/arn.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/boto3_helpers/awslambda.py` & `boto3-helpers-2.0.0/boto3_helpers/awslambda.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/boto3_helpers/cloudwatch.py` & `boto3-helpers-2.0.0/boto3_helpers/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/boto3_helpers/dynamodb.py` & `boto3-helpers-2.0.0/boto3_helpers/dynamodb.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/boto3_helpers/events.py` & `boto3-helpers-2.0.0/boto3_helpers/events.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/boto3_helpers/mediatailor.py` & `boto3-helpers-2.0.0/boto3_helpers/mediatailor.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from boto3 import client as boto3_client
 
 
 def update_playback_configuration(config_name, emt_client=None, **config_kwargs):
     """Do a partial update of a MediaTailor configuration and return the result:
 
+    * *config_name* is the name of the playback configuration that will be updated.
     * *emt_client* is a ``boto3.client('mediatailor')`` instance. If not given, is
       created with ``boto3.client('mediatailor')``.
-    * *config_name* is the name of the playback configuration that will be updated.
     * *config_kwargs* are passed directly to the ``put_playback_configuration`` method.
 
     Usage:
 
     .. code-block:: python
 
         from boto3_helpers.mediatailor import update_playback_configuration
```

### Comparing `boto3-helpers-1.4.0/boto3_helpers/pagination.py` & `boto3-helpers-2.0.0/boto3_helpers/pagination.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/boto3_helpers/s3.py` & `boto3-helpers-2.0.0/boto3_helpers/s3.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/boto3_helpers/signed_requests.py` & `boto3-helpers-2.0.0/boto3_helpers/signed_requests.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/boto3_helpers/sqs.py` & `boto3-helpers-2.0.0/boto3_helpers/sqs.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/boto3_helpers/sts.py` & `boto3-helpers-2.0.0/boto3_helpers/sts.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/boto3_helpers.egg-info/PKG-INFO` & `boto3-helpers-2.0.0/boto3_helpers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: boto3-helpers
-Version: 1.4.0
+Version: 2.0.0
 Summary: Helper utilities for boto3
 Author: Bo Bayles
 Author-email: bo.bayles@wurl.com
 License: Apache 2.0
 Project-URL: homepage, https://github.com/openwurl/boto3-helpers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 boto3-helpers
 =============
 
 ``boto3_helpers`` is a Python library that aims to provide a smoother interface for
```

### Comparing `boto3-helpers-1.4.0/boto3_helpers.egg-info/SOURCES.txt` & `boto3-helpers-2.0.0/boto3_helpers.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.py
 boto3_helpers/__init__.py
 boto3_helpers/arn.py
 boto3_helpers/awslambda.py
 boto3_helpers/cloudwatch.py
 boto3_helpers/dynamodb.py
 boto3_helpers/events.py
+boto3_helpers/medialive.py
 boto3_helpers/mediatailor.py
 boto3_helpers/pagination.py
 boto3_helpers/s3.py
 boto3_helpers/signed_requests.py
 boto3_helpers/sqs.py
 boto3_helpers/sts.py
 boto3_helpers.egg-info/PKG-INFO
@@ -21,13 +22,14 @@
 boto3_helpers.egg-info/requires.txt
 boto3_helpers.egg-info/top_level.txt
 tests/test_arn.py
 tests/test_awslambda.py
 tests/test_cloudwatch.py
 tests/test_dynamodb.py
 tests/test_events.py
+tests/test_medialive.py
 tests/test_mediatailor.py
 tests/test_pagination.py
 tests/test_s3.py
 tests/test_signed_requests.py
 tests/test_sqs.py
 tests/test_sts.py
```

### Comparing `boto3-helpers-1.4.0/setup.cfg` & `boto3-helpers-2.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = boto3-helpers
-version = 1.4.0
+version = 2.0.0
 description = Helper utilities for boto3
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Bo Bayles
 author_email = bo.bayles@wurl.com
 license = Apache 2.0
 license_files = 
@@ -14,15 +14,15 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 project_urls = 
 	homepage = https://github.com/openwurl/boto3-helpers
 
 [options]
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.8
 install_requires = 
 	boto3
 	botocore
 
 [options.packages.find]
 exclude = 
 	tests
```

### Comparing `boto3-helpers-1.4.0/tests/test_arn.py` & `boto3-helpers-2.0.0/tests/test_arn.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/tests/test_awslambda.py` & `boto3-helpers-2.0.0/tests/test_awslambda.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/tests/test_cloudwatch.py` & `boto3-helpers-2.0.0/tests/test_cloudwatch.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/tests/test_dynamodb.py` & `boto3-helpers-2.0.0/tests/test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/tests/test_events.py` & `boto3-helpers-2.0.0/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/tests/test_mediatailor.py` & `boto3-helpers-2.0.0/tests/test_mediatailor.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/tests/test_pagination.py` & `boto3-helpers-2.0.0/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/tests/test_s3.py` & `boto3-helpers-2.0.0/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/tests/test_signed_requests.py` & `boto3-helpers-2.0.0/tests/test_signed_requests.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/tests/test_sqs.py` & `boto3-helpers-2.0.0/tests/test_sqs.py`

 * *Files identical despite different names*

### Comparing `boto3-helpers-1.4.0/tests/test_sts.py` & `boto3-helpers-2.0.0/tests/test_sts.py`

 * *Files identical despite different names*

