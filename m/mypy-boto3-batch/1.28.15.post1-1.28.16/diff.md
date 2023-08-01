# Comparing `tmp/mypy-boto3-batch-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-batch-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-batch-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:37 2023, max compression
+gzip compressed data, was "mypy-boto3-batch-1.28.16.tar", last modified: Tue Aug  1 11:36:18 2023, max compression
```

## Comparing `mypy-boto3-batch-1.28.15.post1.tar` & `mypy-boto3-batch-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:37.201032 mypy-boto3-batch-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18366 2023-07-29 10:02:37.197032 mypy-boto3-batch-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:37.181032 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21074 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    51341 2023-07-29 09:39:04.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    51272 2023-07-29 09:39:03.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:37.197032 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18366 2023-07-29 10:02:36.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-29 10:02:36.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:36.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:36.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:36.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 10:02:36.000000 mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:37.201032 mypy-boto3-batch-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-29 09:39:02.000000 mypy-boto3-batch-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.516940 mypy-boto3-batch-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18553 2023-08-01 11:36:18.516940 mypy-boto3-batch-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17077 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.516940 mypy-boto3-batch-1.28.16/mypy_boto3_batch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20595 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20559 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-08-01 11:11:36.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-08-01 11:11:37.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52029 2023-08-01 11:11:36.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.516940 mypy-boto3-batch-1.28.16/mypy_boto3_batch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18553 2023-08-01 11:36:18.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-01 11:36:18.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:18.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:18.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:18.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 11:36:18.000000 mypy-boto3-batch-1.28.16/mypy_boto3_batch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:18.516940 mypy-boto3-batch-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-01 11:11:35.000000 mypy-boto3-batch-1.28.16/setup.py
```

### Comparing `mypy-boto3-batch-1.28.15.post1/LICENSE` & `mypy-boto3-batch-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.15.post1/PKG-INFO` & `mypy-boto3-batch-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-batch
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Batch 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Batch 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 batch type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 batch type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-batch)](https://pepy.tech/project/mypy-boto3-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Batch 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[boto3.Batch 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
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
 [mypy-boto3-batch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/).
 
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
@@ -351,20 +351,20 @@
 )
 
 
 def check_value(value: ArrayJobDependencyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_batch.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_batch.type_defs import (
     ArrayPropertiesDetailTypeDef,
     ArrayPropertiesSummaryTypeDef,
     ArrayPropertiesTypeDef,
     NetworkInterfaceTypeDef,
@@ -463,50 +463,56 @@
     ListJobsRequestRequestTypeDef,
     LinuxParametersOutputTypeDef,
     LinuxParametersTypeDef,
     ListSchedulingPoliciesResponseTypeDef,
     AttemptDetailTypeDef,
     DescribeJobQueuesResponseTypeDef,
     ComputeEnvironmentDetailTypeDef,
+    ComputeResourceUnionTypeDef,
     CreateComputeEnvironmentRequestRequestTypeDef,
     UpdateComputeEnvironmentRequestRequestTypeDef,
     NodePropertyOverrideTypeDef,
     VolumeTypeDef,
     EksPodPropertiesOverrideTypeDef,
     EksPodPropertiesDetailTypeDef,
     EksPodPropertiesOutputTypeDef,
     EksPodPropertiesTypeDef,
+    RetryStrategyUnionTypeDef,
     SchedulingPolicyDetailTypeDef,
     CreateSchedulingPolicyRequestRequestTypeDef,
+    FairsharePolicyUnionTypeDef,
     UpdateSchedulingPolicyRequestRequestTypeDef,
     ListJobsResponseTypeDef,
     DescribeComputeEnvironmentsResponseTypeDef,
     NodeOverridesTypeDef,
     ContainerDetailTypeDef,
     ContainerPropertiesOutputTypeDef,
     ContainerPropertiesTypeDef,
     EksPropertiesOverrideTypeDef,
     EksPropertiesDetailTypeDef,
     EksPropertiesOutputTypeDef,
     EksPropertiesTypeDef,
     DescribeSchedulingPoliciesResponseTypeDef,
     NodeRangePropertyOutputTypeDef,
+    ContainerPropertiesUnionTypeDef,
     NodeRangePropertyTypeDef,
     SubmitJobRequestRequestTypeDef,
+    EksPropertiesUnionTypeDef,
     NodePropertiesOutputTypeDef,
     NodePropertiesTypeDef,
     JobDefinitionTypeDef,
     JobDetailTypeDef,
+    NodePropertiesUnionTypeDef,
     RegisterJobDefinitionRequestRequestTypeDef,
     DescribeJobDefinitionsResponseTypeDef,
     DescribeJobsResponseTypeDef,
 )
 
 
-def get_structure() -> ArrayPropertiesDetailTypeDef:
+def get_value() -> ArrayPropertiesDetailTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-batch-1.28.15.post1/README.md` & `mypy-boto3-batch-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-batch)](https://pepy.tech/project/mypy-boto3-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Batch 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[boto3.Batch 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
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
 [mypy-boto3-batch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/).
 
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
@@ -319,20 +319,20 @@
 )
 
 
 def check_value(value: ArrayJobDependencyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_batch.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_batch.type_defs import (
     ArrayPropertiesDetailTypeDef,
     ArrayPropertiesSummaryTypeDef,
     ArrayPropertiesTypeDef,
     NetworkInterfaceTypeDef,
@@ -431,50 +431,56 @@
     ListJobsRequestRequestTypeDef,
     LinuxParametersOutputTypeDef,
     LinuxParametersTypeDef,
     ListSchedulingPoliciesResponseTypeDef,
     AttemptDetailTypeDef,
     DescribeJobQueuesResponseTypeDef,
     ComputeEnvironmentDetailTypeDef,
+    ComputeResourceUnionTypeDef,
     CreateComputeEnvironmentRequestRequestTypeDef,
     UpdateComputeEnvironmentRequestRequestTypeDef,
     NodePropertyOverrideTypeDef,
     VolumeTypeDef,
     EksPodPropertiesOverrideTypeDef,
     EksPodPropertiesDetailTypeDef,
     EksPodPropertiesOutputTypeDef,
     EksPodPropertiesTypeDef,
+    RetryStrategyUnionTypeDef,
     SchedulingPolicyDetailTypeDef,
     CreateSchedulingPolicyRequestRequestTypeDef,
+    FairsharePolicyUnionTypeDef,
     UpdateSchedulingPolicyRequestRequestTypeDef,
     ListJobsResponseTypeDef,
     DescribeComputeEnvironmentsResponseTypeDef,
     NodeOverridesTypeDef,
     ContainerDetailTypeDef,
     ContainerPropertiesOutputTypeDef,
     ContainerPropertiesTypeDef,
     EksPropertiesOverrideTypeDef,
     EksPropertiesDetailTypeDef,
     EksPropertiesOutputTypeDef,
     EksPropertiesTypeDef,
     DescribeSchedulingPoliciesResponseTypeDef,
     NodeRangePropertyOutputTypeDef,
+    ContainerPropertiesUnionTypeDef,
     NodeRangePropertyTypeDef,
     SubmitJobRequestRequestTypeDef,
+    EksPropertiesUnionTypeDef,
     NodePropertiesOutputTypeDef,
     NodePropertiesTypeDef,
     JobDefinitionTypeDef,
     JobDetailTypeDef,
+    NodePropertiesUnionTypeDef,
     RegisterJobDefinitionRequestRequestTypeDef,
     DescribeJobDefinitionsResponseTypeDef,
     DescribeJobsResponseTypeDef,
 )
 
 
-def get_structure() -> ArrayPropertiesDetailTypeDef:
+def get_value() -> ArrayPropertiesDetailTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/__init__.py` & `mypy-boto3-batch-1.28.16/mypy_boto3_batch/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/__init__.pyi` & `mypy-boto3-batch-1.28.16/mypy_boto3_batch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/__main__.py` & `mypy-boto3-batch-1.28.16/mypy_boto3_batch/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Batch 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.Batch 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch\nOther"
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

### Comparing `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/client.py` & `mypy-boto3-batch-1.28.16/mypy_boto3_batch/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_batch.client import BatchClient
 
     session = Session()
     client: BatchClient = session.client("batch")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CEStateType,
     CETypeType,
     JobDefinitionTypeType,
@@ -32,46 +32,40 @@
     DescribeJobQueuesPaginator,
     ListJobsPaginator,
     ListSchedulingPoliciesPaginator,
 )
 from .type_defs import (
     ArrayPropertiesTypeDef,
     ComputeEnvironmentOrderTypeDef,
-    ComputeResourceOutputTypeDef,
-    ComputeResourceTypeDef,
+    ComputeResourceUnionTypeDef,
     ComputeResourceUpdateTypeDef,
     ContainerOverridesTypeDef,
-    ContainerPropertiesOutputTypeDef,
-    ContainerPropertiesTypeDef,
+    ContainerPropertiesUnionTypeDef,
     CreateComputeEnvironmentResponseTypeDef,
     CreateJobQueueResponseTypeDef,
     CreateSchedulingPolicyResponseTypeDef,
     DescribeComputeEnvironmentsResponseTypeDef,
     DescribeJobDefinitionsResponseTypeDef,
     DescribeJobQueuesResponseTypeDef,
     DescribeJobsResponseTypeDef,
     DescribeSchedulingPoliciesResponseTypeDef,
     EksConfigurationTypeDef,
-    EksPropertiesOutputTypeDef,
     EksPropertiesOverrideTypeDef,
-    EksPropertiesTypeDef,
-    FairsharePolicyOutputTypeDef,
-    FairsharePolicyTypeDef,
+    EksPropertiesUnionTypeDef,
+    FairsharePolicyUnionTypeDef,
     JobDependencyTypeDef,
     JobTimeoutTypeDef,
     KeyValuesPairTypeDef,
     ListJobsResponseTypeDef,
     ListSchedulingPoliciesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NodeOverridesTypeDef,
-    NodePropertiesOutputTypeDef,
-    NodePropertiesTypeDef,
+    NodePropertiesUnionTypeDef,
     RegisterJobDefinitionResponseTypeDef,
-    RetryStrategyOutputTypeDef,
-    RetryStrategyTypeDef,
+    RetryStrategyUnionTypeDef,
     SubmitJobResponseTypeDef,
     UpdateComputeEnvironmentResponseTypeDef,
     UpdateJobQueueResponseTypeDef,
     UpdatePolicyTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -141,15 +135,15 @@
     def create_compute_environment(
         self,
         *,
         computeEnvironmentName: str,
         type: CETypeType,
         state: CEStateType = ...,
         unmanagedvCpus: int = ...,
-        computeResources: Union[ComputeResourceTypeDef, ComputeResourceOutputTypeDef] = ...,
+        computeResources: ComputeResourceUnionTypeDef = ...,
         serviceRole: str = ...,
         tags: Mapping[str, str] = ...,
         eksConfiguration: EksConfigurationTypeDef = ...
     ) -> CreateComputeEnvironmentResponseTypeDef:
         """
         Creates an Batch compute environment.
 
@@ -174,15 +168,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#create_job_queue)
         """
 
     def create_scheduling_policy(
         self,
         *,
         name: str,
-        fairsharePolicy: Union[FairsharePolicyTypeDef, FairsharePolicyOutputTypeDef] = ...,
+        fairsharePolicy: FairsharePolicyUnionTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateSchedulingPolicyResponseTypeDef:
         """
         Creates an Batch scheduling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_scheduling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#create_scheduling_policy)
@@ -331,24 +325,22 @@
     def register_job_definition(
         self,
         *,
         jobDefinitionName: str,
         type: JobDefinitionTypeType,
         parameters: Mapping[str, str] = ...,
         schedulingPriority: int = ...,
-        containerProperties: Union[
-            ContainerPropertiesTypeDef, ContainerPropertiesOutputTypeDef
-        ] = ...,
-        nodeProperties: Union[NodePropertiesTypeDef, NodePropertiesOutputTypeDef] = ...,
-        retryStrategy: Union[RetryStrategyTypeDef, RetryStrategyOutputTypeDef] = ...,
+        containerProperties: ContainerPropertiesUnionTypeDef = ...,
+        nodeProperties: NodePropertiesUnionTypeDef = ...,
+        retryStrategy: RetryStrategyUnionTypeDef = ...,
         propagateTags: bool = ...,
         timeout: JobTimeoutTypeDef = ...,
         tags: Mapping[str, str] = ...,
         platformCapabilities: Sequence[PlatformCapabilityType] = ...,
-        eksProperties: Union[EksPropertiesTypeDef, EksPropertiesOutputTypeDef] = ...
+        eksProperties: EksPropertiesUnionTypeDef = ...
     ) -> RegisterJobDefinitionResponseTypeDef:
         """
         Registers an Batch job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.register_job_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#register_job_definition)
         """
@@ -362,15 +354,15 @@
         shareIdentifier: str = ...,
         schedulingPriorityOverride: int = ...,
         arrayProperties: ArrayPropertiesTypeDef = ...,
         dependsOn: Sequence[JobDependencyTypeDef] = ...,
         parameters: Mapping[str, str] = ...,
         containerOverrides: ContainerOverridesTypeDef = ...,
         nodeOverrides: NodeOverridesTypeDef = ...,
-        retryStrategy: Union[RetryStrategyTypeDef, RetryStrategyOutputTypeDef] = ...,
+        retryStrategy: RetryStrategyUnionTypeDef = ...,
         propagateTags: bool = ...,
         timeout: JobTimeoutTypeDef = ...,
         tags: Mapping[str, str] = ...,
         eksPropertiesOverride: EksPropertiesOverrideTypeDef = ...
     ) -> SubmitJobResponseTypeDef:
         """
         Submits an Batch job from a job definition.
@@ -433,18 +425,15 @@
         Updates a job queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_job_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#update_job_queue)
         """
 
     def update_scheduling_policy(
-        self,
-        *,
-        arn: str,
-        fairsharePolicy: Union[FairsharePolicyTypeDef, FairsharePolicyOutputTypeDef] = ...
+        self, *, arn: str, fairsharePolicy: FairsharePolicyUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a scheduling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_scheduling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#update_scheduling_policy)
         """
```

### Comparing `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/client.pyi` & `mypy-boto3-batch-1.28.16/mypy_boto3_batch/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_batch.client import BatchClient
 
     session = Session()
     client: BatchClient = session.client("batch")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CEStateType,
     CETypeType,
     JobDefinitionTypeType,
@@ -32,46 +32,40 @@
     DescribeJobQueuesPaginator,
     ListJobsPaginator,
     ListSchedulingPoliciesPaginator,
 )
 from .type_defs import (
     ArrayPropertiesTypeDef,
     ComputeEnvironmentOrderTypeDef,
-    ComputeResourceOutputTypeDef,
-    ComputeResourceTypeDef,
+    ComputeResourceUnionTypeDef,
     ComputeResourceUpdateTypeDef,
     ContainerOverridesTypeDef,
-    ContainerPropertiesOutputTypeDef,
-    ContainerPropertiesTypeDef,
+    ContainerPropertiesUnionTypeDef,
     CreateComputeEnvironmentResponseTypeDef,
     CreateJobQueueResponseTypeDef,
     CreateSchedulingPolicyResponseTypeDef,
     DescribeComputeEnvironmentsResponseTypeDef,
     DescribeJobDefinitionsResponseTypeDef,
     DescribeJobQueuesResponseTypeDef,
     DescribeJobsResponseTypeDef,
     DescribeSchedulingPoliciesResponseTypeDef,
     EksConfigurationTypeDef,
-    EksPropertiesOutputTypeDef,
     EksPropertiesOverrideTypeDef,
-    EksPropertiesTypeDef,
-    FairsharePolicyOutputTypeDef,
-    FairsharePolicyTypeDef,
+    EksPropertiesUnionTypeDef,
+    FairsharePolicyUnionTypeDef,
     JobDependencyTypeDef,
     JobTimeoutTypeDef,
     KeyValuesPairTypeDef,
     ListJobsResponseTypeDef,
     ListSchedulingPoliciesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NodeOverridesTypeDef,
-    NodePropertiesOutputTypeDef,
-    NodePropertiesTypeDef,
+    NodePropertiesUnionTypeDef,
     RegisterJobDefinitionResponseTypeDef,
-    RetryStrategyOutputTypeDef,
-    RetryStrategyTypeDef,
+    RetryStrategyUnionTypeDef,
     SubmitJobResponseTypeDef,
     UpdateComputeEnvironmentResponseTypeDef,
     UpdateJobQueueResponseTypeDef,
     UpdatePolicyTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -133,15 +127,15 @@
     def create_compute_environment(
         self,
         *,
         computeEnvironmentName: str,
         type: CETypeType,
         state: CEStateType = ...,
         unmanagedvCpus: int = ...,
-        computeResources: Union[ComputeResourceTypeDef, ComputeResourceOutputTypeDef] = ...,
+        computeResources: ComputeResourceUnionTypeDef = ...,
         serviceRole: str = ...,
         tags: Mapping[str, str] = ...,
         eksConfiguration: EksConfigurationTypeDef = ...
     ) -> CreateComputeEnvironmentResponseTypeDef:
         """
         Creates an Batch compute environment.
 
@@ -164,15 +158,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_job_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#create_job_queue)
         """
     def create_scheduling_policy(
         self,
         *,
         name: str,
-        fairsharePolicy: Union[FairsharePolicyTypeDef, FairsharePolicyOutputTypeDef] = ...,
+        fairsharePolicy: FairsharePolicyUnionTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateSchedulingPolicyResponseTypeDef:
         """
         Creates an Batch scheduling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_scheduling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#create_scheduling_policy)
@@ -307,24 +301,22 @@
     def register_job_definition(
         self,
         *,
         jobDefinitionName: str,
         type: JobDefinitionTypeType,
         parameters: Mapping[str, str] = ...,
         schedulingPriority: int = ...,
-        containerProperties: Union[
-            ContainerPropertiesTypeDef, ContainerPropertiesOutputTypeDef
-        ] = ...,
-        nodeProperties: Union[NodePropertiesTypeDef, NodePropertiesOutputTypeDef] = ...,
-        retryStrategy: Union[RetryStrategyTypeDef, RetryStrategyOutputTypeDef] = ...,
+        containerProperties: ContainerPropertiesUnionTypeDef = ...,
+        nodeProperties: NodePropertiesUnionTypeDef = ...,
+        retryStrategy: RetryStrategyUnionTypeDef = ...,
         propagateTags: bool = ...,
         timeout: JobTimeoutTypeDef = ...,
         tags: Mapping[str, str] = ...,
         platformCapabilities: Sequence[PlatformCapabilityType] = ...,
-        eksProperties: Union[EksPropertiesTypeDef, EksPropertiesOutputTypeDef] = ...
+        eksProperties: EksPropertiesUnionTypeDef = ...
     ) -> RegisterJobDefinitionResponseTypeDef:
         """
         Registers an Batch job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.register_job_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#register_job_definition)
         """
@@ -337,15 +329,15 @@
         shareIdentifier: str = ...,
         schedulingPriorityOverride: int = ...,
         arrayProperties: ArrayPropertiesTypeDef = ...,
         dependsOn: Sequence[JobDependencyTypeDef] = ...,
         parameters: Mapping[str, str] = ...,
         containerOverrides: ContainerOverridesTypeDef = ...,
         nodeOverrides: NodeOverridesTypeDef = ...,
-        retryStrategy: Union[RetryStrategyTypeDef, RetryStrategyOutputTypeDef] = ...,
+        retryStrategy: RetryStrategyUnionTypeDef = ...,
         propagateTags: bool = ...,
         timeout: JobTimeoutTypeDef = ...,
         tags: Mapping[str, str] = ...,
         eksPropertiesOverride: EksPropertiesOverrideTypeDef = ...
     ) -> SubmitJobResponseTypeDef:
         """
         Submits an Batch job from a job definition.
@@ -402,18 +394,15 @@
         """
         Updates a job queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_job_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#update_job_queue)
         """
     def update_scheduling_policy(
-        self,
-        *,
-        arn: str,
-        fairsharePolicy: Union[FairsharePolicyTypeDef, FairsharePolicyOutputTypeDef] = ...
+        self, *, arn: str, fairsharePolicy: FairsharePolicyUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a scheduling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_scheduling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/client/#update_scheduling_policy)
         """
```

### Comparing `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/literals.py` & `mypy-boto3-batch-1.28.16/mypy_boto3_batch/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/literals.pyi` & `mypy-boto3-batch-1.28.16/mypy_boto3_batch/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/paginator.py` & `mypy-boto3-batch-1.28.16/mypy_boto3_batch/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/paginator.pyi` & `mypy-boto3-batch-1.28.16/mypy_boto3_batch/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/type_defs.py` & `mypy-boto3-batch-1.28.16/mypy_boto3_batch/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_batch.type_defs import ArrayPropertiesDetailTypeDef
 
-    data: ArrayPropertiesDetailTypeDef = {...}
+    data: ArrayPropertiesDetailTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ArrayJobDependencyType,
     AssignPublicIpType,
     CEStateType,
     CEStatusType,
     CETypeType,
@@ -143,43 +143,49 @@
     "ListJobsRequestRequestTypeDef",
     "LinuxParametersOutputTypeDef",
     "LinuxParametersTypeDef",
     "ListSchedulingPoliciesResponseTypeDef",
     "AttemptDetailTypeDef",
     "DescribeJobQueuesResponseTypeDef",
     "ComputeEnvironmentDetailTypeDef",
+    "ComputeResourceUnionTypeDef",
     "CreateComputeEnvironmentRequestRequestTypeDef",
     "UpdateComputeEnvironmentRequestRequestTypeDef",
     "NodePropertyOverrideTypeDef",
     "VolumeTypeDef",
     "EksPodPropertiesOverrideTypeDef",
     "EksPodPropertiesDetailTypeDef",
     "EksPodPropertiesOutputTypeDef",
     "EksPodPropertiesTypeDef",
+    "RetryStrategyUnionTypeDef",
     "SchedulingPolicyDetailTypeDef",
     "CreateSchedulingPolicyRequestRequestTypeDef",
+    "FairsharePolicyUnionTypeDef",
     "UpdateSchedulingPolicyRequestRequestTypeDef",
     "ListJobsResponseTypeDef",
     "DescribeComputeEnvironmentsResponseTypeDef",
     "NodeOverridesTypeDef",
     "ContainerDetailTypeDef",
     "ContainerPropertiesOutputTypeDef",
     "ContainerPropertiesTypeDef",
     "EksPropertiesOverrideTypeDef",
     "EksPropertiesDetailTypeDef",
     "EksPropertiesOutputTypeDef",
     "EksPropertiesTypeDef",
     "DescribeSchedulingPoliciesResponseTypeDef",
     "NodeRangePropertyOutputTypeDef",
+    "ContainerPropertiesUnionTypeDef",
     "NodeRangePropertyTypeDef",
     "SubmitJobRequestRequestTypeDef",
+    "EksPropertiesUnionTypeDef",
     "NodePropertiesOutputTypeDef",
     "NodePropertiesTypeDef",
     "JobDefinitionTypeDef",
     "JobDetailTypeDef",
+    "NodePropertiesUnionTypeDef",
     "RegisterJobDefinitionRequestRequestTypeDef",
     "DescribeJobDefinitionsResponseTypeDef",
     "DescribeJobsResponseTypeDef",
 )
 
 ArrayPropertiesDetailTypeDef = TypedDict(
     "ArrayPropertiesDetailTypeDef",
@@ -1480,14 +1486,15 @@
 
 class ComputeEnvironmentDetailTypeDef(
     _RequiredComputeEnvironmentDetailTypeDef, _OptionalComputeEnvironmentDetailTypeDef
 ):
     pass
 
 
+ComputeResourceUnionTypeDef = Union[ComputeResourceTypeDef, ComputeResourceOutputTypeDef]
 _RequiredCreateComputeEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateComputeEnvironmentRequestRequestTypeDef",
     {
         "computeEnvironmentName": str,
         "type": CETypeType,
     },
 )
@@ -1615,14 +1622,15 @@
         "containers": Sequence[EksContainerTypeDef],
         "volumes": Sequence[EksVolumeTypeDef],
         "metadata": EksMetadataTypeDef,
     },
     total=False,
 )
 
+RetryStrategyUnionTypeDef = Union[RetryStrategyTypeDef, RetryStrategyOutputTypeDef]
 _RequiredSchedulingPolicyDetailTypeDef = TypedDict(
     "_RequiredSchedulingPolicyDetailTypeDef",
     {
         "name": str,
         "arn": str,
     },
 )
@@ -1661,14 +1669,15 @@
 class CreateSchedulingPolicyRequestRequestTypeDef(
     _RequiredCreateSchedulingPolicyRequestRequestTypeDef,
     _OptionalCreateSchedulingPolicyRequestRequestTypeDef,
 ):
     pass
 
 
+FairsharePolicyUnionTypeDef = Union[FairsharePolicyTypeDef, FairsharePolicyOutputTypeDef]
 _RequiredUpdateSchedulingPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSchedulingPolicyRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateSchedulingPolicyRequestRequestTypeDef = TypedDict(
@@ -1864,14 +1873,17 @@
 
 class NodeRangePropertyOutputTypeDef(
     _RequiredNodeRangePropertyOutputTypeDef, _OptionalNodeRangePropertyOutputTypeDef
 ):
     pass
 
 
+ContainerPropertiesUnionTypeDef = Union[
+    ContainerPropertiesTypeDef, ContainerPropertiesOutputTypeDef
+]
 _RequiredNodeRangePropertyTypeDef = TypedDict(
     "_RequiredNodeRangePropertyTypeDef",
     {
         "targetNodes": str,
     },
 )
 _OptionalNodeRangePropertyTypeDef = TypedDict(
@@ -1919,14 +1931,15 @@
 
 class SubmitJobRequestRequestTypeDef(
     _RequiredSubmitJobRequestRequestTypeDef, _OptionalSubmitJobRequestRequestTypeDef
 ):
     pass
 
 
+EksPropertiesUnionTypeDef = Union[EksPropertiesTypeDef, EksPropertiesOutputTypeDef]
 NodePropertiesOutputTypeDef = TypedDict(
     "NodePropertiesOutputTypeDef",
     {
         "numNodes": int,
         "mainNode": int,
         "nodeRangeProperties": List[NodeRangePropertyOutputTypeDef],
     },
@@ -2015,14 +2028,15 @@
 )
 
 
 class JobDetailTypeDef(_RequiredJobDetailTypeDef, _OptionalJobDetailTypeDef):
     pass
 
 
+NodePropertiesUnionTypeDef = Union[NodePropertiesTypeDef, NodePropertiesOutputTypeDef]
 _RequiredRegisterJobDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterJobDefinitionRequestRequestTypeDef",
     {
         "jobDefinitionName": str,
         "type": JobDefinitionTypeType,
     },
 )
```

### Comparing `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch/type_defs.pyi` & `mypy-boto3-batch-1.28.16/mypy_boto3_batch/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_batch.type_defs import ArrayPropertiesDetailTypeDef
 
-    data: ArrayPropertiesDetailTypeDef = {...}
+    data: ArrayPropertiesDetailTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ArrayJobDependencyType,
     AssignPublicIpType,
     CEStateType,
     CEStatusType,
     CETypeType,
@@ -142,43 +142,49 @@
     "ListJobsRequestRequestTypeDef",
     "LinuxParametersOutputTypeDef",
     "LinuxParametersTypeDef",
     "ListSchedulingPoliciesResponseTypeDef",
     "AttemptDetailTypeDef",
     "DescribeJobQueuesResponseTypeDef",
     "ComputeEnvironmentDetailTypeDef",
+    "ComputeResourceUnionTypeDef",
     "CreateComputeEnvironmentRequestRequestTypeDef",
     "UpdateComputeEnvironmentRequestRequestTypeDef",
     "NodePropertyOverrideTypeDef",
     "VolumeTypeDef",
     "EksPodPropertiesOverrideTypeDef",
     "EksPodPropertiesDetailTypeDef",
     "EksPodPropertiesOutputTypeDef",
     "EksPodPropertiesTypeDef",
+    "RetryStrategyUnionTypeDef",
     "SchedulingPolicyDetailTypeDef",
     "CreateSchedulingPolicyRequestRequestTypeDef",
+    "FairsharePolicyUnionTypeDef",
     "UpdateSchedulingPolicyRequestRequestTypeDef",
     "ListJobsResponseTypeDef",
     "DescribeComputeEnvironmentsResponseTypeDef",
     "NodeOverridesTypeDef",
     "ContainerDetailTypeDef",
     "ContainerPropertiesOutputTypeDef",
     "ContainerPropertiesTypeDef",
     "EksPropertiesOverrideTypeDef",
     "EksPropertiesDetailTypeDef",
     "EksPropertiesOutputTypeDef",
     "EksPropertiesTypeDef",
     "DescribeSchedulingPoliciesResponseTypeDef",
     "NodeRangePropertyOutputTypeDef",
+    "ContainerPropertiesUnionTypeDef",
     "NodeRangePropertyTypeDef",
     "SubmitJobRequestRequestTypeDef",
+    "EksPropertiesUnionTypeDef",
     "NodePropertiesOutputTypeDef",
     "NodePropertiesTypeDef",
     "JobDefinitionTypeDef",
     "JobDetailTypeDef",
+    "NodePropertiesUnionTypeDef",
     "RegisterJobDefinitionRequestRequestTypeDef",
     "DescribeJobDefinitionsResponseTypeDef",
     "DescribeJobsResponseTypeDef",
 )
 
 ArrayPropertiesDetailTypeDef = TypedDict(
     "ArrayPropertiesDetailTypeDef",
@@ -1435,14 +1441,15 @@
 )
 
 class ComputeEnvironmentDetailTypeDef(
     _RequiredComputeEnvironmentDetailTypeDef, _OptionalComputeEnvironmentDetailTypeDef
 ):
     pass
 
+ComputeResourceUnionTypeDef = Union[ComputeResourceTypeDef, ComputeResourceOutputTypeDef]
 _RequiredCreateComputeEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateComputeEnvironmentRequestRequestTypeDef",
     {
         "computeEnvironmentName": str,
         "type": CETypeType,
     },
 )
@@ -1564,14 +1571,15 @@
         "containers": Sequence[EksContainerTypeDef],
         "volumes": Sequence[EksVolumeTypeDef],
         "metadata": EksMetadataTypeDef,
     },
     total=False,
 )
 
+RetryStrategyUnionTypeDef = Union[RetryStrategyTypeDef, RetryStrategyOutputTypeDef]
 _RequiredSchedulingPolicyDetailTypeDef = TypedDict(
     "_RequiredSchedulingPolicyDetailTypeDef",
     {
         "name": str,
         "arn": str,
     },
 )
@@ -1606,14 +1614,15 @@
 
 class CreateSchedulingPolicyRequestRequestTypeDef(
     _RequiredCreateSchedulingPolicyRequestRequestTypeDef,
     _OptionalCreateSchedulingPolicyRequestRequestTypeDef,
 ):
     pass
 
+FairsharePolicyUnionTypeDef = Union[FairsharePolicyTypeDef, FairsharePolicyOutputTypeDef]
 _RequiredUpdateSchedulingPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSchedulingPolicyRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateSchedulingPolicyRequestRequestTypeDef = TypedDict(
@@ -1805,14 +1814,17 @@
 )
 
 class NodeRangePropertyOutputTypeDef(
     _RequiredNodeRangePropertyOutputTypeDef, _OptionalNodeRangePropertyOutputTypeDef
 ):
     pass
 
+ContainerPropertiesUnionTypeDef = Union[
+    ContainerPropertiesTypeDef, ContainerPropertiesOutputTypeDef
+]
 _RequiredNodeRangePropertyTypeDef = TypedDict(
     "_RequiredNodeRangePropertyTypeDef",
     {
         "targetNodes": str,
     },
 )
 _OptionalNodeRangePropertyTypeDef = TypedDict(
@@ -1856,14 +1868,15 @@
 )
 
 class SubmitJobRequestRequestTypeDef(
     _RequiredSubmitJobRequestRequestTypeDef, _OptionalSubmitJobRequestRequestTypeDef
 ):
     pass
 
+EksPropertiesUnionTypeDef = Union[EksPropertiesTypeDef, EksPropertiesOutputTypeDef]
 NodePropertiesOutputTypeDef = TypedDict(
     "NodePropertiesOutputTypeDef",
     {
         "numNodes": int,
         "mainNode": int,
         "nodeRangeProperties": List[NodeRangePropertyOutputTypeDef],
     },
@@ -1948,14 +1961,15 @@
     },
     total=False,
 )
 
 class JobDetailTypeDef(_RequiredJobDetailTypeDef, _OptionalJobDetailTypeDef):
     pass
 
+NodePropertiesUnionTypeDef = Union[NodePropertiesTypeDef, NodePropertiesOutputTypeDef]
 _RequiredRegisterJobDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterJobDefinitionRequestRequestTypeDef",
     {
         "jobDefinitionName": str,
         "type": JobDefinitionTypeType,
     },
 )
```

### Comparing `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch.egg-info/PKG-INFO` & `mypy-boto3-batch-1.28.16/mypy_boto3_batch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-batch
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Batch 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Batch 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 batch type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 batch type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-batch)](https://pepy.tech/project/mypy-boto3-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Batch 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[boto3.Batch 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
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
 [mypy-boto3-batch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/).
 
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
@@ -351,20 +351,20 @@
 )
 
 
 def check_value(value: ArrayJobDependencyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_batch.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_batch.type_defs import (
     ArrayPropertiesDetailTypeDef,
     ArrayPropertiesSummaryTypeDef,
     ArrayPropertiesTypeDef,
     NetworkInterfaceTypeDef,
@@ -463,50 +463,56 @@
     ListJobsRequestRequestTypeDef,
     LinuxParametersOutputTypeDef,
     LinuxParametersTypeDef,
     ListSchedulingPoliciesResponseTypeDef,
     AttemptDetailTypeDef,
     DescribeJobQueuesResponseTypeDef,
     ComputeEnvironmentDetailTypeDef,
+    ComputeResourceUnionTypeDef,
     CreateComputeEnvironmentRequestRequestTypeDef,
     UpdateComputeEnvironmentRequestRequestTypeDef,
     NodePropertyOverrideTypeDef,
     VolumeTypeDef,
     EksPodPropertiesOverrideTypeDef,
     EksPodPropertiesDetailTypeDef,
     EksPodPropertiesOutputTypeDef,
     EksPodPropertiesTypeDef,
+    RetryStrategyUnionTypeDef,
     SchedulingPolicyDetailTypeDef,
     CreateSchedulingPolicyRequestRequestTypeDef,
+    FairsharePolicyUnionTypeDef,
     UpdateSchedulingPolicyRequestRequestTypeDef,
     ListJobsResponseTypeDef,
     DescribeComputeEnvironmentsResponseTypeDef,
     NodeOverridesTypeDef,
     ContainerDetailTypeDef,
     ContainerPropertiesOutputTypeDef,
     ContainerPropertiesTypeDef,
     EksPropertiesOverrideTypeDef,
     EksPropertiesDetailTypeDef,
     EksPropertiesOutputTypeDef,
     EksPropertiesTypeDef,
     DescribeSchedulingPoliciesResponseTypeDef,
     NodeRangePropertyOutputTypeDef,
+    ContainerPropertiesUnionTypeDef,
     NodeRangePropertyTypeDef,
     SubmitJobRequestRequestTypeDef,
+    EksPropertiesUnionTypeDef,
     NodePropertiesOutputTypeDef,
     NodePropertiesTypeDef,
     JobDefinitionTypeDef,
     JobDetailTypeDef,
+    NodePropertiesUnionTypeDef,
     RegisterJobDefinitionRequestRequestTypeDef,
     DescribeJobDefinitionsResponseTypeDef,
     DescribeJobsResponseTypeDef,
 )
 
 
-def get_structure() -> ArrayPropertiesDetailTypeDef:
+def get_value() -> ArrayPropertiesDetailTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-batch-1.28.15.post1/mypy_boto3_batch.egg-info/SOURCES.txt` & `mypy-boto3-batch-1.28.16/mypy_boto3_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.28.15.post1/setup.py` & `mypy-boto3-batch-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-batch",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_batch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Batch 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.Batch 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 batch type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 batch type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_batch": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

