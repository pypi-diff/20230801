# Comparing `tmp/mypy-boto3-ssm-contacts-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-ssm-contacts-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ssm-contacts-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:16 2023, max compression
+gzip compressed data, was "mypy-boto3-ssm-contacts-1.28.16.tar", last modified: Tue Aug  1 11:37:55 2023, max compression
```

## Comparing `mypy-boto3-ssm-contacts-1.28.15.post1.tar` & `mypy-boto3-ssm-contacts-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:16.013419 mypy-boto3-ssm-contacts-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18745 2023-07-29 10:04:16.005419 mypy-boto3-ssm-contacts-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17233 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:15.997419 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32497 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32440 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-07-29 10:00:15.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-07-29 10:00:15.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13897 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40555 2023-07-29 10:00:16.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40478 2023-07-29 10:00:15.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:16.005419 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18745 2023-07-29 10:04:15.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-29 10:04:15.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:15.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:15.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:15.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:04:15.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:16.013419 mypy-boto3-ssm-contacts-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:55.216720 mypy-boto3-ssm-contacts-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:33:49.000000 mypy-boto3-ssm-contacts-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18815 2023-08-01 11:37:55.216720 mypy-boto3-ssm-contacts-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17312 2023-08-01 11:33:49.000000 mypy-boto3-ssm-contacts-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:55.204720 mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-08-01 11:33:49.000000 mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-08-01 11:33:49.000000 mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-01 11:33:49.000000 mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32209 2023-08-01 11:33:49.000000 mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32152 2023-08-01 11:33:49.000000 mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-08-01 11:33:49.000000 mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-08-01 11:33:49.000000 mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13787 2023-08-01 11:33:49.000000 mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13774 2023-08-01 11:33:49.000000 mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:33:49.000000 mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40747 2023-08-01 11:33:50.000000 mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40670 2023-08-01 11:33:50.000000 mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:33:49.000000 mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:55.216720 mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18815 2023-08-01 11:37:54.000000 mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 11:37:55.000000 mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:54.000000 mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:54.000000 mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:54.000000 mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 11:37:54.000000 mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:55.216720 mypy-boto3-ssm-contacts-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-01 11:33:49.000000 mypy-boto3-ssm-contacts-1.28.16/setup.py
```

### Comparing `mypy-boto3-ssm-contacts-1.28.15.post1/LICENSE` & `mypy-boto3-ssm-contacts-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.15.post1/PKG-INFO` & `mypy-boto3-ssm-contacts-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-contacts
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SSMContacts 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SSMContacts 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ssm-contacts type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 ssm-contacts type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-contacts.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-contacts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-contacts)](https://pepy.tech/project/mypy-boto3-ssm-contacts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMContacts 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
+[boto3.SSMContacts 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
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
 [mypy-boto3-ssm-contacts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/).
 
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
@@ -364,33 +364,33 @@
 )
 
 
 def check_value(value: AcceptCodeValidationType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ssm_contacts.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ssm_contacts.type_defs import (
     AcceptPageRequestRequestTypeDef,
     ActivateContactChannelRequestRequestTypeDef,
     ChannelTargetInfoTypeDef,
     ContactChannelAddressTypeDef,
     ContactTargetInfoTypeDef,
     ContactTypeDef,
     HandOffTimeTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
-    CreateRotationOverrideRequestRequestTypeDef,
+    TimestampTypeDef,
     DeactivateContactChannelRequestRequestTypeDef,
     DeleteContactChannelRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
     DeleteRotationOverrideRequestRequestTypeDef,
     DeleteRotationRequestRequestTypeDef,
     DescribeEngagementRequestRequestTypeDef,
     DescribePageRequestRequestTypeDef,
@@ -399,26 +399,22 @@
     GetContactPolicyRequestRequestTypeDef,
     GetContactRequestRequestTypeDef,
     GetRotationOverrideRequestRequestTypeDef,
     GetRotationRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListContactChannelsRequestRequestTypeDef,
     ListContactsRequestRequestTypeDef,
-    TimeRangeTypeDef,
     ListPageReceiptsRequestRequestTypeDef,
     ReceiptTypeDef,
     ListPageResolutionsRequestRequestTypeDef,
     ResolutionContactTypeDef,
     ListPagesByContactRequestRequestTypeDef,
     PageTypeDef,
     ListPagesByEngagementRequestRequestTypeDef,
-    PreviewOverrideTypeDef,
-    ListRotationOverridesRequestRequestTypeDef,
     RotationOverrideTypeDef,
-    ListRotationShiftsRequestRequestTypeDef,
     ListRotationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PutContactPolicyRequestRequestTypeDef,
     ShiftDetailsTypeDef,
     SendActivationCodeRequestRequestTypeDef,
     StartEngagementRequestRequestTypeDef,
     StopEngagementRequestRequestTypeDef,
@@ -439,55 +435,62 @@
     GetContactChannelResultTypeDef,
     GetContactPolicyResultTypeDef,
     GetRotationOverrideResultTypeDef,
     ListContactsResultTypeDef,
     StartEngagementResultTypeDef,
     ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateRotationOverrideRequestRequestTypeDef,
+    ListRotationOverridesRequestRequestTypeDef,
+    ListRotationShiftsRequestRequestTypeDef,
+    PreviewOverrideTypeDef,
+    TimeRangeTypeDef,
     ListEngagementsResultTypeDef,
     ListContactChannelsRequestListContactChannelsPaginateTypeDef,
     ListContactsRequestListContactsPaginateTypeDef,
     ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
     ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
     ListPagesByContactRequestListPagesByContactPaginateTypeDef,
     ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
     ListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
     ListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
     ListRotationsRequestListRotationsPaginateTypeDef,
-    ListEngagementsRequestListEngagementsPaginateTypeDef,
-    ListEngagementsRequestRequestTypeDef,
     ListPageReceiptsResultTypeDef,
     ListPageResolutionsResultTypeDef,
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListRotationOverridesResultTypeDef,
     RotationShiftTypeDef,
     ListContactChannelsResultTypeDef,
     StageOutputTypeDef,
     StageTypeDef,
     RecurrenceSettingsOutputTypeDef,
     RecurrenceSettingsTypeDef,
+    ListEngagementsRequestListEngagementsPaginateTypeDef,
+    ListEngagementsRequestRequestTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationShiftsResultTypeDef,
     PlanOutputTypeDef,
     PlanTypeDef,
     GetRotationResultTypeDef,
     RotationTypeDef,
     CreateRotationRequestRequestTypeDef,
     ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef,
     ListPreviewRotationShiftsRequestRequestTypeDef,
+    RecurrenceSettingsUnionTypeDef,
     UpdateRotationRequestRequestTypeDef,
     GetContactResultTypeDef,
     CreateContactRequestRequestTypeDef,
+    PlanUnionTypeDef,
     UpdateContactRequestRequestTypeDef,
     ListRotationsResultTypeDef,
 )
 
 
-def get_structure() -> AcceptPageRequestRequestTypeDef:
+def get_value() -> AcceptPageRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ssm-contacts-1.28.15.post1/README.md` & `mypy-boto3-ssm-contacts-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-contacts.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-contacts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-contacts)](https://pepy.tech/project/mypy-boto3-ssm-contacts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMContacts 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
+[boto3.SSMContacts 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
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
 [mypy-boto3-ssm-contacts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/).
 
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
@@ -332,33 +332,33 @@
 )
 
 
 def check_value(value: AcceptCodeValidationType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ssm_contacts.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ssm_contacts.type_defs import (
     AcceptPageRequestRequestTypeDef,
     ActivateContactChannelRequestRequestTypeDef,
     ChannelTargetInfoTypeDef,
     ContactChannelAddressTypeDef,
     ContactTargetInfoTypeDef,
     ContactTypeDef,
     HandOffTimeTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
-    CreateRotationOverrideRequestRequestTypeDef,
+    TimestampTypeDef,
     DeactivateContactChannelRequestRequestTypeDef,
     DeleteContactChannelRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
     DeleteRotationOverrideRequestRequestTypeDef,
     DeleteRotationRequestRequestTypeDef,
     DescribeEngagementRequestRequestTypeDef,
     DescribePageRequestRequestTypeDef,
@@ -367,26 +367,22 @@
     GetContactPolicyRequestRequestTypeDef,
     GetContactRequestRequestTypeDef,
     GetRotationOverrideRequestRequestTypeDef,
     GetRotationRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListContactChannelsRequestRequestTypeDef,
     ListContactsRequestRequestTypeDef,
-    TimeRangeTypeDef,
     ListPageReceiptsRequestRequestTypeDef,
     ReceiptTypeDef,
     ListPageResolutionsRequestRequestTypeDef,
     ResolutionContactTypeDef,
     ListPagesByContactRequestRequestTypeDef,
     PageTypeDef,
     ListPagesByEngagementRequestRequestTypeDef,
-    PreviewOverrideTypeDef,
-    ListRotationOverridesRequestRequestTypeDef,
     RotationOverrideTypeDef,
-    ListRotationShiftsRequestRequestTypeDef,
     ListRotationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PutContactPolicyRequestRequestTypeDef,
     ShiftDetailsTypeDef,
     SendActivationCodeRequestRequestTypeDef,
     StartEngagementRequestRequestTypeDef,
     StopEngagementRequestRequestTypeDef,
@@ -407,55 +403,62 @@
     GetContactChannelResultTypeDef,
     GetContactPolicyResultTypeDef,
     GetRotationOverrideResultTypeDef,
     ListContactsResultTypeDef,
     StartEngagementResultTypeDef,
     ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateRotationOverrideRequestRequestTypeDef,
+    ListRotationOverridesRequestRequestTypeDef,
+    ListRotationShiftsRequestRequestTypeDef,
+    PreviewOverrideTypeDef,
+    TimeRangeTypeDef,
     ListEngagementsResultTypeDef,
     ListContactChannelsRequestListContactChannelsPaginateTypeDef,
     ListContactsRequestListContactsPaginateTypeDef,
     ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
     ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
     ListPagesByContactRequestListPagesByContactPaginateTypeDef,
     ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
     ListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
     ListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
     ListRotationsRequestListRotationsPaginateTypeDef,
-    ListEngagementsRequestListEngagementsPaginateTypeDef,
-    ListEngagementsRequestRequestTypeDef,
     ListPageReceiptsResultTypeDef,
     ListPageResolutionsResultTypeDef,
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListRotationOverridesResultTypeDef,
     RotationShiftTypeDef,
     ListContactChannelsResultTypeDef,
     StageOutputTypeDef,
     StageTypeDef,
     RecurrenceSettingsOutputTypeDef,
     RecurrenceSettingsTypeDef,
+    ListEngagementsRequestListEngagementsPaginateTypeDef,
+    ListEngagementsRequestRequestTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationShiftsResultTypeDef,
     PlanOutputTypeDef,
     PlanTypeDef,
     GetRotationResultTypeDef,
     RotationTypeDef,
     CreateRotationRequestRequestTypeDef,
     ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef,
     ListPreviewRotationShiftsRequestRequestTypeDef,
+    RecurrenceSettingsUnionTypeDef,
     UpdateRotationRequestRequestTypeDef,
     GetContactResultTypeDef,
     CreateContactRequestRequestTypeDef,
+    PlanUnionTypeDef,
     UpdateContactRequestRequestTypeDef,
     ListRotationsResultTypeDef,
 )
 
 
-def get_structure() -> AcceptPageRequestRequestTypeDef:
+def get_value() -> AcceptPageRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/__init__.py` & `mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/__init__.pyi` & `mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/__main__.py` & `mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSMContacts 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.SSMContacts 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts\nOther"
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

### Comparing `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/client.py` & `mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_ssm_contacts.client import SSMContactsClient
 
     session = Session()
     client: SSMContactsClient = session.client("ssm-contacts")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import AcceptCodeValidationType, AcceptTypeType, ChannelTypeType, ContactTypeType
 from .paginator import (
     ListContactChannelsPaginator,
     ListContactsPaginator,
@@ -54,53 +53,48 @@
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationOverridesResultTypeDef,
     ListRotationShiftsResultTypeDef,
     ListRotationsResultTypeDef,
     ListTagsForResourceResultTypeDef,
-    PlanOutputTypeDef,
-    PlanTypeDef,
+    PlanUnionTypeDef,
     PreviewOverrideTypeDef,
-    RecurrenceSettingsOutputTypeDef,
-    RecurrenceSettingsTypeDef,
+    RecurrenceSettingsUnionTypeDef,
     StartEngagementResultTypeDef,
     TagTypeDef,
     TimeRangeTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SSMContactsClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     DataEncryptionException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class SSMContactsClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/)
     """
 
     meta: ClientMeta
@@ -109,15 +103,14 @@
     def exceptions(self) -> Exceptions:
         """
         SSMContactsClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#exceptions)
         """
-
     def accept_page(
         self,
         *,
         PageId: str,
         AcceptType: AcceptTypeType,
         AcceptCode: str,
         ContactChannelId: str = ...,
@@ -126,60 +119,55 @@
     ) -> Dict[str, Any]:
         """
         Used to acknowledge an engagement to a contact channel during an incident.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.accept_page)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#accept_page)
         """
-
     def activate_contact_channel(
         self, *, ContactChannelId: str, ActivationCode: str
     ) -> Dict[str, Any]:
         """
         Activates a contact's contact channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.activate_contact_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#activate_contact_channel)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#close)
         """
-
     def create_contact(
         self,
         *,
         Alias: str,
         Type: ContactTypeType,
-        Plan: Union[PlanTypeDef, PlanOutputTypeDef],
+        Plan: PlanUnionTypeDef,
         DisplayName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> CreateContactResultTypeDef:
         """
         Contacts are either the contacts that Incident Manager engages during an
         incident or the escalation plans that Incident Manager uses to engage contacts
         in phases during an incident.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.create_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#create_contact)
         """
-
     def create_contact_channel(
         self,
         *,
         ContactId: str,
         Name: str,
         Type: ChannelTypeType,
         DeliveryAddress: ContactChannelAddressTypeDef,
@@ -189,333 +177,303 @@
         """
         A contact channel is the method that Incident Manager uses to engage your
         contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.create_contact_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#create_contact_channel)
         """
-
     def create_rotation(
         self,
         *,
         Name: str,
         ContactIds: Sequence[str],
         TimeZoneId: str,
-        Recurrence: Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef],
-        StartTime: Union[datetime, str] = ...,
+        Recurrence: RecurrenceSettingsUnionTypeDef,
+        StartTime: TimestampTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> CreateRotationResultTypeDef:
         """
         Creates a rotation in an on-call schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.create_rotation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#create_rotation)
         """
-
     def create_rotation_override(
         self,
         *,
         RotationId: str,
         NewContactIds: Sequence[str],
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         IdempotencyToken: str = ...
     ) -> CreateRotationOverrideResultTypeDef:
         """
         Creates an override for a rotation in an on-call schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.create_rotation_override)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#create_rotation_override)
         """
-
     def deactivate_contact_channel(self, *, ContactChannelId: str) -> Dict[str, Any]:
         """
         To no longer receive Incident Manager engagements to a contact channel, you can
         deactivate the channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.deactivate_contact_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#deactivate_contact_channel)
         """
-
     def delete_contact(self, *, ContactId: str) -> Dict[str, Any]:
         """
         To remove a contact from Incident Manager, you can delete the contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.delete_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#delete_contact)
         """
-
     def delete_contact_channel(self, *, ContactChannelId: str) -> Dict[str, Any]:
         """
         To no longer receive engagements on a contact channel, you can delete the
         channel from a contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.delete_contact_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#delete_contact_channel)
         """
-
     def delete_rotation(self, *, RotationId: str) -> Dict[str, Any]:
         """
         Deletes a rotation from the system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.delete_rotation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#delete_rotation)
         """
-
     def delete_rotation_override(
         self, *, RotationId: str, RotationOverrideId: str
     ) -> Dict[str, Any]:
         """
         Deletes an existing override for an on-call rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.delete_rotation_override)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#delete_rotation_override)
         """
-
     def describe_engagement(self, *, EngagementId: str) -> DescribeEngagementResultTypeDef:
         """
         Incident Manager uses engagements to engage contacts and escalation plans during
         an incident.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.describe_engagement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#describe_engagement)
         """
-
     def describe_page(self, *, PageId: str) -> DescribePageResultTypeDef:
         """
         Lists details of the engagement to a contact channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.describe_page)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#describe_page)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#generate_presigned_url)
         """
-
     def get_contact(self, *, ContactId: str) -> GetContactResultTypeDef:
         """
         Retrieves information about the specified contact or escalation plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_contact)
         """
-
     def get_contact_channel(self, *, ContactChannelId: str) -> GetContactChannelResultTypeDef:
         """
         List details about a specific contact channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_contact_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_contact_channel)
         """
-
     def get_contact_policy(self, *, ContactArn: str) -> GetContactPolicyResultTypeDef:
         """
         Retrieves the resource policies attached to the specified contact or escalation
         plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_contact_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_contact_policy)
         """
-
     def get_rotation(self, *, RotationId: str) -> GetRotationResultTypeDef:
         """
         Retrieves information about an on-call rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_rotation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_rotation)
         """
-
     def get_rotation_override(
         self, *, RotationId: str, RotationOverrideId: str
     ) -> GetRotationOverrideResultTypeDef:
         """
         Retrieves information about an override to an on-call rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_rotation_override)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_rotation_override)
         """
-
     def list_contact_channels(
         self, *, ContactId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListContactChannelsResultTypeDef:
         """
         Lists all contact channels for the specified contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_contact_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_contact_channels)
         """
-
     def list_contacts(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         AliasPrefix: str = ...,
         Type: ContactTypeType = ...
     ) -> ListContactsResultTypeDef:
         """
         Lists all contacts and escalation plans in Incident Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_contacts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_contacts)
         """
-
     def list_engagements(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         IncidentId: str = ...,
         TimeRangeValue: TimeRangeTypeDef = ...
     ) -> ListEngagementsResultTypeDef:
         """
         Lists all engagements that have happened in an incident.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_engagements)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_engagements)
         """
-
     def list_page_receipts(
         self, *, PageId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListPageReceiptsResultTypeDef:
         """
         Lists all of the engagements to contact channels that have been acknowledged.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_page_receipts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_page_receipts)
         """
-
     def list_page_resolutions(
         self, *, PageId: str, NextToken: str = ...
     ) -> ListPageResolutionsResultTypeDef:
         """
         Returns the resolution path of an engagement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_page_resolutions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_page_resolutions)
         """
-
     def list_pages_by_contact(
         self, *, ContactId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListPagesByContactResultTypeDef:
         """
         Lists the engagements to a contact's contact channels.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_pages_by_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_pages_by_contact)
         """
-
     def list_pages_by_engagement(
         self, *, EngagementId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListPagesByEngagementResultTypeDef:
         """
         Lists the engagements to contact channels that occurred by engaging a contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_pages_by_engagement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_pages_by_engagement)
         """
-
     def list_preview_rotation_shifts(
         self,
         *,
-        EndTime: Union[datetime, str],
+        EndTime: TimestampTypeDef,
         Members: Sequence[str],
         TimeZoneId: str,
-        Recurrence: Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef],
-        RotationStartTime: Union[datetime, str] = ...,
-        StartTime: Union[datetime, str] = ...,
+        Recurrence: RecurrenceSettingsUnionTypeDef,
+        RotationStartTime: TimestampTypeDef = ...,
+        StartTime: TimestampTypeDef = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListPreviewRotationShiftsResultTypeDef:
         """
         Returns a list of shifts based on rotation configuration parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_preview_rotation_shifts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_preview_rotation_shifts)
         """
-
     def list_rotation_overrides(
         self,
         *,
         RotationId: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListRotationOverridesResultTypeDef:
         """
         Retrieves a list of overrides currently specified for an on-call rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_rotation_overrides)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_rotation_overrides)
         """
-
     def list_rotation_shifts(
         self,
         *,
         RotationId: str,
-        EndTime: Union[datetime, str],
-        StartTime: Union[datetime, str] = ...,
+        EndTime: TimestampTypeDef,
+        StartTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListRotationShiftsResultTypeDef:
         """
         Returns a list of shifts generated by an existing rotation in the system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_rotation_shifts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_rotation_shifts)
         """
-
     def list_rotations(
         self, *, RotationNamePrefix: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListRotationsResultTypeDef:
         """
         Retrieves a list of on-call rotations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_rotations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_rotations)
         """
-
     def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResultTypeDef:
         """
         Lists the tags of an escalation plan or contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_tags_for_resource)
         """
-
     def put_contact_policy(self, *, ContactArn: str, Policy: str) -> Dict[str, Any]:
         """
         Adds a resource policy to the specified contact or escalation plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.put_contact_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#put_contact_policy)
         """
-
     def send_activation_code(self, *, ContactChannelId: str) -> Dict[str, Any]:
         """
         Sends an activation code to a contact channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.send_activation_code)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#send_activation_code)
         """
-
     def start_engagement(
         self,
         *,
         ContactId: str,
         Sender: str,
         Subject: str,
         Content: str,
@@ -526,171 +484,150 @@
     ) -> StartEngagementResultTypeDef:
         """
         Starts an engagement to a contact or escalation plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.start_engagement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#start_engagement)
         """
-
     def stop_engagement(self, *, EngagementId: str, Reason: str = ...) -> Dict[str, Any]:
         """
         Stops an engagement before it finishes the final stage of the escalation plan or
         engagement plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.stop_engagement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#stop_engagement)
         """
-
     def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Tags a contact or escalation plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#tag_resource)
         """
