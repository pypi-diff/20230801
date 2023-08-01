# Comparing `tmp/mypy-boto3-kafka-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-kafka-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kafka-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:24 2023, max compression
+gzip compressed data, was "mypy-boto3-kafka-1.28.16.tar", last modified: Tue Aug  1 11:37:05 2023, max compression
```

## Comparing `mypy-boto3-kafka-1.28.15.post1.tar` & `mypy-boto3-kafka-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:24.877205 mypy-boto3-kafka-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:28.000000 mypy-boto3-kafka-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-07-29 10:03:24.873205 mypy-boto3-kafka-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19749 2023-07-29 09:48:28.000000 mypy-boto3-kafka-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:24.865205 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-29 09:48:28.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-29 09:48:28.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-29 09:48:28.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36834 2023-07-29 09:48:31.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36769 2023-07-29 09:48:29.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-07-29 09:48:31.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-07-29 09:48:31.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12582 2023-07-29 09:48:31.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-07-29 09:48:31.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:28.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60653 2023-07-29 09:48:33.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60576 2023-07-29 09:48:32.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:28.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:24.873205 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-07-29 10:03:24.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-29 10:03:24.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:24.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:24.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:24.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 10:03:24.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:24.877205 mypy-boto3-kafka-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-29 09:48:28.000000 mypy-boto3-kafka-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:05.692854 mypy-boto3-kafka-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:21:16.000000 mypy-boto3-kafka-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21316 2023-08-01 11:37:05.684854 mypy-boto3-kafka-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19840 2023-08-01 11:21:16.000000 mypy-boto3-kafka-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:05.676854 mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-08-01 11:21:16.000000 mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-08-01 11:21:16.000000 mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-01 11:21:16.000000 mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36483 2023-08-01 11:21:16.000000 mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36418 2023-08-01 11:21:16.000000 mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-08-01 11:21:17.000000 mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-08-01 11:21:17.000000 mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12582 2023-08-01 11:21:16.000000 mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-08-01 11:21:16.000000 mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:21:16.000000 mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60964 2023-08-01 11:21:18.000000 mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60887 2023-08-01 11:21:18.000000 mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:21:16.000000 mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:05.684854 mypy-boto3-kafka-1.28.16/mypy_boto3_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21316 2023-08-01 11:37:05.000000 mypy-boto3-kafka-1.28.16/mypy_boto3_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-01 11:37:05.000000 mypy-boto3-kafka-1.28.16/mypy_boto3_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:05.000000 mypy-boto3-kafka-1.28.16/mypy_boto3_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:05.000000 mypy-boto3-kafka-1.28.16/mypy_boto3_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:05.000000 mypy-boto3-kafka-1.28.16/mypy_boto3_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 11:37:05.000000 mypy-boto3-kafka-1.28.16/mypy_boto3_kafka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:05.692854 mypy-boto3-kafka-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-01 11:21:16.000000 mypy-boto3-kafka-1.28.16/setup.py
```

### Comparing `mypy-boto3-kafka-1.28.15.post1/LICENSE` & `mypy-boto3-kafka-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.15.post1/PKG-INFO` & `mypy-boto3-kafka-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kafka
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Kafka 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Kafka 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kafka type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 kafka type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kafka)](https://pepy.tech/project/mypy-boto3-kafka)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kafka 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
+[boto3.Kafka 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
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
 [mypy-boto3-kafka docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/).
 
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
@@ -366,27 +366,28 @@
 )
 
 
 def check_value(value: BrokerAZDistributionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kafka.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kafka.type_defs import (
     BatchAssociateScramSecretRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     UnprocessedScramSecretTypeDef,
     BatchDisassociateScramSecretRequestRequestTypeDef,
+    BlobTypeDef,
     ProvisionedThroughputTypeDef,
     CloudWatchLogsTypeDef,
     FirehoseTypeDef,
     S3TypeDef,
     BrokerSoftwareInfoTypeDef,
     TlsOutputTypeDef,
     UnauthenticatedTypeDef,
@@ -396,15 +397,14 @@
     ErrorInfoTypeDef,
     ClusterOperationStepInfoTypeDef,
     ClusterOperationV2SummaryTypeDef,
     CompatibleKafkaVersionTypeDef,
     ConfigurationInfoTypeDef,
     ConfigurationRevisionTypeDef,
     PublicAccessTypeDef,
-    CreateConfigurationRequestRequestTypeDef,
     CreateVpcConnectionRequestRequestTypeDef,
     DeleteClusterPolicyRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteConfigurationRequestRequestTypeDef,
     DeleteVpcConnectionRequestRequestTypeDef,
     DescribeClusterOperationRequestRequestTypeDef,
     DescribeClusterOperationV2RequestRequestTypeDef,
@@ -445,15 +445,14 @@
     ScramTypeDef,
     VpcConfigTypeDef,
     VpcConfigOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrokerCountRequestRequestTypeDef,
     UpdateBrokerTypeRequestRequestTypeDef,
-    UpdateConfigurationRequestRequestTypeDef,
     UserIdentityTypeDef,
     VpcConnectivityTlsTypeDef,
     VpcConnectivityIamTypeDef,
     VpcConnectivityScramTypeDef,
     CreateClusterResponseTypeDef,
     CreateClusterV2ResponseTypeDef,
     CreateVpcConnectionResponseTypeDef,
@@ -476,14 +475,16 @@
     UpdateClusterKafkaVersionResponseTypeDef,
     UpdateConnectivityResponseTypeDef,
     UpdateMonitoringResponseTypeDef,
     UpdateSecurityResponseTypeDef,
     UpdateStorageResponseTypeDef,
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
+    CreateConfigurationRequestRequestTypeDef,
+    UpdateConfigurationRequestRequestTypeDef,
     BrokerEBSVolumeInfoTypeDef,
     EBSStorageInfoTypeDef,
     UpdateStorageRequestRequestTypeDef,
     BrokerLogsTypeDef,
     BrokerNodeInfoTypeDef,
     ListClientVpcConnectionsResponseTypeDef,
     ClusterOperationStepTypeDef,
@@ -529,23 +530,25 @@
     ClientAuthenticationTypeDef,
     ClusterOperationV2ServerlessTypeDef,
     VpcConnectivityClientAuthenticationTypeDef,
     ListNodesResponseTypeDef,
     ServerlessRequestTypeDef,
     ServerlessTypeDef,
     UpdateMonitoringRequestRequestTypeDef,
+    ClientAuthenticationUnionTypeDef,
     UpdateSecurityRequestRequestTypeDef,
     VpcConnectivityTypeDef,
     ConnectivityInfoTypeDef,
     BrokerNodeGroupInfoOutputTypeDef,
     BrokerNodeGroupInfoTypeDef,
     MutableClusterInfoTypeDef,
     UpdateConnectivityRequestRequestTypeDef,
     ClusterInfoTypeDef,
     ProvisionedTypeDef,
+    BrokerNodeGroupInfoUnionTypeDef,
     CreateClusterRequestRequestTypeDef,
     ProvisionedRequestTypeDef,
     ClusterOperationInfoTypeDef,
     ClusterOperationV2ProvisionedTypeDef,
     DescribeClusterResponseTypeDef,
     ListClustersResponseTypeDef,
     ClusterTypeDef,
@@ -555,15 +558,15 @@
     ClusterOperationV2TypeDef,
     DescribeClusterV2ResponseTypeDef,
     ListClustersV2ResponseTypeDef,
     DescribeClusterOperationV2ResponseTypeDef,
 )
 
 
-def get_structure() -> BatchAssociateScramSecretRequestRequestTypeDef:
+def get_value() -> BatchAssociateScramSecretRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kafka-1.28.15.post1/README.md` & `mypy-boto3-kafka-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kafka)](https://pepy.tech/project/mypy-boto3-kafka)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kafka 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
+[boto3.Kafka 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
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
 [mypy-boto3-kafka docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/).
 
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
@@ -334,27 +334,28 @@
 )
 
 
 def check_value(value: BrokerAZDistributionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kafka.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kafka.type_defs import (
     BatchAssociateScramSecretRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     UnprocessedScramSecretTypeDef,
     BatchDisassociateScramSecretRequestRequestTypeDef,
+    BlobTypeDef,
     ProvisionedThroughputTypeDef,
     CloudWatchLogsTypeDef,
     FirehoseTypeDef,
     S3TypeDef,
     BrokerSoftwareInfoTypeDef,
     TlsOutputTypeDef,
     UnauthenticatedTypeDef,
@@ -364,15 +365,14 @@
     ErrorInfoTypeDef,
     ClusterOperationStepInfoTypeDef,
     ClusterOperationV2SummaryTypeDef,
     CompatibleKafkaVersionTypeDef,
     ConfigurationInfoTypeDef,
     ConfigurationRevisionTypeDef,
     PublicAccessTypeDef,
-    CreateConfigurationRequestRequestTypeDef,
     CreateVpcConnectionRequestRequestTypeDef,
     DeleteClusterPolicyRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteConfigurationRequestRequestTypeDef,
     DeleteVpcConnectionRequestRequestTypeDef,
     DescribeClusterOperationRequestRequestTypeDef,
     DescribeClusterOperationV2RequestRequestTypeDef,
@@ -413,15 +413,14 @@
     ScramTypeDef,
     VpcConfigTypeDef,
     VpcConfigOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrokerCountRequestRequestTypeDef,
     UpdateBrokerTypeRequestRequestTypeDef,
-    UpdateConfigurationRequestRequestTypeDef,
     UserIdentityTypeDef,
     VpcConnectivityTlsTypeDef,
     VpcConnectivityIamTypeDef,
     VpcConnectivityScramTypeDef,
     CreateClusterResponseTypeDef,
     CreateClusterV2ResponseTypeDef,
     CreateVpcConnectionResponseTypeDef,
@@ -444,14 +443,16 @@
     UpdateClusterKafkaVersionResponseTypeDef,
     UpdateConnectivityResponseTypeDef,
     UpdateMonitoringResponseTypeDef,
     UpdateSecurityResponseTypeDef,
     UpdateStorageResponseTypeDef,
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
+    CreateConfigurationRequestRequestTypeDef,
+    UpdateConfigurationRequestRequestTypeDef,
     BrokerEBSVolumeInfoTypeDef,
     EBSStorageInfoTypeDef,
     UpdateStorageRequestRequestTypeDef,
     BrokerLogsTypeDef,
     BrokerNodeInfoTypeDef,
     ListClientVpcConnectionsResponseTypeDef,
     ClusterOperationStepTypeDef,
@@ -497,23 +498,25 @@
     ClientAuthenticationTypeDef,
     ClusterOperationV2ServerlessTypeDef,
     VpcConnectivityClientAuthenticationTypeDef,
     ListNodesResponseTypeDef,
     ServerlessRequestTypeDef,
     ServerlessTypeDef,
     UpdateMonitoringRequestRequestTypeDef,
+    ClientAuthenticationUnionTypeDef,
     UpdateSecurityRequestRequestTypeDef,
     VpcConnectivityTypeDef,
     ConnectivityInfoTypeDef,
     BrokerNodeGroupInfoOutputTypeDef,
     BrokerNodeGroupInfoTypeDef,
     MutableClusterInfoTypeDef,
     UpdateConnectivityRequestRequestTypeDef,
     ClusterInfoTypeDef,
     ProvisionedTypeDef,
+    BrokerNodeGroupInfoUnionTypeDef,
     CreateClusterRequestRequestTypeDef,
     ProvisionedRequestTypeDef,
     ClusterOperationInfoTypeDef,
     ClusterOperationV2ProvisionedTypeDef,
     DescribeClusterResponseTypeDef,
     ListClustersResponseTypeDef,
     ClusterTypeDef,
@@ -523,15 +526,15 @@
     ClusterOperationV2TypeDef,
     DescribeClusterV2ResponseTypeDef,
     ListClustersV2ResponseTypeDef,
     DescribeClusterOperationV2ResponseTypeDef,
 )
 
 
-def get_structure() -> BatchAssociateScramSecretRequestRequestTypeDef:
+def get_value() -> BatchAssociateScramSecretRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/__init__.py` & `mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/__init__.pyi` & `mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/__main__.py` & `mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Kafka 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.Kafka 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka\nOther"
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

### Comparing `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/client.py` & `mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     from mypy_boto3_kafka.client import KafkaClient
 
     session = Session()
     client: KafkaClient = session.client("kafka")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import EnhancedMonitoringType, StorageModeType
 from .paginator import (
     ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
     ListClusterOperationsV2Paginator,
     ListClustersPaginator,
@@ -32,19 +31,18 @@
     ListNodesPaginator,
     ListScramSecretsPaginator,
     ListVpcConnectionsPaginator,
 )
 from .type_defs import (
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
+    BlobTypeDef,
     BrokerEBSVolumeInfoTypeDef,
-    BrokerNodeGroupInfoOutputTypeDef,
-    BrokerNodeGroupInfoTypeDef,
-    ClientAuthenticationOutputTypeDef,
-    ClientAuthenticationTypeDef,
+    BrokerNodeGroupInfoUnionTypeDef,
+    ClientAuthenticationUnionTypeDef,
     ConfigurationInfoTypeDef,
     ConnectivityInfoTypeDef,
     CreateClusterResponseTypeDef,
     CreateClusterV2ResponseTypeDef,
     CreateConfigurationResponseTypeDef,
     CreateVpcConnectionResponseTypeDef,
     DeleteClusterResponseTypeDef,
@@ -174,21 +172,19 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#close)
         """
 
     def create_cluster(
         self,
         *,
-        BrokerNodeGroupInfo: Union[BrokerNodeGroupInfoTypeDef, BrokerNodeGroupInfoOutputTypeDef],
+        BrokerNodeGroupInfo: BrokerNodeGroupInfoUnionTypeDef,
         ClusterName: str,
         KafkaVersion: str,
         NumberOfBrokerNodes: int,
-        ClientAuthentication: Union[
-            ClientAuthenticationTypeDef, ClientAuthenticationOutputTypeDef
-        ] = ...,
+        ClientAuthentication: ClientAuthenticationUnionTypeDef = ...,
         ConfigurationInfo: ConfigurationInfoTypeDef = ...,
         EncryptionInfo: EncryptionInfoTypeDef = ...,
         EnhancedMonitoring: EnhancedMonitoringType = ...,
         OpenMonitoring: OpenMonitoringInfoTypeDef = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         StorageMode: StorageModeType = ...
@@ -215,15 +211,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#create_cluster_v2)
         """
 
     def create_configuration(
         self,
         *,
         Name: str,
-        ServerProperties: Union[str, bytes, IO[Any], StreamingBody],
+        ServerProperties: BlobTypeDef,
         Description: str = ...,
         KafkaVersions: Sequence[str] = ...
     ) -> CreateConfigurationResponseTypeDef:
         """
         Creates a new MSK configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_configuration)
@@ -621,19 +617,15 @@
         Updates the Apache Kafka version for the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_cluster_kafka_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#update_cluster_kafka_version)
         """
 
     def update_configuration(
-        self,
-        *,
-        Arn: str,
-        ServerProperties: Union[str, bytes, IO[Any], StreamingBody],
-        Description: str = ...
+        self, *, Arn: str, ServerProperties: BlobTypeDef, Description: str = ...
     ) -> UpdateConfigurationResponseTypeDef:
         """
         Updates an MSK configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#update_configuration)
         """
@@ -665,17 +657,15 @@
         """
 
     def update_security(
         self,
         *,
         ClusterArn: str,
         CurrentVersion: str,
-        ClientAuthentication: Union[
-            ClientAuthenticationTypeDef, ClientAuthenticationOutputTypeDef
-        ] = ...,
+        ClientAuthentication: ClientAuthenticationUnionTypeDef = ...,
         EncryptionInfo: EncryptionInfoTypeDef = ...
     ) -> UpdateSecurityResponseTypeDef:
         """
         Updates the security settings for the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_security)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#update_security)
```

### Comparing `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/client.pyi` & `mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     from mypy_boto3_kafka.client import KafkaClient
 
     session = Session()
     client: KafkaClient = session.client("kafka")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import EnhancedMonitoringType, StorageModeType
 from .paginator import (
     ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
     ListClusterOperationsV2Paginator,
     ListClustersPaginator,
@@ -32,19 +31,18 @@
     ListNodesPaginator,
     ListScramSecretsPaginator,
     ListVpcConnectionsPaginator,
 )
 from .type_defs import (
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
+    BlobTypeDef,
     BrokerEBSVolumeInfoTypeDef,
-    BrokerNodeGroupInfoOutputTypeDef,
-    BrokerNodeGroupInfoTypeDef,
-    ClientAuthenticationOutputTypeDef,
-    ClientAuthenticationTypeDef,
+    BrokerNodeGroupInfoUnionTypeDef,
+    ClientAuthenticationUnionTypeDef,
     ConfigurationInfoTypeDef,
     ConnectivityInfoTypeDef,
     CreateClusterResponseTypeDef,
     CreateClusterV2ResponseTypeDef,
     CreateConfigurationResponseTypeDef,
     CreateVpcConnectionResponseTypeDef,
     DeleteClusterResponseTypeDef,
@@ -165,21 +163,19 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#close)
         """
     def create_cluster(
         self,
         *,
-        BrokerNodeGroupInfo: Union[BrokerNodeGroupInfoTypeDef, BrokerNodeGroupInfoOutputTypeDef],
+        BrokerNodeGroupInfo: BrokerNodeGroupInfoUnionTypeDef,
         ClusterName: str,
         KafkaVersion: str,
         NumberOfBrokerNodes: int,
-        ClientAuthentication: Union[
-            ClientAuthenticationTypeDef, ClientAuthenticationOutputTypeDef
-        ] = ...,
+        ClientAuthentication: ClientAuthenticationUnionTypeDef = ...,
         ConfigurationInfo: ConfigurationInfoTypeDef = ...,
         EncryptionInfo: EncryptionInfoTypeDef = ...,
         EnhancedMonitoring: EnhancedMonitoringType = ...,
         OpenMonitoring: OpenMonitoringInfoTypeDef = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         StorageMode: StorageModeType = ...
@@ -204,15 +200,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_cluster_v2)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#create_cluster_v2)
         """
     def create_configuration(
         self,
         *,
         Name: str,
-        ServerProperties: Union[str, bytes, IO[Any], StreamingBody],
+        ServerProperties: BlobTypeDef,
         Description: str = ...,
         KafkaVersions: Sequence[str] = ...
     ) -> CreateConfigurationResponseTypeDef:
         """
         Creates a new MSK configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_configuration)
@@ -571,19 +567,15 @@
         """
         Updates the Apache Kafka version for the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_cluster_kafka_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#update_cluster_kafka_version)
         """
     def update_configuration(
-        self,
-        *,
-        Arn: str,
-        ServerProperties: Union[str, bytes, IO[Any], StreamingBody],
-        Description: str = ...
+        self, *, Arn: str, ServerProperties: BlobTypeDef, Description: str = ...
     ) -> UpdateConfigurationResponseTypeDef:
         """
         Updates an MSK configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#update_configuration)
         """
@@ -612,17 +604,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#update_monitoring)
         """
     def update_security(
         self,
         *,
         ClusterArn: str,
         CurrentVersion: str,
-        ClientAuthentication: Union[
-            ClientAuthenticationTypeDef, ClientAuthenticationOutputTypeDef
-        ] = ...,
+        ClientAuthentication: ClientAuthenticationUnionTypeDef = ...,
         EncryptionInfo: EncryptionInfoTypeDef = ...
     ) -> UpdateSecurityResponseTypeDef:
         """
         Updates the security settings for the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_security)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#update_security)
```

### Comparing `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/literals.py` & `mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/literals.pyi` & `mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/paginator.py` & `mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/paginator.pyi` & `mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/type_defs.py` & `mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_kafka.type_defs import BatchAssociateScramSecretRequestRequestTypeDef
 
-    data: BatchAssociateScramSecretRequestRequestTypeDef = {...}
+    data: BatchAssociateScramSecretRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -34,20 +34,20 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BatchAssociateScramSecretRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "UnprocessedScramSecretTypeDef",
     "BatchDisassociateScramSecretRequestRequestTypeDef",
+    "BlobTypeDef",
     "ProvisionedThroughputTypeDef",
     "CloudWatchLogsTypeDef",
     "FirehoseTypeDef",
     "S3TypeDef",
     "BrokerSoftwareInfoTypeDef",
     "TlsOutputTypeDef",
     "UnauthenticatedTypeDef",
@@ -57,15 +57,14 @@
     "ErrorInfoTypeDef",
     "ClusterOperationStepInfoTypeDef",
     "ClusterOperationV2SummaryTypeDef",
     "CompatibleKafkaVersionTypeDef",
     "ConfigurationInfoTypeDef",
     "ConfigurationRevisionTypeDef",
     "PublicAccessTypeDef",
-    "CreateConfigurationRequestRequestTypeDef",
     "CreateVpcConnectionRequestRequestTypeDef",
     "DeleteClusterPolicyRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteConfigurationRequestRequestTypeDef",
     "DeleteVpcConnectionRequestRequestTypeDef",
     "DescribeClusterOperationRequestRequestTypeDef",
     "DescribeClusterOperationV2RequestRequestTypeDef",
@@ -106,15 +105,14 @@
     "ScramTypeDef",
     "VpcConfigTypeDef",
     "VpcConfigOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrokerCountRequestRequestTypeDef",
     "UpdateBrokerTypeRequestRequestTypeDef",
-    "UpdateConfigurationRequestRequestTypeDef",
     "UserIdentityTypeDef",
     "VpcConnectivityTlsTypeDef",
     "VpcConnectivityIamTypeDef",
     "VpcConnectivityScramTypeDef",
     "CreateClusterResponseTypeDef",
     "CreateClusterV2ResponseTypeDef",
     "CreateVpcConnectionResponseTypeDef",
@@ -137,14 +135,16 @@
     "UpdateClusterKafkaVersionResponseTypeDef",
     "UpdateConnectivityResponseTypeDef",
     "UpdateMonitoringResponseTypeDef",
     "UpdateSecurityResponseTypeDef",
     "UpdateStorageResponseTypeDef",
     "BatchAssociateScramSecretResponseTypeDef",
     "BatchDisassociateScramSecretResponseTypeDef",
+    "CreateConfigurationRequestRequestTypeDef",
+    "UpdateConfigurationRequestRequestTypeDef",
     "BrokerEBSVolumeInfoTypeDef",
     "EBSStorageInfoTypeDef",
     "UpdateStorageRequestRequestTypeDef",
     "BrokerLogsTypeDef",
     "BrokerNodeInfoTypeDef",
     "ListClientVpcConnectionsResponseTypeDef",
     "ClusterOperationStepTypeDef",
@@ -190,23 +190,25 @@
     "ClientAuthenticationTypeDef",
     "ClusterOperationV2ServerlessTypeDef",
     "VpcConnectivityClientAuthenticationTypeDef",
     "ListNodesResponseTypeDef",
     "ServerlessRequestTypeDef",
     "ServerlessTypeDef",
     "UpdateMonitoringRequestRequestTypeDef",
+    "ClientAuthenticationUnionTypeDef",
     "UpdateSecurityRequestRequestTypeDef",
     "VpcConnectivityTypeDef",
     "ConnectivityInfoTypeDef",
     "BrokerNodeGroupInfoOutputTypeDef",
     "BrokerNodeGroupInfoTypeDef",
     "MutableClusterInfoTypeDef",
     "UpdateConnectivityRequestRequestTypeDef",
     "ClusterInfoTypeDef",
     "ProvisionedTypeDef",
+    "BrokerNodeGroupInfoUnionTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "ProvisionedRequestTypeDef",
     "ClusterOperationInfoTypeDef",
     "ClusterOperationV2ProvisionedTypeDef",
     "DescribeClusterResponseTypeDef",
     "ListClustersResponseTypeDef",
     "ClusterTypeDef",
@@ -252,14 +254,15 @@
     "BatchDisassociateScramSecretRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "SecretArnList": Sequence[str],
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ProvisionedThroughputTypeDef = TypedDict(
     "ProvisionedThroughputTypeDef",
     {
         "Enabled": bool,
         "VolumeThroughput": int,
     },
     total=False,
@@ -275,38 +278,34 @@
     "_OptionalCloudWatchLogsTypeDef",
     {
         "LogGroup": str,
     },
     total=False,
 )
 
-
 class CloudWatchLogsTypeDef(_RequiredCloudWatchLogsTypeDef, _OptionalCloudWatchLogsTypeDef):
     pass
 
-
 _RequiredFirehoseTypeDef = TypedDict(
     "_RequiredFirehoseTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalFirehoseTypeDef = TypedDict(
     "_OptionalFirehoseTypeDef",
     {
         "DeliveryStream": str,
     },
     total=False,
 )
 
-
 class FirehoseTypeDef(_RequiredFirehoseTypeDef, _OptionalFirehoseTypeDef):
     pass
 
-
 _RequiredS3TypeDef = TypedDict(
     "_RequiredS3TypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalS3TypeDef = TypedDict(
@@ -314,19 +313,17 @@
     {
         "Bucket": str,
         "Prefix": str,
     },
     total=False,
 )
 
-
 class S3TypeDef(_RequiredS3TypeDef, _OptionalS3TypeDef):
     pass
 
-
 BrokerSoftwareInfoTypeDef = TypedDict(
     "BrokerSoftwareInfoTypeDef",
     {
         "ConfigurationArn": str,
         "ConfigurationRevision": int,
         "KafkaVersion": str,
     },
@@ -372,21 +369,19 @@
         "CreationTime": datetime,
         "State": VpcConnectionStateType,
         "Owner": str,
     },
     total=False,
 )
 
-
 class ClientVpcConnectionTypeDef(
     _RequiredClientVpcConnectionTypeDef, _OptionalClientVpcConnectionTypeDef
 ):
     pass
 
-
 StateInfoTypeDef = TypedDict(
     "StateInfoTypeDef",
     {
         "Code": str,
         "Message": str,
     },
     total=False,
@@ -451,53 +446,27 @@
     "_OptionalConfigurationRevisionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class ConfigurationRevisionTypeDef(
     _RequiredConfigurationRevisionTypeDef, _OptionalConfigurationRevisionTypeDef
 ):
     pass
 
-
 PublicAccessTypeDef = TypedDict(
     "PublicAccessTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-_RequiredCreateConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateConfigurationRequestRequestTypeDef",
-    {
-        "Name": str,
-        "ServerProperties": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalCreateConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateConfigurationRequestRequestTypeDef",
-    {
-        "Description": str,
-        "KafkaVersions": Sequence[str],
-    },
-    total=False,
-)
-
-
-class CreateConfigurationRequestRequestTypeDef(
-    _RequiredCreateConfigurationRequestRequestTypeDef,
-    _OptionalCreateConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredCreateVpcConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcConnectionRequestRequestTypeDef",
     {
         "TargetClusterArn": str,
         "Authentication": str,
         "VpcId": str,
         "ClientSubnets": Sequence[str],
@@ -508,22 +477,20 @@
     "_OptionalCreateVpcConnectionRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateVpcConnectionRequestRequestTypeDef(
     _RequiredCreateVpcConnectionRequestRequestTypeDef,
     _OptionalCreateVpcConnectionRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteClusterPolicyRequestRequestTypeDef = TypedDict(
     "DeleteClusterPolicyRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 
@@ -537,21 +504,19 @@
     "_OptionalDeleteClusterRequestRequestTypeDef",
     {
         "CurrentVersion": str,
     },
     total=False,
 )
 
-
 class DeleteClusterRequestRequestTypeDef(
     _RequiredDeleteClusterRequestRequestTypeDef, _OptionalDeleteClusterRequestRequestTypeDef
 ):
     pass
 
-
 DeleteConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteConfigurationRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
@@ -702,22 +667,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListClientVpcConnectionsRequestRequestTypeDef(
     _RequiredListClientVpcConnectionsRequestRequestTypeDef,
     _OptionalListClientVpcConnectionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListClusterOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredListClusterOperationsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListClusterOperationsRequestRequestTypeDef = TypedDict(
@@ -725,22 +688,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListClusterOperationsRequestRequestTypeDef(
     _RequiredListClusterOperationsRequestRequestTypeDef,
     _OptionalListClusterOperationsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListClusterOperationsV2RequestRequestTypeDef = TypedDict(
     "_RequiredListClusterOperationsV2RequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListClusterOperationsV2RequestRequestTypeDef = TypedDict(
@@ -748,22 +709,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListClusterOperationsV2RequestRequestTypeDef(
     _RequiredListClusterOperationsV2RequestRequestTypeDef,
     _OptionalListClusterOperationsV2RequestRequestTypeDef,
 ):
     pass
 
-
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "ClusterNameFilter": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -792,22 +751,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListConfigurationRevisionsRequestRequestTypeDef(
     _RequiredListConfigurationRevisionsRequestRequestTypeDef,
     _OptionalListConfigurationRevisionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListConfigurationsRequestRequestTypeDef = TypedDict(
     "ListConfigurationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -833,21 +790,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListNodesRequestRequestTypeDef(
     _RequiredListNodesRequestRequestTypeDef, _OptionalListNodesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListScramSecretsRequestRequestTypeDef = TypedDict(
     "_RequiredListScramSecretsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListScramSecretsRequestRequestTypeDef = TypedDict(
@@ -855,21 +810,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListScramSecretsRequestRequestTypeDef(
     _RequiredListScramSecretsRequestRequestTypeDef, _OptionalListScramSecretsRequestRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -896,19 +849,17 @@
         "Authentication": str,
         "VpcId": str,
         "State": VpcConnectionStateType,
     },
     total=False,
 )
 
-
 class VpcConnectionTypeDef(_RequiredVpcConnectionTypeDef, _OptionalVpcConnectionTypeDef):
     pass
 
-
 NodeExporterInfoTypeDef = TypedDict(
     "NodeExporterInfoTypeDef",
     {
         "EnabledInBroker": bool,
     },
 )
 
@@ -942,21 +893,19 @@
     "_OptionalPutClusterPolicyRequestRequestTypeDef",
     {
         "CurrentVersion": str,
     },
     total=False,
 )
 
-
 class PutClusterPolicyRequestRequestTypeDef(
     _RequiredPutClusterPolicyRequestRequestTypeDef, _OptionalPutClusterPolicyRequestRequestTypeDef
 ):
     pass
 
-
 RebootBrokerRequestRequestTypeDef = TypedDict(
     "RebootBrokerRequestRequestTypeDef",
     {
         "BrokerIds": Sequence[str],
         "ClusterArn": str,
     },
 )
@@ -987,38 +936,34 @@
     "_OptionalVpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class VpcConfigTypeDef(_RequiredVpcConfigTypeDef, _OptionalVpcConfigTypeDef):
     pass
 
-
 _RequiredVpcConfigOutputTypeDef = TypedDict(
     "_RequiredVpcConfigOutputTypeDef",
     {
         "SubnetIds": List[str],
     },
 )
 _OptionalVpcConfigOutputTypeDef = TypedDict(
     "_OptionalVpcConfigOutputTypeDef",
     {
         "SecurityGroupIds": List[str],
     },
     total=False,
 )
 
-
 class VpcConfigOutputTypeDef(_RequiredVpcConfigOutputTypeDef, _OptionalVpcConfigOutputTypeDef):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -1045,37 +990,14 @@
     {
         "ClusterArn": str,
         "CurrentVersion": str,
         "TargetInstanceType": str,
     },
 )
 
-_RequiredUpdateConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateConfigurationRequestRequestTypeDef",
-    {
-        "Arn": str,
-        "ServerProperties": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalUpdateConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateConfigurationRequestRequestTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-
-class UpdateConfigurationRequestRequestTypeDef(
-    _RequiredUpdateConfigurationRequestRequestTypeDef,
-    _OptionalUpdateConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
 UserIdentityTypeDef = TypedDict(
     "UserIdentityTypeDef",
     {
         "Type": UserIdentityTypeType,
         "PrincipalId": str,
     },
     total=False,
@@ -1358,14 +1280,57 @@
     {
         "ClusterArn": str,
         "UnprocessedScramSecrets": List[UnprocessedScramSecretTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateConfigurationRequestRequestTypeDef",
+    {
+        "Name": str,
+        "ServerProperties": BlobTypeDef,
+    },
+)
+_OptionalCreateConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+        "KafkaVersions": Sequence[str],
+    },
+    total=False,
+)
+
+class CreateConfigurationRequestRequestTypeDef(
+    _RequiredCreateConfigurationRequestRequestTypeDef,
+    _OptionalCreateConfigurationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateConfigurationRequestRequestTypeDef",
+    {
+        "Arn": str,
+        "ServerProperties": BlobTypeDef,
+    },
+)
+_OptionalUpdateConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+class UpdateConfigurationRequestRequestTypeDef(
+    _RequiredUpdateConfigurationRequestRequestTypeDef,
+    _OptionalUpdateConfigurationRequestRequestTypeDef,
+):
+    pass
+
 _RequiredBrokerEBSVolumeInfoTypeDef = TypedDict(
     "_RequiredBrokerEBSVolumeInfoTypeDef",
     {
         "KafkaBrokerNodeId": str,
     },
 )
 _OptionalBrokerEBSVolumeInfoTypeDef = TypedDict(
@@ -1373,21 +1338,19 @@
     {
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
         "VolumeSizeGB": int,
     },
     total=False,
 )
 
-
 class BrokerEBSVolumeInfoTypeDef(
     _RequiredBrokerEBSVolumeInfoTypeDef, _OptionalBrokerEBSVolumeInfoTypeDef
 ):
     pass
 
-
 EBSStorageInfoTypeDef = TypedDict(
     "EBSStorageInfoTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
         "VolumeSize": int,
     },
     total=False,
@@ -1406,21 +1369,19 @@
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
         "StorageMode": StorageModeType,
         "VolumeSizeGB": int,
     },
     total=False,
 )
 
-
 class UpdateStorageRequestRequestTypeDef(
     _RequiredUpdateStorageRequestRequestTypeDef, _OptionalUpdateStorageRequestRequestTypeDef
 ):
     pass
 
-
 BrokerLogsTypeDef = TypedDict(
     "BrokerLogsTypeDef",
     {
         "CloudWatchLogs": CloudWatchLogsTypeDef,
         "Firehose": FirehoseTypeDef,
         "S3": S3TypeDef,
     },
@@ -1496,22 +1457,20 @@
     "_OptionalUpdateClusterKafkaVersionRequestRequestTypeDef",
     {
         "ConfigurationInfo": ConfigurationInfoTypeDef,
     },
     total=False,
 )
 
-
 class UpdateClusterKafkaVersionRequestRequestTypeDef(
     _RequiredUpdateClusterKafkaVersionRequestRequestTypeDef,
     _OptionalUpdateClusterKafkaVersionRequestRequestTypeDef,
 ):
     pass
 
-
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "Description": str,
         "KafkaVersions": List[str],
@@ -1601,66 +1560,60 @@
     "_OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef(
     _RequiredListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
     _OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
     "_RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
     "_OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListClusterOperationsRequestListClusterOperationsPaginateTypeDef(
     _RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
     _OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef = TypedDict(
     "_RequiredListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef = TypedDict(
     "_OptionalListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef(
     _RequiredListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef,
     _OptionalListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef,
 ):
     pass
 
-
 ListClustersRequestListClustersPaginateTypeDef = TypedDict(
     "ListClustersRequestListClustersPaginateTypeDef",
     {
         "ClusterNameFilter": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1686,22 +1639,20 @@
     "_OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef(
     _RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
     _OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
 ):
     pass
 
-
 ListConfigurationsRequestListConfigurationsPaginateTypeDef = TypedDict(
     "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1724,44 +1675,40 @@
     "_OptionalListNodesRequestListNodesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListNodesRequestListNodesPaginateTypeDef(
     _RequiredListNodesRequestListNodesPaginateTypeDef,
     _OptionalListNodesRequestListNodesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef = TypedDict(
     "_RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef = TypedDict(
     "_OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListScramSecretsRequestListScramSecretsPaginateTypeDef(
     _RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef,
     _OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef,
 ):
     pass
 
-
 ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef = TypedDict(
     "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1957,40 +1904,36 @@
     "_OptionalServerlessRequestTypeDef",
     {
         "ClientAuthentication": ServerlessClientAuthenticationTypeDef,
     },
     total=False,
 )
 
-
 class ServerlessRequestTypeDef(
     _RequiredServerlessRequestTypeDef, _OptionalServerlessRequestTypeDef
 ):
     pass
 
-
 _RequiredServerlessTypeDef = TypedDict(
     "_RequiredServerlessTypeDef",
     {
         "VpcConfigs": List[VpcConfigOutputTypeDef],
     },
 )
 _OptionalServerlessTypeDef = TypedDict(
     "_OptionalServerlessTypeDef",
     {
         "ClientAuthentication": ServerlessClientAuthenticationTypeDef,
     },
     total=False,
 )
 
-
 class ServerlessTypeDef(_RequiredServerlessTypeDef, _OptionalServerlessTypeDef):
     pass
 
-
 _RequiredUpdateMonitoringRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMonitoringRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "CurrentVersion": str,
     },
 )
@@ -2000,21 +1943,22 @@
         "EnhancedMonitoring": EnhancedMonitoringType,
         "OpenMonitoring": OpenMonitoringInfoTypeDef,
         "LoggingInfo": LoggingInfoTypeDef,
     },
     total=False,
 )
 
-
 class UpdateMonitoringRequestRequestTypeDef(
     _RequiredUpdateMonitoringRequestRequestTypeDef, _OptionalUpdateMonitoringRequestRequestTypeDef
 ):
     pass
 
-
+ClientAuthenticationUnionTypeDef = Union[
+    ClientAuthenticationTypeDef, ClientAuthenticationOutputTypeDef
+]
 _RequiredUpdateSecurityRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSecurityRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "CurrentVersion": str,
     },
 )
@@ -2023,21 +1967,19 @@
     {
         "ClientAuthentication": ClientAuthenticationTypeDef,
         "EncryptionInfo": EncryptionInfoTypeDef,
     },
     total=False,
 )
 
-
 class UpdateSecurityRequestRequestTypeDef(
     _RequiredUpdateSecurityRequestRequestTypeDef, _OptionalUpdateSecurityRequestRequestTypeDef
 ):
     pass
 
-
 VpcConnectivityTypeDef = TypedDict(
     "VpcConnectivityTypeDef",
     {
         "ClientAuthentication": VpcConnectivityClientAuthenticationTypeDef,
     },
     total=False,
 )
@@ -2066,21 +2008,19 @@
         "StorageInfo": StorageInfoTypeDef,
         "ConnectivityInfo": ConnectivityInfoTypeDef,
         "ZoneIds": List[str],
     },
     total=False,
 )
 
-
 class BrokerNodeGroupInfoOutputTypeDef(
     _RequiredBrokerNodeGroupInfoOutputTypeDef, _OptionalBrokerNodeGroupInfoOutputTypeDef
 ):
     pass
 
-
 _RequiredBrokerNodeGroupInfoTypeDef = TypedDict(
     "_RequiredBrokerNodeGroupInfoTypeDef",
     {
         "ClientSubnets": Sequence[str],
         "InstanceType": str,
     },
 )
@@ -2092,21 +2032,19 @@
         "StorageInfo": StorageInfoTypeDef,
         "ConnectivityInfo": ConnectivityInfoTypeDef,
         "ZoneIds": Sequence[str],
     },
     total=False,
 )
 
-
 class BrokerNodeGroupInfoTypeDef(
     _RequiredBrokerNodeGroupInfoTypeDef, _OptionalBrokerNodeGroupInfoTypeDef
 ):
     pass
 
-
 MutableClusterInfoTypeDef = TypedDict(
     "MutableClusterInfoTypeDef",
     {
         "BrokerEBSVolumeInfo": List[BrokerEBSVolumeInfoTypeDef],
         "ConfigurationInfo": ConfigurationInfoTypeDef,
         "NumberOfBrokerNodes": int,
         "EnhancedMonitoring": EnhancedMonitoringType,
@@ -2176,19 +2114,20 @@
         "ZookeeperConnectString": str,
         "ZookeeperConnectStringTls": str,
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
-
 class ProvisionedTypeDef(_RequiredProvisionedTypeDef, _OptionalProvisionedTypeDef):
     pass
 
-
+BrokerNodeGroupInfoUnionTypeDef = Union[
+    BrokerNodeGroupInfoTypeDef, BrokerNodeGroupInfoOutputTypeDef
+]
 _RequiredCreateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterRequestRequestTypeDef",
     {
         "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
         "ClusterName": str,
         "KafkaVersion": str,
         "NumberOfBrokerNodes": int,
@@ -2205,21 +2144,19 @@
         "LoggingInfo": LoggingInfoTypeDef,
         "Tags": Mapping[str, str],
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
-
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredProvisionedRequestTypeDef = TypedDict(
     "_RequiredProvisionedRequestTypeDef",
     {
         "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
         "KafkaVersion": str,
         "NumberOfBrokerNodes": int,
     },
@@ -2234,21 +2171,19 @@
         "OpenMonitoring": OpenMonitoringInfoTypeDef,
         "LoggingInfo": LoggingInfoTypeDef,
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
-
 class ProvisionedRequestTypeDef(
     _RequiredProvisionedRequestTypeDef, _OptionalProvisionedRequestTypeDef
 ):
     pass
 
-
 ClusterOperationInfoTypeDef = TypedDict(
     "ClusterOperationInfoTypeDef",
     {
         "ClientRequestId": str,
         "ClusterArn": str,
         "CreationTime": datetime,
         "EndTime": datetime,
@@ -2322,21 +2257,19 @@
         "Tags": Mapping[str, str],
         "Provisioned": ProvisionedRequestTypeDef,
         "Serverless": ServerlessRequestTypeDef,
     },
     total=False,
 )
 
-
 class CreateClusterV2RequestRequestTypeDef(
     _RequiredCreateClusterV2RequestRequestTypeDef, _OptionalCreateClusterV2RequestRequestTypeDef
 ):
     pass
 
-
 DescribeClusterOperationResponseTypeDef = TypedDict(
     "DescribeClusterOperationResponseTypeDef",
     {
         "ClusterOperationInfo": ClusterOperationInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/type_defs.pyi` & `mypy-boto3-kafka-1.28.16/mypy_boto3_kafka/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_kafka.type_defs import BatchAssociateScramSecretRequestRequestTypeDef
 
-    data: BatchAssociateScramSecretRequestRequestTypeDef = {...}
+    data: BatchAssociateScramSecretRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -34,19 +34,21 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "BatchAssociateScramSecretRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "UnprocessedScramSecretTypeDef",
     "BatchDisassociateScramSecretRequestRequestTypeDef",
+    "BlobTypeDef",
     "ProvisionedThroughputTypeDef",
     "CloudWatchLogsTypeDef",
     "FirehoseTypeDef",
     "S3TypeDef",
     "BrokerSoftwareInfoTypeDef",
     "TlsOutputTypeDef",
     "UnauthenticatedTypeDef",
@@ -56,15 +58,14 @@
     "ErrorInfoTypeDef",
     "ClusterOperationStepInfoTypeDef",
     "ClusterOperationV2SummaryTypeDef",
     "CompatibleKafkaVersionTypeDef",
     "ConfigurationInfoTypeDef",
     "ConfigurationRevisionTypeDef",
     "PublicAccessTypeDef",
-    "CreateConfigurationRequestRequestTypeDef",
     "CreateVpcConnectionRequestRequestTypeDef",
     "DeleteClusterPolicyRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteConfigurationRequestRequestTypeDef",
     "DeleteVpcConnectionRequestRequestTypeDef",
     "DescribeClusterOperationRequestRequestTypeDef",
     "DescribeClusterOperationV2RequestRequestTypeDef",
@@ -105,15 +106,14 @@
     "ScramTypeDef",
     "VpcConfigTypeDef",
     "VpcConfigOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrokerCountRequestRequestTypeDef",
     "UpdateBrokerTypeRequestRequestTypeDef",
-    "UpdateConfigurationRequestRequestTypeDef",
     "UserIdentityTypeDef",
     "VpcConnectivityTlsTypeDef",
     "VpcConnectivityIamTypeDef",
     "VpcConnectivityScramTypeDef",
     "CreateClusterResponseTypeDef",
     "CreateClusterV2ResponseTypeDef",
     "CreateVpcConnectionResponseTypeDef",
@@ -136,14 +136,16 @@
     "UpdateClusterKafkaVersionResponseTypeDef",
     "UpdateConnectivityResponseTypeDef",
     "UpdateMonitoringResponseTypeDef",
     "UpdateSecurityResponseTypeDef",
     "UpdateStorageResponseTypeDef",
     "BatchAssociateScramSecretResponseTypeDef",
     "BatchDisassociateScramSecretResponseTypeDef",
+    "CreateConfigurationRequestRequestTypeDef",
+    "UpdateConfigurationRequestRequestTypeDef",
     "BrokerEBSVolumeInfoTypeDef",
     "EBSStorageInfoTypeDef",
     "UpdateStorageRequestRequestTypeDef",
     "BrokerLogsTypeDef",
     "BrokerNodeInfoTypeDef",
     "ListClientVpcConnectionsResponseTypeDef",
     "ClusterOperationStepTypeDef",
@@ -189,23 +191,25 @@
     "ClientAuthenticationTypeDef",
     "ClusterOperationV2ServerlessTypeDef",
     "VpcConnectivityClientAuthenticationTypeDef",
     "ListNodesResponseTypeDef",
     "ServerlessRequestTypeDef",
     "ServerlessTypeDef",
     "UpdateMonitoringRequestRequestTypeDef",
+    "ClientAuthenticationUnionTypeDef",
     "UpdateSecurityRequestRequestTypeDef",
     "VpcConnectivityTypeDef",
     "ConnectivityInfoTypeDef",
     "BrokerNodeGroupInfoOutputTypeDef",
     "BrokerNodeGroupInfoTypeDef",
     "MutableClusterInfoTypeDef",
     "UpdateConnectivityRequestRequestTypeDef",
     "ClusterInfoTypeDef",
     "ProvisionedTypeDef",
+    "BrokerNodeGroupInfoUnionTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "ProvisionedRequestTypeDef",
     "ClusterOperationInfoTypeDef",
     "ClusterOperationV2ProvisionedTypeDef",
     "DescribeClusterResponseTypeDef",
     "ListClustersResponseTypeDef",
     "ClusterTypeDef",
@@ -251,14 +255,15 @@
     "BatchDisassociateScramSecretRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "SecretArnList": Sequence[str],
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ProvisionedThroughputTypeDef = TypedDict(
     "ProvisionedThroughputTypeDef",
     {
         "Enabled": bool,
         "VolumeThroughput": int,
     },
     total=False,
@@ -274,34 +279,38 @@
     "_OptionalCloudWatchLogsTypeDef",
     {
         "LogGroup": str,
     },
     total=False,
 )
 
+
 class CloudWatchLogsTypeDef(_RequiredCloudWatchLogsTypeDef, _OptionalCloudWatchLogsTypeDef):
     pass
 
+
 _RequiredFirehoseTypeDef = TypedDict(
     "_RequiredFirehoseTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalFirehoseTypeDef = TypedDict(
     "_OptionalFirehoseTypeDef",
     {
         "DeliveryStream": str,
     },
     total=False,
 )
 
+
 class FirehoseTypeDef(_RequiredFirehoseTypeDef, _OptionalFirehoseTypeDef):
     pass
 
+
 _RequiredS3TypeDef = TypedDict(
     "_RequiredS3TypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalS3TypeDef = TypedDict(
@@ -309,17 +318,19 @@
     {
         "Bucket": str,
         "Prefix": str,
     },
     total=False,
 )
 
+
 class S3TypeDef(_RequiredS3TypeDef, _OptionalS3TypeDef):
     pass
 
+
 BrokerSoftwareInfoTypeDef = TypedDict(
     "BrokerSoftwareInfoTypeDef",
     {
         "ConfigurationArn": str,
         "ConfigurationRevision": int,
         "KafkaVersion": str,
     },
@@ -365,19 +376,21 @@
         "CreationTime": datetime,
         "State": VpcConnectionStateType,
         "Owner": str,
     },
     total=False,
 )
 
+
 class ClientVpcConnectionTypeDef(
     _RequiredClientVpcConnectionTypeDef, _OptionalClientVpcConnectionTypeDef
 ):
     pass
 
+
 StateInfoTypeDef = TypedDict(
     "StateInfoTypeDef",
     {
         "Code": str,
         "Message": str,
     },
     total=False,
@@ -442,49 +455,29 @@
     "_OptionalConfigurationRevisionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class ConfigurationRevisionTypeDef(
     _RequiredConfigurationRevisionTypeDef, _OptionalConfigurationRevisionTypeDef
 ):
     pass
 
+
 PublicAccessTypeDef = TypedDict(
     "PublicAccessTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-_RequiredCreateConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateConfigurationRequestRequestTypeDef",
-    {
-        "Name": str,
-        "ServerProperties": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalCreateConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateConfigurationRequestRequestTypeDef",
-    {
-        "Description": str,
-        "KafkaVersions": Sequence[str],
-    },
-    total=False,
-)
-
-class CreateConfigurationRequestRequestTypeDef(
-    _RequiredCreateConfigurationRequestRequestTypeDef,
-    _OptionalCreateConfigurationRequestRequestTypeDef,
-):
-    pass
-
 _RequiredCreateVpcConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcConnectionRequestRequestTypeDef",
     {
         "TargetClusterArn": str,
         "Authentication": str,
         "VpcId": str,
         "ClientSubnets": Sequence[str],
@@ -495,20 +488,22 @@
     "_OptionalCreateVpcConnectionRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateVpcConnectionRequestRequestTypeDef(
     _RequiredCreateVpcConnectionRequestRequestTypeDef,
     _OptionalCreateVpcConnectionRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteClusterPolicyRequestRequestTypeDef = TypedDict(
     "DeleteClusterPolicyRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 
@@ -522,19 +517,21 @@
     "_OptionalDeleteClusterRequestRequestTypeDef",
     {
         "CurrentVersion": str,
     },
     total=False,
 )
 
+
 class DeleteClusterRequestRequestTypeDef(
     _RequiredDeleteClusterRequestRequestTypeDef, _OptionalDeleteClusterRequestRequestTypeDef
 ):
     pass
 
+
 DeleteConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteConfigurationRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
@@ -685,20 +682,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListClientVpcConnectionsRequestRequestTypeDef(
     _RequiredListClientVpcConnectionsRequestRequestTypeDef,
     _OptionalListClientVpcConnectionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListClusterOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredListClusterOperationsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListClusterOperationsRequestRequestTypeDef = TypedDict(
@@ -706,20 +705,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListClusterOperationsRequestRequestTypeDef(
     _RequiredListClusterOperationsRequestRequestTypeDef,
     _OptionalListClusterOperationsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListClusterOperationsV2RequestRequestTypeDef = TypedDict(
     "_RequiredListClusterOperationsV2RequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListClusterOperationsV2RequestRequestTypeDef = TypedDict(
@@ -727,20 +728,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListClusterOperationsV2RequestRequestTypeDef(
     _RequiredListClusterOperationsV2RequestRequestTypeDef,
     _OptionalListClusterOperationsV2RequestRequestTypeDef,
 ):
     pass
 
+
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "ClusterNameFilter": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -769,20 +772,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListConfigurationRevisionsRequestRequestTypeDef(
     _RequiredListConfigurationRevisionsRequestRequestTypeDef,
     _OptionalListConfigurationRevisionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListConfigurationsRequestRequestTypeDef = TypedDict(
     "ListConfigurationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -808,19 +813,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListNodesRequestRequestTypeDef(
     _RequiredListNodesRequestRequestTypeDef, _OptionalListNodesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListScramSecretsRequestRequestTypeDef = TypedDict(
     "_RequiredListScramSecretsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListScramSecretsRequestRequestTypeDef = TypedDict(
@@ -828,19 +835,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListScramSecretsRequestRequestTypeDef(
     _RequiredListScramSecretsRequestRequestTypeDef, _OptionalListScramSecretsRequestRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -867,17 +876,19 @@
         "Authentication": str,
         "VpcId": str,
         "State": VpcConnectionStateType,
     },
     total=False,
 )
 
+
 class VpcConnectionTypeDef(_RequiredVpcConnectionTypeDef, _OptionalVpcConnectionTypeDef):
     pass
 
+
 NodeExporterInfoTypeDef = TypedDict(
     "NodeExporterInfoTypeDef",
     {
         "EnabledInBroker": bool,
     },
 )
 
@@ -911,19 +922,21 @@
     "_OptionalPutClusterPolicyRequestRequestTypeDef",
     {
         "CurrentVersion": str,
     },
     total=False,
 )
 
+
 class PutClusterPolicyRequestRequestTypeDef(
     _RequiredPutClusterPolicyRequestRequestTypeDef, _OptionalPutClusterPolicyRequestRequestTypeDef
 ):
     pass
 
+
 RebootBrokerRequestRequestTypeDef = TypedDict(
     "RebootBrokerRequestRequestTypeDef",
     {
         "BrokerIds": Sequence[str],
         "ClusterArn": str,
     },
 )
@@ -954,34 +967,38 @@
     "_OptionalVpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class VpcConfigTypeDef(_RequiredVpcConfigTypeDef, _OptionalVpcConfigTypeDef):
     pass
 
+
 _RequiredVpcConfigOutputTypeDef = TypedDict(
     "_RequiredVpcConfigOutputTypeDef",
     {
         "SubnetIds": List[str],
     },
 )
 _OptionalVpcConfigOutputTypeDef = TypedDict(
     "_OptionalVpcConfigOutputTypeDef",
     {
         "SecurityGroupIds": List[str],
     },
     total=False,
 )
 
+
 class VpcConfigOutputTypeDef(_RequiredVpcConfigOutputTypeDef, _OptionalVpcConfigOutputTypeDef):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -1008,35 +1025,14 @@
     {
         "ClusterArn": str,
         "CurrentVersion": str,
         "TargetInstanceType": str,
     },
 )
 
-_RequiredUpdateConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateConfigurationRequestRequestTypeDef",
-    {
-        "Arn": str,
-        "ServerProperties": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalUpdateConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateConfigurationRequestRequestTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-class UpdateConfigurationRequestRequestTypeDef(
-    _RequiredUpdateConfigurationRequestRequestTypeDef,
-    _OptionalUpdateConfigurationRequestRequestTypeDef,
-):
-    pass
-
 UserIdentityTypeDef = TypedDict(
     "UserIdentityTypeDef",
     {
         "Type": UserIdentityTypeType,
         "PrincipalId": str,
     },
     total=False,
@@ -1319,14 +1315,61 @@
     {
         "ClusterArn": str,
         "UnprocessedScramSecrets": List[UnprocessedScramSecretTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateConfigurationRequestRequestTypeDef",
+    {
+        "Name": str,
+        "ServerProperties": BlobTypeDef,
+    },
+)
+_OptionalCreateConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+        "KafkaVersions": Sequence[str],
+    },
+    total=False,
+)
+
+
+class CreateConfigurationRequestRequestTypeDef(
+    _RequiredCreateConfigurationRequestRequestTypeDef,
+    _OptionalCreateConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateConfigurationRequestRequestTypeDef",
+    {
+        "Arn": str,
+        "ServerProperties": BlobTypeDef,
+    },
+)
+_OptionalUpdateConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+
+class UpdateConfigurationRequestRequestTypeDef(
+    _RequiredUpdateConfigurationRequestRequestTypeDef,
+    _OptionalUpdateConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredBrokerEBSVolumeInfoTypeDef = TypedDict(
     "_RequiredBrokerEBSVolumeInfoTypeDef",
     {
         "KafkaBrokerNodeId": str,
     },
 )
 _OptionalBrokerEBSVolumeInfoTypeDef = TypedDict(
@@ -1334,19 +1377,21 @@
     {
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
         "VolumeSizeGB": int,
     },
     total=False,
 )
 
+
 class BrokerEBSVolumeInfoTypeDef(
     _RequiredBrokerEBSVolumeInfoTypeDef, _OptionalBrokerEBSVolumeInfoTypeDef
 ):
     pass
 
+
 EBSStorageInfoTypeDef = TypedDict(
     "EBSStorageInfoTypeDef",
     {
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
         "VolumeSize": int,
     },
     total=False,
@@ -1365,19 +1410,21 @@
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
         "StorageMode": StorageModeType,
         "VolumeSizeGB": int,
     },
     total=False,
 )
 
+
 class UpdateStorageRequestRequestTypeDef(
     _RequiredUpdateStorageRequestRequestTypeDef, _OptionalUpdateStorageRequestRequestTypeDef
 ):
     pass
 
+
 BrokerLogsTypeDef = TypedDict(
     "BrokerLogsTypeDef",
     {
         "CloudWatchLogs": CloudWatchLogsTypeDef,
         "Firehose": FirehoseTypeDef,
         "S3": S3TypeDef,
     },
@@ -1453,20 +1500,22 @@
     "_OptionalUpdateClusterKafkaVersionRequestRequestTypeDef",
     {
         "ConfigurationInfo": ConfigurationInfoTypeDef,
     },
     total=False,
 )
 
+
 class UpdateClusterKafkaVersionRequestRequestTypeDef(
     _RequiredUpdateClusterKafkaVersionRequestRequestTypeDef,
     _OptionalUpdateClusterKafkaVersionRequestRequestTypeDef,
 ):
     pass
 
+
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "Description": str,
         "KafkaVersions": List[str],
@@ -1556,60 +1605,66 @@
     "_OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef(
     _RequiredListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
     _OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
     "_RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
     "_OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListClusterOperationsRequestListClusterOperationsPaginateTypeDef(
     _RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
     _OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef = TypedDict(
     "_RequiredListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef = TypedDict(
     "_OptionalListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef(
     _RequiredListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef,
     _OptionalListClusterOperationsV2RequestListClusterOperationsV2PaginateTypeDef,
 ):
     pass
 
+
 ListClustersRequestListClustersPaginateTypeDef = TypedDict(
     "ListClustersRequestListClustersPaginateTypeDef",
     {
         "ClusterNameFilter": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1635,20 +1690,22 @@
     "_OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef(
     _RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
     _OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
 ):
     pass
 
+
 ListConfigurationsRequestListConfigurationsPaginateTypeDef = TypedDict(
     "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1671,40 +1728,44 @@
     "_OptionalListNodesRequestListNodesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListNodesRequestListNodesPaginateTypeDef(
     _RequiredListNodesRequestListNodesPaginateTypeDef,
     _OptionalListNodesRequestListNodesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef = TypedDict(
     "_RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef = TypedDict(
     "_OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListScramSecretsRequestListScramSecretsPaginateTypeDef(
     _RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef,
     _OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef,
 ):
     pass
 
+
 ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef = TypedDict(
     "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1900,36 +1961,40 @@
     "_OptionalServerlessRequestTypeDef",
     {
         "ClientAuthentication": ServerlessClientAuthenticationTypeDef,
     },
     total=False,
 )
 
+
 class ServerlessRequestTypeDef(
     _RequiredServerlessRequestTypeDef, _OptionalServerlessRequestTypeDef
 ):
     pass
 
+
 _RequiredServerlessTypeDef = TypedDict(
     "_RequiredServerlessTypeDef",
     {
         "VpcConfigs": List[VpcConfigOutputTypeDef],
     },
 )
 _OptionalServerlessTypeDef = TypedDict(
     "_OptionalServerlessTypeDef",
     {
         "ClientAuthentication": ServerlessClientAuthenticationTypeDef,
     },
     total=False,
 )
 
+
 class ServerlessTypeDef(_RequiredServerlessTypeDef, _OptionalServerlessTypeDef):
     pass
 
+
 _RequiredUpdateMonitoringRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMonitoringRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "CurrentVersion": str,
     },
 )
@@ -1939,19 +2004,24 @@
         "EnhancedMonitoring": EnhancedMonitoringType,
         "OpenMonitoring": OpenMonitoringInfoTypeDef,
         "LoggingInfo": LoggingInfoTypeDef,
     },
     total=False,
 )
 
+
 class UpdateMonitoringRequestRequestTypeDef(
     _RequiredUpdateMonitoringRequestRequestTypeDef, _OptionalUpdateMonitoringRequestRequestTypeDef
 ):
     pass
 
+
+ClientAuthenticationUnionTypeDef = Union[
+    ClientAuthenticationTypeDef, ClientAuthenticationOutputTypeDef
+]
 _RequiredUpdateSecurityRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSecurityRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "CurrentVersion": str,
     },
 )
@@ -1960,19 +2030,21 @@
     {
         "ClientAuthentication": ClientAuthenticationTypeDef,
         "EncryptionInfo": EncryptionInfoTypeDef,
     },
     total=False,
 )
 
+
 class UpdateSecurityRequestRequestTypeDef(
     _RequiredUpdateSecurityRequestRequestTypeDef, _OptionalUpdateSecurityRequestRequestTypeDef
 ):
     pass
 
+
 VpcConnectivityTypeDef = TypedDict(
     "VpcConnectivityTypeDef",
     {
         "ClientAuthentication": VpcConnectivityClientAuthenticationTypeDef,
     },
     total=False,
 )
@@ -2001,19 +2073,21 @@
         "StorageInfo": StorageInfoTypeDef,
         "ConnectivityInfo": ConnectivityInfoTypeDef,
         "ZoneIds": List[str],
     },
     total=False,
 )
 
+
 class BrokerNodeGroupInfoOutputTypeDef(
     _RequiredBrokerNodeGroupInfoOutputTypeDef, _OptionalBrokerNodeGroupInfoOutputTypeDef
 ):
     pass
 
+
 _RequiredBrokerNodeGroupInfoTypeDef = TypedDict(
     "_RequiredBrokerNodeGroupInfoTypeDef",
     {
         "ClientSubnets": Sequence[str],
         "InstanceType": str,
     },
 )
@@ -2025,19 +2099,21 @@
         "StorageInfo": StorageInfoTypeDef,
         "ConnectivityInfo": ConnectivityInfoTypeDef,
         "ZoneIds": Sequence[str],
     },
     total=False,
 )
 
+
 class BrokerNodeGroupInfoTypeDef(
     _RequiredBrokerNodeGroupInfoTypeDef, _OptionalBrokerNodeGroupInfoTypeDef
 ):
     pass
 
+
 MutableClusterInfoTypeDef = TypedDict(
     "MutableClusterInfoTypeDef",
     {
         "BrokerEBSVolumeInfo": List[BrokerEBSVolumeInfoTypeDef],
         "ConfigurationInfo": ConfigurationInfoTypeDef,
         "NumberOfBrokerNodes": int,
         "EnhancedMonitoring": EnhancedMonitoringType,
@@ -2107,17 +2183,22 @@
         "ZookeeperConnectString": str,
         "ZookeeperConnectStringTls": str,
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
+
 class ProvisionedTypeDef(_RequiredProvisionedTypeDef, _OptionalProvisionedTypeDef):
     pass
 
+
+BrokerNodeGroupInfoUnionTypeDef = Union[
+    BrokerNodeGroupInfoTypeDef, BrokerNodeGroupInfoOutputTypeDef
+]
 _RequiredCreateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterRequestRequestTypeDef",
     {
         "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
         "ClusterName": str,
         "KafkaVersion": str,
         "NumberOfBrokerNodes": int,
@@ -2134,19 +2215,21 @@
         "LoggingInfo": LoggingInfoTypeDef,
         "Tags": Mapping[str, str],
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
+
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredProvisionedRequestTypeDef = TypedDict(
     "_RequiredProvisionedRequestTypeDef",
     {
         "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
         "KafkaVersion": str,
         "NumberOfBrokerNodes": int,
     },
@@ -2161,19 +2244,21 @@
         "OpenMonitoring": OpenMonitoringInfoTypeDef,
         "LoggingInfo": LoggingInfoTypeDef,
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
+
 class ProvisionedRequestTypeDef(
     _RequiredProvisionedRequestTypeDef, _OptionalProvisionedRequestTypeDef
 ):
     pass
 
+
 ClusterOperationInfoTypeDef = TypedDict(
     "ClusterOperationInfoTypeDef",
     {
         "ClientRequestId": str,
         "ClusterArn": str,
         "CreationTime": datetime,
         "EndTime": datetime,
@@ -2247,19 +2332,21 @@
         "Tags": Mapping[str, str],
         "Provisioned": ProvisionedRequestTypeDef,
         "Serverless": ServerlessRequestTypeDef,
     },
     total=False,
 )
 
+
 class CreateClusterV2RequestRequestTypeDef(
     _RequiredCreateClusterV2RequestRequestTypeDef, _OptionalCreateClusterV2RequestRequestTypeDef
 ):
     pass
 
+
 DescribeClusterOperationResponseTypeDef = TypedDict(
     "DescribeClusterOperationResponseTypeDef",
     {
         "ClusterOperationInfo": ClusterOperationInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka.egg-info/PKG-INFO` & `mypy-boto3-kafka-1.28.16/mypy_boto3_kafka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kafka
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Kafka 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Kafka 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kafka type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 kafka type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kafka)](https://pepy.tech/project/mypy-boto3-kafka)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kafka 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
+[boto3.Kafka 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
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
 [mypy-boto3-kafka docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/).
 
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
@@ -366,27 +366,28 @@
 )
 
 
 def check_value(value: BrokerAZDistributionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kafka.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kafka.type_defs import (
     BatchAssociateScramSecretRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     UnprocessedScramSecretTypeDef,
     BatchDisassociateScramSecretRequestRequestTypeDef,
+    BlobTypeDef,
     ProvisionedThroughputTypeDef,
     CloudWatchLogsTypeDef,
     FirehoseTypeDef,
     S3TypeDef,
     BrokerSoftwareInfoTypeDef,
     TlsOutputTypeDef,
     UnauthenticatedTypeDef,
@@ -396,15 +397,14 @@
     ErrorInfoTypeDef,
     ClusterOperationStepInfoTypeDef,
     ClusterOperationV2SummaryTypeDef,
     CompatibleKafkaVersionTypeDef,
     ConfigurationInfoTypeDef,
     ConfigurationRevisionTypeDef,
     PublicAccessTypeDef,
-    CreateConfigurationRequestRequestTypeDef,
     CreateVpcConnectionRequestRequestTypeDef,
     DeleteClusterPolicyRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteConfigurationRequestRequestTypeDef,
     DeleteVpcConnectionRequestRequestTypeDef,
     DescribeClusterOperationRequestRequestTypeDef,
     DescribeClusterOperationV2RequestRequestTypeDef,
@@ -445,15 +445,14 @@
     ScramTypeDef,
     VpcConfigTypeDef,
     VpcConfigOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrokerCountRequestRequestTypeDef,
     UpdateBrokerTypeRequestRequestTypeDef,
-    UpdateConfigurationRequestRequestTypeDef,
     UserIdentityTypeDef,
     VpcConnectivityTlsTypeDef,
     VpcConnectivityIamTypeDef,
     VpcConnectivityScramTypeDef,
     CreateClusterResponseTypeDef,
     CreateClusterV2ResponseTypeDef,
     CreateVpcConnectionResponseTypeDef,
@@ -476,14 +475,16 @@
     UpdateClusterKafkaVersionResponseTypeDef,
     UpdateConnectivityResponseTypeDef,
     UpdateMonitoringResponseTypeDef,
     UpdateSecurityResponseTypeDef,
     UpdateStorageResponseTypeDef,
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
+    CreateConfigurationRequestRequestTypeDef,
+    UpdateConfigurationRequestRequestTypeDef,
     BrokerEBSVolumeInfoTypeDef,
     EBSStorageInfoTypeDef,
     UpdateStorageRequestRequestTypeDef,
     BrokerLogsTypeDef,
     BrokerNodeInfoTypeDef,
     ListClientVpcConnectionsResponseTypeDef,
     ClusterOperationStepTypeDef,
@@ -529,23 +530,25 @@
     ClientAuthenticationTypeDef,
     ClusterOperationV2ServerlessTypeDef,
     VpcConnectivityClientAuthenticationTypeDef,
     ListNodesResponseTypeDef,
     ServerlessRequestTypeDef,
     ServerlessTypeDef,
     UpdateMonitoringRequestRequestTypeDef,
+    ClientAuthenticationUnionTypeDef,
     UpdateSecurityRequestRequestTypeDef,
     VpcConnectivityTypeDef,
     ConnectivityInfoTypeDef,
     BrokerNodeGroupInfoOutputTypeDef,
     BrokerNodeGroupInfoTypeDef,
     MutableClusterInfoTypeDef,
     UpdateConnectivityRequestRequestTypeDef,
     ClusterInfoTypeDef,
     ProvisionedTypeDef,
+    BrokerNodeGroupInfoUnionTypeDef,
     CreateClusterRequestRequestTypeDef,
     ProvisionedRequestTypeDef,
     ClusterOperationInfoTypeDef,
     ClusterOperationV2ProvisionedTypeDef,
     DescribeClusterResponseTypeDef,
     ListClustersResponseTypeDef,
     ClusterTypeDef,
@@ -555,15 +558,15 @@
     ClusterOperationV2TypeDef,
     DescribeClusterV2ResponseTypeDef,
     ListClustersV2ResponseTypeDef,
     DescribeClusterOperationV2ResponseTypeDef,
 )
 
 
-def get_structure() -> BatchAssociateScramSecretRequestRequestTypeDef:
+def get_value() -> BatchAssociateScramSecretRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka.egg-info/SOURCES.txt` & `mypy-boto3-kafka-1.28.16/mypy_boto3_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.15.post1/setup.py` & `mypy-boto3-kafka-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kafka",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_kafka"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Kafka 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.Kafka 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 kafka type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 kafka type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_kafka": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

