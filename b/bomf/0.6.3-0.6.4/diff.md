# Comparing `tmp/bomf-0.6.3.tar.gz` & `tmp/bomf-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bomf-0.6.3.tar", last modified: Tue Aug  1 06:15:26 2023, max compression
+gzip compressed data, was "bomf-0.6.4.tar", last modified: Tue Aug  1 10:32:31 2023, max compression
```

## Comparing `bomf-0.6.3.tar` & `bomf-0.6.4.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.061545 bomf-0.6.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-01 06:15:14.000000 bomf-0.6.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.061545 bomf-0.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-01 06:15:14.000000 bomf-0.6.3/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-01 06:15:14.000000 bomf-0.6.3/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-01 06:15:14.000000 bomf-0.6.3/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-01 06:15:14.000000 bomf-0.6.3/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-01 06:15:14.000000 bomf-0.6.3/.github/workflows/packaging_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-08-01 06:15:14.000000 bomf-0.6.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-01 06:15:14.000000 bomf-0.6.3/.github/workflows/pythonlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-01 06:15:14.000000 bomf-0.6.3/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-01 06:15:14.000000 bomf-0.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-01 06:15:14.000000 bomf-0.6.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-01 06:15:14.000000 bomf-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-08-01 06:15:26.065546 bomf-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-08-01 06:15:14.000000 bomf-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-01 06:15:14.000000 bomf-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-01 06:15:14.000000 bomf-0.6.3/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-01 06:15:14.000000 bomf-0.6.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-01 06:15:26.069546 bomf-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-01 06:15:14.000000 bomf-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.057546 bomf-0.6.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.061545 bomf-0.6.3/src/bomf/
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-08-01 06:15:14.000000 bomf-0.6.3/src/bomf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/src/bomf/filter/
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-08-01 06:15:14.000000 bomf-0.6.3/src/bomf/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-08-01 06:15:14.000000 bomf-0.6.3/src/bomf/filter/sourcedataproviderfilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/src/bomf/loader/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-01 06:15:14.000000 bomf-0.6.3/src/bomf/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-08-01 06:15:14.000000 bomf-0.6.3/src/bomf/loader/entityloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/src/bomf/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-08-01 06:15:14.000000 bomf-0.6.3/src/bomf/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/src/bomf/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-08-01 06:15:14.000000 bomf-0.6.3/src/bomf/mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/src/bomf/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-08-01 06:15:14.000000 bomf-0.6.3/src/bomf/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/src/bomf/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/src/bomf/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/src/bomf/validation/core/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/core/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17565 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/core/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/path_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/query_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-01 06:15:15.000000 bomf-0.6.3/src/bomf/validation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/src/bomf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-08-01 06:15:25.000000 bomf-0.6.3/src/bomf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-08-01 06:15:26.000000 bomf-0.6.3/src/bomf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:15:25.000000 bomf-0.6.3/src/bomf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:15:25.000000 bomf-0.6.3/src/bomf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-01 06:15:25.000000 bomf-0.6.3/src/bomf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 06:15:25.000000 bomf-0.6.3/src/bomf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-08-01 06:15:15.000000 bomf-0.6.3/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:15:26.065546 bomf-0.6.3/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/example_source_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/test_bo4e_data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/test_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/test_list_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/test_source_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    21261 2023-08-01 06:15:15.000000 bomf-0.6.3/unittests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:32:31.037448 bomf-0.6.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:32:31.025448 bomf-0.6.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-01 10:32:19.000000 bomf-0.6.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:32:31.029448 bomf-0.6.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-01 10:32:19.000000 bomf-0.6.4/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-01 10:32:19.000000 bomf-0.6.4/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-01 10:32:19.000000 bomf-0.6.4/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-01 10:32:19.000000 bomf-0.6.4/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-01 10:32:19.000000 bomf-0.6.4/.github/workflows/packaging_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-08-01 10:32:19.000000 bomf-0.6.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-01 10:32:19.000000 bomf-0.6.4/.github/workflows/pythonlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-01 10:32:19.000000 bomf-0.6.4/.github/workflows/unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-01 10:32:19.000000 bomf-0.6.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-01 10:32:19.000000 bomf-0.6.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-01 10:32:19.000000 bomf-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-08-01 10:32:31.037448 bomf-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-08-01 10:32:19.000000 bomf-0.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-01 10:32:19.000000 bomf-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-01 10:32:19.000000 bomf-0.6.4/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-01 10:32:19.000000 bomf-0.6.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-01 10:32:31.037448 bomf-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-01 10:32:19.000000 bomf-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:32:31.025448 bomf-0.6.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:32:31.029448 bomf-0.6.4/src/bomf/
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-08-01 10:32:19.000000 bomf-0.6.4/src/bomf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:32:31.029448 bomf-0.6.4/src/bomf/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-08-01 10:32:19.000000 bomf-0.6.4/src/bomf/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-08-01 10:32:19.000000 bomf-0.6.4/src/bomf/filter/sourcedataproviderfilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:32:31.029448 bomf-0.6.4/src/bomf/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-01 10:32:19.000000 bomf-0.6.4/src/bomf/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-08-01 10:32:19.000000 bomf-0.6.4/src/bomf/loader/entityloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:32:31.033448 bomf-0.6.4/src/bomf/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-08-01 10:32:19.000000 bomf-0.6.4/src/bomf/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:32:31.033448 bomf-0.6.4/src/bomf/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-08-01 10:32:19.000000 bomf-0.6.4/src/bomf/mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:32:31.033448 bomf-0.6.4/src/bomf/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-08-01 10:32:19.000000 bomf-0.6.4/src/bomf/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:32:31.033448 bomf-0.6.4/src/bomf/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-08-01 10:32:19.000000 bomf-0.6.4/src/bomf/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-01 10:32:19.000000 bomf-0.6.4/src/bomf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:32:31.033448 bomf-0.6.4/src/bomf/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-01 10:32:19.000000 bomf-0.6.4/src/bomf/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:32:31.033448 bomf-0.6.4/src/bomf/validation/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-01 10:32:19.000000 bomf-0.6.4/src/bomf/validation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-08-01 10:32:19.000000 bomf-0.6.4/src/bomf/validation/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-08-01 10:32:19.000000 bomf-0.6.4/src/bomf/validation/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17565 2023-08-01 10:32:19.000000 bomf-0.6.4/src/bomf/validation/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-01 10:32:19.000000 bomf-0.6.4/src/bomf/validation/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-01 10:32:19.000000 bomf-0.6.4/src/bomf/validation/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-08-01 10:32:19.000000 bomf-0.6.4/src/bomf/validation/core/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-08-01 10:32:19.000000 bomf-0.6.4/src/bomf/validation/path_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-08-01 10:32:19.000000 bomf-0.6.4/src/bomf/validation/query_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-01 10:32:19.000000 bomf-0.6.4/src/bomf/validation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:32:31.029448 bomf-0.6.4/src/bomf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-08-01 10:32:30.000000 bomf-0.6.4/src/bomf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-08-01 10:32:30.000000 bomf-0.6.4/src/bomf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 10:32:30.000000 bomf-0.6.4/src/bomf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 10:32:30.000000 bomf-0.6.4/src/bomf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-01 10:32:30.000000 bomf-0.6.4/src/bomf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 10:32:30.000000 bomf-0.6.4/src/bomf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-08-01 10:32:19.000000 bomf-0.6.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:32:31.037448 bomf-0.6.4/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-01 10:32:19.000000 bomf-0.6.4/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-01 10:32:19.000000 bomf-0.6.4/unittests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-01 10:32:19.000000 bomf-0.6.4/unittests/example_source_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-01 10:32:19.000000 bomf-0.6.4/unittests/test_bo4e_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-08-01 10:32:19.000000 bomf-0.6.4/unittests/test_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-08-01 10:32:19.000000 bomf-0.6.4/unittests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-01 10:32:19.000000 bomf-0.6.4/unittests/test_list_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-08-01 10:32:19.000000 bomf-0.6.4/unittests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-08-01 10:32:19.000000 bomf-0.6.4/unittests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-08-01 10:32:19.000000 bomf-0.6.4/unittests/test_source_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21261 2023-08-01 10:32:19.000000 bomf-0.6.4/unittests/test_validation.py
```

### Comparing `bomf-0.6.3/.github/dependabot.yml` & `bomf-0.6.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/.github/workflows/black.yml` & `bomf-0.6.4/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/.github/workflows/codeql-analysis.yml` & `bomf-0.6.4/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/.github/workflows/coverage.yml` & `bomf-0.6.4/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/.github/workflows/packaging_test.yml` & `bomf-0.6.4/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/.github/workflows/python-publish.yml` & `bomf-0.6.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/.github/workflows/pythonlint.yml` & `bomf-0.6.4/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/.github/workflows/unittests.yml` & `bomf-0.6.4/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/.gitignore` & `bomf-0.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/.pre-commit-config.yaml` & `bomf-0.6.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/LICENSE` & `bomf-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/PKG-INFO` & `bomf-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.6.3
+Version: 0.6.4
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.6.3/README.md` & `bomf-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/pyproject.toml` & `bomf-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/requirements.txt` & `bomf-0.6.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/setup.cfg` & `bomf-0.6.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/src/bomf/__init__.py` & `bomf-0.6.4/src/bomf/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/src/bomf/filter/__init__.py` & `bomf-0.6.4/src/bomf/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/src/bomf/filter/sourcedataproviderfilter.py` & `bomf-0.6.4/src/bomf/filter/sourcedataproviderfilter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/src/bomf/loader/entityloader.py` & `bomf-0.6.4/src/bomf/loader/entityloader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/src/bomf/logging/__init__.py` & `bomf-0.6.4/src/bomf/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/src/bomf/mapper/__init__.py` & `bomf-0.6.4/src/bomf/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/src/bomf/model/__init__.py` & `bomf-0.6.4/src/bomf/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/src/bomf/provider/__init__.py` & `bomf-0.6.4/src/bomf/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/src/bomf/validation/core/analysis.py` & `bomf-0.6.4/src/bomf/validation/core/analysis.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/src/bomf/validation/core/errors.py` & `bomf-0.6.4/src/bomf/validation/core/errors.py`

 * *Files 14% similar despite different names*

```diff
@@ -74,17 +74,23 @@
     if last_id is not None:
         logger.get().debug(
             "Duplicated ID for %s and %s. Generating new ID...", identifier, _ERROR_ID_MAP.inverse[last_id]
         )
         random.seed(last_id)
     else:
         module_name_hash = int(hashlib.blake2s((identifier[0] + identifier[1]).encode(), digest_size=4).hexdigest(), 16)
