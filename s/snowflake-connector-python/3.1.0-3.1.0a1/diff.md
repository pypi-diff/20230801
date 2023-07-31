# Comparing `tmp/snowflake-connector-python-3.1.0.tar.gz` & `tmp/snowflake-connector-python-3.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake-connector-python-3.1.0.tar", last modified: Mon Jul 31 21:18:25 2023, max compression
+gzip compressed data, was "snowflake-connector-python-3.1.0a1.tar", last modified: Tue Jul 25 20:38:49 2023, max compression
```

## Comparing `snowflake-connector-python-3.1.0.tar` & `snowflake-connector-python-3.1.0a1.tar`

### file list

```diff
@@ -1,203 +1,246 @@
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-31 21:18:25.100921 snowflake-connector-python-3.1.0/
--rw-r--r--   0 user      (1005) user      (1005)     1701 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/CONTRIBUTING.md
--rw-r--r--   0 user      (1005) user      (1005)    50115 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/DESCRIPTION.md
--rw-r--r--   0 user      (1005) user      (1005)    11365 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/LICENSE.txt
--rw-r--r--   0 user      (1005) user      (1005)      578 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/MANIFEST.in
--rw-r--r--   0 user      (1005) user      (1005)      457 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/NOTICE
--rw-r--r--   0 user      (1005) user      (1005)    52123 2023-07-31 21:18:25.100921 snowflake-connector-python-3.1.0/PKG-INFO
--rw-r--r--   0 user      (1005) user      (1005)     3045 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/README.md
--rw-r--r--   0 user      (1005) user      (1005)      308 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/SECURITY.md
--rw-r--r--   0 user      (1005) user      (1005)      696 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/pyproject.toml
--rw-r--r--   0 user      (1005) user      (1005)     3019 2023-07-31 21:18:25.100921 snowflake-connector-python-3.1.0/setup.cfg
--rw-r--r--   0 user      (1005) user      (1005)     8264 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/setup.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-31 21:18:25.064920 snowflake-connector-python-3.1.0/src/
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-31 21:18:25.060920 snowflake-connector-python-3.1.0/src/snowflake/
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-31 21:18:25.076920 snowflake-connector-python-3.1.0/src/snowflake/connector/
--rw-r--r--   0 user      (1005) user      (1005)     1693 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)    11339 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/_query_context_cache.py
--rw-r--r--   0 user      (1005) user      (1005)     1521 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/_sql_util.py
--rw-r--r--   0 user      (1005) user      (1005)     4888 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/arrow_context.py
--rw-r--r--   0 user      (1005) user      (1005)     6959 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/arrow_iterator.pyx
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-31 21:18:25.080920 snowflake-connector-python-3.1.0/src/snowflake/connector/auth/
--rw-r--r--   0 user      (1005) user      (1005)      991 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/auth/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)    27245 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/auth/_auth.py
--rw-r--r--   0 user      (1005) user      (1005)     7025 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/auth/by_plugin.py
--rw-r--r--   0 user      (1005) user      (1005)     1016 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/auth/default.py
--rw-r--r--   0 user      (1005) user      (1005)     2006 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/auth/idtoken.py
--rw-r--r--   0 user      (1005) user      (1005)     6369 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/auth/keypair.py
--rw-r--r--   0 user      (1005) user      (1005)     1470 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/auth/oauth.py
--rw-r--r--   0 user      (1005) user      (1005)    11336 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/auth/okta.py
--rw-r--r--   0 user      (1005) user      (1005)     1955 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/auth/usrpwdmfa.py
--rw-r--r--   0 user      (1005) user      (1005)    14011 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/auth/webbrowser.py
--rw-r--r--   0 user      (1005) user      (1005)     9873 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/azure_storage_client.py
--rw-r--r--   0 user      (1005) user      (1005)     2355 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/bind_upload_agent.py
--rw-r--r--   0 user      (1005) user      (1005)    23454 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cache.py
--rw-r--r--   0 user      (1005) user      (1005)     2894 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/compat.py
--rw-r--r--   0 user      (1005) user      (1005)    14891 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/config_manager.py
--rw-r--r--   0 user      (1005) user      (1005)    67498 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/connection.py
--rw-r--r--   0 user      (1005) user      (1005)    30347 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/connection_diagnostic.py
--rw-r--r--   0 user      (1005) user      (1005)     9716 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/constants.py
--rw-r--r--   0 user      (1005) user      (1005)    26078 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/converter.py
--rw-r--r--   0 user      (1005) user      (1005)     2822 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/converter_issue23517.py
--rw-r--r--   0 user      (1005) user      (1005)      437 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/converter_null.py
--rw-r--r--   0 user      (1005) user      (1005)     7633 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/converter_snowsql.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-31 21:18:25.060920 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-31 21:18:25.084921 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/
--rw-r--r--   0 user      (1005) user      (1005)      651 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)      555 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)      565 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)      512 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)    14375 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp
--rw-r--r--   0 user      (1005) user      (1005)     2308 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp
--rw-r--r--   0 user      (1005) user      (1005)      443 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.cpp
--rw-r--r--   0 user      (1005) user      (1005)     1793 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp
--rw-r--r--   0 user      (1005) user      (1005)    34612 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp
--rw-r--r--   0 user      (1005) user      (1005)     5606 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp
--rw-r--r--   0 user      (1005) user      (1005)     1601 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)     1036 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)     1625 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)     2769 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)     1032 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)      800 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)      472 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/IColumnConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)      240 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/IntConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)     1687 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-31 21:18:25.084921 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/Python/
--rw-r--r--   0 user      (1005) user      (1005)      218 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/Python/Common.cpp
--rw-r--r--   0 user      (1005) user      (1005)     2335 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp
--rw-r--r--   0 user      (1005) user      (1005)     1457 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp
--rw-r--r--   0 user      (1005) user      (1005)      939 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp
--rw-r--r--   0 user      (1005) user      (1005)     1287 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp
--rw-r--r--   0 user      (1005) user      (1005)      884 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp
--rw-r--r--   0 user      (1005) user      (1005)      649 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)      555 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)      241 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)     1838 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp
--rw-r--r--   0 user      (1005) user      (1005)     9470 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp
--rw-r--r--   0 user      (1005) user      (1005)     4063 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-31 21:18:25.084921 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/Util/
--rw-r--r--   0 user      (1005) user      (1005)      470 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/Util/macros.hpp
--rw-r--r--   0 user      (1005) user      (1005)     2013 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp
--rw-r--r--   0 user      (1005) user      (1005)     2269 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-31 21:18:25.084921 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/Logging/
--rw-r--r--   0 user      (1005) user      (1005)     3008 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/Logging/logging.cpp
--rw-r--r--   0 user      (1005) user      (1005)     1280 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/Logging/logging.hpp
--rw-r--r--   0 user      (1005) user      (1005)    57036 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/cursor.py
--rw-r--r--   0 user      (1005) user      (1005)     1268 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/dbapi.py
--rw-r--r--   0 user      (1005) user      (1005)      615 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/description.py
--rw-r--r--   0 user      (1005) user      (1005)     9376 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/encryption_util.py
--rw-r--r--   0 user      (1005) user      (1005)     2646 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/errorcode.py
--rw-r--r--   0 user      (1005) user      (1005)    20184 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/errors.py
--rw-r--r--   0 user      (1005) user      (1005)      184 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/feature.py
--rw-r--r--   0 user      (1005) user      (1005)     3246 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/file_compression_type.py
--rw-r--r--   0 user      (1005) user      (1005)    47198 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/file_transfer_agent.py
--rw-r--r--   0 user      (1005) user      (1005)     5427 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/file_util.py
--rw-r--r--   0 user      (1005) user      (1005)    16072 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/gcs_storage_client.py
--rw-r--r--   0 user      (1005) user      (1005)     2802 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/gzip_decoder.py
--rw-r--r--   0 user      (1005) user      (1005)     2919 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/local_storage_client.py
--rw-r--r--   0 user      (1005) user      (1005)    42002 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/network.py
--rw-r--r--   0 user      (1005) user      (1005)    18429 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/ocsp_asn1crypto.py
--rw-r--r--   0 user      (1005) user      (1005)    68581 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/ocsp_snowflake.py
--rw-r--r--   0 user      (1005) user      (1005)     4573 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/options.py
--rw-r--r--   0 user      (1005) user      (1005)    20379 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/pandas_tools.py
--rw-r--r--   0 user      (1005) user      (1005)     1582 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/proxy.py
--rw-r--r--   0 user      (1005) user      (1005)        0 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/py.typed
--rw-r--r--   0 user      (1005) user      (1005)    25927 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/result_batch.py
--rw-r--r--   0 user      (1005) user      (1005)     9022 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/result_set.py
--rw-r--r--   0 user      (1005) user      (1005)    21830 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/s3_storage_client.py
--rw-r--r--   0 user      (1005) user      (1005)     5343 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/secret_detector.py
--rw-r--r--   0 user      (1005) user      (1005)     4055 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/sf_dirs.py
--rw-r--r--   0 user      (1005) user      (1005)     1120 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/sfbinaryformat.py
--rw-r--r--   0 user      (1005) user      (1005)    12449 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/sfdatetime.py
--rw-r--r--   0 user      (1005) user      (1005)     4313 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/snow_logging.py
--rw-r--r--   0 user      (1005) user      (1005)      432 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/sqlstate.py
--rw-r--r--   0 user      (1005) user      (1005)      813 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/ssd_internal_keys.py
--rw-r--r--   0 user      (1005) user      (1005)     4563 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/ssl_wrap_socket.py
--rw-r--r--   0 user      (1005) user      (1005)    17583 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/storage_client.py
--rw-r--r--   0 user      (1005) user      (1005)     8861 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/telemetry.py
--rw-r--r--   0 user      (1005) user      (1005)    18837 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/telemetry_oob.py
--rw-r--r--   0 user      (1005) user      (1005)      982 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/test_util.py
--rw-r--r--   0 user      (1005) user      (1005)     2795 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/time_util.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-31 21:18:25.088920 snowflake-connector-python-3.1.0/src/snowflake/connector/tool/
--rw-r--r--   0 user      (1005) user      (1005)       76 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/tool/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)     1485 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/tool/dump_certs.py
--rw-r--r--   0 user      (1005) user      (1005)     4575 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/tool/dump_ocsp_response.py
--rw-r--r--   0 user      (1005) user      (1005)     6601 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/tool/dump_ocsp_response_cache.py
--rw-r--r--   0 user      (1005) user      (1005)     2119 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/tool/probe_connection.py
--rw-r--r--   0 user      (1005) user      (1005)     1021 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/url_util.py
--rw-r--r--   0 user      (1005) user      (1005)    10405 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/util_text.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-31 21:18:25.088920 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/
--rw-r--r--   0 user      (1005) user      (1005)       76 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/__init__.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-31 21:18:25.092921 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/
--rw-r--r--   0 user      (1005) user      (1005)    10142 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/LICENSE
--rw-r--r--   0 user      (1005) user      (1005)     4751 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)      435 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/__version__.py
--rw-r--r--   0 user      (1005) user      (1005)     1495 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/_internal_utils.py
--rw-r--r--   0 user      (1005) user      (1005)    19602 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/adapters.py
--rw-r--r--   0 user      (1005) user      (1005)     6449 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/api.py
--rw-r--r--   0 user      (1005) user      (1005)    10187 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/auth.py
--rw-r--r--   0 user      (1005) user      (1005)      429 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/certs.py
--rw-r--r--   0 user      (1005) user      (1005)     1451 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/compat.py
--rw-r--r--   0 user      (1005) user      (1005)    18560 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/cookies.py
--rw-r--r--   0 user      (1005) user      (1005)     3813 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/exceptions.py
--rw-r--r--   0 user      (1005) user      (1005)     3885 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/help.py
--rw-r--r--   0 user      (1005) user      (1005)      733 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/hooks.py
--rw-r--r--   0 user      (1005) user      (1005)    35231 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/models.py
--rw-r--r--   0 user      (1005) user      (1005)    30180 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/sessions.py
--rw-r--r--   0 user      (1005) user      (1005)     4235 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/status_codes.py
--rw-r--r--   0 user      (1005) user      (1005)     2912 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/structures.py
--rw-r--r--   0 user      (1005) user      (1005)    33450 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/utils.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-31 21:18:25.092921 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/
--rw-r--r--   0 user      (1005) user      (1005)     1115 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/LICENSE.txt
--rw-r--r--   0 user      (1005) user      (1005)     3333 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)    10811 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/_collections.py
--rw-r--r--   0 user      (1005) user      (1005)       64 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/_version.py
--rw-r--r--   0 user      (1005) user      (1005)    20300 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/connection.py
--rw-r--r--   0 user      (1005) user      (1005)    39128 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/connectionpool.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-31 21:18:25.096921 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/contrib/
--rw-r--r--   0 user      (1005) user      (1005)        0 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)      957 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-31 21:18:25.096921 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
--rw-r--r--   0 user      (1005) user      (1005)        0 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)    17632 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 user      (1005) user      (1005)    13922 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 user      (1005) user      (1005)    11012 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
--rw-r--r--   0 user      (1005) user      (1005)     4528 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 user      (1005) user      (1005)    17055 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 user      (1005) user      (1005)    34416 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
--rw-r--r--   0 user      (1005) user      (1005)     7097 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/contrib/socks.py
--rw-r--r--   0 user      (1005) user      (1005)     8217 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/exceptions.py
--rw-r--r--   0 user      (1005) user      (1005)     8579 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/fields.py
--rw-r--r--   0 user      (1005) user      (1005)     2440 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/filepost.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-31 21:18:25.096921 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/packages/
--rw-r--r--   0 user      (1005) user      (1005)        0 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/packages/__init__.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-31 21:18:25.096921 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/packages/backports/
--rw-r--r--   0 user      (1005) user      (1005)        0 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)     1417 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
--rw-r--r--   0 user      (1005) user      (1005)    34665 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/packages/six.py
--rw-r--r--   0 user      (1005) user      (1005)    19786 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/poolmanager.py
--rw-r--r--   0 user      (1005) user      (1005)     5985 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/request.py
--rw-r--r--   0 user      (1005) user      (1005)    30761 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/response.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-31 21:18:25.100921 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/
--rw-r--r--   0 user      (1005) user      (1005)     1155 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/__init__.py
--rw-r--r--   0 user      (1005) user      (1005)     4901 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/connection.py
--rw-r--r--   0 user      (1005) user      (1005)     1605 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/proxy.py
--rw-r--r--   0 user      (1005) user      (1005)      498 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/queue.py
--rw-r--r--   0 user      (1005) user      (1005)     4225 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/request.py
--rw-r--r--   0 user      (1005) user      (1005)     3510 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/response.py
--rw-r--r--   0 user      (1005) user      (1005)    22003 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/retry.py
--rw-r--r--   0 user      (1005) user      (1005)    17165 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/ssl_.py
--rw-r--r--   0 user      (1005) user      (1005)     5758 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0 user      (1005) user      (1005)     6895 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
--rw-r--r--   0 user      (1005) user      (1005)    10168 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/timeout.py
--rw-r--r--   0 user      (1005) user      (1005)    14279 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/url.py
--rw-r--r--   0 user      (1005) user      (1005)     5403 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/wait.py
--rw-r--r--   0 user      (1005) user      (1005)      107 2023-07-31 21:13:06.000000 snowflake-connector-python-3.1.0/src/snowflake/connector/version.py
-drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-31 21:18:25.100921 snowflake-connector-python-3.1.0/src/snowflake_connector_python.egg-info/
--rw-r--r--   0 user      (1005) user      (1005)    52123 2023-07-31 21:18:25.000000 snowflake-connector-python-3.1.0/src/snowflake_connector_python.egg-info/PKG-INFO
--rw-r--r--   0 user      (1005) user      (1005)     8899 2023-07-31 21:18:25.000000 snowflake-connector-python-3.1.0/src/snowflake_connector_python.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1005) user      (1005)        1 2023-07-31 21:18:25.000000 snowflake-connector-python-3.1.0/src/snowflake_connector_python.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1005) user      (1005)      322 2023-07-31 21:18:25.000000 snowflake-connector-python-3.1.0/src/snowflake_connector_python.egg-info/entry_points.txt
--rw-r--r--   0 user      (1005) user      (1005)        1 2023-07-31 21:13:57.000000 snowflake-connector-python-3.1.0/src/snowflake_connector_python.egg-info/not-zip-safe
--rw-r--r--   0 user      (1005) user      (1005)      682 2023-07-31 21:18:25.000000 snowflake-connector-python-3.1.0/src/snowflake_connector_python.egg-info/requires.txt
--rw-r--r--   0 user      (1005) user      (1005)       10 2023-07-31 21:18:25.000000 snowflake-connector-python-3.1.0/src/snowflake_connector_python.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.773818 snowflake-connector-python-3.1.0a1/
+-rw-r--r--   0 user      (1005) user      (1005)     1701 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/CONTRIBUTING.md
+-rw-r--r--   0 user      (1005) user      (1005)    50252 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/DESCRIPTION.md
+-rw-r--r--   0 user      (1005) user      (1005)    11365 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/LICENSE.txt
+-rw-r--r--   0 user      (1005) user      (1005)      701 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/MANIFEST.in
+-rw-r--r--   0 user      (1005) user      (1005)      457 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/NOTICE
+-rw-r--r--   0 user      (1005) user      (1005)    52250 2023-07-25 20:38:49.773818 snowflake-connector-python-3.1.0a1/PKG-INFO
+-rw-r--r--   0 user      (1005) user      (1005)     3045 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/README.md
+-rw-r--r--   0 user      (1005) user      (1005)      308 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/SECURITY.md
+-rw-r--r--   0 user      (1005) user      (1005)      593 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/pyproject.toml
+-rw-r--r--   0 user      (1005) user      (1005)     2991 2023-07-25 20:38:49.773818 snowflake-connector-python-3.1.0a1/setup.cfg
+-rw-r--r--   0 user      (1005) user      (1005)     6362 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/setup.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.729817 snowflake-connector-python-3.1.0a1/src/
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.725817 snowflake-connector-python-3.1.0a1/src/snowflake/
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.741817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/
+-rw-r--r--   0 user      (1005) user      (1005)     1693 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)    11339 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/_query_context_cache.py
+-rw-r--r--   0 user      (1005) user      (1005)     1521 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/_sql_util.py
+-rw-r--r--   0 user      (1005) user      (1005)     5266 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/arrow_context.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.741817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/
+-rw-r--r--   0 user      (1005) user      (1005)      991 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)    27245 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/_auth.py
+-rw-r--r--   0 user      (1005) user      (1005)     7025 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/by_plugin.py
+-rw-r--r--   0 user      (1005) user      (1005)     1016 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/default.py
+-rw-r--r--   0 user      (1005) user      (1005)     2006 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/idtoken.py
+-rw-r--r--   0 user      (1005) user      (1005)     6369 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/keypair.py
+-rw-r--r--   0 user      (1005) user      (1005)     1470 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/oauth.py
+-rw-r--r--   0 user      (1005) user      (1005)    10609 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/okta.py
+-rw-r--r--   0 user      (1005) user      (1005)     1955 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/usrpwdmfa.py
+-rw-r--r--   0 user      (1005) user      (1005)    14011 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/webbrowser.py
+-rw-r--r--   0 user      (1005) user      (1005)     9873 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/azure_storage_client.py
+-rw-r--r--   0 user      (1005) user      (1005)     2355 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/bind_upload_agent.py
+-rw-r--r--   0 user      (1005) user      (1005)    23657 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cache.py
+-rw-r--r--   0 user      (1005) user      (1005)     2894 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/compat.py
+-rw-r--r--   0 user      (1005) user      (1005)    13188 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/config_manager.py
+-rw-r--r--   0 user      (1005) user      (1005)    67794 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/connection.py
+-rw-r--r--   0 user      (1005) user      (1005)    30347 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/connection_diagnostic.py
+-rw-r--r--   0 user      (1005) user      (1005)     9670 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/constants.py
+-rw-r--r--   0 user      (1005) user      (1005)    26078 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/converter.py
+-rw-r--r--   0 user      (1005) user      (1005)     2822 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/converter_issue23517.py
+-rw-r--r--   0 user      (1005) user      (1005)      437 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/converter_null.py
+-rw-r--r--   0 user      (1005) user      (1005)     7633 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/converter_snowsql.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.725817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.753817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/
+-rw-r--r--   0 user      (1005) user      (1005)      630 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      544 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)      496 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      500 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)    16954 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     2233 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     2531 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     3735 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp
+-rw-r--r--   0 user      (1005) user      (1005)    36800 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     4258 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     1521 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      991 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     3086 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     1674 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)      943 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      755 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)      472 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/IColumnConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)      750 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/IntConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     1024 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.753817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Python/
+-rw-r--r--   0 user      (1005) user      (1005)      218 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Python/Common.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     2188 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     1457 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      939 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     1287 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      884 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp
+-rw-r--r--   0 user      (1005) user      (1005)      626 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      568 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     1272 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)      705 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp
+-rw-r--r--   0 user      (1005) user      (1005)    13176 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     3886 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.753817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Util/
+-rw-r--r--   0 user      (1005) user      (1005)      470 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Util/macros.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     2013 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     2269 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp
+-rw-r--r--   0 user      (1005) user      (1005)     7293 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/arrow_iterator.pyx
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.757817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/
+-rw-r--r--   0 user      (1005) user      (1005)     6007 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_accessors.h
+-rw-r--r--   0 user      (1005) user      (1005)     3515 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_alloc.h
+-rw-r--r--   0 user      (1005) user      (1005)     1179 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_assert.h
+-rw-r--r--   0 user      (1005) user      (1005)    79675 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_builder.h
+-rw-r--r--   0 user      (1005) user      (1005)     7437 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_emitter.h
+-rw-r--r--   0 user      (1005) user      (1005)     3998 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_endian.h
+-rw-r--r--   0 user      (1005) user      (1005)      120 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_epilogue.h
+-rw-r--r--   0 user      (1005) user      (1005)     1380 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_flatbuffers.h
+-rw-r--r--   0 user      (1005) user      (1005)     4778 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_identifier.h
+-rw-r--r--   0 user      (1005) user      (1005)      575 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_iov.h
+-rw-r--r--   0 user      (1005) user      (1005)      165 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_prologue.h
+-rw-r--r--   0 user      (1005) user      (1005)     4826 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_refmap.h
+-rw-r--r--   0 user      (1005) user      (1005)     4917 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_rtconfig.h
+-rw-r--r--   0 user      (1005) user      (1005)     3091 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_types.h
+-rw-r--r--   0 user      (1005) user      (1005)    10913 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/flatcc_verifier.h
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.761818 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/
+-rw-r--r--   0 user      (1005) user      (1005)      198 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/flatcc_portable.h
+-rw-r--r--   0 user      (1005) user      (1005)     5857 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/paligned_alloc.h
+-rw-r--r--   0 user      (1005) user      (1005)     2400 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pattributes.h
+-rw-r--r--   0 user      (1005) user      (1005)     2614 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pdiagnostic.h
+-rw-r--r--   0 user      (1005) user      (1005)      600 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pdiagnostic_pop.h
+-rw-r--r--   0 user      (1005) user      (1005)     1179 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pdiagnostic_push.h
+-rw-r--r--   0 user      (1005) user      (1005)     5284 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pendian.h
+-rw-r--r--   0 user      (1005) user      (1005)     3719 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pendian_detect.h
+-rw-r--r--   0 user      (1005) user      (1005)      424 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pinline.h
+-rw-r--r--   0 user      (1005) user      (1005)     1064 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pinttypes.h
+-rw-r--r--   0 user      (1005) user      (1005)      104 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/portable.h
+-rw-r--r--   0 user      (1005) user      (1005)      677 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/portable_basic.h
+-rw-r--r--   0 user      (1005) user      (1005)     1844 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pstatic_assert.h
+-rw-r--r--   0 user      (1005) user      (1005)     4295 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pstdalign.h
+-rw-r--r--   0 user      (1005) user      (1005)    31201 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pstdint.h
+-rw-r--r--   0 user      (1005) user      (1005)     8883 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/punaligned.h
+-rw-r--r--   0 user      (1005) user      (1005)      190 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pversion.h
+-rw-r--r--   0 user      (1005) user      (1005)     1645 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc/portable/pwarnings.h
+-rw-r--r--   0 user      (1005) user      (1005)   101560 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/flatcc.c
+-rw-r--r--   0 user      (1005) user      (1005)   106278 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/nanoarrow.c
+-rw-r--r--   0 user      (1005) user      (1005)   123683 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/nanoarrow.h
+-rw-r--r--   0 user      (1005) user      (1005)    11881 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/nanoarrow.hpp
+-rw-r--r--   0 user      (1005) user      (1005)    18597 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/nanoarrow_device.c
+-rw-r--r--   0 user      (1005) user      (1005)    14163 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/nanoarrow_device.h
+-rw-r--r--   0 user      (1005) user      (1005)  1312469 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/nanoarrow_ipc.c
+-rw-r--r--   0 user      (1005) user      (1005)    17566 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/nanoarrow_ipc.h
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.761818 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/Logging/
+-rw-r--r--   0 user      (1005) user      (1005)     3008 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/Logging/logging.cpp
+-rw-r--r--   0 user      (1005) user      (1005)     1280 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/Logging/logging.hpp
+-rw-r--r--   0 user      (1005) user      (1005)    57036 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/cursor.py
+-rw-r--r--   0 user      (1005) user      (1005)     1268 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/dbapi.py
+-rw-r--r--   0 user      (1005) user      (1005)      869 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/description.py
+-rw-r--r--   0 user      (1005) user      (1005)     9376 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/encryption_util.py
+-rw-r--r--   0 user      (1005) user      (1005)     2646 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/errorcode.py
+-rw-r--r--   0 user      (1005) user      (1005)    19672 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/errors.py
+-rw-r--r--   0 user      (1005) user      (1005)      184 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/feature.py
+-rw-r--r--   0 user      (1005) user      (1005)     3246 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/file_compression_type.py
+-rw-r--r--   0 user      (1005) user      (1005)    47198 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/file_transfer_agent.py
+-rw-r--r--   0 user      (1005) user      (1005)     5427 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/file_util.py
+-rw-r--r--   0 user      (1005) user      (1005)    16072 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/gcs_storage_client.py
+-rw-r--r--   0 user      (1005) user      (1005)     2802 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/gzip_decoder.py
+-rw-r--r--   0 user      (1005) user      (1005)     2919 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/local_storage_client.py
+-rw-r--r--   0 user      (1005) user      (1005)    41733 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/network.py
+-rw-r--r--   0 user      (1005) user      (1005)    18429 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/ocsp_asn1crypto.py
+-rw-r--r--   0 user      (1005) user      (1005)    68581 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/ocsp_snowflake.py
+-rw-r--r--   0 user      (1005) user      (1005)     4573 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/options.py
+-rw-r--r--   0 user      (1005) user      (1005)    20379 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/pandas_tools.py
+-rw-r--r--   0 user      (1005) user      (1005)     1582 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/proxy.py
+-rw-r--r--   0 user      (1005) user      (1005)        0 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/py.typed
+-rw-r--r--   0 user      (1005) user      (1005)    25893 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/result_batch.py
+-rw-r--r--   0 user      (1005) user      (1005)     9022 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/result_set.py
+-rw-r--r--   0 user      (1005) user      (1005)    21830 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/s3_storage_client.py
+-rw-r--r--   0 user      (1005) user      (1005)     5343 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/secret_detector.py
+-rw-r--r--   0 user      (1005) user      (1005)     4055 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/sf_dirs.py
+-rw-r--r--   0 user      (1005) user      (1005)     1120 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/sfbinaryformat.py
+-rw-r--r--   0 user      (1005) user      (1005)    12449 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/sfdatetime.py
+-rw-r--r--   0 user      (1005) user      (1005)     4313 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/snow_logging.py
+-rw-r--r--   0 user      (1005) user      (1005)      432 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/sqlstate.py
+-rw-r--r--   0 user      (1005) user      (1005)      813 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/ssd_internal_keys.py
+-rw-r--r--   0 user      (1005) user      (1005)     4563 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/ssl_wrap_socket.py
+-rw-r--r--   0 user      (1005) user      (1005)    17583 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/storage_client.py
+-rw-r--r--   0 user      (1005) user      (1005)     8901 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/telemetry.py
+-rw-r--r--   0 user      (1005) user      (1005)    18837 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/telemetry_oob.py
+-rw-r--r--   0 user      (1005) user      (1005)      982 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/test_util.py
+-rw-r--r--   0 user      (1005) user      (1005)     2795 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/time_util.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.761818 snowflake-connector-python-3.1.0a1/src/snowflake/connector/tool/
+-rw-r--r--   0 user      (1005) user      (1005)       76 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/tool/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)     1485 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/tool/dump_certs.py
+-rw-r--r--   0 user      (1005) user      (1005)     4575 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/tool/dump_ocsp_response.py
+-rw-r--r--   0 user      (1005) user      (1005)     6601 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/tool/dump_ocsp_response_cache.py
+-rw-r--r--   0 user      (1005) user      (1005)     2119 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/tool/probe_connection.py
+-rw-r--r--   0 user      (1005) user      (1005)     1021 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/url_util.py
+-rw-r--r--   0 user      (1005) user      (1005)    10405 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/util_text.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.761818 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/
+-rw-r--r--   0 user      (1005) user      (1005)       76 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/__init__.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.765817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/
+-rw-r--r--   0 user      (1005) user      (1005)    10142 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/LICENSE
+-rw-r--r--   0 user      (1005) user      (1005)     4751 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)      435 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/__version__.py
+-rw-r--r--   0 user      (1005) user      (1005)     1495 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/_internal_utils.py
+-rw-r--r--   0 user      (1005) user      (1005)    19602 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/adapters.py
+-rw-r--r--   0 user      (1005) user      (1005)     6449 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/api.py
+-rw-r--r--   0 user      (1005) user      (1005)    10187 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/auth.py
+-rw-r--r--   0 user      (1005) user      (1005)      429 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/certs.py
+-rw-r--r--   0 user      (1005) user      (1005)     1451 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/compat.py
+-rw-r--r--   0 user      (1005) user      (1005)    18560 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/cookies.py
+-rw-r--r--   0 user      (1005) user      (1005)     3813 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/exceptions.py
+-rw-r--r--   0 user      (1005) user      (1005)     3885 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/help.py
+-rw-r--r--   0 user      (1005) user      (1005)      733 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/hooks.py
+-rw-r--r--   0 user      (1005) user      (1005)    35231 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/models.py
+-rw-r--r--   0 user      (1005) user      (1005)    30180 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/sessions.py
+-rw-r--r--   0 user      (1005) user      (1005)     4235 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/status_codes.py
+-rw-r--r--   0 user      (1005) user      (1005)     2912 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/structures.py
+-rw-r--r--   0 user      (1005) user      (1005)    33450 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/utils.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.765817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/
+-rw-r--r--   0 user      (1005) user      (1005)     1115 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/LICENSE.txt
+-rw-r--r--   0 user      (1005) user      (1005)     3333 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)    10811 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/_collections.py
+-rw-r--r--   0 user      (1005) user      (1005)       64 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/_version.py
+-rw-r--r--   0 user      (1005) user      (1005)    20300 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/connection.py
+-rw-r--r--   0 user      (1005) user      (1005)    39128 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/connectionpool.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.769817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/
+-rw-r--r--   0 user      (1005) user      (1005)        0 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)      957 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.769817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
+-rw-r--r--   0 user      (1005) user      (1005)        0 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)    17632 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 user      (1005) user      (1005)    13922 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 user      (1005) user      (1005)    11012 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
+-rw-r--r--   0 user      (1005) user      (1005)     4528 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 user      (1005) user      (1005)    17055 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 user      (1005) user      (1005)    34416 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
+-rw-r--r--   0 user      (1005) user      (1005)     7097 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/socks.py
+-rw-r--r--   0 user      (1005) user      (1005)     8217 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/exceptions.py
+-rw-r--r--   0 user      (1005) user      (1005)     8579 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/fields.py
+-rw-r--r--   0 user      (1005) user      (1005)     2440 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/filepost.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.769817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/packages/
+-rw-r--r--   0 user      (1005) user      (1005)        0 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/packages/__init__.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.769817 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/packages/backports/
+-rw-r--r--   0 user      (1005) user      (1005)        0 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)     1417 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 user      (1005) user      (1005)    34665 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/packages/six.py
+-rw-r--r--   0 user      (1005) user      (1005)    19786 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/poolmanager.py
+-rw-r--r--   0 user      (1005) user      (1005)     5985 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/request.py
+-rw-r--r--   0 user      (1005) user      (1005)    30761 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/response.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.773818 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/
+-rw-r--r--   0 user      (1005) user      (1005)     1155 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/__init__.py
+-rw-r--r--   0 user      (1005) user      (1005)     4901 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/connection.py
+-rw-r--r--   0 user      (1005) user      (1005)     1605 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/proxy.py
+-rw-r--r--   0 user      (1005) user      (1005)      498 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/queue.py
+-rw-r--r--   0 user      (1005) user      (1005)     4225 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/request.py
+-rw-r--r--   0 user      (1005) user      (1005)     3510 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/response.py
+-rw-r--r--   0 user      (1005) user      (1005)    22003 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/retry.py
+-rw-r--r--   0 user      (1005) user      (1005)    17165 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/ssl_.py
+-rw-r--r--   0 user      (1005) user      (1005)     5758 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 user      (1005) user      (1005)     6895 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
+-rw-r--r--   0 user      (1005) user      (1005)    10168 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/timeout.py
+-rw-r--r--   0 user      (1005) user      (1005)    14279 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/url.py
+-rw-r--r--   0 user      (1005) user      (1005)     5403 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/wait.py
+-rw-r--r--   0 user      (1005) user      (1005)      111 2023-07-25 20:36:06.000000 snowflake-connector-python-3.1.0a1/src/snowflake/connector/version.py
+drwxr-xr-x   0 user      (1005) user      (1005)        0 2023-07-25 20:38:49.773818 snowflake-connector-python-3.1.0a1/src/snowflake_connector_python.egg-info/
+-rw-r--r--   0 user      (1005) user      (1005)    52250 2023-07-25 20:38:49.000000 snowflake-connector-python-3.1.0a1/src/snowflake_connector_python.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1005) user      (1005)    11658 2023-07-25 20:38:49.000000 snowflake-connector-python-3.1.0a1/src/snowflake_connector_python.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1005) user      (1005)        1 2023-07-25 20:38:49.000000 snowflake-connector-python-3.1.0a1/src/snowflake_connector_python.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1005) user      (1005)      322 2023-07-25 20:38:49.000000 snowflake-connector-python-3.1.0a1/src/snowflake_connector_python.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1005) user      (1005)        1 2023-07-25 20:36:46.000000 snowflake-connector-python-3.1.0a1/src/snowflake_connector_python.egg-info/not-zip-safe
+-rw-r--r--   0 user      (1005) user      (1005)      666 2023-07-25 20:38:49.000000 snowflake-connector-python-3.1.0a1/src/snowflake_connector_python.egg-info/requires.txt
+-rw-r--r--   0 user      (1005) user      (1005)       10 2023-07-25 20:38:49.000000 snowflake-connector-python-3.1.0a1/src/snowflake_connector_python.egg-info/top_level.txt
```

### Comparing `snowflake-connector-python-3.1.0/CONTRIBUTING.md` & `snowflake-connector-python-3.1.0a1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/DESCRIPTION.md` & `snowflake-connector-python-3.1.0a1/DESCRIPTION.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,51 +4,51 @@
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Source code is also available at: https://github.com/snowflakedb/snowflake-connector-python
 
 # Release Notes
 
