# Comparing `tmp/seb-0.0.0.tar.gz` & `tmp/seb-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seb-0.0.0.tar", last modified: Tue Aug  1 03:37:43 2023, max compression
+gzip compressed data, was "seb-0.1.5.tar", last modified: Tue Aug  1 04:13:23 2023, max compression
```

## Comparing `seb-0.0.0.tar` & `seb-0.1.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 03:37:43.182105 seb-0.0.0/
--rw-r--r--   0 root         (0) root         (0)      478 2023-08-01 03:37:34.000000 seb-0.0.0/.cookiecutter.json
--rw-r--r--   0 root         (0) root         (0)      725 2023-08-01 03:37:34.000000 seb-0.0.0/.cruft.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 03:37:43.174105 seb-0.0.0/.github/
--rw-r--r--   0 root         (0) root         (0)      529 2023-08-01 03:37:34.000000 seb-0.0.0/.github/dependabot.yml
--rw-r--r--   0 root         (0) root         (0)     1703 2023-08-01 03:37:34.000000 seb-0.0.0/.github/recommended_repo_setup.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 03:37:43.174105 seb-0.0.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      720 2023-08-01 03:37:34.000000 seb-0.0.0/.github/workflows/check_for_rej.yml
--rw-r--r--   0 root         (0) root         (0)     2082 2023-08-01 03:37:34.000000 seb-0.0.0/.github/workflows/cruft.yml
--rw-r--r--   0 root         (0) root         (0)     1023 2023-08-01 03:37:34.000000 seb-0.0.0/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)      717 2023-08-01 03:37:34.000000 seb-0.0.0/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)     2882 2023-08-01 03:37:34.000000 seb-0.0.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 root         (0) root         (0)     1663 2023-08-01 03:37:34.000000 seb-0.0.0/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     1132 2023-08-01 03:37:34.000000 seb-0.0.0/.github/workflows/stalebot.yml
--rw-r--r--   0 root         (0) root         (0)     3260 2023-08-01 03:37:34.000000 seb-0.0.0/.github/workflows/static_type_checks.yml
--rw-r--r--   0 root         (0) root         (0)     2570 2023-08-01 03:37:34.000000 seb-0.0.0/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)      269 2023-08-01 03:37:34.000000 seb-0.0.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)      644 2023-08-01 03:37:34.000000 seb-0.0.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    14143 2023-08-01 03:37:34.000000 seb-0.0.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5532 2023-08-01 03:37:34.000000 seb-0.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     2442 2023-08-01 03:37:34.000000 seb-0.0.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     1074 2023-08-01 03:37:34.000000 seb-0.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5010 2023-08-01 03:37:43.182105 seb-0.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2922 2023-08-01 03:37:34.000000 seb-0.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 03:37:43.174105 seb-0.0.0/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 03:37:43.178105 seb-0.0.0/docs/_static/
--rw-r--r--   0 root         (0) root         (0)   417053 2023-08-01 03:37:34.000000 seb-0.0.0/docs/_static/logo.png
--rw-r--r--   0 root         (0) root         (0)  1221950 2023-08-01 03:37:34.000000 seb-0.0.0/docs/_static/social.png
--rw-r--r--   0 root         (0) root         (0)      459 2023-08-01 03:37:34.000000 seb-0.0.0/docs/api.md
--rw-r--r--   0 root         (0) root         (0)     5462 2023-08-01 03:37:34.000000 seb-0.0.0/docs/getting_started.ipynb
--rw-r--r--   0 root         (0) root         (0)     2468 2023-08-01 03:37:34.000000 seb-0.0.0/docs/index.md
--rw-r--r--   0 root         (0) root         (0)      401 2023-08-01 03:37:34.000000 seb-0.0.0/docs/installation.md
--rw-r--r--   0 root         (0) root         (0)     3232 2023-08-01 03:37:34.000000 seb-0.0.0/docs/run_benchmark.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-08-01 03:37:34.000000 seb-0.0.0/mkdocs.yml
--rw-r--r--   0 root         (0) root         (0)     3808 2023-08-01 03:37:34.000000 seb-0.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 03:37:43.182105 seb-0.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 03:37:43.170105 seb-0.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 03:37:43.178105 seb-0.0.0/src/seb/
--rw-r--r--   0 root         (0) root         (0)      465 2023-08-01 03:37:34.000000 seb-0.0.0/src/seb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4480 2023-08-01 03:37:34.000000 seb-0.0.0/src/seb/benchmark.py
--rw-r--r--   0 root         (0) root         (0)      914 2023-08-01 03:37:34.000000 seb-0.0.0/src/seb/full_benchmark.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-08-01 03:37:34.000000 seb-0.0.0/src/seb/model_interface.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 03:37:34.000000 seb-0.0.0/src/seb/py.typed
--rw-r--r--   0 root         (0) root         (0)     1031 2023-08-01 03:37:34.000000 seb-0.0.0/src/seb/registries.py
--rw-r--r--   0 root         (0) root         (0)     3256 2023-08-01 03:37:34.000000 seb-0.0.0/src/seb/result_dataclasses.py
--rw-r--r--   0 root         (0) root         (0)    10168 2023-08-01 03:37:34.000000 seb-0.0.0/src/seb/seb_models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 03:37:43.182105 seb-0.0.0/src/seb/seb_tasks/
--rw-r--r--   0 root         (0) root         (0)       98 2023-08-01 03:37:34.000000 seb-0.0.0/src/seb/seb_tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1164 2023-08-01 03:37:34.000000 seb-0.0.0/src/seb/seb_tasks/danish.py
--rw-r--r--   0 root         (0) root         (0)     2599 2023-08-01 03:37:34.000000 seb-0.0.0/src/seb/seb_tasks/multilingual.py
--rw-r--r--   0 root         (0) root         (0)      513 2023-08-01 03:37:34.000000 seb-0.0.0/src/seb/seb_tasks/norwegian.py
--rw-r--r--   0 root         (0) root         (0)      445 2023-08-01 03:37:34.000000 seb-0.0.0/src/seb/seb_tasks/swedish.py
--rw-r--r--   0 root         (0) root         (0)     2404 2023-08-01 03:37:34.000000 seb-0.0.0/src/seb/tasks_interface.py
--rw-r--r--   0 root         (0) root         (0)     1815 2023-08-01 03:37:34.000000 seb-0.0.0/src/seb/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 03:37:43.182105 seb-0.0.0/src/seb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5010 2023-08-01 03:37:43.000000 seb-0.0.0/src/seb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1341 2023-08-01 03:37:43.000000 seb-0.0.0/src/seb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 03:37:43.000000 seb-0.0.0/src/seb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      448 2023-08-01 03:37:43.000000 seb-0.0.0/src/seb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-08-01 03:37:43.000000 seb-0.0.0/src/seb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    12429 2023-08-01 03:37:34.000000 seb-0.0.0/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 03:37:43.182105 seb-0.0.0/tests/
--rw-r--r--   0 root         (0) root         (0)      631 2023-08-01 03:37:34.000000 seb-0.0.0/tests/dummy_model.py
--rw-r--r--   0 root         (0) root         (0)     1909 2023-08-01 03:37:34.000000 seb-0.0.0/tests/dummy_task.py
--rw-r--r--   0 root         (0) root         (0)      589 2023-08-01 03:37:34.000000 seb-0.0.0/tests/test_all_models.py
--rw-r--r--   0 root         (0) root         (0)     4116 2023-08-01 03:37:34.000000 seb-0.0.0/tests/test_benchmark.py
--rw-r--r--   0 root         (0) root         (0)      379 2023-08-01 03:37:34.000000 seb-0.0.0/tests/test_seb_models.py
--rw-r--r--   0 root         (0) root         (0)     2324 2023-08-01 03:37:34.000000 seb-0.0.0/tests/test_tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 04:13:23.281247 seb-0.1.5/
+-rw-r--r--   0 root         (0) root         (0)      478 2023-08-01 04:13:12.000000 seb-0.1.5/.cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)      725 2023-08-01 04:13:12.000000 seb-0.1.5/.cruft.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 04:13:23.273247 seb-0.1.5/.github/
+-rw-r--r--   0 root         (0) root         (0)      529 2023-08-01 04:13:12.000000 seb-0.1.5/.github/dependabot.yml
+-rw-r--r--   0 root         (0) root         (0)     1703 2023-08-01 04:13:12.000000 seb-0.1.5/.github/recommended_repo_setup.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 04:13:23.273247 seb-0.1.5/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-08-01 04:13:12.000000 seb-0.1.5/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-08-01 04:13:12.000000 seb-0.1.5/.github/workflows/cruft.yml
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-08-01 04:13:12.000000 seb-0.1.5/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)      717 2023-08-01 04:13:12.000000 seb-0.1.5/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)     2882 2023-08-01 04:13:12.000000 seb-0.1.5/.github/workflows/pre-commit.yml
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-08-01 04:13:12.000000 seb-0.1.5/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-08-01 04:13:12.000000 seb-0.1.5/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)     3260 2023-08-01 04:13:12.000000 seb-0.1.5/.github/workflows/static_type_checks.yml
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-08-01 04:13:12.000000 seb-0.1.5/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)      269 2023-08-01 04:13:12.000000 seb-0.1.5/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      644 2023-08-01 04:13:12.000000 seb-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    15720 2023-08-01 04:13:12.000000 seb-0.1.5/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5532 2023-08-01 04:13:12.000000 seb-0.1.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     2442 2023-08-01 04:13:12.000000 seb-0.1.5/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-08-01 04:13:12.000000 seb-0.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4931 2023-08-01 04:13:23.281247 seb-0.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2843 2023-08-01 04:13:12.000000 seb-0.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 04:13:23.273247 seb-0.1.5/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 04:13:23.277247 seb-0.1.5/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)   417053 2023-08-01 04:13:12.000000 seb-0.1.5/docs/_static/logo.png
+-rw-r--r--   0 root         (0) root         (0)  1221950 2023-08-01 04:13:12.000000 seb-0.1.5/docs/_static/social.png
+-rw-r--r--   0 root         (0) root         (0)      459 2023-08-01 04:13:12.000000 seb-0.1.5/docs/api.md
+-rw-r--r--   0 root         (0) root         (0)     5462 2023-08-01 04:13:12.000000 seb-0.1.5/docs/getting_started.ipynb
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-08-01 04:13:12.000000 seb-0.1.5/docs/index.md
+-rw-r--r--   0 root         (0) root         (0)      401 2023-08-01 04:13:12.000000 seb-0.1.5/docs/installation.md
+-rw-r--r--   0 root         (0) root         (0)     3232 2023-08-01 04:13:12.000000 seb-0.1.5/docs/run_benchmark.py
+-rw-r--r--   0 root         (0) root         (0)     1319 2023-08-01 04:13:12.000000 seb-0.1.5/mkdocs.yml
+-rw-r--r--   0 root         (0) root         (0)     3765 2023-08-01 04:13:13.000000 seb-0.1.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 04:13:23.281247 seb-0.1.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 04:13:23.269247 seb-0.1.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 04:13:23.277247 seb-0.1.5/src/seb/
+-rw-r--r--   0 root         (0) root         (0)      465 2023-08-01 04:13:12.000000 seb-0.1.5/src/seb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4480 2023-08-01 04:13:12.000000 seb-0.1.5/src/seb/benchmark.py
+-rw-r--r--   0 root         (0) root         (0)      914 2023-08-01 04:13:12.000000 seb-0.1.5/src/seb/full_benchmark.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-08-01 04:13:12.000000 seb-0.1.5/src/seb/model_interface.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 04:13:12.000000 seb-0.1.5/src/seb/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-08-01 04:13:12.000000 seb-0.1.5/src/seb/registries.py
+-rw-r--r--   0 root         (0) root         (0)     3256 2023-08-01 04:13:12.000000 seb-0.1.5/src/seb/result_dataclasses.py
+-rw-r--r--   0 root         (0) root         (0)    10168 2023-08-01 04:13:12.000000 seb-0.1.5/src/seb/seb_models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 04:13:23.281247 seb-0.1.5/src/seb/seb_tasks/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-08-01 04:13:12.000000 seb-0.1.5/src/seb/seb_tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2023-08-01 04:13:12.000000 seb-0.1.5/src/seb/seb_tasks/danish.py
+-rw-r--r--   0 root         (0) root         (0)     2599 2023-08-01 04:13:12.000000 seb-0.1.5/src/seb/seb_tasks/multilingual.py
+-rw-r--r--   0 root         (0) root         (0)      513 2023-08-01 04:13:12.000000 seb-0.1.5/src/seb/seb_tasks/norwegian.py
+-rw-r--r--   0 root         (0) root         (0)      445 2023-08-01 04:13:12.000000 seb-0.1.5/src/seb/seb_tasks/swedish.py
+-rw-r--r--   0 root         (0) root         (0)     2404 2023-08-01 04:13:12.000000 seb-0.1.5/src/seb/tasks_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2023-08-01 04:13:12.000000 seb-0.1.5/src/seb/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 04:13:23.281247 seb-0.1.5/src/seb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4931 2023-08-01 04:13:23.000000 seb-0.1.5/src/seb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-08-01 04:13:23.000000 seb-0.1.5/src/seb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 04:13:23.000000 seb-0.1.5/src/seb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      448 2023-08-01 04:13:23.000000 seb-0.1.5/src/seb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-08-01 04:13:23.000000 seb-0.1.5/src/seb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    12429 2023-08-01 04:13:12.000000 seb-0.1.5/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 04:13:23.281247 seb-0.1.5/tests/
+-rw-r--r--   0 root         (0) root         (0)      631 2023-08-01 04:13:12.000000 seb-0.1.5/tests/dummy_model.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-08-01 04:13:12.000000 seb-0.1.5/tests/dummy_task.py
+-rw-r--r--   0 root         (0) root         (0)      589 2023-08-01 04:13:12.000000 seb-0.1.5/tests/test_all_models.py
+-rw-r--r--   0 root         (0) root         (0)     4116 2023-08-01 04:13:12.000000 seb-0.1.5/tests/test_benchmark.py
+-rw-r--r--   0 root         (0) root         (0)      379 2023-08-01 04:13:12.000000 seb-0.1.5/tests/test_seb_models.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-08-01 04:13:12.000000 seb-0.1.5/tests/test_tasks.py
```

### Comparing `seb-0.0.0/.cruft.json` & `seb-0.1.5/.cruft.json`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/.github/dependabot.yml` & `seb-0.1.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/.github/recommended_repo_setup.md` & `seb-0.1.5/.github/recommended_repo_setup.md`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/.github/workflows/check_for_rej.yml` & `seb-0.1.5/.github/workflows/check_for_rej.yml`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/.github/workflows/cruft.yml` & `seb-0.1.5/.github/workflows/cruft.yml`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/.github/workflows/dependabot_automerge.yml` & `seb-0.1.5/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/.github/workflows/documentation.yml` & `seb-0.1.5/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/.github/workflows/pre-commit.yml` & `seb-0.1.5/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/.github/workflows/release.yml` & `seb-0.1.5/.github/workflows/release.yml`

 * *Files 7% similar despite different names*

```diff
@@ -13,32 +13,33 @@
 jobs:
   release:
     runs-on: ubuntu-latest
     concurrency: release
     permissions:
       id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
 
