# Comparing `tmp/edc-model-fields-0.3.7.tar.gz` & `tmp/edc-model-fields-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-model-fields-0.3.7.tar", last modified: Wed May 24 16:32:55 2023, max compression
+gzip compressed data, was "edc-model-fields-0.3.8.tar", last modified: Tue Aug  1 05:07:06 2023, max compression
```

## Comparing `edc-model-fields-0.3.7.tar` & `edc-model-fields-0.3.8.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:32:55.633887 edc-model-fields-0.3.7/
--rw-r--r--   0 erikvw     (501) staff       (20)      107 2020-03-04 22:59:17.000000 edc-model-fields-0.3.7/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-08 16:53:28.000000 edc-model-fields-0.3.7/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:32:55.623777 edc-model-fields-0.3.7/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:32:55.628007 edc-model-fields-0.3.7/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 16:32:46.000000 edc-model-fields-0.3.7/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1478 2022-09-25 19:19:15.000000 edc-model-fields-0.3.7/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 16:32:46.000000 edc-model-fields-0.3.7/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-09-25 19:19:15.000000 edc-model-fields-0.3.7/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-25 19:19:15.000000 edc-model-fields-0.3.7/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-25 19:19:15.000000 edc-model-fields-0.3.7/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-03-04 22:58:48.000000 edc-model-fields-0.3.7/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      165 2022-09-25 19:19:15.000000 edc-model-fields-0.3.7/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1505 2023-05-24 16:32:55.633987 edc-model-fields-0.3.7/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      628 2022-09-25 19:19:15.000000 edc-model-fields-0.3.7/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-09-25 19:19:15.000000 edc-model-fields-0.3.7/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:32:55.628501 edc-model-fields-0.3.7/edc_model_fields/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:59:17.000000 edc-model-fields-0.3.7/edc_model_fields/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      157 2022-09-25 19:32:50.000000 edc-model-fields-0.3.7/edc_model_fields/apps.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:32:55.630517 edc-model-fields-0.3.7/edc_model_fields/fields/
--rw-r--r--   0 erikvw     (501) staff       (20)      385 2020-03-04 22:59:17.000000 edc-model-fields-0.3.7/edc_model_fields/fields/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1695 2022-09-25 19:32:50.000000 edc-model-fields-0.3.7/edc_model_fields/fields/date_estimated.py
--rw-r--r--   0 erikvw     (501) staff       (20)      555 2023-05-24 16:32:46.000000 edc-model-fields-0.3.7/edc_model_fields/fields/hostname_modification_field.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1203 2022-09-25 19:32:50.000000 edc-model-fields-0.3.7/edc_model_fields/fields/identity_type_field.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1129 2023-05-24 16:32:46.000000 edc-model-fields-0.3.7/edc_model_fields/fields/initials_field.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1014 2022-09-25 19:32:50.000000 edc-model-fields-0.3.7/edc_model_fields/fields/other_charfield.py
--rw-r--r--   0 erikvw     (501) staff       (20)      861 2023-05-24 16:32:46.000000 edc-model-fields-0.3.7/edc_model_fields/fields/userfield.py
--rw-r--r--   0 erikvw     (501) staff       (20)      281 2022-09-25 19:32:50.000000 edc-model-fields-0.3.7/edc_model_fields/fields/uuid_auto_field.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-25 19:32:50.000000 edc-model-fields-0.3.7/edc_model_fields/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:32:55.624086 edc-model-fields-0.3.7/edc_model_fields/static/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:32:55.630979 edc-model-fields-0.3.7/edc_model_fields/static/edc_model_fields/
--rw-r--r--   0 erikvw     (501) staff       (20)     1359 2022-09-25 19:19:15.000000 edc-model-fields-0.3.7/edc_model_fields/static/edc_model_fields/slider.css
--rw-r--r--   0 erikvw     (501) staff       (20)    10150 2020-10-20 21:23:27.000000 edc-model-fields-0.3.7/edc_model_fields/static/edc_model_fields/slider.png
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:32:55.624213 edc-model-fields-0.3.7/edc_model_fields/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:32:55.624258 edc-model-fields-0.3.7/edc_model_fields/templates/edc_model_fields/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:32:55.631153 edc-model-fields-0.3.7/edc_model_fields/templates/edc_model_fields/widgets/
--rw-r--r--   0 erikvw     (501) staff       (20)      917 2020-10-20 21:23:27.000000 edc-model-fields-0.3.7/edc_model_fields/templates/edc_model_fields/widgets/slider.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:32:55.631686 edc-model-fields-0.3.7/edc_model_fields/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:59:17.000000 edc-model-fields-0.3.7/edc_model_fields/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:32:55.633049 edc-model-fields-0.3.7/edc_model_fields/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-08 16:59:53.000000 edc-model-fields-0.3.7/edc_model_fields/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-08 16:59:53.000000 edc-model-fields-0.3.7/edc_model_fields/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2021-02-08 16:59:53.000000 edc-model-fields-0.3.7/edc_model_fields/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-02-08 16:59:53.000000 edc-model-fields-0.3.7/edc_model_fields/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-02-08 16:59:53.000000 edc-model-fields-0.3.7/edc_model_fields/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-02-08 16:59:53.000000 edc-model-fields-0.3.7/edc_model_fields/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-08 16:59:53.000000 edc-model-fields-0.3.7/edc_model_fields/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-08 16:59:53.000000 edc-model-fields-0.3.7/edc_model_fields/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      522 2020-03-10 04:06:14.000000 edc-model-fields-0.3.7/edc_model_fields/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)      417 2023-05-24 16:32:46.000000 edc-model-fields-0.3.7/edc_model_fields/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:32:55.633316 edc-model-fields-0.3.7/edc_model_fields/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-08 16:53:28.000000 edc-model-fields-0.3.7/edc_model_fields/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3469 2021-02-08 16:53:28.000000 edc-model-fields-0.3.7/edc_model_fields/tests/tests/test_fields.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-04 22:59:17.000000 edc-model-fields-0.3.7/edc_model_fields/tests/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:32:55.633748 edc-model-fields-0.3.7/edc_model_fields/widgets/
--rw-r--r--   0 erikvw     (501) staff       (20)       40 2020-10-20 21:23:27.000000 edc-model-fields-0.3.7/edc_model_fields/widgets/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1224 2020-10-20 21:23:27.000000 edc-model-fields-0.3.7/edc_model_fields/widgets/slider_widget.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:32:55.629170 edc-model-fields-0.3.7/edc_model_fields.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1505 2023-05-24 16:32:55.000000 edc-model-fields-0.3.7/edc_model_fields.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1706 2023-05-24 16:32:55.000000 edc-model-fields-0.3.7/edc_model_fields.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-24 16:32:55.000000 edc-model-fields-0.3.7/edc_model_fields.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 22:59:17.000000 edc-model-fields-0.3.7/edc_model_fields.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       17 2023-05-24 16:32:55.000000 edc-model-fields-0.3.7/edc_model_fields.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1778 2023-05-24 16:32:46.000000 edc-model-fields-0.3.7/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1950 2022-09-25 19:13:53.000000 edc-model-fields-0.3.7/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1176 2023-05-24 16:32:55.634311 edc-model-fields-0.3.7/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:07:06.268171 edc-model-fields-0.3.8/
+-rw-r--r--   0 erikvw     (501) staff       (20)      107 2020-03-04 22:59:17.000000 edc-model-fields-0.3.8/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-08 16:53:28.000000 edc-model-fields-0.3.8/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:07:06.257075 edc-model-fields-0.3.8/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:07:06.262479 edc-model-fields-0.3.8/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 16:32:46.000000 edc-model-fields-0.3.8/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1478 2022-09-25 19:19:15.000000 edc-model-fields-0.3.8/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 16:32:46.000000 edc-model-fields-0.3.8/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-09-25 19:19:15.000000 edc-model-fields-0.3.8/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-25 19:19:15.000000 edc-model-fields-0.3.8/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-25 19:19:15.000000 edc-model-fields-0.3.8/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-03-04 22:58:48.000000 edc-model-fields-0.3.8/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      165 2022-09-25 19:19:15.000000 edc-model-fields-0.3.8/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1505 2023-08-01 05:07:06.268273 edc-model-fields-0.3.8/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      628 2022-09-25 19:19:15.000000 edc-model-fields-0.3.8/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-09-25 19:19:15.000000 edc-model-fields-0.3.8/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:07:06.263029 edc-model-fields-0.3.8/edc_model_fields/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:59:17.000000 edc-model-fields-0.3.8/edc_model_fields/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      157 2022-09-25 19:32:50.000000 edc-model-fields-0.3.8/edc_model_fields/apps.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:07:06.265175 edc-model-fields-0.3.8/edc_model_fields/fields/
+-rw-r--r--   0 erikvw     (501) staff       (20)      385 2020-03-04 22:59:17.000000 edc-model-fields-0.3.8/edc_model_fields/fields/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1695 2022-09-25 19:32:50.000000 edc-model-fields-0.3.8/edc_model_fields/fields/date_estimated.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      555 2023-05-24 16:32:46.000000 edc-model-fields-0.3.8/edc_model_fields/fields/hostname_modification_field.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1203 2022-09-25 19:32:50.000000 edc-model-fields-0.3.8/edc_model_fields/fields/identity_type_field.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1129 2023-05-24 16:32:46.000000 edc-model-fields-0.3.8/edc_model_fields/fields/initials_field.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1014 2022-09-25 19:32:50.000000 edc-model-fields-0.3.8/edc_model_fields/fields/other_charfield.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      861 2023-05-24 16:32:46.000000 edc-model-fields-0.3.8/edc_model_fields/fields/userfield.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      281 2022-09-25 19:32:50.000000 edc-model-fields-0.3.8/edc_model_fields/fields/uuid_auto_field.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-25 19:32:50.000000 edc-model-fields-0.3.8/edc_model_fields/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:07:06.257386 edc-model-fields-0.3.8/edc_model_fields/static/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:07:06.265669 edc-model-fields-0.3.8/edc_model_fields/static/edc_model_fields/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1359 2022-09-25 19:19:15.000000 edc-model-fields-0.3.8/edc_model_fields/static/edc_model_fields/slider.css
+-rw-r--r--   0 erikvw     (501) staff       (20)    10150 2020-10-20 21:23:27.000000 edc-model-fields-0.3.8/edc_model_fields/static/edc_model_fields/slider.png
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:07:06.257498 edc-model-fields-0.3.8/edc_model_fields/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:07:06.257544 edc-model-fields-0.3.8/edc_model_fields/templates/edc_model_fields/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:07:06.265832 edc-model-fields-0.3.8/edc_model_fields/templates/edc_model_fields/widgets/
+-rw-r--r--   0 erikvw     (501) staff       (20)      917 2020-10-20 21:23:27.000000 edc-model-fields-0.3.8/edc_model_fields/templates/edc_model_fields/widgets/slider.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:07:06.266365 edc-model-fields-0.3.8/edc_model_fields/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:59:17.000000 edc-model-fields-0.3.8/edc_model_fields/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:07:06.267508 edc-model-fields-0.3.8/edc_model_fields/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-08 16:59:53.000000 edc-model-fields-0.3.8/edc_model_fields/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-08 16:59:53.000000 edc-model-fields-0.3.8/edc_model_fields/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2021-02-08 16:59:53.000000 edc-model-fields-0.3.8/edc_model_fields/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-02-08 16:59:53.000000 edc-model-fields-0.3.8/edc_model_fields/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-02-08 16:59:53.000000 edc-model-fields-0.3.8/edc_model_fields/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-02-08 16:59:53.000000 edc-model-fields-0.3.8/edc_model_fields/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-08 16:59:53.000000 edc-model-fields-0.3.8/edc_model_fields/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-08 16:59:53.000000 edc-model-fields-0.3.8/edc_model_fields/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      522 2020-03-10 04:06:14.000000 edc-model-fields-0.3.8/edc_model_fields/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)      417 2023-05-24 16:32:46.000000 edc-model-fields-0.3.8/edc_model_fields/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:07:06.267737 edc-model-fields-0.3.8/edc_model_fields/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-08 16:53:28.000000 edc-model-fields-0.3.8/edc_model_fields/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3469 2021-02-08 16:53:28.000000 edc-model-fields-0.3.8/edc_model_fields/tests/tests/test_fields.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-04 22:59:17.000000 edc-model-fields-0.3.8/edc_model_fields/tests/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:07:06.268044 edc-model-fields-0.3.8/edc_model_fields/widgets/
+-rw-r--r--   0 erikvw     (501) staff       (20)       40 2020-10-20 21:23:27.000000 edc-model-fields-0.3.8/edc_model_fields/widgets/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1224 2020-10-20 21:23:27.000000 edc-model-fields-0.3.8/edc_model_fields/widgets/slider_widget.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:07:06.263663 edc-model-fields-0.3.8/edc_model_fields.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1505 2023-08-01 05:07:06.000000 edc-model-fields-0.3.8/edc_model_fields.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1706 2023-08-01 05:07:06.000000 edc-model-fields-0.3.8/edc_model_fields.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-08-01 05:07:06.000000 edc-model-fields-0.3.8/edc_model_fields.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 22:59:17.000000 edc-model-fields-0.3.8/edc_model_fields.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       17 2023-08-01 05:07:06.000000 edc-model-fields-0.3.8/edc_model_fields.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1778 2023-05-24 16:32:46.000000 edc-model-fields-0.3.8/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2009 2023-08-01 05:06:58.000000 edc-model-fields-0.3.8/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1176 2023-08-01 05:07:06.268565 edc-model-fields-0.3.8/setup.cfg
```

### Comparing `edc-model-fields-0.3.7/.github/workflows/build.yml` & `edc-model-fields-0.3.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-model-fields-0.3.7/.gitignore` & `edc-model-fields-0.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-model-fields-0.3.7/.pre-commit-config.yaml` & `edc-model-fields-0.3.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-model-fields-0.3.7/LICENSE` & `edc-model-fields-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-model-fields-0.3.7/PKG-INFO` & `edc-model-fields-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-model-fields
-Version: 0.3.7
+Version: 0.3.8
 Summary: Model field classes for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-model-fields
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django model field class django edc clinicedc clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-model-fields-0.3.7/README.rst` & `edc-model-fields-0.3.8/README.rst`

 * *Files identical despite different names*

### Comparing `edc-model-fields-0.3.7/edc_model_fields/fields/date_estimated.py` & `edc-model-fields-0.3.8/edc_model_fields/fields/date_estimated.py`

 * *Files identical despite different names*

### Comparing `edc-model-fields-0.3.7/edc_model_fields/fields/hostname_modification_field.py` & `edc-model-fields-0.3.8/edc_model_fields/fields/hostname_modification_field.py`

 * *Files identical despite different names*

### Comparing `edc-model-fields-0.3.7/edc_model_fields/fields/identity_type_field.py` & `edc-model-fields-0.3.8/edc_model_fields/fields/identity_type_field.py`

 * *Files identical despite different names*

### Comparing `edc-model-fields-0.3.7/edc_model_fields/fields/initials_field.py` & `edc-model-fields-0.3.8/edc_model_fields/fields/initials_field.py`

 * *Files identical despite different names*

### Comparing `edc-model-fields-0.3.7/edc_model_fields/fields/other_charfield.py` & `edc-model-fields-0.3.8/edc_model_fields/fields/other_charfield.py`

 * *Files identical despite different names*

### Comparing `edc-model-fields-0.3.7/edc_model_fields/fields/userfield.py` & `edc-model-fields-0.3.8/edc_model_fields/fields/userfield.py`

 * *Files identical despite different names*

### Comparing `edc-model-fields-0.3.7/edc_model_fields/static/edc_model_fields/slider.css` & `edc-model-fields-0.3.8/edc_model_fields/static/edc_model_fields/slider.css`

 * *Files identical despite different names*

### Comparing `edc-model-fields-0.3.7/edc_model_fields/static/edc_model_fields/slider.png` & `edc-model-fields-0.3.8/edc_model_fields/static/edc_model_fields/slider.png`

 * *Files identical despite different names*

### Comparing `edc-model-fields-0.3.7/edc_model_fields/templates/edc_model_fields/widgets/slider.html` & `edc-model-fields-0.3.8/edc_model_fields/templates/edc_model_fields/widgets/slider.html`

 * *Files identical despite different names*

### Comparing `edc-model-fields-0.3.7/edc_model_fields/tests/etc/user-rsa-local-private.pem` & `edc-model-fields-0.3.8/edc_model_fields/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-model-fields-0.3.7/edc_model_fields/tests/etc/user-rsa-restricted-private.pem` & `edc-model-fields-0.3.8/edc_model_fields/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-model-fields-0.3.7/edc_model_fields/tests/holidays.csv` & `edc-model-fields-0.3.8/edc_model_fields/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `edc-model-fields-0.3.7/edc_model_fields/tests/tests/test_fields.py` & `edc-model-fields-0.3.8/edc_model_fields/tests/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `edc-model-fields-0.3.7/edc_model_fields/widgets/slider_widget.py` & `edc-model-fields-0.3.8/edc_model_fields/widgets/slider_widget.py`

 * *Files identical despite different names*

### Comparing `edc-model-fields-0.3.7/edc_model_fields.egg-info/PKG-INFO` & `edc-model-fields-0.3.8/edc_model_fields.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-model-fields
-Version: 0.3.7
+Version: 0.3.8
 Summary: Model field classes for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-model-fields
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django model field class django edc clinicedc clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-model-fields-0.3.7/edc_model_fields.egg-info/SOURCES.txt` & `edc-model-fields-0.3.8/edc_model_fields.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-model-fields-0.3.7/pyproject.toml` & `edc-model-fields-0.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-model-fields-0.3.7/runtests.py` & `edc-model-fields-0.3.8/runtests.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 base_dir = dirname(abspath(__file__))
 
 DEFAULT_SETTINGS = DefaultTestSettings(
     calling_file=__file__,
     template_dirs=[os.path.join(base_dir, app_name, "tests", "templates")],
     BASE_DIR=base_dir,
     APP_NAME=app_name,
+    SUBJECT_VISIT_MODEL="edc_visit_tracking.subjectvisit",
     INSTALLED_APPS=[
         "django.contrib.admin",
         "django.contrib.auth",
         "django.contrib.contenttypes",
         "django.contrib.sessions",
         "django.contrib.messages",
         "django.contrib.staticfiles",
```

### Comparing `edc-model-fields-0.3.7/setup.cfg` & `edc-model-fields-0.3.8/setup.cfg`

 * *Files identical despite different names*

