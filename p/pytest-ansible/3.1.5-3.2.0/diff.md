# Comparing `tmp/pytest-ansible-3.1.5.tar.gz` & `tmp/pytest-ansible-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-ansible-3.1.5.tar", last modified: Mon May 15 20:06:18 2023, max compression
+gzip compressed data, was "pytest-ansible-3.2.0.tar", last modified: Tue Aug  1 14:04:54 2023, max compression
```

## Comparing `pytest-ansible-3.1.5.tar` & `pytest-ansible-3.2.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.722703 pytest-ansible-3.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.706703 pytest-ansible-3.1.5/.config/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.config/requirements-lock.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.config/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.config/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.706703 pytest-ansible-3.1.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.706703 pytest-ansible-3.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.706703 pytest-ansible-3.1.5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-05-15 20:06:18.722703 pytest-ansible-3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/inventory
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 20:06:18.722703 pytest-ansible-3.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.698703 pytest-ansible-3.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.710703 pytest-ansible-3.1.5/src/pytest_ansible/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 20:06:18.000000 pytest-ansible-3.1.5/src/pytest_ansible/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/has_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.714703 pytest-ansible-3.1.5/src/pytest_ansible/host_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/host_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v212.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v213.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v24.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v28.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v29.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.718703 pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v212.py
--rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v213.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v24.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v28.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v29.py
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/src/pytest_ansible/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.714703 pytest-ansible-3.1.5/src/pytest_ansible.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-05-15 20:06:18.000000 pytest-ansible-3.1.5/src/pytest_ansible.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-15 20:06:18.000000 pytest-ansible-3.1.5/src/pytest_ansible.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:06:18.000000 pytest-ansible-3.1.5/src/pytest_ansible.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-15 20:06:18.000000 pytest-ansible-3.1.5/src/pytest_ansible.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-15 20:06:18.000000 pytest-ansible-3.1.5/src/pytest_ansible.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 20:06:18.000000 pytest-ansible-3.1.5/src/pytest_ansible.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.722703 pytest-ansible-3.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tests/test_adhoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tests/test_adhoc_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tests/test_host_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tests/test_module_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tests/test_module_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tests/test_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:06:18.722703 pytest-ansible-3.1.5/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tests/unit/test_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-15 20:06:03.000000 pytest-ansible-3.1.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.163216 pytest-ansible-3.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.139216 pytest-ansible-3.2.0/.config/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.config/requirements-lock.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.config/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.139216 pytest-ansible-3.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.143216 pytest-ansible-3.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.143216 pytest-ansible-3.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-08-01 14:04:54.163216 pytest-ansible-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/inventory
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:04:54.163216 pytest-ansible-3.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.131216 pytest-ansible-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.147216 pytest-ansible-3.2.0/src/pytest_ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-01 14:04:54.000000 pytest-ansible-3.2.0/src/pytest_ansible/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/has_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.151216 pytest-ansible-3.2.0/src/pytest_ansible/host_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/host_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v212.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v213.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v24.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v28.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v29.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.155216 pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v212.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v213.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v24.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v28.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v29.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11532 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/src/pytest_ansible/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.147216 pytest-ansible-3.2.0/src/pytest_ansible.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-08-01 14:04:54.000000 pytest-ansible-3.2.0/src/pytest_ansible.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-08-01 14:04:54.000000 pytest-ansible-3.2.0/src/pytest_ansible.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:04:54.000000 pytest-ansible-3.2.0/src/pytest_ansible.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-01 14:04:54.000000 pytest-ansible-3.2.0/src/pytest_ansible.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-01 14:04:54.000000 pytest-ansible-3.2.0/src/pytest_ansible.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 14:04:54.000000 pytest-ansible-3.2.0/src/pytest_ansible.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.159216 pytest-ansible-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tests/test_adhoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tests/test_adhoc_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tests/test_host_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tests/test_module_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tests/test_module_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tests/test_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:04:54.159216 pytest-ansible-3.2.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tests/unit/test_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-01 14:04:37.000000 pytest-ansible-3.2.0/tox.ini
```

### Comparing `pytest-ansible-3.1.5/.flake8` & `pytest-ansible-3.2.0/.flake8`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/.github/workflows/release.yml` & `pytest-ansible-3.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/.github/workflows/tox.yml` & `pytest-ansible-3.2.0/.github/workflows/tox.yml`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         uses: coactions/dynamic-matrix@v1
         with:
           min_python: "3.7"
           max_python: "3.11"
           other_names: |
             lint
             pkg
-            devel
+            py310-devel
           platforms: linux
 
   build:
     name: ${{ matrix.name }}
     runs-on: ${{ matrix.os || 'ubuntu-22.04' }}
     # Failure of 'devel' job should not mark the whole workflow as failed
     continue-on-error: ${{ contains(matrix.name, 'devel') && true || false }}
@@ -96,19 +96,14 @@
         run: python3 -m tox --notest --skip-missing-interpreters false -vv -e ${{ matrix.passed_name }}
         timeout-minutes: 5 # average is under 1, but macos can be over 3
 
       # sequential run improves browsing experience (almost no speed impact)
       - name: tox -e ${{ matrix.passed_name }}
         run: python3 -m tox -e ${{ matrix.passed_name }}
 
