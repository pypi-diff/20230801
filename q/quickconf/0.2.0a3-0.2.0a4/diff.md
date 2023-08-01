# Comparing `tmp/quickconf-0.2.0a3.tar.gz` & `tmp/quickconf-0.2.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickconf-0.2.0a3.tar", last modified: Tue Aug  1 19:23:36 2023, max compression
+gzip compressed data, was "quickconf-0.2.0a4.tar", last modified: Tue Aug  1 20:20:51 2023, max compression
```

## Comparing `quickconf-0.2.0a3.tar` & `quickconf-0.2.0a4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.753342 quickconf-0.2.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.745342 quickconf-0.2.0a3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.749342 quickconf-0.2.0a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 19:23:16.000000 quickconf-0.2.0a3/.version
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-01 19:23:36.749342 quickconf-0.2.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.749342 quickconf-0.2.0a3/demo/
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/demo/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/demo/settings.toml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/demo/settings_updated.toml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/demo/typecheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 19:23:36.753342 quickconf-0.2.0a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.745342 quickconf-0.2.0a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.749342 quickconf-0.2.0a3/src/quickconf/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/src/quickconf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 19:23:16.000000 quickconf-0.2.0a3/src/quickconf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15097 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/src/quickconf/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.749342 quickconf-0.2.0a3/src/quickconf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-01 19:23:36.000000 quickconf-0.2.0a3/src/quickconf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-01 19:23:36.000000 quickconf-0.2.0a3/src/quickconf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:23:36.000000 quickconf-0.2.0a3/src/quickconf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-01 19:23:36.000000 quickconf-0.2.0a3/src/quickconf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 19:23:36.000000 quickconf-0.2.0a3/src/quickconf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:23:36.749342 quickconf-0.2.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-01 19:23:09.000000 quickconf-0.2.0a3/tests/test_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:20:51.610807 quickconf-0.2.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-01 20:20:39.000000 quickconf-0.2.0a4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:20:51.606807 quickconf-0.2.0a4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:20:51.610807 quickconf-0.2.0a4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-01 20:20:39.000000 quickconf-0.2.0a4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-08-01 20:20:39.000000 quickconf-0.2.0a4/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-01 20:20:39.000000 quickconf-0.2.0a4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-01 20:20:39.000000 quickconf-0.2.0a4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 20:20:41.000000 quickconf-0.2.0a4/.version
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-01 20:20:39.000000 quickconf-0.2.0a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-01 20:20:51.610807 quickconf-0.2.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-01 20:20:39.000000 quickconf-0.2.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:20:51.610807 quickconf-0.2.0a4/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-08-01 20:20:39.000000 quickconf-0.2.0a4/demo/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-01 20:20:39.000000 quickconf-0.2.0a4/demo/settings.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-01 20:20:39.000000 quickconf-0.2.0a4/demo/settings_updated.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-01 20:20:39.000000 quickconf-0.2.0a4/demo/typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-01 20:20:39.000000 quickconf-0.2.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 20:20:39.000000 quickconf-0.2.0a4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:20:51.610807 quickconf-0.2.0a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:20:51.606807 quickconf-0.2.0a4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:20:51.610807 quickconf-0.2.0a4/src/quickconf/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 20:20:39.000000 quickconf-0.2.0a4/src/quickconf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 20:20:41.000000 quickconf-0.2.0a4/src/quickconf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15097 2023-08-01 20:20:39.000000 quickconf-0.2.0a4/src/quickconf/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:20:51.610807 quickconf-0.2.0a4/src/quickconf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-01 20:20:51.000000 quickconf-0.2.0a4/src/quickconf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-01 20:20:51.000000 quickconf-0.2.0a4/src/quickconf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:20:51.000000 quickconf-0.2.0a4/src/quickconf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-01 20:20:51.000000 quickconf-0.2.0a4/src/quickconf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 20:20:51.000000 quickconf-0.2.0a4/src/quickconf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:20:51.610807 quickconf-0.2.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-01 20:20:39.000000 quickconf-0.2.0a4/tests/test_conf.py
```

### Comparing `quickconf-0.2.0a3/.github/workflows/release.yml` & `quickconf-0.2.0a4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a3/.github/workflows/tests.yml` & `quickconf-0.2.0a4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a3/.gitignore` & `quickconf-0.2.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a3/.pre-commit-config.yaml` & `quickconf-0.2.0a4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a3/LICENSE` & `quickconf-0.2.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a3/PKG-INFO` & `quickconf-0.2.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickconf
-Version: 0.2.0a3
+Version: 0.2.0a4
 Summary: Simple and flexible TOML-file based configurations framework
 Author-email: Kenneth Trelborg Vestergaard <mortencombat@fastmail.com>
 Project-URL: Homepage, https://github.com/mortencombat/quickconf
 Project-URL: Repository, https://github.com/mortencombat/quickconf
 Keywords: configuration,settings,options,toml
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `quickconf-0.2.0a3/README.md` & `quickconf-0.2.0a4/README.md`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a3/demo/example.py` & `quickconf-0.2.0a4/demo/example.py`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a3/pyproject.toml` & `quickconf-0.2.0a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a3/src/quickconf/core.py` & `quickconf-0.2.0a4/src/quickconf/core.py`

 * *Files identical despite different names*

### Comparing `quickconf-0.2.0a3/src/quickconf.egg-info/PKG-INFO` & `quickconf-0.2.0a4/src/quickconf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickconf
-Version: 0.2.0a3
+Version: 0.2.0a4
 Summary: Simple and flexible TOML-file based configurations framework
 Author-email: Kenneth Trelborg Vestergaard <mortencombat@fastmail.com>
 Project-URL: Homepage, https://github.com/mortencombat/quickconf
 Project-URL: Repository, https://github.com/mortencombat/quickconf
 Keywords: configuration,settings,options,toml
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `quickconf-0.2.0a3/src/quickconf.egg-info/SOURCES.txt` & `quickconf-0.2.0a4/src/quickconf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

