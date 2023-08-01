# Comparing `tmp/invenio-rdm-migrator-1.0.0a9.tar.gz` & `tmp/invenio-rdm-migrator-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-rdm-migrator-1.0.0a9.tar", last modified: Tue May  9 13:25:51 2023, max compression
+gzip compressed data, was "dist/invenio-rdm-migrator-2.0.0.tar", last modified: Tue Aug  1 12:46:07 2023, max compression
```

## Comparing `invenio-rdm-migrator-1.0.0a9.tar` & `invenio-rdm-migrator-2.0.0.tar`

### file list

```diff
@@ -1,114 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/extract/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/extract/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/load/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/load/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/load/ids.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/load/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8166 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/load/postgresql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/communities/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/communities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/communities/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/communities/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/communities/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/communities/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/files/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/files/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/files/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/files/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/files/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/table_generators/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/table_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/table_generators/drafts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/table_generators/parents.py
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/table_generators/records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/table_generators/versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/requests/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/requests/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/requests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/requests/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/requests/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/users/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/users/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/users/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/users/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/users/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/transform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-05-09 13:25:50.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:25:50.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:25:50.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-09 13:25:50.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-09 13:25:50.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/communities/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/communities/test_communities_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/communities/test_communities_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/communities/test_communities_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/files/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/files/test_files_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/files/test_files_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/files/test_files_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/records/
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/records/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/records/test_records_table_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/requests/
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/requests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/requests/test_requests_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/requests/test_requests_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/requests/test_requests_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/test_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16107 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/actions/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/extract/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/extract/jsonlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/extract/null.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/extract/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/bulk/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/bulk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/bulk/copy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/bulk/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/bulk/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/bulk/generators/existing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/bulk/generators/single.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/bulk/generators/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/sequences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/transactions/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/transactions/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/transactions/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/actions/drafts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/awards/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/awards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/awards/load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/communities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/communities/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/communities/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/communities/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/files/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/files/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/files/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/funders/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/funders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/funders/load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/awards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/communities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/funders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/pids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/oauth/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/oauth/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/drafts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/parents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/requests/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/requests/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/requests/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/users/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/users/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/users/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/transform/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/transform/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/transform/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/transform/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16107 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/tests/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/extract/test_base_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/extract/test_jsonlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/extract/test_null.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/tests/load/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/load/test_base_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/load/test_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/load/test_postgresql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/tests/streams/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/tests/streams/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/actions/test_drafts_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/tests/streams/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/communities/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/communities/test_communities_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/communities/test_communities_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/communities/test_communities_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/tests/streams/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/files/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/files/test_files_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/files/test_files_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/files/test_files_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/tests/streams/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/records/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17205 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/records/test_records_table_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/tests/streams/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/requests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/requests/test_requests_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/requests/test_requests_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/requests/test_requests_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/test_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/tests/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/transform/test_base_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/transform/test_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/transform/test_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/transform/test_transactions.py
```

### Comparing `invenio-rdm-migrator-1.0.0a9/.editorconfig` & `invenio-rdm-migrator-2.0.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a9/.github/workflows/pypi-publish.yml` & `invenio-rdm-migrator-2.0.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a9/.github/workflows/tests.yml` & `invenio-rdm-migrator-2.0.0/.github/workflows/tests.yml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         default: "Manual trigger"
 
 jobs:
   Tests:
     runs-on: ubuntu-20.04
     strategy:
       matrix:
-        python-version: [3.7, 3.8, 3.9]
+        python-version: [3.9]
         requirements-level: [pypi]
         db-service: [postgresql13]
         include:
           - db-service: postgresql13
             DB_EXTRAS: "postgresql"
 
     env:
```

### Comparing `invenio-rdm-migrator-1.0.0a9/CONTRIBUTING.rst` & `invenio-rdm-migrator-2.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a9/LICENSE` & `invenio-rdm-migrator-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a9/MANIFEST.in` & `invenio-rdm-migrator-2.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a9/PKG-INFO` & `invenio-rdm-migrator-2.0.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,314 +1,328 @@
-Metadata-Version: 2.1
-Name: invenio-rdm-migrator
-Version: 1.0.0a9
-Summary: InvenioRDM module for data migration.
-Home-page: https://github.com/inveniosoftware/invenio-rdm-migrator
-Author: CERN
-Author-email: info@inveniosoftware.org
-License: MIT
-Description: ..
-            Copyright (C) 2022 CERN.
-        
-        
-            Invenio-RDM-Migrator is free software; you can redistribute it and/or
-            modify it under the terms of the MIT License; see LICENSE file for more
-            details.
-        
-        =====================
-         Invenio-RDM-Migrator
-        =====================
-        
-        .. image:: https://github.com/inveniosoftware/invenio-rdm-migrator/workflows/CI/badge.svg
-                :target: https://github.com/inveniosoftware/invenio-rdm-migrator/actions?query=workflow%3ACI+branch%3Amaster
-        
-        .. image:: https://img.shields.io/github/tag/inveniosoftware/invenio-rdm-migrator.svg
-                :target: https://github.com/inveniosoftware/invenio-rdm-migrator/releases
-        
-        .. image:: https://img.shields.io/pypi/dm/invenio-rdm-migrator.svg
-                :target: https://pypi.python.org/pypi/invenio-rdm-migrator
-        
-        .. image:: https://img.shields.io/github/license/inveniosoftware/invenio-rdm-migrator.svg
-                :target: https://github.com/inveniosoftware/invenio-rdm-migrator/blob/master/LICENSE
-        
-        DataCite-based data model for Invenio.
-        
-        
-        Development
-        ===========
-        
-        Install
-        -------
-        
-        Make sure that you have `libpq-dev` installed in your system. See
-        `psycopg installation instructions <https://www.psycopg.org/install/>`_
-        for more information.
-        
-        Choose a version of search and database, then run:
-        
-        .. code-block:: console
-        
-            pip install -e .
-        
-        
-        Tests
-        -----
-        
-        .. code-block:: console
-        
-            ./run-tests.sh
-        
-        How to run it
-        =============
-        
-        To run the migration you need:
-        
-        - A running InvenioRDM instance.
-        - If your data contains references to other records (e.g. vocabularies),
-          then it is also required to run the setup step.
-        
-        .. code-block:: console
-        
-            invenio-cli services setup --force --no-demo-data
-        
-        - Install Invenio-RDM-Migrator, any other dependencies must be handled
-          in the Pipfile of your instance.
-        
-        .. code-block:: console
-        
-            $ pip install invenio-rdm-migrator
-        
-        - Create/edit the configuration file on your instance, for example
-          `streams.yaml`:
-        
-        .. code-block:: yaml
-        
-            records:
-                extract:
-                    filename: /path/to/records.json
-                load:
-                    db_uri: postgresql+psycopg2://inveniordm:inveniordm@localhost:5432/inveniordm
-                    tmp_dir: /tmp/migrator
-        
-        
-        - You will need to create a small python script
-          putting together the different blocks of the ETL. You can find an eample
-          at `my-site/site/my_site/migrator/__main__.py`.
-        
-        .. code-block:: python
-        
-            from invenio_rdm_migrator.streams import StreamDefinition
-            from invenio_rdm_migrator.streams.records import RDMRecordCopyLoad
-        
-            if __name__ == "__main__":
-                RecordStreamDefinition = StreamDefinition(
-                    name="records",
-                    extract_cls=JSONLExtract,
-                    transform_cls=ZenodoToRDMRecordTransform,
-                    load_cls=RDMRecordCopyLoad,
-                )
-        
-                runner = Runner(
-                    stream_definitions=[
-                        RecordStreamDefinition,
-                    ],
-                    config_filepath="path/to/your/streams.yaml",
-                )
-                runner.run()
-        
-        - Finally, you can execute the above code. Since it is in the `__main__` file
-          of the python package, you can run it as a module:
-        
-        .. code-block:: console
-        
-            $ python -m my_site.migrator
-        
-        - Once the migration has completed, in your instance you can reindex the data.
-          For example, for users and records it would look like:
-        
-        .. code-block:: console
-        
-            $ invenio-cli pyshell
-        
-            In [1]: from invenio_access.permissions import system_identity
-            In [2]: from invenio_rdm_records.proxies import current_rdm_records_service
-            In [3]: from invenio_users_resources.proxies import current_users_service
-        
-            In [4]: current_users_service.rebuild_index(identity=system_identity)
-            In [5]: current_rdm_records_service.rebuild_index(identity=system_identity)
-        
-        Implement your {Extract/Transform/Load}
-        =======================================
-        
-        There are for packages in this module `extract`, `transform`, `load`, and
-        `streams`. The first three correspond to the three steps of an ETL process.
-        The `streams` package contains the logic to run the process and different
-        stream-specific implementations of ETL classes (e.g. `records`).
-        
-        Extract
-        -------
-        
-        The extract is the first part of the data processing stream. It's
-        functionality is quite simple: return an iterator (e.g. of records), where each
-        yielded value is a dictionary. Note that the data in this step is _transformed_
-        to an extent, but only in format (e.g. JSON, XML), not in content. For example,
-        to implement a `XMLExtract` class:
-        
-        .. code-block:: python
-        
-            class XMLExtract(Extract):
-            ...
-        
-                def run(self):
-                    with open("file.xml") as file:
-                        for entry in file:
-                            yield xml.loads(entry)
-        
-        Transform
-        ---------
-        
-        The transformer is in charge of modifying the content to suit, in this case,
-        the InvenioRDM data model (e.g. for records) so it can be imported in the DB.
-        It will loop through the entries (i.e. the iterator returned by the extract
-        class), transform and yield (e.g. the record). Diving more in the example of
-        a record:
-        
-        To transform something to an RDM record, you need to implement
-        `streams/records/transform.py:RDMRecordTransform`. For each record it will
-        yield what is considered a semantically "full" record: the record itself,
-        its parent, its draft in case it exists and the files related them.
-        
-        .. code-block:: python
-        
+..
+    Copyright (C) 2022-2023 CERN.
+
+
+    Invenio-RDM-Migrator is free software; you can redistribute it and/or
+    modify it under the terms of the MIT License; see LICENSE file for more
+    details.
+
+=====================
+ Invenio-RDM-Migrator
+=====================
+
+.. image:: https://github.com/inveniosoftware/invenio-rdm-migrator/workflows/CI/badge.svg
+        :target: https://github.com/inveniosoftware/invenio-rdm-migrator/actions?query=workflow%3ACI+branch%3Amaster
+
+.. image:: https://img.shields.io/github/tag/inveniosoftware/invenio-rdm-migrator.svg
+        :target: https://github.com/inveniosoftware/invenio-rdm-migrator/releases
+
+.. image:: https://img.shields.io/pypi/dm/invenio-rdm-migrator.svg
+        :target: https://pypi.python.org/pypi/invenio-rdm-migrator
+
+.. image:: https://img.shields.io/github/license/inveniosoftware/invenio-rdm-migrator.svg
+        :target: https://github.com/inveniosoftware/invenio-rdm-migrator/blob/master/LICENSE
+
+DataCite-based data model for Invenio.
+
+
+Development
+===========
+
+Install
+-------
+
+Make sure that you have `libpq-dev` installed in your system. See
+`psycopg installation instructions <https://www.psycopg.org/install/>`_
+for more information.
+
+Choose a version of search and database, then run:
+
+.. code-block:: console
+
+    pip install -e .
+
+
+Tests
+-----
+
+.. code-block:: console
+
+    ./run-tests.sh
+
+How to run it
+=============
+
+To run the migration you need:
+
+- A running InvenioRDM instance.
+- If your data contains references to other records (e.g. vocabularies),
+  then it is also required to run the setup step.
+
+.. code-block:: console
+
+    invenio-cli services setup --force --no-demo-data
+
+- Install Invenio-RDM-Migrator, any other dependencies must be handled
+  in the Pipfile of your instance.
+
+.. code-block:: console
+
+    $ pip install invenio-rdm-migrator
+
+- Create/edit the configuration file on your instance, for example
+  `streams.yaml`:
+
+.. code-block:: yaml
+
+    data_dir: /path/to/data
+    tmp_dir: /path/to/tmp
+    state_dir: /path/to/state
+    log_dir: /path/to/logs
+    db_uri: postgresql+psycopg2://inveniordm:inveniordm@localhost:5432/inveniordm
+    old_secret_key: CHANGE_ME
+    new_secret_key: CHANGE_ME
+    records:
+        extract:
+            filename: /path/to/records.json
+
+
+- You will need to create a small python script
+  putting together the different blocks of the ETL. You can find an eample
+  at `my-site/site/my_site/migrator/__main__.py`.
+
+.. code-block:: python
+
+    from invenio_rdm_migrator.streams import StreamDefinition
+    from invenio_rdm_migrator.streams.records import RDMRecordCopyLoad
+
+    if __name__ == "__main__":
+        RecordStreamDefinition = StreamDefinition(
+            name="records",
+            extract_cls=JSONLExtract,
+            transform_cls=ZenodoToRDMRecordTransform,
+            load_cls=RDMRecordCopyLoad,
+        )
+
+        runner = Runner(
+            stream_definitions=[
+                RecordStreamDefinition,
+            ],
+            config_filepath="path/to/your/streams.yaml",
+        )
+
+        runner.run()
+
+- Finally, you can execute the above code. Since it is in the `__main__` file
+  of the python package, you can run it as a module:
+
+.. code-block:: console
+
+    $ python -m my_site.migrator
+
+- Once the migration has completed, in your instance you can reindex the data.
+  Following the records example above, it would look like:
+
+.. code-block:: console
+
+    $ invenio-cli pyshell
+
+    In [1]: from invenio_access.permissions import system_identity
+    In [2]: from invenio_rdm_records.proxies import current_rdm_records_service
+    In [3]: current_rdm_records_service.rebuild_index(identity=system_identity)
+
+ETL {Extract/Transform/Load} architecture
+=========================================
+
+There are four packages in this module `extract`, `transform`, `load`, and
+`streams`. The first three correspond to the three steps of an ETL process.
+The `streams` package contains the logic to run the process and different
+stream-specific implementations of ETL classes (e.g. `records`).
+
+Extract
+-------
+
+The extract is the first part of the data processing stream. It's
+functionality is quite simple: return an iterator (e.g. of records), where each
+yielded value is a dictionary. Note that the data in this step is _transformed_
+in format (e.g. JSON, XML), not in content. For example, the implementation of
+`XMLExtract` would look as follows:
+
+.. code-block:: python
+
+    class XMLExtract(Extract):
+    ...
+
+        def run(self):
+            with open("file.xml") as file:
+                for entry in file:
+                    yield xml.loads(entry)
+
+Transform
+---------
+
+The transformer is in charge of modifying the content to suit, in this case,
+the InvenioRDM data model (e.g. for records) so it can be imported in the DB.
+It will loop through the entries (i.e. the iterator returned by the extract
+class), transform and yield (e.g. the record). Diving more in the example of
+a record:
+
+To transform something to an RDM record, you need to implement
+`streams/records/transform.py:RDMRecordTransform`. For each record it will
+yield what is considered a semantically "full" record: the record itself,
+its parent, its draft in case it exists and the files related them.
+
+.. code-block:: python
+
+    {
+        "record": self._record(entry),
+        "draft": self._draft(entry),
+        "parent": self._parent(entry),
+        "record_files": self._record_files(entry),
+        "draft_files": self._draft_files(entry),
+    }
+
+This means that you will need to implement the functions for each key. Note
+that, only `_record` and `_parent` should return content, the others can return
+`None`.
+
+Some of these functions can themselves use a `transform/base:Entry`
+transformer. An _entry_ transformer is an extra layer of abstraction, to
+provide an interface with the methods needed to generate valid data for part of
+the `Transform` class. In the record example, you can implement
+`transform.base:RDMRecordEntry`, which can be used in the
+`RDMRecordTransform._record` function mentioned in the code snippet above. Note
+that implementing this interface will produce valid _data_ for a record.
+However, there is no abc for _metadata_. It is an open question how much we
+should define these interfaces and avoid duplicating the already existing
+Marshmallow schemas of InvenioRDM.
+
+At this point you might be wondering "Why not Marshmallow then?". The answer is
+"separation of responsibilities, performance and simplicity". The later lays
+with the fact that most of the data transformation is custom, so we would end
+up with a schema full of `Method` fields, which does not differ much from what
+we have but would have an impact on performance (Marshmallow is slow...).
+Regarding the responsibilities part, validating (mostly referential, like
+vocabularies) can only be done on (or after) _load_ where RDM instance knowledge/appctx
+is available.
+
+Note that no validation, not even structural, is done in this step.
+
+Load
+----
+
+The final step to have the records available in the RDM instance is to load
+them. There are two types of loading _bulk_ or _transactions_.
+
+Bulk
+....
+
+Bulk loading will insert data in the database table by table using `COPY`. Since
+the order of the tables is not guaranteed it is necessary to drop foreign keys before
+loading. They can be restored afterwards. In addition, dropping indices would increase
+performance since they will only be calculated once, when they are restored after loading.
+
+Bulk loading is done using the `load.postgresql.bulk:PostgreSQLCopyLoad` class, which will
+carry out 2 steps:
+
+1. Prepare the data, writing one DB row per line in a csv file:
+
+.. code-block:: console
+
+    $ /path/to/data/tables1668697280.943311
+        |
+        | - pidstore_pid.csv
+        | - rdm_parents_metadata.csv
+        | - rdm_records_metadata.csv
+        | - rdm_versions_state.csv
+
+2. Perform the actual loading, using `COPY`. Inserting all rows at once is more
+   efficient than performing one `INSERT` per row.
+
+Internally what is happening is that the `prepare` function makes use of
+`TableGenerator` implementations and then yields the list of csv files.
+So the `load` only iterates through the filenames, not the actual entries.
+
+A `TableGenerator` will, for each value in the iterator, yield one
+or more rows (lines to be written to the a csv file). For example for a record
+it will yield: recid, DOI and OAI (PersistentIdentifiers), record and parent
+metadata, etc. which will be written to the respective CSV file.
+
+
+Transactions
+............
+
+Another option is to migrate transactions. For example, once you have done the initial
+part of it in bulk, you can migrate the changes that were persisted while the bulk
+migration happened. That can be achieved by migrating transactions. A transaction is a
+group of operations, which can be understod as SQL statement and thus have two values:
+the operation type (created, update, delete) and its data represented as a database model.
+
+Transaction loading is done using the `load.postgresql.transactions:PostgreSQLExecuteLoad`
+class, which will carry out 2 similar steps to the one above:
+
+1. Prepare the data, storing in memory a series of `Operation`\s.
+2. Perform the actual loading by adding or removing from the session, or updating the
+   corresponding object. Each operation is flushed to the database to avoid foreing key
+   violations. However, each transaction is atomic, meaning that an error in one of the
+   operations will cause the full transaction to fail as a group.
+
+Internally, the load will use an instance of
+`load.postgresql.transactions.generators.group:TxGenerator` to prepare the
+operations. This class contains a mapping between table names and
+`load.postgresql.transactions.generators.row:RowGenerators`, which will return a list of
+operations with the data as database model in the `obj` attribute.
+
+Note that the `TxGenerator` is tightly coupled to the
+`transform.transactions.Tx` since it expects the dictionaries to have a
+specific structure:
+
+.. code-block::
+
+    {
+        "tx_id": the actual transaction id, useful for debug and error handling
+        "action": this information refers to the semantic meaning of the group
+                       for example: record metadata update or file upload
+        "operations": [
             {
-                "record": self._record(entry),
-                "draft": self._draft(entry),
-                "parent": self._parent(entry),
+                "op": c (create), u (update), d (delete)
+                "table": the name of the table in the source system (e.g. Zenodo)
+                "data": the transformed data, this can use any `Transform` implementation
             }
-        
-        This means that you will need to implement the functions for each key. Note
-        that, only `_record` and `_parent` should return content, the others can return
-        `None`. In this case we will need to re-think which methods should be
-        `abstractmethod` and which ones be defaulted to `None/{}/some other default` in
-        the base. You can find an example implementation at
-        `zenodo-rdm/site/zenodo_rdm/migrator/transform.py:ZenodoToRDMRecordTransform`.
-        
-        Some of these functions can themselves use a `transform/base:Entry`
-        transformer. An _entry_ transformer is a one layer deeper abstraction, to
-        provide an interface with the methods needed to generate valid data for part of
-        the `Transform` class. In the record example, you can implement
-        `transform.base:RDMRecordEntry`, which can be used in the
-        `RDMRecordTransform._record` function mentioned in the code snippet above. Note
-        that implementing this interface will produce valid _data_ for a record.
-        However, the _metadata_ is not interfaced. It is an open question how much we
-        should define these interfaces and avoid duplicating already existing
-        Marshmallow schemas.
-        
-        At this point you might be wondering "Why not Marshmallow then?". The answer is
-        "separation of responsibilities, performance and simplicity". The later lays
-        with the fact that most of the data transformation is custom, so we would end
-        up with a schema full of `Method` fields, which does not differ much from what
-        we have but would have an impact on performance (Marshmallow is slow...).
-        Regarding the responsibilities part, validating - mostly referential, like
-        vocabularies - can only be done on _load_ where RDM instance knowledge/appctx
-        is available.
-        
-        Note that no validation (not even structural) is done (at the moment) in this
-        step.
-        
-        Load
-        ----
-        
-        The final step to have the records available in the RDM instance is to load
-        them. The available `load/postgresql:PostgreSQLCopyLoad` will carry out 2 steps:
-        
-        - 1. Prepare the data, writing one DB row per line in a csv file:
-        
-        .. code-block:: console
-        
-            $ /path/to/data/tables1668697280.943311
-                |
-                | - pidstore_pid.csv
-                | - rdm_parents_metadata.csv
-                | - rdm_records_metadata.csv
-                | - rdm_versions_state.csv
-        
-        2. Perform the actual loading, using `COPY`. Inserting all rows at once is more
-           efficient than performing one `INSERT` per row.
-        
-        Internally what is happening is that the `prepare` function makes use of
-        `TableGenerator` implementations and then yields the list of csv files.
-        So the `load` only iterates through the filenames, not the actual entries.
-        
-        A `TableGenerator` will, for each value in the received iterator, yield one
-        or more rows (lines to be written to the a csv file). For example for a record
-        it will yield: recid, DOI and OAI (PersistentIdentifiers), record and parent
-        metadata, etc.
-        
-        Notes
-        =====
-        
-        **Shared cache between streams**
-        
-        During a migration run, there is a need to share information across different streams,
-        e.g populate communities before records and keep the map between community slug names
-        and autogenerated community ids, or at the same stream across different `TableGenerator`
-        instances, e.g on records stream we keep the "seen" parent ids so we can update the
-        information of the parent for different record versions.
-        For that reason, we pass a cache dict, that can change in the future in a type of
-        persistent storage e.g redis, in each `stream.load` step so streams can populate/consume
-        the cache.
-        The cache for each stream can also be populated in each stream configuration like below
-        in your `streams.yaml`:
-        
-        .. code-block:: yaml
-        
-            records:
-                extract:
-                    filename: /path/to/records.json
-                load:
-                    cache:
-                        communities:
-                            community_slug: <community_id>
-                    db_uri: postgresql+psycopg2://inveniordm:inveniordm@localhost:5432/inveniordm
-                    tmp_dir: /tmp/migrator
-        
-        When the runner will instantiate each stream will merge the existing state of the cache
-        with whatever is provided in the stream configuration. That means, that the stream
-        configuration takes precedence and can override the whole cache before the stream runs!
-        Any cache state that exists before is overridden for the rest of the migration run.
-        
-        **Infrastructure**
-        
-        While now we are chaining the iterator from one step into the other in the
-        streams, the idea is that all three steps will pull/push to/from queues so
-        they can be deployed in different parts of the system (e.g. the load part
-        in the worker nodes).
-        
-        **Others**
-        
-        - Using generators instead of lists, allows us to iterate through the data
-          only once and perform the E-T-L steps on them. Instead of loop for E, loop
-          for T, loop for L. In addition, this allows us to have the csv files open
-          during the writing and closing them at the end (open/close is an expensive
-          op when done 3M times).
-        
-        ..
-            Copyright (C) 2022 CERN.
-        
-        
-            Invenio-RDM-Migrator is free software; you can redistribute it and/or
-            modify it under the terms of the MIT License; see LICENSE file for more
-            details.
-        
-        Changes
-        =======
-        
-        Version 1.0.0
-        
-        - Initial public release.
-        
-Keywords: invenio rdm migration
-Platform: any
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.7
-Provides-Extra: tests
+        ]
+    }
+
+State
+=====
+
+During a migration run, there is a need to share information across different streams
+or different generators on the same stream. For example, the records stream needs to
+access the UUID to slug map that was populated on the communities stream; or the
+drafts generator needs to know which parent records have been created on the records
+generator to keep the version state consistent.
+
+All this information is persisted to a SQLite database. This state database is kept
+in memory during each stream processing, and it is persisted to disk if the stream
+finishes without errors. The state will be saved with the name of the stream
+(e.g. `records.db`) to avoid overwriting a previous state. Therefore, a migration can be
+restarted from any stream.
+
+There are two ways to add more information to the state:
+
+- Full entities, for example record or users, require their own DB table. Those must be
+  defined at `state.py:State._initialize_db`. In addition, to abstract the access to that
+  table, a state entity is required. It needs to be initialized in the `Runner.py:Runner`
+  constructor and added the the `state_entities` dictionary.
+- Independent value, for example the maximum value of generated primary keys. Those can be
+  stored in the `global_state`. This state has two columns: key and value; adding
+  information to it would look like `{key: name_of_the_value, value: actual_value}`.
+
+Notes
+=====
+
+**Using python generators**
+
+Using generators instead of lists, allows us to iterate through the data
+only once and perform the E-T-L steps on them. Instead of loop for E, loop
+for T, loop for L. In addition, this allows us to have the csv files open
+during the writing and closing them at the end (open/close is an expensive
+op when done 3M times).
```

### Comparing `invenio-rdm-migrator-1.0.0a9/docs/Makefile` & `invenio-rdm-migrator-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a9/docs/conf.py` & `invenio-rdm-migrator-2.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a9/docs/index.rst` & `invenio-rdm-migrator-2.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a9/docs/make.bat` & `invenio-rdm-migrator-2.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/communities/__init__.py` & `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/communities/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio RDM migration users stream."""
 
 from .load import CommunityCopyLoad
 from .transform import (
     CommunityEntry,
+    CommunityFileEntry,
     CommunityMemberEntry,
     CommunityTransform,
     FeaturedCommunityEntry,
     ParentCommunityEntry,
 )
 
 __all__ = (
     "CommunityCopyLoad",
     "CommunityEntry",
     "CommunityMemberEntry",
     "CommunityTransform",
+    "CommunityFileEntry",
     "FeaturedCommunityEntry",
     "ParentCommunityEntry",
 )
```

### Comparing `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/communities/transform.py` & `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/communities/transform.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,18 +26,24 @@
         pass
 
     @abstractmethod
     def _featured_community(self, entry):
         """Transform the featured community."""
         pass
 
+    @abstractmethod
+    def _community_files(self, entry):
+        """Transform the community files."""
+        pass
+
     def _transform(self, entry):
         """Transform a single entry."""
         return {
             "community": self._community(entry),
+            "community_files": self._community_files(entry),
             "community_members": self._community_members(entry),
             "featured_community": self._featured_community(entry),
         }
 
 
 class CommunityEntry(Entry):
     """Transform a single community entry."""
@@ -221,7 +227,52 @@
     def transform(self, entry):
         """Transform a featured community entry."""
         return {
             "created": self._created(entry),
             "updated": self._updated(entry),
             "start_date": self._start_date(entry),
         }
+
+
+class CommunityFileEntry(Entry):
+    """Transform a community file entry."""
+
+    @abstractmethod
+    def _created(self, entry):
+        """Returns the creation date."""
+        pass
+
+    @abstractmethod
+    def _updated(self, entry):
+        """Returns the update date."""
+        pass
+
+    @abstractmethod
+    def _id(self, entry):
+        """Returns the file id."""
+        pass
+
+    @abstractmethod
+    def _json(self, entry):
+        """Returns the file metadata."""
+        pass
+
+    @abstractmethod
+    def _version_id(self, entry):
+        """Returns the version id."""
+        pass
+
+    @abstractmethod
+    def _key(self, entry):
+        """Return the filepath."""
+        pass
+
+    def transform(self, entry):
+        """Transforms a community file entry."""
+        return {
+            "id": self._id(entry),
+            "json": self._json(entry),
+            "version_id": self._version_id(entry),
+            "key": self._key(entry),
+            "created": self._created(entry),
+            "updated": self._updated(entry),
+        }
```

### Comparing `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/files/__init__.py` & `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/files/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022 CERN.
+# Copyright (C) 2022-2023 CERN.
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio RDM migration users stream."""
 
