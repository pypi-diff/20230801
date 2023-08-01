# Comparing `tmp/snowflake-connector-python-nightly-2023.7.8.tar.gz` & `tmp/snowflake-connector-python-nightly-2023.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake-connector-python-nightly-2023.7.8.tar", last modified: Sat Jul  8 04:06:52 2023, max compression
+gzip compressed data, was "snowflake-connector-python-nightly-2023.8.1.tar", last modified: Tue Aug  1 04:06:35 2023, max compression
```

## Comparing `snowflake-connector-python-nightly-2023.7.8.tar` & `snowflake-connector-python-nightly-2023.8.1.tar`

### file list

```diff
@@ -1,203 +1,203 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:52.815678 snowflake-connector-python-nightly-2023.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-08 04:06:45.000000 snowflake-connector-python-nightly-2023.7.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    48322 2023-07-08 04:06:45.000000 snowflake-connector-python-nightly-2023.7.8/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-07-08 04:06:45.000000 snowflake-connector-python-nightly-2023.7.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-08 04:06:45.000000 snowflake-connector-python-nightly-2023.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-08 04:06:45.000000 snowflake-connector-python-nightly-2023.7.8/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-08 04:06:52.815678 snowflake-connector-python-nightly-2023.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-08 04:06:45.000000 snowflake-connector-python-nightly-2023.7.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-08 04:06:45.000000 snowflake-connector-python-nightly-2023.7.8/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-08 04:06:45.000000 snowflake-connector-python-nightly-2023.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-08 04:06:52.815678 snowflake-connector-python-nightly-2023.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-07-08 04:06:45.000000 snowflake-connector-python-nightly-2023.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:52.791678 snowflake-connector-python-nightly-2023.7.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:52.791678 snowflake-connector-python-nightly-2023.7.8/src/snowflake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:52.799678 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/_query_context_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/_sql_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/arrow_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/arrow_iterator.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:52.803678 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27245 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/auth/_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/auth/by_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/auth/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/auth/idtoken.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/auth/keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/auth/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/auth/okta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/auth/usrpwdmfa.py
--rw-r--r--   0 runner    (1001) docker     (123)    14011 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/auth/webbrowser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/azure_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/bind_upload_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    67296 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    30347 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/connection_diagnostic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    26078 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/converter_issue23517.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/converter_null.py
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/converter_snowsql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:52.791678 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:52.803678 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    34612 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/IColumnConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/IntConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:52.803678 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/Python/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/Python/Common.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:52.807678 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/Util/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/Util/macros.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:52.807678 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/Logging/
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/Logging/logging.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/Logging/logging.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    57032 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/dbapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/description.py
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/encryption_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/errorcode.py
--rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/file_compression_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    47199 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/file_transfer_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    16068 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/gcs_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/gzip_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/local_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40861 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    18430 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/ocsp_asn1crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)    68441 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/ocsp_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    19498 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/pandas_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25929 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/result_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/result_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    21830 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/s3_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/secret_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/sf_dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/sfbinaryformat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/sfdatetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/snow_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/sqlstate.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-08 04:06:46.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/ssd_internal_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/ssl_wrap_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)    17320 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/storage_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    18837 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/telemetry_oob.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/time_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:52.807678 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/tool/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/tool/dump_certs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/tool/dump_ocsp_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/tool/dump_ocsp_response_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/tool/probe_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/url_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/util_text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:52.807678 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:52.807678 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/_internal_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19602 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/certs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/help.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    35231 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30180 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/status_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    33450 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:52.811678 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    20300 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    39128 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/connectionpool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:52.811678 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:52.811678 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    34416 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/contrib/socks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/filepost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:52.811678 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:52.811678 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/packages/backports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)    34665 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/packages/six.py
--rw-r--r--   0 runner    (1001) docker     (123)    19786 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/poolmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/request.py
--rw-r--r--   0 runner    (1001) docker     (123)    30761 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:52.811678 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    22003 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/ssl_.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-08 04:06:48.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/wait.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-08 04:06:47.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:06:52.815678 snowflake-connector-python-nightly-2023.7.8/src/snowflake_connector_python_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-08 04:06:52.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake_connector_python_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-07-08 04:06:52.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 04:06:52.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake_connector_python_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-08 04:06:52.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake_connector_python_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 04:06:52.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake_connector_python_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-08 04:06:52.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake_connector_python_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 04:06:52.000000 snowflake-connector-python-nightly-2023.7.8/src/snowflake_connector_python_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.305805 snowflake-connector-python-nightly-2023.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-08-01 04:06:24.000000 snowflake-connector-python-nightly-2023.8.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    50115 2023-08-01 04:06:24.000000 snowflake-connector-python-nightly-2023.8.1/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-08-01 04:06:24.000000 snowflake-connector-python-nightly-2023.8.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-01 04:06:24.000000 snowflake-connector-python-nightly-2023.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-01 04:06:24.000000 snowflake-connector-python-nightly-2023.8.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-08-01 04:06:35.305805 snowflake-connector-python-nightly-2023.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-08-01 04:06:24.000000 snowflake-connector-python-nightly-2023.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-01 04:06:24.000000 snowflake-connector-python-nightly-2023.8.1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 04:06:24.000000 snowflake-connector-python-nightly-2023.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-08-01 04:06:35.305805 snowflake-connector-python-nightly-2023.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-08-01 04:06:24.000000 snowflake-connector-python-nightly-2023.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.285803 snowflake-connector-python-nightly-2023.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.281803 snowflake-connector-python-nightly-2023.8.1/src/snowflake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.293804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-08-01 04:06:25.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-08-01 04:06:25.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/_query_context_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-08-01 04:06:25.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/_sql_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-08-01 04:06:25.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/arrow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-08-01 04:06:25.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/arrow_iterator.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.293804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27245 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/by_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/idtoken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/okta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/usrpwdmfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14011 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/webbrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-08-01 04:06:25.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/azure_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-08-01 04:06:25.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/bind_upload_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23454 2023-08-01 04:06:25.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-08-01 04:06:25.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67498 2023-08-01 04:06:25.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30347 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/connection_diagnostic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26078 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/converter_issue23517.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/converter_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/converter_snowsql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.285803 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.297804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    34612 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/IColumnConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/IntConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.297804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Python/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Python/Common.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.297804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Util/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Util/macros.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.297804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/Logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/Logging/logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/Logging/logging.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    57036 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/dbapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/encryption_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/errorcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20184 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/file_compression_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47198 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/file_transfer_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16072 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/gcs_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/gzip_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/local_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42002 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18429 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/ocsp_asn1crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68581 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/ocsp_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20379 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/pandas_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25927 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/result_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/result_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21830 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/s3_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/secret_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/sf_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-01 04:06:27.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/sfbinaryformat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/sfdatetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/snow_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/sqlstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/ssd_internal_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/ssl_wrap_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17583 2023-08-01 04:06:26.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18837 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/telemetry_oob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/time_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.297804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/tool/dump_certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/tool/dump_ocsp_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/tool/dump_ocsp_response_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/tool/probe_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/url_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/util_text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.297804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.301804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/_internal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19602 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35231 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30180 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/status_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33450 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.301804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20300 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39128 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/connectionpool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.301804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.301804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34416 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/socks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/filepost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.301804 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.305805 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/packages/backports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34665 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/packages/six.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19786 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/poolmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30761 2023-08-01 04:06:29.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.305805 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22003 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/ssl_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-08-01 04:06:30.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-01 04:06:28.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:06:35.305805 snowflake-connector-python-nightly-2023.8.1/src/snowflake_connector_python_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-08-01 04:06:35.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake_connector_python_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-08-01 04:06:35.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 04:06:35.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake_connector_python_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-01 04:06:35.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake_connector_python_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 04:06:35.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake_connector_python_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-08-01 04:06:35.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake_connector_python_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 04:06:35.000000 snowflake-connector-python-nightly-2023.8.1/src/snowflake_connector_python_nightly.egg-info/top_level.txt
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/DESCRIPTION.md` & `snowflake-connector-python-nightly-2023.8.1/DESCRIPTION.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,51 @@
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Source code is also available at: https://github.com/snowflakedb/snowflake-connector-python
 
 # Release Notes
 