-- v3.1.0(July 31,2023)
-
-  - Added a feature that lets you add connection definitions to the `connections.toml` configuration file. A connection definition refers to a collection of connection parameters, for example, if you wanted to define a connection named `prod``:
-
-    ```toml
-    [prod]
-    account = "my_account"
-    user = "my_user"
-    password = "my_password"
-    ```
-    By default, we look for the `connections.toml` file in the location specified in the `SNOWFLAKE_HOME` environment variable (default: `~/.snowflake`). If this folder does not exist, the Python connector looks for the file in the [platformdirs](https://github.com/platformdirs/platformdirs/blob/main/README.rst) location, as follows:
-
-    - On Linux: `~/.config/snowflake/`,  but follows XDG settings
-    - On Mac: `~/Library/Application Support/snowflake/`
-    - On Windows: `%USERPROFILE%\AppData\Local\snowflake\`
-
-    You can determine which file is used by running the following command:
-
-    ```
-    python -c "from snowflake.connector.constants import CONNECTIONS_FILE; print(str(CONNECTIONS_FILE))"
-    ```
-  - Bumped cryptography dependency from <41.0.0,>=3.1.0 to >=3.1.0,<42.0.0.
-  - Improved OCSP response caching to remove tmp cache files on Windows.
-  - Improved OCSP response caching to reduce the times of disk writing.
-  - Added a parameter `server_session_keep_alive` in `SnowflakeConnection` that skips session deletion when client connection closes.
-  - Tightened our pinning of platformdirs, to prevent their new releases breaking us.
-  - Fixed a bug where SFPlatformDirs would incorrectly append application_name/version to its path.
-  - Added retry reason for queries that are retried by the client.
-  - Fixed a bug where `write_pandas` fails when user does not have the privilege to create stage or file format in the target schema, but has the right privilege for the current schema.
-  - Remove Python 3.7 support.
-  - Worked around a segfault which sometimes occurred during cache serialization in multi-threaded scenarios.
-  - Improved error handling of connection reset error.
-  - Fixed a bug about deleting the temporary files happened when running PUT command.
-  - Allowed to pass `type_mapper` to `fetch_pandas_batches()` and `fetch_pandas_all()`.
-  - Fixed a bug where pickle.dump segfaults during cache serialization in multi-threaded scenarios.
-  - Improved retry logic for okta authentication to refresh token if authentication gets throttled.
-  - Note that this release does not include the changes introduced in the previous 3.1.0a1 release. Those will be released at a later time.
+- v3.1.0a1(July 24, 2023)
+  - Version 3.1.0a1 is our first efforts to build snowflake-connector-python based on apache nanoarrow project, which
+reduces the package size as well as removes a hard dependency on a specific version of pyarrow.
+  - This version also includes the following features and bug fixes from the unreleased v3.0.5:
+    - Added a feature that lets you add connection definitions to the `config.toml` configuration file. A connection definition refers to a collection of connection parameters. The connection configuration name must begin with **connections**, similar to the following that defines the parameters for the `prod` connection:
+
+      ```toml
+      [connections.prod]
+      account = "my_account"
+      user = "my_user"
+      password = "my_password"
+      ```
+      By default, we look for the `config.toml` file in the location specified in the `SNOWFLAKE_HOME` environment variable (default: `~/.snowflake`). If this folder does not exist, the Python connector looks for the file in the `platformdirs` location, as follows:
+
+      - On Linux: `~/.config/snowflake/`,  but follows XDG settings
+      - On Mac: `~/Library/Application Support/snowflake/`
+      - On Windows: `%USERPROFILE%\AppData\Local\snowflake\`
+
+      You can determine which file is used by running the following command:
+
+      ```
+      python -c "from snowflake.connector.constants import CONFIG_FILE; print(str(CONFIG_FILE))"
+      ```
+    - Bumped cryptography dependency from <41.0.0,>=3.1.0 to >=3.1.0,<42.0.0.
+    - Improved OCSP response caching to remove tmp cache files on Windows.
+    - Improved OCSP response caching to reduce the times of disk writing.
+    - Added a parameter `server_session_keep_alive` in `SnowflakeConnection` that skips session deletion when client connection closes.
+    - Tightened our pinning of platformdirs, to prevent their new releases breaking us.
+    - Fixed a bug where SFPlatformDirs would incorrectly append application_name/version to its path.
+    - Added retry reason for queries that are retried by the client.
+    - Fixed a bug where `write_pandas` fails when user does not have the privilege to create stage or file format in the target schema, but has the right privilege for the current schema.
+    - Remove Python 3.7 support.
+    - Worked around a segfault which sometimes occurred during cache serialization in multi-threaded scenarios.
+    - Improved error handling of connection reset error.
+    - Fixed a bug about deleting the temporary files happened when running PUT command.
+    - Allowed to pass `type_mapper` to `fetch_pandas_batches()` and `fetch_pandas_all()`.
+    - Fixed a bug where pickle.dump segfaults during cache serialization in multi-threaded scenarios.
 
 - v3.0.4(May 23,2023)
   - Fixed a bug in which `cursor.execute()` could modify the argument statement_params dictionary object when executing a multistatement query.
   - Added the json_result_force_utf8_decoding connection parameter to force decoding JSON content in utf-8 when the result format is JSON.
   - Fixed a bug in which we cannot call `SnowflakeCursor.nextset` before fetching the result of the first query if the cursor runs an async multistatement query.
   - Bumped vendored library urllib3 to 1.26.15
   - Bumped vendored library requests to 2.29.0
```

