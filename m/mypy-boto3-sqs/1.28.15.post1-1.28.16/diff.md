# Comparing `tmp/mypy-boto3-sqs-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-sqs-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sqs-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:15 2023, max compression
+gzip compressed data, was "mypy-boto3-sqs-1.28.16.tar", last modified: Tue Aug  1 11:37:55 2023, max compression
```

## Comparing `mypy-boto3-sqs-1.28.15.post1.tar` & `mypy-boto3-sqs-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:15.945419 mypy-boto3-sqs-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:59:57.000000 mypy-boto3-sqs-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17758 2023-07-29 10:04:15.945419 mypy-boto3-sqs-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16281 2023-07-29 09:59:57.000000 mypy-boto3-sqs-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:15.945419 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-29 09:59:57.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-29 09:59:57.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:59:57.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18196 2023-07-29 09:59:58.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18164 2023-07-29 09:59:58.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-07-29 09:59:58.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-29 09:59:58.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-29 09:59:58.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-29 09:59:58.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:59:57.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19031 2023-07-29 09:59:58.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    18992 2023-07-29 09:59:58.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25272 2023-07-29 09:59:59.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25233 2023-07-29 09:59:58.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:59:57.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:15.945419 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17758 2023-07-29 10:04:15.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-29 10:04:15.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:15.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:15.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:15.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:04:15.000000 mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:15.945419 mypy-boto3-sqs-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:59:57.000000 mypy-boto3-sqs-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:55.224720 mypy-boto3-sqs-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:33:31.000000 mypy-boto3-sqs-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17804 2023-08-01 11:37:55.224720 mypy-boto3-sqs-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16336 2023-08-01 11:33:31.000000 mypy-boto3-sqs-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:55.220720 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-01 11:33:31.000000 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-01 11:33:31.000000 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 11:33:31.000000 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18094 2023-08-01 11:33:31.000000 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18062 2023-08-01 11:33:31.000000 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-08-01 11:33:32.000000 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-08-01 11:33:32.000000 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-08-01 11:33:32.000000 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-08-01 11:33:32.000000 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:33:31.000000 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19031 2023-08-01 11:33:32.000000 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18992 2023-08-01 11:33:32.000000 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25320 2023-08-01 11:33:33.000000 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25281 2023-08-01 11:33:32.000000 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:33:31.000000 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:55.224720 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17804 2023-08-01 11:37:54.000000 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-01 11:37:55.000000 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:54.000000 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:54.000000 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:54.000000 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:37:54.000000 mypy-boto3-sqs-1.28.16/mypy_boto3_sqs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:55.224720 mypy-boto3-sqs-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 11:33:31.000000 mypy-boto3-sqs-1.28.16/setup.py
```

### Comparing `mypy-boto3-sqs-1.28.15.post1/LICENSE` & `mypy-boto3-sqs-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.15.post1/PKG-INFO` & `mypy-boto3-sqs-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sqs
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SQS 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SQS 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sqs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 sqs type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sqs)](https://pepy.tech/project/mypy-boto3-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SQS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[boto3.SQS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
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
 [mypy-boto3-sqs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -78,15 +78,15 @@
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -403,26 +403,27 @@
 )
 
 
 def check_value(value: ListDeadLetterSourceQueuesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sqs.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sqs.type_defs import (
     AddPermissionRequestQueueAddPermissionTypeDef,
     AddPermissionRequestRequestTypeDef,
     BatchResultErrorEntryTypeDef,
+    BlobTypeDef,
     CancelMessageMoveTaskRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultEntryTypeDef,
     ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef,
     ChangeMessageVisibilityRequestRequestTypeDef,
     CreateQueueRequestRequestTypeDef,
@@ -437,27 +438,27 @@
     PaginatorConfigTypeDef,
     ListDeadLetterSourceQueuesRequestRequestTypeDef,
     ListMessageMoveTasksRequestRequestTypeDef,
     ListMessageMoveTasksResultEntryTypeDef,
     ListQueueTagsRequestRequestTypeDef,
     ListQueuesRequestRequestTypeDef,
     MessageAttributeValueOutputTypeDef,
-    MessageAttributeValueTypeDef,
-    MessageSystemAttributeValueTypeDef,
     PurgeQueueRequestRequestTypeDef,
     ReceiveMessageRequestQueueReceiveMessagesTypeDef,
     ReceiveMessageRequestRequestTypeDef,
     RemovePermissionRequestQueueRemovePermissionTypeDef,
     RemovePermissionRequestRequestTypeDef,
     SendMessageBatchResultEntryTypeDef,
     SetQueueAttributesRequestQueueSetAttributesTypeDef,
     SetQueueAttributesRequestRequestTypeDef,
     StartMessageMoveTaskRequestRequestTypeDef,
     TagQueueRequestRequestTypeDef,
     UntagQueueRequestRequestTypeDef,
+    MessageAttributeValueTypeDef,
+    MessageSystemAttributeValueTypeDef,
     CancelMessageMoveTaskResultTypeDef,
     CreateQueueResultTypeDef,
     EmptyResponseMetadataTypeDef,
     GetQueueAttributesResultTypeDef,
     GetQueueUrlResultTypeDef,
     ListDeadLetterSourceQueuesResultTypeDef,
     ListQueueTagsResultTypeDef,
@@ -470,25 +471,26 @@
     DeleteMessageBatchRequestQueueDeleteMessagesTypeDef,
     DeleteMessageBatchRequestRequestTypeDef,
     DeleteMessageBatchResultTypeDef,
     ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
     ListQueuesRequestListQueuesPaginateTypeDef,
     ListMessageMoveTasksResultTypeDef,
     MessageTypeDef,
+    SendMessageBatchResultTypeDef,
+    MessageAttributeValueUnionTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageRequestQueueSendMessageTypeDef,
-    SendMessageRequestRequestTypeDef,
-    SendMessageBatchResultTypeDef,
     ReceiveMessageResultTypeDef,
+    SendMessageRequestRequestTypeDef,
     SendMessageBatchRequestQueueSendMessagesTypeDef,
     SendMessageBatchRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddPermissionRequestQueueAddPermissionTypeDef:
+def get_value() -> AddPermissionRequestQueueAddPermissionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sqs-1.28.15.post1/README.md` & `mypy-boto3-sqs-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sqs)](https://pepy.tech/project/mypy-boto3-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SQS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[boto3.SQS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
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
 [mypy-boto3-sqs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -46,15 +46,15 @@
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -371,26 +371,27 @@
 )
 
 
 def check_value(value: ListDeadLetterSourceQueuesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sqs.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sqs.type_defs import (
     AddPermissionRequestQueueAddPermissionTypeDef,
     AddPermissionRequestRequestTypeDef,
     BatchResultErrorEntryTypeDef,
+    BlobTypeDef,
     CancelMessageMoveTaskRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultEntryTypeDef,
     ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef,
     ChangeMessageVisibilityRequestRequestTypeDef,
     CreateQueueRequestRequestTypeDef,
@@ -405,27 +406,27 @@
     PaginatorConfigTypeDef,
     ListDeadLetterSourceQueuesRequestRequestTypeDef,
     ListMessageMoveTasksRequestRequestTypeDef,
     ListMessageMoveTasksResultEntryTypeDef,
     ListQueueTagsRequestRequestTypeDef,
     ListQueuesRequestRequestTypeDef,
     MessageAttributeValueOutputTypeDef,
-    MessageAttributeValueTypeDef,
-    MessageSystemAttributeValueTypeDef,
     PurgeQueueRequestRequestTypeDef,
     ReceiveMessageRequestQueueReceiveMessagesTypeDef,
     ReceiveMessageRequestRequestTypeDef,
     RemovePermissionRequestQueueRemovePermissionTypeDef,
     RemovePermissionRequestRequestTypeDef,
     SendMessageBatchResultEntryTypeDef,
     SetQueueAttributesRequestQueueSetAttributesTypeDef,
     SetQueueAttributesRequestRequestTypeDef,
     StartMessageMoveTaskRequestRequestTypeDef,
     TagQueueRequestRequestTypeDef,
     UntagQueueRequestRequestTypeDef,
+    MessageAttributeValueTypeDef,
+    MessageSystemAttributeValueTypeDef,
     CancelMessageMoveTaskResultTypeDef,
     CreateQueueResultTypeDef,
     EmptyResponseMetadataTypeDef,
     GetQueueAttributesResultTypeDef,
     GetQueueUrlResultTypeDef,
     ListDeadLetterSourceQueuesResultTypeDef,
     ListQueueTagsResultTypeDef,
@@ -438,25 +439,26 @@
     DeleteMessageBatchRequestQueueDeleteMessagesTypeDef,
     DeleteMessageBatchRequestRequestTypeDef,
     DeleteMessageBatchResultTypeDef,
     ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
     ListQueuesRequestListQueuesPaginateTypeDef,
     ListMessageMoveTasksResultTypeDef,
     MessageTypeDef,
+    SendMessageBatchResultTypeDef,
+    MessageAttributeValueUnionTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageRequestQueueSendMessageTypeDef,
-    SendMessageRequestRequestTypeDef,
-    SendMessageBatchResultTypeDef,
     ReceiveMessageResultTypeDef,
+    SendMessageRequestRequestTypeDef,
     SendMessageBatchRequestQueueSendMessagesTypeDef,
     SendMessageBatchRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddPermissionRequestQueueAddPermissionTypeDef:
+def get_value() -> AddPermissionRequestQueueAddPermissionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/__init__.py` & `mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/__init__.pyi` & `mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/__main__.py` & `mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SQS 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.SQS 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS\nOther"
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

### Comparing `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/client.py` & `mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_sqs.client import SQSClient
 
     session = Session()
     client: SQSClient = session.client("sqs")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import QueueAttributeFilterType, QueueAttributeNameType
 from .paginator import ListDeadLetterSourceQueuesPaginator, ListQueuesPaginator
 from .type_defs import (
     CancelMessageMoveTaskResultTypeDef,
@@ -30,16 +30,15 @@
     EmptyResponseMetadataTypeDef,
     GetQueueAttributesResultTypeDef,
     GetQueueUrlResultTypeDef,
     ListDeadLetterSourceQueuesResultTypeDef,
     ListMessageMoveTasksResultTypeDef,
     ListQueuesResultTypeDef,
     ListQueueTagsResultTypeDef,
-    MessageAttributeValueOutputTypeDef,
-    MessageAttributeValueTypeDef,
+    MessageAttributeValueUnionTypeDef,
     MessageSystemAttributeValueTypeDef,
     ReceiveMessageResultTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageBatchResultTypeDef,
     SendMessageResultTypeDef,
     StartMessageMoveTaskResultTypeDef,
 )
@@ -307,17 +306,15 @@
 
     def send_message(
         self,
         *,
         QueueUrl: str,
         MessageBody: str,
         DelaySeconds: int = ...,
-        MessageAttributes: Mapping[
-            str, Union[MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef]
-        ] = ...,
+        MessageAttributes: Mapping[str, MessageAttributeValueUnionTypeDef] = ...,
         MessageSystemAttributes: Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ] = ...,
         MessageDeduplicationId: str = ...,
         MessageGroupId: str = ...
     ) -> SendMessageResultTypeDef:
         """
```

### Comparing `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/client.pyi` & `mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_sqs.client import SQSClient
 
     session = Session()
     client: SQSClient = session.client("sqs")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import QueueAttributeFilterType, QueueAttributeNameType
 from .paginator import ListDeadLetterSourceQueuesPaginator, ListQueuesPaginator
 from .type_defs import (
     CancelMessageMoveTaskResultTypeDef,
@@ -30,16 +30,15 @@
     EmptyResponseMetadataTypeDef,
     GetQueueAttributesResultTypeDef,
     GetQueueUrlResultTypeDef,
     ListDeadLetterSourceQueuesResultTypeDef,
     ListMessageMoveTasksResultTypeDef,
     ListQueuesResultTypeDef,
     ListQueueTagsResultTypeDef,
-    MessageAttributeValueOutputTypeDef,
-    MessageAttributeValueTypeDef,
+    MessageAttributeValueUnionTypeDef,
     MessageSystemAttributeValueTypeDef,
     ReceiveMessageResultTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageBatchResultTypeDef,
     SendMessageResultTypeDef,
     StartMessageMoveTaskResultTypeDef,
 )
@@ -282,17 +281,15 @@
         """
     def send_message(
         self,
         *,
         QueueUrl: str,
         MessageBody: str,
         DelaySeconds: int = ...,
-        MessageAttributes: Mapping[
-            str, Union[MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef]
-        ] = ...,
+        MessageAttributes: Mapping[str, MessageAttributeValueUnionTypeDef] = ...,
         MessageSystemAttributes: Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ] = ...,
         MessageDeduplicationId: str = ...,
         MessageGroupId: str = ...
     ) -> SendMessageResultTypeDef:
         """
```

### Comparing `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/literals.py` & `mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/literals.pyi` & `mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/paginator.py` & `mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/paginator.pyi` & `mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/service_resource.py` & `mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/service_resource.pyi` & `mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/type_defs.py` & `mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_sqs.type_defs import AddPermissionRequestQueueAddPermissionTypeDef
 
-    data: AddPermissionRequestQueueAddPermissionTypeDef = {...}
+    data: AddPermissionRequestQueueAddPermissionTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
@@ -32,14 +32,15 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddPermissionRequestQueueAddPermissionTypeDef",
     "AddPermissionRequestRequestTypeDef",
     "BatchResultErrorEntryTypeDef",
+    "BlobTypeDef",
     "CancelMessageMoveTaskRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ChangeMessageVisibilityBatchRequestEntryTypeDef",
     "ChangeMessageVisibilityBatchResultEntryTypeDef",
     "ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef",
     "ChangeMessageVisibilityRequestRequestTypeDef",
     "CreateQueueRequestRequestTypeDef",
@@ -54,27 +55,27 @@
     "PaginatorConfigTypeDef",
     "ListDeadLetterSourceQueuesRequestRequestTypeDef",
     "ListMessageMoveTasksRequestRequestTypeDef",
     "ListMessageMoveTasksResultEntryTypeDef",
     "ListQueueTagsRequestRequestTypeDef",
     "ListQueuesRequestRequestTypeDef",
     "MessageAttributeValueOutputTypeDef",
-    "MessageAttributeValueTypeDef",
-    "MessageSystemAttributeValueTypeDef",
     "PurgeQueueRequestRequestTypeDef",
     "ReceiveMessageRequestQueueReceiveMessagesTypeDef",
     "ReceiveMessageRequestRequestTypeDef",
     "RemovePermissionRequestQueueRemovePermissionTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "SendMessageBatchResultEntryTypeDef",
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     "SetQueueAttributesRequestRequestTypeDef",
     "StartMessageMoveTaskRequestRequestTypeDef",
     "TagQueueRequestRequestTypeDef",
     "UntagQueueRequestRequestTypeDef",
+    "MessageAttributeValueTypeDef",
+    "MessageSystemAttributeValueTypeDef",
     "CancelMessageMoveTaskResultTypeDef",
     "CreateQueueResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetQueueAttributesResultTypeDef",
     "GetQueueUrlResultTypeDef",
     "ListDeadLetterSourceQueuesResultTypeDef",
     "ListQueueTagsResultTypeDef",
@@ -87,19 +88,20 @@
     "DeleteMessageBatchRequestQueueDeleteMessagesTypeDef",
     "DeleteMessageBatchRequestRequestTypeDef",
     "DeleteMessageBatchResultTypeDef",
     "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
     "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListMessageMoveTasksResultTypeDef",
     "MessageTypeDef",
+    "SendMessageBatchResultTypeDef",
+    "MessageAttributeValueUnionTypeDef",
     "SendMessageBatchRequestEntryTypeDef",
     "SendMessageRequestQueueSendMessageTypeDef",
-    "SendMessageRequestRequestTypeDef",
-    "SendMessageBatchResultTypeDef",
     "ReceiveMessageResultTypeDef",
+    "SendMessageRequestRequestTypeDef",
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
     "SendMessageBatchRequestRequestTypeDef",
 )
 
 AddPermissionRequestQueueAddPermissionTypeDef = TypedDict(
     "AddPermissionRequestQueueAddPermissionTypeDef",
     {
@@ -138,14 +140,15 @@
 
 class BatchResultErrorEntryTypeDef(
     _RequiredBatchResultErrorEntryTypeDef, _OptionalBatchResultErrorEntryTypeDef
 ):
     pass
 
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelMessageMoveTaskRequestRequestTypeDef = TypedDict(
     "CancelMessageMoveTaskRequestRequestTypeDef",
     {
         "TaskHandle": str,
     },
 )
 
@@ -454,62 +457,14 @@
 
 class MessageAttributeValueOutputTypeDef(
     _RequiredMessageAttributeValueOutputTypeDef, _OptionalMessageAttributeValueOutputTypeDef
 ):
     pass
 
 
-_RequiredMessageAttributeValueTypeDef = TypedDict(
-    "_RequiredMessageAttributeValueTypeDef",
-    {
-        "DataType": str,
-    },
-)
-_OptionalMessageAttributeValueTypeDef = TypedDict(
-    "_OptionalMessageAttributeValueTypeDef",
-    {
-        "StringValue": str,
-        "BinaryValue": Union[str, bytes, IO[Any], StreamingBody],
-        "StringListValues": Sequence[str],
-        "BinaryListValues": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
-    },
-    total=False,
-)
-
-
-class MessageAttributeValueTypeDef(
-    _RequiredMessageAttributeValueTypeDef, _OptionalMessageAttributeValueTypeDef
-):
-    pass
-
-
-_RequiredMessageSystemAttributeValueTypeDef = TypedDict(
-    "_RequiredMessageSystemAttributeValueTypeDef",
-    {
-        "DataType": str,
-    },
-)
-_OptionalMessageSystemAttributeValueTypeDef = TypedDict(
-    "_OptionalMessageSystemAttributeValueTypeDef",
-    {
-        "StringValue": str,
-        "BinaryValue": Union[str, bytes, IO[Any], StreamingBody],
-        "StringListValues": Sequence[str],
-        "BinaryListValues": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
-    },
-    total=False,
-)
-
-
-class MessageSystemAttributeValueTypeDef(
-    _RequiredMessageSystemAttributeValueTypeDef, _OptionalMessageSystemAttributeValueTypeDef
-):
-    pass
-
-
 PurgeQueueRequestRequestTypeDef = TypedDict(
     "PurgeQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
@@ -642,14 +597,62 @@
     "UntagQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "TagKeys": Sequence[str],
     },
 )
 
+_RequiredMessageAttributeValueTypeDef = TypedDict(
+    "_RequiredMessageAttributeValueTypeDef",
+    {
+        "DataType": str,
+    },
+)
+_OptionalMessageAttributeValueTypeDef = TypedDict(
+    "_OptionalMessageAttributeValueTypeDef",
+    {
+        "StringValue": str,
+        "BinaryValue": BlobTypeDef,
+        "StringListValues": Sequence[str],
+        "BinaryListValues": Sequence[BlobTypeDef],
+    },
+    total=False,
+)
+
+
+class MessageAttributeValueTypeDef(
+    _RequiredMessageAttributeValueTypeDef, _OptionalMessageAttributeValueTypeDef
+):
+    pass
+
+
+_RequiredMessageSystemAttributeValueTypeDef = TypedDict(
+    "_RequiredMessageSystemAttributeValueTypeDef",
+    {
+        "DataType": str,
+    },
+)
+_OptionalMessageSystemAttributeValueTypeDef = TypedDict(
+    "_OptionalMessageSystemAttributeValueTypeDef",
+    {
+        "StringValue": str,
+        "BinaryValue": BlobTypeDef,
+        "StringListValues": Sequence[str],
+        "BinaryListValues": Sequence[BlobTypeDef],
+    },
+    total=False,
+)
+
+
+class MessageSystemAttributeValueTypeDef(
+    _RequiredMessageSystemAttributeValueTypeDef, _OptionalMessageSystemAttributeValueTypeDef
+):
+    pass
+
+
 CancelMessageMoveTaskResultTypeDef = TypedDict(
     "CancelMessageMoveTaskResultTypeDef",
     {
         "ApproximateNumberOfMessagesMoved": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -828,14 +831,26 @@
         "Attributes": Dict[MessageSystemAttributeNameType, str],
         "MD5OfMessageAttributes": str,
         "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
     },
     total=False,
 )
 
+SendMessageBatchResultTypeDef = TypedDict(
+    "SendMessageBatchResultTypeDef",
+    {
+        "Successful": List[SendMessageBatchResultEntryTypeDef],
+        "Failed": List[BatchResultErrorEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MessageAttributeValueUnionTypeDef = Union[
+    MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef
+]
 _RequiredSendMessageBatchRequestEntryTypeDef = TypedDict(
     "_RequiredSendMessageBatchRequestEntryTypeDef",
     {
         "Id": str,
         "MessageBody": str,
     },
 )
@@ -884,28 +899,34 @@
 class SendMessageRequestQueueSendMessageTypeDef(
     _RequiredSendMessageRequestQueueSendMessageTypeDef,
     _OptionalSendMessageRequestQueueSendMessageTypeDef,
 ):
     pass
 
 
+ReceiveMessageResultTypeDef = TypedDict(
+    "ReceiveMessageResultTypeDef",
+    {
+        "Messages": List[MessageTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredSendMessageRequestRequestTypeDef = TypedDict(
     "_RequiredSendMessageRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "MessageBody": str,
     },
 )
 _OptionalSendMessageRequestRequestTypeDef = TypedDict(
     "_OptionalSendMessageRequestRequestTypeDef",
     {
         "DelaySeconds": int,
-        "MessageAttributes": Mapping[
-            str, Union[MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef]
-        ],
+        "MessageAttributes": Mapping[str, MessageAttributeValueUnionTypeDef],
         "MessageSystemAttributes": Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ],
         "MessageDeduplicationId": str,
         "MessageGroupId": str,
     },
     total=False,
@@ -914,31 +935,14 @@
 
 class SendMessageRequestRequestTypeDef(
     _RequiredSendMessageRequestRequestTypeDef, _OptionalSendMessageRequestRequestTypeDef
 ):
     pass
 
 
-SendMessageBatchResultTypeDef = TypedDict(
-    "SendMessageBatchResultTypeDef",
-    {
-        "Successful": List[SendMessageBatchResultEntryTypeDef],
-        "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ReceiveMessageResultTypeDef = TypedDict(
-    "ReceiveMessageResultTypeDef",
-    {
-        "Messages": List[MessageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 SendMessageBatchRequestQueueSendMessagesTypeDef = TypedDict(
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
     {
         "Entries": Sequence[SendMessageBatchRequestEntryTypeDef],
     },
 )
```

### Comparing `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs/type_defs.pyi` & `mypy-boto3-sqs-1.28.16/mypy_boto3_sqs/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_sqs.type_defs import AddPermissionRequestQueueAddPermissionTypeDef
 
-    data: AddPermissionRequestQueueAddPermissionTypeDef = {...}
+    data: AddPermissionRequestQueueAddPermissionTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
@@ -31,14 +31,15 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddPermissionRequestQueueAddPermissionTypeDef",
     "AddPermissionRequestRequestTypeDef",
     "BatchResultErrorEntryTypeDef",
+    "BlobTypeDef",
     "CancelMessageMoveTaskRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ChangeMessageVisibilityBatchRequestEntryTypeDef",
     "ChangeMessageVisibilityBatchResultEntryTypeDef",
     "ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef",
     "ChangeMessageVisibilityRequestRequestTypeDef",
     "CreateQueueRequestRequestTypeDef",
@@ -53,27 +54,27 @@
     "PaginatorConfigTypeDef",
     "ListDeadLetterSourceQueuesRequestRequestTypeDef",
     "ListMessageMoveTasksRequestRequestTypeDef",
     "ListMessageMoveTasksResultEntryTypeDef",
     "ListQueueTagsRequestRequestTypeDef",
     "ListQueuesRequestRequestTypeDef",
     "MessageAttributeValueOutputTypeDef",
-    "MessageAttributeValueTypeDef",
-    "MessageSystemAttributeValueTypeDef",
     "PurgeQueueRequestRequestTypeDef",
     "ReceiveMessageRequestQueueReceiveMessagesTypeDef",
     "ReceiveMessageRequestRequestTypeDef",
     "RemovePermissionRequestQueueRemovePermissionTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "SendMessageBatchResultEntryTypeDef",
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     "SetQueueAttributesRequestRequestTypeDef",
     "StartMessageMoveTaskRequestRequestTypeDef",
     "TagQueueRequestRequestTypeDef",
     "UntagQueueRequestRequestTypeDef",
+    "MessageAttributeValueTypeDef",
+    "MessageSystemAttributeValueTypeDef",
     "CancelMessageMoveTaskResultTypeDef",
     "CreateQueueResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetQueueAttributesResultTypeDef",
     "GetQueueUrlResultTypeDef",
     "ListDeadLetterSourceQueuesResultTypeDef",
     "ListQueueTagsResultTypeDef",
@@ -86,19 +87,20 @@
     "DeleteMessageBatchRequestQueueDeleteMessagesTypeDef",
     "DeleteMessageBatchRequestRequestTypeDef",
     "DeleteMessageBatchResultTypeDef",
     "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
     "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListMessageMoveTasksResultTypeDef",
     "MessageTypeDef",
+    "SendMessageBatchResultTypeDef",
+    "MessageAttributeValueUnionTypeDef",
     "SendMessageBatchRequestEntryTypeDef",
     "SendMessageRequestQueueSendMessageTypeDef",
-    "SendMessageRequestRequestTypeDef",
-    "SendMessageBatchResultTypeDef",
     "ReceiveMessageResultTypeDef",
+    "SendMessageRequestRequestTypeDef",
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
     "SendMessageBatchRequestRequestTypeDef",
 )
 
 AddPermissionRequestQueueAddPermissionTypeDef = TypedDict(
     "AddPermissionRequestQueueAddPermissionTypeDef",
     {
@@ -135,14 +137,15 @@
 )
 
 class BatchResultErrorEntryTypeDef(
     _RequiredBatchResultErrorEntryTypeDef, _OptionalBatchResultErrorEntryTypeDef
 ):
     pass
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelMessageMoveTaskRequestRequestTypeDef = TypedDict(
     "CancelMessageMoveTaskRequestRequestTypeDef",
     {
         "TaskHandle": str,
     },
 )
 
@@ -433,58 +436,14 @@
 )
 
 class MessageAttributeValueOutputTypeDef(
     _RequiredMessageAttributeValueOutputTypeDef, _OptionalMessageAttributeValueOutputTypeDef
 ):
     pass
 
-_RequiredMessageAttributeValueTypeDef = TypedDict(
-    "_RequiredMessageAttributeValueTypeDef",
-    {
-        "DataType": str,
-    },
-)
-_OptionalMessageAttributeValueTypeDef = TypedDict(
-    "_OptionalMessageAttributeValueTypeDef",
-    {
-        "StringValue": str,
-        "BinaryValue": Union[str, bytes, IO[Any], StreamingBody],
-        "StringListValues": Sequence[str],
-        "BinaryListValues": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
-    },
-    total=False,
-)
-
-class MessageAttributeValueTypeDef(
-    _RequiredMessageAttributeValueTypeDef, _OptionalMessageAttributeValueTypeDef
-):
-    pass
-
-_RequiredMessageSystemAttributeValueTypeDef = TypedDict(
-    "_RequiredMessageSystemAttributeValueTypeDef",
-    {
-        "DataType": str,
-    },
-)
-_OptionalMessageSystemAttributeValueTypeDef = TypedDict(
-    "_OptionalMessageSystemAttributeValueTypeDef",
-    {
-        "StringValue": str,
-        "BinaryValue": Union[str, bytes, IO[Any], StreamingBody],
-        "StringListValues": Sequence[str],
-        "BinaryListValues": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
-    },
-    total=False,
-)
-
-class MessageSystemAttributeValueTypeDef(
-    _RequiredMessageSystemAttributeValueTypeDef, _OptionalMessageSystemAttributeValueTypeDef
-):
-    pass
-
 PurgeQueueRequestRequestTypeDef = TypedDict(
     "PurgeQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
@@ -611,14 +570,58 @@
     "UntagQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "TagKeys": Sequence[str],
     },
 )
 
+_RequiredMessageAttributeValueTypeDef = TypedDict(
+    "_RequiredMessageAttributeValueTypeDef",
+    {
+        "DataType": str,
+    },
+)
+_OptionalMessageAttributeValueTypeDef = TypedDict(
+    "_OptionalMessageAttributeValueTypeDef",
+    {
+        "StringValue": str,
+        "BinaryValue": BlobTypeDef,
+        "StringListValues": Sequence[str],
+        "BinaryListValues": Sequence[BlobTypeDef],
+    },
+    total=False,
+)
+
+class MessageAttributeValueTypeDef(
+    _RequiredMessageAttributeValueTypeDef, _OptionalMessageAttributeValueTypeDef
+):
+    pass
+
+_RequiredMessageSystemAttributeValueTypeDef = TypedDict(
+    "_RequiredMessageSystemAttributeValueTypeDef",
+    {
+        "DataType": str,
+    },
+)
+_OptionalMessageSystemAttributeValueTypeDef = TypedDict(
+    "_OptionalMessageSystemAttributeValueTypeDef",
+    {
+        "StringValue": str,
+        "BinaryValue": BlobTypeDef,
+        "StringListValues": Sequence[str],
+        "BinaryListValues": Sequence[BlobTypeDef],
+    },
+    total=False,
+)
+
+class MessageSystemAttributeValueTypeDef(
+    _RequiredMessageSystemAttributeValueTypeDef, _OptionalMessageSystemAttributeValueTypeDef
+):
+    pass
+
 CancelMessageMoveTaskResultTypeDef = TypedDict(
     "CancelMessageMoveTaskResultTypeDef",
     {
         "ApproximateNumberOfMessagesMoved": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -795,14 +798,26 @@
         "Attributes": Dict[MessageSystemAttributeNameType, str],
         "MD5OfMessageAttributes": str,
         "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
     },
     total=False,
 )
 
+SendMessageBatchResultTypeDef = TypedDict(
+    "SendMessageBatchResultTypeDef",
+    {
+        "Successful": List[SendMessageBatchResultEntryTypeDef],
+        "Failed": List[BatchResultErrorEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MessageAttributeValueUnionTypeDef = Union[
+    MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef
+]
 _RequiredSendMessageBatchRequestEntryTypeDef = TypedDict(
     "_RequiredSendMessageBatchRequestEntryTypeDef",
     {
         "Id": str,
         "MessageBody": str,
     },
 )
@@ -847,59 +862,48 @@
 
 class SendMessageRequestQueueSendMessageTypeDef(
     _RequiredSendMessageRequestQueueSendMessageTypeDef,
     _OptionalSendMessageRequestQueueSendMessageTypeDef,
 ):
     pass
 
+ReceiveMessageResultTypeDef = TypedDict(
+    "ReceiveMessageResultTypeDef",
+    {
+        "Messages": List[MessageTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredSendMessageRequestRequestTypeDef = TypedDict(
     "_RequiredSendMessageRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "MessageBody": str,
     },
 )
 _OptionalSendMessageRequestRequestTypeDef = TypedDict(
     "_OptionalSendMessageRequestRequestTypeDef",
     {
         "DelaySeconds": int,
-        "MessageAttributes": Mapping[
-            str, Union[MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef]
-        ],
+        "MessageAttributes": Mapping[str, MessageAttributeValueUnionTypeDef],
         "MessageSystemAttributes": Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ],
         "MessageDeduplicationId": str,
         "MessageGroupId": str,
     },
     total=False,
 )
 
 class SendMessageRequestRequestTypeDef(
     _RequiredSendMessageRequestRequestTypeDef, _OptionalSendMessageRequestRequestTypeDef
 ):
     pass
 
-SendMessageBatchResultTypeDef = TypedDict(
-    "SendMessageBatchResultTypeDef",
-    {
-        "Successful": List[SendMessageBatchResultEntryTypeDef],
-        "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ReceiveMessageResultTypeDef = TypedDict(
-    "ReceiveMessageResultTypeDef",
-    {
-        "Messages": List[MessageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 SendMessageBatchRequestQueueSendMessagesTypeDef = TypedDict(
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
     {
         "Entries": Sequence[SendMessageBatchRequestEntryTypeDef],
     },
 )
```

### Comparing `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs.egg-info/PKG-INFO` & `mypy-boto3-sqs-1.28.16/mypy_boto3_sqs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sqs
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SQS 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SQS 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sqs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 sqs type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sqs)](https://pepy.tech/project/mypy-boto3-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SQS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[boto3.SQS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
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
 [mypy-boto3-sqs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -78,15 +78,15 @@
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -403,26 +403,27 @@
 )
 
 
 def check_value(value: ListDeadLetterSourceQueuesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sqs.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sqs.type_defs import (
     AddPermissionRequestQueueAddPermissionTypeDef,
     AddPermissionRequestRequestTypeDef,
     BatchResultErrorEntryTypeDef,
+    BlobTypeDef,
     CancelMessageMoveTaskRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultEntryTypeDef,
     ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef,
     ChangeMessageVisibilityRequestRequestTypeDef,
     CreateQueueRequestRequestTypeDef,
@@ -437,27 +438,27 @@
     PaginatorConfigTypeDef,
     ListDeadLetterSourceQueuesRequestRequestTypeDef,
     ListMessageMoveTasksRequestRequestTypeDef,
     ListMessageMoveTasksResultEntryTypeDef,
     ListQueueTagsRequestRequestTypeDef,
     ListQueuesRequestRequestTypeDef,
     MessageAttributeValueOutputTypeDef,
-    MessageAttributeValueTypeDef,
-    MessageSystemAttributeValueTypeDef,
     PurgeQueueRequestRequestTypeDef,
     ReceiveMessageRequestQueueReceiveMessagesTypeDef,
     ReceiveMessageRequestRequestTypeDef,
     RemovePermissionRequestQueueRemovePermissionTypeDef,
     RemovePermissionRequestRequestTypeDef,
     SendMessageBatchResultEntryTypeDef,
     SetQueueAttributesRequestQueueSetAttributesTypeDef,
     SetQueueAttributesRequestRequestTypeDef,
     StartMessageMoveTaskRequestRequestTypeDef,
     TagQueueRequestRequestTypeDef,
     UntagQueueRequestRequestTypeDef,
+    MessageAttributeValueTypeDef,
+    MessageSystemAttributeValueTypeDef,
     CancelMessageMoveTaskResultTypeDef,
     CreateQueueResultTypeDef,
     EmptyResponseMetadataTypeDef,
     GetQueueAttributesResultTypeDef,
     GetQueueUrlResultTypeDef,
     ListDeadLetterSourceQueuesResultTypeDef,
     ListQueueTagsResultTypeDef,
@@ -470,25 +471,26 @@
     DeleteMessageBatchRequestQueueDeleteMessagesTypeDef,
     DeleteMessageBatchRequestRequestTypeDef,
     DeleteMessageBatchResultTypeDef,
     ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
     ListQueuesRequestListQueuesPaginateTypeDef,
     ListMessageMoveTasksResultTypeDef,
     MessageTypeDef,
+    SendMessageBatchResultTypeDef,
+    MessageAttributeValueUnionTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageRequestQueueSendMessageTypeDef,
-    SendMessageRequestRequestTypeDef,
-    SendMessageBatchResultTypeDef,
     ReceiveMessageResultTypeDef,
+    SendMessageRequestRequestTypeDef,
     SendMessageBatchRequestQueueSendMessagesTypeDef,
     SendMessageBatchRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddPermissionRequestQueueAddPermissionTypeDef:
+def get_value() -> AddPermissionRequestQueueAddPermissionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sqs-1.28.15.post1/mypy_boto3_sqs.egg-info/SOURCES.txt` & `mypy-boto3-sqs-1.28.16/mypy_boto3_sqs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.15.post1/setup.py` & `mypy-boto3-sqs-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sqs",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_sqs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SQS 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.SQS 1.28.16 service generated with mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -33,15 +33,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
-    keywords="boto3 sqs type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 sqs type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_sqs": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

