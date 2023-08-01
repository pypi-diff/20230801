# Comparing `tmp/swoop.db-7.0.3.tar.gz` & `tmp/swoop.db-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swoop.db-7.0.3.tar", last modified: Tue Jul 25 17:51:45 2023, max compression
+gzip compressed data, was "swoop.db-8.0.0.tar", last modified: Tue Aug  1 19:06:15 2023, max compression
```

## Comparing `swoop.db-7.0.3.tar` & `swoop.db-8.0.0.tar`

### file list

```diff
@@ -1,77 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.557848 swoop.db-7.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-25 17:51:18.000000 swoop.db-7.0.3/.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.541848 swoop.db-7.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.545848 swoop.db-7.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-25 17:51:18.000000 swoop.db-7.0.3/.github/workflows/publish-image.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-25 17:51:18.000000 swoop.db-7.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-25 17:51:18.000000 swoop.db-7.0.3/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-25 17:51:18.000000 swoop.db-7.0.3/.github/workflows/snyk-scan.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-25 17:51:18.000000 swoop.db-7.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-25 17:51:18.000000 swoop.db-7.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-25 17:51:18.000000 swoop.db-7.0.3/.snyk
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-25 17:51:18.000000 swoop.db-7.0.3/.sqlfluff
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-25 17:51:18.000000 swoop.db-7.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-25 17:51:18.000000 swoop.db-7.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-25 17:51:18.000000 swoop.db-7.0.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-25 17:51:18.000000 swoop.db-7.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-25 17:51:45.557848 swoop.db-7.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-25 17:51:18.000000 swoop.db-7.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-25 17:51:18.000000 swoop.db-7.0.3/RELEASE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.549848 swoop.db-7.0.3/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2870 2023-07-25 17:51:18.000000 swoop.db-7.0.3/bin/db-initialization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-07-25 17:51:18.000000 swoop.db-7.0.3/bin/get-max-migration-version.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-25 17:51:18.000000 swoop.db-7.0.3/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-25 17:51:18.000000 swoop.db-7.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-25 17:51:18.000000 swoop.db-7.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 17:51:45.557848 swoop.db-7.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.541848 swoop.db-7.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.541848 swoop.db-7.0.3/src/swoop/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.549848 swoop.db-7.0.3/src/swoop/db/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.549848 swoop.db-7.0.3/src/swoop/db/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/fixtures/base_01.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.553848 swoop.db-7.0.3/src/swoop/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00000_base_schema.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00001_version.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00002_cache_func.down.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00002_cache_func.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00003_remove_items.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00004_update_thread.down.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00004_update_thread.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00005_handler_type.down.sql
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00005_handler_type.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00006_workflow_constraint.down.sql
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00006_workflow_constraint.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00007_change-uuid-formats.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16734 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.549848 swoop.db-7.0.3/src/swoop.db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-25 17:51:45.000000 swoop.db-7.0.3/src/swoop.db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-25 17:51:45.000000 swoop.db-7.0.3/src/swoop.db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 17:51:45.000000 swoop.db-7.0.3/src/swoop.db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 17:51:45.000000 swoop.db-7.0.3/src/swoop.db.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-25 17:51:45.000000 swoop.db-7.0.3/src/swoop.db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 17:51:45.000000 swoop.db-7.0.3/src/swoop.db.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.553848 swoop.db-7.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.545848 swoop.db-7.0.3/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.557848 swoop.db-7.0.3/tests/fixtures/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/fixtures/migrations/0_base_01.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/fixtures/migrations/1_result.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/fixtures/migrations/2_base_01.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/fixtures/migrations/2_result.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/fixtures/migrations/6_base_01.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/fixtures/migrations/6_result.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/fixtures/migrations/7_base_01.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/fixtures/migrations/7_result.sql
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/fixtures/migrations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.557848 swoop.db-7.0.3/tests/pgtap/
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/pgtap/test_action.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/pgtap/test_find_cached_action_for_payload.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/pgtap/test_limit-locking.sql
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/pgtap/test_uuid_v7.sql
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/test_migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.509295 swoop.db-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-01 19:05:59.000000 swoop.db-8.0.0/.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.505295 swoop.db-8.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.509295 swoop.db-8.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-08-01 19:05:59.000000 swoop.db-8.0.0/.github/workflows/publish-image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-01 19:05:59.000000 swoop.db-8.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-08-01 19:05:59.000000 swoop.db-8.0.0/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-01 19:05:59.000000 swoop.db-8.0.0/.github/workflows/snyk-scan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-08-01 19:05:59.000000 swoop.db-8.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-08-01 19:05:59.000000 swoop.db-8.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-01 19:05:59.000000 swoop.db-8.0.0/.snyk
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-01 19:05:59.000000 swoop.db-8.0.0/.sqlfluff
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-08-01 19:05:59.000000 swoop.db-8.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-08-01 19:05:59.000000 swoop.db-8.0.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-08-01 19:05:59.000000 swoop.db-8.0.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-08-01 19:05:59.000000 swoop.db-8.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-08-01 19:06:15.509295 swoop.db-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-08-01 19:05:59.000000 swoop.db-8.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-01 19:05:59.000000 swoop.db-8.0.0/RELEASE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.509295 swoop.db-8.0.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3622 2023-08-01 19:05:59.000000 swoop.db-8.0.0/bin/db-initialization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-08-01 19:05:59.000000 swoop.db-8.0.0/bin/get-max-migration-version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-01 19:05:59.000000 swoop.db-8.0.0/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-01 19:05:59.000000 swoop.db-8.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-01 19:05:59.000000 swoop.db-8.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 19:06:15.509295 swoop.db-8.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.505295 swoop.db-8.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.505295 swoop.db-8.0.0/src/swoop/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.509295 swoop.db-8.0.0/src/swoop/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-01 19:05:59.000000 swoop.db-8.0.0/src/swoop/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-01 19:05:59.000000 swoop.db-8.0.0/src/swoop/db/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-01 19:05:59.000000 swoop.db-8.0.0/src/swoop/db/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.509295 swoop.db-8.0.0/src/swoop/db/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-08-01 19:05:59.000000 swoop.db-8.0.0/src/swoop/db/fixtures/base_01.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.509295 swoop.db-8.0.0/src/swoop/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    16778 2023-08-01 19:05:59.000000 swoop.db-8.0.0/src/swoop/db/migrations/00008_new_base.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:05:59.000000 swoop.db-8.0.0/src/swoop/db/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16736 2023-08-01 19:05:59.000000 swoop.db-8.0.0/src/swoop/db/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.509295 swoop.db-8.0.0/src/swoop.db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-08-01 19:06:15.000000 swoop.db-8.0.0/src/swoop.db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-01 19:06:15.000000 swoop.db-8.0.0/src/swoop.db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:06:15.000000 swoop.db-8.0.0/src/swoop.db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 19:06:15.000000 swoop.db-8.0.0/src/swoop.db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-08-01 19:06:15.000000 swoop.db-8.0.0/src/swoop.db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 19:06:15.000000 swoop.db-8.0.0/src/swoop.db.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.509295 swoop.db-8.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-08-01 19:05:59.000000 swoop.db-8.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.505295 swoop.db-8.0.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.509295 swoop.db-8.0.0/tests/fixtures/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-01 19:05:59.000000 swoop.db-8.0.0/tests/fixtures/migrations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:06:15.509295 swoop.db-8.0.0/tests/pgtap/
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-08-01 19:05:59.000000 swoop.db-8.0.0/tests/pgtap/test_action.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-08-01 19:05:59.000000 swoop.db-8.0.0/tests/pgtap/test_find_cached_action_for_payload.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-01 19:05:59.000000 swoop.db-8.0.0/tests/pgtap/test_limit-locking.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-01 19:05:59.000000 swoop.db-8.0.0/tests/pgtap/test_uuid_v7.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-01 19:05:59.000000 swoop.db-8.0.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-01 19:05:59.000000 swoop.db-8.0.0/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-08-01 19:05:59.000000 swoop.db-8.0.0/tests/test_migrations.py
```

### Comparing `swoop.db-7.0.3/.env` & `swoop.db-8.0.0/.env`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 export PGPORT="6543"
 export PGUSER="postgres"
 export PGPASSWORD="password"
 export PGDATABASE="swoop"
 export PGSSLMODE="disable"
 export PGAUTHMETHOD="trust"
 
-SWOOP_DB_SCHEMA_VERSION_TABLE="swoop.schema_version"
+export SWOOP_DB_SCHEMA_VERSION_TABLE="swoop.schema_version"
```