### Comparing `snowflake-connector-python-3.1.0/LICENSE.txt` & `snowflake-connector-python-3.1.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/MANIFEST.in` & `snowflake-connector-python-3.1.0a1/MANIFEST.in`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 include LICENSE.txt
 include NOTICE
 include pyproject.toml
 recursive-include src/snowflake/connector py.typed *.py *.pyx
 recursive-include src/snowflake/connector/vendored LICENSE*
 
 recursive-include src/snowflake/connector/cpp *.cpp *.hpp
+recursive-include src/snowflake/connector/cpp *.c *.h
 exclude src/snowflake/connector/arrow_iterator.cpp
+exclude src/snowflake/connector/cpp/ArrowIterator/arrow_iterator.cpp
 
 exclude .git-blame-ignore-revs
 exclude .pre-commit-config.yaml
 exclude license_header.txt
 exclude tox.ini
 exclude mypy.ini
```

### Comparing `snowflake-connector-python-3.1.0/PKG-INFO` & `snowflake-connector-python-3.1.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python
-Version: 3.1.0
+Version: 3.1.0a1
 Summary: Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/snowflakedb/snowflake-connector-python
 Project-URL: Issues, https://github.com/snowflakedb/snowflake-connector-python/issues
 Project-URL: Changelog, https://github.com/snowflakedb/snowflake-connector-python/blob/main/DESCRIPTION.md
 Keywords: Snowflake db database cloud analytics warehouse
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
@@ -47,51 +47,51 @@
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Source code is also available at: https://github.com/snowflakedb/snowflake-connector-python
 
 # Release Notes
 
