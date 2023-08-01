# Comparing `tmp/trex-model-1.0.4.tar.gz` & `tmp/trex-model-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-model-1.0.4.tar", last modified: Mon May 15 06:17:26 2023, max compression
+gzip compressed data, was "trex-model-1.0.6.tar", last modified: Tue Aug  1 02:32:09 2023, max compression
```

## Comparing `trex-model-1.0.4.tar` & `trex-model-1.0.6.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:17:26.511225 trex-model-1.0.4/
--rw-r--r--   0 jacklok    (501) staff       (20)     1074 2020-09-06 08:34:15.000000 trex-model-1.0.4/LICENSE
--rw-r--r--   0 jacklok    (501) staff       (20)       60 2020-09-10 05:51:48.000000 trex-model-1.0.4/MANIFEST.in
--rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-05-15 06:17:26.511367 trex-model-1.0.4/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       57 2020-09-06 08:43:45.000000 trex-model-1.0.4/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-05-15 06:17:26.511832 trex-model-1.0.4/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      922 2023-05-15 06:17:22.000000 trex-model-1.0.4/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:17:26.464380 trex-model-1.0.4/trex_model.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-05-15 06:17:26.000000 trex-model-1.0.4/trex_model.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1847 2023-05-15 06:17:26.000000 trex-model-1.0.4/trex_model.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-05-15 06:17:26.000000 trex-model-1.0.4/trex_model.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       95 2023-05-15 06:17:26.000000 trex-model-1.0.4/trex_model.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       16 2023-05-15 06:17:26.000000 trex-model-1.0.4/trex_model.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:17:26.466964 trex-model-1.0.4/trexmodel/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-06 08:58:46.000000 trex-model-1.0.4/trexmodel/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1122 2021-09-03 09:11:14.000000 trex-model-1.0.4/trexmodel/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:17:26.469833 trex-model-1.0.4/trexmodel/models/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-03 01:59:33.000000 trex-model-1.0.4/trexmodel/models/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:17:26.507839 trex-model-1.0.4/trexmodel/models/datastore/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 04:46:11.000000 trex-model-1.0.4/trexmodel/models/datastore/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4892 2022-11-14 06:42:31.000000 trex-model-1.0.4/trexmodel/models/datastore/admin_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3223 2023-04-11 07:48:46.000000 trex-model-1.0.4/trexmodel/models/datastore/analytic_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2155 2021-02-19 08:24:29.000000 trex-model-1.0.4/trexmodel/models/datastore/coporate_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    13539 2023-03-15 08:15:01.000000 trex-model-1.0.4/trexmodel/models/datastore/customer_model_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)    48341 2023-05-12 06:20:00.000000 trex-model-1.0.4/trexmodel/models/datastore/customer_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1712 2020-10-26 01:02:17.000000 trex-model-1.0.4/trexmodel/models/datastore/fb_subsriber_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1351 2021-08-19 08:33:56.000000 trex-model-1.0.4/trexmodel/models/datastore/inventory_model.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5974 2023-05-15 01:59:38.000000 trex-model-1.0.4/trexmodel/models/datastore/loyalty_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3663 2023-05-12 08:12:47.000000 trex-model-1.0.4/trexmodel/models/datastore/lucky_draw_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    11281 2023-04-05 03:48:05.000000 trex-model-1.0.4/trexmodel/models/datastore/membership_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    57379 2023-05-15 02:58:36.000000 trex-model-1.0.4/trexmodel/models/datastore/merchant_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1785 2021-05-17 10:44:34.000000 trex-model-1.0.4/trexmodel/models/datastore/model_decorators.py
--rw-r--r--   0 jacklok    (501) staff       (20)    17711 2023-02-10 02:53:30.000000 trex-model-1.0.4/trexmodel/models/datastore/ndb_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    32251 2023-05-15 02:04:46.000000 trex-model-1.0.4/trexmodel/models/datastore/pos_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    20750 2023-04-10 08:59:10.000000 trex-model-1.0.4/trexmodel/models/datastore/prepaid_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    38941 2023-02-28 05:40:30.000000 trex-model-1.0.4/trexmodel/models/datastore/product_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    47521 2023-03-15 14:31:35.000000 trex-model-1.0.4/trexmodel/models/datastore/program_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    36350 2023-04-13 13:46:37.000000 trex-model-1.0.4/trexmodel/models/datastore/redeem_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    31165 2023-04-10 09:19:08.000000 trex-model-1.0.4/trexmodel/models/datastore/reward_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)      602 2021-02-19 08:54:31.000000 trex-model-1.0.4/trexmodel/models/datastore/spending_base_program_model.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6610 2021-03-30 06:42:06.000000 trex-model-1.0.4/trexmodel/models/datastore/system_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1348 2020-09-09 01:17:56.000000 trex-model-1.0.4/trexmodel/models/datastore/task_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1319 2022-09-09 14:28:48.000000 trex-model-1.0.4/trexmodel/models/datastore/test_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    36809 2023-04-24 09:59:51.000000 trex-model-1.0.4/trexmodel/models/datastore/transaction_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    15228 2022-09-23 07:10:51.000000 trex-model-1.0.4/trexmodel/models/datastore/user_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    17441 2022-12-29 13:44:05.000000 trex-model-1.0.4/trexmodel/models/datastore/voucher_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6452 2023-03-19 11:12:11.000000 trex-model-1.0.4/trexmodel/models/merchant_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-05-16 04:55:29.000000 trex-model-1.0.4/trexmodel/models/model_decorator.py
--rw-r--r--   0 jacklok    (501) staff       (20)      331 2021-09-02 08:53:31.000000 trex-model-1.0.4/trexmodel/models/prepaid_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)      172 2022-03-04 03:54:52.000000 trex-model-1.0.4/trexmodel/pos_conf.py
--rw-r--r--   0 jacklok    (501) staff       (20)    16572 2023-04-07 03:52:51.000000 trex-model-1.0.4/trexmodel/program_conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:17:26.509205 trex-model-1.0.4/trexmodel/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.4/trexmodel/utils/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:17:26.509659 trex-model-1.0.4/trexmodel/utils/gcloud/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.4/trexmodel/utils/gcloud/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      291 2020-08-31 07:47:30.000000 trex-model-1.0.4/trexmodel/utils/gcloud/datastore_util.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:17:26.510544 trex-model-1.0.4/trexmodel/utils/model/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.4/trexmodel/utils/model/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2453 2022-09-09 14:29:07.000000 trex-model-1.0.4/trexmodel/utils/model/model_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:32:09.211511 trex-model-1.0.6/
+-rw-r--r--   0 jacklok    (501) staff       (20)     1074 2020-09-06 08:34:15.000000 trex-model-1.0.6/LICENSE
+-rw-r--r--   0 jacklok    (501) staff       (20)       60 2020-09-10 05:51:48.000000 trex-model-1.0.6/MANIFEST.in
+-rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-08-01 02:32:09.211940 trex-model-1.0.6/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       57 2020-09-06 08:43:45.000000 trex-model-1.0.6/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-08-01 02:32:09.212713 trex-model-1.0.6/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      922 2023-08-01 02:30:21.000000 trex-model-1.0.6/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:32:09.163745 trex-model-1.0.6/trex_model.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-08-01 02:32:08.000000 trex-model-1.0.6/trex_model.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1888 2023-08-01 02:32:09.000000 trex-model-1.0.6/trex_model.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-08-01 02:32:08.000000 trex-model-1.0.6/trex_model.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       95 2023-08-01 02:32:08.000000 trex-model-1.0.6/trex_model.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       16 2023-08-01 02:32:08.000000 trex-model-1.0.6/trex_model.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:32:09.166646 trex-model-1.0.6/trexmodel/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-06 08:58:46.000000 trex-model-1.0.6/trexmodel/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1122 2021-09-03 09:11:14.000000 trex-model-1.0.6/trexmodel/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:32:09.170331 trex-model-1.0.6/trexmodel/models/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-03 01:59:33.000000 trex-model-1.0.6/trexmodel/models/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:32:09.206272 trex-model-1.0.6/trexmodel/models/datastore/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 04:46:11.000000 trex-model-1.0.6/trexmodel/models/datastore/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4892 2022-11-14 06:42:31.000000 trex-model-1.0.6/trexmodel/models/datastore/admin_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3223 2023-04-11 07:48:46.000000 trex-model-1.0.6/trexmodel/models/datastore/analytic_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2397 2023-05-24 02:56:50.000000 trex-model-1.0.6/trexmodel/models/datastore/app_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2155 2021-02-19 08:24:29.000000 trex-model-1.0.6/trexmodel/models/datastore/coporate_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    13782 2023-06-30 04:11:05.000000 trex-model-1.0.6/trexmodel/models/datastore/customer_model_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    52732 2023-07-14 08:30:13.000000 trex-model-1.0.6/trexmodel/models/datastore/customer_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1712 2020-10-26 01:02:17.000000 trex-model-1.0.6/trexmodel/models/datastore/fb_subsriber_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1351 2021-08-19 08:33:56.000000 trex-model-1.0.6/trexmodel/models/datastore/inventory_model.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5998 2023-05-23 01:07:42.000000 trex-model-1.0.6/trexmodel/models/datastore/loyalty_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    39152 2023-07-14 08:31:03.000000 trex-model-1.0.6/trexmodel/models/datastore/lucky_draw_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11262 2023-05-24 00:59:12.000000 trex-model-1.0.6/trexmodel/models/datastore/membership_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    63360 2023-07-07 06:20:55.000000 trex-model-1.0.6/trexmodel/models/datastore/merchant_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1785 2021-05-17 10:44:34.000000 trex-model-1.0.6/trexmodel/models/datastore/model_decorators.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    17711 2023-02-10 02:53:30.000000 trex-model-1.0.6/trexmodel/models/datastore/ndb_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    32274 2023-05-23 01:09:58.000000 trex-model-1.0.6/trexmodel/models/datastore/pos_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    20750 2023-04-10 08:59:10.000000 trex-model-1.0.6/trexmodel/models/datastore/prepaid_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    38941 2023-02-28 05:40:30.000000 trex-model-1.0.6/trexmodel/models/datastore/product_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    47495 2023-06-16 09:42:26.000000 trex-model-1.0.6/trexmodel/models/datastore/program_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    36350 2023-04-13 13:46:37.000000 trex-model-1.0.6/trexmodel/models/datastore/redeem_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    31635 2023-06-30 13:35:40.000000 trex-model-1.0.6/trexmodel/models/datastore/reward_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      602 2021-02-19 08:54:31.000000 trex-model-1.0.6/trexmodel/models/datastore/spending_base_program_model.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6610 2021-03-30 06:42:06.000000 trex-model-1.0.6/trexmodel/models/datastore/system_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1348 2020-09-09 01:17:56.000000 trex-model-1.0.6/trexmodel/models/datastore/task_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1319 2022-09-09 14:28:48.000000 trex-model-1.0.6/trexmodel/models/datastore/test_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    40475 2023-06-30 07:45:10.000000 trex-model-1.0.6/trexmodel/models/datastore/transaction_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    15859 2023-07-31 15:06:26.000000 trex-model-1.0.6/trexmodel/models/datastore/user_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    17441 2022-12-29 13:44:05.000000 trex-model-1.0.6/trexmodel/models/datastore/voucher_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     9169 2023-07-07 06:21:27.000000 trex-model-1.0.6/trexmodel/models/merchant_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-05-16 04:55:29.000000 trex-model-1.0.6/trexmodel/models/model_decorator.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      331 2021-09-02 08:53:31.000000 trex-model-1.0.6/trexmodel/models/prepaid_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      172 2022-03-04 03:54:52.000000 trex-model-1.0.6/trexmodel/pos_conf.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    18959 2023-07-06 08:34:50.000000 trex-model-1.0.6/trexmodel/program_conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:32:09.208088 trex-model-1.0.6/trexmodel/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.6/trexmodel/utils/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:32:09.208726 trex-model-1.0.6/trexmodel/utils/gcloud/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.6/trexmodel/utils/gcloud/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      291 2020-08-31 07:47:30.000000 trex-model-1.0.6/trexmodel/utils/gcloud/datastore_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:32:09.210573 trex-model-1.0.6/trexmodel/utils/model/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.6/trexmodel/utils/model/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2453 2022-09-09 14:29:07.000000 trex-model-1.0.6/trexmodel/utils/model/model_util.py
```

### Comparing `trex-model-1.0.4/LICENSE` & `trex-model-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.4/setup.py` & `trex-model-1.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
      name='trex-model',  
