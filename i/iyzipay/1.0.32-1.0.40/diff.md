# Comparing `tmp/iyzipay-1.0.32.tar.gz` & `tmp/iyzipay-1.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/iyzipay-1.0.32.tar", last modified: Fri May 11 13:29:51 2018, max compression
+gzip compressed data, was "iyzipay-1.0.40.tar", last modified: Tue Aug  1 15:05:55 2023, max compression
```

## Comparing `iyzipay-1.0.32.tar` & `iyzipay-1.0.40.tar`

### file list

```diff
@@ -1,48 +1,63 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-05-11 13:29:51.000000 iyzipay-1.0.32/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-05-11 13:29:51.000000 iyzipay-1.0.32/iyzipay/
--rw-r--r--   0 travis    (2000) travis    (2000)     1178 2018-05-11 13:29:22.000000 iyzipay-1.0.32/iyzipay/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)    40407 2018-05-11 13:29:22.000000 iyzipay-1.0.32/iyzipay/iyzipay_resource.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1508 2018-05-11 13:29:22.000000 iyzipay-1.0.32/iyzipay/pki_builder.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-05-11 13:29:51.000000 iyzipay-1.0.32/iyzipay.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     9134 2018-05-11 13:29:51.000000 iyzipay-1.0.32/iyzipay.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)     1261 2018-05-11 13:29:51.000000 iyzipay-1.0.32/iyzipay.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-05-11 13:29:51.000000 iyzipay-1.0.32/iyzipay.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        8 2018-05-11 13:29:51.000000 iyzipay-1.0.32/iyzipay.egg-info/top_level.txt
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-05-11 13:29:51.000000 iyzipay-1.0.32/samples/
--rw-r--r--   0 travis    (2000) travis    (2000)      167 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/api_test.py
--rw-r--r--   0 travis    (2000) travis    (2000)      347 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/approve.py
--rw-r--r--   0 travis    (2000) travis    (2000)      439 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/cancel.py
--rw-r--r--   0 travis    (2000) travis    (2000)      545 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/create_card.py
--rw-r--r--   0 travis    (2000) travis    (2000)      759 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/create_limited_company_sub_merchant.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2290 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/create_marketplace_payment.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2044 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/create_payment.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1945 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/create_payment_with_registered_card.py
--rw-r--r--   0 travis    (2000) travis    (2000)      350 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/create_pecco_payment.py
--rw-r--r--   0 travis    (2000) travis    (2000)      734 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/create_personal_sub_merchant.py
--rw-r--r--   0 travis    (2000) travis    (2000)      757 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/create_private_sub_merchant.py
--rw-r--r--   0 travis    (2000) travis    (2000)      401 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/create_threeds_payment.py
--rw-r--r--   0 travis    (2000) travis    (2000)      574 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/create_user_and_card.py
--rw-r--r--   0 travis    (2000) travis    (2000)      369 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/delete_card.py
--rw-r--r--   0 travis    (2000) travis    (2000)      356 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/disapprove.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1851 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/initialize_bkm.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1927 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/initialize_checkout_form.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1869 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/initialize_pecco.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2132 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/initialize_threeds.py
--rw-r--r--   0 travis    (2000) travis    (2000)      493 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/refund.py
--rw-r--r--   0 travis    (2000) travis    (2000)      348 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/retrieve_bin.py
--rw-r--r--   0 travis    (2000) travis    (2000)      323 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/retrieve_bkm_result.py
--rw-r--r--   0 travis    (2000) travis    (2000)      402 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/retrieve_bounced_bank_transfers.py
--rw-r--r--   0 travis    (2000) travis    (2000)      354 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/retrieve_cards.py
--rw-r--r--   0 travis    (2000) travis    (2000)      366 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/retrieve_checkout_form_result.py
--rw-r--r--   0 travis    (2000) travis    (2000)      386 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/retrieve_installments.py
--rw-r--r--   0 travis    (2000) travis    (2000)      377 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/retrieve_payment_result.py
--rw-r--r--   0 travis    (2000) travis    (2000)      423 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/retrieve_payout_completed_transactions.py
--rw-r--r--   0 travis    (2000) travis    (2000)      367 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/retrieve_sub_merchant.py
--rw-r--r--   0 travis    (2000) travis    (2000)      704 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/update_limited_company_sub_merchant.py
--rw-r--r--   0 travis    (2000) travis    (2000)      702 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/update_personal_sub_merchant.py
--rw-r--r--   0 travis    (2000) travis    (2000)      718 2018-05-11 13:29:22.000000 iyzipay-1.0.32/samples/update_private_sub_merchant.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1119 2018-05-11 13:29:22.000000 iyzipay-1.0.32/LICENSE
--rw-r--r--   0 travis    (2000) travis    (2000)     5581 2018-05-11 13:29:22.000000 iyzipay-1.0.32/README.md
--rwxr-xr-x   0 travis    (2000) travis    (2000)     1853 2018-05-11 13:29:22.000000 iyzipay-1.0.32/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)     9134 2018-05-11 13:29:51.000000 iyzipay-1.0.32/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)       38 2018-05-11 13:29:51.000000 iyzipay-1.0.32/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:05:55.083842 iyzipay-1.0.40/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:05:55.075842 iyzipay-1.0.40/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:05:55.075842 iyzipay-1.0.40/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-01 15:05:38.000000 iyzipay-1.0.40/.github/workflows/github_pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-01 15:05:38.000000 iyzipay-1.0.40/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-01 15:05:38.000000 iyzipay-1.0.40/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-01 15:05:55.083842 iyzipay-1.0.40/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-08-01 15:05:38.000000 iyzipay-1.0.40/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:05:55.075842 iyzipay-1.0.40/iyzipay/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-08-01 15:05:38.000000 iyzipay-1.0.40/iyzipay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44379 2023-08-01 15:05:38.000000 iyzipay-1.0.40/iyzipay/iyzipay_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-08-01 15:05:38.000000 iyzipay-1.0.40/iyzipay/pki_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:05:55.075842 iyzipay-1.0.40/iyzipay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-01 15:05:55.000000 iyzipay-1.0.40/iyzipay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-01 15:05:55.000000 iyzipay-1.0.40/iyzipay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:05:55.000000 iyzipay-1.0.40/iyzipay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 15:05:55.000000 iyzipay-1.0.40/iyzipay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 15:05:38.000000 iyzipay-1.0.40/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:05:55.083842 iyzipay-1.0.40/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/approve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/create_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/create_limited_company_sub_merchant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/create_marketplace_payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/create_payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/create_payment_with_registered_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/create_payment_with_reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/create_pecco_payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/create_personal_sub_merchant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/create_private_sub_merchant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/create_threeds_payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/create_user_and_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/delete_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/disapprove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/initialize_bkm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/initialize_checkout_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/initialize_pecco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/initialize_threeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/initialize_threeds_with_reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/iyzilink_create_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/iyzilink_delete_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/iyzilink_retrieve_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/iyzilink_retrieve_product_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/iyzilink_update_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/refund.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/retrieve_bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/retrieve_bkm_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/retrieve_bounced_bank_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/retrieve_cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/retrieve_checkout_form_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/retrieve_installments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/retrieve_loyalty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/retrieve_payment_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/retrieve_payment_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/retrieve_payout_completed_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/retrieve_sub_merchant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/retrieve_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/update_limited_company_sub_merchant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/update_personal_sub_merchant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-08-01 15:05:38.000000 iyzipay-1.0.40/samples/update_private_sub_merchant.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 15:05:55.083842 iyzipay-1.0.40/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-08-01 15:05:38.000000 iyzipay-1.0.40/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `iyzipay-1.0.32/iyzipay/__init__.py` & `iyzipay-1.0.40/iyzipay/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,12 +42,18 @@
     BasicPayment,
     BasicPaymentPreAuth,
     BasicPaymentPostAuth,
     BasicThreedsInitialize,
     BasicThreedsInitializePreAuth,
     BasicThreedsPayment,
     BasicBkm,
-    BasicBkmInitialize)
+    BasicBkmInitialize,
+    RetrievePaymentDetails,
+    RetrieveTransactions,
+    IyziLinkProduct,
+    IyziFileBase64Encoder,
+    RetrieveLoyalty)
 
 from iyzipay.pki_builder import (  # noqa
-    PKIBuilder)
+    PKIBuilder,
+)
```