-- v3.1.0(July 31,2023)
-
-  - Added a feature that lets you add connection definitions to the `connections.toml` configuration file. A connection definition refers to a collection of connection parameters, for example, if you wanted to define a connection named `prod``:
-
-    ```toml
-    [prod]
-    account = "my_account"
-    user = "my_user"
-    password = "my_password"
-    ```
-    By default, we look for the `connections.toml` file in the location specified in the `SNOWFLAKE_HOME` environment variable (default: `~/.snowflake`). If this folder does not exist, the Python connector looks for the file in the [platformdirs](https://github.com/platformdirs/platformdirs/blob/main/README.rst) location, as follows:
-
-    - On Linux: `~/.config/snowflake/`,  but follows XDG settings
-    - On Mac: `~/Library/Application Support/snowflake/`
-    - On Windows: `%USERPROFILE%\AppData\Local\snowflake\`
-
-    You can determine which file is used by running the following command:
-
-    ```
-    python -c "from snowflake.connector.constants import CONNECTIONS_FILE; print(str(CONNECTIONS_FILE))"
-    ```
-  - Bumped cryptography dependency from <41.0.0,>=3.1.0 to >=3.1.0,<42.0.0.
-  - Improved OCSP response caching to remove tmp cache files on Windows.
-  - Improved OCSP response caching to reduce the times of disk writing.
-  - Added a parameter `server_session_keep_alive` in `SnowflakeConnection` that skips session deletion when client connection closes.
-  - Tightened our pinning of platformdirs, to prevent their new releases breaking us.
-  - Fixed a bug where SFPlatformDirs would incorrectly append application_name/version to its path.
-  - Added retry reason for queries that are retried by the client.
-  - Fixed a bug where `write_pandas` fails when user does not have the privilege to create stage or file format in the target schema, but has the right privilege for the current schema.
-  - Remove Python 3.7 support.
-  - Worked around a segfault which sometimes occurred during cache serialization in multi-threaded scenarios.
-  - Improved error handling of connection reset error.
-  - Fixed a bug about deleting the temporary files happened when running PUT command.
-  - Allowed to pass `type_mapper` to `fetch_pandas_batches()` and `fetch_pandas_all()`.
-  - Fixed a bug where pickle.dump segfaults during cache serialization in multi-threaded scenarios.
-  - Improved retry logic for okta authentication to refresh token if authentication gets throttled.
-  - Note that this release does not include the changes introduced in the previous 3.1.0a1 release. Those will be released at a later time.
+- v3.1.0a1(July 24, 2023)
+  - Version 3.1.0a1 is our first efforts to build snowflake-connector-python based on apache nanoarrow project, which
+reduces the package size as well as removes a hard dependency on a specific version of pyarrow.
+  - This version also includes the following features and bug fixes from the unreleased v3.0.5:
+    - Added a feature that lets you add connection definitions to the `config.toml` configuration file. A connection definition refers to a collection of connection parameters. The connection configuration name must begin with **connections**, similar to the following that defines the parameters for the `prod` connection:
+
+      ```toml
+      [connections.prod]
+      account = "my_account"
+      user = "my_user"
+      password = "my_password"
+      ```
+      By default, we look for the `config.toml` file in the location specified in the `SNOWFLAKE_HOME` environment variable (default: `~/.snowflake`). If this folder does not exist, the Python connector looks for the file in the `platformdirs` location, as follows:
+
+      - On Linux: `~/.config/snowflake/`,  but follows XDG settings
+      - On Mac: `~/Library/Application Support/snowflake/`
+      - On Windows: `%USERPROFILE%\AppData\Local\snowflake\`
+
+      You can determine which file is used by running the following command:
+
+      ```
+      python -c "from snowflake.connector.constants import CONFIG_FILE; print(str(CONFIG_FILE))"
+      ```
+    - Bumped cryptography dependency from <41.0.0,>=3.1.0 to >=3.1.0,<42.0.0.
+    - Improved OCSP response caching to remove tmp cache files on Windows.
+    - Improved OCSP response caching to reduce the times of disk writing.
+    - Added a parameter `server_session_keep_alive` in `SnowflakeConnection` that skips session deletion when client connection closes.
+    - Tightened our pinning of platformdirs, to prevent their new releases breaking us.
+    - Fixed a bug where SFPlatformDirs would incorrectly append application_name/version to its path.
+    - Added retry reason for queries that are retried by the client.
+    - Fixed a bug where `write_pandas` fails when user does not have the privilege to create stage or file format in the target schema, but has the right privilege for the current schema.
+    - Remove Python 3.7 support.
+    - Worked around a segfault which sometimes occurred during cache serialization in multi-threaded scenarios.
+    - Improved error handling of connection reset error.
+    - Fixed a bug about deleting the temporary files happened when running PUT command.
+    - Allowed to pass `type_mapper` to `fetch_pandas_batches()` and `fetch_pandas_all()`.
+    - Fixed a bug where pickle.dump segfaults during cache serialization in multi-threaded scenarios.
 
 - v3.0.4(May 23,2023)
   - Fixed a bug in which `cursor.execute()` could modify the argument statement_params dictionary object when executing a multistatement query.
   - Added the json_result_force_utf8_decoding connection parameter to force decoding JSON content in utf-8 when the result format is JSON.
   - Fixed a bug in which we cannot call `SnowflakeCursor.nextset` before fetching the result of the first query if the cursor runs an async multistatement query.
   - Bumped vendored library urllib3 to 1.26.15
   - Bumped vendored library requests to 2.29.0
```

### Comparing `snowflake-connector-python-3.1.0/README.md` & `snowflake-connector-python-3.1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/setup.cfg` & `snowflake-connector-python-3.1.0a1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description_content_type = text/markdown
 url = https://www.snowflake.com/
 author = Snowflake, Inc
 author_email = snowflake-python-libraries-dl@snowflake.com
 license = Apache-2.0
 license_files = LICENSE.txt, NOTICE
 classifiers = 
-	Development Status :: 5 - Production/Stable
+	Development Status :: 3 - Alpha
 	Environment :: Console
 	Environment :: Other Environment
 	Intended Audience :: Developers
 	Intended Audience :: Education
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
@@ -83,23 +83,23 @@
 development = 
 	Cython
 	coverage
 	more-itertools
 	numpy<1.26.0
 	pendulum!=2.1.1
 	pexpect
-	pytest<7.5.0
+	pytest<7.4.0
 	pytest-cov
 	pytest-rerunfailures
 	pytest-timeout
 	pytest-xdist
 	pytzdata
 pandas = 
 	pandas>=1.0.0,<2.1.0
-	pyarrow>=10.0.1,<10.1.0
+	pyarrow
 secure-local-storage = 
 	keyring!=16.1.0,<25.0.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/__init__.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/_query_context_cache.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/_query_context_cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/_sql_util.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/_sql_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/arrow_context.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/arrow_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from __future__ import annotations
 
 import decimal
 import time
 from datetime import datetime, timedelta, tzinfo
 from logging import getLogger
+from sys import byteorder
 from typing import TYPE_CHECKING
 
 import pytz
 from pytz import UTC
 
 from .constants import PARAMETER_TIMEZONE
 from .converter import _generate_tzinfo_from_tzoffset
@@ -144,7 +145,15 @@
         return numpy.datetime64(nanoseconds, "ns")
 
     def TIMESTAMP_NTZ_TWO_FIELD_to_numpy_datetime64(
         self, epoch: int, fraction: int
     ) -> datetime64:
         nanoseconds = int(decimal.Decimal(epoch).scaleb(9) + decimal.Decimal(fraction))
         return numpy.datetime64(nanoseconds, "ns")