-from .load import FilesCopyLoad
+from .load import ExistingFilesLoad, FilesCopyLoad
 from .transform import (
     FilesBucketEntry,
     FilesInstanceEntry,
     FilesObjectVersionEntry,
     FilesTransform,
 )
 
 __all__ = (
+    "ExistingFilesLoad",
     "FilesCopyLoad",
     "FilesBucketEntry",
     "FilesInstanceEntry",
     "FilesObjectVersionEntry",
     "FilesTransform",
 )
```

### Comparing `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/files/load.py` & `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/users/load.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2022 CERN.
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
-"""Invenio RDM migration files load module."""
+"""Invenio RDM migration users load module."""
 
-from ...load import PostgreSQLCopyLoad
-from .table_generator import FilesTableGenerator
+from ...load.postgresql.bulk import PostgreSQLCopyLoad
+from .table_generator import UserTableGenerator
 
 
-class FilesCopyLoad(PostgreSQLCopyLoad):
-    """PostgreSQL files COPY load."""
+class UserCopyLoad(PostgreSQLCopyLoad):
+    """PostgreSQL users COPY load."""
 
-    def __init__(self, db_uri=None, tmp_dir=None, cache=None):
+    def __init__(self, **kwargs):
         """Constructor."""
         super().__init__(
-            db_uri=db_uri,
             table_generators=[
-                FilesTableGenerator(),
+                UserTableGenerator(),
             ],
-            tmp_dir=tmp_dir,
+            **kwargs,
         )
-
-    def _validate(self):
-        """Validate data before loading."""
-        return True
```

### Comparing `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/files/table_generator.py` & `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/files/table_generator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022 CERN.
+# Copyright (C) 2022-2023 CERN.
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
-"""Invenio RDM migration user table load module."""
+"""Invenio RDM migration files table load module."""
 
-
-from ...load.postgresql import TableGenerator
-from .models import FilesBucket, FilesInstance, FilesObjectVersion
+from ...load.postgresql.bulk.generators import TableGenerator
+from ..models.files import FilesBucket, FilesInstance, FilesObjectVersion
 
 
 class FilesTableGenerator(TableGenerator):
