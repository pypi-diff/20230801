# Comparing `tmp/mypy-boto3-appflow-1.28.15.post2.tar.gz` & `tmp/mypy-boto3-appflow-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appflow-1.28.15.post2.tar", last modified: Sat Jul 29 10:02:30 2023, max compression
+gzip compressed data, was "mypy-boto3-appflow-1.28.16.tar", last modified: Tue Aug  1 11:36:11 2023, max compression
```

## Comparing `mypy-boto3-appflow-1.28.15.post2.tar` & `mypy-boto3-appflow-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:30.945007 mypy-boto3-appflow-1.28.15.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20715 2023-07-29 10:02:30.945007 mypy-boto3-appflow-1.28.15.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19222 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:30.937007 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20024 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19992 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18437 2023-07-29 09:38:09.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18435 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    86173 2023-07-29 09:38:12.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    86041 2023-07-29 09:38:11.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:30.945007 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20715 2023-07-29 10:02:30.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-29 10:02:30.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:30.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:02:30.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:30.945007 mypy-boto3-appflow-1.28.15.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:11.816950 mypy-boto3-appflow-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:10:39.000000 mypy-boto3-appflow-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20853 2023-08-01 11:36:11.808950 mypy-boto3-appflow-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19369 2023-08-01 11:10:39.000000 mypy-boto3-appflow-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:11.808950 mypy-boto3-appflow-1.28.16/mypy_boto3_appflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-01 11:10:39.000000 mypy-boto3-appflow-1.28.16/mypy_boto3_appflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-01 11:10:39.000000 mypy-boto3-appflow-1.28.16/mypy_boto3_appflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-01 11:10:39.000000 mypy-boto3-appflow-1.28.16/mypy_boto3_appflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19619 2023-08-01 11:10:40.000000 mypy-boto3-appflow-1.28.16/mypy_boto3_appflow/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19587 2023-08-01 11:10:39.000000 mypy-boto3-appflow-1.28.16/mypy_boto3_appflow/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18437 2023-08-01 11:10:40.000000 mypy-boto3-appflow-1.28.16/mypy_boto3_appflow/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18435 2023-08-01 11:10:40.000000 mypy-boto3-appflow-1.28.16/mypy_boto3_appflow/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:10:39.000000 mypy-boto3-appflow-1.28.16/mypy_boto3_appflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    86543 2023-08-01 11:10:42.000000 mypy-boto3-appflow-1.28.16/mypy_boto3_appflow/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86411 2023-08-01 11:10:41.000000 mypy-boto3-appflow-1.28.16/mypy_boto3_appflow/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:10:39.000000 mypy-boto3-appflow-1.28.16/mypy_boto3_appflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:11.808950 mypy-boto3-appflow-1.28.16/mypy_boto3_appflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20853 2023-08-01 11:36:11.000000 mypy-boto3-appflow-1.28.16/mypy_boto3_appflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-01 11:36:11.000000 mypy-boto3-appflow-1.28.16/mypy_boto3_appflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:11.000000 mypy-boto3-appflow-1.28.16/mypy_boto3_appflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:11.000000 mypy-boto3-appflow-1.28.16/mypy_boto3_appflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:11.000000 mypy-boto3-appflow-1.28.16/mypy_boto3_appflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 11:36:11.000000 mypy-boto3-appflow-1.28.16/mypy_boto3_appflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:11.816950 mypy-boto3-appflow-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-01 11:10:38.000000 mypy-boto3-appflow-1.28.16/setup.py
```

### Comparing `mypy-boto3-appflow-1.28.15.post2/LICENSE` & `mypy-boto3-appflow-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.15.post2/PKG-INFO` & `mypy-boto3-appflow-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appflow
-Version: 1.28.15.post2
-Summary: Type annotations for boto3.Appflow 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Appflow 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 appflow type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 appflow type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-appflow)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appflow)](https://pepy.tech/project/mypy-boto3-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Appflow 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[boto3.Appflow 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
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
 [mypy-boto3-appflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -330,20 +330,20 @@
 )
 
 
 def check_value(value: AggregationTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_appflow.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_appflow.type_defs import (
     AggregationConfigTypeDef,
     AmplitudeConnectorProfileCredentialsTypeDef,
     AmplitudeSourcePropertiesTypeDef,
     ApiKeyCredentialsTypeDef,
@@ -424,15 +424,15 @@
     PrefixConfigTypeDef,
     ResetConnectorMetadataCacheRequestRequestTypeDef,
     S3InputFormatConfigTypeDef,
     SuccessResponseHandlingConfigTypeDef,
     SAPODataSourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
     ScheduledTriggerPropertiesOutputTypeDef,
-    ScheduledTriggerPropertiesTypeDef,
+    TimestampTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     SingularSourcePropertiesTypeDef,
     SlackSourcePropertiesTypeDef,
     TrendmicroSourcePropertiesTypeDef,
     VeevaSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     StartFlowRequestRequestTypeDef,
@@ -493,17 +493,18 @@
     UpsolverS3OutputFormatConfigOutputTypeDef,
     S3OutputFormatConfigTypeDef,
     UpsolverS3OutputFormatConfigTypeDef,
     S3SourcePropertiesTypeDef,
     SAPODataDestinationPropertiesOutputTypeDef,
     SAPODataDestinationPropertiesTypeDef,
     TriggerPropertiesOutputTypeDef,
-    TriggerPropertiesTypeDef,
+    ScheduledTriggerPropertiesTypeDef,
     CustomConnectorProfileCredentialsTypeDef,
     SAPODataConnectorProfileCredentialsTypeDef,
+    TaskUnionTypeDef,
     RegisterConnectorRequestRequestTypeDef,
     UpdateConnectorRegistrationRequestRequestTypeDef,
     ListFlowsResponseTypeDef,
     SupportedFieldTypeDetailsTypeDef,
     ExecutionRecordTypeDef,
     AuthenticationConfigTypeDef,
     ConnectorProfilePropertiesOutputTypeDef,
@@ -511,40 +512,44 @@
     S3DestinationPropertiesOutputTypeDef,
     UpsolverDestinationPropertiesOutputTypeDef,
     S3DestinationPropertiesTypeDef,
     UpsolverDestinationPropertiesTypeDef,
     SourceConnectorPropertiesOutputTypeDef,
     SourceConnectorPropertiesTypeDef,
     TriggerConfigOutputTypeDef,
-    TriggerConfigTypeDef,
+    TriggerPropertiesTypeDef,
     ConnectorProfileCredentialsTypeDef,
     ConnectorEntityFieldTypeDef,
     DescribeFlowExecutionRecordsResponseTypeDef,
     ConnectorConfigurationTypeDef,
     ConnectorProfileTypeDef,
     DestinationConnectorPropertiesOutputTypeDef,
     DestinationConnectorPropertiesTypeDef,
     SourceFlowConfigOutputTypeDef,
     SourceFlowConfigTypeDef,
+    TriggerConfigTypeDef,
     ConnectorProfileConfigTypeDef,
     DescribeConnectorEntityResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeConnectorsResponseTypeDef,
     DescribeConnectorProfilesResponseTypeDef,
     DestinationFlowConfigOutputTypeDef,
     DestinationFlowConfigTypeDef,
+    SourceFlowConfigUnionTypeDef,
+    TriggerConfigUnionTypeDef,
     CreateConnectorProfileRequestRequestTypeDef,
     UpdateConnectorProfileRequestRequestTypeDef,
     DescribeFlowResponseTypeDef,
+    DestinationFlowConfigUnionTypeDef,
     CreateFlowRequestRequestTypeDef,
     UpdateFlowRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AggregationConfigTypeDef:
+def get_value() -> AggregationConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appflow-1.28.15.post2/README.md` & `mypy-boto3-appflow-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-appflow)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appflow)](https://pepy.tech/project/mypy-boto3-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Appflow 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[boto3.Appflow 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
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
 [mypy-boto3-appflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +41,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -298,20 +298,20 @@
 )
 
 
 def check_value(value: AggregationTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_appflow.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_appflow.type_defs import (
     AggregationConfigTypeDef,
     AmplitudeConnectorProfileCredentialsTypeDef,
     AmplitudeSourcePropertiesTypeDef,
     ApiKeyCredentialsTypeDef,
@@ -392,15 +392,15 @@
     PrefixConfigTypeDef,
     ResetConnectorMetadataCacheRequestRequestTypeDef,
     S3InputFormatConfigTypeDef,
     SuccessResponseHandlingConfigTypeDef,
     SAPODataSourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
     ScheduledTriggerPropertiesOutputTypeDef,
-    ScheduledTriggerPropertiesTypeDef,
+    TimestampTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     SingularSourcePropertiesTypeDef,
     SlackSourcePropertiesTypeDef,
     TrendmicroSourcePropertiesTypeDef,
     VeevaSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     StartFlowRequestRequestTypeDef,
@@ -461,17 +461,18 @@
     UpsolverS3OutputFormatConfigOutputTypeDef,
     S3OutputFormatConfigTypeDef,
     UpsolverS3OutputFormatConfigTypeDef,
     S3SourcePropertiesTypeDef,
     SAPODataDestinationPropertiesOutputTypeDef,
     SAPODataDestinationPropertiesTypeDef,
     TriggerPropertiesOutputTypeDef,
-    TriggerPropertiesTypeDef,
+    ScheduledTriggerPropertiesTypeDef,
     CustomConnectorProfileCredentialsTypeDef,
     SAPODataConnectorProfileCredentialsTypeDef,
+    TaskUnionTypeDef,
     RegisterConnectorRequestRequestTypeDef,
     UpdateConnectorRegistrationRequestRequestTypeDef,
     ListFlowsResponseTypeDef,
     SupportedFieldTypeDetailsTypeDef,
     ExecutionRecordTypeDef,
     AuthenticationConfigTypeDef,
     ConnectorProfilePropertiesOutputTypeDef,
@@ -479,40 +480,44 @@
     S3DestinationPropertiesOutputTypeDef,
     UpsolverDestinationPropertiesOutputTypeDef,
     S3DestinationPropertiesTypeDef,
     UpsolverDestinationPropertiesTypeDef,
     SourceConnectorPropertiesOutputTypeDef,
     SourceConnectorPropertiesTypeDef,
     TriggerConfigOutputTypeDef,
-    TriggerConfigTypeDef,
+    TriggerPropertiesTypeDef,
     ConnectorProfileCredentialsTypeDef,
     ConnectorEntityFieldTypeDef,
     DescribeFlowExecutionRecordsResponseTypeDef,
     ConnectorConfigurationTypeDef,
     ConnectorProfileTypeDef,
     DestinationConnectorPropertiesOutputTypeDef,
     DestinationConnectorPropertiesTypeDef,
     SourceFlowConfigOutputTypeDef,
     SourceFlowConfigTypeDef,
+    TriggerConfigTypeDef,
     ConnectorProfileConfigTypeDef,
     DescribeConnectorEntityResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeConnectorsResponseTypeDef,
     DescribeConnectorProfilesResponseTypeDef,
     DestinationFlowConfigOutputTypeDef,
     DestinationFlowConfigTypeDef,
+    SourceFlowConfigUnionTypeDef,
+    TriggerConfigUnionTypeDef,
     CreateConnectorProfileRequestRequestTypeDef,
     UpdateConnectorProfileRequestRequestTypeDef,
     DescribeFlowResponseTypeDef,
+    DestinationFlowConfigUnionTypeDef,
     CreateFlowRequestRequestTypeDef,
     UpdateFlowRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AggregationConfigTypeDef:
+def get_value() -> AggregationConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/__main__.py` & `mypy-boto3-appflow-1.28.16/mypy_boto3_appflow/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Appflow 1.28.15\nVersion:         1.28.15.post2\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Appflow 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15.post2")
+    print("1.28.16")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/client.py` & `mypy-boto3-appflow-1.28.16/mypy_boto3_appflow/client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_appflow.client import AppflowClient
 
     session = Session()
     client: AppflowClient = session.client("appflow")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ConnectionModeType, ConnectorTypeType
 from .type_defs import (
     CancelFlowExecutionsResponseTypeDef,
     ConnectorProfileConfigTypeDef,
@@ -27,66 +27,58 @@
     CreateFlowResponseTypeDef,
     DescribeConnectorEntityResponseTypeDef,
     DescribeConnectorProfilesResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeConnectorsResponseTypeDef,
     DescribeFlowExecutionRecordsResponseTypeDef,
     DescribeFlowResponseTypeDef,
-    DestinationFlowConfigOutputTypeDef,
-    DestinationFlowConfigTypeDef,
+    DestinationFlowConfigUnionTypeDef,
     ListConnectorEntitiesResponseTypeDef,
     ListConnectorsResponseTypeDef,
     ListFlowsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MetadataCatalogConfigTypeDef,
     RegisterConnectorResponseTypeDef,
-    SourceFlowConfigOutputTypeDef,
-    SourceFlowConfigTypeDef,
+    SourceFlowConfigUnionTypeDef,
     StartFlowResponseTypeDef,
     StopFlowResponseTypeDef,
-    TaskOutputTypeDef,
-    TaskTypeDef,
-    TriggerConfigOutputTypeDef,
-    TriggerConfigTypeDef,
+    TaskUnionTypeDef,
+    TriggerConfigUnionTypeDef,
     UpdateConnectorProfileResponseTypeDef,
     UpdateConnectorRegistrationResponseTypeDef,
     UpdateFlowResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AppflowClient",)
 
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
     ConnectorAuthenticationException: Type[BotocoreClientError]
     ConnectorServerException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnsupportedOperationException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class AppflowClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/)
     """
 
     meta: ClientMeta
@@ -95,41 +87,37 @@
     def exceptions(self) -> Exceptions:
         """
         AppflowClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#can_paginate)
         """
-
     def cancel_flow_executions(
         self, *, flowName: str, executionIds: Sequence[str] = ...
     ) -> CancelFlowExecutionsResponseTypeDef:
         """
         Cancels active runs for a flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.cancel_flow_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#cancel_flow_executions)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#close)
         """
-
     def create_connector_profile(
         self,
         *,
         connectorProfileName: str,
         connectorType: ConnectorTypeType,
         connectionMode: ConnectionModeType,
         connectorProfileConfig: ConnectorProfileConfigTypeDef,
@@ -140,67 +128,60 @@
         """
         Creates a new connector profile associated with your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.create_connector_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#create_connector_profile)
         """
-
     def create_flow(
         self,
         *,
         flowName: str,
-        triggerConfig: Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef],
-        sourceFlowConfig: Union[SourceFlowConfigTypeDef, SourceFlowConfigOutputTypeDef],
-        destinationFlowConfigList: Sequence[
-            Union[DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef]
-        ],
-        tasks: Sequence[Union[TaskTypeDef, TaskOutputTypeDef]],
+        triggerConfig: TriggerConfigUnionTypeDef,
+        sourceFlowConfig: SourceFlowConfigUnionTypeDef,
+        destinationFlowConfigList: Sequence[DestinationFlowConfigUnionTypeDef],
+        tasks: Sequence[TaskUnionTypeDef],
         description: str = ...,
         kmsArn: str = ...,
         tags: Mapping[str, str] = ...,
         metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
         clientToken: str = ...
     ) -> CreateFlowResponseTypeDef:
         """
         Enables your application to create a new flow using Amazon AppFlow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.create_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#create_flow)
         """
-
     def delete_connector_profile(
         self, *, connectorProfileName: str, forceDelete: bool = ...
     ) -> Dict[str, Any]:
         """
         Enables you to delete an existing connector profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.delete_connector_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#delete_connector_profile)
         """
-
     def delete_flow(self, *, flowName: str, forceDelete: bool = ...) -> Dict[str, Any]:
         """
         Enables your application to delete an existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.delete_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#delete_flow)
         """
-
     def describe_connector(
         self, *, connectorType: ConnectorTypeType, connectorLabel: str = ...
     ) -> DescribeConnectorResponseTypeDef:
         """
         Describes the given custom connector registered in your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connector)
         """
-
     def describe_connector_entity(
         self,
         *,
         connectorEntityName: str,
         connectorType: ConnectorTypeType = ...,
         connectorProfileName: str = ...,
         apiVersion: str = ...
@@ -208,15 +189,14 @@
         """
         Provides details regarding the entity used with the connector, with a
         description of the data model for each field in that entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector_entity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connector_entity)
         """
-
     def describe_connector_profiles(
         self,
         *,
         connectorProfileNames: Sequence[str] = ...,
         connectorType: ConnectorTypeType = ...,
         connectorLabel: str = ...,
         maxResults: int = ...,
@@ -225,61 +205,56 @@
         """
         Returns a list of `connector-profile` details matching the provided `connector-
         profile` names and `connector-types`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connector_profiles)
         """
-
     def describe_connectors(
         self,
         *,
         connectorTypes: Sequence[ConnectorTypeType] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeConnectorsResponseTypeDef:
         """
         Describes the connectors vended by Amazon AppFlow for specified connector types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connectors)
         """
-
     def describe_flow(self, *, flowName: str) -> DescribeFlowResponseTypeDef:
         """
         Provides a description of the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_flow)
         """
-
     def describe_flow_execution_records(
         self, *, flowName: str, maxResults: int = ..., nextToken: str = ...
     ) -> DescribeFlowExecutionRecordsResponseTypeDef:
         """
         Fetches the execution history of the flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_flow_execution_records)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_flow_execution_records)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#generate_presigned_url)
         """
-
     def list_connector_entities(
         self,
         *,
         connectorProfileName: str = ...,
         connectorType: ConnectorTypeType = ...,
         entitiesPath: str = ...,
         apiVersion: str = ...,
@@ -288,44 +263,40 @@
     ) -> ListConnectorEntitiesResponseTypeDef:
         """
         Returns the list of available connector entities supported by Amazon AppFlow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_connector_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_connector_entities)
         """
-
     def list_connectors(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListConnectorsResponseTypeDef:
         """
         Returns the list of all registered custom connectors in your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_connectors)
         """
-
     def list_flows(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListFlowsResponseTypeDef:
         """
         Lists all of the flows associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_flows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_flows)
         """
-
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Retrieves the tags that are associated with a specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_tags_for_resource)
         """