-- v3.0.5(TBD)
-  - Added the ability to read Snowflake's central configuration file.
+- v3.1.0(July 31,2023)
+
+  - Added a feature that lets you add connection definitions to the `connections.toml` configuration file. A connection definition refers to a collection of connection parameters, for example, if you wanted to define a connection named `prod``:
+
+    ```toml
+    [prod]
+    account = "my_account"
+    user = "my_user"
+    password = "my_password"
+    ```
+    By default, we look for the `connections.toml` file in the location specified in the `SNOWFLAKE_HOME` environment variable (default: `~/.snowflake`). If this folder does not exist, the Python connector looks for the file in the [platformdirs](https://github.com/platformdirs/platformdirs/blob/main/README.rst) location, as follows:
+
+    - On Linux: `~/.config/snowflake/`,  but follows XDG settings
+    - On Mac: `~/Library/Application Support/snowflake/`
+    - On Windows: `%USERPROFILE%\AppData\Local\snowflake\`
+
+    You can determine which file is used by running the following command:
+
+    ```
+    python -c "from snowflake.connector.constants import CONNECTIONS_FILE; print(str(CONNECTIONS_FILE))"
+    ```
   - Bumped cryptography dependency from <41.0.0,>=3.1.0 to >=3.1.0,<42.0.0.
   - Improved OCSP response caching to remove tmp cache files on Windows.
+  - Improved OCSP response caching to reduce the times of disk writing.
   - Added a parameter `server_session_keep_alive` in `SnowflakeConnection` that skips session deletion when client connection closes.
   - Tightened our pinning of platformdirs, to prevent their new releases breaking us.
   - Fixed a bug where SFPlatformDirs would incorrectly append application_name/version to its path.
   - Added retry reason for queries that are retried by the client.
   - Fixed a bug where `write_pandas` fails when user does not have the privilege to create stage or file format in the target schema, but has the right privilege for the current schema.
+  - Remove Python 3.7 support.
+  - Worked around a segfault which sometimes occurred during cache serialization in multi-threaded scenarios.
+  - Improved error handling of connection reset error.
+  - Fixed a bug about deleting the temporary files happened when running PUT command.
+  - Allowed to pass `type_mapper` to `fetch_pandas_batches()` and `fetch_pandas_all()`.
+  - Fixed a bug where pickle.dump segfaults during cache serialization in multi-threaded scenarios.
+  - Improved retry logic for okta authentication to refresh token if authentication gets throttled.
+  - Note that this release does not include the changes introduced in the previous 3.1.0a1 release. Those will be released at a later time.
 
 - v3.0.4(May 23,2023)
   - Fixed a bug in which `cursor.execute()` could modify the argument statement_params dictionary object when executing a multistatement query.
   - Added the json_result_force_utf8_decoding connection parameter to force decoding JSON content in utf-8 when the result format is JSON.
   - Fixed a bug in which we cannot call `SnowflakeCursor.nextset` before fetching the result of the first query if the cursor runs an async multistatement query.
   - Bumped vendored library urllib3 to 1.26.15
   - Bumped vendored library requests to 2.29.0
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/LICENSE.txt` & `snowflake-connector-python-nightly-2023.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/MANIFEST.in` & `snowflake-connector-python-nightly-2023.8.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/PKG-INFO` & `snowflake-connector-python-nightly-2023.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python-nightly
-Version: 2023.7.8
+Version: 2023.8.1
 Summary: Nigthly build of Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/keller00/snowflake-connector-python-nightlies/
@@ -18,27 +18,26 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: pandas
 Provides-Extra: secure-local-storage
 License-File: LICENSE.txt
 License-File: NOTICE
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/README.md` & `snowflake-connector-python-nightly-2023.8.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,42 +11,42 @@
 The Snowflake Connector for Python provides an interface for developing Python
 applications that can connect to Snowflake and perform all standard operations. It
 provides a programming alternative to developing applications in Java or C/C++
 using the Snowflake JDBC or ODBC drivers.
 
 The connector has **no** dependencies on JDBC or ODBC.
 It can be installed using ``pip`` on Linux, Mac OSX, and Windows platforms
-where Python 3.7.0 (or higher) is installed.
+where Python 3.8.0 (or higher) is installed.
 
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Feel free to file an issue or submit a PR here for general cases. For official support, contact Snowflake support at:
 https://community.snowflake.com/s/article/How-To-Submit-a-Support-Case-in-Snowflake-Lodge
 
 ## How to build
 
 ### Locally
 
-Install Python 3.7.0 or higher. Clone the Snowflake Connector for Python repository, then run the following commands
+Install Python 3.8.0 or higher. Clone the Snowflake Connector for Python repository, then run the following commands
 to create a wheel package using PEP-517 build:
 
 ```shell
 git clone git@github.com:snowflakedb/snowflake-connector-python.git
 cd snowflake-connector-python
 python -m pip install -U pip setuptools wheel build
 python -m build --wheel .
 ```
 
 Find the `snowflake_connector_python*.whl` package in the `./dist` directory.
 
 ### In Docker
 Or use our Dockerized build script `ci/build_docker.sh` and find the built wheel files in `dist/repaired_wheels`.
 
-Note: `ci/build_docker.sh` can be used to compile only certain versions, like this: `ci/build_docker.sh "3.7 3.8"`
+Note: `ci/build_docker.sh` can be used to compile only certain versions, like this: `ci/build_docker.sh "3.8 3.9"`
 
 ## Code hygiene and other utilities
 These tools are integrated into `tox` to allow us to easily set them up universally on any computer.
 
 * **fix_lint**: Runs `pre-commit` to check for a bunch of lint issues. This can be installed to run upon each
   time a commit is created locally, keep an eye out for the hint that this environment prints upon succeeding.
 * **coverage**: Runs `coverage.py` to combine generated coverage data files. Useful when multiple categories were run
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/pyproject.toml` & `snowflake-connector-python-nightly-2023.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/setup.cfg` & `snowflake-connector-python-nightly-2023.8.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 	Intended Audience :: Education
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: SQL
 	Topic :: Database
 	Topic :: Scientific/Engineering :: Information Analysis
@@ -36,15 +35,15 @@
 project_urls = 
 	Documentation=https://docs.snowflake.com/en/user-guide/python-connector.html
 	Source=https://github.com/keller00/snowflake-connector-python-nightlies/
 	Issues=https://github.com/snowflakedb/snowflake-connector-python/issues
 	Changelog=https://github.com/snowflakedb/snowflake-connector-python/blob/main/DESCRIPTION.md
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.8
 packages = find_namespace:
 install_requires = 
 	asn1crypto>0.24.0,<2.0.0
 	cffi>=1.9,<2.0.0
 	cryptography>=3.1.0,<42.0.0
 	oscrypto<2.0.0
 	pyOpenSSL>=16.2.0,<24.0.0
@@ -84,15 +83,15 @@
 development = 
 	Cython
 	coverage
 	more-itertools
 	numpy<1.26.0
 	pendulum!=2.1.1
 	pexpect
-	pytest<7.4.0
+	pytest<7.5.0
 	pytest-cov
 	pytest-rerunfailures
 	pytest-timeout
 	pytest-xdist
 	pytzdata
 pandas = 
 	pandas>=1.0.0,<2.1.0
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/setup.py` & `snowflake-connector-python-nightly-2023.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,11 +204,11 @@
                 ret.append(source)
 
             return ret
 
     cmd_class = {"build_ext": MyBuildExt}
 
 setup(
-    version="2023.07.08",
+    version="2023.08.01",
     ext_modules=extensions,
     cmdclass=cmd_class,
 )
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/__init__.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/_query_context_cache.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/_query_context_cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #
 # Copyright (c) 2012-2023 Snowflake Computing Inc. All rights reserved.
 #
 from __future__ import annotations
 
-import json
 from functools import total_ordering
 from hashlib import md5
 from logging import getLogger
 from threading import Lock
 from typing import Any, Iterable
 
 from sortedcontainers import SortedSet
@@ -147,45 +146,47 @@
 
     def _get_elements(self) -> Iterable[QueryContextElement]:
         return self._tree_set
 
     def _last(self) -> QueryContextElement:
         return self._tree_set[-1]
 
-    def serialize_to_json(self) -> str:
+    def serialize_to_dict(self) -> dict:
         with self._lock:
-            logger.debug("serialize_to_json() called")
+            logger.debug("serialize_to_dict() called")
             self.log_cache_entries()
 
             if len(self._tree_set) == 0:
-                return ""
+                return {}  # we should return an empty dict
 
             try:
                 data = {
                     "entries": [
                         {
                             "id": qce.id,
                             "timestamp": qce.read_timestamp,
                             "priority": qce.priority,
-                            "context": qce.context,
+                            "context": {"base64Data": qce.context}
+                            if qce.context is not None
+                            else {},
                         }
                         for qce in self._tree_set
                     ]
                 }
-                # Serialize the data to JSON
-                serialized_data = json.dumps(data)
+                # Because on GS side, `context` field is an object with `base64Data`  string member variable,
+                # we should serialize `context` field to an object instead of string directly to stay consistent with GS side.
 
-                logger.debug(
-                    f"serialize_to_json(): data to send to server {serialized_data}"
-                )
+                logger.debug(f"serialize_to_dict(): data to send to server {data}")
 
-                return serialized_data
+                # query context shoule be an object field of the HTTP request body JSON and on GS side. here we should only return a dict
+                # and let the outer HTTP request body to convert the entire big dict to a single JSON.
+                return data
             except Exception as e:
-                logger.debug(f"serialize_to_json(): Exception {e}")
-                return ""
+                logger.debug(f"serialize_to_dict(): Exception {e}")
+                return {}
 
     def deserialize_json_dict(self, data: dict) -> None:
         with self._lock:
             logger.debug(f"deserialize_json_dict() called: data from server: {data}")
             self.log_cache_entries()
 
             if data is None or len(data) == 0:
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/_sql_util.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/_sql_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/arrow_context.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/arrow_context.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/arrow_iterator.pyx` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/arrow_iterator.pyx`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/auth/__init__.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/auth/_auth.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/_auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/auth/by_plugin.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/by_plugin.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/auth/default.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/default.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/auth/idtoken.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/idtoken.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/auth/keypair.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/keypair.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/auth/oauth.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/auth/okta.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/okta.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 # Copyright (c) 2012-2023 Snowflake Computing Inc. All rights reserved.
 #
 
 from __future__ import annotations
 
 import json
 import logging
-from typing import TYPE_CHECKING, Any
+import time
+from functools import partial
+from typing import TYPE_CHECKING, Any, Callable
 
 from ..compat import unescape, urlencode, urlsplit
 from ..constants import (
     HTTP_HEADER_ACCEPT,
     HTTP_HEADER_CONTENT_TYPE,
     HTTP_HEADER_SERVICE_NAME,
     HTTP_HEADER_USER_AGENT,
 )
 from ..errorcode import ER_IDP_CONNECTION_ERROR, ER_INCORRECT_DESTINATION
-from ..errors import DatabaseError, Error
+from ..errors import DatabaseError, Error, RefreshTokenError
 from ..network import CONTENT_TYPE_APPLICATION_JSON, PYTHON_CONNECTOR_USER_AGENT
 from ..sqlstate import SQLSTATE_CONNECTION_WAS_NOT_ESTABLISHED
 from . import Auth
 from .by_plugin import AuthByPlugin, AuthType
 
 if TYPE_CHECKING:
     from .. import SnowflakeConnection
@@ -129,16 +131,19 @@
             conn,
             authenticator,
             service_name,
             account,
             user,
         )
         self._step2(conn, authenticator, sso_url, token_url)
-        one_time_token = self._step3(conn, headers, token_url, user, password)
-        response_html = self._step4(conn, one_time_token, sso_url)
+        response_html = self._step4(
+            conn,
+            partial(self._step3, conn, headers, token_url, user, password),
+            sso_url,
+        )
         self._step5(conn, response_html)
 
     def reauthenticate(self, **kwargs: Any) -> dict[str, bool]:
         return {"success": False}
 
     def _step1(
         self,
@@ -262,34 +267,43 @@
                 },
             )
         return one_time_token
 
     @staticmethod
     def _step4(
         conn: SnowflakeConnection,
-        one_time_token: str,
+        generate_one_time_token: Callable,
         sso_url: str,
-    ):
+    ) -> dict[Any, Any]:
         logger.debug("step 4: query IDP URL snowflake app to get SAML " "response")
-        url_parameters = {
-            "RelayState": "/some/deep/link",
-            "onetimetoken": one_time_token,
-        }
-        sso_url = sso_url + "?" + urlencode(url_parameters)
-        headers = {
-            HTTP_HEADER_ACCEPT: "*/*",
-        }
-        response_html = conn._rest.fetch(
-            "get",
-            sso_url,
-            headers,
-            timeout=conn.login_timeout,
-            socket_timeout=conn.login_timeout,
-            is_raw_text=True,
-        )
+        timeout_time = time.time() + conn.login_timeout if conn.login_timeout else None
+        response_html = {}
+        while timeout_time is None or time.time() < timeout_time:
+            try:
+                url_parameters = {
+                    "RelayState": "/some/deep/link",
+                    "onetimetoken": generate_one_time_token(),
+                }
+                sso_url = sso_url + "?" + urlencode(url_parameters)
+                headers = {
+                    HTTP_HEADER_ACCEPT: "*/*",
+                }
+                remaining_timeout = timeout_time - time.time() if timeout_time else None
+                response_html = conn._rest.fetch(
+                    "get",
+                    sso_url,
+                    headers,
+                    timeout=remaining_timeout,
+                    socket_timeout=remaining_timeout,
+                    is_raw_text=True,
+                    is_okta_authentication=True,
+                )
+                break
+            except RefreshTokenError:
+                logger.debug("step4: refresh token for re-authentication")
         return response_html
 
     def _step5(
         self,
         conn: SnowflakeConnection,
         response_html: str,
     ) -> None:
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/auth/usrpwdmfa.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/usrpwdmfa.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/auth/webbrowser.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/auth/webbrowser.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/azure_storage_client.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/azure_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/bind_upload_agent.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/bind_upload_agent.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cache.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,22 +16,25 @@
 from threading import Lock
 from typing import Generic, NoReturn, TypeVar
 
 from filelock import FileLock, Timeout
 from typing_extensions import NamedTuple, Self
 
 from . import constants
+from .constants import ENV_VAR_TEST_MODE
 
 now = datetime.datetime.now
 getmtime = os.path.getmtime
 
 T = TypeVar("T")
 
 logger = logging.getLogger(__name__)
 
+test_mode = os.getenv(ENV_VAR_TEST_MODE, "").lower() == "true"
+
 
 class CacheEntry(NamedTuple, Generic[T]):
     expiry: datetime.datetime
     entry: T
 
 
 K = TypeVar("K")
@@ -71,55 +74,56 @@
     ) -> Self:
         """Create an dictionary cache from an already existing dictionary.
 
         Note that the same references will be stored in the cache than in
         the dictionary provided.
         """
         cache = cls(**kw)
-        for k, v in _dict.items():
-            cache[k] = v
+        cache.update(_dict)
         return cache
 
     def _getitem(
         self,
         k: K,
         *,
         should_record_hits: bool = True,
     ) -> V:
         """Non-locking version of __getitem__.
 
         This should only be used by internal functions when already
         holding self._lock.
         """
+        if test_mode:
+            assert (
+                self._lock.locked()
+            ), "The mutex self._lock should be locked by this thread"
         try:
             t, v = self._cache[k]
         except KeyError:
             self._miss(k)
             raise
         if is_expired(t):
             self._expire(k)
         if should_record_hits:
             self._hit(k)
         return v
 
-    def _getitem_non_locking(
-        self,
-        k: K,
-        *,
-        should_record_hits: bool = True,
-    ) -> V:
-        # aliasing _getitem to unify the api with SFDictFileCache
-        return self._getitem(k, should_record_hits=should_record_hits)
+    # aliasing _getitem to unify the api with SFDictFileCache
+    _getitem_non_locking = _getitem
 
     def _setitem(self, k: K, v: V) -> None:
         """Non-locking version of __setitem__.
 
         This should only be used by internal functions when already
         holding self._lock.
         """
+        if test_mode:
+            assert (
+                self._lock.locked()
+            ), "The mutex self._lock should be locked by this thread"
         self._cache[k] = CacheEntry(
             expiry=now() + self._entry_lifetime,
             entry=v,
         )
         self._add_or_remove()
 
     def __getitem__(
@@ -178,14 +182,18 @@
         key: K,
     ) -> None:
         """Non-locking version of __delitem__.
 
         This should only be used by internal functions when already
         holding self._lock.
         """
+        if test_mode:
+            assert (
+                self._lock.locked()
+            ), "The mutex self._lock should be locked by this thread"
         del self._cache[key]
         self._add_or_remove()
 
     def __delitem__(
         self,
         key: K,
     ) -> None:
@@ -205,25 +213,34 @@
                 return False
 
     def _update(
         self,
         other: dict[K, V] | list[tuple[K, V]] | SFDictCache[K, V],
         update_newer_only: bool = False,
     ) -> bool:
+        """Non-locking version of update.
+
+        This should only be used by internal functions when already
+        holding self._lock and other._lock.
+        """
+        if test_mode:
+            assert (
+                self._lock.locked()
+            ), "The mutex self._lock should be locked by this thread"
         to_insert: dict[K, CacheEntry[V]]
         self._clear_expired_entries()
         if isinstance(other, (list, dict)):
             expiry = now() + self._entry_lifetime
             if isinstance(other, list):
                 g = iter(other)
             elif isinstance(other, dict):
                 g = iter(other.items())
             to_insert = {k: CacheEntry(expiry=expiry, entry=v) for k, v in g}
         elif isinstance(other, SFDictCache):
-            other._clear_expired_entries()
+            other.clear_expired_entries()
             others_items = list(other._cache.items())
             # Only accept values from another cache if their key is not in self,
             #  or if expiry is later the self known one
             to_insert = {
                 k: v
                 for k, v in others_items
                 if (
@@ -234,20 +251,23 @@
                     # other has newer expiry time we want to update newer values only
                     or self._cache[k].expiry < v.expiry
                 )
             }
         else:
             raise TypeError
         self._cache.update(to_insert)
-        self._add_or_remove()
+        if to_insert:
+            self._add_or_remove()
+        # TODO: this should really save_if_should
         return len(to_insert) > 0
 
     def update(
         self,
         other: dict[K, V] | list[tuple[K, V]] | SFDictCache[K, V],
+        update_newer_only: bool = False,
     ) -> bool:
         """Insert multiple values at the same time, if self could learn from the other.
 
         If this function is given a dictionary, or list expiration timestamps
         will be all the same a self._entry_lifetime form now. If it's
         given another SFDictCache then the timestamps will be taken
         from the other cache.
@@ -257,34 +277,42 @@
         Note that clear_expired_entries will be called on both caches. To
         prevent deadlocks this is done without acquiring other._lock. The
         intended behavior is to use this function with an unpickled/unused cache.
         If live caches are being merged then use .items() on them first and merge those
         into the other caches.
         """
         with self._lock:
-            return self._update(other)
+            return self._update(other, update_newer_only)
 
     def update_newer(
         self,
         other: dict[K, V] | list[tuple[K, V]] | SFDictCache[K, V],
     ) -> bool:
         """This function is like update, but it only updates newer elements."""
         with self._lock:
             return self._update(
                 other,
                 update_newer_only=True,
             )
 
     def _clear_expired_entries(self) -> None:
+        if test_mode:
+            assert (
+                self._lock.locked()
+            ), "The mutex self._lock should be locked by this thread"
+        cache_updated = False
         for k in list(self._cache.keys()):
             try:
                 self._getitem(k, should_record_hits=False)
             except KeyError:
-                continue
-        self._add_or_remove()
+                # the only case KeyError raised in this method
+                # is that k is expired
+                cache_updated = True
+        if cache_updated:
+            self._add_or_remove()
 
     def clear_expired_entries(self) -> None:
         """Remove expired entries from the cache."""
         with self._lock:
             self._clear_expired_entries()
 
     # Telemetry related functions, these can be plugged by child classes
@@ -339,15 +367,14 @@
         Note that while this function does not interact with lock, but it's only
         called from contexts where the lock is already held.
         """
         self.telemetry["size"] = len(self._cache)
 
 
 class SFDictFileCache(SFDictCache):
-
     # This number decides the chance of saving after writing (probability: 1/n+1)
     MAX_RAND_INT = 9
     _ATTRIBUTES_TO_PICKLE = (
         "_entry_lifetime",
         "_cache",
         "telemetry",
         "file_path",
@@ -415,15 +442,19 @@
             if os.path.exists(tmp_file_path) and os.path.isfile(tmp_file_path):
                 os.unlink(tmp_file_path)
         self.file_timeout = file_timeout
         self._file_lock_path = f"{self.file_path}.lock"
         self._file_lock = FileLock(self._file_lock_path, timeout=self.file_timeout)
         self.last_loaded: datetime.datetime | None = None
         if os.path.exists(self.file_path):
-            self._load()
+            with self._lock:
+                self._load()
+        # indicate whether the cache is modified or not, this variable is for
+        # SFDictFileCache to determine whether to dump cache to file when _save is called
+        self._cache_modified = False
 
     def _getitem_non_locking(
         self,
         k: K,
         *,
         should_record_hits: bool = True,
     ) -> V:
@@ -452,72 +483,69 @@
                 # Raises KeyError
                 self._expire(k)
         self._hit(k)
         return v
 
     def __getitem__(self, k: K) -> V:
         """Returns an element if it hasn't expired yet in a thread-safe way."""
-        self._lock.acquire()
-        # TODO: This variable could be replaced by a wrapper class that keeps track
-        #  of whether the lock is locked, but unless this function gets extended I
-        #  feel like it's an overkill. Make sure to change the bool right after
-        #  self._lock.acquire() and self._lock.release().
-        currently_holding = True
-        try:
-            if k not in self._cache:
-                self._lock.release()
-                currently_holding = False
-                loaded = self._load_if_should()
-                self._lock.acquire()
-                currently_holding = True
-                if (not loaded) or k not in self._cache:
-                    self._miss(k)
-                    raise KeyError
-            t, v = self._cache[k]
-            if is_expired(t):
-                self._lock.release()
-                currently_holding = False
-                loaded = self._load_if_should()
-                self._lock.acquire()
-                currently_holding = True
-                expire_item = True
-                if loaded:
-                    t, v = self._cache[k]
-                    expire_item = is_expired(t)
-                if expire_item:
-                    # Raises KeyError
-                    self._expire(k)
-            self._hit(k)
-            return v
-        finally:
-            if currently_holding:
-                self._lock.release()
+        with self._lock:
+            return self._getitem_non_locking(k)
 
     def _setitem(self, k: K, v: V) -> None:
         super()._setitem(k, v)
         self._save_if_should()
 
     def _load(self) -> bool:
         """Load cache from disk if possible, returns whether it was able to load."""
         try:
             with open(self.file_path, "rb") as r_file:
-                other = pickle.load(r_file)
-            self._update(
-                other,
+                other: SFDictFileCache = pickle.load(r_file)
+            # Since we want to know whether we are dirty after loading
+            #  we have to know whether the file could learn anything from self
+            #  so instead of calling self.update we call other.update and swap
+            #  the 2 underlying caches after.
+            self._lock.release()
+            cache_file_learnt = other.update(
+                self,
                 update_newer_only=True,
             )
+            self._lock.acquire()
+            self._cache, other._cache = other._cache, self._cache
+            self.telemetry["size"] = other.telemetry["size"]
+            self._cache_modified = cache_file_learnt
             self.last_loaded = now()
             return True
+        except (AssertionError, RuntimeError):
+            raise
         except Exception as e:
             logger.debug("Fail to read cache from disk due to error: %s", e)
             return False
 
-    def _save(self, load_first: bool = True) -> bool:
-        """Save cache to disk if possible, returns whether it was able to save."""
+    def load(self) -> bool:
+        """Load cache from disk if possible, returns whether it was able to load.
+
+        This is the public version of _load, it makes sure that all the
+        necessary locks are acquired.
+        """
+        with self._lock:
+            return self._load()
+
+    def _save(self, load_first: bool = True, force_flush: bool = False) -> bool:
+        """Save cache to disk if possible, returns whether it was able to save.
+
+        This function is non-locking when it comes to self._lock.
+        """
+        if test_mode:
+            assert (
+                self._lock.locked()
+            ), "The mutex self._lock should be locked by this thread"
         self._clear_expired_entries()
+        if not self._cache_modified and not force_flush:
+            # cache is not updated, so there is no need to dump cache to file, we just return
+            return False
         try:
             with self._file_lock:
                 if load_first:
                     self._load_if_should()
                 _dir, fname = os.path.split(self.file_path)
                 try:
                     tmp_file, tmp_file_path = tempfile.mkstemp(
@@ -527,20 +555,22 @@
                     # tmp_file is an opened OS level handle, which means we need to close it manually.
                     # https://docs.python.org/3/library/tempfile.html#tempfile.mkstemp
                     # ideally we shall just use the tmp_file fd to write,
                     # however, using os.write(tmp_file, bytes) causes seg fault during garbage collection when exiting
                     # python program.
                     # thus we fall back to the approach using the normal open() method to open a file and write.
                     with open(tmp_file, "wb") as w_file:
-                        pickle.dump(self, w_file)
+                        w_file.write(pickle.dumps(self))
                     # We write to a tmp file and then move it to have atomic write
                     os.replace(tmp_file_path, self.file_path)
                     self.last_loaded = datetime.datetime.fromtimestamp(
                         getmtime(self.file_path),
                     )
+                    # after update, reset self._cache_modified to indicate it's up-to-update to avoid unnecessary flush
+                    self._cache_modified = False
                     return True
                 except NameError:
                     # note: when exiting python program, garbage collection will kick in
                     # leading to `open` being garbage collected,
                     # calling `open` raises NameError, we close the tmp file fd here to release the tmp file fd
                     try:
                         os.close(tmp_file)
@@ -555,18 +585,29 @@
                 finally:
                     if os.path.exists(tmp_file_path) and os.path.isfile(tmp_file_path):
                         os.unlink(tmp_file_path)
         except Timeout:
             logger.debug(
                 f"acquiring {self._file_lock_path} timed out, skipping saving..."
             )
+        except (AssertionError, RuntimeError):
+            raise
         except Exception as e:
             logger.debug("Fail to write cache to disk due to error: %s", e)
         return False
 
+    def save(self, load_first: bool = True) -> bool:
+        """Save cache to disk if possible, returns whether it was able to save.
+
+        This is the public version of _save, it makes sure that all the
+        necessary locks are acquired.
+        """
+        with self._lock:
+            return self._save(load_first)
+
     def _save_if_should(self) -> bool:
         """Saves file to disk if necessary and returns whether it saved.
 
         Uses self._should_save to decide whether to save.
         """
         if self._should_save():
             return self._save()
@@ -601,39 +642,40 @@
                 datetime.datetime.fromtimestamp(
                     getmtime(self.file_path),
                 )
                 > self.last_loaded
             )
         return False
 
-    def __del__(self) -> None:
-        try:
-            self._save()
-        except Exception:
-            # At tear-down time builtins module might be already gone, ignore every error
-            pass
-
-    def clear_expired_entries(self) -> None:
-        super().clear_expired_entries()
-        self._save_if_should()
-
     def clear(self) -> None:
         super().clear()
         # This unlink prevents us from loading just before saving
         with self._file_lock:
             if os.path.exists(self.file_path) and os.path.isfile(self.file_path):
                 os.unlink(self.file_path)
-        self._save(load_first=False)
+        # TODO: is this necessary?
+        with self._lock:
+            self._save(load_first=False, force_flush=True)
 
     # Custom pickling implementation
 
     def __getstate__(self) -> dict:
         return {
             k: v
             for k, v in self.__dict__.items()
             if k in SFDictFileCache._ATTRIBUTES_TO_PICKLE
         }
 
     def __setstate__(self, state: dict) -> None:
         self.__dict__.update(state)
+        self._cache_modified = False
         self._lock = Lock()
         self._file_lock = FileLock(self._file_lock_path, timeout=self.file_timeout)
+
+    def _add_or_remove(self) -> None:
+        """This function gets called when an element is added, or removed.
+
+        Note that while this function does not interact with lock, but it's only
+        called from contexts where the lock is already held.
+        """
+        super()._add_or_remove()
+        self._cache_modified = True
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/compat.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/config_manager.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/config_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,52 @@
 #
 # Copyright (c) 2012-2023 Snowflake Computing Inc. All rights reserved.
 #
 
 from __future__ import annotations
 
+import itertools
 import logging
 import os
 import stat
 from collections.abc import Iterable
 from operator import methodcaller
 from pathlib import Path
-from typing import Any, Callable, TypeVar
+from typing import Any, Callable, Literal, NamedTuple, TypeVar
 from warnings import warn
 
 import tomlkit
 from tomlkit.items import Table
-from typing_extensions import Literal
 
-from snowflake.connector.constants import CONFIG_FILE
-from snowflake.connector.errors import ConfigManagerError, ConfigSourceError
+from snowflake.connector.constants import CONFIG_FILE, CONNECTIONS_FILE
+from snowflake.connector.errors import (
+    ConfigManagerError,
+    ConfigSourceError,
+    MissingConfigOptionError,
+)
 
 _T = TypeVar("_T")
 
 LOGGER = logging.getLogger(__name__)
 READABLE_BY_OTHERS = stat.S_IRGRP | stat.S_IROTH
 
 
+class ConfigSliceOptions(NamedTuple):
+    """Class that defines settings individual configuration files."""
+
+    check_permissions: bool = True
+    only_in_slice: bool = False
+
+
+class ConfigSlice(NamedTuple):
+    path: Path
+    options: ConfigSliceOptions
+    section: str
+
+
 class ConfigOption:
     """ConfigOption represents a flag/setting.
 
     The class knows how to read the value out of all sources and implements
     order of precedence between them.
 
     Attributes:
@@ -135,27 +152,34 @@
         if isinstance(loaded_var, (Table, tomlkit.TOMLDocument)):
             # If we got a TOML table we probably want it in dictionary form
             return True, loaded_var.value
         return True, loaded_var
 
     def _get_config(self) -> Any:
         """Get value from the cached config file."""
-        if self._root_manager.conf_file_cache is None and (
-            self._root_manager.file_path is not None
-            and self._root_manager.file_path.exists()
-            and self._root_manager.file_path.is_file()
+        if (
+            self._root_manager.conf_file_cache is None
+            and self._root_manager.file_path is not None
         ):
             self._root_manager.read_config()
         e = self._root_manager.conf_file_cache
         if e is None:
             raise ConfigManagerError(
                 f"Root parser '{self._root_manager.name}' is missing file_path",
             )
         for k in self._nest_path[1:]:
-            e = e[k]
+            try:
+                e = e[k]
+            except tomlkit.exceptions.NonExistentKey:
+                raise MissingConfigOptionError(  # TOOO: maybe a child Exception for missing option?
+                    f"Configuration option '{self.option_name}' is not defined anywhere, "
+                    "have you forgotten to set it in a configuration file, "
+                    "or environmental variable?"
+                )
+
         if isinstance(e, (Table, tomlkit.TOMLDocument)):
             # If we got a TOML table we probably want it in dictionary form
             return e.value
         return e
 
 
 class ConfigManager:
@@ -187,24 +211,28 @@
     """
 
     def __init__(
         self,
         *,
         name: str,
         file_path: Path | None = None,
+        _slices: list[ConfigSlice] | None = None,
     ):
         """Create a new ConfigManager.
 
         Args:
             name: Name of this ConfigManager.
             file_path: File this parser should read values from. Can be omitted
               for all child parsers.
         """
+        if _slices is None:
+            _slices = list()
         self.name = name
         self.file_path = file_path
+        self._slices = _slices
         # Objects holding subparsers and options
         self._options: dict[str, ConfigOption] = dict()
         self._sub_parsers: dict[str, ConfigManager] = dict()
         # Dictionary to cache read in config file
         self.conf_file_cache: tomlkit.TOMLDocument | None = None
         # Information necessary to be able to nest elements
         #  and add options in O(1)
@@ -222,37 +250,50 @@
         adding new options to their configuration files.
         """
         if self.file_path is None:
             raise ConfigManagerError(
                 "ConfigManager is trying to read config file, but it doesn't "
                 "have one"
             )
-        if not self.file_path.exists():
-            raise ConfigSourceError(
-                f"The config file '{self.file_path}' does not exist"
-            )
-        if (
-            # Same check as openssh does for permissions
-            #  https://github.com/openssh/openssh-portable/blob/2709809fd616a0991dc18e3a58dea10fb383c3f0/readconf.c#LL2264C1-L2264C1
-            self.file_path.stat().st_mode & READABLE_BY_OTHERS != 0
-            or (
-                # TODO: Windows doesn't have getuid, skip checking
-                hasattr(os, "getuid")
-                and self.file_path.stat().st_uid != 0
-                and self.file_path.stat().st_uid != os.getuid()
-            )
+        read_config_file = tomlkit.TOMLDocument()
+
+        # Read in all of the config slices
+        for filep, sliceoptions, section in itertools.chain(
+            ((self.file_path, ConfigSliceOptions(), None),),
+            self._slices,
         ):
-            warn(f"Bad owner or permissions on {self.file_path}")
-        LOGGER.debug(f"reading configuration file from {str(self.file_path)}")
-        try:
-            self.conf_file_cache = tomlkit.parse(self.file_path.read_text())
-        except Exception as e:
-            raise ConfigSourceError(
-                "An unknown error happened while loading " f"'{str(self.file_path)}'"
-            ) from e
+            if sliceoptions.only_in_slice:
+                del read_config_file[section]
+            if not filep.exists():
+                continue
+            if (
+                sliceoptions.check_permissions  # Skip checking if this file couldn't hold sensitive information
+                # Same check as openssh does for permissions
+                #  https://github.com/openssh/openssh-portable/blob/2709809fd616a0991dc18e3a58dea10fb383c3f0/readconf.c#LL2264C1-L2264C1
+                and filep.stat().st_mode & READABLE_BY_OTHERS != 0
+                or (
+                    # Windows doesn't have getuid, skip checking
+                    hasattr(os, "getuid")
+                    and filep.stat().st_uid != 0
+                    and filep.stat().st_uid != os.getuid()
+                )
+            ):
+                warn(f"Bad owner or permissions on {str(filep)}")
+            LOGGER.debug(f"reading configuration file from {str(filep)}")
+            try:
+                read_config_piece = tomlkit.parse(filep.read_text())
+            except Exception as e:
+                raise ConfigSourceError(
+                    "An unknown error happened while loading " f"'{str(filep)}'"
+                ) from e
+            if section is None:
+                read_config_file = read_config_piece
+            else:
+                read_config_file[section] = read_config_piece
+        self.conf_file_cache = read_config_file
 
     def add_option(
         self,
         *,
         option_cls: type[ConfigOption] = ConfigOption,
         **kwargs,
     ) -> None:
@@ -328,14 +369,23 @@
             )
         return self._sub_parsers[name]
 
 
 CONFIG_PARSER = ConfigManager(
     name="CONFIG_PARSER",
     file_path=CONFIG_FILE,
+    _slices=[
+        ConfigSlice(  # Optional connections file to read in connections from
+            CONNECTIONS_FILE,
+            ConfigSliceOptions(
+                check_permissions=True,  # connections could live here, check permissions
+            ),
+            "connections",
+        ),
+    ],
 )
 CONFIG_PARSER.add_option(
     name="connections",
     parse_str=tomlkit.parse,
 )
 
 __all__ = [
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/connection.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,15 +293,15 @@
     """
 
     OCSP_ENV_LOCK = Lock()
 
     def __init__(
         self,
         connection_name: str | None = None,
-        config_file_path: pathlib.Path | None = None,
+        connections_file_path: pathlib.Path | None = None,
         **kwargs,
     ) -> None:
         self._lock_sequence_counter = Lock()
         self.sequence_counter = 0
         self._errorhandler = Error.default_errorhandler
         self._lock_converter = Lock()
         self.messages = []
@@ -328,18 +328,21 @@
                 kwargs["application"] = os.environ[ENV_VAR_PARTNER]
             elif "streamlit" in sys.modules:
                 kwargs["application"] = "streamlit"
 
         self.converter = None
         self.query_context_cache: QueryContextCache | None = None
         self.query_context_cache_size = 5
-        if config_file_path is not None:
+        if connections_file_path is not None:
             # Change config file path and force update cache
-            CONFIG_PARSER.file_path = config_file_path
-            CONFIG_PARSER.read_config()
+            for i, s in enumerate(CONFIG_PARSER._slices):
+                if s.section == "connections":
+                    CONFIG_PARSER._slices[i] = s._replace(path=connections_file_path)
+                    CONFIG_PARSER.read_config()
+                    break
         if connection_name is not None:
             connections = CONFIG_PARSER["connections"]
             if connection_name not in connections:
                 raise Error(
                     f"Invalid connection_name '{connection_name}',"
                     f" known ones are {list(connections.keys())}"
                 )
@@ -362,15 +365,16 @@
         return self._insecure_mode
 
     @property
     def ocsp_fail_open(self) -> bool:
         return self._ocsp_fail_open
 
     def _ocsp_mode(self) -> OCSPMode:
-        """OCSP mode. INSECURE, FAIL_OPEN or FAIL_CLOSED."""
+        """OCSP mode. INSEC
+        URE, FAIL_OPEN or FAIL_CLOSED."""
         if self.insecure_mode:
             return OCSPMode.INSECURE
         elif self.ocsp_fail_open:
             return OCSPMode.FAIL_OPEN
         else:
             return OCSPMode.FAIL_CLOSED
 
@@ -1103,16 +1107,18 @@
         if binding_stage is not None:
             # binding stage for bulk array binding
             data["bindStage"] = binding_stage
         if binding_params is not None:
             # binding parameters. This is for qmarks paramstyle.
             data["bindings"] = binding_params
         if not _no_results:
-            # not an async query
-            data["queryContext"] = self.get_query_context()
+            # not an async query.
+            queryContext = self.get_query_context()
+            #  Here queryContextDTO should be a dict object field, same with `parameters` field
+            data["queryContextDTO"] = queryContext
         client = "sfsql_file_transfer" if is_file_transfer else "sfsql"
 
         if logger.getEffectiveLevel() <= logging.DEBUG:
             logger.debug(
                 "sql=[%s], sequence_id=[%s], is_file_transfer=[%s]",
                 self._format_query_for_log(data["sqlText"]),
                 data["sequenceId"],
@@ -1643,18 +1649,18 @@
             )
         return status
 
     def initialize_query_context_cache(self) -> None:
         if not self.is_query_context_cache_disabled:
             self.query_context_cache = QueryContextCache(self.query_context_cache_size)
 
-    def get_query_context(self) -> str | None:
+    def get_query_context(self) -> dict | None:
         if self.is_query_context_cache_disabled:
             return None
-        return self.query_context_cache.serialize_to_json()
+        return self.query_context_cache.serialize_to_dict()
 
     def set_query_context(self, data: dict) -> None:
         if not self.is_query_context_cache_disabled:
             self.query_context_cache.deserialize_json_dict(data)
 
     @staticmethod
     def is_still_running(status: QueryStatus) -> bool:
@@ -1681,18 +1687,15 @@
 
     def _all_async_queries_finished(self) -> bool:
         """Checks whether all async queries started by this Connection have finished executing."""
 
         if not self._async_sfqids:
             return True
 
-        if sys.version_info >= (3, 8):
-            queries = list(reversed(self._async_sfqids.keys()))
-        else:
-            queries = list(reversed(list(self._async_sfqids.keys())))
+        queries = list(reversed(self._async_sfqids.keys()))
 
         num_workers = min(self.client_prefetch_threads, len(queries))
         found_unfinished_query = False
 
         def async_query_check_helper(
             sfq_id: str,
         ) -> bool:
@@ -1700,15 +1703,14 @@
             return found_unfinished_query or self.is_still_running(
                 self.get_query_status(sfq_id)
             )
 
         with ThreadPoolExecutor(
             max_workers=num_workers, thread_name_prefix="async_query_check_"
         ) as tpe:  # We should upgrade to using cancel_futures=True once supporting 3.9+
-
             futures = (tpe.submit(async_query_check_helper, sfqid) for sfqid in queries)
             for f in as_completed(futures):
                 if f.result():
                     found_unfinished_query = True
                     break
             for f in futures:
                 f.cancel()
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/connection_diagnostic.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/connection_diagnostic.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/constants.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 
 # Snowflake's central platform dependent directories, if the folder
 # ~/.snowflake/ (customizable by the environment variable SNOWFLAKE_HOME) exists
 # we use that folder for everything. Otherwise, we fall back to platformdirs
 # defaults. Please see comments in sf_dir.py for more information.
 DIRS = _resolve_platform_dirs()
 
-# Snowflake's central configuration file. By default, platformdirs will resolve
+# Snowflake's configuration files. By default, platformdirs will resolve
 # them to these places depending on OS:
-#   * Linux: `~/.config/snowflake/config.toml` but can be updated with XDG vars
-#   * Windows: `%USERPROFILE%\AppData\Local\snowflake\config.toml`
-#   * Mac: `~/Library/Application Support/$appname/config.toml`
+#   * Linux: `~/.config/snowflake/filename` but can be updated with XDG vars
+#   * Windows: `%USERPROFILE%\AppData\Local\snowflake\filename`
+#   * Mac: `~/Library/Application Support/snowflake/filename`
+CONNECTIONS_FILE = DIRS.user_config_path / "connections.toml"
 CONFIG_FILE = DIRS.user_config_path / "config.toml"
 
 DBAPI_TYPE_STRING = 0
 DBAPI_TYPE_BINARY = 1
 DBAPI_TYPE_NUMBER = 2
 DBAPI_TYPE_TIMESTAMP = 3
 
@@ -319,7 +320,8 @@
 S3_CHUNK_SIZE = 8388608  # boto3 default
 AZURE_CHUNK_SIZE = 4 * megabyte
 
 DAY_IN_SECONDS = 60 * 60 * 24
 
 # TODO: all env variables definitions should be here
 ENV_VAR_PARTNER = "SF_PARTNER"
+ENV_VAR_TEST_MODE = "SNOWFLAKE_TEST_MODE"
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/converter.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/converter.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/converter_issue23517.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/converter_issue23517.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/converter_snowsql.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/converter_snowsql.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/Logging/logging.cpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/Logging/logging.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cpp/Logging/logging.hpp` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cpp/Logging/logging.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/cursor.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,22 +18,23 @@
 from types import TracebackType
 from typing import (
     IO,
     TYPE_CHECKING,
     Any,
     Callable,
     Iterator,
+    Literal,
     NamedTuple,
     NoReturn,
     Sequence,
     TypeVar,
     overload,
 )
 
