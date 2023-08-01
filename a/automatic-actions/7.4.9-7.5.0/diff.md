# Comparing `tmp/automatic-actions-7.4.9.tar.gz` & `tmp/automatic-actions-7.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automatic-actions-7.4.9.tar", last modified: Tue Aug  1 13:23:04 2023, max compression
+gzip compressed data, was "automatic-actions-7.5.0.tar", last modified: Tue Aug  1 13:45:10 2023, max compression
```

## Comparing `automatic-actions-7.4.9.tar` & `automatic-actions-7.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:23:04.855055 automatic-actions-7.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-01 13:22:52.000000 automatic-actions-7.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-01 13:23:04.855055 automatic-actions-7.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 13:22:52.000000 automatic-actions-7.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:23:04.855055 automatic-actions-7.4.9/automatic_actions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-01 13:23:04.000000 automatic-actions-7.4.9/automatic_actions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-01 13:23:04.000000 automatic-actions-7.4.9/automatic_actions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:23:04.000000 automatic-actions-7.4.9/automatic_actions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-08-01 13:23:04.000000 automatic-actions-7.4.9/automatic_actions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-01 13:23:04.000000 automatic-actions-7.4.9/automatic_actions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-01 13:22:52.000000 automatic-actions-7.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 13:23:04.855055 automatic-actions-7.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-08-01 13:22:52.000000 automatic-actions-7.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:23:04.855055 automatic-actions-7.4.9/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:22:52.000000 automatic-actions-7.4.9/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-01 13:22:52.000000 automatic-actions-7.4.9/src/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:22:52.000000 automatic-actions-7.4.9/src/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-01 13:22:52.000000 automatic-actions-7.4.9/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:45:10.734024 automatic-actions-7.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-01 13:44:55.000000 automatic-actions-7.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-01 13:45:10.734024 automatic-actions-7.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 13:44:55.000000 automatic-actions-7.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:45:10.730024 automatic-actions-7.5.0/automatic_actions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-01 13:45:10.000000 automatic-actions-7.5.0/automatic_actions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-01 13:45:10.000000 automatic-actions-7.5.0/automatic_actions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:45:10.000000 automatic-actions-7.5.0/automatic_actions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-08-01 13:45:10.000000 automatic-actions-7.5.0/automatic_actions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-01 13:45:10.000000 automatic-actions-7.5.0/automatic_actions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-01 13:44:55.000000 automatic-actions-7.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 13:45:10.734024 automatic-actions-7.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-08-01 13:44:55.000000 automatic-actions-7.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:45:10.734024 automatic-actions-7.5.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:55.000000 automatic-actions-7.5.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-01 13:44:55.000000 automatic-actions-7.5.0/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:44:55.000000 automatic-actions-7.5.0/src/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-01 13:44:55.000000 automatic-actions-7.5.0/src/version.py
```

### Comparing `automatic-actions-7.4.9/LICENSE` & `automatic-actions-7.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `automatic-actions-7.4.9/PKG-INFO` & `automatic-actions-7.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automatic-actions
-Version: 7.4.9
+Version: 7.5.0
 Summary: Test lib for automatic actions.
 Home-page: https://github.com/cxnt/automatic-actions
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `automatic-actions-7.4.9/automatic_actions.egg-info/PKG-INFO` & `automatic-actions-7.5.0/automatic_actions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automatic-actions
-Version: 7.4.9
+Version: 7.5.0
 Summary: Test lib for automatic actions.
 Home-page: https://github.com/cxnt/automatic-actions
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `automatic-actions-7.4.9/automatic_actions.egg-info/requires.txt` & `automatic-actions-7.5.0/automatic_actions.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `automatic-actions-7.4.9/setup.py` & `automatic-actions-7.5.0/setup.py`

 * *Files identical despite different names*

