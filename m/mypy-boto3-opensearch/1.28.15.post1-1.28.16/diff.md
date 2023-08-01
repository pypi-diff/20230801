# Comparing `tmp/mypy-boto3-opensearch-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-opensearch-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-opensearch-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:47 2023, max compression
+gzip compressed data, was "mypy-boto3-opensearch-1.28.16.tar", last modified: Tue Aug  1 11:37:27 2023, max compression
```

## Comparing `mypy-boto3-opensearch-1.28.15.post1.tar` & `mypy-boto3-opensearch-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:47.785315 mypy-boto3-opensearch-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:52:28.000000 mypy-boto3-opensearch-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20816 2023-07-29 10:03:47.777315 mypy-boto3-opensearch-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19304 2023-07-29 09:52:28.000000 mypy-boto3-opensearch-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:47.773315 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-29 09:52:28.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-29 09:52:28.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-29 09:52:28.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41172 2023-07-29 09:52:28.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-07-29 09:52:28.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-07-29 09:52:29.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-07-29 09:52:29.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:52:28.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    68707 2023-07-29 09:52:31.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    68650 2023-07-29 09:52:30.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:52:28.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:47.777315 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20816 2023-07-29 10:03:47.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-29 10:03:47.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:47.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:47.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:47.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:03:47.000000 mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:47.785315 mypy-boto3-opensearch-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-29 09:52:28.000000 mypy-boto3-opensearch-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:27.584804 mypy-boto3-opensearch-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:25:26.000000 mypy-boto3-opensearch-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20861 2023-08-01 11:37:27.584804 mypy-boto3-opensearch-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19358 2023-08-01 11:25:26.000000 mypy-boto3-opensearch-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:27.580803 mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-01 11:25:26.000000 mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-01 11:25:26.000000 mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-01 11:25:26.000000 mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41094 2023-08-01 11:25:29.000000 mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41033 2023-08-01 11:25:29.000000 mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-08-01 11:25:30.000000 mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-08-01 11:25:29.000000 mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:25:26.000000 mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    68895 2023-08-01 11:25:31.000000 mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68838 2023-08-01 11:25:31.000000 mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:25:26.000000 mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:27.584804 mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20861 2023-08-01 11:37:27.000000 mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-01 11:37:27.000000 mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:27.000000 mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:27.000000 mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:27.000000 mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 11:37:27.000000 mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:27.584804 mypy-boto3-opensearch-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-01 11:25:26.000000 mypy-boto3-opensearch-1.28.16/setup.py
```

### Comparing `mypy-boto3-opensearch-1.28.15.post1/LICENSE` & `mypy-boto3-opensearch-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.28.15.post1/PKG-INFO` & `mypy-boto3-opensearch-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opensearch
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.OpenSearchService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.OpenSearchService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 opensearch type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 opensearch type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opensearch)](https://pepy.tech/project/mypy-boto3-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
+[boto3.OpenSearchService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
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
 [mypy-boto3-opensearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/).
 
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
@@ -329,20 +329,20 @@
 )
 
 
 def check_value(value: ActionSeverityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_opensearch.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_opensearch.type_defs import (
     AWSDomainInformationTypeDef,
     AcceptInboundConnectionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     OptionStatusTypeDef,
@@ -350,14 +350,15 @@
     AdditionalLimitTypeDef,
     MasterUserOptionsTypeDef,
     AssociatePackageRequestRequestTypeDef,
     AuthorizeVpcEndpointAccessRequestRequestTypeDef,
     AuthorizedPrincipalTypeDef,
     ScheduledAutoTuneDetailsTypeDef,
     DurationTypeDef,
+    TimestampTypeDef,
     AutoTuneOptionsOutputTypeDef,
     AutoTuneStatusTypeDef,
     AvailabilityZoneInfoTypeDef,
     CancelServiceSoftwareUpdateRequestRequestTypeDef,
     ServiceSoftwareOptionsTypeDef,
     ChangeProgressDetailsTypeDef,
     ChangeProgressStageTypeDef,
@@ -526,14 +527,15 @@
     GetUpgradeHistoryResponseTypeDef,
     AcceptInboundConnectionResponseTypeDef,
     DeleteInboundConnectionResponseTypeDef,
     DescribeInboundConnectionsResponseTypeDef,
     RejectInboundConnectionResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     AutoTuneOptionsStatusTypeDef,
+    AutoTuneOptionsUnionTypeDef,
     DeleteOutboundConnectionResponseTypeDef,
     DescribeOutboundConnectionsResponseTypeDef,
     OffPeakWindowOptionsStatusTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateDomainConfigRequestRequestTypeDef,
     AdvancedSecurityOptionsStatusTypeDef,
     DomainStatusTypeDef,
@@ -545,15 +547,15 @@
     DescribeDomainsResponseTypeDef,
     DescribeDryRunProgressResponseTypeDef,
     DescribeDomainConfigResponseTypeDef,
     UpdateDomainConfigResponseTypeDef,
 )
 
 
-def get_structure() -> AWSDomainInformationTypeDef:
+def get_value() -> AWSDomainInformationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-opensearch-1.28.15.post1/README.md` & `mypy-boto3-opensearch-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opensearch)](https://pepy.tech/project/mypy-boto3-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
+[boto3.OpenSearchService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
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
 [mypy-boto3-opensearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/).
 
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
@@ -297,20 +297,20 @@
 )
 
 
 def check_value(value: ActionSeverityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_opensearch.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_opensearch.type_defs import (
     AWSDomainInformationTypeDef,
     AcceptInboundConnectionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     OptionStatusTypeDef,
@@ -318,14 +318,15 @@
     AdditionalLimitTypeDef,
     MasterUserOptionsTypeDef,
     AssociatePackageRequestRequestTypeDef,
     AuthorizeVpcEndpointAccessRequestRequestTypeDef,
     AuthorizedPrincipalTypeDef,
     ScheduledAutoTuneDetailsTypeDef,
     DurationTypeDef,
+    TimestampTypeDef,
     AutoTuneOptionsOutputTypeDef,
     AutoTuneStatusTypeDef,
     AvailabilityZoneInfoTypeDef,
     CancelServiceSoftwareUpdateRequestRequestTypeDef,
     ServiceSoftwareOptionsTypeDef,
     ChangeProgressDetailsTypeDef,
     ChangeProgressStageTypeDef,
@@ -494,14 +495,15 @@
     GetUpgradeHistoryResponseTypeDef,
     AcceptInboundConnectionResponseTypeDef,
     DeleteInboundConnectionResponseTypeDef,
     DescribeInboundConnectionsResponseTypeDef,
     RejectInboundConnectionResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     AutoTuneOptionsStatusTypeDef,
+    AutoTuneOptionsUnionTypeDef,
     DeleteOutboundConnectionResponseTypeDef,
     DescribeOutboundConnectionsResponseTypeDef,
     OffPeakWindowOptionsStatusTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateDomainConfigRequestRequestTypeDef,
     AdvancedSecurityOptionsStatusTypeDef,
     DomainStatusTypeDef,
@@ -513,15 +515,15 @@
     DescribeDomainsResponseTypeDef,
     DescribeDryRunProgressResponseTypeDef,
     DescribeDomainConfigResponseTypeDef,
     UpdateDomainConfigResponseTypeDef,
 )
 
 
-def get_structure() -> AWSDomainInformationTypeDef:
+def get_value() -> AWSDomainInformationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/__main__.py` & `mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpenSearchService 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.OpenSearchService 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService\nOther"
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

### Comparing `mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/client.py` & `mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_opensearch.client import OpenSearchServiceClient
 
     session = Session()
     client: OpenSearchServiceClient = session.client("opensearch")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ActionTypeType,
     ConnectionModeType,
     DryRunModeType,
@@ -28,17 +28,16 @@
     ScheduleAtType,
 )
 from .type_defs import (
     AcceptInboundConnectionResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AssociatePackageResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
-    AutoTuneOptionsExtraOutputTypeDef,
     AutoTuneOptionsInputTypeDef,
-    AutoTuneOptionsTypeDef,
+    AutoTuneOptionsUnionTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     ClusterConfigTypeDef,
     CognitoOptionsTypeDef,
     ConnectionPropertiesTypeDef,
     CreateDomainResponseTypeDef,
     CreateOutboundConnectionResponseTypeDef,
     CreatePackageResponseTypeDef,
@@ -736,15 +735,15 @@
         AdvancedOptions: Mapping[str, str] = ...,
         AccessPolicies: str = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
-        AutoTuneOptions: Union[AutoTuneOptionsTypeDef, AutoTuneOptionsExtraOutputTypeDef] = ...,
+        AutoTuneOptions: AutoTuneOptionsUnionTypeDef = ...,
         DryRun: bool = ...,
         DryRunMode: DryRunModeType = ...,
         OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,
         SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...
     ) -> UpdateDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Amazon OpenSearch Service
```

### Comparing `mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/client.pyi` & `mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_opensearch.client import OpenSearchServiceClient
 
     session = Session()
     client: OpenSearchServiceClient = session.client("opensearch")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ActionTypeType,
     ConnectionModeType,
     DryRunModeType,
@@ -28,17 +28,16 @@
     ScheduleAtType,
 )
 from .type_defs import (
     AcceptInboundConnectionResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AssociatePackageResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
-    AutoTuneOptionsExtraOutputTypeDef,
     AutoTuneOptionsInputTypeDef,
-    AutoTuneOptionsTypeDef,
+    AutoTuneOptionsUnionTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     ClusterConfigTypeDef,
     CognitoOptionsTypeDef,
     ConnectionPropertiesTypeDef,
     CreateDomainResponseTypeDef,
     CreateOutboundConnectionResponseTypeDef,
     CreatePackageResponseTypeDef,
@@ -679,15 +678,15 @@
         AdvancedOptions: Mapping[str, str] = ...,
         AccessPolicies: str = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
-        AutoTuneOptions: Union[AutoTuneOptionsTypeDef, AutoTuneOptionsExtraOutputTypeDef] = ...,
+        AutoTuneOptions: AutoTuneOptionsUnionTypeDef = ...,
         DryRun: bool = ...,
         DryRunMode: DryRunModeType = ...,
         OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,
         SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...
     ) -> UpdateDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Amazon OpenSearch Service