-
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#untag_resource)
         """
-
     def update_contact(
-        self,
-        *,
-        ContactId: str,
-        DisplayName: str = ...,
-        Plan: Union[PlanTypeDef, PlanOutputTypeDef] = ...
+        self, *, ContactId: str, DisplayName: str = ..., Plan: PlanUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the contact or escalation plan specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.update_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#update_contact)
         """
-
     def update_contact_channel(
         self,
         *,
         ContactChannelId: str,
         Name: str = ...,
         DeliveryAddress: ContactChannelAddressTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a contact's contact channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.update_contact_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#update_contact_channel)
         """
-
     def update_rotation(
         self,
         *,
         RotationId: str,
-        Recurrence: Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef],
+        Recurrence: RecurrenceSettingsUnionTypeDef,
         ContactIds: Sequence[str] = ...,
-        StartTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
         TimeZoneId: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the information specified for an on-call rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.update_rotation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#update_rotation)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_contact_channels"]
     ) -> ListContactChannelsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_contacts"]) -> ListContactsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_engagements"]
     ) -> ListEngagementsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_page_receipts"]
     ) -> ListPageReceiptsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_page_resolutions"]
     ) -> ListPageResolutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_pages_by_contact"]
     ) -> ListPagesByContactPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_pages_by_engagement"]
     ) -> ListPagesByEngagementPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_preview_rotation_shifts"]
     ) -> ListPreviewRotationShiftsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_rotation_overrides"]
     ) -> ListRotationOverridesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_rotation_shifts"]
     ) -> ListRotationShiftsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_rotations"]) -> ListRotationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/client.pyi` & `mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_ssm_contacts.client import SSMContactsClient
 
     session = Session()
     client: SSMContactsClient = session.client("ssm-contacts")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import AcceptCodeValidationType, AcceptTypeType, ChannelTypeType, ContactTypeType
 from .paginator import (
     ListContactChannelsPaginator,
     ListContactsPaginator,
@@ -54,49 +53,52 @@
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationOverridesResultTypeDef,
     ListRotationShiftsResultTypeDef,
     ListRotationsResultTypeDef,
     ListTagsForResourceResultTypeDef,
-    PlanOutputTypeDef,
-    PlanTypeDef,
+    PlanUnionTypeDef,
     PreviewOverrideTypeDef,
-    RecurrenceSettingsOutputTypeDef,
-    RecurrenceSettingsTypeDef,
+    RecurrenceSettingsUnionTypeDef,
     StartEngagementResultTypeDef,
     TagTypeDef,
     TimeRangeTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("SSMContactsClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     DataEncryptionException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class SSMContactsClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/)
     """
 
     meta: ClientMeta
@@ -105,14 +107,15 @@
     def exceptions(self) -> Exceptions:
         """
         SSMContactsClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#exceptions)
         """
+
     def accept_page(
         self,
         *,
         PageId: str,
         AcceptType: AcceptTypeType,
         AcceptCode: str,
         ContactChannelId: str = ...,
@@ -121,55 +124,60 @@
     ) -> Dict[str, Any]:
         """
         Used to acknowledge an engagement to a contact channel during an incident.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.accept_page)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#accept_page)
         """
+
     def activate_contact_channel(
         self, *, ContactChannelId: str, ActivationCode: str
     ) -> Dict[str, Any]:
         """
         Activates a contact's contact channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.activate_contact_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#activate_contact_channel)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#close)
         """
+
     def create_contact(
         self,
         *,
         Alias: str,
         Type: ContactTypeType,
-        Plan: Union[PlanTypeDef, PlanOutputTypeDef],
+        Plan: PlanUnionTypeDef,
         DisplayName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> CreateContactResultTypeDef:
         """
         Contacts are either the contacts that Incident Manager engages during an
         incident or the escalation plans that Incident Manager uses to engage contacts
         in phases during an incident.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.create_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#create_contact)
         """
+
     def create_contact_channel(
         self,
         *,
         ContactId: str,
         Name: str,
         Type: ChannelTypeType,
         DeliveryAddress: ContactChannelAddressTypeDef,
@@ -179,303 +187,333 @@
         """
         A contact channel is the method that Incident Manager uses to engage your
         contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.create_contact_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#create_contact_channel)
         """
+
     def create_rotation(
         self,
         *,
         Name: str,
         ContactIds: Sequence[str],
         TimeZoneId: str,
-        Recurrence: Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef],
-        StartTime: Union[datetime, str] = ...,
+        Recurrence: RecurrenceSettingsUnionTypeDef,
+        StartTime: TimestampTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> CreateRotationResultTypeDef:
         """
         Creates a rotation in an on-call schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.create_rotation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#create_rotation)
         """
+
     def create_rotation_override(
         self,
         *,
         RotationId: str,
         NewContactIds: Sequence[str],
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         IdempotencyToken: str = ...
     ) -> CreateRotationOverrideResultTypeDef:
         """
         Creates an override for a rotation in an on-call schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.create_rotation_override)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#create_rotation_override)
         """
+
     def deactivate_contact_channel(self, *, ContactChannelId: str) -> Dict[str, Any]:
         """
         To no longer receive Incident Manager engagements to a contact channel, you can
         deactivate the channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.deactivate_contact_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#deactivate_contact_channel)
         """
+
     def delete_contact(self, *, ContactId: str) -> Dict[str, Any]:
         """
         To remove a contact from Incident Manager, you can delete the contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.delete_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#delete_contact)
         """
+
     def delete_contact_channel(self, *, ContactChannelId: str) -> Dict[str, Any]:
         """
         To no longer receive engagements on a contact channel, you can delete the
         channel from a contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.delete_contact_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#delete_contact_channel)
         """
+
     def delete_rotation(self, *, RotationId: str) -> Dict[str, Any]:
         """
         Deletes a rotation from the system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.delete_rotation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#delete_rotation)
         """
+
     def delete_rotation_override(
         self, *, RotationId: str, RotationOverrideId: str
     ) -> Dict[str, Any]:
         """
         Deletes an existing override for an on-call rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.delete_rotation_override)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#delete_rotation_override)
         """
+
     def describe_engagement(self, *, EngagementId: str) -> DescribeEngagementResultTypeDef:
         """
         Incident Manager uses engagements to engage contacts and escalation plans during
         an incident.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.describe_engagement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#describe_engagement)
         """
+
     def describe_page(self, *, PageId: str) -> DescribePageResultTypeDef:
         """
         Lists details of the engagement to a contact channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.describe_page)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#describe_page)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#generate_presigned_url)
         """
+
     def get_contact(self, *, ContactId: str) -> GetContactResultTypeDef:
         """
         Retrieves information about the specified contact or escalation plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_contact)
         """
+
     def get_contact_channel(self, *, ContactChannelId: str) -> GetContactChannelResultTypeDef:
         """
         List details about a specific contact channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_contact_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_contact_channel)
         """
+
     def get_contact_policy(self, *, ContactArn: str) -> GetContactPolicyResultTypeDef:
         """
         Retrieves the resource policies attached to the specified contact or escalation
         plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_contact_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_contact_policy)
         """
+
     def get_rotation(self, *, RotationId: str) -> GetRotationResultTypeDef:
         """
         Retrieves information about an on-call rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_rotation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_rotation)
         """
+
     def get_rotation_override(
         self, *, RotationId: str, RotationOverrideId: str
     ) -> GetRotationOverrideResultTypeDef:
         """
         Retrieves information about an override to an on-call rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_rotation_override)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_rotation_override)
         """
+
     def list_contact_channels(
         self, *, ContactId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListContactChannelsResultTypeDef:
         """
         Lists all contact channels for the specified contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_contact_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_contact_channels)
         """
+
     def list_contacts(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         AliasPrefix: str = ...,
         Type: ContactTypeType = ...
     ) -> ListContactsResultTypeDef:
         """
         Lists all contacts and escalation plans in Incident Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_contacts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_contacts)
         """
+
     def list_engagements(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         IncidentId: str = ...,
         TimeRangeValue: TimeRangeTypeDef = ...
     ) -> ListEngagementsResultTypeDef:
         """
         Lists all engagements that have happened in an incident.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_engagements)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_engagements)
         """
+
     def list_page_receipts(
         self, *, PageId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListPageReceiptsResultTypeDef:
         """
         Lists all of the engagements to contact channels that have been acknowledged.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_page_receipts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_page_receipts)
         """
+
     def list_page_resolutions(
         self, *, PageId: str, NextToken: str = ...
     ) -> ListPageResolutionsResultTypeDef:
         """
         Returns the resolution path of an engagement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_page_resolutions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_page_resolutions)
         """
+
     def list_pages_by_contact(
         self, *, ContactId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListPagesByContactResultTypeDef:
         """
         Lists the engagements to a contact's contact channels.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_pages_by_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_pages_by_contact)
         """
+
     def list_pages_by_engagement(
         self, *, EngagementId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListPagesByEngagementResultTypeDef:
         """
         Lists the engagements to contact channels that occurred by engaging a contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_pages_by_engagement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_pages_by_engagement)
         """
+
     def list_preview_rotation_shifts(
         self,
         *,
-        EndTime: Union[datetime, str],
+        EndTime: TimestampTypeDef,
         Members: Sequence[str],
         TimeZoneId: str,
-        Recurrence: Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef],
-        RotationStartTime: Union[datetime, str] = ...,
-        StartTime: Union[datetime, str] = ...,
+        Recurrence: RecurrenceSettingsUnionTypeDef,
+        RotationStartTime: TimestampTypeDef = ...,
+        StartTime: TimestampTypeDef = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListPreviewRotationShiftsResultTypeDef:
         """
         Returns a list of shifts based on rotation configuration parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_preview_rotation_shifts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_preview_rotation_shifts)
         """
+
     def list_rotation_overrides(
         self,
         *,
         RotationId: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListRotationOverridesResultTypeDef:
         """
         Retrieves a list of overrides currently specified for an on-call rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_rotation_overrides)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_rotation_overrides)
         """
+
     def list_rotation_shifts(
         self,
         *,
         RotationId: str,
-        EndTime: Union[datetime, str],
-        StartTime: Union[datetime, str] = ...,
+        EndTime: TimestampTypeDef,
+        StartTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListRotationShiftsResultTypeDef:
         """
         Returns a list of shifts generated by an existing rotation in the system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_rotation_shifts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_rotation_shifts)
         """
+
     def list_rotations(
         self, *, RotationNamePrefix: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListRotationsResultTypeDef:
         """
         Retrieves a list of on-call rotations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_rotations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_rotations)
         """
+
     def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResultTypeDef:
         """
         Lists the tags of an escalation plan or contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#list_tags_for_resource)
         """
+
     def put_contact_policy(self, *, ContactArn: str, Policy: str) -> Dict[str, Any]:
         """
         Adds a resource policy to the specified contact or escalation plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.put_contact_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#put_contact_policy)
         """
+
     def send_activation_code(self, *, ContactChannelId: str) -> Dict[str, Any]:
         """
         Sends an activation code to a contact channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.send_activation_code)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#send_activation_code)
         """
+
     def start_engagement(
         self,
         *,
         ContactId: str,
         Sender: str,
         Subject: str,
         Content: str,
@@ -486,154 +524,167 @@
     ) -> StartEngagementResultTypeDef:
         """
         Starts an engagement to a contact or escalation plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.start_engagement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#start_engagement)
         """
+
     def stop_engagement(self, *, EngagementId: str, Reason: str = ...) -> Dict[str, Any]:
         """
         Stops an engagement before it finishes the final stage of the escalation plan or
         engagement plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.stop_engagement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#stop_engagement)
         """
+
     def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Tags a contact or escalation plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#tag_resource)
         """
+
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#untag_resource)
         """
+
     def update_contact(
-        self,
-        *,
-        ContactId: str,
-        DisplayName: str = ...,
-        Plan: Union[PlanTypeDef, PlanOutputTypeDef] = ...
+        self, *, ContactId: str, DisplayName: str = ..., Plan: PlanUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the contact or escalation plan specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.update_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#update_contact)
         """
+
     def update_contact_channel(
         self,
         *,
         ContactChannelId: str,
         Name: str = ...,
         DeliveryAddress: ContactChannelAddressTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a contact's contact channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.update_contact_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#update_contact_channel)
         """
+
     def update_rotation(
         self,
         *,
         RotationId: str,
-        Recurrence: Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef],
+        Recurrence: RecurrenceSettingsUnionTypeDef,
         ContactIds: Sequence[str] = ...,
-        StartTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
         TimeZoneId: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the information specified for an on-call rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.update_rotation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#update_rotation)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_contact_channels"]
     ) -> ListContactChannelsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_contacts"]) -> ListContactsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_engagements"]
     ) -> ListEngagementsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_page_receipts"]
     ) -> ListPageReceiptsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_page_resolutions"]
     ) -> ListPageResolutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_pages_by_contact"]
     ) -> ListPagesByContactPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_pages_by_engagement"]
     ) -> ListPagesByEngagementPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_preview_rotation_shifts"]
     ) -> ListPreviewRotationShiftsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_rotation_overrides"]
     ) -> ListRotationOverridesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_rotation_shifts"]
     ) -> ListRotationShiftsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_rotations"]) -> ListRotationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/literals.py` & `mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/literals.pyi` & `mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/paginator.py` & `mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,15 @@
     list_pages_by_engagement_paginator: ListPagesByEngagementPaginator = client.get_paginator("list_pages_by_engagement")
     list_preview_rotation_shifts_paginator: ListPreviewRotationShiftsPaginator = client.get_paginator("list_preview_rotation_shifts")
     list_rotation_overrides_paginator: ListRotationOverridesPaginator = client.get_paginator("list_rotation_overrides")
     list_rotation_shifts_paginator: ListRotationShiftsPaginator = client.get_paginator("list_rotation_shifts")
     list_rotations_paginator: ListRotationsPaginator = client.get_paginator("list_rotations")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ContactTypeType
 from .type_defs import (
     ListContactChannelsResultTypeDef,
     ListContactsResultTypeDef,
@@ -55,17 +54,17 @@
     ListPagesByEngagementResultTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationOverridesResultTypeDef,
     ListRotationShiftsResultTypeDef,
     ListRotationsResultTypeDef,
     PaginatorConfigTypeDef,
     PreviewOverrideTypeDef,
-    RecurrenceSettingsOutputTypeDef,
-    RecurrenceSettingsTypeDef,
+    RecurrenceSettingsUnionTypeDef,
     TimeRangeTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListContactChannelsPaginator",
     "ListContactsPaginator",
     "ListEngagementsPaginator",
     "ListPageReceiptsPaginator",
@@ -207,20 +206,20 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpreviewrotationshiftspaginator)
     """
 
     def paginate(
         self,
         *,
-        EndTime: Union[datetime, str],
+        EndTime: TimestampTypeDef,
         Members: Sequence[str],
         TimeZoneId: str,
-        Recurrence: Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef],
-        RotationStartTime: Union[datetime, str] = ...,
-        StartTime: Union[datetime, str] = ...,
+        Recurrence: RecurrenceSettingsUnionTypeDef,
+        RotationStartTime: TimestampTypeDef = ...,
+        StartTime: TimestampTypeDef = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPreviewRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpreviewrotationshiftspaginator)
         """
@@ -232,16 +231,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationoverridespaginator)
     """
 
     def paginate(
         self,
         *,
         RotationId: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRotationOverridesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationOverrides.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationoverridespaginator)
         """
 
