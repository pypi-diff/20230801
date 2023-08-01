# Comparing `tmp/aiooss2-0.2.6.tar.gz` & `tmp/aiooss2-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiooss2-0.2.6.tar", last modified: Mon Jun 12 11:05:06 2023, max compression
+gzip compressed data, was "aiooss2-0.2.7.tar", last modified: Tue Aug  1 15:20:04 2023, max compression
```

## Comparing `aiooss2-0.2.6.tar` & `aiooss2-0.2.7.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.028393 aiooss2-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-12 11:04:42.000000 aiooss2-0.2.6/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 11:04:42.000000 aiooss2-0.2.6/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.020393 aiooss2-0.2.6/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-12 11:04:42.000000 aiooss2-0.2.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.024393 aiooss2-0.2.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-12 11:04:42.000000 aiooss2-0.2.6/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-12 11:04:42.000000 aiooss2-0.2.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-12 11:04:42.000000 aiooss2-0.2.6/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-12 11:04:42.000000 aiooss2-0.2.6/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-12 11:04:42.000000 aiooss2-0.2.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-12 11:04:42.000000 aiooss2-0.2.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-12 11:04:42.000000 aiooss2-0.2.6/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-12 11:04:42.000000 aiooss2-0.2.6/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-12 11:04:42.000000 aiooss2-0.2.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-12 11:04:42.000000 aiooss2-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-12 11:04:42.000000 aiooss2-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-12 11:05:06.028393 aiooss2-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-12 11:04:42.000000 aiooss2-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-12 11:04:42.000000 aiooss2-0.2.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.024393 aiooss2-0.2.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.024393 aiooss2-0.2.6/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-12 11:04:42.000000 aiooss2-0.2.6/docs/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-12 11:04:42.000000 aiooss2-0.2.6/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-12 11:04:42.000000 aiooss2-0.2.6/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.024393 aiooss2-0.2.6/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-12 11:04:42.000000 aiooss2-0.2.6/examples/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-12 11:04:42.000000 aiooss2-0.2.6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-12 11:04:42.000000 aiooss2-0.2.6/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-12 11:04:42.000000 aiooss2-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-12 11:05:06.028393 aiooss2-0.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.020393 aiooss2-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.024393 aiooss2-0.2.6/src/aiooss2/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29416 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/multipart.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19767 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/resumable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.024393 aiooss2-0.2.6/src/aiooss2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-12 11:05:05.000000 aiooss2-0.2.6/src/aiooss2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-12 11:05:06.000000 aiooss2-0.2.6/src/aiooss2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 11:05:05.000000 aiooss2-0.2.6/src/aiooss2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 11:05:05.000000 aiooss2-0.2.6/src/aiooss2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-12 11:05:05.000000 aiooss2-0.2.6/src/aiooss2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 11:05:05.000000 aiooss2-0.2.6/src/aiooss2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.024393 aiooss2-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-12 11:04:42.000000 aiooss2-0.2.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-12 11:04:42.000000 aiooss2-0.2.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.028393 aiooss2-0.2.6/tests/func/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 11:04:42.000000 aiooss2-0.2.6/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-12 11:04:42.000000 aiooss2-0.2.6/tests/func/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-06-12 11:04:42.000000 aiooss2-0.2.6/tests/func/test_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-12 11:04:42.000000 aiooss2-0.2.6/tests/func/test_resumable.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-12 11:04:42.000000 aiooss2-0.2.6/tests/test_aiooss2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.028393 aiooss2-0.2.6/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 11:04:42.000000 aiooss2-0.2.6/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-12 11:04:42.000000 aiooss2-0.2.6/tests/unit/test_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:20:04.229576 aiooss2-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-08-01 15:19:35.000000 aiooss2-0.2.7/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 15:19:35.000000 aiooss2-0.2.7/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:20:04.225576 aiooss2-0.2.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-01 15:19:35.000000 aiooss2-0.2.7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:20:04.225576 aiooss2-0.2.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-01 15:19:35.000000 aiooss2-0.2.7/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-08-01 15:19:35.000000 aiooss2-0.2.7/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-01 15:19:35.000000 aiooss2-0.2.7/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-08-01 15:19:35.000000 aiooss2-0.2.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-08-01 15:19:35.000000 aiooss2-0.2.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-01 15:19:35.000000 aiooss2-0.2.7/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-08-01 15:19:35.000000 aiooss2-0.2.7/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-01 15:19:35.000000 aiooss2-0.2.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-08-01 15:19:35.000000 aiooss2-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-01 15:19:35.000000 aiooss2-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-08-01 15:20:04.229576 aiooss2-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-08-01 15:19:35.000000 aiooss2-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-01 15:19:35.000000 aiooss2-0.2.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:20:04.225576 aiooss2-0.2.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:20:04.225576 aiooss2-0.2.7/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-08-01 15:19:35.000000 aiooss2-0.2.7/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-01 15:19:35.000000 aiooss2-0.2.7/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 15:19:35.000000 aiooss2-0.2.7/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:20:04.225576 aiooss2-0.2.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-08-01 15:19:35.000000 aiooss2-0.2.7/examples/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-01 15:19:35.000000 aiooss2-0.2.7/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-08-01 15:19:35.000000 aiooss2-0.2.7/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-08-01 15:19:35.000000 aiooss2-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-01 15:20:04.229576 aiooss2-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:20:04.221576 aiooss2-0.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:20:04.225576 aiooss2-0.2.7/src/aiooss2/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-01 15:19:35.000000 aiooss2-0.2.7/src/aiooss2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-08-01 15:19:35.000000 aiooss2-0.2.7/src/aiooss2/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29416 2023-08-01 15:19:35.000000 aiooss2-0.2.7/src/aiooss2/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-01 15:19:35.000000 aiooss2-0.2.7/src/aiooss2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-08-01 15:19:35.000000 aiooss2-0.2.7/src/aiooss2/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-08-01 15:19:35.000000 aiooss2-0.2.7/src/aiooss2/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-08-01 15:19:35.000000 aiooss2-0.2.7/src/aiooss2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-08-01 15:19:35.000000 aiooss2-0.2.7/src/aiooss2/multipart.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:19:35.000000 aiooss2-0.2.7/src/aiooss2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19767 2023-08-01 15:19:35.000000 aiooss2-0.2.7/src/aiooss2/resumable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-08-01 15:19:35.000000 aiooss2-0.2.7/src/aiooss2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:20:04.229576 aiooss2-0.2.7/src/aiooss2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-08-01 15:20:04.000000 aiooss2-0.2.7/src/aiooss2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 15:20:04.000000 aiooss2-0.2.7/src/aiooss2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:20:04.000000 aiooss2-0.2.7/src/aiooss2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:20:03.000000 aiooss2-0.2.7/src/aiooss2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-01 15:20:04.000000 aiooss2-0.2.7/src/aiooss2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 15:20:04.000000 aiooss2-0.2.7/src/aiooss2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:20:04.229576 aiooss2-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-01 15:19:35.000000 aiooss2-0.2.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-08-01 15:19:35.000000 aiooss2-0.2.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:20:04.229576 aiooss2-0.2.7/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:19:35.000000 aiooss2-0.2.7/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-01 15:19:35.000000 aiooss2-0.2.7/tests/func/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-08-01 15:19:35.000000 aiooss2-0.2.7/tests/func/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-08-01 15:19:35.000000 aiooss2-0.2.7/tests/func/test_resumable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-01 15:19:35.000000 aiooss2-0.2.7/tests/test_aiooss2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:20:04.229576 aiooss2-0.2.7/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:19:35.000000 aiooss2-0.2.7/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-08-01 15:19:35.000000 aiooss2-0.2.7/tests/unit/test_adapter.py
```

### Comparing `aiooss2-0.2.6/.cruft.json` & `aiooss2-0.2.7/.cruft.json`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/.github/dependabot.yml` & `aiooss2-0.2.7/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/.github/workflows/release.yml` & `aiooss2-0.2.7/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/.github/workflows/tests.yml` & `aiooss2-0.2.7/.github/workflows/tests.yml`

 * *Files 12% similar despite different names*

