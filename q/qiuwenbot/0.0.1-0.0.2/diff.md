# Comparing `tmp/qiuwenbot-0.0.1.tar.gz` & `tmp/qiuwenbot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiuwenbot-0.0.1.tar", last modified: Sun Jul 30 17:38:15 2023, max compression
+gzip compressed data, was "qiuwenbot-0.0.2.tar", last modified: Mon Jul 31 22:50:57 2023, max compression
```

## Comparing `qiuwenbot-0.0.1.tar` & `qiuwenbot-0.0.2.tar`

### file list

```diff
@@ -1,64 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:38:15.770710 qiuwenbot-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:38:15.762710 qiuwenbot-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:38:15.762710 qiuwenbot-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/.github/workflows/mirror.yml
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42628 2023-07-30 17:38:15.770710 qiuwenbot-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:38:15.766710 qiuwenbot-0.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/examples/check_duplicate.json
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/examples/filter_all.json
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/examples/filter_new.json
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:38:15.766710 qiuwenbot-0.0.1/qiuwenbot/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:38:15.766710 qiuwenbot-0.0.1/qiuwenbot/entrypoints/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/entrypoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/entrypoints/submit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:38:15.766710 qiuwenbot-0.0.1/qiuwenbot/filter/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/filter/clean_refs.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/filter/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/filter/deprecated_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/filter/expired_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/filter/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/filter/gov.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/filter/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/filter/hk.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/filter/ref_blacklist.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/filter/roc_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/filter/roc_year.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/filter/tw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/filter/wg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/qwfamily.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/qwlogger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:38:15.770710 qiuwenbot-0.0.1/qiuwenbot/task/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/task/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/task/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/user-config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/qiuwenbot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:38:15.766710 qiuwenbot-0.0.1/qiuwenbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42628 2023-07-30 17:38:15.000000 qiuwenbot-0.0.1/qiuwenbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-30 17:38:15.000000 qiuwenbot-0.0.1/qiuwenbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 17:38:15.000000 qiuwenbot-0.0.1/qiuwenbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-30 17:38:15.000000 qiuwenbot-0.0.1/qiuwenbot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-30 17:38:15.000000 qiuwenbot-0.0.1/qiuwenbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-30 17:38:15.000000 qiuwenbot-0.0.1/qiuwenbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 17:38:15.770710 qiuwenbot-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:38:15.770710 qiuwenbot-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-30 17:38:05.000000 qiuwenbot-0.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:50:57.329849 qiuwenbot-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:50:57.317849 qiuwenbot-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:50:57.321849 qiuwenbot-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/.github/workflows/mirror.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42649 2023-07-31 22:50:57.329849 qiuwenbot-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:50:57.321849 qiuwenbot-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/docs/args.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:50:57.321849 qiuwenbot-0.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/examples/check_duplicate.json
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/examples/filter_all.json
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/examples/filter_new.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:50:57.325849 qiuwenbot-0.0.2/qiuwenbot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:50:57.325849 qiuwenbot-0.0.2/qiuwenbot/entrypoints/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/entrypoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/entrypoints/submit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:50:57.329849 qiuwenbot-0.0.2/qiuwenbot/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/filter/clean_refs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/filter/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/filter/deprecated_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/filter/expired_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/filter/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/filter/gov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/filter/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/filter/hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/filter/ref_blacklist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/filter/roc_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/filter/roc_year.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/filter/tw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/filter/wg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/qwfamily.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/qwlogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:50:57.329849 qiuwenbot-0.0.2/qiuwenbot/task/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/task/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/task/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/user-config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/qiuwenbot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:50:57.325849 qiuwenbot-0.0.2/qiuwenbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42649 2023-07-31 22:50:57.000000 qiuwenbot-0.0.2/qiuwenbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-31 22:50:57.000000 qiuwenbot-0.0.2/qiuwenbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 22:50:57.000000 qiuwenbot-0.0.2/qiuwenbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-31 22:50:57.000000 qiuwenbot-0.0.2/qiuwenbot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-31 22:50:57.000000 qiuwenbot-0.0.2/qiuwenbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 22:50:57.000000 qiuwenbot-0.0.2/qiuwenbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 22:50:57.329849 qiuwenbot-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:50:57.329849 qiuwenbot-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-31 22:50:45.000000 qiuwenbot-0.0.2/tox.ini
```

### Comparing `qiuwenbot-0.0.1/.github/workflows/release.yml` & `qiuwenbot-0.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/.github/workflows/test.yml` & `qiuwenbot-0.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/.gitignore` & `qiuwenbot-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/.pre-commit-config.yaml` & `qiuwenbot-0.0.2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     -   id: check-added-large-files
     -   id: check-merge-conflict
     -   id: check-symlinks
     -   id: check-toml
 # Python
 -   repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