@@ -252,16 +251,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationshiftspaginator)
     """
 
     def paginate(
         self,
         *,
         RotationId: str,
-        EndTime: Union[datetime, str],
-        StartTime: Union[datetime, str] = ...,
+        EndTime: TimestampTypeDef,
+        StartTime: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationShifts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationshiftspaginator)
         """
```

### Comparing `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/paginator.pyi` & `mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -35,16 +35,15 @@
     list_pages_by_engagement_paginator: ListPagesByEngagementPaginator = client.get_paginator("list_pages_by_engagement")
     list_preview_rotation_shifts_paginator: ListPreviewRotationShiftsPaginator = client.get_paginator("list_preview_rotation_shifts")
     list_rotation_overrides_paginator: ListRotationOverridesPaginator = client.get_paginator("list_rotation_overrides")
     list_rotation_shifts_paginator: ListRotationShiftsPaginator = client.get_paginator("list_rotation_shifts")
     list_rotations_paginator: ListRotationsPaginator = client.get_paginator("list_rotations")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ContactTypeType
 from .type_defs import (
     ListContactChannelsResultTypeDef,
     ListContactsResultTypeDef,
@@ -55,17 +54,17 @@
     ListPagesByEngagementResultTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationOverridesResultTypeDef,
     ListRotationShiftsResultTypeDef,
     ListRotationsResultTypeDef,
     PaginatorConfigTypeDef,
     PreviewOverrideTypeDef,
-    RecurrenceSettingsOutputTypeDef,
-    RecurrenceSettingsTypeDef,
+    RecurrenceSettingsUnionTypeDef,
     TimeRangeTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListContactChannelsPaginator",
     "ListContactsPaginator",
     "ListEngagementsPaginator",
     "ListPageReceiptsPaginator",
@@ -197,20 +196,20 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpreviewrotationshiftspaginator)
     """
 
     def paginate(
         self,
         *,
-        EndTime: Union[datetime, str],
+        EndTime: TimestampTypeDef,
         Members: Sequence[str],
         TimeZoneId: str,
-        Recurrence: Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef],
-        RotationStartTime: Union[datetime, str] = ...,
-        StartTime: Union[datetime, str] = ...,
+        Recurrence: RecurrenceSettingsUnionTypeDef,
+        RotationStartTime: TimestampTypeDef = ...,
+        StartTime: TimestampTypeDef = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPreviewRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpreviewrotationshiftspaginator)
         """