```diff
@@ -55,10 +55,7 @@
       run: nox -s tests-${{ matrix.nox_pyv || matrix.pyv }} -- --cov-report=xml
 
     - name: Upload coverage report
       uses: codecov/codecov-action@v3.1.1
 
     - name: Build package
       run: nox -s build
-
-    - name: Build docs
-      run: nox -s docs
```

### Comparing `aiooss2-0.2.6/.gitignore` & `aiooss2-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/.pre-commit-config.yaml` & `aiooss2-0.2.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/CODE_OF_CONDUCT.rst` & `aiooss2-0.2.7/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/CONTRIBUTING.rst` & `aiooss2-0.2.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/LICENSE` & `aiooss2-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/PKG-INFO` & `aiooss2-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: aiooss2
-Version: 0.2.6
+Version: 0.2.7
 Summary: Async client for aliyun OSS(Object Storage Service) using oss2 and aiohttp/asyncio
 Home-page: https://github.com/karajan1001/aiooss2
 Maintainer-email: mishanyo1001@gmail.com
 License: Apache-2.0
 Keywords: "oss,aio"
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: dev
 License-File: LICENSE
 
 Aiooss2
 --------
```

### Comparing `aiooss2-0.2.6/README.md` & `aiooss2-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/README.rst` & `aiooss2-0.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/docs/assets/logo.svg` & `aiooss2-0.2.7/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/docs/gen_ref_pages.py` & `aiooss2-0.2.7/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/examples/simple.py` & `aiooss2-0.2.7/examples/simple.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/mkdocs.yml` & `aiooss2-0.2.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/noxfile.py` & `aiooss2-0.2.7/noxfile.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,20 +5,14 @@
 import nox
 
 nox.options.reuse_existing_virtualenvs = True
 nox.options.sessions = "lint", "tests"
 locations = "src", "tests"
 
 
