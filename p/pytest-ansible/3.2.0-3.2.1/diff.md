# Comparing `tmp/pytest-ansible-3.2.0.tar.gz` & `tmp/pytest-ansible-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-ansible-3.2.0.tar", last modified: Tue Aug  1 14:04:54 2023, max compression
+gzip compressed data, was "pytest-ansible-3.2.1.tar", last modified: Tue Aug  1 16:20:00 2023, max compression
```

## Comparing `pytest-ansible-3.2.0.tar` & `pytest-ansible-3.2.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.163216 pytest-ansible-3.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.139216 pytest-ansible-3.2.0/.config/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.config/requirements-lock.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.config/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.config/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.139216 pytest-ansible-3.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.143216 pytest-ansible-3.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.143216 pytest-ansible-3.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-08-01 14:04:54.163216 pytest-ansible-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/inventory
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:04:54.163216 pytest-ansible-3.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.131216 pytest-ansible-3.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.147216 pytest-ansible-3.2.0/src/pytest_ansible/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-01 14:04:54.000000 pytest-ansible-3.2.0/src/pytest_ansible/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/has_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.151216 pytest-ansible-3.2.0/src/pytest_ansible/host_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/host_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v212.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v213.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v24.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v28.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v29.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.155216 pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v212.py
--rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v213.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v24.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v28.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v29.py
--rw-r--r--   0 runner    (1001) docker     (123)    11532 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.147216 pytest-ansible-3.2.0/src/pytest_ansible.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-08-01 14:04:54.000000 pytest-ansible-3.2.0/src/pytest_ansible.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-08-01 14:04:54.000000 pytest-ansible-3.2.0/src/pytest_ansible.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:04:54.000000 pytest-ansible-3.2.0/src/pytest_ansible.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-01 14:04:54.000000 pytest-ansible-3.2.0/src/pytest_ansible.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-01 14:04:54.000000 pytest-ansible-3.2.0/src/pytest_ansible.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 14:04:54.000000 pytest-ansible-3.2.0/src/pytest_ansible.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.159216 pytest-ansible-3.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tests/test_adhoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tests/test_adhoc_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tests/test_host_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tests/test_module_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tests/test_module_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tests/test_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.159216 pytest-ansible-3.2.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tests/unit/test_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:20:00.468285 pytest-ansible-3.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:20:00.456286 pytest-ansible-3.2.1/.config/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/.config/requirements-lock.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/.config/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:20:00.456286 pytest-ansible-3.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:20:00.456286 pytest-ansible-3.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:20:00.456286 pytest-ansible-3.2.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-08-01 16:20:00.468285 pytest-ansible-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/inventory
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 16:20:00.468285 pytest-ansible-3.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:20:00.452286 pytest-ansible-3.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:20:00.460286 pytest-ansible-3.2.1/src/pytest_ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-01 16:20:00.000000 pytest-ansible-3.2.1/src/pytest_ansible/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/has_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:20:00.460286 pytest-ansible-3.2.1/src/pytest_ansible/host_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/host_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/host_manager/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/host_manager/v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/host_manager/v212.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/host_manager/v213.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/host_manager/v24.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/host_manager/v28.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/host_manager/v29.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:20:00.464285 pytest-ansible-3.2.1/src/pytest_ansible/module_dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/module_dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/module_dispatcher/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/module_dispatcher/v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/module_dispatcher/v212.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/module_dispatcher/v213.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/module_dispatcher/v24.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/module_dispatcher/v28.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/module_dispatcher/v29.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11532 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/src/pytest_ansible/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:20:00.460286 pytest-ansible-3.2.1/src/pytest_ansible.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-08-01 16:20:00.000000 pytest-ansible-3.2.1/src/pytest_ansible.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-08-01 16:20:00.000000 pytest-ansible-3.2.1/src/pytest_ansible.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 16:20:00.000000 pytest-ansible-3.2.1/src/pytest_ansible.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-01 16:20:00.000000 pytest-ansible-3.2.1/src/pytest_ansible.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-01 16:20:00.000000 pytest-ansible-3.2.1/src/pytest_ansible.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 16:20:00.000000 pytest-ansible-3.2.1/src/pytest_ansible.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:20:00.468285 pytest-ansible-3.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/tests/test_adhoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/tests/test_adhoc_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/tests/test_host_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/tests/test_module_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/tests/test_module_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/tests/test_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:20:00.468285 pytest-ansible-3.2.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/tests/unit/test_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-01 16:19:45.000000 pytest-ansible-3.2.1/tox.ini
```

### Comparing `pytest-ansible-3.2.0/.config/requirements.txt` & `pytest-ansible-3.2.1/.config/requirements.txt`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/.flake8` & `pytest-ansible-3.2.1/.flake8`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/.github/workflows/release.yml` & `pytest-ansible-3.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/.github/workflows/tox.yml` & `pytest-ansible-3.2.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/.gitignore` & `pytest-ansible-3.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/.pre-commit-config.yaml` & `pytest-ansible-3.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/HISTORY.md` & `pytest-ansible-3.2.1/HISTORY.md`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/LICENSE` & `pytest-ansible-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/PKG-INFO` & `pytest-ansible-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-ansible
-Version: 3.2.0
+Version: 3.2.1
 Summary: Plugin for pytest to simplify calling ansible modules from tests or fixtures
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/pytest-ansible
 Project-URL: documentation, https://github.com/ansible-community/pytest-ansible
 Project-URL: repository, https://github.com/ansible-community/pytest-ansible
```

