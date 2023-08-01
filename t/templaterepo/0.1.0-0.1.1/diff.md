# Comparing `tmp/templaterepo-0.1.0.tar.gz` & `tmp/templaterepo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templaterepo-0.1.0.tar", last modified: Tue Aug  1 20:36:11 2023, max compression
+gzip compressed data, was "templaterepo-0.1.1.tar", last modified: Tue Aug  1 20:41:18 2023, max compression
```

## Comparing `templaterepo-0.1.0.tar` & `templaterepo-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:11.102963 templaterepo-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-08-01 20:36:03.000000 templaterepo-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 20:36:03.000000 templaterepo-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-01 20:36:11.102963 templaterepo-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-01 20:36:03.000000 templaterepo-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-08-01 20:36:03.000000 templaterepo-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:36:11.102963 templaterepo-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-08-01 20:36:03.000000 templaterepo-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:11.098963 templaterepo-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:11.102963 templaterepo-0.1.0/src/templaterepo/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-01 20:36:11.102963 templaterepo-0.1.0/src/templaterepo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:11.102963 templaterepo-0.1.0/src/templaterepo/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-01 20:36:03.000000 templaterepo-0.1.0/src/templaterepo/_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:11.102963 templaterepo-0.1.0/src/templaterepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-01 20:36:11.000000 templaterepo-0.1.0/src/templaterepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-01 20:36:11.000000 templaterepo-0.1.0/src/templaterepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:36:11.000000 templaterepo-0.1.0/src/templaterepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:36:10.000000 templaterepo-0.1.0/src/templaterepo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 20:36:11.000000 templaterepo-0.1.0/src/templaterepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 20:36:11.000000 templaterepo-0.1.0/src/templaterepo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:11.102963 templaterepo-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-01 20:36:03.000000 templaterepo-0.1.0/tests/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:41:18.644000 templaterepo-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-08-01 20:41:09.000000 templaterepo-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 20:41:09.000000 templaterepo-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-01 20:41:18.644000 templaterepo-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-01 20:41:09.000000 templaterepo-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-08-01 20:41:09.000000 templaterepo-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:41:18.644000 templaterepo-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-08-01 20:41:09.000000 templaterepo-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:41:18.644000 templaterepo-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:41:18.648000 templaterepo-0.1.1/src/templaterepo/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-01 20:41:18.648000 templaterepo-0.1.1/src/templaterepo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:41:18.644000 templaterepo-0.1.1/src/templaterepo/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-01 20:41:09.000000 templaterepo-0.1.1/src/templaterepo/_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:41:18.644000 templaterepo-0.1.1/src/templaterepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-01 20:41:18.000000 templaterepo-0.1.1/src/templaterepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-01 20:41:18.000000 templaterepo-0.1.1/src/templaterepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:41:18.000000 templaterepo-0.1.1/src/templaterepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:41:18.000000 templaterepo-0.1.1/src/templaterepo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 20:41:18.000000 templaterepo-0.1.1/src/templaterepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 20:41:18.000000 templaterepo-0.1.1/src/templaterepo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:41:18.644000 templaterepo-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-01 20:41:09.000000 templaterepo-0.1.1/tests/test_template.py
```

### Comparing `templaterepo-0.1.0/LICENSE.txt` & `templaterepo-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `templaterepo-0.1.0/pyproject.toml` & `templaterepo-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `templaterepo-0.1.0/setup.py` & `templaterepo-0.1.1/setup.py`

 * *Files identical despite different names*