-        random.seed(module_name_hash + identifier[2])
+        random.seed(module_name_hash)
     # This range has no further meaning, but you have to define it.
-    return random.randint(1_000_000, 9_999_999)
+    rand_range = (1_000_000, 9_998_999)
+    # This guarantees that functions with up to 1000 lines of code remain stable in their first digits if an error
+    # changes in its line number inside the function.
+    error_id_range = (1_000_000, 9_999_999)
+    return (random.randint(*rand_range) + identifier[2] - error_id_range[0]) % (
+        error_id_range[1] - error_id_range[0] + 1
+    ) + error_id_range[0]
 
 
 def _get_error_id(identifier: _IdentifierType) -> _IDType:
     """
     Returns a unique ID for the provided identifier.
     """
     if identifier not in _ERROR_ID_MAP:
```

### Comparing `bomf-0.6.3/src/bomf/validation/core/execution.py` & `bomf-0.6.4/src/bomf/validation/core/execution.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/src/bomf/validation/core/types.py` & `bomf-0.6.4/src/bomf/validation/core/types.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/src/bomf/validation/core/utils.py` & `bomf-0.6.4/src/bomf/validation/core/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/src/bomf/validation/core/validator.py` & `bomf-0.6.4/src/bomf/validation/core/validator.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/src/bomf/validation/path_map.py` & `bomf-0.6.4/src/bomf/validation/path_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/src/bomf/validation/query_map.py` & `bomf-0.6.4/src/bomf/validation/query_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/src/bomf/validation/utils.py` & `bomf-0.6.4/src/bomf/validation/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/src/bomf.egg-info/PKG-INFO` & `bomf-0.6.4/src/bomf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.6.3
+Version: 0.6.4
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.6.3/src/bomf.egg-info/SOURCES.txt` & `bomf-0.6.4/src/bomf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/tox.ini` & `bomf-0.6.4/tox.ini`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/unittests/test_bo4e_data_set.py` & `bomf-0.6.4/unittests/test_bo4e_data_set.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/unittests/test_entity_loader.py` & `bomf-0.6.4/unittests/test_entity_loader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/unittests/test_filter.py` & `bomf-0.6.4/unittests/test_filter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/unittests/test_list_conversion.py` & `bomf-0.6.4/unittests/test_list_conversion.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/unittests/test_mapper.py` & `bomf-0.6.4/unittests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/unittests/test_migration.py` & `bomf-0.6.4/unittests/test_migration.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/unittests/test_source_data_provider.py` & `bomf-0.6.4/unittests/test_source_data_provider.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.3/unittests/test_validation.py` & `bomf-0.6.4/unittests/test_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,15 +449,15 @@
         # Different errors in the same function should get different error IDs.
         assert (
             sub_exceptions1[PathMappedValidator(validator_check_different_fails, {"x": "x"})].error_id
             != sub_exceptions1[PathMappedValidator(validator_check_different_fails, {"x": "z.x"})].error_id
         )
         # This ensures that the ID is constant across python sessions - as long as the line number of the raising
         # exception in `check_fail` doesn't change.
-        assert sub_exceptions1[PathMappedValidator(validator_check_fail, {"x": "x"})].error_id == 1746866
+        assert sub_exceptions1[PathMappedValidator(validator_check_fail, {"x": "x"})].error_id == 8103059
 
     async def test_utility_required_and_optional(self):
         validation_manager = ValidationManager[DataSetTest]()
         validation_manager.register(
             PathMappedValidator(validator_check_required_and_optional_with_utility, {"z": "z"}),
         )
         validation_summary = await validation_manager.validate(dataset_instance)
```