### Comparing `pytest-ansible-3.2.0/README.md` & `pytest-ansible-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/inventory` & `pytest-ansible-3.2.1/inventory`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/pyproject.toml` & `pytest-ansible-3.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/errors.py` & `pytest-ansible-3.2.1/src/pytest_ansible/errors.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/fixtures.py` & `pytest-ansible-3.2.1/src/pytest_ansible/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/has_version.py` & `pytest-ansible-3.2.1/src/pytest_ansible/has_version.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/host_manager/__init__.py` & `pytest-ansible-3.2.1/src/pytest_ansible/host_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v1.py` & `pytest-ansible-3.2.1/src/pytest_ansible/host_manager/v1.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v2.py` & `pytest-ansible-3.2.1/src/pytest_ansible/host_manager/v2.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v212.py` & `pytest-ansible-3.2.1/src/pytest_ansible/host_manager/v212.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v213.py` & `pytest-ansible-3.2.1/src/pytest_ansible/host_manager/v213.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v24.py` & `pytest-ansible-3.2.1/src/pytest_ansible/host_manager/v24.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v28.py` & `pytest-ansible-3.2.1/src/pytest_ansible/host_manager/v28.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v29.py` & `pytest-ansible-3.2.1/src/pytest_ansible/host_manager/v29.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/__init__.py` & `pytest-ansible-3.2.1/src/pytest_ansible/module_dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v1.py` & `pytest-ansible-3.2.1/src/pytest_ansible/module_dispatcher/v1.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v2.py` & `pytest-ansible-3.2.1/src/pytest_ansible/module_dispatcher/v2.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v212.py` & `pytest-ansible-3.2.1/src/pytest_ansible/module_dispatcher/v212.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v213.py` & `pytest-ansible-3.2.1/src/pytest_ansible/module_dispatcher/v213.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v24.py` & `pytest-ansible-3.2.1/src/pytest_ansible/module_dispatcher/v24.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v28.py` & `pytest-ansible-3.2.1/src/pytest_ansible/module_dispatcher/v28.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v29.py` & `pytest-ansible-3.2.1/src/pytest_ansible/module_dispatcher/v29.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/plugin.py` & `pytest-ansible-3.2.1/src/pytest_ansible/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/results.py` & `pytest-ansible-3.2.1/src/pytest_ansible/results.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible/units.py` & `pytest-ansible-3.2.1/src/pytest_ansible/units.py`

 * *Files 15% similar despite different names*

