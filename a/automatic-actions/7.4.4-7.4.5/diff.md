# Comparing `tmp/automatic-actions-7.4.4.tar.gz` & `tmp/automatic-actions-7.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automatic-actions-7.4.4.tar", last modified: Tue Aug  1 12:39:57 2023, max compression
+gzip compressed data, was "automatic-actions-7.4.5.tar", last modified: Tue Aug  1 12:58:20 2023, max compression
```

## Comparing `automatic-actions-7.4.4.tar` & `automatic-actions-7.4.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:39:57.253348 automatic-actions-7.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-01 12:39:41.000000 automatic-actions-7.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-01 12:39:57.253348 automatic-actions-7.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 12:39:41.000000 automatic-actions-7.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:39:57.253348 automatic-actions-7.4.4/automatic_actions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-01 12:39:57.000000 automatic-actions-7.4.4/automatic_actions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-01 12:39:57.000000 automatic-actions-7.4.4/automatic_actions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:39:57.000000 automatic-actions-7.4.4/automatic_actions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-08-01 12:39:57.000000 automatic-actions-7.4.4/automatic_actions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-01 12:39:57.000000 automatic-actions-7.4.4/automatic_actions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-01 12:39:41.000000 automatic-actions-7.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 12:39:57.253348 automatic-actions-7.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-08-01 12:39:41.000000 automatic-actions-7.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:39:57.253348 automatic-actions-7.4.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:39:41.000000 automatic-actions-7.4.4/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-01 12:39:41.000000 automatic-actions-7.4.4/src/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:39:41.000000 automatic-actions-7.4.4/src/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-01 12:39:41.000000 automatic-actions-7.4.4/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:58:20.931711 automatic-actions-7.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-01 12:58:06.000000 automatic-actions-7.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-01 12:58:20.931711 automatic-actions-7.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 12:58:06.000000 automatic-actions-7.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:58:20.931711 automatic-actions-7.4.5/automatic_actions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-01 12:58:20.000000 automatic-actions-7.4.5/automatic_actions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-01 12:58:20.000000 automatic-actions-7.4.5/automatic_actions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:58:20.000000 automatic-actions-7.4.5/automatic_actions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-08-01 12:58:20.000000 automatic-actions-7.4.5/automatic_actions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-01 12:58:20.000000 automatic-actions-7.4.5/automatic_actions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-01 12:58:06.000000 automatic-actions-7.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 12:58:20.931711 automatic-actions-7.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-08-01 12:58:06.000000 automatic-actions-7.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:58:20.931711 automatic-actions-7.4.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:58:06.000000 automatic-actions-7.4.5/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-01 12:58:06.000000 automatic-actions-7.4.5/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:58:06.000000 automatic-actions-7.4.5/src/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-01 12:58:06.000000 automatic-actions-7.4.5/src/version.py
```

### Comparing `automatic-actions-7.4.4/LICENSE` & `automatic-actions-7.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `automatic-actions-7.4.4/PKG-INFO` & `automatic-actions-7.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automatic-actions
-Version: 7.4.4
+Version: 7.4.5
 Summary: Test lib for automatic actions.
 Home-page: https://github.com/cxnt/automatic-actions
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `automatic-actions-7.4.4/automatic_actions.egg-info/PKG-INFO` & `automatic-actions-7.4.5/automatic_actions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automatic-actions
-Version: 7.4.4
+Version: 7.4.5
 Summary: Test lib for automatic actions.
 Home-page: https://github.com/cxnt/automatic-actions
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `automatic-actions-7.4.4/automatic_actions.egg-info/requires.txt` & `automatic-actions-7.4.5/automatic_actions.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `automatic-actions-7.4.4/setup.py` & `automatic-actions-7.4.5/setup.py`

 * *Files identical despite different names*