```

### Comparing `mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/literals.py` & `mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/literals.pyi` & `mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/type_defs.py` & `mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_opensearch.type_defs import AWSDomainInformationTypeDef
 
-    data: AWSDomainInformationTypeDef = {...}
+    data: AWSDomainInformationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -76,14 +76,15 @@
     "AdditionalLimitTypeDef",
     "MasterUserOptionsTypeDef",
     "AssociatePackageRequestRequestTypeDef",
     "AuthorizeVpcEndpointAccessRequestRequestTypeDef",
     "AuthorizedPrincipalTypeDef",
     "ScheduledAutoTuneDetailsTypeDef",
     "DurationTypeDef",
+    "TimestampTypeDef",
     "AutoTuneOptionsOutputTypeDef",
     "AutoTuneStatusTypeDef",
     "AvailabilityZoneInfoTypeDef",
     "CancelServiceSoftwareUpdateRequestRequestTypeDef",
     "ServiceSoftwareOptionsTypeDef",
     "ChangeProgressDetailsTypeDef",
     "ChangeProgressStageTypeDef",
@@ -252,14 +253,15 @@
     "GetUpgradeHistoryResponseTypeDef",
     "AcceptInboundConnectionResponseTypeDef",
     "DeleteInboundConnectionResponseTypeDef",
     "DescribeInboundConnectionsResponseTypeDef",
     "RejectInboundConnectionResponseTypeDef",
     "DescribeDomainAutoTunesResponseTypeDef",
     "AutoTuneOptionsStatusTypeDef",
