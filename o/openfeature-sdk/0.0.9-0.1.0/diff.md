# Comparing `tmp/openfeature_sdk-0.0.9.tar.gz` & `tmp/openfeature_sdk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfeature_sdk-0.0.9.tar", last modified: Fri Jan 27 14:39:14 2023, max compression
+gzip compressed data, was "openfeature_sdk-0.1.0.tar", last modified: Tue Aug  1 15:33:40 2023, max compression
```

## Comparing `openfeature_sdk-0.0.9.tar` & `openfeature_sdk-0.1.0.tar`

### file list

```diff
@@ -1,45 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 14:39:14.154985 openfeature_sdk-0.0.9/
--rw-r--r--   0 root         (0) root         (0)    11323 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)    16694 2023-01-27 14:39:14.154985 openfeature_sdk-0.0.9/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 14:39:14.146985 openfeature_sdk-0.0.9/open_feature/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 14:39:14.146985 openfeature_sdk-0.0.9/open_feature/evaluation_context/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/evaluation_context/__init__.py
--rw-r--r--   0 root         (0) root         (0)      616 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/evaluation_context/evaluation_context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 14:39:14.146985 openfeature_sdk-0.0.9/open_feature/exception/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/exception/__init__.py
--rw-r--r--   0 root         (0) root         (0)      315 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/exception/error_code.py
--rw-r--r--   0 root         (0) root         (0)     4128 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/exception/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 14:39:14.146985 openfeature_sdk-0.0.9/open_feature/flag_evaluation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/flag_evaluation/__init__.py
--rw-r--r--   0 root         (0) root         (0)      474 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/flag_evaluation/flag_evaluation_details.py
--rw-r--r--   0 root         (0) root         (0)      249 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/flag_evaluation/flag_evaluation_options.py
--rw-r--r--   0 root         (0) root         (0)      170 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/flag_evaluation/flag_type.py
--rw-r--r--   0 root         (0) root         (0)      198 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/flag_evaluation/reason.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 14:39:14.150985 openfeature_sdk-0.0.9/open_feature/hooks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2500 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/hooks/hook.py
--rw-r--r--   0 root         (0) root         (0)      438 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/hooks/hook_context.py
--rw-r--r--   0 root         (0) root         (0)     4428 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/hooks/hook_support.py
--rw-r--r--   0 root         (0) root         (0)      144 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/hooks/hook_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 14:39:14.150985 openfeature_sdk-0.0.9/open_feature/immutable_dict/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/immutable_dict/__init__.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/immutable_dict/mapping_proxy_type.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/open_feature_api.py
--rw-r--r--   0 root         (0) root         (0)    13117 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/open_feature_client.py
--rw-r--r--   0 root         (0) root         (0)      558 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/open_feature_evaluation_context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 14:39:14.150985 openfeature_sdk-0.0.9/open_feature/provider/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/provider/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/provider/metadata.py
--rw-r--r--   0 root         (0) root         (0)      200 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/provider/no_op_metadata.py
--rw-r--r--   0 root         (0) root         (0)     2687 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/provider/no_op_provider.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/open_feature/provider/provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 14:39:14.154985 openfeature_sdk-0.0.9/openfeature_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16694 2023-01-27 14:39:14.000000 openfeature_sdk-0.0.9/openfeature_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1241 2023-01-27 14:39:14.000000 openfeature_sdk-0.0.9/openfeature_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-27 14:39:14.000000 openfeature_sdk-0.0.9/openfeature_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-01-27 14:39:14.000000 openfeature_sdk-0.0.9/openfeature_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-01-27 14:39:14.000000 openfeature_sdk-0.0.9/openfeature_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      807 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     3268 2023-01-27 14:39:03.000000 openfeature_sdk-0.0.9/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-27 14:39:14.154985 openfeature_sdk-0.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 15:33:40.639144 openfeature_sdk-0.1.0/
+-rw-r--r--   0 root         (0) root         (0)    11323 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    21095 2023-08-01 15:33:40.639144 openfeature_sdk-0.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 15:33:40.631143 openfeature_sdk-0.1.0/open_feature/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 15:33:40.631143 openfeature_sdk-0.1.0/open_feature/_backports/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/_backports/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      191 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/_backports/strenum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 15:33:40.631143 openfeature_sdk-0.1.0/open_feature/evaluation_context/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/evaluation_context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      616 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/evaluation_context/evaluation_context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 15:33:40.635144 openfeature_sdk-0.1.0/open_feature/exception/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/exception/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      315 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/exception/error_code.py
+-rw-r--r--   0 root         (0) root         (0)     4128 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/exception/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 15:33:40.635144 openfeature_sdk-0.1.0/open_feature/flag_evaluation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/flag_evaluation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      474 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/flag_evaluation/flag_evaluation_details.py
+-rw-r--r--   0 root         (0) root         (0)      249 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/flag_evaluation/flag_evaluation_options.py
+-rw-r--r--   0 root         (0) root         (0)      158 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/flag_evaluation/flag_type.py
+-rw-r--r--   0 root         (0) root         (0)      275 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/flag_evaluation/reason.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/flag_evaluation/resolution_details.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 15:33:40.635144 openfeature_sdk-0.1.0/open_feature/hooks/
+-rw-r--r--   0 root         (0) root         (0)      317 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/hooks/hook.py
+-rw-r--r--   0 root         (0) root         (0)      438 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/hooks/hook_context.py
+-rw-r--r--   0 root         (0) root         (0)     4428 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/hooks/hook_support.py
+-rw-r--r--   0 root         (0) root         (0)      144 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/hooks/hook_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 15:33:40.635144 openfeature_sdk-0.1.0/open_feature/immutable_dict/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/immutable_dict/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/immutable_dict/mapping_proxy_type.py
+-rw-r--r--   0 root         (0) root         (0)      945 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/open_feature_api.py
+-rw-r--r--   0 root         (0) root         (0)    13886 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/open_feature_client.py
+-rw-r--r--   0 root         (0) root         (0)      558 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/open_feature_evaluation_context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 15:33:40.639144 openfeature_sdk-0.1.0/open_feature/provider/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/provider/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3974 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/provider/in_memory_provider.py
+-rw-r--r--   0 root         (0) root         (0)       77 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/provider/metadata.py
+-rw-r--r--   0 root         (0) root         (0)      200 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/provider/no_op_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     2527 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/provider/no_op_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1739 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/open_feature/provider/provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 15:33:40.639144 openfeature_sdk-0.1.0/openfeature_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    21095 2023-08-01 15:33:40.000000 openfeature_sdk-0.1.0/openfeature_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1561 2023-08-01 15:33:40.000000 openfeature_sdk-0.1.0/openfeature_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 15:33:40.000000 openfeature_sdk-0.1.0/openfeature_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-08-01 15:33:40.000000 openfeature_sdk-0.1.0/openfeature_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 15:33:40.000000 openfeature_sdk-0.1.0/openfeature_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      807 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     7669 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/readme.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 15:33:40.639144 openfeature_sdk-0.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 15:33:40.639144 openfeature_sdk-0.1.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/tests/test_open_feature_api.py
+-rw-r--r--   0 root         (0) root         (0)     4667 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/tests/test_open_feature_client.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/tests/test_open_feature_evaluation_context.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-08-01 15:33:25.000000 openfeature_sdk-0.1.0/tests/test_open_feature_flag_evaluation.py
```

### Comparing `openfeature_sdk-0.0.9/LICENSE` & `openfeature_sdk-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openfeature_sdk-0.0.9/PKG-INFO` & `openfeature_sdk-0.1.0/openfeature_sdk.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openfeature_sdk
-Version: 0.0.9
+Name: openfeature-sdk
+Version: 0.1.0
 Summary: Standardizing Feature Flagging for Everyone
 Author-email: OpenFeature <openfeature-core@groups.io>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,97 +209,206 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# OpenFeature SDK for Python