-     version='1.0.4',
+     version='1.0.6',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex database module package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-model",
      packages=setuptools.find_packages(),
```

### Comparing `trex-model-1.0.4/trex_model.egg-info/SOURCES.txt` & `trex-model-1.0.6/trex_model.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 trexmodel/models/__init__.py
 trexmodel/models/merchant_helpers.py
 trexmodel/models/model_decorator.py
 trexmodel/models/prepaid_helpers.py
 trexmodel/models/datastore/__init__.py
 trexmodel/models/datastore/admin_models.py
 trexmodel/models/datastore/analytic_models.py
+trexmodel/models/datastore/app_models.py
 trexmodel/models/datastore/coporate_models.py
 trexmodel/models/datastore/customer_model_helpers.py
 trexmodel/models/datastore/customer_models.py
 trexmodel/models/datastore/fb_subsriber_models.py
 trexmodel/models/datastore/inventory_model.py
 trexmodel/models/datastore/loyalty_models.py
 trexmodel/models/datastore/lucky_draw_models.py
```

### Comparing `trex-model-1.0.4/trexmodel/conf.py` & `trex-model-1.0.6/trexmodel/conf.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/admin_models.py` & `trex-model-1.0.6/trexmodel/models/datastore/admin_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/analytic_models.py` & `trex-model-1.0.6/trexmodel/models/datastore/analytic_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/coporate_models.py` & `trex-model-1.0.6/trexmodel/models/datastore/coporate_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/customer_model_helpers.py` & `trex-model-1.0.6/trexmodel/models/datastore/customer_model_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,24 +197,25 @@
                             'count'             : len(redeem_info_list), 
                             
                             }
         customer_entitled_voucher_summary[merchant_voucher_key] = voucher_summary
 
     return customer_entitled_voucher_summary
 
-def update_customer_entiteld_voucher_summary_after_reverted_voucher(customer_entitled_voucher_summary, reverted_customer_voucher):
+
+def update_customer_entiteld_voucher_summary_after_removed_voucher(customer_entitled_voucher_summary, removed_customer_voucher):
     '''
     removed entitled voucher from customer entitled voucher summary 
     '''
     logger.debug('customer_entitled_voucher_summary=%s', customer_entitled_voucher_summary)
     
     
     if customer_entitled_voucher_summary:
-        merchant_voucher_key                    = reverted_customer_voucher.entitled_voucher_key
-        redeem_code_of_reverting_voucher        = reverted_customer_voucher.redeem_code
+        merchant_voucher_key                    = removed_customer_voucher.entitled_voucher_key
+        redeem_code_of_reverting_voucher        = removed_customer_voucher.redeem_code
         
         logger.debug('merchant_voucher_key=%s', merchant_voucher_key)
         logger.debug('redeem_code_of_reverting_voucher=%s', redeem_code_of_reverting_voucher)
         
         voucher_summary = customer_entitled_voucher_summary.get(merchant_voucher_key)
         
         logger.debug('voucher_summary=%s', voucher_summary)
@@ -231,17 +232,21 @@
                 del customer_entitled_voucher_summary[merchant_voucher_key]
             else:
                 customer_entitled_voucher_summary[merchant_voucher_key]['redeem_info_list'] = new_redeem_info_list
                 customer_entitled_voucher_summary[merchant_voucher_key]['count']            = len(new_redeem_info_list)
                 
     return customer_entitled_voucher_summary
     
-    
+
+def update_customer_entiteld_voucher_summary_after_reverted_voucher(entitled_voucher_summary, reverted_customer_voucher):
+    return update_customer_entiteld_voucher_summary_after_removed_voucher(entitled_voucher_summary, reverted_customer_voucher)
+
 def update_customer_entiteld_voucher_summary_after_redeemed_voucher(entitled_voucher_summary, redeemed_customer_voucher):
-    return update_customer_entiteld_voucher_summary_after_reverted_voucher(entitled_voucher_summary, redeemed_customer_voucher)
+    return update_customer_entiteld_voucher_summary_after_removed_voucher(entitled_voucher_summary, redeemed_customer_voucher)
+
 
 ''' --------------- End: Update reward summary for voucher--------------'''
 
 ''' --------------- Start: Update reward summary for prepaid--------------'''
 
 def update_prepaid_summary_with_new_prepaid(existing_prepaid_summary, new_prepaid_summary):
     prepaid_amount              = new_prepaid_summary.get('amount')
