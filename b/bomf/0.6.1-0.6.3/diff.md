# Comparing `tmp/bomf-0.6.1.tar.gz` & `tmp/bomf-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bomf-0.6.1.tar", last modified: Mon Jul 31 11:03:37 2023, max compression
+gzip compressed data, was "bomf-0.6.3.tar", last modified: Tue Aug  1 06:15:26 2023, max compression
```

## Comparing `bomf-0.6.1.tar` & `bomf-0.6.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.602330 bomf-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-31 11:03:30.000000 bomf-0.6.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-31 11:03:30.000000 bomf-0.6.1/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-31 11:03:30.000000 bomf-0.6.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-31 11:03:30.000000 bomf-0.6.1/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-31 11:03:30.000000 bomf-0.6.1/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-31 11:03:30.000000 bomf-0.6.1/.github/workflows/packaging_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-31 11:03:30.000000 bomf-0.6.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-31 11:03:30.000000 bomf-0.6.1/.github/workflows/pythonlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-31 11:03:30.000000 bomf-0.6.1/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-31 11:03:30.000000 bomf-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-31 11:03:30.000000 bomf-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-31 11:03:30.000000 bomf-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-31 11:03:37.602330 bomf-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-31 11:03:30.000000 bomf-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-31 11:03:30.000000 bomf-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-31 11:03:30.000000 bomf-0.6.1/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-31 11:03:30.000000 bomf-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-31 11:03:37.602330 bomf-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-31 11:03:30.000000 bomf-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.594330 bomf-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/src/bomf/
--rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/src/bomf/filter/
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/filter/sourcedataproviderfilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/src/bomf/loader/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/loader/entityloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/src/bomf/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/src/bomf/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/src/bomf/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/src/bomf/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/src/bomf/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/src/bomf/validation/core/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/core/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17565 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/core/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/path_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/query_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/src/bomf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-31 11:03:37.000000 bomf-0.6.1/src/bomf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-31 11:03:37.000000 bomf-0.6.1/src/bomf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 11:03:37.000000 bomf-0.6.1/src/bomf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 11:03:37.000000 bomf-0.6.1/src/bomf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-31 11:03:37.000000 bomf-0.6.1/src/bomf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 11:03:37.000000 bomf-0.6.1/src/bomf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-31 11:03:30.000000 bomf-0.6.1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.602330 bomf-0.6.1/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/example_source_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/test_bo4e_data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/test_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/test_list_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/test_source_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    21261 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.061545 bomf-0.6.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-01 06:15:14.000000 bomf-0.6.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.061545 bomf-0.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-01 06:15:14.000000 bomf-0.6.3/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-01 06:15:14.000000 bomf-0.6.3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-01 06:15:14.000000 bomf-0.6.3/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-01 06:15:14.000000 bomf-0.6.3/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-01 06:15:14.000000 bomf-0.6.3/.github/workflows/packaging_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-08-01 06:15:14.000000 bomf-0.6.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-01 06:15:14.000000 bomf-0.6.3/.github/workflows/pythonlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-01 06:15:14.000000 bomf-0.6.3/.github/workflows/unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-01 06:15:14.000000 bomf-0.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-01 06:15:14.000000 bomf-0.6.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-01 06:15:14.000000 bomf-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-08-01 06:15:26.065546 bomf-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-08-01 06:15:14.000000 bomf-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-01 06:15:14.000000 bomf-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-01 06:15:14.000000 bomf-0.6.3/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-01 06:15:14.000000 bomf-0.6.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-01 06:15:26.069546 bomf-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-01 06:15:14.000000 bomf-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.057546 bomf-0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.061545 bomf-0.6.3/src/bomf/
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-08-01 06:15:14.000000 bomf-0.6.3/src/bomf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/src/bomf/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-08-01 06:15:14.000000 bomf-0.6.3/src/bomf/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-08-01 06:15:14.000000 bomf-0.6.3/src/bomf/filter/sourcedataproviderfilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/src/bomf/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-01 06:15:14.000000 bomf-0.6.3/src/bomf/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-08-01 06:15:14.000000 bomf-0.6.3/src/bomf/loader/entityloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/src/bomf/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-08-01 06:15:14.000000 bomf-0.6.3/src/bomf/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/src/bomf/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-08-01 06:15:14.000000 bomf-0.6.3/src/bomf/mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/src/bomf/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-08-01 06:15:14.000000 bomf-0.6.3/src/bomf/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/src/bomf/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/src/bomf/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/src/bomf/validation/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17565 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/core/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/path_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/query_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/src/bomf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-08-01 06:15:25.000000 bomf-0.6.3/src/bomf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-08-01 06:15:26.000000 bomf-0.6.3/src/bomf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:15:25.000000 bomf-0.6.3/src/bomf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:15:25.000000 bomf-0.6.3/src/bomf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-01 06:15:25.000000 bomf-0.6.3/src/bomf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 06:15:25.000000 bomf-0.6.3/src/bomf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-08-01 06:15:15.000000 bomf-0.6.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/example_source_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/test_bo4e_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/test_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/test_list_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/test_source_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21261 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/test_validation.py
```

### Comparing `bomf-0.6.1/.github/dependabot.yml` & `bomf-0.6.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/.github/workflows/black.yml` & `bomf-0.6.3/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/.github/workflows/codeql-analysis.yml` & `bomf-0.6.3/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/.github/workflows/coverage.yml` & `bomf-0.6.3/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/.github/workflows/packaging_test.yml` & `bomf-0.6.3/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/.github/workflows/python-publish.yml` & `bomf-0.6.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/.github/workflows/pythonlint.yml` & `bomf-0.6.3/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/.github/workflows/unittests.yml` & `bomf-0.6.3/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/.gitignore` & `bomf-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/.pre-commit-config.yaml` & `bomf-0.6.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/LICENSE` & `bomf-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/PKG-INFO` & `bomf-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.6.1
+Version: 0.6.3
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.6.1/README.md` & `bomf-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/pyproject.toml` & `bomf-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/requirements.txt` & `bomf-0.6.3/requirements.txt`

 * *Files 19% similar despite different names*

```diff
@@ -24,13 +24,14 @@
     # via
     #   -r requirements.in
     #   bo4e
 pydantic-core==2.4.0
     # via pydantic
 pyhumps==3.8.0
     # via bo4e