+
+    def DECIMAL128_to_decimal(self, int128_bytes: bytes, scale: int):
+        int128 = int.from_bytes(int128_bytes, byteorder=byteorder, signed=True)
+        if scale == 0:
+            return int128
+        digits = [int(digit) for digit in str(int128) if digit != "-"]
+        sign = int128 < 0
+        return decimal.Decimal((sign, digits, -scale))
```

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/arrow_iterator.pyx` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/arrow_iterator.pyx`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,75 @@
 #
 # Copyright (c) 2012-2023 Snowflake Computing Inc. All rights reserved.
 #
 
 # distutils: language = c++
 # cython: language_level=3
 
+
 from cpython.ref cimport PyObject
 from cython.operator cimport dereference
+from libc.stdint cimport int64_t, uint8_t, uintptr_t
 from libcpp.memory cimport shared_ptr
 from libcpp.vector cimport vector
-from pyarrow.includes.common cimport CResult, CStatus, GetResultValue
-from pyarrow.includes.libarrow cimport (
-    CBuffer,
-    CInputStream,
-    CIpcReadOptions,
-    CRecordBatch,
-    CRecordBatchReader,
-    CRecordBatchStreamReader,
-    FileInterface,
-    FileMode,
-    Readable,
-    Seekable,
-)
 
-IF ARROW_LESS_THAN_8:
-    from pyarrow.includes.libarrow cimport PyReadableFile
-ELSE:
-    from pyarrow.includes.libarrow_python cimport PyReadableFile
+INSTALLED_PYARROW = False
+try:
+    import pyarrow
+    INSTALLED_PYARROW = True
+except ImportError:
+    pass
 
 from .constants import IterUnit
 from .errorcode import (
     ER_FAILED_TO_CONVERT_ROW_TO_PYTHON_TYPE,
     ER_FAILED_TO_READ_ARROW_STREAM,
+    ER_NO_PYARROW,
 )
-from .errors import Error, InterfaceError, OperationalError
+from .errors import Error, InterfaceError, OperationalError, ProgrammingError
 from .snow_logging import getSnowLogger
 
 snow_logger = getSnowLogger(__name__)
 
 
-cdef extern from "cpp/ArrowIterator/CArrowIterator.hpp" namespace "sf":
+cdef extern from "CArrowIterator.hpp" namespace "sf":
     cdef cppclass ReturnVal:
         PyObject * successObj;
 
         PyObject * exception;
 
     cdef cppclass CArrowIterator:
         shared_ptr[ReturnVal] next() except +;
+        vector[uintptr_t] getArrowArrayPtrs();
+        vector[uintptr_t] getArrowSchemaPtrs();
 
 
-cdef extern from "cpp/ArrowIterator/CArrowChunkIterator.hpp" namespace "sf":
+cdef extern from "CArrowChunkIterator.hpp" namespace "sf":
     cdef cppclass CArrowChunkIterator(CArrowIterator):
         CArrowChunkIterator(
-                PyObject* context,
-                vector[shared_ptr[CRecordBatch]]* batches,
-                PyObject* use_numpy,
+            PyObject* context,
+            char* arrow_bytes,
+            int64_t arrow_bytes_size,
+            PyObject* use_numpy,
         ) except +
 
     cdef cppclass DictCArrowChunkIterator(CArrowChunkIterator):
         DictCArrowChunkIterator(
-                PyObject* context,
-                vector[shared_ptr[CRecordBatch]]* batches,
-                PyObject* use_numpy
+            PyObject* context,
+            char* arrow_bytes,
+            int64_t arrow_bytes_size,
+            PyObject* use_numpy
         ) except +
 
-
-cdef extern from "cpp/ArrowIterator/CArrowTableIterator.hpp" namespace "sf":
+cdef extern from "CArrowTableIterator.hpp" namespace "sf":
     cdef cppclass CArrowTableIterator(CArrowIterator):
         CArrowTableIterator(
             PyObject* context,
-            vector[shared_ptr[CRecordBatch]]* batches,
+            char* arrow_bytes,
+            int64_t arrow_bytes_size,
             bint number_to_decimal,
         ) except +
 
 
 cdef class EmptyPyArrowIterator:
 
     def __iter__(self):
@@ -87,92 +83,72 @@
 
 
 cdef class PyArrowIterator(EmptyPyArrowIterator):
     cdef object context
     cdef CArrowIterator* cIterator
     cdef str unit
     cdef shared_ptr[ReturnVal] cret
-    cdef vector[shared_ptr[CRecordBatch]] batches
     cdef object use_dict_result
     cdef object cursor
+    cdef vector[uintptr_t] nanoarrow_Table
+    cdef vector[uintptr_t] nanoarrow_Schema
+    cdef object table_returned
+    cdef char* arrow_bytes
+    cdef int64_t arrow_bytes_size
 
     # this is the flag indicating whether fetch data as numpy datatypes or not. The flag
     # is passed from the constructor of SnowflakeConnection class. Note, only FIXED, REAL
     # and TIMESTAMP_NTZ will be converted into numpy data types, all other sql types will
     # still be converted into native python types.
     # https://docs.snowflake.com/en/user-guide/sqlalchemy.html#numpy-data-type-support
     cdef object use_numpy
     cdef object number_to_decimal
+    cdef object pyarrow_table
+    # this is needed keep the original reference of the python bytes object
+    cdef object python_bytes
 
     def __cinit__(
             self,
             object cursor,
-            object py_inputstream,
+            object arrow_bytes,
             object arrow_context,
             object use_dict_result,
             object numpy,
             object number_to_decimal,
-    ):
-        cdef shared_ptr[CInputStream] input_stream
-        cdef shared_ptr[CRecordBatch] record_batch
-        cdef CStatus ret
-        input_stream.reset(new PyReadableFile(py_inputstream))
-        cdef CResult[shared_ptr[CRecordBatchReader]] readerRet = CRecordBatchStreamReader.Open(
-            input_stream,
-            CIpcReadOptions.Defaults()
-            )
-        if not readerRet.ok():
-            Error.errorhandler_wrapper(
-                cursor.connection if cursor is not None else None,
-                cursor,
-                OperationalError,
-                {
-                    'msg': f'Failed to open arrow stream: {readerRet.status().message()}',
-                    'errno': ER_FAILED_TO_READ_ARROW_STREAM
-                })
-
-        cdef shared_ptr[CRecordBatchReader] reader = dereference(readerRet)
-
-        while True:
-            ret = reader.get().ReadNext(&record_batch)
-            if not ret.ok():
-                Error.errorhandler_wrapper(
-                    cursor.connection if cursor is not None else None,
-                    cursor,
-                    OperationalError,
-                    {
-                        'msg': f'Failed to read next arrow batch: {ret.message()}',
-                        'errno': ER_FAILED_TO_READ_ARROW_STREAM
-                    }
-                )
-
-            if record_batch.get() is NULL:
-                break
-
-            self.batches.push_back(record_batch)
-
-        snow_logger.debug(msg=f"Batches read: {self.batches.size()}", path_name=__file__, func_name="__cinit__")
 
+    ):
         self.context = arrow_context
         self.cIterator = NULL
         self.unit = ''
         self.use_dict_result = use_dict_result
         self.cursor = cursor
         self.use_numpy = numpy
         self.number_to_decimal = number_to_decimal
+        self.pyarrow_table = None
+        self.table_returned = False
+        self.arrow_bytes = <char*>arrow_bytes
+        self.arrow_bytes_size = len(arrow_bytes)
+        self.python_bytes = arrow_bytes
 
     def __dealloc__(self):
         del self.cIterator
 
     def __iter__(self):
         return self
 
     def __next__(self):
         if self.cIterator is NULL:
             self.init_row_unit()
+
+        if self.unit == IterUnit.TABLE_UNIT.value:
+            if not self.table_returned:
+                self.table_returned = True
+                return self.pyarrow_table
+            raise StopIteration
+
         self.cret = self.cIterator.next()
 
         if not self.cret.get().successObj:
             Error.errorhandler_wrapper(
                 self.cursor.connection if self.cursor is not None else None,
                 self.cursor,
                 InterfaceError,
@@ -196,23 +172,53 @@
         elif iter_unit == IterUnit.TABLE_UNIT.value:
             self.init_table_unit()
         self.unit = iter_unit
 
     def init_row_unit(self) -> None:
         self.cIterator = new CArrowChunkIterator(
             <PyObject *> self.context,
-            &self.batches,
+            self.arrow_bytes,
+            self.arrow_bytes_size,
             <PyObject *> self.use_numpy
         ) \
             if not self.use_dict_result \
             else new DictCArrowChunkIterator(
             <PyObject *> self.context,
-            &self.batches,
+            self.arrow_bytes,
+            self.arrow_bytes_size,
             <PyObject *> self.use_numpy
             )
+        snow_logger.debug(msg=f"Batches read: {self.cIterator.getArrowArrayPtrs().size()}", path_name=__file__, func_name="init_row_unit")
 
     def init_table_unit(self) -> None:
+        if not INSTALLED_PYARROW:
+            raise Error.errorhandler_make_exception(
+                ProgrammingError,
+                {
+                    "msg": (
+                        "Optional dependency: 'pyarrow' is not installed, please see the following link for install "
+                        "instructions: https://docs.snowflake.com/en/user-guide/python-connector-pandas.html#installation"
+                    ),
+                    "errno": ER_NO_PYARROW,
+                },
+            )
+
         self.cIterator = new CArrowTableIterator(
             <PyObject *> self.context,
-            &self.batches,
+            self.arrow_bytes,
+            self.arrow_bytes_size,
             self.number_to_decimal,
         )
+
+        self.cret = self.cIterator.next()
+        self.unit = 'table'
+        self.nanoarrow_Table = self.cIterator.getArrowArrayPtrs()
+        self.nanoarrow_Schema = self.cIterator.getArrowSchemaPtrs()
+        self.pyarrow_table = pyarrow.Table.from_batches(
+            batches=[
+                pyarrow.RecordBatch._import_from_c(
+                    self.nanoarrow_Table[i],
+                    self.nanoarrow_Schema[i]
+                ) for i in range(self.nanoarrow_Table.size())
+            ]
+        )
+        snow_logger.debug(msg=f"Batches read: {self.nanoarrow_Table.size()}", path_name=__file__, func_name="init_table_unit")
```

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/auth/__init__.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/auth/_auth.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/_auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/auth/by_plugin.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/by_plugin.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/auth/default.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/default.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/auth/idtoken.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/idtoken.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/auth/keypair.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/keypair.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/auth/oauth.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/auth/okta.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/okta.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,27 +3,25 @@
 # Copyright (c) 2012-2023 Snowflake Computing Inc. All rights reserved.
 #
 
 from __future__ import annotations
 
 import json
 import logging
-import time
-from functools import partial
-from typing import TYPE_CHECKING, Any, Callable
+from typing import TYPE_CHECKING, Any
 
 from ..compat import unescape, urlencode, urlsplit
 from ..constants import (
     HTTP_HEADER_ACCEPT,
     HTTP_HEADER_CONTENT_TYPE,
     HTTP_HEADER_SERVICE_NAME,
     HTTP_HEADER_USER_AGENT,
 )
 from ..errorcode import ER_IDP_CONNECTION_ERROR, ER_INCORRECT_DESTINATION
-from ..errors import DatabaseError, Error, RefreshTokenError
+from ..errors import DatabaseError, Error
 from ..network import CONTENT_TYPE_APPLICATION_JSON, PYTHON_CONNECTOR_USER_AGENT
 from ..sqlstate import SQLSTATE_CONNECTION_WAS_NOT_ESTABLISHED
 from . import Auth
 from .by_plugin import AuthByPlugin, AuthType
 
 if TYPE_CHECKING:
     from .. import SnowflakeConnection
@@ -131,19 +129,16 @@
             conn,
             authenticator,
             service_name,
             account,
             user,
         )
         self._step2(conn, authenticator, sso_url, token_url)
-        response_html = self._step4(
-            conn,
-            partial(self._step3, conn, headers, token_url, user, password),
-            sso_url,
-        )
+        one_time_token = self._step3(conn, headers, token_url, user, password)
+        response_html = self._step4(conn, one_time_token, sso_url)
         self._step5(conn, response_html)
 
     def reauthenticate(self, **kwargs: Any) -> dict[str, bool]:
         return {"success": False}
 
     def _step1(
         self,
@@ -267,43 +262,34 @@
                 },
             )
         return one_time_token
 
     @staticmethod
     def _step4(
         conn: SnowflakeConnection,
-        generate_one_time_token: Callable,
+        one_time_token: str,
         sso_url: str,
-    ) -> dict[Any, Any]:
+    ):
         logger.debug("step 4: query IDP URL snowflake app to get SAML " "response")
-        timeout_time = time.time() + conn.login_timeout if conn.login_timeout else None
-        response_html = {}
-        while timeout_time is None or time.time() < timeout_time:
-            try:
-                url_parameters = {
-                    "RelayState": "/some/deep/link",
-                    "onetimetoken": generate_one_time_token(),
-                }
-                sso_url = sso_url + "?" + urlencode(url_parameters)
-                headers = {
-                    HTTP_HEADER_ACCEPT: "*/*",
-                }
-                remaining_timeout = timeout_time - time.time() if timeout_time else None
-                response_html = conn._rest.fetch(
-                    "get",
-                    sso_url,
-                    headers,
-                    timeout=remaining_timeout,
-                    socket_timeout=remaining_timeout,
-                    is_raw_text=True,
-                    is_okta_authentication=True,
-                )
-                break
-            except RefreshTokenError:
-                logger.debug("step4: refresh token for re-authentication")
+        url_parameters = {
+            "RelayState": "/some/deep/link",
+            "onetimetoken": one_time_token,
+        }
+        sso_url = sso_url + "?" + urlencode(url_parameters)
+        headers = {
+            HTTP_HEADER_ACCEPT: "*/*",
+        }
+        response_html = conn._rest.fetch(
+            "get",
+            sso_url,
+            headers,
+            timeout=conn.login_timeout,
+            socket_timeout=conn.login_timeout,
+            is_raw_text=True,
+        )
         return response_html
 
     def _step5(
         self,
         conn: SnowflakeConnection,
         response_html: str,
     ) -> None:
```

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/auth/usrpwdmfa.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/usrpwdmfa.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/auth/webbrowser.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/auth/webbrowser.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/azure_storage_client.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/azure_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/bind_upload_agent.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/bind_upload_agent.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/cache.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -642,14 +642,21 @@
                 datetime.datetime.fromtimestamp(
                     getmtime(self.file_path),
                 )
                 > self.last_loaded
             )
         return False
 
+    def __del__(self) -> None:
+        try:
+            self._save()
+        except Exception:
+            # At tear-down time builtins module might be already gone, ignore every error
+            pass
+
     def clear(self) -> None:
         super().clear()
         # This unlink prevents us from loading just before saving
         with self._file_lock:
             if os.path.exists(self.file_path) and os.path.isfile(self.file_path):
                 os.unlink(self.file_path)
         # TODO: is this necessary?
```

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/compat.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/config_manager.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/config_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,34 @@
 #
 # Copyright (c) 2012-2023 Snowflake Computing Inc. All rights reserved.
 #
 
 from __future__ import annotations
 
-import itertools
 import logging
 import os
 import stat
 from collections.abc import Iterable
 from operator import methodcaller
 from pathlib import Path
-from typing import Any, Callable, Literal, NamedTuple, TypeVar
+from typing import Any, Callable, Literal, TypeVar
 from warnings import warn
 
 import tomlkit
 from tomlkit.items import Table
 
-from snowflake.connector.constants import CONFIG_FILE, CONNECTIONS_FILE
-from snowflake.connector.errors import (
-    ConfigManagerError,
-    ConfigSourceError,
-    MissingConfigOptionError,
-)
+from snowflake.connector.constants import CONFIG_FILE
+from snowflake.connector.errors import ConfigManagerError, ConfigSourceError
 
 _T = TypeVar("_T")
 
 LOGGER = logging.getLogger(__name__)
 READABLE_BY_OTHERS = stat.S_IRGRP | stat.S_IROTH
 
 