+    "AutoTuneOptionsUnionTypeDef",
     "DeleteOutboundConnectionResponseTypeDef",
     "DescribeOutboundConnectionsResponseTypeDef",
     "OffPeakWindowOptionsStatusTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateDomainConfigRequestRequestTypeDef",
     "AdvancedSecurityOptionsStatusTypeDef",
     "DomainStatusTypeDef",
@@ -404,14 +406,15 @@
     {
         "Value": int,
         "Unit": Literal["HOURS"],
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 AutoTuneOptionsOutputTypeDef = TypedDict(
     "AutoTuneOptionsOutputTypeDef",
     {
         "State": AutoTuneStateType,
         "ErrorMessage": str,
         "UseOffPeakWindow": bool,
     },
@@ -1508,15 +1511,15 @@
     },
     total=False,
 )
 
 AutoTuneMaintenanceScheduleTypeDef = TypedDict(
     "AutoTuneMaintenanceScheduleTypeDef",
     {
-        "StartAt": Union[datetime, str],
+        "StartAt": TimestampTypeDef,
         "Duration": DurationTypeDef,
         "CronExpressionForRecurrence": str,
     },
     total=False,
 )
 
 EnvironmentInfoTypeDef = TypedDict(
@@ -2383,14 +2386,15 @@
     {
         "Options": AutoTuneOptionsExtraOutputTypeDef,
         "Status": AutoTuneStatusTypeDef,
     },
     total=False,
 )
 
