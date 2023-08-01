# Comparing `tmp/edc-rx-0.1.7.tar.gz` & `tmp/edc-rx-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-rx-0.1.7.tar", last modified: Wed Jul 12 23:51:00 2023, max compression
+gzip compressed data, was "edc-rx-0.1.8.tar", last modified: Tue Aug  1 05:30:14 2023, max compression
```

## Comparing `edc-rx-0.1.7.tar` & `edc-rx-0.1.8.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.970413 edc-rx-0.1.7/
--rw-r--r--   0 erikvw     (501) staff       (20)       78 2022-11-29 04:55:26.000000 edc-rx-0.1.7/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-29 04:55:26.000000 edc-rx-0.1.7/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.961844 edc-rx-0.1.7/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.965728 edc-rx-0.1.7/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 15:54:44.000000 edc-rx-0.1.7/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-11-29 04:55:26.000000 edc-rx-0.1.7/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1173 2023-05-24 15:54:44.000000 edc-rx-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-29 04:55:26.000000 edc-rx-0.1.7/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.7/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.7/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-29 03:26:32.000000 edc-rx-0.1.7/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-11-29 04:55:26.000000 edc-rx-0.1.7/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1487 2023-07-12 23:51:00.970514 edc-rx-0.1.7/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      613 2022-11-29 04:55:26.000000 edc-rx-0.1.7/README.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.966646 edc-rx-0.1.7/edc_rx/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      157 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      270 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/apps.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.967700 edc-rx-0.1.7/edc_rx/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)     5179 2023-04-18 01:41:25.000000 edc-rx-0.1.7/edc_rx/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 06:36:26.000000 edc-rx-0.1.7/edc_rx/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.968276 edc-rx-0.1.7/edc_rx/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      181 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1612 2023-07-12 23:50:53.000000 edc-rx-0.1.7/edc_rx/model_mixins/drug_refill_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      865 2023-04-18 01:41:25.000000 edc-rx-0.1.7/edc_rx/model_mixins/drug_supply_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1249 2023-04-18 01:41:25.000000 edc-rx-0.1.7/edc_rx/model_mixins/treatment_pay_methods.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.968661 edc-rx-0.1.7/edc_rx/modeladmin_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/modeladmin_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1237 2023-07-12 23:50:53.000000 edc-rx-0.1.7/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      723 2023-07-12 23:50:53.000000 edc-rx-0.1.7/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.968908 edc-rx-0.1.7/edc_rx/modelform_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)       73 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/modelform_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2047 2023-07-12 23:50:53.000000 edc-rx-0.1.7/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      440 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.969011 edc-rx-0.1.7/edc_rx/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.7/edc_rx/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.970077 edc-rx-0.1.7/edc_rx/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/tests/etc/user-salt-restricted.key
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.970300 edc-rx-0.1.7/edc_rx/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.7/edc_rx/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4204 2023-07-12 23:50:53.000000 edc-rx-0.1.7/edc_rx/tests/tests/test_utils.py
--rw-r--r--   0 erikvw     (501) staff       (20)      277 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      757 2023-07-12 23:50:53.000000 edc-rx-0.1.7/edc_rx/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.967329 edc-rx-0.1.7/edc_rx.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1487 2023-07-12 23:51:00.000000 edc-rx-0.1.7/edc_rx.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1335 2023-07-12 23:51:00.000000 edc-rx-0.1.7/edc_rx.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-12 23:51:00.000000 edc-rx-0.1.7/edc_rx.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-29 04:55:34.000000 edc-rx-0.1.7/edc_rx.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)        7 2023-07-12 23:51:00.000000 edc-rx-0.1.7/edc_rx.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1758 2023-05-24 15:54:44.000000 edc-rx-0.1.7/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1106 2023-03-31 01:08:39.000000 edc-rx-0.1.7/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1166 2023-07-12 23:51:00.970837 edc-rx-0.1.7/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.360447 edc-rx-0.1.8/
+-rw-r--r--   0 erikvw     (501) staff       (20)       78 2022-11-29 04:55:26.000000 edc-rx-0.1.8/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-29 04:55:26.000000 edc-rx-0.1.8/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.351813 edc-rx-0.1.8/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.355169 edc-rx-0.1.8/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 15:54:44.000000 edc-rx-0.1.8/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-11-29 04:55:26.000000 edc-rx-0.1.8/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1173 2023-05-24 15:54:44.000000 edc-rx-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-29 04:55:26.000000 edc-rx-0.1.8/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.8/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.8/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-29 03:26:32.000000 edc-rx-0.1.8/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-11-29 04:55:26.000000 edc-rx-0.1.8/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1487 2023-08-01 05:30:14.360540 edc-rx-0.1.8/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      613 2022-11-29 04:55:26.000000 edc-rx-0.1.8/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.356082 edc-rx-0.1.8/edc_rx/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      157 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      270 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/apps.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.357295 edc-rx-0.1.8/edc_rx/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)     5179 2023-04-18 01:41:25.000000 edc-rx-0.1.8/edc_rx/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 06:36:26.000000 edc-rx-0.1.8/edc_rx/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.357886 edc-rx-0.1.8/edc_rx/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      181 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1610 2023-08-01 05:30:07.000000 edc-rx-0.1.8/edc_rx/model_mixins/drug_refill_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      865 2023-04-18 01:41:25.000000 edc-rx-0.1.8/edc_rx/model_mixins/drug_supply_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1249 2023-04-18 01:41:25.000000 edc-rx-0.1.8/edc_rx/model_mixins/treatment_pay_methods.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.358404 edc-rx-0.1.8/edc_rx/modeladmin_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/modeladmin_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1237 2023-07-12 23:50:53.000000 edc-rx-0.1.8/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      723 2023-07-12 23:50:53.000000 edc-rx-0.1.8/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.358769 edc-rx-0.1.8/edc_rx/modelform_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)       73 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/modelform_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2047 2023-07-12 23:50:53.000000 edc-rx-0.1.8/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      440 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.358912 edc-rx-0.1.8/edc_rx/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.8/edc_rx/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.360070 edc-rx-0.1.8/edc_rx/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/tests/etc/user-salt-restricted.key
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.360309 edc-rx-0.1.8/edc_rx/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.8/edc_rx/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4204 2023-07-12 23:50:53.000000 edc-rx-0.1.8/edc_rx/tests/tests/test_utils.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      277 2022-11-29 04:55:26.000000 edc-rx-0.1.8/edc_rx/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      757 2023-07-12 23:50:53.000000 edc-rx-0.1.8/edc_rx/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:30:14.356927 edc-rx-0.1.8/edc_rx.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1487 2023-08-01 05:30:14.000000 edc-rx-0.1.8/edc_rx.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1335 2023-08-01 05:30:14.000000 edc-rx-0.1.8/edc_rx.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-08-01 05:30:14.000000 edc-rx-0.1.8/edc_rx.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-29 04:55:34.000000 edc-rx-0.1.8/edc_rx.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)        7 2023-08-01 05:30:14.000000 edc-rx-0.1.8/edc_rx.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1758 2023-05-24 15:54:44.000000 edc-rx-0.1.8/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1106 2023-03-31 01:08:39.000000 edc-rx-0.1.8/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1166 2023-08-01 05:30:14.360826 edc-rx-0.1.8/setup.cfg
```

### Comparing `edc-rx-0.1.7/.github/workflows/build.yml` & `edc-rx-0.1.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.7/.gitignore` & `edc-rx-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.7/.pre-commit-config.yaml` & `edc-rx-0.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.7/LICENSE` & `edc-rx-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.7/PKG-INFO` & `edc-rx-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-rx
-Version: 0.1.7
+Version: 0.1.8
 Summary: Medications refill and supply model/form mixins for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-rx
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc rx-refill,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-rx-0.1.7/README.rst` & `edc-rx-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.7/edc_rx/migrations/0001_initial.py` & `edc-rx-0.1.8/edc_rx/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.7/edc_rx/model_mixins/drug_refill_model_mixin.py` & `edc-rx-0.1.8/edc_rx/model_mixins/drug_refill_model_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,13 +45,13 @@
         verbose_name="If other, please specify ...",
         max_length=150,
         null=True,
         blank=True,
     )
 
     rx_days = models.IntegerField(
-        verbose_name=("Number of days of medication prescribed?"),
+        verbose_name="Number of days of medication prescribed?",
         validators=[MinValueValidator(0), MaxValueValidator(186)],
     )
 
     class Meta:
         abstract = True