-class ConfigSliceOptions(NamedTuple):
-    """Class that defines settings individual configuration files."""
-
-    check_permissions: bool = True
-    only_in_slice: bool = False
-
-
-class ConfigSlice(NamedTuple):
-    path: Path
-    options: ConfigSliceOptions
-    section: str
-
-
 class ConfigOption:
     """ConfigOption represents a flag/setting.
 
     The class knows how to read the value out of all sources and implements
     order of precedence between them.
 
     Attributes:
@@ -152,34 +134,27 @@
         if isinstance(loaded_var, (Table, tomlkit.TOMLDocument)):
             # If we got a TOML table we probably want it in dictionary form
             return True, loaded_var.value
         return True, loaded_var
 
     def _get_config(self) -> Any:
         """Get value from the cached config file."""
-        if (
-            self._root_manager.conf_file_cache is None
-            and self._root_manager.file_path is not None
+        if self._root_manager.conf_file_cache is None and (
+            self._root_manager.file_path is not None
+            and self._root_manager.file_path.exists()
+            and self._root_manager.file_path.is_file()
         ):
             self._root_manager.read_config()
         e = self._root_manager.conf_file_cache
         if e is None:
             raise ConfigManagerError(
                 f"Root parser '{self._root_manager.name}' is missing file_path",
             )
         for k in self._nest_path[1:]:
-            try:
-                e = e[k]
-            except tomlkit.exceptions.NonExistentKey:
-                raise MissingConfigOptionError(  # TOOO: maybe a child Exception for missing option?
-                    f"Configuration option '{self.option_name}' is not defined anywhere, "
-                    "have you forgotten to set it in a configuration file, "
-                    "or environmental variable?"
-                )
-
+            e = e[k]
         if isinstance(e, (Table, tomlkit.TOMLDocument)):
             # If we got a TOML table we probably want it in dictionary form
             return e.value
         return e
 
 
 class ConfigManager:
@@ -211,28 +186,24 @@
     """
 
     def __init__(
         self,
         *,
         name: str,
         file_path: Path | None = None,
-        _slices: list[ConfigSlice] | None = None,
     ):
         """Create a new ConfigManager.
 
         Args:
             name: Name of this ConfigManager.
             file_path: File this parser should read values from. Can be omitted
               for all child parsers.
         """
-        if _slices is None:
-            _slices = list()
         self.name = name
         self.file_path = file_path
-        self._slices = _slices
         # Objects holding subparsers and options
         self._options: dict[str, ConfigOption] = dict()
         self._sub_parsers: dict[str, ConfigManager] = dict()
         # Dictionary to cache read in config file
         self.conf_file_cache: tomlkit.TOMLDocument | None = None
         # Information necessary to be able to nest elements
         #  and add options in O(1)
@@ -250,50 +221,37 @@
         adding new options to their configuration files.
         """
         if self.file_path is None:
             raise ConfigManagerError(
                 "ConfigManager is trying to read config file, but it doesn't "
                 "have one"
             )
-        read_config_file = tomlkit.TOMLDocument()
-
-        # Read in all of the config slices
-        for filep, sliceoptions, section in itertools.chain(
-            ((self.file_path, ConfigSliceOptions(), None),),
-            self._slices,
+        if not self.file_path.exists():
+            raise ConfigSourceError(
+                f"The config file '{self.file_path}' does not exist"
+            )
+        if (
+            # Same check as openssh does for permissions
+            #  https://github.com/openssh/openssh-portable/blob/2709809fd616a0991dc18e3a58dea10fb383c3f0/readconf.c#LL2264C1-L2264C1
+            self.file_path.stat().st_mode & READABLE_BY_OTHERS != 0
+            or (
+                # TODO: Windows doesn't have getuid, skip checking
+                hasattr(os, "getuid")
+                and self.file_path.stat().st_uid != 0
+                and self.file_path.stat().st_uid != os.getuid()
+            )
         ):
-            if sliceoptions.only_in_slice:
-                del read_config_file[section]
-            if not filep.exists():
-                continue
-            if (
-                sliceoptions.check_permissions  # Skip checking if this file couldn't hold sensitive information
-                # Same check as openssh does for permissions
-                #  https://github.com/openssh/openssh-portable/blob/2709809fd616a0991dc18e3a58dea10fb383c3f0/readconf.c#LL2264C1-L2264C1
-                and filep.stat().st_mode & READABLE_BY_OTHERS != 0
-                or (
-                    # Windows doesn't have getuid, skip checking
-                    hasattr(os, "getuid")
-                    and filep.stat().st_uid != 0
-                    and filep.stat().st_uid != os.getuid()
-                )
-            ):
-                warn(f"Bad owner or permissions on {str(filep)}")
-            LOGGER.debug(f"reading configuration file from {str(filep)}")
-            try:
-                read_config_piece = tomlkit.parse(filep.read_text())
-            except Exception as e:
-                raise ConfigSourceError(
-                    "An unknown error happened while loading " f"'{str(filep)}'"
-                ) from e
-            if section is None:
-                read_config_file = read_config_piece
-            else:
-                read_config_file[section] = read_config_piece
-        self.conf_file_cache = read_config_file
+            warn(f"Bad owner or permissions on {self.file_path}")
+        LOGGER.debug(f"reading configuration file from {str(self.file_path)}")
+        try:
+            self.conf_file_cache = tomlkit.parse(self.file_path.read_text())
+        except Exception as e:
+            raise ConfigSourceError(
+                "An unknown error happened while loading " f"'{str(self.file_path)}'"
+            ) from e
 
     def add_option(
         self,
         *,
         option_cls: type[ConfigOption] = ConfigOption,
         **kwargs,
     ) -> None:
@@ -369,23 +327,14 @@
             )
         return self._sub_parsers[name]
 
 
 CONFIG_PARSER = ConfigManager(
     name="CONFIG_PARSER",
     file_path=CONFIG_FILE,
-    _slices=[
-        ConfigSlice(  # Optional connections file to read in connections from
-            CONNECTIONS_FILE,
-            ConfigSliceOptions(
-                check_permissions=True,  # connections could live here, check permissions
-            ),
-            "connections",
-        ),
-    ],
 )
 CONFIG_PARSER.add_option(
     name="connections",
     parse_str=tomlkit.parse,
 )
 
 __all__ = [
```

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/connection.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     SnowflakeRestful,
 )
 from .sqlstate import SQLSTATE_CONNECTION_NOT_EXISTS, SQLSTATE_FEATURE_NOT_SUPPORTED
 from .telemetry import TelemetryClient, TelemetryData, TelemetryField
 from .telemetry_oob import TelemetryService
 from .time_util import HeartBeatTimer, get_time_millis
 from .util_text import construct_hostname, parse_account, split_statements
+from .version import VERSION
 
 DEFAULT_CLIENT_PREFETCH_THREADS = 4
 MAX_CLIENT_PREFETCH_THREADS = 10
 
 
 def DefaultConverterClass() -> type:
     if IS_WINDOWS:
@@ -293,15 +294,15 @@
     """
 
     OCSP_ENV_LOCK = Lock()
 
     def __init__(
         self,
         connection_name: str | None = None,
-        connections_file_path: pathlib.Path | None = None,
+        config_file_path: pathlib.Path | None = None,
         **kwargs,
     ) -> None:
         self._lock_sequence_counter = Lock()
         self.sequence_counter = 0
         self._errorhandler = Error.default_errorhandler
         self._lock_converter = Lock()
         self.messages = []
@@ -328,35 +329,42 @@
                 kwargs["application"] = os.environ[ENV_VAR_PARTNER]
             elif "streamlit" in sys.modules:
                 kwargs["application"] = "streamlit"
 
         self.converter = None
         self.query_context_cache: QueryContextCache | None = None
         self.query_context_cache_size = 5
-        if connections_file_path is not None:
+        if config_file_path is not None:
             # Change config file path and force update cache
-            for i, s in enumerate(CONFIG_PARSER._slices):
-                if s.section == "connections":
-                    CONFIG_PARSER._slices[i] = s._replace(path=connections_file_path)
-                    CONFIG_PARSER.read_config()
-                    break
+            CONFIG_PARSER.file_path = config_file_path
+            CONFIG_PARSER.read_config()
         if connection_name is not None:
             connections = CONFIG_PARSER["connections"]
             if connection_name not in connections:
                 raise Error(
                     f"Invalid connection_name '{connection_name}',"
                     f" known ones are {list(connections.keys())}"
                 )
             kwargs = {**connections[connection_name], **kwargs}
         self.__set_error_attributes()
         self.connect(**kwargs)
         self._telemetry = TelemetryClient(self._rest)
-
         # get the imported modules from sys.modules
         self._log_telemetry_imported_packages()
+        # in the future we won't need this if the backend supports prerelease versions
+        self._log_telemetry(
+            TelemetryData.from_telemetry_data_dict(
+                from_dict={
+                    TelemetryField.KEY_IS_PRERELEASE.value: TelemetryData.FALSE
+                    if str(VERSION[2]).isdigit()
+                    else TelemetryData.TRUE
+                },
+                timestamp=get_time_millis(),
+            )
+        )
 
     def __del__(self) -> None:  # pragma: no cover
         try:
             self.close(retry=False)
         except Exception:
             pass
 
@@ -365,16 +373,15 @@
         return self._insecure_mode
 
     @property
     def ocsp_fail_open(self) -> bool:
         return self._ocsp_fail_open
 
     def _ocsp_mode(self) -> OCSPMode:
-        """OCSP mode. INSEC
-        URE, FAIL_OPEN or FAIL_CLOSED."""
+        """OCSP mode. INSECURE, FAIL_OPEN or FAIL_CLOSED."""
         if self.insecure_mode:
             return OCSPMode.INSECURE
         elif self.ocsp_fail_open:
             return OCSPMode.FAIL_OPEN
         else:
             return OCSPMode.FAIL_CLOSED
```

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/connection_diagnostic.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/connection_diagnostic.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/constants.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,20 +17,19 @@
 
 # Snowflake's central platform dependent directories, if the folder
 # ~/.snowflake/ (customizable by the environment variable SNOWFLAKE_HOME) exists
 # we use that folder for everything. Otherwise, we fall back to platformdirs
 # defaults. Please see comments in sf_dir.py for more information.
 DIRS = _resolve_platform_dirs()
 
-# Snowflake's configuration files. By default, platformdirs will resolve
+# Snowflake's central configuration file. By default, platformdirs will resolve
 # them to these places depending on OS:
-#   * Linux: `~/.config/snowflake/filename` but can be updated with XDG vars
-#   * Windows: `%USERPROFILE%\AppData\Local\snowflake\filename`
-#   * Mac: `~/Library/Application Support/snowflake/filename`
-CONNECTIONS_FILE = DIRS.user_config_path / "connections.toml"
+#   * Linux: `~/.config/snowflake/config.toml` but can be updated with XDG vars
+#   * Windows: `%USERPROFILE%\AppData\Local\snowflake\config.toml`
+#   * Mac: `~/Library/Application Support/snowflake/config.toml`
 CONFIG_FILE = DIRS.user_config_path / "config.toml"
 
 DBAPI_TYPE_STRING = 0
 DBAPI_TYPE_BINARY = 1
 DBAPI_TYPE_NUMBER = 2
 DBAPI_TYPE_TIMESTAMP = 3
```

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/converter.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/converter.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/converter_issue23517.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/converter_issue23517.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/converter_snowsql.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/converter_snowsql.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp`

 * *Files 27% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 //
 
 #ifndef PC_BINARYCONVERTER_HPP
 #define PC_BINARYCONVERTER_HPP
 
 #include "IColumnConverter.hpp"
 #include "logging.hpp"
+#include "nanoarrow.h"
 #include <memory>
 
 namespace sf
 {
 
 class BinaryConverter : public IColumnConverter
 {
 public:
-  explicit BinaryConverter(std::shared_ptr<arrow::Array> array);
+  explicit BinaryConverter(ArrowArrayView* array);
 
   PyObject* toPyObject(int64_t rowIndex) const override;
 
 private:
-  std::shared_ptr<arrow::BinaryArray> m_array;
+  ArrowArrayView* m_array;
 
   static Logger* logger;
 };
 
 }  // namespace sf
 
 #endif  // PC_BINARYCONVERTER_HPP
```

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 #ifndef PC_ARROWCHUNKITERATOR_HPP
 #define PC_ARROWCHUNKITERATOR_HPP
 
 #include "CArrowIterator.hpp"
 #include "IColumnConverter.hpp"
 #include "Python/Common.hpp"
