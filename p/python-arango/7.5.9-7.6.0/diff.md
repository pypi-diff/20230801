# Comparing `tmp/python-arango-7.5.9.tar.gz` & `tmp/python-arango-7.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-arango-7.5.9.tar", last modified: Fri Jul 14 09:18:45 2023, max compression
+gzip compressed data, was "python-arango-7.6.0.tar", last modified: Tue Aug  1 15:03:35 2023, max compression
```

## Comparing `python-arango-7.5.9.tar` & `python-arango-7.6.0.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:18:45.003551 python-arango-7.5.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:18:44.995550 python-arango-7.5.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:18:44.999551 python-arango-7.5.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-14 09:18:33.000000 python-arango-7.5.9/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-14 09:18:33.000000 python-arango-7.5.9/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-14 09:18:33.000000 python-arango-7.5.9/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-14 09:18:33.000000 python-arango-7.5.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-14 09:18:33.000000 python-arango-7.5.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-14 09:18:33.000000 python-arango-7.5.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-14 09:18:33.000000 python-arango-7.5.9/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-14 09:18:33.000000 python-arango-7.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-14 09:18:33.000000 python-arango-7.5.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-07-14 09:18:45.003551 python-arango-7.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-14 09:18:33.000000 python-arango-7.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:18:44.999551 python-arango-7.5.9/arango/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27539 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/aql.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)   123588 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)   102581 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    34373 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/errno.py
--rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17317 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    41559 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32737 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/foxx.py
--rw-r--r--   0 runner    (1001) docker     (123)    35862 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/pregel.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33852 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/replication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/result.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 09:18:44.000000 python-arango-7.5.9/arango/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-07-14 09:18:33.000000 python-arango-7.5.9/arango/wal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:18:45.003551 python-arango-7.5.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/admin.rst
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/analyzer.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/aql.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/async.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/auth.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/backup.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/batch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/certificates.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/cluster.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/collection.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/cursor.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/database.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/document.rst
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/errno.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/foxx.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/graph.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/http.rst
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/indexes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/overload.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/pregel.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/replication.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/serializer.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/simple.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/specs.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:18:45.003551 python-arango-7.5.9/docs/static/
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/task.rst
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/threading.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/transaction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/user.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/view.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-14 09:18:33.000000 python-arango-7.5.9/docs/wal.rst
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-14 09:18:33.000000 python-arango-7.5.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:18:45.003551 python-arango-7.5.9/python_arango.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-07-14 09:18:44.000000 python-arango-7.5.9/python_arango.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-14 09:18:44.000000 python-arango-7.5.9/python_arango.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:18:44.000000 python-arango-7.5.9/python_arango.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-14 09:18:44.000000 python-arango-7.5.9/python_arango.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 09:18:44.000000 python-arango-7.5.9/python_arango.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-14 09:18:45.015551 python-arango-7.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-14 09:18:33.000000 python-arango-7.5.9/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4095 2023-07-14 09:18:33.000000 python-arango-7.5.9/tester.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:03:35.838951 python-arango-7.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:03:35.826951 python-arango-7.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:03:35.830951 python-arango-7.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-08-01 15:03:19.000000 python-arango-7.6.0/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-01 15:03:19.000000 python-arango-7.6.0/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-08-01 15:03:19.000000 python-arango-7.6.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-08-01 15:03:19.000000 python-arango-7.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-01 15:03:19.000000 python-arango-7.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-08-01 15:03:19.000000 python-arango-7.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-01 15:03:19.000000 python-arango-7.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 15:03:19.000000 python-arango-7.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-01 15:03:19.000000 python-arango-7.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-08-01 15:03:35.838951 python-arango-7.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-08-01 15:03:19.000000 python-arango-7.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:03:35.830951 python-arango-7.6.0/arango/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27539 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/aql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127009 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103562 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34373 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/errno.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17317 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41559 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32737 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/foxx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35862 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/pregel.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33852 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-01 15:03:35.000000 python-arango-7.6.0/arango/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-08-01 15:03:19.000000 python-arango-7.6.0/arango/wal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:03:35.834951 python-arango-7.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/admin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/analyzer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/aql.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/async.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/auth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/backup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/batch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/certificates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/cluster.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/collection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/cursor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/document.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/errno.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/foxx.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/graph.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/http.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/indexes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/overload.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/pregel.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/replication.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/serializer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/simple.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/specs.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:03:35.834951 python-arango-7.6.0/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/task.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/threading.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/transaction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/view.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-08-01 15:03:19.000000 python-arango-7.6.0/docs/wal.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-01 15:03:19.000000 python-arango-7.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:03:35.834951 python-arango-7.6.0/python_arango.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-08-01 15:03:35.000000 python-arango-7.6.0/python_arango.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-08-01 15:03:35.000000 python-arango-7.6.0/python_arango.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:03:35.000000 python-arango-7.6.0/python_arango.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-01 15:03:35.000000 python-arango-7.6.0/python_arango.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 15:03:35.000000 python-arango-7.6.0/python_arango.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-01 15:03:35.850952 python-arango-7.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-08-01 15:03:19.000000 python-arango-7.6.0/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4095 2023-08-01 15:03:19.000000 python-arango-7.6.0/tester.sh
```

### Comparing `python-arango-7.5.9/.github/workflows/build.yaml` & `python-arango-7.6.0/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/.github/workflows/pypi.yaml` & `python-arango-7.6.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/.gitignore` & `python-arango-7.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/.pre-commit-config.yaml` & `python-arango-7.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/CONTRIBUTING.md` & `python-arango-7.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/LICENSE` & `python-arango-7.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/PKG-INFO` & `python-arango-7.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-arango
-Version: 7.5.9
+Version: 7.6.0
 Summary: Python Driver for ArangoDB
 Home-page: https://github.com/ArangoDB-Community/python-arango
 Author: Joohwan Oh
 Author-email: joohwan.oh@outlook.com
 License: MIT
 Keywords: arangodb,python,driver
 Classifier: Intended Audience :: Developers