-from typing_extensions import Literal, Self
+from typing_extensions import Self
 
 from snowflake.connector.result_batch import create_batches_from_response
 from snowflake.connector.result_set import ResultSet
 
 from . import compat
 from ._sql_util import get_file_transfer_type
 from .bind_upload_agent import BindUploadAgent, BindUploadError
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/dbapi.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/dbapi.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/description.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/description.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/encryption_util.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/encryption_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/errorcode.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/errorcode.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/errors.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -545,14 +545,25 @@
             msg=kwargs.get("msg") or "HTTP 429: Too Many Requests",
             errno=kwargs.get("errno"),
             sqlstate=kwargs.get("sqlstate"),
             sfqid=kwargs.get("sfqid"),
         )
 
 
+class RefreshTokenError(Error):
+    def __init__(self, **kwargs) -> None:
+        Error.__init__(
+            self,
+            msg=kwargs.get("msg") or "Token Refresh Required",
+            errno=kwargs.get("errno"),
+            sqlstate=kwargs.get("sqlstate"),
+            sfqid=kwargs.get("sfqid"),
+        )
+
+
 class OtherHTTPRetryableError(Error):
     """Exception for other HTTP error for retry."""
 
     def __init__(self, **kwargs) -> None:
         code = kwargs.get("code", "n/a")
         Error.__init__(
             self,
@@ -597,12 +608,19 @@
 class ConfigSourceError(Error):
     """Configuration source related errors.
 
     Examples are environmental variable and configuration file.
     """
 
 
+class MissingConfigOptionError(ConfigSourceError):
+    """When a configuration option is missing from the final, resolved configurations.
+
+    This is a special-case of ConfigSourceError.
+    """
+
+
 class ConfigManagerError(Error):
     """Configuration parser related errors.
 
     These mean that ConfigManager is misused by a developer.
     """
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/file_compression_type.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/file_compression_type.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/file_transfer_agent.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/file_transfer_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -841,15 +841,14 @@
                                 query_stage_master_key=elem["queryStageMasterKey"],
                                 query_id=elem["queryId"],
                                 smk_id=elem["smkId"],
                             )
                         )
 
     def _parse_command(self) -> None:
-
         if "data" not in self._ret:
             Error.errorhandler_wrapper(
                 self._cursor.connection,
                 self._cursor,
                 DatabaseError,
                 {
                     "msg": "Failed to parse server's response",
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/file_util.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/file_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/gcs_storage_client.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/gcs_storage_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,17 +137,17 @@
                             "KeyWrappingMetadata": {"EncryptionLibrary": "Java 5.3.0"},
                         }
                     ),
                     GCS_METADATA_MATDESC_KEY: self.encryption_metadata.matdesc,
                 }
             )
 
-        def generate_url_and_rest_args() -> tuple[
-            str, dict[str, dict[str | Any, str | None] | bytes]
-        ]:
+        def generate_url_and_rest_args() -> (
+            tuple[str, dict[str, dict[str | Any, str | None] | bytes]]
+        ):
             if not self.presigned_url:
                 upload_url = self.generate_file_url(
                     self.stage_info["location"], meta.dst_file_name.lstrip("/")
                 )
                 access_token = self.security_token
             else:
                 upload_url = self.presigned_url
@@ -166,17 +166,17 @@
         meta.gcs_file_header_encryption_metadata = json.loads(
             gcs_headers.get(GCS_METADATA_ENCRYPTIONDATAPROP, "null")
         )
 
     def download_chunk(self, chunk_id: int) -> None:
         meta = self.meta
 