### Comparing `iyzipay-1.0.32/iyzipay/iyzipay_resource.py` & `iyzipay-1.0.40/iyzipay/iyzipay_resource.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,89 @@
-import random
-import string
 import base64
 import hashlib
+import hmac
+import importlib
 import json
-import sys
-import warnings
+import random
+import re
+import string
 
 import iyzipay
 
 
 class IyzipayResource:
+    RANDOM_STRING_SIZE = 8
+    RE_SEARCH_V2 = r'/v2/'
+    header = {
+        "Accept": "application/json", 
+        "Content-type": "application/json",
+        'x-iyzi-client-version': 'iyzipay-python-1.0.40'
+    }
+
     def __init__(self):
-        pass
+        self.httplib = importlib.import_module('http.client')
 
-    RANDOM_STRING_SIZE = 8
+    def connect(self, method, url, options, request_body_dict=None, pki=None):
+        connection = self.httplib.HTTPSConnection(options['base_url'])
+        body_str = json.dumps(request_body_dict)
+        header = self.get_http_header(url, options, body_str, pki)
+        connection.request(method, url, body_str, header)
+        return connection.getresponse()
 
-    def connect(self, method, url, options, request=None, pki=None):
-        if (2, 6) <= sys.version_info < (2, 7, 9):
-            warnings.warn(
-                'Python 2.6 will not be supported in March 2018 for TLS 1.2 migration. '
-                'Please upgrade your Python version to minimum 2.7.9. '
-                'If you have any questions, please open an issue on Github or '
-                'contact us at integration@iyzico.com.',
-                DeprecationWarning)
-        if (2, 6) <= sys.version_info < (3, 0):
-            import httplib
-            connection = httplib.HTTPSConnection(options['base_url'])
+    def get_http_header(self, url, options=None, body_str=None, pki_string=None):
+        random_str = self.generate_random_string(self.RANDOM_STRING_SIZE)
+        self.header.update({'x-iyzi-rnd': random_str})
+        if re.search(self.RE_SEARCH_V2, url, re.IGNORECASE) is not None:
+            return self.get_http_header_v2(url, options, random_str, body_str)
         else:
-            import http.client
-            connection = http.client.HTTPSConnection(options['base_url'])
-        request_json = json.dumps(request)
-        connection.request(method, url, request_json, self.get_http_header(options, pki))
-        return connection.getresponse()
+            return self.get_http_header_v1(options, pki_string, random_str)
 
-    def get_http_header(self, options=None, pki_string=None):
-        header = {"Accept": "application/json", "Content-type": "application/json"}
+    def get_http_header_v1(self, options, pki_string, random_str=None):
         if pki_string is not None:
-            random_header_value = "".join(
-                random.SystemRandom().choice(string.ascii_lowercase + string.ascii_uppercase + string.digits) for _ in
-                range(self.RANDOM_STRING_SIZE))
-            header.update(
-                {'Authorization': self.prepare_auth_string(options, random_header_value, pki_string)})
-            header.update({'x-iyzi-rnd': random_header_value})
-            header.update({'x-iyzi-client-version': 'iyzipay-python-1.0.32'})
-        return header
+            self.header.update(
+                {'Authorization': self.prepare_auth_string(options, random_str, pki_string)})
+        return self.header
+
+    def get_http_header_v2(self, url, options, random_str, body_str):
+        url = url.split('?')[0]
+        hashed_v2_str = self.generate_v2_hash(options['api_key'], url, options['secret_key'], random_str, body_str)
+        self.header.update({'Authorization': 'IYZWSv2 %s' % hashed_v2_str})
+        return self.header
+
+    def generate_v2_hash(self, api_key, url, secret_key, random_str, body_str):
+        secret_key = bytes(secret_key.encode('utf-8'))
+        msg = (random_str + url + body_str).encode('utf-8')
+
+        hmac_obj = hmac.new(secret_key, digestmod=hashlib.sha256)
+        hmac_obj.update(msg)
+        signature = hmac_obj.hexdigest()
+        authorization_params = [
+            'apiKey:' + api_key,
+            'randomKey:' + random_str,
+            'signature:' + signature
+        ]
+        return base64.b64encode('&'.join(authorization_params).encode()).decode()
 
     def get_plain_http_header(self, options):
-        return self.get_http_header(None, options)
+        return self.get_http_header_v1(None, options)
 
     def prepare_auth_string(self, options, random_str, pki_string):
         hashed = self.generate_hash(options['api_key'], options['secret_key'], random_str, pki_string)
         return self.format_header_string(options['api_key'], hashed)
 
+    def generate_random_string(self, size):
+        return "".join(
+                random.SystemRandom().choice(string.ascii_letters + string.digits) for _ in
+                range(size))
+
     @staticmethod
     def generate_hash(api_key, secret_key, random_string, pki_string):
         hash_str = api_key + random_string + secret_key + pki_string
