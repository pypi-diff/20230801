# Comparing `tmp/edc-lab-results-0.1.38.tar.gz` & `tmp/edc-lab-results-0.1.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-lab-results-0.1.38.tar", last modified: Wed May 24 17:18:39 2023, max compression
+gzip compressed data, was "edc-lab-results-0.1.39.tar", last modified: Tue Aug  1 04:34:50 2023, max compression
```

## Comparing `edc-lab-results-0.1.38.tar` & `edc-lab-results-0.1.39.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.393019 edc-lab-results-0.1.38/
--rw-r--r--   0 erikvw     (501) staff       (20)       76 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.380264 edc-lab-results-0.1.38/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.384183 edc-lab-results-0.1.38/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 17:18:30.000000 edc-lab-results-0.1.38/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1842 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 17:18:30.000000 edc-lab-results-0.1.38/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-09 19:25:16.000000 edc-lab-results-0.1.38/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)      402 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-06-25 20:27:10.000000 edc-lab-results-0.1.38/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1644 2023-05-24 17:18:39.393122 edc-lab-results-0.1.38/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      733 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-09 19:25:16.000000 edc-lab-results-0.1.38/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.385881 edc-lab-results-0.1.38/edc_lab_results/
--rw-r--r--   0 erikvw     (501) staff       (20)      276 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3809 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/edc_lab_results/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.387194 edc-lab-results-0.1.38/edc_lab_results/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      154 2022-10-26 16:30:10.000000 edc-lab-results-0.1.38/edc_lab_results/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-10-26 16:30:10.000000 edc-lab-results-0.1.38/edc_lab_results/admin/blood_results_modeladmin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1867 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/edc_lab_results/admin/reportable_results_modeladmin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      157 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1002 2022-07-27 02:24:23.000000 edc-lab-results-0.1.38/edc_lab_results/calculate_missing.py
--rw-r--r--   0 erikvw     (501) staff       (20)      504 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3813 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/edc_lab_results/fieldsets.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.387981 edc-lab-results-0.1.38/edc_lab_results/form_validator_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      251 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/form_validator_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      836 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/form_validator_mixins/blood_results_fbg_form_validator_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3990 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/edc_lab_results/form_validator_mixins/blood_results_form_validator_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      437 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/form_validator_mixins/blood_results_glu_form_validator_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.389873 edc-lab-results-0.1.38/edc_lab_results/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)     1189 2022-08-15 00:51:30.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4343 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/blood_result_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      955 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/electrolytes_model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4420 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/fbc_model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1749 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/fbg_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1748 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/glucose_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1267 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/hba1c_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1140 2023-05-24 17:18:30.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/insulin_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3107 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/lft_model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1723 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/lipid_model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      426 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/proteinuria_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1367 2022-08-15 00:51:30.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/rft_model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.391056 edc-lab-results-0.1.38/edc_lab_results/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.392318 edc-lab-results-0.1.38/edc_lab_results/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1367 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/edc_lab_results/tests/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)      508 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)      683 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/lab_profiles.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2039 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/edc_lab_results/tests/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2702 2022-09-30 01:31:16.000000 edc-lab-results-0.1.38/edc_lab_results/tests/test_case_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.392799 edc-lab-results-0.1.38/edc_lab_results/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4438 2023-03-31 15:04:16.000000 edc-lab-results-0.1.38/edc_lab_results/tests/tests/test_blood_result.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7333 2022-10-25 19:12:51.000000 edc-lab-results-0.1.38/edc_lab_results/tests/tests/test_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      261 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2104 2022-09-30 01:31:16.000000 edc-lab-results-0.1.38/edc_lab_results/tests/visit_schedule.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.386551 edc-lab-results-0.1.38/edc_lab_results.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1644 2023-05-24 17:18:39.000000 edc-lab-results-0.1.38/edc_lab_results.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     2465 2023-05-24 17:18:39.000000 edc-lab-results-0.1.38/edc_lab_results.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-24 17:18:39.000000 edc-lab-results-0.1.38/edc_lab_results.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-07 00:14:15.000000 edc-lab-results-0.1.38/edc_lab_results.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       16 2023-05-24 17:18:39.000000 edc-lab-results-0.1.38/edc_lab_results.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1776 2023-05-24 17:18:30.000000 edc-lab-results-0.1.38/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2211 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1210 2023-05-24 17:18:39.393426 edc-lab-results-0.1.38/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.491017 edc-lab-results-0.1.39/
+-rw-r--r--   0 erikvw     (501) staff       (20)       76 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.477632 edc-lab-results-0.1.39/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.481223 edc-lab-results-0.1.39/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 17:18:30.000000 edc-lab-results-0.1.39/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1842 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 17:18:30.000000 edc-lab-results-0.1.39/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-09 19:25:16.000000 edc-lab-results-0.1.39/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)      402 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-06-25 20:27:10.000000 edc-lab-results-0.1.39/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1644 2023-08-01 04:34:50.491112 edc-lab-results-0.1.39/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      733 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-09 19:25:16.000000 edc-lab-results-0.1.39/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.482847 edc-lab-results-0.1.39/edc_lab_results/
+-rw-r--r--   0 erikvw     (501) staff       (20)      276 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3809 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/edc_lab_results/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.484120 edc-lab-results-0.1.39/edc_lab_results/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      154 2022-10-26 16:30:10.000000 edc-lab-results-0.1.39/edc_lab_results/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-10-26 16:30:10.000000 edc-lab-results-0.1.39/edc_lab_results/admin/blood_results_modeladmin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1867 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/edc_lab_results/admin/reportable_results_modeladmin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      157 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1002 2022-07-27 02:24:23.000000 edc-lab-results-0.1.39/edc_lab_results/calculate_missing.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      504 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3813 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/edc_lab_results/fieldsets.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.485011 edc-lab-results-0.1.39/edc_lab_results/form_validator_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      251 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/form_validator_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      836 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/form_validator_mixins/blood_results_fbg_form_validator_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3990 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/edc_lab_results/form_validator_mixins/blood_results_form_validator_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      437 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/form_validator_mixins/blood_results_glu_form_validator_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.487670 edc-lab-results-0.1.39/edc_lab_results/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1189 2022-08-15 00:51:30.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4343 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/blood_result_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      955 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/electrolytes_model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4420 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/fbc_model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1749 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/fbg_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1748 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/glucose_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1267 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/hba1c_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1140 2023-05-24 17:18:30.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/insulin_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3107 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/lft_model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1723 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/lipid_model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      426 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/proteinuria_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1367 2022-08-15 00:51:30.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/rft_model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.489058 edc-lab-results-0.1.39/edc_lab_results/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.490395 edc-lab-results-0.1.39/edc_lab_results/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1367 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/edc_lab_results/tests/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      508 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)      683 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/lab_profiles.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2039 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/edc_lab_results/tests/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2708 2023-08-01 04:34:43.000000 edc-lab-results-0.1.39/edc_lab_results/tests/test_case_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.490891 edc-lab-results-0.1.39/edc_lab_results/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4466 2023-08-01 04:34:43.000000 edc-lab-results-0.1.39/edc_lab_results/tests/tests/test_blood_result.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7389 2023-08-01 04:34:43.000000 edc-lab-results-0.1.39/edc_lab_results/tests/tests/test_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      261 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2104 2022-09-30 01:31:16.000000 edc-lab-results-0.1.39/edc_lab_results/tests/visit_schedule.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.483584 edc-lab-results-0.1.39/edc_lab_results.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1644 2023-08-01 04:34:50.000000 edc-lab-results-0.1.39/edc_lab_results.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     2465 2023-08-01 04:34:50.000000 edc-lab-results-0.1.39/edc_lab_results.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-08-01 04:34:50.000000 edc-lab-results-0.1.39/edc_lab_results.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-07 00:14:15.000000 edc-lab-results-0.1.39/edc_lab_results.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       16 2023-08-01 04:34:50.000000 edc-lab-results-0.1.39/edc_lab_results.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1776 2023-05-24 17:18:30.000000 edc-lab-results-0.1.39/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2217 2023-08-01 04:34:43.000000 edc-lab-results-0.1.39/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1210 2023-08-01 04:34:50.491441 edc-lab-results-0.1.39/setup.cfg
```

### Comparing `edc-lab-results-0.1.38/.github/workflows/build.yml` & `edc-lab-results-0.1.39/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/.gitignore` & `edc-lab-results-0.1.39/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/.pre-commit-config.yaml` & `edc-lab-results-0.1.39/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/LICENSE` & `edc-lab-results-0.1.39/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/PKG-INFO` & `edc-lab-results-0.1.39/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-lab-results
-Version: 0.1.38
+Version: 0.1.39
 Summary: Simple blood result data collection format model classes for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-lab-results
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django laboratory data collection,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-lab-results-0.1.38/README.rst` & `edc-lab-results-0.1.39/README.rst`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/action_items.py` & `edc-lab-results-0.1.39/edc_lab_results/action_items.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/admin/reportable_results_modeladmin_mixin.py` & `edc-lab-results-0.1.39/edc_lab_results/admin/reportable_results_modeladmin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/calculate_missing.py` & `edc-lab-results-0.1.39/edc_lab_results/calculate_missing.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/fieldsets.py` & `edc-lab-results-0.1.39/edc_lab_results/fieldsets.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/form_validator_mixins/blood_results_fbg_form_validator_mixin.py` & `edc-lab-results-0.1.39/edc_lab_results/form_validator_mixins/blood_results_fbg_form_validator_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/form_validator_mixins/blood_results_form_validator_mixin.py` & `edc-lab-results-0.1.39/edc_lab_results/form_validator_mixins/blood_results_form_validator_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/model_mixins/__init__.py` & `edc-lab-results-0.1.39/edc_lab_results/model_mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/model_mixins/blood_result_model_mixin.py` & `edc-lab-results-0.1.39/edc_lab_results/model_mixins/blood_result_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/model_mixins/electrolytes_model_mixins.py` & `edc-lab-results-0.1.39/edc_lab_results/model_mixins/electrolytes_model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/model_mixins/fbc_model_mixins.py` & `edc-lab-results-0.1.39/edc_lab_results/model_mixins/fbc_model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/model_mixins/fbg_model_mixin.py` & `edc-lab-results-0.1.39/edc_lab_results/model_mixins/fbg_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/model_mixins/glucose_model_mixin.py` & `edc-lab-results-0.1.39/edc_lab_results/model_mixins/glucose_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/model_mixins/hba1c_model_mixin.py` & `edc-lab-results-0.1.39/edc_lab_results/model_mixins/hba1c_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/model_mixins/insulin_model_mixin.py` & `edc-lab-results-0.1.39/edc_lab_results/model_mixins/insulin_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/model_mixins/lft_model_mixins.py` & `edc-lab-results-0.1.39/edc_lab_results/model_mixins/lft_model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/model_mixins/lipid_model_mixins.py` & `edc-lab-results-0.1.39/edc_lab_results/model_mixins/lipid_model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/model_mixins/rft_model_mixins.py` & `edc-lab-results-0.1.39/edc_lab_results/model_mixins/rft_model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/tests/etc/user-rsa-local-private.pem` & `edc-lab-results-0.1.39/edc_lab_results/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/tests/etc/user-rsa-restricted-private.pem` & `edc-lab-results-0.1.39/edc_lab_results/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/tests/forms.py` & `edc-lab-results-0.1.39/edc_lab_results/tests/forms.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/tests/lab_profiles.py` & `edc-lab-results-0.1.39/edc_lab_results/tests/lab_profiles.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/tests/models.py` & `edc-lab-results-0.1.39/edc_lab_results/tests/models.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results/tests/test_case_mixin.py` & `edc-lab-results-0.1.39/edc_lab_results/tests/test_case_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         )
         import_holidays()
         site_reportables.register(
             name="my_reportables", normal_data=normal_data, grading_data=grading_data
         )
         site_labs.register(lab_profile=subject_lab_profile)
         site_reference_configs.register_from_visit_schedule(
-            visit_models={"edc_appointment.appointment": "edc_metadata.subjectvisit"}
+            visit_models={"edc_appointment.appointment": "edc_visit_tracking.subjectvisit"}
         )
         register_actions()
 
     @staticmethod
     def enroll(subject_identifier=None):
         subject_identifier = subject_identifier or "1111111"
         subject_consent = SubjectConsent.objects.create(
```

