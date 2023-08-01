# Comparing `tmp/edc-next-appointment-0.1.2.tar.gz` & `tmp/edc-next-appointment-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-next-appointment-0.1.2.tar", last modified: Thu Jul 27 12:18:35 2023, max compression
+gzip compressed data, was "edc-next-appointment-0.1.3.tar", last modified: Tue Aug  1 05:11:37 2023, max compression
```

## Comparing `edc-next-appointment-0.1.2.tar` & `edc-next-appointment-0.1.3.tar`

### file list

```diff
@@ -1,59 +1,72 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.162643 edc-next-appointment-0.1.2/
--rw-r--r--   0 erikvw     (501) staff       (20)      253 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.154609 edc-next-appointment-0.1.2/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.157835 edc-next-appointment-0.1.2/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     3121 2023-07-27 12:18:27.000000 edc-next-appointment-0.1.2/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       23 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2023-07-24 19:09:02.000000 edc-next-appointment-0.1.2/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      126 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     2531 2023-07-27 12:18:35.162732 edc-next-appointment-0.1.2/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1600 2023-07-27 01:53:02.000000 edc-next-appointment-0.1.2/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.159547 edc-next-appointment-0.1.2/edc_next_appointment/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      250 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      184 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/choices.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.160722 edc-next-appointment-0.1.2/edc_next_appointment/form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)      143 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1578 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/form_validators/form_validator_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      309 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/form_validators/next_appointment_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1928 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/form_validators.py
--rw-r--r--   0 erikvw     (501) staff       (20)      550 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.160993 edc-next-appointment-0.1.2/edc_next_appointment/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)     2898 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1789 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1771 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/modeladmin_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4541 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/modelform_mixins.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.161235 edc-next-appointment-0.1.2/edc_next_appointment/models/
--rw-r--r--   0 erikvw     (501) staff       (20)       37 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      224 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/models/list_models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.161378 edc-next-appointment-0.1.2/edc_next_appointment/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.162425 edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/user-salt-restricted.key
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.162553 edc-next-appointment-0.1.2/edc_next_appointment/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      214 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      760 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.160301 edc-next-appointment-0.1.2/edc_next_appointment.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     2531 2023-07-27 12:18:35.000000 edc-next-appointment-0.1.2/edc_next_appointment.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1654 2023-07-27 12:18:35.000000 edc-next-appointment-0.1.2/edc_next_appointment.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-27 12:18:35.000000 edc-next-appointment-0.1.2/edc_next_appointment.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-25 13:58:46.000000 edc-next-appointment-0.1.2/edc_next_appointment.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       21 2023-07-27 12:18:35.000000 edc-next-appointment-0.1.2/edc_next_appointment.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1786 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1860 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1238 2023-07-27 12:18:35.163022 edc-next-appointment-0.1.2/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.682360 edc-next-appointment-0.1.3/
+-rw-r--r--   0 erikvw     (501) staff       (20)      253 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.672717 edc-next-appointment-0.1.3/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.676073 edc-next-appointment-0.1.3/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     3121 2023-07-27 12:18:27.000000 edc-next-appointment-0.1.3/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       23 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2023-07-24 19:09:02.000000 edc-next-appointment-0.1.3/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      126 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     2531 2023-08-01 05:11:37.682454 edc-next-appointment-0.1.3/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1600 2023-07-27 01:53:02.000000 edc-next-appointment-0.1.3/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.677398 edc-next-appointment-0.1.3/edc_next_appointment/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      250 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      184 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/choices.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.678558 edc-next-appointment-0.1.3/edc_next_appointment/form_validators/
+-rw-r--r--   0 erikvw     (501) staff       (20)      143 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/form_validators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1578 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/form_validators/form_validator_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      309 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/form_validators/next_appointment_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2153 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/edc_next_appointment/form_validators.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      550 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.678868 edc-next-appointment-0.1.3/edc_next_appointment/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2898 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1789 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1771 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/modeladmin_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4541 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/modelform_mixins.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.679117 edc-next-appointment-0.1.3/edc_next_appointment/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)       37 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      224 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/models/list_models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.679381 edc-next-appointment-0.1.3/edc_next_appointment/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.680560 edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1019 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.680824 edc-next-appointment-0.1.3/edc_next_appointment/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1972 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/edc_next_appointment/tests/tests/test_next_appointment.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      214 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      760 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/edc_next_appointment/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.678126 edc-next-appointment-0.1.3/edc_next_appointment.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2531 2023-08-01 05:11:37.000000 edc-next-appointment-0.1.3/edc_next_appointment.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     2074 2023-08-01 05:11:37.000000 edc-next-appointment-0.1.3/edc_next_appointment.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-08-01 05:11:37.000000 edc-next-appointment-0.1.3/edc_next_appointment.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-25 13:58:46.000000 edc-next-appointment-0.1.3/edc_next_appointment.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       42 2023-08-01 05:11:37.000000 edc-next-appointment-0.1.3/edc_next_appointment.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:37.682228 edc-next-appointment-0.1.3/next_appointment_app/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/next_appointment_app/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1051 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/next_appointment_app/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      191 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/next_appointment_app/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      165 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/next_appointment_app/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      444 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/next_appointment_app/consents.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2154 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/next_appointment_app/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      292 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/next_appointment_app/navbars.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      694 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/next_appointment_app/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      370 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/next_appointment_app/views.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2051 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/next_appointment_app/visit_schedules.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1786 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.3/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2083 2023-08-01 05:11:30.000000 edc-next-appointment-0.1.3/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1238 2023-08-01 05:11:37.682765 edc-next-appointment-0.1.3/setup.cfg
```

### Comparing `edc-next-appointment-0.1.2/.github/workflows/build.yml` & `edc-next-appointment-0.1.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.2/.gitignore` & `edc-next-appointment-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.2/.pre-commit-config.yaml` & `edc-next-appointment-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.2/LICENSE` & `edc-next-appointment-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.2/PKG-INFO` & `edc-next-appointment-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-next-appointment
-Version: 0.1.2
+Version: 0.1.3
 Summary: Base classes for managing next appointment CRF at each timepoint in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-next-appointment
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc appointment,scheduling,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-next-appointment-0.1.2/README.rst` & `edc-next-appointment-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.2/edc_next_appointment/form_validators/form_validator_mixins.py` & `edc-next-appointment-0.1.3/edc_next_appointment/form_validators/form_validator_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.2/edc_next_appointment/form_validators.py` & `edc-next-appointment-0.1.3/edc_next_appointment/form_validators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,55 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from edc_crf.crf_form_validator import CrfFormValidator
 from edc_dx_review.utils import raise_if_clinical_review_does_not_exist
 from edc_form_validators import INVALID_ERROR
 
