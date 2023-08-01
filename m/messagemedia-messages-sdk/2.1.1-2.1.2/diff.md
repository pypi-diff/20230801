# Comparing `tmp/messagemedia-messages-sdk-2.1.1.tar.gz` & `tmp/messagemedia-messages-sdk-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "messagemedia-messages-sdk-2.1.1.tar", last modified: Mon Feb 13 00:55:38 2023, max compression
+gzip compressed data, was "messagemedia-messages-sdk-2.1.2.tar", last modified: Tue Aug  1 01:45:20 2023, max compression
```

## Comparing `messagemedia-messages-sdk-2.1.1.tar` & `messagemedia-messages-sdk-2.1.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 sharavan.gurrala   (502) staff       (20)        0 2023-02-13 00:55:38.438791 messagemedia-messages-sdk-2.1.1/
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)    11543 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/LICENSE
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)       34 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/MANIFEST.in
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)    11963 2023-02-13 00:55:38.438404 messagemedia-messages-sdk-2.1.1/PKG-INFO
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)    11586 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/README.md
-drwxr-xr-x   0 sharavan.gurrala   (502) staff       (20)        0 2023-02-13 00:55:38.379457 messagemedia-messages-sdk-2.1.1/message_media_messages/
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      177 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/__init__.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)    13834 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/api_helper.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1168 2023-02-13 00:36:37.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/configuration.py
-drwxr-xr-x   0 sharavan.gurrala   (502) staff       (20)        0 2023-02-13 00:55:38.383641 messagemedia-messages-sdk-2.1.1/message_media_messages/controllers/
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      127 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/controllers/__init__.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     3612 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/controllers/base_controller.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     8516 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/controllers/delivery_reports_controller.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)    15997 2023-02-13 00:36:37.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/controllers/messages_controller.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     8304 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/controllers/replies_controller.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      540 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/decorators.py
-drwxr-xr-x   0 sharavan.gurrala   (502) staff       (20)        0 2023-02-13 00:55:38.385132 messagemedia-messages-sdk-2.1.1/message_media_messages/exceptions/
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)       78 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/exceptions/__init__.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      931 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/exceptions/api_exception.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1353 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/exceptions/send_messages_400_response_exception.py
-drwxr-xr-x   0 sharavan.gurrala   (502) staff       (20)        0 2023-02-13 00:55:38.411584 messagemedia-messages-sdk-2.1.1/message_media_messages/http/
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      181 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/http/__init__.py
-drwxr-xr-x   0 sharavan.gurrala   (502) staff       (20)        0 2023-02-13 00:55:38.414640 messagemedia-messages-sdk-2.1.1/message_media_messages/http/auth/
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)       36 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/http/auth/__init__.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     3676 2023-02-13 00:36:37.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/http/auth/auth_manager.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1146 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/http/http_call_back.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     7147 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/http/http_client.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      992 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/http/http_context.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      951 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/http/http_method_enum.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     2865 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/http/http_request.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1119 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/http/http_response.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     3606 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/http/requests_client.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1355 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/message_media_messages_client.py
-drwxr-xr-x   0 sharavan.gurrala   (502) staff       (20)        0 2023-02-13 00:55:38.427016 messagemedia-messages-sdk-2.1.1/message_media_messages/models/
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      615 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/models/__init__.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1519 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/models/cancel_scheduled_message_request.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1913 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/models/check_delivery_reports_response.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1720 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/models/check_replies_response.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1624 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/models/confirm_delivery_reports_as_received_request.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1587 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/models/confirm_delivery_reports_as_received_request_1.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1509 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/models/confirm_replies_as_received_request.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1460 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/models/confirm_replies_as_received_request_1.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     4978 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/models/delivery_report.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      493 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/models/format_1_enum.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      477 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/models/format_enum.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     5236 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/models/get_message_status_response.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     4905 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/models/message.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     4053 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/models/reply.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1731 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/models/send_messages_request.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1734 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/models/send_messages_response.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      629 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/models/source_number_type_enum.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      848 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/models/status_2_enum.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1118 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/models/status_enum.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1657 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.1/message_media_messages/models/vendor_account_id.py
-drwxr-xr-x   0 sharavan.gurrala   (502) staff       (20)        0 2023-02-13 00:55:38.436735 messagemedia-messages-sdk-2.1.1/messagemedia_messages_sdk.egg-info/
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)    11963 2023-02-13 00:55:38.000000 messagemedia-messages-sdk-2.1.1/messagemedia_messages_sdk.egg-info/PKG-INFO
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     2575 2023-02-13 00:55:38.000000 messagemedia-messages-sdk-2.1.1/messagemedia_messages_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)        1 2023-02-13 00:55:38.000000 messagemedia-messages-sdk-2.1.1/messagemedia_messages_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      168 2023-02-13 00:55:38.000000 messagemedia-messages-sdk-2.1.1/messagemedia_messages_sdk.egg-info/requires.txt
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)       29 2023-02-13 00:55:38.000000 messagemedia-messages-sdk-2.1.1/messagemedia_messages_sdk.egg-info/top_level.txt
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)       38 2023-02-13 00:55:38.438844 messagemedia-messages-sdk-2.1.1/setup.cfg
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      993 2023-02-13 00:36:37.000000 messagemedia-messages-sdk-2.1.1/setup.py
-drwxr-xr-x   0 sharavan.gurrala   (502) staff       (20)        0 2023-02-13 00:55:38.437924 messagemedia-messages-sdk-2.1.1/tests/
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)       54 2023-02-13 00:36:37.000000 messagemedia-messages-sdk-2.1.1/tests/__init__.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     4389 2023-02-13 00:36:37.000000 messagemedia-messages-sdk-2.1.1/tests/auth_manager_test.py
--rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      792 2023-02-13 00:36:37.000000 messagemedia-messages-sdk-2.1.1/tests/test_util.py
+drwxr-xr-x   0 sharavan.gurrala   (502) staff       (20)        0 2023-08-01 01:45:20.379723 messagemedia-messages-sdk-2.1.2/
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)    11543 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/LICENSE
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)       34 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/MANIFEST.in
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)    11963 2023-08-01 01:45:20.379260 messagemedia-messages-sdk-2.1.2/PKG-INFO
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)    11586 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/README.md
+drwxr-xr-x   0 sharavan.gurrala   (502) staff       (20)        0 2023-08-01 01:45:20.220867 messagemedia-messages-sdk-2.1.2/message_media_messages/
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      177 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/__init__.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)    13834 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/api_helper.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1124 2023-08-01 01:43:47.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/configuration.py
+drwxr-xr-x   0 sharavan.gurrala   (502) staff       (20)        0 2023-08-01 01:45:20.244032 messagemedia-messages-sdk-2.1.2/message_media_messages/controllers/
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      127 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/controllers/__init__.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     3612 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/controllers/base_controller.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     8516 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/controllers/delivery_reports_controller.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)    15997 2023-02-13 00:36:37.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/controllers/messages_controller.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     8304 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/controllers/replies_controller.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      540 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/decorators.py
+drwxr-xr-x   0 sharavan.gurrala   (502) staff       (20)        0 2023-08-01 01:45:20.253244 messagemedia-messages-sdk-2.1.2/message_media_messages/exceptions/
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)       78 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/exceptions/__init__.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      931 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/exceptions/api_exception.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1353 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/exceptions/send_messages_400_response_exception.py
+drwxr-xr-x   0 sharavan.gurrala   (502) staff       (20)        0 2023-08-01 01:45:20.280944 messagemedia-messages-sdk-2.1.2/message_media_messages/http/
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      181 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/http/__init__.py
+drwxr-xr-x   0 sharavan.gurrala   (502) staff       (20)        0 2023-08-01 01:45:20.290098 messagemedia-messages-sdk-2.1.2/message_media_messages/http/auth/
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)       36 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/http/auth/__init__.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     3688 2023-08-01 01:43:47.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/http/auth/auth_manager.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1146 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/http/http_call_back.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     7147 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/http/http_client.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      992 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/http/http_context.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      951 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/http/http_method_enum.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     2865 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/http/http_request.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1119 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/http/http_response.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     3606 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/http/requests_client.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1353 2023-08-01 01:43:47.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/message_media_messages_client.py
+drwxr-xr-x   0 sharavan.gurrala   (502) staff       (20)        0 2023-08-01 01:45:20.362061 messagemedia-messages-sdk-2.1.2/message_media_messages/models/
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      615 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/models/__init__.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1519 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/models/cancel_scheduled_message_request.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1913 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/models/check_delivery_reports_response.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1720 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/models/check_replies_response.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1624 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/models/confirm_delivery_reports_as_received_request.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1587 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/models/confirm_delivery_reports_as_received_request_1.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1509 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/models/confirm_replies_as_received_request.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1460 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/models/confirm_replies_as_received_request_1.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     4978 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/models/delivery_report.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      493 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/models/format_1_enum.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      477 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/models/format_enum.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     5236 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/models/get_message_status_response.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     4905 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/models/message.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     4053 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/models/reply.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1731 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/models/send_messages_request.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1734 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/models/send_messages_response.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      629 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/models/source_number_type_enum.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      848 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/models/status_2_enum.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1118 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/models/status_enum.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     1657 2023-01-23 03:16:19.000000 messagemedia-messages-sdk-2.1.2/message_media_messages/models/vendor_account_id.py
+drwxr-xr-x   0 sharavan.gurrala   (502) staff       (20)        0 2023-08-01 01:45:20.370443 messagemedia-messages-sdk-2.1.2/messagemedia_messages_sdk.egg-info/
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)    11963 2023-08-01 01:45:19.000000 messagemedia-messages-sdk-2.1.2/messagemedia_messages_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     2575 2023-08-01 01:45:19.000000 messagemedia-messages-sdk-2.1.2/messagemedia_messages_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)        1 2023-08-01 01:45:19.000000 messagemedia-messages-sdk-2.1.2/messagemedia_messages_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      168 2023-08-01 01:45:19.000000 messagemedia-messages-sdk-2.1.2/messagemedia_messages_sdk.egg-info/requires.txt
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)       29 2023-08-01 01:45:19.000000 messagemedia-messages-sdk-2.1.2/messagemedia_messages_sdk.egg-info/top_level.txt
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)       38 2023-08-01 01:45:20.379789 messagemedia-messages-sdk-2.1.2/setup.cfg
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      993 2023-08-01 01:43:47.000000 messagemedia-messages-sdk-2.1.2/setup.py
+drwxr-xr-x   0 sharavan.gurrala   (502) staff       (20)        0 2023-08-01 01:45:20.378708 messagemedia-messages-sdk-2.1.2/tests/
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)       54 2023-02-13 00:36:37.000000 messagemedia-messages-sdk-2.1.2/tests/__init__.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)     4389 2023-02-13 00:36:37.000000 messagemedia-messages-sdk-2.1.2/tests/auth_manager_test.py
+-rw-r--r--   0 sharavan.gurrala   (502) staff       (20)      792 2023-02-13 00:36:37.000000 messagemedia-messages-sdk-2.1.2/tests/test_util.py
```

### Comparing `messagemedia-messages-sdk-2.1.1/LICENSE` & `messagemedia-messages-sdk-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/PKG-INFO` & `messagemedia-messages-sdk-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messagemedia-messages-sdk
-Version: 2.1.1
+Version: 2.1.2
 Summary: The MessageMedia Messages API provides a number of endpoints for building powerful two-way messaging applications.
 Home-page: https://developers.messagemedia.com
 Author: MessageMedia Developers
 Author-email: developers@messagemedia.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `messagemedia-messages-sdk-2.1.1/README.md` & `messagemedia-messages-sdk-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/api_helper.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/api_helper.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/controllers/base_controller.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/controllers/delivery_reports_controller.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/controllers/delivery_reports_controller.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/controllers/messages_controller.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/controllers/messages_controller.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/controllers/replies_controller.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/controllers/replies_controller.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/decorators.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/decorators.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/exceptions/api_exception.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/exceptions/send_messages_400_response_exception.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/exceptions/send_messages_400_response_exception.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/http/auth/auth_manager.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/http/auth/auth_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                 authentication will be added.
             url (str): The url of the request.
             body (str): The body of the request. None for GET requests.
 
         """
 
         if Configuration.hmac_auth_user_name is not None and \
-            Configuration.hmac_auth_password is not None:
+                Configuration.hmac_auth_password is not None:
             AuthManager.apply_hmac_auth(http_request, url, body)
         else:
             AuthManager.apply_basic_auth(http_request)
 
     @staticmethod
     def apply_basic_auth(http_request):
         """ Add basic authentication to the request.
@@ -87,23 +87,23 @@
         http_request.headers["date"] = date_header
 
         hmac_signature = AuthManager.create_signature(date_header,
                                                       content_signature,
                                                       url,
                                                       request_type)
 
-        joined = 'username="{}", algorithm="hmac-sha1", headers="date {}'\
-            'request-line", signature="{}"'\
+        joined = 'username="{}", algorithm="hmac-sha1", headers="date {}' \
+                 'request-line", signature="{}"' \
             .format(username, content_header, hmac_signature)
 
         header_value = "hmac {}".format(joined)
         http_request.headers["Authorization"] = header_value
 
     @staticmethod
     def create_signature(date, content_signature, url, request_type):
-        signing_string = "date: {}\n{}{} {} HTTP/1.1"\
+        signing_string = "date: {}\n{}{} {} HTTP/1.1" \
             .format(date, content_signature, request_type, url)
 
         hashed = hmac.new(Configuration.hmac_auth_password.encode("utf-8"),
                           signing_string.encode("utf-8"), hashlib.sha1)
 
         return base64.b64encode(hashed.digest()).decode('utf-8')
```

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/http/http_call_back.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/http/http_call_back.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/http/http_client.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/http/http_client.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/http/http_context.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/http/http_context.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/http/http_method_enum.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/http/http_method_enum.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/http/http_request.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/http/http_request.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/http/http_response.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/http/http_response.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/http/requests_client.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/http/requests_client.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/message_media_messages_client.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/message_media_messages_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,8 +37,7 @@
         if use_hmac_authentication:
             Configuration.hmac_auth_user_name = auth_user_name
             Configuration.hmac_auth_password = auth_password
         else:
             Configuration.basic_auth_user_name = auth_user_name
             Configuration.basic_auth_password = auth_password
 