```

### Comparing `python-arango-7.5.9/README.md` & `python-arango-7.6.0/README.md`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/arango/api.py` & `python-arango-7.6.0/arango/api.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/arango/aql.py` & `python-arango-7.6.0/arango/aql.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/arango/backup.py` & `python-arango-7.6.0/arango/backup.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/arango/client.py` & `python-arango-7.6.0/arango/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,38 @@
     HostResolver,
     RandomHostResolver,
     RoundRobinHostResolver,
     SingleHostResolver,
 )
 
 
+def default_serializer(x: Any) -> str:
+    """
+    Default JSON serializer
+
+    :param x: A JSON data type object to serialize
+    :type x: Any
+    :return: The object serialized as a JSON string
+    :rtype: str
+    """
+    return dumps(x)
+
+
+def default_deserializer(x: str) -> Any:
+    """
+    Default JSON de-serializer
+
+    :param x: A JSON string to deserialize
+    :type x: str
+    :return: The de-serialized JSON object
+    :rtype: Any
+    """
+    return loads(x)
+
+
 class ArangoClient:
     """ArangoDB client.
 
     :param hosts: Host URL or list of URLs (coordinators in a cluster).
     :type hosts: str | [str]
     :param host_resolver: Host resolver. This parameter used for clusters (when
         multiple host URLs are provided). Accepted values are "roundrobin" and
@@ -63,18 +87,18 @@
 
     def __init__(
         self,
         hosts: Union[str, Sequence[str]] = "http://127.0.0.1:8529",
         host_resolver: str = "roundrobin",
         resolver_max_tries: Optional[int] = None,
         http_client: Optional[HTTPClient] = None,
-        serializer: Callable[..., str] = lambda x: dumps(x),
-        deserializer: Callable[[str], Any] = lambda x: loads(x),
+        serializer: Callable[..., str] = default_serializer,
+        deserializer: Callable[[str], Any] = default_deserializer,
         verify_override: Union[bool, str, None] = None,
-        request_timeout: Union[int, float] = DEFAULT_REQUEST_TIMEOUT,
+        request_timeout: Union[int, float, None] = DEFAULT_REQUEST_TIMEOUT,
     ) -> None:
         if isinstance(hosts, str):
             self._hosts = [host.strip("/") for host in hosts.split(",")]
         else:
             self._hosts = [host.strip("/") for host in hosts]
 
         host_count = len(self._hosts)
```

