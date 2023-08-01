# Comparing `tmp/mypy-boto3-inspector2-1.28.16.tar.gz` & `tmp/mypy-boto3-inspector2-1.28.16.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-inspector2-1.28.16.tar", last modified: Mon Jul 31 19:32:46 2023, max compression
+gzip compressed data, was "mypy-boto3-inspector2-1.28.16.post1.tar", last modified: Tue Aug  1 11:36:56 2023, max compression
```

## Comparing `mypy-boto3-inspector2-1.28.16.tar` & `mypy-boto3-inspector2-1.28.16.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.246207 mypy-boto3-inspector2-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23511 2023-07-31 19:32:46.246207 mypy-boto3-inspector2-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22012 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.242207 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36576 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36513 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17810 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17808 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    77088 2023-07-31 19:32:17.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    77007 2023-07-31 19:32:16.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.246207 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23511 2023-07-31 19:32:46.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-31 19:32:46.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:46.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:46.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 19:32:46.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 19:32:46.000000 mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:32:46.246207 mypy-boto3-inspector2-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-31 19:32:15.000000 mypy-boto3-inspector2-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:56.532873 mypy-boto3-inspector2-1.28.16.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:20:00.000000 mypy-boto3-inspector2-1.28.16.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23607 2023-08-01 11:36:56.532873 mypy-boto3-inspector2-1.28.16.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22105 2023-08-01 11:20:00.000000 mypy-boto3-inspector2-1.28.16.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:56.532873 mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-01 11:20:00.000000 mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-01 11:20:00.000000 mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-01 11:20:00.000000 mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36320 2023-08-01 11:20:00.000000 mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36257 2023-08-01 11:20:00.000000 mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17810 2023-08-01 11:20:01.000000 mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17808 2023-08-01 11:20:00.000000 mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-08-01 11:20:00.000000 mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-08-01 11:20:00.000000 mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:20:00.000000 mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    77414 2023-08-01 11:20:03.000000 mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77333 2023-08-01 11:20:02.000000 mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 11:20:00.000000 mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:56.532873 mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23607 2023-08-01 11:36:56.000000 mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-01 11:36:56.000000 mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:56.000000 mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:56.000000 mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:56.000000 mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 11:36:56.000000 mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:56.532873 mypy-boto3-inspector2-1.28.16.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-01 11:20:00.000000 mypy-boto3-inspector2-1.28.16.post1/setup.py
```

### Comparing `mypy-boto3-inspector2-1.28.16/LICENSE` & `mypy-boto3-inspector2-1.28.16.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.16/PKG-INFO` & `mypy-boto3-inspector2-1.28.16.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector2
-Version: 1.28.16
-Summary: Type annotations for boto3.Inspector2 1.28.16 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16.post1
+Summary: Type annotations for boto3.Inspector2 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 inspector2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 inspector2 type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -47,15 +47,15 @@
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
 [mypy-boto3-inspector2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/).
 
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
@@ -411,20 +411,20 @@
 )
 
 
 def check_value(value: AccountSortByType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_inspector2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_inspector2.type_defs import (
     SeverityCountsTypeDef,
     AccountAggregationTypeDef,
     StateTypeDef,
     ResourceStatusTypeDef,
@@ -451,25 +451,24 @@
     CancelFindingsReportRequestRequestTypeDef,
     CancelSbomExportRequestRequestTypeDef,
     CisaDataTypeDef,
     CodeFilePathTypeDef,
     CodeLineTypeDef,
     SuggestedFixTypeDef,
     CountsTypeDef,
-    CoverageDateFilterTypeDef,
+    TimestampTypeDef,
     CoverageMapFilterTypeDef,
     CoverageStringFilterTypeDef,
     ScanStatusTypeDef,
     DestinationTypeDef,
     Cvss2TypeDef,
     Cvss3TypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DateFilterOutputTypeDef,
-    DateFilterTypeDef,
     DelegatedAdminAccountTypeDef,
     DelegatedAdminTypeDef,
     DeleteFilterRequestRequestTypeDef,
     DisableDelegatedAdminAccountRequestRequestTypeDef,
     DisableRequestRequestTypeDef,
     DisassociateMemberRequestRequestTypeDef,
     MapFilterTypeDef,
@@ -559,15 +558,16 @@
     AwsLambdaFunctionDetailsTypeDef,
     BatchGetMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef,
     CodeVulnerabilityDetailsTypeDef,
     CodeSnippetResultTypeDef,
     ListCoverageStatisticsResponseTypeDef,
-    CoverageFilterCriteriaTypeDef,
+    CoverageDateFilterTypeDef,
+    DateFilterTypeDef,
     CvssScoreDetailsTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     Ec2InstanceAggregationTypeDef,
     LambdaFunctionAggregationTypeDef,
     EcrConfigurationStateTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
@@ -594,51 +594,54 @@
     UsageTotalTypeDef,
     AggregationResponseTypeDef,
     AccountStateTypeDef,
     DisableResponseTypeDef,
     EnableResponseTypeDef,
     ResourceDetailsTypeDef,
     BatchGetCodeSnippetResponseTypeDef,
-    ListCoverageRequestListCoveragePaginateTypeDef,
-    ListCoverageRequestRequestTypeDef,
-    ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef,
-    ListCoverageStatisticsRequestRequestTypeDef,
+    CoverageFilterCriteriaTypeDef,
     InspectorScoreDetailsTypeDef,
     AggregationRequestTypeDef,
     GetConfigurationResponseTypeDef,
     BatchGetFindingDetailsResponseTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
     FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     BatchGetFreeTrialInfoResponseTypeDef,
     CoveredResourceTypeDef,
     NetworkReachabilityDetailsTypeDef,
     GetSbomExportResponseTypeDef,
     CreateSbomExportRequestRequestTypeDef,
+    ResourceFilterCriteriaUnionTypeDef,
     ListUsageTotalsResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     BatchGetAccountStatusResponseTypeDef,
     ResourceTypeDef,
+    ListCoverageRequestListCoveragePaginateTypeDef,
+    ListCoverageRequestRequestTypeDef,
+    ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef,
+    ListCoverageStatisticsRequestRequestTypeDef,
     ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef,
     ListFindingAggregationsRequestRequestTypeDef,
     FilterTypeDef,
     GetFindingsReportStatusResponseTypeDef,
     CreateFilterRequestRequestTypeDef,
     CreateFindingsReportRequestRequestTypeDef,
+    FilterCriteriaUnionTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFilterRequestRequestTypeDef,
     ListCoverageResponseTypeDef,
     FindingTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> SeverityCountsTypeDef:
+def get_value() -> SeverityCountsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-inspector2-1.28.16/README.md` & `mypy-boto3-inspector2-1.28.16.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
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
 [mypy-boto3-inspector2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/).
 
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
@@ -379,20 +379,20 @@
 )
 
 
 def check_value(value: AccountSortByType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_inspector2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_inspector2.type_defs import (
     SeverityCountsTypeDef,
     AccountAggregationTypeDef,
     StateTypeDef,
     ResourceStatusTypeDef,
@@ -419,25 +419,24 @@
     CancelFindingsReportRequestRequestTypeDef,
     CancelSbomExportRequestRequestTypeDef,
     CisaDataTypeDef,
     CodeFilePathTypeDef,
     CodeLineTypeDef,
     SuggestedFixTypeDef,
     CountsTypeDef,
-    CoverageDateFilterTypeDef,
+    TimestampTypeDef,
     CoverageMapFilterTypeDef,
     CoverageStringFilterTypeDef,
     ScanStatusTypeDef,
     DestinationTypeDef,
     Cvss2TypeDef,
     Cvss3TypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DateFilterOutputTypeDef,
-    DateFilterTypeDef,
     DelegatedAdminAccountTypeDef,
     DelegatedAdminTypeDef,
     DeleteFilterRequestRequestTypeDef,
     DisableDelegatedAdminAccountRequestRequestTypeDef,
     DisableRequestRequestTypeDef,
     DisassociateMemberRequestRequestTypeDef,
     MapFilterTypeDef,
@@ -527,15 +526,16 @@
     AwsLambdaFunctionDetailsTypeDef,
     BatchGetMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef,
     CodeVulnerabilityDetailsTypeDef,
     CodeSnippetResultTypeDef,
     ListCoverageStatisticsResponseTypeDef,
-    CoverageFilterCriteriaTypeDef,
+    CoverageDateFilterTypeDef,
+    DateFilterTypeDef,
     CvssScoreDetailsTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     Ec2InstanceAggregationTypeDef,
     LambdaFunctionAggregationTypeDef,
     EcrConfigurationStateTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
@@ -562,51 +562,54 @@
     UsageTotalTypeDef,
     AggregationResponseTypeDef,
     AccountStateTypeDef,
     DisableResponseTypeDef,
     EnableResponseTypeDef,
     ResourceDetailsTypeDef,
     BatchGetCodeSnippetResponseTypeDef,
-    ListCoverageRequestListCoveragePaginateTypeDef,
-    ListCoverageRequestRequestTypeDef,
-    ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef,
-    ListCoverageStatisticsRequestRequestTypeDef,
+    CoverageFilterCriteriaTypeDef,
     InspectorScoreDetailsTypeDef,
     AggregationRequestTypeDef,
     GetConfigurationResponseTypeDef,
     BatchGetFindingDetailsResponseTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
     FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     BatchGetFreeTrialInfoResponseTypeDef,
     CoveredResourceTypeDef,
     NetworkReachabilityDetailsTypeDef,
     GetSbomExportResponseTypeDef,
     CreateSbomExportRequestRequestTypeDef,
+    ResourceFilterCriteriaUnionTypeDef,
     ListUsageTotalsResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     BatchGetAccountStatusResponseTypeDef,
     ResourceTypeDef,
+    ListCoverageRequestListCoveragePaginateTypeDef,
+    ListCoverageRequestRequestTypeDef,
+    ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef,
+    ListCoverageStatisticsRequestRequestTypeDef,
     ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef,
     ListFindingAggregationsRequestRequestTypeDef,
     FilterTypeDef,
     GetFindingsReportStatusResponseTypeDef,
     CreateFilterRequestRequestTypeDef,
     CreateFindingsReportRequestRequestTypeDef,
+    FilterCriteriaUnionTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFilterRequestRequestTypeDef,
     ListCoverageResponseTypeDef,
     FindingTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> SeverityCountsTypeDef:
+def get_value() -> SeverityCountsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/__init__.py` & `mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/__init__.pyi` & `mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/__main__.py` & `mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Inspector2 1.28.16\nVersion:         1.28.16\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.Inspector2 1.28.16\nVersion:         1.28.16.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.16.post1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/client.py` & `mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_inspector2.client import Inspector2Client
 
     session = Session()
     client: Inspector2Client = session.client("inspector2")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AggregationTypeType,
     FilterActionType,
     GroupKeyType,
@@ -62,16 +62,15 @@
     DestinationTypeDef,
     DisableDelegatedAdminAccountResponseTypeDef,
     DisableResponseTypeDef,
     DisassociateMemberResponseTypeDef,
     EcrConfigurationTypeDef,
     EnableDelegatedAdminAccountResponseTypeDef,
     EnableResponseTypeDef,
-    FilterCriteriaOutputTypeDef,
-    FilterCriteriaTypeDef,
+    FilterCriteriaUnionTypeDef,
     GetConfigurationResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     GetEc2DeepInspectionConfigurationResponseTypeDef,
     GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusResponseTypeDef,
     GetMemberResponseTypeDef,
     GetSbomExportResponseTypeDef,
@@ -82,16 +81,15 @@
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsageTotalsResponseTypeDef,
     MemberAccountEc2DeepInspectionStatusTypeDef,
-    ResourceFilterCriteriaOutputTypeDef,
-    ResourceFilterCriteriaTypeDef,
+    ResourceFilterCriteriaUnionTypeDef,
     SearchVulnerabilitiesFilterCriteriaTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
     SortCriteriaTypeDef,
     StringFilterTypeDef,
     UpdateEc2DeepInspectionConfigurationResponseTypeDef,
     UpdateFilterResponseTypeDef,
     UpdateOrganizationConfigurationResponseTypeDef,
@@ -248,15 +246,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#close)
         """
 
     def create_filter(
         self,
         *,
         action: FilterActionType,
-        filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef],
+        filterCriteria: FilterCriteriaUnionTypeDef,
         name: str,
         description: str = ...,
         reason: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFilterResponseTypeDef:
         """
         Creates a filter resource using specified filter criteria.
@@ -266,31 +264,29 @@
         """
 
     def create_findings_report(
         self,
         *,
         reportFormat: ReportFormatType,
         s3Destination: DestinationTypeDef,
-        filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...
+        filterCriteria: FilterCriteriaUnionTypeDef = ...
     ) -> CreateFindingsReportResponseTypeDef:
         """
         Creates a finding report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_findings_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_findings_report)
         """
 
     def create_sbom_export(
         self,
         *,
         reportFormat: SbomReportFormatType,
         s3Destination: DestinationTypeDef,
-        resourceFilterCriteria: Union[
-            ResourceFilterCriteriaTypeDef, ResourceFilterCriteriaOutputTypeDef
-        ] = ...
+        resourceFilterCriteria: ResourceFilterCriteriaUnionTypeDef = ...
     ) -> CreateSbomExportResponseTypeDef:
         """
         Creates a software bill of materials (SBOM) report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_sbom_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_sbom_export)
         """
@@ -527,15 +523,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_finding_aggregations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_finding_aggregations)
         """
 
     def list_findings(
         self,
         *,
-        filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
+        filterCriteria: FilterCriteriaUnionTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortCriteria: SortCriteriaTypeDef = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Lists findings for your environment.
 
@@ -639,15 +635,15 @@
 
     def update_filter(
         self,
         *,
         filterArn: str,
         action: FilterActionType = ...,
         description: str = ...,
-        filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
+        filterCriteria: FilterCriteriaUnionTypeDef = ...,
         name: str = ...,
         reason: str = ...
     ) -> UpdateFilterResponseTypeDef:
         """
         Specifies the action that is to be applied to the findings that match the
         filter.
```

### Comparing `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/client.pyi` & `mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_inspector2.client import Inspector2Client
 
     session = Session()
     client: Inspector2Client = session.client("inspector2")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AggregationTypeType,
     FilterActionType,
     GroupKeyType,
@@ -62,16 +62,15 @@
     DestinationTypeDef,
     DisableDelegatedAdminAccountResponseTypeDef,
     DisableResponseTypeDef,
     DisassociateMemberResponseTypeDef,
     EcrConfigurationTypeDef,
     EnableDelegatedAdminAccountResponseTypeDef,
     EnableResponseTypeDef,
-    FilterCriteriaOutputTypeDef,
-    FilterCriteriaTypeDef,
+    FilterCriteriaUnionTypeDef,
     GetConfigurationResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     GetEc2DeepInspectionConfigurationResponseTypeDef,
     GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusResponseTypeDef,
     GetMemberResponseTypeDef,
     GetSbomExportResponseTypeDef,
@@ -82,16 +81,15 @@
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsageTotalsResponseTypeDef,
     MemberAccountEc2DeepInspectionStatusTypeDef,
-    ResourceFilterCriteriaOutputTypeDef,
-    ResourceFilterCriteriaTypeDef,
+    ResourceFilterCriteriaUnionTypeDef,
     SearchVulnerabilitiesFilterCriteriaTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
     SortCriteriaTypeDef,
     StringFilterTypeDef,
     UpdateEc2DeepInspectionConfigurationResponseTypeDef,
     UpdateFilterResponseTypeDef,
     UpdateOrganizationConfigurationResponseTypeDef,
@@ -232,15 +230,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#close)
         """
     def create_filter(
         self,
         *,
         action: FilterActionType,
-        filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef],
+        filterCriteria: FilterCriteriaUnionTypeDef,
         name: str,
         description: str = ...,
         reason: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFilterResponseTypeDef:
         """
         Creates a filter resource using specified filter criteria.
@@ -249,30 +247,28 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_filter)
         """
     def create_findings_report(
         self,
         *,
         reportFormat: ReportFormatType,
         s3Destination: DestinationTypeDef,
-        filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...
+        filterCriteria: FilterCriteriaUnionTypeDef = ...
     ) -> CreateFindingsReportResponseTypeDef:
         """
         Creates a finding report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_findings_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_findings_report)
         """
     def create_sbom_export(
         self,
         *,
         reportFormat: SbomReportFormatType,
         s3Destination: DestinationTypeDef,
-        resourceFilterCriteria: Union[
-            ResourceFilterCriteriaTypeDef, ResourceFilterCriteriaOutputTypeDef
-        ] = ...
+        resourceFilterCriteria: ResourceFilterCriteriaUnionTypeDef = ...
     ) -> CreateSbomExportResponseTypeDef:
         """
         Creates a software bill of materials (SBOM) report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_sbom_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_sbom_export)
         """
@@ -487,15 +483,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_finding_aggregations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_finding_aggregations)
         """
     def list_findings(
         self,
         *,
-        filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
+        filterCriteria: FilterCriteriaUnionTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortCriteria: SortCriteriaTypeDef = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Lists findings for your environment.
 
@@ -588,15 +584,15 @@
         """
     def update_filter(
         self,
         *,
         filterArn: str,
         action: FilterActionType = ...,
         description: str = ...,
-        filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
+        filterCriteria: FilterCriteriaUnionTypeDef = ...,
         name: str = ...,
         reason: str = ...
     ) -> UpdateFilterResponseTypeDef:
         """
         Specifies the action that is to be applied to the findings that match the
         filter.
```

### Comparing `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/literals.py` & `mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/literals.pyi` & `mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/paginator.py` & `mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,24 +33,23 @@
     list_finding_aggregations_paginator: ListFindingAggregationsPaginator = client.get_paginator("list_finding_aggregations")
     list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_usage_totals_paginator: ListUsageTotalsPaginator = client.get_paginator("list_usage_totals")
     search_vulnerabilities_paginator: SearchVulnerabilitiesPaginator = client.get_paginator("search_vulnerabilities")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import AggregationTypeType, FilterActionType, GroupKeyType, ServiceType
 from .type_defs import (
     AggregationRequestTypeDef,
     CoverageFilterCriteriaTypeDef,
-    FilterCriteriaOutputTypeDef,
-    FilterCriteriaTypeDef,
+    FilterCriteriaUnionTypeDef,
     ListAccountPermissionsResponseTypeDef,
     ListCoverageResponseTypeDef,
     ListCoverageStatisticsResponseTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
@@ -198,15 +197,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
+        filterCriteria: FilterCriteriaUnionTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfindingspaginator)
         """
```

### Comparing `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/paginator.pyi` & `mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -33,24 +33,23 @@
     list_finding_aggregations_paginator: ListFindingAggregationsPaginator = client.get_paginator("list_finding_aggregations")
     list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_usage_totals_paginator: ListUsageTotalsPaginator = client.get_paginator("list_usage_totals")
     search_vulnerabilities_paginator: SearchVulnerabilitiesPaginator = client.get_paginator("search_vulnerabilities")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import AggregationTypeType, FilterActionType, GroupKeyType, ServiceType
 from .type_defs import (
     AggregationRequestTypeDef,
     CoverageFilterCriteriaTypeDef,
-    FilterCriteriaOutputTypeDef,
-    FilterCriteriaTypeDef,
+    FilterCriteriaUnionTypeDef,
     ListAccountPermissionsResponseTypeDef,
     ListCoverageResponseTypeDef,
     ListCoverageStatisticsResponseTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
@@ -189,15 +188,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        filterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
+        filterCriteria: FilterCriteriaUnionTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfindingspaginator)
         """
```

### Comparing `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/type_defs.py` & `mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_inspector2.type_defs import SeverityCountsTypeDef
 
-    data: SeverityCountsTypeDef = {...}
+    data: SeverityCountsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -114,25 +114,24 @@
     "CancelFindingsReportRequestRequestTypeDef",
     "CancelSbomExportRequestRequestTypeDef",
     "CisaDataTypeDef",
     "CodeFilePathTypeDef",
     "CodeLineTypeDef",
     "SuggestedFixTypeDef",
     "CountsTypeDef",
-    "CoverageDateFilterTypeDef",
+    "TimestampTypeDef",
     "CoverageMapFilterTypeDef",
     "CoverageStringFilterTypeDef",
     "ScanStatusTypeDef",
     "DestinationTypeDef",
     "Cvss2TypeDef",
     "Cvss3TypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
     "DateFilterOutputTypeDef",
-    "DateFilterTypeDef",
     "DelegatedAdminAccountTypeDef",
     "DelegatedAdminTypeDef",
     "DeleteFilterRequestRequestTypeDef",
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
     "DisableRequestRequestTypeDef",
     "DisassociateMemberRequestRequestTypeDef",
     "MapFilterTypeDef",
@@ -222,15 +221,16 @@
     "AwsLambdaFunctionDetailsTypeDef",
     "BatchGetMemberEc2DeepInspectionStatusResponseTypeDef",
     "BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef",
     "BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef",
     "CodeVulnerabilityDetailsTypeDef",
     "CodeSnippetResultTypeDef",
     "ListCoverageStatisticsResponseTypeDef",
-    "CoverageFilterCriteriaTypeDef",
+    "CoverageDateFilterTypeDef",
+    "DateFilterTypeDef",
     "CvssScoreDetailsTypeDef",
     "ListDelegatedAdminAccountsResponseTypeDef",
     "GetDelegatedAdminAccountResponseTypeDef",
     "Ec2InstanceAggregationTypeDef",
     "LambdaFunctionAggregationTypeDef",
     "EcrConfigurationStateTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
@@ -257,40 +257,43 @@
     "UsageTotalTypeDef",
     "AggregationResponseTypeDef",
     "AccountStateTypeDef",
     "DisableResponseTypeDef",
     "EnableResponseTypeDef",
     "ResourceDetailsTypeDef",
     "BatchGetCodeSnippetResponseTypeDef",
-    "ListCoverageRequestListCoveragePaginateTypeDef",
-    "ListCoverageRequestRequestTypeDef",
-    "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
-    "ListCoverageStatisticsRequestRequestTypeDef",
+    "CoverageFilterCriteriaTypeDef",
     "InspectorScoreDetailsTypeDef",
     "AggregationRequestTypeDef",
     "GetConfigurationResponseTypeDef",
     "BatchGetFindingDetailsResponseTypeDef",
     "SearchVulnerabilitiesResponseTypeDef",
     "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "BatchGetFreeTrialInfoResponseTypeDef",
     "CoveredResourceTypeDef",
     "NetworkReachabilityDetailsTypeDef",
     "GetSbomExportResponseTypeDef",
     "CreateSbomExportRequestRequestTypeDef",
+    "ResourceFilterCriteriaUnionTypeDef",
     "ListUsageTotalsResponseTypeDef",
     "ListFindingAggregationsResponseTypeDef",
     "BatchGetAccountStatusResponseTypeDef",
     "ResourceTypeDef",
+    "ListCoverageRequestListCoveragePaginateTypeDef",
+    "ListCoverageRequestRequestTypeDef",
+    "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
+    "ListCoverageStatisticsRequestRequestTypeDef",
     "ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     "ListFindingAggregationsRequestRequestTypeDef",
     "FilterTypeDef",
     "GetFindingsReportStatusResponseTypeDef",
     "CreateFilterRequestRequestTypeDef",
     "CreateFindingsReportRequestRequestTypeDef",
+    "FilterCriteriaUnionTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFilterRequestRequestTypeDef",
     "ListCoverageResponseTypeDef",
     "FindingTypeDef",
     "ListFiltersResponseTypeDef",
     "ListFindingsResponseTypeDef",
@@ -645,23 +648,15 @@
     {
         "count": int,
         "groupKey": GroupKeyType,
     },
     total=False,
 )
 
-CoverageDateFilterTypeDef = TypedDict(
-    "CoverageDateFilterTypeDef",
-    {
-        "endInclusive": Union[datetime, str],
-        "startInclusive": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredCoverageMapFilterTypeDef = TypedDict(
     "_RequiredCoverageMapFilterTypeDef",
     {
         "comparison": Literal["EQUALS"],
         "key": str,
     },
 )
@@ -757,23 +752,14 @@
     {
         "endInclusive": datetime,
         "startInclusive": datetime,
     },
     total=False,
 )
 
-DateFilterTypeDef = TypedDict(
-    "DateFilterTypeDef",
-    {
-        "endInclusive": Union[datetime, str],
-        "startInclusive": Union[datetime, str],
-    },
-    total=False,
-)
-
 DelegatedAdminAccountTypeDef = TypedDict(
     "DelegatedAdminAccountTypeDef",
     {
         "accountId": str,
         "status": DelegatedAdminStatusType,
     },
     total=False,
@@ -1903,30 +1889,28 @@
         "countsByGroup": List[CountsTypeDef],
         "nextToken": str,
         "totalCounts": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CoverageFilterCriteriaTypeDef = TypedDict(
-    "CoverageFilterCriteriaTypeDef",
+CoverageDateFilterTypeDef = TypedDict(
+    "CoverageDateFilterTypeDef",
     {
-        "accountId": Sequence[CoverageStringFilterTypeDef],
-        "ec2InstanceTags": Sequence[CoverageMapFilterTypeDef],
-        "ecrImageTags": Sequence[CoverageStringFilterTypeDef],
-        "ecrRepositoryName": Sequence[CoverageStringFilterTypeDef],
-        "lambdaFunctionName": Sequence[CoverageStringFilterTypeDef],
-        "lambdaFunctionRuntime": Sequence[CoverageStringFilterTypeDef],
-        "lambdaFunctionTags": Sequence[CoverageMapFilterTypeDef],
-        "lastScannedAt": Sequence[CoverageDateFilterTypeDef],
-        "resourceId": Sequence[CoverageStringFilterTypeDef],
-        "resourceType": Sequence[CoverageStringFilterTypeDef],
-        "scanStatusCode": Sequence[CoverageStringFilterTypeDef],
-        "scanStatusReason": Sequence[CoverageStringFilterTypeDef],
-        "scanType": Sequence[CoverageStringFilterTypeDef],
+        "endInclusive": TimestampTypeDef,
+        "startInclusive": TimestampTypeDef,
+    },
+    total=False,
+)
+
+DateFilterTypeDef = TypedDict(
+    "DateFilterTypeDef",
+    {
+        "endInclusive": TimestampTypeDef,
+        "startInclusive": TimestampTypeDef,
     },
     total=False,
 )
 
 _RequiredCvssScoreDetailsTypeDef = TypedDict(
     "_RequiredCvssScoreDetailsTypeDef",
     {
@@ -2351,49 +2335,30 @@
     {
         "codeSnippetResults": List[CodeSnippetResultTypeDef],
         "errors": List[CodeSnippetErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListCoverageRequestListCoveragePaginateTypeDef = TypedDict(
-    "ListCoverageRequestListCoveragePaginateTypeDef",
-    {
-        "filterCriteria": CoverageFilterCriteriaTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCoverageRequestRequestTypeDef = TypedDict(
-    "ListCoverageRequestRequestTypeDef",
-    {
-        "filterCriteria": CoverageFilterCriteriaTypeDef,
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef = TypedDict(
-    "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
-    {
-        "filterCriteria": CoverageFilterCriteriaTypeDef,
-        "groupBy": GroupKeyType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCoverageStatisticsRequestRequestTypeDef = TypedDict(
-    "ListCoverageStatisticsRequestRequestTypeDef",
+CoverageFilterCriteriaTypeDef = TypedDict(
+    "CoverageFilterCriteriaTypeDef",
     {
-        "filterCriteria": CoverageFilterCriteriaTypeDef,
-        "groupBy": GroupKeyType,
-        "nextToken": str,
+        "accountId": Sequence[CoverageStringFilterTypeDef],
+        "ec2InstanceTags": Sequence[CoverageMapFilterTypeDef],
+        "ecrImageTags": Sequence[CoverageStringFilterTypeDef],
+        "ecrRepositoryName": Sequence[CoverageStringFilterTypeDef],
+        "lambdaFunctionName": Sequence[CoverageStringFilterTypeDef],
+        "lambdaFunctionRuntime": Sequence[CoverageStringFilterTypeDef],
+        "lambdaFunctionTags": Sequence[CoverageMapFilterTypeDef],
+        "lastScannedAt": Sequence[CoverageDateFilterTypeDef],
+        "resourceId": Sequence[CoverageStringFilterTypeDef],
+        "resourceType": Sequence[CoverageStringFilterTypeDef],
+        "scanStatusCode": Sequence[CoverageStringFilterTypeDef],
+        "scanStatusReason": Sequence[CoverageStringFilterTypeDef],
+        "scanType": Sequence[CoverageStringFilterTypeDef],
     },
     total=False,
 )
 
 InspectorScoreDetailsTypeDef = TypedDict(
     "InspectorScoreDetailsTypeDef",
     {
@@ -2618,14 +2583,17 @@
 
 class CreateSbomExportRequestRequestTypeDef(
     _RequiredCreateSbomExportRequestRequestTypeDef, _OptionalCreateSbomExportRequestRequestTypeDef
 ):
     pass
 
 
+ResourceFilterCriteriaUnionTypeDef = Union[
+    ResourceFilterCriteriaTypeDef, ResourceFilterCriteriaOutputTypeDef
+]
 ListUsageTotalsResponseTypeDef = TypedDict(
     "ListUsageTotalsResponseTypeDef",
     {
         "nextToken": str,
         "totals": List[UsageTotalTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2669,14 +2637,53 @@
 )
 
 
 class ResourceTypeDef(_RequiredResourceTypeDef, _OptionalResourceTypeDef):
     pass
 
 
+ListCoverageRequestListCoveragePaginateTypeDef = TypedDict(
+    "ListCoverageRequestListCoveragePaginateTypeDef",
+    {
+        "filterCriteria": CoverageFilterCriteriaTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCoverageRequestRequestTypeDef = TypedDict(
+    "ListCoverageRequestRequestTypeDef",
+    {
+        "filterCriteria": CoverageFilterCriteriaTypeDef,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef = TypedDict(
+    "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
+    {
+        "filterCriteria": CoverageFilterCriteriaTypeDef,
+        "groupBy": GroupKeyType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCoverageStatisticsRequestRequestTypeDef = TypedDict(
+    "ListCoverageStatisticsRequestRequestTypeDef",
+    {
+        "filterCriteria": CoverageFilterCriteriaTypeDef,
+        "groupBy": GroupKeyType,
+        "nextToken": str,
+    },
+    total=False,
+)
+
 _RequiredListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef = TypedDict(
     "_RequiredListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     {
         "aggregationType": AggregationTypeType,
     },
 )
 _OptionalListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef = TypedDict(
@@ -2806,14 +2813,15 @@
 class CreateFindingsReportRequestRequestTypeDef(
     _RequiredCreateFindingsReportRequestRequestTypeDef,
     _OptionalCreateFindingsReportRequestRequestTypeDef,
 ):
     pass
 
 
+FilterCriteriaUnionTypeDef = Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef]
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "filterCriteria": FilterCriteriaTypeDef,
         "sortCriteria": SortCriteriaTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
```

### Comparing `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2/type_defs.pyi` & `mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_inspector2.type_defs import SeverityCountsTypeDef
 
-    data: SeverityCountsTypeDef = {...}
+    data: SeverityCountsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -113,25 +113,24 @@
     "CancelFindingsReportRequestRequestTypeDef",
     "CancelSbomExportRequestRequestTypeDef",
     "CisaDataTypeDef",
     "CodeFilePathTypeDef",
     "CodeLineTypeDef",
     "SuggestedFixTypeDef",
     "CountsTypeDef",
-    "CoverageDateFilterTypeDef",
+    "TimestampTypeDef",
     "CoverageMapFilterTypeDef",
     "CoverageStringFilterTypeDef",
     "ScanStatusTypeDef",
     "DestinationTypeDef",
     "Cvss2TypeDef",
     "Cvss3TypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
     "DateFilterOutputTypeDef",
-    "DateFilterTypeDef",
     "DelegatedAdminAccountTypeDef",
     "DelegatedAdminTypeDef",
     "DeleteFilterRequestRequestTypeDef",
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
     "DisableRequestRequestTypeDef",
     "DisassociateMemberRequestRequestTypeDef",
     "MapFilterTypeDef",
@@ -221,15 +220,16 @@
     "AwsLambdaFunctionDetailsTypeDef",
     "BatchGetMemberEc2DeepInspectionStatusResponseTypeDef",
     "BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef",
     "BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef",
     "CodeVulnerabilityDetailsTypeDef",
     "CodeSnippetResultTypeDef",
     "ListCoverageStatisticsResponseTypeDef",
-    "CoverageFilterCriteriaTypeDef",
+    "CoverageDateFilterTypeDef",
+    "DateFilterTypeDef",
     "CvssScoreDetailsTypeDef",
     "ListDelegatedAdminAccountsResponseTypeDef",
     "GetDelegatedAdminAccountResponseTypeDef",
     "Ec2InstanceAggregationTypeDef",
     "LambdaFunctionAggregationTypeDef",
     "EcrConfigurationStateTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
@@ -256,40 +256,43 @@
     "UsageTotalTypeDef",
     "AggregationResponseTypeDef",
     "AccountStateTypeDef",
     "DisableResponseTypeDef",
     "EnableResponseTypeDef",
     "ResourceDetailsTypeDef",
     "BatchGetCodeSnippetResponseTypeDef",
-    "ListCoverageRequestListCoveragePaginateTypeDef",
-    "ListCoverageRequestRequestTypeDef",
-    "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
-    "ListCoverageStatisticsRequestRequestTypeDef",
+    "CoverageFilterCriteriaTypeDef",
     "InspectorScoreDetailsTypeDef",
     "AggregationRequestTypeDef",
     "GetConfigurationResponseTypeDef",
     "BatchGetFindingDetailsResponseTypeDef",
     "SearchVulnerabilitiesResponseTypeDef",
     "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "BatchGetFreeTrialInfoResponseTypeDef",
     "CoveredResourceTypeDef",
     "NetworkReachabilityDetailsTypeDef",
     "GetSbomExportResponseTypeDef",
     "CreateSbomExportRequestRequestTypeDef",
+    "ResourceFilterCriteriaUnionTypeDef",
     "ListUsageTotalsResponseTypeDef",
     "ListFindingAggregationsResponseTypeDef",
     "BatchGetAccountStatusResponseTypeDef",
     "ResourceTypeDef",
+    "ListCoverageRequestListCoveragePaginateTypeDef",
+    "ListCoverageRequestRequestTypeDef",
+    "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
+    "ListCoverageStatisticsRequestRequestTypeDef",
     "ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     "ListFindingAggregationsRequestRequestTypeDef",
     "FilterTypeDef",
     "GetFindingsReportStatusResponseTypeDef",
     "CreateFilterRequestRequestTypeDef",
     "CreateFindingsReportRequestRequestTypeDef",
+    "FilterCriteriaUnionTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFilterRequestRequestTypeDef",
     "ListCoverageResponseTypeDef",
     "FindingTypeDef",
     "ListFiltersResponseTypeDef",
     "ListFindingsResponseTypeDef",
@@ -634,23 +637,15 @@
     {
         "count": int,
         "groupKey": GroupKeyType,
     },
     total=False,
 )
 
-CoverageDateFilterTypeDef = TypedDict(
-    "CoverageDateFilterTypeDef",
-    {
-        "endInclusive": Union[datetime, str],
-        "startInclusive": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredCoverageMapFilterTypeDef = TypedDict(
     "_RequiredCoverageMapFilterTypeDef",
     {
         "comparison": Literal["EQUALS"],
         "key": str,
     },
 )
@@ -742,23 +737,14 @@
     {
         "endInclusive": datetime,
         "startInclusive": datetime,
     },
     total=False,
 )
 
-DateFilterTypeDef = TypedDict(
-    "DateFilterTypeDef",
-    {
-        "endInclusive": Union[datetime, str],
-        "startInclusive": Union[datetime, str],
-    },
-    total=False,
-)
-
 DelegatedAdminAccountTypeDef = TypedDict(
     "DelegatedAdminAccountTypeDef",
     {
         "accountId": str,
         "status": DelegatedAdminStatusType,
     },
     total=False,
@@ -1852,30 +1838,28 @@
         "countsByGroup": List[CountsTypeDef],
         "nextToken": str,
         "totalCounts": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CoverageFilterCriteriaTypeDef = TypedDict(
-    "CoverageFilterCriteriaTypeDef",
+CoverageDateFilterTypeDef = TypedDict(
+    "CoverageDateFilterTypeDef",
     {
-        "accountId": Sequence[CoverageStringFilterTypeDef],
-        "ec2InstanceTags": Sequence[CoverageMapFilterTypeDef],
-        "ecrImageTags": Sequence[CoverageStringFilterTypeDef],
-        "ecrRepositoryName": Sequence[CoverageStringFilterTypeDef],
-        "lambdaFunctionName": Sequence[CoverageStringFilterTypeDef],
-        "lambdaFunctionRuntime": Sequence[CoverageStringFilterTypeDef],
-        "lambdaFunctionTags": Sequence[CoverageMapFilterTypeDef],
-        "lastScannedAt": Sequence[CoverageDateFilterTypeDef],
-        "resourceId": Sequence[CoverageStringFilterTypeDef],
-        "resourceType": Sequence[CoverageStringFilterTypeDef],
-        "scanStatusCode": Sequence[CoverageStringFilterTypeDef],
-        "scanStatusReason": Sequence[CoverageStringFilterTypeDef],
-        "scanType": Sequence[CoverageStringFilterTypeDef],
+        "endInclusive": TimestampTypeDef,
+        "startInclusive": TimestampTypeDef,
+    },
+    total=False,
+)
+
+DateFilterTypeDef = TypedDict(
+    "DateFilterTypeDef",
+    {
+        "endInclusive": TimestampTypeDef,
+        "startInclusive": TimestampTypeDef,
     },
     total=False,
 )
 
 _RequiredCvssScoreDetailsTypeDef = TypedDict(
     "_RequiredCvssScoreDetailsTypeDef",
     {
@@ -2290,49 +2274,30 @@
     {
         "codeSnippetResults": List[CodeSnippetResultTypeDef],
         "errors": List[CodeSnippetErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListCoverageRequestListCoveragePaginateTypeDef = TypedDict(
-    "ListCoverageRequestListCoveragePaginateTypeDef",
-    {
-        "filterCriteria": CoverageFilterCriteriaTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCoverageRequestRequestTypeDef = TypedDict(
-    "ListCoverageRequestRequestTypeDef",
-    {
-        "filterCriteria": CoverageFilterCriteriaTypeDef,
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef = TypedDict(
-    "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
-    {
-        "filterCriteria": CoverageFilterCriteriaTypeDef,
-        "groupBy": GroupKeyType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCoverageStatisticsRequestRequestTypeDef = TypedDict(
-    "ListCoverageStatisticsRequestRequestTypeDef",
+CoverageFilterCriteriaTypeDef = TypedDict(
+    "CoverageFilterCriteriaTypeDef",
     {
-        "filterCriteria": CoverageFilterCriteriaTypeDef,
-        "groupBy": GroupKeyType,
-        "nextToken": str,
+        "accountId": Sequence[CoverageStringFilterTypeDef],
+        "ec2InstanceTags": Sequence[CoverageMapFilterTypeDef],
+        "ecrImageTags": Sequence[CoverageStringFilterTypeDef],
+        "ecrRepositoryName": Sequence[CoverageStringFilterTypeDef],
+        "lambdaFunctionName": Sequence[CoverageStringFilterTypeDef],
+        "lambdaFunctionRuntime": Sequence[CoverageStringFilterTypeDef],
+        "lambdaFunctionTags": Sequence[CoverageMapFilterTypeDef],
+        "lastScannedAt": Sequence[CoverageDateFilterTypeDef],
+        "resourceId": Sequence[CoverageStringFilterTypeDef],
+        "resourceType": Sequence[CoverageStringFilterTypeDef],
+        "scanStatusCode": Sequence[CoverageStringFilterTypeDef],
+        "scanStatusReason": Sequence[CoverageStringFilterTypeDef],
+        "scanType": Sequence[CoverageStringFilterTypeDef],
     },
     total=False,
 )
 
 InspectorScoreDetailsTypeDef = TypedDict(
     "InspectorScoreDetailsTypeDef",
     {
@@ -2553,14 +2518,17 @@
 )
 
 class CreateSbomExportRequestRequestTypeDef(
     _RequiredCreateSbomExportRequestRequestTypeDef, _OptionalCreateSbomExportRequestRequestTypeDef
 ):
     pass
 
+ResourceFilterCriteriaUnionTypeDef = Union[
+    ResourceFilterCriteriaTypeDef, ResourceFilterCriteriaOutputTypeDef
+]
 ListUsageTotalsResponseTypeDef = TypedDict(
     "ListUsageTotalsResponseTypeDef",
     {
         "nextToken": str,
         "totals": List[UsageTotalTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2602,14 +2570,53 @@
     },
     total=False,
 )
 
 class ResourceTypeDef(_RequiredResourceTypeDef, _OptionalResourceTypeDef):
     pass
 
+ListCoverageRequestListCoveragePaginateTypeDef = TypedDict(
+    "ListCoverageRequestListCoveragePaginateTypeDef",
+    {
+        "filterCriteria": CoverageFilterCriteriaTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCoverageRequestRequestTypeDef = TypedDict(
+    "ListCoverageRequestRequestTypeDef",
+    {
+        "filterCriteria": CoverageFilterCriteriaTypeDef,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef = TypedDict(
+    "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
+    {
+        "filterCriteria": CoverageFilterCriteriaTypeDef,
+        "groupBy": GroupKeyType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCoverageStatisticsRequestRequestTypeDef = TypedDict(
+    "ListCoverageStatisticsRequestRequestTypeDef",
+    {
+        "filterCriteria": CoverageFilterCriteriaTypeDef,
+        "groupBy": GroupKeyType,
+        "nextToken": str,
+    },
+    total=False,
+)
+
 _RequiredListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef = TypedDict(
     "_RequiredListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     {
         "aggregationType": AggregationTypeType,
     },
 )
 _OptionalListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef = TypedDict(
@@ -2729,14 +2736,15 @@
 
 class CreateFindingsReportRequestRequestTypeDef(
     _RequiredCreateFindingsReportRequestRequestTypeDef,
     _OptionalCreateFindingsReportRequestRequestTypeDef,
 ):
     pass
 
+FilterCriteriaUnionTypeDef = Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef]
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "filterCriteria": FilterCriteriaTypeDef,
         "sortCriteria": SortCriteriaTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
```

### Comparing `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2.egg-info/PKG-INFO` & `mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector2
-Version: 1.28.16
-Summary: Type annotations for boto3.Inspector2 1.28.16 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16.post1
+Summary: Type annotations for boto3.Inspector2 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 inspector2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 inspector2 type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -47,15 +47,15 @@
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
 [mypy-boto3-inspector2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/).
 
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
@@ -411,20 +411,20 @@
 )
 
 
 def check_value(value: AccountSortByType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_inspector2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_inspector2.type_defs import (
     SeverityCountsTypeDef,
     AccountAggregationTypeDef,
     StateTypeDef,
     ResourceStatusTypeDef,
@@ -451,25 +451,24 @@
     CancelFindingsReportRequestRequestTypeDef,
     CancelSbomExportRequestRequestTypeDef,
     CisaDataTypeDef,
     CodeFilePathTypeDef,
     CodeLineTypeDef,
     SuggestedFixTypeDef,
     CountsTypeDef,
-    CoverageDateFilterTypeDef,
+    TimestampTypeDef,
     CoverageMapFilterTypeDef,
     CoverageStringFilterTypeDef,
     ScanStatusTypeDef,
     DestinationTypeDef,
     Cvss2TypeDef,
     Cvss3TypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DateFilterOutputTypeDef,
-    DateFilterTypeDef,
     DelegatedAdminAccountTypeDef,
     DelegatedAdminTypeDef,
     DeleteFilterRequestRequestTypeDef,
     DisableDelegatedAdminAccountRequestRequestTypeDef,
     DisableRequestRequestTypeDef,
     DisassociateMemberRequestRequestTypeDef,
     MapFilterTypeDef,
@@ -559,15 +558,16 @@
     AwsLambdaFunctionDetailsTypeDef,
     BatchGetMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef,
     CodeVulnerabilityDetailsTypeDef,
     CodeSnippetResultTypeDef,
     ListCoverageStatisticsResponseTypeDef,
-    CoverageFilterCriteriaTypeDef,
+    CoverageDateFilterTypeDef,
+    DateFilterTypeDef,
     CvssScoreDetailsTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     Ec2InstanceAggregationTypeDef,
     LambdaFunctionAggregationTypeDef,
     EcrConfigurationStateTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
@@ -594,51 +594,54 @@
     UsageTotalTypeDef,
     AggregationResponseTypeDef,
     AccountStateTypeDef,
     DisableResponseTypeDef,
     EnableResponseTypeDef,
     ResourceDetailsTypeDef,
     BatchGetCodeSnippetResponseTypeDef,
-    ListCoverageRequestListCoveragePaginateTypeDef,
-    ListCoverageRequestRequestTypeDef,
-    ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef,
-    ListCoverageStatisticsRequestRequestTypeDef,
+    CoverageFilterCriteriaTypeDef,
     InspectorScoreDetailsTypeDef,
     AggregationRequestTypeDef,
     GetConfigurationResponseTypeDef,
     BatchGetFindingDetailsResponseTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
     FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     BatchGetFreeTrialInfoResponseTypeDef,
     CoveredResourceTypeDef,
     NetworkReachabilityDetailsTypeDef,
     GetSbomExportResponseTypeDef,
     CreateSbomExportRequestRequestTypeDef,
+    ResourceFilterCriteriaUnionTypeDef,
     ListUsageTotalsResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     BatchGetAccountStatusResponseTypeDef,
     ResourceTypeDef,
+    ListCoverageRequestListCoveragePaginateTypeDef,
+    ListCoverageRequestRequestTypeDef,
+    ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef,
+    ListCoverageStatisticsRequestRequestTypeDef,
     ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef,
     ListFindingAggregationsRequestRequestTypeDef,
     FilterTypeDef,
     GetFindingsReportStatusResponseTypeDef,
     CreateFilterRequestRequestTypeDef,
     CreateFindingsReportRequestRequestTypeDef,
+    FilterCriteriaUnionTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFilterRequestRequestTypeDef,
     ListCoverageResponseTypeDef,
     FindingTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> SeverityCountsTypeDef:
+def get_value() -> SeverityCountsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-inspector2-1.28.16/mypy_boto3_inspector2.egg-info/SOURCES.txt` & `mypy-boto3-inspector2-1.28.16.post1/mypy_boto3_inspector2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.28.16/setup.py` & `mypy-boto3-inspector2-1.28.16.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-inspector2",
-    version="1.28.16",
+    version="1.28.16.post1",
     packages=["mypy_boto3_inspector2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Inspector2 1.28.16 service generated with mypy-boto3-builder"
-        " 7.16.2"
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
-    keywords="boto3 inspector2 type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 inspector2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_inspector2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