+#include "nanoarrow.h"
+#include "nanoarrow.hpp"
 #include <memory>
 #include <vector>
 
 namespace sf
 {
 
 /**
@@ -21,18 +23,18 @@
  */
 class CArrowChunkIterator : public CArrowIterator
 {
 public:
   /**
    * Constructor
    */
-  CArrowChunkIterator(PyObject* context, std::vector<std::shared_ptr<arrow::RecordBatch>> * batches, PyObject *use_numpy);
+  CArrowChunkIterator(PyObject* context, char* arrow_bytes, int64_t arrow_bytes_size, PyObject *use_numpy);
 
   /**
-   * Desctructor
+   * Destructor
    */
   virtual ~CArrowChunkIterator() = default;
 
   /**
    * @return a python tuple object which contains all data in current row
    */
   std::shared_ptr<ReturnVal> next() override;
@@ -44,21 +46,17 @@
   virtual void createRowPyObject();
 
   /** pointer to the latest returned python tuple(row) result */
   py::UniqueRef m_latestReturnedRow;
 
   /** list of column converters*/
   std::vector<std::shared_ptr<sf::IColumnConverter>> m_currentBatchConverters;
-
   /** row index inside current record batch (start from 0) */
   int m_rowIndexInBatch;
 
-  /** schema of current record batch */
-  std::shared_ptr<arrow::Schema> m_currentSchema;
-
 private:
   /** number of columns */
   int m_columnCount;
 
   /** number of record batch in current chunk */
   int m_batchCount;
 
@@ -79,15 +77,15 @@
 
   void initColumnConverters();
 };
 
 class DictCArrowChunkIterator : public CArrowChunkIterator
 {
 public:
-  DictCArrowChunkIterator(PyObject* context, std::vector<std::shared_ptr<arrow::RecordBatch>> * batches, PyObject *use_numpy);
+  DictCArrowChunkIterator(PyObject* context, char* arrow_bytes, int64_t arrow_bytes_size, PyObject *use_numpy);
 
   ~DictCArrowChunkIterator() = default;
 
 private:
 
   void createRowPyObject() override;
```

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -19,47 +19,41 @@
     py::importPythonModule("datetime", pyDatetimeModule);
     py::importFromModule(pyDatetimeModule, "date", pyDatetimeDate);
     Py_XINCREF(pyDatetimeDate.get());
   }
   return pyDatetimeDate;
 }
 
-DateConverter::DateConverter(std::shared_ptr<arrow::Array> array)
-: m_array(std::dynamic_pointer_cast<arrow::Date32Array>(array)),
+DateConverter::DateConverter(ArrowArrayView* array)
+: m_array(array),
   m_pyDatetimeDate(initPyDatetimeDate())
 {
 }
 
 PyObject* DateConverter::toPyObject(int64_t rowIndex) const
 {
-  if (m_array->IsValid(rowIndex))
-  {
-    int32_t deltaDays = m_array->Value(rowIndex);
+    if(ArrowArrayViewIsNull(m_array, rowIndex)) {
+    Py_RETURN_NONE;
+    }
+
+    int64_t deltaDays = ArrowArrayViewGetIntUnsafe(m_array, rowIndex);
     return PyObject_CallMethod(m_pyDatetimeDate.get(), "fromordinal", "i",
                                epochDay + deltaDays);
-  }
-  else
-  {
-    Py_RETURN_NONE;
-  }
 }
 
-NumpyDateConverter::NumpyDateConverter(std::shared_ptr<arrow::Array> array, PyObject * context)
-: m_array(std::dynamic_pointer_cast<arrow::Date32Array>(array)),
+NumpyDateConverter::NumpyDateConverter(ArrowArrayView* array, PyObject * context)
+: m_array(array),
   m_context(context)
 {
 }
 
 PyObject* NumpyDateConverter::toPyObject(int64_t rowIndex) const
 {
-  if (m_array->IsValid(rowIndex))
-  {
-    int32_t deltaDays = m_array->Value(rowIndex);
-    return PyObject_CallMethod(m_context, "DATE_to_numpy_datetime64", "i", deltaDays);
-  }
-  else
-  {
+    if(ArrowArrayViewIsNull(m_array, rowIndex)) {
     Py_RETURN_NONE;
-  }
+    }
+
+    int64_t deltaDays = ArrowArrayViewGetIntUnsafe(m_array, rowIndex);
+    return PyObject_CallMethod(m_context, "DATE_to_numpy_datetime64", "i", deltaDays);
 }
 
 }  // namespace sf
```

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp`

 * *Files 25% similar despite different names*

```diff
@@ -26,37 +26,77 @@
     py::importFromModule(decimalModule, "Decimal", pyDecimalConstructor);
     Py_XINCREF(pyDecimalConstructor.get());
   }
 
   return pyDecimalConstructor;
 }
 
+DecimalFromIntConverter::DecimalFromIntConverter(ArrowArrayView* array,
+                                   int precision, int scale)
+  : m_array(array),
+    m_precision(precision),
+    m_scale(scale)
+  {
+  }
+
+PyObject* DecimalFromIntConverter::toPyObject(int64_t rowIndex) const
+{
+  if(ArrowArrayViewIsNull(m_array, rowIndex)) {
+    Py_RETURN_NONE;
+  }
+  int64_t val = ArrowArrayViewGetIntUnsafe(m_array, rowIndex);
+  py::UniqueRef decimal(
+        PyObject_CallFunction(m_pyDecimalConstructor.get(), "L", val));
+  return PyObject_CallMethod(decimal.get(), "scaleb", "i", -m_scale);
+}
+
+NumpyDecimalConverter::NumpyDecimalConverter(ArrowArrayView* array,
+                                 int precision, int scale, PyObject * context)
+  : m_array(array),
+    m_precision(precision),
+    m_scale(scale),
+    m_context(context)
+  {
+  }
+
+PyObject* NumpyDecimalConverter::toPyObject(int64_t rowIndex) const
+{
+    if(ArrowArrayViewIsNull(m_array, rowIndex)) {
+        Py_RETURN_NONE;
+    }
+    int64_t val = ArrowArrayViewGetIntUnsafe(m_array, rowIndex);
+    return PyObject_CallMethod(m_context, "FIXED_to_numpy_float64", "Li", val, m_scale);
+}
+
 DecimalFromDecimalConverter::DecimalFromDecimalConverter(
-    std::shared_ptr<arrow::Array> array, int scale)
-: m_array(std::dynamic_pointer_cast<arrow::Decimal128Array>(array)),
+    PyObject* context,
+    ArrowArrayView* array, int scale)
+: m_array(array),
+  m_context(context),
   m_scale(scale)
 {
 }
 
 PyObject* DecimalFromDecimalConverter::toPyObject(int64_t rowIndex) const
 {
-  if (m_array->IsValid(rowIndex))
-  {
-    std::string formatDecimalString = m_array->FormatValue(rowIndex);
-    if (m_scale == 0)
-    {
-      return PyLong_FromString(formatDecimalString.c_str(), nullptr, 0);
-    }
-
-    /** the reason we use c_str() instead of std::string here is that we may
-     * meet some encoding problem with std::string */
-    return PyObject_CallFunction(m_pyDecimalConstructor.get(), "s#",
-                                 formatDecimalString.c_str(),
-                                 static_cast<Py_ssize_t>(formatDecimalString.size()));
-  }
-  else
-  {
+  if(ArrowArrayViewIsNull(m_array, rowIndex)) {
     Py_RETURN_NONE;
   }
+  int64_t bytes_start = 16 * (m_array->array->offset + rowIndex);
+  const char* ptr_start = m_array->buffer_views[1].data.as_char;
+  PyObject* int128_bytes = PyBytes_FromStringAndSize(&(ptr_start[bytes_start]), 16);
+  /**
+  # Alternatively, the decimal conversion can be implemented using the ArrowDecimal related APIs in the following
+  # code snippets, however, it's less performant than the direct memory manipulation.
+  # The code snippets here is for context reference.
+
+  ArrowDecimal arrowDecimal;
+  ArrowDecimalInit(&arrowDecimal, 128, precision, scale);
+  ArrowArrayViewGetDecimalUnsafe(m_array, rowIndex, &arrowDecimal);
+  uint8_t outBytes[16];
+  ArrowDecimalGetBytes(&arrowDecimal, outBytes);
+  PyObject* int128_bytes = PyBytes_FromStringAndSize(&outBytes, 16);
+  */
+  return PyObject_CallMethod(m_context, "DECIMAL128_to_decimal", "Si", int128_bytes, m_scale);
 }
 
 }  // namespace sf
```

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 //
 
 #ifndef PC_DECIMALCONVERTER_HPP
 #define PC_DECIMALCONVERTER_HPP
 
 #include "IColumnConverter.hpp"
 #include "Python/Common.hpp"
+#include "nanoarrow.h"
 #include <memory>
 
 namespace sf
 {
 
 class DecimalBaseConverter : public IColumnConverter
 {
@@ -24,104 +25,54 @@
 private:
   static py::UniqueRef& initPyDecimalConstructor();
 };
 
 class DecimalFromDecimalConverter : public DecimalBaseConverter
 {
 public:
-  explicit DecimalFromDecimalConverter(std::shared_ptr<arrow::Array> array,
-                                       int scale);
+  explicit DecimalFromDecimalConverter(PyObject* context, ArrowArrayView* array, int scale);
 
   PyObject* toPyObject(int64_t rowIndex) const override;
 
 private:
-  std::shared_ptr<arrow::Decimal128Array> m_array;
-
+  ArrowArrayView* m_array;
+  PyObject* m_context;
   int m_scale;
   /** no need for this converter to store precision*/
 };
 
-template <typename T>
 class DecimalFromIntConverter : public DecimalBaseConverter
 {
 public:
-  explicit DecimalFromIntConverter(std::shared_ptr<arrow::Array> array,
-                                   int precision, int scale)
-  : m_array(std::dynamic_pointer_cast<T>(array)),
-    m_precision(precision),
-    m_scale(scale)
-  {
-  }
+  explicit DecimalFromIntConverter(ArrowArrayView* array, int precision, int scale);
 
   PyObject* toPyObject(int64_t rowIndex) const override;
 
 private:
-  std::shared_ptr<T> m_array;
-
+  ArrowArrayView* m_array;
   int m_precision;  // looks like the precision here is not useful, and this
                     // will be removed soon when it's been confirmed
 
   int m_scale;
 };
 
-template <typename T>
-PyObject* DecimalFromIntConverter<T>::toPyObject(int64_t rowIndex) const
-{
-  if (m_array->IsValid(rowIndex))
-  {
-    int64_t val = m_array->Value(rowIndex);
-
-    py::UniqueRef decimal(
-        PyObject_CallFunction(m_pyDecimalConstructor.get(), "L", val));
-    return PyObject_CallMethod(decimal.get(), "scaleb", "i", -m_scale);
-  }
-  else
-  {
-    Py_RETURN_NONE;
-  }
-}
-
 
-template <typename T>
 class NumpyDecimalConverter : public IColumnConverter
 {
 public:
-  explicit NumpyDecimalConverter(std::shared_ptr<arrow::Array> array,
-                                 int precision, int scale, PyObject * context)
-  : m_array(std::dynamic_pointer_cast<T>(array)),
-    m_precision(precision),
-    m_scale(scale),
-    m_context(context)
-  {
-  }
+  explicit NumpyDecimalConverter(ArrowArrayView* array, int precision, int scale, PyObject * context);
 
   PyObject* toPyObject(int64_t rowIndex) const override;
 
 private:
-  std::shared_ptr<T> m_array;
+  ArrowArrayView* m_array;
 
   int m_precision;
 
   int m_scale;
 
   PyObject * m_context;
 };
 
-template <typename T>
-PyObject* NumpyDecimalConverter<T>::toPyObject(int64_t rowIndex) const
-{
-  if (m_array->IsValid(rowIndex))
-  {
-    int64_t val = m_array->Value(rowIndex);
-
-    return PyObject_CallMethod(m_context, "FIXED_to_numpy_float64", "Li", val, m_scale);
-  }
-  else
-  {
-    Py_RETURN_NONE;
-  }
-}
-
-
 }  // namespace sf
 
 #endif  // PC_DECIMALCONVERTER_HPP
```

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -8,19 +8,14 @@
 // Support for not having PY_SSIZE_T_CLEAN defined will end in Python 3.10. It causes
 //  argument parsing to not accept integers, leaving only Py_ssize_t as an option
 #define PY_SSIZE_T_CLEAN
 
 // We have to make sure that we import Python.h once for special flags that need to be
 //  set before importing it
 #include <Python.h>