### Comparing `python-arango-7.5.9/arango/cluster.py` & `python-arango-7.6.0/arango/cluster.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/arango/collection.py` & `python-arango-7.6.0/arango/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1464,14 +1464,15 @@
         sync: Optional[bool] = None,
         silent: bool = False,
         overwrite: bool = False,
         return_old: bool = False,
         overwrite_mode: Optional[str] = None,
         keep_none: Optional[bool] = None,
         merge: Optional[bool] = None,
+        refill_index_caches: Optional[bool] = None,
     ) -> Result[Union[bool, List[Union[Json, ArangoServerError]]]]:
         """Insert multiple documents.
 
         .. note::
 
             If inserting a document fails, the exception is not raised but
             returned as an object in the result list. It is up to you to
@@ -1514,16 +1515,18 @@
             in the document. Otherwise, they are removed completely. Applies
             only when **overwrite_mode** is set to "update" (update-insert).
         :type keep_none: bool | None
         :param merge: If set to True (default), sub-dictionaries are merged
             instead of the new one overwriting the old one. Applies only when
             **overwrite_mode** is set to "update" (update-insert).
         :type merge: bool | None
-        :return: Document metadata (e.g. document key, revision) or True if
-            parameter **silent** was set to True.
+        :param refill_index_caches: Whether to add new entries to in-memory
+            index caches if document insertions affect the edge index or
+            cache-enabled persistent indexes.
+        :type refill_index_caches: bool | None
         :return: List of document metadata (e.g. document keys, revisions) and
             any exception, or True if parameter **silent** was set to True.
         :rtype: [dict | ArangoServerError] | bool
         :raise arango.exceptions.DocumentInsertError: If insert fails.
         """
         documents = [self._ensure_key_from_id(doc) for doc in documents]
 
@@ -1539,14 +1542,18 @@
         if overwrite_mode is not None:
             params["overwriteMode"] = overwrite_mode
         if keep_none is not None:
             params["keepNull"] = keep_none
         if merge is not None:
             params["mergeObjects"] = merge
 
+        # New in ArangoDB 3.9.6 and 3.10.2
+        if refill_index_caches is not None:
+            params["refillIndexCaches"] = refill_index_caches
+
         request = Request(
             method="post",
             endpoint=f"/_api/document/{self.name}",
             data=documents,
             params=params,
         )
 
@@ -1578,14 +1585,15 @@
         check_rev: bool = True,
         merge: bool = True,
         keep_none: bool = True,
         return_new: bool = False,
         return_old: bool = False,
         sync: Optional[bool] = None,
         silent: bool = False,
+        refill_index_caches: Optional[bool] = None,
     ) -> Result[Union[bool, List[Union[Json, ArangoServerError]]]]:
         """Update multiple documents.
 
         .. note::
 
             If updating a document fails, the exception is not raised but
             returned as an object in the result list. It is up to you to
@@ -1620,14 +1628,18 @@
             metadata. Ignored if parameter **silent** is set to True.
         :type return_old: bool
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool | None
         :param silent: If set to True, no document metadata is returned. This
             can be used to save resources.
         :type silent: bool
+        :param refill_index_caches: Whether to add new entries to in-memory
+            index caches if document operations affect the edge index or
+            cache-enabled persistent indexes.
+        :type refill_index_caches: bool | None
         :return: List of document metadata (e.g. document keys, revisions) and
             any exceptions, or True if parameter **silent** was set to True.
         :rtype: [dict | ArangoError] | bool
         :raise arango.exceptions.DocumentUpdateError: If update fails.
         """
         params: Params = {
             "keepNull": keep_none,
@@ -1637,14 +1649,18 @@
             "ignoreRevs": not check_rev,
             "overwrite": not check_rev,
             "silent": silent,
         }
         if sync is not None:
             params["waitForSync"] = sync
 