### Comparing `swoop.db-7.0.3/.github/workflows/publish-image.yml` & `swoop.db-8.0.0/.github/workflows/publish-image.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/.github/workflows/python-publish.yml` & `swoop.db-8.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/.github/workflows/python-test.yml` & `swoop.db-8.0.0/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/.github/workflows/snyk-scan.yml` & `swoop.db-8.0.0/.github/workflows/snyk-scan.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/.gitignore` & `swoop.db-8.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/.pre-commit-config.yaml` & `swoop.db-8.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/.snyk` & `swoop.db-8.0.0/.snyk`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/CHANGELOG.md` & `swoop.db-8.0.0/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,38 @@
-
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v8.0.0] - 2023-08-01
+
+### Added
+
+- Migration `00008_new_base` consolidates all prior migrations in a single
+  non-backward-compatible file. This fixes a problem applying `LEAKPROOF`
+  functions as a non-superuser. ([#25])
+
+### Changed
+
+- `/bin/db-initialization.py` script makes database owner a login role for use
+  running migration to fix ownership issues. ([#25])
+- Update [dbami] dependency to v0.3.0 ([#25])
+
+
+## [v7.0.3] - 2023-07-25
+
+### Added
+
+- `/bin/db-initialization.py` script as an example for how to create a new
+  swoop db with roles. ([#23])
+
 ## [v7.0.2] - 2023-07-12
 
 ### Changed
 
 - Properly set required env vars in Dockerfile ([#22])
 
 ## [v7.0.1] - 2023-07-11
@@ -72,23 +93,27 @@
 
 - `UNKNOWN` state removed from `event_state` ([#14])
 
 ## [v0.1.0] - 2023-05-31
 
 Initial release
 
-[unreleased]: https://github.com/element84/swoop-db/compare/v7.0.2...main
+[unreleased]: https://github.com/element84/swoop-db/compare/v8.0.0...main
+[v8.0.0]: https://github.com/element84/swoop-db/compare/v7.0.3...8.0.0
+[v7.0.3]: https://github.com/element84/swoop-db/compare/v7.0.2...7.0.3
 [v7.0.2]: https://github.com/element84/swoop-db/compare/v7.0.1...7.0.2
 [v7.0.1]: https://github.com/element84/swoop-db/compare/v7.0.0...7.0.1
 [v7.0.0]: https://github.com/element84/swoop-db/compare/v2.0.0...7.0.0
 [v2.0.0]: https://github.com/element84/swoop-db/compare/v0.1.0...2.0.0
 [v0.1.0]: https://github.com/element84/swoop-db/tree/v0.1.0
 
 [#12]: https://github.com/Element84/swoop-db/pull/12
 [#14]: https://github.com/Element84/swoop-db/pull/14
 [#15]: https://github.com/Element84/swoop-db/pull/15
 [#19]: https://github.com/Element84/swoop-db/pull/19
 [#20]: https://github.com/Element84/swoop-db/pull/20
 [#21]: https://github.com/Element84/swoop-db/pull/21
 [#22]: https://github.com/Element84/swoop-db/pull/22
+[#23]: https://github.com/Element84/swoop-db/pull/23
+[#25]: https://github.com/Element84/swoop-db/pull/25
 
 [dbami]: https://github.com/element84/dbami
```

### Comparing `swoop.db-7.0.3/CONTRIBUTING.md` & `swoop.db-8.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/Dockerfile` & `swoop.db-8.0.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/LICENSE` & `swoop.db-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/PKG-INFO` & `swoop.db-8.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoop.db
-Version: 7.0.3
+Version: 8.0.0
 Summary: Database for STAC Workflow Open Orchestration Framework
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,stac,workflow,geospatial
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `swoop.db-7.0.3/README.md` & `swoop.db-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/RELEASE.md` & `swoop.db-8.0.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/docker-compose.yml` & `swoop.db-8.0.0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/pyproject.toml` & `swoop.db-8.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ]
 license = {text = "Apache License 2.0"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "asyncpg >=0.27.0",
-    "dbami >=0.2.0",
+    "dbami >=0.3.0",
 ]
 dynamic = [
   "version",
   "readme",
 ]
 
 [project.scripts]
```

### Comparing `swoop.db-7.0.3/src/swoop/db/cli.py` & `swoop.db-8.0.0/src/swoop/db/cli.py`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/src/swoop/db/fixtures/base_01.sql` & `swoop.db-8.0.0/src/swoop/db/fixtures/base_01.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/src/swoop/db/migrations/00000_base_schema.up.sql` & `swoop.db-8.0.0/src/swoop/db/schema.sql`

 * *Files 9% similar despite different names*

```diff
@@ -12,59 +12,157 @@
 ('PENDING', 'Action created and waiting to be executed'),
 ('QUEUED', 'Action queued for handler'),
 ('RUNNING', 'Action being run by handler'),
 ('SUCCESSFUL', 'Action successful'),
 ('FAILED', 'Action failed'),
 ('CANCELED', 'Action canceled'),
 ('TIMED_OUT', 'Action did not complete within allowed timeframe'),
-('UNKNOWN', 'Last update was unknown state'),
 ('BACKOFF', 'Transient error, waiting to retry'),
 (
   'INVALID',
   'Action could not be completed successfully due to '
   || 'configuration error or other incompatibility'
 ),
 (
   'RETRIES_EXHAUSTED',
   'Call did not fail within allowed time or number of retries'
 ),
 ('INFO', 'Event is informational and does not change thread state');
 
 
+-- gen_uuid_v7() modified from
+-- https://gist.github.com/kjmph/5bd772b2c2df145aa645b837da7eca74
+--
+-- Original license:
+--
+-- Copyright 2023 Kyle Hubert <kjmph@users.noreply.github.com>
+-- (https://github.com/kjmph)
+--
+-- Permission is hereby granted, free of charge, to any person obtaining a copy
+-- of this software and associated documentation files (the “Software”), to
+-- deal in the Software without restriction, including without limitation the
+-- rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
+-- sell copies of the Software, and to permit persons to whom the Software is
+-- furnished to do so, subject to the following conditions:
+--
+-- The above copyright notice and this permission notice shall be included in
+-- all copies or substantial portions of the Software.
+--
+-- THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+-- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+-- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+-- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+-- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+-- FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
+-- IN THE SOFTWARE.
+CREATE FUNCTION public.gen_uuid_v7(_timestamp timestamptz)
+RETURNS uuid
+LANGUAGE plpgsql VOLATILE
+AS $$
+DECLARE
+  _unix_ts_ms bytea;
+  _uuid_bytes bytea;
+BEGIN
+  _unix_ts_ms = substring(
+    int8send(floor(extract(epoch from _timestamp) * 1000)::bigint) from 3
+  );
+
+  -- use random v4 uuid as starting point (which has the same variant we need)
+  _uuid_bytes = uuid_send(gen_random_uuid());
+
+  -- overlay timestamp
+  _uuid_bytes = overlay(_uuid_bytes PLACING _unix_ts_ms FROM 1 FOR 6);
+
+  -- set version 7
+  _uuid_bytes = set_byte(
+    _uuid_bytes,
+    6,
+    (b'0111' || get_byte(_uuid_bytes, 6)::bit(4))::bit(8)::int
+  );
+
+  RETURN encode(_uuid_bytes, 'hex')::uuid;
+END;
+$$;
+
+
+CREATE FUNCTION public.uuid_version(_uuid_bytes bytea)
+RETURNS integer
+LANGUAGE sql IMMUTABLE PARALLEL SAFE STRICT
+AS $$
+  SELECT get_byte(_uuid_bytes, 6)::bit(8)::bit(4)::int;
+$$;
+
+
+CREATE FUNCTION public.uuid_version(_uuid uuid)
+RETURNS integer
+LANGUAGE sql IMMUTABLE PARALLEL SAFE STRICT
+AS $$
+  SELECT uuid_version(uuid_send(_uuid));
+$$;
+
+
+CREATE FUNCTION public.timestamp_from_uuid_v7(_uuid uuid)
+RETURNS timestamptz
+LANGUAGE plpgsql IMMUTABLE PARALLEL SAFE STRICT
+AS $$
+DECLARE
+  _uuid_version integer;
+  _uuid_bytes bytea;
+BEGIN
+  SELECT uuid_send(_uuid) INTO _uuid_bytes;
+  SELECT uuid_version(_uuid_bytes) INTO _uuid_version;
+
+  IF _uuid_version != 7 THEN
+    RAISE EXCEPTION 'UUID must be version 7, not %', _uuid_version
+      USING HINT = 'You can only call this function with a UUID v7 input';
+  END IF;
+
+  RETURN to_timestamp(('x0000' || encode(
+    substring(_uuid_bytes FOR 4) || substring(_uuid_bytes FROM 5 FOR 2),
+    'hex'
+  ))::bit(64)::bigint::numeric / 1000);
+END;
+$$;
+
+
 CREATE TABLE swoop.payload_cache (
-  payload_uuid uuid DEFAULT gen_random_uuid() PRIMARY KEY,
-  payload_hash bytea UNIQUE,
-  workflow_version smallint NOT NULL,
+  payload_uuid uuid PRIMARY KEY CHECK (uuid_version(payload_uuid) = 5),
   workflow_name text NOT NULL,
   created_at timestamptz NOT NULL DEFAULT now(),
   invalid_after timestamptz
 );
 
-CREATE INDEX ON swoop.payload_cache (payload_hash);
-
 
 CREATE TABLE swoop.action (
-  action_uuid uuid NOT NULL DEFAULT gen_random_uuid(),
-  action_type text NOT NULL CHECK (action_type IN ('callback', 'workflow')),
   action_name text,
+  action_type text NOT NULL CHECK (action_type IN ('callback', 'workflow')),
+  action_uuid uuid NOT NULL DEFAULT gen_uuid_v7(now()),
+  created_at timestamptz NOT NULL DEFAULT now(),
   handler_name text NOT NULL,
+  handler_type text NOT NULL,
   parent_uuid uuid, -- reference omitted, we don't need referential integrity
-  created_at timestamptz NOT NULL DEFAULT now(),
-  priority smallint DEFAULT 100,
   payload_uuid uuid REFERENCES swoop.payload_cache ON DELETE RESTRICT,
+  priority smallint DEFAULT 100,
+  workflow_version smallint,
+
+  CONSTRAINT uuid_timestamp_matches_created_at CHECK (
+    timestamp_from_uuid_v7(action_uuid) = date_trunc('ms', created_at)
+  ),
 
   CONSTRAINT workflow_or_callback CHECK (
     CASE
       WHEN action_type = 'callback'
         THEN
           parent_uuid IS NOT NULL
           AND payload_uuid IS NULL
       WHEN action_type = 'workflow' THEN
         action_name IS NOT NULL
         AND payload_uuid IS NOT NULL
+        AND parent_uuid IS NULL
+        AND workflow_version IS NOT NULL
     END
   )
 ) PARTITION BY RANGE (created_at);
 
 CREATE INDEX ON swoop.action (created_at);
 CREATE INDEX ON swoop.action (action_uuid);
 CREATE INDEX ON swoop.action (handler_name);
@@ -108,15 +206,17 @@
   --   swoop.lock_thread(thread.lock_id)
   --   swoop.unlock_thread(thread.lock_id)
   lock_id integer GENERATED ALWAYS AS IDENTITY (
     SEQUENCE NAME swoop.thread_lock_id_seq
     MINVALUE -2147483648
     START WITH 1
     CYCLE
-  )
+  ),
+  started_at timestamptz
+
 ) PARTITION BY RANGE (created_at);
 
 CREATE INDEX ON swoop.thread (created_at);
 CREATE INDEX ON swoop.thread (action_uuid);
 CREATE INDEX ON swoop.thread (status);
 CREATE INDEX ON swoop.thread (handler_name);
 CREATE TABLE swoop.thread_template (LIKE swoop.thread);
@@ -153,30 +253,14 @@
   'event_time',
   'native',
   'monthly',
   p_template_table => 'swoop.event_template'
 );
 
 
-CREATE TABLE swoop.input_item (
-  item_uuid uuid PRIMARY KEY DEFAULT gen_random_uuid(),
-  item_id text NOT NULL,
-  collection text,
-  UNIQUE NULLS NOT DISTINCT (item_id, collection)
-);
-
-CREATE TABLE swoop.item_payload (
-  item_uuid uuid REFERENCES swoop.input_item ON DELETE RESTRICT,
-  payload_uuid uuid REFERENCES swoop.payload_cache ON DELETE CASCADE,
-  PRIMARY KEY (item_uuid, payload_uuid)
-);
-
-CREATE INDEX ON swoop.item_payload (item_uuid);
-
-
 CREATE FUNCTION swoop.add_pending_event()
 RETURNS trigger
 LANGUAGE plpgsql VOLATILE
 AS $$
 DECLARE
 BEGIN
   INSERT INTO swoop.event (event_time, action_uuid, status, event_source) VALUES
@@ -222,43 +306,45 @@
 
 CREATE FUNCTION swoop.update_thread()
 RETURNS trigger
 LANGUAGE plpgsql VOLATILE
 AS $$
 DECLARE
   _latest timestamptz;
-  _status text;
   _next_attempt timestamptz;
+  _started timestamptz;
 BEGIN
-  SELECT last_update FROM swoop.thread WHERE action_uuid = NEW.action_uuid INTO _latest;
+  SELECT last_update, started_at FROM swoop.thread WHERE action_uuid = NEW.action_uuid
+    INTO _latest, _started;
 
   -- If the event time is older than the last update we don't update the thread
   -- (we can't use a trigger condition to filter this because we don't know the
   -- last update time from the event alone).
   IF _latest IS NOT NULL AND NEW.event_time < _latest THEN
+    IF NEW.status = 'RUNNING' THEN
+        UPDATE swoop.thread as t SET started_at = NEW.event_time WHERE t.action_uuid = NEW.action_uuid;
+    END IF;
     RETURN NULL;
   END IF;
 
-  -- Coerce status to UNKNOWN if it doesn't match a known status type
-  SELECT name from swoop.event_state WHERE name = NEW.status
-  UNION
-  SELECT 'UNKNOWN'
-  LIMIT 1
-  INTO _status;
-
   -- If we need a next attempt time let's calculate it
   IF NEW.retry_seconds IS NOT NULL THEN
     SELECT NEW.event_time + (NEW.retry_seconds * interval '1 second') INTO _next_attempt;
   END IF;
 
+  IF _started IS NULL AND NEW.status = 'RUNNING' THEN
+    SELECT  NEW.event_time INTO _started;
+  END IF;
+
   UPDATE swoop.thread as t SET
     last_update = NEW.event_time,
-    status = _status,
+    status = NEW.status,
     next_attempt_after = _next_attempt,
-    error = NEW.error
+    error = NEW.error,
+    started_at = _started
   WHERE
     t.action_uuid = NEW.action_uuid;
 
   -- We _could_ try to drop the thread lock here, which would be nice for
   -- swoop-conductor so it didn't have to explicitly unlock, but the unlock
   -- function raises a warning. Being explicit isn't the worst thing either,
   -- given the complications with possible relocking and the need for clients
@@ -432,72 +518,46 @@
 BEGIN
   RETURN (
     SELECT pg_advisory_unlock(to_regclass('swoop.thread')::oid::integer, _lock_id)
   );
 END;
 $$;
 
-CREATE FUNCTION swoop.check_cache(
-  plhash bytea, wf_version smallint, wf_name text, invalid timestamptz
+
+CREATE FUNCTION swoop.find_cached_action_for_payload(
+  _payload_uuid uuid,
+  _wf_version smallint
 )
-RETURNS record
+RETURNS uuid
 LANGUAGE plpgsql VOLATILE
 AS $$
 DECLARE
-  rec RECORD;
+  v_status text;
+  n_version smallint;
+  d_invalid timestamptz;
+  v_action_id uuid;
 BEGIN
-    IF EXISTS (SELECT * FROM swoop.payload_cache WHERE payload_hash = plhash) THEN
-    -- An entry exists in the cache
-        DECLARE
-            v_status text;
-            v_job_id uuid;
-            v_payload_id uuid;
-        BEGIN
-            SELECT t.status, t.action_uuid, p.payload_uuid
-            INTO v_status, v_job_id, v_payload_id
-            FROM swoop.payload_cache p
-            INNER JOIN swoop.action a
-            ON p.payload_uuid = a.payload_uuid
-            INNER JOIN swoop.thread t
-            ON a.action_uuid = t.action_uuid
-            WHERE p.payload_hash = plhash
-            ORDER BY t.created_at DESC
-			LIMIT 1;
-
-            IF v_status IN ('RUNNING', 'PENDING', 'QUEUED', 'BACKOFF', 'SUCCESSFUL', 'INVALID') THEN
-            -- Redirect to job details for that workflow, and do not process
-                SELECT FALSE, v_job_id INTO rec;
-            ELSE
-            -- Reprocess payload
-                DECLARE
-                    n_version smallint;
-                    d_invalid timestamptz;
-                BEGIN
-                    SELECT workflow_version, invalid_after
-                    INTO n_version, d_invalid
-                    FROM   swoop.payload_cache
-                    WHERE  payload_hash = plhash;
-
-                    -- Check workflow version and invalidation
-                    IF wf_version > n_version OR d_invalid < NOW() THEN
-                        IF wf_version > n_version AND d_invalid < NOW() THEN
-                            UPDATE swoop.payload_cache SET workflow_version = wf_version, invalid_after = NULL WHERE payload_hash = plhash;
-                        ELSIF wf_version > n_version THEN
-                            UPDATE swoop.payload_cache SET workflow_version = wf_version WHERE payload_hash = plhash;
-                        ELSE
-                            UPDATE swoop.payload_cache SET invalid_after = NULL WHERE payload_hash = plhash;
-                        END IF;
-                    END IF;
-                    -- Reprocess payload with a new action_uuid
-                    SELECT TRUE, v_payload_id, gen_random_uuid() INTO rec;
-                END;
-            END IF;
-        END;
-	ELSE
-        -- Insert a new entry into cache table and process payload with a new action_uuid
-        INSERT INTO swoop.payload_cache(payload_hash, workflow_version, workflow_name, invalid_after)
-        VALUES (plhash, wf_version, wf_name, invalid)
-        RETURNING TRUE, payload_uuid, gen_random_uuid() INTO rec;
-	END IF;
-    RETURN rec;
+  SELECT t.status, a.workflow_version, p.invalid_after, a.action_uuid
+  INTO v_status, n_version, d_invalid, v_action_id
+  FROM swoop.payload_cache p
+  INNER JOIN swoop.action a
+  USING (payload_uuid)
+  INNER JOIN swoop.thread t
+  USING (action_uuid)
+  WHERE p.payload_uuid = _payload_uuid
+  ORDER BY t.created_at DESC
+  LIMIT 1;
+
+  IF v_status IN ('RUNNING', 'PENDING', 'QUEUED', 'BACKOFF') THEN
+  -- Redirect to job details for that workflow, and do not process
+    RETURN v_action_id;
+  ELSIF _wf_version > n_version THEN
+    RETURN null;
+  ELSIF d_invalid IS NOT NULL and d_invalid < now() THEN
+    RETURN null;
+  ELSIF v_status IN ('SUCCESSFUL', 'INVALID') THEN
+    RETURN v_action_id;
+  ELSE
+    RETURN null;
+  END IF;
 END;
 $$;
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `swoop.db-7.0.3/src/swoop/db/schema.sql` & `swoop.db-8.0.0/src/swoop/db/migrations/00008_new_base.up.sql`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-CREATE SCHEMA swoop;
-CREATE SCHEMA partman;
-CREATE EXTENSION pg_partman SCHEMA partman;
+CREATE SCHEMA IF NOT EXISTS swoop;
+CREATE SCHEMA IF NOT EXISTS partman;
+CREATE EXTENSION IF NOT EXISTS pg_partman SCHEMA partman;
 
 
 CREATE TABLE swoop.event_state (
   name text PRIMARY KEY,
   description text NOT NULL
 );
 
@@ -82,31 +82,31 @@
   RETURN encode(_uuid_bytes, 'hex')::uuid;
 END;
 $$;
 
 
 CREATE FUNCTION public.uuid_version(_uuid_bytes bytea)
 RETURNS integer
-LANGUAGE sql IMMUTABLE PARALLEL SAFE STRICT LEAKPROOF
+LANGUAGE sql IMMUTABLE PARALLEL SAFE STRICT
 AS $$
   SELECT get_byte(_uuid_bytes, 6)::bit(8)::bit(4)::int;
 $$;
 
 
 CREATE FUNCTION public.uuid_version(_uuid uuid)
 RETURNS integer
-LANGUAGE sql IMMUTABLE PARALLEL SAFE STRICT LEAKPROOF
+LANGUAGE sql IMMUTABLE PARALLEL SAFE STRICT
 AS $$
   SELECT uuid_version(uuid_send(_uuid));
 $$;
 
 
 CREATE FUNCTION public.timestamp_from_uuid_v7(_uuid uuid)
 RETURNS timestamptz
-LANGUAGE plpgsql IMMUTABLE PARALLEL SAFE STRICT LEAKPROOF
+LANGUAGE plpgsql IMMUTABLE PARALLEL SAFE STRICT
 AS $$
 DECLARE
   _uuid_version integer;
   _uuid_bytes bytea;
 BEGIN
   SELECT uuid_send(_uuid) INTO _uuid_bytes;
   SELECT uuid_version(_uuid_bytes) INTO _uuid_version;
@@ -129,24 +129,24 @@
   workflow_name text NOT NULL,
   created_at timestamptz NOT NULL DEFAULT now(),
   invalid_after timestamptz
 );
 
 
 CREATE TABLE swoop.action (
-  action_uuid uuid NOT NULL DEFAULT gen_uuid_v7(now()),
-  action_type text NOT NULL CHECK (action_type IN ('callback', 'workflow')),
   action_name text,
+  action_type text NOT NULL CHECK (action_type IN ('callback', 'workflow')),
+  action_uuid uuid NOT NULL DEFAULT gen_uuid_v7(now()),
+  created_at timestamptz NOT NULL DEFAULT now(),
   handler_name text NOT NULL,
+  handler_type text NOT NULL,
   parent_uuid uuid, -- reference omitted, we don't need referential integrity
-  created_at timestamptz NOT NULL DEFAULT now(),
-  priority smallint DEFAULT 100,
   payload_uuid uuid REFERENCES swoop.payload_cache ON DELETE RESTRICT,
-  workflow_version smallint NOT NULL,
-  handler_type text NOT NULL,
+  priority smallint DEFAULT 100,
+  workflow_version smallint,
 
   CONSTRAINT uuid_timestamp_matches_created_at CHECK (
     timestamp_from_uuid_v7(action_uuid) = date_trunc('ms', created_at)
   ),
 
   CONSTRAINT workflow_or_callback CHECK (
     CASE
@@ -154,14 +154,15 @@
         THEN
           parent_uuid IS NOT NULL
           AND payload_uuid IS NULL
       WHEN action_type = 'workflow' THEN
         action_name IS NOT NULL
         AND payload_uuid IS NOT NULL
         AND parent_uuid IS NULL
+        AND workflow_version IS NOT NULL
     END
   )
 ) PARTITION BY RANGE (created_at);
 
 CREATE INDEX ON swoop.action (created_at);
 CREATE INDEX ON swoop.action (action_uuid);
 CREATE INDEX ON swoop.action (handler_name);
```

### Comparing `swoop.db-7.0.3/src/swoop.db.egg-info/PKG-INFO` & `swoop.db-8.0.0/src/swoop.db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoop.db
-Version: 7.0.3
+Version: 8.0.0
 Summary: Database for STAC Workflow Open Orchestration Framework
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,stac,workflow,geospatial
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `swoop.db-7.0.3/tests/conftest.py` & `swoop.db-8.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/tests/fixtures/migrations/README.md` & `swoop.db-8.0.0/tests/fixtures/migrations/README.md`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/tests/pgtap/test_action.sql` & `swoop.db-8.0.0/tests/pgtap/test_action.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/tests/pgtap/test_find_cached_action_for_payload.sql` & `swoop.db-8.0.0/tests/pgtap/test_find_cached_action_for_payload.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/tests/pgtap/test_limit-locking.sql` & `swoop.db-8.0.0/tests/pgtap/test_limit-locking.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/tests/pgtap/test_uuid_v7.sql` & `swoop.db-8.0.0/tests/pgtap/test_uuid_v7.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/tests/test_database.py` & `swoop.db-8.0.0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.3/tests/test_migrations.py` & `swoop.db-8.0.0/tests/test_migrations.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,29 @@
-import re
 from pathlib import Path
 
 import pytest
 from dbami.pg_dump import pg_dump as _pg_dump
 
 from swoop.db import SwoopDB
 
 
 @pytest.fixture(scope="session")
 def migration_fixtures(pytestconfig) -> Path:
     return pytestconfig.rootpath.joinpath("tests", "fixtures", "migrations")
 
 
-def uuid_replacer(instr: str) -> str:
-    uuids: list[str] = re.findall(
-        r"'[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}'",
-        instr,
-    )
-
-    for index, uuid in enumerate(uuids):
-        instr = instr.replace(uuid, f"'uuid{index}'")
-
-    return instr
-
-
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     "start,end,result_editor",
     [
-        (0, 1, None),
-        (0, 2, None),
-        (2, 6, None),
-        (6, 7, uuid_replacer),
+        # (8, 9, None),
     ],
 )
 async def test_migration(start, end, result_editor, migration_fixtures, pg_dump):
-    if result_editor is None:
-
-        def result_editor(x):
-            return x
+    result_editor = (lambda x: x) if result_editor is None else result_editor
 
     fixture = migration_fixtures.joinpath(f"{start}_base_01.sql")
     result = migration_fixtures.joinpath(f"{end}_result.sql")
     DB_NAME = f"swoop_test_migration_{start}_{end}"
     test_db = SwoopDB()
 
     dump_args = [
```