-      - name: Combine coverage data
-        if: ${{ startsWith(matrix.passed_name, 'py') }}
-        # produce a single .coverage file at repo root
-        run: tox -e coverage
-
       - name: Upload coverage data
         if: ${{ startsWith(matrix.passed_name, 'py') }}
         uses: codecov/codecov-action@v3
         with:
           name: ${{ matrix.passed_name }}
           fail_ci_if_error: false # see https://github.com/codecov/codecov-action/issues/598
           token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `pytest-ansible-3.1.5/.gitignore` & `pytest-ansible-3.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/.pre-commit-config.yaml` & `pytest-ansible-3.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/HISTORY.md` & `pytest-ansible-3.2.0/HISTORY.md`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/LICENSE` & `pytest-ansible-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/PKG-INFO` & `pytest-ansible-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-ansible
-Version: 3.1.5
+Version: 3.2.0
 Summary: Plugin for pytest to simplify calling ansible modules from tests or fixtures
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/pytest-ansible
 Project-URL: documentation, https://github.com/ansible-community/pytest-ansible
 Project-URL: repository, https://github.com/ansible-community/pytest-ansible
@@ -70,15 +70,15 @@
     [--become-method <method>] \
     [--limit <limit>] \
     [--check]
 ```
 
 ## Inventory
 
-Using ansible first starts with defining your inventory. This can be done
+Using ansible first starts with defining your inventory. This can be done in
 several ways, but to start, we'll use the `ansible_adhoc` fixture.
 
 ```python
 def test_my_inventory(ansible_adhoc):
     hosts = ansible_adhoc()
 ```
```

### Comparing `pytest-ansible-3.1.5/README.md` & `pytest-ansible-3.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     [--become-method <method>] \
     [--limit <limit>] \
     [--check]
 ```
 
 ## Inventory
 
-Using ansible first starts with defining your inventory. This can be done
+Using ansible first starts with defining your inventory. This can be done in
 several ways, but to start, we'll use the `ansible_adhoc` fixture.
 
 ```python
 def test_my_inventory(ansible_adhoc):
     hosts = ansible_adhoc()
 ```
```

### Comparing `pytest-ansible-3.1.5/inventory` & `pytest-ansible-3.2.0/inventory`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/pyproject.toml` & `pytest-ansible-3.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
   "too-many-locals",
   "too-many-statements",
   "unexpected-keyword-arg",
   "unused-argument",
   "invalid-name",
 ]
 
