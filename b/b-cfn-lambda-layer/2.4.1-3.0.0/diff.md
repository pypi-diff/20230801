# Comparing `tmp/b_cfn_lambda_layer-2.4.1.tar.gz` & `tmp/b_cfn_lambda_layer-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b_cfn_lambda_layer-2.4.1.tar", last modified: Fri Aug 26 10:25:54 2022, max compression
+gzip compressed data, was "b_cfn_lambda_layer-3.0.0.tar", last modified: Tue Aug  1 11:05:49 2023, max compression
```

## Comparing `b_cfn_lambda_layer-2.4.1.tar` & `b_cfn_lambda_layer-3.0.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.314351 b_cfn_lambda_layer-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9639 2022-08-26 10:25:54.314351 b_cfn_lambda_layer-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5848 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.310351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/dependency.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.314351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/dockerignore/
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/dockerignore/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)     4867 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/lambda_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3686 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/lambda_layer_code.py
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/package_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/pip_install.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.314351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.310351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/layer1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.314351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/layer1/layer1/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/layer1/layer1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/layer1/layer1/dummy_module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.310351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/layer2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.314351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/layer2/layer2/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/layer2/layer2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/layer2/layer2/dummy_module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.310351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/layer3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.314351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/layer3/layer3/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/layer3/layer3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/layer3/layer3/dummy_module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.310351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/layer_cross_stack/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.314351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/layer_cross_stack/layer_cross_stack/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/layer_cross_stack/layer_cross_stack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/layer_cross_stack/layer_cross_stack/dummy_module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.310351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/layer_source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.314351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/layer_source/layer_source/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/layer_source/layer_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/tmp/layer_source/layer_source/dummy_module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.310351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9639 2022-08-26 10:25:54.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2939 2022-08-26 10:25:54.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 10:25:54.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-08-26 10:25:54.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-08-26 10:25:54.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.310351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.314351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.314351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2698 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/cross_stack_layers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2091 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/function1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1602 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/function2.py
--rw-r--r--   0 runner    (1001) docker     (121)     2941 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/function3.py
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/function4.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.314351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/layer1/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/layer1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/layer1/dummy_module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.314351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/layer2/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/layer2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/layer2/dummy_module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.314351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/layer3/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/layer3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/layer3/dummy_module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.314351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/layer_cross_stack/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/layer_cross_stack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/layer_cross_stack/dummy_module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.314351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/layer_source/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/layer_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/layer_source/dummy_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/main_stack.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 10:25:54.314351 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/tests/test_lambda_layer_cross_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     1209 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/tests/test_lambda_layer_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/tests/test_lambda_layer_multiple.py
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/tests/test_lambda_layer_no_code.py
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/tests/test_lambda_layer_source_code.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 10:25:54.314351 b_cfn_lambda_layer-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-08-26 10:18:24.000000 b_cfn_lambda_layer-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.519945 b_cfn_lambda_layer-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-08-01 11:05:49.519945 b_cfn_lambda_layer-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.511945 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/dependency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.511945 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/dockerignore/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/dockerignore/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/lambda_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/lambda_layer_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/package_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/pip_install.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.511945 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.499945 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/layer1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.511945 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/layer1/layer1/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/layer1/layer1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/layer1/layer1/dummy_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.503945 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/layer2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.511945 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/layer2/layer2/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/layer2/layer2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/layer2/layer2/dummy_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.503945 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/layer3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.515946 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/layer3/layer3/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/layer3/layer3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/layer3/layer3/dummy_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.503945 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/layer_cross_stack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.515946 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/layer_cross_stack/layer_cross_stack/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/layer_cross_stack/layer_cross_stack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/layer_cross_stack/layer_cross_stack/dummy_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.503945 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/layer_source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.515946 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/layer_source/layer_source/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/layer_source/layer_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/tmp/layer_source/layer_source/dummy_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.511945 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-08-01 11:05:49.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-08-01 11:05:49.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:05:49.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-01 11:05:49.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 11:05:49.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.503945 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.515946 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.515946 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/cross_stack_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/function1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/function2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/function3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/function4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.515946 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/layer1/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/layer1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/layer1/dummy_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.515946 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/layer2/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/layer2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/layer2/dummy_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.515946 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/layer3/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/layer3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/layer3/dummy_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.515946 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/layer_cross_stack/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/layer_cross_stack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/layer_cross_stack/dummy_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.515946 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/layer_source/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/layer_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/layer_source/dummy_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/main_stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:05:49.519945 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/tests/test_lambda_layer_cross_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/tests/test_lambda_layer_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/tests/test_lambda_layer_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/tests/test_lambda_layer_no_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/tests/test_lambda_layer_source_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:05:49.519945 b_cfn_lambda_layer-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-08-01 10:57:51.000000 b_cfn_lambda_layer-3.0.0/setup.py
```

### Comparing `b_cfn_lambda_layer-2.4.1/HISTORY.md` & `b_cfn_lambda_layer-3.0.0/HISTORY.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Release history
 
