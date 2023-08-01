# Comparing `tmp/b_cfn_custom_userpool_authorizer-1.0.0.tar.gz` & `tmp/b_cfn_custom_userpool_authorizer-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b_cfn_custom_userpool_authorizer-1.0.0.tar", last modified: Fri Aug 26 10:33:28 2022, max compression
+gzip compressed data, was "b_cfn_custom_userpool_authorizer-2.0.0.tar", last modified: Tue Aug  1 11:35:00 2023, max compression
```

## Comparing `b_cfn_custom_userpool_authorizer-1.0.0.tar` & `b_cfn_custom_userpool_authorizer-2.0.0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:33:28.212933 b_cfn_custom_userpool_authorizer-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6916 2022-08-26 10:33:28.212933 b_cfn_custom_userpool_authorizer-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4025 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:33:28.208933 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:33:28.212933 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/config/user_pool_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      763 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/config/user_pool_ssm_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:33:28.212933 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/source/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/source/auth_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)      860 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/source/index.py
--rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/source/policy_document.py
--rw-r--r--   0 runner    (1001) docker     (121)     3514 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/source/token_verification.py
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/source/user_pool_resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)     3032 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/user_pool_custom_authorizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2218 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/user_pool_custom_authorizer_function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:33:28.212933 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6916 2022-08-26 10:33:28.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2258 2022-08-26 10:33:28.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 10:33:28.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-08-26 10:33:28.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-26 10:33:28.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:33:28.208933 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:33:28.212933 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:33:28.212933 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2092 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/fixtures/access_token.py
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/infra_create.py
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/infra_destroy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:33:28.212933 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2073 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/infrastructure/authorized_endpoint_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/infrastructure/main_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     2067 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/infrastructure/user_pool_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:33:28.212933 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      872 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/tests/test_authorizer_allow.py
--rw-r--r--   0 runner    (1001) docker     (121)     2828 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/tests/test_authorizer_deny.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:33:28.212933 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/util/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/util/urlsafe_json.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 10:33:28.212933 b_cfn_custom_userpool_authorizer-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1713 2022-08-26 10:27:36.000000 b_cfn_custom_userpool_authorizer-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:35:00.202961 b_cfn_custom_userpool_authorizer-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-08-01 11:35:00.202961 b_cfn_custom_userpool_authorizer-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:35:00.198960 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:35:00.198960 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/config/user_pool_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/config/user_pool_ssm_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:35:00.198960 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/source/auth_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/source/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/source/policy_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/source/token_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/source/user_pool_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/user_pool_custom_authorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/user_pool_custom_authorizer_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:35:00.198960 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-08-01 11:35:00.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-08-01 11:35:00.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:35:00.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-01 11:35:00.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-01 11:35:00.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:35:00.194960 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:35:00.198960 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:35:00.198960 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/fixtures/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/infra_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/infra_destroy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:35:00.198960 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/infrastructure/api_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/infrastructure/authorized_endpoint_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/infrastructure/main_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/infrastructure/user_pool_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:35:00.202961 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/tests/test_authorizer_allow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/tests/test_authorizer_deny.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:35:00.202961 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/util/urlsafe_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:35:00.202961 b_cfn_custom_userpool_authorizer-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-01 11:28:02.000000 b_cfn_custom_userpool_authorizer-2.0.0/setup.py
```

### Comparing `b_cfn_custom_userpool_authorizer-1.0.0/HISTORY.md` & `b_cfn_custom_userpool_authorizer-2.0.0/HISTORY.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Release history
 
+### 2.0.0
+* Upgrade CDK support from v1 to v2.
+* Upgrade GitHub pipelines checkout version from v2 to v3.
+* Upgrade biomapas/cicd-full image version to 5.0.0.
+
 ### 1.0.0
 * Upgrade dependencies to breaking versions.
 
 ### 0.1.2
 * Make dependency range more strict.
 
 ### 0.1.1
```

### Comparing `b_cfn_custom_userpool_authorizer-1.0.0/LICENSE` & `b_cfn_custom_userpool_authorizer-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_userpool_authorizer-1.0.0/README.md` & `b_cfn_custom_userpool_authorizer-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 pip install b-cfn-custom-userpool-authorizer
 ```
 
 
 ### Usage & Examples
 
 ```python
-from aws_cdk.core import Stack
+from aws_cdk import Stack
 from aws_cdk.aws_cognito import UserPool, UserPoolClient
 from aws_cdk.aws_apigatewayv2 import CfnApi
 
 from b_cfn_custom_userpool_authorizer.config.user_pool_config import UserPoolConfig
 from b_cfn_custom_userpool_authorizer.user_pool_custom_authorizer import UserPoolCustomAuthorizer
 
 # Create user pool and client.