```

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/customer_models.py` & `trex-model-1.0.6/trexmodel/models/datastore/customer_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 from trexlib.utils.common.date_util import convert_date_to_datetime,\
     to_day_of_year
 from trexmodel import conf, program_conf
 from six import string_types
 from datetime import datetime, timedelta
 from trexmodel.models.datastore.membership_models import MerchantTierMembership,\
     MerchantMembership
+from trexmodel.models.datastore.customer_model_helpers import update_customer_entiteld_voucher_summary_after_removed_voucher,\
+    update_customer_entiteld_voucher_summary_with_customer_new_voucher
     
 
 logger = logging.getLogger('model')
 
 
 class Customer(BaseNModel, DictModel, FullTextSearchable):
     '''
@@ -62,22 +64,23 @@
     previous_tier_membership    = ndb.KeyProperty(name="previous_tier_membership", kind=MerchantTierMembership)
     
     reward_summary                              = ndb.JsonProperty()
     prepaid_summary                             = ndb.JsonProperty()
     entitled_voucher_summary                    = ndb.JsonProperty()
     entitled_birthday_reward_summary            = ndb.JsonProperty()
     entitled_membership_reward_summary          = ndb.JsonProperty()
+    entitled_lucky_draw_ticket_summary          = ndb.JsonProperty(required=False)
     
     kpi_summary                         = ndb.JsonProperty()
     
     fulltextsearch_field_name           = 'name'
     
     dict_properties     = ['name', 'mobile_phone', 'email', 'gender', 'birth_date', 'reference_code', 'merchant_reference_code',  
                            'tags_list', 'memberships_list', 'registered_merchant_acct', 'entitled_membership_reward_summary',
-                           'reward_summary', 'entitled_voucher_summary', 'prepaid_summary', 'kpi_summary', 
+                           'reward_summary', 'entitled_voucher_summary', 'prepaid_summary', 'kpi_summary', 'entitled_lucky_draw_ticket_summary',
                            'entitled_birthday_reward_summary', 'tier_membership_key',
                            'registered_outlet_key', 'registered_merchant_acct_key', 'registered_datetime', 'modified_datetime']
     
     @property
     def registered_user_acct_key(self):
         return self.key.parent().urlsafe().decode('utf-8')
     
@@ -155,14 +158,90 @@
     def update_tier_membership(customer_acct, new_tier_membership):
         if customer_acct.tier_membership is not None:
             customer_acct.previous_tier_membership  = customer_acct.tier_membership
         
         customer_acct.tier_membership           = new_tier_membership.create_ndb_key()
         customer_acct.put()        
     
+    @staticmethod
+    def add_new_tickets_list_into_lucky_draw_ticket_summary(customer_acct, new_entitled_draw_tickets_list):
+        
+        logger.debug('new_entitled_draw_tickets_list=%s', new_entitled_draw_tickets_list)
+        
+        entitled_lucky_draw_ticket_summary = {}
+        if customer_acct.entitled_lucky_draw_ticket_summary:
+            entitled_lucky_draw_ticket_summary = customer_acct.entitled_lucky_draw_ticket_summary
+        
+        entitled_tickets_list = entitled_lucky_draw_ticket_summary.get('tickets') or []
+        
+        tickets_to_update_list = []
+        
+        #check before add
+        for new_ticket in new_entitled_draw_tickets_list:
+            check_ticket = next((obj for obj in entitled_tickets_list if obj.get('ticket_key') == new_ticket.get('ticket_key')), None)
+            if check_ticket is None:
+                logger.debug('Cannot find ticket, thus going to add ticket')
+                tickets_to_update_list.append(new_ticket)
+            else:
+                logger.debug('Found ticket, thus ignore to avoid duplicated ticket')
+                continue
+        
+        entitled_tickets_list.extend(tickets_to_update_list)
+        
+        entitled_lucky_draw_ticket_summary['tickets']    = entitled_tickets_list
+        entitled_lucky_draw_ticket_summary['count']      = len(entitled_tickets_list)
+        
+        customer_acct.entitled_lucky_draw_ticket_summary = entitled_lucky_draw_ticket_summary
+         
+        
+        customer_acct.put()
+        
+    @staticmethod
+    def update_ticket_into_lucky_draw_ticket_summary(customer_acct, updated_draw_ticket):
+        entitled_lucky_draw_ticket_summary = {}
+        if customer_acct.entitled_lucky_draw_ticket_summary:
+            entitled_lucky_draw_ticket_summary = customer_acct.entitled_lucky_draw_ticket_summary
+        
+        draw_tickets_list = entitled_lucky_draw_ticket_summary.get('tickets') or []
+        
+        new_tickets_list = []
+        
+        for ticket in draw_tickets_list:
+            if ticket.get('ticket_key')!=updated_draw_ticket.get('ticket_key'):
+                new_tickets_list.append(ticket)
+            else:
+                new_tickets_list.append(updated_draw_ticket)
+                
+        customer_acct.entitled_lucky_draw_ticket_summary['tickets'] = new_tickets_list
+        customer_acct.put()
+        
+    @staticmethod
+    def remove_ticket_from_lucky_draw_ticket_summary(customer_acct, removed_draw_ticket):
+        entitled_lucky_draw_ticket_summary = {}
+        if customer_acct.entitled_lucky_draw_ticket_summary:
+            entitled_lucky_draw_ticket_summary = customer_acct.entitled_lucky_draw_ticket_summary
+        
+        draw_tickets_list = entitled_lucky_draw_ticket_summary.get('tickets') or []
+        
+        new_tickets_list = []
+        
+        for ticket in draw_tickets_list:
+            if ticket.get('ticket_key')!=removed_draw_ticket.get('ticket_key'):
+                new_tickets_list.append(ticket)
+            
+                
+        customer_acct.entitled_lucky_draw_ticket_summary['tickets'] = new_tickets_list
+        customer_acct.entitled_lucky_draw_ticket_summary['count']   = len(new_tickets_list)
+        customer_acct.put()    
+        
+    @staticmethod
+    def update_tickets_list_into_lucky_draw_ticket_summary(customer_acct, tickets_list):
+        for ticket in tickets_list:
+            ticket.patch_prize_image_base_url()
+            Customer.update_ticket_into_lucky_draw_ticket_summary(customer_acct, ticket.to_configuration())
     @classmethod
     def get_by_reference_code(cls, reference_code, merchant_acct):
         return cls.query(ndb.AND(cls.reference_code==reference_code, cls.merchant_acct==merchant_acct.create_ndb_key())).get()
     
     @classmethod
     def get_by_merchant_reference_code(cls, merchant_reference_code, merchant_acct):
         return cls.query(ndb.AND(cls.merchant_reference_code==merchant_reference_code, cls.merchant_acct==merchant_acct.create_ndb_key())).get()
@@ -563,15 +642,25 @@
                     
                         entitled_membership_yearly_reward_summary[year_str] = this_year_entitled_membership_reward_summary
                         entitled_membership_reward_summary['yearly']        = entitled_membership_yearly_reward_summary    
                     
         if is_membership_reward_has_been_given==False:
             customer_acct.entitled_membership_reward_summary  = entitled_membership_reward_summary
             customer_acct.put()
-
+    
+    def update_after_removed_voucher(self, removed_voucher):
+        entitled_voucher_summary = self.entitled_voucher_summary
+        update_customer_entiteld_voucher_summary_after_removed_voucher(entitled_voucher_summary, removed_voucher)
+        self.put()
+        
+    def update_after_added_voucher(self, added_voucher):
+        entitled_voucher_summary = self.entitled_voucher_summary
+        update_customer_entiteld_voucher_summary_with_customer_new_voucher(entitled_voucher_summary, added_voucher)
+        self.put()    
+    
 class CustomerMembership(BaseNModel, DictModel):
     '''
     parent is Customer
     '''
     
     merchant_acct               = ndb.KeyProperty(name="merchant_acct", kind=MerchantAcct)
     merchant_membership         = ndb.KeyProperty(name="merchant_membership", kind=MerchantMembership)
```

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/fb_subsriber_models.py` & `trex-model-1.0.6/trexmodel/models/datastore/fb_subsriber_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/inventory_model.py` & `trex-model-1.0.6/trexmodel/models/datastore/inventory_model.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/loyalty_models.py` & `trex-model-1.0.6/trexmodel/models/datastore/loyalty_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     device_id               = ndb.StringProperty(required=False)
     activated               = ndb.BooleanProperty(required=True, default=False)
     assigned_outlet         = ndb.KeyProperty(name="assigned_outlet", kind=Outlet)
     created_datetime        = ndb.DateTimeProperty(required=True, auto_now_add=True)
     activated_datetime      = ndb.DateTimeProperty(required=False)
     testing                 = ndb.BooleanProperty(required=False, default=False)
     
-    dict_properties = ['device_name', 'activation_code', 'device_id', 'activated', 'assigned_outlet_key', 'activated_datetime', 'created_datetime']
+    dict_properties = ['device_name', 'activation_code', 'device_id', 'activated', 'assigned_outlet_key', 
+                       'activated_datetime', 'created_datetime']
     
     @property
     def is_test_setting(self):
         return self.testing
     
     @property
     def assigned_outlet_key(self):
```

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/membership_models.py` & `trex-model-1.0.6/trexmodel/models/datastore/membership_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,17 +49,14 @@
     def merchant_acct(self):
         return MerchantAcct.fetch(self.key.parent().urlsafe())
     
     @classmethod
     def list_by_merchant_acct(cls, merchant_acct, is_archived=False):
         return cls.query(ndb.AND(MerchantMembership.archived == is_archived), ancestor=merchant_acct.create_ndb_key()).fetch(limit=model_conf.MAX_FETCH_RECORD)
     
-    
-    
-        
     def calc_expiry_date(self, start_date=None):
         
         if start_date is None:
             start_date = datetime.utcnow()
         
         logger.debug('start_date=%s', start_date)
         logger.debug('self.expiration_type=%s', self.expiration_type)
```

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/merchant_models.py` & `trex-model-1.0.6/trexmodel/models/datastore/merchant_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,26 +67,29 @@
     membership_configuration                = ndb.JsonProperty()
     tier_membership_configuration           = ndb.JsonProperty()
     
     reward_naming_configuration             = ndb.JsonProperty()
     
     prepaid_configuration                   = ndb.JsonProperty()
     