+### 3.0.0
+* Upgrade CDK support from v1 to v2.
+* Update GitHub pipelines checkout, setup-node and setup-python versions.
+
 ### 2.4.1
 * Fix package manifest.
 
 ### 2.4.0
 * Now you no longer need to specify a path to source code. You can have
   an absolutely empty layer if you desire so.
```

### Comparing `b_cfn_lambda_layer-2.4.1/LICENSE` & `b_cfn_lambda_layer-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `b_cfn_lambda_layer-2.4.1/README.md` & `b_cfn_lambda_layer-3.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -90,43 +90,43 @@
 
 #### Full example
 
 This is a full example where we create a lambda layer and use it in lambda function.
 
 ```python
 from aws_cdk.aws_lambda import Function, Code, Runtime
-from aws_cdk.core import Stack
+from aws_cdk import Stack
 
 from b_cfn_lambda_layer.lambda_layer import LambdaLayer
 from b_cfn_lambda_layer.package_version import PackageVersion
 
 # Create layer with custom dependencies.
 layer = LambdaLayer(
     scope=Stack(...),
     name='TestLayer',
     # You can conveniently specify path to source code to include.
     # Or not specify it at all if you care only about dependencies.
     # source_path=None,
     source_path='/path/to/your/layer/source/code',
-    code_runtimes=[Runtime.PYTHON_3_6, Runtime.PYTHON_3_7, Runtime.PYTHON_3_8],
+    code_runtimes=[Runtime.PYTHON_3_8, Runtime.PYTHON_3_9, Runtime.PYTHON_3_10],
     # You can conveniently specify dependencies to include.
     dependencies={
         'python-jose': PackageVersion.from_string_version('3.3.0'),
         'boto3': PackageVersion.from_string_version('1.16.35'),
         'botocore': PackageVersion.from_string_version('1.19.35')
     }
 )
 
 # Create a function with a layer.
 Function(
     scope=Stack(...),
     id='MyFunction',
     code=Code.from_asset('/path/to/lambda/function/code'),
     handler='index.handler',
-    runtime=Runtime.PYTHON_3_6,
+    runtime=Runtime.PYTHON_3_10,
     # Specify layers.
     layers=[layer]
 )
 ```
 
 #### Using layers in multiple stacks
```

### Comparing `b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/Dockerfile` & `b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/Dockerfile`

 * *Files identical despite different names*

### Comparing `b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/dependency.py` & `b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/dependency.py`

 * *Files identical despite different names*

### Comparing `b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/lambda_layer.py` & `b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/lambda_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from functools import lru_cache
 from typing import List, Optional, Dict
 
-from aws_cdk.aws_lambda import LayerVersion, Runtime, Function, ILayerVersion
+from aws_cdk import Stack, DockerImage
+from aws_cdk.aws_lambda import LayerVersion, Runtime, ILayerVersion, Function
 from aws_cdk.aws_ssm import StringParameter
-from aws_cdk.core import Stack, DockerImage
 
 from b_cfn_lambda_layer.dependency import Dependency
 from b_cfn_lambda_layer.lambda_layer_code import LambdaLayerCode
 from b_cfn_lambda_layer.package_version import PackageVersion
 
 LOGGER = logging.getLogger(__name__)
 
@@ -57,15 +57,16 @@
                 dependencies=[Dependency(key, value) for key, value in (dependencies or {}).items()],
                 docker_image=docker_image
             ).build(),
             compatible_runtimes=code_runtimes or [
                 Runtime.PYTHON_3_6,
                 Runtime.PYTHON_3_7,
                 Runtime.PYTHON_3_8,
-                Runtime.PYTHON_3_9
+                Runtime.PYTHON_3_9,
+                Runtime.PYTHON_3_10
             ]
         )
 
         for argument in args:
             LOGGER.warning(f'Positional argument: ({argument}) is not supported!')
 
         for name, argument in kwargs.items():
```

### Comparing `b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/lambda_layer_code.py` & `b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/lambda_layer_code.py`

 * *Files identical despite different names*

### Comparing `b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/package_version.py` & `b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/package_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+from __future__ import annotations
+
 from enum import Enum
 from typing import Optional
 
 
 class PackageVersion:
-
     class VersionType(Enum):
-
         NONE = 'NONE'
         SPECIFIC = 'SPECIFIC'
         LATEST = 'LATEST'
 
     def __init__(self, version: Optional[str] = None, version_type: Optional[VersionType] = None):
         self.__version = version
         self.__version_type = version_type
@@ -19,17 +19,17 @@
         return self.__version
 
     @property
     def version_type(self) -> VersionType:
         return self.__version_type
 
     @classmethod
-    def from_string_version(cls, version_string: str) -> 'PackageVersion':
+    def from_string_version(cls, version_string: str) -> PackageVersion:
         return cls(version=version_string, version_type=cls.VersionType.SPECIFIC)
 
     @classmethod
-    def latest(cls) -> 'PackageVersion':
+    def latest(cls) -> PackageVersion:
         return cls(version_type=cls.VersionType.LATEST)
 
     @classmethod
-    def dont_install(cls) -> 'PackageVersion':
+    def dont_install(cls) -> PackageVersion:
         return cls(version_type=cls.VersionType.NONE)
```

### Comparing `b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer/pip_install.py` & `b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer/pip_install.py`

 * *Files identical despite different names*

### Comparing `b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer.egg-info/SOURCES.txt` & `b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/conftest.py` & `b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/cross_stack_layers.py` & `b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/cross_stack_layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from aws_cdk import Stack
 from aws_cdk.aws_lambda import Runtime, Function, Code
-from aws_cdk.core import Construct, Stack
 from b_aws_testing_framework.tools.cdk_testing.testing_stack import TestingStack
+from constructs import Construct
 
 from b_cfn_lambda_layer.lambda_layer import LambdaLayer
 from b_cfn_lambda_layer_test.integration.infrastructure.layer_cross_stack import root
 
 
 class CrossStackLayers(Stack):
     def __init__(self, scope: Construct):
```

### Comparing `b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/function1.py` & `b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/function1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+from aws_cdk import Stack
 from aws_cdk.aws_lambda import Function, Code, Runtime
-from aws_cdk.core import Stack
 from b_aws_testing_framework.tools.cdk_testing.testing_stack import TestingStack
 
 from b_cfn_lambda_layer.lambda_layer import LambdaLayer
 from b_cfn_lambda_layer.package_version import PackageVersion
 from b_cfn_lambda_layer_test.integration.infrastructure.layer_source import root
 
 
 class Function1(Function):
     """
     Function that allows us to test whether installing dependencies works.
     """
