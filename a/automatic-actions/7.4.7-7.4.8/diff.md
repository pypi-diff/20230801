# Comparing `tmp/automatic-actions-7.4.7.tar.gz` & `tmp/automatic-actions-7.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automatic-actions-7.4.7.tar", last modified: Tue Aug  1 13:07:39 2023, max compression
+gzip compressed data, was "automatic-actions-7.4.8.tar", last modified: Tue Aug  1 13:15:08 2023, max compression
```

## Comparing `automatic-actions-7.4.7.tar` & `automatic-actions-7.4.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:07:39.994928 automatic-actions-7.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-01 13:07:27.000000 automatic-actions-7.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-01 13:07:39.990928 automatic-actions-7.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 13:07:27.000000 automatic-actions-7.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:07:39.990928 automatic-actions-7.4.7/automatic_actions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-01 13:07:39.000000 automatic-actions-7.4.7/automatic_actions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-01 13:07:39.000000 automatic-actions-7.4.7/automatic_actions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:07:39.000000 automatic-actions-7.4.7/automatic_actions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-08-01 13:07:39.000000 automatic-actions-7.4.7/automatic_actions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-01 13:07:39.000000 automatic-actions-7.4.7/automatic_actions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-01 13:07:27.000000 automatic-actions-7.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 13:07:39.994928 automatic-actions-7.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-08-01 13:07:27.000000 automatic-actions-7.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:07:39.990928 automatic-actions-7.4.7/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:07:27.000000 automatic-actions-7.4.7/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-01 13:07:27.000000 automatic-actions-7.4.7/src/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:07:27.000000 automatic-actions-7.4.7/src/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-01 13:07:27.000000 automatic-actions-7.4.7/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:15:08.153731 automatic-actions-7.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-01 13:14:50.000000 automatic-actions-7.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-01 13:15:08.149731 automatic-actions-7.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 13:14:50.000000 automatic-actions-7.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:15:08.149731 automatic-actions-7.4.8/automatic_actions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-01 13:15:08.000000 automatic-actions-7.4.8/automatic_actions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-01 13:15:08.000000 automatic-actions-7.4.8/automatic_actions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:15:08.000000 automatic-actions-7.4.8/automatic_actions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-08-01 13:15:08.000000 automatic-actions-7.4.8/automatic_actions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-01 13:15:08.000000 automatic-actions-7.4.8/automatic_actions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-01 13:14:50.000000 automatic-actions-7.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 13:15:08.153731 automatic-actions-7.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-08-01 13:14:50.000000 automatic-actions-7.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:15:08.149731 automatic-actions-7.4.8/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:14:50.000000 automatic-actions-7.4.8/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-01 13:14:50.000000 automatic-actions-7.4.8/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:14:50.000000 automatic-actions-7.4.8/src/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-01 13:14:50.000000 automatic-actions-7.4.8/src/version.py
```

### Comparing `automatic-actions-7.4.7/LICENSE` & `automatic-actions-7.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `automatic-actions-7.4.7/PKG-INFO` & `automatic-actions-7.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automatic-actions
-Version: 7.4.7
+Version: 7.4.8
 Summary: Test lib for automatic actions.
 Home-page: https://github.com/cxnt/automatic-actions
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `automatic-actions-7.4.7/automatic_actions.egg-info/PKG-INFO` & `automatic-actions-7.4.8/automatic_actions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automatic-actions
-Version: 7.4.7
+Version: 7.4.8
 Summary: Test lib for automatic actions.
 Home-page: https://github.com/cxnt/automatic-actions
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `automatic-actions-7.4.7/automatic_actions.egg-info/requires.txt` & `automatic-actions-7.4.8/automatic_actions.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `automatic-actions-7.4.7/setup.py` & `automatic-actions-7.4.8/setup.py`

 * *Files identical despite different names*