+        # New in ArangoDB 3.9.6 and 3.10.2
+        if refill_index_caches is not None:
+            params["refillIndexCaches"] = refill_index_caches
+
         documents = [self._ensure_key_in_body(doc) for doc in documents]
 
         request = Request(
             method="patch",
             endpoint=f"/_api/document/{self.name}",
             data=documents,
             params=params,
@@ -1749,14 +1765,15 @@
         self,
         documents: Sequence[Json],
         check_rev: bool = True,
         return_new: bool = False,
         return_old: bool = False,
         sync: Optional[bool] = None,
         silent: bool = False,
+        refill_index_caches: Optional[bool] = None,
     ) -> Result[Union[bool, List[Union[Json, ArangoServerError]]]]:
         """Replace multiple documents.
 
         .. note::
 
             If replacing a document fails, the exception is not raised but
             returned as an object in the result list. It is up to you to
@@ -1786,14 +1803,18 @@
             metadata. Ignored if parameter **silent** is set to True.
         :type return_old: bool
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool | None
         :param silent: If set to True, no document metadata is returned. This
             can be used to save resources.
         :type silent: bool
+        :param refill_index_caches: Whether to add new entries to in-memory
+            index caches if document operations affect the edge index or
+            cache-enabled persistent indexes.
+        :type refill_index_caches: bool | None
         :return: List of document metadata (e.g. document keys, revisions) and
             any exceptions, or True if parameter **silent** was set to True.
         :rtype: [dict | ArangoServerError] | bool
         :raise arango.exceptions.DocumentReplaceError: If replace fails.
         """
         params: Params = {
             "returnNew": return_new,
@@ -1801,14 +1822,18 @@
             "ignoreRevs": not check_rev,
             "overwrite": not check_rev,
             "silent": silent,
         }
         if sync is not None:
             params["waitForSync"] = sync
 
