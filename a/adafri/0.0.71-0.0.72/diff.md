# Comparing `tmp/adafri-0.0.71.tar.gz` & `tmp/adafri-0.0.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.71.tar", last modified: Mon Jul 31 02:28:15 2023, max compression
+gzip compressed data, was "adafri-0.0.72.tar", last modified: Tue Aug  1 01:31:39 2023, max compression
```

## Comparing `adafri-0.0.71.tar` & `adafri-0.0.72.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.030449 adafri-0.0.71/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-31 02:28:15.029816 adafri-0.0.71/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:14.979828 adafri-0.0.71/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-31 02:28:02.000000 adafri-0.0.71/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:14.995497 adafri-0.0.71/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.71/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.71/adafri/utils/country.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.71/adafri/utils/phone_number.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1356 2023-07-31 01:55:04.000000 adafri-0.0.71/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    19150 2023-07-31 02:21:52.000000 adafri-0.0.71/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:14.996374 adafri-0.0.71/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.71/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:14.997445 adafri-0.0.71/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.71/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.000902 adafri-0.0.71/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.71/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.71/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3852 2023-07-28 08:14:22.000000 adafri-0.0.71/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.001886 adafri-0.0.71/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.71/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.003708 adafri-0.0.71/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.71/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.71/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.005063 adafri-0.0.71/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.71/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.005839 adafri-0.0.71/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      965 2023-07-28 08:17:28.000000 adafri-0.0.71/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.016964 adafri-0.0.71/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.71/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6979 2023-07-31 01:04:15.000000 adafri-0.0.71/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5478 2023-07-28 08:09:48.000000 adafri-0.0.71/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6529 2023-07-31 01:47:56.000000 adafri-0.0.71/adafri/v1/auth/oauth/models/code.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2505 2023-07-31 01:28:33.000000 adafri-0.0.71/adafri/v1/auth/oauth/models/code_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16147 2023-07-31 01:04:27.000000 adafri-0.0.71/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3653 2023-07-28 08:10:56.000000 adafri-0.0.71/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9468 2023-07-31 01:04:45.000000 adafri-0.0.71/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3728 2023-07-28 08:11:40.000000 adafri-0.0.71/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.020739 adafri-0.0.71/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.71/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.71/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.71/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.023157 adafri-0.0.71/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.71/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.71/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.023954 adafri-0.0.71/adafri/v1/mailing/
--rw-r--r--   0 ibrahima   (502) staff       (20)    11306 2023-07-31 02:27:42.000000 adafri-0.0.71/adafri/v1/mailing/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.024781 adafri-0.0.71/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.71/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.028205 adafri-0.0.71/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.71/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    11624 2023-07-26 07:42:34.000000 adafri-0.0.71/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     7382 2023-07-28 08:13:51.000000 adafri-0.0.71/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:14.989522 adafri-0.0.71/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-31 02:28:14.000000 adafri-0.0.71/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1329 2023-07-31 02:28:14.000000 adafri-0.0.71/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-31 02:28:14.000000 adafri-0.0.71/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-31 02:28:14.000000 adafri-0.0.71/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-31 02:28:15.030810 adafri-0.0.71/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.71/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.349430 adafri-0.0.72/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-01 01:31:39.349062 adafri-0.0.72/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.314703 adafri-0.0.72/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-08-01 01:31:32.000000 adafri-0.0.72/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.322450 adafri-0.0.72/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.72/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.72/adafri/utils/country.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.72/adafri/utils/phone_number.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1356 2023-07-31 01:55:04.000000 adafri-0.0.72/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    19150 2023-07-31 02:21:52.000000 adafri-0.0.72/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.323683 adafri-0.0.72/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.72/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.324649 adafri-0.0.72/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.72/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.327269 adafri-0.0.72/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.72/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.72/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3852 2023-07-28 08:14:22.000000 adafri-0.0.72/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.328086 adafri-0.0.72/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.72/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.329692 adafri-0.0.72/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.72/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.72/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.330675 adafri-0.0.72/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.72/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.331102 adafri-0.0.72/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      965 2023-07-28 08:17:28.000000 adafri-0.0.72/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.339090 adafri-0.0.72/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.72/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6979 2023-07-31 01:04:15.000000 adafri-0.0.72/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5478 2023-07-28 08:09:48.000000 adafri-0.0.72/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6529 2023-07-31 01:47:56.000000 adafri-0.0.72/adafri/v1/auth/oauth/models/code.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2505 2023-07-31 01:28:33.000000 adafri-0.0.72/adafri/v1/auth/oauth/models/code_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16147 2023-07-31 01:04:27.000000 adafri-0.0.72/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3653 2023-07-28 08:10:56.000000 adafri-0.0.72/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9468 2023-07-31 01:04:45.000000 adafri-0.0.72/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3728 2023-07-28 08:11:40.000000 adafri-0.0.72/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.341751 adafri-0.0.72/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.72/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.72/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.72/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.343325 adafri-0.0.72/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.72/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.72/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.344190 adafri-0.0.72/adafri/v1/mailing/
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11325 2023-08-01 01:31:24.000000 adafri-0.0.72/adafri/v1/mailing/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.344977 adafri-0.0.72/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.72/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.348039 adafri-0.0.72/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.72/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11624 2023-07-26 07:42:34.000000 adafri-0.0.72/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     7382 2023-07-28 08:13:51.000000 adafri-0.0.72/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.317885 adafri-0.0.72/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-01 01:31:39.000000 adafri-0.0.72/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1329 2023-08-01 01:31:39.000000 adafri-0.0.72/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-08-01 01:31:39.000000 adafri-0.0.72/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-08-01 01:31:39.000000 adafri-0.0.72/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-08-01 01:31:39.349674 adafri-0.0.72/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.72/setup.py
```

### Comparing `adafri-0.0.71/adafri/utils/country.py` & `adafri-0.0.72/adafri/utils/country.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/adafri/utils/phone_number.py` & `adafri-0.0.72/adafri/utils/phone_number.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/adafri/utils/response.py` & `adafri-0.0.72/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/adafri/utils/utils.py` & `adafri-0.0.72/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/adafri/v1/account/models/account.py` & `adafri-0.0.72/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/adafri/v1/account/models/account_fields.py` & `adafri-0.0.72/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.72/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.72/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.72/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.72/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/adafri/v1/auth/oauth/models/code.py` & `adafri-0.0.72/adafri/v1/auth/oauth/models/code.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/adafri/v1/auth/oauth/models/code_fields.py` & `adafri-0.0.72/adafri/v1/auth/oauth/models/code_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.72/adafri/v1/auth/oauth/models/grant.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.72/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.72/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.72/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.72/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.72/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/adafri/v1/base/firebase_collection.py` & `adafri-0.0.72/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/adafri/v1/mailing/__init__.py` & `adafri-0.0.72/adafri/v1/mailing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,23 +85,24 @@
         if api_key is None:
             api_key = SENDGRID_API_KEY;
         return SendGridAPIClient(api_key);
 
     def check_time_send(self, check=True):
         user_model = User().query([{"key": "email", "value": self.destination, "comp": "=="}], True);
         if user_model is not None and user_model.uid is None:
-            return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error('User not exist', 'INVALID_REQUEST'))
+            return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error('User not exist', 'USER_NOT_EXIST'))
         if check:
             time_sended = getTimeSended(user_model);
             if time_sended['status']=='error':
-                return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error('User not exist', 'INVALID_REQUEST'))
+                return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error('User not exist', 'USER_NOT_EXIST'))
             if time_sended[VALIDATION_FIELD]!='now':
                 compare = compareTimes(time_sended[VALIDATION_FIELD]);
                 if compare['status'] == 'error':
-                    return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"Please wait {DEFAULT_EMAIL_TIME_TO_RESEND - compare['difference']} minutes and retry", 'INVALID_REQUEST'))
+                    minutes = DEFAULT_EMAIL_TIME_TO_RESEND - compare['difference']
+                    return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, {"minutes": minutes}, Error(f"Please wait {minutes} minutes and retry", 'WAIT_FEW_MINUTES'))
 
         return ApiResponse(ResponseStatus.OK, StatusCode.status_200, user_model, None)
     
     def sendMailRegistration(self, domain, _api_key=None, _template_id=None, bccs=[]):
         if domain is None:
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error('Invalid domain', 'INVALID_REQUEST'))
         result = None
@@ -187,24 +188,23 @@
                 personalization.dynamic_template_data = custom_data
             personalization.add_to(Email(self.destination))
             personalization.subject = self.subject
             for bcc in bccs:
                 personalization.add_bcc(Email(bcc))
             message.add_personalization(personalization)
             email_test_mode = boolean(os.environ.get('EMAIL_TEST_MODE'))
-            if email_test_mode is None or email_test_mode is False:
+            if email_test_mode is None or email_test_mode is True:
                 response = Object(status_code=200, message="success")
             else:
-                # response = self.sendgrid_client(_api_key).send(message) 
-                response = Object(status_code=200, message="success")
+                response = self.sendgrid_client(_api_key).send(message) 
             if response.status_code==200 or response.status_code==202:
                 setTimeSended(user_model);
                 result = ApiResponse(ResponseStatus.OK, response.status_code, {"message": "Email sent successfully"}, None)
             else:
-                result = ApiResponse(ResponseStatus.ERROR, response.status_code, None, Error('An error occurated', 'INVALID_REQUEST'))
+                result = ApiResponse(ResponseStatus.ERROR, response.status_code, None, Error('An error occurated that\'s why your email were not sent', 'EMAIL_NOT_SENT', 1))
         except Exception as e:
             print(e)
             result = ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(str(e), 'INVALID_REQUEST'))
         
         return result
```

### Comparing `adafri-0.0.71/adafri/v1/user/models/user.py` & `adafri-0.0.72/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/adafri/v1/user/models/user_fields.py` & `adafri-0.0.72/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/adafri.egg-info/SOURCES.txt` & `adafri-0.0.72/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.71/setup.py` & `adafri-0.0.72/setup.py`

 * *Files identical despite different names*