-        if sys.version_info < (3, 0):
-            hex_dig = hashlib.sha1(hash_str).digest()
-        else:
-            hex_dig = hashlib.sha1(hash_str.encode()).digest()
+        hex_dig = hashlib.sha1(hash_str.encode()).digest()
+
         return base64.b64encode(hex_dig)
 
     @staticmethod
     def format_header_string(api_key, hashed):
         hashed = hashed.decode('utf-8')
         return 'IYZWS %s:%s' % (api_key, hashed)
 
@@ -155,14 +176,20 @@
         pki_builder.append('cardAlias', card.get('cardAlias'))
         pki_builder.append('cardNumber', card.get('cardNumber'))
         pki_builder.append('expireYear', card.get('expireYear'))
         pki_builder.append('expireMonth', card.get('expireMonth'))
         pki_builder.append('cardHolderName', card.get('cardHolderName'))
         return pki_builder.get_request_string()
 
+    @staticmethod
+    def reward_usage_pki(reward_usage):
+        pki_builder = iyzipay.PKIBuilder('')
+        pki_builder.append('rewardAmount', reward_usage.get('rewardAmount'))
+        pki_builder.append('rewardUsage', reward_usage.get('rewardUsage'))
+        return pki_builder.get_request_string()
 
 class ApiTest(IyzipayResource):
     def retrieve(self, options):
         return self.connect('GET', '/payment/test', options)
 
 
 class BinNumber(IyzipayResource):
@@ -228,14 +255,15 @@
         pki_builder.append('paymentSource', request.get('paymentSource'))
         pki_builder.append('currency', request.get('currency'))
         pki_builder.append('posOrderId', request.get('posOrderId'))
         pki_builder.append_price('paidPrice', request.get('paidPrice'))
         pki_builder.append('forceThreeDS', request.get('forceThreeDS'))
         pki_builder.append('cardUserKey', request.get('cardUserKey'))
         pki_builder.append_array('enabledInstallments', request.get('enabledInstallments'))
+        pki_builder.append('debitCardAllowed', request.get('debitCardAllowed'))
         return pki_builder.get_request_string()
 
 
 class CheckoutForm(IyzipayResource):
     def retrieve(self, request, options):
         pki = self.to_pki_string(request)
         return self.connect('POST', '/payment/iyzipos/checkoutform/auth/ecom/detail', options, request, pki)
@@ -268,14 +296,15 @@
         pki_builder.append('shippingAddress', self.address_pki(request.get('shippingAddress')))
         pki_builder.append('billingAddress', self.address_pki(request.get('billingAddress')))
         pki_builder.append_array('basketItems', self.basket_pki(request.get('basketItems')))
         pki_builder.append('paymentSource', request.get('paymentSource'))
         pki_builder.append('currency', request.get('currency'))
         pki_builder.append('posOrderId', request.get('posOrderId'))
         pki_builder.append('connectorName', request.get('connectorName'))
+        pki_builder.append('plusInstallmentUsage', request.get('plusInstallmentUsage'))
         pki_builder.append('callbackUrl', request.get('callbackUrl'))
         return pki_builder.get_request_string()
 
     def to_pki_string_retrieve(self, request):
         pki_builder = iyzipay.PKIBuilder(self.resource_pki(request))
         pki_builder.append('paymentId', request.get('paymentId'))
         pki_builder.append('paymentConversationId', request.get('paymentConversationId'))
@@ -298,14 +327,17 @@
         pki_builder.append('paymentCard', self.payment_card_pki(request.get('paymentCard')))
         pki_builder.append('buyer', self.buyer_pki(request.get('buyer')))
         pki_builder.append('shippingAddress', self.address_pki(request.get('shippingAddress')))
         pki_builder.append('billingAddress', self.address_pki(request.get('billingAddress')))
         pki_builder.append_array('basketItems', self.basket_pki(request.get('basketItems')))
         pki_builder.append('paymentSource', request.get('paymentSource'))
         pki_builder.append('currency', request.get('currency'))
+        pki_builder.append('posOrderId', request.get('posOrderId'))
+        pki_builder.append('connectorName', request.get('connectorName'))
+        pki_builder.append('plusInstallmentUsage', request.get('plusInstallmentUsage'))
         pki_builder.append('callbackUrl', request.get('callbackUrl'))
         return pki_builder.get_request_string()
 
 
 class ThreedsPayment(IyzipayResource):
     def create(self, request, options):
         pki = self.to_pki_string_create(request)
@@ -804,7 +836,68 @@
         pki_builder.append('callbackUrl', request.get('callbackUrl'))
         pki_builder.append('buyerEmail', request.get('buyerEmail'))
         pki_builder.append('buyerId', request.get('buyerId'))
         pki_builder.append('buyerIp', request.get('buyerIp'))
         pki_builder.append('posOrderId', request.get('posOrderId'))
         pki_builder.append_array('installmentDetails', self.installment_details_pki(request.get('installmentDetails')))
         return pki_builder.get_request_string()