+    lucky_draw_configuration                = ndb.JsonProperty(required=False)
+    
     product_modifier_configuration          = ndb.JsonProperty()
     
     program_settings                        = ndb.JsonProperty()
     
     stat_figure_update_interval_in_minutes  = conf.MERCHANT_STAT_FIGURE_UPDATE_INTERVAL_IN_MINUTES
     stat_figure_update_datetime_format      = '%d-%m-%Y %H:%M:%S'
     
     dict_properties = ['company_name', 'brand_name', 'contact_name', 'business_reg_no', 'mobile_phone', 'office_phone', 'fax_phone', 'email', 'account_code', 'country',
                        'registered_datetime', 'modified_datetime', 'plan_start_date', 'plan_end_date', 'currency_code', 
                        'published_program_configuration', 'published_voucher_configuration', 'membership_configuration', 
-                       'tier_membership_configuration', 'prepaid_configuration', 'product_modifier_configuration',
-                       'dashboard_stat_figure', 'program_settings', 'is_tier_membership_configured', 'website',
+                       'tier_membership_configuration', 'prepaid_configuration', 'lucky_draw_configuration', 'product_modifier_configuration',
+                       'dashboard_stat_figure', 'program_settings', 'is_tier_membership_configured', 'website', 
+                       
                        ]
     
     
     def to_login_dict(self):
         return {
                 'account_code'      : self.account_code,
                 'plan_end_date'     : self.plan_end_date,
@@ -102,14 +105,17 @@
             return []
     
     
     @property
     def is_tier_membership_configured(self):
         return is_not_empty(self.tier_membership_configuration)
     
+    @property
+    def image_default_base_url(self):
+        return program_conf.IMAGE_BASE_URL
     
     @property
     def days_of_return_policy(self):
         return self.program_settings.get('days_of_return_policy') or MerchantAcct.default_program_settings().get('days_of_return_policy')
     
     @property
     def days_of_repeat_purchase_measurement(self):
@@ -119,23 +125,74 @@
     def membership_renew_advance_day(self):
         return self.program_settings.get('membership_renew_advance_day') or MerchantAcct.default_program_settings().get('membership_renew_advance_day')
     
     @property
     def membership_renew_late_day(self):
         return self.program_settings.get('membership_renew_late_day') or MerchantAcct.default_program_settings().get('membership_renew_late_day')
     
+    
+    
+    @property
+    def lucky_draw_program_count(self):
+        if self.lucky_draw_configuration:
+            if self.lucky_draw_configuration.get('count'):
+                return self.lucky_draw_configuration.get('count')
+        return 0
+    
+    @property
+    def lucky_draw_ticket_is_recurring_scheme(self):
+        if self.lucky_draw_configuration.get('settings')  and self.lucky_draw_configuration.get('settings').get('is_recurring_scheme'):
+            return self.lucky_draw_configuration.get('is_recurring_scheme')
+        else:
+            return False
+            
+    @property
+    def lucky_draw_ticket_spending_currency(self):
+        if self.lucky_draw_configuration.get('settings') and self.lucky_draw_configuration.get('settings').get('spending_currency'):
+            return self.lucky_draw_configuration.get('settings').get('spending_currency')
+        else:
+            return 0
+    
+    @property
+    def lucky_draw_ticket_limit_type(self):
+        if self.lucky_draw_configuration.get('settings'):
+            return self.lucky_draw_configuration.get('settings').get('ticket_limit_type') or program_conf.REWARD_LIMIT_TYPE_NO_LIMIT
+        else:
+            return program_conf.REWARD_LIMIT_TYPE_NO_LIMIT
+            
+    
+    @property
+    def lucky_draw_ticket_limit_amount(self):
+        if self.lucky_draw_configuration.get('settings'):
+            return self.lucky_draw_configuration.get('settings').get('ticket_limit_amount')
+        
+        return 0
+    
+    @property
+    def lucky_draw_ticket_expiry_date_length_in_day(self):
+        if self.lucky_draw_configuration.get('settings'):
+            return self.lucky_draw_configuration.get('settings').get('ticket_expiry_date_length_in_day')
+        
+        return 0
+    
+    @property
+    def lucky_draw_ticket_image_url(self):
+        if self.lucky_draw_configuration.get('settings'):
+            return self.lucky_draw_configuration['settings']['ticket_image_url']
+    
     @staticmethod
     def default_program_settings():
         return {
                 'days_of_return_policy'                 : 3,
                 'days_of_repeat_purchase_measurement'   : 7,
                 'membership_renew_advance_day'          : 7,
                 'membership_renew_late_day'             : 30,
-                }   
-    
+                
+                }
+        
     
     @staticmethod
     def update_details(merchant_acct, company_name=None, brand_name=None, business_reg_no=None, contact_name=None, 
                        email=None, mobile_phone=None, office_phone=None, currency_code=None, country=None, website=None):
         merchant_acct.company_name      = company_name
         merchant_acct.brand_name        = brand_name
         merchant_acct.business_reg_no   = business_reg_no
@@ -359,14 +416,56 @@
             existing_prepaid_program_list.append(prepaid_configuration)
             
             self.prepaid_configuration['programs']        = existing_prepaid_program_list
             self.prepaid_configuration['count']           = len(existing_prepaid_program_list) 
             
         self.put()
         
+    def update_lucky_draw_program(self, lucky_draw_configuration):
+        logger.debug('update_lucky_draw_program debug: lucky_draw_configuration = %s', lucky_draw_configuration)
+        if self.lucky_draw_configuration is None or len(self.lucky_draw_configuration)==0:
+            self.lucky_draw_configuration = {
+                                                'programs'  :[lucky_draw_configuration],
+                                                'count'     : 1,
+                                                } 
+                                                
+        existing_lucky_draw_list  = self.lucky_draw_configuration.get('programs')
+        
+        program_key = lucky_draw_configuration.get('program_key')
+        
+        index = 0
+        for v in existing_lucky_draw_list:
+            if v.get('program_key') == program_key:
+                existing_lucky_draw_list.pop(index)
+            
+            index = index+1
+        
+        existing_lucky_draw_list.append(lucky_draw_configuration)
+        
+        self.lucky_draw_configuration['programs']        = existing_lucky_draw_list
+        self.lucky_draw_configuration['count']           = len(existing_lucky_draw_list) 
+            
+        self.put()    
+        
+    def update_lucky_draw_program_settings(self, lucky_draw_program_settings):
+        logger.debug('update_lucky_draw_program_settings debug: lucky_draw_program_settings = %s', lucky_draw_program_settings)
+        if self.lucky_draw_configuration is None or len(self.lucky_draw_configuration)==0:
+            self.lucky_draw_configuration = {'settings':{}}
+            
+        self.lucky_draw_configuration['settings'] = lucky_draw_program_settings
+        self.put()
+        
+    def update_lucky_draw_ticket_image(self, ticket_image_url):
+        if self.lucky_draw_configuration is None or len(self.lucky_draw_configuration)==0:
+            self.lucky_draw_configuration = {'settings':{}}
+            
+        self.lucky_draw_configuration['settings']['ticket_image_url'] = ticket_image_url
+        self.put()    
+        
+        
     def update_product_modifier(self, product_modifier_configuration):
         if self.product_modifier_configuration is None or len(self.product_modifier_configuration)==0:
             self.product_modifier_configuration = {
                                                 'modifiers'  :[product_modifier_configuration],
                                                 'count'     : 1,
                                                 } 
                                             
@@ -576,14 +675,51 @@
             logger.debug('program_count after remove=%s', program_count)
             
             self.prepaid_configuration['programs']    = existing_programs_list
             self.prepaid_configuration['count']       = program_count
                 
             self.put() 
             
+    def remove_lucky_draw_program_configuration(self, program_key_to_remove):
+        
+        logger.debug('remove_prepaid_program_configuration: program_key_to_remove=%s', program_key_to_remove)
+        if self.lucky_draw_configuration and self.lucky_draw_configuration.get('programs'):
+            existing_programs_list  = self.lucky_draw_configuration['programs']
+            program_count           = len(existing_programs_list)
+            
+            logger.debug('program_count before remove=%s', program_count)
+            
+            index = 0
+            found = False
+            
+            for program in existing_programs_list:
+                
+                logger.debug('program_key=%s', program.get('program_key'))
+                
+                is_same_program_key = program.get('program_key') == program_key_to_remove
+                
+                logger.debug('is_same_program_key=%s', is_same_program_key)
+                
+                if is_same_program_key:
+                    existing_programs_list.pop(index)
+                    found = True
+                    logger.debug('Found program to be remove')
+                    
+                index = index+1
+            
+            if found:
+                program_count = len(existing_programs_list)
+                
+                logger.debug('program_count after remove=%s', program_count)
+                
+                self.lucky_draw_configuration['programs']    = existing_programs_list
+                self.lucky_draw_configuration['count']       = program_count
+                    
+                self.put()         
+            
     def remove_product_modifier_configuration(self, modifier_key_to_remove):
         
         logger.debug('remove_product_modifier_configuration: modifier_key_to_remove=%s', modifier_key_to_remove)
         if self.product_modifier_configuration and self.product_modifier_configuration.get('modifiers'):
             existing_product_modifiers_list     = self.product_modifier_configuration['modifiers']
             modifiers_count                     = len(existing_product_modifiers_list)
             
@@ -1142,19 +1278,19 @@
     receipt_footer_settings = ndb.JsonProperty()
     modified_datetime       = ndb.DateTimeProperty(auto_now=True)
     
     
     dict_properties = ['receipt_header_settings', 'receipt_footer_settings']
     
     @staticmethod
-    def create(merchant_acct, receipt_header_settings={}):
+    def create(merchant_acct, receipt_header_settings={}, receipt_footer_settings={}):
         receipt_setup = ReceiptSetup(
                                         parent                  = merchant_acct.create_ndb_key(),
                                         receipt_header_settings = receipt_header_settings,    
-                                        receipt_footer_settings = {},
+                                        receipt_footer_settings = receipt_footer_settings,
                                         )
         receipt_setup.put() 
         
         return receipt_setup
     
     @staticmethod
     def update(receipt_setup, receipt_header_settings={}, receipt_footer_settings={}):
```

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/model_decorators.py` & `trex-model-1.0.6/trexmodel/models/datastore/model_decorators.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/ndb_models.py` & `trex-model-1.0.6/trexmodel/models/datastore/ndb_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/pos_models.py` & `trex-model-1.0.6/trexmodel/models/datastore/pos_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,16 @@
     activated               = ndb.BooleanProperty(required=True, default=False)
     assigned_outlet         = ndb.KeyProperty(name="assigned_outlet", kind=Outlet)
     #assigned_catalogue      = ndb.KeyProperty(name="assigned_outlet", kind=ProductCatalogue)
     created_datetime        = ndb.DateTimeProperty(required=True, auto_now_add=True)
     activated_datetime      = ndb.DateTimeProperty(required=False)
     testing                 = ndb.BooleanProperty(required=False, default=False)
     
-    dict_properties = ['device_name', 'activation_code', 'device_id', 'activated', 'assigned_outlet_key', 'activated_datetime', 'created_datetime']
+    dict_properties = ['device_name', 'activation_code', 'device_id', 'activated', 'assigned_outlet_key', 
+                       'activated_datetime', 'created_datetime']
     
     @property
     def is_test_setting(self):
         return self.testing
     
     @property
     def assigned_outlet_key(self):
@@ -118,15 +119,15 @@
                         POSSetting.assigned_outlet==assigned_outlet.create_ndb_key()
                         ),ancestor=merchant_acct.create_ndb_key())
         
         return POSSetting.count_with_condition_query(query)
         
     def activate(self, device_id):
         self.device_id          = device_id
-        #self.activated          = True
+        self.activated          = True
         self.activated_datetime = datetime.utcnow()
         self.put()
         
         
     @staticmethod
     def remove_by_activation_code(activation_code):
         checking_pos_setting = POSSetting.get_by_activation_code(activation_code)
```

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/prepaid_models.py` & `trex-model-1.0.6/trexmodel/models/datastore/prepaid_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/product_models.py` & `trex-model-1.0.6/trexmodel/models/datastore/product_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/program_models.py` & `trex-model-1.0.6/trexmodel/models/datastore/program_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,16 @@
     @property
     def is_reward_amount_required(self):
         return self.reward_format in (program_conf.REWARD_FORMAT_POINT, program_conf.REWARD_FORMAT_STAMP)
     
     @property
     def is_recurring_scheme(self):
         if self.program_settings and self.program_settings.get('scheme'):