-typeguard==4.0.1
+typeguard==4.1.0
     # via -r requirements.in
 typing-extensions==4.7.1
     # via
     #   pydantic
     #   pydantic-core
+    #   typeguard
```

### Comparing `bomf-0.6.1/setup.cfg` & `bomf-0.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/src/bomf/__init__.py` & `bomf-0.6.3/src/bomf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         2. mapping intermediate models to target
         3. load to target system.
         They have been encapsulated because they're used by both the migrate and migrate_paginated methods.
         """
         _logger = logger.get()
         if self.validation_manager is not None:
             _logger.info("Applying validation rules to %i bo4e data sets", len(bo4e_datasets))
-            validation_result = await self.validation_manager.validate(*bo4e_datasets)
+            validation_result = await self.validation_manager.validate(*bo4e_datasets, log_summary=True)
             _logger.info(
                 "Creating target models from those %i datasets that passed the validation",
                 len(validation_result.succeeded_data_sets),
             )
             target_data_models = await self.bo4e_to_target_mapper.create_target_models(
                 validation_result.succeeded_data_sets
             )
```

### Comparing `bomf-0.6.1/src/bomf/filter/__init__.py` & `bomf-0.6.3/src/bomf/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/src/bomf/filter/sourcedataproviderfilter.py` & `bomf-0.6.3/src/bomf/filter/sourcedataproviderfilter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/src/bomf/loader/entityloader.py` & `bomf-0.6.3/src/bomf/loader/entityloader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/src/bomf/logging/__init__.py` & `bomf-0.6.3/src/bomf/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/src/bomf/mapper/__init__.py` & `bomf-0.6.3/src/bomf/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/src/bomf/model/__init__.py` & `bomf-0.6.3/src/bomf/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/src/bomf/provider/__init__.py` & `bomf-0.6.3/src/bomf/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/src/bomf/validation/core/analysis.py` & `bomf-0.6.3/src/bomf/validation/core/analysis.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/src/bomf/validation/core/errors.py` & `bomf-0.6.3/src/bomf/validation/core/errors.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/src/bomf/validation/core/execution.py` & `bomf-0.6.3/src/bomf/validation/core/execution.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/src/bomf/validation/core/types.py` & `bomf-0.6.3/src/bomf/validation/core/types.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/src/bomf/validation/core/utils.py` & `bomf-0.6.3/src/bomf/validation/core/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/src/bomf/validation/core/validator.py` & `bomf-0.6.3/src/bomf/validation/core/validator.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/src/bomf/validation/path_map.py` & `bomf-0.6.3/src/bomf/validation/path_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/src/bomf/validation/query_map.py` & `bomf-0.6.3/src/bomf/validation/query_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/src/bomf/validation/utils.py` & `bomf-0.6.3/src/bomf/validation/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/src/bomf.egg-info/PKG-INFO` & `bomf-0.6.3/src/bomf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.6.1
+Version: 0.6.3
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.6.1/src/bomf.egg-info/SOURCES.txt` & `bomf-0.6.3/src/bomf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/tox.ini` & `bomf-0.6.3/tox.ini`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/unittests/test_bo4e_data_set.py` & `bomf-0.6.3/unittests/test_bo4e_data_set.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/unittests/test_entity_loader.py` & `bomf-0.6.3/unittests/test_entity_loader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/unittests/test_filter.py` & `bomf-0.6.3/unittests/test_filter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/unittests/test_list_conversion.py` & `bomf-0.6.3/unittests/test_list_conversion.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/unittests/test_mapper.py` & `bomf-0.6.3/unittests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/unittests/test_migration.py` & `bomf-0.6.3/unittests/test_migration.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/unittests/test_source_data_provider.py` & `bomf-0.6.3/unittests/test_source_data_provider.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.1/unittests/test_validation.py` & `bomf-0.6.3/unittests/test_validation.py`

 * *Files identical despite different names*