```diff
@@ -115,22 +115,25 @@
     logger.debug("sys.path updated: %s", sys.path)
 
     # TODO: Should we install any collection dependencies as well?
     # or let the developer do that?
     # e.g. ansible-galaxy collection install etc
 
     # Set the environment variable as courtesy for integration tests
+
+    envvar_name = determine_envvar()
     env_paths = os.pathsep.join(paths)
-    logger.info("Setting ANSIBLE_COLLECTIONS_PATH to %s", env_paths)
-    os.environ["ANSIBLE_COLLECTIONS_PATH"] = env_paths
+    logger.info("Setting %s to %s", envvar_name, env_paths)
+    os.environ[envvar_name] = env_paths
 
 
 def inject_only() -> None:
-    """Inject the current ANSIBLE_COLLECTIONS_PATH."""
-    env_paths = os.environ.get("ANSIBLE_COLLECTIONS_PATH", "")
+    """Inject the current ANSIBLE_COLLECTIONS_PATH(S)."""
+    envvar_name = determine_envvar()
+    env_paths = os.environ.get(envvar_name, "")
     path_list = env_paths.split(os.pathsep)
     for path in path_list:
         if path:
             sys.path.insert(0, path)
     logger.debug("sys.path updated: %s", sys.path)
     acf_inject(paths=path_list)
 
@@ -144,7 +147,21 @@
     if HAS_COLLECTION_FINDER:
         acf = _AnsibleCollectionFinder(paths=paths)
         acf._install()
         logger.debug("_ACF installed: %s", paths)
         logger.debug("_ACF configured paths: %s", acf._n_configured_paths)
     else:
         logger.debug("_ACF not available")
+
+
+def determine_envvar() -> str:
+    """Use the existence of the AnsibleCollectionFinder to determine
+    the ansible version.
+
+    ansible 2.9 did not have AnsibleCollectionFinder and did not support ANSIBLE_COLLECTIONS_PATH
+    later versions do.
+
+    :returns: The appropriate environment variable to use
+    """
+    if not HAS_COLLECTION_FINDER:
+        return "ANSIBLE_COLLECTIONS_PATHS"
+    return "ANSIBLE_COLLECTIONS_PATH"
```

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible.egg-info/PKG-INFO` & `pytest-ansible-3.2.1/src/pytest_ansible.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-ansible
-Version: 3.2.0
+Version: 3.2.1
 Summary: Plugin for pytest to simplify calling ansible modules from tests or fixtures
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/pytest-ansible
 Project-URL: documentation, https://github.com/ansible-community/pytest-ansible
 Project-URL: repository, https://github.com/ansible-community/pytest-ansible
```

### Comparing `pytest-ansible-3.2.0/src/pytest_ansible.egg-info/SOURCES.txt` & `pytest-ansible-3.2.1/src/pytest_ansible.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/tests/conftest.py` & `pytest-ansible-3.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/tests/test_adhoc.py` & `pytest-ansible-3.2.1/tests/test_adhoc.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/tests/test_adhoc_result.py` & `pytest-ansible-3.2.1/tests/test_adhoc_result.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/tests/test_fixtures.py` & `pytest-ansible-3.2.1/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/tests/test_host_manager.py` & `pytest-ansible-3.2.1/tests/test_host_manager.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/tests/test_module_dispatcher.py` & `pytest-ansible-3.2.1/tests/test_module_dispatcher.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/tests/test_module_result.py` & `pytest-ansible-3.2.1/tests/test_module_result.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/tests/test_params.py` & `pytest-ansible-3.2.1/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/tests/unit/test_unit.py` & `pytest-ansible-3.2.1/tests/unit/test_unit.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.2.0/tox.ini` & `pytest-ansible-3.2.1/tox.ini`

 * *Files identical despite different names*