-            return self.program_settings.get('scheme').get('is_recurring_scheme') or True
+            return self.program_settings.get('scheme').get('is_recurring_scheme')
+        return False
         
     @property
     def giveaway_system_condition(self):
         if self.program_settings and self.program_settings.get('giveaway_system_settings'):
             return self.program_settings.get('giveaway_system_settings').get('giveaway_system_condition')
         
     @property
@@ -154,15 +155,15 @@
                 modified_by_username = modified_by.username
         
         program_settings = program.program_settings
         program_settings['exclusivity'] = exclusivity_configuration
             
         program.modified_by            = modified_by.create_ndb_key()
         program.modified_by_username   = modified_by_username
-        program.completed_status       = program_conf.PROGRAM_STATUS_REWARD_EXCLUSIVITY
+        program.completed_status       = program_conf.PROGRAM_STATUS_EXCLUSIVITY
         program.program_settings       = program_settings
         
         program.put()
         
         return program
     
     @classmethod
@@ -190,15 +191,15 @@
     @model_transactional(desc="publish_program")
     def publish_program(cls, program):
         program.completed_status = program_conf.PROGRAM_STATUS_PUBLISH
         program.published_datetime = datetime.now()
         program.put()
         
         merchant_acct = program.merchant_acct
-        merchant_acct.update_published_program(program.to_program_configuration())
+        merchant_acct.update_published_program(program.to_configuration())
         
         cls.__create_schedule_program(merchant_acct, program)
         
     @classmethod
     @model_transactional(desc="archive_program")
     def archive_program(cls, program):
         program.archived = True
@@ -225,15 +226,15 @@
         program.modified_by            = modified_by.create_ndb_key()
         program.modified_by_username   = modified_by_username
         
         program.put()
         
         if program.is_published:
             merchant_acct = program.merchant_acct
-            merchant_acct.update_published_program(program.to_program_configuration())
+            merchant_acct.update_published_program(program.to_configuration())
             
             cls.__create_schedule_program(merchant_acct, program)
             
         
     @classmethod
     @model_transactional(desc="disable program")
     def disable(cls, program, modified_by=None):
@@ -251,15 +252,15 @@
         program.put()  
         
         merchant_acct = program.merchant_acct
         merchant_acct.remove_program_from_published_program_configuration(program.key_in_str)
         
         cls.__remove_schedule_program(program)
         
-    def to_program_configuration(self):
+    def to_configuration(self):
         program_configuration = {
                                 'merchant_acct_key'                 : self.parent_key,
                                 'program_key'                       : self.key_in_str,
                                 'label'                             : self.label,
                                 'desc'                              : self.desc,
                                 'reward_base'                       : self.reward_base,
                                 'reward_format'                     : self.reward_format,
@@ -975,15 +976,15 @@
     
     @staticmethod
     def __create(merchant_acct, schedule_type, merchant_program):
         schedule_program    = MerchantScheduleProgram(
                                 parent                  = merchant_acct.create_ndb_key(),
                                 merchant_program        = merchant_program.create_ndb_key(),
                                 schedule_type           = schedule_type,
-                                program_configuration   = merchant_program.to_program_configuration(),
+                                program_configuration   = merchant_program.to_configuration(),
                                 start_date              = merchant_program.start_date,
                                 end_date                = merchant_program.end_date,
                                 
                             )
         
         schedule_program.put()
```

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/redeem_models.py` & `trex-model-1.0.6/trexmodel/models/datastore/redeem_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/reward_models.py` & `trex-model-1.0.6/trexmodel/models/datastore/reward_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,18 @@
     reward_program              = ndb.KeyProperty(name="reward_program", kind=MerchantProgram)
     
     @property
     def entitled_customer_key(self):
         return self.key.parent().urlsafe().decode('utf-8')
     
     @property
+    def entitled_customer_acct(self):
+        return Customer.fetch(self.key.parent().urlsafe())
+    
+    @property
     def reward_program_key(self):
         return self.reward_program.urlsafe().decode('utf-8')
     
     @property
     def rewarded_by_merchant_acct_entity(self):
         return MerchantAcct.fetch(self.merchant_acct.urlsafe())
     
@@ -320,35 +324,43 @@
         self.status = program_conf.REDEEM_STATUS_VALID
         self.redeemed_datetime      = None
         self.redeemed_by            = None
         self.redeemed_by_username   = None
         self.put()
         
     
-    def redeem(self, redeemed_by, redeemed_datetime=None):
+    def redeem(self, redeemed_by=None, redeemed_datetime=None):
         self.status = program_conf.REWARD_STATUS_REDEEMED   
         
         if redeemed_datetime is None:
-            redeemed_datetime = datetime.now()
+            redeemed_datetime = datetime.utcnow()
+        
+        redeemed_by_username = None
+        if redeemed_by:
+            redeemed_by_username = redeemed_by.username
         
         self.redeemed_datetime      = redeemed_datetime
         self.redeemed_by            = redeemed_by.create_ndb_key()
-        self.redeemed_by_username   = redeemed_by.username
+        self.redeemed_by_username   = redeemed_by_username
         self.put()
     
-    def remove(self, removed_by, removed_datetime=None):
+    def remove(self, removed_by=None, removed_datetime=None):
         self.status = program_conf.REWARD_STATUS_REMOVED   
         
         if removed_datetime is None:
-            removed_datetime = datetime.now()
+            removed_datetime = datetime.utcnow()
         
+        removed_by_username = None
+        if removed_by:
+            removed_by_username = removed_by.username
+            
         self.removed_datetime      = removed_datetime
-        self.removed_by_username   = removed_by.username
+        self.removed_by_username   = removed_by_username
         self.put() 
-      
+        
     @property
     def entitled_customer_entity(self):
         return Customer.fetch(self.key.parent().urlsafe()) 
         
     @property
     def is_used(self):
         return self.status == program_conf.REWARD_STATUS_REDEEMED
@@ -421,14 +433,16 @@
                                             rewarded_datetime       = rewarded_datetime,
                                             
                                             user_acct               = customer_acct.registered_user_acct.create_ndb_key(),
                                             )
         
         customer_entiteld_voucher.put()
         
+        #customer_acct.update_after_added_voucher(customer_entiteld_voucher)
+        
         return customer_entiteld_voucher
         
         
     @staticmethod
     def get_by_redeem_code(redeem_code):
         return  CustomerEntitledVoucher.query(CustomerEntitledVoucher.redeem_code==redeem_code).get()
```

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/spending_base_program_model.py` & `trex-model-1.0.6/trexmodel/models/datastore/spending_base_program_model.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/system_models.py` & `trex-model-1.0.6/trexmodel/models/datastore/system_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/task_models.py` & `trex-model-1.0.6/trexmodel/models/datastore/task_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/test_models.py` & `trex-model-1.0.6/trexmodel/models/datastore/test_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/transaction_models.py` & `trex-model-1.0.6/trexmodel/models/datastore/transaction_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,14 @@
     MerchantUser
 import logging
 from trexmodel import conf, program_conf
 from datetime import datetime, timedelta
 from trexmodel.utils.model.model_util import generate_transaction_id
 from trexmodel.models.datastore.membership_models import MerchantMembership,\
     MerchantTierMembership
-from trexmodel.program_conf import REWARD_FORMAT_POINT
-from trexmodel.models.datastore.prepaid_models import CustomerPrepaidReward
-from trexmodel.models.datastore.reward_models import CustomerPointReward,\
-    CustomerStampReward, CustomerEntitledVoucher
 
 logger = logging.getLogger('model')
 
 class SalesTransaction(BaseNModel, DictModel):
     transact_merchant           = ndb.KeyProperty(name="transact_merchant", kind=MerchantAcct)
     transact_outlet             = ndb.KeyProperty(name="transact_outlet", kind=Outlet)
     
@@ -50,23 +46,24 @@
     transact_by_username        = ndb.StringProperty(required=False)
     
     sales_channel               = ndb.StringProperty(required=False)
     
     is_revert                   = ndb.BooleanProperty(required=False, default=False)
     is_sales_transaction        = ndb.BooleanProperty(required=False, default=True)
     allow_to_revert             = ndb.BooleanProperty(required=False, default=True)
+    used                        = ndb.BooleanProperty(required=False, default=False)
     
     reward_expiry_date          = ndb.DateProperty(required=False)
     
     dict_properties         = [
                                'transaction_id', 'invoice_id', 'remarks', 'system_remarks', 'tax_amount', 'transact_amount', 
                                'transact_customer_acct', 'transact_outlet_details', 'transact_merchant_acct',
                                'transact_datetime', 'created_datetime',  'transact_outlet_key', 
                                'is_sales_transaction', 'allow_to_revert', 'reward_expiry_date',
-                               'transact_by', 'transact_by_username', 
+                               'transact_by', 'transact_by_username', 'used',
                                
                                ]
     
     @property
     def transact_customer_key(self):
         return ''
     
@@ -74,14 +71,19 @@
     def transact_merchant_acct(self):
         return MerchantAcct.fetch(self.transact_merchant.urlsafe())
     
     @property
     def transact_outlet_key(self):
         if self.transact_outlet:
             return self.transact_outlet.urlsafe().decode('utf-8')
+        
+    @property
+    def transact_outlet_entity(self):
+        if self.transact_outlet:
+            return Outlet.fetch(self.transact_outlet.urlsafe())    
     
     @property
     def transact_merchant_acct_key(self):
         return self.transact_merchant.urlsafe().decode('utf-8')
 
     @property
     def transact_by_user(self):
@@ -94,19 +96,23 @@
         
     @property
     def after_deduct_tax_sales_amount(self):
         if self.tax_amount:
             return self.transact_amount - self.tax_amount
         else:
             return self.transact_amount
-    
+        
     @classmethod
     def get_by_invoice_id(cls, invoice_id):
         return cls.query(cls.invoice_id==invoice_id).get()
     
+    @classmethod
+    def get_by_transaction_id(cls, transaction_id):
+        return cls.query(cls.transaction_id==transaction_id).get()
+    
     @staticmethod
     def create(transact_amount=.0, tax_amount=.0, invoice_id=None, remarks=None, system_remarks=None,
                transact_outlet=None, transact_by=None, transact_datetime=None, 
                
                ):
         
         transact_by_username = None
@@ -152,24 +158,27 @@
                                 )
         
         customer_transaction.put()
         #customer.put()
         
         return customer_transaction
     
