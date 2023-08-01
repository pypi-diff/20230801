# Comparing `tmp/mypy-boto3-network-firewall-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-network-firewall-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-network-firewall-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:46 2023, max compression
+gzip compressed data, was "mypy-boto3-network-firewall-1.28.16.tar", last modified: Tue Aug  1 11:37:26 2023, max compression
```

## Comparing `mypy-boto3-network-firewall-1.28.15.post1.tar` & `mypy-boto3-network-firewall-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:46.249309 mypy-boto3-network-firewall-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20271 2023-07-29 10:03:46.237309 mypy-boto3-network-firewall-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18743 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:46.229309 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32579 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32531 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11095 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55242 2023-07-29 09:52:07.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55176 2023-07-29 09:52:06.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:52:05.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:46.237309 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20271 2023-07-29 10:03:45.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-29 10:03:46.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:45.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:45.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:45.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 10:03:45.000000 mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:46.249309 mypy-boto3-network-firewall-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-29 09:52:04.000000 mypy-boto3-network-firewall-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:26.884805 mypy-boto3-network-firewall-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:25:02.000000 mypy-boto3-network-firewall-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20402 2023-08-01 11:37:26.880805 mypy-boto3-network-firewall-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18883 2023-08-01 11:25:02.000000 mypy-boto3-network-firewall-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:26.876805 mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-08-01 11:25:02.000000 mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-01 11:25:02.000000 mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-01 11:25:02.000000 mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32144 2023-08-01 11:25:03.000000 mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32096 2023-08-01 11:25:02.000000 mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11095 2023-08-01 11:25:03.000000 mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-08-01 11:25:03.000000 mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-08-01 11:25:03.000000 mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-08-01 11:25:03.000000 mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:25:02.000000 mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    55795 2023-08-01 11:25:04.000000 mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55729 2023-08-01 11:25:04.000000 mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:25:02.000000 mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:26.880805 mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20402 2023-08-01 11:37:26.000000 mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-01 11:37:26.000000 mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:26.000000 mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:26.000000 mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:26.000000 mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 11:37:26.000000 mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:26.884805 mypy-boto3-network-firewall-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-08-01 11:25:02.000000 mypy-boto3-network-firewall-1.28.16/setup.py
```

### Comparing `mypy-boto3-network-firewall-1.28.15.post1/LICENSE` & `mypy-boto3-network-firewall-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.15.post1/PKG-INFO` & `mypy-boto3-network-firewall-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-network-firewall
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.NetworkFirewall 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.NetworkFirewall 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 network-firewall type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 network-firewall type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-network-firewall.svg?color=blue)](https://pypi.org/project/mypy-boto3-network-firewall)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-network-firewall)](https://pepy.tech/project/mypy-boto3-network-firewall)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.NetworkFirewall 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
+[boto3.NetworkFirewall 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
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
 [mypy-boto3-network-firewall docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/).
 
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
@@ -352,20 +352,20 @@
 )
 
 
 def check_value(value: AttachmentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_network_firewall.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_network_firewall.type_defs import (
     AddressTypeDef,
     AssociateFirewallPolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     SubnetMappingTypeDef,
@@ -480,14 +480,15 @@
     CreateRuleGroupResponseTypeDef,
     DeleteRuleGroupResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     ActionDefinitionOutputTypeDef,
     ActionDefinitionTypeDef,
     DescribeLoggingConfigurationResponseTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
+    LoggingConfigurationUnionTypeDef,
     UpdateLoggingConfigurationRequestRequestTypeDef,
     ServerCertificateConfigurationOutputTypeDef,
     ServerCertificateConfigurationTypeDef,
     RuleDefinitionOutputTypeDef,
     RuleDefinitionTypeDef,
     CreateTLSInspectionConfigurationResponseTypeDef,
     DeleteTLSInspectionConfigurationResponseTypeDef,
@@ -502,31 +503,34 @@
     CreateFirewallResponseTypeDef,
     DeleteFirewallResponseTypeDef,
     DescribeFirewallResponseTypeDef,
     FirewallPolicyOutputTypeDef,
     FirewallPolicyTypeDef,
     DescribeTLSInspectionConfigurationResponseTypeDef,
     CreateTLSInspectionConfigurationRequestRequestTypeDef,
+    TLSInspectionConfigurationUnionTypeDef,
     UpdateTLSInspectionConfigurationRequestRequestTypeDef,
     StatelessRulesAndCustomActionsOutputTypeDef,
     StatelessRulesAndCustomActionsTypeDef,
     DescribeFirewallPolicyResponseTypeDef,
     CreateFirewallPolicyRequestRequestTypeDef,
+    FirewallPolicyUnionTypeDef,
     UpdateFirewallPolicyRequestRequestTypeDef,
     RulesSourceOutputTypeDef,
     RulesSourceTypeDef,
     RuleGroupOutputTypeDef,
     RuleGroupTypeDef,
     DescribeRuleGroupResponseTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
+    RuleGroupUnionTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_value() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-network-firewall-1.28.15.post1/README.md` & `mypy-boto3-network-firewall-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-network-firewall.svg?color=blue)](https://pypi.org/project/mypy-boto3-network-firewall)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-network-firewall)](https://pepy.tech/project/mypy-boto3-network-firewall)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.NetworkFirewall 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
+[boto3.NetworkFirewall 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
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
 [mypy-boto3-network-firewall docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/).
 
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
@@ -320,20 +320,20 @@
 )
 
 
 def check_value(value: AttachmentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_network_firewall.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_network_firewall.type_defs import (
     AddressTypeDef,
     AssociateFirewallPolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     SubnetMappingTypeDef,
@@ -448,14 +448,15 @@
     CreateRuleGroupResponseTypeDef,
     DeleteRuleGroupResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     ActionDefinitionOutputTypeDef,
     ActionDefinitionTypeDef,
     DescribeLoggingConfigurationResponseTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
+    LoggingConfigurationUnionTypeDef,
     UpdateLoggingConfigurationRequestRequestTypeDef,
     ServerCertificateConfigurationOutputTypeDef,
     ServerCertificateConfigurationTypeDef,
     RuleDefinitionOutputTypeDef,
     RuleDefinitionTypeDef,
     CreateTLSInspectionConfigurationResponseTypeDef,
     DeleteTLSInspectionConfigurationResponseTypeDef,
@@ -470,31 +471,34 @@
     CreateFirewallResponseTypeDef,
     DeleteFirewallResponseTypeDef,
     DescribeFirewallResponseTypeDef,
     FirewallPolicyOutputTypeDef,
     FirewallPolicyTypeDef,
     DescribeTLSInspectionConfigurationResponseTypeDef,
     CreateTLSInspectionConfigurationRequestRequestTypeDef,
+    TLSInspectionConfigurationUnionTypeDef,
     UpdateTLSInspectionConfigurationRequestRequestTypeDef,
     StatelessRulesAndCustomActionsOutputTypeDef,
     StatelessRulesAndCustomActionsTypeDef,
     DescribeFirewallPolicyResponseTypeDef,
     CreateFirewallPolicyRequestRequestTypeDef,
+    FirewallPolicyUnionTypeDef,
     UpdateFirewallPolicyRequestRequestTypeDef,
     RulesSourceOutputTypeDef,
     RulesSourceTypeDef,
     RuleGroupOutputTypeDef,
     RuleGroupTypeDef,
     DescribeRuleGroupResponseTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
+    RuleGroupUnionTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_value() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/__init__.py` & `mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/__init__.pyi` & `mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/__main__.py` & `mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.NetworkFirewall 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.NetworkFirewall 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall\nOther"
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

### Comparing `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/client.py` & `mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_network_firewall.client import NetworkFirewallClient
 
     session = Session()
     client: NetworkFirewallClient = session.client("network-firewall")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ResourceManagedStatusType, ResourceManagedTypeType, RuleGroupTypeType
 from .paginator import (
     ListFirewallPoliciesPaginator,
     ListFirewallsPaginator,
@@ -42,30 +42,26 @@
     DescribeLoggingConfigurationResponseTypeDef,
     DescribeResourcePolicyResponseTypeDef,
     DescribeRuleGroupMetadataResponseTypeDef,
     DescribeRuleGroupResponseTypeDef,
     DescribeTLSInspectionConfigurationResponseTypeDef,
     DisassociateSubnetsResponseTypeDef,
     EncryptionConfigurationTypeDef,
-    FirewallPolicyOutputTypeDef,
-    FirewallPolicyTypeDef,
+    FirewallPolicyUnionTypeDef,
     ListFirewallPoliciesResponseTypeDef,
     ListFirewallsResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTLSInspectionConfigurationsResponseTypeDef,
-    LoggingConfigurationOutputTypeDef,
-    LoggingConfigurationTypeDef,
-    RuleGroupOutputTypeDef,
-    RuleGroupTypeDef,
+    LoggingConfigurationUnionTypeDef,
+    RuleGroupUnionTypeDef,
     SourceMetadataTypeDef,
     SubnetMappingTypeDef,
     TagTypeDef,
-    TLSInspectionConfigurationOutputTypeDef,
-    TLSInspectionConfigurationTypeDef,
+    TLSInspectionConfigurationUnionTypeDef,
     UpdateFirewallDeleteProtectionResponseTypeDef,
     UpdateFirewallDescriptionResponseTypeDef,
     UpdateFirewallEncryptionConfigurationResponseTypeDef,
     UpdateFirewallPolicyChangeProtectionResponseTypeDef,
     UpdateFirewallPolicyResponseTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
@@ -191,15 +187,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#create_firewall)
         """
 
     def create_firewall_policy(
         self,
         *,
         FirewallPolicyName: str,
-        FirewallPolicy: Union[FirewallPolicyTypeDef, FirewallPolicyOutputTypeDef],
+        FirewallPolicy: FirewallPolicyUnionTypeDef,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> CreateFirewallPolicyResponseTypeDef:
         """
         Creates the firewall policy for the firewall according to the specifications.
@@ -210,15 +206,15 @@
 
     def create_rule_group(
         self,
         *,
         RuleGroupName: str,
         Type: RuleGroupTypeType,
         Capacity: int,
-        RuleGroup: Union[RuleGroupTypeDef, RuleGroupOutputTypeDef] = ...,
+        RuleGroup: RuleGroupUnionTypeDef = ...,
         Rules: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         SourceMetadata: SourceMetadataTypeDef = ...
     ) -> CreateRuleGroupResponseTypeDef:
@@ -230,17 +226,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#create_rule_group)
         """
 
     def create_tls_inspection_configuration(
         self,
         *,
         TLSInspectionConfigurationName: str,
-        TLSInspectionConfiguration: Union[
-            TLSInspectionConfigurationTypeDef, TLSInspectionConfigurationOutputTypeDef
-        ],
+        TLSInspectionConfiguration: TLSInspectionConfigurationUnionTypeDef,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> CreateTLSInspectionConfigurationResponseTypeDef:
         """
         Creates an Network Firewall TLS inspection configuration.
 
@@ -523,15 +517,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_firewall_encryption_configuration)
         """
 
     def update_firewall_policy(
         self,
         *,
         UpdateToken: str,
-        FirewallPolicy: Union[FirewallPolicyTypeDef, FirewallPolicyOutputTypeDef],
+        FirewallPolicy: FirewallPolicyUnionTypeDef,
         FirewallPolicyArn: str = ...,
         FirewallPolicyName: str = ...,
         Description: str = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> UpdateFirewallPolicyResponseTypeDef:
         """
@@ -558,32 +552,30 @@
         """
 
     def update_logging_configuration(
         self,
         *,
         FirewallArn: str = ...,
         FirewallName: str = ...,
-        LoggingConfiguration: Union[
-            LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
-        ] = ...
+        LoggingConfiguration: LoggingConfigurationUnionTypeDef = ...
     ) -> UpdateLoggingConfigurationResponseTypeDef:
         """
         Sets the logging configuration for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_logging_configuration)
         """
 
     def update_rule_group(
         self,
         *,
         UpdateToken: str,
         RuleGroupArn: str = ...,
         RuleGroupName: str = ...,
-        RuleGroup: Union[RuleGroupTypeDef, RuleGroupOutputTypeDef] = ...,
+        RuleGroup: RuleGroupUnionTypeDef = ...,
         Rules: str = ...,
         Type: RuleGroupTypeType = ...,
         Description: str = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         SourceMetadata: SourceMetadataTypeDef = ...
     ) -> UpdateRuleGroupResponseTypeDef:
@@ -610,17 +602,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_subnet_change_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_subnet_change_protection)
         """
 
     def update_tls_inspection_configuration(
         self,
         *,
-        TLSInspectionConfiguration: Union[
-            TLSInspectionConfigurationTypeDef, TLSInspectionConfigurationOutputTypeDef
-        ],
+        TLSInspectionConfiguration: TLSInspectionConfigurationUnionTypeDef,
         UpdateToken: str,
         TLSInspectionConfigurationArn: str = ...,
         TLSInspectionConfigurationName: str = ...,
         Description: str = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> UpdateTLSInspectionConfigurationResponseTypeDef:
         """
```

### Comparing `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/client.pyi` & `mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_network_firewall.client import NetworkFirewallClient
 
     session = Session()
     client: NetworkFirewallClient = session.client("network-firewall")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ResourceManagedStatusType, ResourceManagedTypeType, RuleGroupTypeType
 from .paginator import (
     ListFirewallPoliciesPaginator,
     ListFirewallsPaginator,
@@ -42,30 +42,26 @@
     DescribeLoggingConfigurationResponseTypeDef,
     DescribeResourcePolicyResponseTypeDef,
     DescribeRuleGroupMetadataResponseTypeDef,
     DescribeRuleGroupResponseTypeDef,
     DescribeTLSInspectionConfigurationResponseTypeDef,
     DisassociateSubnetsResponseTypeDef,
     EncryptionConfigurationTypeDef,
-    FirewallPolicyOutputTypeDef,
-    FirewallPolicyTypeDef,
+    FirewallPolicyUnionTypeDef,
     ListFirewallPoliciesResponseTypeDef,
     ListFirewallsResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTLSInspectionConfigurationsResponseTypeDef,
-    LoggingConfigurationOutputTypeDef,
-    LoggingConfigurationTypeDef,
-    RuleGroupOutputTypeDef,
-    RuleGroupTypeDef,
+    LoggingConfigurationUnionTypeDef,
+    RuleGroupUnionTypeDef,
     SourceMetadataTypeDef,
     SubnetMappingTypeDef,
     TagTypeDef,
-    TLSInspectionConfigurationOutputTypeDef,
-    TLSInspectionConfigurationTypeDef,
+    TLSInspectionConfigurationUnionTypeDef,
     UpdateFirewallDeleteProtectionResponseTypeDef,
     UpdateFirewallDescriptionResponseTypeDef,
     UpdateFirewallEncryptionConfigurationResponseTypeDef,
     UpdateFirewallPolicyChangeProtectionResponseTypeDef,
     UpdateFirewallPolicyResponseTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
@@ -181,15 +177,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_firewall)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#create_firewall)
         """
     def create_firewall_policy(
         self,
         *,
         FirewallPolicyName: str,
-        FirewallPolicy: Union[FirewallPolicyTypeDef, FirewallPolicyOutputTypeDef],
+        FirewallPolicy: FirewallPolicyUnionTypeDef,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> CreateFirewallPolicyResponseTypeDef:
         """
         Creates the firewall policy for the firewall according to the specifications.
@@ -199,15 +195,15 @@
         """
     def create_rule_group(
         self,
         *,
         RuleGroupName: str,
         Type: RuleGroupTypeType,
         Capacity: int,
-        RuleGroup: Union[RuleGroupTypeDef, RuleGroupOutputTypeDef] = ...,
+        RuleGroup: RuleGroupUnionTypeDef = ...,
         Rules: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         SourceMetadata: SourceMetadataTypeDef = ...
     ) -> CreateRuleGroupResponseTypeDef:
@@ -218,17 +214,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.create_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#create_rule_group)
         """
     def create_tls_inspection_configuration(
         self,
         *,
         TLSInspectionConfigurationName: str,
-        TLSInspectionConfiguration: Union[
-            TLSInspectionConfigurationTypeDef, TLSInspectionConfigurationOutputTypeDef
-        ],
+        TLSInspectionConfiguration: TLSInspectionConfigurationUnionTypeDef,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> CreateTLSInspectionConfigurationResponseTypeDef:
         """
         Creates an Network Firewall TLS inspection configuration.
 
@@ -485,15 +479,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_firewall_encryption_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_firewall_encryption_configuration)
         """
     def update_firewall_policy(
         self,
         *,
         UpdateToken: str,
-        FirewallPolicy: Union[FirewallPolicyTypeDef, FirewallPolicyOutputTypeDef],
+        FirewallPolicy: FirewallPolicyUnionTypeDef,
         FirewallPolicyArn: str = ...,
         FirewallPolicyName: str = ...,
         Description: str = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> UpdateFirewallPolicyResponseTypeDef:
         """
@@ -518,31 +512,29 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_firewall_policy_change_protection)
         """
     def update_logging_configuration(
         self,
         *,
         FirewallArn: str = ...,
         FirewallName: str = ...,
-        LoggingConfiguration: Union[
-            LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
-        ] = ...
+        LoggingConfiguration: LoggingConfigurationUnionTypeDef = ...
     ) -> UpdateLoggingConfigurationResponseTypeDef:
         """
         Sets the logging configuration for the specified firewall.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_logging_configuration)
         """
     def update_rule_group(
         self,
         *,
         UpdateToken: str,
         RuleGroupArn: str = ...,
         RuleGroupName: str = ...,
-        RuleGroup: Union[RuleGroupTypeDef, RuleGroupOutputTypeDef] = ...,
+        RuleGroup: RuleGroupUnionTypeDef = ...,
         Rules: str = ...,
         Type: RuleGroupTypeType = ...,
         Description: str = ...,
         DryRun: bool = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         SourceMetadata: SourceMetadataTypeDef = ...
     ) -> UpdateRuleGroupResponseTypeDef:
@@ -567,17 +559,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client.update_subnet_change_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/client/#update_subnet_change_protection)
         """
     def update_tls_inspection_configuration(
         self,
         *,
-        TLSInspectionConfiguration: Union[
-            TLSInspectionConfigurationTypeDef, TLSInspectionConfigurationOutputTypeDef
-        ],
+        TLSInspectionConfiguration: TLSInspectionConfigurationUnionTypeDef,
         UpdateToken: str,
         TLSInspectionConfigurationArn: str = ...,
         TLSInspectionConfigurationName: str = ...,
         Description: str = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...
     ) -> UpdateTLSInspectionConfigurationResponseTypeDef:
         """
```

### Comparing `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/literals.py` & `mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/literals.pyi` & `mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/paginator.py` & `mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/paginator.pyi` & `mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/type_defs.py` & `mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_network_firewall.type_defs import AddressTypeDef
 
-    data: AddressTypeDef = {...}
+    data: AddressTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AttachmentStatusType,
     ConfigurationSyncStateType,
     EncryptionTypeType,
     FirewallStatusValueType,
     GeneratedRulesTypeType,
@@ -164,14 +164,15 @@
     "CreateRuleGroupResponseTypeDef",
     "DeleteRuleGroupResponseTypeDef",
     "UpdateRuleGroupResponseTypeDef",
     "ActionDefinitionOutputTypeDef",
     "ActionDefinitionTypeDef",
     "DescribeLoggingConfigurationResponseTypeDef",
     "UpdateLoggingConfigurationResponseTypeDef",
+    "LoggingConfigurationUnionTypeDef",
     "UpdateLoggingConfigurationRequestRequestTypeDef",
     "ServerCertificateConfigurationOutputTypeDef",
     "ServerCertificateConfigurationTypeDef",
     "RuleDefinitionOutputTypeDef",
     "RuleDefinitionTypeDef",
     "CreateTLSInspectionConfigurationResponseTypeDef",
     "DeleteTLSInspectionConfigurationResponseTypeDef",
@@ -186,26 +187,29 @@
     "CreateFirewallResponseTypeDef",
     "DeleteFirewallResponseTypeDef",
     "DescribeFirewallResponseTypeDef",
     "FirewallPolicyOutputTypeDef",
     "FirewallPolicyTypeDef",
     "DescribeTLSInspectionConfigurationResponseTypeDef",
     "CreateTLSInspectionConfigurationRequestRequestTypeDef",
+    "TLSInspectionConfigurationUnionTypeDef",
     "UpdateTLSInspectionConfigurationRequestRequestTypeDef",
     "StatelessRulesAndCustomActionsOutputTypeDef",
     "StatelessRulesAndCustomActionsTypeDef",
     "DescribeFirewallPolicyResponseTypeDef",
     "CreateFirewallPolicyRequestRequestTypeDef",
+    "FirewallPolicyUnionTypeDef",
     "UpdateFirewallPolicyRequestRequestTypeDef",
     "RulesSourceOutputTypeDef",
     "RulesSourceTypeDef",
     "RuleGroupOutputTypeDef",
     "RuleGroupTypeDef",
     "DescribeRuleGroupResponseTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
+    "RuleGroupUnionTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
 )
 
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "AddressDefinition": str,
@@ -1586,14 +1590,17 @@
         "FirewallArn": str,
         "FirewallName": str,
         "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LoggingConfigurationUnionTypeDef = Union[
+    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+]
 UpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateLoggingConfigurationRequestRequestTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
@@ -1842,14 +1849,17 @@
 class CreateTLSInspectionConfigurationRequestRequestTypeDef(
     _RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef,
     _OptionalCreateTLSInspectionConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+TLSInspectionConfigurationUnionTypeDef = Union[
+    TLSInspectionConfigurationTypeDef, TLSInspectionConfigurationOutputTypeDef
+]
 _RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef",
     {
         "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
         "UpdateToken": str,
     },
 )
@@ -1947,14 +1957,15 @@
 class CreateFirewallPolicyRequestRequestTypeDef(
     _RequiredCreateFirewallPolicyRequestRequestTypeDef,
     _OptionalCreateFirewallPolicyRequestRequestTypeDef,
 ):
     pass
 
 
+FirewallPolicyUnionTypeDef = Union[FirewallPolicyTypeDef, FirewallPolicyOutputTypeDef]
 _RequiredUpdateFirewallPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallPolicyRequestRequestTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicy": FirewallPolicyTypeDef,
     },
 )
@@ -2077,14 +2088,15 @@
 
 class CreateRuleGroupRequestRequestTypeDef(
     _RequiredCreateRuleGroupRequestRequestTypeDef, _OptionalCreateRuleGroupRequestRequestTypeDef
 ):
     pass
 
 
+RuleGroupUnionTypeDef = Union[RuleGroupTypeDef, RuleGroupOutputTypeDef]
 _RequiredUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleGroupRequestRequestTypeDef",
     {
         "UpdateToken": str,
     },
 )
 _OptionalUpdateRuleGroupRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall/type_defs.pyi` & `mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_network_firewall.type_defs import AddressTypeDef
 
-    data: AddressTypeDef = {...}
+    data: AddressTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AttachmentStatusType,
     ConfigurationSyncStateType,
     EncryptionTypeType,
     FirewallStatusValueType,
     GeneratedRulesTypeType,
@@ -163,14 +163,15 @@
     "CreateRuleGroupResponseTypeDef",
     "DeleteRuleGroupResponseTypeDef",
     "UpdateRuleGroupResponseTypeDef",
     "ActionDefinitionOutputTypeDef",
     "ActionDefinitionTypeDef",
     "DescribeLoggingConfigurationResponseTypeDef",
     "UpdateLoggingConfigurationResponseTypeDef",
+    "LoggingConfigurationUnionTypeDef",
     "UpdateLoggingConfigurationRequestRequestTypeDef",
     "ServerCertificateConfigurationOutputTypeDef",
     "ServerCertificateConfigurationTypeDef",
     "RuleDefinitionOutputTypeDef",
     "RuleDefinitionTypeDef",
     "CreateTLSInspectionConfigurationResponseTypeDef",
     "DeleteTLSInspectionConfigurationResponseTypeDef",
@@ -185,26 +186,29 @@
     "CreateFirewallResponseTypeDef",
     "DeleteFirewallResponseTypeDef",
     "DescribeFirewallResponseTypeDef",
     "FirewallPolicyOutputTypeDef",
     "FirewallPolicyTypeDef",
     "DescribeTLSInspectionConfigurationResponseTypeDef",
     "CreateTLSInspectionConfigurationRequestRequestTypeDef",
+    "TLSInspectionConfigurationUnionTypeDef",
     "UpdateTLSInspectionConfigurationRequestRequestTypeDef",
     "StatelessRulesAndCustomActionsOutputTypeDef",
     "StatelessRulesAndCustomActionsTypeDef",
     "DescribeFirewallPolicyResponseTypeDef",
     "CreateFirewallPolicyRequestRequestTypeDef",
+    "FirewallPolicyUnionTypeDef",
     "UpdateFirewallPolicyRequestRequestTypeDef",
     "RulesSourceOutputTypeDef",
     "RulesSourceTypeDef",
     "RuleGroupOutputTypeDef",
     "RuleGroupTypeDef",
     "DescribeRuleGroupResponseTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
+    "RuleGroupUnionTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
 )
 
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "AddressDefinition": str,
@@ -1545,14 +1549,17 @@
         "FirewallArn": str,
         "FirewallName": str,
         "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LoggingConfigurationUnionTypeDef = Union[
+    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+]
 UpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateLoggingConfigurationRequestRequestTypeDef",
     {
         "FirewallArn": str,
         "FirewallName": str,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
@@ -1793,14 +1800,17 @@
 
 class CreateTLSInspectionConfigurationRequestRequestTypeDef(
     _RequiredCreateTLSInspectionConfigurationRequestRequestTypeDef,
     _OptionalCreateTLSInspectionConfigurationRequestRequestTypeDef,
 ):
     pass
 
+TLSInspectionConfigurationUnionTypeDef = Union[
+    TLSInspectionConfigurationTypeDef, TLSInspectionConfigurationOutputTypeDef
+]
 _RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTLSInspectionConfigurationRequestRequestTypeDef",
     {
         "TLSInspectionConfiguration": TLSInspectionConfigurationTypeDef,
         "UpdateToken": str,
     },
 )
@@ -1890,14 +1900,15 @@
 
 class CreateFirewallPolicyRequestRequestTypeDef(
     _RequiredCreateFirewallPolicyRequestRequestTypeDef,
     _OptionalCreateFirewallPolicyRequestRequestTypeDef,
 ):
     pass
 
+FirewallPolicyUnionTypeDef = Union[FirewallPolicyTypeDef, FirewallPolicyOutputTypeDef]
 _RequiredUpdateFirewallPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallPolicyRequestRequestTypeDef",
     {
         "UpdateToken": str,
         "FirewallPolicy": FirewallPolicyTypeDef,
     },
 )
@@ -2012,14 +2023,15 @@
 )
 
 class CreateRuleGroupRequestRequestTypeDef(
     _RequiredCreateRuleGroupRequestRequestTypeDef, _OptionalCreateRuleGroupRequestRequestTypeDef
 ):
     pass
 
+RuleGroupUnionTypeDef = Union[RuleGroupTypeDef, RuleGroupOutputTypeDef]
 _RequiredUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleGroupRequestRequestTypeDef",
     {
         "UpdateToken": str,
     },
 )
 _OptionalUpdateRuleGroupRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall.egg-info/PKG-INFO` & `mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-network-firewall
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.NetworkFirewall 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.NetworkFirewall 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 network-firewall type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 network-firewall type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-network-firewall.svg?color=blue)](https://pypi.org/project/mypy-boto3-network-firewall)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-network-firewall)](https://pepy.tech/project/mypy-boto3-network-firewall)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.NetworkFirewall 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
+[boto3.NetworkFirewall 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
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
 [mypy-boto3-network-firewall docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/).
 
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
@@ -352,20 +352,20 @@
 )
 
 
 def check_value(value: AttachmentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_network_firewall.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_network_firewall.type_defs import (
     AddressTypeDef,
     AssociateFirewallPolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     SubnetMappingTypeDef,
@@ -480,14 +480,15 @@
     CreateRuleGroupResponseTypeDef,
     DeleteRuleGroupResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     ActionDefinitionOutputTypeDef,
     ActionDefinitionTypeDef,
     DescribeLoggingConfigurationResponseTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
+    LoggingConfigurationUnionTypeDef,
     UpdateLoggingConfigurationRequestRequestTypeDef,
     ServerCertificateConfigurationOutputTypeDef,
     ServerCertificateConfigurationTypeDef,
     RuleDefinitionOutputTypeDef,
     RuleDefinitionTypeDef,
     CreateTLSInspectionConfigurationResponseTypeDef,
     DeleteTLSInspectionConfigurationResponseTypeDef,
@@ -502,31 +503,34 @@
     CreateFirewallResponseTypeDef,
     DeleteFirewallResponseTypeDef,
     DescribeFirewallResponseTypeDef,
     FirewallPolicyOutputTypeDef,
     FirewallPolicyTypeDef,
     DescribeTLSInspectionConfigurationResponseTypeDef,
     CreateTLSInspectionConfigurationRequestRequestTypeDef,
+    TLSInspectionConfigurationUnionTypeDef,
     UpdateTLSInspectionConfigurationRequestRequestTypeDef,
     StatelessRulesAndCustomActionsOutputTypeDef,
     StatelessRulesAndCustomActionsTypeDef,
     DescribeFirewallPolicyResponseTypeDef,
     CreateFirewallPolicyRequestRequestTypeDef,
+    FirewallPolicyUnionTypeDef,
     UpdateFirewallPolicyRequestRequestTypeDef,
     RulesSourceOutputTypeDef,
     RulesSourceTypeDef,
     RuleGroupOutputTypeDef,
     RuleGroupTypeDef,
     DescribeRuleGroupResponseTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
+    RuleGroupUnionTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_value() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-network-firewall-1.28.15.post1/mypy_boto3_network_firewall.egg-info/SOURCES.txt` & `mypy-boto3-network-firewall-1.28.16/mypy_boto3_network_firewall.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.28.15.post1/setup.py` & `mypy-boto3-network-firewall-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-network-firewall",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_network_firewall"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.NetworkFirewall 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.NetworkFirewall 1.28.16 service generated with"
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
-    keywords="boto3 network-firewall type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 network-firewall type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_network_firewall": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