-[tool.pytest]
+[tool.pytest.ini_options]
 minversion = 6.0
 addopts = ["-v", "--tb=native"]
 markers = [
   "old",
   "unit",
   "ansible_v1_xfail",
   "requires_ansible_v1",
```

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/errors.py` & `pytest-ansible-3.2.0/src/pytest_ansible/errors.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/fixtures.py` & `pytest-ansible-3.2.0/src/pytest_ansible/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/has_version.py` & `pytest-ansible-3.2.0/src/pytest_ansible/has_version.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/host_manager/__init__.py` & `pytest-ansible-3.2.0/src/pytest_ansible/host_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v1.py` & `pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v1.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v2.py` & `pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v2.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v212.py` & `pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v212.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v213.py` & `pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v213.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v24.py` & `pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v24.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v28.py` & `pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v28.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/host_manager/v29.py` & `pytest-ansible-3.2.0/src/pytest_ansible/host_manager/v29.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/__init__.py` & `pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v1.py` & `pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v1.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v2.py` & `pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v2.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v212.py` & `pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v212.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v213.py` & `pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v213.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v24.py` & `pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v24.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v28.py` & `pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v28.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/module_dispatcher/v29.py` & `pytest-ansible-3.2.0/src/pytest_ansible/module_dispatcher/v29.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/plugin.py` & `pytest-ansible-3.2.0/src/pytest_ansible/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         default=ansible.constants.DEFAULT_BECOME_ASK_PASS,
         help="ask for privilege escalation password (default: %(default)s)",
     )
     group.addoption(
         "--ansible-unit-inject-only",
         action="store_true",
         default=False,
-        help="Enable support for ansible collection unit tests by only injecting exisiting ANSIBLE_COLLECTIONS_PATHS.",
+        help="Enable support for ansible collection unit tests by only injecting exisiting ANSIBLE_COLLECTIONS_PATH.",
     )
     # Add github marker to --help
     parser.addini("ansible", "Ansible integration", "args")
 
 
 def pytest_configure(config):
     """Validate --ansible-* parameters."""
```

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/results.py` & `pytest-ansible-3.2.0/src/pytest_ansible/results.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible/units.py` & `pytest-ansible-3.2.0/src/pytest_ansible/units.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             for entry in start_path.iterdir():
                 if entry.name == "collections":
                     continue
                 os.symlink(entry, name_dir / entry.name)
 
     logger.info("Collections dir: %s", collections_dir)
 
-    # TODO: Make this a configuration option, check COLLECTIONS_PATHS
+    # TODO: Make this a configuration option, check COLLECTIONS_PATH
     # Add the user location for any dependencies
     paths = [str(collections_dir), "~/.ansible/collections"]
     logger.info("Paths: %s", paths)
 
     acf_inject(paths=paths)
 
     # Inject the path for the collection into sys.path
@@ -117,20 +117,20 @@
     # TODO: Should we install any collection dependencies as well?
     # or let the developer do that?
     # e.g. ansible-galaxy collection install etc
 
     # Set the environment variable as courtesy for integration tests
     env_paths = os.pathsep.join(paths)
     logger.info("Setting ANSIBLE_COLLECTIONS_PATH to %s", env_paths)
-    os.environ["ANSIBLE_COLLECTIONS_PATHS"] = env_paths
+    os.environ["ANSIBLE_COLLECTIONS_PATH"] = env_paths
 
 
 def inject_only() -> None:
-    """Inject the current ANSIBLE_COLLECTIONS_PATHS."""
-    env_paths = os.environ.get("ANSIBLE_COLLECTIONS_PATHS", "")
+    """Inject the current ANSIBLE_COLLECTIONS_PATH."""
+    env_paths = os.environ.get("ANSIBLE_COLLECTIONS_PATH", "")
     path_list = env_paths.split(os.pathsep)
     for path in path_list:
         if path:
             sys.path.insert(0, path)
     logger.debug("sys.path updated: %s", sys.path)
     acf_inject(paths=path_list)
```

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible.egg-info/PKG-INFO` & `pytest-ansible-3.2.0/src/pytest_ansible.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-ansible
-Version: 3.1.5
+Version: 3.2.0
 Summary: Plugin for pytest to simplify calling ansible modules from tests or fixtures
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/pytest-ansible
 Project-URL: documentation, https://github.com/ansible-community/pytest-ansible
 Project-URL: repository, https://github.com/ansible-community/pytest-ansible
@@ -70,15 +70,15 @@
     [--become-method <method>] \
     [--limit <limit>] \
     [--check]
 ```
 
 ## Inventory
 
-Using ansible first starts with defining your inventory. This can be done
+Using ansible first starts with defining your inventory. This can be done in
 several ways, but to start, we'll use the `ansible_adhoc` fixture.
 
 ```python
 def test_my_inventory(ansible_adhoc):
     hosts = ansible_adhoc()
 ```
```

### Comparing `pytest-ansible-3.1.5/src/pytest_ansible.egg-info/SOURCES.txt` & `pytest-ansible-3.2.0/src/pytest_ansible.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/tests/conftest.py` & `pytest-ansible-3.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/tests/test_adhoc.py` & `pytest-ansible-3.2.0/tests/test_adhoc.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/tests/test_adhoc_result.py` & `pytest-ansible-3.2.0/tests/test_adhoc_result.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/tests/test_fixtures.py` & `pytest-ansible-3.2.0/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/tests/test_host_manager.py` & `pytest-ansible-3.2.0/tests/test_host_manager.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/tests/test_module_dispatcher.py` & `pytest-ansible-3.2.0/tests/test_module_dispatcher.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/tests/test_module_result.py` & `pytest-ansible-3.2.0/tests/test_module_result.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/tests/test_params.py` & `pytest-ansible-3.2.0/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.5/tests/unit/test_unit.py` & `pytest-ansible-3.2.0/tests/unit/test_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     """Test only injecting a path.
 
     :param monkeypatch: The pytest monkeypatch fixture
     :param tmp_path: The pytest tmp_path fixture
     :param caplog: The pytest caplog fixture
     """
     caplog.set_level(logging.DEBUG)
-    monkeypatch.setenv("ANSIBLE_COLLECTIONS_PATHS", str(tmp_path / "collections"))
+    monkeypatch.setenv("ANSIBLE_COLLECTIONS_PATH", str(tmp_path / "collections"))
 
     (tmp_path / "collections" / "ansible_collections").mkdir(parents=True)
 
     inject_only()
     assert (
         str(tmp_path / "collections")
         == sys.path[0]
```

### Comparing `pytest-ansible-3.1.5/tox.ini` & `pytest-ansible-3.2.0/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 [tox]
 envlist =
     lint,
     pkg,
     py,
-    devel
+    devel,
+    py37,
+    py38
 skip_missing_interpreters = true
 
 [testenv]
 description =
     Run tests
     devel: with ansible-core devel branch and without dependencies constraints
 commands =
@@ -17,14 +19,16 @@
 passenv =
     ANSIBLE_DEBUG
 setenv =
     ANSIBLE_REMOTE_TEMP = {envdir}/.ansible-remote
     ANSIBLE_LOCAL_TEMP = {envdir}/.ansible-local
     PIP_CONSTRAINT = {toxinidir}/.config/requirements.txt
     devel: PIP_CONSTRAINT = /dev/null
+    py37: PIP_CONSTRAINT = /dev/null
+    py38: PIP_CONSTRAINT = /dev/null
 extras =
     test
 allowlist_externals =
     git
     rm
     sh
 deps =
```