@@ -221,16 +220,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationoverridespaginator)
     """
 
     def paginate(
         self,
         *,
         RotationId: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRotationOverridesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationOverrides.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationoverridespaginator)
         """
 
@@ -240,16 +239,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationshiftspaginator)
     """
 
     def paginate(
         self,
         *,
         RotationId: str,
-        EndTime: Union[datetime, str],
-        StartTime: Union[datetime, str] = ...,
+        EndTime: TimestampTypeDef,
+        StartTime: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationShifts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationshiftspaginator)
         """
```

### Comparing `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/type_defs.py` & `mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_ssm_contacts.type_defs import AcceptPageRequestRequestTypeDef
 
-    data: AcceptPageRequestRequestTypeDef = {...}
+    data: AcceptPageRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -38,15 +38,15 @@
     "ChannelTargetInfoTypeDef",
     "ContactChannelAddressTypeDef",
     "ContactTargetInfoTypeDef",
     "ContactTypeDef",
     "HandOffTimeTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
-    "CreateRotationOverrideRequestRequestTypeDef",
+    "TimestampTypeDef",
     "DeactivateContactChannelRequestRequestTypeDef",
     "DeleteContactChannelRequestRequestTypeDef",
     "DeleteContactRequestRequestTypeDef",
     "DeleteRotationOverrideRequestRequestTypeDef",
     "DeleteRotationRequestRequestTypeDef",
     "DescribeEngagementRequestRequestTypeDef",
     "DescribePageRequestRequestTypeDef",