-        def generate_url_and_rest_args() -> tuple[
-            str, dict[str, dict[str, str] | bool]
-        ]:
+        def generate_url_and_rest_args() -> (
+            tuple[str, dict[str, dict[str, str] | bool]]
+        ):
             gcs_headers = {}
             if not self.presigned_url:
                 download_url = self.generate_file_url(
                     self.stage_info["location"], meta.src_file_name.lstrip("/")
                 )
                 access_token = self.security_token
                 gcs_headers["Authorization"] = f"Bearer {access_token}"
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/gzip_decoder.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/gzip_decoder.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/local_storage_client.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/local_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/network.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     GatewayTimeoutError,
     InterfaceError,
     InternalServerError,
     MethodNotAllowed,
     OperationalError,
     OtherHTTPRetryableError,
     ProgrammingError,
+    RefreshTokenError,
     ServiceUnavailableError,
     TooManyRequests,
 )
 from .sqlstate import (
     SQLSTATE_CONNECTION_NOT_EXISTS,
     SQLSTATE_CONNECTION_REJECTED,
     SQLSTATE_CONNECTION_WAS_NOT_ESTABLISHED,
@@ -865,15 +866,14 @@
         headers,
         data,
         retry_ctx,
         no_retry: bool = False,
         token=NO_TOKEN,
         **kwargs,
     ):