@@ -112,9 +112,9 @@
 pytest b_cfn_custom_userpool_authorizer_test/integration/tests
 ```
 
 ### Contribution
 
 Found a bug? Want to add or suggest a new feature? 
 Contributions of any kind are gladly welcome. 
-You may contact us directly, create a pull-request or an issue in github platform. 
+You may contact us directly, create a pull-request or an issue in GitHub platform. 
 Lets modernize the world together.
```

### Comparing `b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/config/user_pool_config.py` & `b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/config/user_pool_config.py`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/config/user_pool_ssm_config.py` & `b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/config/user_pool_ssm_config.py`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/source/index.py` & `b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/source/index.py`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/source/policy_document.py` & `b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/source/policy_document.py`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/source/token_verification.py` & `b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/source/token_verification.py`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/source/user_pool_resolver.py` & `b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/source/user_pool_resolver.py`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/user_pool_custom_authorizer.py` & `b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/user_pool_custom_authorizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Union
 
+from aws_cdk import Stack
 from aws_cdk.aws_apigatewayv2 import CfnAuthorizer, CfnApi
-from aws_cdk.core import Stack
 
 from b_cfn_custom_userpool_authorizer.config.user_pool_config import UserPoolConfig
 from b_cfn_custom_userpool_authorizer.config.user_pool_ssm_config import UserPoolSsmConfig
 from b_cfn_custom_userpool_authorizer.user_pool_custom_authorizer_function import AuthorizerFunction
 
 
 class UserPoolCustomAuthorizer(CfnAuthorizer):
```

### Comparing `b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer/user_pool_custom_authorizer_function.py` & `b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer/user_pool_custom_authorizer_function.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Union
 
+from aws_cdk import Duration, Stack
 from aws_cdk.aws_iam import PolicyStatement
 from aws_cdk.aws_lambda import Function, Code, Runtime, CfnPermission
 from aws_cdk.aws_logs import RetentionDays
-from aws_cdk.core import Duration, Stack
-from b_cfn_lambda_layer.package_version import PackageVersion
 from b_cfn_lambda_layer.lambda_layer import LambdaLayer