-
```

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/models/__init__.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/models/__init__.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/models/cancel_scheduled_message_request.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/models/cancel_scheduled_message_request.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/models/check_delivery_reports_response.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/models/check_delivery_reports_response.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/models/check_replies_response.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/models/check_replies_response.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/models/confirm_delivery_reports_as_received_request.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/models/confirm_delivery_reports_as_received_request.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/models/confirm_delivery_reports_as_received_request_1.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/models/confirm_delivery_reports_as_received_request_1.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/models/confirm_replies_as_received_request.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/models/confirm_replies_as_received_request.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/models/confirm_replies_as_received_request_1.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/models/confirm_replies_as_received_request_1.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/models/delivery_report.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/models/delivery_report.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/models/get_message_status_response.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/models/get_message_status_response.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/models/message.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/models/message.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/models/reply.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/models/reply.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/models/send_messages_request.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/models/send_messages_request.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/models/send_messages_response.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/models/send_messages_response.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/models/source_number_type_enum.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/models/source_number_type_enum.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/models/status_2_enum.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/models/status_2_enum.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/models/status_enum.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/models/status_enum.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/message_media_messages/models/vendor_account_id.py` & `messagemedia-messages-sdk-2.1.2/message_media_messages/models/vendor_account_id.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/messagemedia_messages_sdk.egg-info/PKG-INFO` & `messagemedia-messages-sdk-2.1.2/messagemedia_messages_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messagemedia-messages-sdk
-Version: 2.1.1
+Version: 2.1.2
 Summary: The MessageMedia Messages API provides a number of endpoints for building powerful two-way messaging applications.
 Home-page: https://developers.messagemedia.com
 Author: MessageMedia Developers
 Author-email: developers@messagemedia.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `messagemedia-messages-sdk-2.1.1/messagemedia_messages_sdk.egg-info/SOURCES.txt` & `messagemedia-messages-sdk-2.1.2/messagemedia_messages_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/setup.py` & `messagemedia-messages-sdk-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='messagemedia-messages-sdk',
-    version='2.1.1',
+    version='2.1.2',
     description='The MessageMedia Messages API provides a number of endpoints for building powerful two-way messaging applications.',
     long_description_content_type="text/markdown",
     long_description=long_description,
     author='MessageMedia Developers',
     author_email='developers@messagemedia.com',
     url='https://developers.messagemedia.com',
     packages=find_packages(),
```

### Comparing `messagemedia-messages-sdk-2.1.1/tests/auth_manager_test.py` & `messagemedia-messages-sdk-2.1.2/tests/auth_manager_test.py`

 * *Files identical despite different names*

### Comparing `messagemedia-messages-sdk-2.1.1/tests/test_util.py` & `messagemedia-messages-sdk-2.1.2/tests/test_util.py`

 * *Files identical despite different names*