-
         conn = self._connection
         logger.debug(
             "remaining request timeout: %s, retry cnt: %s",
             retry_ctx.timeout,
             retry_ctx.cnt + 1,
         )
 
@@ -955,14 +955,29 @@
                 sleeping_time,
             )
             time.sleep(sleeping_time)
             reason = getattr(cause, "errno", 0)
             retry_ctx.increment_retry(reason)
             if retry_ctx.timeout is not None:
                 retry_ctx.timeout -= sleeping_time
+            if "Connection aborted" in repr(e) and "ECONNRESET" in repr(e):
+                # connection is reset by the server, the underlying connection is broken and can not be reused
+                # we need a new urllib3 http(s) connection in this case.
+                # We need to first close the old one so that urllib3 pool manager can create a new connection
+                # for new requests
+                try:
+                    logger.debug(
+                        "shutting down requests session adapter due to connection aborted"
+                    )
+                    session.get_adapter(full_url).close()
+                except Exception as close_adapter_exc:
+                    logger.debug(
+                        "Ignored error caused by closing https connection failure: %s",
+                        close_adapter_exc,
+                    )
             return None  # retry
         except Exception as e:
             if not no_retry:
                 raise e
             logger.debug("Ignored error", exc_info=True)
             return {}
 
@@ -1036,14 +1051,15 @@
         data,
         token,
         catch_okta_unauthorized_error: bool = False,
         is_raw_text: bool = False,
         is_raw_binary: bool = False,
         binary_data_handler=None,
         socket_timeout=DEFAULT_SOCKET_CONNECT_TIMEOUT,
+        is_okta_authentication: bool = False,
     ):
         if socket_timeout > DEFAULT_SOCKET_CONNECT_TIMEOUT:
             # socket timeout should not be more than the default.
             # A shorter timeout may be specified for login time, but
             # for query, it should be at least 45 seconds.
             socket_timeout = DEFAULT_SOCKET_CONNECT_TIMEOUT
         logger.debug("socket timeout: %s", socket_timeout)
@@ -1086,14 +1102,18 @@
                 if is_login_request(full_url) and raw_ret.status_code == FORBIDDEN:
                     raise ForbiddenError
 
                 elif is_retryable_http_code(raw_ret.status_code):
                     error = get_http_retryable_error(raw_ret.status_code)
                     logger.debug(f"{error}. Retrying...")
                     # retryable server exceptions
+                    if is_okta_authentication:
+                        raise RefreshTokenError(
+                            msg="OKTA authentication requires token refresh."
+                        )
                     raise RetryRequest(error)
 
                 elif (
                     raw_ret.status_code == UNAUTHORIZED
                     and catch_okta_unauthorized_error
                 ):
                     # OKTA Unauthorized errors
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/ocsp_asn1crypto.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/ocsp_asn1crypto.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,14 @@
         revocation_time = revoked_info.native["revocation_time"]
         revocation_reason = revoked_info.native["revocation_reason"]
         return revocation_time, revocation_reason
 
     def check_cert_time_validity(
         self, cur_time: datetime, ocsp_cert: Certificate
     ) -> tuple[bool, str | None]:
-
         val_start = ocsp_cert["tbs_certificate"]["validity"]["not_before"].native
         val_end = ocsp_cert["tbs_certificate"]["validity"]["not_after"].native
 
         if cur_time > val_end or cur_time < val_start:
             debug_msg = (
                 "Certificate attached to OCSP response is invalid. OCSP response "
                 "current time - {} certificate not before time - {} certificate "
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/ocsp_snowflake.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/ocsp_snowflake.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,14 @@
         cert_id["issuer_name_hash"].dump(),
         cert_id["issuer_key_hash"].dump(),
         cert_id["serial_number"].dump(),
     )
 
 
 class OCSPTelemetryData:
-
     CERTIFICATE_EXTRACTION_FAILED = "CertificateExtractionFailed"
     OCSP_URL_MISSING = "OCSPURLMissing"
     OCSP_RESPONSE_UNAVAILABLE = "OCSPResponseUnavailable"
     OCSP_RESPONSE_FETCH_EXCEPTION = "OCSPResponseFetchException"
     OCSP_RESPONSE_FAILED_TO_CONNECT_CACHE_SERVER = (
         "OCSPResponseFailedToConnectCacheServer"
     )
@@ -360,15 +359,16 @@
                     )
                 logger.debug(
                     "downloaded OCSP response cache file from %s", self.CACHE_SERVER_URL
                 )
                 # len(OCSP_RESPONSE_VALIDATION_CACHE) is thread-safe, however, we do not want to
                 # block for logging purpose, thus using len(OCSP_RESPONSE_VALIDATION_CACHE._cache) here.
                 logger.debug(
-                    "# of certificates: %s", len(OCSP_RESPONSE_VALIDATION_CACHE._cache)
+                    "# of certificates: %u",
+                    len(OCSP_RESPONSE_VALIDATION_CACHE._cache),
                 )
             except RevocationCheckError as rce:
                 logger.debug(
                     "OCSP Response cache download failed. The client"
                     "will reach out to the OCSP Responder directly for"
                     "any missing OCSP responses %s\n" % rce.msg
                 )
@@ -442,15 +442,14 @@
             target_url = self.OCSP_RETRY_URL.format(parsed_url.hostname, b64data)
 
         logger.debug("OCSP Retry URL is - %s", target_url)
         return target_url
 
 
 class OCSPCache:
-
     # OCSP cache lock
     CACHE_LOCK = Lock()
 
     # OCSP cache update flag
     CACHE_UPDATED = False
 
     # Cache Expiration in seconds (120 hours). OCSP validation cache is
@@ -520,15 +519,16 @@
                 OCSPCache.OCSP_RESPONSE_CACHE_URI.replace("\\", "/")
             )
 
         logger.debug("ocsp_response_cache_uri: %s", OCSPCache.OCSP_RESPONSE_CACHE_URI)
         # len(OCSP_RESPONSE_VALIDATION_CACHE) is thread-safe, however, we do not want to
         # block for logging purpose, thus using len(OCSP_RESPONSE_VALIDATION_CACHE._cache) here.
         logger.debug(
-            "OCSP_VALIDATION_CACHE size: %s", len(OCSP_RESPONSE_VALIDATION_CACHE._cache)
+            "OCSP_VALIDATION_CACHE size: %u",
+            len(OCSP_RESPONSE_VALIDATION_CACHE._cache),
         )
 
     @staticmethod
     def read_file(ocsp):
         """Reads OCSP Response cache data from the URI, which is very likely a file."""
         try:
             parsed_url = urlsplit(OCSPCache.OCSP_RESPONSE_CACHE_URI)
@@ -583,15 +583,15 @@
         Updates OCSP Response Cache file.
         Two file shall be updated/saved:
             1. file for OCSP_RESPONSE_VALIDATION_CACHE which keeps ocsp response validation result
             2. ocsp_response_cache.json, the file in the same format as the one downloaded from snowflake cache service
         """
         if OCSPCache.CACHE_UPDATED:
             if isinstance(OCSP_RESPONSE_VALIDATION_CACHE, SFDictFileCache):
-                OCSP_RESPONSE_VALIDATION_CACHE._save()
+                OCSP_RESPONSE_VALIDATION_CACHE.save()
             OCSPCache.update_ocsp_response_cache_file(
                 ocsp, OCSPCache.OCSP_RESPONSE_CACHE_URI
             )
             OCSPCache.CACHE_UPDATED = False
 
     @staticmethod
     def update_ocsp_response_cache_file(ocsp, ocsp_response_cache_uri) -> None:
@@ -866,15 +866,14 @@
     def __init__(
         self,
         ocsp_response_cache_uri=None,
         use_ocsp_cache_server=None,
         use_post_method: bool = True,
         use_fail_open: bool = True,
     ) -> None:
-
         self.test_mode = os.getenv("SF_OCSP_TEST_MODE", None)
 
         if self.test_mode == "true":
             logger.debug("WARNING - DRIVER CONFIGURED IN TEST MODE")
 
         self._use_post_method = use_post_method
         self.OCSP_CACHE_SERVER = OCSPServer()
@@ -939,23 +938,26 @@
         )
 
     def validate(
         self,
         hostname: str | None,
         connection: Connection,
         no_exception: bool = False,
-    ) -> list[
-        tuple[
-            Exception | None,
-            Certificate,
-            Certificate,
-            CertId,
-            str | bytes,
+    ) -> (
+        list[
+            tuple[
+                Exception | None,
+                Certificate,
+                Certificate,
+                CertId,
+                str | bytes,
+            ]
         ]
-    ] | None:
+        | None
+    ):
         """Validates the certificate is not revoked using OCSP."""
         logger.debug("validating certificate: %s", hostname)
 
         do_retry = SnowflakeOCSP.get_ocsp_retry_choice()
 
         m = not SnowflakeOCSP.OCSP_WHITELIST.match(hostname)
         if m or hostname.startswith("ocspssd"):
@@ -1171,35 +1173,35 @@
             )
         except Exception as ex:
             logger.debug(
                 "Caught unknown exception - %s. Continue to validate by direct connection",
                 str(ex),
             )
 
+        to_update_cache_dict = {}
         for issuer, subject in cert_data:
             cert_id, _ = self.create_ocsp_request(issuer=issuer, subject=subject)
             cache_key = self.decode_cert_id_key(cert_id)
             ocsp_response_validation_result = OCSP_RESPONSE_VALIDATION_CACHE.get(
                 cache_key
             )
+
             if (
                 ocsp_response_validation_result is None
                 or not ocsp_response_validation_result.validated
             ):
                 r = self.validate_by_direct_connection(
                     issuer,
                     subject,
                     telemetry_data,
                     hostname,
                     do_retry=do_retry,
                     cache_key=cache_key,
                 )
-                OCSP_RESPONSE_VALIDATION_CACHE[
-                    cache_key
-                ] = OCSPResponseValidationResult(
+                to_update_cache_dict[cache_key] = OCSPResponseValidationResult(
                     *r,
                     ts=int(time.time()),
                     validated=True,
                 )
                 OCSPCache.CACHE_UPDATED = True
                 results.append(r)
             else:
@@ -1208,14 +1210,15 @@
                         ocsp_response_validation_result.exception,
                         ocsp_response_validation_result.issuer,
                         ocsp_response_validation_result.subject,
                         ocsp_response_validation_result.cert_id,
                         ocsp_response_validation_result.ocsp_response,
                     )
                 )
+        OCSP_RESPONSE_VALIDATION_CACHE.update(to_update_cache_dict)
         return results
 
     def _check_ocsp_response_cache_server(
         self,
         cert_data: list[tuple[Certificate, Certificate]],
     ) -> None:
         """Checks if OCSP response is in cache, and if not it downloads the OCSP response cache from the server.
@@ -1611,15 +1614,15 @@
                             validated=False,
                         )
                     elif found:
                         OCSPCache.delete_cache(
                             self, cert_id, cache_key=cache_key, lock_cache=False
                         )
             if new_cache_dict:
-                OCSP_RESPONSE_VALIDATION_CACHE._update(new_cache_dict)
+                OCSP_RESPONSE_VALIDATION_CACHE.update(new_cache_dict)
                 OCSPCache.CACHE_UPDATED = True
         except Exception as ex:
             logger.debug("Caught here - %s", ex)
             ermsg = "Exception raised while decoding OCSP Response Cache {}".format(
                 str(ex)
             )
             raise RevocationCheckError(
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/options.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 #
 # Copyright (c) 2012-2023 Snowflake Computing Inc. All rights reserved.
 #
 
 from __future__ import annotations
 
 import importlib
-import sys
 import warnings
+from importlib.metadata import distributions
 from logging import getLogger
 from types import ModuleType
 from typing import Union
 
 from packaging.requirements import Requirement
 
 from . import errors
 
-if sys.version_info >= (3, 8):
-    from importlib.metadata import distributions
-else:
-    from importlib_metadata import distributions
-
 logger = getLogger(__name__)
 
 """This module helps to manage optional dependencies.
 
 It implements MissingOptionalDependency as a base class. If a module is unavailable an instance of this will be
 returned. These derived classes can be seen in this file pre-defined. The point of these classes is that if someone
 tries to use pyarrow code then by importing pyarrow from this module if they did pyarrow.xxx then that would raise
@@ -65,17 +60,17 @@
     warnings.warn(
         "You have an incompatible version of '{}' installed ({}), please install a version that "
         "adheres to: '{}'".format(dep_name, installed_ver, expected_ver),
         stacklevel=2,
     )
 
 
-def _import_or_missing_pandas_option() -> tuple[
-    ModuleLikeObject, ModuleLikeObject, bool
-]:
+def _import_or_missing_pandas_option() -> (
+    tuple[ModuleLikeObject, ModuleLikeObject, bool]
+):
     """This function tries importing the following packages: pandas, pyarrow.
 
     If available it returns pandas and pyarrow packages with a flag of whether they were imported.
     It also warns users if they have an unsupported pyarrow version installed if possible.
     """
     try:
         pandas = importlib.import_module("pandas")
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/pandas_tools.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/pandas_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,24 @@
 
 import collections.abc
 import os
 import warnings
 from functools import partial
 from logging import getLogger
 from tempfile import TemporaryDirectory
-from typing import TYPE_CHECKING, Any, Callable, Iterable, Iterator, Sequence, TypeVar
-
-from typing_extensions import Literal
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Iterable,
+    Iterator,
+    Literal,
+    Sequence,
+    TypeVar,
+)
 
 from snowflake.connector import ProgrammingError
 from snowflake.connector.options import pandas
 from snowflake.connector.telemetry import TelemetryData, TelemetryField
 from snowflake.connector.util_text import random_string
 
 from .cursor import SnowflakeCursor
@@ -449,21 +456,34 @@
     conn: sqlalchemy.engine.Engine | sqlalchemy.engine.Connection,
     keys: Iterable,
     data_iter: Iterable,
     **kwargs,
 ) -> None:
     """This is a wrapper on top of write_pandas to make it compatible with to_sql method in pandas.
 
+        Notes:
+            Please note that when column names in the pandas DataFrame are consist of strictly lower case letters, column names need to
+            be enquoted, otherwise `ProgrammingError` will be raised.
+
+            This is because `snowflake-sqlalchemy` does not enquote lower case column names when creating the table, but `pd_writer` enquotes the columns by default.
+            the copy into command looks for enquoted column names.
+
+            Future improvements will be made in the snowflake-sqlalchemy library.
+
         Example usage:
             import pandas as pd
             from snowflake.connector.pandas_tools import pd_writer
 
             sf_connector_version_df = pd.DataFrame([('snowflake-connector-python', '1.0')], columns=['NAME', 'NEWEST_VERSION'])
             sf_connector_version_df.to_sql('driver_versions', engine, index=False, method=pd_writer)
 
+            # when the column names are consist of only lower case letters, enquote the column names
+            sf_connector_version_df = pd.DataFrame([('snowflake-connector-python', '1.0')], columns=['"name"', '"newest_version"'])
+            sf_connector_version_df.to_sql('driver_versions', engine, index=False, method=pd_writer)
+
     Args:
         table: Pandas package's table object.
         conn: SQLAlchemy engine object to talk to Snowflake.
         keys: Column names that we are trying to insert.
         data_iter: Iterator over the rows.
 
         More parameters can be provided to be used by 'write_pandas' (excluding 'conn', 'df', 'table_name', and 'schema'),
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/proxy.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/result_batch.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/result_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -631,15 +631,15 @@
         )
         new_chunk._data = data
 
         return new_chunk
 
     def _create_iter(
         self, iter_unit: IterUnit, connection: SnowflakeConnection | None = None
-    ) -> (Iterator[dict | Exception] | Iterator[tuple | Exception] | Iterator[Table]):
+    ) -> Iterator[dict | Exception] | Iterator[tuple | Exception] | Iterator[Table]:
         """Create an iterator for the ResultBatch. Used by get_arrow_iter."""
         if self._local:
             return self._from_data(self._data, iter_unit)
         response = self._download(connection=connection)
         logger.debug(f"started loading result batch id: {self.id}")
         with TimerContextManager() as load_metric:
             loaded_data = self._load(response, iter_unit)
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/result_set.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/result_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #
 # Copyright (c) 2012-2023 Snowflake Computing Inc. All rights reserved.
 #
 
 from __future__ import annotations
 
