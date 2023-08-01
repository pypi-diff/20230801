# Comparing `tmp/bioio-base-0.1.1.tar.gz` & `tmp/bioio-base-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioio-base-0.1.1.tar", last modified: Mon Jul  3 20:27:52 2023, max compression
+gzip compressed data, was "bioio-base-0.2.0.tar", last modified: Tue Aug  1 14:45:07 2023, max compression
```

## Comparing `bioio-base-0.1.1.tar` & `bioio-base-0.2.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:27:52.315457 bioio-base-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-03 20:27:32.000000 bioio-base-0.1.1/.cookiecutter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-03 20:27:32.000000 bioio-base-0.1.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:27:52.307457 bioio-base-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:27:52.307457 bioio-base-0.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-03 20:27:32.000000 bioio-base-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-03 20:27:32.000000 bioio-base-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-03 20:27:32.000000 bioio-base-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-03 20:27:32.000000 bioio-base-0.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:27:52.307457 bioio-base-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-03 20:27:32.000000 bioio-base-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-03 20:27:32.000000 bioio-base-0.1.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-03 20:27:32.000000 bioio-base-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-03 20:27:32.000000 bioio-base-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-07-03 20:27:32.000000 bioio-base-0.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-03 20:27:32.000000 bioio-base-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-03 20:27:32.000000 bioio-base-0.1.1/Justfile
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-03 20:27:32.000000 bioio-base-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-03 20:27:52.315457 bioio-base-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-03 20:27:32.000000 bioio-base-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:27:52.311457 bioio-base-0.1.1/bioio_base/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-03 20:27:32.000000 bioio-base-0.1.1/bioio_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-03 20:27:32.000000 bioio-base-0.1.1/bioio_base/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-07-03 20:27:32.000000 bioio-base-0.1.1/bioio_base/dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-03 20:27:32.000000 bioio-base-0.1.1/bioio_base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-03 20:27:32.000000 bioio-base-0.1.1/bioio_base/image_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-03 20:27:32.000000 bioio-base-0.1.1/bioio_base/io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:27:32.000000 bioio-base-0.1.1/bioio_base/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29812 2023-07-03 20:27:32.000000 bioio-base-0.1.1/bioio_base/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-03 20:27:32.000000 bioio-base-0.1.1/bioio_base/reader_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-07-03 20:27:32.000000 bioio-base-0.1.1/bioio_base/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:27:52.311457 bioio-base-0.1.1/bioio_base/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-03 20:27:32.000000 bioio-base-0.1.1/bioio_base/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-03 20:27:32.000000 bioio-base-0.1.1/bioio_base/tests/test_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-07-03 20:27:32.000000 bioio-base-0.1.1/bioio_base/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-03 20:27:32.000000 bioio-base-0.1.1/bioio_base/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:27:52.311457 bioio-base-0.1.1/bioio_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-03 20:27:52.000000 bioio-base-0.1.1/bioio_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-03 20:27:52.000000 bioio-base-0.1.1/bioio_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:27:52.000000 bioio-base-0.1.1/bioio_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:27:51.000000 bioio-base-0.1.1/bioio_base.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-03 20:27:52.000000 bioio-base-0.1.1/bioio_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 20:27:52.000000 bioio-base-0.1.1/bioio_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:27:52.315457 bioio-base-0.1.1/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5377 2023-07-03 20:27:32.000000 bioio-base-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-03 20:27:32.000000 bioio-base-0.1.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-03 20:27:32.000000 bioio-base-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-03 20:27:32.000000 bioio-base-0.1.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-03 20:27:32.000000 bioio-base-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 20:27:52.315457 bioio-base-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:45:07.369191 bioio-base-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-08-01 14:44:51.000000 bioio-base-0.2.0/.cookiecutter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-01 14:44:51.000000 bioio-base-0.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:45:07.361191 bioio-base-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:45:07.361191 bioio-base-0.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 14:44:51.000000 bioio-base-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-01 14:44:51.000000 bioio-base-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-01 14:44:51.000000 bioio-base-0.2.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-01 14:44:51.000000 bioio-base-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:45:07.365191 bioio-base-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-08-01 14:44:51.000000 bioio-base-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-01 14:44:51.000000 bioio-base-0.2.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-01 14:44:51.000000 bioio-base-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-01 14:44:51.000000 bioio-base-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-08-01 14:44:51.000000 bioio-base-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-08-01 14:44:51.000000 bioio-base-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-08-01 14:44:51.000000 bioio-base-0.2.0/Justfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-01 14:44:51.000000 bioio-base-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-01 14:45:07.369191 bioio-base-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-01 14:44:51.000000 bioio-base-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:45:07.365191 bioio-base-0.2.0/bioio_base/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/image_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29812 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/reader_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:45:07.369191 bioio-base-0.2.0/bioio_base/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/tests/test_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:45:07.365191 bioio-base-0.2.0/bioio_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-01 14:45:07.000000 bioio-base-0.2.0/bioio_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-01 14:45:07.000000 bioio-base-0.2.0/bioio_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:45:07.000000 bioio-base-0.2.0/bioio_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:45:07.000000 bioio-base-0.2.0/bioio_base.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-01 14:45:07.000000 bioio-base-0.2.0/bioio_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 14:45:07.000000 bioio-base-0.2.0/bioio_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:45:07.369191 bioio-base-0.2.0/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5377 2023-08-01 14:44:51.000000 bioio-base-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 14:44:51.000000 bioio-base-0.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-01 14:44:51.000000 bioio-base-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-01 14:44:51.000000 bioio-base-0.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-08-01 14:44:51.000000 bioio-base-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:45:07.369191 bioio-base-0.2.0/setup.cfg
```

### Comparing `bioio-base-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `bioio-base-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md` & `bioio-base-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/.github/PULL_REQUEST_TEMPLATE.md` & `bioio-base-0.2.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/.github/workflows/ci.yml` & `bioio-base-0.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/.github/workflows/docs.yml` & `bioio-base-0.2.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/.gitignore` & `bioio-base-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/.pre-commit-config.yaml` & `bioio-base-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/CODE_OF_CONDUCT.md` & `bioio-base-0.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/CONTRIBUTING.md` & `bioio-base-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/Justfile` & `bioio-base-0.2.0/Justfile`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/LICENSE` & `bioio-base-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/PKG-INFO` & `bioio-base-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioio-base
-Version: 0.1.1
+Version: 0.2.0
 Summary: Typing, base classes, and more for BioIO projects.
 Author-email: Eva Maxfield Brown <evamaxfieldbrown@gmail.com>, Dan Toloudis <danielt@alleninstitute.org>
 License: BSD License
 Project-URL: Homepage, https://github.com/bioio-devs/bioio-base
 Project-URL: Bug Tracker, https://github.com/bioio-devs/bioio-base/issues
 Project-URL: Documentation, https://bioio-devs.github.io/bioio-base
 Project-URL: User Support, https://github.com/bioio-devs/bioio-base/issues