+        # New in ArangoDB 3.9.6 and 3.10.2
+        if refill_index_caches is not None:
+            params["refillIndexCaches"] = refill_index_caches
+
         documents = [self._ensure_key_in_body(doc) for doc in documents]
 
         request = Request(
             method="put",
             endpoint=f"/_api/document/{self.name}",
             params=params,
             data=documents,
@@ -1897,14 +1922,15 @@
     def delete_many(
         self,
         documents: Sequence[Json],
         return_old: bool = False,
         check_rev: bool = True,
         sync: Optional[bool] = None,
         silent: bool = False,
+        refill_index_caches: Optional[bool] = None,
     ) -> Result[Union[bool, List[Union[Json, ArangoServerError]]]]:
         """Delete multiple documents.
 
         .. note::
 
             If deleting a document fails, the exception is not raised but
             returned as an object in the result list. It is up to you to
@@ -1929,28 +1955,36 @@
             are compared against the revisions of target documents.
         :type check_rev: bool
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool | None
         :param silent: If set to True, no document metadata is returned. This
             can be used to save resources.
         :type silent: bool
+        :param refill_index_caches: Whether to add new entries to in-memory
+            index caches if document operations affect the edge index or
+            cache-enabled persistent indexes.
+        :type refill_index_caches: bool | None
         :return: List of document metadata (e.g. document keys, revisions) and
             any exceptions, or True if parameter **silent** was set to True.
         :rtype: [dict | ArangoServerError] | bool
         :raise arango.exceptions.DocumentDeleteError: If delete fails.
         """
         params: Params = {
             "returnOld": return_old,
             "ignoreRevs": not check_rev,
             "overwrite": not check_rev,
             "silent": silent,
         }
         if sync is not None:
             params["waitForSync"] = sync
 
+        # New in ArangoDB 3.9.6 and 3.10.2
+        if refill_index_caches is not None:
+            params["refillCaches"] = refill_index_caches
+
         documents = [
             self._ensure_key_in_body(doc) if isinstance(doc, dict) else doc
             for doc in documents
         ]
 
         request = Request(
             method="delete",
@@ -2225,14 +2259,15 @@
         sync: Optional[bool] = None,
         silent: bool = False,
         overwrite: bool = False,
         return_old: bool = False,
         overwrite_mode: Optional[str] = None,
         keep_none: Optional[bool] = None,
         merge: Optional[bool] = None,
+        refill_index_caches: Optional[bool] = None,
     ) -> Result[Union[bool, Json]]:
         """Insert a new document.
 
         :param document: Document to insert. If it contains the "_key" or "_id"
             field, the value is used as the key of the new document (otherwise
             it is auto-generated). Any "_rev" field is ignored.
         :type document: dict
@@ -2259,14 +2294,18 @@
             in the document. Otherwise, they are removed completely. Applies
             only when **overwrite_mode** is set to "update" (update-insert).
         :type keep_none: bool | None
         :param merge: If set to True (default), sub-dictionaries are merged
             instead of the new one overwriting the old one. Applies only when
             **overwrite_mode** is set to "update" (update-insert).
         :type merge: bool | None
+        :param refill_index_caches: Whether to add new entries to in-memory
+            index caches if document insertions affect the edge index or
+            cache-enabled persistent indexes.
+        :type refill_index_caches: bool | None
         :return: Document metadata (e.g. document key, revision) or True if
             parameter **silent** was set to True.
         :rtype: bool | dict
         :raise arango.exceptions.DocumentInsertError: If insert fails.
         """
         document = self._ensure_key_from_id(document)
 
@@ -2281,14 +2320,18 @@
         if overwrite_mode is not None:
             params["overwriteMode"] = overwrite_mode
         if keep_none is not None:
             params["keepNull"] = keep_none
         if merge is not None:
             params["mergeObjects"] = merge
 
+        # New in ArangoDB 3.9.6 and 3.10.2
+        if refill_index_caches is not None:
+            params["refillIndexCaches"] = refill_index_caches
+
         request = Request(
             method="post",
             endpoint=f"/_api/document/{self.name}",
             data=document,
             params=params,
             write=self.name,
         )
@@ -2313,14 +2356,15 @@
         check_rev: bool = True,
         merge: bool = True,
         keep_none: bool = True,
         return_new: bool = False,
         return_old: bool = False,
         sync: Optional[bool] = None,
         silent: bool = False,
+        refill_index_caches: Optional[bool] = None,
     ) -> Result[Union[bool, Json]]:
         """Update a document.
 
         :param document: Partial or full document with the updated values. It
             must contain the "_id" or "_key" field.
         :type document: dict
         :param check_rev: If set to True, revision of **document** (if given)
@@ -2339,14 +2383,18 @@
             metadata. Ignored if parameter **silent** is set to True.
         :type return_old: bool
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool | None
         :param silent: If set to True, no document metadata is returned. This
             can be used to save resources.
         :type silent: bool
+        :param refill_index_caches: Whether to add new entries to in-memory
+            index caches if document insertions affect the edge index or
+            cache-enabled persistent indexes.
+        :type refill_index_caches: bool | None
         :return: Document metadata (e.g. document key, revision) or True if
             parameter **silent** was set to True.
         :rtype: bool | dict
         :raise arango.exceptions.DocumentUpdateError: If update fails.
         :raise arango.exceptions.DocumentRevisionError: If revisions mismatch.
         """
         params: Params = {
@@ -2357,14 +2405,18 @@
             "ignoreRevs": not check_rev,
             "overwrite": not check_rev,
             "silent": silent,
         }
         if sync is not None:
             params["waitForSync"] = sync
 
+        # New in ArangoDB 3.9.6 and 3.10.2
+        if refill_index_caches is not None:
+            params["refillIndexCaches"] = refill_index_caches
+
         request = Request(
             method="patch",
             endpoint=f"/_api/document/{self._extract_id(document)}",
             data=document,
             params=params,
             write=self.name,
         )
@@ -2387,14 +2439,15 @@
         self,
         document: Json,
         check_rev: bool = True,
         return_new: bool = False,
         return_old: bool = False,
         sync: Optional[bool] = None,
         silent: bool = False,