+        
+    
 class CustomerTransaction(SalesTransaction):
     '''
     Customer as ancestor
     '''
     
     
-    entitled_reward_summary     = ndb.JsonProperty()
-    entitled_voucher_summary    = ndb.JsonProperty()
-    entitled_prepaid_summary    = ndb.JsonProperty()
-    entitled_program_summary    = ndb.JsonProperty()
+    entitled_reward_summary             = ndb.JsonProperty()
+    entitled_voucher_summary            = ndb.JsonProperty()
+    entitled_prepaid_summary            = ndb.JsonProperty()
+    entitled_program_summary            = ndb.JsonProperty()
+    entitled_lucky_draw_ticket_summary  = ndb.JsonProperty(required=False)
     
     reward_giveaway_method      = ndb.StringProperty(required=False, default=program_conf.PROGRAM_REWARD_GIVEAWAY_METHOD_SYSTEM)
     
     
     
     is_from_instant_transaction = ndb.BooleanProperty(required=False, default=False)
     
@@ -184,15 +193,15 @@
     
     upgraded_merchant_tier_membership   = ndb.KeyProperty(name="upgraded_merchant_tier_membership", kind=MerchantTierMembership)
     
     purchased_merchant_membership        = ndb.KeyProperty(name="purchased_merchant_membership", kind=MerchantMembership)
     purchased_customer_membership        = ndb.KeyProperty(name="purchased_customer_membership", kind=CustomerMembership)
     
     dict_properties         = ['transaction_id', 'invoice_id', 'remarks', 'system_remarks', 'tax_amount', 'transact_amount', 'reward_giveaway_method',
-                               'entitled_reward_summary', 'entitled_voucher_summary', 'entitled_prepaid_summary', 
+                               'entitled_reward_summary', 'entitled_voucher_summary', 'entitled_prepaid_summary', 'entitled_lucky_draw_ticket_summary',
                                'transact_customer_acct', 'transact_outlet_details', 'transact_merchant_acct',
                                'transact_datetime', 'created_datetime',  'transact_outlet_key', 'is_revert', 'reverted_datetime', 'reverted_by_username',
                                'transact_by', 'transact_by_username', 'is_reward_redeemed', 'is_sales_transaction', 'allow_to_revert',
                                'is_membership_purchase', 'purchased_merchant_membership_key', 'is_tier_membership_upgraded', 'upgraded_merchant_tier_membership_key',
                                ]
     
     def to_transaction_details_json(self):
@@ -254,14 +263,22 @@
             return CustomerMembership.fetch(self.purchased_customer_membership.urlsafe())
     
     @property
     def upgraded_merchant_tier_membership_key(self):
         if self.upgraded_merchant_tier_membership:
             return self.upgraded_merchant_tier_membership.urlsafe().decode('utf-8')
     
+    def update_entitled_lucky_draw_ticket_summary(self, entitled_lucky_draw_entries_list):
+        if self.entitled_lucky_draw_ticket_summary is None:
+            self.entitled_lucky_draw_ticket_summary = {}
+        
+        self.entitled_lucky_draw_ticket_summary['entries']   = entitled_lucky_draw_entries_list
+        self.entitled_lucky_draw_ticket_summary['count']     = len(entitled_lucky_draw_entries_list)
+        self.put()
+    
     @staticmethod
     def update_transaction_reward_have_been_redeemed(transaction_id, redeem_transaction_id, redeem_voucher_details_dict=None):
         
         logger.debug('Update customer transaction reward have been redeemed by transaction id=%s', transaction_id)
         
         if transaction_id:
             customer_transaction = CustomerTransaction.get_by_transaction_id(transaction_id)
@@ -299,14 +316,51 @@
         return CustomerTransaction.create_system_transaction(customer, remarks=remarks, system_remarks=system_remarks, transact_outlet=transact_outlet, transact_by=transact_by, 
                                    transact_datetime=transact_datetime, reward_giveaway_method=program_conf.PROGRAM_REWARD_GIVEAWAY_METHOD_MANUAL,
                                    is_sales_transaction = is_sales_transaction, allow_to_revert=allow_to_revert, 
                                    is_membership_purchase=is_membership_purchase, is_membership_renew=is_membership_renew,
                                    )    
     
     @staticmethod
+    def create_from_sales_transaction(customer, sales_transaction):
+        if sales_transaction:
+            customer_transaction = CustomerTransaction(
+                                                        parent                          = customer.create_ndb_key(),
+                                                        
+                                                        transact_merchant               = customer.registered_merchant_acct.create_ndb_key(),
+                                                        transact_outlet                 = sales_transaction.transact_outlet,
+                                                        
+                                                        tax_amount                      = sales_transaction.tax_amount,
+                                                        transact_amount                 = sales_transaction.transact_amount,
+                                                        
+                                                        transaction_id                  = sales_transaction.transaction_id,
+                                                        invoice_id                      = sales_transaction.invoice_id,
+                                                        remarks                         = sales_transaction.remarks,
+                                                        system_remarks                  = sales_transaction.system_remarks,
+                                                        
+                                                        transact_by                     = sales_transaction.transact_by,
+                                                        transact_by_username            = sales_transaction.transact_by_username,
+                                                        
+                                                        transact_datetime               = sales_transaction.transact_datetime,
+                                                        is_from_instant_transaction     = True,
+                                                        
+                                                        #is_sales_transaction            = True,
+                                                        #allow_to_revert                 = True,
+                                                        #is_membership_purchase          = False,
+                                                        #is_membership_renew             = False,
+                                                        #purchased_merchant_membership   = False,
+                                                        #purchased_customer_membership   = False,
+                                                        )
+        
+        
+            customer_transaction.put()
+            sales_transaction.used = True
+            sales_transaction.put()
+            return customer_transaction
+    
+    @staticmethod
     def create_system_transaction(customer, transact_amount=.0, tax_amount=.0, invoice_id=None, remarks=None, system_remarks=None,
                transact_outlet=None, transact_by=None, transact_datetime=None, reward_giveaway_method=program_conf.PROGRAM_REWARD_GIVEAWAY_METHOD_SYSTEM,
                is_sales_transaction = False, allow_to_revert=True, is_membership_purchase=False, is_membership_renew=False, purchased_customer_membership=None,
                ):
         
         transact_by_username = None