-
     def register_connector(
         self,
         *,
         connectorLabel: str = ...,
         description: str = ...,
         connectorProvisioningType: Literal["LAMBDA"] = ...,
         connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...,
@@ -333,15 +304,14 @@
     ) -> RegisterConnectorResponseTypeDef:
         """
         Registers a new custom connector with your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.register_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#register_connector)
         """
-
     def reset_connector_metadata_cache(
         self,
         *,
         connectorProfileName: str = ...,
         connectorType: ConnectorTypeType = ...,
         connectorEntityName: str = ...,
         entitiesPath: str = ...,
@@ -350,98 +320,88 @@
         """
         Resets metadata about your connector entities that Amazon AppFlow stored in its
         cache.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.reset_connector_metadata_cache)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#reset_connector_metadata_cache)
         """
-
     def start_flow(self, *, flowName: str, clientToken: str = ...) -> StartFlowResponseTypeDef:
         """
         Activates an existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.start_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#start_flow)
         """
-
     def stop_flow(self, *, flowName: str) -> StopFlowResponseTypeDef:
         """
         Deactivates the existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.stop_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#stop_flow)
         """
-
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Applies a tag to the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#tag_resource)
         """
-
     def unregister_connector(
         self, *, connectorLabel: str, forceDelete: bool = ...
     ) -> Dict[str, Any]:
         """
         Unregisters the custom connector registered in your account that matches the
         connector label provided in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.unregister_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#unregister_connector)
         """
-
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes a tag from the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#untag_resource)
         """
-
     def update_connector_profile(
         self,
         *,
         connectorProfileName: str,
         connectionMode: ConnectionModeType,
         connectorProfileConfig: ConnectorProfileConfigTypeDef,
         clientToken: str = ...
     ) -> UpdateConnectorProfileResponseTypeDef:
         """
         Updates a given connector profile associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_connector_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#update_connector_profile)
         """
-
     def update_connector_registration(
         self,
         *,
         connectorLabel: str,
         description: str = ...,
         connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...,
         clientToken: str = ...
     ) -> UpdateConnectorRegistrationResponseTypeDef:
         """
         Updates a custom connector that you've previously registered.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_connector_registration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#update_connector_registration)
         """
-
     def update_flow(
         self,
         *,
         flowName: str,
-        triggerConfig: Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef],
-        sourceFlowConfig: Union[SourceFlowConfigTypeDef, SourceFlowConfigOutputTypeDef],
-        destinationFlowConfigList: Sequence[
-            Union[DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef]
-        ],
-        tasks: Sequence[Union[TaskTypeDef, TaskOutputTypeDef]],
+        triggerConfig: TriggerConfigUnionTypeDef,
+        sourceFlowConfig: SourceFlowConfigUnionTypeDef,
+        destinationFlowConfigList: Sequence[DestinationFlowConfigUnionTypeDef],
+        tasks: Sequence[TaskUnionTypeDef],
         description: str = ...,
         metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
         clientToken: str = ...
     ) -> UpdateFlowResponseTypeDef:
         """
         Updates an existing flow.
```

### Comparing `mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/client.pyi` & `mypy-boto3-appflow-1.28.16/mypy_boto3_appflow/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_appflow.client import AppflowClient
 
     session = Session()
     client: AppflowClient = session.client("appflow")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ConnectionModeType, ConnectorTypeType
 from .type_defs import (
     CancelFlowExecutionsResponseTypeDef,
     ConnectorProfileConfigTypeDef,
@@ -27,62 +27,62 @@
     CreateFlowResponseTypeDef,
     DescribeConnectorEntityResponseTypeDef,
     DescribeConnectorProfilesResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeConnectorsResponseTypeDef,
     DescribeFlowExecutionRecordsResponseTypeDef,
     DescribeFlowResponseTypeDef,
-    DestinationFlowConfigOutputTypeDef,
-    DestinationFlowConfigTypeDef,
+    DestinationFlowConfigUnionTypeDef,
     ListConnectorEntitiesResponseTypeDef,
     ListConnectorsResponseTypeDef,
     ListFlowsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MetadataCatalogConfigTypeDef,
     RegisterConnectorResponseTypeDef,
-    SourceFlowConfigOutputTypeDef,
-    SourceFlowConfigTypeDef,
+    SourceFlowConfigUnionTypeDef,
     StartFlowResponseTypeDef,
     StopFlowResponseTypeDef,
-    TaskOutputTypeDef,
-    TaskTypeDef,
-    TriggerConfigOutputTypeDef,
-    TriggerConfigTypeDef,
+    TaskUnionTypeDef,
+    TriggerConfigUnionTypeDef,
     UpdateConnectorProfileResponseTypeDef,
     UpdateConnectorRegistrationResponseTypeDef,
     UpdateFlowResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("AppflowClient",)
 
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
     ConnectorAuthenticationException: Type[BotocoreClientError]
     ConnectorServerException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnsupportedOperationException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class AppflowClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/)
     """
 
     meta: ClientMeta
