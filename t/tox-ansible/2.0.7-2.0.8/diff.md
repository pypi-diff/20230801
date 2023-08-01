# Comparing `tmp/tox-ansible-2.0.7.tar.gz` & `tmp/tox-ansible-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tox-ansible-2.0.7.tar", last modified: Mon Jul 31 21:29:21 2023, max compression
+gzip compressed data, was "tox-ansible-2.0.8.tar", last modified: Tue Aug  1 16:21:08 2023, max compression
```

## Comparing `tox-ansible-2.0.7.tar` & `tox-ansible-2.0.8.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:29:21.606878 tox-ansible-2.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:29:21.586878 tox-ansible-2.0.7/.config/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/.config/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/.config/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/.darglint
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:29:21.586878 tox-ansible-2.0.7/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:29:21.590878 tox-ansible-2.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/.github/workflows/run.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-07-31 21:29:21.606878 tox-ansible-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:29:21.594878 tox-ansible-2.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/docs/galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/docs/integration.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/docs/sanity.ini
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/docs/tox-ansible.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/docs/unit.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 21:29:21.606878 tox-ansible-2.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:29:21.582878 tox-ansible-2.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:29:21.594878 tox-ansible-2.0.7/src/tox_ansible/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/src/tox_ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-31 21:29:21.000000 tox-ansible-2.0.7/src/tox_ansible/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16205 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/src/tox_ansible/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:29:21.598878 tox-ansible-2.0.7/src/tox_ansible.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-07-31 21:29:21.000000 tox-ansible-2.0.7/src/tox_ansible.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-31 21:29:21.000000 tox-ansible-2.0.7/src/tox_ansible.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 21:29:21.000000 tox-ansible-2.0.7/src/tox_ansible.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-31 21:29:21.000000 tox-ansible-2.0.7/src/tox_ansible.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-31 21:29:21.000000 tox-ansible-2.0.7/src/tox_ansible.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 21:29:21.000000 tox-ansible-2.0.7/src/tox_ansible.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:29:21.602878 tox-ansible-2.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:29:21.582878 tox-ansible-2.0.7/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:29:21.582878 tox-ansible-2.0.7/tests/fixtures/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:29:21.602878 tox-ansible-2.0.7/tests/fixtures/integration/test_basic/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/tests/fixtures/integration/test_basic/galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/tests/fixtures/integration/test_basic/tox-ansible.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:29:21.602878 tox-ansible-2.0.7/tests/fixtures/integration/test_user_provided/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/tests/fixtures/integration/test_user_provided/galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/tests/fixtures/integration/test_user_provided/tox-ansible.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:29:21.602878 tox-ansible-2.0.7/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/tests/integration/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/tests/integration/test_user_provided.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-31 21:29:00.000000 tox-ansible-2.0.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:21:08.208248 tox-ansible-2.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:21:08.196249 tox-ansible-2.0.8/.config/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/.config/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/.darglint
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:21:08.200249 tox-ansible-2.0.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:21:08.200249 tox-ansible-2.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/.github/workflows/run.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-08-01 16:21:08.208248 tox-ansible-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:21:08.200249 tox-ansible-2.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/docs/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/docs/integration.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/docs/sanity.ini
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/docs/tox-ansible.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/docs/unit.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 16:21:08.208248 tox-ansible-2.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:21:08.196249 tox-ansible-2.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:21:08.204249 tox-ansible-2.0.8/src/tox_ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/src/tox_ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-01 16:21:08.000000 tox-ansible-2.0.8/src/tox_ansible/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16478 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/src/tox_ansible/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:21:08.204249 tox-ansible-2.0.8/src/tox_ansible.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-08-01 16:21:08.000000 tox-ansible-2.0.8/src/tox_ansible.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-01 16:21:08.000000 tox-ansible-2.0.8/src/tox_ansible.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 16:21:08.000000 tox-ansible-2.0.8/src/tox_ansible.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 16:21:08.000000 tox-ansible-2.0.8/src/tox_ansible.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-01 16:21:08.000000 tox-ansible-2.0.8/src/tox_ansible.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 16:21:08.000000 tox-ansible-2.0.8/src/tox_ansible.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:21:08.204249 tox-ansible-2.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:21:08.196249 tox-ansible-2.0.8/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:21:08.196249 tox-ansible-2.0.8/tests/fixtures/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:21:08.204249 tox-ansible-2.0.8/tests/fixtures/integration/test_basic/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/tests/fixtures/integration/test_basic/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/tests/fixtures/integration/test_basic/tox-ansible.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:21:08.204249 tox-ansible-2.0.8/tests/fixtures/integration/test_user_provided/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/tests/fixtures/integration/test_user_provided/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/tests/fixtures/integration/test_user_provided/tox-ansible.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:21:08.208248 tox-ansible-2.0.8/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/tests/integration/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/tests/integration/test_user_provided.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-01 16:20:53.000000 tox-ansible-2.0.8/tox.ini
```

### Comparing `tox-ansible-2.0.7/.flake8` & `tox-ansible-2.0.8/.flake8`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.7/.github/workflows/release.yml` & `tox-ansible-2.0.8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.7/.github/workflows/run.yml` & `tox-ansible-2.0.8/.github/workflows/run.yml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.7/.github/workflows/tox.yml` & `tox-ansible-2.0.8/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.7/.gitignore` & `tox-ansible-2.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.7/.pre-commit-config.yaml` & `tox-ansible-2.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.7/LICENSE` & `tox-ansible-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.7/PKG-INFO` & `tox-ansible-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox-ansible
-Version: 2.0.7
+Version: 2.0.8
 Summary: A radical approach to testing ansible content
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Keywords: ansible,collections,tox
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `tox-ansible-2.0.7/README.md` & `tox-ansible-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.7/cspell.config.yaml` & `tox-ansible-2.0.8/cspell.config.yaml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.7/docs/galaxy.yml` & `tox-ansible-2.0.8/docs/galaxy.yml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.7/docs/integration.ini` & `tox-ansible-2.0.8/docs/integration.ini`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.7/docs/sanity.ini` & `tox-ansible-2.0.8/docs/sanity.ini`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.7/docs/unit.ini` & `tox-ansible-2.0.8/docs/unit.ini`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.7/pyproject.toml` & `tox-ansible-2.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.7/requirements.txt` & `tox-ansible-2.0.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.7/src/tox_ansible/plugin.py` & `tox-ansible-2.0.8/src/tox_ansible/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -530,14 +530,21 @@
     passenv.append("GITHUB_TOKEN")
     return passenv
 
 
 def conf_setenv(env_conf: EnvConfigSet) -> str:
     """Build the set environment variables for the tox environment.
 
+    ansible 2.9 did not support the ANSIBLE_COLLECTION_PATH environment variable
+    ansible 2.16 has it marked for deprecation in 2.19
+
     :param env_conf: The environment configuration.
     :return: The set environment variables.
     """
+    if env_conf.name.endswith("2.9"):
+        envvar_name = "ANSIBLE_COLLECTIONS_PATHS"
+    else:
+        envvar_name = "ANSIBLE_COLLECTIONS_PATH"
     envtmpdir = env_conf["envtmpdir"]
     setenv = []
-    setenv.append(f"ANSIBLE_COLLECTIONS_PATH={envtmpdir}/collections/")
+    setenv.append(f"{envvar_name}={envtmpdir}/collections/")
     return "\n".join(setenv)
```

### Comparing `tox-ansible-2.0.7/src/tox_ansible.egg-info/PKG-INFO` & `tox-ansible-2.0.8/src/tox_ansible.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox-ansible
-Version: 2.0.7
+Version: 2.0.8
 Summary: A radical approach to testing ansible content
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Keywords: ansible,collections,tox
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `tox-ansible-2.0.7/src/tox_ansible.egg-info/SOURCES.txt` & `tox-ansible-2.0.8/src/tox_ansible.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.7/tests/conftest.py` & `tox-ansible-2.0.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.7/tests/integration/test_basic.py` & `tox-ansible-2.0.8/tests/integration/test_basic.py`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.7/tests/integration/test_user_provided.py` & `tox-ansible-2.0.8/tests/integration/test_user_provided.py`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.7/tox.ini` & `tox-ansible-2.0.8/tox.ini`

 * *Files identical despite different names*