@@ -55,26 +55,22 @@
     "GetContactPolicyRequestRequestTypeDef",
     "GetContactRequestRequestTypeDef",
     "GetRotationOverrideRequestRequestTypeDef",
     "GetRotationRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListContactChannelsRequestRequestTypeDef",
     "ListContactsRequestRequestTypeDef",
-    "TimeRangeTypeDef",
     "ListPageReceiptsRequestRequestTypeDef",
     "ReceiptTypeDef",
     "ListPageResolutionsRequestRequestTypeDef",
     "ResolutionContactTypeDef",
     "ListPagesByContactRequestRequestTypeDef",
     "PageTypeDef",
     "ListPagesByEngagementRequestRequestTypeDef",
-    "PreviewOverrideTypeDef",
-    "ListRotationOverridesRequestRequestTypeDef",
     "RotationOverrideTypeDef",
-    "ListRotationShiftsRequestRequestTypeDef",
     "ListRotationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutContactPolicyRequestRequestTypeDef",
     "ShiftDetailsTypeDef",
     "SendActivationCodeRequestRequestTypeDef",
     "StartEngagementRequestRequestTypeDef",
     "StopEngagementRequestRequestTypeDef",
@@ -95,49 +91,56 @@
     "GetContactChannelResultTypeDef",
     "GetContactPolicyResultTypeDef",
     "GetRotationOverrideResultTypeDef",
     "ListContactsResultTypeDef",
     "StartEngagementResultTypeDef",
     "ListTagsForResourceResultTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateRotationOverrideRequestRequestTypeDef",
+    "ListRotationOverridesRequestRequestTypeDef",
+    "ListRotationShiftsRequestRequestTypeDef",
+    "PreviewOverrideTypeDef",
+    "TimeRangeTypeDef",
     "ListEngagementsResultTypeDef",
     "ListContactChannelsRequestListContactChannelsPaginateTypeDef",
     "ListContactsRequestListContactsPaginateTypeDef",
     "ListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
     "ListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
     "ListPagesByContactRequestListPagesByContactPaginateTypeDef",
     "ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
     "ListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
     "ListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
     "ListRotationsRequestListRotationsPaginateTypeDef",
-    "ListEngagementsRequestListEngagementsPaginateTypeDef",
-    "ListEngagementsRequestRequestTypeDef",
     "ListPageReceiptsResultTypeDef",
     "ListPageResolutionsResultTypeDef",
     "ListPagesByContactResultTypeDef",
     "ListPagesByEngagementResultTypeDef",
     "ListRotationOverridesResultTypeDef",
     "RotationShiftTypeDef",
     "ListContactChannelsResultTypeDef",
     "StageOutputTypeDef",
     "StageTypeDef",
     "RecurrenceSettingsOutputTypeDef",
     "RecurrenceSettingsTypeDef",
+    "ListEngagementsRequestListEngagementsPaginateTypeDef",
+    "ListEngagementsRequestRequestTypeDef",
     "ListPreviewRotationShiftsResultTypeDef",
     "ListRotationShiftsResultTypeDef",
     "PlanOutputTypeDef",
     "PlanTypeDef",
     "GetRotationResultTypeDef",
     "RotationTypeDef",
     "CreateRotationRequestRequestTypeDef",
     "ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     "ListPreviewRotationShiftsRequestRequestTypeDef",
+    "RecurrenceSettingsUnionTypeDef",
     "UpdateRotationRequestRequestTypeDef",
     "GetContactResultTypeDef",
     "CreateContactRequestRequestTypeDef",
