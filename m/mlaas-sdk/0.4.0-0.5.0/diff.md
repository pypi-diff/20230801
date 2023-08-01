# Comparing `tmp/mlaas_sdk-0.4.0.tar.gz` & `tmp/mlaas_sdk-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlaas_sdk-0.4.0.tar", max compression
+gzip compressed data, was "mlaas_sdk-0.5.0.tar", max compression
```

## Comparing `mlaas_sdk-0.4.0.tar` & `mlaas_sdk-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      303 2023-05-12 12:51:02.330001 mlaas_sdk-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-05-03 10:29:07.374531 mlaas_sdk-0.4.0/mlaas_sdk/__init__.py
--rw-r--r--   0        0        0      113 2023-05-03 10:29:07.374531 mlaas_sdk-0.4.0/mlaas_sdk/clients/__init__.py
--rw-r--r--   0        0        0      304 2023-05-12 10:15:48.493111 mlaas_sdk-0.4.0/mlaas_sdk/clients/base.py
--rw-r--r--   0        0        0     1922 2023-05-12 10:22:06.149622 mlaas_sdk-0.4.0/mlaas_sdk/clients/blockchain.py
--rw-r--r--   0        0        0     2614 2023-05-12 12:41:44.711426 mlaas_sdk-0.4.0/mlaas_sdk/clients/sharing.py
--rw-r--r--   0        0        0      487 2023-05-12 10:22:31.139642 mlaas_sdk-0.4.0/mlaas_sdk/clients/training.py
--rw-r--r--   0        0        0      105 2023-05-03 10:29:07.374531 mlaas_sdk-0.4.0/mlaas_sdk/exceptions/MLaaSException.py
--rw-r--r--   0        0        0      107 2023-05-03 10:29:07.374531 mlaas_sdk-0.4.0/mlaas_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0     1241 2023-05-03 10:29:07.374531 mlaas_sdk-0.4.0/mlaas_sdk/exceptions/blockchain.py
--rw-r--r--   0        0        0     1475 2023-05-03 10:29:07.374531 mlaas_sdk-0.4.0/mlaas_sdk/exceptions/sharing.py
--rw-r--r--   0        0        0      724 2023-05-03 10:29:07.374531 mlaas_sdk-0.4.0/mlaas_sdk/exceptions/training.py
--rw-r--r--   0        0        0      205 2023-05-03 10:29:07.374531 mlaas_sdk-0.4.0/mlaas_sdk/models/DatasetContract.py
--rw-r--r--   0        0        0      385 2023-05-03 10:29:07.374531 mlaas_sdk-0.4.0/mlaas_sdk/models/ModelContract.py
--rw-r--r--   0        0        0      175 2023-05-03 10:29:07.374531 mlaas_sdk-0.4.0/mlaas_sdk/models/ModelContractUnverified.py
--rw-r--r--   0        0        0      147 2023-05-03 10:29:07.374531 mlaas_sdk-0.4.0/mlaas_sdk/models/__init__.py
--rw-r--r--   0        0        0      331 2023-05-12 10:02:36.337756 mlaas_sdk-0.4.0/mlaas_sdk/utils.py
--rw-r--r--   0        0        0      762 2023-05-12 12:54:08.614569 mlaas_sdk-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 mlaas_sdk-0.4.0/PKG-INFO
+-rwxr-xr-x   0        0        0      303 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/README.md
+-rwxr-xr-x   0        0        0        0 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/__init__.py
+-rwxr-xr-x   0        0        0     1681 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/clients/__init__.py
+-rwxr-xr-x   0        0        0     1894 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/clients/base.py
+-rwxr-xr-x   0        0        0     3551 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/clients/blockchain.py
+-rwxr-xr-x   0        0        0     4185 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/clients/sharing.py
+-rwxr-xr-x   0        0        0     2058 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/clients/training.py
+-rwxr-xr-x   0        0        0     1676 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/exceptions/MLaaSException.py
+-rwxr-xr-x   0        0        0     1678 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/exceptions/__init__.py
+-rwxr-xr-x   0        0        0     2812 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/exceptions/blockchain.py
+-rwxr-xr-x   0        0        0     3046 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/exceptions/sharing.py
+-rwxr-xr-x   0        0        0     2295 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/exceptions/training.py
+-rwxr-xr-x   0        0        0     1776 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/models/DatasetContract.py
+-rwxr-xr-x   0        0        0     1935 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/models/ModelContract.py
+-rwxr-xr-x   0        0        0     1746 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/models/ModelContractUnverified.py
+-rwxr-xr-x   0        0        0     1718 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/models/__init__.py
+-rwxr-xr-x   0        0        0     1960 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/utils.py
+-rwxr-xr-x   0        0        0      523 2023-08-01 09:56:56.917100 mlaas_sdk-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 mlaas_sdk-0.5.0/PKG-INFO
```

### Comparing `mlaas_sdk-0.4.0/PKG-INFO` & `mlaas_sdk-0.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: mlaas-sdk
-Version: 0.4.0
+Version: 0.5.0
 Summary: IoT-NGIN MLaaS Polyglot Model Sharing Framework Python SDK
-Home-page: https://gitlab.com/h2020-iot-ngin/enhancing_iot_intelligence/t3_4/ml-model-sharing
 License: MIT
 Keywords: iot-ngin
 Author: ivanvmoreno
 Author-email: ivan@ivan.build
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
-Project-URL: Repository, https://gitlab.com/h2020-iot-ngin/enhancing_iot_intelligence/t3_4/ml-model-sharing
 Description-Content-Type: text/markdown
 
 # IoT-NGIN — MLaaS Polyglot Model Sharing Framework Python SDK
 Python SDK for interfacing with the IoT-NGIN MLaaS Polyglot Model Sharing Framework's services.
 
 More information available at the [project's repository](https://gitlab.com/h2020-iot-ngin/enhancing_iot_intelligence/t3_4/ml-model-sharing).
```