+AutoTuneOptionsUnionTypeDef = Union[AutoTuneOptionsTypeDef, AutoTuneOptionsExtraOutputTypeDef]
 DeleteOutboundConnectionResponseTypeDef = TypedDict(
     "DeleteOutboundConnectionResponseTypeDef",
     {
         "Connection": OutboundConnectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch/type_defs.pyi` & `mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_opensearch.type_defs import AWSDomainInformationTypeDef
 
-    data: AWSDomainInformationTypeDef = {...}
+    data: AWSDomainInformationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -75,14 +75,15 @@
     "AdditionalLimitTypeDef",
     "MasterUserOptionsTypeDef",
     "AssociatePackageRequestRequestTypeDef",
     "AuthorizeVpcEndpointAccessRequestRequestTypeDef",
     "AuthorizedPrincipalTypeDef",
     "ScheduledAutoTuneDetailsTypeDef",
     "DurationTypeDef",
+    "TimestampTypeDef",
     "AutoTuneOptionsOutputTypeDef",
     "AutoTuneStatusTypeDef",
     "AvailabilityZoneInfoTypeDef",
     "CancelServiceSoftwareUpdateRequestRequestTypeDef",
     "ServiceSoftwareOptionsTypeDef",
     "ChangeProgressDetailsTypeDef",
     "ChangeProgressStageTypeDef",
@@ -251,14 +252,15 @@
     "GetUpgradeHistoryResponseTypeDef",
     "AcceptInboundConnectionResponseTypeDef",
     "DeleteInboundConnectionResponseTypeDef",
     "DescribeInboundConnectionsResponseTypeDef",
     "RejectInboundConnectionResponseTypeDef",
     "DescribeDomainAutoTunesResponseTypeDef",
     "AutoTuneOptionsStatusTypeDef",
+    "AutoTuneOptionsUnionTypeDef",
     "DeleteOutboundConnectionResponseTypeDef",
     "DescribeOutboundConnectionsResponseTypeDef",
     "OffPeakWindowOptionsStatusTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateDomainConfigRequestRequestTypeDef",
     "AdvancedSecurityOptionsStatusTypeDef",
     "DomainStatusTypeDef",
@@ -399,14 +401,15 @@
     {
         "Value": int,
         "Unit": Literal["HOURS"],
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 AutoTuneOptionsOutputTypeDef = TypedDict(
     "AutoTuneOptionsOutputTypeDef",
     {
         "State": AutoTuneStateType,
         "ErrorMessage": str,
         "UseOffPeakWindow": bool,
     },
@@ -1467,15 +1470,15 @@
     },
     total=False,
 )
 
 AutoTuneMaintenanceScheduleTypeDef = TypedDict(
     "AutoTuneMaintenanceScheduleTypeDef",
     {
-        "StartAt": Union[datetime, str],
+        "StartAt": TimestampTypeDef,
         "Duration": DurationTypeDef,
         "CronExpressionForRecurrence": str,
     },
     total=False,
 )
 
 EnvironmentInfoTypeDef = TypedDict(
@@ -2332,14 +2335,15 @@
     {
         "Options": AutoTuneOptionsExtraOutputTypeDef,
         "Status": AutoTuneStatusTypeDef,
     },
     total=False,
 )
 
+AutoTuneOptionsUnionTypeDef = Union[AutoTuneOptionsTypeDef, AutoTuneOptionsExtraOutputTypeDef]
 DeleteOutboundConnectionResponseTypeDef = TypedDict(
     "DeleteOutboundConnectionResponseTypeDef",
     {
         "Connection": OutboundConnectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch.egg-info/PKG-INFO` & `mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opensearch
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.OpenSearchService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.OpenSearchService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 opensearch type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 opensearch type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opensearch)](https://pepy.tech/project/mypy-boto3-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
+[boto3.OpenSearchService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
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
 [mypy-boto3-opensearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/).
 
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
@@ -329,20 +329,20 @@
 )
 
 
 def check_value(value: ActionSeverityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_opensearch.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_opensearch.type_defs import (
     AWSDomainInformationTypeDef,
     AcceptInboundConnectionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     OptionStatusTypeDef,
@@ -350,14 +350,15 @@
     AdditionalLimitTypeDef,
     MasterUserOptionsTypeDef,
     AssociatePackageRequestRequestTypeDef,
     AuthorizeVpcEndpointAccessRequestRequestTypeDef,
     AuthorizedPrincipalTypeDef,
     ScheduledAutoTuneDetailsTypeDef,
     DurationTypeDef,
+    TimestampTypeDef,
     AutoTuneOptionsOutputTypeDef,
     AutoTuneStatusTypeDef,
     AvailabilityZoneInfoTypeDef,
     CancelServiceSoftwareUpdateRequestRequestTypeDef,
     ServiceSoftwareOptionsTypeDef,
     ChangeProgressDetailsTypeDef,
     ChangeProgressStageTypeDef,
@@ -526,14 +527,15 @@
     GetUpgradeHistoryResponseTypeDef,
     AcceptInboundConnectionResponseTypeDef,
     DeleteInboundConnectionResponseTypeDef,
     DescribeInboundConnectionsResponseTypeDef,
     RejectInboundConnectionResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     AutoTuneOptionsStatusTypeDef,
+    AutoTuneOptionsUnionTypeDef,
     DeleteOutboundConnectionResponseTypeDef,
     DescribeOutboundConnectionsResponseTypeDef,
     OffPeakWindowOptionsStatusTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateDomainConfigRequestRequestTypeDef,
     AdvancedSecurityOptionsStatusTypeDef,
     DomainStatusTypeDef,
@@ -545,15 +547,15 @@
     DescribeDomainsResponseTypeDef,
     DescribeDryRunProgressResponseTypeDef,
     DescribeDomainConfigResponseTypeDef,
     UpdateDomainConfigResponseTypeDef,
 )
 
 
-def get_structure() -> AWSDomainInformationTypeDef:
+def get_value() -> AWSDomainInformationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-opensearch-1.28.15.post1/mypy_boto3_opensearch.egg-info/SOURCES.txt` & `mypy-boto3-opensearch-1.28.16/mypy_boto3_opensearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.28.15.post1/setup.py` & `mypy-boto3-opensearch-1.28.16/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-opensearch",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_opensearch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.OpenSearchService 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.OpenSearchService 1.28.16 service generated with"
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
-    keywords="boto3 opensearch type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 opensearch type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_opensearch": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