@@ -91,37 +91,41 @@
     def exceptions(self) -> Exceptions:
         """
         AppflowClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#can_paginate)
         """
+
     def cancel_flow_executions(
         self, *, flowName: str, executionIds: Sequence[str] = ...
     ) -> CancelFlowExecutionsResponseTypeDef:
         """
         Cancels active runs for a flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.cancel_flow_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#cancel_flow_executions)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#close)
         """
+
     def create_connector_profile(
         self,
         *,
         connectorProfileName: str,
         connectorType: ConnectorTypeType,
         connectionMode: ConnectionModeType,
         connectorProfileConfig: ConnectorProfileConfigTypeDef,
@@ -132,62 +136,65 @@
         """
         Creates a new connector profile associated with your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.create_connector_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#create_connector_profile)
         """
+
     def create_flow(
         self,
         *,
         flowName: str,
-        triggerConfig: Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef],
-        sourceFlowConfig: Union[SourceFlowConfigTypeDef, SourceFlowConfigOutputTypeDef],
-        destinationFlowConfigList: Sequence[
-            Union[DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef]
-        ],
-        tasks: Sequence[Union[TaskTypeDef, TaskOutputTypeDef]],
+        triggerConfig: TriggerConfigUnionTypeDef,
+        sourceFlowConfig: SourceFlowConfigUnionTypeDef,
+        destinationFlowConfigList: Sequence[DestinationFlowConfigUnionTypeDef],
+        tasks: Sequence[TaskUnionTypeDef],
         description: str = ...,
         kmsArn: str = ...,
         tags: Mapping[str, str] = ...,
         metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
         clientToken: str = ...
     ) -> CreateFlowResponseTypeDef:
         """
         Enables your application to create a new flow using Amazon AppFlow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.create_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#create_flow)
         """
