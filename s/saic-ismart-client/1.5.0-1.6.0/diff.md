# Comparing `tmp/saic_ismart_client-1.5.0.tar.gz` & `tmp/saic_ismart_client-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saic_ismart_client-1.5.0.tar", last modified: Thu Jul 27 13:59:51 2023, max compression
+gzip compressed data, was "saic_ismart_client-1.6.0.tar", last modified: Tue Aug  1 17:00:54 2023, max compression
```

## Comparing `saic_ismart_client-1.5.0.tar` & `saic_ismart_client-1.6.0.tar`

### file list

```diff
@@ -1,51 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.516771 saic_ismart_client-1.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.516771 saic_ismart_client-1.5.0/src/saic_ismart_client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.516771 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25362 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/common_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/message_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v1_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v1_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v1_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v2_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v2_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v2_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v3_0/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v3_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23497 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v3_0/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    44103 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/src/saic_ismart_client/saic_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/src/saic_ismart_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-27 13:59:51.000000 saic_ismart_client-1.5.0/src/saic_ismart_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-27 13:59:51.000000 saic_ismart_client-1.5.0/src/saic_ismart_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:59:51.000000 saic_ismart_client-1.5.0/src/saic_ismart_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-27 13:59:51.000000 saic_ismart_client-1.5.0/src/saic_ismart_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 13:59:51.000000 saic_ismart_client-1.5.0/src/saic_ismart_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:59:51.520772 saic_ismart_client-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/tests/test_Message_v1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/tests/test_Message_v2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/tests/test_Message_v3_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/tests/test_abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-07-27 13:59:41.000000 saic_ismart_client-1.5.0/tests/test_saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:00:54.595270 saic_ismart_client-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-01 17:00:54.595270 saic_ismart_client-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 17:00:54.595270 saic_ismart_client-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:00:54.591269 saic_ismart_client-1.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:00:54.591269 saic_ismart_client-1.6.0/src/saic_ismart_client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:00:54.591269 saic_ismart_client-1.6.0/src/saic_ismart_client/ASN.1_schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:00:54.595270 saic_ismart_client-1.6.0/src/saic_ismart_client/ASN.1_schema/v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:00:54.595270 saic_ismart_client-1.6.0/src/saic_ismart_client/ASN.1_schema/v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:00:54.595270 saic_ismart_client-1.6.0/src/saic_ismart_client/ASN.1_schema/v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25362 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/common_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/message_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:00:54.595270 saic_ismart_client-1.6.0/src/saic_ismart_client/ota_v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/ota_v1_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/ota_v1_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/ota_v1_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:00:54.595270 saic_ismart_client-1.6.0/src/saic_ismart_client/ota_v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/ota_v2_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/ota_v2_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/ota_v2_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:00:54.595270 saic_ismart_client-1.6.0/src/saic_ismart_client/ota_v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/ota_v3_0/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/ota_v3_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23497 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/ota_v3_0/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:00:54.595270 saic_ismart_client-1.6.0/src/saic_ismart_client/rest_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/rest_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/rest_v2/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/rest_v2/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44243 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/src/saic_ismart_client/saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:00:54.595270 saic_ismart_client-1.6.0/src/saic_ismart_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-01 17:00:54.000000 saic_ismart_client-1.6.0/src/saic_ismart_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-08-01 17:00:54.000000 saic_ismart_client-1.6.0/src/saic_ismart_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 17:00:54.000000 saic_ismart_client-1.6.0/src/saic_ismart_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 17:00:54.000000 saic_ismart_client-1.6.0/src/saic_ismart_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 17:00:54.000000 saic_ismart_client-1.6.0/src/saic_ismart_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:00:54.595270 saic_ismart_client-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/tests/test_Message_v1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/tests/test_Message_v2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/tests/test_Message_v3_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/tests/test_abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-08-01 17:00:41.000000 saic_ismart_client-1.6.0/tests/test_saic_api.py
```

### Comparing `saic_ismart_client-1.5.0/LICENSE` & `saic_ismart_client-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.5.0/PKG-INFO` & `saic_ismart_client-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic_ismart_client
-Version: 1.5.0
+Version: 1.6.0
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.5.0/README.md` & `saic_ismart_client-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.5.0/pyproject.toml` & `saic_ismart_client-1.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saic_ismart_client"
-version = "1.5.0"
+version = "1.6.0"
 authors = [
     { name = "Thomas Salm", email="saic-python-client@devtom.de"},
 ]
 dependencies = [
     "asn1tools >= 0.166.0",
     "requests >= 2.31.0",
     "urllib3 >= 2.0.3",
```

### Comparing `saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1` & `saic_ismart_client-1.6.0/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.6.0/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1` & `saic_ismart_client-1.6.0/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.6.0/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1` & `saic_ismart_client-1.6.0/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.5.0/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1` & `saic_ismart_client-1.6.0/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.5.0/src/saic_ismart_client/abrp_api.py` & `saic_ismart_client-1.6.0/src/saic_ismart_client/abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.5.0/src/saic_ismart_client/common_model.py` & `saic_ismart_client-1.6.0/src/saic_ismart_client/common_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.5.0/src/saic_ismart_client/message_decoder.py` & `saic_ismart_client-1.6.0/src/saic_ismart_client/message_decoder.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v1_1/Message.py` & `saic_ismart_client-1.6.0/src/saic_ismart_client/ota_v1_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v1_1/data_model.py` & `saic_ismart_client-1.6.0/src/saic_ismart_client/ota_v1_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v2_1/Message.py` & `saic_ismart_client-1.6.0/src/saic_ismart_client/ota_v2_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v2_1/data_model.py` & `saic_ismart_client-1.6.0/src/saic_ismart_client/ota_v2_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v3_0/Message.py` & `saic_ismart_client-1.6.0/src/saic_ismart_client/ota_v3_0/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.5.0/src/saic_ismart_client/ota_v3_0/data_model.py` & `saic_ismart_client-1.6.0/src/saic_ismart_client/ota_v3_0/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.5.0/src/saic_ismart_client/saic_api.py` & `saic_ismart_client-1.6.0/src/saic_ismart_client/saic_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 import urllib.parse
 from typing import cast
 
 import requests as requests
 
 from saic_ismart_client.common_model import AbstractMessage, AbstractMessageBody, Header, MessageBodyV2, MessageV2, \
     ScheduledChargingMode, TargetBatteryCode, ChargeCurrentLimitCode
+from saic_ismart_client.exceptions import SaicApiException
 from saic_ismart_client.ota_v1_1.Message import MessageCoderV11
 from saic_ismart_client.ota_v1_1.data_model import AbortSendMessageReq, AlarmSwitch, AlarmSwitchReq, Message, \
     MessageBodyV11, MessageListReq, MessageListResp, MessageV11, MpAlarmSettingType, MpUserLoggingInReq, \
     MpUserLoggingInRsp, StartEndNumber, Timestamp, VinInfo
 from saic_ismart_client.ota_v2_1.Message import MessageCoderV21
 from saic_ismart_client.ota_v2_1.data_model import OtaRvcReq, OtaRvcStatus25857, OtaRvmVehicleStatusReq, \
     OtaRvmVehicleStatusResp25857, RvcReqParam
 from saic_ismart_client.ota_v3_0.Message import MessageBodyV30, MessageCoderV30, MessageV30
 from saic_ismart_client.ota_v3_0.data_model import OtaChrgCtrlReq, OtaChrgCtrlStsResp, OtaChrgHeatReq, \
     OtaChrgHeatResp, OtaChrgMangDataResp, OtaChrgRsvanReq, OtaChrgSetngReq, OtaChrgSetngResp, OtaChrgRsvanResp
+from saic_ismart_client.rest_v2.api import SaicRestV2Api
+from saic_ismart_client.rest_v2.model import TimeZoneEntity
 
 UID_INIT = '0000000000000000000000000000000000000000000000000#'
 AVG_SMS_DELIVERY_TIME = 15
 logging.basicConfig(format='%(asctime)s %(message)s')
 LOG = logging.getLogger(__name__)
 LOG.setLevel(level=os.getenv('LOG_LEVEL', 'INFO').upper())
 
@@ -60,37 +63,34 @@
     else:
         content = None
     return SaicMessage(message.message_id, message.message_type, message.title.decode(),
                        message.message_time.get_timestamp(), message.sender.decode(), content, message.read_status,
                        message.vin)
 
 
-class SaicApiException(Exception):
-    def __init__(self, msg: str, return_code: int = None):
-        if return_code is not None:
-            self.message = f'return code: {return_code}, message: {msg}'
-        else:
-            self.message = msg
-
-    def __str__(self):
-        return self.message
-
-
 class SaicApi:
-    def __init__(self, saic_uri: str, saic_user: str, saic_password: str, relogin_delay: int = None):
+    def __init__(
+            self,
+            saic_uri: str,
+            saic_rest_uri: str,
+            saic_user: str,
+            saic_password: str,
+            relogin_delay: int = None
+    ):
         self.saic_uri = saic_uri
         self.saic_user = saic_user
         self.saic_password = saic_password
         if relogin_delay is None:
             self.relogin_delay = 0
         else:
             self.relogin_delay = relogin_delay
         self.message_v1_1_coder = MessageCoderV11()
         self.message_V2_1_coder = MessageCoderV21()
         self.message_V3_0_coder = MessageCoderV30()
+        self.rest_v2_api = SaicRestV2Api(saic_rest_uri)
         self.cookies = None
         self.uid = ''
         self.token = ''
         self.token_expiration = None
         self.on_publish_raw_value = None
         self.on_publish_json_value = None
 
@@ -841,14 +841,17 @@
     def get_token(self):
         if self.token_expiration is not None:
             token_expiration = cast(Timestamp, self.token_expiration)
             if token_expiration.get_timestamp() < datetime.datetime.now():
                 self.login()
         return self.token
 
+    def get_user_timezone(self):
+        return self.rest_v2_api.get_user_timezone(self.get_token(), self.uid)
+
     def handle_error(self, message_body: AbstractMessageBody, iteration: int):
         if iteration > 0:
             waiting_time = AVG_SMS_DELIVERY_TIME * iteration
         else:
             waiting_time = AVG_SMS_DELIVERY_TIME
         message = f'application ID: {message_body.application_id},' \
                   + f' protocol version: {message_body.application_data_protocol_version},' \
```

### Comparing `saic_ismart_client-1.5.0/src/saic_ismart_client.egg-info/PKG-INFO` & `saic_ismart_client-1.6.0/src/saic_ismart_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic-ismart-client
-Version: 1.5.0
+Version: 1.6.0
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.5.0/src/saic_ismart_client.egg-info/SOURCES.txt` & `saic_ismart_client-1.6.0/src/saic_ismart_client.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 src/saic_ismart_client/__init__.py
 src/saic_ismart_client/abrp_api.py
 src/saic_ismart_client/common_model.py
+src/saic_ismart_client/exceptions.py
 src/saic_ismart_client/message_decoder.py
 src/saic_ismart_client/saic_api.py
 src/saic_ismart_client.egg-info/PKG-INFO
 src/saic_ismart_client.egg-info/SOURCES.txt
 src/saic_ismart_client.egg-info/dependency_links.txt
 src/saic_ismart_client.egg-info/requires.txt
 src/saic_ismart_client.egg-info/top_level.txt
@@ -26,12 +27,15 @@
 src/saic_ismart_client/ota_v1_1/data_model.py
 src/saic_ismart_client/ota_v2_1/Message.py
 src/saic_ismart_client/ota_v2_1/__init__.py
 src/saic_ismart_client/ota_v2_1/data_model.py
 src/saic_ismart_client/ota_v3_0/Message.py
 src/saic_ismart_client/ota_v3_0/__init__.py
 src/saic_ismart_client/ota_v3_0/data_model.py
+src/saic_ismart_client/rest_v2/__init__.py
+src/saic_ismart_client/rest_v2/api.py
+src/saic_ismart_client/rest_v2/model.py
 tests/test_Message_v1_1.py
 tests/test_Message_v2_1.py
 tests/test_Message_v3_0.py
 tests/test_abrp_api.py
 tests/test_saic_api.py
```

### Comparing `saic_ismart_client-1.5.0/tests/test_Message_v1_1.py` & `saic_ismart_client-1.6.0/tests/test_Message_v1_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.5.0/tests/test_Message_v2_1.py` & `saic_ismart_client-1.6.0/tests/test_Message_v2_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.5.0/tests/test_Message_v3_0.py` & `saic_ismart_client-1.6.0/tests/test_Message_v3_0.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.5.0/tests/test_abrp_api.py` & `saic_ismart_client-1.6.0/tests/test_abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.5.0/tests/test_saic_api.py` & `saic_ismart_client-1.6.0/tests/test_saic_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import saic_ismart_client.saic_api
 
 from saic_ismart_client.common_model import Header, MessageV2, MessageBodyV2
 from saic_ismart_client.ota_v1_1.Message import MessageCoderV11
 from saic_ismart_client.ota_v1_1.data_model import MessageV11, MpUserLoggingInRsp, MessageBodyV11, VinInfo, \
     MpAlarmSettingType
 from saic_ismart_client.ota_v2_1.Message import MessageCoderV21
-from saic_ismart_client.ota_v2_1.data_model import OtaRvmVehicleStatusResp25857, RvsPosition, RvsWayPoint,\
+from saic_ismart_client.ota_v2_1.data_model import OtaRvmVehicleStatusResp25857, RvsPosition, RvsWayPoint, \
     RvsWgs84Point, Timestamp4Short, RvsBasicStatus25857, OtaRvcStatus25857
 from saic_ismart_client.ota_v3_0.Message import MessageBodyV30, MessageV30, MessageCoderV30
 from saic_ismart_client.ota_v3_0.data_model import OtaChrgMangDataResp, RvsChargingStatus
 
 from saic_ismart_client.saic_api import SaicApi, SaicApiException
 
 TOKEN = '99X9999X-90XX-99X9-99X9-9XX9XX0X9X9XXX9X'
@@ -44,37 +44,37 @@
 def create_vin_info(vin: str) -> VinInfo:
     vin_info = VinInfo()
     vin_info.vin = vin
     vin_info.series = 'series'
     vin_info.brand_name = b'brandName'
     vin_info.model_name = b'modelName'
     vin_info.active = True
-    vin_info.model_configuration_json_str = 'name:Tire pressure monitoring system,code:J17,value:1;'\
-                                            + 'name:Regular airbags,code:Q00,value:1;'\
-                                            + 'name:Front-seat airbags,code:Q01,value:1;'\
-                                            + 'name:Airbag switch,code:Q09,value:1;'\
-                                            + 'name:Sun Roof,code:S35,value:0;'\
-                                            + 'name:Remote control,code:S61,value:1;'\
-                                            + 'name:Air conditioning,code:T11,value:1;'\
-                                            + 'name:Electric Power Steering,code:EPS,value:1;'\
-                                            + 'name:Security alert,code:SA64,value:0111110000000000001000000100101000000010100000000000000000000110;'\
-                                            + 'name:Bonnut Status,code:BONNUT,value:1;'\
-                                            + 'name:Door Status,code:DOOR,value:1111;'\
-                                            + 'name:Boot Status,code:BOOT,value:1;'\
-                                            + 'name:Engine Status,code:ENGINE,value:1;'\
-                                            + 'name:Electric Vehicle,code:EV,value:0;'\
-                                            + 'name:HeatedSeat,code:HeatedSeat,value:0;'\
-                                            + 'name:Key Position,code:KEYPOS,value:1;'\
-                                            + 'name:Energy state,code:ENERGY,value:0;'\
-                                            + 'name:Battery Voltage,code:BATTERY,value:1;'\
-                                            + 'name:Interior Temperature,code:INTEMP,value:1;'\
-                                            + 'name:Exterior Temperature,code:EXTEMP,value:1;'\
-                                            + 'name:Window Status,code:WINDOW,value:0000;'\
-                                            + 'name:Left-Right Driving,code:LRD,value:0;'\
-                                            + 'name:Bluetooth Key,code:BTKEY,value:0;'\
+    vin_info.model_configuration_json_str = 'name:Tire pressure monitoring system,code:J17,value:1;' \
+                                            + 'name:Regular airbags,code:Q00,value:1;' \
+                                            + 'name:Front-seat airbags,code:Q01,value:1;' \
+                                            + 'name:Airbag switch,code:Q09,value:1;' \
+                                            + 'name:Sun Roof,code:S35,value:0;' \
+                                            + 'name:Remote control,code:S61,value:1;' \
+                                            + 'name:Air conditioning,code:T11,value:1;' \
+                                            + 'name:Electric Power Steering,code:EPS,value:1;' \
+                                            + 'name:Security alert,code:SA64,value:0111110000000000001000000100101000000010100000000000000000000110;' \
+                                            + 'name:Bonnut Status,code:BONNUT,value:1;' \
+                                            + 'name:Door Status,code:DOOR,value:1111;' \
+                                            + 'name:Boot Status,code:BOOT,value:1;' \
+                                            + 'name:Engine Status,code:ENGINE,value:1;' \
+                                            + 'name:Electric Vehicle,code:EV,value:0;' \
+                                            + 'name:HeatedSeat,code:HeatedSeat,value:0;' \
+                                            + 'name:Key Position,code:KEYPOS,value:1;' \
+                                            + 'name:Energy state,code:ENERGY,value:0;' \
+                                            + 'name:Battery Voltage,code:BATTERY,value:1;' \
+                                            + 'name:Interior Temperature,code:INTEMP,value:1;' \
+                                            + 'name:Exterior Temperature,code:EXTEMP,value:1;' \
+                                            + 'name:Window Status,code:WINDOW,value:0000;' \
+                                            + 'name:Left-Right Driving,code:LRD,value:0;' \
+                                            + 'name:Bluetooth Key,code:BTKEY,value:0;' \
                                             + 'name:Battery Type,code:BType,value:2'
     return vin_info
 
 
 def mock_alarm_switch_response_hex(message_coder: MessageCoderV11) -> str:
     header = Header()
     header.protocol_version = 17
@@ -258,15 +258,15 @@
 
     mocked_post.return_value = res()
     type(mocked_post.return_value).content = PropertyMock(return_value=hex_value.encode())
 
 
 class TestSaicApi(TestCase):
     def setUp(self) -> None:
-        self.saic_api = SaicApi('https://tap-eu.soimt.com', 'user@home.de', 'secret')
+        self.saic_api = SaicApi('https://tap-eu.soimt.com', 'https://gateway-eu.soimt.com', 'user@home.de', 'secret')
         self.message_coder_v1_1 = MessageCoderV11()
         self.message_coder_v2_1 = MessageCoderV21()
         self.message_coder_v3_0 = MessageCoderV30()
 
     @patch.object(requests, 'post')
     def test_login(self, mocked_post):
         mock_response(mocked_post, mock_login_response_hex(self.message_coder_v1_1))
```