+        refill_index_caches: Optional[bool] = None,
     ) -> Result[Union[bool, Json]]:
         """Replace a document.
 
         :param document: New document to replace the old one with. It must
             contain the "_id" or "_key" field. Edge document must also have
             "_from" and "_to" fields.
         :type document: dict
@@ -2408,14 +2461,18 @@
             metadata. Ignored if parameter **silent** is set to True.
         :type return_old: bool
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool | None
         :param silent: If set to True, no document metadata is returned. This
             can be used to save resources.
         :type silent: bool
+        :param refill_index_caches: Whether to add new entries to in-memory
+            index caches if document insertions affect the edge index or
+            cache-enabled persistent indexes.
+        :type refill_index_caches: bool | None
         :return: Document metadata (e.g. document key, revision) or True if
             parameter **silent** was set to True.
         :rtype: bool | dict
         :raise arango.exceptions.DocumentReplaceError: If replace fails.
         :raise arango.exceptions.DocumentRevisionError: If revisions mismatch.
         """
         params: Params = {
@@ -2424,14 +2481,18 @@
             "ignoreRevs": not check_rev,
             "overwrite": not check_rev,
             "silent": silent,
         }
         if sync is not None:
             params["waitForSync"] = sync
 
+        # New in ArangoDB 3.9.6 and 3.10.2
+        if refill_index_caches is not None:
+            params["refillIndexCaches"] = refill_index_caches
+
         request = Request(
             method="put",
             endpoint=f"/_api/document/{self._extract_id(document)}",
             params=params,
             data=document,
             write=self.name,
         )
@@ -2457,14 +2518,15 @@
         document: Union[str, Json],
         rev: Optional[str] = None,
         check_rev: bool = True,
         ignore_missing: bool = False,
         return_old: bool = False,
         sync: Optional[bool] = None,
         silent: bool = False,
+        refill_index_caches: Optional[bool] = None,
     ) -> Result[Union[bool, Json]]:
         """Delete a document.
 
         :param document: Document ID, key or body. Document body must contain
             the "_id" or "_key" field.
         :type document: str | dict
         :param rev: Expected document revision. Overrides the value of "_rev"
@@ -2481,14 +2543,18 @@
             metadata. Ignored if parameter **silent** is set to True.
         :type return_old: bool
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool | None
         :param silent: If set to True, no document metadata is returned. This
             can be used to save resources.
         :type silent: bool
+        :param refill_index_caches: Whether to add new entries to in-memory
+            index caches if document operations affect the edge index or
+            cache-enabled persistent indexes.
+        :type refill_index_caches: bool | None
         :return: Document metadata (e.g. document key, revision), or True if
             parameter **silent** was set to True, or False if document was not
             found and **ignore_missing** was set to True (does not apply in
             transactions).
         :rtype: bool | dict
         :raise arango.exceptions.DocumentDeleteError: If delete fails.
         :raise arango.exceptions.DocumentRevisionError: If revisions mismatch.
@@ -2500,14 +2566,18 @@
             "ignoreRevs": not check_rev,
             "overwrite": not check_rev,
             "silent": silent,
         }
         if sync is not None:
             params["waitForSync"] = sync
 
+        # New in ArangoDB 3.9.6 and 3.10.2
+        if refill_index_caches is not None:
+            params["refillIndexCaches"] = refill_index_caches
+
         request = Request(
             method="delete",
             endpoint=f"/_api/document/{handle}",
             params=params,
             headers=headers,
             write=self.name,
         )
```

### Comparing `python-arango-7.5.9/arango/connection.py` & `python-arango-7.6.0/arango/connection.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/arango/cursor.py` & `python-arango-7.6.0/arango/cursor.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/arango/database.py` & `python-arango-7.6.0/arango/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -568,31 +568,42 @@
             result: Json = resp.body
             if "totalAmount" in result:
                 resp.body["total_amount"] = resp.body.pop("totalAmount")
             return result
 
         return self._execute(request, response_handler)
 
-    def log_levels(self) -> Result[Json]:
+    def log_levels(self, server_id: Optional[str] = None) -> Result[Json]:
         """Return current logging levels.
 