+
+
+class RetrievePaymentDetails(IyzipayResource):
+    def retrieve(self, request, options):
+        payment_conversation_id = str(request.get('paymentConversationId'))
+        return self.connect('GET', '/v2/reporting/payment/details?paymentConversationId=' + payment_conversation_id, options)
+
+
+class RetrieveTransactions(IyzipayResource):
+    def retrieve(self, request, options):
+        page = str(request.get('page'))
+        transaction_date = str(request.get('transactionDate'))
+        query_params = 'transactionDate=' + transaction_date + '&page=' + page
+        return self.connect('GET', '/v2/reporting/payment/transactions?' + query_params, options)
+
+
+class IyziFileBase64Encoder:
+    @staticmethod
+    def encode(file_path):
+        with open(file_path, "rb") as f:
+            return base64.b64encode(f.read()).decode('utf-8')
+
+
+class IyziLinkProduct(IyzipayResource):
+    def create(self, request, options):
+        return self.connect('POST', '/v2/iyzilink/products/', options, request)
+    
+    def retrieve(self, request, options):
+        if request.get('token') is None:
+            raise Exception('token must be in request')
+        token = str(request.get('token'))
+        return self.connect('GET', '/v2/iyzilink/products/' + token, options)
+
+    def get(self, request, options):
+        page = str(request.get('page') or 1)
+        count = str(request.get('count') or 10)
+        return self.connect('GET', '/v2/iyzilink/products/?page=' + page + '&count=' + count, options)
+
+    def update(self, request, options):
+        if request.get('token') is None:
+            raise Exception('token must be in request')
+        token = str(request.get('token'))
+        return self.connect('PUT', '/v2/iyzilink/products/' + token, options, request)
+    
+    def delete(self, request, options):
+        if request.get('token') is None:
+            raise Exception('token must be in request')
+        token = str(request.get('token'))
+        return self.connect('DELETE', '/v2/iyzilink/products/' + token, options)
+
+
+class RetrieveLoyalty(IyzipayResource):
+    def retrieve(self, request, options):
+        pki = self.to_pki_string_create(request)
+        return self.connect('POST', '/payment/loyalty/inquire', options, request, pki)
+
+    def to_pki_string_create(self, request):
+        pki_builder = iyzipay.PKIBuilder(self.resource_pki(request))
+        pki_builder.append('paymentCard', self.payment_card_pki(request.get('paymentCard')))
+        pki_builder.append('currency', request.get('currency'))
+        return pki_builder.get_request_string()
```

### Comparing `iyzipay-1.0.32/iyzipay/pki_builder.py` & `iyzipay-1.0.40/iyzipay/pki_builder.py`

 * *Files identical despite different names*

### Comparing `iyzipay-1.0.32/iyzipay.egg-info/SOURCES.txt` & `iyzipay-1.0.40/iyzipay.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 LICENSE
 README.md
+pyproject.toml
 setup.py
+.github/workflows/github_pull_request.yml
+.github/workflows/python-publish.yml
 iyzipay/__init__.py
 iyzipay/iyzipay_resource.py
 iyzipay/pki_builder.py
 iyzipay.egg-info/PKG-INFO
 iyzipay.egg-info/SOURCES.txt
 iyzipay.egg-info/dependency_links.txt
 iyzipay.egg-info/top_level.txt
@@ -12,31 +15,41 @@
 samples/approve.py
 samples/cancel.py
 samples/create_card.py
 samples/create_limited_company_sub_merchant.py
 samples/create_marketplace_payment.py
 samples/create_payment.py
 samples/create_payment_with_registered_card.py
+samples/create_payment_with_reward.py
 samples/create_pecco_payment.py
 samples/create_personal_sub_merchant.py
 samples/create_private_sub_merchant.py
 samples/create_threeds_payment.py
 samples/create_user_and_card.py
 samples/delete_card.py
 samples/disapprove.py
 samples/initialize_bkm.py
 samples/initialize_checkout_form.py
 samples/initialize_pecco.py
 samples/initialize_threeds.py
+samples/initialize_threeds_with_reward.py
+samples/iyzilink_create_product.py
+samples/iyzilink_delete_product.py
+samples/iyzilink_retrieve_product.py
+samples/iyzilink_retrieve_product_list.py
+samples/iyzilink_update_product.py
 samples/refund.py
 samples/retrieve_bin.py
 samples/retrieve_bkm_result.py
 samples/retrieve_bounced_bank_transfers.py
 samples/retrieve_cards.py
 samples/retrieve_checkout_form_result.py
 samples/retrieve_installments.py
