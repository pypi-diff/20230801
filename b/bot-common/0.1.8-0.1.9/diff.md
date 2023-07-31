# Comparing `tmp/bot_common-0.1.8.tar.gz` & `tmp/bot_common-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Utente\Desktop\Bot_v3\Bot_General\bot_common_lib\dist\.tmp-oc32dgba\bot_common-0.1.8.tar", last modified: Fri Jul 28 10:25:33 2023, max compression
+gzip compressed data, was "C:\Users\Utente\Desktop\Bot_v3\Bot_General\bot_common_lib\dist\.tmp-45pffwru\bot_common-0.1.9.tar", last modified: Fri Jul 28 10:39:54 2023, max compression
```

## Comparing `bot_common-0.1.8.tar` & `bot_common-0.1.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 10:25:33.000000 bot_common-0.1.8/
--rw-rw-rw-   0        0        0     1078 2022-11-30 18:30:39.000000 bot_common-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      314 2023-07-28 10:25:33.000000 bot_common-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      109 2022-12-09 17:07:00.000000 bot_common-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 10:25:33.000000 bot_common-0.1.8/bot_common/
--rw-rw-rw-   0        0        0        0 2022-12-01 14:05:41.000000 bot_common-0.1.8/bot_common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 10:25:33.000000 bot_common-0.1.8/bot_common/apis/
--rw-rw-rw-   0        0        0       77 2022-12-04 16:45:54.000000 bot_common-0.1.8/bot_common/apis/__init__.py
--rw-rw-rw-   0        0        0      968 2022-12-08 14:36:20.000000 bot_common-0.1.8/bot_common/apis/api_request.py
-drwxrwxrwx   0        0        0        0 2023-07-28 10:25:33.000000 bot_common-0.1.8/bot_common/companies/
--rw-rw-rw-   0        0        0      208 2022-12-08 14:42:21.000000 bot_common-0.1.8/bot_common/companies/__init__.py
--rw-rw-rw-   0        0        0     6755 2022-12-09 21:25:23.000000 bot_common-0.1.8/bot_common/companies/company.py
--rw-rw-rw-   0        0        0     2526 2022-12-09 19:07:13.000000 bot_common-0.1.8/bot_common/companies/company_model.py
--rw-rw-rw-   0        0        0     9762 2022-12-08 15:44:21.000000 bot_common-0.1.8/bot_common/companies/company_setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 10:25:33.000000 bot_common-0.1.8/bot_common/exceptions/
--rw-rw-rw-   0        0        0      144 2022-12-13 11:30:10.000000 bot_common-0.1.8/bot_common/exceptions/__init__.py
--rw-rw-rw-   0        0        0     2692 2022-12-08 14:16:42.000000 bot_common-0.1.8/bot_common/exceptions/exception.py
--rw-rw-rw-   0        0        0      459 2022-12-01 16:46:34.000000 bot_common-0.1.8/bot_common/exceptions/exception_model.py
--rw-rw-rw-   0        0        0      566 2023-07-08 12:42:26.000000 bot_common-0.1.8/bot_common/lib_conf.py
-drwxrwxrwx   0        0        0        0 2023-07-28 10:25:33.000000 bot_common-0.1.8/bot_common/logs/
--rw-rw-rw-   0        0        0       37 2022-12-01 19:25:45.000000 bot_common-0.1.8/bot_common/logs/__init__.py
--rw-rw-rw-   0        0        0     2858 2022-12-15 09:59:06.000000 bot_common-0.1.8/bot_common/logs/log.py
--rw-rw-rw-   0        0        0     2688 2022-12-15 13:59:36.000000 bot_common-0.1.8/bot_common/logs/log_model.py
-drwxrwxrwx   0        0        0        0 2023-07-28 10:25:33.000000 bot_common-0.1.8/bot_common/messages/
--rw-rw-rw-   0        0        0      151 2022-12-03 15:41:09.000000 bot_common-0.1.8/bot_common/messages/__init__.py
--rw-rw-rw-   0        0        0     7248 2022-12-09 21:38:17.000000 bot_common-0.1.8/bot_common/messages/message.py
--rw-rw-rw-   0        0        0      959 2022-12-03 15:42:34.000000 bot_common-0.1.8/bot_common/messages/message_model.py
--rw-rw-rw-   0        0        0     2562 2022-12-09 21:19:47.000000 bot_common-0.1.8/bot_common/messages/timeout.py
--rw-rw-rw-   0        0        0      506 2022-12-03 13:34:23.000000 bot_common-0.1.8/bot_common/messages/timeout_model.py
-drwxrwxrwx   0        0        0        0 2023-07-28 10:25:33.000000 bot_common-0.1.8/bot_common/send_message/
--rw-rw-rw-   0        0        0      135 2022-12-12 14:41:03.000000 bot_common-0.1.8/bot_common/send_message/__init__.py
--rw-rw-rw-   0        0        0      860 2022-12-12 14:41:03.000000 bot_common-0.1.8/bot_common/send_message/mail.py
--rw-rw-rw-   0        0        0      323 2022-12-12 14:39:04.000000 bot_common-0.1.8/bot_common/send_message/mail_model.py
-drwxrwxrwx   0        0        0        0 2023-07-28 10:25:33.000000 bot_common-0.1.8/bot_common/sessions/
--rw-rw-rw-   0        0        0       61 2022-12-01 19:28:09.000000 bot_common-0.1.8/bot_common/sessions/__init__.py
--rw-rw-rw-   0        0        0     5364 2022-12-15 14:09:56.000000 bot_common-0.1.8/bot_common/sessions/session.py
--rw-rw-rw-   0        0        0     1761 2022-12-15 14:09:56.000000 bot_common-0.1.8/bot_common/sessions/session_model.py
-drwxrwxrwx   0        0        0        0 2023-07-28 10:25:33.000000 bot_common-0.1.8/bot_common/utils/
--rw-rw-rw-   0        0        0      241 2022-12-08 12:30:36.000000 bot_common-0.1.8/bot_common/utils/__init__.py
--rw-rw-rw-   0        0        0     3075 2023-07-08 12:36:02.000000 bot_common-0.1.8/bot_common/utils/db_utils.py
--rw-rw-rw-   0        0        0      266 2022-11-29 18:39:40.000000 bot_common-0.1.8/bot_common/utils/logging_conf.py
--rw-rw-rw-   0        0        0     1971 2023-07-28 10:19:45.000000 bot_common-0.1.8/bot_common/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-28 10:25:33.000000 bot_common-0.1.8/bot_common.egg-info/
--rw-rw-rw-   0        0        0      314 2023-07-28 10:25:33.000000 bot_common-0.1.8/bot_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1138 2023-07-28 10:25:33.000000 bot_common-0.1.8/bot_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 10:25:33.000000 bot_common-0.1.8/bot_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-28 10:25:33.000000 bot_common-0.1.8/bot_common.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-28 10:25:33.000000 bot_common-0.1.8/bot_common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      119 2022-12-08 09:23:59.000000 bot_common-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0      546 2023-07-28 10:25:33.000000 bot_common-0.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 10:39:54.000000 bot_common-0.1.9/
+-rw-rw-rw-   0        0        0     1078 2022-11-30 18:30:39.000000 bot_common-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      314 2023-07-28 10:39:54.000000 bot_common-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2022-12-09 17:07:00.000000 bot_common-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 10:39:53.000000 bot_common-0.1.9/bot_common/
+-rw-rw-rw-   0        0        0        0 2022-12-01 14:05:41.000000 bot_common-0.1.9/bot_common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:39:54.000000 bot_common-0.1.9/bot_common/apis/
+-rw-rw-rw-   0        0        0       77 2022-12-04 16:45:54.000000 bot_common-0.1.9/bot_common/apis/__init__.py
+-rw-rw-rw-   0        0        0      968 2022-12-08 14:36:20.000000 bot_common-0.1.9/bot_common/apis/api_request.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:39:54.000000 bot_common-0.1.9/bot_common/companies/
+-rw-rw-rw-   0        0        0      208 2022-12-08 14:42:21.000000 bot_common-0.1.9/bot_common/companies/__init__.py
+-rw-rw-rw-   0        0        0     6755 2022-12-09 21:25:23.000000 bot_common-0.1.9/bot_common/companies/company.py
+-rw-rw-rw-   0        0        0     2526 2022-12-09 19:07:13.000000 bot_common-0.1.9/bot_common/companies/company_model.py
+-rw-rw-rw-   0        0        0     9762 2022-12-08 15:44:21.000000 bot_common-0.1.9/bot_common/companies/company_setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:39:54.000000 bot_common-0.1.9/bot_common/exceptions/
+-rw-rw-rw-   0        0        0      144 2022-12-13 11:30:10.000000 bot_common-0.1.9/bot_common/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     2692 2022-12-08 14:16:42.000000 bot_common-0.1.9/bot_common/exceptions/exception.py
+-rw-rw-rw-   0        0        0      459 2022-12-01 16:46:34.000000 bot_common-0.1.9/bot_common/exceptions/exception_model.py
+-rw-rw-rw-   0        0        0      566 2023-07-08 12:42:26.000000 bot_common-0.1.9/bot_common/lib_conf.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:39:54.000000 bot_common-0.1.9/bot_common/logs/
+-rw-rw-rw-   0        0        0       37 2022-12-01 19:25:45.000000 bot_common-0.1.9/bot_common/logs/__init__.py
+-rw-rw-rw-   0        0        0     2858 2022-12-15 09:59:06.000000 bot_common-0.1.9/bot_common/logs/log.py
+-rw-rw-rw-   0        0        0     2688 2022-12-15 13:59:36.000000 bot_common-0.1.9/bot_common/logs/log_model.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:39:54.000000 bot_common-0.1.9/bot_common/messages/
+-rw-rw-rw-   0        0        0      151 2022-12-03 15:41:09.000000 bot_common-0.1.9/bot_common/messages/__init__.py
+-rw-rw-rw-   0        0        0     7248 2022-12-09 21:38:17.000000 bot_common-0.1.9/bot_common/messages/message.py
+-rw-rw-rw-   0        0        0      959 2022-12-03 15:42:34.000000 bot_common-0.1.9/bot_common/messages/message_model.py
+-rw-rw-rw-   0        0        0     2562 2022-12-09 21:19:47.000000 bot_common-0.1.9/bot_common/messages/timeout.py
+-rw-rw-rw-   0        0        0      506 2022-12-03 13:34:23.000000 bot_common-0.1.9/bot_common/messages/timeout_model.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:39:54.000000 bot_common-0.1.9/bot_common/send_message/
+-rw-rw-rw-   0        0        0      135 2022-12-12 14:41:03.000000 bot_common-0.1.9/bot_common/send_message/__init__.py
+-rw-rw-rw-   0        0        0      860 2022-12-12 14:41:03.000000 bot_common-0.1.9/bot_common/send_message/mail.py
+-rw-rw-rw-   0        0        0      323 2022-12-12 14:39:04.000000 bot_common-0.1.9/bot_common/send_message/mail_model.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:39:54.000000 bot_common-0.1.9/bot_common/sessions/
+-rw-rw-rw-   0        0        0       61 2022-12-01 19:28:09.000000 bot_common-0.1.9/bot_common/sessions/__init__.py
+-rw-rw-rw-   0        0        0     5364 2022-12-15 14:09:56.000000 bot_common-0.1.9/bot_common/sessions/session.py
+-rw-rw-rw-   0        0        0     1761 2022-12-15 14:09:56.000000 bot_common-0.1.9/bot_common/sessions/session_model.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:39:54.000000 bot_common-0.1.9/bot_common/utils/
+-rw-rw-rw-   0        0        0      280 2023-07-28 10:38:31.000000 bot_common-0.1.9/bot_common/utils/__init__.py
+-rw-rw-rw-   0        0        0     3075 2023-07-08 12:36:02.000000 bot_common-0.1.9/bot_common/utils/db_utils.py
+-rw-rw-rw-   0        0        0      266 2022-11-29 18:39:40.000000 bot_common-0.1.9/bot_common/utils/logging_conf.py
+-rw-rw-rw-   0        0        0     1971 2023-07-28 10:19:45.000000 bot_common-0.1.9/bot_common/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:39:54.000000 bot_common-0.1.9/bot_common.egg-info/
+-rw-rw-rw-   0        0        0      314 2023-07-28 10:39:53.000000 bot_common-0.1.9/bot_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1138 2023-07-28 10:39:53.000000 bot_common-0.1.9/bot_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 10:39:53.000000 bot_common-0.1.9/bot_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-28 10:39:53.000000 bot_common-0.1.9/bot_common.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-28 10:39:53.000000 bot_common-0.1.9/bot_common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      119 2022-12-08 09:23:59.000000 bot_common-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      546 2023-07-28 10:39:54.000000 bot_common-0.1.9/setup.cfg
```

### Comparing `bot_common-0.1.8/LICENSE` & `bot_common-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bot_common-0.1.8/bot_common/apis/api_request.py` & `bot_common-0.1.9/bot_common/apis/api_request.py`

 * *Files identical despite different names*

### Comparing `bot_common-0.1.8/bot_common/companies/company.py` & `bot_common-0.1.9/bot_common/companies/company.py`

 * *Files identical despite different names*

### Comparing `bot_common-0.1.8/bot_common/companies/company_model.py` & `bot_common-0.1.9/bot_common/companies/company_model.py`

 * *Files identical despite different names*

### Comparing `bot_common-0.1.8/bot_common/companies/company_setup.py` & `bot_common-0.1.9/bot_common/companies/company_setup.py`

 * *Files identical despite different names*

### Comparing `bot_common-0.1.8/bot_common/exceptions/exception.py` & `bot_common-0.1.9/bot_common/exceptions/exception.py`

 * *Files identical despite different names*

### Comparing `bot_common-0.1.8/bot_common/lib_conf.py` & `bot_common-0.1.9/bot_common/lib_conf.py`

 * *Files identical despite different names*

### Comparing `bot_common-0.1.8/bot_common/logs/log.py` & `bot_common-0.1.9/bot_common/logs/log.py`

 * *Files identical despite different names*

### Comparing `bot_common-0.1.8/bot_common/logs/log_model.py` & `bot_common-0.1.9/bot_common/logs/log_model.py`

 * *Files identical despite different names*

### Comparing `bot_common-0.1.8/bot_common/messages/message.py` & `bot_common-0.1.9/bot_common/messages/message.py`

 * *Files identical despite different names*

### Comparing `bot_common-0.1.8/bot_common/messages/message_model.py` & `bot_common-0.1.9/bot_common/messages/message_model.py`

 * *Files identical despite different names*

### Comparing `bot_common-0.1.8/bot_common/messages/timeout.py` & `bot_common-0.1.9/bot_common/messages/timeout.py`

 * *Files identical despite different names*

### Comparing `bot_common-0.1.8/bot_common/send_message/mail.py` & `bot_common-0.1.9/bot_common/send_message/mail.py`

 * *Files identical despite different names*

### Comparing `bot_common-0.1.8/bot_common/sessions/session.py` & `bot_common-0.1.9/bot_common/sessions/session.py`

 * *Files identical despite different names*

### Comparing `bot_common-0.1.8/bot_common/sessions/session_model.py` & `bot_common-0.1.9/bot_common/sessions/session_model.py`

 * *Files identical despite different names*

### Comparing `bot_common-0.1.8/bot_common/utils/db_utils.py` & `bot_common-0.1.9/bot_common/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `bot_common-0.1.8/bot_common/utils/utils.py` & `bot_common-0.1.9/bot_common/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bot_common-0.1.8/bot_common.egg-info/SOURCES.txt` & `bot_common-0.1.9/bot_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bot_common-0.1.8/setup.cfg` & `bot_common-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 6f74 5f63 6f6d 6d6f 6e0d 0a76   = bot_common..v
-00000020: 6572 7369 6f6e 203d 2030 2e31 2e38 0d0a  ersion = 0.1.8..
+00000020: 6572 7369 6f6e 203d 2030 2e31 2e39 0d0a  ersion = 0.1.9..
 00000030: 6175 7468 6f72 203d 2043 6c61 7564 696f  author = Claudio
 00000040: 2046 7261 676f 6d65 6c69 0d0a 6175 7468   Fragomeli..auth
 00000050: 6f72 5f65 6d61 696c 203d 2063 6c61 2e66  or_email = cla.f
 00000060: 7261 676f 6d65 6c69 4067 6d61 696c 2e63  ragomeli@gmail.c
 00000070: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000080: 3d20 436f 6d6d 6f6e 206c 6962 7261 7269  = Common librari
 00000090: 6573 2041 4953 4143 2042 6f74 0d0a 6c6f  es AISAC Bot..lo
```