```

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/user_models.py` & `trex-model-1.0.6/trexmodel/models/datastore/user_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,23 @@
         
         is_signin_password_valid = hashed_signin_password == self.password
         
         logger.debug('is_valid_password: is_signin_password_valid=%s', is_signin_password_valid)
         
         return is_signin_password_valid
     
+    def change_password(self, new_password):
+        hashed_new_password = hash_password(self.user_id, new_password)
+        
+        logger.debug('change_password: new_password=%s', new_password)
+        logger.debug('change_password: hashed_new_password=%s', hashed_new_password)
+        
+        self.password = hashed_new_password 
+        self.put()
+    
 class Role(BaseNModel):
     id              = ndb.StringProperty(required=True)
     name            = ndb.StringProperty(required=True)
     description     = ndb.TextProperty(required=False)
 
 
 class UserBase(UserMin):
@@ -161,15 +170,15 @@
     @classmethod
     def get_by_reset_password_token(cls, request_reset_password_token):
         return User.query(ndb.AND(User.request_reset_password_token==request_reset_password_token)).get()
     
     @classmethod
     def create(cls, name=None, email=None, mobile_phone=None, 
                gender=None, birth_date=None, 
-               password=None, create_email_vc=False, create_mobile_phone_vc=False):
+               password=None, is_email_verified=True, is_mobile_phone_verified=False):
         
         user_id             = generate_user_id()
         reference_code      = random_number(16) 
         birth_date_date_str = None
         birth_day_in_year   = 0
         
         if birth_date:
@@ -183,22 +192,26 @@
                            gender=gender, birth_date=birth_date, birth_date_date_str=birth_date_date_str,  birth_day_in_year=birth_day_in_year,
                            reference_code=reference_code
                            )
         
         hashed_password = hash_password(user_id, password)
         created_user.password = hashed_password
         
-        if create_email_vc:
+        
+        created_user.is_email_verified          = is_email_verified
+        created_user.is_mobile_phone_verified   = is_mobile_phone_verified
+        
+        if is_email_verified==False:
             created_user.email_vc                               = random_number(6)
             created_user.email_vc_expiry_datetime               = datetime.now() + timedelta(minutes=10)
         
-        if create_mobile_phone_vc:
+        if is_mobile_phone_verified==False:
             created_user.mobile_phone_vc                        = random_number(6)
-            created_user.mobile_phone_vc_expiry_datetime        = datetime.now() + timedelta(minutes=10)   
-            
+            created_user.mobile_phone_vc_expiry_datetime        = datetime.now() + timedelta(minutes=10)
+        
         created_user.put()
         
         return created_user
     
     @classmethod
     def update(cls, user_acct=None, **kwargs):
         logger.debug('**kwargs=%s', kwargs)
@@ -268,19 +281,20 @@
     def mark_mobile_phone_verified(self):
         self.is_mobile_phone_verified = True
         self.mobile_phone_verified_datetime = datetime.utcnow()
         self.put()    
     
     def reset_email_vc(self):
         self.email_vc = random_number(6)
-        self.email_vc_expiry_datetime = datetime.utcnow() + timedelta(minutes=10)
+        self.email_vc_expiry_datetime = datetime.utcnow() + timedelta(minutes=2)
         self.put() 
         
     def reset_mobile_phone_vc(self):
-        self.email_vc = random_number(6)
+        self.mobile_phone_vc = random_number(6)
+        #self.mobile_phone_vc_expiry_datetime = datetime.utcnow() + timedelta(minutes=10)
         self.mobile_phone_vc_expiry_datetime = datetime.utcnow() + timedelta(minutes=10)  
         self.put()   
         
 class User(UserBase):
     redeem_pin               = ndb.StringProperty(required=False)
     
     dict_properties            = [
```

### Comparing `trex-model-1.0.4/trexmodel/models/datastore/voucher_models.py` & `trex-model-1.0.6/trexmodel/models/datastore/voucher_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.4/trexmodel/models/merchant_helpers.py` & `trex-model-1.0.6/trexmodel/models/merchant_helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,67 @@
 from trexmodel.models.datastore.pos_models import InvoiceNoGeneration,\
     RoundingSetup, DinningOption, PosPaymentMethod
-from trexmodel.models.datastore.merchant_models import ReceiptSetup
+from trexmodel.models.datastore.merchant_models import ReceiptSetup, Outlet,\
+    BannerFile
+
+def construct_merchant_acct_info(merchant_acct):
+    account_settings        = {
+                                'account_code'  : merchant_acct.account_code,
+                                'currency'      : merchant_acct.currency_code,
+                                'locale'        : merchant_acct.locale,    
+                                }
+    
+    outlet_list = Outlet.list_by_merchant_acct(merchant_acct)
+    outlet_json_list = []
+    for o in outlet_list:
+        outlet_json_list.append(construct_outlet_info(o))
+        
+    
+    banner_file_listing =  BannerFile.list_by_merchant_acct(merchant_acct)
+    banner_listing = []
+    if banner_file_listing:
+        for banner_file in banner_file_listing:
+            banner_listing.append(banner_file.banner_file_public_url)
+        
+        
+    invoice_no_generation   = InvoiceNoGeneration.getByMerchantAcct(merchant_acct)
+    
+    if invoice_no_generation:
+        account_settings['invoice_settings']    = {
+                                                     'invoice_no_generators'    : invoice_no_generation.generators_list,
+                                                                     
+                                                    }
+    
+    info =  {
+                'key'                               : merchant_acct.key_in_str,
+                'company_name'                      : merchant_acct.company_name,
+                'brand_name'                        : merchant_acct.brand_name,
+                'website'                           : merchant_acct.website,
+                'account_id'                        : merchant_acct.key_in_str,
+                'api_key'                           : merchant_acct.api_key,
+                'logo_image_url'                    : merchant_acct.logo_public_url,
+                'image_default_base_url'            : merchant_acct.image_default_base_url,
+                'account_settings'                  : account_settings,
+                'outlets'                           : outlet_json_list,
+                'banners'                           : banner_listing,
+                } 
+    return info
+
+def construct_outlet_info(outlet):
+    geo_location = None
+    if outlet.geo_location:
+        geo_location = '%s,%s' % (outlet.geo_location.latitude, outlet.geo_location.longitude)
+    return {
+            'outlet_key'        : outlet.key_in_str,
+            'outlet_name'       : outlet.name,
+            'address'           : outlet.address,
+            'business_hour'     : outlet.business_hour,
+            'geo_location'      : geo_location,
+            
+        }
 
 def construct_setting_by_outlet(outlet, device_setting=None):
 
 
     merchant_acct           = outlet.merchant_acct_entity
     invoice_no_generation   = InvoiceNoGeneration.getByMerchantAcct(merchant_acct)
     rounding_setup          = RoundingSetup.get_by_merchant_acct(merchant_acct)