-    """Files and related tables load."""
+    """Files and related tables load via CSV."""
 
     def __init__(self):
         """Constructor."""
         super().__init__(
             tables=[
                 FilesInstance,
                 FilesBucket,
```

### Comparing `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/files/transform.py` & `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/files/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/table_generators/drafts.py` & `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/records.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,170 +1,202 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2023 CERN.
+# Copyright (C) 2022-2023 CERN.
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio RDM migration record table load module."""
 
 from datetime import datetime
-from functools import partial
+from uuid import UUID
 
 from ....load.ids import generate_recid, generate_uuid, pid_pk
-from ....load.models import PersistentIdentifier
-from ....load.postgresql import TableGenerator
-from ..models import RDMDraftMetadata, RDMParentMetadata
+from ....load.postgresql.bulk.generators import TableGenerator
+from ....logging import Logger
+from ....state import STATE
+from ...models.communities import RDMParentCommunityMetadata
+from ...models.pids import PersistentIdentifier
+from ...models.records import RDMParentMetadata, RDMRecordFile, RDMRecordMetadata
 from .parents import generate_parent_rows
+from .references import CommunitiesReferencesMixin
 
 
-class RDMDraftTableGenerator(TableGenerator):
+def _is_valid_uuid(value):
+    try:
+        UUID(value)
+        return True
+    except:
+        return False
+
+
+def generate_files_uuids(data):
+    """Generate uuid for every file in the list.
+
+    Return the transformed list with the generated ids.
+    """
+    _files = data["record_files"]
+    for _file in _files:
+        _file["id"] = generate_uuid({})
+    return _files
+
+
+def generate_record_uuid(data):
+    """Generate record uuid if not present."""
+    _id = data["record"].get("id")
+    return _id if _id else generate_uuid(None)
+
+
+class RDMRecordTableGenerator(TableGenerator, CommunitiesReferencesMixin):
     """RDM Record and related tables load."""
 
-    def __init__(self, parents_cache, records_cache, communities_cache):
+    def __init__(self):
         """Constructor."""
         super().__init__(
             tables=[
-                RDMDraftMetadata,
-                RDMParentMetadata,
                 PersistentIdentifier,
+                RDMParentMetadata,
+                RDMRecordMetadata,
+                RDMParentCommunityMetadata,
+                RDMRecordFile,
             ],
             pks=[
-                ("draft.id", generate_uuid),
+                ("record.id", generate_record_uuid),
                 ("parent.id", generate_uuid),
-                ("draft.json.pid", partial(generate_recid, status="N")),
+                ("record.json.pid", generate_recid),
                 ("parent.json.pid", generate_recid),
-                ("draft.parent_id", lambda d: d["parent"]["id"]),
+                ("record.parent_id", lambda d: d["parent"]["id"]),
+                ("record_files", generate_files_uuids),
             ],
         )
-        self.parents_cache = parents_cache
-        self.records_cache = records_cache
-        self.communities_cache = communities_cache
 
     def _generate_rows(self, data, **kwargs):
         """Generates rows for a record."""
         now = datetime.utcnow().isoformat()
         parent = data["parent"]
-        draft = data.get("draft")
-        if not draft:
+        record = data.get("record")
+
+        if not record:
             return
 
-        # some legacy records have different pid value in deposit than record
-        # however _deposit.pid.value would contain the correct one
-        # if it is not legacy we get it from the current field (json.id)
-        recid = draft["json"]["id"]
-        forked_published = self.records_cache.get(recid)
-        cached_parent = self.parents_cache.get(parent["json"]["id"])
-        if not cached_parent:
-            self.parents_cache.add(
+        record_pid = record["json"]["pid"]
+
+        # parent
+        state_parent = STATE.PARENTS.get(parent["json"]["id"])
+        if not state_parent:
+            STATE.PARENTS.add(
                 parent["json"]["id"],  # recid
                 {
                     "id": parent["id"],
-                    "next_draft_id": draft["id"],
+                    "latest_index": record["index"],
+                    "latest_id": record["id"],
                 },
             )
-            # drafts have a parent on save
-            # on the other hand there is no community parent/request
             yield from generate_parent_rows(parent)
-        # if there is a parent (else) but there is no record it means that it is a
-        # draft of a new version
-        elif not forked_published:
-            self.parents_cache.update(
-                parent["json"]["id"],
-                {
-                    "next_draft_id": draft["id"],
-                },
-            )
+            # parent community
+            if "default" in parent["json"]["communities"]:
+                parent_def_id = parent["json"]["communities"]["default"]
+                parent_comm_id = parent["id"]
+                # when a community is deleted, its id is the slug and fails on DB
+                # FK expects uuid and not string
+                if _is_valid_uuid(parent_def_id) and _is_valid_uuid(parent_comm_id):
+                    yield RDMParentCommunityMetadata(
+                        community_id=parent_def_id,
+                        record_id=parent_comm_id,
+                        request_id=None,
+                    )
+                else:
+                    record_id = record["json"]["id"]
+                    logger = Logger.get_logger()
+                    logger.error(
+                        f"Record parent community not migrated. Record id[{record_id}]. parent community [{parent_comm_id}] parent default community [{parent_def_id}]."
+                    )
+        else:
+            if state_parent.get("latest_index") < record["index"]:
+                STATE.PARENTS.update(
+                    parent["json"]["id"],
+                    {
+                        "latest_index": record["index"],
+                        "latest_id": record["id"],
+                    },
+                )
 
-        # if its a draft of a published record, its parent should be parent id
-        # if its a new version, its parent should be the one of the previous version
-        # otherwise is a new parent (new record, new draft...)
-        parent_id = cached_parent["id"] if cached_parent else draft["parent_id"]
-        if forked_published:
-            parent_id = forked_published["parent_id"]
-
-        yield RDMDraftMetadata(
-            id=forked_published.get("id") or draft["id"],
-            json=draft["json"],
-            created=draft["created"],
-            updated=draft["updated"],
-            version_id=draft["version_id"],
-            index=forked_published.get("index") or draft["index"],
-            bucket_id=draft.get("bucket_id"),
-            parent_id=parent_id,
-            expires_at=draft["expires_at"],
-            fork_version_id=forked_published.get("fork_version_id")
-            or draft["fork_version_id"],
+        parent_id = state_parent["id"] if state_parent else record["parent_id"]
+        # record
+        STATE.RECORDS.add(
+            record["json"]["id"],  # recid
+            {
+                "index": record["index"],
+                "id": record["id"],  # uuid
+                "parent_id": parent_id,  # parent uuid
+                "fork_version_id": record["version_id"],
+                "pids": record["json"]["pids"],
+            },
         )
 
-        # if there is a record in the cache it means both recid and doi were already
-        # processed in the records table generator, a duplicate would violate unique
-        # constraints and cause the load to fail.
-        if not forked_published:
-            # recid
-            record_pid = draft["json"]["pid"]
+        yield RDMRecordMetadata(
+            id=record["id"],
+            json=record["json"],
+            created=record["created"],
+            updated=record["updated"],
+            version_id=record["version_id"],
+            index=record["index"],
+            bucket_id=record["bucket_id"],
+            parent_id=parent_id,
+        )
+        # recid
+        yield PersistentIdentifier(
+            id=record_pid["pk"],
+            pid_type=record_pid["pid_type"],
+            pid_value=record["json"]["id"],
+            status=record_pid["status"],
+            object_type=record_pid["obj_type"],
+            object_uuid=record["id"],
+            created=now,
+            updated=now,
+        )
+        # DOI
+        if "doi" in record["json"]["pids"]:
+            yield PersistentIdentifier(
+                id=pid_pk(),
+                pid_type="doi",
+                pid_value=record["json"]["pids"]["doi"]["identifier"],
+                status="R",
+                object_type="rec",
+                object_uuid=record["id"],
+                created=now,
+                updated=now,
+            )
+        # OAI
+        if "oai" in record["json"]["pids"]:
             yield PersistentIdentifier(
-                id=record_pid["pk"],
-                pid_type=record_pid["pid_type"],  # FIXME: in rdm both are recid?
-                pid_value=draft["json"]["id"],
-                status=record_pid["status"],
-                object_type=record_pid["obj_type"],
-                object_uuid=draft["id"],
+                id=pid_pk(),
+                pid_type="oai",
+                pid_value=record["json"]["pids"]["oai"]["identifier"],
+                status="R",
+                object_type="rec",
+                object_uuid=record["id"],
                 created=now,
                 updated=now,
             )
-        # we don't emit doi Persistentidentifier for drafts as either they have already
-        # one from records or have an external doi that is registered on publish
 
-    # FIXME: deduplicate with records.py
+        # record files
+        record_files = data["record_files"]
+        for _file in record_files:
+            yield RDMRecordFile(
+                id=_file["id"],
+                json=_file["json"],
+                created=_file["created"],
+                updated=_file["updated"],
+                version_id=_file["version_id"],
+                key=_file["key"],
+                record_id=record["id"],
+                object_version_id=_file["object_version_id"],
+            )
+
     def _resolve_references(self, data, **kwargs):
         """Resolve references e.g communities slug names."""
-
-        def _resolve_communities(communities):
-            default_slug = communities.get("default")
-            default_id = self.communities_cache.get(default_slug)
-            if not default_id:
-                # TODO: maybe raise error without correct default community?
-                communities = {}
-
-            communities["default"] = default_id
-
-            communities_slugs = communities.get("ids", [])
-            _ids = []
-            for slug in communities_slugs:
-                _id = self.communities_cache.get(slug)
-                if _id:
-                    _ids.append(_id)
-            communities["ids"] = _ids
-
-        def _resolve_pids(draft):
-            """Enforce record pids to draft."""
-            if not draft:
-                return
-
-            # some legacy records have different pid value in deposit than record
-            # however _deposit.pid.value would contain the correct one
-            # if it is not legacy we get it from the current field (json.id)
-            recid = draft["json"]["id"]
-            forked_published = self.records_cache.get(recid)
-            if forked_published:
-                pids = draft["json"]["pids"]
-                has_draft_external_doi = (
-                    pids.get("doi", {}).get("provider") == "external"
-                )
-                if has_draft_external_doi:
-                    # then keep the draft external value as it might be there for
-                    # updating the existing value. Update the draft only with `oai`
-                    pids["oai"] = forked_published["pids"]["oai"]
-                else:
-                    # enfore published record pids to draft
-                    pids = forked_published["pids"]
-
         # resolve parent communities slug
         parent = data["parent"]
         communities = parent["json"].get("communities")
         if communities:
-            _resolve_communities(communities)
-        _resolve_pids(data.get("draft"))
-
-    # FIXME: deduplicate with records.py
-    # assumis records post load alters pidstore_pid_id_seq and pidstore_recid_recid_seq
+            self.resolve_communities(communities)
```

### Comparing `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/table_generators/parents.py` & `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/parents.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,34 +5,35 @@
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio RDM migration parent table load module."""
 
 from datetime import datetime
 
-from ....load.models import PersistentIdentifier
-from ..models import RDMParentMetadata
+from ...models.pids import PersistentIdentifier
+from ...models.records import RDMParentMetadata
 
 
 def generate_parent_rows(parent):
     """Generates rows for a parent record."""
     now = datetime.utcnow().isoformat()
     parent_pid = parent["json"]["pid"]
-    # parent record
-    yield RDMParentMetadata(
-        id=parent["id"],
-        json=parent["json"],
-        created=parent["created"],
-        updated=parent["updated"],
-        version_id=parent["version_id"],
-    )
+    # order is important when doing action/streaming migration
     # parent recid
     yield PersistentIdentifier(
         id=parent_pid["pk"],
         pid_type=parent_pid["pid_type"],
         pid_value=parent["json"]["id"],
         status=parent_pid["status"],
         object_type=parent_pid["obj_type"],
         object_uuid=parent["id"],
         created=now,
         updated=now,
     )
+    # parent record
+    yield RDMParentMetadata(
+        id=parent["id"],
+        json=parent["json"],
+        created=parent["created"],
+        updated=parent["updated"],
+        version_id=parent["version_id"],
+    )
```

### Comparing `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/table_generators/versions.py` & `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/versions.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # Copyright (C) 2023 CERN.
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio RDM migration record table load module."""
 
-from ....load.postgresql import TableGenerator
-from ..models import RDMVersionState
+from ....load.postgresql.bulk.generators import TableGenerator
+from ....state import STATE
+from ...models.records import RDMVersionState
 
 
 class RDMVersionStateTableGenerator(TableGenerator):
     """RDM version state computed table."""
 
-    def __init__(self, parents_cache):
+    def __init__(self):
         """Constructor."""
         super().__init__(tables=[RDMVersionState])
-        self.parents_cache = parents_cache
 
     def _generate_rows(self, parent_entry, **kwargs):
         # Version state to be populated in the end from the final state
         yield RDMVersionState(
             latest_index=parent_entry["latest_index"],
             parent_id=parent_entry["id"],
             latest_id=parent_entry["latest_id"],
@@ -30,10 +30,10 @@
 
     def prepare(self, tmp_dir, entry, stack, output_files, **kwargs):
         """Compute rows."""
         # overwrite to avoid it using the parent class on a per
         pass
 
     def post_prepare(self, tmp_dir, stack, output_files, **kwargs):
-        """Overwrite entries with parent cache entries."""
-        for entry in self.parents_cache.all():
+        """Overwrite entries with parent state entries."""
+        for entry in STATE.PARENTS.all():
             super().prepare(tmp_dir, entry, stack, output_files, **kwargs)
```

### Comparing `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/transform.py` & `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,24 +51,14 @@
             "record": self._record(entry),
             "draft": self._draft(entry),
             "parent": self._parent(entry),
             "record_files": self._record_files(entry),
             "draft_files": self._draft_files(entry),
         }
 
-    def run(self, entries, logger=None):
-        """Transform and yield one element at a time."""
-        for entry in entries:
-            try:
-                yield self._transform(entry)
-            except Exception:
-                if logger:
-                    logger.error(entry, exc_info=1)
-                continue
-
 
 class RDMRecordEntry(Entry):
     """Transform a single record entry."""
 
     @abstractmethod
     def _id(self, entry):
         """Returns the rdm record uuid."""
@@ -104,14 +94,19 @@
 
     @abstractmethod
     def _pids(self, entry):
         """Returns the pids of the record."""
         pass
 
     @abstractmethod
+    def _bucket_id(self, entry):
+        """Returns the bucket id of the record."""
+        pass
+
+    @abstractmethod
     def _files(self, entry):
         """Transform the files of a record."""
         pass
 
     @abstractmethod
     def _access(self, entry):
         """Transform the access of a record."""
@@ -136,14 +131,15 @@
         """Transform a record single entry."""
         return {
             "id": self._id(entry),
             "created": self._created(entry),
             "updated": self._updated(entry),
             "version_id": self._version_id(entry),
             "index": self._index(entry),
+            "bucket_id": self._bucket_id(entry),
             "json": {
                 "id": self._recid(entry),
                 "pids": self._pids(entry),
                 "files": self._files(entry),
                 "metadata": self._metadata(entry),
                 "access": self._access(entry),
                 "custom_fields": self._custom_fields(entry),
@@ -193,14 +189,7 @@
             "created": self._created(entry),
             "updated": self._updated(entry),
             "json": self._json(entry),
             "version_id": self._version_id(entry),
             "key": self._key(entry),
             "object_version_id": self._object_version_id(entry),
         }
-
-
-class RDMDraftFileEntry(RDMRecordFileEntry):
-    """Transform a single record file entry.
-
-    Connects draft with files.
-    """
```

### Comparing `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/requests/load.py` & `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/communities/load.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,19 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2023 CERN.
+# Copyright (C) 2022 CERN.
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
-"""Invenio RDM migration requests load module."""
+"""Invenio RDM migration users load module."""
 
-from ...load import PostgreSQLCopyLoad
-from .table_generator import RequestTableGenerator
+from ...load.postgresql.bulk import PostgreSQLCopyLoad
+from .table_generator import CommunityTableGenerator
 
 
-class RequestCopyLoad(PostgreSQLCopyLoad):
-    """PostgreSQL COPY load."""
+class CommunityCopyLoad(PostgreSQLCopyLoad):
+    """PostgreSQL communities COPY load."""
 
-    def __init__(self, cache, db_uri, tmp_dir):
+    def __init__(self, **kwargs):
         """Constructor."""
-        self.communities_cache = cache.get("communities", {})
-        super().__init__(
-            db_uri=db_uri,
-            tmp_dir=tmp_dir,
-            table_generators=[
-                RequestTableGenerator(self.communities_cache),
-            ],
-        )
-
-    def _validate(self):
-        """Validate data before loading."""
-        pass
+        super().__init__(table_generators=[CommunityTableGenerator()], **kwargs)
```

### Comparing `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/requests/table_generator.py` & `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/requests/table_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 # Copyright (C) 2023 CERN.
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio RDM migration requests table load module."""
 
+
 from ...load.ids import generate_uuid
-from ...load.postgresql import TableGenerator
-from .models import RequestMetadata
+from ...load.postgresql.bulk.generators import TableGenerator
+from ...state import STATE
+from ..models.requests import RequestMetadata
 
 
 class RequestTableGenerator(TableGenerator):
     """Requests and related tables load."""
 
-    def __init__(self, communities_cache):
+    def __init__(self):
         """Constructor."""
         super().__init__(
             tables=[RequestMetadata],
             pks=[("id", generate_uuid)],
         )
-        self.communities_cache = communities_cache
 
     def _generate_rows(self, data, **kwargs):
         """Yield requests metadata."""
         request = data
         yield RequestMetadata(
             id=request["id"],
             json=request["json"],
@@ -38,18 +39,18 @@
 
     def _resolve_references(self, data, **kwargs):
         """Resolve references.
 
         Translates community slugs to uuids, and record parent pids to uuids. Both values
         are mandatory, therefore they are access as dict.
 
-        :raises: KeyError if the the parent or community are not found in the cache.
+        :raises: KeyError if the the parent or community are not found in the state.
         """
         # it assumes the data is transformed by an InclusionRequestEntry
         request_slug = data["json"]["receiver"]["community"]
-        community_id = self.communities_cache[request_slug]
+        community_id = STATE.COMMUNITIES.get(request_slug).get("id")
 
         data["json"]["receiver"]["community"] = community_id
 
     def prepare(self, tmp_dir, entry, stack, output_files, **kwargs):
         """Compute rows."""
         super().prepare(tmp_dir, entry, stack, output_files, create=True, **kwargs)
```

### Comparing `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/requests/transform.py` & `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/requests/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/runner.py` & `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/runner.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,103 +3,105 @@
 # Copyright (C) 2022 CERN.
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """InvenioRDM migration streams runner."""
 
-import logging
 from pathlib import Path
 
 import yaml
 
-from ..utils import ts
-from .cache import ParentsCache, RecordsCache
+from ..logging import Logger
+from ..state import STATE, StateDB
+from .records.state import ParentModelValidator
 from .streams import Stream
 
 
 class Runner:
     """ETL streams runner."""
 
     def _read_config(self, filepath):
         """Read config from file."""
         with open(filepath) as f:
             return yaml.safe_load(f)
 
     def __init__(self, stream_definitions, config_filepath):
         """Constructor."""
         config = self._read_config(config_filepath)
+
+        self.data_dir = Path(config.get("data_dir"))
+        self.data_dir.mkdir(parents=True, exist_ok=True)
+
         self.tmp_dir = Path(config.get("tmp_dir"))
         self.tmp_dir.mkdir(parents=True, exist_ok=True)
-        self.cache_dir = Path(config.get("cache_dir"))
-        self.cache_dir.mkdir(parents=True, exist_ok=True)
-        log_dir = Path(config["log_dir"]) if config.get("log_dir") else None
-        self.logger = None
-        if log_dir:
-            log_dir.mkdir(parents=True, exist_ok=True)
-            self.logger = logging.getLogger("migration")
-            self.logger.setLevel(logging.ERROR)
-            fh = logging.FileHandler(log_dir / "error.log")
-            fh.setLevel(logging.ERROR)
-            self.logger.addHandler(fh)
+
+        self.state_dir = Path(config.get("state_dir"))
+        self.state_dir.mkdir(parents=True, exist_ok=True)
+
+        self.log_dir = Path(config.get("log_dir"))
+        self.log_dir.mkdir(parents=True, exist_ok=True)
+
+        Logger.initialize(self.log_dir)
 
         self.db_uri = config.get("db_uri")
         self.streams = []
-        self.cache = {
-            "parents": ParentsCache(filepath=self.cache_dir / "parents.json"),
-            "records": RecordsCache(filepath=self.cache_dir / "records.json"),
-            "communities": {},
-        }
+        self.state = StateDB(
+            db_dir=self.state_dir, validators={"parents": ParentModelValidator}
+        )
+        STATE.initialized_state(self.state)
+        # set up secret keys
+        STATE.VALUES.add(
+            "old_secret_key",
+            {"value": bytes(config.get("old_secret_key"), "utf-8")},
+        )
+        STATE.VALUES.add(
+            "new_secret_key",
+            {"value": bytes(config.get("new_secret_key"), "utf-8")},
+        )
 
+        # start processing streams
         for definition in stream_definitions:
             if definition.name in config:
-                stream_config = config.get(definition.name)
-                if stream_config is not None:
-                    # merge cache objects from stream definition config
-                    stream_cache = stream_config.get("load", {}).pop("cache", {})
-                    self.cache.update(stream_cache)
-                    self.streams.append(
-                        Stream(
-                            definition.name,
-                            definition.extract_cls(**stream_config.get("extract", {})),
-                            definition.transform_cls(
-                                **stream_config.get("transform", {})
-                            ),
-                            definition.load_cls(
-                                cache=self.cache,
-                                tmp_dir=self.tmp_dir,
-                                db_uri=self.db_uri,
-                                **stream_config.get("load", {}),
-                            ),
-                            logger=self.logger,
-                        )
+                # get will return a None for e.g. files:
+                stream_config = config.get(definition.name) or {}
+                # merge state objects from stream definition config
+                existing_data = stream_config.get("existing_data", {})
+
+                # if loading pass source data dir, else pass tmp to dump new csv files
+                data_dir = self.data_dir
+                tmp_dir = self.tmp_dir / definition.name
+                extract = None
+                transform = None
+                if not existing_data:
+                    extract = definition.extract_cls(**stream_config.get("extract", {}))
+                    transform = definition.transform_cls(
+                        **stream_config.get("transform", {})
                     )
-                else:
-                    # stream is not based on config
-                    self.streams.append(
-                        Stream(
-                            definition.name,
-                            definition.extract_cls(),
-                            definition.transform_cls(),
-                            definition.load_cls(
-                                cache=self.cache,
-                                tmp_dir=self.tmp_dir,
-                                db_uri=self.db_uri,
-                            ),
-                            logger=self.logger,
-                        )
+
+                self.streams.append(
+                    Stream(
+                        definition.name,
+                        extract,
+                        transform,
+                        definition.load_cls(
+                            db_uri=self.db_uri,
+                            data_dir=data_dir,
+                            tmp_dir=tmp_dir,
+                            existing_data=existing_data,
+                            **stream_config.get("load", {}),
+                        ),
                     )
+                )
 
     def run(self):
         """Run ETL streams."""
         for stream in self.streams:
             try:
                 stream.run()
-                # sucessfully finished stream run, now we can dump that stream cache
-                for name, cache in self.cache.items():
-                    if name == "communities":  # FIXME: implement communities cache
-                        continue
-                    cache_file = self.cache_dir / f"{name}.json"
-                    cache.dump(cache_file)
+                # on successful stream run, persist state
+                self.state.save(filename=f"{stream.name}.db")
             except Exception:
-                self.logger.error(f"Stream {stream.name} failed.", exc_info=1)
+                Logger.get_logger().exception(
+                    f"Stream {stream.name} failed.", exc_info=1
+                )
                 continue
```

### Comparing `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/users/table_generator.py` & `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/users/table_generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio RDM migration user table load module."""
 
 
-from ...load.postgresql import TableGenerator
-from .models import LoginInformation, User, UserIdentity
+from ...load.postgresql.bulk.generators import TableGenerator
+from ..models.users import LoginInformation, User, UserIdentity
 
 
 class UserTableGenerator(TableGenerator):
     """User and related tables load."""
 
     def __init__(self):
         """Constructor."""
```

### Comparing `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/users/transform.py` & `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/users/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/transform/base.py` & `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/transform/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,39 +5,44 @@
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio RDM migration transform interfaces."""
 
 from abc import ABC, abstractmethod
 
+from ..logging import Logger
+
 
 class Transform(ABC):
     """Base class for data transformation."""
 
     @abstractmethod
-    def _transform(self, entry):
-        """Transform entry."""
+    def _transform(self, entry):  # pragma: no cover
+        """Transform entry.
+
+        :returns: a transformed entry, not an iterator.
+        """
         pass
 
-    def run(self, entries, logger=None):
+    def run(self, entries):
         """Transform and yield one element at a time."""
         for entry in entries:
             try:
                 yield self._transform(entry)
             except Exception:
-                if logger:
-                    logger.error(entry, exc_info=1)
+                logger = Logger.get_logger()
+                logger.exception(entry, exc_info=1)
                 continue
 
 
 class Entry(ABC):
     """Base entry class."""
 
     @abstractmethod
-    def transform(self, entry):
+    def transform(self, entry):  # pragma: no cover
         """Transform entry."""
         pass
 
 
 def drop_nones(data):
     """Recursively drop Nones in dict d and return a new dictionary."""
     dd = {}
```

### Comparing `invenio-rdm-migrator-1.0.0a9/run-tests.sh` & `invenio-rdm-migrator-2.0.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a9/setup.cfg` & `invenio-rdm-migrator-2.0.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 
 [options]
 include_package_data = True
 packages = find:
 python_requires = >=3.7
 zip_safe = False
 install_requires = 
-	invenio-records[postgresql]>=2.0.1
-	psycopg>=3.1.4
+	jsonlines>=3.1.0
+	sqlalchemy>=2.0  # note this will be incompatible with InvenioRDM (see invenio-db)
+	sqlalchemy-utils[encrypted]>=0.38.3
+	psycopg>=3.1.9
 	PyYAML>=5.4.1
 
 [options.extras_require]
 tests = 
 	check-manifest>=0.25
 	coverage>=4.0,<5.0.0
 	dictdiffer>=0.9.0
```

### Comparing `invenio-rdm-migrator-1.0.0a9/tests/streams/communities/conftest.py` & `invenio-rdm-migrator-2.0.0/tests/streams/requests/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,49 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2023 CERN.
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
-"""Community stream fixtures."""
+
+"""Pytest requests configuration."""
 
 from copy import deepcopy
 
 import pytest
 
 
 @pytest.fixture(scope="module")
-def transformed_community_entry():
-    """Community data as after being transformed."""
+def transformed_incl_req_entry():
+    """Request data as after being transformed.
+
+    `topic`, `receiver` and `created_by` could be different.
+    This is a sample inclusion request for a record into a community.
+    """
     return {
-        "community": {
-            "created": "2023-01-01 12:00:00.00000",
-            "updated": "2023-01-31 12:00:00.00000",
-            "slug": "migrator",
-            "version_id": 1,
-            "json": {
-                "title": "Migrator community",
-                "description": "Migrator testing community",
-                "page": "",
-                "curation_policy": "",
-            },
-            "bucket_id": 1,
+        "created": "01/01/2023",
+        "updated": "01/01/2023",
+        "version_id": "1",
+        "json": {
+            "type": "community-inclusion",
+            "title": "title",
+            "topic": {"record": "123456"},
+            "status": "submitted",
+            "receiver": {"community": "comm"},
+            "created_by": {"user": "3"},
+            "$schema": "local://requests/request-v1.0.0.json",
         },
-        "community_members": [
-            {
-                "created": "2023-01-01 12:00:00.00000",
-                "updated": "2023-01-31 12:00:00.00000",
-                "json": {},
-                "version_id": 1,
-                "role": "owner",
-                "visible": True,
-                "active": True,
-                "user_id": 1,
-                "group_id": None,
-                "request_id": None,
-            }
-        ],
-        "featured_community": {},
+        "number": "1",
+        "expires_at": "01/01/2023",
     }
 
 
 @pytest.fixture(scope="module")
-def transformed_community_entry_pks(transformed_community_entry):
+def transformed_incl_req_entry_pks(transformed_incl_req_entry):
     """Request data as after being transformed and passed by generate_pks.
 
     The last step would happen in the table_generator._prepare.
     """
-    data = deepcopy(transformed_community_entry)
-    data["community"]["id"] = "12345678-abcd-1a2b-3c4d-123abc456def"
-    data["community_members"][0]["id"] = "12345678-abcd-1a2b-3c4d-123abc456def"
+    data = deepcopy(transformed_incl_req_entry)
+    data["id"] = "12345678-abcd-1a2b-3c4d-123abc456def"
 
     return data
```

### Comparing `invenio-rdm-migrator-1.0.0a9/tests/streams/communities/test_communities_load.py` & `invenio-rdm-migrator-2.0.0/tests/streams/requests/test_requests_load.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,54 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2023 CERN.
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
-"""Communities load tests."""
+"""Requests load tests."""
 
 import os
 from unittest.mock import patch
 
 import pytest
 
-from invenio_rdm_migrator.streams.communities import CommunityCopyLoad
+from invenio_rdm_migrator.streams.requests import RequestCopyLoad
 
 
 @pytest.fixture(scope="function")
-def community_copy_load(cache, tmp_dir):
-    """Community load instance."""
+def request_copy_load(communities_state, tmp_dir):
+    """Request load instance."""
     # the db queries will be mocked
-    load = CommunityCopyLoad(cache, "None", tmp_dir.name)
+    load = RequestCopyLoad(db_uri="None", tmp_dir=tmp_dir.name)
     yield load
     load._cleanup()
 
 
 @patch(
     "invenio_rdm_migrator.load.ids.uuid4",
     lambda: "12345678-abcd-1a2b-3c4d-123abc456def",
 )
-def test_community_load_prepare(community_copy_load, transformed_community_entry):
+def test_request_load_prepare(request_copy_load, transformed_incl_req_entry):
     """Test the table preparation (file creation)."""
-    tables = list(community_copy_load._prepare([transformed_community_entry]))
+    tables = [
+        table for _, table in request_copy_load._prepare([transformed_incl_req_entry])
+    ]
 
     # assert tables
-    # it has three tables: communities, parent communities and members
-    expected_table_names = [
-        "community_metadata",
-        "communities_members",
-        "rdm_parents_community",
-    ]
-    table_names = [table._table_name for table in tables]
-    assert len(tables) == len(expected_table_names)
-    assert any([e_table in table_names for e_table in expected_table_names])
+    assert len(tables) == 1
+    assert tables[0].__tablename__ == "request_metadata"
 
     # assert files were created and have the content
-    # two files are created: one for the communities and another for members
-    files = list(os.scandir(community_copy_load.tmp_dir))
-    assert len(files) == 2
+    files = list(os.scandir(request_copy_load.tmp_dir))
+    assert len(files) == 1
 
-    # assert communities metadata content
-    with open(f"{community_copy_load.tmp_dir}/communities_metadata.csv", "r") as file:
+    # assert request metadata content
+    with open(f"{request_copy_load.tmp_dir}/request_metadata.csv", "r") as file:
         # uuid, json, created, updated, version_id, number, expired_at
         expected = (
             "12345678-abcd-1a2b-3c4d-123abc456def,"
-            '2023-01-01 12:00:00.00000,2023-01-31 12:00:00.00000,"{""title"": ""Migrator community"", ""description"": ""Migrator testing community"", ""page"": """", ""curation_policy"": """"}",1,migrator,1\n'
+            '"{""type"": ""community-inclusion"", ""title"": ""title"", ""topic"": {""record"": ""123456""}, ""status"": ""submitted"", ""receiver"": {""community"": ""12345678-abcd-1a2b-3c4d-123abc456def""}, ""created_by"": {""user"": ""3""}, ""$schema"": ""local://requests/request-v1.0.0.json""}"'
+            ",01/01/2023,01/01/2023,1,1,01/01/2023\n"
         )
         content = file.read()
         assert content == expected
-
-    # assert communities members content
-    with open(f"{community_copy_load.tmp_dir}/communities_members.csv", "r") as file:
-        # uuid, json, created, updated, version_id, number, expired_at
-        expected = "12345678-abcd-1a2b-3c4d-123abc456def,2023-01-01 12:00:00.00000,2023-01-31 12:00:00.00000,{},1,owner,True,True,12345678-abcd-1a2b-3c4d-123abc456def,1,,\n"
-        content = file.read()
-        assert content == expected
```

### Comparing `invenio-rdm-migrator-1.0.0a9/tests/streams/communities/test_communities_table_generator.py` & `invenio-rdm-migrator-2.0.0/tests/streams/communities/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,91 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2023 CERN.
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
-
-"""Communities table generator tests."""
-
+"""Community stream fixtures."""
 
 from copy import deepcopy
 
-import dictdiffer
-
-from invenio_rdm_migrator.streams.communities.load import CommunityTableGenerator
-from invenio_rdm_migrator.streams.communities.models import Community, CommunityMember
+import pytest
 
 
-def test_generate_rows(transformed_community_entry_pks):
-    """Test the row generation of the request table generator."""
-    tg = CommunityTableGenerator({})  # no need for cache in this test
-    rows = list(tg._generate_rows(transformed_community_entry_pks))
-    expected_rows = [
-        Community(
-            id="12345678-abcd-1a2b-3c4d-123abc456def",
-            created="2023-01-01 12:00:00.00000",
-            updated="2023-01-31 12:00:00.00000",
-            json={
+@pytest.fixture(scope="module")
+def transformed_community_entry():
+    """Community data as after being transformed."""
+    return {
+        "community": {
+            "created": "2023-01-01 12:00:00.00000",
+            "updated": "2023-01-31 12:00:00.00000",
+            "slug": "migrator",
+            "version_id": 1,
+            "json": {
                 "title": "Migrator community",
                 "description": "Migrator testing community",
                 "page": "",
                 "curation_policy": "",
             },
-            version_id=1,
-            slug="migrator",
-            bucket_id=1,
-        ),
-        CommunityMember(
-            id="12345678-abcd-1a2b-3c4d-123abc456def",
-            created="2023-01-01 12:00:00.00000",
-            updated="2023-01-31 12:00:00.00000",
-            json={},
-            version_id=1,
-            role="owner",
-            visible=True,
-            active=True,
-            community_id="12345678-abcd-1a2b-3c4d-123abc456def",
-            user_id=1,
-            group_id=None,
-            request_id=None,
-        ),
-    ]
+            "bucket_id": 1,
+        },
+        "community_members": [
+            {
+                "created": "2023-01-01 12:00:00.00000",
+                "updated": "2023-01-31 12:00:00.00000",
+                "json": {},
+                "version_id": 1,
+                "role": "owner",
+                "visible": True,
+                "active": True,
+                "user_id": 1,
+                "group_id": None,
+                "request_id": None,
+            }
+        ],
+        "featured_community": {},
+        "community_files": {
+            "file": {
+                "created": "2023-01-01 12:00:00.00000",
+                "updated": "2023-01-31 12:00:00.00000",
+                "id": "1",
+                "json": {},
+                "version_id": 1,
+                "key": "logo",
+            },
+            "bucket": {
+                "created": "2023-01-01 12:00:00.00000",
+                "updated": "2023-01-31 12:00:00.00000",
+                "default_location": None,
+                "default_storage_class": "L",
+                "size": 0,
+                "quota_size": 0,
+                "max_file_size": 0,
+                "locked": False,
+                "deleted": False,
+                "id": 1,
+            },
+            "file_object": {
+                "created": "2023-01-01 12:00:00.00000",
+                "updated": "2023-01-31 12:00:00.00000",
+                "bucket_id": 1,
+                "version_id": 1,
+                "key": "logo",
+                "file_id": 1,
+                "_mimetype": None,
+                "is_head": True,
+            },
+        },
+    }
+
+
+@pytest.fixture(scope="module")
+def transformed_community_entry_pks(transformed_community_entry):
+    """Request data as after being transformed and passed by generate_pks.
+
+    The last step would happen in the table_generator._prepare.
+    """
+    data = deepcopy(transformed_community_entry)
+    data["community"]["id"] = "7357c033-abcd-1a2b-3c4d-123abc456def"
+    data["community_members"][0]["id"] = "12345678-abcd-1a2b-3c4d-123abc456def"
 
-    assert rows == expected_rows
+    return data
```

### Comparing `invenio-rdm-migrator-1.0.0a9/tests/streams/communities/test_communities_transform.py` & `invenio-rdm-migrator-2.0.0/tests/streams/communities/test_communities_transform.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,22 +23,34 @@
         """Tramsform the community members."""
         return {"key": "value"}
 
     def _featured_community(self, entry):
         """Transform the featured community."""
         return {"key": "value"}
 
+    def _community_files(self, entry):
+        return {
+            "file": {"key": "value"},
+            "bucket": {"key": "value"},
+            "file_object": {"key": "value"},
+        }
+
 
 def test_community_transform():
     """Test the full community transformation."""
     result = MockCommunityTransform()._transform({})
     expected = {
         "community": {"key": "value"},
         "community_members": {"key": "value"},
         "featured_community": {"key": "value"},
+        "community_files": {
+            "file": {"key": "value"},
+            "bucket": {"key": "value"},
+            "file_object": {"key": "value"},
+        },
     }
     assert not list(dictdiffer.diff(result, expected))
 
 
 class MockCommunityEntry(CommunityEntry):
     """Transform a single mock community entry."""
```

### Comparing `invenio-rdm-migrator-1.0.0a9/tests/streams/files/conftest.py` & `invenio-rdm-migrator-2.0.0/tests/streams/files/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a9/tests/streams/files/test_files_load.py` & `invenio-rdm-migrator-2.0.0/tests/streams/files/test_files_load.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,32 +15,32 @@
 from invenio_rdm_migrator.streams.files import FilesCopyLoad
 
 
 @pytest.fixture(scope="function")
 def files_copy_load(tmp_dir):
     """Request load instance."""
     # the db queries will be mocked
-    load = FilesCopyLoad(cache={}, db_uri="None", tmp_dir=tmp_dir.name)
+    load = FilesCopyLoad(db_uri="None", tmp_dir=tmp_dir.name)
     yield load
     load._cleanup()
 
 
 @patch(
     "invenio_rdm_migrator.load.ids.uuid4",
     lambda: "12345678-abcd-1a2b-3c4d-123abc456def",
 )
 def test_files_load_prepare(files_copy_load, transformed_files_entry):
     """Test the table preparation (file creation)."""
-    tables = list(files_copy_load._prepare([transformed_files_entry]))
+    tables = [table for _, table in files_copy_load._prepare([transformed_files_entry])]
 
     # assert tables
     assert len(tables) == 3
-    assert tables[0]._table_name == "files_files"
-    assert tables[1]._table_name == "files_bucket"
-    assert tables[2]._table_name == "files_object"
+    assert tables[0].__tablename__ == "files_files"
+    assert tables[1].__tablename__ == "files_bucket"
+    assert tables[2].__tablename__ == "files_object"
 
     # assert files were created and have the content
     files = list(os.scandir(files_copy_load.tmp_dir))
     assert len(files) == 3
 
     # assert files bucket content
     with open(f"{files_copy_load.tmp_dir}/files_bucket.csv", "r") as file:
```

### Comparing `invenio-rdm-migrator-1.0.0a9/tests/streams/files/test_files_table_generator.py` & `invenio-rdm-migrator-2.0.0/tests/streams/files/test_files_table_generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Requests table generator tests."""
 
 from invenio_rdm_migrator.streams.files.load import FilesTableGenerator
-from invenio_rdm_migrator.streams.files.models import (
+from invenio_rdm_migrator.streams.models.files import (
     FilesBucket,
     FilesInstance,
     FilesObjectVersion,
 )
 
 
 def test_generate_rows(transformed_files_entry):
```

### Comparing `invenio-rdm-migrator-1.0.0a9/tests/streams/files/test_files_transform.py` & `invenio-rdm-migrator-2.0.0/tests/streams/files/test_files_transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a9/tests/streams/records/conftest.py` & `invenio-rdm-migrator-2.0.0/tests/streams/records/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         },
         "record": {
             "id": "2d6970ea-602d-4e8b-a918-063a59823386",
             "created": "2023-01-01 12:00:00.00000",
             "updated": "2023-01-31 12:00:00.00000",
             "version_id": 1,
             "index": 1,
+            "bucket_id": "bur3c0rd-1234-abcd-1ab2-1234abcd56ef",
             "json": {
                 "id": "12345678",
                 "pids": {
                     "oai": {
                         "provider": "oai",
                         "identifier": "oai:zenodo.org:12345678",
                     },
@@ -56,28 +57,28 @@
 
     It also includes generated PKs and resolved references.
     """
     data = deepcopy(transformed_record_entry)
     data["parent"]["id"] = "12345678-abcd-1a2b-3c4d-123abc456def"
     data["record"]["parent_id"] = "12345678-abcd-1a2b-3c4d-123abc456def"
     data["parent"]["json"]["pid"] = {
-        "pk": "10122",  # pk, not pid value
+        "pk": 1_000_000,  # pk, not pid value
         "obj_type": "rec",
         "pid_type": "recid",
         "status": "R",
     }
     data["parent"]["json"]["communities"] = {
         "ids": [
             "12345678-abcd-1a2b-3c4d-123abc456def",
             "12345678-abcd-1a2b-3c4d-123abc123abc",
         ],
         "default": "12345678-abcd-1a2b-3c4d-123abc456def",
     }
     data["record"]["json"]["pid"] = {
-        "pk": "10123",  # pk, not pid value
+        "pk": 1_000_001,  # pk, not pid value
         "obj_type": "rec",
         "pid_type": "recid",
         "status": "R",
     }
 
     return data
 
@@ -97,52 +98,53 @@
         },
         "draft": {
             "id": "2d6970ea-602d-4e8b-a918-063a59823386",
             "created": "2023-01-01 12:00:00.00000",
             "updated": "2023-01-31 12:00:00.00000",
             "version_id": 1,
             "index": 1,
+            "bucket_id": "bud3p0s1-1234-abcd-1ab2-1234abcd56ef",
             "json": {
                 "id": "12345678",
                 "pids": {
                     "doi": {
                         "provider": "external",
                         "identifier": "10.1234/foo",
                     },
                 },
             },
             "expires_at": "2024-01-01 12:00:00.00000",
             "fork_version_id": None,
         },
-        "record_files": {},
+        "draft_files": {},
     }
 
 
 @pytest.fixture(scope="function")
 def transformed_draft_entry_pks(transformed_draft_entry):
     """Draft data as after being transformed.
 
     It also includes generated PKs and resolved references.
     """
     data = deepcopy(transformed_draft_entry)
     data["parent"]["id"] = "12345678-abcd-1a2b-3c4d-123abc456def"
     data["draft"]["parent_id"] = "12345678-abcd-1a2b-3c4d-123abc456def"
     data["parent"]["json"]["pid"] = {
-        "pk": "10122",
+        "pk": 1_000_000,
         "obj_type": "rec",
         "pid_type": "recid",
         "status": "N",
     }
     data["parent"]["json"]["communities"] = {
         "ids": [
             "12345678-abcd-1a2b-3c4d-123abc456def",
             "12345678-abcd-1a2b-3c4d-123abc123abc",
         ],
         "default": "12345678-abcd-1a2b-3c4d-123abc456def",
     }
     data["draft"]["json"]["pid"] = {
-        "pk": "10123",
+        "pk": 1_000_001,
         "obj_type": "rec",
         "pid_type": "recid",
         "status": "N",
     }
     return data
```

### Comparing `invenio-rdm-migrator-1.0.0a9/tests/streams/records/test_records_table_generator.py` & `invenio-rdm-migrator-2.0.0/tests/streams/records/test_records_table_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,27 +6,30 @@
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Records/Drafts table generator tests."""
 
 from copy import deepcopy
 from unittest.mock import patch
 
-import pytest
-
-from invenio_rdm_migrator.load.models import PersistentIdentifier
-from invenio_rdm_migrator.streams.communities.models import RDMParentCommunityMetadata
-from invenio_rdm_migrator.streams.records.load import (
-    RDMDraftTableGenerator,
-    RDMRecordTableGenerator,
-)
-from invenio_rdm_migrator.streams.records.models import (
+from invenio_rdm_migrator.load.ids import pid_pk
+from invenio_rdm_migrator.streams.models.communities import RDMParentCommunityMetadata
+from invenio_rdm_migrator.streams.models.pids import PersistentIdentifier
+from invenio_rdm_migrator.streams.models.records import (
     RDMDraftMetadata,
     RDMParentMetadata,
     RDMRecordMetadata,
 )
+from invenio_rdm_migrator.streams.records.load import (
+    RDMDraftTableGenerator,
+    RDMRecordTableGenerator,
+)
+
+# IMPORTANT NOTE: since the resolve references method would be called externally
+# (i.e. not by generate_rows) not all pid pk have consistent values coming from
+# pid_pk(). Therefore, some calls are made at the beginning of the tests.
 
 
 class MockUTCDate:
     """Mock UTC date."""
 
     def isoformat(self):
         """ISO formatter datetime."""
@@ -37,64 +40,51 @@
     """Mock datetime class."""
 
     def utcnow(self):
         """Nop func."""
         return MockUTCDate()
 
 
-INIT_PID_PK = 10123
-"""Initial value for PID primary key generation."""
-
-
-@pytest.fixture(scope="function")
-def restart_pid_pk():
-    """Restart counter."""
-    global INIT_PID_PK
-    INIT_PID_PK = 10123
-
-
-def mock_pid_pk():
-    """Mock pid pk generation."""
-    global INIT_PID_PK
-    INIT_PID_PK += 1
-    return str(INIT_PID_PK)
-
-
-@patch(
-    "invenio_rdm_migrator.streams.records.table_generators.records.pid_pk", mock_pid_pk
-)
 @patch(
     "invenio_rdm_migrator.streams.records.table_generators.records.datetime",
     MockDateTime(),
 )
 @patch(
     "invenio_rdm_migrator.streams.records.table_generators.parents.datetime",
     MockDateTime(),
 )
 def test_single_record_generate_rows(
-    cache, restart_pid_pk, transformed_record_entry_pks
+    state, communities_state, parents_state, transformed_record_entry_pks
 ):
-    """A published record with a non cached parent.
+    """A published record with a non state parent.
 
-    It does not make sense to also test with a cached parent since that would mean
+    It does not make sense to also test with a state parent since that would mean
     there was a previous version of the record, which is tested separately in this module.
     """
-    tg = RDMRecordTableGenerator(
-        parents_cache=cache["parents"],
-        records_cache=cache["records"],
-        communities_cache=cache["communities"],
-    )
+    pid_1 = pid_pk()
+    pid_2 = pid_pk()
+    tg = RDMRecordTableGenerator()
     rows = list(tg._generate_rows(transformed_record_entry_pks))
     expected_rows = [
+        PersistentIdentifier(  # parent recid
+            id=pid_1,
+            pid_type="recid",
+            pid_value="12345677",
+            status="R",
+            object_type="rec",
+            object_uuid="12345678-abcd-1a2b-3c4d-123abc456def",
+            created="2023-04-01 12:00:00.00000",
+            updated="2023-04-01 12:00:00.00000",
+        ),
         RDMParentMetadata(  # parent record
             id="12345678-abcd-1a2b-3c4d-123abc456def",
             json={
                 "id": "12345677",
                 "pid": {
-                    "pk": "10122",
+                    "pk": pid_1,
                     "obj_type": "rec",
                     "pid_type": "recid",
                     "status": "R",
                 },
                 "communities": {
                     "ids": [
                         "12345678-abcd-1a2b-3c4d-123abc456def",
@@ -103,35 +93,25 @@
                     "default": "12345678-abcd-1a2b-3c4d-123abc456def",
                 },
             },
             created="2023-01-01 12:00:00.00000",
             updated="2023-01-31 12:00:00.00000",
             version_id=1,
         ),
-        PersistentIdentifier(  # parent recid
-            id="10122",
-            pid_type="recid",
-            pid_value="12345677",
-            status="R",
-            object_type="rec",
-            object_uuid="12345678-abcd-1a2b-3c4d-123abc456def",
-            created="2023-04-01 12:00:00.00000",
-            updated="2023-04-01 12:00:00.00000",
-        ),
         RDMParentCommunityMetadata(  # parent community
             community_id="12345678-abcd-1a2b-3c4d-123abc456def",
             record_id="12345678-abcd-1a2b-3c4d-123abc456def",
             request_id=None,
         ),
         RDMRecordMetadata(  # record
             id="2d6970ea-602d-4e8b-a918-063a59823386",
             json={
                 "id": "12345678",
                 "pid": {
-                    "pk": "10123",
+                    "pk": pid_2,
                     "obj_type": "rec",
                     "pid_type": "recid",
                     "status": "R",
                 },
                 "pids": {
                     "oai": {
                         "provider": "oai",
@@ -144,81 +124,88 @@
                     },
                 },
             },
             created="2023-01-01 12:00:00.00000",
             updated="2023-01-31 12:00:00.00000",
             version_id=1,
             index=1,
-            bucket_id=None,
+            bucket_id="bur3c0rd-1234-abcd-1ab2-1234abcd56ef",
             parent_id="12345678-abcd-1a2b-3c4d-123abc456def",
         ),
         PersistentIdentifier(  # recid
-            id="10123",
+            id=pid_2,
             pid_type="recid",
             pid_value="12345678",
             status="R",
             object_type="rec",
             object_uuid="2d6970ea-602d-4e8b-a918-063a59823386",
             created="2023-04-01 12:00:00.00000",
             updated="2023-04-01 12:00:00.00000",
         ),
         PersistentIdentifier(  # doi
-            id="10124",
+            id=1_000_002,
             pid_type="doi",
             pid_value="10.5281/zenodo.12345678",
             status="R",
             object_type="rec",
             object_uuid="2d6970ea-602d-4e8b-a918-063a59823386",
             created="2023-04-01 12:00:00.00000",
             updated="2023-04-01 12:00:00.00000",
         ),
         PersistentIdentifier(  # oai
-            id="10125",
+            id=1_000_003,
             pid_type="oai",
             pid_value="oai:zenodo.org:12345678",
             status="R",
             object_type="rec",
             object_uuid="2d6970ea-602d-4e8b-a918-063a59823386",
             created="2023-04-01 12:00:00.00000",
             updated="2023-04-01 12:00:00.00000",
         ),
     ]
 
     assert rows == expected_rows
 
-    assert len(cache["parents"].all()) == 2  # pre-existing and new
-    assert len(cache["records"].all()) == 1
+    assert len(list(state.PARENTS.all())) == 2  # pre-existing and new
+    assert len(list(state.RECORDS.all())) == 1
 
 
 @patch(
-    "invenio_rdm_migrator.streams.records.table_generators.drafts.pid_pk", mock_pid_pk
-)
-@patch(
     "invenio_rdm_migrator.streams.records.table_generators.drafts.datetime",
     MockDateTime(),
 )
 @patch(
     "invenio_rdm_migrator.streams.records.table_generators.parents.datetime",
     MockDateTime(),
 )
-def test_single_draft_generate_rows(cache, restart_pid_pk, transformed_draft_entry_pks):
+def test_single_draft_generate_rows(
+    state, communities_state, parents_state, transformed_draft_entry_pks
+):
     """A new draft, not published."""
-    tg = RDMDraftTableGenerator(
-        parents_cache=cache["parents"],
-        records_cache=cache["records"],
-        communities_cache=cache["communities"],
-    )
+    pid_1 = pid_pk()
+    pid_2 = pid_pk()
+    tg = RDMDraftTableGenerator()
     rows = list(tg._generate_rows(transformed_draft_entry_pks))
     expected_rows = [
+        PersistentIdentifier(  # parent recid
+            id=pid_1,
+            pid_type="recid",
+            pid_value="12345677",
+            status="N",
+            object_type="rec",
+            object_uuid="12345678-abcd-1a2b-3c4d-123abc456def",
+            created="2023-04-01 12:00:00.00000",
+            updated="2023-04-01 12:00:00.00000",
+        ),
         RDMParentMetadata(  # parent record
             id="12345678-abcd-1a2b-3c4d-123abc456def",
             json={
                 "id": "12345677",
                 "pid": {
-                    "pk": "10122",
+                    "pk": pid_1,
                     "obj_type": "rec",
                     "pid_type": "recid",
                     "status": "N",
                 },
                 "communities": {
                     "ids": [
                         "12345678-abcd-1a2b-3c4d-123abc456def",
@@ -227,30 +214,20 @@
                     "default": "12345678-abcd-1a2b-3c4d-123abc456def",
                 },
             },
             created="2023-01-01 12:00:00.00000",
             updated="2023-01-31 12:00:00.00000",
             version_id=1,
         ),
-        PersistentIdentifier(  # parent recid
-            id="10122",
-            pid_type="recid",
-            pid_value="12345677",
-            status="N",
-            object_type="rec",
-            object_uuid="12345678-abcd-1a2b-3c4d-123abc456def",
-            created="2023-04-01 12:00:00.00000",
-            updated="2023-04-01 12:00:00.00000",
-        ),
         RDMDraftMetadata(  # record
             id="2d6970ea-602d-4e8b-a918-063a59823386",
             json={
                 "id": "12345678",
                 "pid": {
-                    "pk": "10123",
+                    "pk": pid_2,
                     "obj_type": "rec",
                     "pid_type": "recid",
                     "status": "N",
                 },
                 "pids": {
                     "doi": {
                         "provider": "external",
@@ -258,82 +235,72 @@
                     },
                 },
             },
             created="2023-01-01 12:00:00.00000",
             updated="2023-01-31 12:00:00.00000",
             version_id=1,
             index=1,
-            bucket_id=None,
+            bucket_id="bud3p0s1-1234-abcd-1ab2-1234abcd56ef",
             parent_id="12345678-abcd-1a2b-3c4d-123abc456def",
             expires_at="2024-01-01 12:00:00.00000",
             fork_version_id=None,
         ),
         PersistentIdentifier(  # recid
-            id="10123",
+            id=pid_2,
             pid_type="recid",
             pid_value="12345678",
             status="N",
             object_type="rec",
             object_uuid="2d6970ea-602d-4e8b-a918-063a59823386",
             created="2023-04-01 12:00:00.00000",
             updated="2023-04-01 12:00:00.00000",
         ),
     ]
 
     assert rows == expected_rows
 
-    assert len(cache["parents"].all()) == 2  # pre-existing and new
-    assert len(cache["records"].all()) == 0
+    assert len(list(state.PARENTS.all())) == 2  # pre-existing and new
+    assert len(list(state.RECORDS.all())) == 0
 
 
 @patch(
-    "invenio_rdm_migrator.streams.records.table_generators.records.pid_pk", mock_pid_pk
-)
-@patch(
-    "invenio_rdm_migrator.streams.records.table_generators.drafts.pid_pk", mock_pid_pk
-)
-@patch(
     "invenio_rdm_migrator.streams.records.table_generators.records.datetime",
     MockDateTime(),
 )
 @patch(
     "invenio_rdm_migrator.streams.records.table_generators.drafts.datetime",
     MockDateTime(),
 )
 @patch(
     "invenio_rdm_migrator.streams.records.table_generators.parents.datetime",
     MockDateTime(),
 )
 def test_record_versions_and_old_draft_generate_rows(
-    cache, restart_pid_pk, transformed_record_entry_pks, transformed_draft_entry_pks
+    state,
+    communities_state,
+    parents_state,
+    transformed_record_entry_pks,
+    transformed_draft_entry_pks,
 ):
     """A record with two versions (v1, v2) and a draft of the first version (v1)."""
     tgs = [
-        RDMRecordTableGenerator(
-            parents_cache=cache["parents"],
-            records_cache=cache["records"],
-            communities_cache=cache["communities"],
-        ),
-        RDMDraftTableGenerator(
-            parents_cache=cache["parents"],
-            records_cache=cache["records"],
-            communities_cache=cache["communities"],
-        ),
+        RDMRecordTableGenerator(),
+        RDMDraftTableGenerator(),
     ]
 
     v1 = transformed_record_entry_pks
     v2 = deepcopy(transformed_record_entry_pks)
     v2["record"]["id"] = "2d6970ea-602d-4e8b-a918-063a59823387"
     v2["record"]["index"] = 2
     v2["record"]["json"]["id"] = "12345679"
-    v2["record"]["json"]["pid"]["pk"] = "10126"  # pk, not pid value
+    v2["record"]["json"]["pid"]["pk"] = 1_000_002  # pk, not pid value
     v2["record"]["json"]["pids"]["oai"]["identifier"] = "oai:zenodo.org:12345679"
     v2["record"]["json"]["pids"]["doi"]["identifier"] = "10.5281/zenodo.12345679"
     d_v1 = transformed_draft_entry_pks
-    d_v1["draft"]["json"]["pid"]["pk"] = "10123"  # pk, not pid value, same as v1
+    d_v1["draft"]["json"]["pid"]["pk"] = 1_000_002  # pk, not pid value, same as v1
     d_v1["draft"]["json"]["pid"][
         "status"
     ] = "R"  # same as already R pid form the record
     d_v1["draft"]["fork_version_id"] = 1
 
     rows = []
     for entry in [v1, v2, d_v1]:
@@ -342,15 +309,15 @@
 
     expected_rows_v2 = [
         RDMRecordMetadata(  # record
             id="2d6970ea-602d-4e8b-a918-063a59823387",
             json={
                 "id": "12345679",
                 "pid": {
-                    "pk": "10126",
+                    "pk": 1_000_002,
                     "obj_type": "rec",
                     "pid_type": "recid",
                     "status": "R",
                 },
                 "pids": {
                     "oai": {
                         "provider": "oai",
@@ -363,39 +330,39 @@
                     },
                 },
             },
             created="2023-01-01 12:00:00.00000",
             updated="2023-01-31 12:00:00.00000",
             version_id=1,
             index=2,
-            bucket_id=None,
+            bucket_id="bur3c0rd-1234-abcd-1ab2-1234abcd56ef",
             parent_id="12345678-abcd-1a2b-3c4d-123abc456def",
         ),
         PersistentIdentifier(  # recid
-            id="10126",  # this called is mocked and will not increment the counter
+            id=1_000_002,  # this called is mocked and will not increment the counter
             pid_type="recid",
             pid_value="12345679",
             status="R",
             object_type="rec",
             object_uuid="2d6970ea-602d-4e8b-a918-063a59823387",
             created="2023-04-01 12:00:00.00000",
             updated="2023-04-01 12:00:00.00000",
         ),
         PersistentIdentifier(  # doi
-            id="10126",
+            id=1_000_002,
             pid_type="doi",
             pid_value="10.5281/zenodo.12345679",
             status="R",
             object_type="rec",
             object_uuid="2d6970ea-602d-4e8b-a918-063a59823387",
             created="2023-04-01 12:00:00.00000",
             updated="2023-04-01 12:00:00.00000",
         ),
         PersistentIdentifier(  # oai
-            id="10127",
+            id=1_000_003,
             pid_type="oai",
             pid_value="oai:zenodo.org:12345679",
             status="R",
             object_type="rec",
             object_uuid="2d6970ea-602d-4e8b-a918-063a59823387",
             created="2023-04-01 12:00:00.00000",
             updated="2023-04-01 12:00:00.00000",
@@ -404,15 +371,15 @@
 
     expected_rows_d_v1 = [
         RDMDraftMetadata(  # record
             id="2d6970ea-602d-4e8b-a918-063a59823386",
             json={
                 "id": "12345678",
                 "pid": {
-                    "pk": "10123",
+                    "pk": 1_000_002,
                     "obj_type": "rec",
                     "pid_type": "recid",
                     "status": "R",
                 },
                 "pids": {
                     "doi": {
                         "provider": "external",
@@ -420,91 +387,83 @@
                     },
                 },
             },
             created="2023-01-01 12:00:00.00000",
             updated="2023-01-31 12:00:00.00000",
             version_id=1,
             index=1,
-            bucket_id=None,
+            bucket_id="bud3p0s1-1234-abcd-1ab2-1234abcd56ef",
             parent_id="12345678-abcd-1a2b-3c4d-123abc456def",
             expires_at="2024-01-01 12:00:00.00000",
             fork_version_id=1,
         ),
     ]
 
     assert len(rows) == 12
     # v1 rows not asserted since they are checked at test_single_record_generate_rows
     assert rows[7:11] == expected_rows_v2
     assert rows[11:12] == expected_rows_d_v1
 
-    assert len(cache["parents"].all()) == 2  # pre-existing and new
-    assert len(cache["records"].all()) == 2  # two added records
+    assert len(list(state.PARENTS.all())) == 2  # pre-existing and new
+    assert len(list(state.RECORDS.all())) == 2  # two added records
 
 
 @patch(
-    "invenio_rdm_migrator.streams.records.table_generators.records.pid_pk", mock_pid_pk
-)
-@patch(
-    "invenio_rdm_migrator.streams.records.table_generators.drafts.pid_pk", mock_pid_pk
-)
-@patch(
     "invenio_rdm_migrator.streams.records.table_generators.records.datetime",
     MockDateTime(),
 )
 @patch(
     "invenio_rdm_migrator.streams.records.table_generators.drafts.datetime",
     MockDateTime(),
 )
 @patch(
     "invenio_rdm_migrator.streams.records.table_generators.parents.datetime",
     MockDateTime(),
 )
 def test_record_and_new_version_draft_generate_rows(
-    cache, restart_pid_pk, transformed_record_entry_pks, transformed_draft_entry_pks
+    state,
+    communities_state,
+    parents_state,
+    transformed_record_entry_pks,
+    transformed_draft_entry_pks,
 ):
     """A published record (v1) with a new version draft (v2)."""
     tgs = [
-        RDMRecordTableGenerator(
-            parents_cache=cache["parents"],
-            records_cache=cache["records"],
-            communities_cache=cache["communities"],
-        ),
-        RDMDraftTableGenerator(
-            parents_cache=cache["parents"],
-            records_cache=cache["records"],
-            communities_cache=cache["communities"],
-        ),
+        RDMRecordTableGenerator(),
+        RDMDraftTableGenerator(),
     ]
 
+    pid_1 = pid_pk()
+    pid_2 = pid_pk()
     v1 = transformed_record_entry_pks
     v2 = deepcopy(transformed_record_entry_pks)
     v2["record"]["id"] = "2d6970ea-602d-4e8b-a918-063a59823387"
     v2["record"]["index"] = 2
     v2["record"]["json"]["id"] = "12345679"
-    v2["record"]["json"]["pid"]["pk"] = "10126"  # pk, not pid value
+    v2["record"]["json"]["pid"]["pk"] = pid_1  # pk, not pid value
     v2["record"]["json"]["pids"]["oai"]["identifier"] = "oai:zenodo.org:12345679"
     v2["record"]["json"]["pids"]["doi"]["identifier"] = "10.5281/zenodo.12345679"
     d_v3 = transformed_draft_entry_pks
     d_v3["draft"]["id"] = "2d6970ea-602d-4e8b-a918-063a59823389"
     d_v3["draft"]["json"]["id"] = "12345680"
-    d_v3["draft"]["json"]["pid"]["pk"] = "10128"  # pk, not pid value, same as v1
+    d_v3["draft"]["json"]["pid"]["pk"] = pid_2  # pk, not pid value, same as v1
     d_v3["draft"]["json"]["pids"]["doi"]["identifier"] = "10.1234/bar"
 
     rows = []
     for entry in [v1, v2, d_v3]:
         for tg in tgs:
             rows.extend(list(tg._generate_rows(entry)))
 
     expected_rows_d_v3 = [
         RDMDraftMetadata(  # record
             id="2d6970ea-602d-4e8b-a918-063a59823389",
             json={
                 "id": "12345680",
                 "pid": {
-                    "pk": "10128",
+                    "pk": pid_2,
                     "obj_type": "rec",
                     "pid_type": "recid",
                     "status": "N",
                 },
                 "pids": {
                     "doi": {
                         "provider": "external",
@@ -512,21 +471,21 @@
                     },
                 },
             },
             created="2023-01-01 12:00:00.00000",
             updated="2023-01-31 12:00:00.00000",
             version_id=1,
             index=1,
-            bucket_id=None,
+            bucket_id="bud3p0s1-1234-abcd-1ab2-1234abcd56ef",
             parent_id="12345678-abcd-1a2b-3c4d-123abc456def",
             expires_at="2024-01-01 12:00:00.00000",
             fork_version_id=None,
         ),
         PersistentIdentifier(  # recid
-            id="10128",  # this called is mocked and will not increment the counter
+            id=pid_2,  # this called is mocked and will not increment the counter
             pid_type="recid",
             pid_value="12345680",
             status="N",
             object_type="rec",
             object_uuid="2d6970ea-602d-4e8b-a918-063a59823389",
             created="2023-04-01 12:00:00.00000",
             updated="2023-04-01 12:00:00.00000",
@@ -535,9 +494,9 @@
 
     assert len(rows) == 13
 
     # v1 rows not asserted since they are checked at test_single_record_generate_rows
     # v2 rows not asserted since they are checked at test_record_versions_and_old_draft_generate_rows
     assert rows[11:13] == expected_rows_d_v3
 
-    assert len(cache["parents"].all()) == 2  # pre-existing and new
-    assert len(cache["records"].all()) == 2  # two added records
+    assert len(list(state.PARENTS.all())) == 2  # pre-existing and new
+    assert len(list(state.RECORDS.all())) == 2  # two added records
```

### Comparing `invenio-rdm-migrator-1.0.0a9/tests/streams/requests/conftest.py` & `invenio-rdm-migrator-2.0.0/tests/streams/requests/test_requests_table_generator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2023 CERN.
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
-"""Pytest requests configuration."""
+"""Requests table generator tests."""
 
 from copy import deepcopy
 
-import pytest
+import dictdiffer
 
+from invenio_rdm_migrator.streams.models.requests import RequestMetadata
+from invenio_rdm_migrator.streams.requests.load import RequestTableGenerator
 
-@pytest.fixture(scope="module")
-def transformed_incl_req_entry():
-    """Request data as after being transformed.
-
-    `topic`, `receiver` and `created_by` could be different.
-    This is a sample inclusion request for a record into a community.
-    """
-    return {
-        "created": "01/01/2023",
-        "updated": "01/01/2023",
-        "version_id": "1",
-        "json": {
-            "type": "community-inclusion",
-            "title": "title",
-            "topic": {"record": "123456"},
-            "status": "submitted",
-            "receiver": {"community": "comm"},
-            "created_by": {"user": "3"},
-            "$schema": "local://requests/request-v1.0.0.json",
-        },
-        "number": "1",
-        "expires_at": "01/01/2023",
-    }
-
-
-@pytest.fixture(scope="module")
-def transformed_incl_req_entry_pks(transformed_incl_req_entry):
-    """Request data as after being transformed and passed by generate_pks.
-
-    The last step would happen in the table_generator._prepare.
-    """
-    data = deepcopy(transformed_incl_req_entry)
-    data["id"] = "12345678-abcd-1a2b-3c4d-123abc456def"
 
-    return data
+def test_generate_rows(communities_state, transformed_incl_req_entry_pks):
+    """Test the row generation of the request table generator."""
+    tg = RequestTableGenerator()  # no need for state in this test
+    rows = list(tg._generate_rows(transformed_incl_req_entry_pks))
+    expected_rows = [
+        RequestMetadata(
+            id="12345678-abcd-1a2b-3c4d-123abc456def",
+            json={
+                "type": "community-inclusion",
+                "title": "title",
+                "topic": {"record": "123456"},
+                "status": "submitted",
+                "receiver": {"community": "comm"},
+                "created_by": {"user": "3"},
+                "$schema": "local://requests/request-v1.0.0.json",
+            },
+            created="01/01/2023",
+            updated="01/01/2023",
+            version_id="1",
+            number="1",
+            expires_at="01/01/2023",
+        ),
+    ]
+
+    assert rows == expected_rows
+
+
+def test_resolve_references(communities_state, transformed_incl_req_entry_pks):
+    """Test the parent and community reference resolution."""
+    expected = deepcopy(transformed_incl_req_entry_pks)
+    expected["json"]["receiver"]["community"] = "12345678-abcd-1a2b-3c4d-123abc456def"
+
+    tg = RequestTableGenerator()
+    tg._resolve_references(transformed_incl_req_entry_pks)  # changes in place
+
+    assert not list(dictdiffer.diff(transformed_incl_req_entry_pks, expected))
```

### Comparing `invenio-rdm-migrator-1.0.0a9/tests/streams/requests/test_requests_transform.py` & `invenio-rdm-migrator-2.0.0/tests/streams/requests/test_requests_transform.py`

 * *Files identical despite different names*