+
+    if: ${{ github.ref == 'refs/heads/main' && github.event.workflow_run.conclusion == 'success'}}
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
           token: ${{ secrets.PAT }}
 
       - name: Python Semantic Release
         id: release
         uses: python-semantic-release/python-semantic-release@v8.0.0
         with:
           github_token: ${{ secrets.PAT }}
 
       - name: Publish package distributions to PyPI
-        if: ${{ github.ref == 'refs/heads/main' && github.event.workflow_run.conclusion == 'success' && steps.release.outputs.released == 'true' }}
         uses: pypa/gh-action-pypi-publish@release/v1
+        if: steps.release.outputs.released == 'true'
         # This action supports PyPI's trusted publishing implementation, which allows authentication to PyPI without a manually 
         # configured API token or username/password combination. To perform trusted publishing with this action, your project's 
         # publisher must already be configured on PyPI.
-        
 
       - name: Publish package distributions to GitHub Releases
         uses: python-semantic-release/upload-to-gh-release@main
-        if: ${{ github.ref == 'refs/heads/main' && github.event.workflow_run.conclusion == 'success' && steps.release.outputs.released == 'true' }}
+        if: steps.release.outputs.released == 'true'
         with:
           github_token: ${{ secrets.PAT }}
```

### Comparing `seb-0.0.0/.github/workflows/stalebot.yml` & `seb-0.1.5/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/.github/workflows/static_type_checks.yml` & `seb-0.1.5/.github/workflows/static_type_checks.yml`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/.github/workflows/tests.yml` & `seb-0.1.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/.pre-commit-config.yaml` & `seb-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/CHANGELOG.md` & `seb-0.1.5/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,55 @@
 # CHANGELOG
 
 
 
+## v0.1.4 (2023-08-01)
+
+### Documentation
+
+* docs: Updated links in badge ([`8e3ab16`](https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/commit/8e3ab168b518e095d6f8cd8bf5d8afb2f82de0ba))
+
+### Fix
+
+* fix: ci: removed outdated variables from pyproject.toml ([`b43edd8`](https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/commit/b43edd86701704d25323feb61b5140b5f1059217))
+
+### Unknown
+
+* Merge branch &#39;main&#39; of https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark ([`84244d2`](https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/commit/84244d2117ddf11da2eaf37c4bab1dbef03807d2))
+
+
+## v0.1.3 (2023-08-01)
+
+### Ci
+
+* ci: Added permissions ([`51de97a`](https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/commit/51de97a2af8d43318d6c0e08a51614459fa858b5))
+
+### Fix
+
+* fix: rerun ci ([`94362a9`](https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/commit/94362a97999b17516bdad2bb241675c038ea7350))
+
+### Unknown
+
+* Merge branch &#39;main&#39; of https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark ([`7301671`](https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/commit/73016713ca2b4c253f8211e3ee4db5351bd27fa9))
+
+
 ## v0.1.2 (2023-08-01)
 
 ### Ci
 
 * ci: re-added gh token ([`a280ee6`](https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/commit/a280ee6315c43c8603363d5408065747d0767644))
 
 * ci: Updated release ci to use pypi trusted publishing ([`e5cec02`](https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/commit/e5cec024bce8e907d1edbbf74509360d359e732c))
 
+### Fix
+
+* fix: empty commit ([`73db296`](https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/commit/73db296636c7cc929cf8bb8e4fde2073241a0873))
+
+* fix: Empty commit ([`cc1dfd7`](https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/commit/cc1dfd73c2f011d8ece541effa112b52362e1cc6))
+
 ### Unknown
 
 * Merge branch &#39;main&#39; of https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark ([`66bfdf0`](https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/commit/66bfdf0e9107f00758ae14377885e7fe7e2d9220))
 
 
 ## v0.1.1 (2023-08-01)
```