-@nox.session
-def docs(session: nox.Session) -> None:
-    session.install(".[docs]")
-    session.run("mkdocs", "build")
-
-
 @nox.session(python=["3.8", "3.9", "3.10", "3.11", "pypy3.8", "pypy3.9"])
 def tests(session: nox.Session) -> None:
     session.install(".[tests]")
     session.run(
         "pytest",
         "--cov",
         "--cov-config=pyproject.toml",
```

### Comparing `aiooss2-0.2.6/pyproject.toml` & `aiooss2-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/setup.cfg` & `aiooss2-0.2.7/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -22,35 +22,28 @@
 python_requires = >=3.8
 zip_safe = False
 packages = find:
 package_dir = 
 	=src
 include_package_data = True
 install_requires = 
-	aiohttp==3.8.4
-	oss2==2.18.0
+	aiohttp==3.8.5
+	oss2==2.18.1
 
 [options.extras_require]
-docs = 
-	mkdocs==1.3.1
-	mkdocs-gen-files==0.3.5
-	mkdocs-material==8.4.1
-	mkdocs-section-index==0.3.4
-	mkdocstrings-python==0.7.1
 tests = 
 	pytest==7.2.0
 	pytest-sugar==0.9.5
 	pytest-cov==3.0.0
 	pytest-mock==3.8.2
 	pylint==2.15.0
 	pylint-pytest==1.1.2
 	mypy==0.971
 dev = 
 	%(tests)s
-	%(docs)s
 	nox==2023.4.22
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
 where = src
```

### Comparing `aiooss2-0.2.6/src/aiooss2/adapter.py` & `aiooss2-0.2.7/src/aiooss2/adapter.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/src/aiooss2/api.py` & `aiooss2-0.2.7/src/aiooss2/api.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/src/aiooss2/exceptions.py` & `aiooss2-0.2.7/src/aiooss2/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/src/aiooss2/http.py` & `aiooss2-0.2.7/src/aiooss2/http.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/src/aiooss2/iterators.py` & `aiooss2-0.2.7/src/aiooss2/iterators.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/src/aiooss2/models.py` & `aiooss2-0.2.7/src/aiooss2/models.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/src/aiooss2/multipart.py` & `aiooss2-0.2.7/src/aiooss2/multipart.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/src/aiooss2/resumable.py` & `aiooss2-0.2.7/src/aiooss2/resumable.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/src/aiooss2/utils.py` & `aiooss2-0.2.7/src/aiooss2/utils.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/src/aiooss2.egg-info/PKG-INFO` & `aiooss2-0.2.7/src/aiooss2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: aiooss2
-Version: 0.2.6
+Version: 0.2.7
 Summary: Async client for aliyun OSS(Object Storage Service) using oss2 and aiohttp/asyncio
 Home-page: https://github.com/karajan1001/aiooss2
 Maintainer-email: mishanyo1001@gmail.com
 License: Apache-2.0
 Keywords: "oss,aio"
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: dev
 License-File: LICENSE
 
 Aiooss2
 --------
```

### Comparing `aiooss2-0.2.6/src/aiooss2.egg-info/SOURCES.txt` & `aiooss2-0.2.7/src/aiooss2.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 README.md
 README.rst
 mkdocs.yml
 noxfile.py
 pyproject.toml
 setup.cfg
 .github/dependabot.yml
-.github/workflows/docs.yml
 .github/workflows/release.yml
 .github/workflows/tests.yml
 .github/workflows/update-template.yaml
 docs/gen_ref_pages.py
 docs/index.md
 docs/assets/logo.svg
 examples/simple.py
```

### Comparing `aiooss2-0.2.6/tests/conftest.py` & `aiooss2-0.2.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/tests/func/test_bucket.py` & `aiooss2-0.2.7/tests/func/test_bucket.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/tests/func/test_object.py` & `aiooss2-0.2.7/tests/func/test_object.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/tests/func/test_resumable.py` & `aiooss2-0.2.7/tests/func/test_resumable.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.6/tests/unit/test_adapter.py` & `aiooss2-0.2.7/tests/unit/test_adapter.py`

 * *Files identical despite different names*