+
     def __init__(self, scope: Stack):
         super().__init__(
             scope=scope,
             id=f'{TestingStack.global_prefix()}TestingFunction1',
             code=Code.from_inline(
                 'import urllib3\n'
                 'import jose\n'
@@ -30,21 +31,21 @@
                 '        BotocoreVersion=botocore.__version__,\n'
                 '        JoseVersion=jose.__version__,\n'
                 '        Dummy=DummyModule.action()\n'
                 '    )'
                 '\n'
             ),
             handler='index.handler',
-            runtime=Runtime.PYTHON_3_7,
+            runtime=Runtime.PYTHON_3_10,
             layers=[
                 LambdaLayer(
                     scope=scope,
                     name=f'{TestingStack.global_prefix()}TestingLayer1',
                     source_path=root,
-                    code_runtimes=[Runtime.PYTHON_3_7, Runtime.PYTHON_3_8],
+                    code_runtimes=[Runtime.PYTHON_3_6, Runtime.PYTHON_3_7, Runtime.PYTHON_3_8, Runtime.PYTHON_3_9, Runtime.PYTHON_3_10],
                     dependencies={
                         'python-jose': PackageVersion.from_string_version('3.3.0'),
                         'boto3': PackageVersion.from_string_version('1.16.35'),
                         'botocore': PackageVersion.from_string_version('1.19.35')
                     },
                 )
             ]
```

### Comparing `b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/function2.py` & `b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/function2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from aws_cdk.aws_lambda import Function, Code, Runtime
-from aws_cdk.core import Stack
+from aws_cdk import Stack
 from b_aws_testing_framework.tools.cdk_testing.testing_stack import TestingStack
 
 from b_cfn_lambda_layer.lambda_layer import LambdaLayer
 from b_cfn_lambda_layer_test.integration.infrastructure.layer_source import root
 
 
 class Function2(Function):
     """
     Function that allows us to test whether layer source code is included in the parent directory
     i.e. instead of "from a import A" you would get "from parent_dir.a import A".
     """
+
     def __init__(self, scope: Stack):
         super().__init__(
             scope=scope,
             id=f'{TestingStack.global_prefix()}TestingFunction2',
             code=Code.from_inline(
                 # Ensure that dummy module is accessible from lambda layer
                 # and the parent directory is included.
@@ -24,17 +25,17 @@
                 '    return dict(\n'
                 # Use the dummy module to ensure everything works.
                 '        Dummy=DummyModule.action()\n'
                 '    )'
                 '\n'
             ),
             handler='index.handler',
-            runtime=Runtime.PYTHON_3_7,
+            runtime=Runtime.PYTHON_3_10,
             layers=[
                 LambdaLayer(
                     scope=scope,
                     name=f'{TestingStack.global_prefix()}TestingLayer2',
                     source_path=root,
-                    code_runtimes=[Runtime.PYTHON_3_7, Runtime.PYTHON_3_8],
+                    code_runtimes=[Runtime.PYTHON_3_6, Runtime.PYTHON_3_7, Runtime.PYTHON_3_8, Runtime.PYTHON_3_9, Runtime.PYTHON_3_10],
                 )
             ]
         )
```

### Comparing `b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/function4.py` & `b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/function4.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from aws_cdk import Stack
 from aws_cdk.aws_lambda import Function, Code, Runtime
-from aws_cdk.core import Stack
 from b_aws_testing_framework.tools.cdk_testing.testing_stack import TestingStack
 
 from b_cfn_lambda_layer.lambda_layer import LambdaLayer
 
 
 class Function4(Function):
     """
@@ -18,15 +18,15 @@
                 'def handler(*args, **kwargs):\n'
                 '    return dict(\n'
                 '        Key=123\n'
                 '    )'
                 '\n'
             ),
             handler='index.handler',
-            runtime=Runtime.PYTHON_3_7,
+            runtime=Runtime.PYTHON_3_10,
             layers=[
                 LambdaLayer(
                     scope=scope,
                     name=f'{TestingStack.global_prefix()}TestingLayer4'
                 )
             ]
         )
```

### Comparing `b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/infrastructure/main_stack.py` & `b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/infrastructure/main_stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from aws_cdk.core import Construct
 from b_aws_testing_framework.tools.cdk_testing.testing_stack import TestingStack
+from constructs import Construct
 
 from b_cfn_lambda_layer_test.integration.infrastructure.cross_stack_layers import CrossStackLayers
 from b_cfn_lambda_layer_test.integration.infrastructure.function1 import Function1
 from b_cfn_lambda_layer_test.integration.infrastructure.function2 import Function2
 from b_cfn_lambda_layer_test.integration.infrastructure.function3 import Function3
 from b_cfn_lambda_layer_test.integration.infrastructure.function4 import Function4
```

### Comparing `b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/tests/test_lambda_layer_cross_stack.py` & `b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/tests/test_lambda_layer_cross_stack.py`

 * *Files identical despite different names*

### Comparing `b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/tests/test_lambda_layer_dependencies.py` & `b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/tests/test_lambda_layer_dependencies.py`

 * *Files identical despite different names*

### Comparing `b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/tests/test_lambda_layer_multiple.py` & `b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/tests/test_lambda_layer_multiple.py`

 * *Files identical despite different names*

### Comparing `b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/tests/test_lambda_layer_no_code.py` & `b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/tests/test_lambda_layer_no_code.py`

 * *Files identical despite different names*

### Comparing `b_cfn_lambda_layer-2.4.1/b_cfn_lambda_layer_test/integration/tests/test_lambda_layer_source_code.py` & `b_cfn_lambda_layer-3.0.0/b_cfn_lambda_layer_test/integration/tests/test_lambda_layer_source_code.py`

 * *Files identical despite different names*

### Comparing `b_cfn_lambda_layer-2.4.1/setup.py` & `b_cfn_lambda_layer-3.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     description=(
         'AWS CDK based lambda layer including useful utilities.'
     ),
     long_description=README + '\n\n' + HISTORY,
     long_description_content_type='text/markdown',
     include_package_data=True,
     install_requires=[
-        'aws-cdk.aws_lambda>=1.150.0,<2.0.0',
-        'aws-cdk.aws-ssm>=1.150.0,<2.0.0',
+        'aws-cdk-lib>=2.0.0,<3.0.0',
+        'aws-cdk-constructs>=2.0.0,<3.0.0',
     ],
     author='Laimonas Sutkus',
     author_email='laimonas.sutkus@biomapas.com',
     keywords='AWS CDK Lambda Layer',
     url='https://github.com/biomapas/B.CfnLambdaLayer.git',
     classifiers=[
         'Programming Language :: Python :: 3',
```

