# Comparing `tmp/open_source_sdk-0.0.2.tar.gz` & `tmp/open_source_sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_source_sdk-0.0.2.tar", last modified: Mon Jul 31 11:38:42 2023, max compression
+gzip compressed data, was "open_source_sdk-0.0.3.tar", last modified: Tue Aug  1 12:55:55 2023, max compression
```

## Comparing `open_source_sdk-0.0.2.tar` & `open_source_sdk-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:38:42.125261 open_source_sdk-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-31 11:38:42.125261 open_source_sdk-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:38:42.125261 open_source_sdk-0.0.2/open_source_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/open_source_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/open_source_sdk/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/open_source_sdk/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:38:42.125261 open_source_sdk-0.0.2/open_source_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-31 11:38:42.000000 open_source_sdk-0.0.2/open_source_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-31 11:38:42.000000 open_source_sdk-0.0.2/open_source_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 11:38:42.000000 open_source_sdk-0.0.2/open_source_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-31 11:38:42.000000 open_source_sdk-0.0.2/open_source_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 11:38:42.000000 open_source_sdk-0.0.2/open_source_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/requirements_plot.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 11:38:42.125261 open_source_sdk-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:38:42.125261 open_source_sdk-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/tests/test_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:55.249081 open_source_sdk-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-08-01 12:55:29.000000 open_source_sdk-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-01 12:55:55.249081 open_source_sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-01 12:55:29.000000 open_source_sdk-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:55.245081 open_source_sdk-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-01 12:55:29.000000 open_source_sdk-0.0.3/docs/requirements_docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:55.245081 open_source_sdk-0.0.3/open_source_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:29.000000 open_source_sdk-0.0.3/open_source_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-01 12:55:29.000000 open_source_sdk-0.0.3/open_source_sdk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 12:55:29.000000 open_source_sdk-0.0.3/open_source_sdk/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:55.245081 open_source_sdk-0.0.3/open_source_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-01 12:55:55.000000 open_source_sdk-0.0.3/open_source_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-01 12:55:55.000000 open_source_sdk-0.0.3/open_source_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:55:55.000000 open_source_sdk-0.0.3/open_source_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-01 12:55:55.000000 open_source_sdk-0.0.3/open_source_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 12:55:55.000000 open_source_sdk-0.0.3/open_source_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-08-01 12:55:29.000000 open_source_sdk-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:29.000000 open_source_sdk-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:29.000000 open_source_sdk-0.0.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 12:55:29.000000 open_source_sdk-0.0.3/requirements_plot.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-01 12:55:29.000000 open_source_sdk-0.0.3/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 12:55:55.249081 open_source_sdk-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:55.249081 open_source_sdk-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-01 12:55:29.000000 open_source_sdk-0.0.3/tests/test_demo.py
```

### Comparing `open_source_sdk-0.0.2/LICENSE` & `open_source_sdk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `open_source_sdk-0.0.2/pyproject.toml` & `open_source_sdk-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 readme = {file = "README.md", content-type = "text/markdown"}
 dependencies = {file = "requirements.txt"}
 
 [tool.setuptools.dynamic.optional-dependencies]
 plot = {file = "requirements_plot.txt"}
 test = {file = "requirements_test.txt"}
 dev = {file = "requirements_dev.txt"}
+docs = {file = "docs/requirements_docs.txt"}
 
 [project.urls]
 homepage = "https://github.com/opencivilengineering"
 documentation = "http://opencivilengineering.readthedocs.io"
 
 [tool.setuptools]
 packages = [
```

