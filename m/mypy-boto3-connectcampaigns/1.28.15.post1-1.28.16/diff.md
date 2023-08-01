# Comparing `tmp/mypy-boto3-connectcampaigns-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-connectcampaigns-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connectcampaigns-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:51 2023, max compression
+gzip compressed data, was "mypy-boto3-connectcampaigns-1.28.16.tar", last modified: Tue Aug  1 11:36:32 2023, max compression
```

## Comparing `mypy-boto3-connectcampaigns-1.28.15.post1.tar` & `mypy-boto3-connectcampaigns-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:51.937088 mypy-boto3-connectcampaigns-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:41:42.000000 mypy-boto3-connectcampaigns-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-07-29 10:02:51.937088 mypy-boto3-connectcampaigns-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13831 2023-07-29 09:41:42.000000 mypy-boto3-connectcampaigns-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:51.937088 mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-29 09:41:42.000000 mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-29 09:41:42.000000 mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-29 09:41:42.000000 mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-07-29 09:41:42.000000 mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16729 2023-07-29 09:41:42.000000 mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-07-29 09:41:42.000000 mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-07-29 09:41:42.000000 mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-29 09:41:42.000000 mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-29 09:41:42.000000 mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:42.000000 mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-07-29 09:41:43.000000 mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-07-29 09:41:43.000000 mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:41:42.000000 mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:51.937088 mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-07-29 10:02:51.000000 mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-29 10:02:51.000000 mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:51.000000 mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:51.000000 mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:51.000000 mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 10:02:51.000000 mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:51.937088 mypy-boto3-connectcampaigns-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-29 09:41:42.000000 mypy-boto3-connectcampaigns-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:32.260918 mypy-boto3-connectcampaigns-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:14:15.000000 mypy-boto3-connectcampaigns-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-08-01 11:36:32.256918 mypy-boto3-connectcampaigns-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-08-01 11:14:15.000000 mypy-boto3-connectcampaigns-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:32.252918 mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-01 11:14:15.000000 mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-01 11:14:15.000000 mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-01 11:14:15.000000 mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-08-01 11:14:15.000000 mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16729 2023-08-01 11:14:15.000000 mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-08-01 11:14:16.000000 mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-08-01 11:14:16.000000 mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-08-01 11:14:15.000000 mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-01 11:14:15.000000 mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:14:15.000000 mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-08-01 11:14:16.000000 mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15091 2023-08-01 11:14:16.000000 mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:14:15.000000 mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:32.256918 mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-08-01 11:36:32.000000 mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-01 11:36:32.000000 mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:32.000000 mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:32.000000 mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:32.000000 mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 11:36:32.000000 mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:32.260918 mypy-boto3-connectcampaigns-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-01 11:14:15.000000 mypy-boto3-connectcampaigns-1.28.16/setup.py
```

### Comparing `mypy-boto3-connectcampaigns-1.28.15.post1/LICENSE` & `mypy-boto3-connectcampaigns-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.15.post1/PKG-INFO` & `mypy-boto3-connectcampaigns-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcampaigns
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ConnectCampaignService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ConnectCampaignService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 connectcampaigns type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 connectcampaigns type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcampaigns.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcampaigns)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcampaigns)](https://pepy.tech/project/mypy-boto3-connectcampaigns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCampaignService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
+[boto3.ConnectCampaignService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connectcampaigns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +74,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Typed dictionaries](#typed-dictionaries)
+    - [Type definitions](#type-definitions)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -318,32 +318,32 @@
 )
 
 
 def check_value(value: CampaignStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_connectcampaigns.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_connectcampaigns.type_defs import (
     AnswerMachineDetectionConfigTypeDef,
     InstanceIdFilterTypeDef,
     CampaignSummaryTypeDef,
     ResponseMetadataTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteConnectInstanceConfigRequestRequestTypeDef,
     DeleteInstanceOnboardingJobRequestRequestTypeDef,
     DescribeCampaignRequestRequestTypeDef,
-    DialRequestTypeDef,
+    TimestampTypeDef,
     PredictiveDialerConfigTypeDef,
     ProgressiveDialerConfigTypeDef,
     EncryptionConfigTypeDef,
     FailedCampaignStateResponseTypeDef,
     FailedRequestTypeDef,
     GetCampaignStateBatchRequestRequestTypeDef,
     SuccessfulCampaignStateResponseTypeDef,
@@ -365,33 +365,34 @@
     UpdateCampaignOutboundCallConfigRequestRequestTypeDef,
     CampaignFiltersTypeDef,
     CreateCampaignResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCampaignStateResponseTypeDef,
     ListCampaignsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PutDialRequestBatchRequestRequestTypeDef,
+    DialRequestTypeDef,
     DialerConfigTypeDef,
     InstanceConfigTypeDef,
     StartInstanceOnboardingJobRequestRequestTypeDef,
     GetCampaignStateBatchResponseTypeDef,
     GetInstanceOnboardingJobStatusResponseTypeDef,
     StartInstanceOnboardingJobResponseTypeDef,
     PutDialRequestBatchResponseTypeDef,
     ListCampaignsRequestListCampaignsPaginateTypeDef,
     ListCampaignsRequestRequestTypeDef,
+    PutDialRequestBatchRequestRequestTypeDef,
     CampaignTypeDef,
     CreateCampaignRequestRequestTypeDef,
     UpdateCampaignDialerConfigRequestRequestTypeDef,
     GetConnectInstanceConfigResponseTypeDef,
     DescribeCampaignResponseTypeDef,
 )
 
 
-def get_structure() -> AnswerMachineDetectionConfigTypeDef:
+def get_value() -> AnswerMachineDetectionConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-connectcampaigns-1.28.15.post1/README.md` & `mypy-boto3-connectcampaigns-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcampaigns.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcampaigns)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcampaigns)](https://pepy.tech/project/mypy-boto3-connectcampaigns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCampaignService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
+[boto3.ConnectCampaignService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connectcampaigns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +42,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Typed dictionaries](#typed-dictionaries)
+    - [Type definitions](#type-definitions)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -286,32 +286,32 @@
 )
 
 
 def check_value(value: CampaignStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_connectcampaigns.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_connectcampaigns.type_defs import (
     AnswerMachineDetectionConfigTypeDef,
     InstanceIdFilterTypeDef,
     CampaignSummaryTypeDef,
     ResponseMetadataTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteConnectInstanceConfigRequestRequestTypeDef,
     DeleteInstanceOnboardingJobRequestRequestTypeDef,
     DescribeCampaignRequestRequestTypeDef,
-    DialRequestTypeDef,
+    TimestampTypeDef,
     PredictiveDialerConfigTypeDef,
     ProgressiveDialerConfigTypeDef,
     EncryptionConfigTypeDef,
     FailedCampaignStateResponseTypeDef,
     FailedRequestTypeDef,
     GetCampaignStateBatchRequestRequestTypeDef,
     SuccessfulCampaignStateResponseTypeDef,
@@ -333,33 +333,34 @@
     UpdateCampaignOutboundCallConfigRequestRequestTypeDef,
     CampaignFiltersTypeDef,
     CreateCampaignResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCampaignStateResponseTypeDef,
     ListCampaignsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PutDialRequestBatchRequestRequestTypeDef,
+    DialRequestTypeDef,
     DialerConfigTypeDef,
     InstanceConfigTypeDef,
     StartInstanceOnboardingJobRequestRequestTypeDef,
     GetCampaignStateBatchResponseTypeDef,
     GetInstanceOnboardingJobStatusResponseTypeDef,
     StartInstanceOnboardingJobResponseTypeDef,
     PutDialRequestBatchResponseTypeDef,
     ListCampaignsRequestListCampaignsPaginateTypeDef,
     ListCampaignsRequestRequestTypeDef,
+    PutDialRequestBatchRequestRequestTypeDef,
     CampaignTypeDef,
     CreateCampaignRequestRequestTypeDef,
     UpdateCampaignDialerConfigRequestRequestTypeDef,
     GetConnectInstanceConfigResponseTypeDef,
     DescribeCampaignResponseTypeDef,
 )
 
 
-def get_structure() -> AnswerMachineDetectionConfigTypeDef:
+def get_value() -> AnswerMachineDetectionConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/__init__.py` & `mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/__init__.pyi` & `mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/__main__.py` & `mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConnectCampaignService 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ConnectCampaignService 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15.post1")
+    print("1.28.16")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/client.py` & `mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/client.pyi` & `mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/literals.py` & `mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/literals.pyi` & `mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/paginator.py` & `mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/paginator.pyi` & `mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/type_defs.py` & `mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_connectcampaigns.type_defs import AnswerMachineDetectionConfigTypeDef
 
-    data: AnswerMachineDetectionConfigTypeDef = {...}
+    data: AnswerMachineDetectionConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -38,15 +38,15 @@
     "InstanceIdFilterTypeDef",
     "CampaignSummaryTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteConnectInstanceConfigRequestRequestTypeDef",
     "DeleteInstanceOnboardingJobRequestRequestTypeDef",
     "DescribeCampaignRequestRequestTypeDef",
-    "DialRequestTypeDef",
+    "TimestampTypeDef",
     "PredictiveDialerConfigTypeDef",
     "ProgressiveDialerConfigTypeDef",
     "EncryptionConfigTypeDef",
     "FailedCampaignStateResponseTypeDef",
     "FailedRequestTypeDef",
     "GetCampaignStateBatchRequestRequestTypeDef",
     "SuccessfulCampaignStateResponseTypeDef",
@@ -68,24 +68,25 @@
     "UpdateCampaignOutboundCallConfigRequestRequestTypeDef",
     "CampaignFiltersTypeDef",
     "CreateCampaignResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetCampaignStateResponseTypeDef",
     "ListCampaignsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "PutDialRequestBatchRequestRequestTypeDef",
+    "DialRequestTypeDef",
     "DialerConfigTypeDef",
     "InstanceConfigTypeDef",
     "StartInstanceOnboardingJobRequestRequestTypeDef",
     "GetCampaignStateBatchResponseTypeDef",
     "GetInstanceOnboardingJobStatusResponseTypeDef",
     "StartInstanceOnboardingJobResponseTypeDef",
     "PutDialRequestBatchResponseTypeDef",
     "ListCampaignsRequestListCampaignsPaginateTypeDef",
     "ListCampaignsRequestRequestTypeDef",
+    "PutDialRequestBatchRequestRequestTypeDef",
     "CampaignTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "UpdateCampaignDialerConfigRequestRequestTypeDef",
     "GetConnectInstanceConfigResponseTypeDef",
     "DescribeCampaignResponseTypeDef",
 )
 
@@ -149,24 +150,15 @@
 DescribeCampaignRequestRequestTypeDef = TypedDict(
     "DescribeCampaignRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-DialRequestTypeDef = TypedDict(
-    "DialRequestTypeDef",
-    {
-        "attributes": Mapping[str, str],
-        "clientToken": str,
-        "expirationTime": Union[datetime, str],
-        "phoneNumber": str,
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 PredictiveDialerConfigTypeDef = TypedDict(
     "PredictiveDialerConfigTypeDef",
     {
         "bandwidthAllocation": float,
     },
 )
 
@@ -446,19 +438,21 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutDialRequestBatchRequestRequestTypeDef = TypedDict(
-    "PutDialRequestBatchRequestRequestTypeDef",
+DialRequestTypeDef = TypedDict(
+    "DialRequestTypeDef",
     {
-        "dialRequests": Sequence[DialRequestTypeDef],
-        "id": str,
+        "attributes": Mapping[str, str],
+        "clientToken": str,
+        "expirationTime": TimestampTypeDef,
+        "phoneNumber": str,
     },
 )
 
 DialerConfigTypeDef = TypedDict(
     "DialerConfigTypeDef",
     {
         "predictiveDialerConfig": PredictiveDialerConfigTypeDef,
@@ -533,14 +527,22 @@
         "filters": CampaignFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+PutDialRequestBatchRequestRequestTypeDef = TypedDict(
+    "PutDialRequestBatchRequestRequestTypeDef",
+    {
+        "dialRequests": Sequence[DialRequestTypeDef],
+        "id": str,
+    },
+)
+
 _RequiredCampaignTypeDef = TypedDict(
     "_RequiredCampaignTypeDef",
     {
         "arn": str,
         "connectInstanceId": str,
         "dialerConfig": DialerConfigTypeDef,
         "id": str,
```

### Comparing `mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns/type_defs.pyi` & `mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_connectcampaigns.type_defs import AnswerMachineDetectionConfigTypeDef
 
-    data: AnswerMachineDetectionConfigTypeDef = {...}
+    data: AnswerMachineDetectionConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -37,15 +37,15 @@
     "InstanceIdFilterTypeDef",
     "CampaignSummaryTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteConnectInstanceConfigRequestRequestTypeDef",
     "DeleteInstanceOnboardingJobRequestRequestTypeDef",
     "DescribeCampaignRequestRequestTypeDef",
-    "DialRequestTypeDef",
+    "TimestampTypeDef",
     "PredictiveDialerConfigTypeDef",
     "ProgressiveDialerConfigTypeDef",
     "EncryptionConfigTypeDef",
     "FailedCampaignStateResponseTypeDef",
     "FailedRequestTypeDef",
     "GetCampaignStateBatchRequestRequestTypeDef",
     "SuccessfulCampaignStateResponseTypeDef",
@@ -67,24 +67,25 @@
     "UpdateCampaignOutboundCallConfigRequestRequestTypeDef",
     "CampaignFiltersTypeDef",
     "CreateCampaignResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetCampaignStateResponseTypeDef",
     "ListCampaignsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "PutDialRequestBatchRequestRequestTypeDef",
+    "DialRequestTypeDef",
     "DialerConfigTypeDef",
     "InstanceConfigTypeDef",
     "StartInstanceOnboardingJobRequestRequestTypeDef",
     "GetCampaignStateBatchResponseTypeDef",
     "GetInstanceOnboardingJobStatusResponseTypeDef",
     "StartInstanceOnboardingJobResponseTypeDef",
     "PutDialRequestBatchResponseTypeDef",
     "ListCampaignsRequestListCampaignsPaginateTypeDef",
     "ListCampaignsRequestRequestTypeDef",
+    "PutDialRequestBatchRequestRequestTypeDef",
     "CampaignTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "UpdateCampaignDialerConfigRequestRequestTypeDef",
     "GetConnectInstanceConfigResponseTypeDef",
     "DescribeCampaignResponseTypeDef",
 )
 
@@ -148,24 +149,15 @@
 DescribeCampaignRequestRequestTypeDef = TypedDict(
     "DescribeCampaignRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-DialRequestTypeDef = TypedDict(
-    "DialRequestTypeDef",
-    {
-        "attributes": Mapping[str, str],
-        "clientToken": str,
-        "expirationTime": Union[datetime, str],
-        "phoneNumber": str,
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 PredictiveDialerConfigTypeDef = TypedDict(
     "PredictiveDialerConfigTypeDef",
     {
         "bandwidthAllocation": float,
     },
 )
 
@@ -437,19 +429,21 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutDialRequestBatchRequestRequestTypeDef = TypedDict(
-    "PutDialRequestBatchRequestRequestTypeDef",
+DialRequestTypeDef = TypedDict(
+    "DialRequestTypeDef",
     {
-        "dialRequests": Sequence[DialRequestTypeDef],
-        "id": str,
+        "attributes": Mapping[str, str],
+        "clientToken": str,
+        "expirationTime": TimestampTypeDef,
+        "phoneNumber": str,
     },
 )
 
 DialerConfigTypeDef = TypedDict(
     "DialerConfigTypeDef",
     {
         "predictiveDialerConfig": PredictiveDialerConfigTypeDef,
@@ -524,14 +518,22 @@
         "filters": CampaignFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+PutDialRequestBatchRequestRequestTypeDef = TypedDict(
+    "PutDialRequestBatchRequestRequestTypeDef",
+    {
+        "dialRequests": Sequence[DialRequestTypeDef],
+        "id": str,
+    },
+)
+
 _RequiredCampaignTypeDef = TypedDict(
     "_RequiredCampaignTypeDef",
     {
         "arn": str,
         "connectInstanceId": str,
         "dialerConfig": DialerConfigTypeDef,
         "id": str,
```

### Comparing `mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns.egg-info/PKG-INFO` & `mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcampaigns
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ConnectCampaignService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ConnectCampaignService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 connectcampaigns type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 connectcampaigns type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcampaigns.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcampaigns)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcampaigns)](https://pepy.tech/project/mypy-boto3-connectcampaigns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCampaignService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
+[boto3.ConnectCampaignService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connectcampaigns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +74,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Typed dictionaries](#typed-dictionaries)
+    - [Type definitions](#type-definitions)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -318,32 +318,32 @@
 )
 
 
 def check_value(value: CampaignStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_connectcampaigns.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_connectcampaigns.type_defs import (
     AnswerMachineDetectionConfigTypeDef,
     InstanceIdFilterTypeDef,
     CampaignSummaryTypeDef,
     ResponseMetadataTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteConnectInstanceConfigRequestRequestTypeDef,
     DeleteInstanceOnboardingJobRequestRequestTypeDef,
     DescribeCampaignRequestRequestTypeDef,
-    DialRequestTypeDef,
+    TimestampTypeDef,
     PredictiveDialerConfigTypeDef,
     ProgressiveDialerConfigTypeDef,
     EncryptionConfigTypeDef,
     FailedCampaignStateResponseTypeDef,
     FailedRequestTypeDef,
     GetCampaignStateBatchRequestRequestTypeDef,
     SuccessfulCampaignStateResponseTypeDef,
@@ -365,33 +365,34 @@
     UpdateCampaignOutboundCallConfigRequestRequestTypeDef,
     CampaignFiltersTypeDef,
     CreateCampaignResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCampaignStateResponseTypeDef,
     ListCampaignsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PutDialRequestBatchRequestRequestTypeDef,
+    DialRequestTypeDef,
     DialerConfigTypeDef,
     InstanceConfigTypeDef,
     StartInstanceOnboardingJobRequestRequestTypeDef,
     GetCampaignStateBatchResponseTypeDef,
     GetInstanceOnboardingJobStatusResponseTypeDef,
     StartInstanceOnboardingJobResponseTypeDef,
     PutDialRequestBatchResponseTypeDef,
     ListCampaignsRequestListCampaignsPaginateTypeDef,
     ListCampaignsRequestRequestTypeDef,
+    PutDialRequestBatchRequestRequestTypeDef,
     CampaignTypeDef,
     CreateCampaignRequestRequestTypeDef,
     UpdateCampaignDialerConfigRequestRequestTypeDef,
     GetConnectInstanceConfigResponseTypeDef,
     DescribeCampaignResponseTypeDef,
 )
 
 
-def get_structure() -> AnswerMachineDetectionConfigTypeDef:
+def get_value() -> AnswerMachineDetectionConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-connectcampaigns-1.28.15.post1/mypy_boto3_connectcampaigns.egg-info/SOURCES.txt` & `mypy-boto3-connectcampaigns-1.28.16/mypy_boto3_connectcampaigns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.15.post1/setup.py` & `mypy-boto3-connectcampaigns-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connectcampaigns",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_connectcampaigns"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConnectCampaignService 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ConnectCampaignService 1.28.16 service generated with"
+        " mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -34,15 +34,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
-    keywords="boto3 connectcampaigns type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 connectcampaigns type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_connectcampaigns": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

