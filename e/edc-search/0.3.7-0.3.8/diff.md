# Comparing `tmp/edc-search-0.3.7.tar.gz` & `tmp/edc-search-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-search-0.3.7.tar", last modified: Wed May 24 16:44:33 2023, max compression
+gzip compressed data, was "edc-search-0.3.8.tar", last modified: Tue Aug  1 05:31:13 2023, max compression
```

## Comparing `edc-search-0.3.7.tar` & `edc-search-0.3.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:33.305156 edc-search-0.3.7/
--rw-r--r--   0 erikvw     (501) staff       (20)       90 2021-02-07 13:19:55.000000 edc-search-0.3.7/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-06 15:47:52.000000 edc-search-0.3.7/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:33.298562 edc-search-0.3.7/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:33.301936 edc-search-0.3.7/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 16:44:25.000000 edc-search-0.3.7/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1119 2022-06-01 23:57:05.000000 edc-search-0.3.7/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 16:44:25.000000 edc-search-0.3.7/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      127 2022-06-01 23:57:05.000000 edc-search-0.3.7/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       81 2022-06-01 23:57:05.000000 edc-search-0.3.7/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-03-04 23:12:34.000000 edc-search-0.3.7/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 23:57:05.000000 edc-search-0.3.7/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     2853 2023-05-24 16:44:33.305246 edc-search-0.3.7/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1991 2021-02-06 16:35:53.000000 edc-search-0.3.7/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-25 22:22:08.000000 edc-search-0.3.7/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2021-02-06 15:47:52.000000 edc-search-0.3.7/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:33.302991 edc-search-0.3.7/edc_search/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:12:34.000000 edc-search-0.3.7/edc_search/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      113 2020-03-04 23:12:34.000000 edc-search-0.3.7/edc_search/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1282 2023-05-24 16:44:25.000000 edc-search-0.3.7/edc_search/model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 23:57:05.000000 edc-search-0.3.7/edc_search/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)      812 2021-02-06 15:47:52.000000 edc-search-0.3.7/edc_search/search_slug.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:33.303767 edc-search-0.3.7/edc_search/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:12:34.000000 edc-search-0.3.7/edc_search/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:33.304817 edc-search-0.3.7/edc_search/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-06 15:47:52.000000 edc-search-0.3.7/edc_search/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-06 15:47:52.000000 edc-search-0.3.7/edc_search/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-02-06 15:47:52.000000 edc-search-0.3.7/edc_search/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-02-06 15:47:52.000000 edc-search-0.3.7/edc_search/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-02-06 15:47:52.000000 edc-search-0.3.7/edc_search/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-02-06 15:47:52.000000 edc-search-0.3.7/edc_search/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-06 15:47:52.000000 edc-search-0.3.7/edc_search/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-06 15:47:52.000000 edc-search-0.3.7/edc_search/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1357 2023-05-24 16:44:25.000000 edc-search-0.3.7/edc_search/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:33.305035 edc-search-0.3.7/edc_search/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-06 15:47:52.000000 edc-search-0.3.7/edc_search/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2197 2022-06-01 23:57:05.000000 edc-search-0.3.7/edc_search/tests/tests/tests.py
--rw-r--r--   0 erikvw     (501) staff       (20)      582 2023-05-24 16:44:25.000000 edc-search-0.3.7/edc_search/updater.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-01 23:57:05.000000 edc-search-0.3.7/edc_search/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      171 2020-03-04 23:12:34.000000 edc-search-0.3.7/edc_search/wsgi.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:44:33.303580 edc-search-0.3.7/edc_search.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     2853 2023-05-24 16:44:33.000000 edc-search-0.3.7/edc_search.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1032 2023-05-24 16:44:33.000000 edc-search-0.3.7/edc_search.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-24 16:44:33.000000 edc-search-0.3.7/edc_search.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-06 20:43:35.000000 edc-search-0.3.7/edc_search.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       11 2023-05-24 16:44:33.000000 edc-search-0.3.7/edc_search.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1766 2023-05-24 16:44:25.000000 edc-search-0.3.7/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1620 2022-06-01 23:57:05.000000 edc-search-0.3.7/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1155 2023-05-24 16:44:33.305528 edc-search-0.3.7/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:31:13.288330 edc-search-0.3.8/
+-rw-r--r--   0 erikvw     (501) staff       (20)       90 2021-02-07 13:19:55.000000 edc-search-0.3.8/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-06 15:47:52.000000 edc-search-0.3.8/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:31:13.280576 edc-search-0.3.8/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:31:13.283875 edc-search-0.3.8/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 16:44:25.000000 edc-search-0.3.8/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1119 2022-06-01 23:57:05.000000 edc-search-0.3.8/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 16:44:25.000000 edc-search-0.3.8/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      127 2022-06-01 23:57:05.000000 edc-search-0.3.8/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       81 2022-06-01 23:57:05.000000 edc-search-0.3.8/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-03-04 23:12:34.000000 edc-search-0.3.8/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 23:57:05.000000 edc-search-0.3.8/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     2853 2023-08-01 05:31:13.288426 edc-search-0.3.8/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1991 2021-02-06 16:35:53.000000 edc-search-0.3.8/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-25 22:22:08.000000 edc-search-0.3.8/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2021-02-06 15:47:52.000000 edc-search-0.3.8/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:31:13.285462 edc-search-0.3.8/edc_search/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:12:34.000000 edc-search-0.3.8/edc_search/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      113 2020-03-04 23:12:34.000000 edc-search-0.3.8/edc_search/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1282 2023-05-24 16:44:25.000000 edc-search-0.3.8/edc_search/model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 23:57:05.000000 edc-search-0.3.8/edc_search/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      812 2021-02-06 15:47:52.000000 edc-search-0.3.8/edc_search/search_slug.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:31:13.286464 edc-search-0.3.8/edc_search/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:12:34.000000 edc-search-0.3.8/edc_search/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:31:13.287965 edc-search-0.3.8/edc_search/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-06 15:47:52.000000 edc-search-0.3.8/edc_search/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-06 15:47:52.000000 edc-search-0.3.8/edc_search/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-02-06 15:47:52.000000 edc-search-0.3.8/edc_search/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-02-06 15:47:52.000000 edc-search-0.3.8/edc_search/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-02-06 15:47:52.000000 edc-search-0.3.8/edc_search/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-02-06 15:47:52.000000 edc-search-0.3.8/edc_search/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-06 15:47:52.000000 edc-search-0.3.8/edc_search/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-06 15:47:52.000000 edc-search-0.3.8/edc_search/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1357 2023-05-24 16:44:25.000000 edc-search-0.3.8/edc_search/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:31:13.288210 edc-search-0.3.8/edc_search/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-06 15:47:52.000000 edc-search-0.3.8/edc_search/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2197 2022-06-01 23:57:05.000000 edc-search-0.3.8/edc_search/tests/tests/tests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      582 2023-05-24 16:44:25.000000 edc-search-0.3.8/edc_search/updater.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-01 23:57:05.000000 edc-search-0.3.8/edc_search/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      171 2020-03-04 23:12:34.000000 edc-search-0.3.8/edc_search/wsgi.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 05:31:13.286244 edc-search-0.3.8/edc_search.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2853 2023-08-01 05:31:13.000000 edc-search-0.3.8/edc_search.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1032 2023-08-01 05:31:13.000000 edc-search-0.3.8/edc_search.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-08-01 05:31:13.000000 edc-search-0.3.8/edc_search.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-06 20:43:35.000000 edc-search-0.3.8/edc_search.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       11 2023-08-01 05:31:13.000000 edc-search-0.3.8/edc_search.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1766 2023-05-24 16:44:25.000000 edc-search-0.3.8/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1626 2023-08-01 05:31:06.000000 edc-search-0.3.8/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1155 2023-08-01 05:31:13.288712 edc-search-0.3.8/setup.cfg
```

### Comparing `edc-search-0.3.7/.github/workflows/build.yml` & `edc-search-0.3.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.7/.gitignore` & `edc-search-0.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.7/.pre-commit-config.yaml` & `edc-search-0.3.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.7/LICENSE` & `edc-search-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.7/PKG-INFO` & `edc-search-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-search
-Version: 0.3.7
+Version: 0.3.8
 Summary: Simple edc-search forms and view mixins for the clinicedc/edc
 Home-page: https://github.com/clinicedc/edc-search
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc search,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-search-0.3.7/README.rst` & `edc-search-0.3.8/README.rst`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.7/edc_search/model_mixins.py` & `edc-search-0.3.8/edc_search/model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.7/edc_search/search_slug.py` & `edc-search-0.3.8/edc_search/search_slug.py`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.7/edc_search/tests/etc/user-rsa-local-private.pem` & `edc-search-0.3.8/edc_search/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.7/edc_search/tests/etc/user-rsa-restricted-private.pem` & `edc-search-0.3.8/edc_search/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.7/edc_search/tests/models.py` & `edc-search-0.3.8/edc_search/tests/models.py`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.7/edc_search/tests/tests/tests.py` & `edc-search-0.3.8/edc_search/tests/tests/tests.py`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.7/edc_search/updater.py` & `edc-search-0.3.8/edc_search/updater.py`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.7/edc_search.egg-info/PKG-INFO` & `edc-search-0.3.8/edc_search.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-search
-Version: 0.3.7
+Version: 0.3.8
 Summary: Simple edc-search forms and view mixins for the clinicedc/edc
 Home-page: https://github.com/clinicedc/edc-search
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc search,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-search-0.3.7/edc_search.egg-info/SOURCES.txt` & `edc-search-0.3.8/edc_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.7/pyproject.toml` & `edc-search-0.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-search-0.3.7/runtests.py` & `edc-search-0.3.8/runtests.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 DEFAULT_SETTINGS = DefaultTestSettings(
     calling_file=__file__,
     BASE_DIR=base_dir,
     APP_NAME=app_name,
     ETC_DIR=join(base_dir, app_name, "tests", "etc"),
     SUBJECT_SCREENING_MODEL="edc_metadata.subjectscreening",
     SUBJECT_CONSENT_MODEL="edc_metadata.subjectconsent",
-    SUBJECT_VISIT_MODEL="edc_metadata.subjectvisit",
+    SUBJECT_VISIT_MODEL="edc_visit_tracking.subjectvisit",
     SUBJECT_VISIT_MISSED_MODEL="edc_metadata.subjectvisitmissed",
     INSTALLED_APPS=[
         "django.contrib.admin",
         "django.contrib.auth",
         "django.contrib.contenttypes",
         "django.contrib.sessions",
         "django.contrib.messages",
```

### Comparing `edc-search-0.3.7/setup.cfg` & `edc-search-0.3.8/setup.cfg`

 * *Files identical despite different names*