+if TYPE_CHECKING:
+    from edc_facility.models import HealthFacility
+
 
 class NextAppointmentFormValidatorMixin(CrfFormValidator):
     def __init__(self, **kwargs):
         self._clinic_days = None
+        self._clinic_days_str = None
+        self._health_facility = None
         super().__init__(**kwargs)
 
     def clean(self):
         raise_if_clinical_review_does_not_exist(self.cleaned_data.get("subject_visit"))
         super().clean()
 
     @property
-    def clinic_days(self) -> list[int]:
-        if not self._clinic_days:
+    def health_facility(self) -> HealthFacility | None:
+        if not self._health_facility:
             if self.cleaned_data.get("health_facility"):
-                self._clinic_days = self.cleaned_data.get("health_facility").clinic_days
-        return self._clinic_days
+                self._health_facility = self.cleaned_data.get("health_facility")
+            else:
+                raise self.raise_validation_error(
+                    {"health_facility": "This field is required."}
+                )
+        return self._health_facility
 
     def validate_date_is_on_clinic_day(self):
         if appt_date := self.cleaned_data.get("appt_date"):
-            if appt_date.isoweekday() > 5:
-                day = "Sat" if appt_date.isoweekday() == 6 else "Sun"
-                raise self.raise_validation_error(
-                    {"appt_date": f"Expected Mon-Fri. Got {day}"},
-                    INVALID_ERROR,
-                )
-        if appt_date and self.cleaned_data.get("subject_visit").site:
-            if (
-                self.integrated_clinic_days
-                and appt_date.isoweekday() not in self.integrated_clinic_days
-            ):
-                dct = dict(zip([1, 2, 3, 4, 5, 6, 7], ["M", "T", "W", "Th", "F", "Sa", "Su"]))
-                expected_days = [v for k, v in dct.items() if k in self.clinic_days]
-                raise self.raise_validation_error(
-                    {
-                        "appt_date": (
-                            "Invalid clinic day. "
-                            f"Expected {''.join(expected_days)}. "
-                            f"Got {appt_date.strftime('%A')}"
-                        )
-                    },
-                    INVALID_ERROR,
-                )
+            if not self.health_facility.clinic_days:
+                if appt_date.isoweekday() > 5:
+                    day = "Sat" if appt_date.isoweekday() == 6 else "Sun"
+                    raise self.raise_validation_error(
+                        {"appt_date": f"Expected Mon-Fri. Got {day}"},
+                        INVALID_ERROR,
+                    )
+            else:
+                if appt_date.isoweekday() not in self.health_facility.clinic_days:
+                    raise self.raise_validation_error(
+                        {
+                            "appt_date": (
+                                "Invalid clinic day for facility. "
+                                f"Expected {self.health_facility.clinic_days_str}. "
+                                f"Got {appt_date.strftime('%A')}"
+                            )
+                        },
+                        INVALID_ERROR,
+                    )
```

### Comparing `edc-next-appointment-0.1.2/edc_next_appointment/list_data.py` & `edc-next-appointment-0.1.3/edc_next_appointment/list_data.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.2/edc_next_appointment/migrations/0001_initial.py` & `edc-next-appointment-0.1.3/edc_next_appointment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.2/edc_next_appointment/model_mixins.py` & `edc-next-appointment-0.1.3/edc_next_appointment/model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.2/edc_next_appointment/modeladmin_mixins.py` & `edc-next-appointment-0.1.3/edc_next_appointment/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.2/edc_next_appointment/modelform_mixins.py` & `edc-next-appointment-0.1.3/edc_next_appointment/modelform_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/user-rsa-local-private.pem` & `edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/user-rsa-restricted-private.pem` & `edc-next-appointment-0.1.3/edc_next_appointment/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.2/edc_next_appointment/utils.py` & `edc-next-appointment-0.1.3/edc_next_appointment/utils.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.2/edc_next_appointment.egg-info/PKG-INFO` & `edc-next-appointment-0.1.3/edc_next_appointment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-next-appointment
-Version: 0.1.2
+Version: 0.1.3
 Summary: Base classes for managing next appointment CRF at each timepoint in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-next-appointment
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc appointment,scheduling,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-next-appointment-0.1.2/edc_next_appointment.egg-info/SOURCES.txt` & `edc-next-appointment-0.1.3/edc_next_appointment.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -32,16 +32,28 @@
 edc_next_appointment/form_validators/form_validator_mixins.py
 edc_next_appointment/form_validators/next_appointment_form_validator.py
 edc_next_appointment/migrations/0001_initial.py
 edc_next_appointment/migrations/__init__.py
 edc_next_appointment/models/__init__.py
 edc_next_appointment/models/list_models.py
 edc_next_appointment/tests/__init__.py