+<!-- markdownlint-disable MD033 -->
+<p align="center">
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/open-feature/community/0e23508c163a6a1ac8c0ced3e4bd78faafe627c7/assets/logo/horizontal/white/openfeature-horizontal-white.svg">
+    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/open-feature/community/0e23508c163a6a1ac8c0ced3e4bd78faafe627c7/assets/logo/horizontal/black/openfeature-horizontal-black.svg">
+    <img align="center" alt="OpenFeature Logo">
+  </picture>
+</p>
+
+<h2 align="center">OpenFeature Python SDK</h2>
 
 [![PyPI version](https://badge.fury.io/py/openfeature-sdk.svg)](https://badge.fury.io/py/openfeature-sdk)
 ![Python 3.8+](https://img.shields.io/badge/python->=3.8-blue.svg)
 [![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
 [![Specification](https://img.shields.io/static/v1?label=Specification&message=v0.3.0&color=red)](https://github.com/open-feature/spec/tree/v0.3.0)
 [![on-merge](https://github.com/open-feature/python-sdk/actions/workflows/merge.yml/badge.svg)](https://github.com/open-feature/python-sdk/actions/workflows/merge.yml)
 [![codecov](https://codecov.io/gh/open-feature/python-sdk/branch/main/graph/badge.svg?token=FQ1I444HB3)](https://codecov.io/gh/open-feature/python-sdk)
 
+> ⚠️ Development is in progress, but there's not a stable release available. ⚠️
+
 This is the Python implementation of [OpenFeature](https://openfeature.dev), a vendor-agnostic abstraction library for evaluating feature flags.
 
 We support multiple data types for flags (numbers, strings, booleans, objects) as well as hooks, which can alter the lifecycle of a flag evaluation.
 
 This library is intended to be used in server-side contexts and has not been evaluated for use in mobile devices.
 
-## Usage
-
-While Boolean provides the simplest introduction, we offer a variety of flag types.
-
-```python
-# Depending on the flag type, use one of the methods below
-flag_key = "PROVIDER_FLAG"
-boolean_result = open_feature_client.get_boolean_value(key=flag_key,default_value=False)
-integer_result = open_feature_client.get_integer_value(key=flag_key,default_value=-1)
-float_result = open_feature_client.get_float_value(key=flag_key,default_value=-1)
-string_result = open_feature_client.get_string_value(key=flag_key,default_value="")
-object_result = open_feature_client.get_object_value(key=flag_key,default_value={})
-```
-
-Each provider class may have further setup required i.e. secret keys, environment variables etc
-
-## Requirements
+## 🔍 Requirements:
 
 - Python 3.8+
 
-## Installation
+## 📦 Installation:
 
 ### Add it to your build
 
 <!---x-release-please-start-version-->
 
 Pip install
 
 ```bash
-pip install openfeature-sdk==0.0.9
+pip install openfeature-sdk==0.1.0
 ```
 
 requirements.txt
 
 ```bash
-openfeature-sdk==0.0.9
+openfeature-sdk==0.1.0
 ```
 
 ```python
 pip install requirements.txt
 ```
 
 <!---x-release-please-end-->
 
+## 🌟 Features:
+
+- support for various backend [providers](https://openfeature.dev/docs/reference/concepts/provider)
+- easy integration and extension via [hooks](https://openfeature.dev/docs/reference/concepts/hooks)
+- bool, string, numeric, and object flag types
+- [context-aware](https://openfeature.dev/docs/reference/concepts/evaluation-context) evaluation
+
+## 🚀 Usage:
+
 ### Configure it
 
 In order to use the sdk there is some minor configuration. Follow the script below:
 
 ```python
 from open_feature import open_feature_api
 from open_feature.provider.no_op_provider import NoOpProvider
 
 open_feature_api.set_provider(NoOpProvider())
 open_feature_client = open_feature_api.get_client()
 ```
 
-## Contacting us
+### Basics:
 
-We hold regular meetings which you can see [here](https://github.com/open-feature/community/#meetings-and-events).
+While Boolean provides the simplest introduction, we offer a variety of flag types.
 
-We are also present on the `#openfeature` channel in the [CNCF slack](https://slack.cncf.io/).
+```python
+# Depending on the flag type, use one of the methods below
+flag_key = "PROVIDER_FLAG"
+boolean_result = open_feature_client.get_boolean_value(key=flag_key,default_value=False)
+integer_result = open_feature_client.get_integer_value(key=flag_key,default_value=-1)
+float_result = open_feature_client.get_float_value(key=flag_key,default_value=-1)
+string_result = open_feature_client.get_string_value(key=flag_key,default_value="")
+object_result = open_feature_client.get_object_value(key=flag_key,default_value={})
+```
 
-## Contributors
+You can also bind a provider to a specific client by name instead of setting that provider globally:
 
-Thanks so much to our contributors.
+```python
 
+open_feature_api.set_provider(NoOpProvider())
+```
+
+Each provider class may have further setup required i.e. secret keys, environment variables etc
+
+### Context-aware evaluation:
+
+Sometimes the value of a flag must take into account some dynamic criteria about the application or user, such as the user location, IP, email address, or the location of the server.
+In OpenFeature, we refer to this as [`targeting`](https://openfeature.dev/specification/glossary#targeting).
+If the flag system you're using supports targeting, you can provide the input data using the `EvaluationContext`.
+
+```python
+from open_feature.open_feature_api import get_client, get_provider, set_provider
+from open_feature.open_feature_evaluation_context import (
+    api_evaluation_context,
+    set_api_evaluation_context,
+)
+
+global_context = EvaluationContext(
+    targeting_key="targeting_key1", attributes={"application": "value1"}
+)
+request_context = EvaluationContext(
+    targeting_key="targeting_key2", attributes={"email": request.form['email']}
+)
+
+## set global context
+set_api_evaluation_context(first_context)
+
+# merge second context
+client = get_client(name="No-op Provider", version="0.5.2")
+client.get_string_value("email", None, request_context)
+
+```
+
+### Events
+
+TBD (See Issue [#131](https://github.com/open-feature/python-sdk/issues/131))
+
+### Providers:
+
+To develop a provider, you need to create a new project and include the OpenFeature SDK as a dependency. This can be a new repository or included in [the existing contrib repository](https://github.com/open-feature/python-sdk-contrib) available under the OpenFeature organization. Finally, you’ll then need to write the provider itself. This can be accomplished by implementing the `Provider` interface exported by the OpenFeature SDK.
+
+See [here](https://openfeature.dev/ecosystem) for a catalog of available providers.
+
+### Hooks:
+
+A hook is a mechanism that allows for adding arbitrary behavior at well-defined points of the flag evaluation life-cycle. Use cases include validating the resolved flag value, modifying or adding data to the evaluation context, logging, telemetry, and tracking.
+
+```python
+from open_feature.hooks.hook import Hook
+
+class MyHook(Hook):
+    def after(self, hook_context: HookContext, details: FlagEvaluationDetails, hints: dict):
+        print("This runs after the flag has been evaluated")
+
+
+# set global hooks at the API-level
+from open_feature.hooks import add_api_hooks
+add_api_hooks([MyHook()])
+
+# or configure them in the client
+client = OpenFeatureClient()
+client.add_hooks([MyHook()])
+```
+
+See [here](https://openfeature.dev/ecosystem) for a catalog of available hooks.
+
+### Logging:
+
+TBD
+
+## ⭐️ Support the project
+
+- Give this repo a ⭐️!
+- Follow us on social media:
+  - Twitter: [@openfeature](https://twitter.com/openfeature)
+  - LinkedIn: [OpenFeature](https://www.linkedin.com/company/openfeature/)
+- Join us on [Slack](https://cloud-native.slack.com/archives/C0344AANLA1)
+- For more check out our [community page](https://openfeature.dev/community/)
+
+## 🤝 Contributing
+
+Interested in contributing? Great, we'd love your help! To get started, take a look at the [CONTRIBUTING](CONTRIBUTING.md) guide.
+
+### Thanks to everyone that has already contributed
+
+<!-- TODO: update with correct repo -->
 <a href="https://github.com/open-feature/python-sdk/graphs/contributors">
-  <img src="https://contrib.rocks/image?repo=open-feature/python-sdk" />
+  <img src="https://contrib.rocks/image?repo=open-feature/python-sdk" alt="Pictures of the folks who have contributed to the project" />
 </a>
 
 Made with [contrib.rocks](https://contrib.rocks).
 
-### Development
+## Contacting us
+
+We hold regular meetings which you can see [here](https://github.com/open-feature/community/#meetings-and-events).
+
+We are also present on the `#openfeature` channel in the [CNCF slack](https://slack.cncf.io/).
+
+## 📜 License
+
+[Apache License 2.0](LICENSE)
+
+<!-- TODO: add FOSSA widget -->
 
-If you would like to contribute to the project, please see our [contributing](./CONTRIBUTING.md) documentation!
+[openfeature-website]: https://openfeature.dev
```

### Comparing `openfeature_sdk-0.0.9/open_feature/evaluation_context/evaluation_context.py` & `openfeature_sdk-0.1.0/open_feature/evaluation_context/evaluation_context.py`

 * *Files identical despite different names*

### Comparing `openfeature_sdk-0.0.9/open_feature/exception/exceptions.py` & `openfeature_sdk-0.1.0/open_feature/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `openfeature_sdk-0.0.9/open_feature/hooks/hook.py` & `openfeature_sdk-0.1.0/open_feature/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `openfeature_sdk-0.0.9/open_feature/hooks/hook_support.py` & `openfeature_sdk-0.1.0/open_feature/hooks/hook_support.py`

 * *Files identical despite different names*

### Comparing `openfeature_sdk-0.0.9/open_feature/immutable_dict/mapping_proxy_type.py` & `openfeature_sdk-0.1.0/open_feature/immutable_dict/mapping_proxy_type.py`

 * *Files identical despite different names*

### Comparing `openfeature_sdk-0.0.9/open_feature/open_feature_api.py` & `openfeature_sdk-0.1.0/open_feature/open_feature_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import typing
 
 from open_feature.exception.exceptions import GeneralError
 from open_feature.open_feature_client import OpenFeatureClient
+from open_feature.provider.metadata import Metadata
 from open_feature.provider.no_op_provider import NoOpProvider
 from open_feature.provider.provider import AbstractProvider
 
 _provider: AbstractProvider = NoOpProvider()
 
 
 def get_client(
@@ -20,7 +21,12 @@
         raise GeneralError(error_message="No provider")
     _provider = provider
 
 
 def get_provider() -> typing.Optional[AbstractProvider]:
     global _provider
     return _provider
+
+
+def get_provider_metadata() -> typing.Optional[Metadata]:
+    global _provider
+    return _provider.get_metadata()
```

### Comparing `openfeature_sdk-0.0.9/open_feature/open_feature_client.py` & `openfeature_sdk-0.1.0/open_feature/open_feature_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,61 @@
 import logging
 import typing
+from dataclasses import dataclass
 
 from open_feature.evaluation_context.evaluation_context import EvaluationContext
 from open_feature.exception.error_code import ErrorCode
 from open_feature.exception.exceptions import (
     GeneralError,
     OpenFeatureError,
     TypeMismatchError,
 )
 from open_feature.flag_evaluation.flag_evaluation_details import FlagEvaluationDetails
 from open_feature.flag_evaluation.flag_evaluation_options import FlagEvaluationOptions
 from open_feature.flag_evaluation.flag_type import FlagType
 from open_feature.flag_evaluation.reason import Reason
+from open_feature.flag_evaluation.resolution_details import FlagResolutionDetails
+from open_feature.hooks import api_hooks
 from open_feature.hooks.hook import Hook
 from open_feature.hooks.hook_context import HookContext
 from open_feature.hooks.hook_support import (
     after_all_hooks,
     after_hooks,
     before_hooks,
     error_hooks,
 )
 from open_feature.open_feature_evaluation_context import api_evaluation_context
 from open_feature.provider.no_op_provider import NoOpProvider
 from open_feature.provider.provider import AbstractProvider
 
 GetDetailCallable = typing.Union[
     typing.Callable[
-        [str, bool, typing.Optional[EvaluationContext]], FlagEvaluationDetails[bool]
+        [str, bool, typing.Optional[EvaluationContext]], FlagResolutionDetails[bool]
     ],
     typing.Callable[
-        [str, int, typing.Optional[EvaluationContext]], FlagEvaluationDetails[int]
+        [str, int, typing.Optional[EvaluationContext]], FlagResolutionDetails[int]
     ],
     typing.Callable[
-        [str, float, typing.Optional[EvaluationContext]], FlagEvaluationDetails[float]
+        [str, float, typing.Optional[EvaluationContext]], FlagResolutionDetails[float]
     ],
     typing.Callable[
-        [str, str, typing.Optional[EvaluationContext]], FlagEvaluationDetails[str]
+        [str, str, typing.Optional[EvaluationContext]], FlagResolutionDetails[str]
     ],
     typing.Callable[
-        [str, dict, typing.Optional[EvaluationContext]], FlagEvaluationDetails[dict]
+        [str, typing.Union[dict, list], typing.Optional[EvaluationContext]],
+        FlagResolutionDetails[typing.Union[dict, list]],
     ],
 ]
 
 
+@dataclass
+class ClientMetadata:
+    name: str
+
+
 class OpenFeatureClient:
     def __init__(
         self,
         name: typing.Optional[str],
         version: typing.Optional[str],
         provider: AbstractProvider,
         context: typing.Optional[EvaluationContext] = None,
@@ -54,26 +63,28 @@
     ):
         self.name = name
         self.version = version
         self.context = context or EvaluationContext()
         self.hooks = hooks or []
         self.provider = provider
 
+    def get_metadata(self):
+        return ClientMetadata(name=self.name)
+
     def add_hooks(self, hooks: typing.List[Hook]):
         self.hooks = self.hooks + hooks
 
     def get_boolean_value(
         self,
         flag_key: str,
         default_value: bool,
         evaluation_context: typing.Optional[EvaluationContext] = None,
         flag_evaluation_options: typing.Optional[FlagEvaluationOptions] = None,
     ) -> bool:
-        return self.evaluate_flag_details(
-            FlagType.BOOLEAN,
+        return self.get_boolean_details(
             flag_key,
             default_value,
             evaluation_context,
             flag_evaluation_options,
         ).value
 
     def get_boolean_details(
@@ -94,16 +105,15 @@
     def get_string_value(
         self,
         flag_key: str,
         default_value: str,
         evaluation_context: typing.Optional[EvaluationContext] = None,
         flag_evaluation_options: typing.Optional[FlagEvaluationOptions] = None,
     ) -> str:
-        return self.evaluate_flag_details(
-            FlagType.STRING,
+        return self.get_string_details(
             flag_key,
             default_value,
             evaluation_context,
             flag_evaluation_options,
         ).value
 
     def get_string_details(
@@ -178,30 +188,29 @@
             evaluation_context,
             flag_evaluation_options,
         )
 
     def get_object_value(
         self,
         flag_key: str,
-        default_value: dict,
+        default_value: typing.Union[dict, list],
         evaluation_context: typing.Optional[EvaluationContext] = None,
         flag_evaluation_options: typing.Optional[FlagEvaluationOptions] = None,
     ) -> dict:
-        return self.evaluate_flag_details(
-            FlagType.OBJECT,
+        return self.get_object_details(
             flag_key,
             default_value,
             evaluation_context,
             flag_evaluation_options,
         ).value
 
     def get_object_details(
         self,
         flag_key: str,
-        default_value: dict,
+        default_value: typing.Union[dict, list],
         evaluation_context: typing.Optional[EvaluationContext] = None,
         flag_evaluation_options: typing.Optional[FlagEvaluationOptions] = None,
     ) -> FlagEvaluationDetails:
         return self.evaluate_flag_details(
             FlagType.OBJECT,
             flag_key,
             default_value,
@@ -242,21 +251,22 @@
             flag_key=flag_key,
             flag_type=flag_type,
             default_value=default_value,
             evaluation_context=evaluation_context,
             client_metadata=None,
             provider_metadata=None,
         )
-        # Todo add api level hooks
-        # https://github.com/open-feature/spec/blob/main/specification/sections/04-hooks.md#requirement-442
         # Hooks need to be handled in different orders at different stages
         # in the flag evaluation
         # before: API, Client, Invocation, Provider
         merged_hooks = (
-            self.hooks + evaluation_hooks + self.provider.get_provider_hooks()
+            api_hooks()
+            + self.hooks
+            + evaluation_hooks
+            + self.provider.get_provider_hooks()
         )
         # after, error, finally: Provider, Invocation, Client, API
         reversed_merged_hooks = merged_hooks[:]
         reversed_merged_hooks.reverse()
 
         try:
             # https://github.com/open-feature/spec/blob/main/specification/sections/03-evaluation-context.md
@@ -352,17 +362,35 @@
             FlagType.STRING: self.provider.resolve_string_details,
         }
 
         get_details_callable = get_details_callables.get(flag_type)
         if not get_details_callable:
             raise GeneralError(error_message="Unknown flag type")
 
-        value = get_details_callable(*args)
+        resolution = get_details_callable(*args)
 
         # we need to check the get_args to be compatible with union types.
-        is_right_instance = isinstance(
-            value.value, typing.get_args(flag_type.value)
-        ) or isinstance(value.value, flag_type.value)
-        if not is_right_instance:
-            raise TypeMismatchError()
+        _typecheck_flag_value(resolution.value, flag_type)
+
+        return FlagEvaluationDetails(
+            flag_key=flag_key,
+            value=resolution.value,
+            variant=resolution.variant,
+            reason=resolution.reason,
+            error_code=resolution.error_code,
+            error_message=resolution.error_message,
+        )
+
 
-        return value
+def _typecheck_flag_value(value, flag_type):
+    type_map = {
+        FlagType.BOOLEAN: bool,
+        FlagType.STRING: str,
+        FlagType.OBJECT: typing.Union[dict, list],
+        FlagType.FLOAT: float,
+        FlagType.INTEGER: int,
+    }
+    _type = type_map.get(flag_type)
+    if not _type:
+        raise GeneralError(error_message="Unknown flag type")
+    if not isinstance(value, _type):
+        raise TypeMismatchError(f"Expected type {_type} but got {type(value)}")
```

### Comparing `openfeature_sdk-0.0.9/open_feature/open_feature_evaluation_context.py` & `openfeature_sdk-0.1.0/open_feature/open_feature_evaluation_context.py`

 * *Files identical despite different names*

### Comparing `openfeature_sdk-0.0.9/open_feature/provider/no_op_provider.py` & `openfeature_sdk-0.1.0/open_feature/provider/no_op_provider.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing
 
 from open_feature.evaluation_context.evaluation_context import EvaluationContext
-from open_feature.flag_evaluation.flag_evaluation_details import FlagEvaluationDetails
 from open_feature.flag_evaluation.reason import Reason
+from open_feature.flag_evaluation.resolution_details import FlagResolutionDetails
 from open_feature.hooks.hook import Hook
 from open_feature.provider.metadata import Metadata
 from open_feature.provider.no_op_metadata import NoOpMetadata
 from open_feature.provider.provider import AbstractProvider
 
 PASSED_IN_DEFAULT = "Passed in default"
 
@@ -19,66 +19,61 @@
         return []
 
     def resolve_boolean_details(
         self,
         flag_key: str,
         default_value: bool,
         evaluation_context: typing.Optional[EvaluationContext] = None,
-    ) -> FlagEvaluationDetails[bool]:
-        return FlagEvaluationDetails(
-            flag_key=flag_key,
+    ) -> FlagResolutionDetails[bool]:
+        return FlagResolutionDetails(
             value=default_value,
             reason=Reason.DEFAULT,
             variant=PASSED_IN_DEFAULT,
         )
 
     def resolve_string_details(
         self,
         flag_key: str,
         default_value: str,
         evaluation_context: typing.Optional[EvaluationContext] = None,
-    ) -> FlagEvaluationDetails[str]:
-        return FlagEvaluationDetails(
-            flag_key=flag_key,
+    ) -> FlagResolutionDetails[str]:
+        return FlagResolutionDetails(
             value=default_value,
             reason=Reason.DEFAULT,
             variant=PASSED_IN_DEFAULT,
         )
 
     def resolve_integer_details(
         self,
         flag_key: str,
         default_value: int,
         evaluation_context: typing.Optional[EvaluationContext] = None,
-    ) -> FlagEvaluationDetails[int]:
-        return FlagEvaluationDetails(
-            flag_key=flag_key,
+    ) -> FlagResolutionDetails[int]:
+        return FlagResolutionDetails(
             value=default_value,
             reason=Reason.DEFAULT,
             variant=PASSED_IN_DEFAULT,
         )
 
     def resolve_float_details(
         self,
         flag_key: str,
         default_value: float,
         evaluation_context: typing.Optional[EvaluationContext] = None,
-    ) -> FlagEvaluationDetails[float]:
-        return FlagEvaluationDetails(
-            flag_key=flag_key,
+    ) -> FlagResolutionDetails[float]:
+        return FlagResolutionDetails(
             value=default_value,
             reason=Reason.DEFAULT,
             variant=PASSED_IN_DEFAULT,
         )
 
     def resolve_object_details(
         self,
         flag_key: str,
         default_value: typing.Union[dict, list],
         evaluation_context: typing.Optional[EvaluationContext] = None,
-    ) -> FlagEvaluationDetails[typing.Union[dict, list]]:
-        return FlagEvaluationDetails(
-            flag_key=flag_key,
+    ) -> FlagResolutionDetails[typing.Union[dict, list]]:
+        return FlagResolutionDetails(
             value=default_value,
             reason=Reason.DEFAULT,
             variant=PASSED_IN_DEFAULT,
         )
```

### Comparing `openfeature_sdk-0.0.9/open_feature/provider/provider.py` & `openfeature_sdk-0.1.0/open_feature/provider/provider.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing
 from abc import abstractmethod
 
 from open_feature.evaluation_context.evaluation_context import EvaluationContext
-from open_feature.flag_evaluation.flag_evaluation_details import FlagEvaluationDetails
+from open_feature.flag_evaluation.resolution_details import FlagResolutionDetails
 from open_feature.hooks.hook import Hook
 from open_feature.provider.metadata import Metadata
 
 
 class AbstractProvider:
     @abstractmethod
     def get_metadata(self) -> Metadata:
@@ -18,45 +18,45 @@
 
     @abstractmethod
     def resolve_boolean_details(
         self,
         flag_key: str,
         default_value: bool,
         evaluation_context: typing.Optional[EvaluationContext] = None,
-    ) -> FlagEvaluationDetails[bool]:
+    ) -> FlagResolutionDetails[bool]:
         pass
 
     @abstractmethod
     def resolve_string_details(
         self,
         flag_key: str,
         default_value: str,
         evaluation_context: typing.Optional[EvaluationContext] = None,
-    ) -> FlagEvaluationDetails[str]:
+    ) -> FlagResolutionDetails[str]:
         pass
 
     @abstractmethod
     def resolve_integer_details(
         self,
         flag_key: str,
         default_value: int,
         evaluation_context: typing.Optional[EvaluationContext] = None,
-    ) -> FlagEvaluationDetails[int]:
+    ) -> FlagResolutionDetails[int]:
         pass
 
     @abstractmethod
     def resolve_float_details(
         self,
         flag_key: str,
         default_value: float,
         evaluation_context: typing.Optional[EvaluationContext] = None,
-    ) -> FlagEvaluationDetails[float]:
+    ) -> FlagResolutionDetails[float]:
         pass
 
     @abstractmethod
     def resolve_object_details(
         self,
         flag_key: str,
         default_value: typing.Union[dict, list],
         evaluation_context: typing.Optional[EvaluationContext] = None,
-    ) -> FlagEvaluationDetails[typing.Union[dict, list]]:
+    ) -> FlagResolutionDetails[typing.Union[dict, list]]:
         pass
```

### Comparing `openfeature_sdk-0.0.9/openfeature_sdk.egg-info/PKG-INFO` & `openfeature_sdk-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openfeature-sdk
-Version: 0.0.9
+Name: openfeature_sdk
+Version: 0.1.0
 Summary: Standardizing Feature Flagging for Everyone
 Author-email: OpenFeature <openfeature-core@groups.io>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,97 +209,206 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# OpenFeature SDK for Python
+<!-- markdownlint-disable MD033 -->
+<p align="center">
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/open-feature/community/0e23508c163a6a1ac8c0ced3e4bd78faafe627c7/assets/logo/horizontal/white/openfeature-horizontal-white.svg">
+    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/open-feature/community/0e23508c163a6a1ac8c0ced3e4bd78faafe627c7/assets/logo/horizontal/black/openfeature-horizontal-black.svg">
+    <img align="center" alt="OpenFeature Logo">
+  </picture>
+</p>
+
+<h2 align="center">OpenFeature Python SDK</h2>
 
 [![PyPI version](https://badge.fury.io/py/openfeature-sdk.svg)](https://badge.fury.io/py/openfeature-sdk)
 ![Python 3.8+](https://img.shields.io/badge/python->=3.8-blue.svg)
 [![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
 [![Specification](https://img.shields.io/static/v1?label=Specification&message=v0.3.0&color=red)](https://github.com/open-feature/spec/tree/v0.3.0)
 [![on-merge](https://github.com/open-feature/python-sdk/actions/workflows/merge.yml/badge.svg)](https://github.com/open-feature/python-sdk/actions/workflows/merge.yml)
 [![codecov](https://codecov.io/gh/open-feature/python-sdk/branch/main/graph/badge.svg?token=FQ1I444HB3)](https://codecov.io/gh/open-feature/python-sdk)
 
+> ⚠️ Development is in progress, but there's not a stable release available. ⚠️
+
 This is the Python implementation of [OpenFeature](https://openfeature.dev), a vendor-agnostic abstraction library for evaluating feature flags.
 
 We support multiple data types for flags (numbers, strings, booleans, objects) as well as hooks, which can alter the lifecycle of a flag evaluation.
 
 This library is intended to be used in server-side contexts and has not been evaluated for use in mobile devices.
 
-## Usage
-
-While Boolean provides the simplest introduction, we offer a variety of flag types.
-
-```python
-# Depending on the flag type, use one of the methods below
-flag_key = "PROVIDER_FLAG"
-boolean_result = open_feature_client.get_boolean_value(key=flag_key,default_value=False)
-integer_result = open_feature_client.get_integer_value(key=flag_key,default_value=-1)
-float_result = open_feature_client.get_float_value(key=flag_key,default_value=-1)
-string_result = open_feature_client.get_string_value(key=flag_key,default_value="")
-object_result = open_feature_client.get_object_value(key=flag_key,default_value={})
-```
-
-Each provider class may have further setup required i.e. secret keys, environment variables etc
-
-## Requirements
+## 🔍 Requirements:
 
 - Python 3.8+
 
-## Installation
+## 📦 Installation:
 
 ### Add it to your build
 
 <!---x-release-please-start-version-->
 
 Pip install
 
 ```bash
-pip install openfeature-sdk==0.0.9
+pip install openfeature-sdk==0.1.0
 ```
 
 requirements.txt
 
 ```bash
-openfeature-sdk==0.0.9
+openfeature-sdk==0.1.0
 ```
 
 ```python
 pip install requirements.txt
 ```
 
 <!---x-release-please-end-->
 
+## 🌟 Features:
+
+- support for various backend [providers](https://openfeature.dev/docs/reference/concepts/provider)
+- easy integration and extension via [hooks](https://openfeature.dev/docs/reference/concepts/hooks)
+- bool, string, numeric, and object flag types
+- [context-aware](https://openfeature.dev/docs/reference/concepts/evaluation-context) evaluation
+
+## 🚀 Usage:
+
 ### Configure it
 
 In order to use the sdk there is some minor configuration. Follow the script below:
 
 ```python
 from open_feature import open_feature_api
 from open_feature.provider.no_op_provider import NoOpProvider
 
 open_feature_api.set_provider(NoOpProvider())
 open_feature_client = open_feature_api.get_client()
 ```
 
-## Contacting us
+### Basics:
 
-We hold regular meetings which you can see [here](https://github.com/open-feature/community/#meetings-and-events).
+While Boolean provides the simplest introduction, we offer a variety of flag types.
 
-We are also present on the `#openfeature` channel in the [CNCF slack](https://slack.cncf.io/).
+```python
+# Depending on the flag type, use one of the methods below
+flag_key = "PROVIDER_FLAG"
+boolean_result = open_feature_client.get_boolean_value(key=flag_key,default_value=False)
+integer_result = open_feature_client.get_integer_value(key=flag_key,default_value=-1)
+float_result = open_feature_client.get_float_value(key=flag_key,default_value=-1)
+string_result = open_feature_client.get_string_value(key=flag_key,default_value="")
+object_result = open_feature_client.get_object_value(key=flag_key,default_value={})
+```
 
-## Contributors
+You can also bind a provider to a specific client by name instead of setting that provider globally:
 
-Thanks so much to our contributors.
+```python
 
+open_feature_api.set_provider(NoOpProvider())
+```
+
+Each provider class may have further setup required i.e. secret keys, environment variables etc
+
+### Context-aware evaluation:
+
+Sometimes the value of a flag must take into account some dynamic criteria about the application or user, such as the user location, IP, email address, or the location of the server.
+In OpenFeature, we refer to this as [`targeting`](https://openfeature.dev/specification/glossary#targeting).
+If the flag system you're using supports targeting, you can provide the input data using the `EvaluationContext`.
+
+```python
+from open_feature.open_feature_api import get_client, get_provider, set_provider
+from open_feature.open_feature_evaluation_context import (
+    api_evaluation_context,
+    set_api_evaluation_context,
+)
+
+global_context = EvaluationContext(
+    targeting_key="targeting_key1", attributes={"application": "value1"}
+)
+request_context = EvaluationContext(
+    targeting_key="targeting_key2", attributes={"email": request.form['email']}
+)
+
+## set global context
+set_api_evaluation_context(first_context)
+
+# merge second context
+client = get_client(name="No-op Provider", version="0.5.2")
+client.get_string_value("email", None, request_context)
+
+```
+
+### Events
+
+TBD (See Issue [#131](https://github.com/open-feature/python-sdk/issues/131))
+
+### Providers:
+
+To develop a provider, you need to create a new project and include the OpenFeature SDK as a dependency. This can be a new repository or included in [the existing contrib repository](https://github.com/open-feature/python-sdk-contrib) available under the OpenFeature organization. Finally, you’ll then need to write the provider itself. This can be accomplished by implementing the `Provider` interface exported by the OpenFeature SDK.
+
+See [here](https://openfeature.dev/ecosystem) for a catalog of available providers.
+
+### Hooks:
+
+A hook is a mechanism that allows for adding arbitrary behavior at well-defined points of the flag evaluation life-cycle. Use cases include validating the resolved flag value, modifying or adding data to the evaluation context, logging, telemetry, and tracking.
+
+```python
+from open_feature.hooks.hook import Hook
+
+class MyHook(Hook):
+    def after(self, hook_context: HookContext, details: FlagEvaluationDetails, hints: dict):
+        print("This runs after the flag has been evaluated")
+
+
+# set global hooks at the API-level
+from open_feature.hooks import add_api_hooks
+add_api_hooks([MyHook()])
+
+# or configure them in the client
+client = OpenFeatureClient()
+client.add_hooks([MyHook()])
+```
+
+See [here](https://openfeature.dev/ecosystem) for a catalog of available hooks.
+
+### Logging:
+
+TBD
+
+## ⭐️ Support the project
+
+- Give this repo a ⭐️!
+- Follow us on social media:
+  - Twitter: [@openfeature](https://twitter.com/openfeature)
+  - LinkedIn: [OpenFeature](https://www.linkedin.com/company/openfeature/)
+- Join us on [Slack](https://cloud-native.slack.com/archives/C0344AANLA1)
+- For more check out our [community page](https://openfeature.dev/community/)
+
+## 🤝 Contributing
+
+Interested in contributing? Great, we'd love your help! To get started, take a look at the [CONTRIBUTING](CONTRIBUTING.md) guide.
+
+### Thanks to everyone that has already contributed
+
+<!-- TODO: update with correct repo -->
 <a href="https://github.com/open-feature/python-sdk/graphs/contributors">
-  <img src="https://contrib.rocks/image?repo=open-feature/python-sdk" />
+  <img src="https://contrib.rocks/image?repo=open-feature/python-sdk" alt="Pictures of the folks who have contributed to the project" />
 </a>
 
 Made with [contrib.rocks](https://contrib.rocks).
 
-### Development
+## Contacting us
+
+We hold regular meetings which you can see [here](https://github.com/open-feature/community/#meetings-and-events).
+
+We are also present on the `#openfeature` channel in the [CNCF slack](https://slack.cncf.io/).
+
+## 📜 License
+
+[Apache License 2.0](LICENSE)
+
+<!-- TODO: add FOSSA widget -->
 
-If you would like to contribute to the project, please see our [contributing](./CONTRIBUTING.md) documentation!
+[openfeature-website]: https://openfeature.dev
```

### Comparing `openfeature_sdk-0.0.9/openfeature_sdk.egg-info/SOURCES.txt` & `openfeature_sdk-0.1.0/openfeature_sdk.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 LICENSE
 pyproject.toml
 readme.md
 open_feature/__init__.py
 open_feature/open_feature_api.py
 open_feature/open_feature_client.py
 open_feature/open_feature_evaluation_context.py
+open_feature/_backports/__init__.py
+open_feature/_backports/strenum.py
 open_feature/evaluation_context/__init__.py
 open_feature/evaluation_context/evaluation_context.py
 open_feature/exception/__init__.py
 open_feature/exception/error_code.py
 open_feature/exception/exceptions.py
 open_feature/flag_evaluation/__init__.py
 open_feature/flag_evaluation/flag_evaluation_details.py
 open_feature/flag_evaluation/flag_evaluation_options.py
 open_feature/flag_evaluation/flag_type.py
 open_feature/flag_evaluation/reason.py
+open_feature/flag_evaluation/resolution_details.py
 open_feature/hooks/__init__.py
 open_feature/hooks/hook.py
 open_feature/hooks/hook_context.py
 open_feature/hooks/hook_support.py
 open_feature/hooks/hook_type.py
 open_feature/immutable_dict/__init__.py
 open_feature/immutable_dict/mapping_proxy_type.py
 open_feature/provider/__init__.py
+open_feature/provider/in_memory_provider.py
 open_feature/provider/metadata.py
 open_feature/provider/no_op_metadata.py
 open_feature/provider/no_op_provider.py
 open_feature/provider/provider.py
 openfeature_sdk.egg-info/PKG-INFO
 openfeature_sdk.egg-info/SOURCES.txt
 openfeature_sdk.egg-info/dependency_links.txt
 openfeature_sdk.egg-info/requires.txt
-openfeature_sdk.egg-info/top_level.txt
+openfeature_sdk.egg-info/top_level.txt
+tests/test_open_feature_api.py
+tests/test_open_feature_client.py
+tests/test_open_feature_evaluation_context.py
+tests/test_open_feature_flag_evaluation.py
```

### Comparing `openfeature_sdk-0.0.9/pyproject.toml` & `openfeature_sdk-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pyproject.toml
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openfeature_sdk"
-version = "0.0.9"
+version = "0.1.0"
 description = "Standardizing Feature Flagging for Everyone"
 readme = "readme.md"
 authors = [{ name = "OpenFeature", email = "openfeature-core@groups.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