+samples/retrieve_loyalty.py
+samples/retrieve_payment_detail.py
 samples/retrieve_payment_result.py
 samples/retrieve_payout_completed_transactions.py
 samples/retrieve_sub_merchant.py
+samples/retrieve_transactions.py
 samples/update_limited_company_sub_merchant.py
 samples/update_personal_sub_merchant.py
 samples/update_private_sub_merchant.py
```

### Comparing `iyzipay-1.0.32/samples/create_card.py` & `iyzipay-1.0.40/samples/create_card.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding=utf-8
-
 import iyzipay
 
 options = {
     'api_key': iyzipay.api_key,
     'secret_key': iyzipay.secret_key,
     'base_url': iyzipay.base_url
 }
```

### Comparing `iyzipay-1.0.32/samples/create_limited_company_sub_merchant.py` & `iyzipay-1.0.40/samples/create_private_sub_merchant.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-# coding=utf-8
-
 import iyzipay
 
 options = {
     'api_key': iyzipay.api_key,
     'secret_key': iyzipay.secret_key,
     'base_url': iyzipay.base_url
 }
 
 request = {
     'locale': 'tr',
     'conversationId': '123456789',
-    'subMerchantExternalId': 'AS49224',
-    'subMerchantType': 'LIMITED_OR_JOINT_STOCK_COMPANY',
+    'subMerchantExternalId': 'S49222',
+    'subMerchantType': 'PRIVATE_COMPANY',
     'address': 'Nidakule Göztepe, Merdivenköy Mah. Bora Sok. No:1',
     'taxOffice': 'Tax Office',
-    'taxNumber': '9261877',
-    'legalCompanyTitle': 'XYZ inc',
+    'legalCompanyTitle': 'John Doe inc',
     'email': 'email@submerchantemail.com',
     'gsmNumber': '+905350000000',
     'name': 'John\'s market',
     'iban': 'TR180006200119000006672315',
+    'identityNumber': '31300864726',
     'currency': 'TRY'
 }
 
 sub_merchant = iyzipay.SubMerchant().create(request, options)
 
 print(sub_merchant.read().decode('utf-8'))
```

### Comparing `iyzipay-1.0.32/samples/create_marketplace_payment.py` & `iyzipay-1.0.40/samples/create_marketplace_payment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding=utf-8
-
 import iyzipay
 
 options = {
     'api_key': iyzipay.api_key,
     'secret_key': iyzipay.secret_key,
     'base_url': iyzipay.base_url
 }
```

### Comparing `iyzipay-1.0.32/samples/create_payment.py` & `iyzipay-1.0.40/samples/create_payment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding=utf-8
-
 import iyzipay
 
 options = {
     'api_key': iyzipay.api_key,
     'secret_key': iyzipay.secret_key,
     'base_url': iyzipay.base_url
 }
```

### Comparing `iyzipay-1.0.32/samples/create_payment_with_registered_card.py` & `iyzipay-1.0.40/samples/create_payment_with_registered_card.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding=utf-8
-
 import iyzipay
 
 options = {
     'api_key': iyzipay.api_key,
     'secret_key': iyzipay.secret_key,
     'base_url': iyzipay.base_url
 }
```

### Comparing `iyzipay-1.0.32/samples/create_personal_sub_merchant.py` & `iyzipay-1.0.40/samples/update_personal_sub_merchant.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-# coding=utf-8
-
 import iyzipay
 
 options = {
     'api_key': iyzipay.api_key,
     'secret_key': iyzipay.secret_key,
     'base_url': iyzipay.base_url
 }
 
 request = {
     'locale': 'tr',
     'conversationId': '123456789',
-    'subMerchantExternalId': 'B49224',
-    'subMerchantType': 'PERSONAL',
+    'subMerchantKey': 'sub merchant key',
+    'iban': 'TR180006200119000006672315',
     'address': 'Nidakule Göztepe, Merdivenköy Mah. Bora Sok. No:1',
-    'contactName': 'John',
+    'contactName': 'Jane',
     'contactSurname': 'Doe',
     'email': 'email@submerchantemail.com',
     'gsmNumber': '+905350000000',
-    'name': 'John\'s market',
-    'iban': 'TR180006200119000006672315',
+    'name': 'Jane\'s market',
     'identityNumber': '31300864726',
     'currency': 'TRY'
 }
 
