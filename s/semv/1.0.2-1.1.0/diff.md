# Comparing `tmp/semv-1.0.2.tar.gz` & `tmp/semv-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semv-1.0.2.tar", last modified: Sat Jul 29 20:36:27 2023, max compression
+gzip compressed data, was "semv-1.1.0.tar", last modified: Tue Aug  1 08:01:28 2023, max compression
```

## Comparing `semv-1.0.2.tar` & `semv-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:36:27.503829 semv-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:36:27.487829 semv-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:36:27.491829 semv-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-29 20:35:39.000000 semv-1.0.2/.github/workflows/attempt-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-29 20:35:39.000000 semv-1.0.2/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-29 20:35:39.000000 semv-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-29 20:35:39.000000 semv-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-29 20:36:27.503829 semv-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-29 20:35:39.000000 semv-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-29 20:35:39.000000 semv-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 20:36:27.503829 semv-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:36:27.487829 semv-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:36:27.495829 semv-1.0.2/src/semv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/increment.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/version_control_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:36:27.499829 semv-1.0.2/src/semv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-29 20:36:27.000000 semv-1.0.2/src/semv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-29 20:36:27.000000 semv-1.0.2/src/semv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 20:36:27.000000 semv-1.0.2/src/semv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-29 20:36:27.000000 semv-1.0.2/src/semv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-29 20:36:27.000000 semv-1.0.2/src/semv.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:36:27.487829 semv-1.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:36:27.499829 semv-1.0.2/tests/cram/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-29 20:35:39.000000 semv-1.0.2/tests/cram/setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-29 20:35:39.000000 semv-1.0.2/tests/cram/test_normal_usage.t
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:36:27.503829 semv-1.0.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-29 20:35:39.000000 semv-1.0.2/tests/unit/test_commit_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-29 20:35:39.000000 semv-1.0.2/tests/unit/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-29 20:35:39.000000 semv-1.0.2/tests/unit/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-29 20:35:39.000000 semv-1.0.2/tests/unit/test_version_incrementer.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-29 20:35:39.000000 semv-1.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:01:28.570065 semv-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:01:28.566064 semv-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:01:28.566064 semv-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-08-01 08:00:28.000000 semv-1.1.0/.github/workflows/attempt-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-01 08:00:28.000000 semv-1.1.0/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-01 08:00:28.000000 semv-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 08:00:28.000000 semv-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-08-01 08:01:28.570065 semv-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-01 08:00:28.000000 semv-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-01 08:00:28.000000 semv-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 08:01:28.570065 semv-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:01:28.566064 semv-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:01:28.566064 semv-1.1.0/src/semv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/increment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-01 08:00:28.000000 semv-1.1.0/src/semv/version_control_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:01:28.570065 semv-1.1.0/src/semv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-08-01 08:01:28.000000 semv-1.1.0/src/semv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-01 08:01:28.000000 semv-1.1.0/src/semv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 08:01:28.000000 semv-1.1.0/src/semv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 08:01:28.000000 semv-1.1.0/src/semv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 08:01:28.000000 semv-1.1.0/src/semv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 08:01:28.000000 semv-1.1.0/src/semv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:01:28.566064 semv-1.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:01:28.570065 semv-1.1.0/tests/cram/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-01 08:00:28.000000 semv-1.1.0/tests/cram/setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-01 08:00:28.000000 semv-1.1.0/tests/cram/test_config.t
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-01 08:00:28.000000 semv-1.1.0/tests/cram/test_multiple_branches.t
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-08-01 08:00:28.000000 semv-1.1.0/tests/cram/test_normal_usage.t
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:01:28.570065 semv-1.1.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-01 08:00:28.000000 semv-1.1.0/tests/unit/test_commit_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-01 08:00:28.000000 semv-1.1.0/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-08-01 08:00:28.000000 semv-1.1.0/tests/unit/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-01 08:00:28.000000 semv-1.1.0/tests/unit/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-01 08:00:28.000000 semv-1.1.0/tests/unit/test_version_incrementer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-01 08:00:28.000000 semv-1.1.0/tox.ini
```

### Comparing `semv-1.0.2/.github/workflows/run-tests.yml` & `semv-1.1.0/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `semv-1.0.2/.gitignore` & `semv-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `semv-1.0.2/LICENSE` & `semv-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semv-1.0.2/src/semv/interface.py` & `semv-1.1.0/src/semv/interface.py`

 * *Files identical despite different names*

### Comparing `semv-1.0.2/src/semv/parse.py` & `semv-1.1.0/src/semv/parse.py`

 * *Files identical despite different names*

### Comparing `semv-1.0.2/src/semv/types.py` & `semv-1.1.0/src/semv/types.py`

 * *Files identical despite different names*

### Comparing `semv-1.0.2/src/semv/version_control_system.py` & `semv-1.1.0/src/semv/version_control_system.py`

 * *Files identical despite different names*

### Comparing `semv-1.0.2/tests/cram/test_normal_usage.t` & `semv-1.1.0/tests/cram/test_normal_usage.t`

 * *Files identical despite different names*

### Comparing `semv-1.0.2/tests/unit/test_commit_parsing.py` & `semv-1.1.0/tests/unit/test_commit_parsing.py`

 * *Files identical despite different names*

### Comparing `semv-1.0.2/tests/unit/test_git.py` & `semv-1.1.0/tests/unit/test_git.py`

 * *Files identical despite different names*

### Comparing `semv-1.0.2/tests/unit/test_version.py` & `semv-1.1.0/tests/unit/test_version.py`

 * *Files identical despite different names*

### Comparing `semv-1.0.2/tox.ini` & `semv-1.1.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 [testenv:format]
 skip_install = true
 deps = blue
 commands = blue --check src/semv
 
 [testenv:typing]
 skip_install = true
-deps = mypy
+deps =
+  mypy
+  tomli
 commands = mypy src/semv
 
 [testenv:build]
 skip_dist = true
 skip_install = true
 deps =
   build
```