+    "PlanUnionTypeDef",
     "UpdateContactRequestRequestTypeDef",
     "ListRotationsResultTypeDef",
 )
 
 _RequiredAcceptPageRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptPageRequestRequestTypeDef",
     {
@@ -266,39 +269,15 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-_RequiredCreateRotationOverrideRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRotationOverrideRequestRequestTypeDef",
-    {
-        "RotationId": str,
-        "NewContactIds": Sequence[str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalCreateRotationOverrideRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRotationOverrideRequestRequestTypeDef",
-    {
-        "IdempotencyToken": str,
-    },
-    total=False,
-)
-
-
-class CreateRotationOverrideRequestRequestTypeDef(
-    _RequiredCreateRotationOverrideRequestRequestTypeDef,
-    _OptionalCreateRotationOverrideRequestRequestTypeDef,
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 DeactivateContactChannelRequestRequestTypeDef = TypedDict(
     "DeactivateContactChannelRequestRequestTypeDef",
     {
         "ContactChannelId": str,
     },
 )
 
@@ -444,23 +423,14 @@
         "MaxResults": int,
         "AliasPrefix": str,
         "Type": ContactTypeType,
     },
     total=False,
 )
 
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredListPageReceiptsRequestRequestTypeDef = TypedDict(
     "_RequiredListPageReceiptsRequestRequestTypeDef",
     {
         "PageId": str,
     },
 )
 _OptionalListPageReceiptsRequestRequestTypeDef = TypedDict(
@@ -611,85 +581,25 @@
 class ListPagesByEngagementRequestRequestTypeDef(
     _RequiredListPagesByEngagementRequestRequestTypeDef,
     _OptionalListPagesByEngagementRequestRequestTypeDef,
 ):
     pass
 
 
-PreviewOverrideTypeDef = TypedDict(
-    "PreviewOverrideTypeDef",
-    {
-        "NewMembers": Sequence[str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-_RequiredListRotationOverridesRequestRequestTypeDef = TypedDict(
-    "_RequiredListRotationOverridesRequestRequestTypeDef",
-    {
-        "RotationId": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalListRotationOverridesRequestRequestTypeDef = TypedDict(
-    "_OptionalListRotationOverridesRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-
-class ListRotationOverridesRequestRequestTypeDef(
-    _RequiredListRotationOverridesRequestRequestTypeDef,
-    _OptionalListRotationOverridesRequestRequestTypeDef,
-):
-    pass
-
-
 RotationOverrideTypeDef = TypedDict(
     "RotationOverrideTypeDef",
     {
         "RotationOverrideId": str,
         "NewContactIds": List[str],
         "StartTime": datetime,
         "EndTime": datetime,
         "CreateTime": datetime,
     },
 )
 
-_RequiredListRotationShiftsRequestRequestTypeDef = TypedDict(
-    "_RequiredListRotationShiftsRequestRequestTypeDef",
-    {
-        "RotationId": str,
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalListRotationShiftsRequestRequestTypeDef = TypedDict(
-    "_OptionalListRotationShiftsRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-
-class ListRotationShiftsRequestRequestTypeDef(
-    _RequiredListRotationShiftsRequestRequestTypeDef,
-    _OptionalListRotationShiftsRequestRequestTypeDef,
-):
-    pass
-
-
 ListRotationsRequestRequestTypeDef = TypedDict(
     "ListRotationsRequestRequestTypeDef",
     {
         "RotationNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -1019,14 +929,108 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+_RequiredCreateRotationOverrideRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRotationOverrideRequestRequestTypeDef",
+    {
+        "RotationId": str,
+        "NewContactIds": Sequence[str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalCreateRotationOverrideRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRotationOverrideRequestRequestTypeDef",
+    {
+        "IdempotencyToken": str,
+    },
+    total=False,
+)
+
+
+class CreateRotationOverrideRequestRequestTypeDef(
+    _RequiredCreateRotationOverrideRequestRequestTypeDef,
+    _OptionalCreateRotationOverrideRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListRotationOverridesRequestRequestTypeDef = TypedDict(
+    "_RequiredListRotationOverridesRequestRequestTypeDef",
+    {
+        "RotationId": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalListRotationOverridesRequestRequestTypeDef = TypedDict(
+    "_OptionalListRotationOverridesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class ListRotationOverridesRequestRequestTypeDef(
+    _RequiredListRotationOverridesRequestRequestTypeDef,
+    _OptionalListRotationOverridesRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListRotationShiftsRequestRequestTypeDef = TypedDict(
+    "_RequiredListRotationShiftsRequestRequestTypeDef",
+    {
+        "RotationId": str,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalListRotationShiftsRequestRequestTypeDef = TypedDict(
+    "_OptionalListRotationShiftsRequestRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class ListRotationShiftsRequestRequestTypeDef(
+    _RequiredListRotationShiftsRequestRequestTypeDef,
+    _OptionalListRotationShiftsRequestRequestTypeDef,
+):
+    pass
+
+
+PreviewOverrideTypeDef = TypedDict(
+    "PreviewOverrideTypeDef",
+    {
+        "NewMembers": Sequence[str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+TimeRangeTypeDef = TypedDict(
+    "TimeRangeTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
 ListEngagementsResultTypeDef = TypedDict(
     "ListEngagementsResultTypeDef",
     {
         "NextToken": str,
         "Engagements": List[EngagementTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1152,16 +1156,16 @@
     pass
 
 
 _RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
     "_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
     {
         "RotationId": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
     },
 )
 _OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
     "_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1176,21 +1180,21 @@
     pass
 
 
 _RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
     "_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
     {
         "RotationId": str,
-        "EndTime": Union[datetime, str],
+        "EndTime": TimestampTypeDef,
     },
 )
 _OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
     "_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
     {
-        "StartTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListRotationShiftsRequestListRotationShiftsPaginateTypeDef(
@@ -1205,35 +1209,14 @@
     {
         "RotationNamePrefix": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListEngagementsRequestListEngagementsPaginateTypeDef = TypedDict(
-    "ListEngagementsRequestListEngagementsPaginateTypeDef",
-    {
-        "IncidentId": str,
-        "TimeRangeValue": TimeRangeTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEngagementsRequestRequestTypeDef = TypedDict(
-    "ListEngagementsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "IncidentId": str,
-        "TimeRangeValue": TimeRangeTypeDef,
-    },
-    total=False,
-)
-
 ListPageReceiptsResultTypeDef = TypedDict(
     "ListPageReceiptsResultTypeDef",
     {
         "NextToken": str,
         "Receipts": List[ReceiptTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1368,14 +1351,35 @@
 
 class RecurrenceSettingsTypeDef(
     _RequiredRecurrenceSettingsTypeDef, _OptionalRecurrenceSettingsTypeDef
 ):
     pass
 
 
+ListEngagementsRequestListEngagementsPaginateTypeDef = TypedDict(
+    "ListEngagementsRequestListEngagementsPaginateTypeDef",
+    {
+        "IncidentId": str,
+        "TimeRangeValue": TimeRangeTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEngagementsRequestRequestTypeDef = TypedDict(
+    "ListEngagementsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "IncidentId": str,
+        "TimeRangeValue": TimeRangeTypeDef,
+    },
+    total=False,
+)
+
 ListPreviewRotationShiftsResultTypeDef = TypedDict(
     "ListPreviewRotationShiftsResultTypeDef",
     {
         "RotationShifts": List[RotationShiftTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1452,15 +1456,15 @@
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
     },
 )
 _OptionalCreateRotationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRotationRequestRequestTypeDef",
     {
-        "StartTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
         "Tags": Sequence[TagTypeDef],
         "IdempotencyToken": str,
     },
     total=False,
 )
 
 
@@ -1469,25 +1473,25 @@
 ):
     pass
 
 
 _RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef = TypedDict(
     "_RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     {
-        "EndTime": Union[datetime, str],
+        "EndTime": TimestampTypeDef,
         "Members": Sequence[str],
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
     },
 )
 _OptionalListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef = TypedDict(
     "_OptionalListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     {
-        "RotationStartTime": Union[datetime, str],
-        "StartTime": Union[datetime, str],
+        "RotationStartTime": TimestampTypeDef,
+        "StartTime": TimestampTypeDef,
         "Overrides": Sequence[PreviewOverrideTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
@@ -1497,25 +1501,25 @@
 ):
     pass
 
 
 _RequiredListPreviewRotationShiftsRequestRequestTypeDef = TypedDict(
     "_RequiredListPreviewRotationShiftsRequestRequestTypeDef",
     {
-        "EndTime": Union[datetime, str],
+        "EndTime": TimestampTypeDef,
         "Members": Sequence[str],
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
     },
 )
 _OptionalListPreviewRotationShiftsRequestRequestTypeDef = TypedDict(
     "_OptionalListPreviewRotationShiftsRequestRequestTypeDef",
     {
-        "RotationStartTime": Union[datetime, str],
-        "StartTime": Union[datetime, str],
+        "RotationStartTime": TimestampTypeDef,
+        "StartTime": TimestampTypeDef,
         "Overrides": Sequence[PreviewOverrideTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
@@ -1523,26 +1527,27 @@
 class ListPreviewRotationShiftsRequestRequestTypeDef(
     _RequiredListPreviewRotationShiftsRequestRequestTypeDef,
     _OptionalListPreviewRotationShiftsRequestRequestTypeDef,
 ):
     pass
 
 
+RecurrenceSettingsUnionTypeDef = Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef]
 _RequiredUpdateRotationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRotationRequestRequestTypeDef",
     {
         "RotationId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
     },
 )
 _OptionalUpdateRotationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateRotationRequestRequestTypeDef",
     {
         "ContactIds": Sequence[str],
-        "StartTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
         "TimeZoneId": str,
     },
     total=False,
 )
 
 
 class UpdateRotationRequestRequestTypeDef(
@@ -1584,14 +1589,15 @@
 
 class CreateContactRequestRequestTypeDef(
     _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
 ):
     pass
 
 
+PlanUnionTypeDef = Union[PlanTypeDef, PlanOutputTypeDef]
 _RequiredUpdateContactRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 _OptionalUpdateContactRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/type_defs.pyi` & `mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_ssm_contacts.type_defs import AcceptPageRequestRequestTypeDef
 
-    data: AcceptPageRequestRequestTypeDef = {...}
+    data: AcceptPageRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -37,15 +37,15 @@
     "ChannelTargetInfoTypeDef",
     "ContactChannelAddressTypeDef",
     "ContactTargetInfoTypeDef",
     "ContactTypeDef",
     "HandOffTimeTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
-    "CreateRotationOverrideRequestRequestTypeDef",
+    "TimestampTypeDef",
     "DeactivateContactChannelRequestRequestTypeDef",
     "DeleteContactChannelRequestRequestTypeDef",
     "DeleteContactRequestRequestTypeDef",
     "DeleteRotationOverrideRequestRequestTypeDef",
     "DeleteRotationRequestRequestTypeDef",
     "DescribeEngagementRequestRequestTypeDef",
     "DescribePageRequestRequestTypeDef",
@@ -54,26 +54,22 @@
     "GetContactPolicyRequestRequestTypeDef",
     "GetContactRequestRequestTypeDef",
     "GetRotationOverrideRequestRequestTypeDef",
     "GetRotationRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListContactChannelsRequestRequestTypeDef",
     "ListContactsRequestRequestTypeDef",
-    "TimeRangeTypeDef",
     "ListPageReceiptsRequestRequestTypeDef",
     "ReceiptTypeDef",
     "ListPageResolutionsRequestRequestTypeDef",
     "ResolutionContactTypeDef",
     "ListPagesByContactRequestRequestTypeDef",
     "PageTypeDef",
     "ListPagesByEngagementRequestRequestTypeDef",
-    "PreviewOverrideTypeDef",
-    "ListRotationOverridesRequestRequestTypeDef",
     "RotationOverrideTypeDef",
-    "ListRotationShiftsRequestRequestTypeDef",
     "ListRotationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutContactPolicyRequestRequestTypeDef",
     "ShiftDetailsTypeDef",
     "SendActivationCodeRequestRequestTypeDef",
     "StartEngagementRequestRequestTypeDef",
     "StopEngagementRequestRequestTypeDef",
@@ -94,49 +90,56 @@
     "GetContactChannelResultTypeDef",
     "GetContactPolicyResultTypeDef",
     "GetRotationOverrideResultTypeDef",
     "ListContactsResultTypeDef",
     "StartEngagementResultTypeDef",
     "ListTagsForResourceResultTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateRotationOverrideRequestRequestTypeDef",
+    "ListRotationOverridesRequestRequestTypeDef",
+    "ListRotationShiftsRequestRequestTypeDef",
+    "PreviewOverrideTypeDef",
+    "TimeRangeTypeDef",
     "ListEngagementsResultTypeDef",
     "ListContactChannelsRequestListContactChannelsPaginateTypeDef",
     "ListContactsRequestListContactsPaginateTypeDef",
     "ListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
     "ListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
     "ListPagesByContactRequestListPagesByContactPaginateTypeDef",
     "ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
     "ListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
     "ListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
     "ListRotationsRequestListRotationsPaginateTypeDef",
-    "ListEngagementsRequestListEngagementsPaginateTypeDef",
-    "ListEngagementsRequestRequestTypeDef",
     "ListPageReceiptsResultTypeDef",
     "ListPageResolutionsResultTypeDef",
     "ListPagesByContactResultTypeDef",
     "ListPagesByEngagementResultTypeDef",
     "ListRotationOverridesResultTypeDef",
     "RotationShiftTypeDef",
     "ListContactChannelsResultTypeDef",
     "StageOutputTypeDef",
     "StageTypeDef",
     "RecurrenceSettingsOutputTypeDef",
     "RecurrenceSettingsTypeDef",
+    "ListEngagementsRequestListEngagementsPaginateTypeDef",
+    "ListEngagementsRequestRequestTypeDef",
     "ListPreviewRotationShiftsResultTypeDef",
     "ListRotationShiftsResultTypeDef",
     "PlanOutputTypeDef",
     "PlanTypeDef",
     "GetRotationResultTypeDef",
     "RotationTypeDef",
     "CreateRotationRequestRequestTypeDef",
     "ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     "ListPreviewRotationShiftsRequestRequestTypeDef",
+    "RecurrenceSettingsUnionTypeDef",
     "UpdateRotationRequestRequestTypeDef",
     "GetContactResultTypeDef",
     "CreateContactRequestRequestTypeDef",
+    "PlanUnionTypeDef",
     "UpdateContactRequestRequestTypeDef",
     "ListRotationsResultTypeDef",
 )
 
 _RequiredAcceptPageRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptPageRequestRequestTypeDef",
     {
@@ -257,37 +260,15 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-_RequiredCreateRotationOverrideRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRotationOverrideRequestRequestTypeDef",
-    {
-        "RotationId": str,
-        "NewContactIds": Sequence[str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalCreateRotationOverrideRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRotationOverrideRequestRequestTypeDef",
-    {
-        "IdempotencyToken": str,
-    },
-    total=False,
-)
-
-class CreateRotationOverrideRequestRequestTypeDef(
-    _RequiredCreateRotationOverrideRequestRequestTypeDef,
-    _OptionalCreateRotationOverrideRequestRequestTypeDef,
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 DeactivateContactChannelRequestRequestTypeDef = TypedDict(
     "DeactivateContactChannelRequestRequestTypeDef",
     {
         "ContactChannelId": str,
     },
 )
 
@@ -429,23 +410,14 @@
         "MaxResults": int,
         "AliasPrefix": str,
         "Type": ContactTypeType,
     },
     total=False,
 )
 
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredListPageReceiptsRequestRequestTypeDef = TypedDict(
     "_RequiredListPageReceiptsRequestRequestTypeDef",
     {
         "PageId": str,
     },
 )
 _OptionalListPageReceiptsRequestRequestTypeDef = TypedDict(
@@ -582,81 +554,25 @@
 
 class ListPagesByEngagementRequestRequestTypeDef(
     _RequiredListPagesByEngagementRequestRequestTypeDef,
     _OptionalListPagesByEngagementRequestRequestTypeDef,
 ):
     pass
 
-PreviewOverrideTypeDef = TypedDict(
-    "PreviewOverrideTypeDef",
-    {
-        "NewMembers": Sequence[str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-_RequiredListRotationOverridesRequestRequestTypeDef = TypedDict(
-    "_RequiredListRotationOverridesRequestRequestTypeDef",
-    {
-        "RotationId": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalListRotationOverridesRequestRequestTypeDef = TypedDict(
-    "_OptionalListRotationOverridesRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-class ListRotationOverridesRequestRequestTypeDef(
-    _RequiredListRotationOverridesRequestRequestTypeDef,
-    _OptionalListRotationOverridesRequestRequestTypeDef,
-):
-    pass
-
 RotationOverrideTypeDef = TypedDict(
     "RotationOverrideTypeDef",
     {
         "RotationOverrideId": str,
         "NewContactIds": List[str],
         "StartTime": datetime,
         "EndTime": datetime,
         "CreateTime": datetime,
     },
 )
 
-_RequiredListRotationShiftsRequestRequestTypeDef = TypedDict(
-    "_RequiredListRotationShiftsRequestRequestTypeDef",
-    {
-        "RotationId": str,
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalListRotationShiftsRequestRequestTypeDef = TypedDict(
-    "_OptionalListRotationShiftsRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-class ListRotationShiftsRequestRequestTypeDef(
-    _RequiredListRotationShiftsRequestRequestTypeDef,
-    _OptionalListRotationShiftsRequestRequestTypeDef,
-):
-    pass
-
 ListRotationsRequestRequestTypeDef = TypedDict(
     "ListRotationsRequestRequestTypeDef",
     {
         "RotationNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -976,14 +892,102 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+_RequiredCreateRotationOverrideRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRotationOverrideRequestRequestTypeDef",
+    {
+        "RotationId": str,
+        "NewContactIds": Sequence[str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalCreateRotationOverrideRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRotationOverrideRequestRequestTypeDef",
+    {
+        "IdempotencyToken": str,
+    },
+    total=False,
+)
+
+class CreateRotationOverrideRequestRequestTypeDef(
+    _RequiredCreateRotationOverrideRequestRequestTypeDef,
+    _OptionalCreateRotationOverrideRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListRotationOverridesRequestRequestTypeDef = TypedDict(
+    "_RequiredListRotationOverridesRequestRequestTypeDef",
+    {
+        "RotationId": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalListRotationOverridesRequestRequestTypeDef = TypedDict(
+    "_OptionalListRotationOverridesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class ListRotationOverridesRequestRequestTypeDef(
+    _RequiredListRotationOverridesRequestRequestTypeDef,
+    _OptionalListRotationOverridesRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListRotationShiftsRequestRequestTypeDef = TypedDict(
+    "_RequiredListRotationShiftsRequestRequestTypeDef",
+    {
+        "RotationId": str,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalListRotationShiftsRequestRequestTypeDef = TypedDict(
+    "_OptionalListRotationShiftsRequestRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class ListRotationShiftsRequestRequestTypeDef(
+    _RequiredListRotationShiftsRequestRequestTypeDef,
+    _OptionalListRotationShiftsRequestRequestTypeDef,
+):
+    pass
+
+PreviewOverrideTypeDef = TypedDict(
+    "PreviewOverrideTypeDef",
+    {
+        "NewMembers": Sequence[str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+TimeRangeTypeDef = TypedDict(
+    "TimeRangeTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
 ListEngagementsResultTypeDef = TypedDict(
     "ListEngagementsResultTypeDef",
     {
         "NextToken": str,
         "Engagements": List[EngagementTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1099,16 +1103,16 @@
 ):
     pass
 
 _RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
     "_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
     {
         "RotationId": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
     },
 )
 _OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
     "_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1121,21 +1125,21 @@
 ):
     pass
 
 _RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
     "_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
     {
         "RotationId": str,
-        "EndTime": Union[datetime, str],
+        "EndTime": TimestampTypeDef,
     },
 )
 _OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
     "_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
     {
-        "StartTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListRotationShiftsRequestListRotationShiftsPaginateTypeDef(
     _RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
@@ -1148,35 +1152,14 @@
     {
         "RotationNamePrefix": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListEngagementsRequestListEngagementsPaginateTypeDef = TypedDict(
-    "ListEngagementsRequestListEngagementsPaginateTypeDef",
-    {
-        "IncidentId": str,
-        "TimeRangeValue": TimeRangeTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEngagementsRequestRequestTypeDef = TypedDict(
-    "ListEngagementsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "IncidentId": str,
-        "TimeRangeValue": TimeRangeTypeDef,
-    },
-    total=False,
-)
-
 ListPageReceiptsResultTypeDef = TypedDict(
     "ListPageReceiptsResultTypeDef",
     {
         "NextToken": str,
         "Receipts": List[ReceiptTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1305,14 +1288,35 @@
 )
 
 class RecurrenceSettingsTypeDef(
     _RequiredRecurrenceSettingsTypeDef, _OptionalRecurrenceSettingsTypeDef
 ):
     pass
 
+ListEngagementsRequestListEngagementsPaginateTypeDef = TypedDict(
+    "ListEngagementsRequestListEngagementsPaginateTypeDef",
+    {
+        "IncidentId": str,
+        "TimeRangeValue": TimeRangeTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEngagementsRequestRequestTypeDef = TypedDict(
+    "ListEngagementsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "IncidentId": str,
+        "TimeRangeValue": TimeRangeTypeDef,
+    },
+    total=False,
+)
+
 ListPreviewRotationShiftsResultTypeDef = TypedDict(
     "ListPreviewRotationShiftsResultTypeDef",
     {
         "RotationShifts": List[RotationShiftTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1387,40 +1391,40 @@
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
     },
 )
 _OptionalCreateRotationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRotationRequestRequestTypeDef",
     {
-        "StartTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
         "Tags": Sequence[TagTypeDef],
         "IdempotencyToken": str,
     },
     total=False,
 )
 
 class CreateRotationRequestRequestTypeDef(
     _RequiredCreateRotationRequestRequestTypeDef, _OptionalCreateRotationRequestRequestTypeDef
 ):
     pass
 
 _RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef = TypedDict(
     "_RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     {
-        "EndTime": Union[datetime, str],
+        "EndTime": TimestampTypeDef,
         "Members": Sequence[str],
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
     },
 )
 _OptionalListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef = TypedDict(
     "_OptionalListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     {
-        "RotationStartTime": Union[datetime, str],
-        "StartTime": Union[datetime, str],
+        "RotationStartTime": TimestampTypeDef,
+        "StartTime": TimestampTypeDef,
         "Overrides": Sequence[PreviewOverrideTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef(
@@ -1428,50 +1432,51 @@
     _OptionalListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef,
 ):
     pass
 
 _RequiredListPreviewRotationShiftsRequestRequestTypeDef = TypedDict(
     "_RequiredListPreviewRotationShiftsRequestRequestTypeDef",
     {
-        "EndTime": Union[datetime, str],
+        "EndTime": TimestampTypeDef,
         "Members": Sequence[str],
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
     },
 )
 _OptionalListPreviewRotationShiftsRequestRequestTypeDef = TypedDict(
     "_OptionalListPreviewRotationShiftsRequestRequestTypeDef",
     {
-        "RotationStartTime": Union[datetime, str],
-        "StartTime": Union[datetime, str],
+        "RotationStartTime": TimestampTypeDef,
+        "StartTime": TimestampTypeDef,
         "Overrides": Sequence[PreviewOverrideTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
 class ListPreviewRotationShiftsRequestRequestTypeDef(
     _RequiredListPreviewRotationShiftsRequestRequestTypeDef,
     _OptionalListPreviewRotationShiftsRequestRequestTypeDef,
 ):
     pass
 
+RecurrenceSettingsUnionTypeDef = Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef]
 _RequiredUpdateRotationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRotationRequestRequestTypeDef",
     {
         "RotationId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
     },
 )
 _OptionalUpdateRotationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateRotationRequestRequestTypeDef",
     {
         "ContactIds": Sequence[str],
-        "StartTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
         "TimeZoneId": str,
     },
     total=False,
 )
 
 class UpdateRotationRequestRequestTypeDef(
     _RequiredUpdateRotationRequestRequestTypeDef, _OptionalUpdateRotationRequestRequestTypeDef
@@ -1509,14 +1514,15 @@
 )
 
 class CreateContactRequestRequestTypeDef(
     _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
 ):
     pass
 
+PlanUnionTypeDef = Union[PlanTypeDef, PlanOutputTypeDef]
 _RequiredUpdateContactRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 _OptionalUpdateContactRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts.egg-info/PKG-INFO` & `mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-contacts
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SSMContacts 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SSMContacts 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ssm-contacts type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 ssm-contacts type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-contacts.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-contacts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-contacts)](https://pepy.tech/project/mypy-boto3-ssm-contacts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMContacts 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
+[boto3.SSMContacts 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
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
 [mypy-boto3-ssm-contacts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/).
 
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
@@ -364,33 +364,33 @@
 )
 
 
 def check_value(value: AcceptCodeValidationType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ssm_contacts.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ssm_contacts.type_defs import (
     AcceptPageRequestRequestTypeDef,
     ActivateContactChannelRequestRequestTypeDef,
     ChannelTargetInfoTypeDef,
     ContactChannelAddressTypeDef,
     ContactTargetInfoTypeDef,
     ContactTypeDef,
     HandOffTimeTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
-    CreateRotationOverrideRequestRequestTypeDef,
+    TimestampTypeDef,
     DeactivateContactChannelRequestRequestTypeDef,
     DeleteContactChannelRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
     DeleteRotationOverrideRequestRequestTypeDef,
     DeleteRotationRequestRequestTypeDef,
     DescribeEngagementRequestRequestTypeDef,
     DescribePageRequestRequestTypeDef,
@@ -399,26 +399,22 @@
     GetContactPolicyRequestRequestTypeDef,
     GetContactRequestRequestTypeDef,
     GetRotationOverrideRequestRequestTypeDef,
     GetRotationRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListContactChannelsRequestRequestTypeDef,
     ListContactsRequestRequestTypeDef,
-    TimeRangeTypeDef,
     ListPageReceiptsRequestRequestTypeDef,
     ReceiptTypeDef,
     ListPageResolutionsRequestRequestTypeDef,
     ResolutionContactTypeDef,
     ListPagesByContactRequestRequestTypeDef,
     PageTypeDef,
     ListPagesByEngagementRequestRequestTypeDef,
-    PreviewOverrideTypeDef,
-    ListRotationOverridesRequestRequestTypeDef,
     RotationOverrideTypeDef,
-    ListRotationShiftsRequestRequestTypeDef,
     ListRotationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PutContactPolicyRequestRequestTypeDef,
     ShiftDetailsTypeDef,
     SendActivationCodeRequestRequestTypeDef,
     StartEngagementRequestRequestTypeDef,
     StopEngagementRequestRequestTypeDef,
@@ -439,55 +435,62 @@
     GetContactChannelResultTypeDef,
     GetContactPolicyResultTypeDef,
     GetRotationOverrideResultTypeDef,
     ListContactsResultTypeDef,
     StartEngagementResultTypeDef,
     ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateRotationOverrideRequestRequestTypeDef,
+    ListRotationOverridesRequestRequestTypeDef,
+    ListRotationShiftsRequestRequestTypeDef,
+    PreviewOverrideTypeDef,
+    TimeRangeTypeDef,
     ListEngagementsResultTypeDef,
     ListContactChannelsRequestListContactChannelsPaginateTypeDef,
     ListContactsRequestListContactsPaginateTypeDef,
     ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
     ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
     ListPagesByContactRequestListPagesByContactPaginateTypeDef,
     ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
     ListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
     ListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
     ListRotationsRequestListRotationsPaginateTypeDef,
-    ListEngagementsRequestListEngagementsPaginateTypeDef,
-    ListEngagementsRequestRequestTypeDef,
     ListPageReceiptsResultTypeDef,
     ListPageResolutionsResultTypeDef,
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListRotationOverridesResultTypeDef,
     RotationShiftTypeDef,
     ListContactChannelsResultTypeDef,
     StageOutputTypeDef,
     StageTypeDef,
     RecurrenceSettingsOutputTypeDef,
     RecurrenceSettingsTypeDef,
+    ListEngagementsRequestListEngagementsPaginateTypeDef,
+    ListEngagementsRequestRequestTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationShiftsResultTypeDef,
     PlanOutputTypeDef,
     PlanTypeDef,
     GetRotationResultTypeDef,
     RotationTypeDef,
     CreateRotationRequestRequestTypeDef,
     ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef,
     ListPreviewRotationShiftsRequestRequestTypeDef,
+    RecurrenceSettingsUnionTypeDef,
     UpdateRotationRequestRequestTypeDef,
     GetContactResultTypeDef,
     CreateContactRequestRequestTypeDef,
+    PlanUnionTypeDef,
     UpdateContactRequestRequestTypeDef,
     ListRotationsResultTypeDef,
 )
 
 
-def get_structure() -> AcceptPageRequestRequestTypeDef:
+def get_value() -> AcceptPageRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts.egg-info/SOURCES.txt` & `mypy-boto3-ssm-contacts-1.28.16/mypy_boto3_ssm_contacts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.15.post1/setup.py` & `mypy-boto3-ssm-contacts-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ssm-contacts",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_ssm_contacts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSMContacts 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.SSMContacts 1.28.16 service generated with mypy-boto3-builder"
+        " 7.17.1"
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
-    keywords="boto3 ssm-contacts type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 ssm-contacts type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_ssm_contacts": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