+import inspect
 from collections import deque
 from concurrent.futures import Future
 from concurrent.futures.thread import ThreadPoolExecutor
 from logging import getLogger
 from typing import TYPE_CHECKING, Any, Callable, Deque, Iterable, Iterator
 
 from .constants import IterUnit
@@ -35,15 +36,15 @@
 def result_set_iterator(
     first_batch_iter: Iterator[tuple],
     unconsumed_batches: Deque[Future[Iterator[tuple]]],
     unfetched_batches: Deque[ResultBatch],
     final: Callable[[], None],
     prefetch_thread_num: int,
     **kw: Any,
-) -> (Iterator[dict | Exception] | Iterator[tuple | Exception] | Iterator[Table]):
+) -> Iterator[dict | Exception] | Iterator[tuple | Exception] | Iterator[Table]:
     """Creates an iterator over some other iterators.
 
     Very similar to itertools.chain but we need some keywords to be propagated to
     ``_download`` functions later.
 
     We need this to have ResultChunks fall out of usage so that they can be garbage
     collected.
@@ -174,27 +175,31 @@
     def _fetch_pandas_batches(self, **kwargs) -> Iterator[DataFrame]:
         """Fetches Pandas dataframes in batches, where batch refers to Snowflake Chunk.
 
         Thus, the batch size (the number of rows in dataframe) is determined by
         Snowflake's back-end.
         """
         self._can_create_arrow_iter()
-        return self._create_iter(iter_unit=IterUnit.TABLE_UNIT, structure="pandas")
+        return self._create_iter(
+            iter_unit=IterUnit.TABLE_UNIT, structure="pandas", **kwargs
+        )
 
     def _fetch_pandas_all(self, **kwargs) -> DataFrame:
         """Fetches a single Pandas dataframe."""
-        dataframes = list(self._fetch_pandas_batches())
+        concat_args = list(inspect.signature(pandas.concat).parameters)
+        concat_kwargs = {k: kwargs.pop(k) for k in dict(kwargs) if k in concat_args}
+        dataframes = list(self._fetch_pandas_batches(**kwargs))
         if dataframes:
             return pandas.concat(
                 dataframes,
                 ignore_index=True,  # Don't keep in result batch indexes
-                **kwargs,
+                **concat_kwargs,
             )
         # Empty dataframe
-        return self.batches[0].to_pandas()
+        return self.batches[0].to_pandas(**kwargs)
 
     def _get_metrics(self) -> dict[str, int]:
         """Sum up all the chunks' metrics and show them together."""
         overall_metrics: dict[str, int] = {}
         for c in self.batches:
             for n, v in c._metrics.items():
                 overall_metrics[n] = overall_metrics.get(n, 0) + v
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/s3_storage_client.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/s3_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/secret_detector.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/secret_detector.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/sf_dirs.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/sf_dirs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #
 # Copyright (c) 2012-2023 Snowflake Computing Inc. All rights reserved.
 #
 
 from __future__ import annotations
 
 import os
+from typing import Literal
 
 from platformdirs import PlatformDirs, PlatformDirsABC
-from typing_extensions import Literal
 
 
 def _resolve_platform_dirs() -> PlatformDirsABC:
     """Decide on what PlatformDirs class to use.
 
     In case a folder exists (which can be customized with the environmental
     variable `SNOWFLAKE_HOME`) we use that directory as all platform
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/sfbinaryformat.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/sfbinaryformat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/sfdatetime.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/sfdatetime.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/snow_logging.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/snow_logging.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/ssd_internal_keys.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/ssd_internal_keys.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/ssl_wrap_socket.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/ssl_wrap_socket.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,22 +72,22 @@
     ca_certs_index = get_args(ssl_.ssl_wrap_socket).args.index("ca_certs")
     ca_certs_in_args = len(args) > ca_certs_index
     if not ca_certs_in_args and not kwargs.get("ca_certs"):
         kwargs["ca_certs"] = certifi.where()
 
     ret = ssl_.ssl_wrap_socket(*args, **kwargs)
 
-    from .ocsp_asn1crypto import SnowflakeOCSPAsn1Crypto as SFOCSP
-
     log.debug(
         "OCSP Mode: %s, " "OCSP response cache file name: %s",
         FEATURE_OCSP_MODE.name,
         FEATURE_OCSP_RESPONSE_CACHE_FILE_NAME,
     )
     if FEATURE_OCSP_MODE != OCSPMode.INSECURE:
+        from .ocsp_asn1crypto import SnowflakeOCSPAsn1Crypto as SFOCSP
+
         v = SFOCSP(
             ocsp_response_cache_uri=FEATURE_OCSP_RESPONSE_CACHE_FILE_NAME,
             use_fail_open=FEATURE_OCSP_MODE == OCSPMode.FAIL_OPEN,
         ).validate(server_hostname, ret.connection)
         if not v:
             raise OperationalError(
                 msg=(
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/storage_client.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/storage_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -443,13 +443,18 @@
         return
 
     def delete_client_data(self) -> None:
         """Deletes the tmp_dir and closes the source stream belonging to this client.
         This function is idempotent."""
         if os.path.exists(self.tmp_dir):
             logger.debug(f"cleaning up tmp dir: {self.tmp_dir}")
-            shutil.rmtree(self.tmp_dir)
+            try:
+                shutil.rmtree(self.tmp_dir)
+            except OSError as ex:
+                # it's ok to ignore the exception here because another thread might
+                # have cleaned up the temp directory
+                logger.debug(f"Failed to delete {self.tmp_dir}: {ex}")
         if self.meta.src_stream and not self.meta.src_stream.closed:
             self.meta.src_stream.close()
 
     def __del__(self) -> None:
         self.delete_client_data()
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/telemetry.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/telemetry.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/telemetry_oob.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/telemetry_oob.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/test_util.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/test_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/time_util.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/time_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/tool/dump_certs.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/tool/dump_certs.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/tool/dump_ocsp_response.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/tool/dump_ocsp_response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/tool/dump_ocsp_response_cache.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/tool/dump_ocsp_response_cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/tool/probe_connection.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/tool/probe_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/url_util.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/url_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/util_text.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/util_text.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/LICENSE` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/__init__.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/_internal_utils.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/adapters.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/api.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/api.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/auth.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/compat.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/cookies.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/exceptions.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/help.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/help.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/hooks.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/models.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/models.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/sessions.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/status_codes.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/structures.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/structures.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/requests/utils.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/requests/utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/LICENSE.txt` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/__init__.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/_collections.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/connection.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/connectionpool.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/contrib/appengine.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/contrib/socks.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/exceptions.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/fields.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/filepost.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/packages/six.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/poolmanager.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/request.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/response.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/__init__.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/connection.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/proxy.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/request.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/response.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/retry.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/ssl_.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/ssltransport.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/timeout.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/url.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake/connector/vendored/urllib3/util/wait.py` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake/connector/vendored/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake_connector_python_nightly.egg-info/PKG-INFO` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake_connector_python_nightly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python-nightly
-Version: 2023.7.8
+Version: 2023.8.1
 Summary: Nigthly build of Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/keller00/snowflake-connector-python-nightlies/
@@ -18,27 +18,26 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: pandas
 Provides-Extra: secure-local-storage
 License-File: LICENSE.txt
 License-File: NOTICE
```

### Comparing `snowflake-connector-python-nightly-2023.7.8/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt` & `snowflake-connector-python-nightly-2023.8.1/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