### Comparing `edc-lab-results-0.1.38/edc_lab_results/tests/tests/test_blood_result.py` & `edc-lab-results-0.1.39/edc_lab_results/tests/tests/test_blood_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,17 @@
     def setUp(self):
         super().setUp()
         self.subject_identifier = self.enroll()
         appointment = Appointment.objects.get(
             subject_identifier=self.subject_identifier,
             visit_code="1000",
         )
-        subject_visit = django_apps.get_model("edc_metadata.subjectvisit").objects.create(
+        subject_visit = django_apps.get_model(
+            "edc_visit_tracking.subjectvisit"
+        ).objects.create(
             report_datetime=get_utcnow(),
             appointment=appointment,
             reason=SCHEDULED,
         )
         panel = Panel.objects.get(name="fbc")
         requisition = django_apps.get_model("edc_metadata.subjectrequisition").objects.create(
             subject_visit=subject_visit,
```

### Comparing `edc-lab-results-0.1.38/edc_lab_results/tests/tests/test_form.py` & `edc-lab-results-0.1.39/edc_lab_results/tests/tests/test_form.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,17 @@
         site_action_items.registry = {}
         register_actions()
         self.subject_identifier = self.enroll()
         appointment = Appointment.objects.get(
             subject_identifier=self.subject_identifier,
             visit_code="1000",
         )
-        self.subject_visit = django_apps.get_model("edc_metadata.subjectvisit").objects.create(
+        self.subject_visit = django_apps.get_model(
+            "edc_visit_tracking.subjectvisit"
+        ).objects.create(
             report_datetime=get_utcnow(),
             appointment=appointment,
             reason=SCHEDULED,
         )
         fbc_panel = Panel.objects.get(name="fbc")
         requisition = django_apps.get_model("edc_metadata.subjectrequisition").objects.create(
             subject_visit=self.subject_visit,
@@ -124,15 +126,17 @@
         site_action_items.registry = {}
         register_actions()
         self.subject_identifier = self.enroll()
         appointment = Appointment.objects.get(
             subject_identifier=self.subject_identifier,
             visit_code="1000",
         )
-        self.subject_visit = django_apps.get_model("edc_metadata.subjectvisit").objects.create(
+        self.subject_visit = django_apps.get_model(
+            "edc_visit_tracking.subjectvisit"
+        ).objects.create(
             report_datetime=get_utcnow(),
             appointment=appointment,
             reason=SCHEDULED,
         )
         self.data = dict(
             report_datetime=self.subject_visit.report_datetime,
             subject_visit=self.subject_visit,
```

### Comparing `edc-lab-results-0.1.38/edc_lab_results/tests/visit_schedule.py` & `edc-lab-results-0.1.39/edc_lab_results/tests/visit_schedule.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/edc_lab_results.egg-info/PKG-INFO` & `edc-lab-results-0.1.39/edc_lab_results.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-lab-results
-Version: 0.1.38
+Version: 0.1.39
 Summary: Simple blood result data collection format model classes for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-lab-results
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django laboratory data collection,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-lab-results-0.1.38/edc_lab_results.egg-info/SOURCES.txt` & `edc-lab-results-0.1.39/edc_lab_results.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/pyproject.toml` & `edc-lab-results-0.1.39/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.38/runtests.py` & `edc-lab-results-0.1.39/runtests.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 project_settings = DefaultTestSettings(
     calling_file=__file__,
     BASE_DIR=base_dir,
     APP_NAME=app_name,
     ETC_DIR=join(base_dir, app_name, "tests", "etc"),
     SUBJECT_SCREENING_MODEL="edc_metadata.subjectscreening",
     SUBJECT_CONSENT_MODEL="edc_metadata.subjectconsent",
-    SUBJECT_VISIT_MODEL="edc_metadata.subjectvisit",
+    SUBJECT_VISIT_MODEL="edc_visit_tracking.subjectvisit",
     SUBJECT_VISIT_MISSED_MODEL="edc_metadata.subjectvisitmissed",
     SUBJECT_REQUISITION_MODEL="edc_metadata.subjectrequisition",
     EDC_BLOOD_RESULTS_MODEL_APP_LABEL="edc_lab_results",
     LIST_MODEL_APP_LABEL="edc_metadata",
     INSTALLED_APPS=[
         "django.contrib.admin",
         "django.contrib.auth",
```

### Comparing `edc-lab-results-0.1.38/setup.cfg` & `edc-lab-results-0.1.39/setup.cfg`

 * *Files identical despite different names*

