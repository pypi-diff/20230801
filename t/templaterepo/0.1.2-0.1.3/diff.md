# Comparing `tmp/templaterepo-0.1.2.tar.gz` & `tmp/templaterepo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templaterepo-0.1.2.tar", last modified: Tue Aug  1 20:47:17 2023, max compression
+gzip compressed data, was "templaterepo-0.1.3.tar", last modified: Tue Aug  1 20:56:07 2023, max compression
```

## Comparing `templaterepo-0.1.2.tar` & `templaterepo-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:47:17.434649 templaterepo-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-08-01 20:47:05.000000 templaterepo-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 20:47:05.000000 templaterepo-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-01 20:47:17.434649 templaterepo-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-01 20:47:05.000000 templaterepo-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-08-01 20:47:05.000000 templaterepo-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:47:17.434649 templaterepo-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-08-01 20:47:05.000000 templaterepo-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:47:17.434649 templaterepo-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:47:17.438650 templaterepo-0.1.2/src/templaterepo/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-01 20:47:17.438650 templaterepo-0.1.2/src/templaterepo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:47:17.434649 templaterepo-0.1.2/src/templaterepo/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-01 20:47:05.000000 templaterepo-0.1.2/src/templaterepo/_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:47:17.434649 templaterepo-0.1.2/src/templaterepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-01 20:47:17.000000 templaterepo-0.1.2/src/templaterepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-01 20:47:17.000000 templaterepo-0.1.2/src/templaterepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:47:17.000000 templaterepo-0.1.2/src/templaterepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:47:17.000000 templaterepo-0.1.2/src/templaterepo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 20:47:17.000000 templaterepo-0.1.2/src/templaterepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 20:47:17.000000 templaterepo-0.1.2/src/templaterepo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:47:17.434649 templaterepo-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-01 20:47:05.000000 templaterepo-0.1.2/tests/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:56:07.268079 templaterepo-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-08-01 20:55:58.000000 templaterepo-0.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 20:55:58.000000 templaterepo-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-01 20:56:07.268079 templaterepo-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-01 20:55:58.000000 templaterepo-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-08-01 20:55:58.000000 templaterepo-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:56:07.268079 templaterepo-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-08-01 20:55:58.000000 templaterepo-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:56:07.268079 templaterepo-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:56:07.272077 templaterepo-0.1.3/src/templaterepo/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-01 20:56:07.272077 templaterepo-0.1.3/src/templaterepo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:56:07.268079 templaterepo-0.1.3/src/templaterepo/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-01 20:55:58.000000 templaterepo-0.1.3/src/templaterepo/_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:56:07.268079 templaterepo-0.1.3/src/templaterepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-01 20:56:07.000000 templaterepo-0.1.3/src/templaterepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-01 20:56:07.000000 templaterepo-0.1.3/src/templaterepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:56:07.000000 templaterepo-0.1.3/src/templaterepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:56:07.000000 templaterepo-0.1.3/src/templaterepo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 20:56:07.000000 templaterepo-0.1.3/src/templaterepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 20:56:07.000000 templaterepo-0.1.3/src/templaterepo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:56:07.268079 templaterepo-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-01 20:55:58.000000 templaterepo-0.1.3/tests/test_template.py
```

### Comparing `templaterepo-0.1.2/LICENSE.txt` & `templaterepo-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `templaterepo-0.1.2/pyproject.toml` & `templaterepo-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `templaterepo-0.1.2/setup.py` & `templaterepo-0.1.3/setup.py`

 * *Files identical despite different names*