-sub_merchant = iyzipay.SubMerchant().create(request, options)
+sub_merchant = iyzipay.SubMerchant().update(request, options)
 
 print(sub_merchant.read().decode('utf-8'))
```

### Comparing `iyzipay-1.0.32/samples/create_private_sub_merchant.py` & `iyzipay-1.0.40/samples/update_private_sub_merchant.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-# coding=utf-8
-
 import iyzipay
 
 options = {
     'api_key': iyzipay.api_key,
     'secret_key': iyzipay.secret_key,
     'base_url': iyzipay.base_url
 }
 
 request = {
     'locale': 'tr',
     'conversationId': '123456789',
-    'subMerchantExternalId': 'S49222',
-    'subMerchantType': 'PRIVATE_COMPANY',
+    'subMerchantKey': 'sub merchant key',
     'address': 'Nidakule Göztepe, Merdivenköy Mah. Bora Sok. No:1',
     'taxOffice': 'Tax Office',
-    'legalCompanyTitle': 'John Doe inc',
+    'legalCompanyTitle': 'Jane Doe inc',
     'email': 'email@submerchantemail.com',
     'gsmNumber': '+905350000000',
-    'name': 'John\'s market',
+    'name': 'Jane\'s market',
     'iban': 'TR180006200119000006672315',
     'identityNumber': '31300864726',
     'currency': 'TRY'
 }
 
-sub_merchant = iyzipay.SubMerchant().create(request, options)
+sub_merchant = iyzipay.SubMerchant().update(request, options)
 
 print(sub_merchant.read().decode('utf-8'))
```

### Comparing `iyzipay-1.0.32/samples/create_user_and_card.py` & `iyzipay-1.0.40/samples/create_user_and_card.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding=utf-8
-
 import iyzipay
 
 options = {
     'api_key': iyzipay.api_key,
     'secret_key': iyzipay.secret_key,
     'base_url': iyzipay.base_url
 }
```

### Comparing `iyzipay-1.0.32/samples/initialize_bkm.py` & `iyzipay-1.0.40/samples/initialize_bkm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding=utf-8
-
 import iyzipay
 
 options = {
     'api_key': iyzipay.api_key,
     'secret_key': iyzipay.secret_key,
     'base_url': iyzipay.base_url
 }
```

### Comparing `iyzipay-1.0.32/samples/initialize_checkout_form.py` & `iyzipay-1.0.40/samples/initialize_checkout_form.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding=utf-8
-
 import iyzipay
 
 options = {
     'api_key': iyzipay.api_key,
     'secret_key': iyzipay.secret_key,
     'base_url': iyzipay.base_url
 }
@@ -68,13 +66,14 @@
     'basketId': 'B67832',
     'paymentGroup': 'PRODUCT',
     "callbackUrl": "https://www.merchant.com/callback",
     "enabledInstallments": ['2', '3', '6', '9'],
     'buyer': buyer,
     'shippingAddress': address,
     'billingAddress': address,
-    'basketItems': basket_items
+    'basketItems': basket_items,
+    'debitCardAllowed': True
 }
 
 checkout_form_initialize = iyzipay.CheckoutFormInitialize().create(request, options)
 
 print(checkout_form_initialize.read().decode('utf-8'))
```

### Comparing `iyzipay-1.0.32/samples/initialize_pecco.py` & `iyzipay-1.0.40/samples/initialize_pecco.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding=utf-8
-
 import iyzipay
 
 options = {
     'api_key': iyzipay.api_key,
     'secret_key': iyzipay.secret_key,
     'base_url': iyzipay.base_url
 }
```

### Comparing `iyzipay-1.0.32/samples/initialize_threeds.py` & `iyzipay-1.0.40/samples/initialize_threeds.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding=utf-8
-
 import iyzipay
 
 options = {
     'api_key': iyzipay.api_key,
     'secret_key': iyzipay.secret_key,
     'base_url': iyzipay.base_url
 }
```

### Comparing `iyzipay-1.0.32/samples/update_limited_company_sub_merchant.py` & `iyzipay-1.0.40/samples/update_limited_company_sub_merchant.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# coding=utf-8
-
 import iyzipay
 
 options = {
     'api_key': iyzipay.api_key,
     'secret_key': iyzipay.secret_key,
     'base_url': iyzipay.base_url
 }