+from b_cfn_lambda_layer.package_version import PackageVersion
 
 from b_cfn_custom_userpool_authorizer.config.user_pool_config import UserPoolConfig
 from b_cfn_custom_userpool_authorizer.config.user_pool_ssm_config import UserPoolSsmConfig
 
 
 class AuthorizerFunction(Function):
     def __init__(
```

### Comparing `b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer.egg-info/SOURCES.txt` & `b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 b_cfn_custom_userpool_authorizer_test/integration/conftest.py
 b_cfn_custom_userpool_authorizer_test/integration/infra_create.py
 b_cfn_custom_userpool_authorizer_test/integration/infra_destroy.py
 b_cfn_custom_userpool_authorizer_test/integration/manager.py
 b_cfn_custom_userpool_authorizer_test/integration/fixtures/__init__.py
 b_cfn_custom_userpool_authorizer_test/integration/fixtures/access_token.py
 b_cfn_custom_userpool_authorizer_test/integration/infrastructure/__init__.py
+b_cfn_custom_userpool_authorizer_test/integration/infrastructure/api_stack.py
 b_cfn_custom_userpool_authorizer_test/integration/infrastructure/authorized_endpoint_stack.py
 b_cfn_custom_userpool_authorizer_test/integration/infrastructure/main_stack.py
 b_cfn_custom_userpool_authorizer_test/integration/infrastructure/user_pool_stack.py
 b_cfn_custom_userpool_authorizer_test/integration/tests/__init__.py
 b_cfn_custom_userpool_authorizer_test/integration/tests/test_authorizer_allow.py
 b_cfn_custom_userpool_authorizer_test/integration/tests/test_authorizer_deny.py
 b_cfn_custom_userpool_authorizer_test/integration/util/__init__.py
```

### Comparing `b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/fixtures/access_token.py` & `b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/fixtures/access_token.py`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/infrastructure/authorized_endpoint_stack.py` & `b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/infrastructure/authorized_endpoint_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from aws_cdk import Stack, Duration
 from aws_cdk.aws_apigatewayv2 import CfnRoute, CfnAuthorizer, CfnApi
 from aws_cdk.aws_lambda import Function, Code, Runtime, CfnPermission
-from aws_cdk.core import Stack, Duration
 from b_aws_testing_framework.tools.cdk_testing.testing_stack import TestingStack
 from b_cfn_lambda_integration.lambda_integration import LambdaIntegration
 
 
 class AuthorizedEndpointStack(Stack):
     def __init__(self, scope: Stack, api: CfnApi, authorizer: CfnAuthorizer):
         super().__init__(
```

### Comparing `b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/infrastructure/main_stack.py` & `b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/infrastructure/api_stack.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,23 @@
+from aws_cdk import Stack
 from aws_cdk.aws_apigatewayv2 import CfnApi, CfnStage
-from aws_cdk.core import Construct
 from b_aws_testing_framework.tools.cdk_testing.testing_stack import TestingStack
+from constructs import Construct
 
 from b_cfn_custom_userpool_authorizer.config.user_pool_ssm_config import UserPoolSsmConfig
 from b_cfn_custom_userpool_authorizer.user_pool_custom_authorizer import UserPoolCustomAuthorizer
-from b_cfn_custom_userpool_authorizer_test.integration.infrastructure.authorized_endpoint_stack import AuthorizedEndpointStack
 from b_cfn_custom_userpool_authorizer_test.integration.infrastructure.user_pool_stack import UserPoolStack
 
 
-class MainStack(TestingStack):
-    API_URL_KEY = 'ApiUrl'
-    API_ENDPOINT_KEY = 'ApiEndpoint'
-    USER_POOL_ID_KEY = 'UserPoolId'
-    USER_POOL_CLIENT_ID_KEY = 'UserPoolClientId'
-
-    def __init__(self, scope: Construct) -> None:
-        super().__init__(scope=scope)
+class ApiStack(Stack):
+    def __init__(self, scope: Construct, user_pool_stack: UserPoolStack) -> None:
+        super().__init__(scope=scope, id='ApiStack')
 
         prefix = TestingStack.global_prefix()
 
-        self.user_pool_stack = UserPoolStack(self)
-
         self.api = CfnApi(
             scope=self,
             id='Api',
             name=f'{prefix}Api',
             description='Sample description.',
             protocol_type='HTTP',
             cors_configuration=CfnApi.CorsProperty(
@@ -40,27 +33,20 @@
 
         self.authorizer = UserPoolCustomAuthorizer(
             scope=self,
             name=f'{prefix}UserPoolCustomAuthorizer',
             api=self.api,
             # Dynamically resolve.
             user_pool_config=UserPoolSsmConfig(
-                user_pool_id_ssm_key=self.user_pool_stack.ssm_pool_id.parameter_name,
-                user_pool_client_id_ssm_key=self.user_pool_stack.ssm_pool_client_id.parameter_name,
-                user_pool_region_ssm_key=self.user_pool_stack.ssm_pool_region.parameter_name,
+                user_pool_id_ssm_key=user_pool_stack.ssm_pool_id.parameter_name,
+                user_pool_client_id_ssm_key=user_pool_stack.ssm_pool_client_id.parameter_name,
+                user_pool_region_ssm_key=user_pool_stack.ssm_pool_region.parameter_name,
             )
         )
 
         self.stage: CfnStage = CfnStage(
             scope=self,
             id='Stage',
             stage_name='test',
             api_id=self.api.ref,
             auto_deploy=True,
         )
-
-        self.endpoint_stack = AuthorizedEndpointStack(self, self.api, self.authorizer)
-
-        self.add_output(self.API_URL_KEY, value=self.api.attr_api_endpoint)
-        self.add_output(self.API_ENDPOINT_KEY, value=f'{self.api.attr_api_endpoint}/{self.stage.stage_name}/dummy')
-        self.add_output(self.USER_POOL_ID_KEY, value=self.user_pool_stack.pool.user_pool_id)
-        self.add_output(self.USER_POOL_CLIENT_ID_KEY, value=self.user_pool_stack.client.user_pool_client_id)
```

### Comparing `b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/infrastructure/user_pool_stack.py` & `b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/infrastructure/user_pool_stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from aws_cdk.aws_cognito import *
+from aws_cdk import Stack
+from aws_cdk.aws_cognito import UserPool, AccountRecovery, AutoVerifiedAttrs, SignInAliases, StandardAttributes, StandardAttribute, UserPoolClient, AuthFlow
 from aws_cdk.aws_ssm import StringParameter
-from aws_cdk.core import Stack
 from b_aws_testing_framework.tools.cdk_testing.testing_stack import TestingStack
 
 
 class UserPoolStack(Stack):
     def __init__(self, scope: Stack):
         super().__init__(
             scope=scope,
```

### Comparing `b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/tests/test_authorizer_allow.py` & `b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/tests/test_authorizer_allow.py`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_userpool_authorizer-1.0.0/b_cfn_custom_userpool_authorizer_test/integration/tests/test_authorizer_deny.py` & `b_cfn_custom_userpool_authorizer-2.0.0/b_cfn_custom_userpool_authorizer_test/integration/tests/test_authorizer_deny.py`

 * *Files identical despite different names*