-    rev: v0.0.280
+    rev: v0.0.281
     hooks:
     - id: ruff
       args: ["--fix"]
 -   repo: https://github.com/psf/black
     rev: 23.7.0
     hooks:
     -   id: black-jupyter
```

### Comparing `qiuwenbot-0.0.1/LICENSE` & `qiuwenbot-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/PKG-INFO` & `qiuwenbot-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiuwenbot
-Version: 0.0.1
+Version: 0.0.2
 Summary: Qiuwen Baike bot/求闻百科机器人
 Author-email: Jinzhe Zeng <jinzhe.zeng@rutgers.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,14 +682,15 @@
 Keywords: qiuwen,bot
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: docs
 License-File: LICENSE
 
 # Qiuwen Baike bot / 求闻百科机器人
 
 [Qiuwen Baike](https://www.qiuwenbaike.cn) bot. / [求闻百科](https://www.qiuwenbaike.cn)机器人。
 
 ## Features / 功能
```

### Comparing `qiuwenbot-0.0.1/README.md` & `qiuwenbot-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/pyproject.toml` & `qiuwenbot-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,22 @@
 keywords = ["qiuwen", "bot"]
 
 [project.optional-dependencies]
 test = [
     'pytest',
     'pytest-cov',
 ]
+docs = [
+    "sphinx",
+    "myst-parser",
+    "furo",
+    "numpydoc",
+    "dargs>=0.3.1",
+    "sphinx-argparse",
+]
 
 [project.urls]
 repository = "https://github.com/njzjz/qiuwenbot"
 
 [project.scripts]
 qiuwenbot = "qiuwenbot.__main__:main"
```

### Comparing `qiuwenbot-0.0.1/qiuwenbot/__init__.py` & `qiuwenbot-0.0.2/qiuwenbot/__init__.py`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/qiuwenbot/__main__.py` & `qiuwenbot-0.0.2/qiuwenbot/__main__.py`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/qiuwenbot/argparse.py` & `qiuwenbot-0.0.2/qiuwenbot/argparse.py`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/qiuwenbot/bot.py` & `qiuwenbot-0.0.2/qiuwenbot/bot.py`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/qiuwenbot/entrypoints/submit.py` & `qiuwenbot-0.0.2/qiuwenbot/entrypoints/submit.py`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/qiuwenbot/filter/__init__.py` & `qiuwenbot-0.0.2/qiuwenbot/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/qiuwenbot/filter/clean_refs.py` & `qiuwenbot-0.0.2/qiuwenbot/filter/clean_refs.py`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/qiuwenbot/filter/common.py` & `qiuwenbot-0.0.2/qiuwenbot/filter/common.py`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/qiuwenbot/filter/deprecated_tags.py` & `qiuwenbot-0.0.2/qiuwenbot/filter/deprecated_tags.py`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/qiuwenbot/filter/expired_templates.py` & `qiuwenbot-0.0.2/qiuwenbot/filter/expired_templates.py`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/qiuwenbot/filter/filter.py` & `qiuwenbot-0.0.2/qiuwenbot/filter/filter.py`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/qiuwenbot/filter/gov.py` & `qiuwenbot-0.0.2/qiuwenbot/filter/gov.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 
 @register_filter
 class CNGovFilter(TextReplaceFilter):
     """Filter to fix the Chinese government terms."""
 
     def __init__(self):
         super().__init__(
-            r"""(中国|中國|北京|中共)(当局|當局|政府)""",
+            r"""(中国|中國|中共)(当局|當局|政府)""",
             r"中国政府",
         )
 
     @property
     def log(self) -> str:
         return "修正涉政用语1"
```

### Comparing `qiuwenbot-0.0.1/qiuwenbot/filter/history.py` & `qiuwenbot-0.0.2/qiuwenbot/filter/history.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,14 @@
 
 @register_filter
 class FakeManchukuoFilter(TextReplaceFilter):
     """Filter for Fake Manchukuo authorities."""
 
     def __init__(self):
         super().__init__(
-            r"([^伪僞偽])(滿|满)洲(国|國)",
+            r"([^伪僞偽“‘「『])(滿|满)洲(国|國)",
             r"\1伪满洲国",
         )
 
     @property
     def log(self) -> str:
         return "修正伪满洲国名称"
```

### Comparing `qiuwenbot-0.0.1/qiuwenbot/filter/hk.py` & `qiuwenbot-0.0.2/qiuwenbot/filter/hk.py`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/qiuwenbot/filter/ref_blacklist.txt` & `qiuwenbot-0.0.2/qiuwenbot/filter/ref_blacklist.txt`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/qiuwenbot/filter/roc_flag.py` & `qiuwenbot-0.0.2/qiuwenbot/filter/roc_flag.py`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/qiuwenbot/filter/roc_year.py` & `qiuwenbot-0.0.2/qiuwenbot/filter/roc_year.py`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/qiuwenbot/filter/tw.py` & `qiuwenbot-0.0.2/qiuwenbot/filter/tw.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,32 +73,32 @@
 
 @register_filter
 class TWUnivFilter1(TextReplaceFilter):
     """Filter to fix the name of unversities in the Taiwan area."""
 
     def __init__(self):
         super().__init__(
-            r"(國立|国立)((臺|台)(灣|湾)((师范|師範|海洋|藝術|艺术|体育(运动)?|科技)?大(學|学)|戲曲學院|戏曲学院)|金门大学|金門大學)",
-            r"\2",
+            r"([^“‘「『])(國立|国立)((臺|台)(灣|湾)((师范|師範|海洋|藝術|艺术|体育(运动)?|科技)?大(學|学)|戲曲學院|戏曲学院)|金门大学|金門大學)",
+            r"\1\3",
         )
 
     @property
     def log(self) -> str:
         return "修正涉台用语3"
 
 
 @register_filter
 class TWUnivFilter2(TextReplaceFilter):
     """Filter to fix the name of unversities in the Taiwan area."""
 
     def __init__(self):
         # only fix univ created after 1949
         super().__init__(
-            r"(國立|国立)((高雄师范|高雄師範|彰化師範|彰化师范|台北艺术|臺北藝術|臺南|台南|體育|体育|阳明|陽明|阳明交通|陽明交通)大(学|學)|傳統藝術中心|传统艺术中心)",
-            r"台湾\2",
+            r"([^“‘「『])(國立|国立)((高雄师范|高雄師範|彰化師範|彰化师范|台北艺术|臺北藝術|臺南|台南|體育|体育|阳明|陽明|阳明交通|陽明交通)大(学|學)|傳統藝術中心|传统艺术中心)",
+            r"\1台湾\3",
         )
 
     @property
     def log(self) -> str:
         return "修正涉台用语4"
 
 
@@ -156,15 +156,15 @@
     """Filter to fix the Taiwan name when it is with other countries."""
 
     def __init__(self):
         countries_hant = [convert_for_mw(xx, "zh-hant") for xx in coutries]
         coutries_re = "|".join(coutries + countries_hant)
 
         super().__init__(
-            r"([^国國])(台湾|台灣|臺湾|\[\[台湾\]\]|\[\[台灣\]\]|\[\[臺湾\]\])((和|与|、|,|，|或|或者|及|以及)(\[\[)?(%s))"
+            r"([^国國])(台湾|台灣|臺湾|\[\[台湾\]\]|\[\[台灣\]\]|\[\[臺湾\]\])((和|与|、|,|或|或者|及|以及)(\[\[)?(%s))"
             % coutries_re,
             r"\1中国台湾\3",
         )
 
     @property
     def log(self) -> str:
         return "修正中国台湾与国家并列时的称呼2"
```

### Comparing `qiuwenbot-0.0.1/qiuwenbot/filter/wg.py` & `qiuwenbot-0.0.2/qiuwenbot/filter/wg.py`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/qiuwenbot/qwfamily.py` & `qiuwenbot-0.0.2/qiuwenbot/qwfamily.py`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/qiuwenbot/qwlogger.py` & `qiuwenbot-0.0.2/qiuwenbot/qwlogger.py`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/qiuwenbot/task/duplicate.py` & `qiuwenbot-0.0.2/qiuwenbot/task/duplicate.py`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/qiuwenbot/task/filter.py` & `qiuwenbot-0.0.2/qiuwenbot/task/filter.py`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/qiuwenbot/task/task.py` & `qiuwenbot-0.0.2/qiuwenbot/task/task.py`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/qiuwenbot/utils.py` & `qiuwenbot-0.0.2/qiuwenbot/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     while True:
         title = oldtitle + "/存档%d" % ii
         if title:
             archieve_page = get_page(title, site)
             if not archieve_page.exists():
                 page.text = page.text.replace("{{Archives}}", "")
                 page.save("删除archieves模板")
-                page.move(title, "存档")
+                page.move(title, "存档", movetalk=False, movesubpages=False)
                 oldpage = get_page(oldtitle, site)
                 oldpage.text = "{{Archives}}"
                 oldpage.save("加入archieves模板")
                 return oldpage
         ii += 1
```

### Comparing `qiuwenbot-0.0.1/qiuwenbot.egg-info/PKG-INFO` & `qiuwenbot-0.0.2/qiuwenbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiuwenbot
-Version: 0.0.1
+Version: 0.0.2
 Summary: Qiuwen Baike bot/求闻百科机器人
 Author-email: Jinzhe Zeng <jinzhe.zeng@rutgers.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,14 +682,15 @@
 Keywords: qiuwen,bot
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: docs
 License-File: LICENSE
 
 # Qiuwen Baike bot / 求闻百科机器人
 
 [Qiuwen Baike](https://www.qiuwenbaike.cn) bot. / [求闻百科](https://www.qiuwenbaike.cn)机器人。
 
 ## Features / 功能
```

### Comparing `qiuwenbot-0.0.1/qiuwenbot.egg-info/SOURCES.txt` & `qiuwenbot-0.0.2/qiuwenbot.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 .gitignore
 .pre-commit-config.yaml
+.readthedocs.yaml
 LICENSE
 README.md
 codecov.yml
 pyproject.toml
 tox.ini
 .github/workflows/mirror.yml
 .github/workflows/release.yml
 .github/workflows/test.yml
+docs/args.rst
+docs/cli.rst
+docs/conf.py
+docs/index.rst
+docs/install.rst
+docs/requirements.txt
+docs/usage.rst
 examples/check_duplicate.json
 examples/filter_all.json
 examples/filter_new.json
 qiuwenbot/__init__.py
 qiuwenbot/__main__.py
 qiuwenbot/argparse.py
 qiuwenbot/bot.py
```

### Comparing `qiuwenbot-0.0.1/tests/test_filter.py` & `qiuwenbot-0.0.2/tests/test_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         r"""\
         民国101年，日治時期“[[文化大革命]]”（[[文化大革命|文革]]）[[四人帮]]倒台后，
         [[蔡英文]][[中华民国总统|总统]]死了<ref>{{cite web|url=https://bbc.com/zhongwen/cywsl}}</ref>。
         <timeline>123</timeline>
         <score>456</score>
         <mapframe>789</mapframe>
         [[香港主權移交]]了！
-        北京当局
+        中国当局
         中华民国（台湾）
         中华民国台北市
         """
     )
     expected_text = dedent(
         r"""\
         2012年，日占時期“[[文化大革命]]”（“[[文化大革命|文革]]”）“[[四人帮]]”倒台后，
@@ -120,40 +120,44 @@
 
 
 def test_tw_univ():
     text = dedent(
         r"""\
         国立台湾大学
         国立阳明大学
+        “国立体育大学”
         """
     )
     expected_text = dedent(
         r"""\
         台湾大学
         台湾阳明大学
+        “国立体育大学”
         """
     )
     filter = FilterChain(default_filters)
 
     text = filter.filter(text)
     assert text == expected_text
 
 
 def test_historical_authority():
     text = dedent(
         r"""\
         满洲国
+        “满洲国”
         伪满洲国
         汪精卫政权
         清治时期
         """
     )
     expected_text = dedent(
         r"""\
         伪满洲国
+        “满洲国”
         伪满洲国
         汪伪政权
         清朝时期
         """
     )
     filter = FilterChain(default_filters)
```

### Comparing `qiuwenbot-0.0.1/tests/test_task.py` & `qiuwenbot-0.0.2/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `qiuwenbot-0.0.1/tests/test_utils.py` & `qiuwenbot-0.0.2/tests/test_utils.py`

 * *Files identical despite different names*