+        :param server_id: Forward log level to a specific server. This makes it
+            easier to adjust the log levels in clusters because DB-Servers require
+            JWT authentication whereas Coordinators also support authentication
+            using usernames and passwords.
+        :type server_id: str
         :return: Current logging levels.
         :rtype: dict
         """
-        request = Request(method="get", endpoint="/_admin/log/level")
+        params: Params = {}
+        if server_id is not None:
+            params["serverId"] = server_id
+
+        request = Request(method="get", endpoint="/_admin/log/level", params=params)
 
         def response_handler(resp: Response) -> Json:
             if not resp.is_success:
                 raise ServerLogLevelError(resp, request)
             result: Json = resp.body
             return result
 
         return self._execute(request, response_handler)
 
-    def set_log_levels(self, **kwargs: str) -> Result[Json]:
+    def set_log_levels(
+        self, server_id: Optional[str] = None, **kwargs: str
+    ) -> Result[Json]:
         """Set the logging levels.
 
         This method takes arbitrary keyword arguments where the keys are the
         logger names and the values are the logging levels. For example:
 
         .. code-block:: python
 
@@ -600,18 +611,29 @@
                 agency='DEBUG',
                 collector='INFO',
                 threads='WARNING'
             )
 
         Keys that are not valid logger names are ignored.
 
+        :param server_id: Forward log level to a specific server. This makes it
+            easier to adjust the log levels in clusters because DB-Servers require
+            JWT authentication whereas Coordinators also support authentication
+            using usernames and passwords.
+        :type server_id: str | None
         :return: New logging levels.
         :rtype: dict
         """
-        request = Request(method="put", endpoint="/_admin/log/level", data=kwargs)
+        params: Params = {}
+        if server_id is not None:
+            params["serverId"] = server_id
+
+        request = Request(
+            method="put", endpoint="/_admin/log/level", params=params, data=kwargs
+        )
 
         def response_handler(resp: Response) -> Json:
             if not resp.is_success:
                 raise ServerLogLevelSetError(resp, request)
             result: Json = resp.body
             return result
```

### Comparing `python-arango-7.5.9/arango/errno.py` & `python-arango-7.6.0/arango/errno.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/arango/exceptions.py` & `python-arango-7.6.0/arango/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/arango/executor.py` & `python-arango-7.6.0/arango/executor.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/arango/formatter.py` & `python-arango-7.6.0/arango/formatter.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/arango/foxx.py` & `python-arango-7.6.0/arango/foxx.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/arango/graph.py` & `python-arango-7.6.0/arango/graph.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/arango/http.py` & `python-arango-7.6.0/arango/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,17 +80,27 @@
         and requests will block for pool_timeout seconds and raise
         EmptyPoolError if no connection is available within the time period.
     :type pool_timeout: int | float | None
     :param kwargs: Additional keyword arguments passed to the HTTPAdapter constructor.
     :type kwargs: Any
     """
 
+    __attrs__ = [
+        "max_retries",
+        "config",
+        "_connection_timeout",
+        "_pool_connections",
+        "_pool_maxsize",
+        "_pool_timeout",
+        "_pool_block",
+    ]
+
     def __init__(
         self,
-        connection_timeout: Union[int, float] = DEFAULT_REQUEST_TIMEOUT,
+        connection_timeout: Union[int, float, None] = DEFAULT_REQUEST_TIMEOUT,
         pool_connections: int = DEFAULT_POOLSIZE,
         pool_maxsize: int = DEFAULT_POOLSIZE,
         pool_timeout: Union[int, float, None] = None,
         **kwargs: Any
     ) -> None:
         self._connection_timeout = connection_timeout
         self._pool_timeout = pool_timeout
