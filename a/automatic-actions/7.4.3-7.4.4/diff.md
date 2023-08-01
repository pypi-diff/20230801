# Comparing `tmp/automatic-actions-7.4.3.tar.gz` & `tmp/automatic-actions-7.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automatic-actions-7.4.3.tar", last modified: Mon Feb 13 16:07:42 2023, max compression
+gzip compressed data, was "automatic-actions-7.4.4.tar", last modified: Tue Aug  1 12:39:57 2023, max compression
```

## Comparing `automatic-actions-7.4.3.tar` & `automatic-actions-7.4.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 16:07:42.533563 automatic-actions-7.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-02-13 16:07:31.000000 automatic-actions-7.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-02-13 16:07:42.533563 automatic-actions-7.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-13 16:07:31.000000 automatic-actions-7.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 16:07:42.533563 automatic-actions-7.4.3/automatic_actions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-02-13 16:07:42.000000 automatic-actions-7.4.3/automatic_actions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-13 16:07:42.000000 automatic-actions-7.4.3/automatic_actions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 16:07:42.000000 automatic-actions-7.4.3/automatic_actions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-02-13 16:07:42.000000 automatic-actions-7.4.3/automatic_actions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-13 16:07:42.000000 automatic-actions-7.4.3/automatic_actions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-13 16:07:31.000000 automatic-actions-7.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 16:07:42.533563 automatic-actions-7.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-02-13 16:07:31.000000 automatic-actions-7.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 16:07:42.533563 automatic-actions-7.4.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 16:07:31.000000 automatic-actions-7.4.3/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-02-13 16:07:31.000000 automatic-actions-7.4.3/src/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 16:07:31.000000 automatic-actions-7.4.3/src/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-02-13 16:07:31.000000 automatic-actions-7.4.3/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:39:57.253348 automatic-actions-7.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-01 12:39:41.000000 automatic-actions-7.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-01 12:39:57.253348 automatic-actions-7.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 12:39:41.000000 automatic-actions-7.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:39:57.253348 automatic-actions-7.4.4/automatic_actions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-01 12:39:57.000000 automatic-actions-7.4.4/automatic_actions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-01 12:39:57.000000 automatic-actions-7.4.4/automatic_actions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:39:57.000000 automatic-actions-7.4.4/automatic_actions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-08-01 12:39:57.000000 automatic-actions-7.4.4/automatic_actions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-01 12:39:57.000000 automatic-actions-7.4.4/automatic_actions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-01 12:39:41.000000 automatic-actions-7.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 12:39:57.253348 automatic-actions-7.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-08-01 12:39:41.000000 automatic-actions-7.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:39:57.253348 automatic-actions-7.4.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:39:41.000000 automatic-actions-7.4.4/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-01 12:39:41.000000 automatic-actions-7.4.4/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:39:41.000000 automatic-actions-7.4.4/src/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-01 12:39:41.000000 automatic-actions-7.4.4/src/version.py
```

### Comparing `automatic-actions-7.4.3/LICENSE` & `automatic-actions-7.4.4/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2018 The Python Packaging Authority
+Copyright (c) 2023 The Python Packaging Authority
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `automatic-actions-7.4.3/PKG-INFO` & `automatic-actions-7.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automatic-actions
-Version: 7.4.3
+Version: 7.4.4
 Summary: Test lib for automatic actions.
 Home-page: https://github.com/cxnt/automatic-actions
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `automatic-actions-7.4.3/automatic_actions.egg-info/PKG-INFO` & `automatic-actions-7.4.4/automatic_actions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automatic-actions
-Version: 7.4.3
+Version: 7.4.4
 Summary: Test lib for automatic actions.
 Home-page: https://github.com/cxnt/automatic-actions
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `automatic-actions-7.4.3/automatic_actions.egg-info/requires.txt` & `automatic-actions-7.4.4/automatic_actions.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `automatic-actions-7.4.3/setup.py` & `automatic-actions-7.4.4/setup.py`

 * *Files identical despite different names*

