# Comparing `tmp/edc-document-status-0.1.4.tar.gz` & `tmp/edc-document-status-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-document-status-0.1.4.tar", last modified: Wed May 24 16:44:05 2023, max compression
+gzip compressed data, was "edc-document-status-0.1.5.tar", last modified: Tue Aug  1 04:19:48 2023, max compression
```

## Comparing `edc-document-status-0.1.4.tar` & `edc-document-status-0.1.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:05.220845 edc-document-status-0.1.4/
--rw-r--r--   0 erikvw     (501) staff       (20)      145 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:05.214041 edc-document-status-0.1.4/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:05.217356 edc-document-status-0.1.4/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 16:43:56.000000 edc-document-status-0.1.4/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1844 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 16:43:56.000000 edc-document-status-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-09 18:44:34.000000 edc-document-status-0.1.4/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-05-19 19:51:05.000000 edc-document-status-0.1.4/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1592 2023-05-24 16:44:05.220937 edc-document-status-0.1.4/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      711 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-09 18:44:34.000000 edc-document-status-0.1.4/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:05.218437 edc-document-status-0.1.4/edc_document_status/
--rw-r--r--   0 erikvw     (501) staff       (20)       85 2022-10-26 02:33:20.000000 edc-document-status-0.1.4/edc_document_status/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      241 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      196 2022-08-09 18:44:34.000000 edc-document-status-0.1.4/edc_document_status/fieldsets.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1365 2023-05-24 16:43:56.000000 edc-document-status-0.1.4/edc_document_status/model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      275 2022-08-09 18:44:34.000000 edc-document-status-0.1.4/edc_document_status/modeladmin_mixins.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:05.219396 edc-document-status-0.1.4/edc_document_status/models/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1318 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/models/signals.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:05.219537 edc-document-status-0.1.4/edc_document_status/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:05.220619 edc-document-status-0.1.4/edc_document_status/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/tests/etc/user-salt-restricted.key
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:05.220757 edc-document-status-0.1.4/edc_document_status/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      213 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/edc_document_status/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:05.219183 edc-document-status-0.1.4/edc_document_status.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1592 2023-05-24 16:44:05.000000 edc-document-status-0.1.4/edc_document_status.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1209 2023-05-24 16:44:05.000000 edc-document-status-0.1.4/edc_document_status.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-24 16:44:05.000000 edc-document-status-0.1.4/edc_document_status.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-19 20:39:30.000000 edc-document-status-0.1.4/edc_document_status.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       20 2023-05-24 16:44:05.000000 edc-document-status-0.1.4/edc_document_status.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1784 2023-05-24 16:43:56.000000 edc-document-status-0.1.4/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2225 2022-05-25 03:00:32.000000 edc-document-status-0.1.4/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1186 2023-05-24 16:44:05.221222 edc-document-status-0.1.4/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:19:48.179933 edc-document-status-0.1.5/
+-rw-r--r--   0 erikvw     (501) staff       (20)      145 2022-05-25 03:00:32.000000 edc-document-status-0.1.5/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-25 03:00:32.000000 edc-document-status-0.1.5/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:19:48.173036 edc-document-status-0.1.5/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:19:48.176499 edc-document-status-0.1.5/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 16:43:56.000000 edc-document-status-0.1.5/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1844 2022-05-25 03:00:32.000000 edc-document-status-0.1.5/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 16:43:56.000000 edc-document-status-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-09 18:44:34.000000 edc-document-status-0.1.5/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 03:00:32.000000 edc-document-status-0.1.5/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 03:00:32.000000 edc-document-status-0.1.5/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-05-19 19:51:05.000000 edc-document-status-0.1.5/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-25 03:00:32.000000 edc-document-status-0.1.5/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1592 2023-08-01 04:19:48.180038 edc-document-status-0.1.5/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      711 2022-05-25 03:00:32.000000 edc-document-status-0.1.5/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-09 18:44:34.000000 edc-document-status-0.1.5/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:19:48.177619 edc-document-status-0.1.5/edc_document_status/
+-rw-r--r--   0 erikvw     (501) staff       (20)       85 2022-10-26 02:33:20.000000 edc-document-status-0.1.5/edc_document_status/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      241 2022-05-25 03:00:32.000000 edc-document-status-0.1.5/edc_document_status/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      196 2022-08-09 18:44:34.000000 edc-document-status-0.1.5/edc_document_status/fieldsets.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1365 2023-05-24 16:43:56.000000 edc-document-status-0.1.5/edc_document_status/model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      275 2022-08-09 18:44:34.000000 edc-document-status-0.1.5/edc_document_status/modeladmin_mixins.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:19:48.178490 edc-document-status-0.1.5/edc_document_status/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 03:00:32.000000 edc-document-status-0.1.5/edc_document_status/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1318 2022-05-25 03:00:32.000000 edc-document-status-0.1.5/edc_document_status/models/signals.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:19:48.178620 edc-document-status-0.1.5/edc_document_status/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 03:00:32.000000 edc-document-status-0.1.5/edc_document_status/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:19:48.179719 edc-document-status-0.1.5/edc_document_status/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 03:00:32.000000 edc-document-status-0.1.5/edc_document_status/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 03:00:32.000000 edc-document-status-0.1.5/edc_document_status/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-25 03:00:32.000000 edc-document-status-0.1.5/edc_document_status/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-25 03:00:32.000000 edc-document-status-0.1.5/edc_document_status/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-25 03:00:32.000000 edc-document-status-0.1.5/edc_document_status/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-25 03:00:32.000000 edc-document-status-0.1.5/edc_document_status/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 03:00:32.000000 edc-document-status-0.1.5/edc_document_status/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 03:00:32.000000 edc-document-status-0.1.5/edc_document_status/tests/etc/user-salt-restricted.key
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:19:48.179846 edc-document-status-0.1.5/edc_document_status/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 03:00:32.000000 edc-document-status-0.1.5/edc_document_status/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      213 2022-05-25 03:00:32.000000 edc-document-status-0.1.5/edc_document_status/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:19:48.178290 edc-document-status-0.1.5/edc_document_status.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1592 2023-08-01 04:19:48.000000 edc-document-status-0.1.5/edc_document_status.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1209 2023-08-01 04:19:48.000000 edc-document-status-0.1.5/edc_document_status.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-08-01 04:19:48.000000 edc-document-status-0.1.5/edc_document_status.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-19 20:39:30.000000 edc-document-status-0.1.5/edc_document_status.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       20 2023-08-01 04:19:48.000000 edc-document-status-0.1.5/edc_document_status.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1784 2023-05-24 16:43:56.000000 edc-document-status-0.1.5/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2225 2023-08-01 04:19:41.000000 edc-document-status-0.1.5/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1186 2023-08-01 04:19:48.180342 edc-document-status-0.1.5/setup.cfg
```

### Comparing `edc-document-status-0.1.4/.github/workflows/build.yml` & `edc-document-status-0.1.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-document-status-0.1.4/.gitignore` & `edc-document-status-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-document-status-0.1.4/.pre-commit-config.yaml` & `edc-document-status-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-document-status-0.1.4/LICENSE` & `edc-document-status-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-document-status-0.1.4/PKG-INFO` & `edc-document-status-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-document-status
-Version: 0.1.4
+Version: 0.1.5
 Summary: Base classes for CRFs in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-document-status
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc case report forms,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-document-status-0.1.4/README.rst` & `edc-document-status-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `edc-document-status-0.1.4/edc_document_status/model_mixins.py` & `edc-document-status-0.1.5/edc_document_status/model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-document-status-0.1.4/edc_document_status/models/signals.py` & `edc-document-status-0.1.5/edc_document_status/models/signals.py`

 * *Files identical despite different names*