```

### Comparing `bioio-base-0.1.1/README.md` & `bioio-base-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/bioio_base/dimensions.py` & `bioio-base-0.2.0/bioio_base/dimensions.py`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/bioio_base/exceptions.py` & `bioio-base-0.2.0/bioio_base/exceptions.py`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/bioio_base/image_container.py` & `bioio-base-0.2.0/bioio_base/image_container.py`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/bioio_base/io.py` & `bioio-base-0.2.0/bioio_base/io.py`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/bioio_base/reader.py` & `bioio-base-0.2.0/bioio_base/reader.py`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/bioio_base/test_utilities.py` & `bioio-base-0.2.0/bioio_base/test_utilities.py`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/bioio_base/tests/conftest.py` & `bioio-base-0.2.0/bioio_base/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/bioio_base/transforms.py` & `bioio-base-0.2.0/bioio_base/transforms.py`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/bioio_base/types.py` & `bioio-base-0.2.0/bioio_base/types.py`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/bioio_base.egg-info/PKG-INFO` & `bioio-base-0.2.0/bioio_base.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioio-base
-Version: 0.1.1
+Version: 0.2.0
 Summary: Typing, base classes, and more for BioIO projects.
 Author-email: Eva Maxfield Brown <evamaxfieldbrown@gmail.com>, Dan Toloudis <danielt@alleninstitute.org>
 License: BSD License
 Project-URL: Homepage, https://github.com/bioio-devs/bioio-base
 Project-URL: Bug Tracker, https://github.com/bioio-devs/bioio-base/issues
 Project-URL: Documentation, https://bioio-devs.github.io/bioio-base
 Project-URL: User Support, https://github.com/bioio-devs/bioio-base/issues
```

### Comparing `bioio-base-0.1.1/bioio_base.egg-info/SOURCES.txt` & `bioio-base-0.2.0/bioio_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/docs/conf.py` & `bioio-base-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/docs/installation.rst` & `bioio-base-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `bioio-base-0.1.1/pyproject.toml` & `bioio-base-0.2.0/pyproject.toml`

 * *Files identical despite different names*