+edc_next_appointment/tests/holidays.csv
 edc_next_appointment/tests/etc/user-aes-local.key
 edc_next_appointment/tests/etc/user-aes-restricted.key
 edc_next_appointment/tests/etc/user-rsa-local-private.pem
 edc_next_appointment/tests/etc/user-rsa-local-public.pem
 edc_next_appointment/tests/etc/user-rsa-restricted-private.pem
 edc_next_appointment/tests/etc/user-rsa-restricted-public.pem
 edc_next_appointment/tests/etc/user-salt-local.key
 edc_next_appointment/tests/etc/user-salt-restricted.key
-edc_next_appointment/tests/tests/__init__.py
+edc_next_appointment/tests/tests/__init__.py
+edc_next_appointment/tests/tests/test_next_appointment.py
+next_appointment_app/__init__.py
+next_appointment_app/admin.py
+next_appointment_app/admin_site.py
+next_appointment_app/apps.py
+next_appointment_app/consents.py
+next_appointment_app/models.py
+next_appointment_app/navbars.py
+next_appointment_app/urls.py
+next_appointment_app/views.py
+next_appointment_app/visit_schedules.py
```

### Comparing `edc-next-appointment-0.1.2/pyproject.toml` & `edc-next-appointment-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.2/runtests.py` & `edc-next-appointment-0.1.3/runtests.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,30 +9,34 @@
 base_dir = dirname(abspath(__file__))
 
 project_settings = DefaultTestSettings(
     calling_file=__file__,
     BASE_DIR=base_dir,
     APP_NAME=app_name,
     ETC_DIR=os.path.join(base_dir, app_name, "tests", "etc"),
-    SUBJECT_VISIT_MODEL="visit_schedule_app.subjectvisit",
+    SUBJECT_VISIT_MODEL="edc_visit_tracking.subjectvisit",
     SUBJECT_VISIT_MISSED_MODEL="visit_schedule_app.subjectvisitmissed",
     INSTALLED_APPS=[
         "django.contrib.admin",
         "django.contrib.auth",
         "django.contrib.contenttypes",
         "django.contrib.messages",
         "django.contrib.sessions",
         "django.contrib.sites",
         "django.contrib.staticfiles",
         "django_crypto_fields.apps.AppConfig",
         "django_revision.apps.AppConfig",
         "multisite",
         "edc_action_item.apps.AppConfig",
+        "edc_adverse_event.apps.AppConfig",
+        "adverse_event_app.apps.AppConfig",
         "edc_appointment.apps.AppConfig",
         "edc_consent.apps.AppConfig",
+        "edc_dashboard.apps.AppConfig",
+        "edc_subject_dashboard.apps.AppConfig",
         "edc_device.apps.AppConfig",
         "edc_export.apps.AppConfig",
         "edc_facility.apps.AppConfig",
         "edc_identifier.apps.AppConfig",
         "edc_list_data.apps.AppConfig",
         "edc_metadata.apps.AppConfig",
         "edc_notification.apps.AppConfig",
@@ -41,14 +45,15 @@
         "edc_registration.apps.AppConfig",
         "edc_sites.apps.AppConfig",
         "edc_timepoint.apps.AppConfig",
         "edc_visit_schedule.apps.AppConfig",
         "visit_schedule_app.apps.AppConfig",
         "edc_visit_tracking.apps.AppConfig",
         "edc_next_appointment.apps.AppConfig",
+        "next_appointment_app.apps.AppConfig",
     ],
     add_dashboard_middleware=True,
 ).settings
 
 
 def main():
     func_main(project_settings, f"{app_name}.tests")
```

### Comparing `edc-next-appointment-0.1.2/setup.cfg` & `edc-next-appointment-0.1.3/setup.cfg`

 * *Files identical despite different names*

