# Comparing `tmp/retakesearch-py-2.2.1.tar.gz` & `tmp/retakesearch-py-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retakesearch-py-2.2.1.tar", last modified: Thu Jul 27 03:19:32 2023, max compression
+gzip compressed data, was "retakesearch-py-2.2.2.tar", last modified: Mon Jul 31 22:54:28 2023, max compression
```

## Comparing `retakesearch-py-2.2.1.tar` & `retakesearch-py-2.2.2.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-27 03:19:32.218800 retakesearch-py-2.2.1/
--rw-r--r--   0 mingying   (501) staff       (20)      144 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/AUTHORS
--rw-r--r--   0 mingying   (501) staff       (20)     8426 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/CONTRIBUTING.md
--rw-r--r--   0 mingying   (501) staff       (20)    11356 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/LICENSE.txt
--rw-r--r--   0 mingying   (501) staff       (20)      262 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/MANIFEST.in
--rw-r--r--   0 mingying   (501) staff       (20)      257 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/NOTICE.txt
--rw-r--r--   0 mingying   (501) staff       (20)     5636 2023-07-27 03:19:32.218893 retakesearch-py-2.2.1/PKG-INFO
--rw-r--r--   0 mingying   (501) staff       (20)     3792 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/README.md
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-27 03:19:32.187542 retakesearch-py-2.2.1/opensearchpy/
--rw-r--r--   0 mingying   (501) staff       (20)     6160 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)     6727 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/__init__.pyi
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-27 03:19:32.189344 retakesearch-py-2.2.1/opensearchpy/_async/
--rw-r--r--   0 mingying   (501) staff       (20)     1068 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)     2006 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/_extra_imports.py
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-27 03:19:32.194305 retakesearch-py-2.2.1/opensearchpy/_async/client/
--rw-r--r--   0 mingying   (501) staff       (20)    85442 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)    47018 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/__init__.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    29940 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/cat.py
--rw-r--r--   0 mingying   (501) staff       (20)    22836 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/cat.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    17123 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/cluster.py
--rw-r--r--   0 mingying   (501) staff       (20)    14830 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/cluster.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     3410 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/dangling_indices.py
--rw-r--r--   0 mingying   (501) staff       (20)     3762 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/dangling_indices.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     2294 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/features.py
--rw-r--r--   0 mingying   (501) staff       (20)     2715 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/features.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    70997 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/indices.py
--rw-r--r--   0 mingying   (501) staff       (20)    53603 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/indices.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     5076 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/ingest.py
--rw-r--r--   0 mingying   (501) staff       (20)     5984 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/ingest.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     7921 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/nodes.py
--rw-r--r--   0 mingying   (501) staff       (20)     5859 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/nodes.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     1967 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/plugins.py
--rw-r--r--   0 mingying   (501) staff       (20)      623 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/plugins.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     1363 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/remote.py
--rw-r--r--   0 mingying   (501) staff       (20)     1793 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/remote.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    15136 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/snapshot.py
--rw-r--r--   0 mingying   (501) staff       (20)    12322 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/snapshot.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     4976 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/tasks.py
--rw-r--r--   0 mingying   (501) staff       (20)     3902 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/tasks.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     1235 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/utils.py
--rw-r--r--   0 mingying   (501) staff       (20)     1660 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/client/utils.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     1715 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/compat.py
--rw-r--r--   0 mingying   (501) staff       (20)     1142 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/compat.pyi
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-27 03:19:32.197034 retakesearch-py-2.2.1/opensearchpy/_async/helpers/
--rw-r--r--   0 mingying   (501) staff       (20)      279 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/helpers/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)    17605 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/helpers/actions.py
--rw-r--r--   0 mingying   (501) staff       (20)     3705 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/helpers/actions.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    16308 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/helpers/document.py
--rw-r--r--   0 mingying   (501) staff       (20)      463 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/helpers/document.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     5956 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/helpers/faceted_search.py
--rw-r--r--   0 mingying   (501) staff       (20)      318 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/helpers/faceted_search.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    23606 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/helpers/index.py
--rw-r--r--   0 mingying   (501) staff       (20)      348 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/helpers/index.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     5472 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/helpers/mapping.py
--rw-r--r--   0 mingying   (501) staff       (20)      312 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/helpers/mapping.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    17058 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/helpers/search.py
--rw-r--r--   0 mingying   (501) staff       (20)      398 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/helpers/search.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     1314 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/helpers/test.py
--rw-r--r--   0 mingying   (501) staff       (20)      571 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/helpers/test.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     4675 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/helpers/update_by_query.py
--rw-r--r--   0 mingying   (501) staff       (20)      368 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/helpers/update_by_query.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    14193 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/http_aiohttp.py
--rw-r--r--   0 mingying   (501) staff       (20)     2621 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/http_aiohttp.pyi
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-27 03:19:32.198238 retakesearch-py-2.2.1/opensearchpy/_async/plugins/
--rw-r--r--   0 mingying   (501) staff       (20)      279 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/plugins/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)      279 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/plugins/__init__.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     6548 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/plugins/alerting.py
--rw-r--r--   0 mingying   (501) staff       (20)     2619 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/plugins/alerting.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     4959 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/plugins/index_management.py
--rw-r--r--   0 mingying   (501) staff       (20)     2036 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/plugins/index_management.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    21802 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/plugins/security.py
--rw-r--r--   0 mingying   (501) staff       (20)     7330 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/plugins/security.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    18066 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/transport.py
--rw-r--r--   0 mingying   (501) staff       (20)     3390 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/_async/transport.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     1094 2023-07-27 03:19:20.000000 retakesearch-py-2.2.1/opensearchpy/_version.py
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-27 03:19:32.204413 retakesearch-py-2.2.1/opensearchpy/client/
--rw-r--r--   0 mingying   (501) staff       (20)    84926 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)    46696 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/__init__.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    29568 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/cat.py
--rw-r--r--   0 mingying   (501) staff       (20)    22704 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/cat.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    16943 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/cluster.py
--rw-r--r--   0 mingying   (501) staff       (20)    14740 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/cluster.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     3374 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/dangling_indices.py
--rw-r--r--   0 mingying   (501) staff       (20)     3744 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/dangling_indices.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     2270 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/features.py
--rw-r--r--   0 mingying   (501) staff       (20)     2703 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/features.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    71619 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/indices.py
--rw-r--r--   0 mingying   (501) staff       (20)    53267 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/indices.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     5004 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/ingest.py
--rw-r--r--   0 mingying   (501) staff       (20)     5948 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/ingest.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     7861 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/nodes.py
--rw-r--r--   0 mingying   (501) staff       (20)     5829 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/nodes.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     2020 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/plugins.py
--rw-r--r--   0 mingying   (501) staff       (20)      613 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/plugins.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     1351 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/remote.py
--rw-r--r--   0 mingying   (501) staff       (20)     1787 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/remote.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    14992 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/snapshot.py
--rw-r--r--   0 mingying   (501) staff       (20)    12250 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/snapshot.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     4940 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/tasks.py
--rw-r--r--   0 mingying   (501) staff       (20)     3884 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/tasks.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     6925 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/utils.py
--rw-r--r--   0 mingying   (501) staff       (20)     1988 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/client/utils.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     2403 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/compat.py
--rw-r--r--   0 mingying   (501) staff       (20)     1941 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/compat.pyi
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-27 03:19:32.207559 retakesearch-py-2.2.1/opensearchpy/connection/
--rw-r--r--   0 mingying   (501) staff       (20)     1605 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/connection/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)     1395 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/connection/__init__.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     3813 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/connection/async_connections.py
--rw-r--r--   0 mingying   (501) staff       (20)      308 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/connection/async_connections.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    11045 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/connection/base.py
--rw-r--r--   0 mingying   (501) staff       (20)     3514 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/connection/base.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     4419 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/connection/connections.py
--rw-r--r--   0 mingying   (501) staff       (20)     1154 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/connection/connections.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    10568 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/connection/http_async.py
--rw-r--r--   0 mingying   (501) staff       (20)     1267 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/connection/http_async.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     8719 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/connection/http_requests.py
--rw-r--r--   0 mingying   (501) staff       (20)     1761 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/connection/http_requests.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    10657 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/connection/http_urllib3.py
--rw-r--r--   0 mingying   (501) staff       (20)     2191 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/connection/http_urllib3.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     2048 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/connection/pooling.py
--rw-r--r--   0 mingying   (501) staff       (20)     1332 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/connection/pooling.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    11778 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/connection_pool.py
--rw-r--r--   0 mingying   (501) staff       (20)     3198 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/connection_pool.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     5960 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/exceptions.py
--rw-r--r--   0 mingying   (501) staff       (20)     2275 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/exceptions.pyi
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-27 03:19:32.214740 retakesearch-py-2.2.1/opensearchpy/helpers/
--rw-r--r--   0 mingying   (501) staff       (20)     1929 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)     2139 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/__init__.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    24406 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/actions.py
--rw-r--r--   0 mingying   (501) staff       (20)     4186 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/actions.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     9849 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/aggs.py
--rw-r--r--   0 mingying   (501) staff       (20)     3487 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/aggs.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     8525 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/analysis.py
--rw-r--r--   0 mingying   (501) staff       (20)     2161 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/analysis.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     1866 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/asyncsigner.py
--rw-r--r--   0 mingying   (501) staff       (20)      595 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/asyncsigner.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    18613 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/document.py
--rw-r--r--   0 mingying   (501) staff       (20)     1347 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/document.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     1487 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/errors.py
--rw-r--r--   0 mingying   (501) staff       (20)     1378 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/errors.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    13797 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/faceted_search.py
--rw-r--r--   0 mingying   (501) staff       (20)     1374 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/faceted_search.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    14196 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/field.py
--rw-r--r--   0 mingying   (501) staff       (20)     2257 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/field.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     3857 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/function.py
--rw-r--r--   0 mingying   (501) staff       (20)     1459 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/function.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    22993 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/index.py
--rw-r--r--   0 mingying   (501) staff       (20)     1127 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/index.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     7960 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/mapping.py
--rw-r--r--   0 mingying   (501) staff       (20)     1155 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/mapping.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    12634 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/query.py
--rw-r--r--   0 mingying   (501) staff       (20)     2952 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/query.pyi
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-27 03:19:32.215886 retakesearch-py-2.2.1/opensearchpy/helpers/response/
--rw-r--r--   0 mingying   (501) staff       (20)     4409 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/response/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)     1205 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/response/__init__.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     2946 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/response/aggs.py
--rw-r--r--   0 mingying   (501) staff       (20)     1315 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/response/aggs.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     2161 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/response/hit.py
--rw-r--r--   0 mingying   (501) staff       (20)     1124 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/response/hit.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    27416 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/search.py
--rw-r--r--   0 mingying   (501) staff       (20)     1313 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/search.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     2900 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/signer.py
--rw-r--r--   0 mingying   (501) staff       (20)     3459 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/test.py
--rw-r--r--   0 mingying   (501) staff       (20)     1579 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/test.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     5344 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/update_by_query.py
--rw-r--r--   0 mingying   (501) staff       (20)     1132 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/update_by_query.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    19065 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/utils.py
--rw-r--r--   0 mingying   (501) staff       (20)     1238 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/utils.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     2868 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/wrappers.py
--rw-r--r--   0 mingying   (501) staff       (20)     1125 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/helpers/wrappers.pyi
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-27 03:19:32.217464 retakesearch-py-2.2.1/opensearchpy/plugins/
--rw-r--r--   0 mingying   (501) staff       (20)      281 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/plugins/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)      279 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/plugins/__init__.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     6391 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/plugins/alerting.py
--rw-r--r--   0 mingying   (501) staff       (20)     2396 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/plugins/alerting.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     4863 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/plugins/index_management.py
--rw-r--r--   0 mingying   (501) staff       (20)     1988 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/plugins/index_management.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    21208 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/plugins/security.py
--rw-r--r--   0 mingying   (501) staff       (20)     7652 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/plugins/security.pyi
--rw-r--r--   0 mingying   (501) staff       (20)        0 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/py.typed
--rw-r--r--   0 mingying   (501) staff       (20)     6226 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/serializer.py
--rw-r--r--   0 mingying   (501) staff       (20)     1876 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/serializer.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    18470 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/transport.py
--rw-r--r--   0 mingying   (501) staff       (20)     3507 2023-07-23 18:55:25.000000 retakesearch-py-2.2.1/opensearchpy/transport.pyi
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-27 03:19:32.218616 retakesearch-py-2.2.1/retakesearch_py.egg-info/
--rw-r--r--   0 mingying   (501) staff       (20)     5636 2023-07-27 03:19:32.000000 retakesearch-py-2.2.1/retakesearch_py.egg-info/PKG-INFO
--rw-r--r--   0 mingying   (501) staff       (20)     6173 2023-07-27 03:19:32.000000 retakesearch-py-2.2.1/retakesearch_py.egg-info/SOURCES.txt
--rw-r--r--   0 mingying   (501) staff       (20)        1 2023-07-27 03:19:32.000000 retakesearch-py-2.2.1/retakesearch_py.egg-info/dependency_links.txt
--rw-r--r--   0 mingying   (501) staff       (20)        1 2023-07-23 18:56:34.000000 retakesearch-py-2.2.1/retakesearch_py.egg-info/not-zip-safe
--rw-r--r--   0 mingying   (501) staff       (20)      454 2023-07-27 03:19:32.000000 retakesearch-py-2.2.1/retakesearch_py.egg-info/requires.txt
--rw-r--r--   0 mingying   (501) staff       (20)       13 2023-07-27 03:19:32.000000 retakesearch-py-2.2.1/retakesearch_py.egg-info/top_level.txt
--rw-r--r--   0 mingying   (501) staff       (20)      280 2023-07-27 03:19:32.219206 retakesearch-py-2.2.1/setup.cfg
--rw-r--r--   0 mingying   (501) staff       (20)     4775 2023-07-27 03:09:44.000000 retakesearch-py-2.2.1/setup.py
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-31 22:54:28.983155 retakesearch-py-2.2.2/
+-rw-r--r--   0 mingying   (501) staff       (20)      144 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/AUTHORS
+-rw-r--r--   0 mingying   (501) staff       (20)     8426 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/CONTRIBUTING.md
+-rw-r--r--   0 mingying   (501) staff       (20)    11356 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/LICENSE.txt
+-rw-r--r--   0 mingying   (501) staff       (20)      262 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/MANIFEST.in
+-rw-r--r--   0 mingying   (501) staff       (20)      257 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/NOTICE.txt
+-rw-r--r--   0 mingying   (501) staff       (20)     5636 2023-07-31 22:54:28.983227 retakesearch-py-2.2.2/PKG-INFO
+-rw-r--r--   0 mingying   (501) staff       (20)     3792 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/README.md
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-31 22:54:28.954082 retakesearch-py-2.2.2/opensearchpy/
+-rw-r--r--   0 mingying   (501) staff       (20)     6160 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)     6727 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/__init__.pyi
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-31 22:54:28.955866 retakesearch-py-2.2.2/opensearchpy/_async/
+-rw-r--r--   0 mingying   (501) staff       (20)     1068 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2006 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/_extra_imports.py
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-31 22:54:28.961480 retakesearch-py-2.2.2/opensearchpy/_async/client/
+-rw-r--r--   0 mingying   (501) staff       (20)    85442 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)    47018 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/__init__.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    29940 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/cat.py
+-rw-r--r--   0 mingying   (501) staff       (20)    22836 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/cat.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    17123 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/cluster.py
+-rw-r--r--   0 mingying   (501) staff       (20)    14830 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/cluster.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     3410 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/dangling_indices.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3762 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/dangling_indices.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     2294 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/features.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2715 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/features.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    70997 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/indices.py
+-rw-r--r--   0 mingying   (501) staff       (20)    53603 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/indices.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     5076 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/ingest.py
+-rw-r--r--   0 mingying   (501) staff       (20)     5984 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/ingest.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     7921 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/nodes.py
+-rw-r--r--   0 mingying   (501) staff       (20)     5859 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/nodes.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     1967 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/plugins.py
+-rw-r--r--   0 mingying   (501) staff       (20)      623 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/plugins.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     1363 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/remote.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1793 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/remote.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    15136 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/snapshot.py
+-rw-r--r--   0 mingying   (501) staff       (20)    12322 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/snapshot.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     4976 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/tasks.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3902 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/tasks.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     1235 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/utils.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1660 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/client/utils.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     1715 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/compat.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1142 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/compat.pyi
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-31 22:54:28.965054 retakesearch-py-2.2.2/opensearchpy/_async/helpers/
+-rw-r--r--   0 mingying   (501) staff       (20)      279 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/helpers/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)    17605 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/helpers/actions.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3705 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/helpers/actions.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    16308 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/helpers/document.py
+-rw-r--r--   0 mingying   (501) staff       (20)      463 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/helpers/document.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     5956 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/helpers/faceted_search.py
+-rw-r--r--   0 mingying   (501) staff       (20)      318 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/helpers/faceted_search.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    23606 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/helpers/index.py
+-rw-r--r--   0 mingying   (501) staff       (20)      348 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/helpers/index.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     5472 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/helpers/mapping.py
+-rw-r--r--   0 mingying   (501) staff       (20)      312 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/helpers/mapping.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    17058 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/helpers/search.py
+-rw-r--r--   0 mingying   (501) staff       (20)      398 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/helpers/search.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     1314 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/helpers/test.py
+-rw-r--r--   0 mingying   (501) staff       (20)      571 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/helpers/test.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     4675 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/helpers/update_by_query.py
+-rw-r--r--   0 mingying   (501) staff       (20)      368 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/helpers/update_by_query.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    14193 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/http_aiohttp.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2621 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/http_aiohttp.pyi
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-31 22:54:28.966434 retakesearch-py-2.2.2/opensearchpy/_async/plugins/
+-rw-r--r--   0 mingying   (501) staff       (20)      279 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/plugins/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)      279 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/plugins/__init__.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     6548 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/plugins/alerting.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2619 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/plugins/alerting.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     4959 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/plugins/index_management.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2036 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/plugins/index_management.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    21802 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/plugins/security.py
+-rw-r--r--   0 mingying   (501) staff       (20)     7330 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/plugins/security.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    18066 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/transport.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3390 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/_async/transport.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     1094 2023-07-31 22:52:15.000000 retakesearch-py-2.2.2/opensearchpy/_version.py
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-31 22:54:28.971421 retakesearch-py-2.2.2/opensearchpy/client/
+-rw-r--r--   0 mingying   (501) staff       (20)    84926 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)    46696 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/__init__.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    29568 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/cat.py
+-rw-r--r--   0 mingying   (501) staff       (20)    22704 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/cat.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    16943 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/cluster.py
+-rw-r--r--   0 mingying   (501) staff       (20)    14740 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/cluster.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     3374 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/dangling_indices.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3744 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/dangling_indices.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     2270 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/features.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2703 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/features.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    71619 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/indices.py
+-rw-r--r--   0 mingying   (501) staff       (20)    53267 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/indices.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     5004 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/ingest.py
+-rw-r--r--   0 mingying   (501) staff       (20)     5948 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/ingest.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     7861 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/nodes.py
+-rw-r--r--   0 mingying   (501) staff       (20)     5829 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/nodes.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     2020 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/plugins.py
+-rw-r--r--   0 mingying   (501) staff       (20)      613 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/plugins.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     1351 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/remote.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1787 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/remote.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    14992 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/snapshot.py
+-rw-r--r--   0 mingying   (501) staff       (20)    12250 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/snapshot.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     4940 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/tasks.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3884 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/tasks.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     6925 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/utils.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1988 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/client/utils.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     2403 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/compat.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1941 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/compat.pyi
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-31 22:54:28.973851 retakesearch-py-2.2.2/opensearchpy/connection/
+-rw-r--r--   0 mingying   (501) staff       (20)     1605 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/connection/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1395 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/connection/__init__.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     3813 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/connection/async_connections.py
+-rw-r--r--   0 mingying   (501) staff       (20)      308 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/connection/async_connections.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    11045 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/connection/base.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3514 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/connection/base.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     4419 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/connection/connections.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1154 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/connection/connections.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    10568 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/connection/http_async.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1267 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/connection/http_async.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     8719 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/connection/http_requests.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1761 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/connection/http_requests.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    10657 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/connection/http_urllib3.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2191 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/connection/http_urllib3.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     2048 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/connection/pooling.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1332 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/connection/pooling.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    11778 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/connection_pool.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3198 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/connection_pool.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     5960 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/exceptions.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2275 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/exceptions.pyi
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-31 22:54:28.979907 retakesearch-py-2.2.2/opensearchpy/helpers/
+-rw-r--r--   0 mingying   (501) staff       (20)     1929 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2139 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/__init__.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    24406 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/actions.py
+-rw-r--r--   0 mingying   (501) staff       (20)     4186 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/actions.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     9849 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/aggs.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3487 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/aggs.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     8525 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/analysis.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2161 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/analysis.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     1866 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/asyncsigner.py
+-rw-r--r--   0 mingying   (501) staff       (20)      595 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/asyncsigner.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    18613 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/document.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1347 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/document.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     1487 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/errors.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1378 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/errors.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    13797 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/faceted_search.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1374 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/faceted_search.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    14196 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/field.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2257 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/field.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     3857 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/function.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1459 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/function.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    22993 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/index.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1127 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/index.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     7960 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/mapping.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1155 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/mapping.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    12634 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/query.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2952 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/query.pyi
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-31 22:54:28.980826 retakesearch-py-2.2.2/opensearchpy/helpers/response/
+-rw-r--r--   0 mingying   (501) staff       (20)     4409 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/response/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1205 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/response/__init__.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     2946 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/response/aggs.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1315 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/response/aggs.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     2161 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/response/hit.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1124 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/response/hit.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    27292 2023-07-31 22:41:20.000000 retakesearch-py-2.2.2/opensearchpy/helpers/search.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1313 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/search.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     2900 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/signer.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3459 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/test.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1579 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/test.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     5344 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/update_by_query.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1132 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/update_by_query.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    19065 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/utils.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1238 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/utils.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     2868 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/wrappers.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1125 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/helpers/wrappers.pyi
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-31 22:54:28.982118 retakesearch-py-2.2.2/opensearchpy/plugins/
+-rw-r--r--   0 mingying   (501) staff       (20)      281 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/plugins/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)      279 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/plugins/__init__.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     6391 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/plugins/alerting.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2396 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/plugins/alerting.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     4863 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/plugins/index_management.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1988 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/plugins/index_management.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    21208 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/plugins/security.py
+-rw-r--r--   0 mingying   (501) staff       (20)     7652 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/plugins/security.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)        0 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/py.typed
+-rw-r--r--   0 mingying   (501) staff       (20)     6226 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/serializer.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1876 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/serializer.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    18470 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/transport.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3507 2023-07-23 18:55:25.000000 retakesearch-py-2.2.2/opensearchpy/transport.pyi
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-31 22:54:28.983037 retakesearch-py-2.2.2/retakesearch_py.egg-info/
+-rw-r--r--   0 mingying   (501) staff       (20)     5636 2023-07-31 22:54:28.000000 retakesearch-py-2.2.2/retakesearch_py.egg-info/PKG-INFO
+-rw-r--r--   0 mingying   (501) staff       (20)     6173 2023-07-31 22:54:28.000000 retakesearch-py-2.2.2/retakesearch_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mingying   (501) staff       (20)        1 2023-07-31 22:54:28.000000 retakesearch-py-2.2.2/retakesearch_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mingying   (501) staff       (20)        1 2023-07-23 18:56:34.000000 retakesearch-py-2.2.2/retakesearch_py.egg-info/not-zip-safe
+-rw-r--r--   0 mingying   (501) staff       (20)      454 2023-07-31 22:54:28.000000 retakesearch-py-2.2.2/retakesearch_py.egg-info/requires.txt
+-rw-r--r--   0 mingying   (501) staff       (20)       13 2023-07-31 22:54:28.000000 retakesearch-py-2.2.2/retakesearch_py.egg-info/top_level.txt
+-rw-r--r--   0 mingying   (501) staff       (20)      280 2023-07-31 22:54:28.983492 retakesearch-py-2.2.2/setup.cfg
+-rw-r--r--   0 mingying   (501) staff       (20)     4775 2023-07-31 22:41:58.000000 retakesearch-py-2.2.2/setup.py
```

### Comparing `retakesearch-py-2.2.1/CONTRIBUTING.md` & `retakesearch-py-2.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/LICENSE.txt` & `retakesearch-py-2.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/PKG-INFO` & `retakesearch-py-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retakesearch-py
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python client for OpenSearch
 Home-page: https://github.com/opensearch-project/opensearch-py
 Author: Aleksei Atavin, Denis Zalevskiy, Rushi Agrawal, Shephali Mittal
 Author-email: axeo@aiven.io, dez@aiven.io, rushi.agr@gmail.com, shephalm@amazon.com
 Maintainer: Aleksei Atavin, Denis Zalevskiy, Rushi Agrawal, Shephali Mittal
 Maintainer-email: axeo@aiven.io, dez@aiven.io, rushi.agr@gmail.com, shephalm@amazon.com
 License: Apache-2.0