@@ -136,15 +146,15 @@
         and requests will block for pool_timeout seconds and raise
         EmptyPoolError if no connection is available within the time period.
     :type pool_timeout: int | float | None
     """
 
     def __init__(
         self,
-        request_timeout: Union[int, float] = DEFAULT_REQUEST_TIMEOUT,
+        request_timeout: Union[int, float, None] = DEFAULT_REQUEST_TIMEOUT,
         retry_attempts: int = 3,
         backoff_factor: float = 1.0,
         pool_connections: int = 10,
         pool_maxsize: int = 10,
         pool_timeout: Union[int, float, None] = None,
     ) -> None:
         self.request_timeout = request_timeout
```

### Comparing `python-arango-7.5.9/arango/job.py` & `python-arango-7.6.0/arango/job.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/arango/pregel.py` & `python-arango-7.6.0/arango/pregel.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/arango/replication.py` & `python-arango-7.6.0/arango/replication.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/arango/request.py` & `python-arango-7.6.0/arango/request.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/arango/resolver.py` & `python-arango-7.6.0/arango/resolver.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/arango/response.py` & `python-arango-7.6.0/arango/response.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/arango/utils.py` & `python-arango-7.6.0/arango/utils.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/arango/wal.py` & `python-arango-7.6.0/arango/wal.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/Makefile` & `python-arango-7.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/admin.rst` & `python-arango-7.6.0/docs/admin.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/analyzer.rst` & `python-arango-7.6.0/docs/analyzer.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/aql.rst` & `python-arango-7.6.0/docs/aql.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/async.rst` & `python-arango-7.6.0/docs/async.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/auth.rst` & `python-arango-7.6.0/docs/auth.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/backup.rst` & `python-arango-7.6.0/docs/backup.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/batch.rst` & `python-arango-7.6.0/docs/batch.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/certificates.rst` & `python-arango-7.6.0/docs/certificates.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/cluster.rst` & `python-arango-7.6.0/docs/cluster.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/collection.rst` & `python-arango-7.6.0/docs/collection.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/conf.py` & `python-arango-7.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/contributing.rst` & `python-arango-7.6.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/cursor.rst` & `python-arango-7.6.0/docs/cursor.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/database.rst` & `python-arango-7.6.0/docs/database.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/document.rst` & `python-arango-7.6.0/docs/document.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/errors.rst` & `python-arango-7.6.0/docs/errors.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/foxx.rst` & `python-arango-7.6.0/docs/foxx.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/graph.rst` & `python-arango-7.6.0/docs/graph.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/http.rst` & `python-arango-7.6.0/docs/http.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/index.rst` & `python-arango-7.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/indexes.rst` & `python-arango-7.6.0/docs/indexes.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/logging.rst` & `python-arango-7.6.0/docs/logging.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/make.bat` & `python-arango-7.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/overload.rst` & `python-arango-7.6.0/docs/overload.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/overview.rst` & `python-arango-7.6.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/pregel.rst` & `python-arango-7.6.0/docs/pregel.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/replication.rst` & `python-arango-7.6.0/docs/replication.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/schema.rst` & `python-arango-7.6.0/docs/schema.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/serializer.rst` & `python-arango-7.6.0/docs/serializer.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/simple.rst` & `python-arango-7.6.0/docs/simple.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/specs.rst` & `python-arango-7.6.0/docs/specs.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/static/logo.png` & `python-arango-7.6.0/docs/static/logo.png`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/task.rst` & `python-arango-7.6.0/docs/task.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/threading.rst` & `python-arango-7.6.0/docs/threading.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/transaction.rst` & `python-arango-7.6.0/docs/transaction.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/user.rst` & `python-arango-7.6.0/docs/user.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/view.rst` & `python-arango-7.6.0/docs/view.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/docs/wal.rst` & `python-arango-7.6.0/docs/wal.rst`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/pyproject.toml` & `python-arango-7.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/python_arango.egg-info/PKG-INFO` & `python-arango-7.6.0/python_arango.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-arango
-Version: 7.5.9
+Version: 7.6.0
 Summary: Python Driver for ArangoDB
 Home-page: https://github.com/ArangoDB-Community/python-arango
 Author: Joohwan Oh
 Author-email: joohwan.oh@outlook.com
 License: MIT
 Keywords: arangodb,python,driver
 Classifier: Intended Audience :: Developers
```

### Comparing `python-arango-7.5.9/python_arango.egg-info/SOURCES.txt` & `python-arango-7.6.0/python_arango.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/setup.py` & `python-arango-7.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-arango-7.5.9/tester.sh` & `python-arango-7.6.0/tester.sh`

 * *Files identical despite different names*

