# Comparing `tmp/vertica-python-1.3.2.tar.gz` & `tmp/vertica-python-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertica-python-1.3.2.tar", last modified: Wed Apr 19 08:47:54 2023, max compression
+gzip compressed data, was "vertica-python-1.3.3.tar", last modified: Tue Aug  1 03:55:29 2023, max compression
```

## Comparing `vertica-python-1.3.2.tar` & `vertica-python-1.3.3.tar`

### file list

```diff
@@ -1,112 +1,113 @@
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.499573 vertica-python-1.3.2/
--rw-rw-r--   0 sren      (1000) sren      (1000)    11357 2023-04-19 08:47:53.000000 vertica-python-1.3.2/LICENSE
--rw-rw-r--   0 sren      (1000) sren      (1000)      136 2023-04-19 08:47:53.000000 vertica-python-1.3.2/MANIFEST.in
--rw-rw-r--   0 sren      (1000) sren      (1000)     1393 2023-04-19 08:47:54.499573 vertica-python-1.3.2/PKG-INFO
--rw-rw-r--   0 sren      (1000) sren      (1000)    43416 2023-04-19 08:47:53.000000 vertica-python-1.3.2/README.md
--rw-rw-r--   0 sren      (1000) sren      (1000)       38 2023-04-19 08:47:54.499573 vertica-python-1.3.2/setup.cfg
--rw-rw-r--   0 sren      (1000) sren      (1000)     3662 2023-04-19 08:47:53.000000 vertica-python-1.3.2/setup.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.491573 vertica-python-1.3.2/vertica_python/
--rw-rw-r--   0 sren      (1000) sren      (1000)     3198 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4947 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/compat.py
--rw-rw-r--   0 sren      (1000) sren      (1000)    21640 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/datatypes.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     5635 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/errors.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2254 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/os_utils.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.491573 vertica-python-1.3.2/vertica_python/tests/
--rw-rw-r--   0 sren      (1000) sren      (1000)     1734 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/__init__.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.491573 vertica-python-1.3.2/vertica_python/tests/common/
--rw-rw-r--   0 sren      (1000) sren      (1000)     1734 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/common/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     6410 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/common/base.py
--rw-rw-r--   0 sren      (1000) sren      (1000)      821 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/conftest.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.491573 vertica-python-1.3.2/vertica_python/tests/integration_tests/
--rw-rw-r--   0 sren      (1000) sren      (1000)     1734 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     7563 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/base.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     5771 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_authentication.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4269 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_cancel.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4643 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_column.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4721 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_connection.py
--rw-rw-r--   0 sren      (1000) sren      (1000)    60985 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_cursor.py
--rw-rw-r--   0 sren      (1000) sren      (1000)    41668 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_datatypes.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     7524 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_dates.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2859 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_errors.py
--rw-rw-r--   0 sren      (1000) sren      (1000)    13199 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_loadbalance.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3843 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_timezones.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     5411 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_transfer_format.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4483 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_unicode.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.491573 vertica-python-1.3.2/vertica_python/tests/unit_tests/
--rw-rw-r--   0 sren      (1000) sren      (1000)     1734 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/unit_tests/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2361 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/unit_tests/base.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1967 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/unit_tests/test_errors.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1704 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/unit_tests/test_logging.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3233 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/unit_tests/test_notice.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4596 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/unit_tests/test_parsedsn.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3515 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/unit_tests/test_sql_literal.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4634 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/unit_tests/test_timestamps.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.495573 vertica-python-1.3.2/vertica_python/vertica/
--rw-rw-r--   0 sren      (1000) sren      (1000)     1735 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4861 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/column.py
--rw-rw-r--   0 sren      (1000) sren      (1000)    37620 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/connection.py
--rw-rw-r--   0 sren      (1000) sren      (1000)    44858 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/cursor.py
--rw-rw-r--   0 sren      (1000) sren      (1000)    25060 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/deserializer.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2575 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/log.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.495573 vertica-python-1.3.2/vertica_python/vertica/messages/
--rw-rw-r--   0 sren      (1000) sren      (1000)     2034 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/__init__.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.495573 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/
--rw-rw-r--   0 sren      (1000) sren      (1000)     3383 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3267 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/authentication.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2243 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/backend_key_data.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2008 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/bind_complete.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2010 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/close_complete.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3540 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/command_complete.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2979 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/command_description.py
--rw-rw-r--   0 sren      (1000) sren      (1000)      864 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/copy_done_response.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2182 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/copy_in_response.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2363 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/data_row.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2020 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/empty_query_response.py
--rw-rw-r--   0 sren      (1000) sren      (1000)      868 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/end_of_batch_response.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2137 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/error_response.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2401 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/load_balance_response.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1079 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/load_file.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1996 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/no_data.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3878 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/notice_response.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3542 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/parameter_description.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3024 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/parameter_status.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2010 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/parse_complete.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2669 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/portal_suspended.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2530 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/ready_for_query.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     6516 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/row_description.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2220 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/unknown.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2080 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/verify_files.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2261 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/write_file.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.495573 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/
--rw-rw-r--   0 sren      (1000) sren      (1000)     2753 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4867 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/bind.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2868 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/cancel_request.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2890 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/close.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2314 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/copy_data.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1905 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/copy_done.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1611 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/copy_error.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2451 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/copy_fail.py
--rwxrwxr-x   0 sren      (1000) sren      (1000)    10264 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/crypt_windows.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3396 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/describe.py
--rw-rw-r--   0 sren      (1000) sren      (1000)      973 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/end_of_batch_request.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2815 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/execute.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2274 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/flush.py
--rwxrwxr-x   0 sren      (1000) sren      (1000)     2078 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/load_balance_request.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2983 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/parse.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4274 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/password.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2521 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/query.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2054 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/ssl_request.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4743 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/startup.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1901 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/sync.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1906 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/terminate.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1317 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/verified_files.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     5183 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/message.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.499573 vertica-python-1.3.2/vertica_python/vertica/mixins/
--rw-rw-r--   0 sren      (1000) sren      (1000)      648 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/mixins/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3524 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/mixins/notice_response_attr.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.491573 vertica-python-1.3.2/vertica_python.egg-info/
--rw-rw-r--   0 sren      (1000) sren      (1000)     1393 2023-04-19 08:47:54.000000 vertica-python-1.3.2/vertica_python.egg-info/PKG-INFO
--rw-rw-r--   0 sren      (1000) sren      (1000)     5192 2023-04-19 08:47:54.000000 vertica-python-1.3.2/vertica_python.egg-info/SOURCES.txt
--rw-rw-r--   0 sren      (1000) sren      (1000)        1 2023-04-19 08:47:54.000000 vertica-python-1.3.2/vertica_python.egg-info/dependency_links.txt
--rw-rw-r--   0 sren      (1000) sren      (1000)       33 2023-04-19 08:47:54.000000 vertica-python-1.3.2/vertica_python.egg-info/requires.txt
--rw-rw-r--   0 sren      (1000) sren      (1000)       15 2023-04-19 08:47:54.000000 vertica-python-1.3.2/vertica_python.egg-info/top_level.txt
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.734635 vertica-python-1.3.3/
+-rw-rw-r--   0 sren      (1000) sren      (1000)    11357 2023-08-01 03:55:29.000000 vertica-python-1.3.3/LICENSE
+-rw-rw-r--   0 sren      (1000) sren      (1000)      136 2023-08-01 03:55:29.000000 vertica-python-1.3.3/MANIFEST.in
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1393 2023-08-01 03:55:29.734635 vertica-python-1.3.3/PKG-INFO
+-rw-rw-r--   0 sren      (1000) sren      (1000)    47396 2023-08-01 03:55:29.000000 vertica-python-1.3.3/README.md
+-rw-rw-r--   0 sren      (1000) sren      (1000)       38 2023-08-01 03:55:29.734635 vertica-python-1.3.3/setup.cfg
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3662 2023-08-01 03:55:29.000000 vertica-python-1.3.3/setup.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.726635 vertica-python-1.3.3/vertica_python/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3198 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4947 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/compat.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)    21640 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/datatypes.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     5635 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/errors.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2254 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/os_utils.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.726635 vertica-python-1.3.3/vertica_python/tests/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1734 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/__init__.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.726635 vertica-python-1.3.3/vertica_python/tests/common/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1734 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/common/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     6312 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/common/base.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)      821 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/conftest.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.730635 vertica-python-1.3.3/vertica_python/tests/integration_tests/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1734 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     7779 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/base.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     6453 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_authentication.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4269 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_cancel.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4643 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_column.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     7087 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_connection.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)    60985 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_cursor.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)    42970 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_datatypes.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     7524 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_dates.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2859 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_errors.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)    13199 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_loadbalance.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3843 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_timezones.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     9225 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_tls.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     5411 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_transfer_format.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4483 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_unicode.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.730635 vertica-python-1.3.3/vertica_python/tests/unit_tests/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1734 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/unit_tests/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2361 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/unit_tests/base.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1967 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/unit_tests/test_errors.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1704 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/unit_tests/test_logging.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3233 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/unit_tests/test_notice.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4811 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/unit_tests/test_parsedsn.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3515 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/unit_tests/test_sql_literal.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4634 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/unit_tests/test_timestamps.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.730635 vertica-python-1.3.3/vertica_python/vertica/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1735 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4861 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/column.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)    38153 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/connection.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)    45705 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/cursor.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)    25060 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/deserializer.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2575 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/log.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.730635 vertica-python-1.3.3/vertica_python/vertica/messages/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2034 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/__init__.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.734635 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3383 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3267 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/authentication.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2243 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/backend_key_data.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2008 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/bind_complete.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2010 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/close_complete.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2789 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/command_complete.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2979 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/command_description.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)      864 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/copy_done_response.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2182 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/copy_in_response.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2363 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/data_row.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2020 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/empty_query_response.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)      868 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/end_of_batch_response.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2137 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/error_response.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2401 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/load_balance_response.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1079 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/load_file.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1996 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/no_data.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3878 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/notice_response.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3542 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/parameter_description.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3024 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/parameter_status.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2010 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/parse_complete.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2669 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/portal_suspended.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2530 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/ready_for_query.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     6516 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/row_description.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2220 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/unknown.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2080 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/verify_files.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2261 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/write_file.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.734635 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2753 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4867 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/bind.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2868 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/cancel_request.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2890 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/close.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2314 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/copy_data.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1905 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/copy_done.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1611 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/copy_error.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2451 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/copy_fail.py
+-rwxrwxr-x   0 sren      (1000) sren      (1000)    10264 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/crypt_windows.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3396 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/describe.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)      973 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/end_of_batch_request.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2815 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/execute.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2274 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/flush.py
+-rwxrwxr-x   0 sren      (1000) sren      (1000)     2078 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/load_balance_request.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2983 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/parse.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4354 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/password.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2521 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/query.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2054 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/ssl_request.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     5059 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/startup.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1901 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/sync.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1906 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/terminate.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1317 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/verified_files.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     5183 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/message.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.734635 vertica-python-1.3.3/vertica_python/vertica/mixins/
+-rw-rw-r--   0 sren      (1000) sren      (1000)      648 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/mixins/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3524 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/mixins/notice_response_attr.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.726635 vertica-python-1.3.3/vertica_python.egg-info/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1393 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python.egg-info/PKG-INFO
+-rw-rw-r--   0 sren      (1000) sren      (1000)     5243 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 sren      (1000) sren      (1000)        1 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 sren      (1000) sren      (1000)       33 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python.egg-info/requires.txt
+-rw-rw-r--   0 sren      (1000) sren      (1000)       15 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python.egg-info/top_level.txt
```

### Comparing `vertica-python-1.3.2/LICENSE` & `vertica-python-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/PKG-INFO` & `vertica-python-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertica-python
-Version: 1.3.2
+Version: 1.3.3
 Summary: Official native Python client for the Vertica database.
 Home-page: https://github.com/vertica/vertica-python
 Author: Justin Berka, Alex Kim, Siting Ren
 Author-email: justin.berka@gmail.com, alex.kim@uber.com, sitingren@hotmail.com
 License: Apache License 2.0
 Description: vertica-python is the official Vertica database client for the Python programming language. Please check the [project homepage](https://github.com/vertica/vertica-python) for the details.
 Keywords: database vertica
```

### Comparing `vertica-python-1.3.2/README.md` & `vertica-python-1.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # vertica-python
 
-[![PyPI version](https://badge.fury.io/py/vertica-python.svg)](https://badge.fury.io/py/vertica-python)
+[![PyPI version](https://img.shields.io/pypi/v/vertica-python?color=brightgreen&label=PyPI%20package)](https://pypi.org/project/vertica-python/)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/vertica-python?color=yellowgreen)](https://anaconda.org/conda-forge/vertica-python)
 [![License](https://img.shields.io/badge/License-Apache%202.0-orange.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Python Version](https://img.shields.io/pypi/pyversions/vertica-python.svg)](https://www.python.org/downloads/)
 [![Downloads](https://pepy.tech/badge/vertica-python/week)](https://pepy.tech/project/vertica-python)
 
 *vertica-python* is a native Python client for the Vertica (http://www.vertica.com) database. *vertica-python* is the replacement of the deprecated Python client *vertica_db_client*, which was removed since Vertica server version 9.3.
 
 :loudspeaker: 08/14/2018: *vertica-python* becomes Vertica’s first officially supported open source database client, see the blog [here](https://my.vertica.com/blog/vertica-python-becomes-verticas-first-officially-supported-open-source-database-client/).
 
 Please check out [release notes](https://github.com/vertica/vertica-python/releases) to learn about the latest improvements.
 
-vertica-python has been tested with Vertica 12.0.4 and Python 3.7/3.8/3.9/3.10/3.11. Feel free to submit issues and/or pull requests (Read up on our [contributing guidelines](#contributing-guidelines)).
+vertica-python has been tested with Vertica 23.3.0 and Python 3.7/3.8/3.9/3.10/3.11. Feel free to submit issues and/or pull requests (Read up on our [contributing guidelines](#contributing-guidelines)).
 
 
 ## Installation
 
 To install vertica-python with pip:
 ```bash
 # Latest release version
@@ -98,20 +99,22 @@
 | connection_load_balance | See [Connection Load Balancing](#connection-load-balancing). <br>**_Default_**: False (disabled) |
 | connection_timeout | The number of seconds (can be a nonnegative floating point number) the client waits for a socket operation (Establishing a TCP connection or read/write operation). <br>**_Default_**: None (no timeout) |
 | disable_copy_local | See [COPY FROM LOCAL](#method-2-copy-from-local-sql-with-cursorexecute). <br>**_Default_**: False |
 | kerberos_host_name | See [Kerberos Authentication](#kerberos-authentication). <br>**_Default_**: the value of connection option `host` |
 | kerberos_service_name | See [Kerberos Authentication](#kerberos-authentication). <br>**_Default_**: "vertica" |
 | log_level | See [Logging](#logging). |
 | log_path | See [Logging](#logging). |
+| oauth_access_token | To authenticate via OAuth, provide an OAuth Access Token that authorizes a user to the database. <br>**_Default_**: "" |
+| request_complex_types | See [SQL Data conversion to Python objects](#sql-data-conversion-to-python-objects). <br>**_Default_**: True |
 | session_label | Sets a label for the connection on the server. This value appears in the client_label column of the _v_monitor.sessions_ system table. <br>**_Default_**: an auto-generated label with format of `vertica-python-{version}-{random_uuid}` |
 | ssl | See [TLS/SSL](#tlsssl). <br>**_Default_**: False (disabled) |
 | unicode_error | See [UTF-8 encoding issues](#utf-8-encoding-issues). <br>**_Default_**: 'strict' (throw error on invalid UTF-8 results) |
 | use_prepared_statements | See [Passing parameters to SQL queries](#passing-parameters-to-sql-queries). <br>**_Default_**: False |
+| workload | Sets the workload name associated with this session. Valid values are workload names that already exist in a workload routing rule on the server. If a workload name that doesn't exist is entered, the server will reject it and it will be set to the default. <br>**_Default_**: "" |
 | dsn | See [Set Properties with Connection String](#set-properties-with-connection-string). |
-| request_complex_types | See [SQL Data conversion to Python objects](#sql-data-conversion-to-python-objects). <br>**_Default_**: True |
 
 
 Below are a few important connection topics you may deal with, or you can skip and jump to the next section: [Send Queries and Retrieve Results](#send-queries-and-retrieve-results)
 
 #### Set Properties with Connection String
 Another way to set connection properties is passing a connection string to the keyword parameter `dsn` of `vertica_python.connect(dsn='...', **kwargs)`. The connection string is of the form:
 ```
@@ -134,33 +137,107 @@
     }
 
 with vertica_python.connect(dsn=connection_str, **additional_info) as conn:
    # do things
 ```
 
 #### TLS/SSL
-You can pass an `ssl.SSLContext` to `ssl` to customize the SSL connection options. For example,
+You can pass `True` to `ssl` to enable TLS/SSL connection (Internally [ssl.wrap_socket(sock)](https://docs.python.org/3/library/ssl.html#ssl.wrap_socket) is called).
+
+```python
+import vertica_python
+
+# [TLSMode: require]
+conn_info = {'host': '127.0.0.1',
+             'port': 5433,
+             'user': 'some_user',
+             'password': 'some_password',
+             'database': 'a_database',
+             'ssl': True}
+connection = vertica_python.connect(**conn_info)
+```
+
+You can pass an `ssl.SSLContext` to `ssl` to customize the SSL connection options. Server mode TLS examples:
 
 ```python
 import vertica_python
 import ssl
 
-ssl_context = ssl.SSLContext(ssl.PROTOCOL_SSLv23)
+# [TLSMode: require]
+# Ensure connection is encrypted.
+ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
+ssl_context.check_hostname = False
+ssl_context.verify_mode = ssl.CERT_NONE
+
+conn_info = {'host': '127.0.0.1',
+             'port': 5433,
+             'user': 'some_user',
+             'password': 'some_password',
+             'database': 'a_database',
+             'ssl': ssl_context}
+connection = vertica_python.connect(**conn_info)
+
+
+# [TLSMode: verify-ca]
+# Ensure connection is encrypted, and client trusts server certificate.
+ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
+ssl_context.verify_mode = ssl.CERT_REQUIRED
+ssl_context.check_hostname = False
+ssl_context.load_verify_locations(cafile='/path/to/ca_file.pem') # CA certificate used to verify server certificate
+
+conn_info = {'host': '127.0.0.1',
+             'port': 5433,
+             'user': 'some_user',
+             'password': 'some_password',
+             'database': 'a_database',
+             'ssl': ssl_context}
+connection = vertica_python.connect(**conn_info)
+
+
+# [TLSMode: verify-full]
+# Ensure connection is encrypted, client trusts server certificate,
+# and server hostname matches the one listed in the server certificate.
+ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
 ssl_context.verify_mode = ssl.CERT_REQUIRED
 ssl_context.check_hostname = True
-ssl_context.load_verify_locations(cafile='/path/to/ca_file.pem')
+ssl_context.load_verify_locations(cafile='/path/to/ca_file.pem') # CA certificate used to verify server certificate
 
 conn_info = {'host': '127.0.0.1',
              'port': 5433,
              'user': 'some_user',
              'password': 'some_password',
              'database': 'a_database',
              'ssl': ssl_context}
 connection = vertica_python.connect(**conn_info)
+```
 
+Mutual mode TLS example:
+```python
+import vertica_python
+import ssl
+
+# [TLSMode: verify-full]
+# Ensure connection is encrypted, client trusts server certificate,
+# and server hostname matches the one listed in the server certificate.
+ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
+ssl_context.verify_mode = ssl.CERT_REQUIRED
+ssl_context.check_hostname = True
+ssl_context.load_verify_locations(cafile='/path/to/ca_file.pem') # CA certificate used to verify server certificate
+
+# For Mutual mode, provide client certificate and client private key to ssl_context.
+# CA certificate used to verify client certificate should be set at the server side.
+ssl_context.load_cert_chain(certfile='/path/to/client.pem', keyfile='/path/to/client.key')
+
+conn_info = {'host': '127.0.0.1',
+             'port': 5433,
+             'user': 'some_user',
+             'password': 'some_password',
+             'database': 'a_database',
+             'ssl': ssl_context}
+connection = vertica_python.connect(**conn_info)
 ```
 
 See more on SSL options [here](https://docs.python.org/3/library/ssl.html).
 
 #### Kerberos Authentication
 In order to use Kerberos authentication, install [dependencies](#using-kerberos-authentication) first, and it is the user's responsibility to ensure that an Ticket-Granting Ticket (TGT) is available and valid. Whether a TGT is available can be easily determined by running the `klist` command. If no TGT is available, then it first must be obtained by running the `kinit` command or by logging in. You can pass in optional arguments to customize the authentication. The arguments are `kerberos_service_name`, which defaults to "vertica", and `kerberos_host_name`, which defaults to the value of argument `host`. For example,
 
@@ -572,14 +649,18 @@
 
 cur.execute("INSERT INTO table VALUES (%s, %s)", [100, value], use_prepared_statements=False)  # WRONG
 # Error Message: Column "b" is of type array[date] but expression is of type array[varchar], Sqlstate: 42804, 
 # Hint: You will need to rewrite or cast the expression
 
 cur.execute("INSERT INTO table VALUES (%s, %s::ARRAY[DATE])", [100, value], use_prepared_statements=False)  # correct
 # converted into a SQL command: INSERT INTO vptest VALUES (100, ARRAY['2021-06-10','2021-06-12','2021-06-30']::ARRAY[DATE])
+
+# Client-side binding of cursor.executemany is different from cursor.execute internally
+# But it also supports some of complex types mapping
+cur.executemany("INSERT INTO table (a, b) VALUES (%s, %s)", [[100, value]], use_prepared_statements=False)
 ```
 
 ##### Register new SQL literal adapters
 It is possible to adapt new Python types to SQL literals via `Cursor.register_sql_literal_adapter(py_class_or_type, adapter_function)` function. Example:
 ```python
 class Point(object):
     def __init__(self, x, y):
@@ -742,14 +823,21 @@
     with open('f1.csv', 'r') as fs1, open('f2.csv', 'r') as fs2:
         cur.execute("COPY tlb1(field1, field2) FROM LOCAL STDIN DELIMITER ',';"
                     "COPY tlb2(field1, field2) FROM LOCAL STDIN DELIMITER ',';",
                     copy_stdin=[fs1, fs2], buffer_size=65536)
     print("Rows loaded 1:", cur.fetchall())
     cur.nextset()
     print("Rows loaded 2:", cur.fetchall())
+    
+    # Copy from local stdin (StringIO)
+    from io import StringIO
+    data = "Anna|123-456-789\nBrown|555-444-3333\nCindy|555-867-53093453453\nDodd|123-456-789\nEd|123-456-789"
+    cur.execute("COPY customers (firstNames, phoneNumbers) FROM LOCAL STDIN ENFORCELENGTH RETURNREJECTED AUTO",
+                copy_stdin=StringIO(data))
+
 ```
 When connection option `disable_copy_local` set to True, disables COPY LOCAL operations, including copying data from local files/stdin and using local files to store data and exceptions. You can use this property to prevent users from writing to and copying from files on a Vertica host, including an MC host. Note that this property doesn't apply to `Cursor.copy()`.
 
 The data for copying from/writing to local files is streamed in chunks of `buffer_size` bytes, which defaults to 128 * 2 ** 10.
 
 When executing "COPY FROM LOCAL STDIN", `copy_stdin` should be a file-like object or a list of file-like objects (specifically, any object with a `read()` method).
```

### Comparing `vertica-python-1.3.2/setup.py` & `vertica-python-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 ReqOpts = collections.namedtuple('ReqOpts', ['skip_requirements_regex', 'default_vcs'])
 
 opts = ReqOpts(None, 'git')
 
 # version should use the format 'x.x.x' (instead of 'vx.x.x')
 setup(
     name='vertica-python',
-    version='1.3.2',
+    version='1.3.3',
     description='Official native Python client for the Vertica database.',
     long_description="vertica-python is the official Vertica database client for the Python programming language. Please check the [project homepage](https://github.com/vertica/vertica-python) for the details.",
     long_description_content_type='text/markdown',
     author='Justin Berka, Alex Kim, Siting Ren',
     author_email='justin.berka@gmail.com, alex.kim@uber.com, sitingren@hotmail.com',
     url='https://github.com/vertica/vertica-python',
     keywords="database vertica",
```

### Comparing `vertica-python-1.3.2/vertica_python/__init__.py` & `vertica-python-1.3.3/vertica_python/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,19 +52,19 @@
 
 __all__ = ['Connection', 'PROTOCOL_VERSION', 'version_info', 'apilevel', 'threadsafety',
            'paramstyle', 'connect', 'parse_dsn', 'Error', 'Warning', 'DataError', 'DatabaseError',
            'IntegrityError', 'InterfaceError', 'InternalError', 'NotSupportedError',
            'OperationalError', 'ProgrammingError']
 
 # The version number of this library.
-version_info = (1, 3, 2)
+version_info = (1, 3, 3)
 __version__ = '.'.join(map(str, version_info))
 
-# The protocol version (3.14) implemented in this library.
-PROTOCOL_VERSION = 3 << 16 | 14
+# The protocol version (3.15) implemented in this library.
+PROTOCOL_VERSION = 3 << 16 | 15
 
 apilevel = 2.0
 threadsafety = 1  # Threads may share the module, but not connections!
 
 # Accepted paramstyles are
 #   'qmark' = Question mark style, e.g. '...WHERE name=?'
 #   'named' = Named style, e.g. '...WHERE name=:name'
```

### Comparing `vertica-python-1.3.2/vertica_python/compat.py` & `vertica-python-1.3.3/vertica_python/compat.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/datatypes.py` & `vertica-python-1.3.3/vertica_python/datatypes.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/errors.py` & `vertica-python-1.3.3/vertica_python/errors.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/os_utils.py` & `vertica-python-1.3.3/vertica_python/os_utils.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/tests/__init__.py` & `vertica-python-1.3.3/vertica_python/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/tests/common/__init__.py` & `vertica-python-1.3.3/vertica_python/tests/common/__init__.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/tests/common/base.py` & `vertica-python-1.3.3/vertica_python/tests/common/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,30 +50,32 @@
 default_configs = {
     'log_dir': 'vp_test_log',
     'log_level': logging.WARNING,
     'host': 'localhost',
     'port': 5433,
     'user': getpass.getuser(),
     'password': '',
+    'database': '',
+    'oauth_access_token': '',
+    'oauth_user': '',
 }
 
 
 class VerticaPythonTestCase(unittest.TestCase):
     """
     Base class for all tests
     """
 
     @classmethod
     def _load_test_config(cls, config_list):
         test_config = {}
 
         # load default configurations
         for key in config_list:
-            if key != 'database':
-                test_config[key] = default_configs[key]
+            test_config[key] = default_configs[key]
 
         # override with the configuration file
         confparser = ConfigParser()
         confparser.optionxform = str
         SECTION = 'vp_test_config'  # section name in the configuration file
         # the configuration file is placed in the same directory as this file
         conf_file = os.path.join(os.path.dirname(os.path.abspath(__file__)),
@@ -90,16 +92,14 @@
             if env in os.environ:
                 test_config[k] = os.environ[env]
 
         # data preprocessing
         # value is string when loaded from configuration file and environment variable
         if 'port' in test_config:
             test_config['port'] = int(test_config['port'])
-        if 'database' in config_list and 'user' in test_config:
-            test_config.setdefault('database', test_config['user'])
         if 'log_level' in test_config:
             levels = ['NOTSET', 'DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL']
             if isinstance(test_config['log_level'], str):
                 if test_config['log_level'] not in levels:
                     raise ValueError("Invalid value for VP_TEST_LOG_LEVEL: '{}'".format(test_config['log_level']))
                 test_config['log_level'] = eval('logging.' + test_config['log_level'])
         if 'log_dir' in test_config:
```

### Comparing `vertica-python-1.3.2/vertica_python/tests/conftest.py` & `vertica-python-1.3.3/vertica_python/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/tests/integration_tests/__init__.py` & `vertica-python-1.3.3/vertica_python/tests/integration_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/tests/integration_tests/base.py` & `vertica-python-1.3.3/vertica_python/tests/integration_tests/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,16 @@
     connection info used for all the tests, and provides support code
     to do common assertions and execute common queries.
     """
 
     @classmethod
     def setUpClass(cls):
         config_list = ['log_dir', 'log_level', 'host', 'port',
-                       'user', 'password', 'database']
+                       'user', 'password', 'database',
+                       'oauth_access_token', 'oauth_user',]
         cls.test_config = cls._load_test_config(config_list)
 
         # Test logger
         logfile = cls._setup_logger('integration_tests',
                       cls.test_config['log_dir'], cls.test_config['log_level'])
 
         # Connection info
@@ -69,14 +70,18 @@
             'port': cls.test_config['port'],
             'database': cls.test_config['database'],
             'user': cls.test_config['user'],
             'password': cls.test_config['password'],
             'log_level': cls.test_config['log_level'],
             'log_path': logfile,
         }
+        cls._oauth_info = {
+            'access_token': cls.test_config['oauth_access_token'],
+            'user': cls.test_config['oauth_user'],
+        }
         cls.db_node_num = cls._get_node_num()
         cls.logger.info("Number of database node(s) = {}".format(cls.db_node_num))
 
     @classmethod
     def tearDownClass(cls):
         pass
```

### Comparing `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_authentication.py` & `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_authentication.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,16 @@
         super(AuthenticationTestCase, self).setUp()
         self._user = self._conn_info['user']
         self._password = self._conn_info['password']
 
     def tearDown(self):
         self._conn_info['user'] = self._user
         self._conn_info['password'] = self._password
+        if 'oauth_access_token' in self._conn_info:
+            del self._conn_info['oauth_access_token']
         super(AuthenticationTestCase, self).tearDown()
 
     def test_SHA512(self):
         with self._connect() as conn:
             cur = conn.cursor()
             cur.execute("DROP USER IF EXISTS sha512_user")
             cur.execute("DROP AUTHENTICATION IF EXISTS testIPv4hostHash CASCADE")
@@ -103,9 +105,22 @@
                 # matter whether an exception has occurred or not, otherwise
                 # those authentication methods may affect existing users
                 cur.execute("DROP USER IF EXISTS pw_expire_user")
                 cur.execute("DROP AUTHENTICATION IF EXISTS testIPv4hostHash CASCADE")
                 cur.execute("DROP AUTHENTICATION IF EXISTS testIPv6hostHash CASCADE")
                 cur.execute("DROP AUTHENTICATION IF EXISTS testlocalHash CASCADE")
 
+    def test_oauth(self):
+        self.require_protocol_at_least(3 << 16 | 11)
+        if not self._oauth_info['access_token']:
+            self.skipTest('OAuth not set')
+
+        self._conn_info['user'] = self._oauth_info['user']
+        self._conn_info['oauth_access_token'] = self._oauth_info['access_token']
+        with self._connect() as conn:
+            cur = conn.cursor()
+            cur.execute("SELECT authentication_method FROM sessions WHERE session_id=(SELECT current_session())")
+            res = cur.fetchone()
+            self.assertEqual(res[0], 'OAuth')
+
 
 exec(AuthenticationTestCase.createPrepStmtClass())
```

### Comparing `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_cancel.py` & `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_cancel.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_column.py` & `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_column.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_cursor.py` & `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_datatypes.py` & `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_datatypes.py`

 * *Files 11% similar despite different names*

```diff
@@ -86,116 +86,127 @@
 
     def tearDown(self):
         with self._connect() as conn:
             cur = conn.cursor()
             cur.execute(f"DROP TABLE IF EXISTS {self._table}")
         super(InsertComplexTypeTestCase, self).tearDown()
 
-    def _test_insert_complex_type(self, col_type, values, expected=None):
+    def _test_insert_complex_type(self, col_type, values, expected=None, test_executemany=False):
         if expected is None:
             expected = values
         with self._connect() as conn:
             cur = conn.cursor()
             cur.execute(f"DROP TABLE IF EXISTS {self._table}")
             cur.execute(f"CREATE TABLE {self._table} (a INT, b {col_type})")
-            a = 1
-            for value in values:
+            seq_of_values = [(i, values[i]) for i in range(len(values))]
+            for value in seq_of_values:
                 # Some cases need explicit typecasting
-                cur.execute(f"INSERT INTO {self._table} (a, b) VALUES (%s, %s::{col_type})", [a, value], use_prepared_statements=False)
-                a += 1
+                cur.execute(f"INSERT INTO {self._table} (a, b) VALUES (%s, %s::{col_type})", value, use_prepared_statements=False)
             rows = cur.execute(f"SELECT b FROM {self._table} ORDER BY a").fetchall()
             results = [row[0] for row in rows]
             self.assertEqual(results, expected)
 
+            if not test_executemany:
+                return
+            # test cursor.executemany
+            cur.execute(f"TRUNCATE TABLE {self._table}")
+            cur.executemany(f"INSERT INTO {self._table} (a, b) VALUES (%s, %s)", seq_of_values, use_prepared_statements=False)
+            rows = cur.execute(f"SELECT b FROM {self._table} ORDER BY a").fetchall()
+            results = [row[0] for row in rows]
+            self.assertEqual(results, expected)
+
+
     #######################
     # tests for ARRAY type
     #######################
     def test_Array_boolean_type(self):
-        self._test_insert_complex_type('ARRAY[BOOL]', [[True, False, None], None, [], [None]])
+        self._test_insert_complex_type('ARRAY[BOOL]', [[True, False, None], None, [], [None]], test_executemany=True)
 
     def test_Array_integer_type(self):
-        self._test_insert_complex_type('ARRAY[INT]', [[1,-2,3], [4,None,5], None, [], [None]])
+        self._test_insert_complex_type('ARRAY[INT]', [[1,-2,3], [4,None,5], None, [], [None]], test_executemany=True)
         self._test_insert_complex_type('ARRAY[ARRAY[INT]]', [[[1,2], [3,4], None, [5,None], []],
             None, [], [None]])
         self._test_insert_complex_type('ARRAY[ARRAY[ARRAY[ARRAY[INT]]]]', [[[[None,[1,2,3],None,[1,None,3],[None,None,None],[4,5],[],None]]],
             None, [], [None]])
 
     def test_Array_float_type(self):
-        self._test_insert_complex_type('ARRAY[FLOAT]', [[1.23456e-18,float('Inf'),float('-Inf'),None,-1.234,0.0], None, [], [None]])
+        self._test_insert_complex_type('ARRAY[FLOAT]', [[1.23456e-18,float('Inf'),float('-Inf'),None,-1.234,0.0], None, [], [None]], test_executemany=True)
 
     def test_Array_numeric_type(self):
         self._test_insert_complex_type('ARRAY[NUMERIC]', [[Decimal('-1.1200000000'), Decimal('0E-10'), None, Decimal('1234567890123456789.0123456789')],
-            None, [], [None]])
+            None, [], [None]], test_executemany=True)
 
     def test_Array_char_type(self):
-        self._test_insert_complex_type('ARRAY[CHAR(3)]', [['a', u'\u16b1', None, 'foo'], None, [], [None]], [['a  ', u'\u16b1', None, 'foo'], None, [], [None]])
+        self._test_insert_complex_type('ARRAY[CHAR(3)]', [['a', u'\u16b1', None, 'foo'], None, [], [None]], [['a  ', u'\u16b1', None, 'foo'], None, [], [None]], test_executemany=True)
 
     def test_Array_varchar_type(self):
-        self._test_insert_complex_type('ARRAY[VARCHAR(10)]', [['', u'\u16b1\nb', None, 'foo'], None, [], [None]])
+        self._test_insert_complex_type('ARRAY[VARCHAR(10)]', [['', u'\u16b1\nb', None, 'foo'], None, [], [None]], test_executemany=True)
+        self._test_insert_complex_type('ARRAY[VARCHAR]', [[chr(i)] for i in range(1, 128)], test_executemany=True)
 
     def test_Array_date_type(self):
-        self._test_insert_complex_type('ARRAY[DATE]', [[date(2021, 6, 10),None,date(221, 5, 2)], None, [], [None]])
+        self._test_insert_complex_type('ARRAY[DATE]', [[date(2021, 6, 10),None,date(221, 5, 2)], None, [], [None]], test_executemany=True)
 
     def test_Array_time_type(self):
-        self._test_insert_complex_type('ARRAY[TIME(3)]', [[time(0, 0, 0),None,time(22, 36, 33, 124000)], None, [], [None]])
+        self._test_insert_complex_type('ARRAY[TIME(3)]', [[time(0, 0, 0),None,time(22, 36, 33, 124000)], None, [], [None]], test_executemany=True)
 
     def test_Array_timetz_type(self):
         self._test_insert_complex_type('ARRAY[TIMETZ(3)]', [[time(22, 36, 33, 123000, tzinfo=tzoffset(None, 23400)),None,
-            time(22, 36, 33, 123000, tzinfo=tzoffset(None, -10800))], None, [], [None]])
+            time(22, 36, 33, 123000, tzinfo=tzoffset(None, -10800))], None, [], [None]], test_executemany=True)
 
     def test_Array_timestamp_type(self):
-        self._test_insert_complex_type('ARRAY[TIMESTAMP]', [[datetime(276, 12, 1, 11, 22, 33),None,datetime(2001, 12, 1, 0, 30, 45, 87000)], None, [], [None]])
+        self._test_insert_complex_type('ARRAY[TIMESTAMP]', [[datetime(276, 12, 1, 11, 22, 33),None,datetime(2001, 12, 1, 0, 30, 45, 87000)], None, [], [None]], test_executemany=True)
 
     def test_Array_timestamptz_type(self):
-        self._test_insert_complex_type('ARRAY[TIMESTAMPTZ]', [[datetime(276, 11, 30, 23, 32, 57, tzinfo=tzoffset(None, 3600)),None,datetime(2001, 12, 1, 0, 30, 45, 87000, tzinfo=tzoffset(None, -18000))], None, [], [None]])
+        self._test_insert_complex_type('ARRAY[TIMESTAMPTZ]', [[datetime(276, 11, 30, 23, 32, 57, tzinfo=tzoffset(None, 3600)),None,datetime(2001, 12, 1, 0, 30, 45, 87000, tzinfo=tzoffset(None, -18000))], None, [], [None]], test_executemany=True)
 
     def test_Array_UUID_type(self):
-        self._test_insert_complex_type('ARRAY[UUID]', [[UUID('00010203-0405-0607-0809-0a0b0c0d0e0f'),None,UUID('123e4567-e89b-12d3-a456-426655440a00')], None, [], [None]])
+        self._test_insert_complex_type('ARRAY[UUID]', [[UUID('00010203-0405-0607-0809-0a0b0c0d0e0f'),None,UUID('123e4567-e89b-12d3-a456-426655440a00')], None, [], [None]], test_executemany=True)
 
     #####################
     # tests for SET type
     #####################
     def test_1DSet_boolean_type(self):
-        self._test_insert_complex_type('SET[BOOL]', [{True, False, None}, None, set(), {None}])
+        self._test_insert_complex_type('SET[BOOL]', [{True, False, None}, None, set(), {None}], test_executemany=True)
 
     def test_1DSet_integer_type(self):
-        self._test_insert_complex_type('SET[INT]', [{0, 1, -2, 3, None}, None, set(), {None}])
+        self._test_insert_complex_type('SET[INT]', [{0, 1, -2, 3, None}, None, set(), {None}], test_executemany=True)
 
     def test_1DSet_float_type(self):
-        self._test_insert_complex_type('SET[FLOAT]', [{float('Inf'), float('-Inf'), None, -1.234, 0.0, 1.23456e-18}, None, set(), {None}])
+        self._test_insert_complex_type('SET[FLOAT]', [{float('Inf'), float('-Inf'), None, -1.234, 0.0, 1.23456e-18}, None, set(), {None}], test_executemany=True)
 
     def test_1DSet_numeric_type(self):
         self._test_insert_complex_type('SET[NUMERIC]', [{Decimal('-1.12'), Decimal('0E-15'), None, Decimal('1234567890123456789.0123456789')},
-            None, set(), {None}])
+            None, set(), {None}], test_executemany=True)
 
     def test_1DSet_char_type(self):
-        self._test_insert_complex_type('SET[CHAR(3)]', [{'a  ', u'\u16b1', None, 'foo'}, None, set(), {None}])
+        self._test_insert_complex_type('SET[CHAR(3)]', [{'a  ', u'\u16b1', None, 'foo'}, None, set(), {None}], test_executemany=True)
 
     def test_1DSet_varchar_type(self):
-        self._test_insert_complex_type('SET[VARCHAR(10)]', [{'', u'\u16b1\nb', None, 'foo'}, None, set(), {None}])
+        self._test_insert_complex_type('SET[VARCHAR(10)]', [{'', u'\u16b1\nb', None, 'foo'}, None, set(), {None}], test_executemany=True)
+        self._test_insert_complex_type('SET[VARCHAR]', [{chr(i)} for i in range(1, 128)], test_executemany=True)
 
     def test_1DSet_date_type(self):
-        self._test_insert_complex_type('SET[DATE]', [{date(2021, 6, 10), None, date(221, 5, 2)}, None, set(), {None}])
+        self._test_insert_complex_type('SET[DATE]', [{date(2021, 6, 10), None, date(221, 5, 2)}, None, set(), {None}], test_executemany=True)
 
     def test_1DSet_time_type(self):
-        self._test_insert_complex_type('SET[TIME(3)]', [{time(0, 0, 0), None, time(22, 36, 33, 124000)}, None, set(), {None}])
+        self._test_insert_complex_type('SET[TIME(3)]', [{time(0, 0, 0), None, time(22, 36, 33, 124000)}, None, set(), {None}], test_executemany=True)
 
     def test_1DSet_timetz_type(self):
         self._test_insert_complex_type('SET[TIMETZ(3)]', [{time(22, 36, 33, 123000, tzinfo=tzoffset(None, 23400)),None,
-            time(22, 36, 33, 123000, tzinfo=tzoffset(None, -10800))}, None, set(), {None}])
+            time(22, 36, 33, 123000, tzinfo=tzoffset(None, -10800))}, None, set(), {None}], test_executemany=True)
 
     def test_1DSet_timestamp_type(self):
-        self._test_insert_complex_type('SET[TIMESTAMP]', [{datetime(276, 12, 1, 11, 22, 33),None,datetime(2001, 12, 1, 0, 30, 45, 87000)}, None, set(), {None}])
+        self._test_insert_complex_type('SET[TIMESTAMP]', [{datetime(276, 12, 1, 11, 22, 33),None,datetime(2001, 12, 1, 0, 30, 45, 87000)}, None, set(), {None}], test_executemany=True)
 
     def test_1DSet_timestamptz_type(self):
         self._test_insert_complex_type('SET[TIMESTAMPTZ]', [{datetime(276, 11, 30, 23, 32, 57, tzinfo=tzoffset(None, 3600)),None,
-            datetime(2001, 12, 1, 0, 30, 45, 87000, tzinfo=tzoffset(None, -18000))}, None, set(), {None}])
+            datetime(2001, 12, 1, 0, 30, 45, 87000, tzinfo=tzoffset(None, -18000))}, None, set(), {None}], test_executemany=True)
 
     def test_1DSet_UUID_type(self):
-        self._test_insert_complex_type('SET[UUID]', [{UUID('00010203-0405-0607-0809-0a0b0c0d0e0f'),None,UUID('123e4567-e89b-12d3-a456-426655440a00')}, None, set(), {None}])
+        self._test_insert_complex_type('SET[UUID]', [{UUID('00010203-0405-0607-0809-0a0b0c0d0e0f'),None,UUID('123e4567-e89b-12d3-a456-426655440a00')}, None, set(), {None}], test_executemany=True)
 
     #####################
     # tests for ROW type
     #####################
     def test_row_boolean_type(self):
         self._test_insert_complex_type('ROW(BOOL, ARRAY[BOOL], ROW(BOOL, ARRAY[BOOL]))', [
                 {'f0': True, 'f1': [None, False], 'f2': {'f0': False, 'f1': [True, None]}},
```

### Comparing `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_dates.py` & `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_dates.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_errors.py` & `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_loadbalance.py` & `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_loadbalance.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_timezones.py` & `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_timezones.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_transfer_format.py` & `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_transfer_format.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_unicode.py` & `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/tests/unit_tests/__init__.py` & `vertica-python-1.3.3/vertica_python/tests/unit_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/tests/unit_tests/base.py` & `vertica-python-1.3.3/vertica_python/tests/unit_tests/base.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/tests/unit_tests/test_errors.py` & `vertica-python-1.3.3/vertica_python/tests/unit_tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/tests/unit_tests/test_logging.py` & `vertica-python-1.3.3/vertica_python/tests/unit_tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/tests/unit_tests/test_notice.py` & `vertica-python-1.3.3/vertica_python/tests/unit_tests/test_notice.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/tests/unit_tests/test_parsedsn.py` & `vertica-python-1.3.3/vertica_python/tests/unit_tests/test_parsedsn.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,19 +37,23 @@
         parsed = parse_dsn(dsn)
         self.assertDictEqual(expected, parsed)
 
     def test_str_arguments(self):
         dsn = ('vertica://john:pwd@localhost:5433/db1?'
                'session_label=vpclient&unicode_error=strict&'
                'log_path=/home/admin/vClient.log&log_level=DEBUG&'
+               'oauth_access_token=GciOiJSUzI1NiI&'
+               'workload=python_test_workload&'
                'kerberos_service_name=krb_service&kerberos_host_name=krb_host')
         expected = {'database': 'db1', 'host': 'localhost', 'user': 'john',
                     'password': 'pwd', 'port': 5433, 'log_level': 'DEBUG',
                     'session_label': 'vpclient', 'unicode_error': 'strict',
-                    'log_path': '/home/admin/vClient.log', 
+                    'log_path': '/home/admin/vClient.log',
+                    'oauth_access_token': 'GciOiJSUzI1NiI',
+                    'workload': 'python_test_workload',
                     'kerberos_service_name': 'krb_service',
                     'kerberos_host_name': 'krb_host'}
         parsed = parse_dsn(dsn)
         self.assertDictEqual(expected, parsed)
 
     def test_boolean_arguments(self):
         dsn = ('vertica://mike@127.0.0.1/db1?connection_load_balance=True&'
```

### Comparing `vertica-python-1.3.2/vertica_python/tests/unit_tests/test_sql_literal.py` & `vertica-python-1.3.3/vertica_python/tests/unit_tests/test_sql_literal.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/tests/unit_tests/test_timestamps.py` & `vertica-python-1.3.3/vertica_python/tests/unit_tests/test_timestamps.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/__init__.py` & `vertica-python-1.3.3/vertica_python/vertica/__init__.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/column.py` & `vertica-python-1.3.3/vertica_python/vertica/column.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/connection.py` & `vertica-python-1.3.3/vertica_python/vertica/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,16 @@
 DEFAULT_AUTOCOMMIT = False
 DEFAULT_BACKUP_SERVER_NODE = []
 DEFAULT_KRB_SERVICE_NAME = 'vertica'
 DEFAULT_LOG_LEVEL = logging.WARNING
 DEFAULT_LOG_PATH = 'vertica_python.log'
 DEFAULT_BINARY_TRANSFER = False
 DEFAULT_REQUEST_COMPLEX_TYPES = True
+DEFAULT_OAUTH_ACCESS_TOKEN = ''
+DEFAULT_WORKLOAD = ''
 try:
     DEFAULT_USER = getpass.getuser()
 except Exception as e:
     DEFAULT_USER = None
     warnings.warn(f"Cannot get the login user name: {str(e)}")
 
 
@@ -284,17 +286,19 @@
                 self.options['user'] = DEFAULT_USER
             else:
                 msg = 'Connection option "user" is required'
                 self._logger.error(msg)
                 raise KeyError(msg)
         self.options.setdefault('database', DEFAULT_DATABASE)
         self.options.setdefault('password', DEFAULT_PASSWORD)
+        self.options.setdefault('oauth_access_token', DEFAULT_OAUTH_ACCESS_TOKEN)
         self.options.setdefault('autocommit', DEFAULT_AUTOCOMMIT)
         self.options.setdefault('session_label', _generate_session_label())
         self.options.setdefault('backup_server_node', DEFAULT_BACKUP_SERVER_NODE)
+        self.options.setdefault('workload', DEFAULT_WORKLOAD)
         self.options.setdefault('kerberos_service_name', DEFAULT_KRB_SERVICE_NAME)
         # Kerberos authentication hostname defaults to the host value here so
         # the correct value cannot be overwritten by load balancing or failover
         self.options.setdefault('kerberos_host_name', self.options['host'])
 
         self.address_list = _AddressList(self.options['host'], self.options['port'],
                                          self.options['backup_server_node'], self._logger)
@@ -326,16 +330,17 @@
 
         self._logger.info('Connecting as user "{}" to database "{}" on host "{}" with port {}'.format(
                      self.options['user'], self.options['database'],
                      self.options['host'], self.options['port']))
         self.startup_connection()
 
         # Complex types metadata is returned since protocol version 3.12
-        self.complex_types_enabled = self.parameters['protocol_version'] >= (3 << 16 | 12) and \
+        self.complex_types_enabled = self.parameters.get('protocol_version', 0) >= (3 << 16 | 12) and \
                                      self.parameters.get('request_complex_types', 'off') == 'on'
+
         self._logger.info('Connection is ready')
 
     #############################################
     # supporting `with` statements
     #############################################
     def __enter__(self):
         # type: () -> Self
@@ -819,16 +824,19 @@
         database = self.options['database']
         session_label = self.options['session_label']
         os_user_name = DEFAULT_USER if DEFAULT_USER else ''
         password = self.options['password']
         autocommit = self.options['autocommit']
         binary_transfer = self.options['binary_transfer']
         request_complex_types = self.options['request_complex_types']
+        oauth_access_token = self.options['oauth_access_token']
+        workload = self.options['workload']
 
-        self.write(messages.Startup(user, database, session_label, os_user_name, autocommit, binary_transfer, request_complex_types))
+        self.write(messages.Startup(user, database, session_label, os_user_name, autocommit, binary_transfer, 
+                                    request_complex_types, oauth_access_token, workload))
 
         while True:
             message = self.read_message()
 
             if isinstance(message, messages.Authentication):
                 if message.code == messages.Authentication.OK:
                     self._logger.info("User {} successfully authenticated"
@@ -839,14 +847,16 @@
                     raise errors.ConnectionError(msg)
                 elif message.code == messages.Authentication.PASSWORD_GRACE:
                     password_grace = f'The password for user {self.options["user"]} will expire soon. Please consider changing it.'
                     warnings.warn(password_grace)
                     self._logger.warning(password_grace)
                 elif message.code == messages.Authentication.GSS:
                     self.make_GSS_authentication()
+                elif message.code == messages.Authentication.OAUTH:
+                    self.write(messages.Password(oauth_access_token, message.code))
                 else:
                     self.write(messages.Password(password, message.code,
                                                  {'user': user,
                                                   'salt': getattr(message, 'salt', None),
                                                   'usersalt': getattr(message, 'usersalt', None)}))
             elif isinstance(message, messages.BackendKeyData):
                 self.backend_pid = message.pid
```

### Comparing `vertica-python-1.3.2/vertica_python/vertica/cursor.py` & `vertica-python-1.3.3/vertica_python/vertica/cursor.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,21 +299,22 @@
             if m:
                 target = as_text(m.group('target'))
 
                 variables = as_text(m.group('variables'))
                 variables = ",".join([variable.strip().strip('"') for variable in variables.split(",")])
 
                 values = as_text(m.group('values'))
-                values = ",".join([value.strip().strip('"') for value in values.split(",")])
+                values = "|".join([value.strip().strip('"') for value in values.split(",")])
                 seq_of_values = [self.format_operation_with_parameters(values, parameters, is_copy_data=True)
                                  for parameters in seq_of_parameters]
                 data = "\n".join(seq_of_values)
 
                 copy_statement = (
-                    u"COPY {0} ({1}) FROM STDIN DELIMITER ',' ENCLOSED BY '\"' "
+                    u"COPY {0} ({1}) FROM STDIN "
+                    u"ENCLOSED BY '''' "  # '/r' will have trouble if ENCLOSED BY is not set
                     u"ENFORCELENGTH ABORT ON ERROR{2}").format(target, variables,
                     " NO COMMIT" if not self.connection.autocommit else '')
 
                 self.copy(copy_statement, data)
             else:
                 raise NotImplementedError(
                     "executemany is implemented for simple INSERT statements only")
@@ -586,65 +587,76 @@
 
     def format_row_as_array(self, row_data):
         if self._disable_sqldata_converter:
             return row_data.values
         return [convert(value)
                 for convert, value in zip(self._deserializers, row_data.values)]
 
-    def object_to_string(self, py_obj, is_copy_data):
+    def object_to_string(self, py_obj, is_copy_data, is_collection=False):
         """Return the SQL representation of the object as a string"""
         if type(py_obj) in self._sql_literal_adapters and not is_copy_data:
             adapter = self._sql_literal_adapters[type(py_obj)]
             result = adapter(py_obj)
             if not isinstance(result, (str, bytes)):
                 raise TypeError("Unexpected return type of {} adapter: {}, expected a string type."
                     .format(type(py_obj), type(result)))
             return as_text(result)
 
         if isinstance(py_obj, type(None)):
-            return '' if is_copy_data else 'NULL'
+            return '' if is_copy_data and not is_collection else 'NULL'
         elif isinstance(py_obj, bool):
             return str(py_obj)
         elif isinstance(py_obj, (str, bytes)):
-            return self.format_quote(as_text(py_obj), is_copy_data)
+            return self.format_quote(as_text(py_obj), is_copy_data, is_collection)
         elif isinstance(py_obj, (int, Decimal)):
             return str(py_obj)
         elif isinstance(py_obj, float):
-            if py_obj in (float('Inf'), float('-Inf')) or isnan(py_obj):
+            if not is_copy_data and py_obj in (float('Inf'), float('-Inf')) or isnan(py_obj):
                 return f"'{str(py_obj)}'::FLOAT"
             return str(py_obj)
         elif isinstance(py_obj, tuple):  # tuple and namedtuple
             elements = [None] * len(py_obj)
             for i in range(len(py_obj)):
                 elements[i] = self.object_to_string(py_obj[i], is_copy_data)
             return "(" + ",".join(elements) + ")"
-        elif isinstance(py_obj, list) and not is_copy_data:
+        elif isinstance(py_obj, list):
             elements = [None] * len(py_obj)
-            for i in range(len(py_obj)):
-                elements[i] = self.object_to_string(py_obj[i], False)
-            # Use the ARRAY keyword to construct an array value
-            return f'ARRAY[{",".join(elements)}]'
-        elif isinstance(py_obj, set) and not is_copy_data:
+            if is_copy_data:
+                for i in range(len(py_obj)):
+                    elements[i] = self.object_to_string(py_obj[i], True, True)
+                return f'[{",".join(elements)}]'
+            else:
+                for i in range(len(py_obj)):
+                    elements[i] = self.object_to_string(py_obj[i], False)
+                # Use the ARRAY keyword to construct an array value
+                return f'ARRAY[{",".join(elements)}]'
+        elif isinstance(py_obj, set):
             elements = [None] * len(py_obj)
             i = 0
-            for o in py_obj:
-                elements[i] = self.object_to_string(o, False)
-                i += 1
-            # Use the SET keyword to construct a set value
-            return f'SET[{",".join(elements)}]'
+            if is_copy_data:
+                for o in py_obj:
+                    elements[i] = self.object_to_string(o, True, True)
+                    i += 1
+                return f'[{",".join(elements)}]'
+            else:
+                for o in py_obj:
+                    elements[i] = self.object_to_string(o, False)
+                    i += 1
+                # Use the SET keyword to construct a set value
+                return f'SET[{",".join(elements)}]'
         elif isinstance(py_obj, dict) and not is_copy_data:
             elements = [None] * len(py_obj)
             i = 0
             for k, v in py_obj.items():
                 elements[i] = self.object_to_string(v, False) + f' AS "{k}"'
                 i += 1
             # Use the ROW keyword to construct a row value
             return f'ROW({",".join(elements)})'
         elif isinstance(py_obj, (datetime.datetime, datetime.date, datetime.time, UUID)):
-            return self.format_quote(as_text(str(py_obj)), is_copy_data)
+            return self.format_quote(as_text(str(py_obj)), is_copy_data, is_collection)
         else:
             if is_copy_data:
                 return str(py_obj)
             else:
                 msg = ("Cannot convert {} type object to an SQL string. "
                        "Please register a new adapter for this type via the "
                        "Cursor.register_sql_literal_adapter() function."
@@ -682,21 +694,27 @@
                 tlist.append(value)
             operation = operation % tuple(tlist)
         else:
             raise TypeError("Argument 'parameters' must be dict or tuple/list")
 
         return operation
 
-    def format_quote(self, param, is_copy_data):
-        if is_copy_data:
+    def format_quote(self, param, is_copy_data, is_collection):
+        if is_collection: # COPY COLLECTIONENCLOSE
             s = list(param)
             for i, c in enumerate(param):
-                if c in u'()[]{}?"*+-|^$\\.&~# \t\n\r\v\f':
+                if c in '\\\n\"':
                     s[i] = "\\" + c
             return u'"{0}"'.format(u"".join(s))
+        elif is_copy_data: # COPY ENCLOSED BY
+            s = list(param)
+            for i, c in enumerate(param):
+                if c in '\\|\n\'':
+                    s[i] = "\\" + c
+            return u"'{0}'".format(u"".join(s))
         else:
             return u"'{0}'".format(param.replace(u"'", u"''"))
 
     def _execute_simple_query(self, query):
         """
         Send the query to the server using the simple query protocol.
         Return True if this query contained no SQL (e.g. the string "--comment")
```

### Comparing `vertica-python-1.3.2/vertica_python/vertica/deserializer.py` & `vertica-python-1.3.3/vertica_python/vertica/deserializer.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/log.py` & `vertica-python-1.3.3/vertica_python/vertica/log.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/__init__.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/__init__.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/authentication.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/authentication.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/backend_key_data.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/backend_key_data.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/bind_complete.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/bind_complete.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/close_complete.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/close_complete.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/command_complete.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/command_complete.py`

 * *Files 22% similar despite different names*

```diff
@@ -55,32 +55,20 @@
 
     def __init__(self, data):
         BackendMessage.__init__(self)
         data = unpack('{0}sx'.format(len(data) - 1), data)[0]
         try:
             self.command_tag = data.decode('utf-8')
         except Exception as e:
-            # (workaround for #493) something wrong in the server, hide the problem for now
-            warnings.warn("Hit a known server bug\n"
-                    f"{'='*80}\n"
-                    "We'd like to gather client-side information to help with the bug investigation.\n"
-                    "Please leave a comment under https://github.com/vertica/vertica-python/issues/493"
-                    " with the following info:\n"
-                    f"{'-'*80}\n"
-                    f"command tag length: {len(data)}\n"
-                    f"command tag content: {data}\n"
-                    f"{type(e).__name__}: {str(e)}\n"
-                    "Server version: xxx\n"
-                    "Query executed (if possible): xxx\n"
-                    "The OS of each server node (if possible): xxx\n"
-                    "The locale of each server node (if possible): xxx\n"
-                    f"{'-'*80}\n"
-                    f"We appreciate your help!\n"
-                    f"{'='*80}\n"
-                    )
+            # VER-86494
+            warnings.warn(
+                    f"\n{'-'*70}\n"
+                    "Hit a known server bug (#493). To fix it,\n"
+                    "please upgrade your server to 12.0.4-3 or higher version.\n"
+                    f"{'-'*70}\n")
             self.command_tag = 'x'
 
     def __str__(self):
         return 'CommandComplete: command_tag = "{}"'.format(self.command_tag)
 
 
 BackendMessage.register(CommandComplete)
```

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/command_description.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/command_description.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/copy_done_response.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/copy_done_response.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/copy_in_response.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/copy_in_response.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/data_row.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/data_row.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/empty_query_response.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/empty_query_response.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/end_of_batch_response.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/end_of_batch_response.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/error_response.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/error_response.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/load_balance_response.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/load_balance_response.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/load_file.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/load_file.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/no_data.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/no_data.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/notice_response.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/notice_response.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/parameter_description.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/parameter_description.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/parameter_status.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/parameter_status.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/parse_complete.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/parse_complete.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/portal_suspended.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/portal_suspended.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/ready_for_query.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/ready_for_query.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/row_description.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/row_description.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/unknown.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/unknown.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/verify_files.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/verify_files.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/write_file.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/write_file.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/__init__.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/bind.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/bind.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/cancel_request.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/cancel_request.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/close.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/close.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/copy_data.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/copy_data.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/copy_done.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/copy_done.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/copy_error.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/copy_error.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/copy_fail.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/copy_fail.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/crypt_windows.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/crypt_windows.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/describe.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/describe.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/end_of_batch_request.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/end_of_batch_request.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/execute.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/execute.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/flush.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/flush.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/load_balance_request.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/load_balance_request.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/parse.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/parse.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/password.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/password.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,14 @@
         self._options = options or {}
         if auth_method is not None:
             self._auth_method = auth_method
         else:
             self._auth_method = Authentication.CLEARTEXT_PASSWORD
 
     def encoded_password(self):
-
         if self._auth_method == Authentication.CLEARTEXT_PASSWORD:
             return self._password
         elif self._auth_method == Authentication.CRYPT_PASSWORD:
             return crypt.crypt(self._password, self._options['salt'])
         elif self._auth_method in (Authentication.MD5_PASSWORD,
                                    Authentication.HASH,
                                    Authentication.HASH_MD5,
@@ -79,16 +78,18 @@
                 m.update(self._password + key)
                 hexdigest = m.hexdigest()
                 self._password = hexdigest.encode('utf-8')
             prefix = b'md5' if useMD5 else b'sha512'
             return prefix + self._password
         elif self._auth_method == Authentication.GSS:
             return self._password
+        elif self._auth_method == Authentication.OAUTH:
+            return self._password
         else:
-            raise ValueError("unsupported authentication method: {0}".format(self._auth_method))
+            raise ValueError(f"unsupported authentication method: {self._auth_method}")
 
     def read_bytes(self):
         encoded_pw = self.encoded_password()
         # Vertica server handles GSS messages differently from other passwords
         if self._auth_method == Authentication.GSS:
             bytes_ = pack('{0}s'.format(len(encoded_pw)), encoded_pw)
         else:
```

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/query.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/query.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/ssl_request.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/ssl_request.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/startup.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/startup.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,16 @@
 from ..message import BulkFrontendMessage
 
 
 class Startup(BulkFrontendMessage):
     message_id = None
 
     def __init__(self, user, database, session_label, os_user_name, autocommit,
-                 binary_transfer, request_complex_types):
+                 binary_transfer, request_complex_types, oauth_access_token,
+                 workload):
         BulkFrontendMessage.__init__(self)
 
         try:
             os_platform = platform.platform()
         except Exception as e:
             os_platform = ''
             warnings.warn(f"Cannot get the OS info: {str(e)}")
@@ -91,16 +92,21 @@
             b'client_os_user_name': os_user_name,
             b'client_os_hostname': os_hostname,
             b'client_pid': pid,
             b'autocommit': 'on' if autocommit else 'off',
             b'binary_data_protocol': '1' if binary_transfer else '0', # Defaults to text format '0'
             b'protocol_features': '{"request_complex_types":' + request_complex_types + '}',
             b'protocol_compat': 'VER',
+            b'workload': workload,
         }
 
+        if len(oauth_access_token) > 0:
+            self.parameters[b'oauth_access_token'] = oauth_access_token # protocol version 3.11
+            self.parameters[b'auth_category'] = 'OAuth'                 # protocol version 3.12+
+
     def read_bytes(self):
         # The fixed protocol version is followed by pairs of parameter name and value strings.
         # A zero byte is required as a terminator after the last name/value pair.
         # Parameters can appear in any order.
         fixed_protocol_version = 3 << 16 | 5
         bytes_ = pack('!I', fixed_protocol_version)
```

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/sync.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/sync.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/terminate.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/terminate.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/verified_files.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/verified_files.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     message_id = b'F'
 
     def __init__(self, file_list):
         BulkFrontendMessage.__init__(self)
         self.filenames = file_list
 
     def read_bytes(self):
-        bytes_ = pack('!H', len(self.filenames))
+        bytes_ = pack('!I', len(self.filenames))
         for filename in self.filenames:
             utf_filename = filename.encode('utf-8')
             bytes_ += pack('!{0}sx'.format(len(utf_filename)), utf_filename)
             bytes_ += pack('!Q', os.path.getsize(filename))
 
         return bytes_
```

### Comparing `vertica-python-1.3.2/vertica_python/vertica/messages/message.py` & `vertica-python-1.3.3/vertica_python/vertica/messages/message.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/mixins/__init__.py` & `vertica-python-1.3.3/vertica_python/vertica/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python/vertica/mixins/notice_response_attr.py` & `vertica-python-1.3.3/vertica_python/vertica/mixins/notice_response_attr.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.2/vertica_python.egg-info/PKG-INFO` & `vertica-python-1.3.3/vertica_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertica-python
-Version: 1.3.2
+Version: 1.3.3
 Summary: Official native Python client for the Vertica database.
 Home-page: https://github.com/vertica/vertica-python
 Author: Justin Berka, Alex Kim, Siting Ren
 Author-email: justin.berka@gmail.com, alex.kim@uber.com, sitingren@hotmail.com
 License: Apache License 2.0
 Description: vertica-python is the official Vertica database client for the Python programming language. Please check the [project homepage](https://github.com/vertica/vertica-python) for the details.
 Keywords: database vertica
```

### Comparing `vertica-python-1.3.2/vertica_python.egg-info/SOURCES.txt` & `vertica-python-1.3.3/vertica_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 vertica_python/tests/integration_tests/test_connection.py
 vertica_python/tests/integration_tests/test_cursor.py
 vertica_python/tests/integration_tests/test_datatypes.py
 vertica_python/tests/integration_tests/test_dates.py
 vertica_python/tests/integration_tests/test_errors.py
 vertica_python/tests/integration_tests/test_loadbalance.py
 vertica_python/tests/integration_tests/test_timezones.py
+vertica_python/tests/integration_tests/test_tls.py
 vertica_python/tests/integration_tests/test_transfer_format.py
 vertica_python/tests/integration_tests/test_unicode.py
 vertica_python/tests/unit_tests/__init__.py
 vertica_python/tests/unit_tests/base.py
 vertica_python/tests/unit_tests/test_errors.py
 vertica_python/tests/unit_tests/test_logging.py
 vertica_python/tests/unit_tests/test_notice.py
```