```

### Comparing `retakesearch-py-2.2.1/README.md` & `retakesearch-py-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/__init__.py` & `retakesearch-py-2.2.2/opensearchpy/__init__.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/__init__.pyi` & `retakesearch-py-2.2.2/opensearchpy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/__init__.py` & `retakesearch-py-2.2.2/opensearchpy/_async/__init__.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/_extra_imports.py` & `retakesearch-py-2.2.2/opensearchpy/_async/_extra_imports.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/__init__.py` & `retakesearch-py-2.2.2/opensearchpy/_async/client/__init__.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/__init__.pyi` & `retakesearch-py-2.2.2/opensearchpy/_async/client/__init__.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/cat.py` & `retakesearch-py-2.2.2/opensearchpy/_async/client/cat.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/cat.pyi` & `retakesearch-py-2.2.2/opensearchpy/_async/client/cat.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/cluster.py` & `retakesearch-py-2.2.2/opensearchpy/_async/client/cluster.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/cluster.pyi` & `retakesearch-py-2.2.2/opensearchpy/_async/client/cluster.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/dangling_indices.py` & `retakesearch-py-2.2.2/opensearchpy/_async/client/dangling_indices.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/dangling_indices.pyi` & `retakesearch-py-2.2.2/opensearchpy/_async/client/dangling_indices.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/features.py` & `retakesearch-py-2.2.2/opensearchpy/_async/client/features.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/features.pyi` & `retakesearch-py-2.2.2/opensearchpy/_async/client/features.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/indices.py` & `retakesearch-py-2.2.2/opensearchpy/_async/client/indices.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/indices.pyi` & `retakesearch-py-2.2.2/opensearchpy/_async/client/indices.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/ingest.py` & `retakesearch-py-2.2.2/opensearchpy/_async/client/ingest.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/ingest.pyi` & `retakesearch-py-2.2.2/opensearchpy/_async/client/ingest.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/nodes.py` & `retakesearch-py-2.2.2/opensearchpy/_async/client/nodes.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/nodes.pyi` & `retakesearch-py-2.2.2/opensearchpy/_async/client/nodes.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/plugins.py` & `retakesearch-py-2.2.2/opensearchpy/_async/client/plugins.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/plugins.pyi` & `retakesearch-py-2.2.2/opensearchpy/_async/client/plugins.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/remote.py` & `retakesearch-py-2.2.2/opensearchpy/_async/client/remote.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/remote.pyi` & `retakesearch-py-2.2.2/opensearchpy/_async/client/remote.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/snapshot.py` & `retakesearch-py-2.2.2/opensearchpy/_async/client/snapshot.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/snapshot.pyi` & `retakesearch-py-2.2.2/opensearchpy/_async/client/snapshot.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/tasks.py` & `retakesearch-py-2.2.2/opensearchpy/_async/client/tasks.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/tasks.pyi` & `retakesearch-py-2.2.2/opensearchpy/_async/client/tasks.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/utils.py` & `retakesearch-py-2.2.2/opensearchpy/_async/client/utils.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/client/utils.pyi` & `retakesearch-py-2.2.2/opensearchpy/_async/client/utils.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/compat.py` & `retakesearch-py-2.2.2/opensearchpy/_async/compat.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/compat.pyi` & `retakesearch-py-2.2.2/opensearchpy/_async/compat.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/helpers/actions.py` & `retakesearch-py-2.2.2/opensearchpy/_async/helpers/actions.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/helpers/actions.pyi` & `retakesearch-py-2.2.2/opensearchpy/_async/helpers/actions.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/helpers/document.py` & `retakesearch-py-2.2.2/opensearchpy/_async/helpers/document.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/helpers/faceted_search.py` & `retakesearch-py-2.2.2/opensearchpy/_async/helpers/faceted_search.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/helpers/index.py` & `retakesearch-py-2.2.2/opensearchpy/_async/helpers/index.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/helpers/mapping.py` & `retakesearch-py-2.2.2/opensearchpy/_async/helpers/mapping.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/helpers/search.py` & `retakesearch-py-2.2.2/opensearchpy/_async/helpers/search.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/helpers/test.py` & `retakesearch-py-2.2.2/opensearchpy/_async/helpers/test.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/helpers/test.pyi` & `retakesearch-py-2.2.2/opensearchpy/_async/helpers/test.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/helpers/update_by_query.py` & `retakesearch-py-2.2.2/opensearchpy/_async/helpers/update_by_query.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/http_aiohttp.py` & `retakesearch-py-2.2.2/opensearchpy/_async/http_aiohttp.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/http_aiohttp.pyi` & `retakesearch-py-2.2.2/opensearchpy/_async/http_aiohttp.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/plugins/alerting.py` & `retakesearch-py-2.2.2/opensearchpy/_async/plugins/alerting.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/plugins/alerting.pyi` & `retakesearch-py-2.2.2/opensearchpy/_async/plugins/alerting.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/plugins/index_management.py` & `retakesearch-py-2.2.2/opensearchpy/_async/plugins/index_management.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/plugins/index_management.pyi` & `retakesearch-py-2.2.2/opensearchpy/_async/plugins/index_management.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/plugins/security.py` & `retakesearch-py-2.2.2/opensearchpy/_async/plugins/security.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/plugins/security.pyi` & `retakesearch-py-2.2.2/opensearchpy/_async/plugins/security.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/transport.py` & `retakesearch-py-2.2.2/opensearchpy/_async/transport.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_async/transport.pyi` & `retakesearch-py-2.2.2/opensearchpy/_async/transport.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/_version.py` & `retakesearch-py-2.2.2/opensearchpy/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
-__versionstr__ = "2.2.1"
+__versionstr__ = "2.2.2"
```

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/__init__.py` & `retakesearch-py-2.2.2/opensearchpy/client/__init__.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/__init__.pyi` & `retakesearch-py-2.2.2/opensearchpy/client/__init__.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/cat.py` & `retakesearch-py-2.2.2/opensearchpy/client/cat.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/cat.pyi` & `retakesearch-py-2.2.2/opensearchpy/client/cat.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/cluster.py` & `retakesearch-py-2.2.2/opensearchpy/client/cluster.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/cluster.pyi` & `retakesearch-py-2.2.2/opensearchpy/client/cluster.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/dangling_indices.py` & `retakesearch-py-2.2.2/opensearchpy/client/dangling_indices.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/dangling_indices.pyi` & `retakesearch-py-2.2.2/opensearchpy/client/dangling_indices.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/features.py` & `retakesearch-py-2.2.2/opensearchpy/client/features.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/features.pyi` & `retakesearch-py-2.2.2/opensearchpy/client/features.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/indices.py` & `retakesearch-py-2.2.2/opensearchpy/client/indices.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/indices.pyi` & `retakesearch-py-2.2.2/opensearchpy/client/indices.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/ingest.py` & `retakesearch-py-2.2.2/opensearchpy/client/ingest.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/ingest.pyi` & `retakesearch-py-2.2.2/opensearchpy/client/ingest.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/nodes.py` & `retakesearch-py-2.2.2/opensearchpy/client/nodes.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/nodes.pyi` & `retakesearch-py-2.2.2/opensearchpy/client/nodes.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/plugins.py` & `retakesearch-py-2.2.2/opensearchpy/client/plugins.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/plugins.pyi` & `retakesearch-py-2.2.2/opensearchpy/client/plugins.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/remote.py` & `retakesearch-py-2.2.2/opensearchpy/client/remote.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/remote.pyi` & `retakesearch-py-2.2.2/opensearchpy/client/remote.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/snapshot.py` & `retakesearch-py-2.2.2/opensearchpy/client/snapshot.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/snapshot.pyi` & `retakesearch-py-2.2.2/opensearchpy/client/snapshot.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/tasks.py` & `retakesearch-py-2.2.2/opensearchpy/client/tasks.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/tasks.pyi` & `retakesearch-py-2.2.2/opensearchpy/client/tasks.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/utils.py` & `retakesearch-py-2.2.2/opensearchpy/client/utils.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/client/utils.pyi` & `retakesearch-py-2.2.2/opensearchpy/client/utils.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/compat.py` & `retakesearch-py-2.2.2/opensearchpy/compat.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/compat.pyi` & `retakesearch-py-2.2.2/opensearchpy/compat.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/connection/__init__.py` & `retakesearch-py-2.2.2/opensearchpy/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/connection/__init__.pyi` & `retakesearch-py-2.2.2/opensearchpy/connection/__init__.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/connection/async_connections.py` & `retakesearch-py-2.2.2/opensearchpy/connection/async_connections.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/connection/base.py` & `retakesearch-py-2.2.2/opensearchpy/connection/base.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/connection/base.pyi` & `retakesearch-py-2.2.2/opensearchpy/connection/base.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/connection/connections.py` & `retakesearch-py-2.2.2/opensearchpy/connection/connections.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/connection/connections.pyi` & `retakesearch-py-2.2.2/opensearchpy/connection/connections.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/connection/http_async.py` & `retakesearch-py-2.2.2/opensearchpy/connection/http_async.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/connection/http_async.pyi` & `retakesearch-py-2.2.2/opensearchpy/connection/http_async.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/connection/http_requests.py` & `retakesearch-py-2.2.2/opensearchpy/connection/http_requests.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/connection/http_requests.pyi` & `retakesearch-py-2.2.2/opensearchpy/connection/http_requests.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/connection/http_urllib3.py` & `retakesearch-py-2.2.2/opensearchpy/connection/http_urllib3.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/connection/http_urllib3.pyi` & `retakesearch-py-2.2.2/opensearchpy/connection/http_urllib3.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/connection/pooling.py` & `retakesearch-py-2.2.2/opensearchpy/connection/pooling.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/connection/pooling.pyi` & `retakesearch-py-2.2.2/opensearchpy/connection/pooling.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/connection_pool.py` & `retakesearch-py-2.2.2/opensearchpy/connection_pool.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/connection_pool.pyi` & `retakesearch-py-2.2.2/opensearchpy/connection_pool.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/exceptions.py` & `retakesearch-py-2.2.2/opensearchpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/exceptions.pyi` & `retakesearch-py-2.2.2/opensearchpy/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/__init__.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/__init__.pyi` & `retakesearch-py-2.2.2/opensearchpy/helpers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/actions.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/actions.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/actions.pyi` & `retakesearch-py-2.2.2/opensearchpy/helpers/actions.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/aggs.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/aggs.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/aggs.pyi` & `retakesearch-py-2.2.2/opensearchpy/helpers/aggs.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/analysis.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/analysis.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/analysis.pyi` & `retakesearch-py-2.2.2/opensearchpy/helpers/analysis.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/asyncsigner.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/asyncsigner.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/asyncsigner.pyi` & `retakesearch-py-2.2.2/opensearchpy/helpers/asyncsigner.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/document.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/document.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/document.pyi` & `retakesearch-py-2.2.2/opensearchpy/helpers/document.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/errors.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/errors.pyi` & `retakesearch-py-2.2.2/opensearchpy/helpers/errors.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/faceted_search.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/faceted_search.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/faceted_search.pyi` & `retakesearch-py-2.2.2/opensearchpy/helpers/faceted_search.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/field.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/field.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/field.pyi` & `retakesearch-py-2.2.2/opensearchpy/helpers/field.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/function.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/function.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/function.pyi` & `retakesearch-py-2.2.2/opensearchpy/helpers/function.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/index.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/index.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/index.pyi` & `retakesearch-py-2.2.2/opensearchpy/helpers/index.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/mapping.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/mapping.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/mapping.pyi` & `retakesearch-py-2.2.2/opensearchpy/helpers/mapping.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/query.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/query.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/query.pyi` & `retakesearch-py-2.2.2/opensearchpy/helpers/query.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/response/__init__.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/response/__init__.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/response/__init__.pyi` & `retakesearch-py-2.2.2/opensearchpy/helpers/response/__init__.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/response/aggs.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/response/aggs.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/response/aggs.pyi` & `retakesearch-py-2.2.2/opensearchpy/helpers/response/aggs.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/response/hit.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/response/hit.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/response/hit.pyi` & `retakesearch-py-2.2.2/opensearchpy/helpers/response/hit.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/search.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,41 +344,39 @@
 
     def filter(self, *args, **kwargs):
         return self.query(Bool(filter=[Q(*args, **kwargs)]))
 
     def exclude(self, *args, **kwargs):
         return self.query(Bool(filter=[~Q(*args, **kwargs)]))
 
-    def neuralQuery(self, query, fields):
-        neural_queries = []
+    def _create_semantic_queries(self, query, fields):
         reserved_embedding_field_name_ending = "_retake_embedding"
 
-        for field in fields:
-            vector_field = f"{field}{reserved_embedding_field_name_ending}"
-            neural_queries.append(
-                Q(
-                    "script_score",
-                    query=Q(
-                        "neural",
-                        **{
-                            vector_field: {
-                                "query_text": query,
-                            }
-                        }
-                    ),
-                    script={"source": "_score"}
-                )
+        queries = [
+            Q(
+                "neural",
+                **{
+                    f"{field}{reserved_embedding_field_name_ending}": {
+                        "query_text": query,
+                    }
+                },
             )
+            for field in fields
+        ]
 
-        match_query = Q(
-            "script_score",
-            query=Q("multi_match", query=query, fields=fields),
-            script={"source": "_score"},
-        )
-        queries = neural_queries + [match_query]
+        return queries
+
+    def with_semantic(self, query, fields):
+        queries = self._create_semantic_queries(query, fields)
+
+        return self.query(Bool(should=queries))
+
+    def with_neural(self, query, fields):
+        queries = self._create_semantic_queries(query, fields)
+        queries.append(Q("multi_match", query=query, fields=fields))
 
         return self.query(Bool(should=queries))
 
     def __iter__(self):
         """
         Iterate over the hits.
         """
```

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/search.pyi` & `retakesearch-py-2.2.2/opensearchpy/helpers/search.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/signer.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/signer.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/test.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/test.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/test.pyi` & `retakesearch-py-2.2.2/opensearchpy/helpers/test.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/update_by_query.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/update_by_query.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/update_by_query.pyi` & `retakesearch-py-2.2.2/opensearchpy/helpers/update_by_query.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/utils.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/utils.pyi` & `retakesearch-py-2.2.2/opensearchpy/helpers/utils.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/wrappers.py` & `retakesearch-py-2.2.2/opensearchpy/helpers/wrappers.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/helpers/wrappers.pyi` & `retakesearch-py-2.2.2/opensearchpy/helpers/wrappers.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/plugins/alerting.py` & `retakesearch-py-2.2.2/opensearchpy/plugins/alerting.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/plugins/alerting.pyi` & `retakesearch-py-2.2.2/opensearchpy/plugins/alerting.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/plugins/index_management.py` & `retakesearch-py-2.2.2/opensearchpy/plugins/index_management.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/plugins/index_management.pyi` & `retakesearch-py-2.2.2/opensearchpy/plugins/index_management.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/plugins/security.py` & `retakesearch-py-2.2.2/opensearchpy/plugins/security.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/plugins/security.pyi` & `retakesearch-py-2.2.2/opensearchpy/plugins/security.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/serializer.py` & `retakesearch-py-2.2.2/opensearchpy/serializer.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/serializer.pyi` & `retakesearch-py-2.2.2/opensearchpy/serializer.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/transport.py` & `retakesearch-py-2.2.2/opensearchpy/transport.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/opensearchpy/transport.pyi` & `retakesearch-py-2.2.2/opensearchpy/transport.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/retakesearch_py.egg-info/PKG-INFO` & `retakesearch-py-2.2.2/retakesearch_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retakesearch-py
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python client for OpenSearch
 Home-page: https://github.com/opensearch-project/opensearch-py
 Author: Aleksei Atavin, Denis Zalevskiy, Rushi Agrawal, Shephali Mittal
 Author-email: axeo@aiven.io, dez@aiven.io, rushi.agr@gmail.com, shephalm@amazon.com
 Maintainer: Aleksei Atavin, Denis Zalevskiy, Rushi Agrawal, Shephali Mittal
 Maintainer-email: axeo@aiven.io, dez@aiven.io, rushi.agr@gmail.com, shephalm@amazon.com
 License: Apache-2.0
```

### Comparing `retakesearch-py-2.2.1/retakesearch_py.egg-info/SOURCES.txt` & `retakesearch-py-2.2.2/retakesearch_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.1/setup.py` & `retakesearch-py-2.2.2/setup.py`

 * *Files identical despite different names*