### Comparing `edc-document-status-0.1.4/edc_document_status/tests/etc/user-rsa-local-private.pem` & `edc-document-status-0.1.5/edc_document_status/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-document-status-0.1.4/edc_document_status/tests/etc/user-rsa-restricted-private.pem` & `edc-document-status-0.1.5/edc_document_status/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-document-status-0.1.4/edc_document_status.egg-info/PKG-INFO` & `edc-document-status-0.1.5/edc_document_status.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-document-status
-Version: 0.1.4
+Version: 0.1.5
 Summary: Base classes for CRFs in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-document-status
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc case report forms,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-document-status-0.1.4/edc_document_status.egg-info/SOURCES.txt` & `edc-document-status-0.1.5/edc_document_status.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-document-status-0.1.4/pyproject.toml` & `edc-document-status-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-document-status-0.1.4/runtests.py` & `edc-document-status-0.1.5/runtests.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 base_dir = dirname(abspath(__file__))
 
 DEFAULT_SETTINGS = DefaultTestSettings(
     calling_file=__file__,
     BASE_DIR=base_dir,
     APP_NAME=app_name,
     ETC_DIR=os.path.join(base_dir, app_name, "tests", "etc"),
-    SUBJECT_VISIT_MODEL="visit_schedule_app.subjectvisit",
+    SUBJECT_VISIT_MODEL="edc_visit_tracking.subjectvisit",
     INSTALLED_APPS=[
         "django.contrib.admin",
         "django.contrib.auth",
         "django.contrib.contenttypes",
         "django.contrib.messages",
         "django.contrib.sessions",
         "django.contrib.sites",
```

### Comparing `edc-document-status-0.1.4/setup.cfg` & `edc-document-status-0.1.5/setup.cfg`

 * *Files identical despite different names*