@@ -92,14 +149,15 @@
     program_configurations = {
                             'prepaid_configuration' : merchant_acct.prepaid_configuration,
                             'days_of_return_policy' : merchant_acct.program_settings.get('days_of_return_policy'),
                             }
     
     setting =  {
                 'company_name'                      : merchant_acct.company_name,
+                'brand_name'                        : merchant_acct.brand_name,
                 'website'                           : merchant_acct.website,
                 'account_id'                        : merchant_acct.key_in_str,
                 'api_key'                           : merchant_acct.api_key,
                 'logo_image_url'                    : merchant_acct.logo_public_url,
                 'account_settings'                  : account_settings,
                 'outlet_details'                    : outlet_details,
                 'program_configurations'            : program_configurations,
```

### Comparing `trex-model-1.0.4/trexmodel/program_conf.py` & `trex-model-1.0.6/trexmodel/program_conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 Created on 19 Feb 2021
 
 @author: jacklok
 '''
 #from orderedset import OrderedSet
 #from trexlib.utils.common.common_util import OrderedSet
 
+import os
+
+IMAGE_BASE_URL                          = os.environ.get('IMAGE_BASE_URL')
+
 REWARD_BASE_ON_VISIT                    = 'visit'
 REWARD_BASE_ON_SPENDING                 = 'spending'
 REWARD_BASE_ON_REFER                    = 'refer'
 REWARD_BASE_ON_GIVEAWAY                 = 'giveaway'
 REWARD_BASE_ON_BIRTHDAY                 = 'birthday'
 REWARD_BASE_ON_TIER                     = 'tier'
 
@@ -24,15 +28,15 @@
 REWARD_FORMAT_POINT                     = 'point'
 REWARD_FORMAT_STAMP                     = 'stamp'
 REWARD_FORMAT_CASH                      = 'cash'
 REWARD_FORMAT_VOUCHER                   = 'voucher'
 REWARD_FORMAT_DISCOUNT                  = 'discount'
 REWARD_FORMAT_MIXED                     = 'mixed'
 REWARD_FORMAT_PREPAID                   = 'prepaid'
-
+REWARD_FORMAT_MESSAGE                   = 'message'
 
 SALES_AMOUNT                            = 'sales_amount'
 
 REWARD_FORMAT_SET                       = (REWARD_FORMAT_POINT, REWARD_FORMAT_STAMP, REWARD_FORMAT_CASH, REWARD_FORMAT_VOUCHER, REWARD_FORMAT_MIXED, REWARD_FORMAT_PREPAID)
 BASIC_TYPE_REWARD_FORMAT                = (REWARD_FORMAT_POINT, REWARD_FORMAT_STAMP)
 
 SUPPORT_TIER_REWARD_PROGRAM_CONDITION_REWARD_FORMAT = (REWARD_FORMAT_POINT, REWARD_FORMAT_STAMP)
@@ -44,15 +48,19 @@
 ENTITLE_REWARD_CONDITION_ACCUMULATE_TYPES           = (ENTITLE_REWARD_CONDITION_ACCUMULATE_POINT, ENTITLE_REWARD_CONDITION_ACCUMULATE_STAMP, ENTITLE_REWARD_CONDITION_ACCUMULATE_SALES_AMOUNT)
 
 PROGRAM_STATUS_PROGRAM_BASE             = 'program_base'
 PROGRAM_STATUS_REWARD_SCHEME            = 'reward_scheme'
 PROGRAM_STATUS_REWARD_DETAILS           = 'reward_details'
 PROGRAM_STATUS_DEFINE_TIER              = 'define_program_tier'
 PROGRAM_STATUS_DEFINE_REWARD            = 'define_reward'
-PROGRAM_STATUS_REWARD_EXCLUSIVITY       = 'exclusivity'
+PROGRAM_STATUS_DEFINE_CONDITION         = 'define_condition'
+PROGRAM_STATUS_UPLOAD_TICKET_IMAGE      = 'upload_material'
+PROGRAM_STATUS_DEFINE_PRIZE             = 'define_prize'
+PROGRAM_STATUS_DEFINE_PRIZE_POSSIBILITY = 'define_prize_possibility'
+PROGRAM_STATUS_EXCLUSIVITY              = 'exclusivity'
 PROGRAM_STATUS_REVIEW                   = 'review'
 PROGRAM_STATUS_PUBLISH                  = 'published'
 
 ACTION_AFTER_UNLOCK_TIER_NO_ACTION          = 'no_action'
 ACTION_AFTER_UNLOCK_TIER_CONSUME_REWARD     = 'consume_reward'
 
 
@@ -66,47 +74,60 @@
 GIVEAWAY_SYSTEM_CONDITION_MEMBERSHIP_YEAR       = 'membership_year'
 
 GIVEAWAY_SYSTEM_CONDITION_FOR_MEMBERSHIP        = (GIVEAWAY_SYSTEM_CONDITION_NEW_MEMBERSHIP, GIVEAWAY_SYSTEM_CONDITION_RENEW_MEMBERSHIP)
 
 '''
 BASIC_REWARD_PROGRAM_STATUS                          = OrderedSet([PROGRAM_STATUS_PROGRAM_BASE, 
                                                                   PROGRAM_STATUS_REWARD_SCHEME, 
-                                                                  PROGRAM_STATUS_REWARD_EXCLUSIVITY,
+                                                                  PROGRAM_STATUS_EXCLUSIVITY,
                                                                   PROGRAM_STATUS_PUBLISH
                                                                   ])
 
 TIER_REWARD_PROGRAM_STATUS                          = OrderedSet([PROGRAM_STATUS_PROGRAM_BASE, 
                                                                   PROGRAM_STATUS_DEFINE_TIER, 
                                                                   PROGRAM_STATUS_DEFINE_REWARD,
-                                                                  PROGRAM_STATUS_REWARD_EXCLUSIVITY,
+                                                                  PROGRAM_STATUS_EXCLUSIVITY,
                                                                   PROGRAM_STATUS_PUBLISH,
                                                                   ])
 '''
 
 BASIC_REWARD_PROGRAM_STATUS                          = [PROGRAM_STATUS_PROGRAM_BASE, 
                                                                   PROGRAM_STATUS_REWARD_SCHEME, 
-                                                                  PROGRAM_STATUS_REWARD_EXCLUSIVITY,
+                                                                  PROGRAM_STATUS_EXCLUSIVITY,
+                                                                  #PROGRAM_STATUS_REVIEW,
                                                                   PROGRAM_STATUS_PUBLISH
                                                                   ]
 
 TIER_REWARD_PROGRAM_STATUS                          = [PROGRAM_STATUS_PROGRAM_BASE, 
                                                                   PROGRAM_STATUS_DEFINE_TIER, 
                                                                   PROGRAM_STATUS_DEFINE_REWARD,
-                                                                  PROGRAM_STATUS_REWARD_EXCLUSIVITY,
+                                                                  PROGRAM_STATUS_EXCLUSIVITY,
+                                                                  PROGRAM_STATUS_PUBLISH,
+                                                                  ]
+
+LUCKY_DRAW_PROGRAM_STATUS                          = [
+                                                                  PROGRAM_STATUS_PROGRAM_BASE, 
+                                                                  #PROGRAM_STATUS_DEFINE_CONDITION,
+                                                                  PROGRAM_STATUS_UPLOAD_TICKET_IMAGE,  
+                                                                  PROGRAM_STATUS_DEFINE_PRIZE,  
+                                                                  PROGRAM_STATUS_DEFINE_PRIZE_POSSIBILITY,
+                                                                  PROGRAM_STATUS_EXCLUSIVITY,
                                                                   PROGRAM_STATUS_PUBLISH,
                                                                   ]
 
 ALL_PROGRAM_STATUS                            = (PROGRAM_STATUS_PROGRAM_BASE,
                                                  PROGRAM_STATUS_REWARD_SCHEME,
                                                  PROGRAM_STATUS_DEFINE_TIER,
                                                  PROGRAM_STATUS_DEFINE_REWARD,
-                                                 PROGRAM_STATUS_REWARD_EXCLUSIVITY,
+                                                 PROGRAM_STATUS_EXCLUSIVITY,
                                                  PROGRAM_STATUS_PUBLISH
                                                  )
 
+
+
 PROGRAM_SCHEDULE_TYPE_DAILY             = 'daily'
 PROGRAM_SCHEDULE_TYPE_MONTH_START       = 'month_start'
 PROGRAM_SCHEDULE_TYPE_WEEKEND           = 'weekend'
 PROGRAM_SCHEDULE_TYPE_FRIDAY            = 'friday'
 PROGRAM_SCHEDULE_TYPE_MONDAY            = 'monday'
 
 PROGRAM_SCHEDULE_TYPE_GROUP             = (PROGRAM_SCHEDULE_TYPE_DAILY, PROGRAM_SCHEDULE_TYPE_MONTH_START, PROGRAM_SCHEDULE_TYPE_WEEKEND, PROGRAM_SCHEDULE_TYPE_FRIDAY, PROGRAM_SCHEDULE_TYPE_MONDAY)
@@ -207,14 +228,18 @@
                                                    )
 
 
 MEMBERSHIP_UPGRADE_EXPIRY_TYPE_CONTINUE_EXPIRY                      = 'cont_expiry'
 MEMBERSHIP_UPGRADE_EXPIRY_TYPE_NEW_EXPIRY                           = 'new_expiry'
 
 
+GIVEAWAY_ON_FIRST_DAY_OF_MONTH  = 'month_start'
+GIVEAWAY_ON_DOB                 = 'dob_date'
+GIVEAWAY_IN_ADVANCE             = 'advance_in_day'
+
 REWARD_STATUS_VALID        = 'valid'
 REWARD_STATUS_REACH_LIMIT  = 'limit'
 REWARD_STATUS_REDEEMED     = 'redeemed'
 REWARD_STATUS_REVERTED     = 'reverted'
 REWARD_STATUS_REMOVED      = 'removed'
 
 REDEEM_STATUS_VALID        = 'valid'
@@ -235,14 +260,17 @@
 
 def get_voucher_completed_status_index(completed_status):
     return VOUCHER_STATUS.index(completed_status) 
 
 def get_tier_reward_program_completed_status_index(completed_status):
     return TIER_REWARD_PROGRAM_STATUS.index(completed_status)
 
+def get_lucky_draw_program_completed_status_index(completed_status):
+    return LUCKY_DRAW_PROGRAM_STATUS.index(completed_status)
+
 def is_program_current_status_reach(checking_status, completed_status):
     completed_status_index  = get_program_completed_status_index(completed_status)
     checking_status_index   = get_program_completed_status_index(checking_status)
     
     print('completed_status_index=%s'%completed_status_index)
     print('checking_status_index=%s'%checking_status_index)
     
@@ -262,14 +290,23 @@
     checking_status_index   = get_tier_reward_program_completed_status_index(checking_status)
     
     print('completed_status_index=%s'%completed_status_index)
     print('checking_status_index=%s'%checking_status_index)
     
     return checking_status_index<=completed_status_index+1
 
+def is_lucky_draw_program_current_status_reach(checking_status, completed_status):
+    completed_status_index  = get_lucky_draw_program_completed_status_index(completed_status)
+    checking_status_index   = get_lucky_draw_program_completed_status_index(checking_status)
+    
+    print('completed_status_index=%s'%completed_status_index)
+    print('checking_status_index=%s'%checking_status_index)
+    
+    return checking_status_index<=completed_status_index+1
+
 
 def is_valid_to_update_program_status(checking_status, completed_status):
     completed_status_index  = get_program_completed_status_index(completed_status)
     checking_status_index   = get_program_completed_status_index(checking_status)
     
     return checking_status_index<=completed_status_index+1
 
@@ -297,30 +334,35 @@
     checking_status_index   = get_voucher_completed_status_index(checking_status)
     
     return checking_status_index<completed_status_index
 
 def is_existing_program_status_final_state(completed_status):
     completed_status_index  = get_program_completed_status_index(completed_status)
     
-    return completed_status_index==len(BASIC_REWARD_PROGRAM_STATUS)-2
+    return completed_status_index==len(BASIC_REWARD_PROGRAM_STATUS)-1
 
 def is_existing_tier_reward_program_status_final_state(completed_status):
     completed_status_index  = get_tier_reward_program_completed_status_index(completed_status)
     
-    return completed_status_index==len(TIER_REWARD_PROGRAM_STATUS)-2
+    return completed_status_index==len(TIER_REWARD_PROGRAM_STATUS)-1
 
 def is_existing_voucher_status_final_state(completed_status):
     completed_status_index  = get_voucher_completed_status_index(completed_status)
     
-    return completed_status_index==len(BASIC_REWARD_PROGRAM_STATUS)-2
+    return completed_status_index==len(BASIC_REWARD_PROGRAM_STATUS)-1
 
 def program_completed_progress_percentage(completed_status):
     completed_status_index  = get_program_completed_status_index(completed_status)
     print('program_completed_progress_percentage: completed_status_index(%s)=%s'% (completed_status,completed_status_index))
     return int((completed_status_index+1)/len(BASIC_REWARD_PROGRAM_STATUS) * 100)
 
 def tier_reward_program_completed_progress_percentage(completed_status):
     completed_status_index  = get_tier_reward_program_completed_status_index(completed_status)
-    print('program_completed_progress_percentage: completed_status_index(%s)=%s'% (completed_status,completed_status_index))
+    print('tier_reward_program_completed_progress_percentage: completed_status_index(%s)=%s'% (completed_status,completed_status_index))
     return int((completed_status_index+1)/len(TIER_REWARD_PROGRAM_STATUS) * 100)    
+
+def lucky_draw_program_completed_progress_percentage(completed_status):
+    completed_status_index  = get_lucky_draw_program_completed_status_index(completed_status)
+    print('lucky_draw_program_completed_progress_percentage: completed_status_index(%s)=%s'% (completed_status,completed_status_index))
+    return int((completed_status_index+1)/len(LUCKY_DRAW_PROGRAM_STATUS) * 100)
```

### Comparing `trex-model-1.0.4/trexmodel/utils/model/model_util.py` & `trex-model-1.0.6/trexmodel/utils/model/model_util.py`

 * *Files identical despite different names*