+
     def delete_connector_profile(
         self, *, connectorProfileName: str, forceDelete: bool = ...
     ) -> Dict[str, Any]:
         """
         Enables you to delete an existing connector profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.delete_connector_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#delete_connector_profile)
         """
+
     def delete_flow(self, *, flowName: str, forceDelete: bool = ...) -> Dict[str, Any]:
         """
         Enables your application to delete an existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.delete_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#delete_flow)
         """
+
     def describe_connector(
         self, *, connectorType: ConnectorTypeType, connectorLabel: str = ...
     ) -> DescribeConnectorResponseTypeDef:
         """
         Describes the given custom connector registered in your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connector)
         """
+
     def describe_connector_entity(
         self,
         *,
         connectorEntityName: str,
         connectorType: ConnectorTypeType = ...,
         connectorProfileName: str = ...,
         apiVersion: str = ...
@@ -195,14 +202,15 @@
         """
         Provides details regarding the entity used with the connector, with a
         description of the data model for each field in that entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector_entity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connector_entity)
         """
+
     def describe_connector_profiles(
         self,
         *,
         connectorProfileNames: Sequence[str] = ...,
         connectorType: ConnectorTypeType = ...,
         connectorLabel: str = ...,
         maxResults: int = ...,
@@ -211,56 +219,61 @@
         """
         Returns a list of `connector-profile` details matching the provided `connector-
         profile` names and `connector-types`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connector_profiles)
         """
+
     def describe_connectors(
         self,
         *,
         connectorTypes: Sequence[ConnectorTypeType] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeConnectorsResponseTypeDef:
         """
         Describes the connectors vended by Amazon AppFlow for specified connector types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connectors)
         """
+
     def describe_flow(self, *, flowName: str) -> DescribeFlowResponseTypeDef:
         """
         Provides a description of the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_flow)
         """
+
     def describe_flow_execution_records(
         self, *, flowName: str, maxResults: int = ..., nextToken: str = ...
     ) -> DescribeFlowExecutionRecordsResponseTypeDef:
         """
         Fetches the execution history of the flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_flow_execution_records)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_flow_execution_records)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#generate_presigned_url)
         """
+
     def list_connector_entities(
         self,
         *,
         connectorProfileName: str = ...,
         connectorType: ConnectorTypeType = ...,
         entitiesPath: str = ...,
         apiVersion: str = ...,
@@ -269,40 +282,44 @@
     ) -> ListConnectorEntitiesResponseTypeDef:
         """
         Returns the list of available connector entities supported by Amazon AppFlow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_connector_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_connector_entities)
         """
+
     def list_connectors(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListConnectorsResponseTypeDef:
         """
         Returns the list of all registered custom connectors in your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_connectors)
         """
+
     def list_flows(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListFlowsResponseTypeDef:
         """
         Lists all of the flows associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_flows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_flows)
         """
+
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Retrieves the tags that are associated with a specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_tags_for_resource)
         """
+
     def register_connector(
         self,
         *,
         connectorLabel: str = ...,
         description: str = ...,
         connectorProvisioningType: Literal["LAMBDA"] = ...,
         connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...,
@@ -310,14 +327,15 @@
     ) -> RegisterConnectorResponseTypeDef:
         """
         Registers a new custom connector with your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.register_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#register_connector)
         """
+
     def reset_connector_metadata_cache(
         self,
         *,
         connectorProfileName: str = ...,
         connectorType: ConnectorTypeType = ...,
         connectorEntityName: str = ...,
         entitiesPath: str = ...,
@@ -326,90 +344,96 @@
         """
         Resets metadata about your connector entities that Amazon AppFlow stored in its
         cache.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.reset_connector_metadata_cache)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#reset_connector_metadata_cache)
         """
+
     def start_flow(self, *, flowName: str, clientToken: str = ...) -> StartFlowResponseTypeDef:
         """
         Activates an existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.start_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#start_flow)
         """
+
     def stop_flow(self, *, flowName: str) -> StopFlowResponseTypeDef:
         """
         Deactivates the existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.stop_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#stop_flow)
         """
+
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Applies a tag to the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#tag_resource)
         """
+
     def unregister_connector(
         self, *, connectorLabel: str, forceDelete: bool = ...
     ) -> Dict[str, Any]:
         """
         Unregisters the custom connector registered in your account that matches the
         connector label provided in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.unregister_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#unregister_connector)
         """
+
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes a tag from the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#untag_resource)
         """
+
     def update_connector_profile(
         self,
         *,
         connectorProfileName: str,
         connectionMode: ConnectionModeType,
         connectorProfileConfig: ConnectorProfileConfigTypeDef,
         clientToken: str = ...
     ) -> UpdateConnectorProfileResponseTypeDef:
         """
         Updates a given connector profile associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_connector_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#update_connector_profile)
         """
+
     def update_connector_registration(
         self,
         *,
         connectorLabel: str,
         description: str = ...,
         connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...,
         clientToken: str = ...
     ) -> UpdateConnectorRegistrationResponseTypeDef:
         """
         Updates a custom connector that you've previously registered.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_connector_registration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#update_connector_registration)
         """
+
     def update_flow(
         self,
         *,
         flowName: str,
-        triggerConfig: Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef],
-        sourceFlowConfig: Union[SourceFlowConfigTypeDef, SourceFlowConfigOutputTypeDef],
-        destinationFlowConfigList: Sequence[
-            Union[DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef]
-        ],
-        tasks: Sequence[Union[TaskTypeDef, TaskOutputTypeDef]],
+        triggerConfig: TriggerConfigUnionTypeDef,
+        sourceFlowConfig: SourceFlowConfigUnionTypeDef,
+        destinationFlowConfigList: Sequence[DestinationFlowConfigUnionTypeDef],
+        tasks: Sequence[TaskUnionTypeDef],
         description: str = ...,
         metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
         clientToken: str = ...
     ) -> UpdateFlowResponseTypeDef:
         """
         Updates an existing flow.
```

### Comparing `mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/literals.py` & `mypy-boto3-appflow-1.28.16/mypy_boto3_appflow/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/literals.pyi` & `mypy-boto3-appflow-1.28.16/mypy_boto3_appflow/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/type_defs.py` & `mypy-boto3-appflow-1.28.16/mypy_boto3_appflow/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_appflow.type_defs import AggregationConfigTypeDef
 
-    data: AggregationConfigTypeDef = {...}
+    data: AggregationConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -151,15 +151,15 @@
     "PrefixConfigTypeDef",
     "ResetConnectorMetadataCacheRequestRequestTypeDef",
     "S3InputFormatConfigTypeDef",
     "SuccessResponseHandlingConfigTypeDef",
     "SAPODataSourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
     "ScheduledTriggerPropertiesOutputTypeDef",
-    "ScheduledTriggerPropertiesTypeDef",
+    "TimestampTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "SingularSourcePropertiesTypeDef",
     "SlackSourcePropertiesTypeDef",
     "TrendmicroSourcePropertiesTypeDef",
     "VeevaSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "StartFlowRequestRequestTypeDef",
@@ -220,17 +220,18 @@
     "UpsolverS3OutputFormatConfigOutputTypeDef",
     "S3OutputFormatConfigTypeDef",
     "UpsolverS3OutputFormatConfigTypeDef",
     "S3SourcePropertiesTypeDef",
     "SAPODataDestinationPropertiesOutputTypeDef",
     "SAPODataDestinationPropertiesTypeDef",
     "TriggerPropertiesOutputTypeDef",
-    "TriggerPropertiesTypeDef",
+    "ScheduledTriggerPropertiesTypeDef",
     "CustomConnectorProfileCredentialsTypeDef",
     "SAPODataConnectorProfileCredentialsTypeDef",
+    "TaskUnionTypeDef",
     "RegisterConnectorRequestRequestTypeDef",
     "UpdateConnectorRegistrationRequestRequestTypeDef",
     "ListFlowsResponseTypeDef",
     "SupportedFieldTypeDetailsTypeDef",
     "ExecutionRecordTypeDef",
     "AuthenticationConfigTypeDef",
     "ConnectorProfilePropertiesOutputTypeDef",
@@ -238,34 +239,38 @@
     "S3DestinationPropertiesOutputTypeDef",
     "UpsolverDestinationPropertiesOutputTypeDef",
     "S3DestinationPropertiesTypeDef",
     "UpsolverDestinationPropertiesTypeDef",
     "SourceConnectorPropertiesOutputTypeDef",
     "SourceConnectorPropertiesTypeDef",
     "TriggerConfigOutputTypeDef",
-    "TriggerConfigTypeDef",
+    "TriggerPropertiesTypeDef",
     "ConnectorProfileCredentialsTypeDef",
     "ConnectorEntityFieldTypeDef",
     "DescribeFlowExecutionRecordsResponseTypeDef",
     "ConnectorConfigurationTypeDef",
     "ConnectorProfileTypeDef",
     "DestinationConnectorPropertiesOutputTypeDef",
     "DestinationConnectorPropertiesTypeDef",
     "SourceFlowConfigOutputTypeDef",
     "SourceFlowConfigTypeDef",
+    "TriggerConfigTypeDef",
     "ConnectorProfileConfigTypeDef",
     "DescribeConnectorEntityResponseTypeDef",
     "DescribeConnectorResponseTypeDef",
     "DescribeConnectorsResponseTypeDef",
     "DescribeConnectorProfilesResponseTypeDef",
     "DestinationFlowConfigOutputTypeDef",
     "DestinationFlowConfigTypeDef",
+    "SourceFlowConfigUnionTypeDef",
+    "TriggerConfigUnionTypeDef",
     "CreateConnectorProfileRequestRequestTypeDef",
     "UpdateConnectorProfileRequestRequestTypeDef",
     "DescribeFlowResponseTypeDef",
+    "DestinationFlowConfigUnionTypeDef",
     "CreateFlowRequestRequestTypeDef",
     "UpdateFlowRequestRequestTypeDef",
 )
 
 AggregationConfigTypeDef = TypedDict(
     "AggregationConfigTypeDef",
     {
@@ -1260,41 +1265,15 @@
 class ScheduledTriggerPropertiesOutputTypeDef(
     _RequiredScheduledTriggerPropertiesOutputTypeDef,
     _OptionalScheduledTriggerPropertiesOutputTypeDef,
 ):
     pass
 
 
-_RequiredScheduledTriggerPropertiesTypeDef = TypedDict(
-    "_RequiredScheduledTriggerPropertiesTypeDef",
-    {
-        "scheduleExpression": str,
-    },
-)
-_OptionalScheduledTriggerPropertiesTypeDef = TypedDict(
-    "_OptionalScheduledTriggerPropertiesTypeDef",
-    {
-        "dataPullMode": DataPullModeType,
-        "scheduleStartTime": Union[datetime, str],
-        "scheduleEndTime": Union[datetime, str],
-        "timezone": str,
-        "scheduleOffset": int,
-        "firstExecutionFrom": Union[datetime, str],
-        "flowErrorDeactivationThreshold": int,
-    },
-    total=False,
-)
-
-
-class ScheduledTriggerPropertiesTypeDef(
-    _RequiredScheduledTriggerPropertiesTypeDef, _OptionalScheduledTriggerPropertiesTypeDef
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 ServiceNowSourcePropertiesTypeDef = TypedDict(
     "ServiceNowSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -2378,22 +2357,41 @@
     "TriggerPropertiesOutputTypeDef",
     {
         "Scheduled": ScheduledTriggerPropertiesOutputTypeDef,
     },
     total=False,
 )
 
-TriggerPropertiesTypeDef = TypedDict(
-    "TriggerPropertiesTypeDef",
+_RequiredScheduledTriggerPropertiesTypeDef = TypedDict(
+    "_RequiredScheduledTriggerPropertiesTypeDef",
     {
-        "Scheduled": ScheduledTriggerPropertiesTypeDef,
+        "scheduleExpression": str,
+    },
+)
+_OptionalScheduledTriggerPropertiesTypeDef = TypedDict(
+    "_OptionalScheduledTriggerPropertiesTypeDef",
+    {
+        "dataPullMode": DataPullModeType,
+        "scheduleStartTime": TimestampTypeDef,
+        "scheduleEndTime": TimestampTypeDef,
+        "timezone": str,
+        "scheduleOffset": int,
+        "firstExecutionFrom": TimestampTypeDef,
+        "flowErrorDeactivationThreshold": int,
     },
     total=False,
 )
 
+
+class ScheduledTriggerPropertiesTypeDef(
+    _RequiredScheduledTriggerPropertiesTypeDef, _OptionalScheduledTriggerPropertiesTypeDef
+):
+    pass
+
+
 _RequiredCustomConnectorProfileCredentialsTypeDef = TypedDict(
     "_RequiredCustomConnectorProfileCredentialsTypeDef",
     {
         "authenticationType": AuthenticationTypeType,
     },
 )
 _OptionalCustomConnectorProfileCredentialsTypeDef = TypedDict(
@@ -2420,14 +2418,15 @@
     {
         "basicAuthCredentials": BasicAuthCredentialsTypeDef,
         "oAuthCredentials": OAuthCredentialsTypeDef,
     },
     total=False,
 )
 
+TaskUnionTypeDef = Union[TaskTypeDef, TaskOutputTypeDef]
 RegisterConnectorRequestRequestTypeDef = TypedDict(
     "RegisterConnectorRequestRequestTypeDef",
     {
         "connectorLabel": str,
         "description": str,
         "connectorProvisioningType": Literal["LAMBDA"],
         "connectorProvisioningConfig": ConnectorProvisioningConfigTypeDef,
@@ -2710,33 +2709,22 @@
 
 class TriggerConfigOutputTypeDef(
     _RequiredTriggerConfigOutputTypeDef, _OptionalTriggerConfigOutputTypeDef
 ):
     pass
 
 
-_RequiredTriggerConfigTypeDef = TypedDict(
-    "_RequiredTriggerConfigTypeDef",
-    {
-        "triggerType": TriggerTypeType,
-    },
-)
-_OptionalTriggerConfigTypeDef = TypedDict(
-    "_OptionalTriggerConfigTypeDef",
+TriggerPropertiesTypeDef = TypedDict(
+    "TriggerPropertiesTypeDef",
     {
-        "triggerProperties": TriggerPropertiesTypeDef,
+        "Scheduled": ScheduledTriggerPropertiesTypeDef,
     },
     total=False,
 )
 
-
-class TriggerConfigTypeDef(_RequiredTriggerConfigTypeDef, _OptionalTriggerConfigTypeDef):
-    pass
-
-
 ConnectorProfileCredentialsTypeDef = TypedDict(
     "ConnectorProfileCredentialsTypeDef",
     {
         "Amplitude": AmplitudeConnectorProfileCredentialsTypeDef,
         "Datadog": DatadogConnectorProfileCredentialsTypeDef,
         "Dynatrace": DynatraceConnectorProfileCredentialsTypeDef,
         "GoogleAnalytics": GoogleAnalyticsConnectorProfileCredentialsTypeDef,
@@ -2932,14 +2920,33 @@
 )
 
 
 class SourceFlowConfigTypeDef(_RequiredSourceFlowConfigTypeDef, _OptionalSourceFlowConfigTypeDef):
     pass
 
 
+_RequiredTriggerConfigTypeDef = TypedDict(
+    "_RequiredTriggerConfigTypeDef",
+    {
+        "triggerType": TriggerTypeType,
+    },
+)
+_OptionalTriggerConfigTypeDef = TypedDict(
+    "_OptionalTriggerConfigTypeDef",
+    {
+        "triggerProperties": TriggerPropertiesTypeDef,
+    },
+    total=False,
+)
+
+
+class TriggerConfigTypeDef(_RequiredTriggerConfigTypeDef, _OptionalTriggerConfigTypeDef):
+    pass
+
+
 _RequiredConnectorProfileConfigTypeDef = TypedDict(
     "_RequiredConnectorProfileConfigTypeDef",
     {
         "connectorProfileProperties": ConnectorProfilePropertiesTypeDef,
     },
 )
 _OptionalConnectorProfileConfigTypeDef = TypedDict(
@@ -3034,14 +3041,16 @@
 
 class DestinationFlowConfigTypeDef(
     _RequiredDestinationFlowConfigTypeDef, _OptionalDestinationFlowConfigTypeDef
 ):
     pass
 
 
+SourceFlowConfigUnionTypeDef = Union[SourceFlowConfigTypeDef, SourceFlowConfigOutputTypeDef]
+TriggerConfigUnionTypeDef = Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef]
 _RequiredCreateConnectorProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectorProfileRequestRequestTypeDef",
     {
         "connectorProfileName": str,
         "connectorType": ConnectorTypeType,
         "connectionMode": ConnectionModeType,
         "connectorProfileConfig": ConnectorProfileConfigTypeDef,
@@ -3111,24 +3120,25 @@
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
         "lastRunMetadataCatalogDetails": List[MetadataCatalogDetailTypeDef],
         "schemaVersion": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DestinationFlowConfigUnionTypeDef = Union[
+    DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef
+]
 _RequiredCreateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
-        "destinationFlowConfigList": Sequence[
-            Union[DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef]
-        ],
-        "tasks": Sequence[Union[TaskTypeDef, TaskOutputTypeDef]],
+        "destinationFlowConfigList": Sequence[DestinationFlowConfigUnionTypeDef],
+        "tasks": Sequence[TaskUnionTypeDef],
     },
 )
 _OptionalCreateFlowRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFlowRequestRequestTypeDef",
     {
         "description": str,
         "kmsArn": str,
@@ -3148,18 +3158,16 @@
 
 _RequiredUpdateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
-        "destinationFlowConfigList": Sequence[
-            Union[DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef]
-        ],
-        "tasks": Sequence[Union[TaskTypeDef, TaskOutputTypeDef]],
+        "destinationFlowConfigList": Sequence[DestinationFlowConfigUnionTypeDef],
+        "tasks": Sequence[TaskUnionTypeDef],
     },
 )
 _OptionalUpdateFlowRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateFlowRequestRequestTypeDef",
     {
         "description": str,
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
```

### Comparing `mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/type_defs.pyi` & `mypy-boto3-appflow-1.28.16/mypy_boto3_appflow/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_appflow.type_defs import AggregationConfigTypeDef
 
-    data: AggregationConfigTypeDef = {...}
+    data: AggregationConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -150,15 +150,15 @@
     "PrefixConfigTypeDef",
     "ResetConnectorMetadataCacheRequestRequestTypeDef",
     "S3InputFormatConfigTypeDef",
     "SuccessResponseHandlingConfigTypeDef",
     "SAPODataSourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
     "ScheduledTriggerPropertiesOutputTypeDef",
-    "ScheduledTriggerPropertiesTypeDef",
+    "TimestampTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "SingularSourcePropertiesTypeDef",
     "SlackSourcePropertiesTypeDef",
     "TrendmicroSourcePropertiesTypeDef",
     "VeevaSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "StartFlowRequestRequestTypeDef",
@@ -219,17 +219,18 @@
     "UpsolverS3OutputFormatConfigOutputTypeDef",
     "S3OutputFormatConfigTypeDef",
     "UpsolverS3OutputFormatConfigTypeDef",
     "S3SourcePropertiesTypeDef",
     "SAPODataDestinationPropertiesOutputTypeDef",
     "SAPODataDestinationPropertiesTypeDef",
     "TriggerPropertiesOutputTypeDef",
-    "TriggerPropertiesTypeDef",
+    "ScheduledTriggerPropertiesTypeDef",
     "CustomConnectorProfileCredentialsTypeDef",
     "SAPODataConnectorProfileCredentialsTypeDef",
+    "TaskUnionTypeDef",
     "RegisterConnectorRequestRequestTypeDef",
     "UpdateConnectorRegistrationRequestRequestTypeDef",
     "ListFlowsResponseTypeDef",
     "SupportedFieldTypeDetailsTypeDef",
     "ExecutionRecordTypeDef",
     "AuthenticationConfigTypeDef",
     "ConnectorProfilePropertiesOutputTypeDef",
@@ -237,34 +238,38 @@
     "S3DestinationPropertiesOutputTypeDef",
     "UpsolverDestinationPropertiesOutputTypeDef",
     "S3DestinationPropertiesTypeDef",
     "UpsolverDestinationPropertiesTypeDef",
     "SourceConnectorPropertiesOutputTypeDef",
     "SourceConnectorPropertiesTypeDef",
     "TriggerConfigOutputTypeDef",
-    "TriggerConfigTypeDef",
+    "TriggerPropertiesTypeDef",
     "ConnectorProfileCredentialsTypeDef",
     "ConnectorEntityFieldTypeDef",
     "DescribeFlowExecutionRecordsResponseTypeDef",
     "ConnectorConfigurationTypeDef",
     "ConnectorProfileTypeDef",
     "DestinationConnectorPropertiesOutputTypeDef",
     "DestinationConnectorPropertiesTypeDef",
     "SourceFlowConfigOutputTypeDef",
     "SourceFlowConfigTypeDef",
+    "TriggerConfigTypeDef",
     "ConnectorProfileConfigTypeDef",
     "DescribeConnectorEntityResponseTypeDef",
     "DescribeConnectorResponseTypeDef",
     "DescribeConnectorsResponseTypeDef",
     "DescribeConnectorProfilesResponseTypeDef",
     "DestinationFlowConfigOutputTypeDef",
     "DestinationFlowConfigTypeDef",
+    "SourceFlowConfigUnionTypeDef",
+    "TriggerConfigUnionTypeDef",
     "CreateConnectorProfileRequestRequestTypeDef",
     "UpdateConnectorProfileRequestRequestTypeDef",
     "DescribeFlowResponseTypeDef",
+    "DestinationFlowConfigUnionTypeDef",
     "CreateFlowRequestRequestTypeDef",
     "UpdateFlowRequestRequestTypeDef",
 )
 
 AggregationConfigTypeDef = TypedDict(
     "AggregationConfigTypeDef",
     {
@@ -1227,39 +1232,15 @@
 
 class ScheduledTriggerPropertiesOutputTypeDef(
     _RequiredScheduledTriggerPropertiesOutputTypeDef,
     _OptionalScheduledTriggerPropertiesOutputTypeDef,
 ):
     pass
 
-_RequiredScheduledTriggerPropertiesTypeDef = TypedDict(
-    "_RequiredScheduledTriggerPropertiesTypeDef",
-    {
-        "scheduleExpression": str,
-    },
-)
-_OptionalScheduledTriggerPropertiesTypeDef = TypedDict(
-    "_OptionalScheduledTriggerPropertiesTypeDef",
-    {
-        "dataPullMode": DataPullModeType,
-        "scheduleStartTime": Union[datetime, str],
-        "scheduleEndTime": Union[datetime, str],
-        "timezone": str,
-        "scheduleOffset": int,
-        "firstExecutionFrom": Union[datetime, str],
-        "flowErrorDeactivationThreshold": int,
-    },
-    total=False,
-)
-
-class ScheduledTriggerPropertiesTypeDef(
-    _RequiredScheduledTriggerPropertiesTypeDef, _OptionalScheduledTriggerPropertiesTypeDef
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 ServiceNowSourcePropertiesTypeDef = TypedDict(
     "ServiceNowSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -2281,22 +2262,39 @@
     "TriggerPropertiesOutputTypeDef",
     {
         "Scheduled": ScheduledTriggerPropertiesOutputTypeDef,
     },
     total=False,
 )
 
-TriggerPropertiesTypeDef = TypedDict(
-    "TriggerPropertiesTypeDef",
+_RequiredScheduledTriggerPropertiesTypeDef = TypedDict(
+    "_RequiredScheduledTriggerPropertiesTypeDef",
     {
-        "Scheduled": ScheduledTriggerPropertiesTypeDef,
+        "scheduleExpression": str,
+    },
+)
+_OptionalScheduledTriggerPropertiesTypeDef = TypedDict(
+    "_OptionalScheduledTriggerPropertiesTypeDef",
+    {
+        "dataPullMode": DataPullModeType,
+        "scheduleStartTime": TimestampTypeDef,
+        "scheduleEndTime": TimestampTypeDef,
+        "timezone": str,
+        "scheduleOffset": int,
+        "firstExecutionFrom": TimestampTypeDef,
+        "flowErrorDeactivationThreshold": int,
     },
     total=False,
 )
 
+class ScheduledTriggerPropertiesTypeDef(
+    _RequiredScheduledTriggerPropertiesTypeDef, _OptionalScheduledTriggerPropertiesTypeDef
+):
+    pass
+
 _RequiredCustomConnectorProfileCredentialsTypeDef = TypedDict(
     "_RequiredCustomConnectorProfileCredentialsTypeDef",
     {
         "authenticationType": AuthenticationTypeType,
     },
 )
 _OptionalCustomConnectorProfileCredentialsTypeDef = TypedDict(
@@ -2321,14 +2319,15 @@
     {
         "basicAuthCredentials": BasicAuthCredentialsTypeDef,
         "oAuthCredentials": OAuthCredentialsTypeDef,
     },
     total=False,
 )
 
+TaskUnionTypeDef = Union[TaskTypeDef, TaskOutputTypeDef]
 RegisterConnectorRequestRequestTypeDef = TypedDict(
     "RegisterConnectorRequestRequestTypeDef",
     {
         "connectorLabel": str,
         "description": str,
         "connectorProvisioningType": Literal["LAMBDA"],
         "connectorProvisioningConfig": ConnectorProvisioningConfigTypeDef,
@@ -2599,31 +2598,22 @@
 )
 
 class TriggerConfigOutputTypeDef(
     _RequiredTriggerConfigOutputTypeDef, _OptionalTriggerConfigOutputTypeDef
 ):
     pass
 
-_RequiredTriggerConfigTypeDef = TypedDict(
-    "_RequiredTriggerConfigTypeDef",
-    {
-        "triggerType": TriggerTypeType,
-    },
-)
-_OptionalTriggerConfigTypeDef = TypedDict(
-    "_OptionalTriggerConfigTypeDef",
+TriggerPropertiesTypeDef = TypedDict(
+    "TriggerPropertiesTypeDef",
     {
-        "triggerProperties": TriggerPropertiesTypeDef,
+        "Scheduled": ScheduledTriggerPropertiesTypeDef,
     },
     total=False,
 )
 
-class TriggerConfigTypeDef(_RequiredTriggerConfigTypeDef, _OptionalTriggerConfigTypeDef):
-    pass
-
 ConnectorProfileCredentialsTypeDef = TypedDict(
     "ConnectorProfileCredentialsTypeDef",
     {
         "Amplitude": AmplitudeConnectorProfileCredentialsTypeDef,
         "Datadog": DatadogConnectorProfileCredentialsTypeDef,
         "Dynatrace": DynatraceConnectorProfileCredentialsTypeDef,
         "GoogleAnalytics": GoogleAnalyticsConnectorProfileCredentialsTypeDef,
@@ -2813,14 +2803,31 @@
     },
     total=False,
 )
 
 class SourceFlowConfigTypeDef(_RequiredSourceFlowConfigTypeDef, _OptionalSourceFlowConfigTypeDef):
     pass
 
+_RequiredTriggerConfigTypeDef = TypedDict(
+    "_RequiredTriggerConfigTypeDef",
+    {
+        "triggerType": TriggerTypeType,
+    },
+)
+_OptionalTriggerConfigTypeDef = TypedDict(
+    "_OptionalTriggerConfigTypeDef",
+    {
+        "triggerProperties": TriggerPropertiesTypeDef,
+    },
+    total=False,
+)
+
+class TriggerConfigTypeDef(_RequiredTriggerConfigTypeDef, _OptionalTriggerConfigTypeDef):
+    pass
+
 _RequiredConnectorProfileConfigTypeDef = TypedDict(
     "_RequiredConnectorProfileConfigTypeDef",
     {
         "connectorProfileProperties": ConnectorProfilePropertiesTypeDef,
     },
 )
 _OptionalConnectorProfileConfigTypeDef = TypedDict(
@@ -2909,14 +2916,16 @@
 )
 
 class DestinationFlowConfigTypeDef(
     _RequiredDestinationFlowConfigTypeDef, _OptionalDestinationFlowConfigTypeDef
 ):
     pass
 
+SourceFlowConfigUnionTypeDef = Union[SourceFlowConfigTypeDef, SourceFlowConfigOutputTypeDef]
+TriggerConfigUnionTypeDef = Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef]
 _RequiredCreateConnectorProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectorProfileRequestRequestTypeDef",
     {
         "connectorProfileName": str,
         "connectorType": ConnectorTypeType,
         "connectionMode": ConnectionModeType,
         "connectorProfileConfig": ConnectorProfileConfigTypeDef,
@@ -2982,24 +2991,25 @@
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
         "lastRunMetadataCatalogDetails": List[MetadataCatalogDetailTypeDef],
         "schemaVersion": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DestinationFlowConfigUnionTypeDef = Union[
+    DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef
+]
 _RequiredCreateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
-        "destinationFlowConfigList": Sequence[
-            Union[DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef]
-        ],
-        "tasks": Sequence[Union[TaskTypeDef, TaskOutputTypeDef]],
+        "destinationFlowConfigList": Sequence[DestinationFlowConfigUnionTypeDef],
+        "tasks": Sequence[TaskUnionTypeDef],
     },
 )
 _OptionalCreateFlowRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFlowRequestRequestTypeDef",
     {
         "description": str,
         "kmsArn": str,
@@ -3017,18 +3027,16 @@
 
 _RequiredUpdateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
-        "destinationFlowConfigList": Sequence[
-            Union[DestinationFlowConfigTypeDef, DestinationFlowConfigOutputTypeDef]
-        ],
-        "tasks": Sequence[Union[TaskTypeDef, TaskOutputTypeDef]],
+        "destinationFlowConfigList": Sequence[DestinationFlowConfigUnionTypeDef],
+        "tasks": Sequence[TaskUnionTypeDef],
     },
 )
 _OptionalUpdateFlowRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateFlowRequestRequestTypeDef",
     {
         "description": str,
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
```

### Comparing `mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow.egg-info/PKG-INFO` & `mypy-boto3-appflow-1.28.16/mypy_boto3_appflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appflow
-Version: 1.28.15.post2
-Summary: Type annotations for boto3.Appflow 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Appflow 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 appflow type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 appflow type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-appflow)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appflow)](https://pepy.tech/project/mypy-boto3-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Appflow 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[boto3.Appflow 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
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
 [mypy-boto3-appflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -330,20 +330,20 @@
 )
 
 
 def check_value(value: AggregationTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_appflow.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_appflow.type_defs import (
     AggregationConfigTypeDef,
     AmplitudeConnectorProfileCredentialsTypeDef,
     AmplitudeSourcePropertiesTypeDef,
     ApiKeyCredentialsTypeDef,
@@ -424,15 +424,15 @@
     PrefixConfigTypeDef,
     ResetConnectorMetadataCacheRequestRequestTypeDef,
     S3InputFormatConfigTypeDef,
     SuccessResponseHandlingConfigTypeDef,
     SAPODataSourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
     ScheduledTriggerPropertiesOutputTypeDef,
-    ScheduledTriggerPropertiesTypeDef,
+    TimestampTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     SingularSourcePropertiesTypeDef,
     SlackSourcePropertiesTypeDef,
     TrendmicroSourcePropertiesTypeDef,
     VeevaSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     StartFlowRequestRequestTypeDef,
@@ -493,17 +493,18 @@
     UpsolverS3OutputFormatConfigOutputTypeDef,
     S3OutputFormatConfigTypeDef,
     UpsolverS3OutputFormatConfigTypeDef,
     S3SourcePropertiesTypeDef,
     SAPODataDestinationPropertiesOutputTypeDef,
     SAPODataDestinationPropertiesTypeDef,
     TriggerPropertiesOutputTypeDef,
-    TriggerPropertiesTypeDef,
+    ScheduledTriggerPropertiesTypeDef,
     CustomConnectorProfileCredentialsTypeDef,
     SAPODataConnectorProfileCredentialsTypeDef,
+    TaskUnionTypeDef,
     RegisterConnectorRequestRequestTypeDef,
     UpdateConnectorRegistrationRequestRequestTypeDef,
     ListFlowsResponseTypeDef,
     SupportedFieldTypeDetailsTypeDef,
     ExecutionRecordTypeDef,
     AuthenticationConfigTypeDef,
     ConnectorProfilePropertiesOutputTypeDef,
@@ -511,40 +512,44 @@
     S3DestinationPropertiesOutputTypeDef,
     UpsolverDestinationPropertiesOutputTypeDef,
     S3DestinationPropertiesTypeDef,
     UpsolverDestinationPropertiesTypeDef,
     SourceConnectorPropertiesOutputTypeDef,
     SourceConnectorPropertiesTypeDef,
     TriggerConfigOutputTypeDef,
-    TriggerConfigTypeDef,
+    TriggerPropertiesTypeDef,
     ConnectorProfileCredentialsTypeDef,
     ConnectorEntityFieldTypeDef,
     DescribeFlowExecutionRecordsResponseTypeDef,
     ConnectorConfigurationTypeDef,
     ConnectorProfileTypeDef,
     DestinationConnectorPropertiesOutputTypeDef,
     DestinationConnectorPropertiesTypeDef,
     SourceFlowConfigOutputTypeDef,
     SourceFlowConfigTypeDef,
+    TriggerConfigTypeDef,
     ConnectorProfileConfigTypeDef,
     DescribeConnectorEntityResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeConnectorsResponseTypeDef,
     DescribeConnectorProfilesResponseTypeDef,
     DestinationFlowConfigOutputTypeDef,
     DestinationFlowConfigTypeDef,
+    SourceFlowConfigUnionTypeDef,
+    TriggerConfigUnionTypeDef,
     CreateConnectorProfileRequestRequestTypeDef,
     UpdateConnectorProfileRequestRequestTypeDef,
     DescribeFlowResponseTypeDef,
+    DestinationFlowConfigUnionTypeDef,
     CreateFlowRequestRequestTypeDef,
     UpdateFlowRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AggregationConfigTypeDef:
+def get_value() -> AggregationConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow.egg-info/SOURCES.txt` & `mypy-boto3-appflow-1.28.16/mypy_boto3_appflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.15.post2/setup.py` & `mypy-boto3-appflow-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appflow",
-    version="1.28.15.post2",
+    version="1.28.16",
     packages=["mypy_boto3_appflow"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Appflow 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Appflow 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 appflow type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 appflow type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_appflow": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