-#include <arrow/python/platform.h>
-#include <arrow/api.h>
-#include <arrow/python/pyarrow.h>
-#include <arrow/python/api.h>
-#include <arrow/table.h>
 #include "Util/macros.hpp"
 
 namespace sf
 {
 
 namespace py
 {
```

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 //
 
 #ifndef PC_STRINGCONVERTER_HPP
 #define PC_STRINGCONVERTER_HPP
 
 #include "IColumnConverter.hpp"
 #include "logging.hpp"
+#include "nanoarrow.h"
+#include "nanoarrow.hpp"
 #include <memory>
 
 namespace sf
 {
 
 class StringConverter : public IColumnConverter
 {
 public:
-  explicit StringConverter(std::shared_ptr<arrow::Array> array);
-
+  explicit StringConverter(ArrowArrayView* array);
   PyObject* toPyObject(int64_t rowIndex) const override;
 
 private:
-  std::shared_ptr<arrow::StringArray> m_array;
+  ArrowArrayView* m_array;
 
   static Logger* logger;
 };
 
 }  // namespace sf
 
 #endif  // PC_STRINGCONVERTER_HPP
```

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/Logging/logging.cpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/Logging/logging.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/cpp/Logging/logging.hpp` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cpp/Logging/logging.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/cursor.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/cursor.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/dbapi.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/dbapi.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/encryption_util.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/encryption_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/errorcode.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/errorcode.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/errors.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -545,25 +545,14 @@
             msg=kwargs.get("msg") or "HTTP 429: Too Many Requests",
             errno=kwargs.get("errno"),
             sqlstate=kwargs.get("sqlstate"),
             sfqid=kwargs.get("sfqid"),
         )
 
 
-class RefreshTokenError(Error):
-    def __init__(self, **kwargs) -> None:
-        Error.__init__(
-            self,
-            msg=kwargs.get("msg") or "Token Refresh Required",
-            errno=kwargs.get("errno"),
-            sqlstate=kwargs.get("sqlstate"),
-            sfqid=kwargs.get("sfqid"),
-        )
-
-
 class OtherHTTPRetryableError(Error):
     """Exception for other HTTP error for retry."""
 
     def __init__(self, **kwargs) -> None:
         code = kwargs.get("code", "n/a")
         Error.__init__(
             self,
@@ -608,19 +597,12 @@
 class ConfigSourceError(Error):
     """Configuration source related errors.
 
     Examples are environmental variable and configuration file.
     """
 
 
-class MissingConfigOptionError(ConfigSourceError):
-    """When a configuration option is missing from the final, resolved configurations.
-
-    This is a special-case of ConfigSourceError.
-    """
-
-
 class ConfigManagerError(Error):
     """Configuration parser related errors.
 
     These mean that ConfigManager is misused by a developer.
     """
```

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/file_compression_type.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/file_compression_type.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/file_transfer_agent.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/file_transfer_agent.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/file_util.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/file_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/gcs_storage_client.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/gcs_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/gzip_decoder.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/gzip_decoder.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/local_storage_client.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/local_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/network.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,14 @@
     GatewayTimeoutError,
     InterfaceError,
     InternalServerError,
     MethodNotAllowed,
     OperationalError,
     OtherHTTPRetryableError,
     ProgrammingError,
-    RefreshTokenError,
     ServiceUnavailableError,
     TooManyRequests,
 )
 from .sqlstate import (
     SQLSTATE_CONNECTION_NOT_EXISTS,
     SQLSTATE_CONNECTION_REJECTED,
     SQLSTATE_CONNECTION_WAS_NOT_ESTABLISHED,
@@ -1051,15 +1050,14 @@
         data,
         token,
         catch_okta_unauthorized_error: bool = False,
         is_raw_text: bool = False,
         is_raw_binary: bool = False,
         binary_data_handler=None,
         socket_timeout=DEFAULT_SOCKET_CONNECT_TIMEOUT,
-        is_okta_authentication: bool = False,
     ):
         if socket_timeout > DEFAULT_SOCKET_CONNECT_TIMEOUT:
             # socket timeout should not be more than the default.
             # A shorter timeout may be specified for login time, but
             # for query, it should be at least 45 seconds.
             socket_timeout = DEFAULT_SOCKET_CONNECT_TIMEOUT
         logger.debug("socket timeout: %s", socket_timeout)
@@ -1102,18 +1100,14 @@
                 if is_login_request(full_url) and raw_ret.status_code == FORBIDDEN:
                     raise ForbiddenError
 
                 elif is_retryable_http_code(raw_ret.status_code):
                     error = get_http_retryable_error(raw_ret.status_code)
                     logger.debug(f"{error}. Retrying...")
                     # retryable server exceptions
-                    if is_okta_authentication:
-                        raise RefreshTokenError(
-                            msg="OKTA authentication requires token refresh."
-                        )
                     raise RetryRequest(error)
 
                 elif (
                     raw_ret.status_code == UNAUTHORIZED
                     and catch_okta_unauthorized_error
                 ):
                     # OKTA Unauthorized errors
```

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/ocsp_asn1crypto.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/ocsp_asn1crypto.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/ocsp_snowflake.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/ocsp_snowflake.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/options.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/options.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/pandas_tools.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/pandas_tools.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/proxy.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/result_batch.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/result_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #
 # Copyright (c) 2012-2023 Snowflake Computing Inc. All rights reserved.
 #
 
 from __future__ import annotations
 
 import abc
-import io
 import json
 import time
 from base64 import b64decode
 from enum import Enum, unique
 from logging import getLogger
 from typing import TYPE_CHECKING, Any, Iterator, NamedTuple, Sequence
 
@@ -565,15 +564,15 @@
         This is used to iterate through results in different ways depending on which
         mode that ``PyArrowIterator`` is in.
         """
         from .arrow_iterator import PyArrowIterator
 
         iter = PyArrowIterator(
             None,
-            io.BytesIO(response.content),
+            response.content,
             self._context,
             self._use_dict_result,
             self._numpy,
             self._number_to_decimal,
         )
         if row_unit == IterUnit.TABLE_UNIT:
             iter.init_table_unit()
@@ -591,15 +590,15 @@
         from .arrow_iterator import PyArrowIterator
 
         if len(data) == 0:
             return iter([])
 
         _iter = PyArrowIterator(
             None,
-            io.BytesIO(b64decode(data)),
+            b64decode(data),
             self._context,
             self._use_dict_result,
             self._numpy,
             self._number_to_decimal,
         )
         if iter_unit == IterUnit.TABLE_UNIT:
             _iter.init_table_unit()
```

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/result_set.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/result_set.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/s3_storage_client.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/s3_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/secret_detector.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/secret_detector.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/sf_dirs.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/sf_dirs.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/sfbinaryformat.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/sfbinaryformat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/sfdatetime.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/sfdatetime.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/snow_logging.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/snow_logging.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/ssd_internal_keys.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/ssd_internal_keys.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/ssl_wrap_socket.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/ssl_wrap_socket.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/storage_client.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/telemetry.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/telemetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     # Keys for telemetry data sent through either in-band or out-of-band telemetry
     KEY_TYPE = "type"
     KEY_SOURCE = "source"
     KEY_SFQID = "query_id"
     KEY_SQLSTATE = "sql_state"
     KEY_DRIVER_TYPE = "driver_type"
     KEY_DRIVER_VERSION = "driver_version"
+    KEY_IS_PRERELEASE = "is_prerelease"
     KEY_REASON = "reason"
     KEY_VALUE = "value"
     KEY_EXCEPTION = "exception"
     # Reserved UpperCamelName keys
     KEY_ERROR_NUMBER = "ErrorNumber"
     KEY_ERROR_MESSAGE = "ErrorMessage"
     KEY_STACKTRACE = "Stacktrace"
```

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/telemetry_oob.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/telemetry_oob.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/test_util.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/test_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/time_util.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/time_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/tool/dump_certs.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/tool/dump_certs.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/tool/dump_ocsp_response.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/tool/dump_ocsp_response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/tool/dump_ocsp_response_cache.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/tool/dump_ocsp_response_cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/tool/probe_connection.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/tool/probe_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/url_util.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/url_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/util_text.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/util_text.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/LICENSE` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/__init__.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/_internal_utils.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/adapters.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/api.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/api.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/auth.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/compat.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/cookies.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/exceptions.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/help.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/help.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/hooks.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/models.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/models.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/sessions.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/status_codes.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/structures.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/structures.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/requests/utils.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/requests/utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/LICENSE.txt` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/__init__.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/_collections.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/connection.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/connectionpool.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/contrib/appengine.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/contrib/socks.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/exceptions.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/fields.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/filepost.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/packages/six.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/poolmanager.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/request.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/response.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/__init__.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/connection.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/proxy.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/request.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/response.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/retry.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/ssl_.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/ssltransport.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/timeout.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/url.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake/connector/vendored/urllib3/util/wait.py` & `snowflake-connector-python-3.1.0a1/src/snowflake/connector/vendored/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-3.1.0/src/snowflake_connector_python.egg-info/PKG-INFO` & `snowflake-connector-python-3.1.0a1/src/snowflake_connector_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python
-Version: 3.1.0
+Version: 3.1.0a1
 Summary: Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/snowflakedb/snowflake-connector-python
 Project-URL: Issues, https://github.com/snowflakedb/snowflake-connector-python/issues
 Project-URL: Changelog, https://github.com/snowflakedb/snowflake-connector-python/blob/main/DESCRIPTION.md
 Keywords: Snowflake db database cloud analytics warehouse
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
@@ -47,51 +47,51 @@
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Source code is also available at: https://github.com/snowflakedb/snowflake-connector-python
 
 # Release Notes
 
-- v3.1.0(July 31,2023)
-
-  - Added a feature that lets you add connection definitions to the `connections.toml` configuration file. A connection definition refers to a collection of connection parameters, for example, if you wanted to define a connection named `prod``:
-
-    ```toml
-    [prod]
-    account = "my_account"
-    user = "my_user"
-    password = "my_password"
-    ```
-    By default, we look for the `connections.toml` file in the location specified in the `SNOWFLAKE_HOME` environment variable (default: `~/.snowflake`). If this folder does not exist, the Python connector looks for the file in the [platformdirs](https://github.com/platformdirs/platformdirs/blob/main/README.rst) location, as follows:
-
-    - On Linux: `~/.config/snowflake/`,  but follows XDG settings
-    - On Mac: `~/Library/Application Support/snowflake/`
-    - On Windows: `%USERPROFILE%\AppData\Local\snowflake\`
-
-    You can determine which file is used by running the following command:
-
-    ```
-    python -c "from snowflake.connector.constants import CONNECTIONS_FILE; print(str(CONNECTIONS_FILE))"
-    ```
-  - Bumped cryptography dependency from <41.0.0,>=3.1.0 to >=3.1.0,<42.0.0.
-  - Improved OCSP response caching to remove tmp cache files on Windows.
-  - Improved OCSP response caching to reduce the times of disk writing.
-  - Added a parameter `server_session_keep_alive` in `SnowflakeConnection` that skips session deletion when client connection closes.
-  - Tightened our pinning of platformdirs, to prevent their new releases breaking us.
-  - Fixed a bug where SFPlatformDirs would incorrectly append application_name/version to its path.
-  - Added retry reason for queries that are retried by the client.
-  - Fixed a bug where `write_pandas` fails when user does not have the privilege to create stage or file format in the target schema, but has the right privilege for the current schema.
-  - Remove Python 3.7 support.
-  - Worked around a segfault which sometimes occurred during cache serialization in multi-threaded scenarios.
-  - Improved error handling of connection reset error.
-  - Fixed a bug about deleting the temporary files happened when running PUT command.
-  - Allowed to pass `type_mapper` to `fetch_pandas_batches()` and `fetch_pandas_all()`.
-  - Fixed a bug where pickle.dump segfaults during cache serialization in multi-threaded scenarios.
-  - Improved retry logic for okta authentication to refresh token if authentication gets throttled.
-  - Note that this release does not include the changes introduced in the previous 3.1.0a1 release. Those will be released at a later time.
+- v3.1.0a1(July 24, 2023)
+  - Version 3.1.0a1 is our first efforts to build snowflake-connector-python based on apache nanoarrow project, which
+reduces the package size as well as removes a hard dependency on a specific version of pyarrow.
+  - This version also includes the following features and bug fixes from the unreleased v3.0.5:
+    - Added a feature that lets you add connection definitions to the `config.toml` configuration file. A connection definition refers to a collection of connection parameters. The connection configuration name must begin with **connections**, similar to the following that defines the parameters for the `prod` connection:
+
+      ```toml
+      [connections.prod]
+      account = "my_account"
+      user = "my_user"
+      password = "my_password"
+      ```
+      By default, we look for the `config.toml` file in the location specified in the `SNOWFLAKE_HOME` environment variable (default: `~/.snowflake`). If this folder does not exist, the Python connector looks for the file in the `platformdirs` location, as follows:
+
+      - On Linux: `~/.config/snowflake/`,  but follows XDG settings
+      - On Mac: `~/Library/Application Support/snowflake/`
+      - On Windows: `%USERPROFILE%\AppData\Local\snowflake\`
+
+      You can determine which file is used by running the following command:
+
+      ```
+      python -c "from snowflake.connector.constants import CONFIG_FILE; print(str(CONFIG_FILE))"
+      ```
+    - Bumped cryptography dependency from <41.0.0,>=3.1.0 to >=3.1.0,<42.0.0.
+    - Improved OCSP response caching to remove tmp cache files on Windows.
+    - Improved OCSP response caching to reduce the times of disk writing.
+    - Added a parameter `server_session_keep_alive` in `SnowflakeConnection` that skips session deletion when client connection closes.
+    - Tightened our pinning of platformdirs, to prevent their new releases breaking us.
+    - Fixed a bug where SFPlatformDirs would incorrectly append application_name/version to its path.
+    - Added retry reason for queries that are retried by the client.
+    - Fixed a bug where `write_pandas` fails when user does not have the privilege to create stage or file format in the target schema, but has the right privilege for the current schema.
+    - Remove Python 3.7 support.
+    - Worked around a segfault which sometimes occurred during cache serialization in multi-threaded scenarios.
+    - Improved error handling of connection reset error.
+    - Fixed a bug about deleting the temporary files happened when running PUT command.
+    - Allowed to pass `type_mapper` to `fetch_pandas_batches()` and `fetch_pandas_all()`.
+    - Fixed a bug where pickle.dump segfaults during cache serialization in multi-threaded scenarios.
 
 - v3.0.4(May 23,2023)
   - Fixed a bug in which `cursor.execute()` could modify the argument statement_params dictionary object when executing a multistatement query.
   - Added the json_result_force_utf8_decoding connection parameter to force decoding JSON content in utf-8 when the result format is JSON.
   - Fixed a bug in which we cannot call `SnowflakeCursor.nextset` before fetching the result of the first query if the cursor runs an async multistatement query.
   - Bumped vendored library urllib3 to 1.26.15
   - Bumped vendored library requests to 2.29.0
```

### Comparing `snowflake-connector-python-3.1.0/src/snowflake_connector_python.egg-info/requires.txt` & `snowflake-connector-python-3.1.0a1/src/snowflake_connector_python.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -24,20 +24,20 @@
 [development]
 Cython
 coverage
 more-itertools
 numpy<1.26.0
 pendulum!=2.1.1
 pexpect
-pytest<7.5.0
+pytest<7.4.0
 pytest-cov
 pytest-rerunfailures
 pytest-timeout
 pytest-xdist
 pytzdata
 
 [pandas]
 pandas<2.1.0,>=1.0.0
-pyarrow<10.1.0,>=10.0.1
+pyarrow
 
 [secure-local-storage]
 keyring!=16.1.0,<25.0.0
```