### Comparing `seb-0.0.0/CODE_OF_CONDUCT.md` & `seb-0.1.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/CONTRIBUTING.md` & `seb-0.1.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/LICENSE` & `seb-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/PKG-INFO` & `seb-0.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seb
-Version: 0.0.0
+Version: 0.1.5
 Summary: Scandinavian Embedding Benchmark
 Author-email: Kenneth Enevoldsen <Kennethcenevoldsen@gmail.com>
 License: MIT License
         
         Copyright © 2023 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,42 +40,42 @@
 Provides-Extra: docs
 License-File: LICENSE
 
 <a href="https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark"><img src="https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/blob/main/docs/_static/logo.png?raw=true" width="120" align="right"/></a>
 
 # Scandinavian Embedding Benchmark
 
-[![PyPI](https://img.shields.io/pypi/v/scandinavian-embedding-benchmark.svg)][pypi status]
-[![Python Version](https://img.shields.io/pypi/pyversions/scandinavian-embedding-benchmark)][pypi status]
+[![PyPI](https://img.shields.io/pypi/v/seb.svg)][pypi status]
+[![Python Version](https://img.shields.io/pypi/pyversions/seb)][pypi status]
 [![documentation](https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/actions/workflows/documentation.yml/badge.svg)][documentation]
 [![Tests](https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/actions/workflows/tests.yml/badge.svg)][tests]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 
-[pypi status]: https://pypi.org/project/scandinavian-embedding-benchmark/
+[pypi status]: https://pypi.org/project/seb/
 [documentation]: https://KennethEnevoldsen.github.io/scandinavian-embedding-benchmark/
 [tests]: https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/actions?workflow=Tests
 [black]: https://github.com/psf/black
 
 
 <!-- start short-description -->
 
 A benchmark for evaluating sentence/document embeddings of Scandinavian language models.
 
 <!-- end short-description -->
 
 ## Installation
 
-You can install `scandinavian-embedding-benchmark` via [pip] from [PyPI]:
+You can install the Scandinavian Embedding Benchmark (`seb`) via [pip] from [PyPI]:
 
 ```bash
 pip install seb
 ```
 
 [pip]: https://pip.pypa.io/en/stable/installing/
-[PyPI]: https://pypi.org/project/cuecy/
+[PyPI]: https://pypi.org/project/seb/
 
 
 To see more examples, see the [documentation].
 
 # 📖 Documentation
 
 | Documentation         |                                                          |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seb Version: 0.0.0 Summary: Scandinavian Embedding
+Metadata-Version: 2.1 Name: seb Version: 0.1.5 Summary: Scandinavian Embedding
 Benchmark Author-email: Kenneth Enevoldsen
 gmail.com> License: MIT License Copyright Â© 2023 Kenneth Enevoldsen Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -21,34 +21,33 @@
 benchmark/ Classifier: Operating System :: POSIX :: Linux Classifier: Operating
 System :: MacOS :: MacOS X Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.9 Description-Content-Type:
 text/markdown Provides-Extra: dev Provides-Extra: tests Provides-Extra: docs
 License-File: LICENSE [https://github.com/KennethEnevoldsen/scandinavian-
 embedding-benchmark/blob/main/docs/_static/logo.png?raw=true] # Scandinavian
-Embedding Benchmark [![PyPI](https://img.shields.io/pypi/v/scandinavian-
-embedding-benchmark.svg)][pypi status] [![Python Version](https://
-img.shields.io/pypi/pyversions/scandinavian-embedding-benchmark)][pypi status]
-[![documentation](https://github.com/KennethEnevoldsen/scandinavian-embedding-
-benchmark/actions/workflows/documentation.yml/badge.svg)][documentation] [!
-[Tests](https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/
-actions/workflows/tests.yml/badge.svg)][tests] [![Black](https://
-img.shields.io/badge/code%20style-black-000000.svg)][black] [pypi status]:
-https://pypi.org/project/scandinavian-embedding-benchmark/ [documentation]:
-https://KennethEnevoldsen.github.io/scandinavian-embedding-benchmark/ [tests]:
-https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/
+Embedding Benchmark [![PyPI](https://img.shields.io/pypi/v/seb.svg)][pypi
+status] [![Python Version](https://img.shields.io/pypi/pyversions/seb)][pypi
+status] [![documentation](https://github.com/KennethEnevoldsen/scandinavian-
+embedding-benchmark/actions/workflows/documentation.yml/badge.svg)]
+[documentation] [![Tests](https://github.com/KennethEnevoldsen/scandinavian-
+embedding-benchmark/actions/workflows/tests.yml/badge.svg)][tests] [![Black]
+(https://img.shields.io/badge/code%20style-black-000000.svg)][black] [pypi
+status]: https://pypi.org/project/seb/ [documentation]: https://
+KennethEnevoldsen.github.io/scandinavian-embedding-benchmark/ [tests]: https://
+github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/
 actions?workflow=Tests [black]: https://github.com/psf/black  A benchmark for
 evaluating sentence/document embeddings of Scandinavian language models.  ##
-Installation You can install `scandinavian-embedding-benchmark` via [pip] from
-[PyPI]: ```bash pip install seb ``` [pip]: https://pip.pypa.io/en/stable/
-installing/ [PyPI]: https://pypi.org/project/cuecy/ To see more examples, see
-the [documentation]. # ð Documentation | Documentation | | | ---------------
------- | -------------------------------------------------------- | | ð§ **
-[Installation]** | Installation instructions on how to install this package | |
-ð©âð» **[Usage]** | Introduction on how to use the package | | ð **
+Installation You can install the Scandinavian Embedding Benchmark (`seb`) via
+[pip] from [PyPI]: ```bash pip install seb ``` [pip]: https://pip.pypa.io/en/
+stable/installing/ [PyPI]: https://pypi.org/project/seb/ To see more examples,
+see the [documentation]. # ð Documentation | Documentation | | | -----------
+---------- | -------------------------------------------------------- | | ð§
+**[Installation]** | Installation instructions on how to install this package |
+| ð©âð» **[Usage]** | Introduction on how to use the package | | ð **
 [Documentation]** | A minimal and developing documentation | # ð¬ Where to
 ask questions | Type | | | ------------------------------ | -------------------
 --- | | ð¨ **Bug Reports** | [GitHub Issue Tracker] | | ð **Feature
 Requests & Ideas** | [GitHub Issue Tracker] | | ð©âð» **Usage Questions**
 | [GitHub Discussions] | | ð¯ **General Discussion** | [GitHub Discussions] |
 [Usage]: https://kennethenevoldsen.github.io/scandinavian-embedding-benchmark/
 getting_started/ [Documentation]: https://KennethEnevoldsen.github.io/
```

### Comparing `seb-0.0.0/README.md` & `seb-0.1.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 <a href="https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark"><img src="https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/blob/main/docs/_static/logo.png?raw=true" width="120" align="right"/></a>
 
 # Scandinavian Embedding Benchmark
 
-[![PyPI](https://img.shields.io/pypi/v/scandinavian-embedding-benchmark.svg)][pypi status]
-[![Python Version](https://img.shields.io/pypi/pyversions/scandinavian-embedding-benchmark)][pypi status]
+[![PyPI](https://img.shields.io/pypi/v/seb.svg)][pypi status]
+[![Python Version](https://img.shields.io/pypi/pyversions/seb)][pypi status]
 [![documentation](https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/actions/workflows/documentation.yml/badge.svg)][documentation]
 [![Tests](https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/actions/workflows/tests.yml/badge.svg)][tests]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 
-[pypi status]: https://pypi.org/project/scandinavian-embedding-benchmark/
+[pypi status]: https://pypi.org/project/seb/
 [documentation]: https://KennethEnevoldsen.github.io/scandinavian-embedding-benchmark/
 [tests]: https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/actions?workflow=Tests
 [black]: https://github.com/psf/black
 
 
 <!-- start short-description -->
 
 A benchmark for evaluating sentence/document embeddings of Scandinavian language models.
 
 <!-- end short-description -->
 
 ## Installation
 
-You can install `scandinavian-embedding-benchmark` via [pip] from [PyPI]:
+You can install the Scandinavian Embedding Benchmark (`seb`) via [pip] from [PyPI]:
 
 ```bash
 pip install seb
 ```
 
 [pip]: https://pip.pypa.io/en/stable/installing/
-[PyPI]: https://pypi.org/project/cuecy/
+[PyPI]: https://pypi.org/project/seb/
 
 
 To see more examples, see the [documentation].
 
 # 📖 Documentation
 
 | Documentation         |                                                          |
```

#### html2text {}

```diff
@@ -1,34 +1,33 @@
 [https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/blob/
 main/docs/_static/logo.png?raw=true] # Scandinavian Embedding Benchmark [!
-[PyPI](https://img.shields.io/pypi/v/scandinavian-embedding-benchmark.svg)]
-[pypi status] [![Python Version](https://img.shields.io/pypi/pyversions/
-scandinavian-embedding-benchmark)][pypi status] [![documentation](https://
-github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/actions/
+[PyPI](https://img.shields.io/pypi/v/seb.svg)][pypi status] [![Python Version]
+(https://img.shields.io/pypi/pyversions/seb)][pypi status] [![documentation]
+(https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/actions/
 workflows/documentation.yml/badge.svg)][documentation] [![Tests](https://
 github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/actions/
 workflows/tests.yml/badge.svg)][tests] [![Black](https://img.shields.io/badge/
 code%20style-black-000000.svg)][black] [pypi status]: https://pypi.org/project/
-scandinavian-embedding-benchmark/ [documentation]: https://
-KennethEnevoldsen.github.io/scandinavian-embedding-benchmark/ [tests]: https://
-github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/
-actions?workflow=Tests [black]: https://github.com/psf/black  A benchmark for
-evaluating sentence/document embeddings of Scandinavian language models.  ##
-Installation You can install `scandinavian-embedding-benchmark` via [pip] from
-[PyPI]: ```bash pip install seb ``` [pip]: https://pip.pypa.io/en/stable/
-installing/ [PyPI]: https://pypi.org/project/cuecy/ To see more examples, see
-the [documentation]. # ð Documentation | Documentation | | | ---------------
------- | -------------------------------------------------------- | | ð§ **
-[Installation]** | Installation instructions on how to install this package | |
-ð©âð» **[Usage]** | Introduction on how to use the package | | ð **
-[Documentation]** | A minimal and developing documentation | # ð¬ Where to
-ask questions | Type | | | ------------------------------ | -------------------
---- | | ð¨ **Bug Reports** | [GitHub Issue Tracker] | | ð **Feature
-Requests & Ideas** | [GitHub Issue Tracker] | | ð©âð» **Usage Questions**
-| [GitHub Discussions] | | ð¯ **General Discussion** | [GitHub Discussions] |
-[Usage]: https://kennethenevoldsen.github.io/scandinavian-embedding-benchmark/
+seb/ [documentation]: https://KennethEnevoldsen.github.io/scandinavian-
+embedding-benchmark/ [tests]: https://github.com/KennethEnevoldsen/
+scandinavian-embedding-benchmark/actions?workflow=Tests [black]: https://
+github.com/psf/black  A benchmark for evaluating sentence/document embeddings
+of Scandinavian language models.  ## Installation You can install the
+Scandinavian Embedding Benchmark (`seb`) via [pip] from [PyPI]: ```bash pip
+install seb ``` [pip]: https://pip.pypa.io/en/stable/installing/ [PyPI]: https:
+//pypi.org/project/seb/ To see more examples, see the [documentation]. # ð
+Documentation | Documentation | | | --------------------- | -------------------
+------------------------------------- | | ð§ **[Installation]** |
+Installation instructions on how to install this package | | ð©âð» **
+[Usage]** | Introduction on how to use the package | | ð **[Documentation]**
+| A minimal and developing documentation | # ð¬ Where to ask questions | Type
+| | | ------------------------------ | ---------------------- | | ð¨ **Bug
+Reports** | [GitHub Issue Tracker] | | ð **Feature Requests & Ideas** |
+[GitHub Issue Tracker] | | ð©âð» **Usage Questions** | [GitHub
+Discussions] | | ð¯ **General Discussion** | [GitHub Discussions] | [Usage]:
+https://kennethenevoldsen.github.io/scandinavian-embedding-benchmark/
 getting_started/ [Documentation]: https://KennethEnevoldsen.github.io/
 scandinavian-embedding-benchmark/index.html [Installation]: https://
 KennethEnevoldsen.github.io/scandinavian-embedding-benchmark/installation.html
 [github issue tracker]: https://github.com/KennethEnevoldsen/scandinavian-
 embedding-benchmark/issues [github discussions]: https://github.com/
 KennethEnevoldsen/scandinavian-embedding-benchmark/discussions
```

### Comparing `seb-0.0.0/docs/_static/logo.png` & `seb-0.1.5/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/docs/_static/social.png` & `seb-0.1.5/docs/_static/social.png`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/docs/getting_started.ipynb` & `seb-0.1.5/docs/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/docs/index.md` & `seb-0.1.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/docs/run_benchmark.py` & `seb-0.1.5/docs/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/mkdocs.yml` & `seb-0.1.5/mkdocs.yml`

 * *Files 23% similar despite different names*

```diff
@@ -44,17 +44,13 @@
           type: python
           root_package: seb
           docstring_style: google
           options:
             heading_level: 3
             show_source: true
             show_root_heading: true
-
-  # - social:
-  #     cards_layout: default/only/image
-  #     cards_layout_options:
-  #       background_image: _static/social.png
+  - social
 
 extra:
   social:
     - icon: fontawesome/brands/github
       link: https://github.com/KennethEnevoldsen/Scandinavian-Embedding-Benchmark
```

### Comparing `seb-0.0.0/pyproject.toml` & `seb-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "seb"
-version = "0.0.0"
+version = "0.1.5"
 authors = [
   { name = "Kenneth Enevoldsen", email = "Kennethcenevoldsen@gmail.com" },
 ]
 description = "Scandinavian Embedding Benchmark"
 classifiers = [
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS :: MacOS X",
@@ -144,17 +144,15 @@
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
 [tool.semantic_release]
 branch = "main"
-version_variable = ["pyproject.toml:version"]
-upload_to_pypi = true
-upload_to_release = true
+version_toml = ["pyproject.toml:project.version"]
 build_command = "python -m pip install build; python -m build"
 
 [tool.setuptools]
 include-package-data = true
 
 
 [tool.tox]
```

### Comparing `seb-0.0.0/src/seb/benchmark.py` & `seb-0.1.5/src/seb/benchmark.py`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/src/seb/full_benchmark.py` & `seb-0.1.5/src/seb/full_benchmark.py`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/src/seb/model_interface.py` & `seb-0.1.5/src/seb/model_interface.py`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/src/seb/registries.py` & `seb-0.1.5/src/seb/registries.py`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/src/seb/result_dataclasses.py` & `seb-0.1.5/src/seb/result_dataclasses.py`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/src/seb/seb_models.py` & `seb-0.1.5/src/seb/seb_models.py`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/src/seb/seb_tasks/danish.py` & `seb-0.1.5/src/seb/seb_tasks/danish.py`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/src/seb/seb_tasks/multilingual.py` & `seb-0.1.5/src/seb/seb_tasks/multilingual.py`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/src/seb/seb_tasks/norwegian.py` & `seb-0.1.5/src/seb/seb_tasks/norwegian.py`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/src/seb/tasks_interface.py` & `seb-0.1.5/src/seb/tasks_interface.py`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/src/seb/utils.py` & `seb-0.1.5/src/seb/utils.py`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/src/seb.egg-info/PKG-INFO` & `seb-0.1.5/src/seb.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seb
-Version: 0.0.0
+Version: 0.1.5
 Summary: Scandinavian Embedding Benchmark
 Author-email: Kenneth Enevoldsen <Kennethcenevoldsen@gmail.com>
 License: MIT License
         
         Copyright © 2023 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,42 +40,42 @@
 Provides-Extra: docs
 License-File: LICENSE
 
 <a href="https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark"><img src="https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/blob/main/docs/_static/logo.png?raw=true" width="120" align="right"/></a>
 
 # Scandinavian Embedding Benchmark
 
-[![PyPI](https://img.shields.io/pypi/v/scandinavian-embedding-benchmark.svg)][pypi status]
-[![Python Version](https://img.shields.io/pypi/pyversions/scandinavian-embedding-benchmark)][pypi status]
+[![PyPI](https://img.shields.io/pypi/v/seb.svg)][pypi status]
+[![Python Version](https://img.shields.io/pypi/pyversions/seb)][pypi status]
 [![documentation](https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/actions/workflows/documentation.yml/badge.svg)][documentation]
 [![Tests](https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/actions/workflows/tests.yml/badge.svg)][tests]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 
-[pypi status]: https://pypi.org/project/scandinavian-embedding-benchmark/
+[pypi status]: https://pypi.org/project/seb/
 [documentation]: https://KennethEnevoldsen.github.io/scandinavian-embedding-benchmark/
 [tests]: https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/actions?workflow=Tests
 [black]: https://github.com/psf/black
 
 
 <!-- start short-description -->
 
 A benchmark for evaluating sentence/document embeddings of Scandinavian language models.
 
 <!-- end short-description -->
 
 ## Installation
 
-You can install `scandinavian-embedding-benchmark` via [pip] from [PyPI]:
+You can install the Scandinavian Embedding Benchmark (`seb`) via [pip] from [PyPI]:
 
 ```bash
 pip install seb
 ```
 
 [pip]: https://pip.pypa.io/en/stable/installing/
-[PyPI]: https://pypi.org/project/cuecy/
+[PyPI]: https://pypi.org/project/seb/
 
 
 To see more examples, see the [documentation].
 
 # 📖 Documentation
 
 | Documentation         |                                                          |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seb Version: 0.0.0 Summary: Scandinavian Embedding
+Metadata-Version: 2.1 Name: seb Version: 0.1.5 Summary: Scandinavian Embedding
 Benchmark Author-email: Kenneth Enevoldsen
 gmail.com> License: MIT License Copyright Â© 2023 Kenneth Enevoldsen Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -21,34 +21,33 @@
 benchmark/ Classifier: Operating System :: POSIX :: Linux Classifier: Operating
 System :: MacOS :: MacOS X Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.9 Description-Content-Type:
 text/markdown Provides-Extra: dev Provides-Extra: tests Provides-Extra: docs
 License-File: LICENSE [https://github.com/KennethEnevoldsen/scandinavian-
 embedding-benchmark/blob/main/docs/_static/logo.png?raw=true] # Scandinavian
-Embedding Benchmark [![PyPI](https://img.shields.io/pypi/v/scandinavian-
-embedding-benchmark.svg)][pypi status] [![Python Version](https://
-img.shields.io/pypi/pyversions/scandinavian-embedding-benchmark)][pypi status]
-[![documentation](https://github.com/KennethEnevoldsen/scandinavian-embedding-
-benchmark/actions/workflows/documentation.yml/badge.svg)][documentation] [!
-[Tests](https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/
-actions/workflows/tests.yml/badge.svg)][tests] [![Black](https://
-img.shields.io/badge/code%20style-black-000000.svg)][black] [pypi status]:
-https://pypi.org/project/scandinavian-embedding-benchmark/ [documentation]:
-https://KennethEnevoldsen.github.io/scandinavian-embedding-benchmark/ [tests]:
-https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/
+Embedding Benchmark [![PyPI](https://img.shields.io/pypi/v/seb.svg)][pypi
+status] [![Python Version](https://img.shields.io/pypi/pyversions/seb)][pypi
+status] [![documentation](https://github.com/KennethEnevoldsen/scandinavian-
+embedding-benchmark/actions/workflows/documentation.yml/badge.svg)]
+[documentation] [![Tests](https://github.com/KennethEnevoldsen/scandinavian-
+embedding-benchmark/actions/workflows/tests.yml/badge.svg)][tests] [![Black]
+(https://img.shields.io/badge/code%20style-black-000000.svg)][black] [pypi
+status]: https://pypi.org/project/seb/ [documentation]: https://
+KennethEnevoldsen.github.io/scandinavian-embedding-benchmark/ [tests]: https://
+github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/
 actions?workflow=Tests [black]: https://github.com/psf/black  A benchmark for
 evaluating sentence/document embeddings of Scandinavian language models.  ##
-Installation You can install `scandinavian-embedding-benchmark` via [pip] from
-[PyPI]: ```bash pip install seb ``` [pip]: https://pip.pypa.io/en/stable/
-installing/ [PyPI]: https://pypi.org/project/cuecy/ To see more examples, see
-the [documentation]. # ð Documentation | Documentation | | | ---------------
------- | -------------------------------------------------------- | | ð§ **
-[Installation]** | Installation instructions on how to install this package | |
-ð©âð» **[Usage]** | Introduction on how to use the package | | ð **
+Installation You can install the Scandinavian Embedding Benchmark (`seb`) via
+[pip] from [PyPI]: ```bash pip install seb ``` [pip]: https://pip.pypa.io/en/
+stable/installing/ [PyPI]: https://pypi.org/project/seb/ To see more examples,
+see the [documentation]. # ð Documentation | Documentation | | | -----------
+---------- | -------------------------------------------------------- | | ð§
+**[Installation]** | Installation instructions on how to install this package |
+| ð©âð» **[Usage]** | Introduction on how to use the package | | ð **
 [Documentation]** | A minimal and developing documentation | # ð¬ Where to
 ask questions | Type | | | ------------------------------ | -------------------
 --- | | ð¨ **Bug Reports** | [GitHub Issue Tracker] | | ð **Feature
 Requests & Ideas** | [GitHub Issue Tracker] | | ð©âð» **Usage Questions**
 | [GitHub Discussions] | | ð¯ **General Discussion** | [GitHub Discussions] |
 [Usage]: https://kennethenevoldsen.github.io/scandinavian-embedding-benchmark/
 getting_started/ [Documentation]: https://KennethEnevoldsen.github.io/
```

### Comparing `seb-0.0.0/src/seb.egg-info/SOURCES.txt` & `seb-0.1.5/src/seb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/tasks.py` & `seb-0.1.5/tasks.py`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/tests/dummy_model.py` & `seb-0.1.5/tests/dummy_model.py`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/tests/dummy_task.py` & `seb-0.1.5/tests/dummy_task.py`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/tests/test_all_models.py` & `seb-0.1.5/tests/test_all_models.py`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/tests/test_benchmark.py` & `seb-0.1.5/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `seb-0.0.0/tests/test_tasks.py` & `seb-0.1.5/tests/test_tasks.py`

 * *Files identical despite different names*