```

### Comparing `edc-rx-0.1.7/edc_rx/model_mixins/drug_supply_model_mixin.py` & `edc-rx-0.1.8/edc_rx/model_mixins/drug_supply_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.7/edc_rx/model_mixins/treatment_pay_methods.py` & `edc-rx-0.1.8/edc_rx/model_mixins/treatment_pay_methods.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.7/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py` & `edc-rx-0.1.8/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.7/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py` & `edc-rx-0.1.8/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.7/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py` & `edc-rx-0.1.8/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.7/edc_rx/tests/etc/user-rsa-local-private.pem` & `edc-rx-0.1.8/edc_rx/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.7/edc_rx/tests/etc/user-rsa-restricted-private.pem` & `edc-rx-0.1.8/edc_rx/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.7/edc_rx/tests/tests/test_utils.py` & `edc-rx-0.1.8/edc_rx/tests/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.7/edc_rx/utils.py` & `edc-rx-0.1.8/edc_rx/utils.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.7/edc_rx.egg-info/PKG-INFO` & `edc-rx-0.1.8/edc_rx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-rx
-Version: 0.1.7
+Version: 0.1.8
 Summary: Medications refill and supply model/form mixins for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-rx
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc rx-refill,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-rx-0.1.7/edc_rx.egg-info/SOURCES.txt` & `edc-rx-0.1.8/edc_rx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.7/pyproject.toml` & `edc-rx-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.7/runtests.py` & `edc-rx-0.1.8/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.7/setup.cfg` & `edc-rx-0.1.8/setup.cfg`

 * *Files identical despite different names*