```

### Comparing `iyzipay-1.0.32/samples/update_personal_sub_merchant.py` & `iyzipay-1.0.40/samples/create_personal_sub_merchant.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-# coding=utf-8
-
 import iyzipay
 
 options = {
     'api_key': iyzipay.api_key,
     'secret_key': iyzipay.secret_key,
     'base_url': iyzipay.base_url
 }
 
 request = {
     'locale': 'tr',
     'conversationId': '123456789',
-    'subMerchantKey': 'sub merchant key',
-    'iban': 'TR180006200119000006672315',
+    'subMerchantExternalId': 'B49224',
+    'subMerchantType': 'PERSONAL',
     'address': 'Nidakule Göztepe, Merdivenköy Mah. Bora Sok. No:1',
-    'contactName': 'Jane',
+    'contactName': 'John',
     'contactSurname': 'Doe',
     'email': 'email@submerchantemail.com',
     'gsmNumber': '+905350000000',
-    'name': 'Jane\'s market',
+    'name': 'John\'s market',
+    'iban': 'TR180006200119000006672315',
     'identityNumber': '31300864726',
     'currency': 'TRY'
 }
 
-sub_merchant = iyzipay.SubMerchant().update(request, options)
+sub_merchant = iyzipay.SubMerchant().create(request, options)
 
 print(sub_merchant.read().decode('utf-8'))
```

### Comparing `iyzipay-1.0.32/LICENSE` & `iyzipay-1.0.40/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2016 - iyzico odeme hizmetleri A.S.  (https://iyzico.com)
+Copyright (c) 2020 - iyzico odeme hizmetleri A.S.  (https://iyzico.com)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `iyzipay-1.0.32/README.md` & `iyzipay-1.0.40/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # iyzipay-python
 
-[![Build Status](https://travis-ci.org/iyzico/iyzipay-python.svg?branch=master)](https://travis-ci.org/iyzico/iyzipay-python)
-
 You can sign up for an iyzico account at https://iyzico.com
 
 # Requirements
 
-Python 2.6 and later.
+Python 3.6+
 
-### Note
+### Deprecation Notes
 
-Python 2.6 will not be supported in March 2018 for TLS 1.2 migration. Please upgrade your Python version to minimum 2.7.9. If you have any questions, please open an issue on Github or contact us at integration@iyzico.com.
+- Python 2.7 will not be maintained past 2020. As we iyzico, we will not support of that python version at March of 2020. If you have any questions, please open an issue on Github or contact us at integration@iyzico.com.
+- Python 3.2, 3.3, 3.4 and 3.5 supports are dropped after v1.0.37.
 
 # Installation
 
 ### PyPI
 
 You can install the bindings via [PyPI](https://pypi.python.org). Run the following command:
 
@@ -157,15 +156,14 @@
 
 *Cross border* test cards:
 
 Card Number      | Country
 -----------      | -------
 4054180000000007 | Non-Turkish (Debit)
 5400010000000004 | Non-Turkish (Credit)  
-6221060000000004 | Iran  
 
 Test cards to get specific *error* codes:
 
 Card Number       | Description
 -----------       | -----------
 5406670000000009  | Success but cannot be cancelled, refund or post auth
 4111111111111129  | Not sufficient funds
```

### Comparing `iyzipay-1.0.32/setup.py` & `iyzipay-1.0.40/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,44 @@
 import os
-import sys
-import warnings
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 with open('README.md') as f:
     README = f.read()
 
 with open('LICENSE') as f:
     LICENSE = f.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
-install_requires = []
-
-if sys.version_info < (2, 6):
-    warnings.warn(
-        'Python 2.5 is not officially supported by iyzico. '
-        'If you have any questions, please open an issue on Github or '
-        'contact us at integration@iyzico.com.',
-        DeprecationWarning)
-    install_requires.append('requests >= 0.8.8, < 0.10.1')
-    install_requires.append('ssl')
-else:
-    install_requires.append('requests >= 0.8.8')
+install_requires = [
+    'requests >= 0.8.8',
+]
 
 setup(
     name='iyzipay',
-    version='1.0.32',
+    version='1.0.40',
     use_scm_version=True,
     setup_requires=['setuptools_scm', 'future'],
     description='iyzipay api python client',
-    long_description=README,
+#    long_description=README,
+    long_description="Test Description",
     author='iyzico',
     author_email='iyzico-ci@iyzico.com',
     url='https://github.com/iyzico/iyzipay-python',
-    license=LICENSE,
+#    license=LICENSE,
+    license="MIT",
     packages=find_packages(exclude='tests'),
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.6",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.2",
-        "Programming Language :: Python :: 3.3",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

