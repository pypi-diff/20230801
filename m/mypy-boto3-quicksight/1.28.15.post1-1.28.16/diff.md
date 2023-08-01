# Comparing `tmp/mypy-boto3-quicksight-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-quicksight-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-quicksight-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:57 2023, max compression
+gzip compressed data, was "mypy-boto3-quicksight-1.28.16.tar", last modified: Tue Aug  1 11:37:37 2023, max compression
```

## Comparing `mypy-boto3-quicksight-1.28.15.post1.tar` & `mypy-boto3-quicksight-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:57.065351 mypy-boto3-quicksight-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:55:46.000000 mypy-boto3-quicksight-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    75936 2023-07-29 10:03:57.065351 mypy-boto3-quicksight-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    74431 2023-07-29 09:55:46.000000 mypy-boto3-quicksight-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:57.061351 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-29 09:55:46.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-29 09:55:46.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:55:46.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   127673 2023-07-29 09:55:47.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   127480 2023-07-29 09:55:47.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    36327 2023-07-29 09:55:49.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    36325 2023-07-29 09:55:48.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    29023 2023-07-29 09:55:48.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    28996 2023-07-29 09:55:48.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:55:46.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   552869 2023-07-29 09:56:12.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   552153 2023-07-29 09:56:01.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:55:46.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:57.065351 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    75936 2023-07-29 10:03:56.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 10:03:56.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:56.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:56.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:56.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:03:56.000000 mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:57.065351 mypy-boto3-quicksight-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 09:55:46.000000 mypy-boto3-quicksight-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:37.516778 mypy-boto3-quicksight-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:29:07.000000 mypy-boto3-quicksight-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    76704 2023-08-01 11:37:37.516778 mypy-boto3-quicksight-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    75208 2023-08-01 11:29:07.000000 mypy-boto3-quicksight-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:37.508778 mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-08-01 11:29:07.000000 mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-08-01 11:29:07.000000 mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 11:29:07.000000 mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   123884 2023-08-01 11:29:08.000000 mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   123691 2023-08-01 11:29:07.000000 mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    36327 2023-08-01 11:29:14.000000 mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36325 2023-08-01 11:29:14.000000 mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    29023 2023-08-01 11:29:13.000000 mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28996 2023-08-01 11:29:08.000000 mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:29:07.000000 mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   554054 2023-08-01 11:29:32.000000 mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   553338 2023-08-01 11:29:21.000000 mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:29:07.000000 mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:37.516778 mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    76704 2023-08-01 11:37:37.000000 mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-01 11:37:37.000000 mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:37.000000 mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:37.000000 mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:37.000000 mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 11:37:37.000000 mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:37.516778 mypy-boto3-quicksight-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-01 11:29:06.000000 mypy-boto3-quicksight-1.28.16/setup.py
```

### Comparing `mypy-boto3-quicksight-1.28.15.post1/LICENSE` & `mypy-boto3-quicksight-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.15.post1/PKG-INFO` & `mypy-boto3-quicksight-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-quicksight
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.QuickSight 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.QuickSight 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 quicksight type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 quicksight type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-quicksight.svg?color=blue)](https://pypi.org/project/mypy-boto3-quicksight)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-quicksight)](https://pepy.tech/project/mypy-boto3-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QuickSight 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[boto3.QuickSight 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
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
 [mypy-boto3-quicksight docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/).
 
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
@@ -594,20 +594,20 @@
 )
 
 
 def check_value(value: AnalysisErrorTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_quicksight.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_quicksight.type_defs import (
     AccountCustomizationTypeDef,
     AccountInfoTypeDef,
     AccountSettingsTypeDef,
     ActiveIAMPolicyAssignmentTypeDef,
@@ -654,19 +654,19 @@
     SslPropertiesTypeDef,
     VpcConnectionPropertiesTypeDef,
     AssetBundleImportJobErrorTypeDef,
     AssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef,
     AssetBundleImportJobResourceIdOverrideConfigurationTypeDef,
     AssetBundleImportJobThemeOverrideParametersTypeDef,
     AssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef,
-    AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef,
     AssetBundleImportJobVPCConnectionOverrideParametersTypeDef,
+    TimestampTypeDef,
     AssetBundleImportJobSummaryTypeDef,
     AssetBundleImportSourceDescriptionTypeDef,
-    AssetBundleImportSourceTypeDef,
+    BlobTypeDef,
     AthenaParametersTypeDef,
     AuroraParametersTypeDef,
     AuroraPostgreSqlParametersTypeDef,
     AwsIotAnalyticsParametersTypeDef,
     DateAxisOptionsTypeDef,
     AxisDisplayMinMaxRangeTypeDef,
     AxisLinearScaleTypeDef,
@@ -707,42 +707,36 @@
     ConditionalFormattingSolidColorTypeDef,
     ConditionalFormattingCustomIconOptionsTypeDef,
     ConditionalFormattingIconDisplayConfigurationTypeDef,
     ConditionalFormattingIconSetTypeDef,
     TagTypeDef,
     CreateAccountSubscriptionRequestRequestTypeDef,
     SignupResponseTypeDef,
-    ResourcePermissionOutputTypeDef,
-    ResourcePermissionTypeDef,
     DataSetUsageConfigurationTypeDef,
-    FieldFolderOutputTypeDef,
-    FieldFolderTypeDef,
     RowLevelPermissionDataSetTypeDef,
     CreateFolderMembershipRequestRequestTypeDef,
     FolderMemberTypeDef,
     CreateGroupMembershipRequestRequestTypeDef,
     GroupMemberTypeDef,
     CreateGroupRequestRequestTypeDef,
     GroupTypeDef,
     CreateIAMPolicyAssignmentRequestRequestTypeDef,
     CreateIngestionRequestRequestTypeDef,
     CreateTemplateAliasRequestRequestTypeDef,
     TemplateAliasTypeDef,
     CreateThemeAliasRequestRequestTypeDef,
     ThemeAliasTypeDef,
-    TopicRefreshScheduleTypeDef,
     DecimalPlacesConfigurationTypeDef,
     NegativeValueConfigurationTypeDef,
     NullValueFormatConfigurationTypeDef,
     LocalNavigationConfigurationTypeDef,
     CustomActionURLOperationTypeDef,
     CustomContentConfigurationTypeDef,
     CustomNarrativeOptionsTypeDef,
     CustomParameterValuesOutputTypeDef,
-    CustomParameterValuesTypeDef,
     InputColumnTypeDef,
     DataPointDrillUpDownOptionTypeDef,
     DataPointMenuLabelOptionTypeDef,
     DataPointTooltipOptionTypeDef,
     ExportToCSVOptionTypeDef,
     ExportWithHiddenFieldsOptionTypeDef,
     SheetControlsOptionTypeDef,
@@ -760,14 +754,15 @@
     DataPathLabelTypeTypeDef,
     FieldLabelTypeTypeDef,
     MaximumLabelTypeTypeDef,
     MinimumLabelTypeTypeDef,
     RangeEndsLabelTypeTypeDef,
     DataPathValueTypeDef,
     DataSetSearchFilterTypeDef,
+    FieldFolderOutputTypeDef,
     OutputColumnTypeDef,
     DataSourceErrorInfoTypeDef,
     DatabricksParametersTypeDef,
     ExasolParametersTypeDef,
     JiraParametersTypeDef,
     MariaDbParametersTypeDef,
     MySqlParametersTypeDef,
@@ -781,21 +776,18 @@
     SparkParametersTypeDef,
     SqlServerParametersTypeDef,
     TeradataParametersTypeDef,
     TwitterParametersTypeDef,
     DataSourceSearchFilterTypeDef,
     DataSourceSummaryTypeDef,
     DateTimeDatasetParameterDefaultValuesOutputTypeDef,
-    DateTimeDatasetParameterDefaultValuesTypeDef,
     RollingDateConfigurationTypeDef,
     DateTimeValueWhenUnsetConfigurationOutputTypeDef,
     MappedDataSetParameterTypeDef,
-    DateTimeValueWhenUnsetConfigurationTypeDef,
     DateTimeParameterOutputTypeDef,
-    DateTimeParameterTypeDef,
     SheetControlInfoIconLabelOptionsTypeDef,
     DecimalDatasetParameterDefaultValuesOutputTypeDef,
     DecimalDatasetParameterDefaultValuesTypeDef,
     DecimalValueWhenUnsetConfigurationTypeDef,
     DecimalParameterOutputTypeDef,
     DecimalParameterTypeDef,
     DeleteAccountCustomizationRequestRequestTypeDef,
@@ -822,14 +814,15 @@
     DeleteUserRequestRequestTypeDef,
     DeleteVPCConnectionRequestRequestTypeDef,
     DescribeAccountCustomizationRequestRequestTypeDef,
     DescribeAccountSettingsRequestRequestTypeDef,
     DescribeAccountSubscriptionRequestRequestTypeDef,
     DescribeAnalysisDefinitionRequestRequestTypeDef,
     DescribeAnalysisPermissionsRequestRequestTypeDef,
+    ResourcePermissionOutputTypeDef,
     DescribeAnalysisRequestRequestTypeDef,
     DescribeAssetBundleExportJobRequestRequestTypeDef,
     DescribeAssetBundleImportJobRequestRequestTypeDef,
     DescribeDashboardDefinitionRequestRequestTypeDef,
     DescribeDashboardPermissionsRequestRequestTypeDef,
     DescribeDashboardRequestRequestTypeDef,
     DescribeDashboardSnapshotJobRequestRequestTypeDef,
@@ -869,14 +862,15 @@
     UserTypeDef,
     DescribeVPCConnectionRequestRequestTypeDef,
     NegativeFormatTypeDef,
     DonutCenterOptionsTypeDef,
     ListControlSelectAllOptionsTypeDef,
     ErrorInfoTypeDef,
     ExcludePeriodConfigurationTypeDef,
+    FieldFolderTypeDef,
     FieldSortTypeDef,
     FieldTooltipItemTypeDef,
     GeospatialMapStyleOptionsTypeDef,
     FilterSelectableValuesOutputTypeDef,
     FilterSelectableValuesTypeDef,
     SameSheetTargetVisualConfigurationOutputTypeDef,
     SameSheetTargetVisualConfigurationTypeDef,
@@ -885,16 +879,14 @@
     FolderSummaryTypeDef,
     FontSizeTypeDef,
     FontWeightTypeDef,
     FontTypeDef,
     TimeBasedForecastPropertiesTypeDef,
     WhatIfPointScenarioOutputTypeDef,
     WhatIfRangeScenarioOutputTypeDef,
-    WhatIfPointScenarioTypeDef,
-    WhatIfRangeScenarioTypeDef,
     FreeFormLayoutScreenCanvasSizeOptionsTypeDef,
     FreeFormLayoutElementBackgroundStyleTypeDef,
     FreeFormLayoutElementBorderStyleTypeDef,
     LoadingAnimationTypeDef,
     SessionTagTypeDef,
     GeospatialCoordinateBoundsTypeDef,
     GeospatialHeatmapDataColorTypeDef,
@@ -962,15 +954,14 @@
     ManifestFileLocationTypeDef,
     MarginStyleTypeDef,
     NamedEntityDefinitionMetricOutputTypeDef,
     NamedEntityDefinitionMetricTypeDef,
     NamespaceErrorTypeDef,
     NetworkInterfaceTypeDef,
     NewDefaultValuesOutputTypeDef,
-    NewDefaultValuesTypeDef,
     NumericRangeFilterValueTypeDef,
     ThousandSeparatorOptionsTypeDef,
     PercentileAggregationTypeDef,
     StringParameterOutputTypeDef,
     StringParameterTypeDef,
     PercentVisibleRangeTypeDef,
     PivotTableConditionalFormattingScopeTypeDef,
@@ -987,14 +978,15 @@
     ReferenceLineStaticDataConfigurationTypeDef,
     ReferenceLineStyleConfigurationTypeDef,
     ScheduleRefreshOnEntityTypeDef,
     RegisterUserRequestRequestTypeDef,
     StatePersistenceConfigurationsTypeDef,
     RegisteredUserQSearchBarEmbeddingConfigurationTypeDef,
     RenameColumnOperationTypeDef,
+    ResourcePermissionTypeDef,
     RestoreAnalysisRequestRequestTypeDef,
     RowLevelPermissionTagRuleTypeDef,
     S3BucketConfigurationTypeDef,
     UploadSettingsTypeDef,
     SectionAfterPageBreakTypeDef,
     SpacingTypeDef,
     SheetVisualScopingConfigurationOutputTypeDef,
@@ -1048,30 +1040,40 @@
     DynamicDefaultValueTypeDef,
     FilterOperationSelectedFieldsConfigurationOutputTypeDef,
     FilterOperationSelectedFieldsConfigurationTypeDef,
     NumericEqualityDrillDownFilterTypeDef,
     ParameterSelectableValuesOutputTypeDef,
     ParameterSelectableValuesTypeDef,
     TimeEqualityFilterOutputTypeDef,
-    TimeEqualityFilterTypeDef,
     TimeRangeDrillDownFilterOutputTypeDef,
-    TimeRangeDrillDownFilterTypeDef,
     AnalysisErrorTypeDef,
     DashboardErrorTypeDef,
     TemplateErrorTypeDef,
     SearchAnalysesRequestRequestTypeDef,
     AnalysisSourceTemplateTypeDef,
     DashboardSourceTemplateTypeDef,
     TemplateSourceAnalysisTypeDef,
     AnonymousUserDashboardVisualEmbeddingConfigurationTypeDef,
     RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef,
     ArcAxisConfigurationTypeDef,
     AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef,
     AssetBundleCloudFormationOverridePropertyConfigurationTypeDef,
     AssetBundleImportJobDataSourceCredentialsTypeDef,
+    AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef,
+    CustomParameterValuesTypeDef,
+    DateTimeDatasetParameterDefaultValuesTypeDef,
+    DateTimeParameterTypeDef,
+    DateTimeValueWhenUnsetConfigurationTypeDef,
+    NewDefaultValuesTypeDef,
+    TimeEqualityFilterTypeDef,
+    TimeRangeDrillDownFilterTypeDef,
+    TopicRefreshScheduleTypeDef,
+    WhatIfPointScenarioTypeDef,
+    WhatIfRangeScenarioTypeDef,
+    AssetBundleImportSourceTypeDef,
     AxisDisplayRangeOutputTypeDef,
     AxisDisplayRangeTypeDef,
     AxisScaleTypeDef,
     HistogramBinOptionsTypeDef,
     TileStyleTypeDef,
     BoxPlotOptionsTypeDef,
     CreateColumnsOperationOutputTypeDef,
@@ -1164,46 +1166,24 @@
     ColorsConfigurationOutputTypeDef,
     ColorsConfigurationTypeDef,
     ColumnTagTypeDef,
     ColumnGroupSchemaOutputTypeDef,
     ColumnGroupSchemaTypeDef,
     ColumnGroupOutputTypeDef,
     ColumnGroupTypeDef,
+    ColumnLevelPermissionRuleUnionTypeDef,
     DataSetSchemaOutputTypeDef,
     DataSetSchemaTypeDef,
     ConditionalFormattingCustomIconConditionTypeDef,
     CreateAccountCustomizationRequestRequestTypeDef,
     CreateNamespaceRequestRequestTypeDef,
     CreateVPCConnectionRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateAccountSubscriptionResponseTypeDef,
-    DescribeAnalysisPermissionsResponseTypeDef,
-    DescribeDataSetPermissionsResponseTypeDef,
-    DescribeDataSourcePermissionsResponseTypeDef,
-    DescribeFolderPermissionsResponseTypeDef,
-    DescribeFolderResolvedPermissionsResponseTypeDef,
-    DescribeTemplatePermissionsResponseTypeDef,
-    DescribeThemePermissionsResponseTypeDef,
-    DescribeTopicPermissionsResponseTypeDef,
-    LinkSharingConfigurationTypeDef,
-    UpdateAnalysisPermissionsResponseTypeDef,
-    UpdateFolderPermissionsResponseTypeDef,
-    UpdateTemplatePermissionsResponseTypeDef,
-    UpdateThemePermissionsResponseTypeDef,
-    UpdateTopicPermissionsResponseTypeDef,
-    CreateFolderRequestRequestTypeDef,
-    UpdateAnalysisPermissionsRequestRequestTypeDef,
-    UpdateDashboardPermissionsRequestRequestTypeDef,
-    UpdateDataSetPermissionsRequestRequestTypeDef,
-    UpdateDataSourcePermissionsRequestRequestTypeDef,
-    UpdateFolderPermissionsRequestRequestTypeDef,
-    UpdateTemplatePermissionsRequestRequestTypeDef,
-    UpdateThemePermissionsRequestRequestTypeDef,
-    UpdateTopicPermissionsRequestRequestTypeDef,
     DataSetSummaryTypeDef,
     CreateFolderMembershipResponseTypeDef,
     CreateGroupMembershipResponseTypeDef,
     DescribeGroupMembershipResponseTypeDef,
     ListGroupMembershipsResponseTypeDef,
     CreateGroupResponseTypeDef,
     DescribeGroupResponseTypeDef,
@@ -1215,19 +1195,16 @@
     DescribeTemplateAliasResponseTypeDef,
     ListTemplateAliasesResponseTypeDef,
     UpdateTemplateAliasResponseTypeDef,
     CreateThemeAliasResponseTypeDef,
     DescribeThemeAliasResponseTypeDef,
     ListThemeAliasesResponseTypeDef,
     UpdateThemeAliasResponseTypeDef,
-    CreateTopicRefreshScheduleRequestRequestTypeDef,
-    UpdateTopicRefreshScheduleRequestRequestTypeDef,
     CustomActionNavigationOperationTypeDef,
     CustomValuesConfigurationOutputTypeDef,
-    CustomValuesConfigurationTypeDef,
     CustomSqlOutputTypeDef,
     CustomSqlTypeDef,
     RelationalTableOutputTypeDef,
     RelationalTableTypeDef,
     SearchDashboardsRequestRequestTypeDef,
     ListDashboardsResponseTypeDef,
     SearchDashboardsResponseTypeDef,
@@ -1242,41 +1219,54 @@
     PivotTableDataPathOptionTypeDef,
     PivotTableFieldCollapseStateTargetOutputTypeDef,
     PivotTableFieldCollapseStateTargetTypeDef,
     SearchDataSetsRequestRequestTypeDef,
     SearchDataSourcesRequestRequestTypeDef,
     SearchDataSourcesResponseTypeDef,
     DateTimeDatasetParameterOutputTypeDef,
-    DateTimeDatasetParameterTypeDef,
     TimeRangeFilterValueOutputTypeDef,
     TimeRangeFilterValueTypeDef,
     DecimalDatasetParameterOutputTypeDef,
     DecimalDatasetParameterTypeDef,
+    DescribeAnalysisPermissionsResponseTypeDef,
+    DescribeDataSetPermissionsResponseTypeDef,
+    DescribeDataSourcePermissionsResponseTypeDef,
+    DescribeFolderPermissionsResponseTypeDef,
+    DescribeFolderResolvedPermissionsResponseTypeDef,
+    DescribeTemplatePermissionsResponseTypeDef,
+    DescribeThemePermissionsResponseTypeDef,
+    DescribeTopicPermissionsResponseTypeDef,
+    LinkSharingConfigurationTypeDef,
+    UpdateAnalysisPermissionsResponseTypeDef,
+    UpdateFolderPermissionsResponseTypeDef,
+    UpdateTemplatePermissionsResponseTypeDef,
+    UpdateThemePermissionsResponseTypeDef,
+    UpdateTopicPermissionsResponseTypeDef,
     DescribeFolderResponseTypeDef,
     DescribeIAMPolicyAssignmentResponseTypeDef,
     DescribeTopicRefreshResponseTypeDef,
     DescribeTopicRefreshScheduleResponseTypeDef,
     TopicRefreshScheduleSummaryTypeDef,
     DescribeUserResponseTypeDef,
     ListUsersResponseTypeDef,
     RegisterUserResponseTypeDef,
     UpdateUserResponseTypeDef,
     DisplayFormatOptionsTypeDef,
     DonutOptionsTypeDef,
     RelativeDatesFilterTypeDef,
+    FieldFolderUnionTypeDef,
     FilterOperationTargetVisualsConfigurationOutputTypeDef,
     FilterOperationTargetVisualsConfigurationTypeDef,
     SearchFoldersRequestRequestTypeDef,
     ListFoldersResponseTypeDef,
     SearchFoldersResponseTypeDef,
     FontConfigurationTypeDef,
     TypographyOutputTypeDef,
     TypographyTypeDef,
     ForecastScenarioOutputTypeDef,
-    ForecastScenarioTypeDef,
     FreeFormLayoutCanvasSizeOptionsTypeDef,
     SnapshotAnonymousUserTypeDef,
     GeospatialWindowOptionsTypeDef,
     GeospatialHeatmapColorScaleOutputTypeDef,
     GeospatialHeatmapColorScaleTypeDef,
     TableSideBorderOptionsTypeDef,
     GradientColorOutputTypeDef,
@@ -1327,25 +1317,24 @@
     TileLayoutStyleTypeDef,
     NamedEntityDefinitionOutputTypeDef,
     NamedEntityDefinitionTypeDef,
     NamespaceInfoV2TypeDef,
     VPCConnectionSummaryTypeDef,
     VPCConnectionTypeDef,
     OverrideDatasetParameterOperationOutputTypeDef,
-    OverrideDatasetParameterOperationTypeDef,
     NumericSeparatorConfigurationTypeDef,
     NumericalAggregationFunctionTypeDef,
     ParametersOutputTypeDef,
-    ParametersTypeDef,
     VisibleRangeOptionsTypeDef,
     RadarChartSeriesSettingsTypeDef,
     TopicRangeFilterConstantTypeDef,
     RefreshFrequencyTypeDef,
     RegisteredUserConsoleFeatureConfigurationsTypeDef,
     RegisteredUserDashboardFeatureConfigurationsTypeDef,
+    ResourcePermissionUnionTypeDef,
     RowLevelPermissionTagConfigurationOutputTypeDef,
     RowLevelPermissionTagConfigurationTypeDef,
     SnapshotS3DestinationConfigurationTypeDef,
     S3SourceOutputTypeDef,
     S3SourceTypeDef,
     SectionPageBreakConfigurationTypeDef,
     SectionBasedLayoutPaperCanvasSizeOptionsTypeDef,
@@ -1369,61 +1358,69 @@
     DecimalDefaultValuesOutputTypeDef,
     DecimalDefaultValuesTypeDef,
     IntegerDefaultValuesOutputTypeDef,
     IntegerDefaultValuesTypeDef,
     StringDefaultValuesOutputTypeDef,
     StringDefaultValuesTypeDef,
     DrillDownFilterOutputTypeDef,
-    DrillDownFilterTypeDef,
     AnalysisTypeDef,
     DashboardVersionTypeDef,
     AnalysisSourceEntityTypeDef,
     DashboardSourceEntityTypeDef,
     TemplateSourceEntityTypeDef,
     AnonymousUserEmbeddingExperienceConfigurationTypeDef,
     DescribeAssetBundleExportJobResponseTypeDef,
+    AssetBundleCloudFormationOverridePropertyConfigurationUnionTypeDef,
     StartAssetBundleExportJobRequestRequestTypeDef,
+    CustomValuesConfigurationTypeDef,
+    DateTimeDatasetParameterTypeDef,
+    ParametersTypeDef,
+    OverrideDatasetParameterOperationTypeDef,
+    DrillDownFilterTypeDef,
+    CreateTopicRefreshScheduleRequestRequestTypeDef,
+    TopicRefreshScheduleUnionTypeDef,
+    UpdateTopicRefreshScheduleRequestRequestTypeDef,
+    ForecastScenarioTypeDef,
     NumericAxisOptionsOutputTypeDef,
     NumericAxisOptionsTypeDef,
     CategoryFilterOutputTypeDef,
     CategoryFilterTypeDef,
     ClusterMarkerConfigurationTypeDef,
     TopicCategoryFilterOutputTypeDef,
     TopicCategoryFilterTypeDef,
     TagColumnOperationOutputTypeDef,
     TagColumnOperationTypeDef,
+    ColumnGroupUnionTypeDef,
     DataSetConfigurationOutputTypeDef,
     DataSetConfigurationTypeDef,
     ConditionalFormattingIconTypeDef,
-    DescribeDashboardPermissionsResponseTypeDef,
-    UpdateDashboardPermissionsResponseTypeDef,
     ListDataSetsResponseTypeDef,
     SearchDataSetsResponseTypeDef,
     DestinationParameterValueConfigurationOutputTypeDef,
-    DestinationParameterValueConfigurationTypeDef,
     DashboardPublishOptionsTypeDef,
     VisualPaletteOutputTypeDef,
     VisualPaletteTypeDef,
     PivotTableFieldCollapseStateOptionOutputTypeDef,
     PivotTableFieldCollapseStateOptionTypeDef,
     TimeRangeFilterOutputTypeDef,
     TimeRangeFilterTypeDef,
+    DescribeDashboardPermissionsResponseTypeDef,
+    UpdateDashboardPermissionsResponseTypeDef,
     ListTopicRefreshSchedulesResponseTypeDef,
     DefaultFormattingTypeDef,
     CustomActionFilterOperationOutputTypeDef,
     CustomActionFilterOperationTypeDef,
     AxisLabelOptionsTypeDef,
     DataLabelOptionsOutputTypeDef,
     DataLabelOptionsTypeDef,
     FunnelChartDataLabelOptionsTypeDef,
     LabelOptionsTypeDef,
     PanelTitleOptionsTypeDef,
     TableFieldCustomTextContentTypeDef,
     ForecastConfigurationOutputTypeDef,
-    ForecastConfigurationTypeDef,
     DefaultFreeFormLayoutConfigurationTypeDef,
     SnapshotUserConfigurationTypeDef,
     GeospatialHeatmapConfigurationOutputTypeDef,
     GeospatialHeatmapConfigurationTypeDef,
     GlobalTableBorderOptionsTypeDef,
     ConditionalFormattingGradientColorOutputTypeDef,
     ConditionalFormattingGradientColorTypeDef,
@@ -1451,52 +1448,64 @@
     ScrollBarOptionsTypeDef,
     TopicDateRangeFilterTypeDef,
     TopicNumericRangeFilterTypeDef,
     RefreshScheduleOutputTypeDef,
     RefreshScheduleTypeDef,
     RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef,
     RegisteredUserDashboardEmbeddingConfigurationTypeDef,
+    CreateFolderRequestRequestTypeDef,
+    UpdateAnalysisPermissionsRequestRequestTypeDef,
+    UpdateDashboardPermissionsRequestRequestTypeDef,
+    UpdateDataSetPermissionsRequestRequestTypeDef,
+    UpdateDataSourcePermissionsRequestRequestTypeDef,
+    UpdateFolderPermissionsRequestRequestTypeDef,
+    UpdateTemplatePermissionsRequestRequestTypeDef,
+    UpdateThemePermissionsRequestRequestTypeDef,
+    UpdateTopicPermissionsRequestRequestTypeDef,
+    RowLevelPermissionTagConfigurationUnionTypeDef,
     SnapshotDestinationConfigurationOutputTypeDef,
     SnapshotDestinationConfigurationTypeDef,
     SnapshotJobS3ResultTypeDef,
     PhysicalTableOutputTypeDef,
     PhysicalTableTypeDef,
     SectionBasedLayoutCanvasSizeOptionsTypeDef,
     FilterScopeConfigurationOutputTypeDef,
     FilterScopeConfigurationTypeDef,
     FreeFormLayoutElementOutputTypeDef,
     FreeFormLayoutElementTypeDef,
     SnapshotFileGroupOutputTypeDef,
     SnapshotFileGroupTypeDef,
     DatasetParameterOutputTypeDef,
-    DatasetParameterTypeDef,
     DateTimeParameterDeclarationOutputTypeDef,
     DateTimeParameterDeclarationTypeDef,
     DecimalParameterDeclarationOutputTypeDef,
     DecimalParameterDeclarationTypeDef,
     IntegerParameterDeclarationOutputTypeDef,
     IntegerParameterDeclarationTypeDef,
     StringParameterDeclarationOutputTypeDef,
     StringParameterDeclarationTypeDef,
     DateTimeHierarchyOutputTypeDef,
     ExplicitHierarchyOutputTypeDef,
     PredefinedHierarchyOutputTypeDef,
-    DateTimeHierarchyTypeDef,
-    ExplicitHierarchyTypeDef,
-    PredefinedHierarchyTypeDef,
     DescribeAnalysisResponseTypeDef,
     DashboardTypeDef,
     GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef,
+    DestinationParameterValueConfigurationTypeDef,
+    DatasetParameterTypeDef,
+    ParametersUnionTypeDef,
+    DateTimeHierarchyTypeDef,
+    ExplicitHierarchyTypeDef,
+    PredefinedHierarchyTypeDef,
+    ForecastConfigurationTypeDef,
     AxisDataOptionsOutputTypeDef,
     AxisDataOptionsTypeDef,
     TransformOperationOutputTypeDef,
     TransformOperationTypeDef,
     TemplateVersionTypeDef,
     SetParameterValueConfigurationOutputTypeDef,
-    SetParameterValueConfigurationTypeDef,
     PivotTableFieldOptionsOutputTypeDef,
     PivotTableFieldOptionsTypeDef,
     TopicCalculatedFieldOutputTypeDef,
     TopicCalculatedFieldTypeDef,
     TopicColumnOutputTypeDef,
     TopicColumnTypeDef,
     ChartAxisLabelOptionsOutputTypeDef,
@@ -1536,34 +1545,37 @@
     NumericRangeFilterTypeDef,
     ReferenceLineDynamicDataConfigurationTypeDef,
     TopicFilterOutputTypeDef,
     TopicFilterTypeDef,
     DescribeRefreshScheduleResponseTypeDef,
     ListRefreshSchedulesResponseTypeDef,
     CreateRefreshScheduleRequestRequestTypeDef,
+    RefreshScheduleUnionTypeDef,
     UpdateRefreshScheduleRequestRequestTypeDef,
     RegisteredUserEmbeddingExperienceConfigurationTypeDef,
     SnapshotJobResultFileGroupTypeDef,
+    PhysicalTableUnionTypeDef,
     DefaultSectionBasedLayoutConfigurationTypeDef,
     FreeFormLayoutConfigurationOutputTypeDef,
     FreeFormSectionLayoutConfigurationOutputTypeDef,
     FreeFormLayoutConfigurationTypeDef,
     FreeFormSectionLayoutConfigurationTypeDef,
     SnapshotConfigurationOutputTypeDef,
     SnapshotConfigurationTypeDef,
     ParameterDeclarationOutputTypeDef,
     ParameterDeclarationTypeDef,
     ColumnHierarchyOutputTypeDef,
-    ColumnHierarchyTypeDef,
     DescribeDashboardResponseTypeDef,
+    SetParameterValueConfigurationTypeDef,
+    DatasetParameterUnionTypeDef,
+    ColumnHierarchyTypeDef,
     LogicalTableOutputTypeDef,
     LogicalTableTypeDef,
     TemplateTypeDef,
     CustomActionSetParametersOperationOutputTypeDef,
-    CustomActionSetParametersOperationTypeDef,
     AxisDisplayOptionsOutputTypeDef,
     AxisDisplayOptionsTypeDef,
     FilterDateTimePickerControlTypeDef,
     ParameterDateTimePickerControlTypeDef,
     FilterDropDownControlOutputTypeDef,
     FilterDropDownControlTypeDef,
     ParameterDropDownControlOutputTypeDef,
@@ -1610,14 +1622,15 @@
     AssetBundleImportJobOverrideParametersOutputTypeDef,
     AssetBundleImportJobOverrideParametersTypeDef,
     DataSourceCredentialsTypeDef,
     DescribeDataSourceResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     ThemeVersionTypeDef,
     CreateThemeRequestRequestTypeDef,
+    ThemeConfigurationUnionTypeDef,
     UpdateThemeRequestRequestTypeDef,
     ComparisonConfigurationTypeDef,
     DateTimeFormatConfigurationTypeDef,
     NumberFormatConfigurationTypeDef,
     ReferenceLineValueLabelConfigurationTypeDef,
     StringFormatConfigurationTypeDef,
     TopBottomFilterOutputTypeDef,
@@ -1631,21 +1644,21 @@
     DatasetMetadataTypeDef,
     GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef,
     AnonymousUserSnapshotJobResultTypeDef,
     DefaultPaginatedLayoutConfigurationTypeDef,
     SectionLayoutConfigurationOutputTypeDef,
     SectionLayoutConfigurationTypeDef,
     DescribeDashboardSnapshotJobResponseTypeDef,
+    SnapshotConfigurationUnionTypeDef,
     StartDashboardSnapshotJobRequestRequestTypeDef,
+    CustomActionSetParametersOperationTypeDef,
     DataSetTypeDef,
-    CreateDataSetRequestRequestTypeDef,
-    UpdateDataSetRequestRequestTypeDef,
+    LogicalTableUnionTypeDef,
     DescribeTemplateResponseTypeDef,
     VisualCustomActionOperationOutputTypeDef,
-    VisualCustomActionOperationTypeDef,
     LineSeriesAxisDisplayOptionsOutputTypeDef,
     LineSeriesAxisDisplayOptionsTypeDef,
     FilterControlOutputTypeDef,
     FilterControlTypeDef,
     ParameterControlOutputTypeDef,
     ParameterControlTypeDef,
     TableFieldURLConfigurationTypeDef,
@@ -1658,14 +1671,15 @@
     TableCellConditionalFormattingOutputTypeDef,
     GaugeChartConditionalFormattingOptionTypeDef,
     KPIConditionalFormattingOptionTypeDef,
     FilledMapShapeConditionalFormattingTypeDef,
     PivotTableCellConditionalFormattingTypeDef,
     TableCellConditionalFormattingTypeDef,
     DescribeAssetBundleImportJobResponseTypeDef,
+    AssetBundleImportJobOverrideParametersUnionTypeDef,
     StartAssetBundleImportJobRequestRequestTypeDef,
     CreateDataSourceRequestRequestTypeDef,
     UpdateDataSourceRequestRequestTypeDef,
     ThemeTypeDef,
     GaugeChartOptionsTypeDef,
     KPIOptionsTypeDef,
     DateDimensionFieldTypeDef,
@@ -1716,17 +1730,19 @@
     TopicDetailsTypeDef,
     SnapshotJobResultTypeDef,
     DefaultNewSheetConfigurationTypeDef,
     BodySectionContentOutputTypeDef,
     HeaderFooterSectionConfigurationOutputTypeDef,
     BodySectionContentTypeDef,
     HeaderFooterSectionConfigurationTypeDef,
+    VisualCustomActionOperationTypeDef,
     DescribeDataSetResponseTypeDef,
+    CreateDataSetRequestRequestTypeDef,
+    UpdateDataSetRequestRequestTypeDef,
     VisualCustomActionOutputTypeDef,
-    VisualCustomActionTypeDef,
     TableFieldOptionTypeDef,
     GaugeChartConditionalFormattingOutputTypeDef,
     KPIConditionalFormattingOutputTypeDef,
     FilledMapConditionalFormattingOptionOutputTypeDef,
     PivotTableConditionalFormattingOptionOutputTypeDef,
     TableConditionalFormattingOptionOutputTypeDef,
     GaugeChartConditionalFormattingTypeDef,
@@ -1745,23 +1761,23 @@
     FilterGroupTypeDef,
     PivotTableSortConfigurationOutputTypeDef,
     PivotTableSortConfigurationTypeDef,
     TooltipOptionsOutputTypeDef,
     TooltipOptionsTypeDef,
     DescribeTopicResponseTypeDef,
     CreateTopicRequestRequestTypeDef,
+    TopicDetailsUnionTypeDef,
     UpdateTopicRequestRequestTypeDef,
     DescribeDashboardSnapshotJobResultResponseTypeDef,
     AnalysisDefaultsTypeDef,
     BodySectionConfigurationOutputTypeDef,
     BodySectionConfigurationTypeDef,
+    VisualCustomActionTypeDef,
     CustomContentVisualOutputTypeDef,
     EmptyVisualOutputTypeDef,
-    CustomContentVisualTypeDef,
-    EmptyVisualTypeDef,
     TableFieldOptionsOutputTypeDef,
     TableFieldOptionsTypeDef,
     FilledMapConditionalFormattingOutputTypeDef,
     PivotTableConditionalFormattingOutputTypeDef,
     TableConditionalFormattingOutputTypeDef,
     FilledMapConditionalFormattingTypeDef,
     PivotTableConditionalFormattingTypeDef,
@@ -1818,14 +1834,16 @@
     WaterfallChartAggregatedFieldWellsTypeDef,
     WordCloudAggregatedFieldWellsOutputTypeDef,
     WordCloudAggregatedFieldWellsTypeDef,
     TableUnaggregatedFieldWellsOutputTypeDef,
     TableUnaggregatedFieldWellsTypeDef,
     SectionBasedLayoutConfigurationOutputTypeDef,
     SectionBasedLayoutConfigurationTypeDef,
+    CustomContentVisualTypeDef,
+    EmptyVisualTypeDef,
     BarChartFieldWellsOutputTypeDef,
     BarChartFieldWellsTypeDef,
     BoxPlotFieldWellsOutputTypeDef,
     BoxPlotFieldWellsTypeDef,
     ComboChartFieldWellsOutputTypeDef,
     ComboChartFieldWellsTypeDef,
     FilledMapFieldWellsOutputTypeDef,
@@ -1956,24 +1974,27 @@
     TemplateVersionDefinitionOutputTypeDef,
     AnalysisDefinitionTypeDef,
     DashboardVersionDefinitionTypeDef,
     TemplateVersionDefinitionTypeDef,
     DescribeAnalysisDefinitionResponseTypeDef,
     DescribeDashboardDefinitionResponseTypeDef,
     DescribeTemplateDefinitionResponseTypeDef,
+    AnalysisDefinitionUnionTypeDef,
     CreateAnalysisRequestRequestTypeDef,
     UpdateAnalysisRequestRequestTypeDef,
     CreateDashboardRequestRequestTypeDef,
+    DashboardVersionDefinitionUnionTypeDef,
     UpdateDashboardRequestRequestTypeDef,
     CreateTemplateRequestRequestTypeDef,
+    TemplateVersionDefinitionUnionTypeDef,
     UpdateTemplateRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccountCustomizationTypeDef:
+def get_value() -> AccountCustomizationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-quicksight-1.28.15.post1/README.md` & `mypy-boto3-quicksight-1.28.16/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-quicksight.svg?color=blue)](https://pypi.org/project/mypy-boto3-quicksight)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-quicksight)](https://pepy.tech/project/mypy-boto3-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QuickSight 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[boto3.QuickSight 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
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
 [mypy-boto3-quicksight docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/).
 
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
@@ -562,20 +562,20 @@
 )
 
 
 def check_value(value: AnalysisErrorTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_quicksight.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_quicksight.type_defs import (
     AccountCustomizationTypeDef,
     AccountInfoTypeDef,
     AccountSettingsTypeDef,
     ActiveIAMPolicyAssignmentTypeDef,
@@ -622,19 +622,19 @@
     SslPropertiesTypeDef,
     VpcConnectionPropertiesTypeDef,
     AssetBundleImportJobErrorTypeDef,
     AssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef,
     AssetBundleImportJobResourceIdOverrideConfigurationTypeDef,
     AssetBundleImportJobThemeOverrideParametersTypeDef,
     AssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef,
-    AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef,
     AssetBundleImportJobVPCConnectionOverrideParametersTypeDef,
+    TimestampTypeDef,
     AssetBundleImportJobSummaryTypeDef,
     AssetBundleImportSourceDescriptionTypeDef,
-    AssetBundleImportSourceTypeDef,
+    BlobTypeDef,
     AthenaParametersTypeDef,
     AuroraParametersTypeDef,
     AuroraPostgreSqlParametersTypeDef,
     AwsIotAnalyticsParametersTypeDef,
     DateAxisOptionsTypeDef,
     AxisDisplayMinMaxRangeTypeDef,
     AxisLinearScaleTypeDef,
@@ -675,42 +675,36 @@
     ConditionalFormattingSolidColorTypeDef,
     ConditionalFormattingCustomIconOptionsTypeDef,
     ConditionalFormattingIconDisplayConfigurationTypeDef,
     ConditionalFormattingIconSetTypeDef,
     TagTypeDef,
     CreateAccountSubscriptionRequestRequestTypeDef,
     SignupResponseTypeDef,
-    ResourcePermissionOutputTypeDef,
-    ResourcePermissionTypeDef,
     DataSetUsageConfigurationTypeDef,
-    FieldFolderOutputTypeDef,
-    FieldFolderTypeDef,
     RowLevelPermissionDataSetTypeDef,
     CreateFolderMembershipRequestRequestTypeDef,
     FolderMemberTypeDef,
     CreateGroupMembershipRequestRequestTypeDef,
     GroupMemberTypeDef,
     CreateGroupRequestRequestTypeDef,
     GroupTypeDef,
     CreateIAMPolicyAssignmentRequestRequestTypeDef,
     CreateIngestionRequestRequestTypeDef,
     CreateTemplateAliasRequestRequestTypeDef,
     TemplateAliasTypeDef,
     CreateThemeAliasRequestRequestTypeDef,
     ThemeAliasTypeDef,
-    TopicRefreshScheduleTypeDef,
     DecimalPlacesConfigurationTypeDef,
     NegativeValueConfigurationTypeDef,
     NullValueFormatConfigurationTypeDef,
     LocalNavigationConfigurationTypeDef,
     CustomActionURLOperationTypeDef,
     CustomContentConfigurationTypeDef,
     CustomNarrativeOptionsTypeDef,
     CustomParameterValuesOutputTypeDef,
-    CustomParameterValuesTypeDef,
     InputColumnTypeDef,
     DataPointDrillUpDownOptionTypeDef,
     DataPointMenuLabelOptionTypeDef,
     DataPointTooltipOptionTypeDef,
     ExportToCSVOptionTypeDef,
     ExportWithHiddenFieldsOptionTypeDef,
     SheetControlsOptionTypeDef,
@@ -728,14 +722,15 @@
     DataPathLabelTypeTypeDef,
     FieldLabelTypeTypeDef,
     MaximumLabelTypeTypeDef,
     MinimumLabelTypeTypeDef,
     RangeEndsLabelTypeTypeDef,
     DataPathValueTypeDef,
     DataSetSearchFilterTypeDef,
+    FieldFolderOutputTypeDef,
     OutputColumnTypeDef,
     DataSourceErrorInfoTypeDef,
     DatabricksParametersTypeDef,
     ExasolParametersTypeDef,
     JiraParametersTypeDef,
     MariaDbParametersTypeDef,
     MySqlParametersTypeDef,
@@ -749,21 +744,18 @@
     SparkParametersTypeDef,
     SqlServerParametersTypeDef,
     TeradataParametersTypeDef,
     TwitterParametersTypeDef,
     DataSourceSearchFilterTypeDef,
     DataSourceSummaryTypeDef,
     DateTimeDatasetParameterDefaultValuesOutputTypeDef,
-    DateTimeDatasetParameterDefaultValuesTypeDef,
     RollingDateConfigurationTypeDef,
     DateTimeValueWhenUnsetConfigurationOutputTypeDef,
     MappedDataSetParameterTypeDef,
-    DateTimeValueWhenUnsetConfigurationTypeDef,
     DateTimeParameterOutputTypeDef,
-    DateTimeParameterTypeDef,
     SheetControlInfoIconLabelOptionsTypeDef,
     DecimalDatasetParameterDefaultValuesOutputTypeDef,
     DecimalDatasetParameterDefaultValuesTypeDef,
     DecimalValueWhenUnsetConfigurationTypeDef,
     DecimalParameterOutputTypeDef,
     DecimalParameterTypeDef,
     DeleteAccountCustomizationRequestRequestTypeDef,
@@ -790,14 +782,15 @@
     DeleteUserRequestRequestTypeDef,
     DeleteVPCConnectionRequestRequestTypeDef,
     DescribeAccountCustomizationRequestRequestTypeDef,
     DescribeAccountSettingsRequestRequestTypeDef,
     DescribeAccountSubscriptionRequestRequestTypeDef,
     DescribeAnalysisDefinitionRequestRequestTypeDef,
     DescribeAnalysisPermissionsRequestRequestTypeDef,
+    ResourcePermissionOutputTypeDef,
     DescribeAnalysisRequestRequestTypeDef,
     DescribeAssetBundleExportJobRequestRequestTypeDef,
     DescribeAssetBundleImportJobRequestRequestTypeDef,
     DescribeDashboardDefinitionRequestRequestTypeDef,
     DescribeDashboardPermissionsRequestRequestTypeDef,
     DescribeDashboardRequestRequestTypeDef,
     DescribeDashboardSnapshotJobRequestRequestTypeDef,
@@ -837,14 +830,15 @@
     UserTypeDef,
     DescribeVPCConnectionRequestRequestTypeDef,
     NegativeFormatTypeDef,
     DonutCenterOptionsTypeDef,
     ListControlSelectAllOptionsTypeDef,
     ErrorInfoTypeDef,
     ExcludePeriodConfigurationTypeDef,
+    FieldFolderTypeDef,
     FieldSortTypeDef,
     FieldTooltipItemTypeDef,
     GeospatialMapStyleOptionsTypeDef,
     FilterSelectableValuesOutputTypeDef,
     FilterSelectableValuesTypeDef,
     SameSheetTargetVisualConfigurationOutputTypeDef,
     SameSheetTargetVisualConfigurationTypeDef,
@@ -853,16 +847,14 @@
     FolderSummaryTypeDef,
     FontSizeTypeDef,
     FontWeightTypeDef,
     FontTypeDef,
     TimeBasedForecastPropertiesTypeDef,
     WhatIfPointScenarioOutputTypeDef,
     WhatIfRangeScenarioOutputTypeDef,
-    WhatIfPointScenarioTypeDef,
-    WhatIfRangeScenarioTypeDef,
     FreeFormLayoutScreenCanvasSizeOptionsTypeDef,
     FreeFormLayoutElementBackgroundStyleTypeDef,
     FreeFormLayoutElementBorderStyleTypeDef,
     LoadingAnimationTypeDef,
     SessionTagTypeDef,
     GeospatialCoordinateBoundsTypeDef,
     GeospatialHeatmapDataColorTypeDef,
@@ -930,15 +922,14 @@
     ManifestFileLocationTypeDef,
     MarginStyleTypeDef,
     NamedEntityDefinitionMetricOutputTypeDef,
     NamedEntityDefinitionMetricTypeDef,
     NamespaceErrorTypeDef,
     NetworkInterfaceTypeDef,
     NewDefaultValuesOutputTypeDef,
-    NewDefaultValuesTypeDef,
     NumericRangeFilterValueTypeDef,
     ThousandSeparatorOptionsTypeDef,
     PercentileAggregationTypeDef,
     StringParameterOutputTypeDef,
     StringParameterTypeDef,
     PercentVisibleRangeTypeDef,
     PivotTableConditionalFormattingScopeTypeDef,
@@ -955,14 +946,15 @@
     ReferenceLineStaticDataConfigurationTypeDef,
     ReferenceLineStyleConfigurationTypeDef,
     ScheduleRefreshOnEntityTypeDef,
     RegisterUserRequestRequestTypeDef,
     StatePersistenceConfigurationsTypeDef,
     RegisteredUserQSearchBarEmbeddingConfigurationTypeDef,
     RenameColumnOperationTypeDef,
+    ResourcePermissionTypeDef,
     RestoreAnalysisRequestRequestTypeDef,
     RowLevelPermissionTagRuleTypeDef,
     S3BucketConfigurationTypeDef,
     UploadSettingsTypeDef,
     SectionAfterPageBreakTypeDef,
     SpacingTypeDef,
     SheetVisualScopingConfigurationOutputTypeDef,
@@ -1016,30 +1008,40 @@
     DynamicDefaultValueTypeDef,
     FilterOperationSelectedFieldsConfigurationOutputTypeDef,
     FilterOperationSelectedFieldsConfigurationTypeDef,
     NumericEqualityDrillDownFilterTypeDef,
     ParameterSelectableValuesOutputTypeDef,
     ParameterSelectableValuesTypeDef,
     TimeEqualityFilterOutputTypeDef,
-    TimeEqualityFilterTypeDef,
     TimeRangeDrillDownFilterOutputTypeDef,
-    TimeRangeDrillDownFilterTypeDef,
     AnalysisErrorTypeDef,
     DashboardErrorTypeDef,
     TemplateErrorTypeDef,
     SearchAnalysesRequestRequestTypeDef,
     AnalysisSourceTemplateTypeDef,
     DashboardSourceTemplateTypeDef,
     TemplateSourceAnalysisTypeDef,
     AnonymousUserDashboardVisualEmbeddingConfigurationTypeDef,
     RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef,
     ArcAxisConfigurationTypeDef,
     AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef,
     AssetBundleCloudFormationOverridePropertyConfigurationTypeDef,
     AssetBundleImportJobDataSourceCredentialsTypeDef,
+    AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef,
+    CustomParameterValuesTypeDef,
+    DateTimeDatasetParameterDefaultValuesTypeDef,
+    DateTimeParameterTypeDef,
+    DateTimeValueWhenUnsetConfigurationTypeDef,
+    NewDefaultValuesTypeDef,
+    TimeEqualityFilterTypeDef,
+    TimeRangeDrillDownFilterTypeDef,
+    TopicRefreshScheduleTypeDef,
+    WhatIfPointScenarioTypeDef,
+    WhatIfRangeScenarioTypeDef,
+    AssetBundleImportSourceTypeDef,
     AxisDisplayRangeOutputTypeDef,
     AxisDisplayRangeTypeDef,
     AxisScaleTypeDef,
     HistogramBinOptionsTypeDef,
     TileStyleTypeDef,
     BoxPlotOptionsTypeDef,
     CreateColumnsOperationOutputTypeDef,
@@ -1132,46 +1134,24 @@
     ColorsConfigurationOutputTypeDef,
     ColorsConfigurationTypeDef,
     ColumnTagTypeDef,
     ColumnGroupSchemaOutputTypeDef,
     ColumnGroupSchemaTypeDef,
     ColumnGroupOutputTypeDef,
     ColumnGroupTypeDef,
+    ColumnLevelPermissionRuleUnionTypeDef,
     DataSetSchemaOutputTypeDef,
     DataSetSchemaTypeDef,
     ConditionalFormattingCustomIconConditionTypeDef,
     CreateAccountCustomizationRequestRequestTypeDef,
     CreateNamespaceRequestRequestTypeDef,
     CreateVPCConnectionRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateAccountSubscriptionResponseTypeDef,
-    DescribeAnalysisPermissionsResponseTypeDef,
-    DescribeDataSetPermissionsResponseTypeDef,
-    DescribeDataSourcePermissionsResponseTypeDef,
-    DescribeFolderPermissionsResponseTypeDef,
-    DescribeFolderResolvedPermissionsResponseTypeDef,
-    DescribeTemplatePermissionsResponseTypeDef,
-    DescribeThemePermissionsResponseTypeDef,
-    DescribeTopicPermissionsResponseTypeDef,
-    LinkSharingConfigurationTypeDef,
-    UpdateAnalysisPermissionsResponseTypeDef,
-    UpdateFolderPermissionsResponseTypeDef,
-    UpdateTemplatePermissionsResponseTypeDef,
-    UpdateThemePermissionsResponseTypeDef,
-    UpdateTopicPermissionsResponseTypeDef,
-    CreateFolderRequestRequestTypeDef,
-    UpdateAnalysisPermissionsRequestRequestTypeDef,
-    UpdateDashboardPermissionsRequestRequestTypeDef,
-    UpdateDataSetPermissionsRequestRequestTypeDef,
-    UpdateDataSourcePermissionsRequestRequestTypeDef,
-    UpdateFolderPermissionsRequestRequestTypeDef,
-    UpdateTemplatePermissionsRequestRequestTypeDef,
-    UpdateThemePermissionsRequestRequestTypeDef,
-    UpdateTopicPermissionsRequestRequestTypeDef,
     DataSetSummaryTypeDef,
     CreateFolderMembershipResponseTypeDef,
     CreateGroupMembershipResponseTypeDef,
     DescribeGroupMembershipResponseTypeDef,
     ListGroupMembershipsResponseTypeDef,
     CreateGroupResponseTypeDef,
     DescribeGroupResponseTypeDef,
@@ -1183,19 +1163,16 @@
     DescribeTemplateAliasResponseTypeDef,
     ListTemplateAliasesResponseTypeDef,
     UpdateTemplateAliasResponseTypeDef,
     CreateThemeAliasResponseTypeDef,
     DescribeThemeAliasResponseTypeDef,
     ListThemeAliasesResponseTypeDef,
     UpdateThemeAliasResponseTypeDef,
-    CreateTopicRefreshScheduleRequestRequestTypeDef,
-    UpdateTopicRefreshScheduleRequestRequestTypeDef,
     CustomActionNavigationOperationTypeDef,
     CustomValuesConfigurationOutputTypeDef,
-    CustomValuesConfigurationTypeDef,
     CustomSqlOutputTypeDef,
     CustomSqlTypeDef,
     RelationalTableOutputTypeDef,
     RelationalTableTypeDef,
     SearchDashboardsRequestRequestTypeDef,
     ListDashboardsResponseTypeDef,
     SearchDashboardsResponseTypeDef,
@@ -1210,41 +1187,54 @@
     PivotTableDataPathOptionTypeDef,
     PivotTableFieldCollapseStateTargetOutputTypeDef,
     PivotTableFieldCollapseStateTargetTypeDef,
     SearchDataSetsRequestRequestTypeDef,
     SearchDataSourcesRequestRequestTypeDef,
     SearchDataSourcesResponseTypeDef,
     DateTimeDatasetParameterOutputTypeDef,
-    DateTimeDatasetParameterTypeDef,
     TimeRangeFilterValueOutputTypeDef,
     TimeRangeFilterValueTypeDef,
     DecimalDatasetParameterOutputTypeDef,
     DecimalDatasetParameterTypeDef,
+    DescribeAnalysisPermissionsResponseTypeDef,
+    DescribeDataSetPermissionsResponseTypeDef,
+    DescribeDataSourcePermissionsResponseTypeDef,
+    DescribeFolderPermissionsResponseTypeDef,
+    DescribeFolderResolvedPermissionsResponseTypeDef,
+    DescribeTemplatePermissionsResponseTypeDef,
+    DescribeThemePermissionsResponseTypeDef,
+    DescribeTopicPermissionsResponseTypeDef,
+    LinkSharingConfigurationTypeDef,
+    UpdateAnalysisPermissionsResponseTypeDef,
+    UpdateFolderPermissionsResponseTypeDef,
+    UpdateTemplatePermissionsResponseTypeDef,
+    UpdateThemePermissionsResponseTypeDef,
+    UpdateTopicPermissionsResponseTypeDef,
     DescribeFolderResponseTypeDef,
     DescribeIAMPolicyAssignmentResponseTypeDef,
     DescribeTopicRefreshResponseTypeDef,
     DescribeTopicRefreshScheduleResponseTypeDef,
     TopicRefreshScheduleSummaryTypeDef,
     DescribeUserResponseTypeDef,
     ListUsersResponseTypeDef,
     RegisterUserResponseTypeDef,
     UpdateUserResponseTypeDef,
     DisplayFormatOptionsTypeDef,
     DonutOptionsTypeDef,
     RelativeDatesFilterTypeDef,
+    FieldFolderUnionTypeDef,
     FilterOperationTargetVisualsConfigurationOutputTypeDef,
     FilterOperationTargetVisualsConfigurationTypeDef,
     SearchFoldersRequestRequestTypeDef,
     ListFoldersResponseTypeDef,
     SearchFoldersResponseTypeDef,
     FontConfigurationTypeDef,
     TypographyOutputTypeDef,
     TypographyTypeDef,
     ForecastScenarioOutputTypeDef,
-    ForecastScenarioTypeDef,
     FreeFormLayoutCanvasSizeOptionsTypeDef,
     SnapshotAnonymousUserTypeDef,
     GeospatialWindowOptionsTypeDef,
     GeospatialHeatmapColorScaleOutputTypeDef,
     GeospatialHeatmapColorScaleTypeDef,
     TableSideBorderOptionsTypeDef,
     GradientColorOutputTypeDef,
@@ -1295,25 +1285,24 @@
     TileLayoutStyleTypeDef,
     NamedEntityDefinitionOutputTypeDef,
     NamedEntityDefinitionTypeDef,
     NamespaceInfoV2TypeDef,
     VPCConnectionSummaryTypeDef,
     VPCConnectionTypeDef,
     OverrideDatasetParameterOperationOutputTypeDef,
-    OverrideDatasetParameterOperationTypeDef,
     NumericSeparatorConfigurationTypeDef,
     NumericalAggregationFunctionTypeDef,
     ParametersOutputTypeDef,
-    ParametersTypeDef,
     VisibleRangeOptionsTypeDef,
     RadarChartSeriesSettingsTypeDef,
     TopicRangeFilterConstantTypeDef,
     RefreshFrequencyTypeDef,
     RegisteredUserConsoleFeatureConfigurationsTypeDef,
     RegisteredUserDashboardFeatureConfigurationsTypeDef,
+    ResourcePermissionUnionTypeDef,
     RowLevelPermissionTagConfigurationOutputTypeDef,
     RowLevelPermissionTagConfigurationTypeDef,
     SnapshotS3DestinationConfigurationTypeDef,
     S3SourceOutputTypeDef,
     S3SourceTypeDef,
     SectionPageBreakConfigurationTypeDef,
     SectionBasedLayoutPaperCanvasSizeOptionsTypeDef,
@@ -1337,61 +1326,69 @@
     DecimalDefaultValuesOutputTypeDef,
     DecimalDefaultValuesTypeDef,
     IntegerDefaultValuesOutputTypeDef,
     IntegerDefaultValuesTypeDef,
     StringDefaultValuesOutputTypeDef,
     StringDefaultValuesTypeDef,
     DrillDownFilterOutputTypeDef,
-    DrillDownFilterTypeDef,
     AnalysisTypeDef,
     DashboardVersionTypeDef,
     AnalysisSourceEntityTypeDef,
     DashboardSourceEntityTypeDef,
     TemplateSourceEntityTypeDef,
     AnonymousUserEmbeddingExperienceConfigurationTypeDef,
     DescribeAssetBundleExportJobResponseTypeDef,
+    AssetBundleCloudFormationOverridePropertyConfigurationUnionTypeDef,
     StartAssetBundleExportJobRequestRequestTypeDef,
+    CustomValuesConfigurationTypeDef,
+    DateTimeDatasetParameterTypeDef,
+    ParametersTypeDef,
+    OverrideDatasetParameterOperationTypeDef,
+    DrillDownFilterTypeDef,
+    CreateTopicRefreshScheduleRequestRequestTypeDef,
+    TopicRefreshScheduleUnionTypeDef,
+    UpdateTopicRefreshScheduleRequestRequestTypeDef,
+    ForecastScenarioTypeDef,
     NumericAxisOptionsOutputTypeDef,
     NumericAxisOptionsTypeDef,
     CategoryFilterOutputTypeDef,
     CategoryFilterTypeDef,
     ClusterMarkerConfigurationTypeDef,
     TopicCategoryFilterOutputTypeDef,
     TopicCategoryFilterTypeDef,
     TagColumnOperationOutputTypeDef,
     TagColumnOperationTypeDef,
+    ColumnGroupUnionTypeDef,
     DataSetConfigurationOutputTypeDef,
     DataSetConfigurationTypeDef,
     ConditionalFormattingIconTypeDef,
-    DescribeDashboardPermissionsResponseTypeDef,
-    UpdateDashboardPermissionsResponseTypeDef,
     ListDataSetsResponseTypeDef,
     SearchDataSetsResponseTypeDef,
     DestinationParameterValueConfigurationOutputTypeDef,
-    DestinationParameterValueConfigurationTypeDef,
     DashboardPublishOptionsTypeDef,
     VisualPaletteOutputTypeDef,
     VisualPaletteTypeDef,
     PivotTableFieldCollapseStateOptionOutputTypeDef,
     PivotTableFieldCollapseStateOptionTypeDef,
     TimeRangeFilterOutputTypeDef,
     TimeRangeFilterTypeDef,
+    DescribeDashboardPermissionsResponseTypeDef,
+    UpdateDashboardPermissionsResponseTypeDef,
     ListTopicRefreshSchedulesResponseTypeDef,
     DefaultFormattingTypeDef,
     CustomActionFilterOperationOutputTypeDef,
     CustomActionFilterOperationTypeDef,
     AxisLabelOptionsTypeDef,
     DataLabelOptionsOutputTypeDef,
     DataLabelOptionsTypeDef,
     FunnelChartDataLabelOptionsTypeDef,
     LabelOptionsTypeDef,
     PanelTitleOptionsTypeDef,
     TableFieldCustomTextContentTypeDef,
     ForecastConfigurationOutputTypeDef,
-    ForecastConfigurationTypeDef,
     DefaultFreeFormLayoutConfigurationTypeDef,
     SnapshotUserConfigurationTypeDef,
     GeospatialHeatmapConfigurationOutputTypeDef,
     GeospatialHeatmapConfigurationTypeDef,
     GlobalTableBorderOptionsTypeDef,
     ConditionalFormattingGradientColorOutputTypeDef,
     ConditionalFormattingGradientColorTypeDef,
@@ -1419,52 +1416,64 @@
     ScrollBarOptionsTypeDef,
     TopicDateRangeFilterTypeDef,
     TopicNumericRangeFilterTypeDef,
     RefreshScheduleOutputTypeDef,
     RefreshScheduleTypeDef,
     RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef,
     RegisteredUserDashboardEmbeddingConfigurationTypeDef,
+    CreateFolderRequestRequestTypeDef,
+    UpdateAnalysisPermissionsRequestRequestTypeDef,
+    UpdateDashboardPermissionsRequestRequestTypeDef,
+    UpdateDataSetPermissionsRequestRequestTypeDef,
+    UpdateDataSourcePermissionsRequestRequestTypeDef,
+    UpdateFolderPermissionsRequestRequestTypeDef,
+    UpdateTemplatePermissionsRequestRequestTypeDef,
+    UpdateThemePermissionsRequestRequestTypeDef,
+    UpdateTopicPermissionsRequestRequestTypeDef,
+    RowLevelPermissionTagConfigurationUnionTypeDef,
     SnapshotDestinationConfigurationOutputTypeDef,
     SnapshotDestinationConfigurationTypeDef,
     SnapshotJobS3ResultTypeDef,
     PhysicalTableOutputTypeDef,
     PhysicalTableTypeDef,
     SectionBasedLayoutCanvasSizeOptionsTypeDef,
     FilterScopeConfigurationOutputTypeDef,
     FilterScopeConfigurationTypeDef,
     FreeFormLayoutElementOutputTypeDef,
     FreeFormLayoutElementTypeDef,
     SnapshotFileGroupOutputTypeDef,
     SnapshotFileGroupTypeDef,
     DatasetParameterOutputTypeDef,
-    DatasetParameterTypeDef,
     DateTimeParameterDeclarationOutputTypeDef,
     DateTimeParameterDeclarationTypeDef,
     DecimalParameterDeclarationOutputTypeDef,
     DecimalParameterDeclarationTypeDef,
     IntegerParameterDeclarationOutputTypeDef,
     IntegerParameterDeclarationTypeDef,
     StringParameterDeclarationOutputTypeDef,
     StringParameterDeclarationTypeDef,
     DateTimeHierarchyOutputTypeDef,
     ExplicitHierarchyOutputTypeDef,
     PredefinedHierarchyOutputTypeDef,
-    DateTimeHierarchyTypeDef,
-    ExplicitHierarchyTypeDef,
-    PredefinedHierarchyTypeDef,
     DescribeAnalysisResponseTypeDef,
     DashboardTypeDef,
     GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef,
+    DestinationParameterValueConfigurationTypeDef,
+    DatasetParameterTypeDef,
+    ParametersUnionTypeDef,
+    DateTimeHierarchyTypeDef,
+    ExplicitHierarchyTypeDef,
+    PredefinedHierarchyTypeDef,
+    ForecastConfigurationTypeDef,
     AxisDataOptionsOutputTypeDef,
     AxisDataOptionsTypeDef,
     TransformOperationOutputTypeDef,
     TransformOperationTypeDef,
     TemplateVersionTypeDef,
     SetParameterValueConfigurationOutputTypeDef,
-    SetParameterValueConfigurationTypeDef,
     PivotTableFieldOptionsOutputTypeDef,
     PivotTableFieldOptionsTypeDef,
     TopicCalculatedFieldOutputTypeDef,
     TopicCalculatedFieldTypeDef,
     TopicColumnOutputTypeDef,
     TopicColumnTypeDef,
     ChartAxisLabelOptionsOutputTypeDef,
@@ -1504,34 +1513,37 @@
     NumericRangeFilterTypeDef,
     ReferenceLineDynamicDataConfigurationTypeDef,
     TopicFilterOutputTypeDef,
     TopicFilterTypeDef,
     DescribeRefreshScheduleResponseTypeDef,
     ListRefreshSchedulesResponseTypeDef,
     CreateRefreshScheduleRequestRequestTypeDef,
+    RefreshScheduleUnionTypeDef,
     UpdateRefreshScheduleRequestRequestTypeDef,
     RegisteredUserEmbeddingExperienceConfigurationTypeDef,
     SnapshotJobResultFileGroupTypeDef,
+    PhysicalTableUnionTypeDef,
     DefaultSectionBasedLayoutConfigurationTypeDef,
     FreeFormLayoutConfigurationOutputTypeDef,
     FreeFormSectionLayoutConfigurationOutputTypeDef,
     FreeFormLayoutConfigurationTypeDef,
     FreeFormSectionLayoutConfigurationTypeDef,
     SnapshotConfigurationOutputTypeDef,
     SnapshotConfigurationTypeDef,
     ParameterDeclarationOutputTypeDef,
     ParameterDeclarationTypeDef,
     ColumnHierarchyOutputTypeDef,
-    ColumnHierarchyTypeDef,
     DescribeDashboardResponseTypeDef,
+    SetParameterValueConfigurationTypeDef,
+    DatasetParameterUnionTypeDef,
+    ColumnHierarchyTypeDef,
     LogicalTableOutputTypeDef,
     LogicalTableTypeDef,
     TemplateTypeDef,
     CustomActionSetParametersOperationOutputTypeDef,
-    CustomActionSetParametersOperationTypeDef,
     AxisDisplayOptionsOutputTypeDef,
     AxisDisplayOptionsTypeDef,
     FilterDateTimePickerControlTypeDef,
     ParameterDateTimePickerControlTypeDef,
     FilterDropDownControlOutputTypeDef,
     FilterDropDownControlTypeDef,
     ParameterDropDownControlOutputTypeDef,
@@ -1578,14 +1590,15 @@
     AssetBundleImportJobOverrideParametersOutputTypeDef,
     AssetBundleImportJobOverrideParametersTypeDef,
     DataSourceCredentialsTypeDef,
     DescribeDataSourceResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     ThemeVersionTypeDef,
     CreateThemeRequestRequestTypeDef,
+    ThemeConfigurationUnionTypeDef,
     UpdateThemeRequestRequestTypeDef,
     ComparisonConfigurationTypeDef,
     DateTimeFormatConfigurationTypeDef,
     NumberFormatConfigurationTypeDef,
     ReferenceLineValueLabelConfigurationTypeDef,
     StringFormatConfigurationTypeDef,
     TopBottomFilterOutputTypeDef,
@@ -1599,21 +1612,21 @@
     DatasetMetadataTypeDef,
     GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef,
     AnonymousUserSnapshotJobResultTypeDef,
     DefaultPaginatedLayoutConfigurationTypeDef,
     SectionLayoutConfigurationOutputTypeDef,
     SectionLayoutConfigurationTypeDef,
     DescribeDashboardSnapshotJobResponseTypeDef,
+    SnapshotConfigurationUnionTypeDef,
     StartDashboardSnapshotJobRequestRequestTypeDef,
+    CustomActionSetParametersOperationTypeDef,
     DataSetTypeDef,
-    CreateDataSetRequestRequestTypeDef,
-    UpdateDataSetRequestRequestTypeDef,
+    LogicalTableUnionTypeDef,
     DescribeTemplateResponseTypeDef,
     VisualCustomActionOperationOutputTypeDef,
-    VisualCustomActionOperationTypeDef,
     LineSeriesAxisDisplayOptionsOutputTypeDef,
     LineSeriesAxisDisplayOptionsTypeDef,
     FilterControlOutputTypeDef,
     FilterControlTypeDef,
     ParameterControlOutputTypeDef,
     ParameterControlTypeDef,
     TableFieldURLConfigurationTypeDef,
@@ -1626,14 +1639,15 @@
     TableCellConditionalFormattingOutputTypeDef,
     GaugeChartConditionalFormattingOptionTypeDef,
     KPIConditionalFormattingOptionTypeDef,
     FilledMapShapeConditionalFormattingTypeDef,
     PivotTableCellConditionalFormattingTypeDef,
     TableCellConditionalFormattingTypeDef,
     DescribeAssetBundleImportJobResponseTypeDef,
+    AssetBundleImportJobOverrideParametersUnionTypeDef,
     StartAssetBundleImportJobRequestRequestTypeDef,
     CreateDataSourceRequestRequestTypeDef,
     UpdateDataSourceRequestRequestTypeDef,
     ThemeTypeDef,
     GaugeChartOptionsTypeDef,
     KPIOptionsTypeDef,
     DateDimensionFieldTypeDef,
@@ -1684,17 +1698,19 @@
     TopicDetailsTypeDef,
     SnapshotJobResultTypeDef,
     DefaultNewSheetConfigurationTypeDef,
     BodySectionContentOutputTypeDef,
     HeaderFooterSectionConfigurationOutputTypeDef,
     BodySectionContentTypeDef,
     HeaderFooterSectionConfigurationTypeDef,
+    VisualCustomActionOperationTypeDef,
     DescribeDataSetResponseTypeDef,
+    CreateDataSetRequestRequestTypeDef,
+    UpdateDataSetRequestRequestTypeDef,
     VisualCustomActionOutputTypeDef,
-    VisualCustomActionTypeDef,
     TableFieldOptionTypeDef,
     GaugeChartConditionalFormattingOutputTypeDef,
     KPIConditionalFormattingOutputTypeDef,
     FilledMapConditionalFormattingOptionOutputTypeDef,
     PivotTableConditionalFormattingOptionOutputTypeDef,
     TableConditionalFormattingOptionOutputTypeDef,
     GaugeChartConditionalFormattingTypeDef,
@@ -1713,23 +1729,23 @@
     FilterGroupTypeDef,
     PivotTableSortConfigurationOutputTypeDef,
     PivotTableSortConfigurationTypeDef,
     TooltipOptionsOutputTypeDef,
     TooltipOptionsTypeDef,
     DescribeTopicResponseTypeDef,
     CreateTopicRequestRequestTypeDef,
+    TopicDetailsUnionTypeDef,
     UpdateTopicRequestRequestTypeDef,
     DescribeDashboardSnapshotJobResultResponseTypeDef,
     AnalysisDefaultsTypeDef,
     BodySectionConfigurationOutputTypeDef,
     BodySectionConfigurationTypeDef,
+    VisualCustomActionTypeDef,
     CustomContentVisualOutputTypeDef,
     EmptyVisualOutputTypeDef,
-    CustomContentVisualTypeDef,
-    EmptyVisualTypeDef,
     TableFieldOptionsOutputTypeDef,
     TableFieldOptionsTypeDef,
     FilledMapConditionalFormattingOutputTypeDef,
     PivotTableConditionalFormattingOutputTypeDef,
     TableConditionalFormattingOutputTypeDef,
     FilledMapConditionalFormattingTypeDef,
     PivotTableConditionalFormattingTypeDef,
@@ -1786,14 +1802,16 @@
     WaterfallChartAggregatedFieldWellsTypeDef,
     WordCloudAggregatedFieldWellsOutputTypeDef,
     WordCloudAggregatedFieldWellsTypeDef,
     TableUnaggregatedFieldWellsOutputTypeDef,
     TableUnaggregatedFieldWellsTypeDef,
     SectionBasedLayoutConfigurationOutputTypeDef,
     SectionBasedLayoutConfigurationTypeDef,
+    CustomContentVisualTypeDef,
+    EmptyVisualTypeDef,
     BarChartFieldWellsOutputTypeDef,
     BarChartFieldWellsTypeDef,
     BoxPlotFieldWellsOutputTypeDef,
     BoxPlotFieldWellsTypeDef,
     ComboChartFieldWellsOutputTypeDef,
     ComboChartFieldWellsTypeDef,
     FilledMapFieldWellsOutputTypeDef,
@@ -1924,24 +1942,27 @@
     TemplateVersionDefinitionOutputTypeDef,
     AnalysisDefinitionTypeDef,
     DashboardVersionDefinitionTypeDef,
     TemplateVersionDefinitionTypeDef,
     DescribeAnalysisDefinitionResponseTypeDef,
     DescribeDashboardDefinitionResponseTypeDef,
     DescribeTemplateDefinitionResponseTypeDef,
+    AnalysisDefinitionUnionTypeDef,
     CreateAnalysisRequestRequestTypeDef,
     UpdateAnalysisRequestRequestTypeDef,
     CreateDashboardRequestRequestTypeDef,
+    DashboardVersionDefinitionUnionTypeDef,
     UpdateDashboardRequestRequestTypeDef,
     CreateTemplateRequestRequestTypeDef,
+    TemplateVersionDefinitionUnionTypeDef,
     UpdateTemplateRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccountCustomizationTypeDef:
+def get_value() -> AccountCustomizationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/__init__.py` & `mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/__init__.pyi` & `mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/client.py` & `mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_quicksight.client import QuickSightClient
 
     session = Session()
     client: QuickSightClient = session.client("quicksight")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AssetBundleExportFormatType,
     AssetBundleImportFailureActionType,
     AssignmentStatusType,
@@ -58,29 +58,24 @@
     SearchDashboardsPaginator,
     SearchDataSetsPaginator,
     SearchDataSourcesPaginator,
     SearchGroupsPaginator,
 )
 from .type_defs import (
     AccountCustomizationTypeDef,
-    AnalysisDefinitionOutputTypeDef,
-    AnalysisDefinitionTypeDef,
+    AnalysisDefinitionUnionTypeDef,
     AnalysisSearchFilterTypeDef,
     AnalysisSourceEntityTypeDef,
     AnonymousUserEmbeddingExperienceConfigurationTypeDef,
-    AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef,
-    AssetBundleCloudFormationOverridePropertyConfigurationTypeDef,
-    AssetBundleImportJobOverrideParametersOutputTypeDef,
-    AssetBundleImportJobOverrideParametersTypeDef,
+    AssetBundleCloudFormationOverridePropertyConfigurationUnionTypeDef,
+    AssetBundleImportJobOverrideParametersUnionTypeDef,
     AssetBundleImportSourceTypeDef,
     CancelIngestionResponseTypeDef,
-    ColumnGroupOutputTypeDef,
-    ColumnGroupTypeDef,
-    ColumnLevelPermissionRuleOutputTypeDef,
-    ColumnLevelPermissionRuleTypeDef,
+    ColumnGroupUnionTypeDef,
+    ColumnLevelPermissionRuleUnionTypeDef,
     CreateAccountCustomizationResponseTypeDef,
     CreateAccountSubscriptionResponseTypeDef,
     CreateAnalysisResponseTypeDef,
     CreateDashboardResponseTypeDef,
     CreateDataSetResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateFolderMembershipResponseTypeDef,
@@ -97,18 +92,16 @@
     CreateThemeResponseTypeDef,
     CreateTopicRefreshScheduleResponseTypeDef,
     CreateTopicResponseTypeDef,
     CreateVPCConnectionResponseTypeDef,
     DashboardPublishOptionsTypeDef,
     DashboardSearchFilterTypeDef,
     DashboardSourceEntityTypeDef,
-    DashboardVersionDefinitionOutputTypeDef,
-    DashboardVersionDefinitionTypeDef,
-    DatasetParameterOutputTypeDef,
-    DatasetParameterTypeDef,
+    DashboardVersionDefinitionUnionTypeDef,
+    DatasetParameterUnionTypeDef,
     DataSetRefreshPropertiesTypeDef,
     DataSetSearchFilterTypeDef,
     DataSetUsageConfigurationTypeDef,
     DataSourceCredentialsTypeDef,
     DataSourceParametersTypeDef,
     DataSourceSearchFilterTypeDef,
     DeleteAccountCustomizationResponseTypeDef,
@@ -171,16 +164,15 @@
     DescribeThemeResponseTypeDef,
     DescribeTopicPermissionsResponseTypeDef,
     DescribeTopicRefreshResponseTypeDef,
     DescribeTopicRefreshScheduleResponseTypeDef,
     DescribeTopicResponseTypeDef,
     DescribeUserResponseTypeDef,
     DescribeVPCConnectionResponseTypeDef,
-    FieldFolderOutputTypeDef,
-    FieldFolderTypeDef,
+    FieldFolderUnionTypeDef,
     FolderSearchFilterTypeDef,
     GenerateEmbedUrlForAnonymousUserResponseTypeDef,
     GenerateEmbedUrlForRegisteredUserResponseTypeDef,
     GetDashboardEmbedUrlResponseTypeDef,
     GetSessionEmbedUrlResponseTypeDef,
     GroupSearchFilterTypeDef,
     ListAnalysesResponseTypeDef,
@@ -207,56 +199,45 @@
     ListThemesResponseTypeDef,
     ListThemeVersionsResponseTypeDef,
     ListTopicRefreshSchedulesResponseTypeDef,
     ListTopicsResponseTypeDef,
     ListUserGroupsResponseTypeDef,
     ListUsersResponseTypeDef,
     ListVPCConnectionsResponseTypeDef,
-    LogicalTableOutputTypeDef,
-    LogicalTableTypeDef,
-    ParametersOutputTypeDef,
-    ParametersTypeDef,
-    PhysicalTableOutputTypeDef,
-    PhysicalTableTypeDef,
+    LogicalTableUnionTypeDef,
+    ParametersUnionTypeDef,
+    PhysicalTableUnionTypeDef,
     PutDataSetRefreshPropertiesResponseTypeDef,
-    RefreshScheduleOutputTypeDef,
-    RefreshScheduleTypeDef,
+    RefreshScheduleUnionTypeDef,
     RegisteredUserEmbeddingExperienceConfigurationTypeDef,
     RegisterUserResponseTypeDef,
-    ResourcePermissionOutputTypeDef,
-    ResourcePermissionTypeDef,
+    ResourcePermissionUnionTypeDef,
     RestoreAnalysisResponseTypeDef,
     RowLevelPermissionDataSetTypeDef,
-    RowLevelPermissionTagConfigurationOutputTypeDef,
-    RowLevelPermissionTagConfigurationTypeDef,
+    RowLevelPermissionTagConfigurationUnionTypeDef,
     SearchAnalysesResponseTypeDef,
     SearchDashboardsResponseTypeDef,
     SearchDataSetsResponseTypeDef,
     SearchDataSourcesResponseTypeDef,
     SearchFoldersResponseTypeDef,
     SearchGroupsResponseTypeDef,
     SessionTagTypeDef,
-    SnapshotConfigurationOutputTypeDef,
-    SnapshotConfigurationTypeDef,
+    SnapshotConfigurationUnionTypeDef,
     SnapshotUserConfigurationTypeDef,
     SslPropertiesTypeDef,
     StartAssetBundleExportJobResponseTypeDef,
     StartAssetBundleImportJobResponseTypeDef,
     StartDashboardSnapshotJobResponseTypeDef,
     TagResourceResponseTypeDef,
     TagTypeDef,
     TemplateSourceEntityTypeDef,
-    TemplateVersionDefinitionOutputTypeDef,
-    TemplateVersionDefinitionTypeDef,
-    ThemeConfigurationOutputTypeDef,
-    ThemeConfigurationTypeDef,
-    TopicDetailsOutputTypeDef,
-    TopicDetailsTypeDef,
-    TopicRefreshScheduleOutputTypeDef,
-    TopicRefreshScheduleTypeDef,
+    TemplateVersionDefinitionUnionTypeDef,
+    ThemeConfigurationUnionTypeDef,
+    TopicDetailsUnionTypeDef,
+    TopicRefreshScheduleUnionTypeDef,
     UntagResourceResponseTypeDef,
     UpdateAccountCustomizationResponseTypeDef,
     UpdateAccountSettingsResponseTypeDef,
     UpdateAnalysisPermissionsResponseTypeDef,
     UpdateAnalysisResponseTypeDef,
     UpdateDashboardPermissionsResponseTypeDef,
     UpdateDashboardPublishedVersionResponseTypeDef,
@@ -413,48 +394,42 @@
 
     def create_analysis(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
         Name: str,
-        Parameters: Union[ParametersTypeDef, ParametersOutputTypeDef] = ...,
-        Permissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
+        Parameters: ParametersUnionTypeDef = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         SourceEntity: AnalysisSourceEntityTypeDef = ...,
         ThemeArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        Definition: Union[AnalysisDefinitionTypeDef, AnalysisDefinitionOutputTypeDef] = ...
+        Definition: AnalysisDefinitionUnionTypeDef = ...
     ) -> CreateAnalysisResponseTypeDef:
         """
         Creates an analysis in Amazon QuickSight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_analysis)
         """
 
     def create_dashboard(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         Name: str,
-        Parameters: Union[ParametersTypeDef, ParametersOutputTypeDef] = ...,
-        Permissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
+        Parameters: ParametersUnionTypeDef = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         SourceEntity: DashboardSourceEntityTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         VersionDescription: str = ...,
         DashboardPublishOptions: DashboardPublishOptionsTypeDef = ...,
         ThemeArn: str = ...,
-        Definition: Union[
-            DashboardVersionDefinitionTypeDef, DashboardVersionDefinitionOutputTypeDef
-        ] = ...
+        Definition: DashboardVersionDefinitionUnionTypeDef = ...
     ) -> CreateDashboardResponseTypeDef:
         """
         Creates a dashboard from either a template or directly with a
         `DashboardDefinition`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_dashboard)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_dashboard)
@@ -462,35 +437,26 @@
 
     def create_data_set(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
         Name: str,
-        PhysicalTableMap: Mapping[str, Union[PhysicalTableTypeDef, PhysicalTableOutputTypeDef]],
+        PhysicalTableMap: Mapping[str, PhysicalTableUnionTypeDef],
         ImportMode: DataSetImportModeType,
-        LogicalTableMap: Mapping[str, Union[LogicalTableTypeDef, LogicalTableOutputTypeDef]] = ...,
-        ColumnGroups: Sequence[Union[ColumnGroupTypeDef, ColumnGroupOutputTypeDef]] = ...,
-        FieldFolders: Mapping[str, Union[FieldFolderTypeDef, FieldFolderOutputTypeDef]] = ...,
-        Permissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
+        LogicalTableMap: Mapping[str, LogicalTableUnionTypeDef] = ...,
+        ColumnGroups: Sequence[ColumnGroupUnionTypeDef] = ...,
+        FieldFolders: Mapping[str, FieldFolderUnionTypeDef] = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         RowLevelPermissionDataSet: RowLevelPermissionDataSetTypeDef = ...,
-        RowLevelPermissionTagConfiguration: Union[
-            RowLevelPermissionTagConfigurationTypeDef,
-            RowLevelPermissionTagConfigurationOutputTypeDef,
-        ] = ...,
-        ColumnLevelPermissionRules: Sequence[
-            Union[ColumnLevelPermissionRuleTypeDef, ColumnLevelPermissionRuleOutputTypeDef]
-        ] = ...,
+        RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationUnionTypeDef = ...,
+        ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DataSetUsageConfiguration: DataSetUsageConfigurationTypeDef = ...,
-        DatasetParameters: Sequence[
-            Union[DatasetParameterTypeDef, DatasetParameterOutputTypeDef]
-        ] = ...
+        DatasetParameters: Sequence[DatasetParameterUnionTypeDef] = ...
     ) -> CreateDataSetResponseTypeDef:
         """
         Creates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_data_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_data_set)
         """
@@ -500,17 +466,15 @@
         *,
         AwsAccountId: str,
         DataSourceId: str,
         Name: str,
         Type: DataSourceTypeType,
         DataSourceParameters: DataSourceParametersTypeDef = ...,
         Credentials: DataSourceCredentialsTypeDef = ...,
-        Permissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         VpcConnectionProperties: VpcConnectionPropertiesTypeDef = ...,
         SslProperties: SslPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a data source.
 
@@ -522,17 +486,15 @@
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
         Name: str = ...,
         FolderType: Literal["SHARED"] = ...,
         ParentFolderArn: str = ...,
-        Permissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateFolderResponseTypeDef:
         """
         Creates an empty shared folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_folder)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_folder)
@@ -614,42 +576,34 @@
         QuickSight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_namespace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_namespace)
         """
 
     def create_refresh_schedule(
-        self,
-        *,
-        DataSetId: str,
-        AwsAccountId: str,
-        Schedule: Union[RefreshScheduleTypeDef, RefreshScheduleOutputTypeDef]
+        self, *, DataSetId: str, AwsAccountId: str, Schedule: RefreshScheduleUnionTypeDef
     ) -> CreateRefreshScheduleResponseTypeDef:
         """
         Creates a refresh schedule for a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_refresh_schedule)
         """
 
     def create_template(
         self,
         *,
         AwsAccountId: str,
         TemplateId: str,
         Name: str = ...,
-        Permissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         SourceEntity: TemplateSourceEntityTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         VersionDescription: str = ...,
-        Definition: Union[
-            TemplateVersionDefinitionTypeDef, TemplateVersionDefinitionOutputTypeDef
-        ] = ...
+        Definition: TemplateVersionDefinitionUnionTypeDef = ...
     ) -> CreateTemplateResponseTypeDef:
         """
         Creates a template either from a `TemplateDefinition` or from an existing Amazon
         QuickSight analysis or template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_template)
@@ -668,19 +622,17 @@
     def create_theme(
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
         Name: str,
         BaseThemeId: str,
-        Configuration: Union[ThemeConfigurationTypeDef, ThemeConfigurationOutputTypeDef],
+        Configuration: ThemeConfigurationUnionTypeDef,
         VersionDescription: str = ...,
-        Permissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateThemeResponseTypeDef:
         """
         Creates a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_theme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_theme)
@@ -697,15 +649,15 @@
         """
 
     def create_topic(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
-        Topic: Union[TopicDetailsTypeDef, TopicDetailsOutputTypeDef],
+        Topic: TopicDetailsUnionTypeDef,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateTopicResponseTypeDef:
         """
         Creates a new Q topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_topic)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_topic)
@@ -713,15 +665,15 @@
 
     def create_topic_refresh_schedule(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
         DatasetArn: str,
-        RefreshSchedule: Union[TopicRefreshScheduleTypeDef, TopicRefreshScheduleOutputTypeDef],
+        RefreshSchedule: TopicRefreshScheduleUnionTypeDef,
         DatasetName: str = ...
     ) -> CreateTopicRefreshScheduleResponseTypeDef:
         """
         Creates a topic refresh schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_topic_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_topic_refresh_schedule)
@@ -1939,36 +1891,30 @@
         self,
         *,
         AwsAccountId: str,
         AssetBundleExportJobId: str,
         ResourceArns: Sequence[str],
         ExportFormat: AssetBundleExportFormatType,
         IncludeAllDependencies: bool = ...,
-        CloudFormationOverridePropertyConfiguration: Union[
-            AssetBundleCloudFormationOverridePropertyConfigurationTypeDef,
-            AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef,
-        ] = ...
+        CloudFormationOverridePropertyConfiguration: AssetBundleCloudFormationOverridePropertyConfigurationUnionTypeDef = ...
     ) -> StartAssetBundleExportJobResponseTypeDef:
         """
         Starts an Asset Bundle export job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_asset_bundle_export_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#start_asset_bundle_export_job)
         """
 
     def start_asset_bundle_import_job(
         self,
         *,
         AwsAccountId: str,
         AssetBundleImportJobId: str,
         AssetBundleImportSource: AssetBundleImportSourceTypeDef,
-        OverrideParameters: Union[
-            AssetBundleImportJobOverrideParametersTypeDef,
-            AssetBundleImportJobOverrideParametersOutputTypeDef,
-        ] = ...,
+        OverrideParameters: AssetBundleImportJobOverrideParametersUnionTypeDef = ...,
         FailureAction: AssetBundleImportFailureActionType = ...
     ) -> StartAssetBundleImportJobResponseTypeDef:
         """
         Starts an Asset Bundle import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_asset_bundle_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#start_asset_bundle_import_job)
@@ -1977,17 +1923,15 @@
     def start_dashboard_snapshot_job(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         SnapshotJobId: str,
         UserConfiguration: SnapshotUserConfigurationTypeDef,
-        SnapshotConfiguration: Union[
-            SnapshotConfigurationTypeDef, SnapshotConfigurationOutputTypeDef
-        ]
+        SnapshotConfiguration: SnapshotConfigurationUnionTypeDef
     ) -> StartDashboardSnapshotJobResponseTypeDef:
         """
         Starts an asynchronous job that generates a dashboard snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_dashboard_snapshot_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#start_dashboard_snapshot_job)
         """
@@ -2045,38 +1989,34 @@
 
     def update_analysis(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
         Name: str,
-        Parameters: Union[ParametersTypeDef, ParametersOutputTypeDef] = ...,
+        Parameters: ParametersUnionTypeDef = ...,
         SourceEntity: AnalysisSourceEntityTypeDef = ...,
         ThemeArn: str = ...,
-        Definition: Union[AnalysisDefinitionTypeDef, AnalysisDefinitionOutputTypeDef] = ...
+        Definition: AnalysisDefinitionUnionTypeDef = ...
     ) -> UpdateAnalysisResponseTypeDef:
         """
         Updates an analysis in Amazon QuickSight See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/quicksight-2018-04-01/UpdateAnalysis).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_analysis)
         """
 
     def update_analysis_permissions(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
-        GrantPermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
-        RevokePermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...
     ) -> UpdateAnalysisPermissionsResponseTypeDef:
         """
         Updates the read and write permissions for an analysis.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_analysis_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_analysis_permissions)
         """
@@ -2084,46 +2024,36 @@
     def update_dashboard(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         Name: str,
         SourceEntity: DashboardSourceEntityTypeDef = ...,
-        Parameters: Union[ParametersTypeDef, ParametersOutputTypeDef] = ...,
+        Parameters: ParametersUnionTypeDef = ...,
         VersionDescription: str = ...,
         DashboardPublishOptions: DashboardPublishOptionsTypeDef = ...,
         ThemeArn: str = ...,
-        Definition: Union[
-            DashboardVersionDefinitionTypeDef, DashboardVersionDefinitionOutputTypeDef
-        ] = ...
+        Definition: DashboardVersionDefinitionUnionTypeDef = ...
     ) -> UpdateDashboardResponseTypeDef:
         """
         Updates a dashboard in an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_dashboard)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_dashboard)
         """
 
     def update_dashboard_permissions(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
-        GrantPermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
-        RevokePermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
-        GrantLinkPermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
-        RevokeLinkPermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        GrantLinkPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokeLinkPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...
     ) -> UpdateDashboardPermissionsResponseTypeDef:
         """
         Updates read and write permissions on a dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_dashboard_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_dashboard_permissions)
         """
@@ -2140,50 +2070,39 @@
 
     def update_data_set(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
         Name: str,
-        PhysicalTableMap: Mapping[str, Union[PhysicalTableTypeDef, PhysicalTableOutputTypeDef]],
+        PhysicalTableMap: Mapping[str, PhysicalTableUnionTypeDef],
         ImportMode: DataSetImportModeType,
-        LogicalTableMap: Mapping[str, Union[LogicalTableTypeDef, LogicalTableOutputTypeDef]] = ...,
-        ColumnGroups: Sequence[Union[ColumnGroupTypeDef, ColumnGroupOutputTypeDef]] = ...,
-        FieldFolders: Mapping[str, Union[FieldFolderTypeDef, FieldFolderOutputTypeDef]] = ...,
+        LogicalTableMap: Mapping[str, LogicalTableUnionTypeDef] = ...,
+        ColumnGroups: Sequence[ColumnGroupUnionTypeDef] = ...,
+        FieldFolders: Mapping[str, FieldFolderUnionTypeDef] = ...,
         RowLevelPermissionDataSet: RowLevelPermissionDataSetTypeDef = ...,
-        RowLevelPermissionTagConfiguration: Union[
-            RowLevelPermissionTagConfigurationTypeDef,
-            RowLevelPermissionTagConfigurationOutputTypeDef,
-        ] = ...,
-        ColumnLevelPermissionRules: Sequence[
-            Union[ColumnLevelPermissionRuleTypeDef, ColumnLevelPermissionRuleOutputTypeDef]
-        ] = ...,
+        RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationUnionTypeDef = ...,
+        ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleUnionTypeDef] = ...,
         DataSetUsageConfiguration: DataSetUsageConfigurationTypeDef = ...,
-        DatasetParameters: Sequence[
-            Union[DatasetParameterTypeDef, DatasetParameterOutputTypeDef]
-        ] = ...
+        DatasetParameters: Sequence[DatasetParameterUnionTypeDef] = ...
     ) -> UpdateDataSetResponseTypeDef:
         """
         Updates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_data_set)
         """
 
     def update_data_set_permissions(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
-        GrantPermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
-        RevokePermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...
     ) -> UpdateDataSetPermissionsResponseTypeDef:
         """
         Updates the permissions on a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_set_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_data_set_permissions)
         """
@@ -2207,20 +2126,16 @@
         """
 
     def update_data_source_permissions(
         self,
         *,
         AwsAccountId: str,
         DataSourceId: str,
-        GrantPermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
-        RevokePermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...
     ) -> UpdateDataSourcePermissionsResponseTypeDef:
         """
         Updates the permissions to a data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_source_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_data_source_permissions)
         """
@@ -2236,20 +2151,16 @@
         """
 
     def update_folder_permissions(
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
-        GrantPermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
-        RevokePermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...
     ) -> UpdateFolderPermissionsResponseTypeDef:
         """
         Updates permissions of a folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_folder_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_folder_permissions)
         """
@@ -2303,19 +2214,15 @@
         public sharing settings of an Amazon QuickSight dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_public_sharing_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_public_sharing_settings)
         """
 
     def update_refresh_schedule(
-        self,
-        *,
-        DataSetId: str,
-        AwsAccountId: str,
-        Schedule: Union[RefreshScheduleTypeDef, RefreshScheduleOutputTypeDef]
+        self, *, DataSetId: str, AwsAccountId: str, Schedule: RefreshScheduleUnionTypeDef
     ) -> UpdateRefreshScheduleResponseTypeDef:
         """
         Updates a refresh schedule for a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_refresh_schedule)
         """
@@ -2324,17 +2231,15 @@
         self,
         *,
         AwsAccountId: str,
         TemplateId: str,
         SourceEntity: TemplateSourceEntityTypeDef = ...,
         VersionDescription: str = ...,
         Name: str = ...,
-        Definition: Union[
-            TemplateVersionDefinitionTypeDef, TemplateVersionDefinitionOutputTypeDef
-        ] = ...
+        Definition: TemplateVersionDefinitionUnionTypeDef = ...
     ) -> UpdateTemplateResponseTypeDef:
         """
         Updates a template from an existing Amazon QuickSight analysis or another
         template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_template)
@@ -2351,20 +2256,16 @@
         """
 
     def update_template_permissions(
         self,
         *,
         AwsAccountId: str,
         TemplateId: str,
-        GrantPermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
-        RevokePermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...
     ) -> UpdateTemplatePermissionsResponseTypeDef:
         """
         Updates the resource permissions for a template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_template_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_template_permissions)
         """
@@ -2373,15 +2274,15 @@
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
         BaseThemeId: str,
         Name: str = ...,
         VersionDescription: str = ...,
-        Configuration: Union[ThemeConfigurationTypeDef, ThemeConfigurationOutputTypeDef] = ...
+        Configuration: ThemeConfigurationUnionTypeDef = ...
     ) -> UpdateThemeResponseTypeDef:
         """
         Updates a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_theme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_theme)
         """
@@ -2397,68 +2298,56 @@
         """
 
     def update_theme_permissions(
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
-        GrantPermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
-        RevokePermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...
     ) -> UpdateThemePermissionsResponseTypeDef:
         """
         Updates the resource permissions for a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_theme_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_theme_permissions)
         """
 
     def update_topic(
-        self,
-        *,
-        AwsAccountId: str,
-        TopicId: str,
-        Topic: Union[TopicDetailsTypeDef, TopicDetailsOutputTypeDef]
+        self, *, AwsAccountId: str, TopicId: str, Topic: TopicDetailsUnionTypeDef
     ) -> UpdateTopicResponseTypeDef:
         """
         Updates a topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_topic)
         """
 
     def update_topic_permissions(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
-        GrantPermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
-        RevokePermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...
     ) -> UpdateTopicPermissionsResponseTypeDef:
         """
         Updates the permissions of a topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_topic_permissions)
         """
 
     def update_topic_refresh_schedule(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
         DatasetId: str,
-        RefreshSchedule: Union[TopicRefreshScheduleTypeDef, TopicRefreshScheduleOutputTypeDef]
+        RefreshSchedule: TopicRefreshScheduleUnionTypeDef
     ) -> UpdateTopicRefreshScheduleResponseTypeDef:
         """
         Updates a topic refresh schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_topic_refresh_schedule)
         """
```

### Comparing `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/client.pyi` & `mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/client.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_quicksight.client import QuickSightClient
 
     session = Session()
     client: QuickSightClient = session.client("quicksight")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AssetBundleExportFormatType,
     AssetBundleImportFailureActionType,
     AssignmentStatusType,
@@ -58,29 +58,24 @@
     SearchDashboardsPaginator,
     SearchDataSetsPaginator,
     SearchDataSourcesPaginator,
     SearchGroupsPaginator,
 )
 from .type_defs import (
     AccountCustomizationTypeDef,
-    AnalysisDefinitionOutputTypeDef,
-    AnalysisDefinitionTypeDef,
+    AnalysisDefinitionUnionTypeDef,
     AnalysisSearchFilterTypeDef,
     AnalysisSourceEntityTypeDef,
     AnonymousUserEmbeddingExperienceConfigurationTypeDef,
-    AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef,
-    AssetBundleCloudFormationOverridePropertyConfigurationTypeDef,
-    AssetBundleImportJobOverrideParametersOutputTypeDef,
-    AssetBundleImportJobOverrideParametersTypeDef,
+    AssetBundleCloudFormationOverridePropertyConfigurationUnionTypeDef,
+    AssetBundleImportJobOverrideParametersUnionTypeDef,
     AssetBundleImportSourceTypeDef,
     CancelIngestionResponseTypeDef,
-    ColumnGroupOutputTypeDef,
-    ColumnGroupTypeDef,
-    ColumnLevelPermissionRuleOutputTypeDef,
-    ColumnLevelPermissionRuleTypeDef,
+    ColumnGroupUnionTypeDef,
+    ColumnLevelPermissionRuleUnionTypeDef,
     CreateAccountCustomizationResponseTypeDef,
     CreateAccountSubscriptionResponseTypeDef,
     CreateAnalysisResponseTypeDef,
     CreateDashboardResponseTypeDef,
     CreateDataSetResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateFolderMembershipResponseTypeDef,
@@ -97,18 +92,16 @@
     CreateThemeResponseTypeDef,
     CreateTopicRefreshScheduleResponseTypeDef,
     CreateTopicResponseTypeDef,
     CreateVPCConnectionResponseTypeDef,
     DashboardPublishOptionsTypeDef,
     DashboardSearchFilterTypeDef,
     DashboardSourceEntityTypeDef,
-    DashboardVersionDefinitionOutputTypeDef,
-    DashboardVersionDefinitionTypeDef,
-    DatasetParameterOutputTypeDef,
-    DatasetParameterTypeDef,
+    DashboardVersionDefinitionUnionTypeDef,
+    DatasetParameterUnionTypeDef,
     DataSetRefreshPropertiesTypeDef,
     DataSetSearchFilterTypeDef,
     DataSetUsageConfigurationTypeDef,
     DataSourceCredentialsTypeDef,
     DataSourceParametersTypeDef,
     DataSourceSearchFilterTypeDef,
     DeleteAccountCustomizationResponseTypeDef,
@@ -171,16 +164,15 @@
     DescribeThemeResponseTypeDef,
     DescribeTopicPermissionsResponseTypeDef,
     DescribeTopicRefreshResponseTypeDef,
     DescribeTopicRefreshScheduleResponseTypeDef,
     DescribeTopicResponseTypeDef,
     DescribeUserResponseTypeDef,
     DescribeVPCConnectionResponseTypeDef,
-    FieldFolderOutputTypeDef,
-    FieldFolderTypeDef,
+    FieldFolderUnionTypeDef,
     FolderSearchFilterTypeDef,
     GenerateEmbedUrlForAnonymousUserResponseTypeDef,
     GenerateEmbedUrlForRegisteredUserResponseTypeDef,
     GetDashboardEmbedUrlResponseTypeDef,
     GetSessionEmbedUrlResponseTypeDef,
     GroupSearchFilterTypeDef,
     ListAnalysesResponseTypeDef,
@@ -207,56 +199,45 @@
     ListThemesResponseTypeDef,
     ListThemeVersionsResponseTypeDef,
     ListTopicRefreshSchedulesResponseTypeDef,
     ListTopicsResponseTypeDef,
     ListUserGroupsResponseTypeDef,
     ListUsersResponseTypeDef,
     ListVPCConnectionsResponseTypeDef,
-    LogicalTableOutputTypeDef,
-    LogicalTableTypeDef,
-    ParametersOutputTypeDef,
-    ParametersTypeDef,
-    PhysicalTableOutputTypeDef,
-    PhysicalTableTypeDef,
+    LogicalTableUnionTypeDef,
+    ParametersUnionTypeDef,
+    PhysicalTableUnionTypeDef,
     PutDataSetRefreshPropertiesResponseTypeDef,
-    RefreshScheduleOutputTypeDef,
-    RefreshScheduleTypeDef,
+    RefreshScheduleUnionTypeDef,
     RegisteredUserEmbeddingExperienceConfigurationTypeDef,
     RegisterUserResponseTypeDef,
-    ResourcePermissionOutputTypeDef,
-    ResourcePermissionTypeDef,
+    ResourcePermissionUnionTypeDef,
     RestoreAnalysisResponseTypeDef,
     RowLevelPermissionDataSetTypeDef,
-    RowLevelPermissionTagConfigurationOutputTypeDef,
-    RowLevelPermissionTagConfigurationTypeDef,
+    RowLevelPermissionTagConfigurationUnionTypeDef,
     SearchAnalysesResponseTypeDef,
     SearchDashboardsResponseTypeDef,
     SearchDataSetsResponseTypeDef,
     SearchDataSourcesResponseTypeDef,
     SearchFoldersResponseTypeDef,
     SearchGroupsResponseTypeDef,
     SessionTagTypeDef,
-    SnapshotConfigurationOutputTypeDef,
-    SnapshotConfigurationTypeDef,
+    SnapshotConfigurationUnionTypeDef,
     SnapshotUserConfigurationTypeDef,
     SslPropertiesTypeDef,
     StartAssetBundleExportJobResponseTypeDef,
     StartAssetBundleImportJobResponseTypeDef,
     StartDashboardSnapshotJobResponseTypeDef,
     TagResourceResponseTypeDef,
     TagTypeDef,
     TemplateSourceEntityTypeDef,
-    TemplateVersionDefinitionOutputTypeDef,
-    TemplateVersionDefinitionTypeDef,
-    ThemeConfigurationOutputTypeDef,
-    ThemeConfigurationTypeDef,
-    TopicDetailsOutputTypeDef,
-    TopicDetailsTypeDef,
-    TopicRefreshScheduleOutputTypeDef,
-    TopicRefreshScheduleTypeDef,
+    TemplateVersionDefinitionUnionTypeDef,
+    ThemeConfigurationUnionTypeDef,
+    TopicDetailsUnionTypeDef,
+    TopicRefreshScheduleUnionTypeDef,
     UntagResourceResponseTypeDef,
     UpdateAccountCustomizationResponseTypeDef,
     UpdateAccountSettingsResponseTypeDef,
     UpdateAnalysisPermissionsResponseTypeDef,
     UpdateAnalysisResponseTypeDef,
     UpdateDashboardPermissionsResponseTypeDef,
     UpdateDashboardPublishedVersionResponseTypeDef,
@@ -403,82 +384,67 @@
         """
     def create_analysis(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
         Name: str,
-        Parameters: Union[ParametersTypeDef, ParametersOutputTypeDef] = ...,
-        Permissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
+        Parameters: ParametersUnionTypeDef = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         SourceEntity: AnalysisSourceEntityTypeDef = ...,
         ThemeArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        Definition: Union[AnalysisDefinitionTypeDef, AnalysisDefinitionOutputTypeDef] = ...
+        Definition: AnalysisDefinitionUnionTypeDef = ...
     ) -> CreateAnalysisResponseTypeDef:
         """
         Creates an analysis in Amazon QuickSight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_analysis)
         """
     def create_dashboard(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         Name: str,
-        Parameters: Union[ParametersTypeDef, ParametersOutputTypeDef] = ...,
-        Permissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
+        Parameters: ParametersUnionTypeDef = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         SourceEntity: DashboardSourceEntityTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         VersionDescription: str = ...,
         DashboardPublishOptions: DashboardPublishOptionsTypeDef = ...,
         ThemeArn: str = ...,
-        Definition: Union[
-            DashboardVersionDefinitionTypeDef, DashboardVersionDefinitionOutputTypeDef
-        ] = ...
+        Definition: DashboardVersionDefinitionUnionTypeDef = ...
     ) -> CreateDashboardResponseTypeDef:
         """
         Creates a dashboard from either a template or directly with a
         `DashboardDefinition`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_dashboard)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_dashboard)
         """
     def create_data_set(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
         Name: str,
-        PhysicalTableMap: Mapping[str, Union[PhysicalTableTypeDef, PhysicalTableOutputTypeDef]],
+        PhysicalTableMap: Mapping[str, PhysicalTableUnionTypeDef],
         ImportMode: DataSetImportModeType,
-        LogicalTableMap: Mapping[str, Union[LogicalTableTypeDef, LogicalTableOutputTypeDef]] = ...,
-        ColumnGroups: Sequence[Union[ColumnGroupTypeDef, ColumnGroupOutputTypeDef]] = ...,
-        FieldFolders: Mapping[str, Union[FieldFolderTypeDef, FieldFolderOutputTypeDef]] = ...,
-        Permissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
+        LogicalTableMap: Mapping[str, LogicalTableUnionTypeDef] = ...,
+        ColumnGroups: Sequence[ColumnGroupUnionTypeDef] = ...,
+        FieldFolders: Mapping[str, FieldFolderUnionTypeDef] = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         RowLevelPermissionDataSet: RowLevelPermissionDataSetTypeDef = ...,
-        RowLevelPermissionTagConfiguration: Union[
-            RowLevelPermissionTagConfigurationTypeDef,
-            RowLevelPermissionTagConfigurationOutputTypeDef,
-        ] = ...,
-        ColumnLevelPermissionRules: Sequence[
-            Union[ColumnLevelPermissionRuleTypeDef, ColumnLevelPermissionRuleOutputTypeDef]
-        ] = ...,
+        RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationUnionTypeDef = ...,
+        ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DataSetUsageConfiguration: DataSetUsageConfigurationTypeDef = ...,
-        DatasetParameters: Sequence[
-            Union[DatasetParameterTypeDef, DatasetParameterOutputTypeDef]
-        ] = ...
+        DatasetParameters: Sequence[DatasetParameterUnionTypeDef] = ...
     ) -> CreateDataSetResponseTypeDef:
         """
         Creates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_data_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_data_set)
         """
@@ -487,17 +453,15 @@
         *,
         AwsAccountId: str,
         DataSourceId: str,
         Name: str,
         Type: DataSourceTypeType,
         DataSourceParameters: DataSourceParametersTypeDef = ...,
         Credentials: DataSourceCredentialsTypeDef = ...,
-        Permissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         VpcConnectionProperties: VpcConnectionPropertiesTypeDef = ...,
         SslProperties: SslPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a data source.
 
@@ -508,17 +472,15 @@
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
         Name: str = ...,
         FolderType: Literal["SHARED"] = ...,
         ParentFolderArn: str = ...,
-        Permissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateFolderResponseTypeDef:
         """
         Creates an empty shared folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_folder)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_folder)
@@ -593,41 +555,33 @@
         (Enterprise edition only) Creates a new namespace for you to use with Amazon
         QuickSight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_namespace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_namespace)
         """
     def create_refresh_schedule(
-        self,
-        *,
-        DataSetId: str,
-        AwsAccountId: str,
-        Schedule: Union[RefreshScheduleTypeDef, RefreshScheduleOutputTypeDef]
+        self, *, DataSetId: str, AwsAccountId: str, Schedule: RefreshScheduleUnionTypeDef
     ) -> CreateRefreshScheduleResponseTypeDef:
         """
         Creates a refresh schedule for a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_refresh_schedule)
         """
     def create_template(
         self,
         *,
         AwsAccountId: str,
         TemplateId: str,
         Name: str = ...,
-        Permissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         SourceEntity: TemplateSourceEntityTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         VersionDescription: str = ...,
-        Definition: Union[
-            TemplateVersionDefinitionTypeDef, TemplateVersionDefinitionOutputTypeDef
-        ] = ...
+        Definition: TemplateVersionDefinitionUnionTypeDef = ...
     ) -> CreateTemplateResponseTypeDef:
         """
         Creates a template either from a `TemplateDefinition` or from an existing Amazon
         QuickSight analysis or template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_template)
@@ -644,19 +598,17 @@
     def create_theme(
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
         Name: str,
         BaseThemeId: str,
-        Configuration: Union[ThemeConfigurationTypeDef, ThemeConfigurationOutputTypeDef],
+        Configuration: ThemeConfigurationUnionTypeDef,
         VersionDescription: str = ...,
-        Permissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateThemeResponseTypeDef:
         """
         Creates a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_theme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_theme)
@@ -671,30 +623,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_theme_alias)
         """
     def create_topic(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
-        Topic: Union[TopicDetailsTypeDef, TopicDetailsOutputTypeDef],
+        Topic: TopicDetailsUnionTypeDef,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateTopicResponseTypeDef:
         """
         Creates a new Q topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_topic)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_topic)
         """
     def create_topic_refresh_schedule(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
         DatasetArn: str,
-        RefreshSchedule: Union[TopicRefreshScheduleTypeDef, TopicRefreshScheduleOutputTypeDef],
+        RefreshSchedule: TopicRefreshScheduleUnionTypeDef,
         DatasetName: str = ...
     ) -> CreateTopicRefreshScheduleResponseTypeDef:
         """
         Creates a topic refresh schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_topic_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_topic_refresh_schedule)
@@ -1804,35 +1756,29 @@
         self,
         *,
         AwsAccountId: str,
         AssetBundleExportJobId: str,
         ResourceArns: Sequence[str],
         ExportFormat: AssetBundleExportFormatType,
         IncludeAllDependencies: bool = ...,
-        CloudFormationOverridePropertyConfiguration: Union[
-            AssetBundleCloudFormationOverridePropertyConfigurationTypeDef,
-            AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef,
-        ] = ...
+        CloudFormationOverridePropertyConfiguration: AssetBundleCloudFormationOverridePropertyConfigurationUnionTypeDef = ...
     ) -> StartAssetBundleExportJobResponseTypeDef:
         """
         Starts an Asset Bundle export job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_asset_bundle_export_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#start_asset_bundle_export_job)
         """
     def start_asset_bundle_import_job(
         self,
         *,
         AwsAccountId: str,
         AssetBundleImportJobId: str,
         AssetBundleImportSource: AssetBundleImportSourceTypeDef,
-        OverrideParameters: Union[
-            AssetBundleImportJobOverrideParametersTypeDef,
-            AssetBundleImportJobOverrideParametersOutputTypeDef,
-        ] = ...,
+        OverrideParameters: AssetBundleImportJobOverrideParametersUnionTypeDef = ...,
         FailureAction: AssetBundleImportFailureActionType = ...
     ) -> StartAssetBundleImportJobResponseTypeDef:
         """
         Starts an Asset Bundle import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_asset_bundle_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#start_asset_bundle_import_job)
@@ -1840,17 +1786,15 @@
     def start_dashboard_snapshot_job(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         SnapshotJobId: str,
         UserConfiguration: SnapshotUserConfigurationTypeDef,
-        SnapshotConfiguration: Union[
-            SnapshotConfigurationTypeDef, SnapshotConfigurationOutputTypeDef
-        ]
+        SnapshotConfiguration: SnapshotConfigurationUnionTypeDef
     ) -> StartDashboardSnapshotJobResponseTypeDef:
         """
         Starts an asynchronous job that generates a dashboard snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_dashboard_snapshot_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#start_dashboard_snapshot_job)
         """
@@ -1903,82 +1847,68 @@
         """
     def update_analysis(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
         Name: str,
-        Parameters: Union[ParametersTypeDef, ParametersOutputTypeDef] = ...,
+        Parameters: ParametersUnionTypeDef = ...,
         SourceEntity: AnalysisSourceEntityTypeDef = ...,
         ThemeArn: str = ...,
-        Definition: Union[AnalysisDefinitionTypeDef, AnalysisDefinitionOutputTypeDef] = ...
+        Definition: AnalysisDefinitionUnionTypeDef = ...
     ) -> UpdateAnalysisResponseTypeDef:
         """
         Updates an analysis in Amazon QuickSight See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/quicksight-2018-04-01/UpdateAnalysis).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_analysis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_analysis)
         """
     def update_analysis_permissions(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
-        GrantPermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
-        RevokePermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...
     ) -> UpdateAnalysisPermissionsResponseTypeDef:
         """
         Updates the read and write permissions for an analysis.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_analysis_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_analysis_permissions)
         """
     def update_dashboard(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         Name: str,
         SourceEntity: DashboardSourceEntityTypeDef = ...,
-        Parameters: Union[ParametersTypeDef, ParametersOutputTypeDef] = ...,
+        Parameters: ParametersUnionTypeDef = ...,
         VersionDescription: str = ...,
         DashboardPublishOptions: DashboardPublishOptionsTypeDef = ...,
         ThemeArn: str = ...,
-        Definition: Union[
-            DashboardVersionDefinitionTypeDef, DashboardVersionDefinitionOutputTypeDef
-        ] = ...
+        Definition: DashboardVersionDefinitionUnionTypeDef = ...
     ) -> UpdateDashboardResponseTypeDef:
         """
         Updates a dashboard in an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_dashboard)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_dashboard)
         """
     def update_dashboard_permissions(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
-        GrantPermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
-        RevokePermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
-        GrantLinkPermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
-        RevokeLinkPermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        GrantLinkPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokeLinkPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...
     ) -> UpdateDashboardPermissionsResponseTypeDef:
         """
         Updates read and write permissions on a dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_dashboard_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_dashboard_permissions)
         """
@@ -1993,49 +1923,38 @@
         """
     def update_data_set(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
         Name: str,
-        PhysicalTableMap: Mapping[str, Union[PhysicalTableTypeDef, PhysicalTableOutputTypeDef]],
+        PhysicalTableMap: Mapping[str, PhysicalTableUnionTypeDef],
         ImportMode: DataSetImportModeType,
-        LogicalTableMap: Mapping[str, Union[LogicalTableTypeDef, LogicalTableOutputTypeDef]] = ...,
-        ColumnGroups: Sequence[Union[ColumnGroupTypeDef, ColumnGroupOutputTypeDef]] = ...,
-        FieldFolders: Mapping[str, Union[FieldFolderTypeDef, FieldFolderOutputTypeDef]] = ...,
+        LogicalTableMap: Mapping[str, LogicalTableUnionTypeDef] = ...,
+        ColumnGroups: Sequence[ColumnGroupUnionTypeDef] = ...,
+        FieldFolders: Mapping[str, FieldFolderUnionTypeDef] = ...,
         RowLevelPermissionDataSet: RowLevelPermissionDataSetTypeDef = ...,
-        RowLevelPermissionTagConfiguration: Union[
-            RowLevelPermissionTagConfigurationTypeDef,
-            RowLevelPermissionTagConfigurationOutputTypeDef,
-        ] = ...,
-        ColumnLevelPermissionRules: Sequence[
-            Union[ColumnLevelPermissionRuleTypeDef, ColumnLevelPermissionRuleOutputTypeDef]
-        ] = ...,
+        RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationUnionTypeDef = ...,
+        ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleUnionTypeDef] = ...,
         DataSetUsageConfiguration: DataSetUsageConfigurationTypeDef = ...,
-        DatasetParameters: Sequence[
-            Union[DatasetParameterTypeDef, DatasetParameterOutputTypeDef]
-        ] = ...
+        DatasetParameters: Sequence[DatasetParameterUnionTypeDef] = ...
     ) -> UpdateDataSetResponseTypeDef:
         """
         Updates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_data_set)
         """
     def update_data_set_permissions(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
-        GrantPermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
-        RevokePermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...
     ) -> UpdateDataSetPermissionsResponseTypeDef:
         """
         Updates the permissions on a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_set_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_data_set_permissions)
         """
@@ -2057,20 +1976,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_data_source)
         """
     def update_data_source_permissions(
         self,
         *,
         AwsAccountId: str,
         DataSourceId: str,
-        GrantPermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
-        RevokePermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...
     ) -> UpdateDataSourcePermissionsResponseTypeDef:
         """
         Updates the permissions to a data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_source_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_data_source_permissions)
         """
@@ -2084,20 +1999,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_folder)
         """
     def update_folder_permissions(
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
-        GrantPermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
-        RevokePermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...
     ) -> UpdateFolderPermissionsResponseTypeDef:
         """
         Updates permissions of a folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_folder_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_folder_permissions)
         """
@@ -2146,19 +2057,15 @@
         Use the `UpdatePublicSharingSettings` operation to turn on or turn off the
         public sharing settings of an Amazon QuickSight dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_public_sharing_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_public_sharing_settings)
         """
     def update_refresh_schedule(
-        self,
-        *,
-        DataSetId: str,
-        AwsAccountId: str,
-        Schedule: Union[RefreshScheduleTypeDef, RefreshScheduleOutputTypeDef]
+        self, *, DataSetId: str, AwsAccountId: str, Schedule: RefreshScheduleUnionTypeDef
     ) -> UpdateRefreshScheduleResponseTypeDef:
         """
         Updates a refresh schedule for a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_refresh_schedule)
         """
@@ -2166,17 +2073,15 @@
         self,
         *,
         AwsAccountId: str,
         TemplateId: str,
         SourceEntity: TemplateSourceEntityTypeDef = ...,
         VersionDescription: str = ...,
         Name: str = ...,
-        Definition: Union[
-            TemplateVersionDefinitionTypeDef, TemplateVersionDefinitionOutputTypeDef
-        ] = ...
+        Definition: TemplateVersionDefinitionUnionTypeDef = ...
     ) -> UpdateTemplateResponseTypeDef:
         """
         Updates a template from an existing Amazon QuickSight analysis or another
         template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_template)
@@ -2191,20 +2096,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_template_alias)
         """
     def update_template_permissions(
         self,
         *,
         AwsAccountId: str,
         TemplateId: str,
-        GrantPermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
-        RevokePermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...
     ) -> UpdateTemplatePermissionsResponseTypeDef:
         """
         Updates the resource permissions for a template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_template_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_template_permissions)
         """
@@ -2212,15 +2113,15 @@
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
         BaseThemeId: str,
         Name: str = ...,
         VersionDescription: str = ...,
-        Configuration: Union[ThemeConfigurationTypeDef, ThemeConfigurationOutputTypeDef] = ...
+        Configuration: ThemeConfigurationUnionTypeDef = ...
     ) -> UpdateThemeResponseTypeDef:
         """
         Updates a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_theme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_theme)
         """
@@ -2234,65 +2135,53 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_theme_alias)
         """
     def update_theme_permissions(
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
-        GrantPermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
-        RevokePermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...
     ) -> UpdateThemePermissionsResponseTypeDef:
         """
         Updates the resource permissions for a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_theme_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_theme_permissions)
         """
     def update_topic(
-        self,
-        *,
-        AwsAccountId: str,
-        TopicId: str,
-        Topic: Union[TopicDetailsTypeDef, TopicDetailsOutputTypeDef]
+        self, *, AwsAccountId: str, TopicId: str, Topic: TopicDetailsUnionTypeDef
     ) -> UpdateTopicResponseTypeDef:
         """
         Updates a topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_topic)
         """
     def update_topic_permissions(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
-        GrantPermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...,
-        RevokePermissions: Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ] = ...
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...
     ) -> UpdateTopicPermissionsResponseTypeDef:
         """
         Updates the permissions of a topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_topic_permissions)
         """
     def update_topic_refresh_schedule(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
         DatasetId: str,
-        RefreshSchedule: Union[TopicRefreshScheduleTypeDef, TopicRefreshScheduleOutputTypeDef]
+        RefreshSchedule: TopicRefreshScheduleUnionTypeDef
     ) -> UpdateTopicRefreshScheduleResponseTypeDef:
         """
         Updates a topic refresh schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_topic_refresh_schedule)
         """
```

### Comparing `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/literals.py` & `mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/literals.pyi` & `mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/paginator.py` & `mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/paginator.pyi` & `mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/type_defs.py` & `mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_quicksight.type_defs import AccountCustomizationTypeDef
 
-    data: AccountCustomizationTypeDef = {...}
+    data: AccountCustomizationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -249,19 +249,19 @@
     "SslPropertiesTypeDef",
     "VpcConnectionPropertiesTypeDef",
     "AssetBundleImportJobErrorTypeDef",
     "AssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef",
     "AssetBundleImportJobResourceIdOverrideConfigurationTypeDef",
     "AssetBundleImportJobThemeOverrideParametersTypeDef",
     "AssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef",
-    "AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
     "AssetBundleImportJobVPCConnectionOverrideParametersTypeDef",
+    "TimestampTypeDef",
     "AssetBundleImportJobSummaryTypeDef",
     "AssetBundleImportSourceDescriptionTypeDef",
-    "AssetBundleImportSourceTypeDef",
+    "BlobTypeDef",
     "AthenaParametersTypeDef",
     "AuroraParametersTypeDef",
     "AuroraPostgreSqlParametersTypeDef",
     "AwsIotAnalyticsParametersTypeDef",
     "DateAxisOptionsTypeDef",
     "AxisDisplayMinMaxRangeTypeDef",
     "AxisLinearScaleTypeDef",
@@ -302,42 +302,36 @@
     "ConditionalFormattingSolidColorTypeDef",
     "ConditionalFormattingCustomIconOptionsTypeDef",
     "ConditionalFormattingIconDisplayConfigurationTypeDef",
     "ConditionalFormattingIconSetTypeDef",
     "TagTypeDef",
     "CreateAccountSubscriptionRequestRequestTypeDef",
     "SignupResponseTypeDef",
-    "ResourcePermissionOutputTypeDef",
-    "ResourcePermissionTypeDef",
     "DataSetUsageConfigurationTypeDef",
-    "FieldFolderOutputTypeDef",
-    "FieldFolderTypeDef",
     "RowLevelPermissionDataSetTypeDef",
     "CreateFolderMembershipRequestRequestTypeDef",
     "FolderMemberTypeDef",
     "CreateGroupMembershipRequestRequestTypeDef",
     "GroupMemberTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "GroupTypeDef",
     "CreateIAMPolicyAssignmentRequestRequestTypeDef",
     "CreateIngestionRequestRequestTypeDef",
     "CreateTemplateAliasRequestRequestTypeDef",
     "TemplateAliasTypeDef",
     "CreateThemeAliasRequestRequestTypeDef",
     "ThemeAliasTypeDef",
-    "TopicRefreshScheduleTypeDef",
     "DecimalPlacesConfigurationTypeDef",
     "NegativeValueConfigurationTypeDef",
     "NullValueFormatConfigurationTypeDef",
     "LocalNavigationConfigurationTypeDef",
     "CustomActionURLOperationTypeDef",
     "CustomContentConfigurationTypeDef",
     "CustomNarrativeOptionsTypeDef",
     "CustomParameterValuesOutputTypeDef",
-    "CustomParameterValuesTypeDef",
     "InputColumnTypeDef",
     "DataPointDrillUpDownOptionTypeDef",
     "DataPointMenuLabelOptionTypeDef",
     "DataPointTooltipOptionTypeDef",
     "ExportToCSVOptionTypeDef",
     "ExportWithHiddenFieldsOptionTypeDef",
     "SheetControlsOptionTypeDef",
@@ -355,14 +349,15 @@
     "DataPathLabelTypeTypeDef",
     "FieldLabelTypeTypeDef",
     "MaximumLabelTypeTypeDef",
     "MinimumLabelTypeTypeDef",
     "RangeEndsLabelTypeTypeDef",
     "DataPathValueTypeDef",
     "DataSetSearchFilterTypeDef",
+    "FieldFolderOutputTypeDef",
     "OutputColumnTypeDef",
     "DataSourceErrorInfoTypeDef",
     "DatabricksParametersTypeDef",
     "ExasolParametersTypeDef",
     "JiraParametersTypeDef",
     "MariaDbParametersTypeDef",
     "MySqlParametersTypeDef",
@@ -376,21 +371,18 @@
     "SparkParametersTypeDef",
     "SqlServerParametersTypeDef",
     "TeradataParametersTypeDef",
     "TwitterParametersTypeDef",
     "DataSourceSearchFilterTypeDef",
     "DataSourceSummaryTypeDef",
     "DateTimeDatasetParameterDefaultValuesOutputTypeDef",
-    "DateTimeDatasetParameterDefaultValuesTypeDef",
     "RollingDateConfigurationTypeDef",
     "DateTimeValueWhenUnsetConfigurationOutputTypeDef",
     "MappedDataSetParameterTypeDef",
-    "DateTimeValueWhenUnsetConfigurationTypeDef",
     "DateTimeParameterOutputTypeDef",
-    "DateTimeParameterTypeDef",
     "SheetControlInfoIconLabelOptionsTypeDef",
     "DecimalDatasetParameterDefaultValuesOutputTypeDef",
     "DecimalDatasetParameterDefaultValuesTypeDef",
     "DecimalValueWhenUnsetConfigurationTypeDef",
     "DecimalParameterOutputTypeDef",
     "DecimalParameterTypeDef",
     "DeleteAccountCustomizationRequestRequestTypeDef",
@@ -417,14 +409,15 @@
     "DeleteUserRequestRequestTypeDef",
     "DeleteVPCConnectionRequestRequestTypeDef",
     "DescribeAccountCustomizationRequestRequestTypeDef",
     "DescribeAccountSettingsRequestRequestTypeDef",
     "DescribeAccountSubscriptionRequestRequestTypeDef",
     "DescribeAnalysisDefinitionRequestRequestTypeDef",
     "DescribeAnalysisPermissionsRequestRequestTypeDef",
+    "ResourcePermissionOutputTypeDef",
     "DescribeAnalysisRequestRequestTypeDef",
     "DescribeAssetBundleExportJobRequestRequestTypeDef",
     "DescribeAssetBundleImportJobRequestRequestTypeDef",
     "DescribeDashboardDefinitionRequestRequestTypeDef",
     "DescribeDashboardPermissionsRequestRequestTypeDef",
     "DescribeDashboardRequestRequestTypeDef",
     "DescribeDashboardSnapshotJobRequestRequestTypeDef",
@@ -464,14 +457,15 @@
     "UserTypeDef",
     "DescribeVPCConnectionRequestRequestTypeDef",
     "NegativeFormatTypeDef",
     "DonutCenterOptionsTypeDef",
     "ListControlSelectAllOptionsTypeDef",
     "ErrorInfoTypeDef",
     "ExcludePeriodConfigurationTypeDef",
+    "FieldFolderTypeDef",
     "FieldSortTypeDef",
     "FieldTooltipItemTypeDef",
     "GeospatialMapStyleOptionsTypeDef",
     "FilterSelectableValuesOutputTypeDef",
     "FilterSelectableValuesTypeDef",
     "SameSheetTargetVisualConfigurationOutputTypeDef",
     "SameSheetTargetVisualConfigurationTypeDef",
@@ -480,16 +474,14 @@
     "FolderSummaryTypeDef",
     "FontSizeTypeDef",
     "FontWeightTypeDef",
     "FontTypeDef",
     "TimeBasedForecastPropertiesTypeDef",
     "WhatIfPointScenarioOutputTypeDef",
     "WhatIfRangeScenarioOutputTypeDef",
-    "WhatIfPointScenarioTypeDef",
-    "WhatIfRangeScenarioTypeDef",
     "FreeFormLayoutScreenCanvasSizeOptionsTypeDef",
     "FreeFormLayoutElementBackgroundStyleTypeDef",
     "FreeFormLayoutElementBorderStyleTypeDef",
     "LoadingAnimationTypeDef",
     "SessionTagTypeDef",
     "GeospatialCoordinateBoundsTypeDef",
     "GeospatialHeatmapDataColorTypeDef",
@@ -557,15 +549,14 @@
     "ManifestFileLocationTypeDef",
     "MarginStyleTypeDef",
     "NamedEntityDefinitionMetricOutputTypeDef",
     "NamedEntityDefinitionMetricTypeDef",
     "NamespaceErrorTypeDef",
     "NetworkInterfaceTypeDef",
     "NewDefaultValuesOutputTypeDef",
-    "NewDefaultValuesTypeDef",
     "NumericRangeFilterValueTypeDef",
     "ThousandSeparatorOptionsTypeDef",
     "PercentileAggregationTypeDef",
     "StringParameterOutputTypeDef",
     "StringParameterTypeDef",
     "PercentVisibleRangeTypeDef",
     "PivotTableConditionalFormattingScopeTypeDef",
@@ -582,14 +573,15 @@
     "ReferenceLineStaticDataConfigurationTypeDef",
     "ReferenceLineStyleConfigurationTypeDef",
     "ScheduleRefreshOnEntityTypeDef",
     "RegisterUserRequestRequestTypeDef",
     "StatePersistenceConfigurationsTypeDef",
     "RegisteredUserQSearchBarEmbeddingConfigurationTypeDef",
     "RenameColumnOperationTypeDef",
+    "ResourcePermissionTypeDef",
     "RestoreAnalysisRequestRequestTypeDef",
     "RowLevelPermissionTagRuleTypeDef",
     "S3BucketConfigurationTypeDef",
     "UploadSettingsTypeDef",
     "SectionAfterPageBreakTypeDef",
     "SpacingTypeDef",
     "SheetVisualScopingConfigurationOutputTypeDef",
@@ -643,30 +635,40 @@
     "DynamicDefaultValueTypeDef",
     "FilterOperationSelectedFieldsConfigurationOutputTypeDef",
     "FilterOperationSelectedFieldsConfigurationTypeDef",
     "NumericEqualityDrillDownFilterTypeDef",
     "ParameterSelectableValuesOutputTypeDef",
     "ParameterSelectableValuesTypeDef",
     "TimeEqualityFilterOutputTypeDef",
-    "TimeEqualityFilterTypeDef",
     "TimeRangeDrillDownFilterOutputTypeDef",
-    "TimeRangeDrillDownFilterTypeDef",
     "AnalysisErrorTypeDef",
     "DashboardErrorTypeDef",
     "TemplateErrorTypeDef",
     "SearchAnalysesRequestRequestTypeDef",
     "AnalysisSourceTemplateTypeDef",
     "DashboardSourceTemplateTypeDef",
     "TemplateSourceAnalysisTypeDef",
     "AnonymousUserDashboardVisualEmbeddingConfigurationTypeDef",
     "RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef",
     "ArcAxisConfigurationTypeDef",
     "AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef",
     "AssetBundleCloudFormationOverridePropertyConfigurationTypeDef",
     "AssetBundleImportJobDataSourceCredentialsTypeDef",
+    "AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
+    "CustomParameterValuesTypeDef",
+    "DateTimeDatasetParameterDefaultValuesTypeDef",
+    "DateTimeParameterTypeDef",
+    "DateTimeValueWhenUnsetConfigurationTypeDef",
+    "NewDefaultValuesTypeDef",
+    "TimeEqualityFilterTypeDef",
+    "TimeRangeDrillDownFilterTypeDef",
+    "TopicRefreshScheduleTypeDef",
+    "WhatIfPointScenarioTypeDef",
+    "WhatIfRangeScenarioTypeDef",
+    "AssetBundleImportSourceTypeDef",
     "AxisDisplayRangeOutputTypeDef",
     "AxisDisplayRangeTypeDef",
     "AxisScaleTypeDef",
     "HistogramBinOptionsTypeDef",
     "TileStyleTypeDef",
     "BoxPlotOptionsTypeDef",
     "CreateColumnsOperationOutputTypeDef",
@@ -759,46 +761,24 @@
     "ColorsConfigurationOutputTypeDef",
     "ColorsConfigurationTypeDef",
     "ColumnTagTypeDef",
     "ColumnGroupSchemaOutputTypeDef",
     "ColumnGroupSchemaTypeDef",
     "ColumnGroupOutputTypeDef",
     "ColumnGroupTypeDef",
+    "ColumnLevelPermissionRuleUnionTypeDef",
     "DataSetSchemaOutputTypeDef",
     "DataSetSchemaTypeDef",
     "ConditionalFormattingCustomIconConditionTypeDef",
     "CreateAccountCustomizationRequestRequestTypeDef",
     "CreateNamespaceRequestRequestTypeDef",
     "CreateVPCConnectionRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateAccountSubscriptionResponseTypeDef",
-    "DescribeAnalysisPermissionsResponseTypeDef",
-    "DescribeDataSetPermissionsResponseTypeDef",
-    "DescribeDataSourcePermissionsResponseTypeDef",
-    "DescribeFolderPermissionsResponseTypeDef",
-    "DescribeFolderResolvedPermissionsResponseTypeDef",
-    "DescribeTemplatePermissionsResponseTypeDef",
-    "DescribeThemePermissionsResponseTypeDef",
-    "DescribeTopicPermissionsResponseTypeDef",
-    "LinkSharingConfigurationTypeDef",
-    "UpdateAnalysisPermissionsResponseTypeDef",
-    "UpdateFolderPermissionsResponseTypeDef",
-    "UpdateTemplatePermissionsResponseTypeDef",
-    "UpdateThemePermissionsResponseTypeDef",
-    "UpdateTopicPermissionsResponseTypeDef",
-    "CreateFolderRequestRequestTypeDef",
-    "UpdateAnalysisPermissionsRequestRequestTypeDef",
-    "UpdateDashboardPermissionsRequestRequestTypeDef",
-    "UpdateDataSetPermissionsRequestRequestTypeDef",
-    "UpdateDataSourcePermissionsRequestRequestTypeDef",
-    "UpdateFolderPermissionsRequestRequestTypeDef",
-    "UpdateTemplatePermissionsRequestRequestTypeDef",
-    "UpdateThemePermissionsRequestRequestTypeDef",
-    "UpdateTopicPermissionsRequestRequestTypeDef",
     "DataSetSummaryTypeDef",
     "CreateFolderMembershipResponseTypeDef",
     "CreateGroupMembershipResponseTypeDef",
     "DescribeGroupMembershipResponseTypeDef",
     "ListGroupMembershipsResponseTypeDef",
     "CreateGroupResponseTypeDef",
     "DescribeGroupResponseTypeDef",
@@ -810,19 +790,16 @@
     "DescribeTemplateAliasResponseTypeDef",
     "ListTemplateAliasesResponseTypeDef",
     "UpdateTemplateAliasResponseTypeDef",
     "CreateThemeAliasResponseTypeDef",
     "DescribeThemeAliasResponseTypeDef",
     "ListThemeAliasesResponseTypeDef",
     "UpdateThemeAliasResponseTypeDef",
-    "CreateTopicRefreshScheduleRequestRequestTypeDef",
-    "UpdateTopicRefreshScheduleRequestRequestTypeDef",
     "CustomActionNavigationOperationTypeDef",
     "CustomValuesConfigurationOutputTypeDef",
-    "CustomValuesConfigurationTypeDef",
     "CustomSqlOutputTypeDef",
     "CustomSqlTypeDef",
     "RelationalTableOutputTypeDef",
     "RelationalTableTypeDef",
     "SearchDashboardsRequestRequestTypeDef",
     "ListDashboardsResponseTypeDef",
     "SearchDashboardsResponseTypeDef",
@@ -837,41 +814,54 @@
     "PivotTableDataPathOptionTypeDef",
     "PivotTableFieldCollapseStateTargetOutputTypeDef",
     "PivotTableFieldCollapseStateTargetTypeDef",
     "SearchDataSetsRequestRequestTypeDef",
     "SearchDataSourcesRequestRequestTypeDef",
     "SearchDataSourcesResponseTypeDef",
     "DateTimeDatasetParameterOutputTypeDef",
-    "DateTimeDatasetParameterTypeDef",
     "TimeRangeFilterValueOutputTypeDef",
     "TimeRangeFilterValueTypeDef",
     "DecimalDatasetParameterOutputTypeDef",
     "DecimalDatasetParameterTypeDef",
+    "DescribeAnalysisPermissionsResponseTypeDef",
+    "DescribeDataSetPermissionsResponseTypeDef",
+    "DescribeDataSourcePermissionsResponseTypeDef",
+    "DescribeFolderPermissionsResponseTypeDef",
+    "DescribeFolderResolvedPermissionsResponseTypeDef",
+    "DescribeTemplatePermissionsResponseTypeDef",
+    "DescribeThemePermissionsResponseTypeDef",
+    "DescribeTopicPermissionsResponseTypeDef",
+    "LinkSharingConfigurationTypeDef",
+    "UpdateAnalysisPermissionsResponseTypeDef",
+    "UpdateFolderPermissionsResponseTypeDef",
+    "UpdateTemplatePermissionsResponseTypeDef",
+    "UpdateThemePermissionsResponseTypeDef",
+    "UpdateTopicPermissionsResponseTypeDef",
     "DescribeFolderResponseTypeDef",
     "DescribeIAMPolicyAssignmentResponseTypeDef",
     "DescribeTopicRefreshResponseTypeDef",
     "DescribeTopicRefreshScheduleResponseTypeDef",
     "TopicRefreshScheduleSummaryTypeDef",
     "DescribeUserResponseTypeDef",
     "ListUsersResponseTypeDef",
     "RegisterUserResponseTypeDef",
     "UpdateUserResponseTypeDef",
     "DisplayFormatOptionsTypeDef",
     "DonutOptionsTypeDef",
     "RelativeDatesFilterTypeDef",
+    "FieldFolderUnionTypeDef",
     "FilterOperationTargetVisualsConfigurationOutputTypeDef",
     "FilterOperationTargetVisualsConfigurationTypeDef",
     "SearchFoldersRequestRequestTypeDef",
     "ListFoldersResponseTypeDef",
     "SearchFoldersResponseTypeDef",
     "FontConfigurationTypeDef",
     "TypographyOutputTypeDef",
     "TypographyTypeDef",
     "ForecastScenarioOutputTypeDef",
-    "ForecastScenarioTypeDef",
     "FreeFormLayoutCanvasSizeOptionsTypeDef",
     "SnapshotAnonymousUserTypeDef",
     "GeospatialWindowOptionsTypeDef",
     "GeospatialHeatmapColorScaleOutputTypeDef",
     "GeospatialHeatmapColorScaleTypeDef",
     "TableSideBorderOptionsTypeDef",
     "GradientColorOutputTypeDef",
@@ -922,25 +912,24 @@
     "TileLayoutStyleTypeDef",
     "NamedEntityDefinitionOutputTypeDef",
     "NamedEntityDefinitionTypeDef",
     "NamespaceInfoV2TypeDef",
     "VPCConnectionSummaryTypeDef",
     "VPCConnectionTypeDef",
     "OverrideDatasetParameterOperationOutputTypeDef",
-    "OverrideDatasetParameterOperationTypeDef",
     "NumericSeparatorConfigurationTypeDef",
     "NumericalAggregationFunctionTypeDef",
     "ParametersOutputTypeDef",
-    "ParametersTypeDef",
     "VisibleRangeOptionsTypeDef",
     "RadarChartSeriesSettingsTypeDef",
     "TopicRangeFilterConstantTypeDef",
     "RefreshFrequencyTypeDef",
     "RegisteredUserConsoleFeatureConfigurationsTypeDef",
     "RegisteredUserDashboardFeatureConfigurationsTypeDef",
+    "ResourcePermissionUnionTypeDef",
     "RowLevelPermissionTagConfigurationOutputTypeDef",
     "RowLevelPermissionTagConfigurationTypeDef",
     "SnapshotS3DestinationConfigurationTypeDef",
     "S3SourceOutputTypeDef",
     "S3SourceTypeDef",
     "SectionPageBreakConfigurationTypeDef",
     "SectionBasedLayoutPaperCanvasSizeOptionsTypeDef",
@@ -964,61 +953,69 @@
     "DecimalDefaultValuesOutputTypeDef",
     "DecimalDefaultValuesTypeDef",
     "IntegerDefaultValuesOutputTypeDef",
     "IntegerDefaultValuesTypeDef",
     "StringDefaultValuesOutputTypeDef",
     "StringDefaultValuesTypeDef",
     "DrillDownFilterOutputTypeDef",
-    "DrillDownFilterTypeDef",
     "AnalysisTypeDef",
     "DashboardVersionTypeDef",
     "AnalysisSourceEntityTypeDef",
     "DashboardSourceEntityTypeDef",
     "TemplateSourceEntityTypeDef",
     "AnonymousUserEmbeddingExperienceConfigurationTypeDef",
     "DescribeAssetBundleExportJobResponseTypeDef",
+    "AssetBundleCloudFormationOverridePropertyConfigurationUnionTypeDef",
     "StartAssetBundleExportJobRequestRequestTypeDef",
+    "CustomValuesConfigurationTypeDef",
+    "DateTimeDatasetParameterTypeDef",
+    "ParametersTypeDef",
+    "OverrideDatasetParameterOperationTypeDef",
+    "DrillDownFilterTypeDef",
+    "CreateTopicRefreshScheduleRequestRequestTypeDef",
+    "TopicRefreshScheduleUnionTypeDef",
+    "UpdateTopicRefreshScheduleRequestRequestTypeDef",
+    "ForecastScenarioTypeDef",
     "NumericAxisOptionsOutputTypeDef",
     "NumericAxisOptionsTypeDef",
     "CategoryFilterOutputTypeDef",
     "CategoryFilterTypeDef",
     "ClusterMarkerConfigurationTypeDef",
     "TopicCategoryFilterOutputTypeDef",
     "TopicCategoryFilterTypeDef",
     "TagColumnOperationOutputTypeDef",
     "TagColumnOperationTypeDef",
+    "ColumnGroupUnionTypeDef",
     "DataSetConfigurationOutputTypeDef",
     "DataSetConfigurationTypeDef",
     "ConditionalFormattingIconTypeDef",
-    "DescribeDashboardPermissionsResponseTypeDef",
-    "UpdateDashboardPermissionsResponseTypeDef",
     "ListDataSetsResponseTypeDef",
     "SearchDataSetsResponseTypeDef",
     "DestinationParameterValueConfigurationOutputTypeDef",
-    "DestinationParameterValueConfigurationTypeDef",
     "DashboardPublishOptionsTypeDef",
     "VisualPaletteOutputTypeDef",
     "VisualPaletteTypeDef",
     "PivotTableFieldCollapseStateOptionOutputTypeDef",
     "PivotTableFieldCollapseStateOptionTypeDef",
     "TimeRangeFilterOutputTypeDef",
     "TimeRangeFilterTypeDef",
+    "DescribeDashboardPermissionsResponseTypeDef",
+    "UpdateDashboardPermissionsResponseTypeDef",
     "ListTopicRefreshSchedulesResponseTypeDef",
     "DefaultFormattingTypeDef",
     "CustomActionFilterOperationOutputTypeDef",
     "CustomActionFilterOperationTypeDef",
     "AxisLabelOptionsTypeDef",
     "DataLabelOptionsOutputTypeDef",
     "DataLabelOptionsTypeDef",
     "FunnelChartDataLabelOptionsTypeDef",
     "LabelOptionsTypeDef",
     "PanelTitleOptionsTypeDef",
     "TableFieldCustomTextContentTypeDef",
     "ForecastConfigurationOutputTypeDef",
-    "ForecastConfigurationTypeDef",
     "DefaultFreeFormLayoutConfigurationTypeDef",
     "SnapshotUserConfigurationTypeDef",
     "GeospatialHeatmapConfigurationOutputTypeDef",
     "GeospatialHeatmapConfigurationTypeDef",
     "GlobalTableBorderOptionsTypeDef",
     "ConditionalFormattingGradientColorOutputTypeDef",
     "ConditionalFormattingGradientColorTypeDef",
@@ -1046,52 +1043,64 @@
     "ScrollBarOptionsTypeDef",
     "TopicDateRangeFilterTypeDef",
     "TopicNumericRangeFilterTypeDef",
     "RefreshScheduleOutputTypeDef",
     "RefreshScheduleTypeDef",
     "RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef",
     "RegisteredUserDashboardEmbeddingConfigurationTypeDef",
+    "CreateFolderRequestRequestTypeDef",
+    "UpdateAnalysisPermissionsRequestRequestTypeDef",
+    "UpdateDashboardPermissionsRequestRequestTypeDef",
+    "UpdateDataSetPermissionsRequestRequestTypeDef",
+    "UpdateDataSourcePermissionsRequestRequestTypeDef",
+    "UpdateFolderPermissionsRequestRequestTypeDef",
+    "UpdateTemplatePermissionsRequestRequestTypeDef",
+    "UpdateThemePermissionsRequestRequestTypeDef",
+    "UpdateTopicPermissionsRequestRequestTypeDef",
+    "RowLevelPermissionTagConfigurationUnionTypeDef",
     "SnapshotDestinationConfigurationOutputTypeDef",
     "SnapshotDestinationConfigurationTypeDef",
     "SnapshotJobS3ResultTypeDef",
     "PhysicalTableOutputTypeDef",
     "PhysicalTableTypeDef",
     "SectionBasedLayoutCanvasSizeOptionsTypeDef",
     "FilterScopeConfigurationOutputTypeDef",
     "FilterScopeConfigurationTypeDef",
     "FreeFormLayoutElementOutputTypeDef",
     "FreeFormLayoutElementTypeDef",
     "SnapshotFileGroupOutputTypeDef",
     "SnapshotFileGroupTypeDef",
     "DatasetParameterOutputTypeDef",
-    "DatasetParameterTypeDef",
     "DateTimeParameterDeclarationOutputTypeDef",
     "DateTimeParameterDeclarationTypeDef",
     "DecimalParameterDeclarationOutputTypeDef",
     "DecimalParameterDeclarationTypeDef",
     "IntegerParameterDeclarationOutputTypeDef",
     "IntegerParameterDeclarationTypeDef",
     "StringParameterDeclarationOutputTypeDef",
     "StringParameterDeclarationTypeDef",
     "DateTimeHierarchyOutputTypeDef",
     "ExplicitHierarchyOutputTypeDef",
     "PredefinedHierarchyOutputTypeDef",
-    "DateTimeHierarchyTypeDef",
-    "ExplicitHierarchyTypeDef",
-    "PredefinedHierarchyTypeDef",
     "DescribeAnalysisResponseTypeDef",
     "DashboardTypeDef",
     "GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef",
+    "DestinationParameterValueConfigurationTypeDef",
+    "DatasetParameterTypeDef",
+    "ParametersUnionTypeDef",
+    "DateTimeHierarchyTypeDef",
+    "ExplicitHierarchyTypeDef",
+    "PredefinedHierarchyTypeDef",
+    "ForecastConfigurationTypeDef",
     "AxisDataOptionsOutputTypeDef",
     "AxisDataOptionsTypeDef",
     "TransformOperationOutputTypeDef",
     "TransformOperationTypeDef",
     "TemplateVersionTypeDef",
     "SetParameterValueConfigurationOutputTypeDef",
-    "SetParameterValueConfigurationTypeDef",
     "PivotTableFieldOptionsOutputTypeDef",
     "PivotTableFieldOptionsTypeDef",
     "TopicCalculatedFieldOutputTypeDef",
     "TopicCalculatedFieldTypeDef",
     "TopicColumnOutputTypeDef",
     "TopicColumnTypeDef",
     "ChartAxisLabelOptionsOutputTypeDef",
@@ -1131,34 +1140,37 @@
     "NumericRangeFilterTypeDef",
     "ReferenceLineDynamicDataConfigurationTypeDef",
     "TopicFilterOutputTypeDef",
     "TopicFilterTypeDef",
     "DescribeRefreshScheduleResponseTypeDef",
     "ListRefreshSchedulesResponseTypeDef",
     "CreateRefreshScheduleRequestRequestTypeDef",
+    "RefreshScheduleUnionTypeDef",
     "UpdateRefreshScheduleRequestRequestTypeDef",
     "RegisteredUserEmbeddingExperienceConfigurationTypeDef",
     "SnapshotJobResultFileGroupTypeDef",
+    "PhysicalTableUnionTypeDef",
     "DefaultSectionBasedLayoutConfigurationTypeDef",
     "FreeFormLayoutConfigurationOutputTypeDef",
     "FreeFormSectionLayoutConfigurationOutputTypeDef",
     "FreeFormLayoutConfigurationTypeDef",
     "FreeFormSectionLayoutConfigurationTypeDef",
     "SnapshotConfigurationOutputTypeDef",
     "SnapshotConfigurationTypeDef",
     "ParameterDeclarationOutputTypeDef",
     "ParameterDeclarationTypeDef",
     "ColumnHierarchyOutputTypeDef",
-    "ColumnHierarchyTypeDef",
     "DescribeDashboardResponseTypeDef",
+    "SetParameterValueConfigurationTypeDef",
+    "DatasetParameterUnionTypeDef",
+    "ColumnHierarchyTypeDef",
     "LogicalTableOutputTypeDef",
     "LogicalTableTypeDef",
     "TemplateTypeDef",
     "CustomActionSetParametersOperationOutputTypeDef",
-    "CustomActionSetParametersOperationTypeDef",
     "AxisDisplayOptionsOutputTypeDef",
     "AxisDisplayOptionsTypeDef",
     "FilterDateTimePickerControlTypeDef",
     "ParameterDateTimePickerControlTypeDef",
     "FilterDropDownControlOutputTypeDef",
     "FilterDropDownControlTypeDef",
     "ParameterDropDownControlOutputTypeDef",
@@ -1205,14 +1217,15 @@
     "AssetBundleImportJobOverrideParametersOutputTypeDef",
     "AssetBundleImportJobOverrideParametersTypeDef",
     "DataSourceCredentialsTypeDef",
     "DescribeDataSourceResponseTypeDef",
     "ListDataSourcesResponseTypeDef",
     "ThemeVersionTypeDef",
     "CreateThemeRequestRequestTypeDef",
+    "ThemeConfigurationUnionTypeDef",
     "UpdateThemeRequestRequestTypeDef",
     "ComparisonConfigurationTypeDef",
     "DateTimeFormatConfigurationTypeDef",
     "NumberFormatConfigurationTypeDef",
     "ReferenceLineValueLabelConfigurationTypeDef",
     "StringFormatConfigurationTypeDef",
     "TopBottomFilterOutputTypeDef",
@@ -1226,21 +1239,21 @@
     "DatasetMetadataTypeDef",
     "GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef",
     "AnonymousUserSnapshotJobResultTypeDef",
     "DefaultPaginatedLayoutConfigurationTypeDef",
     "SectionLayoutConfigurationOutputTypeDef",
     "SectionLayoutConfigurationTypeDef",
     "DescribeDashboardSnapshotJobResponseTypeDef",
+    "SnapshotConfigurationUnionTypeDef",
     "StartDashboardSnapshotJobRequestRequestTypeDef",
+    "CustomActionSetParametersOperationTypeDef",
     "DataSetTypeDef",
-    "CreateDataSetRequestRequestTypeDef",
-    "UpdateDataSetRequestRequestTypeDef",
+    "LogicalTableUnionTypeDef",
     "DescribeTemplateResponseTypeDef",
     "VisualCustomActionOperationOutputTypeDef",
-    "VisualCustomActionOperationTypeDef",
     "LineSeriesAxisDisplayOptionsOutputTypeDef",
     "LineSeriesAxisDisplayOptionsTypeDef",
     "FilterControlOutputTypeDef",
     "FilterControlTypeDef",
     "ParameterControlOutputTypeDef",
     "ParameterControlTypeDef",
     "TableFieldURLConfigurationTypeDef",
@@ -1253,14 +1266,15 @@
     "TableCellConditionalFormattingOutputTypeDef",
     "GaugeChartConditionalFormattingOptionTypeDef",
     "KPIConditionalFormattingOptionTypeDef",
     "FilledMapShapeConditionalFormattingTypeDef",
     "PivotTableCellConditionalFormattingTypeDef",
     "TableCellConditionalFormattingTypeDef",
     "DescribeAssetBundleImportJobResponseTypeDef",
+    "AssetBundleImportJobOverrideParametersUnionTypeDef",
     "StartAssetBundleImportJobRequestRequestTypeDef",
     "CreateDataSourceRequestRequestTypeDef",
     "UpdateDataSourceRequestRequestTypeDef",
     "ThemeTypeDef",
     "GaugeChartOptionsTypeDef",
     "KPIOptionsTypeDef",
     "DateDimensionFieldTypeDef",
@@ -1311,17 +1325,19 @@
     "TopicDetailsTypeDef",
     "SnapshotJobResultTypeDef",
     "DefaultNewSheetConfigurationTypeDef",
     "BodySectionContentOutputTypeDef",
     "HeaderFooterSectionConfigurationOutputTypeDef",
     "BodySectionContentTypeDef",
     "HeaderFooterSectionConfigurationTypeDef",
+    "VisualCustomActionOperationTypeDef",
     "DescribeDataSetResponseTypeDef",
+    "CreateDataSetRequestRequestTypeDef",
+    "UpdateDataSetRequestRequestTypeDef",
     "VisualCustomActionOutputTypeDef",
-    "VisualCustomActionTypeDef",
     "TableFieldOptionTypeDef",
     "GaugeChartConditionalFormattingOutputTypeDef",
     "KPIConditionalFormattingOutputTypeDef",
     "FilledMapConditionalFormattingOptionOutputTypeDef",
     "PivotTableConditionalFormattingOptionOutputTypeDef",
     "TableConditionalFormattingOptionOutputTypeDef",
     "GaugeChartConditionalFormattingTypeDef",
@@ -1340,23 +1356,23 @@
     "FilterGroupTypeDef",
     "PivotTableSortConfigurationOutputTypeDef",
     "PivotTableSortConfigurationTypeDef",
     "TooltipOptionsOutputTypeDef",
     "TooltipOptionsTypeDef",
     "DescribeTopicResponseTypeDef",
     "CreateTopicRequestRequestTypeDef",
+    "TopicDetailsUnionTypeDef",
     "UpdateTopicRequestRequestTypeDef",
     "DescribeDashboardSnapshotJobResultResponseTypeDef",
     "AnalysisDefaultsTypeDef",
     "BodySectionConfigurationOutputTypeDef",
     "BodySectionConfigurationTypeDef",
+    "VisualCustomActionTypeDef",
     "CustomContentVisualOutputTypeDef",
     "EmptyVisualOutputTypeDef",
-    "CustomContentVisualTypeDef",
-    "EmptyVisualTypeDef",
     "TableFieldOptionsOutputTypeDef",
     "TableFieldOptionsTypeDef",
     "FilledMapConditionalFormattingOutputTypeDef",
     "PivotTableConditionalFormattingOutputTypeDef",
     "TableConditionalFormattingOutputTypeDef",
     "FilledMapConditionalFormattingTypeDef",
     "PivotTableConditionalFormattingTypeDef",
@@ -1413,14 +1429,16 @@
     "WaterfallChartAggregatedFieldWellsTypeDef",
     "WordCloudAggregatedFieldWellsOutputTypeDef",
     "WordCloudAggregatedFieldWellsTypeDef",
     "TableUnaggregatedFieldWellsOutputTypeDef",
     "TableUnaggregatedFieldWellsTypeDef",
     "SectionBasedLayoutConfigurationOutputTypeDef",
     "SectionBasedLayoutConfigurationTypeDef",
+    "CustomContentVisualTypeDef",
+    "EmptyVisualTypeDef",
     "BarChartFieldWellsOutputTypeDef",
     "BarChartFieldWellsTypeDef",
     "BoxPlotFieldWellsOutputTypeDef",
     "BoxPlotFieldWellsTypeDef",
     "ComboChartFieldWellsOutputTypeDef",
     "ComboChartFieldWellsTypeDef",
     "FilledMapFieldWellsOutputTypeDef",
@@ -1551,19 +1569,22 @@
     "TemplateVersionDefinitionOutputTypeDef",
     "AnalysisDefinitionTypeDef",
     "DashboardVersionDefinitionTypeDef",
     "TemplateVersionDefinitionTypeDef",
     "DescribeAnalysisDefinitionResponseTypeDef",
     "DescribeDashboardDefinitionResponseTypeDef",
     "DescribeTemplateDefinitionResponseTypeDef",
+    "AnalysisDefinitionUnionTypeDef",
     "CreateAnalysisRequestRequestTypeDef",
     "UpdateAnalysisRequestRequestTypeDef",
     "CreateDashboardRequestRequestTypeDef",
+    "DashboardVersionDefinitionUnionTypeDef",
     "UpdateDashboardRequestRequestTypeDef",
     "CreateTemplateRequestRequestTypeDef",
+    "TemplateVersionDefinitionUnionTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
 )
 
 AccountCustomizationTypeDef = TypedDict(
     "AccountCustomizationTypeDef",
     {
         "DefaultTheme": str,
@@ -2281,37 +2302,14 @@
 class AssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef(
     _RequiredAssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef,
     _OptionalAssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef,
 ):
     pass
 
 
-_RequiredAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef = TypedDict(
-    "_RequiredAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
-    {
-        "DataSetId": str,
-        "ScheduleId": str,
-    },
-)
-_OptionalAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef = TypedDict(
-    "_OptionalAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
-    {
-        "StartAfterDateTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef(
-    _RequiredAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef,
-    _OptionalAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef,
-):
-    pass
-
-
 _RequiredAssetBundleImportJobVPCConnectionOverrideParametersTypeDef = TypedDict(
     "_RequiredAssetBundleImportJobVPCConnectionOverrideParametersTypeDef",
     {
         "VPCConnectionId": str,
     },
 )
 _OptionalAssetBundleImportJobVPCConnectionOverrideParametersTypeDef = TypedDict(
@@ -2330,14 +2328,15 @@
 class AssetBundleImportJobVPCConnectionOverrideParametersTypeDef(
     _RequiredAssetBundleImportJobVPCConnectionOverrideParametersTypeDef,
     _OptionalAssetBundleImportJobVPCConnectionOverrideParametersTypeDef,
 ):
     pass
 
 
+TimestampTypeDef = Union[datetime, str]
 AssetBundleImportJobSummaryTypeDef = TypedDict(
     "AssetBundleImportJobSummaryTypeDef",
     {
         "JobStatus": AssetBundleImportJobStatusType,
         "Arn": str,
         "CreatedTime": datetime,
         "AssetBundleImportJobId": str,
@@ -2351,23 +2350,15 @@
     {
         "Body": str,
         "S3Uri": str,
     },
     total=False,
 )
 
-AssetBundleImportSourceTypeDef = TypedDict(
-    "AssetBundleImportSourceTypeDef",
-    {
-        "Body": Union[str, bytes, IO[Any], StreamingBody],
-        "S3Uri": str,
-    },
-    total=False,
-)
-
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 AthenaParametersTypeDef = TypedDict(
     "AthenaParametersTypeDef",
     {
         "WorkGroup": str,
         "RoleArn": str,
     },
     total=False,
@@ -2951,57 +2942,23 @@
         "userLoginName": str,
         "accountName": str,
         "directoryType": str,
     },
     total=False,
 )
 
-ResourcePermissionOutputTypeDef = TypedDict(
-    "ResourcePermissionOutputTypeDef",
-    {
-        "Principal": str,
-        "Actions": List[str],
-    },
-)
-
-ResourcePermissionTypeDef = TypedDict(
-    "ResourcePermissionTypeDef",
-    {
-        "Principal": str,
-        "Actions": Sequence[str],
-    },
-)
-
 DataSetUsageConfigurationTypeDef = TypedDict(
     "DataSetUsageConfigurationTypeDef",
     {
         "DisableUseAsDirectQuerySource": bool,
         "DisableUseAsImportedSource": bool,
     },
     total=False,
 )
 
-FieldFolderOutputTypeDef = TypedDict(
-    "FieldFolderOutputTypeDef",
-    {
-        "description": str,
-        "columns": List[str],
-    },
-    total=False,
-)
-
-FieldFolderTypeDef = TypedDict(
-    "FieldFolderTypeDef",
-    {
-        "description": str,
-        "columns": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredRowLevelPermissionDataSetTypeDef = TypedDict(
     "_RequiredRowLevelPermissionDataSetTypeDef",
     {
         "Arn": str,
         "PermissionPolicy": RowLevelPermissionPolicyType,
     },
 )
@@ -3179,39 +3136,14 @@
         "Arn": str,
         "AliasName": str,
         "ThemeVersionNumber": int,
     },
     total=False,
 )
 
-_RequiredTopicRefreshScheduleTypeDef = TypedDict(
-    "_RequiredTopicRefreshScheduleTypeDef",
-    {
-        "IsEnabled": bool,
-        "BasedOnSpiceSchedule": bool,
-    },
-)
-_OptionalTopicRefreshScheduleTypeDef = TypedDict(
-    "_OptionalTopicRefreshScheduleTypeDef",
-    {
-        "StartingAt": Union[datetime, str],
-        "Timezone": str,
-        "RepeatAt": str,
-        "TopicScheduleType": TopicScheduleTypeType,
-    },
-    total=False,
-)
-
-
-class TopicRefreshScheduleTypeDef(
-    _RequiredTopicRefreshScheduleTypeDef, _OptionalTopicRefreshScheduleTypeDef
-):
-    pass
-
-
 DecimalPlacesConfigurationTypeDef = TypedDict(
     "DecimalPlacesConfigurationTypeDef",
     {
         "DecimalPlaces": int,
     },
 )
 
@@ -3268,25 +3200,14 @@
         "IntegerValues": List[int],
         "DecimalValues": List[float],
         "DateTimeValues": List[datetime],
     },
     total=False,
 )
 
-CustomParameterValuesTypeDef = TypedDict(
-    "CustomParameterValuesTypeDef",
-    {
-        "StringValues": Sequence[str],
-        "IntegerValues": Sequence[int],
-        "DecimalValues": Sequence[float],
-        "DateTimeValues": Sequence[Union[datetime, str]],
-    },
-    total=False,
-)
-
 InputColumnTypeDef = TypedDict(
     "InputColumnTypeDef",
     {
         "Name": str,
         "Type": InputColumnDataTypeType,
     },
 )
@@ -3525,14 +3446,23 @@
     {
         "Operator": FilterOperatorType,
         "Name": DataSetFilterAttributeType,
         "Value": str,
     },
 )
 
+FieldFolderOutputTypeDef = TypedDict(
+    "FieldFolderOutputTypeDef",
+    {
+        "description": str,
+        "columns": List[str],
+    },
+    total=False,
+)
+
 OutputColumnTypeDef = TypedDict(
     "OutputColumnTypeDef",
     {
         "Name": str,
         "Description": str,
         "Type": ColumnDataTypeType,
     },
@@ -3724,22 +3654,14 @@
     "DateTimeDatasetParameterDefaultValuesOutputTypeDef",
     {
         "StaticValues": List[datetime],
     },
     total=False,
 )
 
-DateTimeDatasetParameterDefaultValuesTypeDef = TypedDict(
-    "DateTimeDatasetParameterDefaultValuesTypeDef",
-    {
-        "StaticValues": Sequence[Union[datetime, str]],
-    },
-    total=False,
-)
-
 _RequiredRollingDateConfigurationTypeDef = TypedDict(
     "_RequiredRollingDateConfigurationTypeDef",
     {
         "Expression": str,
     },
 )
 _OptionalRollingDateConfigurationTypeDef = TypedDict(
@@ -3770,39 +3692,22 @@
     "MappedDataSetParameterTypeDef",
     {
         "DataSetIdentifier": str,
         "DataSetParameterName": str,
     },
 )
 
-DateTimeValueWhenUnsetConfigurationTypeDef = TypedDict(
-    "DateTimeValueWhenUnsetConfigurationTypeDef",
-    {
-        "ValueWhenUnsetOption": ValueWhenUnsetOptionType,
-        "CustomValue": Union[datetime, str],
-    },
-    total=False,
-)
-
 DateTimeParameterOutputTypeDef = TypedDict(
     "DateTimeParameterOutputTypeDef",
     {
         "Name": str,
         "Values": List[datetime],
     },
 )
 
-DateTimeParameterTypeDef = TypedDict(
-    "DateTimeParameterTypeDef",
-    {
-        "Name": str,
-        "Values": Sequence[Union[datetime, str]],
-    },
-)
-
 SheetControlInfoIconLabelOptionsTypeDef = TypedDict(
     "SheetControlInfoIconLabelOptionsTypeDef",
     {
         "Visibility": VisibilityType,
         "InfoIconText": str,
     },
     total=False,
@@ -4164,14 +4069,22 @@
     "DescribeAnalysisPermissionsRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
     },
 )
 
+ResourcePermissionOutputTypeDef = TypedDict(
+    "ResourcePermissionOutputTypeDef",
+    {
+        "Principal": str,
+        "Actions": List[str],
+    },
+)
+
 DescribeAnalysisRequestRequestTypeDef = TypedDict(
     "DescribeAnalysisRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
     },
 )
@@ -4686,14 +4599,23 @@
 
 class ExcludePeriodConfigurationTypeDef(
     _RequiredExcludePeriodConfigurationTypeDef, _OptionalExcludePeriodConfigurationTypeDef
 ):
     pass
 
 
+FieldFolderTypeDef = TypedDict(
+    "FieldFolderTypeDef",
+    {
+        "description": str,
+        "columns": Sequence[str],
+    },
+    total=False,
+)
+
 FieldSortTypeDef = TypedDict(
     "FieldSortTypeDef",
     {
         "FieldId": str,
         "Direction": SortDirectionType,
     },
 )
@@ -4840,31 +4762,14 @@
     {
         "StartDate": datetime,
         "EndDate": datetime,
         "Value": float,
     },
 )
 
-WhatIfPointScenarioTypeDef = TypedDict(
-    "WhatIfPointScenarioTypeDef",
-    {
-        "Date": Union[datetime, str],
-        "Value": float,
-    },
-)
-
-WhatIfRangeScenarioTypeDef = TypedDict(
-    "WhatIfRangeScenarioTypeDef",
-    {
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "Value": float,
-    },
-)
-
 FreeFormLayoutScreenCanvasSizeOptionsTypeDef = TypedDict(
     "FreeFormLayoutScreenCanvasSizeOptionsTypeDef",
     {
         "OptimizedViewPortWidth": str,
     },
 )
 
@@ -5964,25 +5869,14 @@
         "DecimalStaticValues": List[float],
         "DateTimeStaticValues": List[datetime],
         "IntegerStaticValues": List[int],
     },
     total=False,
 )
 
-NewDefaultValuesTypeDef = TypedDict(
-    "NewDefaultValuesTypeDef",
-    {
-        "StringStaticValues": Sequence[str],
-        "DecimalStaticValues": Sequence[float],
-        "DateTimeStaticValues": Sequence[Union[datetime, str]],
-        "IntegerStaticValues": Sequence[int],
-    },
-    total=False,
-)
-
 NumericRangeFilterValueTypeDef = TypedDict(
     "NumericRangeFilterValueTypeDef",
     {
         "StaticValue": float,
         "Parameter": str,
     },
     total=False,
@@ -6208,14 +6102,22 @@
     "RenameColumnOperationTypeDef",
     {
         "ColumnName": str,
         "NewColumnName": str,
     },
 )
 
+ResourcePermissionTypeDef = TypedDict(
+    "ResourcePermissionTypeDef",
+    {
+        "Principal": str,
+        "Actions": Sequence[str],
+    },
+)
+
 RestoreAnalysisRequestRequestTypeDef = TypedDict(
     "RestoreAnalysisRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
     },
 )
@@ -7006,58 +6908,24 @@
 
 class TimeEqualityFilterOutputTypeDef(
     _RequiredTimeEqualityFilterOutputTypeDef, _OptionalTimeEqualityFilterOutputTypeDef
 ):
     pass
 
 
-_RequiredTimeEqualityFilterTypeDef = TypedDict(
-    "_RequiredTimeEqualityFilterTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierTypeDef,
-    },
-)
-_OptionalTimeEqualityFilterTypeDef = TypedDict(
-    "_OptionalTimeEqualityFilterTypeDef",
-    {
-        "Value": Union[datetime, str],
-        "ParameterName": str,
-        "TimeGranularity": TimeGranularityType,
-    },
-    total=False,
-)
-
-
-class TimeEqualityFilterTypeDef(
-    _RequiredTimeEqualityFilterTypeDef, _OptionalTimeEqualityFilterTypeDef
-):
-    pass
-
-
 TimeRangeDrillDownFilterOutputTypeDef = TypedDict(
     "TimeRangeDrillDownFilterOutputTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
         "RangeMinimum": datetime,
         "RangeMaximum": datetime,
         "TimeGranularity": TimeGranularityType,
     },
 )
 
-TimeRangeDrillDownFilterTypeDef = TypedDict(
-    "TimeRangeDrillDownFilterTypeDef",
-    {
-        "Column": ColumnIdentifierTypeDef,
-        "RangeMinimum": Union[datetime, str],
-        "RangeMaximum": Union[datetime, str],
-        "TimeGranularity": TimeGranularityType,
-    },
-)
-
 AnalysisErrorTypeDef = TypedDict(
     "AnalysisErrorTypeDef",
     {
         "Type": AnalysisErrorTypeType,
         "Message": str,
         "ViolatedEntities": List[EntityTypeDef],
     },
@@ -7195,14 +7063,169 @@
     {
         "CredentialPair": AssetBundleImportJobDataSourceCredentialPairTypeDef,
         "SecretArn": str,
     },
     total=False,
 )
 
+_RequiredAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef = TypedDict(
+    "_RequiredAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
+    {
+        "DataSetId": str,
+        "ScheduleId": str,
+    },
+)
+_OptionalAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef = TypedDict(
+    "_OptionalAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
+    {
+        "StartAfterDateTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef(
+    _RequiredAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef,
+    _OptionalAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef,
+):
+    pass
+
+
+CustomParameterValuesTypeDef = TypedDict(
+    "CustomParameterValuesTypeDef",
+    {
+        "StringValues": Sequence[str],
+        "IntegerValues": Sequence[int],
+        "DecimalValues": Sequence[float],
+        "DateTimeValues": Sequence[TimestampTypeDef],
+    },
+    total=False,
+)
+
+DateTimeDatasetParameterDefaultValuesTypeDef = TypedDict(
+    "DateTimeDatasetParameterDefaultValuesTypeDef",
+    {
+        "StaticValues": Sequence[TimestampTypeDef],
+    },
+    total=False,
+)
+
+DateTimeParameterTypeDef = TypedDict(
+    "DateTimeParameterTypeDef",
+    {
+        "Name": str,
+        "Values": Sequence[TimestampTypeDef],
+    },
+)
+
+DateTimeValueWhenUnsetConfigurationTypeDef = TypedDict(
+    "DateTimeValueWhenUnsetConfigurationTypeDef",
+    {
+        "ValueWhenUnsetOption": ValueWhenUnsetOptionType,
+        "CustomValue": TimestampTypeDef,
+    },
+    total=False,
+)
+
+NewDefaultValuesTypeDef = TypedDict(
+    "NewDefaultValuesTypeDef",
+    {
+        "StringStaticValues": Sequence[str],
+        "DecimalStaticValues": Sequence[float],
+        "DateTimeStaticValues": Sequence[TimestampTypeDef],
+        "IntegerStaticValues": Sequence[int],
+    },
+    total=False,
+)
+
+_RequiredTimeEqualityFilterTypeDef = TypedDict(
+    "_RequiredTimeEqualityFilterTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+    },
+)
+_OptionalTimeEqualityFilterTypeDef = TypedDict(
+    "_OptionalTimeEqualityFilterTypeDef",
+    {
+        "Value": TimestampTypeDef,
+        "ParameterName": str,
+        "TimeGranularity": TimeGranularityType,
+    },
+    total=False,
+)
+
+
+class TimeEqualityFilterTypeDef(
+    _RequiredTimeEqualityFilterTypeDef, _OptionalTimeEqualityFilterTypeDef
+):
+    pass
+
+
+TimeRangeDrillDownFilterTypeDef = TypedDict(
+    "TimeRangeDrillDownFilterTypeDef",
+    {
+        "Column": ColumnIdentifierTypeDef,
+        "RangeMinimum": TimestampTypeDef,
+        "RangeMaximum": TimestampTypeDef,
+        "TimeGranularity": TimeGranularityType,
+    },
+)
+
+_RequiredTopicRefreshScheduleTypeDef = TypedDict(
+    "_RequiredTopicRefreshScheduleTypeDef",
+    {
+        "IsEnabled": bool,
+        "BasedOnSpiceSchedule": bool,
+    },
+)
+_OptionalTopicRefreshScheduleTypeDef = TypedDict(
+    "_OptionalTopicRefreshScheduleTypeDef",
+    {
+        "StartingAt": TimestampTypeDef,
+        "Timezone": str,
+        "RepeatAt": str,
+        "TopicScheduleType": TopicScheduleTypeType,
+    },
+    total=False,
+)
+
+
+class TopicRefreshScheduleTypeDef(
+    _RequiredTopicRefreshScheduleTypeDef, _OptionalTopicRefreshScheduleTypeDef
+):
+    pass
+
+
+WhatIfPointScenarioTypeDef = TypedDict(
+    "WhatIfPointScenarioTypeDef",
+    {
+        "Date": TimestampTypeDef,
+        "Value": float,
+    },
+)
+
+WhatIfRangeScenarioTypeDef = TypedDict(
+    "WhatIfRangeScenarioTypeDef",
+    {
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "Value": float,
+    },
+)
+
+AssetBundleImportSourceTypeDef = TypedDict(
+    "AssetBundleImportSourceTypeDef",
+    {
+        "Body": BlobTypeDef,
+        "S3Uri": str,
+    },
+    total=False,
+)
+
 AxisDisplayRangeOutputTypeDef = TypedDict(
     "AxisDisplayRangeOutputTypeDef",
     {
         "MinMax": AxisDisplayMinMaxRangeTypeDef,
         "DataDriven": Dict[str, Any],
     },
     total=False,
@@ -8286,14 +8309,17 @@
     "ColumnGroupTypeDef",
     {
         "GeoSpatialColumnGroup": GeoSpatialColumnGroupTypeDef,
     },
     total=False,
 )
 
+ColumnLevelPermissionRuleUnionTypeDef = Union[
+    ColumnLevelPermissionRuleTypeDef, ColumnLevelPermissionRuleOutputTypeDef
+]
 DataSetSchemaOutputTypeDef = TypedDict(
     "DataSetSchemaOutputTypeDef",
     {
         "ColumnSchemaList": List[ColumnSchemaTypeDef],
     },
     total=False,
 )
@@ -8429,434 +8455,14 @@
         "SignupResponse": SignupResponseTypeDef,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAnalysisPermissionsResponseTypeDef = TypedDict(
-    "DescribeAnalysisPermissionsResponseTypeDef",
-    {
-        "AnalysisId": str,
-        "AnalysisArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDataSetPermissionsResponseTypeDef = TypedDict(
-    "DescribeDataSetPermissionsResponseTypeDef",
-    {
-        "DataSetArn": str,
-        "DataSetId": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDataSourcePermissionsResponseTypeDef = TypedDict(
-    "DescribeDataSourcePermissionsResponseTypeDef",
-    {
-        "DataSourceArn": str,
-        "DataSourceId": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFolderPermissionsResponseTypeDef = TypedDict(
-    "DescribeFolderPermissionsResponseTypeDef",
-    {
-        "Status": int,
-        "FolderId": str,
-        "Arn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFolderResolvedPermissionsResponseTypeDef = TypedDict(
-    "DescribeFolderResolvedPermissionsResponseTypeDef",
-    {
-        "Status": int,
-        "FolderId": str,
-        "Arn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeTemplatePermissionsResponseTypeDef = TypedDict(
-    "DescribeTemplatePermissionsResponseTypeDef",
-    {
-        "TemplateId": str,
-        "TemplateArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeThemePermissionsResponseTypeDef = TypedDict(
-    "DescribeThemePermissionsResponseTypeDef",
-    {
-        "ThemeId": str,
-        "ThemeArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeTopicPermissionsResponseTypeDef = TypedDict(
-    "DescribeTopicPermissionsResponseTypeDef",
-    {
-        "TopicId": str,
-        "TopicArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LinkSharingConfigurationTypeDef = TypedDict(
-    "LinkSharingConfigurationTypeDef",
-    {
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-    },
-    total=False,
-)
-
-UpdateAnalysisPermissionsResponseTypeDef = TypedDict(
-    "UpdateAnalysisPermissionsResponseTypeDef",
-    {
-        "AnalysisArn": str,
-        "AnalysisId": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateFolderPermissionsResponseTypeDef = TypedDict(
-    "UpdateFolderPermissionsResponseTypeDef",
-    {
-        "Status": int,
-        "Arn": str,
-        "FolderId": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTemplatePermissionsResponseTypeDef = TypedDict(
-    "UpdateTemplatePermissionsResponseTypeDef",
-    {
-        "TemplateId": str,
-        "TemplateArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateThemePermissionsResponseTypeDef = TypedDict(
-    "UpdateThemePermissionsResponseTypeDef",
-    {
-        "ThemeId": str,
-        "ThemeArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTopicPermissionsResponseTypeDef = TypedDict(
-    "UpdateTopicPermissionsResponseTypeDef",
-    {
-        "TopicId": str,
-        "TopicArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredCreateFolderRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFolderRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "FolderId": str,
-    },
-)
-_OptionalCreateFolderRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFolderRequestRequestTypeDef",
-    {
-        "Name": str,
-        "FolderType": Literal["SHARED"],
-        "ParentFolderArn": str,
-        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateFolderRequestRequestTypeDef(
-    _RequiredCreateFolderRequestRequestTypeDef, _OptionalCreateFolderRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateAnalysisPermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAnalysisPermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "AnalysisId": str,
-    },
-)
-_OptionalUpdateAnalysisPermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAnalysisPermissionsRequestRequestTypeDef",
-    {
-        "GrantPermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-        "RevokePermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-
-class UpdateAnalysisPermissionsRequestRequestTypeDef(
-    _RequiredUpdateAnalysisPermissionsRequestRequestTypeDef,
-    _OptionalUpdateAnalysisPermissionsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateDashboardPermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDashboardPermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "DashboardId": str,
-    },
-)
-_OptionalUpdateDashboardPermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDashboardPermissionsRequestRequestTypeDef",
-    {
-        "GrantPermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-        "RevokePermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-        "GrantLinkPermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-        "RevokeLinkPermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-
-class UpdateDashboardPermissionsRequestRequestTypeDef(
-    _RequiredUpdateDashboardPermissionsRequestRequestTypeDef,
-    _OptionalUpdateDashboardPermissionsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateDataSetPermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDataSetPermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "DataSetId": str,
-    },
-)
-_OptionalUpdateDataSetPermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDataSetPermissionsRequestRequestTypeDef",
-    {
-        "GrantPermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-        "RevokePermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-
-class UpdateDataSetPermissionsRequestRequestTypeDef(
-    _RequiredUpdateDataSetPermissionsRequestRequestTypeDef,
-    _OptionalUpdateDataSetPermissionsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateDataSourcePermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDataSourcePermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "DataSourceId": str,
-    },
-)
-_OptionalUpdateDataSourcePermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDataSourcePermissionsRequestRequestTypeDef",
-    {
-        "GrantPermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-        "RevokePermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-
-class UpdateDataSourcePermissionsRequestRequestTypeDef(
-    _RequiredUpdateDataSourcePermissionsRequestRequestTypeDef,
-    _OptionalUpdateDataSourcePermissionsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateFolderPermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFolderPermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "FolderId": str,
-    },
-)
-_OptionalUpdateFolderPermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFolderPermissionsRequestRequestTypeDef",
-    {
-        "GrantPermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-        "RevokePermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-
-class UpdateFolderPermissionsRequestRequestTypeDef(
-    _RequiredUpdateFolderPermissionsRequestRequestTypeDef,
-    _OptionalUpdateFolderPermissionsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateTemplatePermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateTemplatePermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "TemplateId": str,
-    },
-)
-_OptionalUpdateTemplatePermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateTemplatePermissionsRequestRequestTypeDef",
-    {
-        "GrantPermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-        "RevokePermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-
-class UpdateTemplatePermissionsRequestRequestTypeDef(
-    _RequiredUpdateTemplatePermissionsRequestRequestTypeDef,
-    _OptionalUpdateTemplatePermissionsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateThemePermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateThemePermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "ThemeId": str,
-    },
-)
-_OptionalUpdateThemePermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateThemePermissionsRequestRequestTypeDef",
-    {
-        "GrantPermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-        "RevokePermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-
-class UpdateThemePermissionsRequestRequestTypeDef(
-    _RequiredUpdateThemePermissionsRequestRequestTypeDef,
-    _OptionalUpdateThemePermissionsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateTopicPermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateTopicPermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "TopicId": str,
-    },
-)
-_OptionalUpdateTopicPermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateTopicPermissionsRequestRequestTypeDef",
-    {
-        "GrantPermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-        "RevokePermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-
-class UpdateTopicPermissionsRequestRequestTypeDef(
-    _RequiredUpdateTopicPermissionsRequestRequestTypeDef,
-    _OptionalUpdateTopicPermissionsRequestRequestTypeDef,
-):
-    pass
-
-
 DataSetSummaryTypeDef = TypedDict(
     "DataSetSummaryTypeDef",
     {
         "Arn": str,
         "DataSetId": str,
         "Name": str,
         "CreatedTime": datetime,
@@ -9051,49 +8657,14 @@
         "ThemeAlias": ThemeAliasTypeDef,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateTopicRefreshScheduleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTopicRefreshScheduleRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "TopicId": str,
-        "DatasetArn": str,
-        "RefreshSchedule": TopicRefreshScheduleTypeDef,
-    },
-)
-_OptionalCreateTopicRefreshScheduleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTopicRefreshScheduleRequestRequestTypeDef",
-    {
-        "DatasetName": str,
-    },
-    total=False,
-)
-
-
-class CreateTopicRefreshScheduleRequestRequestTypeDef(
-    _RequiredCreateTopicRefreshScheduleRequestRequestTypeDef,
-    _OptionalCreateTopicRefreshScheduleRequestRequestTypeDef,
-):
-    pass
-
-
-UpdateTopicRefreshScheduleRequestRequestTypeDef = TypedDict(
-    "UpdateTopicRefreshScheduleRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "TopicId": str,
-        "DatasetId": str,
-        "RefreshSchedule": TopicRefreshScheduleTypeDef,
-    },
-)
-
 CustomActionNavigationOperationTypeDef = TypedDict(
     "CustomActionNavigationOperationTypeDef",
     {
         "LocalNavigationConfiguration": LocalNavigationConfigurationTypeDef,
     },
     total=False,
 )
@@ -9115,35 +8686,14 @@
 
 class CustomValuesConfigurationOutputTypeDef(
     _RequiredCustomValuesConfigurationOutputTypeDef, _OptionalCustomValuesConfigurationOutputTypeDef
 ):
     pass
 
 
-_RequiredCustomValuesConfigurationTypeDef = TypedDict(
-    "_RequiredCustomValuesConfigurationTypeDef",
-    {
-        "CustomValues": CustomParameterValuesTypeDef,
-    },
-)
-_OptionalCustomValuesConfigurationTypeDef = TypedDict(
-    "_OptionalCustomValuesConfigurationTypeDef",
-    {
-        "IncludeNullValue": bool,
-    },
-    total=False,
-)
-
-
-class CustomValuesConfigurationTypeDef(
-    _RequiredCustomValuesConfigurationTypeDef, _OptionalCustomValuesConfigurationTypeDef
-):
-    pass
-
-
 _RequiredCustomSqlOutputTypeDef = TypedDict(
     "_RequiredCustomSqlOutputTypeDef",
     {
         "DataSourceArn": str,
         "Name": str,
         "SqlQuery": str,
     },
@@ -9485,52 +9035,28 @@
 
 class DateTimeDatasetParameterOutputTypeDef(
     _RequiredDateTimeDatasetParameterOutputTypeDef, _OptionalDateTimeDatasetParameterOutputTypeDef
 ):
     pass
 
 
-_RequiredDateTimeDatasetParameterTypeDef = TypedDict(
-    "_RequiredDateTimeDatasetParameterTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "ValueType": DatasetParameterValueTypeType,
-    },
-)
-_OptionalDateTimeDatasetParameterTypeDef = TypedDict(
-    "_OptionalDateTimeDatasetParameterTypeDef",
-    {
-        "TimeGranularity": TimeGranularityType,
-        "DefaultValues": DateTimeDatasetParameterDefaultValuesTypeDef,
-    },
-    total=False,
-)
-
-
-class DateTimeDatasetParameterTypeDef(
-    _RequiredDateTimeDatasetParameterTypeDef, _OptionalDateTimeDatasetParameterTypeDef
-):
-    pass
-
-
 TimeRangeFilterValueOutputTypeDef = TypedDict(
     "TimeRangeFilterValueOutputTypeDef",
     {
         "StaticValue": datetime,
         "RollingDate": RollingDateConfigurationTypeDef,
         "Parameter": str,
     },
     total=False,
 )
 
 TimeRangeFilterValueTypeDef = TypedDict(
     "TimeRangeFilterValueTypeDef",
     {
-        "StaticValue": Union[datetime, str],
+        "StaticValue": TimestampTypeDef,
         "RollingDate": RollingDateConfigurationTypeDef,
         "Parameter": str,
     },
     total=False,
 )
 
 _RequiredDecimalDatasetParameterOutputTypeDef = TypedDict(
@@ -9575,14 +9101,178 @@
 
 class DecimalDatasetParameterTypeDef(
     _RequiredDecimalDatasetParameterTypeDef, _OptionalDecimalDatasetParameterTypeDef
 ):
     pass
 
 
+DescribeAnalysisPermissionsResponseTypeDef = TypedDict(
+    "DescribeAnalysisPermissionsResponseTypeDef",
+    {
+        "AnalysisId": str,
+        "AnalysisArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDataSetPermissionsResponseTypeDef = TypedDict(
+    "DescribeDataSetPermissionsResponseTypeDef",
+    {
+        "DataSetArn": str,
+        "DataSetId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDataSourcePermissionsResponseTypeDef = TypedDict(
+    "DescribeDataSourcePermissionsResponseTypeDef",
+    {
+        "DataSourceArn": str,
+        "DataSourceId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFolderPermissionsResponseTypeDef = TypedDict(
+    "DescribeFolderPermissionsResponseTypeDef",
+    {
+        "Status": int,
+        "FolderId": str,
+        "Arn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFolderResolvedPermissionsResponseTypeDef = TypedDict(
+    "DescribeFolderResolvedPermissionsResponseTypeDef",
+    {
+        "Status": int,
+        "FolderId": str,
+        "Arn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTemplatePermissionsResponseTypeDef = TypedDict(
+    "DescribeTemplatePermissionsResponseTypeDef",
+    {
+        "TemplateId": str,
+        "TemplateArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeThemePermissionsResponseTypeDef = TypedDict(
+    "DescribeThemePermissionsResponseTypeDef",
+    {
+        "ThemeId": str,
+        "ThemeArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTopicPermissionsResponseTypeDef = TypedDict(
+    "DescribeTopicPermissionsResponseTypeDef",
+    {
+        "TopicId": str,
+        "TopicArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LinkSharingConfigurationTypeDef = TypedDict(
+    "LinkSharingConfigurationTypeDef",
+    {
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+    },
+    total=False,
+)
+
+UpdateAnalysisPermissionsResponseTypeDef = TypedDict(
+    "UpdateAnalysisPermissionsResponseTypeDef",
+    {
+        "AnalysisArn": str,
+        "AnalysisId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFolderPermissionsResponseTypeDef = TypedDict(
+    "UpdateFolderPermissionsResponseTypeDef",
+    {
+        "Status": int,
+        "Arn": str,
+        "FolderId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTemplatePermissionsResponseTypeDef = TypedDict(
+    "UpdateTemplatePermissionsResponseTypeDef",
+    {
+        "TemplateId": str,
+        "TemplateArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateThemePermissionsResponseTypeDef = TypedDict(
+    "UpdateThemePermissionsResponseTypeDef",
+    {
+        "ThemeId": str,
+        "ThemeArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTopicPermissionsResponseTypeDef = TypedDict(
+    "UpdateTopicPermissionsResponseTypeDef",
+    {
+        "TopicId": str,
+        "TopicArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeFolderResponseTypeDef = TypedDict(
     "DescribeFolderResponseTypeDef",
     {
         "Status": int,
         "Folder": FolderTypeDef,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -9728,14 +9418,15 @@
 
 class RelativeDatesFilterTypeDef(
     _RequiredRelativeDatesFilterTypeDef, _OptionalRelativeDatesFilterTypeDef
 ):
     pass
 
 
+FieldFolderUnionTypeDef = Union[FieldFolderTypeDef, FieldFolderOutputTypeDef]
 FilterOperationTargetVisualsConfigurationOutputTypeDef = TypedDict(
     "FilterOperationTargetVisualsConfigurationOutputTypeDef",
     {
         "SameSheetTargetVisualConfiguration": SameSheetTargetVisualConfigurationOutputTypeDef,
     },
     total=False,
 )
@@ -9826,23 +9517,14 @@
     {
         "WhatIfPointScenario": WhatIfPointScenarioOutputTypeDef,
         "WhatIfRangeScenario": WhatIfRangeScenarioOutputTypeDef,
     },
     total=False,
 )
 
-ForecastScenarioTypeDef = TypedDict(
-    "ForecastScenarioTypeDef",
-    {
-        "WhatIfPointScenario": WhatIfPointScenarioTypeDef,
-        "WhatIfRangeScenario": WhatIfRangeScenarioTypeDef,
-    },
-    total=False,
-)
-
 FreeFormLayoutCanvasSizeOptionsTypeDef = TypedDict(
     "FreeFormLayoutCanvasSizeOptionsTypeDef",
     {
         "ScreenCanvasSizeOptions": FreeFormLayoutScreenCanvasSizeOptionsTypeDef,
     },
     total=False,
 )
@@ -10844,37 +10526,14 @@
 class OverrideDatasetParameterOperationOutputTypeDef(
     _RequiredOverrideDatasetParameterOperationOutputTypeDef,
     _OptionalOverrideDatasetParameterOperationOutputTypeDef,
 ):
     pass
 
 
-_RequiredOverrideDatasetParameterOperationTypeDef = TypedDict(
-    "_RequiredOverrideDatasetParameterOperationTypeDef",
-    {
-        "ParameterName": str,
-    },
-)
-_OptionalOverrideDatasetParameterOperationTypeDef = TypedDict(
-    "_OptionalOverrideDatasetParameterOperationTypeDef",
-    {
-        "NewParameterName": str,
-        "NewDefaultValues": NewDefaultValuesTypeDef,
-    },
-    total=False,
-)
-
-
-class OverrideDatasetParameterOperationTypeDef(
-    _RequiredOverrideDatasetParameterOperationTypeDef,
-    _OptionalOverrideDatasetParameterOperationTypeDef,
-):
-    pass
-
-
 NumericSeparatorConfigurationTypeDef = TypedDict(
     "NumericSeparatorConfigurationTypeDef",
     {
         "DecimalSeparator": NumericSeparatorSymbolType,
         "ThousandsSeparator": ThousandSeparatorOptionsTypeDef,
     },
     total=False,
@@ -10896,25 +10555,14 @@
         "IntegerParameters": List[IntegerParameterOutputTypeDef],
         "DecimalParameters": List[DecimalParameterOutputTypeDef],
         "DateTimeParameters": List[DateTimeParameterOutputTypeDef],
     },
     total=False,
 )
 
-ParametersTypeDef = TypedDict(
-    "ParametersTypeDef",
-    {
-        "StringParameters": Sequence[StringParameterTypeDef],
-        "IntegerParameters": Sequence[IntegerParameterTypeDef],
-        "DecimalParameters": Sequence[DecimalParameterTypeDef],
-        "DateTimeParameters": Sequence[DateTimeParameterTypeDef],
-    },
-    total=False,
-)
-
 VisibleRangeOptionsTypeDef = TypedDict(
     "VisibleRangeOptionsTypeDef",
     {
         "PercentRange": PercentVisibleRangeTypeDef,
     },
     total=False,
 )
@@ -10970,14 +10618,15 @@
     {
         "StatePersistence": StatePersistenceConfigurationsTypeDef,
         "Bookmarks": BookmarksConfigurationsTypeDef,
     },
     total=False,
 )
 
+ResourcePermissionUnionTypeDef = Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
 _RequiredRowLevelPermissionTagConfigurationOutputTypeDef = TypedDict(
     "_RequiredRowLevelPermissionTagConfigurationOutputTypeDef",
     {
         "TagRules": List[RowLevelPermissionTagRuleTypeDef],
     },
 )
 _OptionalRowLevelPermissionTagConfigurationOutputTypeDef = TypedDict(
@@ -11251,15 +10900,15 @@
     total=False,
 )
 
 DateTimeDefaultValuesTypeDef = TypedDict(
     "DateTimeDefaultValuesTypeDef",
     {
         "DynamicValue": DynamicDefaultValueTypeDef,
-        "StaticValues": Sequence[Union[datetime, str]],
+        "StaticValues": Sequence[TimestampTypeDef],
         "RollingDate": RollingDateConfigurationTypeDef,
     },
     total=False,
 )
 
 DecimalDefaultValuesOutputTypeDef = TypedDict(
     "DecimalDefaultValuesOutputTypeDef",
@@ -11321,24 +10970,14 @@
         "NumericEqualityFilter": NumericEqualityDrillDownFilterTypeDef,
         "CategoryFilter": CategoryDrillDownFilterOutputTypeDef,
         "TimeRangeFilter": TimeRangeDrillDownFilterOutputTypeDef,
     },
     total=False,
 )
 
-DrillDownFilterTypeDef = TypedDict(
-    "DrillDownFilterTypeDef",
-    {
-        "NumericEqualityFilter": NumericEqualityDrillDownFilterTypeDef,
-        "CategoryFilter": CategoryDrillDownFilterTypeDef,
-        "TimeRangeFilter": TimeRangeDrillDownFilterTypeDef,
-    },
-    total=False,
-)
-
 AnalysisTypeDef = TypedDict(
     "AnalysisTypeDef",
     {
         "AnalysisId": str,
         "Arn": str,
         "Name": str,
         "Status": ResourceStatusType,
@@ -11422,14 +11061,18 @@
         ),
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AssetBundleCloudFormationOverridePropertyConfigurationUnionTypeDef = Union[
+    AssetBundleCloudFormationOverridePropertyConfigurationTypeDef,
+    AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef,
+]
 _RequiredStartAssetBundleExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartAssetBundleExportJobRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AssetBundleExportJobId": str,
         "ResourceArns": Sequence[str],
         "ExportFormat": AssetBundleExportFormatType,
@@ -11450,14 +11093,150 @@
 class StartAssetBundleExportJobRequestRequestTypeDef(
     _RequiredStartAssetBundleExportJobRequestRequestTypeDef,
     _OptionalStartAssetBundleExportJobRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredCustomValuesConfigurationTypeDef = TypedDict(
+    "_RequiredCustomValuesConfigurationTypeDef",
+    {
+        "CustomValues": CustomParameterValuesTypeDef,
+    },
+)
+_OptionalCustomValuesConfigurationTypeDef = TypedDict(
+    "_OptionalCustomValuesConfigurationTypeDef",
+    {
+        "IncludeNullValue": bool,
+    },
+    total=False,
+)
+
+
+class CustomValuesConfigurationTypeDef(
+    _RequiredCustomValuesConfigurationTypeDef, _OptionalCustomValuesConfigurationTypeDef
+):
+    pass
+
+
+_RequiredDateTimeDatasetParameterTypeDef = TypedDict(
+    "_RequiredDateTimeDatasetParameterTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "ValueType": DatasetParameterValueTypeType,
+    },
+)
+_OptionalDateTimeDatasetParameterTypeDef = TypedDict(
+    "_OptionalDateTimeDatasetParameterTypeDef",
+    {
+        "TimeGranularity": TimeGranularityType,
+        "DefaultValues": DateTimeDatasetParameterDefaultValuesTypeDef,
+    },
+    total=False,
+)
+
+
+class DateTimeDatasetParameterTypeDef(
+    _RequiredDateTimeDatasetParameterTypeDef, _OptionalDateTimeDatasetParameterTypeDef
+):
+    pass
+
+
+ParametersTypeDef = TypedDict(
+    "ParametersTypeDef",
+    {
+        "StringParameters": Sequence[StringParameterTypeDef],
+        "IntegerParameters": Sequence[IntegerParameterTypeDef],
+        "DecimalParameters": Sequence[DecimalParameterTypeDef],
+        "DateTimeParameters": Sequence[DateTimeParameterTypeDef],
+    },
+    total=False,
+)
+
+_RequiredOverrideDatasetParameterOperationTypeDef = TypedDict(
+    "_RequiredOverrideDatasetParameterOperationTypeDef",
+    {
+        "ParameterName": str,
+    },
+)
+_OptionalOverrideDatasetParameterOperationTypeDef = TypedDict(
+    "_OptionalOverrideDatasetParameterOperationTypeDef",
+    {
+        "NewParameterName": str,
+        "NewDefaultValues": NewDefaultValuesTypeDef,
+    },
+    total=False,
+)
+
+
+class OverrideDatasetParameterOperationTypeDef(
+    _RequiredOverrideDatasetParameterOperationTypeDef,
+    _OptionalOverrideDatasetParameterOperationTypeDef,
+):
+    pass
+
+
+DrillDownFilterTypeDef = TypedDict(
+    "DrillDownFilterTypeDef",
+    {
+        "NumericEqualityFilter": NumericEqualityDrillDownFilterTypeDef,
+        "CategoryFilter": CategoryDrillDownFilterTypeDef,
+        "TimeRangeFilter": TimeRangeDrillDownFilterTypeDef,
+    },
+    total=False,
+)
+
+_RequiredCreateTopicRefreshScheduleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTopicRefreshScheduleRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "TopicId": str,
+        "DatasetArn": str,
+        "RefreshSchedule": TopicRefreshScheduleTypeDef,
+    },
+)
+_OptionalCreateTopicRefreshScheduleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTopicRefreshScheduleRequestRequestTypeDef",
+    {
+        "DatasetName": str,
+    },
+    total=False,
+)
+
+
+class CreateTopicRefreshScheduleRequestRequestTypeDef(
+    _RequiredCreateTopicRefreshScheduleRequestRequestTypeDef,
+    _OptionalCreateTopicRefreshScheduleRequestRequestTypeDef,
+):
+    pass
+
+
+TopicRefreshScheduleUnionTypeDef = Union[
+    TopicRefreshScheduleTypeDef, TopicRefreshScheduleOutputTypeDef
+]
+UpdateTopicRefreshScheduleRequestRequestTypeDef = TypedDict(
+    "UpdateTopicRefreshScheduleRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "TopicId": str,
+        "DatasetId": str,
+        "RefreshSchedule": TopicRefreshScheduleTypeDef,
+    },
+)
+
+ForecastScenarioTypeDef = TypedDict(
+    "ForecastScenarioTypeDef",
+    {
+        "WhatIfPointScenario": WhatIfPointScenarioTypeDef,
+        "WhatIfRangeScenario": WhatIfRangeScenarioTypeDef,
+    },
+    total=False,
+)
+
 NumericAxisOptionsOutputTypeDef = TypedDict(
     "NumericAxisOptionsOutputTypeDef",
     {
         "Scale": AxisScaleTypeDef,
         "Range": AxisDisplayRangeOutputTypeDef,
     },
     total=False,
@@ -11532,14 +11311,15 @@
     "TagColumnOperationTypeDef",
     {
         "ColumnName": str,
         "Tags": Sequence[ColumnTagTypeDef],
     },
 )
 
+ColumnGroupUnionTypeDef = Union[ColumnGroupTypeDef, ColumnGroupOutputTypeDef]
 DataSetConfigurationOutputTypeDef = TypedDict(
     "DataSetConfigurationOutputTypeDef",
     {
         "Placeholder": str,
         "DataSetSchema": DataSetSchemaOutputTypeDef,
         "ColumnGroupSchemaList": List[ColumnGroupSchemaOutputTypeDef],
     },
@@ -11561,40 +11341,14 @@
     {
         "IconSet": ConditionalFormattingIconSetTypeDef,
         "CustomCondition": ConditionalFormattingCustomIconConditionTypeDef,
     },
     total=False,
 )
 
-DescribeDashboardPermissionsResponseTypeDef = TypedDict(
-    "DescribeDashboardPermissionsResponseTypeDef",
-    {
-        "DashboardId": str,
-        "DashboardArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "LinkSharingConfiguration": LinkSharingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateDashboardPermissionsResponseTypeDef = TypedDict(
-    "UpdateDashboardPermissionsResponseTypeDef",
-    {
-        "DashboardArn": str,
-        "DashboardId": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "LinkSharingConfiguration": LinkSharingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListDataSetsResponseTypeDef = TypedDict(
     "ListDataSetsResponseTypeDef",
     {
         "DataSetSummaries": List[DataSetSummaryTypeDef],
         "NextToken": str,
         "RequestId": str,
         "Status": int,
@@ -11621,26 +11375,14 @@
         "SourceParameterName": str,
         "SourceField": str,
         "SourceColumn": ColumnIdentifierTypeDef,
     },
     total=False,
 )
 
-DestinationParameterValueConfigurationTypeDef = TypedDict(
-    "DestinationParameterValueConfigurationTypeDef",
-    {
-        "CustomValuesConfiguration": CustomValuesConfigurationTypeDef,
-        "SelectAllValueOptions": Literal["ALL_VALUES"],
-        "SourceParameterName": str,
-        "SourceField": str,
-        "SourceColumn": ColumnIdentifierTypeDef,
-    },
-    total=False,
-)
-
 DashboardPublishOptionsTypeDef = TypedDict(
     "DashboardPublishOptionsTypeDef",
     {
         "AdHocFilteringOption": AdHocFilteringOptionTypeDef,
         "ExportToCSVOption": ExportToCSVOptionTypeDef,
         "SheetControlsOption": SheetControlsOptionTypeDef,
         "VisualPublishOptions": DashboardVisualPublishOptionsTypeDef,
@@ -11767,14 +11509,40 @@
 )
 
 
 class TimeRangeFilterTypeDef(_RequiredTimeRangeFilterTypeDef, _OptionalTimeRangeFilterTypeDef):
     pass
 
 
+DescribeDashboardPermissionsResponseTypeDef = TypedDict(
+    "DescribeDashboardPermissionsResponseTypeDef",
+    {
+        "DashboardId": str,
+        "DashboardArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "LinkSharingConfiguration": LinkSharingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDashboardPermissionsResponseTypeDef = TypedDict(
+    "UpdateDashboardPermissionsResponseTypeDef",
+    {
+        "DashboardArn": str,
+        "DashboardId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "LinkSharingConfiguration": LinkSharingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTopicRefreshSchedulesResponseTypeDef = TypedDict(
     "ListTopicRefreshSchedulesResponseTypeDef",
     {
         "TopicId": str,
         "TopicArn": str,
         "RefreshSchedules": List[TopicRefreshScheduleSummaryTypeDef],
         "Status": int,
@@ -11912,23 +11680,14 @@
     {
         "ForecastProperties": TimeBasedForecastPropertiesTypeDef,
         "Scenario": ForecastScenarioOutputTypeDef,
     },
     total=False,
 )
 
-ForecastConfigurationTypeDef = TypedDict(
-    "ForecastConfigurationTypeDef",
-    {
-        "ForecastProperties": TimeBasedForecastPropertiesTypeDef,
-        "Scenario": ForecastScenarioTypeDef,
-    },
-    total=False,
-)
-
 DefaultFreeFormLayoutConfigurationTypeDef = TypedDict(
     "DefaultFreeFormLayoutConfigurationTypeDef",
     {
         "CanvasSizeOptions": FreeFormLayoutCanvasSizeOptionsTypeDef,
     },
 )
 
@@ -12350,15 +12109,15 @@
         "ScheduleFrequency": RefreshFrequencyTypeDef,
         "RefreshType": IngestionTypeType,
     },
 )
 _OptionalRefreshScheduleTypeDef = TypedDict(
     "_OptionalRefreshScheduleTypeDef",
     {
-        "StartAfterDateTime": Union[datetime, str],
+        "StartAfterDateTime": TimestampTypeDef,
         "Arn": str,
     },
     total=False,
 )
 
 
 class RefreshScheduleTypeDef(_RequiredRefreshScheduleTypeDef, _OptionalRefreshScheduleTypeDef):
@@ -12392,14 +12151,237 @@
 class RegisteredUserDashboardEmbeddingConfigurationTypeDef(
     _RequiredRegisteredUserDashboardEmbeddingConfigurationTypeDef,
     _OptionalRegisteredUserDashboardEmbeddingConfigurationTypeDef,
 ):
     pass
 
 
+_RequiredCreateFolderRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFolderRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "FolderId": str,
+    },
+)
+_OptionalCreateFolderRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFolderRequestRequestTypeDef",
+    {
+        "Name": str,
+        "FolderType": Literal["SHARED"],
+        "ParentFolderArn": str,
+        "Permissions": Sequence[ResourcePermissionUnionTypeDef],
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateFolderRequestRequestTypeDef(
+    _RequiredCreateFolderRequestRequestTypeDef, _OptionalCreateFolderRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateAnalysisPermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAnalysisPermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "AnalysisId": str,
+    },
+)
+_OptionalUpdateAnalysisPermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAnalysisPermissionsRequestRequestTypeDef",
+    {
+        "GrantPermissions": Sequence[ResourcePermissionUnionTypeDef],
+        "RevokePermissions": Sequence[ResourcePermissionUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateAnalysisPermissionsRequestRequestTypeDef(
+    _RequiredUpdateAnalysisPermissionsRequestRequestTypeDef,
+    _OptionalUpdateAnalysisPermissionsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateDashboardPermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDashboardPermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "DashboardId": str,
+    },
+)
+_OptionalUpdateDashboardPermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDashboardPermissionsRequestRequestTypeDef",
+    {
+        "GrantPermissions": Sequence[ResourcePermissionUnionTypeDef],
+        "RevokePermissions": Sequence[ResourcePermissionUnionTypeDef],
+        "GrantLinkPermissions": Sequence[ResourcePermissionUnionTypeDef],
+        "RevokeLinkPermissions": Sequence[ResourcePermissionUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateDashboardPermissionsRequestRequestTypeDef(
+    _RequiredUpdateDashboardPermissionsRequestRequestTypeDef,
+    _OptionalUpdateDashboardPermissionsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateDataSetPermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDataSetPermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "DataSetId": str,
+    },
+)
+_OptionalUpdateDataSetPermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDataSetPermissionsRequestRequestTypeDef",
+    {
+        "GrantPermissions": Sequence[ResourcePermissionUnionTypeDef],
+        "RevokePermissions": Sequence[ResourcePermissionUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateDataSetPermissionsRequestRequestTypeDef(
+    _RequiredUpdateDataSetPermissionsRequestRequestTypeDef,
+    _OptionalUpdateDataSetPermissionsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateDataSourcePermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDataSourcePermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "DataSourceId": str,
+    },
+)
+_OptionalUpdateDataSourcePermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDataSourcePermissionsRequestRequestTypeDef",
+    {
+        "GrantPermissions": Sequence[ResourcePermissionUnionTypeDef],
+        "RevokePermissions": Sequence[ResourcePermissionUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateDataSourcePermissionsRequestRequestTypeDef(
+    _RequiredUpdateDataSourcePermissionsRequestRequestTypeDef,
+    _OptionalUpdateDataSourcePermissionsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateFolderPermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFolderPermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "FolderId": str,
+    },
+)
+_OptionalUpdateFolderPermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFolderPermissionsRequestRequestTypeDef",
+    {
+        "GrantPermissions": Sequence[ResourcePermissionUnionTypeDef],
+        "RevokePermissions": Sequence[ResourcePermissionUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateFolderPermissionsRequestRequestTypeDef(
+    _RequiredUpdateFolderPermissionsRequestRequestTypeDef,
+    _OptionalUpdateFolderPermissionsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateTemplatePermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateTemplatePermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "TemplateId": str,
+    },
+)
+_OptionalUpdateTemplatePermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateTemplatePermissionsRequestRequestTypeDef",
+    {
+        "GrantPermissions": Sequence[ResourcePermissionUnionTypeDef],
+        "RevokePermissions": Sequence[ResourcePermissionUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateTemplatePermissionsRequestRequestTypeDef(
+    _RequiredUpdateTemplatePermissionsRequestRequestTypeDef,
+    _OptionalUpdateTemplatePermissionsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateThemePermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateThemePermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "ThemeId": str,
+    },
+)
+_OptionalUpdateThemePermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateThemePermissionsRequestRequestTypeDef",
+    {
+        "GrantPermissions": Sequence[ResourcePermissionUnionTypeDef],
+        "RevokePermissions": Sequence[ResourcePermissionUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateThemePermissionsRequestRequestTypeDef(
+    _RequiredUpdateThemePermissionsRequestRequestTypeDef,
+    _OptionalUpdateThemePermissionsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateTopicPermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateTopicPermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "TopicId": str,
+    },
+)
+_OptionalUpdateTopicPermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateTopicPermissionsRequestRequestTypeDef",
+    {
+        "GrantPermissions": Sequence[ResourcePermissionUnionTypeDef],
+        "RevokePermissions": Sequence[ResourcePermissionUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateTopicPermissionsRequestRequestTypeDef(
+    _RequiredUpdateTopicPermissionsRequestRequestTypeDef,
+    _OptionalUpdateTopicPermissionsRequestRequestTypeDef,
+):
+    pass
+
+
+RowLevelPermissionTagConfigurationUnionTypeDef = Union[
+    RowLevelPermissionTagConfigurationTypeDef, RowLevelPermissionTagConfigurationOutputTypeDef
+]
 SnapshotDestinationConfigurationOutputTypeDef = TypedDict(
     "SnapshotDestinationConfigurationOutputTypeDef",
     {
         "S3Destinations": List[SnapshotS3DestinationConfigurationTypeDef],
     },
     total=False,
 )
@@ -12551,25 +12533,14 @@
         "DecimalDatasetParameter": DecimalDatasetParameterOutputTypeDef,
         "IntegerDatasetParameter": IntegerDatasetParameterOutputTypeDef,
         "DateTimeDatasetParameter": DateTimeDatasetParameterOutputTypeDef,
     },
     total=False,
 )
 
-DatasetParameterTypeDef = TypedDict(
-    "DatasetParameterTypeDef",
-    {
-        "StringDatasetParameter": StringDatasetParameterTypeDef,
-        "DecimalDatasetParameter": DecimalDatasetParameterTypeDef,
-        "IntegerDatasetParameter": IntegerDatasetParameterTypeDef,
-        "DateTimeDatasetParameter": DateTimeDatasetParameterTypeDef,
-    },
-    total=False,
-)
-
 _RequiredDateTimeParameterDeclarationOutputTypeDef = TypedDict(
     "_RequiredDateTimeParameterDeclarationOutputTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDateTimeParameterDeclarationOutputTypeDef = TypedDict(
@@ -12823,14 +12794,89 @@
 
 class PredefinedHierarchyOutputTypeDef(
     _RequiredPredefinedHierarchyOutputTypeDef, _OptionalPredefinedHierarchyOutputTypeDef
 ):
     pass
 
 
+DescribeAnalysisResponseTypeDef = TypedDict(
+    "DescribeAnalysisResponseTypeDef",
+    {
+        "Analysis": AnalysisTypeDef,
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DashboardTypeDef = TypedDict(
+    "DashboardTypeDef",
+    {
+        "DashboardId": str,
+        "Arn": str,
+        "Name": str,
+        "Version": DashboardVersionTypeDef,
+        "CreatedTime": datetime,
+        "LastPublishedTime": datetime,
+        "LastUpdatedTime": datetime,
+    },
+    total=False,
+)
+
+_RequiredGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef = TypedDict(
+    "_RequiredGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "Namespace": str,
+        "AuthorizedResourceArns": Sequence[str],
+        "ExperienceConfiguration": AnonymousUserEmbeddingExperienceConfigurationTypeDef,
+    },
+)
+_OptionalGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef = TypedDict(
+    "_OptionalGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef",
+    {
+        "SessionLifetimeInMinutes": int,
+        "SessionTags": Sequence[SessionTagTypeDef],
+        "AllowedDomains": Sequence[str],
+    },
+    total=False,
+)
+
+
+class GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef(
+    _RequiredGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef,
+    _OptionalGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef,
+):
+    pass
+
+
+DestinationParameterValueConfigurationTypeDef = TypedDict(
+    "DestinationParameterValueConfigurationTypeDef",
+    {
+        "CustomValuesConfiguration": CustomValuesConfigurationTypeDef,
+        "SelectAllValueOptions": Literal["ALL_VALUES"],
+        "SourceParameterName": str,
+        "SourceField": str,
+        "SourceColumn": ColumnIdentifierTypeDef,
+    },
+    total=False,
+)
+
+DatasetParameterTypeDef = TypedDict(
+    "DatasetParameterTypeDef",
+    {
+        "StringDatasetParameter": StringDatasetParameterTypeDef,
+        "DecimalDatasetParameter": DecimalDatasetParameterTypeDef,
+        "IntegerDatasetParameter": IntegerDatasetParameterTypeDef,
+        "DateTimeDatasetParameter": DateTimeDatasetParameterTypeDef,
+    },
+    total=False,
+)
+
+ParametersUnionTypeDef = Union[ParametersTypeDef, ParametersOutputTypeDef]
 _RequiredDateTimeHierarchyTypeDef = TypedDict(
     "_RequiredDateTimeHierarchyTypeDef",
     {
         "HierarchyId": str,
     },
 )
 _OptionalDateTimeHierarchyTypeDef = TypedDict(
@@ -12888,65 +12934,23 @@
 
 class PredefinedHierarchyTypeDef(
     _RequiredPredefinedHierarchyTypeDef, _OptionalPredefinedHierarchyTypeDef
 ):
     pass
 
 
-DescribeAnalysisResponseTypeDef = TypedDict(
-    "DescribeAnalysisResponseTypeDef",
-    {
-        "Analysis": AnalysisTypeDef,
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DashboardTypeDef = TypedDict(
-    "DashboardTypeDef",
-    {
-        "DashboardId": str,
-        "Arn": str,
-        "Name": str,
-        "Version": DashboardVersionTypeDef,
-        "CreatedTime": datetime,
-        "LastPublishedTime": datetime,
-        "LastUpdatedTime": datetime,
-    },
-    total=False,
-)
-
-_RequiredGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef = TypedDict(
-    "_RequiredGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "Namespace": str,
-        "AuthorizedResourceArns": Sequence[str],
-        "ExperienceConfiguration": AnonymousUserEmbeddingExperienceConfigurationTypeDef,
-    },
-)
-_OptionalGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef = TypedDict(
-    "_OptionalGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef",
+ForecastConfigurationTypeDef = TypedDict(
+    "ForecastConfigurationTypeDef",
     {
-        "SessionLifetimeInMinutes": int,
-        "SessionTags": Sequence[SessionTagTypeDef],
-        "AllowedDomains": Sequence[str],
+        "ForecastProperties": TimeBasedForecastPropertiesTypeDef,
+        "Scenario": ForecastScenarioTypeDef,
     },
     total=False,
 )
 
-
-class GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef(
-    _RequiredGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef,
-    _OptionalGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef,
-):
-    pass
-
-
 AxisDataOptionsOutputTypeDef = TypedDict(
     "AxisDataOptionsOutputTypeDef",
     {
         "NumericAxisOptions": NumericAxisOptionsOutputTypeDef,
         "DateAxisOptions": DateAxisOptionsTypeDef,
     },
     total=False,
@@ -13011,22 +13015,14 @@
     "SetParameterValueConfigurationOutputTypeDef",
     {
         "DestinationParameterName": str,
         "Value": DestinationParameterValueConfigurationOutputTypeDef,
     },
 )
 
-SetParameterValueConfigurationTypeDef = TypedDict(
-    "SetParameterValueConfigurationTypeDef",
-    {
-        "DestinationParameterName": str,
-        "Value": DestinationParameterValueConfigurationTypeDef,
-    },
-)
-
 PivotTableFieldOptionsOutputTypeDef = TypedDict(
     "PivotTableFieldOptionsOutputTypeDef",
     {
         "SelectedFieldOptions": List[PivotTableFieldOptionTypeDef],
         "DataPathOptions": List[PivotTableDataPathOptionOutputTypeDef],
         "CollapseStateOptions": List[PivotTableFieldCollapseStateOptionOutputTypeDef],
     },
@@ -13745,14 +13741,15 @@
     {
         "DataSetId": str,
         "AwsAccountId": str,
         "Schedule": RefreshScheduleTypeDef,
     },
 )
 
+RefreshScheduleUnionTypeDef = Union[RefreshScheduleTypeDef, RefreshScheduleOutputTypeDef]
 UpdateRefreshScheduleRequestRequestTypeDef = TypedDict(
     "UpdateRefreshScheduleRequestRequestTypeDef",
     {
         "DataSetId": str,
         "AwsAccountId": str,
         "Schedule": RefreshScheduleTypeDef,
     },
@@ -13774,14 +13771,15 @@
     {
         "Files": List[SnapshotFileOutputTypeDef],
         "S3Results": List[SnapshotJobS3ResultTypeDef],
     },
     total=False,
 )
 
+PhysicalTableUnionTypeDef = Union[PhysicalTableTypeDef, PhysicalTableOutputTypeDef]
 DefaultSectionBasedLayoutConfigurationTypeDef = TypedDict(
     "DefaultSectionBasedLayoutConfigurationTypeDef",
     {
         "CanvasSizeOptions": SectionBasedLayoutCanvasSizeOptionsTypeDef,
     },
 )
 
@@ -13914,34 +13912,43 @@
         "ExplicitHierarchy": ExplicitHierarchyOutputTypeDef,
         "DateTimeHierarchy": DateTimeHierarchyOutputTypeDef,
         "PredefinedHierarchy": PredefinedHierarchyOutputTypeDef,
     },
     total=False,
 )
 
-ColumnHierarchyTypeDef = TypedDict(
-    "ColumnHierarchyTypeDef",
-    {
-        "ExplicitHierarchy": ExplicitHierarchyTypeDef,
-        "DateTimeHierarchy": DateTimeHierarchyTypeDef,
-        "PredefinedHierarchy": PredefinedHierarchyTypeDef,
-    },
-    total=False,
-)
-
 DescribeDashboardResponseTypeDef = TypedDict(
     "DescribeDashboardResponseTypeDef",
     {
         "Dashboard": DashboardTypeDef,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SetParameterValueConfigurationTypeDef = TypedDict(
+    "SetParameterValueConfigurationTypeDef",
+    {
+        "DestinationParameterName": str,
+        "Value": DestinationParameterValueConfigurationTypeDef,
+    },
+)
+
+DatasetParameterUnionTypeDef = Union[DatasetParameterTypeDef, DatasetParameterOutputTypeDef]
+ColumnHierarchyTypeDef = TypedDict(
+    "ColumnHierarchyTypeDef",
+    {
+        "ExplicitHierarchy": ExplicitHierarchyTypeDef,
+        "DateTimeHierarchy": DateTimeHierarchyTypeDef,
+        "PredefinedHierarchy": PredefinedHierarchyTypeDef,
+    },
+    total=False,
+)
+
 _RequiredLogicalTableOutputTypeDef = TypedDict(
     "_RequiredLogicalTableOutputTypeDef",
     {
         "Alias": str,
         "Source": LogicalTableSourceTypeDef,
     },
 )
@@ -13996,21 +14003,14 @@
 CustomActionSetParametersOperationOutputTypeDef = TypedDict(
     "CustomActionSetParametersOperationOutputTypeDef",
     {
         "ParameterValueConfigurations": List[SetParameterValueConfigurationOutputTypeDef],
     },
 )
 
-CustomActionSetParametersOperationTypeDef = TypedDict(
-    "CustomActionSetParametersOperationTypeDef",
-    {
-        "ParameterValueConfigurations": Sequence[SetParameterValueConfigurationTypeDef],
-    },
-)
-
 AxisDisplayOptionsOutputTypeDef = TypedDict(
     "AxisDisplayOptionsOutputTypeDef",
     {
         "TickLabelOptions": AxisTickLabelOptionsTypeDef,
         "AxisLineVisibility": VisibilityType,
         "GridLineVisibility": VisibilityType,
         "DataOptions": AxisDataOptionsOutputTypeDef,
@@ -14833,27 +14833,28 @@
         "Configuration": ThemeConfigurationTypeDef,
     },
 )
 _OptionalCreateThemeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateThemeRequestRequestTypeDef",
     {
         "VersionDescription": str,
-        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
+        "Permissions": Sequence[ResourcePermissionUnionTypeDef],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
 class CreateThemeRequestRequestTypeDef(
     _RequiredCreateThemeRequestRequestTypeDef, _OptionalCreateThemeRequestRequestTypeDef
 ):
     pass
 
 
+ThemeConfigurationUnionTypeDef = Union[ThemeConfigurationTypeDef, ThemeConfigurationOutputTypeDef]
 _RequiredUpdateThemeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateThemeRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "ThemeId": str,
         "BaseThemeId": str,
     },
@@ -15137,25 +15138,35 @@
         "LastUpdatedTime": datetime,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SnapshotConfigurationUnionTypeDef = Union[
+    SnapshotConfigurationTypeDef, SnapshotConfigurationOutputTypeDef
+]
 StartDashboardSnapshotJobRequestRequestTypeDef = TypedDict(
     "StartDashboardSnapshotJobRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "DashboardId": str,
         "SnapshotJobId": str,
         "UserConfiguration": SnapshotUserConfigurationTypeDef,
         "SnapshotConfiguration": SnapshotConfigurationTypeDef,
     },
 )
 
+CustomActionSetParametersOperationTypeDef = TypedDict(
+    "CustomActionSetParametersOperationTypeDef",
+    {
+        "ParameterValueConfigurations": Sequence[SetParameterValueConfigurationTypeDef],
+    },
+)
+
 DataSetTypeDef = TypedDict(
     "DataSetTypeDef",
     {
         "Arn": str,
         "DataSetId": str,
         "Name": str,
         "CreatedTime": datetime,
@@ -15172,88 +15183,15 @@
         "ColumnLevelPermissionRules": List[ColumnLevelPermissionRuleOutputTypeDef],
         "DataSetUsageConfiguration": DataSetUsageConfigurationTypeDef,
         "DatasetParameters": List[DatasetParameterOutputTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateDataSetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDataSetRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "DataSetId": str,
-        "Name": str,
-        "PhysicalTableMap": Mapping[str, Union[PhysicalTableTypeDef, PhysicalTableOutputTypeDef]],
-        "ImportMode": DataSetImportModeType,
-    },
-)
-_OptionalCreateDataSetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDataSetRequestRequestTypeDef",
-    {
-        "LogicalTableMap": Mapping[str, Union[LogicalTableTypeDef, LogicalTableOutputTypeDef]],
-        "ColumnGroups": Sequence[Union[ColumnGroupTypeDef, ColumnGroupOutputTypeDef]],
-        "FieldFolders": Mapping[str, Union[FieldFolderTypeDef, FieldFolderOutputTypeDef]],
-        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
-        "RowLevelPermissionDataSet": RowLevelPermissionDataSetTypeDef,
-        "RowLevelPermissionTagConfiguration": RowLevelPermissionTagConfigurationTypeDef,
-        "ColumnLevelPermissionRules": Sequence[
-            Union[ColumnLevelPermissionRuleTypeDef, ColumnLevelPermissionRuleOutputTypeDef]
-        ],
-        "Tags": Sequence[TagTypeDef],
-        "DataSetUsageConfiguration": DataSetUsageConfigurationTypeDef,
-        "DatasetParameters": Sequence[
-            Union[DatasetParameterTypeDef, DatasetParameterOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-
-class CreateDataSetRequestRequestTypeDef(
-    _RequiredCreateDataSetRequestRequestTypeDef, _OptionalCreateDataSetRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateDataSetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDataSetRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "DataSetId": str,
-        "Name": str,
-        "PhysicalTableMap": Mapping[str, Union[PhysicalTableTypeDef, PhysicalTableOutputTypeDef]],
-        "ImportMode": DataSetImportModeType,
-    },
-)
-_OptionalUpdateDataSetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDataSetRequestRequestTypeDef",
-    {
-        "LogicalTableMap": Mapping[str, Union[LogicalTableTypeDef, LogicalTableOutputTypeDef]],
-        "ColumnGroups": Sequence[Union[ColumnGroupTypeDef, ColumnGroupOutputTypeDef]],
-        "FieldFolders": Mapping[str, Union[FieldFolderTypeDef, FieldFolderOutputTypeDef]],
-        "RowLevelPermissionDataSet": RowLevelPermissionDataSetTypeDef,
-        "RowLevelPermissionTagConfiguration": RowLevelPermissionTagConfigurationTypeDef,
-        "ColumnLevelPermissionRules": Sequence[
-            Union[ColumnLevelPermissionRuleTypeDef, ColumnLevelPermissionRuleOutputTypeDef]
-        ],
-        "DataSetUsageConfiguration": DataSetUsageConfigurationTypeDef,
-        "DatasetParameters": Sequence[
-            Union[DatasetParameterTypeDef, DatasetParameterOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-
-class UpdateDataSetRequestRequestTypeDef(
-    _RequiredUpdateDataSetRequestRequestTypeDef, _OptionalUpdateDataSetRequestRequestTypeDef
-):
-    pass
-
-
+LogicalTableUnionTypeDef = Union[LogicalTableTypeDef, LogicalTableOutputTypeDef]
 DescribeTemplateResponseTypeDef = TypedDict(
     "DescribeTemplateResponseTypeDef",
     {
         "Template": TemplateTypeDef,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -15267,25 +15205,14 @@
         "NavigationOperation": CustomActionNavigationOperationTypeDef,
         "URLOperation": CustomActionURLOperationTypeDef,
         "SetParametersOperation": CustomActionSetParametersOperationOutputTypeDef,
     },
     total=False,
 )
 
-VisualCustomActionOperationTypeDef = TypedDict(
-    "VisualCustomActionOperationTypeDef",
-    {
-        "FilterOperation": CustomActionFilterOperationTypeDef,
-        "NavigationOperation": CustomActionNavigationOperationTypeDef,
-        "URLOperation": CustomActionURLOperationTypeDef,
-        "SetParametersOperation": CustomActionSetParametersOperationTypeDef,
-    },
-    total=False,
-)
-
 LineSeriesAxisDisplayOptionsOutputTypeDef = TypedDict(
     "LineSeriesAxisDisplayOptionsOutputTypeDef",
     {
         "AxisOptions": AxisDisplayOptionsOutputTypeDef,
         "MissingDataConfigurations": List[MissingDataConfigurationTypeDef],
     },
     total=False,
@@ -15571,14 +15498,18 @@
         "FailureAction": AssetBundleImportFailureActionType,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AssetBundleImportJobOverrideParametersUnionTypeDef = Union[
+    AssetBundleImportJobOverrideParametersTypeDef,
+    AssetBundleImportJobOverrideParametersOutputTypeDef,
+]
 _RequiredStartAssetBundleImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartAssetBundleImportJobRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AssetBundleImportJobId": str,
         "AssetBundleImportSource": AssetBundleImportSourceTypeDef,
     },
@@ -15610,15 +15541,15 @@
     },
 )
 _OptionalCreateDataSourceRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDataSourceRequestRequestTypeDef",
     {
         "DataSourceParameters": DataSourceParametersTypeDef,
         "Credentials": DataSourceCredentialsTypeDef,
-        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
+        "Permissions": Sequence[ResourcePermissionUnionTypeDef],
         "VpcConnectionProperties": VpcConnectionPropertiesTypeDef,
         "SslProperties": SslPropertiesTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
@@ -16313,68 +16244,121 @@
 class HeaderFooterSectionConfigurationTypeDef(
     _RequiredHeaderFooterSectionConfigurationTypeDef,
     _OptionalHeaderFooterSectionConfigurationTypeDef,
 ):
     pass
 
 
+VisualCustomActionOperationTypeDef = TypedDict(
+    "VisualCustomActionOperationTypeDef",
+    {
+        "FilterOperation": CustomActionFilterOperationTypeDef,
+        "NavigationOperation": CustomActionNavigationOperationTypeDef,
+        "URLOperation": CustomActionURLOperationTypeDef,
+        "SetParametersOperation": CustomActionSetParametersOperationTypeDef,
+    },
+    total=False,
+)
+
 DescribeDataSetResponseTypeDef = TypedDict(
     "DescribeDataSetResponseTypeDef",
     {
         "DataSet": DataSetTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredVisualCustomActionOutputTypeDef = TypedDict(
-    "_RequiredVisualCustomActionOutputTypeDef",
+_RequiredCreateDataSetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDataSetRequestRequestTypeDef",
     {
-        "CustomActionId": str,
+        "AwsAccountId": str,
+        "DataSetId": str,
         "Name": str,
-        "Trigger": VisualCustomActionTriggerType,
-        "ActionOperations": List[VisualCustomActionOperationOutputTypeDef],
+        "PhysicalTableMap": Mapping[str, PhysicalTableUnionTypeDef],
+        "ImportMode": DataSetImportModeType,
     },
 )
-_OptionalVisualCustomActionOutputTypeDef = TypedDict(
-    "_OptionalVisualCustomActionOutputTypeDef",
+_OptionalCreateDataSetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDataSetRequestRequestTypeDef",
     {
-        "Status": WidgetStatusType,
+        "LogicalTableMap": Mapping[str, LogicalTableUnionTypeDef],
+        "ColumnGroups": Sequence[ColumnGroupUnionTypeDef],
+        "FieldFolders": Mapping[str, FieldFolderUnionTypeDef],
+        "Permissions": Sequence[ResourcePermissionUnionTypeDef],
+        "RowLevelPermissionDataSet": RowLevelPermissionDataSetTypeDef,
+        "RowLevelPermissionTagConfiguration": RowLevelPermissionTagConfigurationTypeDef,
+        "ColumnLevelPermissionRules": Sequence[ColumnLevelPermissionRuleUnionTypeDef],
+        "Tags": Sequence[TagTypeDef],
+        "DataSetUsageConfiguration": DataSetUsageConfigurationTypeDef,
+        "DatasetParameters": Sequence[DatasetParameterUnionTypeDef],
     },
     total=False,
 )
 
 
-class VisualCustomActionOutputTypeDef(
-    _RequiredVisualCustomActionOutputTypeDef, _OptionalVisualCustomActionOutputTypeDef
+class CreateDataSetRequestRequestTypeDef(
+    _RequiredCreateDataSetRequestRequestTypeDef, _OptionalCreateDataSetRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredVisualCustomActionTypeDef = TypedDict(
-    "_RequiredVisualCustomActionTypeDef",
+_RequiredUpdateDataSetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDataSetRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "DataSetId": str,
+        "Name": str,
+        "PhysicalTableMap": Mapping[str, PhysicalTableUnionTypeDef],
+        "ImportMode": DataSetImportModeType,
+    },
+)
+_OptionalUpdateDataSetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDataSetRequestRequestTypeDef",
+    {
+        "LogicalTableMap": Mapping[str, LogicalTableUnionTypeDef],
+        "ColumnGroups": Sequence[ColumnGroupUnionTypeDef],
+        "FieldFolders": Mapping[str, FieldFolderUnionTypeDef],
+        "RowLevelPermissionDataSet": RowLevelPermissionDataSetTypeDef,
+        "RowLevelPermissionTagConfiguration": RowLevelPermissionTagConfigurationTypeDef,
+        "ColumnLevelPermissionRules": Sequence[ColumnLevelPermissionRuleUnionTypeDef],
+        "DataSetUsageConfiguration": DataSetUsageConfigurationTypeDef,
+        "DatasetParameters": Sequence[DatasetParameterUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateDataSetRequestRequestTypeDef(
+    _RequiredUpdateDataSetRequestRequestTypeDef, _OptionalUpdateDataSetRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredVisualCustomActionOutputTypeDef = TypedDict(
+    "_RequiredVisualCustomActionOutputTypeDef",
     {
         "CustomActionId": str,
         "Name": str,
         "Trigger": VisualCustomActionTriggerType,
-        "ActionOperations": Sequence[VisualCustomActionOperationTypeDef],
+        "ActionOperations": List[VisualCustomActionOperationOutputTypeDef],
     },
 )
-_OptionalVisualCustomActionTypeDef = TypedDict(
-    "_OptionalVisualCustomActionTypeDef",
+_OptionalVisualCustomActionOutputTypeDef = TypedDict(
+    "_OptionalVisualCustomActionOutputTypeDef",
     {
         "Status": WidgetStatusType,
     },
     total=False,
 )
 
 
-class VisualCustomActionTypeDef(
-    _RequiredVisualCustomActionTypeDef, _OptionalVisualCustomActionTypeDef
+class VisualCustomActionOutputTypeDef(
+    _RequiredVisualCustomActionOutputTypeDef, _OptionalVisualCustomActionOutputTypeDef
 ):
     pass
 
 
 _RequiredTableFieldOptionTypeDef = TypedDict(
     "_RequiredTableFieldOptionTypeDef",
     {
@@ -16710,14 +16694,15 @@
 
 class CreateTopicRequestRequestTypeDef(
     _RequiredCreateTopicRequestRequestTypeDef, _OptionalCreateTopicRequestRequestTypeDef
 ):
     pass
 
 
+TopicDetailsUnionTypeDef = Union[TopicDetailsTypeDef, TopicDetailsOutputTypeDef]
 UpdateTopicRequestRequestTypeDef = TypedDict(
     "UpdateTopicRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "TopicId": str,
         "Topic": TopicDetailsTypeDef,
     },
@@ -16787,14 +16772,38 @@
 
 class BodySectionConfigurationTypeDef(
     _RequiredBodySectionConfigurationTypeDef, _OptionalBodySectionConfigurationTypeDef
 ):
     pass
 
 
+_RequiredVisualCustomActionTypeDef = TypedDict(
+    "_RequiredVisualCustomActionTypeDef",
+    {
+        "CustomActionId": str,
+        "Name": str,
+        "Trigger": VisualCustomActionTriggerType,
+        "ActionOperations": Sequence[VisualCustomActionOperationTypeDef],
+    },
+)
+_OptionalVisualCustomActionTypeDef = TypedDict(
+    "_OptionalVisualCustomActionTypeDef",
+    {
+        "Status": WidgetStatusType,
+    },
+    total=False,
+)
+
+
+class VisualCustomActionTypeDef(
+    _RequiredVisualCustomActionTypeDef, _OptionalVisualCustomActionTypeDef
+):
+    pass
+
+
 _RequiredCustomContentVisualOutputTypeDef = TypedDict(
     "_RequiredCustomContentVisualOutputTypeDef",
     {
         "VisualId": str,
         "DataSetIdentifier": str,
     },
 )
@@ -16834,59 +16843,14 @@
 
 class EmptyVisualOutputTypeDef(
     _RequiredEmptyVisualOutputTypeDef, _OptionalEmptyVisualOutputTypeDef
 ):
     pass
 
 
-_RequiredCustomContentVisualTypeDef = TypedDict(
-    "_RequiredCustomContentVisualTypeDef",
-    {
-        "VisualId": str,
-        "DataSetIdentifier": str,
-    },
-)
-_OptionalCustomContentVisualTypeDef = TypedDict(
-    "_OptionalCustomContentVisualTypeDef",
-    {
-        "Title": VisualTitleLabelOptionsTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": CustomContentConfigurationTypeDef,
-        "Actions": Sequence[VisualCustomActionTypeDef],
-    },
-    total=False,
-)
-
-
-class CustomContentVisualTypeDef(
-    _RequiredCustomContentVisualTypeDef, _OptionalCustomContentVisualTypeDef
-):
-    pass
-
-
-_RequiredEmptyVisualTypeDef = TypedDict(
-    "_RequiredEmptyVisualTypeDef",
-    {
-        "VisualId": str,
-        "DataSetIdentifier": str,
-    },
-)
-_OptionalEmptyVisualTypeDef = TypedDict(
-    "_OptionalEmptyVisualTypeDef",
-    {
-        "Actions": Sequence[VisualCustomActionTypeDef],
-    },
-    total=False,
-)
-
-
-class EmptyVisualTypeDef(_RequiredEmptyVisualTypeDef, _OptionalEmptyVisualTypeDef):
-    pass
-
-
 TableFieldOptionsOutputTypeDef = TypedDict(
     "TableFieldOptionsOutputTypeDef",
     {
         "SelectedFieldOptions": List[TableFieldOptionTypeDef],
         "Order": List[str],
     },
     total=False,
@@ -17642,14 +17606,59 @@
         "HeaderSections": Sequence[HeaderFooterSectionConfigurationTypeDef],
         "BodySections": Sequence[BodySectionConfigurationTypeDef],
         "FooterSections": Sequence[HeaderFooterSectionConfigurationTypeDef],
         "CanvasSizeOptions": SectionBasedLayoutCanvasSizeOptionsTypeDef,
     },
 )
 
+_RequiredCustomContentVisualTypeDef = TypedDict(
+    "_RequiredCustomContentVisualTypeDef",
+    {
+        "VisualId": str,
+        "DataSetIdentifier": str,
+    },
+)
+_OptionalCustomContentVisualTypeDef = TypedDict(
+    "_OptionalCustomContentVisualTypeDef",
+    {
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": CustomContentConfigurationTypeDef,
+        "Actions": Sequence[VisualCustomActionTypeDef],
+    },
+    total=False,
+)
+
+
+class CustomContentVisualTypeDef(
+    _RequiredCustomContentVisualTypeDef, _OptionalCustomContentVisualTypeDef
+):
+    pass
+
+
+_RequiredEmptyVisualTypeDef = TypedDict(
+    "_RequiredEmptyVisualTypeDef",
+    {
+        "VisualId": str,
+        "DataSetIdentifier": str,
+    },
+)
+_OptionalEmptyVisualTypeDef = TypedDict(
+    "_OptionalEmptyVisualTypeDef",
+    {
+        "Actions": Sequence[VisualCustomActionTypeDef],
+    },
+    total=False,
+)
+
+
+class EmptyVisualTypeDef(_RequiredEmptyVisualTypeDef, _OptionalEmptyVisualTypeDef):
+    pass
+
+
 BarChartFieldWellsOutputTypeDef = TypedDict(
     "BarChartFieldWellsOutputTypeDef",
     {
         "BarChartAggregatedFieldWells": BarChartAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
@@ -19982,27 +19991,28 @@
         "Definition": TemplateVersionDefinitionOutputTypeDef,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AnalysisDefinitionUnionTypeDef = Union[AnalysisDefinitionTypeDef, AnalysisDefinitionOutputTypeDef]
 _RequiredCreateAnalysisRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnalysisRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
         "Name": str,
     },
 )
 _OptionalCreateAnalysisRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAnalysisRequestRequestTypeDef",
     {
         "Parameters": ParametersTypeDef,
-        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
+        "Permissions": Sequence[ResourcePermissionUnionTypeDef],
         "SourceEntity": AnalysisSourceEntityTypeDef,
         "ThemeArn": str,
         "Tags": Sequence[TagTypeDef],
         "Definition": AnalysisDefinitionTypeDef,
     },
     total=False,
 )
@@ -20048,15 +20058,15 @@
         "Name": str,
     },
 )
 _OptionalCreateDashboardRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDashboardRequestRequestTypeDef",
     {
         "Parameters": ParametersTypeDef,
-        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
+        "Permissions": Sequence[ResourcePermissionUnionTypeDef],
         "SourceEntity": DashboardSourceEntityTypeDef,
         "Tags": Sequence[TagTypeDef],
         "VersionDescription": str,
         "DashboardPublishOptions": DashboardPublishOptionsTypeDef,
         "ThemeArn": str,
         "Definition": DashboardVersionDefinitionTypeDef,
     },
@@ -20066,14 +20076,17 @@
 
 class CreateDashboardRequestRequestTypeDef(
     _RequiredCreateDashboardRequestRequestTypeDef, _OptionalCreateDashboardRequestRequestTypeDef
 ):
     pass
 
 
+DashboardVersionDefinitionUnionTypeDef = Union[
+    DashboardVersionDefinitionTypeDef, DashboardVersionDefinitionOutputTypeDef
+]
 _RequiredUpdateDashboardRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDashboardRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "DashboardId": str,
         "Name": str,
     },
@@ -20105,15 +20118,15 @@
         "TemplateId": str,
     },
 )
 _OptionalCreateTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTemplateRequestRequestTypeDef",
     {
         "Name": str,
-        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
+        "Permissions": Sequence[ResourcePermissionUnionTypeDef],
         "SourceEntity": TemplateSourceEntityTypeDef,
         "Tags": Sequence[TagTypeDef],
         "VersionDescription": str,
         "Definition": TemplateVersionDefinitionTypeDef,
     },
     total=False,
 )
@@ -20121,14 +20134,17 @@
 
 class CreateTemplateRequestRequestTypeDef(
     _RequiredCreateTemplateRequestRequestTypeDef, _OptionalCreateTemplateRequestRequestTypeDef
 ):
     pass
 
 
+TemplateVersionDefinitionUnionTypeDef = Union[
+    TemplateVersionDefinitionTypeDef, TemplateVersionDefinitionOutputTypeDef
+]
 _RequiredUpdateTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTemplateRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "TemplateId": str,
     },
 )
```

### Comparing `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight/type_defs.pyi` & `mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_quicksight.type_defs import AccountCustomizationTypeDef
 
-    data: AccountCustomizationTypeDef = {...}
+    data: AccountCustomizationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -248,19 +248,19 @@
     "SslPropertiesTypeDef",
     "VpcConnectionPropertiesTypeDef",
     "AssetBundleImportJobErrorTypeDef",
     "AssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef",
     "AssetBundleImportJobResourceIdOverrideConfigurationTypeDef",
     "AssetBundleImportJobThemeOverrideParametersTypeDef",
     "AssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef",
-    "AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
     "AssetBundleImportJobVPCConnectionOverrideParametersTypeDef",
+    "TimestampTypeDef",
     "AssetBundleImportJobSummaryTypeDef",
     "AssetBundleImportSourceDescriptionTypeDef",
-    "AssetBundleImportSourceTypeDef",
+    "BlobTypeDef",
     "AthenaParametersTypeDef",
     "AuroraParametersTypeDef",
     "AuroraPostgreSqlParametersTypeDef",
     "AwsIotAnalyticsParametersTypeDef",
     "DateAxisOptionsTypeDef",
     "AxisDisplayMinMaxRangeTypeDef",
     "AxisLinearScaleTypeDef",
@@ -301,42 +301,36 @@
     "ConditionalFormattingSolidColorTypeDef",
     "ConditionalFormattingCustomIconOptionsTypeDef",
     "ConditionalFormattingIconDisplayConfigurationTypeDef",
     "ConditionalFormattingIconSetTypeDef",
     "TagTypeDef",
     "CreateAccountSubscriptionRequestRequestTypeDef",
     "SignupResponseTypeDef",
-    "ResourcePermissionOutputTypeDef",
-    "ResourcePermissionTypeDef",
     "DataSetUsageConfigurationTypeDef",
-    "FieldFolderOutputTypeDef",
-    "FieldFolderTypeDef",
     "RowLevelPermissionDataSetTypeDef",
     "CreateFolderMembershipRequestRequestTypeDef",
     "FolderMemberTypeDef",
     "CreateGroupMembershipRequestRequestTypeDef",
     "GroupMemberTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "GroupTypeDef",
     "CreateIAMPolicyAssignmentRequestRequestTypeDef",
     "CreateIngestionRequestRequestTypeDef",
     "CreateTemplateAliasRequestRequestTypeDef",
     "TemplateAliasTypeDef",
     "CreateThemeAliasRequestRequestTypeDef",
     "ThemeAliasTypeDef",
-    "TopicRefreshScheduleTypeDef",
     "DecimalPlacesConfigurationTypeDef",
     "NegativeValueConfigurationTypeDef",
     "NullValueFormatConfigurationTypeDef",
     "LocalNavigationConfigurationTypeDef",
     "CustomActionURLOperationTypeDef",
     "CustomContentConfigurationTypeDef",
     "CustomNarrativeOptionsTypeDef",
     "CustomParameterValuesOutputTypeDef",
-    "CustomParameterValuesTypeDef",
     "InputColumnTypeDef",
     "DataPointDrillUpDownOptionTypeDef",
     "DataPointMenuLabelOptionTypeDef",
     "DataPointTooltipOptionTypeDef",
     "ExportToCSVOptionTypeDef",
     "ExportWithHiddenFieldsOptionTypeDef",
     "SheetControlsOptionTypeDef",
@@ -354,14 +348,15 @@
     "DataPathLabelTypeTypeDef",
     "FieldLabelTypeTypeDef",
     "MaximumLabelTypeTypeDef",
     "MinimumLabelTypeTypeDef",
     "RangeEndsLabelTypeTypeDef",
     "DataPathValueTypeDef",
     "DataSetSearchFilterTypeDef",
+    "FieldFolderOutputTypeDef",
     "OutputColumnTypeDef",
     "DataSourceErrorInfoTypeDef",
     "DatabricksParametersTypeDef",
     "ExasolParametersTypeDef",
     "JiraParametersTypeDef",
     "MariaDbParametersTypeDef",
     "MySqlParametersTypeDef",
@@ -375,21 +370,18 @@
     "SparkParametersTypeDef",
     "SqlServerParametersTypeDef",
     "TeradataParametersTypeDef",
     "TwitterParametersTypeDef",
     "DataSourceSearchFilterTypeDef",
     "DataSourceSummaryTypeDef",
     "DateTimeDatasetParameterDefaultValuesOutputTypeDef",
-    "DateTimeDatasetParameterDefaultValuesTypeDef",
     "RollingDateConfigurationTypeDef",
     "DateTimeValueWhenUnsetConfigurationOutputTypeDef",
     "MappedDataSetParameterTypeDef",
-    "DateTimeValueWhenUnsetConfigurationTypeDef",
     "DateTimeParameterOutputTypeDef",
-    "DateTimeParameterTypeDef",
     "SheetControlInfoIconLabelOptionsTypeDef",
     "DecimalDatasetParameterDefaultValuesOutputTypeDef",
     "DecimalDatasetParameterDefaultValuesTypeDef",
     "DecimalValueWhenUnsetConfigurationTypeDef",
     "DecimalParameterOutputTypeDef",
     "DecimalParameterTypeDef",
     "DeleteAccountCustomizationRequestRequestTypeDef",
@@ -416,14 +408,15 @@
     "DeleteUserRequestRequestTypeDef",
     "DeleteVPCConnectionRequestRequestTypeDef",
     "DescribeAccountCustomizationRequestRequestTypeDef",
     "DescribeAccountSettingsRequestRequestTypeDef",
     "DescribeAccountSubscriptionRequestRequestTypeDef",
     "DescribeAnalysisDefinitionRequestRequestTypeDef",
     "DescribeAnalysisPermissionsRequestRequestTypeDef",
+    "ResourcePermissionOutputTypeDef",
     "DescribeAnalysisRequestRequestTypeDef",
     "DescribeAssetBundleExportJobRequestRequestTypeDef",
     "DescribeAssetBundleImportJobRequestRequestTypeDef",
     "DescribeDashboardDefinitionRequestRequestTypeDef",
     "DescribeDashboardPermissionsRequestRequestTypeDef",
     "DescribeDashboardRequestRequestTypeDef",
     "DescribeDashboardSnapshotJobRequestRequestTypeDef",
@@ -463,14 +456,15 @@
     "UserTypeDef",
     "DescribeVPCConnectionRequestRequestTypeDef",
     "NegativeFormatTypeDef",
     "DonutCenterOptionsTypeDef",
     "ListControlSelectAllOptionsTypeDef",
     "ErrorInfoTypeDef",
     "ExcludePeriodConfigurationTypeDef",
+    "FieldFolderTypeDef",
     "FieldSortTypeDef",
     "FieldTooltipItemTypeDef",
     "GeospatialMapStyleOptionsTypeDef",
     "FilterSelectableValuesOutputTypeDef",
     "FilterSelectableValuesTypeDef",
     "SameSheetTargetVisualConfigurationOutputTypeDef",
     "SameSheetTargetVisualConfigurationTypeDef",
@@ -479,16 +473,14 @@
     "FolderSummaryTypeDef",
     "FontSizeTypeDef",
     "FontWeightTypeDef",
     "FontTypeDef",
     "TimeBasedForecastPropertiesTypeDef",
     "WhatIfPointScenarioOutputTypeDef",
     "WhatIfRangeScenarioOutputTypeDef",
-    "WhatIfPointScenarioTypeDef",
-    "WhatIfRangeScenarioTypeDef",
     "FreeFormLayoutScreenCanvasSizeOptionsTypeDef",
     "FreeFormLayoutElementBackgroundStyleTypeDef",
     "FreeFormLayoutElementBorderStyleTypeDef",
     "LoadingAnimationTypeDef",
     "SessionTagTypeDef",
     "GeospatialCoordinateBoundsTypeDef",
     "GeospatialHeatmapDataColorTypeDef",
@@ -556,15 +548,14 @@
     "ManifestFileLocationTypeDef",
     "MarginStyleTypeDef",
     "NamedEntityDefinitionMetricOutputTypeDef",
     "NamedEntityDefinitionMetricTypeDef",
     "NamespaceErrorTypeDef",
     "NetworkInterfaceTypeDef",
     "NewDefaultValuesOutputTypeDef",
-    "NewDefaultValuesTypeDef",
     "NumericRangeFilterValueTypeDef",
     "ThousandSeparatorOptionsTypeDef",
     "PercentileAggregationTypeDef",
     "StringParameterOutputTypeDef",
     "StringParameterTypeDef",
     "PercentVisibleRangeTypeDef",
     "PivotTableConditionalFormattingScopeTypeDef",
@@ -581,14 +572,15 @@
     "ReferenceLineStaticDataConfigurationTypeDef",
     "ReferenceLineStyleConfigurationTypeDef",
     "ScheduleRefreshOnEntityTypeDef",
     "RegisterUserRequestRequestTypeDef",
     "StatePersistenceConfigurationsTypeDef",
     "RegisteredUserQSearchBarEmbeddingConfigurationTypeDef",
     "RenameColumnOperationTypeDef",
+    "ResourcePermissionTypeDef",
     "RestoreAnalysisRequestRequestTypeDef",
     "RowLevelPermissionTagRuleTypeDef",
     "S3BucketConfigurationTypeDef",
     "UploadSettingsTypeDef",
     "SectionAfterPageBreakTypeDef",
     "SpacingTypeDef",
     "SheetVisualScopingConfigurationOutputTypeDef",
@@ -642,30 +634,40 @@
     "DynamicDefaultValueTypeDef",
     "FilterOperationSelectedFieldsConfigurationOutputTypeDef",
     "FilterOperationSelectedFieldsConfigurationTypeDef",
     "NumericEqualityDrillDownFilterTypeDef",
     "ParameterSelectableValuesOutputTypeDef",
     "ParameterSelectableValuesTypeDef",
     "TimeEqualityFilterOutputTypeDef",
-    "TimeEqualityFilterTypeDef",
     "TimeRangeDrillDownFilterOutputTypeDef",
-    "TimeRangeDrillDownFilterTypeDef",
     "AnalysisErrorTypeDef",
     "DashboardErrorTypeDef",
     "TemplateErrorTypeDef",
     "SearchAnalysesRequestRequestTypeDef",
     "AnalysisSourceTemplateTypeDef",
     "DashboardSourceTemplateTypeDef",
     "TemplateSourceAnalysisTypeDef",
     "AnonymousUserDashboardVisualEmbeddingConfigurationTypeDef",
     "RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef",
     "ArcAxisConfigurationTypeDef",
     "AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef",
     "AssetBundleCloudFormationOverridePropertyConfigurationTypeDef",
     "AssetBundleImportJobDataSourceCredentialsTypeDef",
+    "AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
+    "CustomParameterValuesTypeDef",
+    "DateTimeDatasetParameterDefaultValuesTypeDef",
+    "DateTimeParameterTypeDef",
+    "DateTimeValueWhenUnsetConfigurationTypeDef",
+    "NewDefaultValuesTypeDef",
+    "TimeEqualityFilterTypeDef",
+    "TimeRangeDrillDownFilterTypeDef",
+    "TopicRefreshScheduleTypeDef",
+    "WhatIfPointScenarioTypeDef",
+    "WhatIfRangeScenarioTypeDef",
+    "AssetBundleImportSourceTypeDef",
     "AxisDisplayRangeOutputTypeDef",
     "AxisDisplayRangeTypeDef",
     "AxisScaleTypeDef",
     "HistogramBinOptionsTypeDef",
     "TileStyleTypeDef",
     "BoxPlotOptionsTypeDef",
     "CreateColumnsOperationOutputTypeDef",
@@ -758,46 +760,24 @@
     "ColorsConfigurationOutputTypeDef",
     "ColorsConfigurationTypeDef",
     "ColumnTagTypeDef",
     "ColumnGroupSchemaOutputTypeDef",
     "ColumnGroupSchemaTypeDef",
     "ColumnGroupOutputTypeDef",
     "ColumnGroupTypeDef",
+    "ColumnLevelPermissionRuleUnionTypeDef",
     "DataSetSchemaOutputTypeDef",
     "DataSetSchemaTypeDef",
     "ConditionalFormattingCustomIconConditionTypeDef",
     "CreateAccountCustomizationRequestRequestTypeDef",
     "CreateNamespaceRequestRequestTypeDef",
     "CreateVPCConnectionRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateAccountSubscriptionResponseTypeDef",
-    "DescribeAnalysisPermissionsResponseTypeDef",
-    "DescribeDataSetPermissionsResponseTypeDef",
-    "DescribeDataSourcePermissionsResponseTypeDef",
-    "DescribeFolderPermissionsResponseTypeDef",
-    "DescribeFolderResolvedPermissionsResponseTypeDef",
-    "DescribeTemplatePermissionsResponseTypeDef",
-    "DescribeThemePermissionsResponseTypeDef",
-    "DescribeTopicPermissionsResponseTypeDef",
-    "LinkSharingConfigurationTypeDef",
-    "UpdateAnalysisPermissionsResponseTypeDef",
-    "UpdateFolderPermissionsResponseTypeDef",
-    "UpdateTemplatePermissionsResponseTypeDef",
-    "UpdateThemePermissionsResponseTypeDef",
-    "UpdateTopicPermissionsResponseTypeDef",
-    "CreateFolderRequestRequestTypeDef",
-    "UpdateAnalysisPermissionsRequestRequestTypeDef",
-    "UpdateDashboardPermissionsRequestRequestTypeDef",
-    "UpdateDataSetPermissionsRequestRequestTypeDef",
-    "UpdateDataSourcePermissionsRequestRequestTypeDef",
-    "UpdateFolderPermissionsRequestRequestTypeDef",
-    "UpdateTemplatePermissionsRequestRequestTypeDef",
-    "UpdateThemePermissionsRequestRequestTypeDef",
-    "UpdateTopicPermissionsRequestRequestTypeDef",
     "DataSetSummaryTypeDef",
     "CreateFolderMembershipResponseTypeDef",
     "CreateGroupMembershipResponseTypeDef",
     "DescribeGroupMembershipResponseTypeDef",
     "ListGroupMembershipsResponseTypeDef",
     "CreateGroupResponseTypeDef",
     "DescribeGroupResponseTypeDef",
@@ -809,19 +789,16 @@
     "DescribeTemplateAliasResponseTypeDef",
     "ListTemplateAliasesResponseTypeDef",
     "UpdateTemplateAliasResponseTypeDef",
     "CreateThemeAliasResponseTypeDef",
     "DescribeThemeAliasResponseTypeDef",
     "ListThemeAliasesResponseTypeDef",
     "UpdateThemeAliasResponseTypeDef",
-    "CreateTopicRefreshScheduleRequestRequestTypeDef",
-    "UpdateTopicRefreshScheduleRequestRequestTypeDef",
     "CustomActionNavigationOperationTypeDef",
     "CustomValuesConfigurationOutputTypeDef",
-    "CustomValuesConfigurationTypeDef",
     "CustomSqlOutputTypeDef",
     "CustomSqlTypeDef",
     "RelationalTableOutputTypeDef",
     "RelationalTableTypeDef",
     "SearchDashboardsRequestRequestTypeDef",
     "ListDashboardsResponseTypeDef",
     "SearchDashboardsResponseTypeDef",
@@ -836,41 +813,54 @@
     "PivotTableDataPathOptionTypeDef",
     "PivotTableFieldCollapseStateTargetOutputTypeDef",
     "PivotTableFieldCollapseStateTargetTypeDef",
     "SearchDataSetsRequestRequestTypeDef",
     "SearchDataSourcesRequestRequestTypeDef",
     "SearchDataSourcesResponseTypeDef",
     "DateTimeDatasetParameterOutputTypeDef",
-    "DateTimeDatasetParameterTypeDef",
     "TimeRangeFilterValueOutputTypeDef",
     "TimeRangeFilterValueTypeDef",
     "DecimalDatasetParameterOutputTypeDef",
     "DecimalDatasetParameterTypeDef",
+    "DescribeAnalysisPermissionsResponseTypeDef",
+    "DescribeDataSetPermissionsResponseTypeDef",
+    "DescribeDataSourcePermissionsResponseTypeDef",
+    "DescribeFolderPermissionsResponseTypeDef",
+    "DescribeFolderResolvedPermissionsResponseTypeDef",
+    "DescribeTemplatePermissionsResponseTypeDef",
+    "DescribeThemePermissionsResponseTypeDef",
+    "DescribeTopicPermissionsResponseTypeDef",
+    "LinkSharingConfigurationTypeDef",
+    "UpdateAnalysisPermissionsResponseTypeDef",
+    "UpdateFolderPermissionsResponseTypeDef",
+    "UpdateTemplatePermissionsResponseTypeDef",
+    "UpdateThemePermissionsResponseTypeDef",
+    "UpdateTopicPermissionsResponseTypeDef",
     "DescribeFolderResponseTypeDef",
     "DescribeIAMPolicyAssignmentResponseTypeDef",
     "DescribeTopicRefreshResponseTypeDef",
     "DescribeTopicRefreshScheduleResponseTypeDef",
     "TopicRefreshScheduleSummaryTypeDef",
     "DescribeUserResponseTypeDef",
     "ListUsersResponseTypeDef",
     "RegisterUserResponseTypeDef",
     "UpdateUserResponseTypeDef",
     "DisplayFormatOptionsTypeDef",
     "DonutOptionsTypeDef",
     "RelativeDatesFilterTypeDef",
+    "FieldFolderUnionTypeDef",
     "FilterOperationTargetVisualsConfigurationOutputTypeDef",
     "FilterOperationTargetVisualsConfigurationTypeDef",
     "SearchFoldersRequestRequestTypeDef",
     "ListFoldersResponseTypeDef",
     "SearchFoldersResponseTypeDef",
     "FontConfigurationTypeDef",
     "TypographyOutputTypeDef",
     "TypographyTypeDef",
     "ForecastScenarioOutputTypeDef",
-    "ForecastScenarioTypeDef",
     "FreeFormLayoutCanvasSizeOptionsTypeDef",
     "SnapshotAnonymousUserTypeDef",
     "GeospatialWindowOptionsTypeDef",
     "GeospatialHeatmapColorScaleOutputTypeDef",
     "GeospatialHeatmapColorScaleTypeDef",
     "TableSideBorderOptionsTypeDef",
     "GradientColorOutputTypeDef",
@@ -921,25 +911,24 @@
     "TileLayoutStyleTypeDef",
     "NamedEntityDefinitionOutputTypeDef",
     "NamedEntityDefinitionTypeDef",
     "NamespaceInfoV2TypeDef",
     "VPCConnectionSummaryTypeDef",
     "VPCConnectionTypeDef",
     "OverrideDatasetParameterOperationOutputTypeDef",
-    "OverrideDatasetParameterOperationTypeDef",
     "NumericSeparatorConfigurationTypeDef",
     "NumericalAggregationFunctionTypeDef",
     "ParametersOutputTypeDef",
-    "ParametersTypeDef",
     "VisibleRangeOptionsTypeDef",
     "RadarChartSeriesSettingsTypeDef",
     "TopicRangeFilterConstantTypeDef",
     "RefreshFrequencyTypeDef",
     "RegisteredUserConsoleFeatureConfigurationsTypeDef",
     "RegisteredUserDashboardFeatureConfigurationsTypeDef",
+    "ResourcePermissionUnionTypeDef",
     "RowLevelPermissionTagConfigurationOutputTypeDef",
     "RowLevelPermissionTagConfigurationTypeDef",
     "SnapshotS3DestinationConfigurationTypeDef",
     "S3SourceOutputTypeDef",
     "S3SourceTypeDef",
     "SectionPageBreakConfigurationTypeDef",
     "SectionBasedLayoutPaperCanvasSizeOptionsTypeDef",
@@ -963,61 +952,69 @@
     "DecimalDefaultValuesOutputTypeDef",
     "DecimalDefaultValuesTypeDef",
     "IntegerDefaultValuesOutputTypeDef",
     "IntegerDefaultValuesTypeDef",
     "StringDefaultValuesOutputTypeDef",
     "StringDefaultValuesTypeDef",
     "DrillDownFilterOutputTypeDef",
-    "DrillDownFilterTypeDef",
     "AnalysisTypeDef",
     "DashboardVersionTypeDef",
     "AnalysisSourceEntityTypeDef",
     "DashboardSourceEntityTypeDef",
     "TemplateSourceEntityTypeDef",
     "AnonymousUserEmbeddingExperienceConfigurationTypeDef",
     "DescribeAssetBundleExportJobResponseTypeDef",
+    "AssetBundleCloudFormationOverridePropertyConfigurationUnionTypeDef",
     "StartAssetBundleExportJobRequestRequestTypeDef",
+    "CustomValuesConfigurationTypeDef",
+    "DateTimeDatasetParameterTypeDef",
+    "ParametersTypeDef",
+    "OverrideDatasetParameterOperationTypeDef",
+    "DrillDownFilterTypeDef",
+    "CreateTopicRefreshScheduleRequestRequestTypeDef",
+    "TopicRefreshScheduleUnionTypeDef",
+    "UpdateTopicRefreshScheduleRequestRequestTypeDef",
+    "ForecastScenarioTypeDef",
     "NumericAxisOptionsOutputTypeDef",
     "NumericAxisOptionsTypeDef",
     "CategoryFilterOutputTypeDef",
     "CategoryFilterTypeDef",
     "ClusterMarkerConfigurationTypeDef",
     "TopicCategoryFilterOutputTypeDef",
     "TopicCategoryFilterTypeDef",
     "TagColumnOperationOutputTypeDef",
     "TagColumnOperationTypeDef",
+    "ColumnGroupUnionTypeDef",
     "DataSetConfigurationOutputTypeDef",
     "DataSetConfigurationTypeDef",
     "ConditionalFormattingIconTypeDef",
-    "DescribeDashboardPermissionsResponseTypeDef",
-    "UpdateDashboardPermissionsResponseTypeDef",
     "ListDataSetsResponseTypeDef",
     "SearchDataSetsResponseTypeDef",
     "DestinationParameterValueConfigurationOutputTypeDef",
-    "DestinationParameterValueConfigurationTypeDef",
     "DashboardPublishOptionsTypeDef",
     "VisualPaletteOutputTypeDef",
     "VisualPaletteTypeDef",
     "PivotTableFieldCollapseStateOptionOutputTypeDef",
     "PivotTableFieldCollapseStateOptionTypeDef",
     "TimeRangeFilterOutputTypeDef",
     "TimeRangeFilterTypeDef",
+    "DescribeDashboardPermissionsResponseTypeDef",
+    "UpdateDashboardPermissionsResponseTypeDef",
     "ListTopicRefreshSchedulesResponseTypeDef",
     "DefaultFormattingTypeDef",
     "CustomActionFilterOperationOutputTypeDef",
     "CustomActionFilterOperationTypeDef",
     "AxisLabelOptionsTypeDef",
     "DataLabelOptionsOutputTypeDef",
     "DataLabelOptionsTypeDef",
     "FunnelChartDataLabelOptionsTypeDef",
     "LabelOptionsTypeDef",
     "PanelTitleOptionsTypeDef",
     "TableFieldCustomTextContentTypeDef",
     "ForecastConfigurationOutputTypeDef",
-    "ForecastConfigurationTypeDef",
     "DefaultFreeFormLayoutConfigurationTypeDef",
     "SnapshotUserConfigurationTypeDef",
     "GeospatialHeatmapConfigurationOutputTypeDef",
     "GeospatialHeatmapConfigurationTypeDef",
     "GlobalTableBorderOptionsTypeDef",
     "ConditionalFormattingGradientColorOutputTypeDef",
     "ConditionalFormattingGradientColorTypeDef",
@@ -1045,52 +1042,64 @@
     "ScrollBarOptionsTypeDef",
     "TopicDateRangeFilterTypeDef",
     "TopicNumericRangeFilterTypeDef",
     "RefreshScheduleOutputTypeDef",
     "RefreshScheduleTypeDef",
     "RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef",
     "RegisteredUserDashboardEmbeddingConfigurationTypeDef",
+    "CreateFolderRequestRequestTypeDef",
+    "UpdateAnalysisPermissionsRequestRequestTypeDef",
+    "UpdateDashboardPermissionsRequestRequestTypeDef",
+    "UpdateDataSetPermissionsRequestRequestTypeDef",
+    "UpdateDataSourcePermissionsRequestRequestTypeDef",
+    "UpdateFolderPermissionsRequestRequestTypeDef",
+    "UpdateTemplatePermissionsRequestRequestTypeDef",
+    "UpdateThemePermissionsRequestRequestTypeDef",
+    "UpdateTopicPermissionsRequestRequestTypeDef",
+    "RowLevelPermissionTagConfigurationUnionTypeDef",
     "SnapshotDestinationConfigurationOutputTypeDef",
     "SnapshotDestinationConfigurationTypeDef",
     "SnapshotJobS3ResultTypeDef",
     "PhysicalTableOutputTypeDef",
     "PhysicalTableTypeDef",
     "SectionBasedLayoutCanvasSizeOptionsTypeDef",
     "FilterScopeConfigurationOutputTypeDef",
     "FilterScopeConfigurationTypeDef",
     "FreeFormLayoutElementOutputTypeDef",
     "FreeFormLayoutElementTypeDef",
     "SnapshotFileGroupOutputTypeDef",
     "SnapshotFileGroupTypeDef",
     "DatasetParameterOutputTypeDef",
-    "DatasetParameterTypeDef",
     "DateTimeParameterDeclarationOutputTypeDef",
     "DateTimeParameterDeclarationTypeDef",
     "DecimalParameterDeclarationOutputTypeDef",
     "DecimalParameterDeclarationTypeDef",
     "IntegerParameterDeclarationOutputTypeDef",
     "IntegerParameterDeclarationTypeDef",
     "StringParameterDeclarationOutputTypeDef",
     "StringParameterDeclarationTypeDef",
     "DateTimeHierarchyOutputTypeDef",
     "ExplicitHierarchyOutputTypeDef",
     "PredefinedHierarchyOutputTypeDef",
-    "DateTimeHierarchyTypeDef",
-    "ExplicitHierarchyTypeDef",
-    "PredefinedHierarchyTypeDef",
     "DescribeAnalysisResponseTypeDef",
     "DashboardTypeDef",
     "GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef",
+    "DestinationParameterValueConfigurationTypeDef",
+    "DatasetParameterTypeDef",
+    "ParametersUnionTypeDef",
+    "DateTimeHierarchyTypeDef",
+    "ExplicitHierarchyTypeDef",
+    "PredefinedHierarchyTypeDef",
+    "ForecastConfigurationTypeDef",
     "AxisDataOptionsOutputTypeDef",
     "AxisDataOptionsTypeDef",
     "TransformOperationOutputTypeDef",
     "TransformOperationTypeDef",
     "TemplateVersionTypeDef",
     "SetParameterValueConfigurationOutputTypeDef",
-    "SetParameterValueConfigurationTypeDef",
     "PivotTableFieldOptionsOutputTypeDef",
     "PivotTableFieldOptionsTypeDef",
     "TopicCalculatedFieldOutputTypeDef",
     "TopicCalculatedFieldTypeDef",
     "TopicColumnOutputTypeDef",
     "TopicColumnTypeDef",
     "ChartAxisLabelOptionsOutputTypeDef",
@@ -1130,34 +1139,37 @@
     "NumericRangeFilterTypeDef",
     "ReferenceLineDynamicDataConfigurationTypeDef",
     "TopicFilterOutputTypeDef",
     "TopicFilterTypeDef",
     "DescribeRefreshScheduleResponseTypeDef",
     "ListRefreshSchedulesResponseTypeDef",
     "CreateRefreshScheduleRequestRequestTypeDef",
+    "RefreshScheduleUnionTypeDef",
     "UpdateRefreshScheduleRequestRequestTypeDef",
     "RegisteredUserEmbeddingExperienceConfigurationTypeDef",
     "SnapshotJobResultFileGroupTypeDef",
+    "PhysicalTableUnionTypeDef",
     "DefaultSectionBasedLayoutConfigurationTypeDef",
     "FreeFormLayoutConfigurationOutputTypeDef",
     "FreeFormSectionLayoutConfigurationOutputTypeDef",
     "FreeFormLayoutConfigurationTypeDef",
     "FreeFormSectionLayoutConfigurationTypeDef",
     "SnapshotConfigurationOutputTypeDef",
     "SnapshotConfigurationTypeDef",
     "ParameterDeclarationOutputTypeDef",
     "ParameterDeclarationTypeDef",
     "ColumnHierarchyOutputTypeDef",
-    "ColumnHierarchyTypeDef",
     "DescribeDashboardResponseTypeDef",
+    "SetParameterValueConfigurationTypeDef",
+    "DatasetParameterUnionTypeDef",
+    "ColumnHierarchyTypeDef",
     "LogicalTableOutputTypeDef",
     "LogicalTableTypeDef",
     "TemplateTypeDef",
     "CustomActionSetParametersOperationOutputTypeDef",
-    "CustomActionSetParametersOperationTypeDef",
     "AxisDisplayOptionsOutputTypeDef",
     "AxisDisplayOptionsTypeDef",
     "FilterDateTimePickerControlTypeDef",
     "ParameterDateTimePickerControlTypeDef",
     "FilterDropDownControlOutputTypeDef",
     "FilterDropDownControlTypeDef",
     "ParameterDropDownControlOutputTypeDef",
@@ -1204,14 +1216,15 @@
     "AssetBundleImportJobOverrideParametersOutputTypeDef",
     "AssetBundleImportJobOverrideParametersTypeDef",
     "DataSourceCredentialsTypeDef",
     "DescribeDataSourceResponseTypeDef",
     "ListDataSourcesResponseTypeDef",
     "ThemeVersionTypeDef",
     "CreateThemeRequestRequestTypeDef",
+    "ThemeConfigurationUnionTypeDef",
     "UpdateThemeRequestRequestTypeDef",
     "ComparisonConfigurationTypeDef",
     "DateTimeFormatConfigurationTypeDef",
     "NumberFormatConfigurationTypeDef",
     "ReferenceLineValueLabelConfigurationTypeDef",
     "StringFormatConfigurationTypeDef",
     "TopBottomFilterOutputTypeDef",
@@ -1225,21 +1238,21 @@
     "DatasetMetadataTypeDef",
     "GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef",
     "AnonymousUserSnapshotJobResultTypeDef",
     "DefaultPaginatedLayoutConfigurationTypeDef",
     "SectionLayoutConfigurationOutputTypeDef",
     "SectionLayoutConfigurationTypeDef",
     "DescribeDashboardSnapshotJobResponseTypeDef",
+    "SnapshotConfigurationUnionTypeDef",
     "StartDashboardSnapshotJobRequestRequestTypeDef",
+    "CustomActionSetParametersOperationTypeDef",
     "DataSetTypeDef",
-    "CreateDataSetRequestRequestTypeDef",
-    "UpdateDataSetRequestRequestTypeDef",
+    "LogicalTableUnionTypeDef",
     "DescribeTemplateResponseTypeDef",
     "VisualCustomActionOperationOutputTypeDef",
-    "VisualCustomActionOperationTypeDef",
     "LineSeriesAxisDisplayOptionsOutputTypeDef",
     "LineSeriesAxisDisplayOptionsTypeDef",
     "FilterControlOutputTypeDef",
     "FilterControlTypeDef",
     "ParameterControlOutputTypeDef",
     "ParameterControlTypeDef",
     "TableFieldURLConfigurationTypeDef",
@@ -1252,14 +1265,15 @@
     "TableCellConditionalFormattingOutputTypeDef",
     "GaugeChartConditionalFormattingOptionTypeDef",
     "KPIConditionalFormattingOptionTypeDef",
     "FilledMapShapeConditionalFormattingTypeDef",
     "PivotTableCellConditionalFormattingTypeDef",
     "TableCellConditionalFormattingTypeDef",
     "DescribeAssetBundleImportJobResponseTypeDef",
+    "AssetBundleImportJobOverrideParametersUnionTypeDef",
     "StartAssetBundleImportJobRequestRequestTypeDef",
     "CreateDataSourceRequestRequestTypeDef",
     "UpdateDataSourceRequestRequestTypeDef",
     "ThemeTypeDef",
     "GaugeChartOptionsTypeDef",
     "KPIOptionsTypeDef",
     "DateDimensionFieldTypeDef",
@@ -1310,17 +1324,19 @@
     "TopicDetailsTypeDef",
     "SnapshotJobResultTypeDef",
     "DefaultNewSheetConfigurationTypeDef",
     "BodySectionContentOutputTypeDef",
     "HeaderFooterSectionConfigurationOutputTypeDef",
     "BodySectionContentTypeDef",
     "HeaderFooterSectionConfigurationTypeDef",
+    "VisualCustomActionOperationTypeDef",
     "DescribeDataSetResponseTypeDef",
+    "CreateDataSetRequestRequestTypeDef",
+    "UpdateDataSetRequestRequestTypeDef",
     "VisualCustomActionOutputTypeDef",
-    "VisualCustomActionTypeDef",
     "TableFieldOptionTypeDef",
     "GaugeChartConditionalFormattingOutputTypeDef",
     "KPIConditionalFormattingOutputTypeDef",
     "FilledMapConditionalFormattingOptionOutputTypeDef",
     "PivotTableConditionalFormattingOptionOutputTypeDef",
     "TableConditionalFormattingOptionOutputTypeDef",
     "GaugeChartConditionalFormattingTypeDef",
@@ -1339,23 +1355,23 @@
     "FilterGroupTypeDef",
     "PivotTableSortConfigurationOutputTypeDef",
     "PivotTableSortConfigurationTypeDef",
     "TooltipOptionsOutputTypeDef",
     "TooltipOptionsTypeDef",
     "DescribeTopicResponseTypeDef",
     "CreateTopicRequestRequestTypeDef",
+    "TopicDetailsUnionTypeDef",
     "UpdateTopicRequestRequestTypeDef",
     "DescribeDashboardSnapshotJobResultResponseTypeDef",
     "AnalysisDefaultsTypeDef",
     "BodySectionConfigurationOutputTypeDef",
     "BodySectionConfigurationTypeDef",
+    "VisualCustomActionTypeDef",
     "CustomContentVisualOutputTypeDef",
     "EmptyVisualOutputTypeDef",
-    "CustomContentVisualTypeDef",
-    "EmptyVisualTypeDef",
     "TableFieldOptionsOutputTypeDef",
     "TableFieldOptionsTypeDef",
     "FilledMapConditionalFormattingOutputTypeDef",
     "PivotTableConditionalFormattingOutputTypeDef",
     "TableConditionalFormattingOutputTypeDef",
     "FilledMapConditionalFormattingTypeDef",
     "PivotTableConditionalFormattingTypeDef",
@@ -1412,14 +1428,16 @@
     "WaterfallChartAggregatedFieldWellsTypeDef",
     "WordCloudAggregatedFieldWellsOutputTypeDef",
     "WordCloudAggregatedFieldWellsTypeDef",
     "TableUnaggregatedFieldWellsOutputTypeDef",
     "TableUnaggregatedFieldWellsTypeDef",
     "SectionBasedLayoutConfigurationOutputTypeDef",
     "SectionBasedLayoutConfigurationTypeDef",
+    "CustomContentVisualTypeDef",
+    "EmptyVisualTypeDef",
     "BarChartFieldWellsOutputTypeDef",
     "BarChartFieldWellsTypeDef",
     "BoxPlotFieldWellsOutputTypeDef",
     "BoxPlotFieldWellsTypeDef",
     "ComboChartFieldWellsOutputTypeDef",
     "ComboChartFieldWellsTypeDef",
     "FilledMapFieldWellsOutputTypeDef",
@@ -1550,19 +1568,22 @@
     "TemplateVersionDefinitionOutputTypeDef",
     "AnalysisDefinitionTypeDef",
     "DashboardVersionDefinitionTypeDef",
     "TemplateVersionDefinitionTypeDef",
     "DescribeAnalysisDefinitionResponseTypeDef",
     "DescribeDashboardDefinitionResponseTypeDef",
     "DescribeTemplateDefinitionResponseTypeDef",
+    "AnalysisDefinitionUnionTypeDef",
     "CreateAnalysisRequestRequestTypeDef",
     "UpdateAnalysisRequestRequestTypeDef",
     "CreateDashboardRequestRequestTypeDef",
+    "DashboardVersionDefinitionUnionTypeDef",
     "UpdateDashboardRequestRequestTypeDef",
     "CreateTemplateRequestRequestTypeDef",
+    "TemplateVersionDefinitionUnionTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
 )
 
 AccountCustomizationTypeDef = TypedDict(
     "AccountCustomizationTypeDef",
     {
         "DefaultTheme": str,
@@ -2240,35 +2261,14 @@
 
 class AssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef(
     _RequiredAssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef,
     _OptionalAssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef,
 ):
     pass
 
-_RequiredAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef = TypedDict(
-    "_RequiredAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
-    {
-        "DataSetId": str,
-        "ScheduleId": str,
-    },
-)
-_OptionalAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef = TypedDict(
-    "_OptionalAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
-    {
-        "StartAfterDateTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-class AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef(
-    _RequiredAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef,
-    _OptionalAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef,
-):
-    pass
-
 _RequiredAssetBundleImportJobVPCConnectionOverrideParametersTypeDef = TypedDict(
     "_RequiredAssetBundleImportJobVPCConnectionOverrideParametersTypeDef",
     {
         "VPCConnectionId": str,
     },
 )
 _OptionalAssetBundleImportJobVPCConnectionOverrideParametersTypeDef = TypedDict(
@@ -2285,14 +2285,15 @@
 
 class AssetBundleImportJobVPCConnectionOverrideParametersTypeDef(
     _RequiredAssetBundleImportJobVPCConnectionOverrideParametersTypeDef,
     _OptionalAssetBundleImportJobVPCConnectionOverrideParametersTypeDef,
 ):
     pass
 
+TimestampTypeDef = Union[datetime, str]
 AssetBundleImportJobSummaryTypeDef = TypedDict(
     "AssetBundleImportJobSummaryTypeDef",
     {
         "JobStatus": AssetBundleImportJobStatusType,
         "Arn": str,
         "CreatedTime": datetime,
         "AssetBundleImportJobId": str,
@@ -2306,23 +2307,15 @@
     {
         "Body": str,
         "S3Uri": str,
     },
     total=False,
 )
 
-AssetBundleImportSourceTypeDef = TypedDict(
-    "AssetBundleImportSourceTypeDef",
-    {
-        "Body": Union[str, bytes, IO[Any], StreamingBody],
-        "S3Uri": str,
-    },
-    total=False,
-)
-
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 AthenaParametersTypeDef = TypedDict(
     "AthenaParametersTypeDef",
     {
         "WorkGroup": str,
         "RoleArn": str,
     },
     total=False,
@@ -2882,57 +2875,23 @@
         "userLoginName": str,
         "accountName": str,
         "directoryType": str,
     },
     total=False,
 )
 
-ResourcePermissionOutputTypeDef = TypedDict(
-    "ResourcePermissionOutputTypeDef",
-    {
-        "Principal": str,
-        "Actions": List[str],
-    },
-)
-
-ResourcePermissionTypeDef = TypedDict(
-    "ResourcePermissionTypeDef",
-    {
-        "Principal": str,
-        "Actions": Sequence[str],
-    },
-)
-
 DataSetUsageConfigurationTypeDef = TypedDict(
     "DataSetUsageConfigurationTypeDef",
     {
         "DisableUseAsDirectQuerySource": bool,
         "DisableUseAsImportedSource": bool,
     },
     total=False,
 )
 
-FieldFolderOutputTypeDef = TypedDict(
-    "FieldFolderOutputTypeDef",
-    {
-        "description": str,
-        "columns": List[str],
-    },
-    total=False,
-)
-
-FieldFolderTypeDef = TypedDict(
-    "FieldFolderTypeDef",
-    {
-        "description": str,
-        "columns": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredRowLevelPermissionDataSetTypeDef = TypedDict(
     "_RequiredRowLevelPermissionDataSetTypeDef",
     {
         "Arn": str,
         "PermissionPolicy": RowLevelPermissionPolicyType,
     },
 )
@@ -3102,37 +3061,14 @@
         "Arn": str,
         "AliasName": str,
         "ThemeVersionNumber": int,
     },
     total=False,
 )
 
-_RequiredTopicRefreshScheduleTypeDef = TypedDict(
-    "_RequiredTopicRefreshScheduleTypeDef",
-    {
-        "IsEnabled": bool,
-        "BasedOnSpiceSchedule": bool,
-    },
-)
-_OptionalTopicRefreshScheduleTypeDef = TypedDict(
-    "_OptionalTopicRefreshScheduleTypeDef",
-    {
-        "StartingAt": Union[datetime, str],
-        "Timezone": str,
-        "RepeatAt": str,
-        "TopicScheduleType": TopicScheduleTypeType,
-    },
-    total=False,
-)
-
-class TopicRefreshScheduleTypeDef(
-    _RequiredTopicRefreshScheduleTypeDef, _OptionalTopicRefreshScheduleTypeDef
-):
-    pass
-
 DecimalPlacesConfigurationTypeDef = TypedDict(
     "DecimalPlacesConfigurationTypeDef",
     {
         "DecimalPlaces": int,
     },
 )
 
@@ -3189,25 +3125,14 @@
         "IntegerValues": List[int],
         "DecimalValues": List[float],
         "DateTimeValues": List[datetime],
     },
     total=False,
 )
 
-CustomParameterValuesTypeDef = TypedDict(
-    "CustomParameterValuesTypeDef",
-    {
-        "StringValues": Sequence[str],
-        "IntegerValues": Sequence[int],
-        "DecimalValues": Sequence[float],
-        "DateTimeValues": Sequence[Union[datetime, str]],
-    },
-    total=False,
-)
-
 InputColumnTypeDef = TypedDict(
     "InputColumnTypeDef",
     {
         "Name": str,
         "Type": InputColumnDataTypeType,
     },
 )
@@ -3442,14 +3367,23 @@
     {
         "Operator": FilterOperatorType,
         "Name": DataSetFilterAttributeType,
         "Value": str,
     },
 )
 
+FieldFolderOutputTypeDef = TypedDict(
+    "FieldFolderOutputTypeDef",
+    {
+        "description": str,
+        "columns": List[str],
+    },
+    total=False,
+)
+
 OutputColumnTypeDef = TypedDict(
     "OutputColumnTypeDef",
     {
         "Name": str,
         "Description": str,
         "Type": ColumnDataTypeType,
     },
@@ -3639,22 +3573,14 @@
     "DateTimeDatasetParameterDefaultValuesOutputTypeDef",
     {
         "StaticValues": List[datetime],
     },
     total=False,
 )
 
-DateTimeDatasetParameterDefaultValuesTypeDef = TypedDict(
-    "DateTimeDatasetParameterDefaultValuesTypeDef",
-    {
-        "StaticValues": Sequence[Union[datetime, str]],
-    },
-    total=False,
-)
-
 _RequiredRollingDateConfigurationTypeDef = TypedDict(
     "_RequiredRollingDateConfigurationTypeDef",
     {
         "Expression": str,
     },
 )
 _OptionalRollingDateConfigurationTypeDef = TypedDict(
@@ -3683,39 +3609,22 @@
     "MappedDataSetParameterTypeDef",
     {
         "DataSetIdentifier": str,
         "DataSetParameterName": str,
     },
 )
 
-DateTimeValueWhenUnsetConfigurationTypeDef = TypedDict(
-    "DateTimeValueWhenUnsetConfigurationTypeDef",
-    {
-        "ValueWhenUnsetOption": ValueWhenUnsetOptionType,
-        "CustomValue": Union[datetime, str],
-    },
-    total=False,
-)
-
 DateTimeParameterOutputTypeDef = TypedDict(
     "DateTimeParameterOutputTypeDef",
     {
         "Name": str,
         "Values": List[datetime],
     },
 )
 
-DateTimeParameterTypeDef = TypedDict(
-    "DateTimeParameterTypeDef",
-    {
-        "Name": str,
-        "Values": Sequence[Union[datetime, str]],
-    },
-)
-
 SheetControlInfoIconLabelOptionsTypeDef = TypedDict(
     "SheetControlInfoIconLabelOptionsTypeDef",
     {
         "Visibility": VisibilityType,
         "InfoIconText": str,
     },
     total=False,
@@ -4065,14 +3974,22 @@
     "DescribeAnalysisPermissionsRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
     },
 )
 
+ResourcePermissionOutputTypeDef = TypedDict(
+    "ResourcePermissionOutputTypeDef",
+    {
+        "Principal": str,
+        "Actions": List[str],
+    },
+)
+
 DescribeAnalysisRequestRequestTypeDef = TypedDict(
     "DescribeAnalysisRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
     },
 )
@@ -4573,14 +4490,23 @@
 )
 
 class ExcludePeriodConfigurationTypeDef(
     _RequiredExcludePeriodConfigurationTypeDef, _OptionalExcludePeriodConfigurationTypeDef
 ):
     pass
 
+FieldFolderTypeDef = TypedDict(
+    "FieldFolderTypeDef",
+    {
+        "description": str,
+        "columns": Sequence[str],
+    },
+    total=False,
+)
+
 FieldSortTypeDef = TypedDict(
     "FieldSortTypeDef",
     {
         "FieldId": str,
         "Direction": SortDirectionType,
     },
 )
@@ -4725,31 +4651,14 @@
     {
         "StartDate": datetime,
         "EndDate": datetime,
         "Value": float,
     },
 )
 
-WhatIfPointScenarioTypeDef = TypedDict(
-    "WhatIfPointScenarioTypeDef",
-    {
-        "Date": Union[datetime, str],
-        "Value": float,
-    },
-)
-
-WhatIfRangeScenarioTypeDef = TypedDict(
-    "WhatIfRangeScenarioTypeDef",
-    {
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "Value": float,
-    },
-)
-
 FreeFormLayoutScreenCanvasSizeOptionsTypeDef = TypedDict(
     "FreeFormLayoutScreenCanvasSizeOptionsTypeDef",
     {
         "OptimizedViewPortWidth": str,
     },
 )
 
@@ -5789,25 +5698,14 @@
         "DecimalStaticValues": List[float],
         "DateTimeStaticValues": List[datetime],
         "IntegerStaticValues": List[int],
     },
     total=False,
 )
 
-NewDefaultValuesTypeDef = TypedDict(
-    "NewDefaultValuesTypeDef",
-    {
-        "StringStaticValues": Sequence[str],
-        "DecimalStaticValues": Sequence[float],
-        "DateTimeStaticValues": Sequence[Union[datetime, str]],
-        "IntegerStaticValues": Sequence[int],
-    },
-    total=False,
-)
-
 NumericRangeFilterValueTypeDef = TypedDict(
     "NumericRangeFilterValueTypeDef",
     {
         "StaticValue": float,
         "Parameter": str,
     },
     total=False,
@@ -6029,14 +5927,22 @@
     "RenameColumnOperationTypeDef",
     {
         "ColumnName": str,
         "NewColumnName": str,
     },
 )
 
+ResourcePermissionTypeDef = TypedDict(
+    "ResourcePermissionTypeDef",
+    {
+        "Principal": str,
+        "Actions": Sequence[str],
+    },
+)
+
 RestoreAnalysisRequestRequestTypeDef = TypedDict(
     "RestoreAnalysisRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
     },
 )
@@ -6795,56 +6701,24 @@
 )
 
 class TimeEqualityFilterOutputTypeDef(
     _RequiredTimeEqualityFilterOutputTypeDef, _OptionalTimeEqualityFilterOutputTypeDef
 ):
     pass
 
-_RequiredTimeEqualityFilterTypeDef = TypedDict(
-    "_RequiredTimeEqualityFilterTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierTypeDef,
-    },
-)
-_OptionalTimeEqualityFilterTypeDef = TypedDict(
-    "_OptionalTimeEqualityFilterTypeDef",
-    {
-        "Value": Union[datetime, str],
-        "ParameterName": str,
-        "TimeGranularity": TimeGranularityType,
-    },
-    total=False,
-)
-
-class TimeEqualityFilterTypeDef(
-    _RequiredTimeEqualityFilterTypeDef, _OptionalTimeEqualityFilterTypeDef
-):
-    pass
-
 TimeRangeDrillDownFilterOutputTypeDef = TypedDict(
     "TimeRangeDrillDownFilterOutputTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
         "RangeMinimum": datetime,
         "RangeMaximum": datetime,
         "TimeGranularity": TimeGranularityType,
     },
 )
 
-TimeRangeDrillDownFilterTypeDef = TypedDict(
-    "TimeRangeDrillDownFilterTypeDef",
-    {
-        "Column": ColumnIdentifierTypeDef,
-        "RangeMinimum": Union[datetime, str],
-        "RangeMaximum": Union[datetime, str],
-        "TimeGranularity": TimeGranularityType,
-    },
-)
-
 AnalysisErrorTypeDef = TypedDict(
     "AnalysisErrorTypeDef",
     {
         "Type": AnalysisErrorTypeType,
         "Message": str,
         "ViolatedEntities": List[EntityTypeDef],
     },
@@ -6980,14 +6854,163 @@
     {
         "CredentialPair": AssetBundleImportJobDataSourceCredentialPairTypeDef,
         "SecretArn": str,
     },
     total=False,
 )
 
+_RequiredAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef = TypedDict(
+    "_RequiredAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
+    {
+        "DataSetId": str,
+        "ScheduleId": str,
+    },
+)
+_OptionalAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef = TypedDict(
+    "_OptionalAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
+    {
+        "StartAfterDateTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef(
+    _RequiredAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef,
+    _OptionalAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef,
+):
+    pass
+
+CustomParameterValuesTypeDef = TypedDict(
+    "CustomParameterValuesTypeDef",
+    {
+        "StringValues": Sequence[str],
+        "IntegerValues": Sequence[int],
+        "DecimalValues": Sequence[float],
+        "DateTimeValues": Sequence[TimestampTypeDef],
+    },
+    total=False,
+)
+
+DateTimeDatasetParameterDefaultValuesTypeDef = TypedDict(
+    "DateTimeDatasetParameterDefaultValuesTypeDef",
+    {
+        "StaticValues": Sequence[TimestampTypeDef],
+    },
+    total=False,
+)
+
+DateTimeParameterTypeDef = TypedDict(
+    "DateTimeParameterTypeDef",
+    {
+        "Name": str,
+        "Values": Sequence[TimestampTypeDef],
+    },
+)
+
+DateTimeValueWhenUnsetConfigurationTypeDef = TypedDict(
+    "DateTimeValueWhenUnsetConfigurationTypeDef",
+    {
+        "ValueWhenUnsetOption": ValueWhenUnsetOptionType,
+        "CustomValue": TimestampTypeDef,
+    },
+    total=False,
+)
+
+NewDefaultValuesTypeDef = TypedDict(
+    "NewDefaultValuesTypeDef",
+    {
+        "StringStaticValues": Sequence[str],
+        "DecimalStaticValues": Sequence[float],
+        "DateTimeStaticValues": Sequence[TimestampTypeDef],
+        "IntegerStaticValues": Sequence[int],
+    },
+    total=False,
+)
+
+_RequiredTimeEqualityFilterTypeDef = TypedDict(
+    "_RequiredTimeEqualityFilterTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+    },
+)
+_OptionalTimeEqualityFilterTypeDef = TypedDict(
+    "_OptionalTimeEqualityFilterTypeDef",
+    {
+        "Value": TimestampTypeDef,
+        "ParameterName": str,
+        "TimeGranularity": TimeGranularityType,
+    },
+    total=False,
+)
+
+class TimeEqualityFilterTypeDef(
+    _RequiredTimeEqualityFilterTypeDef, _OptionalTimeEqualityFilterTypeDef
+):
+    pass
+
+TimeRangeDrillDownFilterTypeDef = TypedDict(
+    "TimeRangeDrillDownFilterTypeDef",
+    {
+        "Column": ColumnIdentifierTypeDef,
+        "RangeMinimum": TimestampTypeDef,
+        "RangeMaximum": TimestampTypeDef,
+        "TimeGranularity": TimeGranularityType,
+    },
+)
+
+_RequiredTopicRefreshScheduleTypeDef = TypedDict(
+    "_RequiredTopicRefreshScheduleTypeDef",
+    {
+        "IsEnabled": bool,
+        "BasedOnSpiceSchedule": bool,
+    },
+)
+_OptionalTopicRefreshScheduleTypeDef = TypedDict(
+    "_OptionalTopicRefreshScheduleTypeDef",
+    {
+        "StartingAt": TimestampTypeDef,
+        "Timezone": str,
+        "RepeatAt": str,
+        "TopicScheduleType": TopicScheduleTypeType,
+    },
+    total=False,
+)
+
+class TopicRefreshScheduleTypeDef(
+    _RequiredTopicRefreshScheduleTypeDef, _OptionalTopicRefreshScheduleTypeDef
+):
+    pass
+
+WhatIfPointScenarioTypeDef = TypedDict(
+    "WhatIfPointScenarioTypeDef",
+    {
+        "Date": TimestampTypeDef,
+        "Value": float,
+    },
+)
+
+WhatIfRangeScenarioTypeDef = TypedDict(
+    "WhatIfRangeScenarioTypeDef",
+    {
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "Value": float,
+    },
+)
+
+AssetBundleImportSourceTypeDef = TypedDict(
+    "AssetBundleImportSourceTypeDef",
+    {
+        "Body": BlobTypeDef,
+        "S3Uri": str,
+    },
+    total=False,
+)
+
 AxisDisplayRangeOutputTypeDef = TypedDict(
     "AxisDisplayRangeOutputTypeDef",
     {
         "MinMax": AxisDisplayMinMaxRangeTypeDef,
         "DataDriven": Dict[str, Any],
     },
     total=False,
@@ -8067,14 +8090,17 @@
     "ColumnGroupTypeDef",
     {
         "GeoSpatialColumnGroup": GeoSpatialColumnGroupTypeDef,
     },
     total=False,
 )
 
+ColumnLevelPermissionRuleUnionTypeDef = Union[
+    ColumnLevelPermissionRuleTypeDef, ColumnLevelPermissionRuleOutputTypeDef
+]
 DataSetSchemaOutputTypeDef = TypedDict(
     "DataSetSchemaOutputTypeDef",
     {
         "ColumnSchemaList": List[ColumnSchemaTypeDef],
     },
     total=False,
 )
@@ -8202,416 +8228,14 @@
         "SignupResponse": SignupResponseTypeDef,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAnalysisPermissionsResponseTypeDef = TypedDict(
-    "DescribeAnalysisPermissionsResponseTypeDef",
-    {
-        "AnalysisId": str,
-        "AnalysisArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDataSetPermissionsResponseTypeDef = TypedDict(
-    "DescribeDataSetPermissionsResponseTypeDef",
-    {
-        "DataSetArn": str,
-        "DataSetId": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDataSourcePermissionsResponseTypeDef = TypedDict(
-    "DescribeDataSourcePermissionsResponseTypeDef",
-    {
-        "DataSourceArn": str,
-        "DataSourceId": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFolderPermissionsResponseTypeDef = TypedDict(
-    "DescribeFolderPermissionsResponseTypeDef",
-    {
-        "Status": int,
-        "FolderId": str,
-        "Arn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFolderResolvedPermissionsResponseTypeDef = TypedDict(
-    "DescribeFolderResolvedPermissionsResponseTypeDef",
-    {
-        "Status": int,
-        "FolderId": str,
-        "Arn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeTemplatePermissionsResponseTypeDef = TypedDict(
-    "DescribeTemplatePermissionsResponseTypeDef",
-    {
-        "TemplateId": str,
-        "TemplateArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeThemePermissionsResponseTypeDef = TypedDict(
-    "DescribeThemePermissionsResponseTypeDef",
-    {
-        "ThemeId": str,
-        "ThemeArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeTopicPermissionsResponseTypeDef = TypedDict(
-    "DescribeTopicPermissionsResponseTypeDef",
-    {
-        "TopicId": str,
-        "TopicArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LinkSharingConfigurationTypeDef = TypedDict(
-    "LinkSharingConfigurationTypeDef",
-    {
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-    },
-    total=False,
-)
-
-UpdateAnalysisPermissionsResponseTypeDef = TypedDict(
-    "UpdateAnalysisPermissionsResponseTypeDef",
-    {
-        "AnalysisArn": str,
-        "AnalysisId": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateFolderPermissionsResponseTypeDef = TypedDict(
-    "UpdateFolderPermissionsResponseTypeDef",
-    {
-        "Status": int,
-        "Arn": str,
-        "FolderId": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTemplatePermissionsResponseTypeDef = TypedDict(
-    "UpdateTemplatePermissionsResponseTypeDef",
-    {
-        "TemplateId": str,
-        "TemplateArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateThemePermissionsResponseTypeDef = TypedDict(
-    "UpdateThemePermissionsResponseTypeDef",
-    {
-        "ThemeId": str,
-        "ThemeArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTopicPermissionsResponseTypeDef = TypedDict(
-    "UpdateTopicPermissionsResponseTypeDef",
-    {
-        "TopicId": str,
-        "TopicArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredCreateFolderRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFolderRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "FolderId": str,
-    },
-)
-_OptionalCreateFolderRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFolderRequestRequestTypeDef",
-    {
-        "Name": str,
-        "FolderType": Literal["SHARED"],
-        "ParentFolderArn": str,
-        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateFolderRequestRequestTypeDef(
-    _RequiredCreateFolderRequestRequestTypeDef, _OptionalCreateFolderRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateAnalysisPermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAnalysisPermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "AnalysisId": str,
-    },
-)
-_OptionalUpdateAnalysisPermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAnalysisPermissionsRequestRequestTypeDef",
-    {
-        "GrantPermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-        "RevokePermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-class UpdateAnalysisPermissionsRequestRequestTypeDef(
-    _RequiredUpdateAnalysisPermissionsRequestRequestTypeDef,
-    _OptionalUpdateAnalysisPermissionsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateDashboardPermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDashboardPermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "DashboardId": str,
-    },
-)
-_OptionalUpdateDashboardPermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDashboardPermissionsRequestRequestTypeDef",
-    {
-        "GrantPermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-        "RevokePermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-        "GrantLinkPermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-        "RevokeLinkPermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-class UpdateDashboardPermissionsRequestRequestTypeDef(
-    _RequiredUpdateDashboardPermissionsRequestRequestTypeDef,
-    _OptionalUpdateDashboardPermissionsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateDataSetPermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDataSetPermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "DataSetId": str,
-    },
-)
-_OptionalUpdateDataSetPermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDataSetPermissionsRequestRequestTypeDef",
-    {
-        "GrantPermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-        "RevokePermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-class UpdateDataSetPermissionsRequestRequestTypeDef(
-    _RequiredUpdateDataSetPermissionsRequestRequestTypeDef,
-    _OptionalUpdateDataSetPermissionsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateDataSourcePermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDataSourcePermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "DataSourceId": str,
-    },
-)
-_OptionalUpdateDataSourcePermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDataSourcePermissionsRequestRequestTypeDef",
-    {
-        "GrantPermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-        "RevokePermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-class UpdateDataSourcePermissionsRequestRequestTypeDef(
-    _RequiredUpdateDataSourcePermissionsRequestRequestTypeDef,
-    _OptionalUpdateDataSourcePermissionsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateFolderPermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFolderPermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "FolderId": str,
-    },
-)
-_OptionalUpdateFolderPermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFolderPermissionsRequestRequestTypeDef",
-    {
-        "GrantPermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-        "RevokePermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-class UpdateFolderPermissionsRequestRequestTypeDef(
-    _RequiredUpdateFolderPermissionsRequestRequestTypeDef,
-    _OptionalUpdateFolderPermissionsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateTemplatePermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateTemplatePermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "TemplateId": str,
-    },
-)
-_OptionalUpdateTemplatePermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateTemplatePermissionsRequestRequestTypeDef",
-    {
-        "GrantPermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-        "RevokePermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-class UpdateTemplatePermissionsRequestRequestTypeDef(
-    _RequiredUpdateTemplatePermissionsRequestRequestTypeDef,
-    _OptionalUpdateTemplatePermissionsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateThemePermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateThemePermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "ThemeId": str,
-    },
-)
-_OptionalUpdateThemePermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateThemePermissionsRequestRequestTypeDef",
-    {
-        "GrantPermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-        "RevokePermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-class UpdateThemePermissionsRequestRequestTypeDef(
-    _RequiredUpdateThemePermissionsRequestRequestTypeDef,
-    _OptionalUpdateThemePermissionsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateTopicPermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateTopicPermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "TopicId": str,
-    },
-)
-_OptionalUpdateTopicPermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateTopicPermissionsRequestRequestTypeDef",
-    {
-        "GrantPermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-        "RevokePermissions": Sequence[
-            Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-class UpdateTopicPermissionsRequestRequestTypeDef(
-    _RequiredUpdateTopicPermissionsRequestRequestTypeDef,
-    _OptionalUpdateTopicPermissionsRequestRequestTypeDef,
-):
-    pass
-
 DataSetSummaryTypeDef = TypedDict(
     "DataSetSummaryTypeDef",
     {
         "Arn": str,
         "DataSetId": str,
         "Name": str,
         "CreatedTime": datetime,
@@ -8806,47 +8430,14 @@
         "ThemeAlias": ThemeAliasTypeDef,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateTopicRefreshScheduleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTopicRefreshScheduleRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "TopicId": str,
-        "DatasetArn": str,
-        "RefreshSchedule": TopicRefreshScheduleTypeDef,
-    },
-)
-_OptionalCreateTopicRefreshScheduleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTopicRefreshScheduleRequestRequestTypeDef",
-    {
-        "DatasetName": str,
-    },
-    total=False,
-)
-
-class CreateTopicRefreshScheduleRequestRequestTypeDef(
-    _RequiredCreateTopicRefreshScheduleRequestRequestTypeDef,
-    _OptionalCreateTopicRefreshScheduleRequestRequestTypeDef,
-):
-    pass
-
-UpdateTopicRefreshScheduleRequestRequestTypeDef = TypedDict(
-    "UpdateTopicRefreshScheduleRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "TopicId": str,
-        "DatasetId": str,
-        "RefreshSchedule": TopicRefreshScheduleTypeDef,
-    },
-)
-
 CustomActionNavigationOperationTypeDef = TypedDict(
     "CustomActionNavigationOperationTypeDef",
     {
         "LocalNavigationConfiguration": LocalNavigationConfigurationTypeDef,
     },
     total=False,
 )
@@ -8866,33 +8457,14 @@
 )
 
 class CustomValuesConfigurationOutputTypeDef(
     _RequiredCustomValuesConfigurationOutputTypeDef, _OptionalCustomValuesConfigurationOutputTypeDef
 ):
     pass
 
-_RequiredCustomValuesConfigurationTypeDef = TypedDict(
-    "_RequiredCustomValuesConfigurationTypeDef",
-    {
-        "CustomValues": CustomParameterValuesTypeDef,
-    },
-)
-_OptionalCustomValuesConfigurationTypeDef = TypedDict(
-    "_OptionalCustomValuesConfigurationTypeDef",
-    {
-        "IncludeNullValue": bool,
-    },
-    total=False,
-)
-
-class CustomValuesConfigurationTypeDef(
-    _RequiredCustomValuesConfigurationTypeDef, _OptionalCustomValuesConfigurationTypeDef
-):
-    pass
-
 _RequiredCustomSqlOutputTypeDef = TypedDict(
     "_RequiredCustomSqlOutputTypeDef",
     {
         "DataSourceArn": str,
         "Name": str,
         "SqlQuery": str,
     },
@@ -9212,50 +8784,28 @@
 )
 
 class DateTimeDatasetParameterOutputTypeDef(
     _RequiredDateTimeDatasetParameterOutputTypeDef, _OptionalDateTimeDatasetParameterOutputTypeDef
 ):
     pass
 
-_RequiredDateTimeDatasetParameterTypeDef = TypedDict(
-    "_RequiredDateTimeDatasetParameterTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "ValueType": DatasetParameterValueTypeType,
-    },
-)
-_OptionalDateTimeDatasetParameterTypeDef = TypedDict(
-    "_OptionalDateTimeDatasetParameterTypeDef",
-    {
-        "TimeGranularity": TimeGranularityType,
-        "DefaultValues": DateTimeDatasetParameterDefaultValuesTypeDef,
-    },
-    total=False,
-)
-
-class DateTimeDatasetParameterTypeDef(
-    _RequiredDateTimeDatasetParameterTypeDef, _OptionalDateTimeDatasetParameterTypeDef
-):
-    pass
-
 TimeRangeFilterValueOutputTypeDef = TypedDict(
     "TimeRangeFilterValueOutputTypeDef",
     {
         "StaticValue": datetime,
         "RollingDate": RollingDateConfigurationTypeDef,
         "Parameter": str,
     },
     total=False,
 )
 
 TimeRangeFilterValueTypeDef = TypedDict(
     "TimeRangeFilterValueTypeDef",
     {
-        "StaticValue": Union[datetime, str],
+        "StaticValue": TimestampTypeDef,
         "RollingDate": RollingDateConfigurationTypeDef,
         "Parameter": str,
     },
     total=False,
 )
 
 _RequiredDecimalDatasetParameterOutputTypeDef = TypedDict(
@@ -9296,14 +8846,178 @@
 )
 
 class DecimalDatasetParameterTypeDef(
     _RequiredDecimalDatasetParameterTypeDef, _OptionalDecimalDatasetParameterTypeDef
 ):
     pass
 
+DescribeAnalysisPermissionsResponseTypeDef = TypedDict(
+    "DescribeAnalysisPermissionsResponseTypeDef",
+    {
+        "AnalysisId": str,
+        "AnalysisArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDataSetPermissionsResponseTypeDef = TypedDict(
+    "DescribeDataSetPermissionsResponseTypeDef",
+    {
+        "DataSetArn": str,
+        "DataSetId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDataSourcePermissionsResponseTypeDef = TypedDict(
+    "DescribeDataSourcePermissionsResponseTypeDef",
+    {
+        "DataSourceArn": str,
+        "DataSourceId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFolderPermissionsResponseTypeDef = TypedDict(
+    "DescribeFolderPermissionsResponseTypeDef",
+    {
+        "Status": int,
+        "FolderId": str,
+        "Arn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFolderResolvedPermissionsResponseTypeDef = TypedDict(
+    "DescribeFolderResolvedPermissionsResponseTypeDef",
+    {
+        "Status": int,
+        "FolderId": str,
+        "Arn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTemplatePermissionsResponseTypeDef = TypedDict(
+    "DescribeTemplatePermissionsResponseTypeDef",
+    {
+        "TemplateId": str,
+        "TemplateArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeThemePermissionsResponseTypeDef = TypedDict(
+    "DescribeThemePermissionsResponseTypeDef",
+    {
+        "ThemeId": str,
+        "ThemeArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTopicPermissionsResponseTypeDef = TypedDict(
+    "DescribeTopicPermissionsResponseTypeDef",
+    {
+        "TopicId": str,
+        "TopicArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LinkSharingConfigurationTypeDef = TypedDict(
+    "LinkSharingConfigurationTypeDef",
+    {
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+    },
+    total=False,
+)
+
+UpdateAnalysisPermissionsResponseTypeDef = TypedDict(
+    "UpdateAnalysisPermissionsResponseTypeDef",
+    {
+        "AnalysisArn": str,
+        "AnalysisId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFolderPermissionsResponseTypeDef = TypedDict(
+    "UpdateFolderPermissionsResponseTypeDef",
+    {
+        "Status": int,
+        "Arn": str,
+        "FolderId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTemplatePermissionsResponseTypeDef = TypedDict(
+    "UpdateTemplatePermissionsResponseTypeDef",
+    {
+        "TemplateId": str,
+        "TemplateArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateThemePermissionsResponseTypeDef = TypedDict(
+    "UpdateThemePermissionsResponseTypeDef",
+    {
+        "ThemeId": str,
+        "ThemeArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTopicPermissionsResponseTypeDef = TypedDict(
+    "UpdateTopicPermissionsResponseTypeDef",
+    {
+        "TopicId": str,
+        "TopicArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeFolderResponseTypeDef = TypedDict(
     "DescribeFolderResponseTypeDef",
     {
         "Status": int,
         "Folder": FolderTypeDef,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -9447,14 +9161,15 @@
 )
 
 class RelativeDatesFilterTypeDef(
     _RequiredRelativeDatesFilterTypeDef, _OptionalRelativeDatesFilterTypeDef
 ):
     pass
 
+FieldFolderUnionTypeDef = Union[FieldFolderTypeDef, FieldFolderOutputTypeDef]
 FilterOperationTargetVisualsConfigurationOutputTypeDef = TypedDict(
     "FilterOperationTargetVisualsConfigurationOutputTypeDef",
     {
         "SameSheetTargetVisualConfiguration": SameSheetTargetVisualConfigurationOutputTypeDef,
     },
     total=False,
 )
@@ -9543,23 +9258,14 @@
     {
         "WhatIfPointScenario": WhatIfPointScenarioOutputTypeDef,
         "WhatIfRangeScenario": WhatIfRangeScenarioOutputTypeDef,
     },
     total=False,
 )
 
-ForecastScenarioTypeDef = TypedDict(
-    "ForecastScenarioTypeDef",
-    {
-        "WhatIfPointScenario": WhatIfPointScenarioTypeDef,
-        "WhatIfRangeScenario": WhatIfRangeScenarioTypeDef,
-    },
-    total=False,
-)
-
 FreeFormLayoutCanvasSizeOptionsTypeDef = TypedDict(
     "FreeFormLayoutCanvasSizeOptionsTypeDef",
     {
         "ScreenCanvasSizeOptions": FreeFormLayoutScreenCanvasSizeOptionsTypeDef,
     },
     total=False,
 )
@@ -10497,35 +10203,14 @@
 
 class OverrideDatasetParameterOperationOutputTypeDef(
     _RequiredOverrideDatasetParameterOperationOutputTypeDef,
     _OptionalOverrideDatasetParameterOperationOutputTypeDef,
 ):
     pass
 
-_RequiredOverrideDatasetParameterOperationTypeDef = TypedDict(
-    "_RequiredOverrideDatasetParameterOperationTypeDef",
-    {
-        "ParameterName": str,
-    },
-)
-_OptionalOverrideDatasetParameterOperationTypeDef = TypedDict(
-    "_OptionalOverrideDatasetParameterOperationTypeDef",
-    {
-        "NewParameterName": str,
-        "NewDefaultValues": NewDefaultValuesTypeDef,
-    },
-    total=False,
-)
-
-class OverrideDatasetParameterOperationTypeDef(
-    _RequiredOverrideDatasetParameterOperationTypeDef,
-    _OptionalOverrideDatasetParameterOperationTypeDef,
-):
-    pass
-
 NumericSeparatorConfigurationTypeDef = TypedDict(
     "NumericSeparatorConfigurationTypeDef",
     {
         "DecimalSeparator": NumericSeparatorSymbolType,
         "ThousandsSeparator": ThousandSeparatorOptionsTypeDef,
     },
     total=False,
@@ -10547,25 +10232,14 @@
         "IntegerParameters": List[IntegerParameterOutputTypeDef],
         "DecimalParameters": List[DecimalParameterOutputTypeDef],
         "DateTimeParameters": List[DateTimeParameterOutputTypeDef],
     },
     total=False,
 )
 
-ParametersTypeDef = TypedDict(
-    "ParametersTypeDef",
-    {
-        "StringParameters": Sequence[StringParameterTypeDef],
-        "IntegerParameters": Sequence[IntegerParameterTypeDef],
-        "DecimalParameters": Sequence[DecimalParameterTypeDef],
-        "DateTimeParameters": Sequence[DateTimeParameterTypeDef],
-    },
-    total=False,
-)
-
 VisibleRangeOptionsTypeDef = TypedDict(
     "VisibleRangeOptionsTypeDef",
     {
         "PercentRange": PercentVisibleRangeTypeDef,
     },
     total=False,
 )
@@ -10619,14 +10293,15 @@
     {
         "StatePersistence": StatePersistenceConfigurationsTypeDef,
         "Bookmarks": BookmarksConfigurationsTypeDef,
     },
     total=False,
 )
 
+ResourcePermissionUnionTypeDef = Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]
 _RequiredRowLevelPermissionTagConfigurationOutputTypeDef = TypedDict(
     "_RequiredRowLevelPermissionTagConfigurationOutputTypeDef",
     {
         "TagRules": List[RowLevelPermissionTagRuleTypeDef],
     },
 )
 _OptionalRowLevelPermissionTagConfigurationOutputTypeDef = TypedDict(
@@ -10888,15 +10563,15 @@
     total=False,
 )
 
 DateTimeDefaultValuesTypeDef = TypedDict(
     "DateTimeDefaultValuesTypeDef",
     {
         "DynamicValue": DynamicDefaultValueTypeDef,
-        "StaticValues": Sequence[Union[datetime, str]],
+        "StaticValues": Sequence[TimestampTypeDef],
         "RollingDate": RollingDateConfigurationTypeDef,
     },
     total=False,
 )
 
 DecimalDefaultValuesOutputTypeDef = TypedDict(
     "DecimalDefaultValuesOutputTypeDef",
@@ -10958,24 +10633,14 @@
         "NumericEqualityFilter": NumericEqualityDrillDownFilterTypeDef,
         "CategoryFilter": CategoryDrillDownFilterOutputTypeDef,
         "TimeRangeFilter": TimeRangeDrillDownFilterOutputTypeDef,
     },
     total=False,
 )
 
-DrillDownFilterTypeDef = TypedDict(
-    "DrillDownFilterTypeDef",
-    {
-        "NumericEqualityFilter": NumericEqualityDrillDownFilterTypeDef,
-        "CategoryFilter": CategoryDrillDownFilterTypeDef,
-        "TimeRangeFilter": TimeRangeDrillDownFilterTypeDef,
-    },
-    total=False,
-)
-
 AnalysisTypeDef = TypedDict(
     "AnalysisTypeDef",
     {
         "AnalysisId": str,
         "Arn": str,
         "Name": str,
         "Status": ResourceStatusType,
@@ -11059,14 +10724,18 @@
         ),
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AssetBundleCloudFormationOverridePropertyConfigurationUnionTypeDef = Union[
+    AssetBundleCloudFormationOverridePropertyConfigurationTypeDef,
+    AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef,
+]
 _RequiredStartAssetBundleExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartAssetBundleExportJobRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AssetBundleExportJobId": str,
         "ResourceArns": Sequence[str],
         "ExportFormat": AssetBundleExportFormatType,
@@ -11085,14 +10754,142 @@
 
 class StartAssetBundleExportJobRequestRequestTypeDef(
     _RequiredStartAssetBundleExportJobRequestRequestTypeDef,
     _OptionalStartAssetBundleExportJobRequestRequestTypeDef,
 ):
     pass
 
+_RequiredCustomValuesConfigurationTypeDef = TypedDict(
+    "_RequiredCustomValuesConfigurationTypeDef",
+    {
+        "CustomValues": CustomParameterValuesTypeDef,
+    },
+)
+_OptionalCustomValuesConfigurationTypeDef = TypedDict(
+    "_OptionalCustomValuesConfigurationTypeDef",
+    {
+        "IncludeNullValue": bool,
+    },
+    total=False,
+)
+
+class CustomValuesConfigurationTypeDef(
+    _RequiredCustomValuesConfigurationTypeDef, _OptionalCustomValuesConfigurationTypeDef
+):
+    pass
+
+_RequiredDateTimeDatasetParameterTypeDef = TypedDict(
+    "_RequiredDateTimeDatasetParameterTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "ValueType": DatasetParameterValueTypeType,
+    },
+)
+_OptionalDateTimeDatasetParameterTypeDef = TypedDict(
+    "_OptionalDateTimeDatasetParameterTypeDef",
+    {
+        "TimeGranularity": TimeGranularityType,
+        "DefaultValues": DateTimeDatasetParameterDefaultValuesTypeDef,
+    },
+    total=False,
+)
+
+class DateTimeDatasetParameterTypeDef(
+    _RequiredDateTimeDatasetParameterTypeDef, _OptionalDateTimeDatasetParameterTypeDef
+):
+    pass
+
+ParametersTypeDef = TypedDict(
+    "ParametersTypeDef",
+    {
+        "StringParameters": Sequence[StringParameterTypeDef],
+        "IntegerParameters": Sequence[IntegerParameterTypeDef],
+        "DecimalParameters": Sequence[DecimalParameterTypeDef],
+        "DateTimeParameters": Sequence[DateTimeParameterTypeDef],
+    },
+    total=False,
+)
+
+_RequiredOverrideDatasetParameterOperationTypeDef = TypedDict(
+    "_RequiredOverrideDatasetParameterOperationTypeDef",
+    {
+        "ParameterName": str,
+    },
+)
+_OptionalOverrideDatasetParameterOperationTypeDef = TypedDict(
+    "_OptionalOverrideDatasetParameterOperationTypeDef",
+    {
+        "NewParameterName": str,
+        "NewDefaultValues": NewDefaultValuesTypeDef,
+    },
+    total=False,
+)
+
+class OverrideDatasetParameterOperationTypeDef(
+    _RequiredOverrideDatasetParameterOperationTypeDef,
+    _OptionalOverrideDatasetParameterOperationTypeDef,
+):
+    pass
+
+DrillDownFilterTypeDef = TypedDict(
+    "DrillDownFilterTypeDef",
+    {
+        "NumericEqualityFilter": NumericEqualityDrillDownFilterTypeDef,
+        "CategoryFilter": CategoryDrillDownFilterTypeDef,
+        "TimeRangeFilter": TimeRangeDrillDownFilterTypeDef,
+    },
+    total=False,
+)
+
+_RequiredCreateTopicRefreshScheduleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTopicRefreshScheduleRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "TopicId": str,
+        "DatasetArn": str,
+        "RefreshSchedule": TopicRefreshScheduleTypeDef,
+    },
+)
+_OptionalCreateTopicRefreshScheduleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTopicRefreshScheduleRequestRequestTypeDef",
+    {
+        "DatasetName": str,
+    },
+    total=False,
+)
+
+class CreateTopicRefreshScheduleRequestRequestTypeDef(
+    _RequiredCreateTopicRefreshScheduleRequestRequestTypeDef,
+    _OptionalCreateTopicRefreshScheduleRequestRequestTypeDef,
+):
+    pass
+
+TopicRefreshScheduleUnionTypeDef = Union[
+    TopicRefreshScheduleTypeDef, TopicRefreshScheduleOutputTypeDef
+]
+UpdateTopicRefreshScheduleRequestRequestTypeDef = TypedDict(
+    "UpdateTopicRefreshScheduleRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "TopicId": str,
+        "DatasetId": str,
+        "RefreshSchedule": TopicRefreshScheduleTypeDef,
+    },
+)
+
+ForecastScenarioTypeDef = TypedDict(
+    "ForecastScenarioTypeDef",
+    {
+        "WhatIfPointScenario": WhatIfPointScenarioTypeDef,
+        "WhatIfRangeScenario": WhatIfRangeScenarioTypeDef,
+    },
+    total=False,
+)
+
 NumericAxisOptionsOutputTypeDef = TypedDict(
     "NumericAxisOptionsOutputTypeDef",
     {
         "Scale": AxisScaleTypeDef,
         "Range": AxisDisplayRangeOutputTypeDef,
     },
     total=False,
@@ -11167,14 +10964,15 @@
     "TagColumnOperationTypeDef",
     {
         "ColumnName": str,
         "Tags": Sequence[ColumnTagTypeDef],
     },
 )
 
+ColumnGroupUnionTypeDef = Union[ColumnGroupTypeDef, ColumnGroupOutputTypeDef]
 DataSetConfigurationOutputTypeDef = TypedDict(
     "DataSetConfigurationOutputTypeDef",
     {
         "Placeholder": str,
         "DataSetSchema": DataSetSchemaOutputTypeDef,
         "ColumnGroupSchemaList": List[ColumnGroupSchemaOutputTypeDef],
     },
@@ -11196,40 +10994,14 @@
     {
         "IconSet": ConditionalFormattingIconSetTypeDef,
         "CustomCondition": ConditionalFormattingCustomIconConditionTypeDef,
     },
     total=False,
 )
 
-DescribeDashboardPermissionsResponseTypeDef = TypedDict(
-    "DescribeDashboardPermissionsResponseTypeDef",
-    {
-        "DashboardId": str,
-        "DashboardArn": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "LinkSharingConfiguration": LinkSharingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateDashboardPermissionsResponseTypeDef = TypedDict(
-    "UpdateDashboardPermissionsResponseTypeDef",
-    {
-        "DashboardArn": str,
-        "DashboardId": str,
-        "Permissions": List[ResourcePermissionOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "LinkSharingConfiguration": LinkSharingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListDataSetsResponseTypeDef = TypedDict(
     "ListDataSetsResponseTypeDef",
     {
         "DataSetSummaries": List[DataSetSummaryTypeDef],
         "NextToken": str,
         "RequestId": str,
         "Status": int,
@@ -11256,26 +11028,14 @@
         "SourceParameterName": str,
         "SourceField": str,
         "SourceColumn": ColumnIdentifierTypeDef,
     },
     total=False,
 )
 
-DestinationParameterValueConfigurationTypeDef = TypedDict(
-    "DestinationParameterValueConfigurationTypeDef",
-    {
-        "CustomValuesConfiguration": CustomValuesConfigurationTypeDef,
-        "SelectAllValueOptions": Literal["ALL_VALUES"],
-        "SourceParameterName": str,
-        "SourceField": str,
-        "SourceColumn": ColumnIdentifierTypeDef,
-    },
-    total=False,
-)
-
 DashboardPublishOptionsTypeDef = TypedDict(
     "DashboardPublishOptionsTypeDef",
     {
         "AdHocFilteringOption": AdHocFilteringOptionTypeDef,
         "ExportToCSVOption": ExportToCSVOptionTypeDef,
         "SheetControlsOption": SheetControlsOptionTypeDef,
         "VisualPublishOptions": DashboardVisualPublishOptionsTypeDef,
@@ -11394,14 +11154,40 @@
     },
     total=False,
 )
 
 class TimeRangeFilterTypeDef(_RequiredTimeRangeFilterTypeDef, _OptionalTimeRangeFilterTypeDef):
     pass
 
+DescribeDashboardPermissionsResponseTypeDef = TypedDict(
+    "DescribeDashboardPermissionsResponseTypeDef",
+    {
+        "DashboardId": str,
+        "DashboardArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "LinkSharingConfiguration": LinkSharingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDashboardPermissionsResponseTypeDef = TypedDict(
+    "UpdateDashboardPermissionsResponseTypeDef",
+    {
+        "DashboardArn": str,
+        "DashboardId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "LinkSharingConfiguration": LinkSharingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTopicRefreshSchedulesResponseTypeDef = TypedDict(
     "ListTopicRefreshSchedulesResponseTypeDef",
     {
         "TopicId": str,
         "TopicArn": str,
         "RefreshSchedules": List[TopicRefreshScheduleSummaryTypeDef],
         "Status": int,
@@ -11537,23 +11323,14 @@
     {
         "ForecastProperties": TimeBasedForecastPropertiesTypeDef,
         "Scenario": ForecastScenarioOutputTypeDef,
     },
     total=False,
 )
 
-ForecastConfigurationTypeDef = TypedDict(
-    "ForecastConfigurationTypeDef",
-    {
-        "ForecastProperties": TimeBasedForecastPropertiesTypeDef,
-        "Scenario": ForecastScenarioTypeDef,
-    },
-    total=False,
-)
-
 DefaultFreeFormLayoutConfigurationTypeDef = TypedDict(
     "DefaultFreeFormLayoutConfigurationTypeDef",
     {
         "CanvasSizeOptions": FreeFormLayoutCanvasSizeOptionsTypeDef,
     },
 )
 
@@ -11961,15 +11738,15 @@
         "ScheduleFrequency": RefreshFrequencyTypeDef,
         "RefreshType": IngestionTypeType,
     },
 )
 _OptionalRefreshScheduleTypeDef = TypedDict(
     "_OptionalRefreshScheduleTypeDef",
     {
-        "StartAfterDateTime": Union[datetime, str],
+        "StartAfterDateTime": TimestampTypeDef,
         "Arn": str,
     },
     total=False,
 )
 
 class RefreshScheduleTypeDef(_RequiredRefreshScheduleTypeDef, _OptionalRefreshScheduleTypeDef):
     pass
@@ -11999,14 +11776,219 @@
 
 class RegisteredUserDashboardEmbeddingConfigurationTypeDef(
     _RequiredRegisteredUserDashboardEmbeddingConfigurationTypeDef,
     _OptionalRegisteredUserDashboardEmbeddingConfigurationTypeDef,
 ):
     pass
 
+_RequiredCreateFolderRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFolderRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "FolderId": str,
+    },
+)
+_OptionalCreateFolderRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFolderRequestRequestTypeDef",
+    {
+        "Name": str,
+        "FolderType": Literal["SHARED"],
+        "ParentFolderArn": str,
+        "Permissions": Sequence[ResourcePermissionUnionTypeDef],
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateFolderRequestRequestTypeDef(
+    _RequiredCreateFolderRequestRequestTypeDef, _OptionalCreateFolderRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateAnalysisPermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAnalysisPermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "AnalysisId": str,
+    },
+)
+_OptionalUpdateAnalysisPermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAnalysisPermissionsRequestRequestTypeDef",
+    {
+        "GrantPermissions": Sequence[ResourcePermissionUnionTypeDef],
+        "RevokePermissions": Sequence[ResourcePermissionUnionTypeDef],
+    },
+    total=False,
+)
+
+class UpdateAnalysisPermissionsRequestRequestTypeDef(
+    _RequiredUpdateAnalysisPermissionsRequestRequestTypeDef,
+    _OptionalUpdateAnalysisPermissionsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateDashboardPermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDashboardPermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "DashboardId": str,
+    },
+)
+_OptionalUpdateDashboardPermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDashboardPermissionsRequestRequestTypeDef",
+    {
+        "GrantPermissions": Sequence[ResourcePermissionUnionTypeDef],
+        "RevokePermissions": Sequence[ResourcePermissionUnionTypeDef],
+        "GrantLinkPermissions": Sequence[ResourcePermissionUnionTypeDef],
+        "RevokeLinkPermissions": Sequence[ResourcePermissionUnionTypeDef],
+    },
+    total=False,
+)
+
+class UpdateDashboardPermissionsRequestRequestTypeDef(
+    _RequiredUpdateDashboardPermissionsRequestRequestTypeDef,
+    _OptionalUpdateDashboardPermissionsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateDataSetPermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDataSetPermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "DataSetId": str,
+    },
+)
+_OptionalUpdateDataSetPermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDataSetPermissionsRequestRequestTypeDef",
+    {
+        "GrantPermissions": Sequence[ResourcePermissionUnionTypeDef],
+        "RevokePermissions": Sequence[ResourcePermissionUnionTypeDef],
+    },
+    total=False,
+)
+
+class UpdateDataSetPermissionsRequestRequestTypeDef(
+    _RequiredUpdateDataSetPermissionsRequestRequestTypeDef,
+    _OptionalUpdateDataSetPermissionsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateDataSourcePermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDataSourcePermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "DataSourceId": str,
+    },
+)
+_OptionalUpdateDataSourcePermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDataSourcePermissionsRequestRequestTypeDef",
+    {
+        "GrantPermissions": Sequence[ResourcePermissionUnionTypeDef],
+        "RevokePermissions": Sequence[ResourcePermissionUnionTypeDef],
+    },
+    total=False,
+)
+
+class UpdateDataSourcePermissionsRequestRequestTypeDef(
+    _RequiredUpdateDataSourcePermissionsRequestRequestTypeDef,
+    _OptionalUpdateDataSourcePermissionsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateFolderPermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFolderPermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "FolderId": str,
+    },
+)
+_OptionalUpdateFolderPermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFolderPermissionsRequestRequestTypeDef",
+    {
+        "GrantPermissions": Sequence[ResourcePermissionUnionTypeDef],
+        "RevokePermissions": Sequence[ResourcePermissionUnionTypeDef],
+    },
+    total=False,
+)
+
+class UpdateFolderPermissionsRequestRequestTypeDef(
+    _RequiredUpdateFolderPermissionsRequestRequestTypeDef,
+    _OptionalUpdateFolderPermissionsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateTemplatePermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateTemplatePermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "TemplateId": str,
+    },
+)
+_OptionalUpdateTemplatePermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateTemplatePermissionsRequestRequestTypeDef",
+    {
+        "GrantPermissions": Sequence[ResourcePermissionUnionTypeDef],
+        "RevokePermissions": Sequence[ResourcePermissionUnionTypeDef],
+    },
+    total=False,
+)
+
+class UpdateTemplatePermissionsRequestRequestTypeDef(
+    _RequiredUpdateTemplatePermissionsRequestRequestTypeDef,
+    _OptionalUpdateTemplatePermissionsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateThemePermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateThemePermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "ThemeId": str,
+    },
+)
+_OptionalUpdateThemePermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateThemePermissionsRequestRequestTypeDef",
+    {
+        "GrantPermissions": Sequence[ResourcePermissionUnionTypeDef],
+        "RevokePermissions": Sequence[ResourcePermissionUnionTypeDef],
+    },
+    total=False,
+)
+
+class UpdateThemePermissionsRequestRequestTypeDef(
+    _RequiredUpdateThemePermissionsRequestRequestTypeDef,
+    _OptionalUpdateThemePermissionsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateTopicPermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateTopicPermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "TopicId": str,
+    },
+)
+_OptionalUpdateTopicPermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateTopicPermissionsRequestRequestTypeDef",
+    {
+        "GrantPermissions": Sequence[ResourcePermissionUnionTypeDef],
+        "RevokePermissions": Sequence[ResourcePermissionUnionTypeDef],
+    },
+    total=False,
+)
+
+class UpdateTopicPermissionsRequestRequestTypeDef(
+    _RequiredUpdateTopicPermissionsRequestRequestTypeDef,
+    _OptionalUpdateTopicPermissionsRequestRequestTypeDef,
+):
+    pass
+
+RowLevelPermissionTagConfigurationUnionTypeDef = Union[
+    RowLevelPermissionTagConfigurationTypeDef, RowLevelPermissionTagConfigurationOutputTypeDef
+]
 SnapshotDestinationConfigurationOutputTypeDef = TypedDict(
     "SnapshotDestinationConfigurationOutputTypeDef",
     {
         "S3Destinations": List[SnapshotS3DestinationConfigurationTypeDef],
     },
     total=False,
 )
@@ -12154,25 +12136,14 @@
         "DecimalDatasetParameter": DecimalDatasetParameterOutputTypeDef,
         "IntegerDatasetParameter": IntegerDatasetParameterOutputTypeDef,
         "DateTimeDatasetParameter": DateTimeDatasetParameterOutputTypeDef,
     },
     total=False,
 )
 
-DatasetParameterTypeDef = TypedDict(
-    "DatasetParameterTypeDef",
-    {
-        "StringDatasetParameter": StringDatasetParameterTypeDef,
-        "DecimalDatasetParameter": DecimalDatasetParameterTypeDef,
-        "IntegerDatasetParameter": IntegerDatasetParameterTypeDef,
-        "DateTimeDatasetParameter": DateTimeDatasetParameterTypeDef,
-    },
-    total=False,
-)
-
 _RequiredDateTimeParameterDeclarationOutputTypeDef = TypedDict(
     "_RequiredDateTimeParameterDeclarationOutputTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDateTimeParameterDeclarationOutputTypeDef = TypedDict(
@@ -12404,14 +12375,87 @@
 )
 
 class PredefinedHierarchyOutputTypeDef(
     _RequiredPredefinedHierarchyOutputTypeDef, _OptionalPredefinedHierarchyOutputTypeDef
 ):
     pass
 
+DescribeAnalysisResponseTypeDef = TypedDict(
+    "DescribeAnalysisResponseTypeDef",
+    {
+        "Analysis": AnalysisTypeDef,
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DashboardTypeDef = TypedDict(
+    "DashboardTypeDef",
+    {
+        "DashboardId": str,
+        "Arn": str,
+        "Name": str,
+        "Version": DashboardVersionTypeDef,
+        "CreatedTime": datetime,
+        "LastPublishedTime": datetime,
+        "LastUpdatedTime": datetime,
+    },
+    total=False,
+)
+
+_RequiredGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef = TypedDict(
+    "_RequiredGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "Namespace": str,
+        "AuthorizedResourceArns": Sequence[str],
+        "ExperienceConfiguration": AnonymousUserEmbeddingExperienceConfigurationTypeDef,
+    },
+)
+_OptionalGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef = TypedDict(
+    "_OptionalGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef",
+    {
+        "SessionLifetimeInMinutes": int,
+        "SessionTags": Sequence[SessionTagTypeDef],
+        "AllowedDomains": Sequence[str],
+    },
+    total=False,
+)
+
+class GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef(
+    _RequiredGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef,
+    _OptionalGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef,
+):
+    pass
+
+DestinationParameterValueConfigurationTypeDef = TypedDict(
+    "DestinationParameterValueConfigurationTypeDef",
+    {
+        "CustomValuesConfiguration": CustomValuesConfigurationTypeDef,
+        "SelectAllValueOptions": Literal["ALL_VALUES"],
+        "SourceParameterName": str,
+        "SourceField": str,
+        "SourceColumn": ColumnIdentifierTypeDef,
+    },
+    total=False,
+)
+
+DatasetParameterTypeDef = TypedDict(
+    "DatasetParameterTypeDef",
+    {
+        "StringDatasetParameter": StringDatasetParameterTypeDef,
+        "DecimalDatasetParameter": DecimalDatasetParameterTypeDef,
+        "IntegerDatasetParameter": IntegerDatasetParameterTypeDef,
+        "DateTimeDatasetParameter": DateTimeDatasetParameterTypeDef,
+    },
+    total=False,
+)
+
+ParametersUnionTypeDef = Union[ParametersTypeDef, ParametersOutputTypeDef]
 _RequiredDateTimeHierarchyTypeDef = TypedDict(
     "_RequiredDateTimeHierarchyTypeDef",
     {
         "HierarchyId": str,
     },
 )
 _OptionalDateTimeHierarchyTypeDef = TypedDict(
@@ -12463,63 +12507,23 @@
 )
 
 class PredefinedHierarchyTypeDef(
     _RequiredPredefinedHierarchyTypeDef, _OptionalPredefinedHierarchyTypeDef
 ):
     pass
 
-DescribeAnalysisResponseTypeDef = TypedDict(
-    "DescribeAnalysisResponseTypeDef",
-    {
-        "Analysis": AnalysisTypeDef,
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DashboardTypeDef = TypedDict(
-    "DashboardTypeDef",
-    {
-        "DashboardId": str,
-        "Arn": str,
-        "Name": str,
-        "Version": DashboardVersionTypeDef,
-        "CreatedTime": datetime,
-        "LastPublishedTime": datetime,
-        "LastUpdatedTime": datetime,
-    },
-    total=False,
-)
-
-_RequiredGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef = TypedDict(
-    "_RequiredGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "Namespace": str,
-        "AuthorizedResourceArns": Sequence[str],
-        "ExperienceConfiguration": AnonymousUserEmbeddingExperienceConfigurationTypeDef,
-    },
-)
-_OptionalGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef = TypedDict(
-    "_OptionalGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef",
+ForecastConfigurationTypeDef = TypedDict(
+    "ForecastConfigurationTypeDef",
     {
-        "SessionLifetimeInMinutes": int,
-        "SessionTags": Sequence[SessionTagTypeDef],
-        "AllowedDomains": Sequence[str],
+        "ForecastProperties": TimeBasedForecastPropertiesTypeDef,
+        "Scenario": ForecastScenarioTypeDef,
     },
     total=False,
 )
 
-class GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef(
-    _RequiredGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef,
-    _OptionalGenerateEmbedUrlForAnonymousUserRequestRequestTypeDef,
-):
-    pass
-
 AxisDataOptionsOutputTypeDef = TypedDict(
     "AxisDataOptionsOutputTypeDef",
     {
         "NumericAxisOptions": NumericAxisOptionsOutputTypeDef,
         "DateAxisOptions": DateAxisOptionsTypeDef,
     },
     total=False,
@@ -12584,22 +12588,14 @@
     "SetParameterValueConfigurationOutputTypeDef",
     {
         "DestinationParameterName": str,
         "Value": DestinationParameterValueConfigurationOutputTypeDef,
     },
 )
 
-SetParameterValueConfigurationTypeDef = TypedDict(
-    "SetParameterValueConfigurationTypeDef",
-    {
-        "DestinationParameterName": str,
-        "Value": DestinationParameterValueConfigurationTypeDef,
-    },
-)
-
 PivotTableFieldOptionsOutputTypeDef = TypedDict(
     "PivotTableFieldOptionsOutputTypeDef",
     {
         "SelectedFieldOptions": List[PivotTableFieldOptionTypeDef],
         "DataPathOptions": List[PivotTableDataPathOptionOutputTypeDef],
         "CollapseStateOptions": List[PivotTableFieldCollapseStateOptionOutputTypeDef],
     },
@@ -13290,14 +13286,15 @@
     {
         "DataSetId": str,
         "AwsAccountId": str,
         "Schedule": RefreshScheduleTypeDef,
     },
 )
 
+RefreshScheduleUnionTypeDef = Union[RefreshScheduleTypeDef, RefreshScheduleOutputTypeDef]
 UpdateRefreshScheduleRequestRequestTypeDef = TypedDict(
     "UpdateRefreshScheduleRequestRequestTypeDef",
     {
         "DataSetId": str,
         "AwsAccountId": str,
         "Schedule": RefreshScheduleTypeDef,
     },
@@ -13319,14 +13316,15 @@
     {
         "Files": List[SnapshotFileOutputTypeDef],
         "S3Results": List[SnapshotJobS3ResultTypeDef],
     },
     total=False,
 )
 
+PhysicalTableUnionTypeDef = Union[PhysicalTableTypeDef, PhysicalTableOutputTypeDef]
 DefaultSectionBasedLayoutConfigurationTypeDef = TypedDict(
     "DefaultSectionBasedLayoutConfigurationTypeDef",
     {
         "CanvasSizeOptions": SectionBasedLayoutCanvasSizeOptionsTypeDef,
     },
 )
 
@@ -13451,34 +13449,43 @@
         "ExplicitHierarchy": ExplicitHierarchyOutputTypeDef,
         "DateTimeHierarchy": DateTimeHierarchyOutputTypeDef,
         "PredefinedHierarchy": PredefinedHierarchyOutputTypeDef,
     },
     total=False,
 )
 
-ColumnHierarchyTypeDef = TypedDict(
-    "ColumnHierarchyTypeDef",
-    {
-        "ExplicitHierarchy": ExplicitHierarchyTypeDef,
-        "DateTimeHierarchy": DateTimeHierarchyTypeDef,
-        "PredefinedHierarchy": PredefinedHierarchyTypeDef,
-    },
-    total=False,
-)
-
 DescribeDashboardResponseTypeDef = TypedDict(
     "DescribeDashboardResponseTypeDef",
     {
         "Dashboard": DashboardTypeDef,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SetParameterValueConfigurationTypeDef = TypedDict(
+    "SetParameterValueConfigurationTypeDef",
+    {
+        "DestinationParameterName": str,
+        "Value": DestinationParameterValueConfigurationTypeDef,
+    },
+)
+
+DatasetParameterUnionTypeDef = Union[DatasetParameterTypeDef, DatasetParameterOutputTypeDef]
+ColumnHierarchyTypeDef = TypedDict(
+    "ColumnHierarchyTypeDef",
+    {
+        "ExplicitHierarchy": ExplicitHierarchyTypeDef,
+        "DateTimeHierarchy": DateTimeHierarchyTypeDef,
+        "PredefinedHierarchy": PredefinedHierarchyTypeDef,
+    },
+    total=False,
+)
+
 _RequiredLogicalTableOutputTypeDef = TypedDict(
     "_RequiredLogicalTableOutputTypeDef",
     {
         "Alias": str,
         "Source": LogicalTableSourceTypeDef,
     },
 )
@@ -13529,21 +13536,14 @@
 CustomActionSetParametersOperationOutputTypeDef = TypedDict(
     "CustomActionSetParametersOperationOutputTypeDef",
     {
         "ParameterValueConfigurations": List[SetParameterValueConfigurationOutputTypeDef],
     },
 )
 
-CustomActionSetParametersOperationTypeDef = TypedDict(
-    "CustomActionSetParametersOperationTypeDef",
-    {
-        "ParameterValueConfigurations": Sequence[SetParameterValueConfigurationTypeDef],
-    },
-)
-
 AxisDisplayOptionsOutputTypeDef = TypedDict(
     "AxisDisplayOptionsOutputTypeDef",
     {
         "TickLabelOptions": AxisTickLabelOptionsTypeDef,
         "AxisLineVisibility": VisibilityType,
         "GridLineVisibility": VisibilityType,
         "DataOptions": AxisDataOptionsOutputTypeDef,
@@ -14332,25 +14332,26 @@
         "Configuration": ThemeConfigurationTypeDef,
     },
 )
 _OptionalCreateThemeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateThemeRequestRequestTypeDef",
     {
         "VersionDescription": str,
-        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
+        "Permissions": Sequence[ResourcePermissionUnionTypeDef],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 class CreateThemeRequestRequestTypeDef(
     _RequiredCreateThemeRequestRequestTypeDef, _OptionalCreateThemeRequestRequestTypeDef
 ):
     pass
 
+ThemeConfigurationUnionTypeDef = Union[ThemeConfigurationTypeDef, ThemeConfigurationOutputTypeDef]
 _RequiredUpdateThemeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateThemeRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "ThemeId": str,
         "BaseThemeId": str,
     },
@@ -14622,25 +14623,35 @@
         "LastUpdatedTime": datetime,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SnapshotConfigurationUnionTypeDef = Union[
+    SnapshotConfigurationTypeDef, SnapshotConfigurationOutputTypeDef
+]
 StartDashboardSnapshotJobRequestRequestTypeDef = TypedDict(
     "StartDashboardSnapshotJobRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "DashboardId": str,
         "SnapshotJobId": str,
         "UserConfiguration": SnapshotUserConfigurationTypeDef,
         "SnapshotConfiguration": SnapshotConfigurationTypeDef,
     },
 )
 
+CustomActionSetParametersOperationTypeDef = TypedDict(
+    "CustomActionSetParametersOperationTypeDef",
+    {
+        "ParameterValueConfigurations": Sequence[SetParameterValueConfigurationTypeDef],
+    },
+)
+
 DataSetTypeDef = TypedDict(
     "DataSetTypeDef",
     {
         "Arn": str,
         "DataSetId": str,
         "Name": str,
         "CreatedTime": datetime,
@@ -14657,84 +14668,15 @@
         "ColumnLevelPermissionRules": List[ColumnLevelPermissionRuleOutputTypeDef],
         "DataSetUsageConfiguration": DataSetUsageConfigurationTypeDef,
         "DatasetParameters": List[DatasetParameterOutputTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateDataSetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDataSetRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "DataSetId": str,
-        "Name": str,
-        "PhysicalTableMap": Mapping[str, Union[PhysicalTableTypeDef, PhysicalTableOutputTypeDef]],
-        "ImportMode": DataSetImportModeType,
-    },
-)
-_OptionalCreateDataSetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDataSetRequestRequestTypeDef",
-    {
-        "LogicalTableMap": Mapping[str, Union[LogicalTableTypeDef, LogicalTableOutputTypeDef]],
-        "ColumnGroups": Sequence[Union[ColumnGroupTypeDef, ColumnGroupOutputTypeDef]],
-        "FieldFolders": Mapping[str, Union[FieldFolderTypeDef, FieldFolderOutputTypeDef]],
-        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
-        "RowLevelPermissionDataSet": RowLevelPermissionDataSetTypeDef,
-        "RowLevelPermissionTagConfiguration": RowLevelPermissionTagConfigurationTypeDef,
-        "ColumnLevelPermissionRules": Sequence[
-            Union[ColumnLevelPermissionRuleTypeDef, ColumnLevelPermissionRuleOutputTypeDef]
-        ],
-        "Tags": Sequence[TagTypeDef],
-        "DataSetUsageConfiguration": DataSetUsageConfigurationTypeDef,
-        "DatasetParameters": Sequence[
-            Union[DatasetParameterTypeDef, DatasetParameterOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-class CreateDataSetRequestRequestTypeDef(
-    _RequiredCreateDataSetRequestRequestTypeDef, _OptionalCreateDataSetRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateDataSetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDataSetRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "DataSetId": str,
-        "Name": str,
-        "PhysicalTableMap": Mapping[str, Union[PhysicalTableTypeDef, PhysicalTableOutputTypeDef]],
-        "ImportMode": DataSetImportModeType,
-    },
-)
-_OptionalUpdateDataSetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDataSetRequestRequestTypeDef",
-    {
-        "LogicalTableMap": Mapping[str, Union[LogicalTableTypeDef, LogicalTableOutputTypeDef]],
-        "ColumnGroups": Sequence[Union[ColumnGroupTypeDef, ColumnGroupOutputTypeDef]],
-        "FieldFolders": Mapping[str, Union[FieldFolderTypeDef, FieldFolderOutputTypeDef]],
-        "RowLevelPermissionDataSet": RowLevelPermissionDataSetTypeDef,
-        "RowLevelPermissionTagConfiguration": RowLevelPermissionTagConfigurationTypeDef,
-        "ColumnLevelPermissionRules": Sequence[
-            Union[ColumnLevelPermissionRuleTypeDef, ColumnLevelPermissionRuleOutputTypeDef]
-        ],
-        "DataSetUsageConfiguration": DataSetUsageConfigurationTypeDef,
-        "DatasetParameters": Sequence[
-            Union[DatasetParameterTypeDef, DatasetParameterOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-class UpdateDataSetRequestRequestTypeDef(
-    _RequiredUpdateDataSetRequestRequestTypeDef, _OptionalUpdateDataSetRequestRequestTypeDef
-):
-    pass
-
+LogicalTableUnionTypeDef = Union[LogicalTableTypeDef, LogicalTableOutputTypeDef]
 DescribeTemplateResponseTypeDef = TypedDict(
     "DescribeTemplateResponseTypeDef",
     {
         "Template": TemplateTypeDef,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -14748,25 +14690,14 @@
         "NavigationOperation": CustomActionNavigationOperationTypeDef,
         "URLOperation": CustomActionURLOperationTypeDef,
         "SetParametersOperation": CustomActionSetParametersOperationOutputTypeDef,
     },
     total=False,
 )
 
-VisualCustomActionOperationTypeDef = TypedDict(
-    "VisualCustomActionOperationTypeDef",
-    {
-        "FilterOperation": CustomActionFilterOperationTypeDef,
-        "NavigationOperation": CustomActionNavigationOperationTypeDef,
-        "URLOperation": CustomActionURLOperationTypeDef,
-        "SetParametersOperation": CustomActionSetParametersOperationTypeDef,
-    },
-    total=False,
-)
-
 LineSeriesAxisDisplayOptionsOutputTypeDef = TypedDict(
     "LineSeriesAxisDisplayOptionsOutputTypeDef",
     {
         "AxisOptions": AxisDisplayOptionsOutputTypeDef,
         "MissingDataConfigurations": List[MissingDataConfigurationTypeDef],
     },
     total=False,
@@ -15040,14 +14971,18 @@
         "FailureAction": AssetBundleImportFailureActionType,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AssetBundleImportJobOverrideParametersUnionTypeDef = Union[
+    AssetBundleImportJobOverrideParametersTypeDef,
+    AssetBundleImportJobOverrideParametersOutputTypeDef,
+]
 _RequiredStartAssetBundleImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartAssetBundleImportJobRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AssetBundleImportJobId": str,
         "AssetBundleImportSource": AssetBundleImportSourceTypeDef,
     },
@@ -15077,15 +15012,15 @@
     },
 )
 _OptionalCreateDataSourceRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDataSourceRequestRequestTypeDef",
     {
         "DataSourceParameters": DataSourceParametersTypeDef,
         "Credentials": DataSourceCredentialsTypeDef,
-        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
+        "Permissions": Sequence[ResourcePermissionUnionTypeDef],
         "VpcConnectionProperties": VpcConnectionPropertiesTypeDef,
         "SslProperties": SslPropertiesTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
@@ -15760,65 +15695,116 @@
 
 class HeaderFooterSectionConfigurationTypeDef(
     _RequiredHeaderFooterSectionConfigurationTypeDef,
     _OptionalHeaderFooterSectionConfigurationTypeDef,
 ):
     pass
 
+VisualCustomActionOperationTypeDef = TypedDict(
+    "VisualCustomActionOperationTypeDef",
+    {
+        "FilterOperation": CustomActionFilterOperationTypeDef,
+        "NavigationOperation": CustomActionNavigationOperationTypeDef,
+        "URLOperation": CustomActionURLOperationTypeDef,
+        "SetParametersOperation": CustomActionSetParametersOperationTypeDef,
+    },
+    total=False,
+)
+
 DescribeDataSetResponseTypeDef = TypedDict(
     "DescribeDataSetResponseTypeDef",
     {
         "DataSet": DataSetTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredVisualCustomActionOutputTypeDef = TypedDict(
-    "_RequiredVisualCustomActionOutputTypeDef",
+_RequiredCreateDataSetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDataSetRequestRequestTypeDef",
     {
-        "CustomActionId": str,
+        "AwsAccountId": str,
+        "DataSetId": str,
         "Name": str,
-        "Trigger": VisualCustomActionTriggerType,
-        "ActionOperations": List[VisualCustomActionOperationOutputTypeDef],
+        "PhysicalTableMap": Mapping[str, PhysicalTableUnionTypeDef],
+        "ImportMode": DataSetImportModeType,
     },
 )
-_OptionalVisualCustomActionOutputTypeDef = TypedDict(
-    "_OptionalVisualCustomActionOutputTypeDef",
+_OptionalCreateDataSetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDataSetRequestRequestTypeDef",
     {
-        "Status": WidgetStatusType,
+        "LogicalTableMap": Mapping[str, LogicalTableUnionTypeDef],
+        "ColumnGroups": Sequence[ColumnGroupUnionTypeDef],
+        "FieldFolders": Mapping[str, FieldFolderUnionTypeDef],
+        "Permissions": Sequence[ResourcePermissionUnionTypeDef],
+        "RowLevelPermissionDataSet": RowLevelPermissionDataSetTypeDef,
+        "RowLevelPermissionTagConfiguration": RowLevelPermissionTagConfigurationTypeDef,
+        "ColumnLevelPermissionRules": Sequence[ColumnLevelPermissionRuleUnionTypeDef],
+        "Tags": Sequence[TagTypeDef],
+        "DataSetUsageConfiguration": DataSetUsageConfigurationTypeDef,
+        "DatasetParameters": Sequence[DatasetParameterUnionTypeDef],
     },
     total=False,
 )
 
-class VisualCustomActionOutputTypeDef(
-    _RequiredVisualCustomActionOutputTypeDef, _OptionalVisualCustomActionOutputTypeDef
+class CreateDataSetRequestRequestTypeDef(
+    _RequiredCreateDataSetRequestRequestTypeDef, _OptionalCreateDataSetRequestRequestTypeDef
 ):
     pass
 
-_RequiredVisualCustomActionTypeDef = TypedDict(
-    "_RequiredVisualCustomActionTypeDef",
+_RequiredUpdateDataSetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDataSetRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "DataSetId": str,
+        "Name": str,
+        "PhysicalTableMap": Mapping[str, PhysicalTableUnionTypeDef],
+        "ImportMode": DataSetImportModeType,
+    },
+)
+_OptionalUpdateDataSetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDataSetRequestRequestTypeDef",
+    {
+        "LogicalTableMap": Mapping[str, LogicalTableUnionTypeDef],
+        "ColumnGroups": Sequence[ColumnGroupUnionTypeDef],
+        "FieldFolders": Mapping[str, FieldFolderUnionTypeDef],
+        "RowLevelPermissionDataSet": RowLevelPermissionDataSetTypeDef,
+        "RowLevelPermissionTagConfiguration": RowLevelPermissionTagConfigurationTypeDef,
+        "ColumnLevelPermissionRules": Sequence[ColumnLevelPermissionRuleUnionTypeDef],
+        "DataSetUsageConfiguration": DataSetUsageConfigurationTypeDef,
+        "DatasetParameters": Sequence[DatasetParameterUnionTypeDef],
+    },
+    total=False,
+)
+
+class UpdateDataSetRequestRequestTypeDef(
+    _RequiredUpdateDataSetRequestRequestTypeDef, _OptionalUpdateDataSetRequestRequestTypeDef
+):
+    pass
+
+_RequiredVisualCustomActionOutputTypeDef = TypedDict(
+    "_RequiredVisualCustomActionOutputTypeDef",
     {
         "CustomActionId": str,
         "Name": str,
         "Trigger": VisualCustomActionTriggerType,
-        "ActionOperations": Sequence[VisualCustomActionOperationTypeDef],
+        "ActionOperations": List[VisualCustomActionOperationOutputTypeDef],
     },
 )
-_OptionalVisualCustomActionTypeDef = TypedDict(
-    "_OptionalVisualCustomActionTypeDef",
+_OptionalVisualCustomActionOutputTypeDef = TypedDict(
+    "_OptionalVisualCustomActionOutputTypeDef",
     {
         "Status": WidgetStatusType,
     },
     total=False,
 )
 
-class VisualCustomActionTypeDef(
-    _RequiredVisualCustomActionTypeDef, _OptionalVisualCustomActionTypeDef
+class VisualCustomActionOutputTypeDef(
+    _RequiredVisualCustomActionOutputTypeDef, _OptionalVisualCustomActionOutputTypeDef
 ):
     pass
 
 _RequiredTableFieldOptionTypeDef = TypedDict(
     "_RequiredTableFieldOptionTypeDef",
     {
         "FieldId": str,
@@ -16137,14 +16123,15 @@
 )
 
 class CreateTopicRequestRequestTypeDef(
     _RequiredCreateTopicRequestRequestTypeDef, _OptionalCreateTopicRequestRequestTypeDef
 ):
     pass
 
+TopicDetailsUnionTypeDef = Union[TopicDetailsTypeDef, TopicDetailsOutputTypeDef]
 UpdateTopicRequestRequestTypeDef = TypedDict(
     "UpdateTopicRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "TopicId": str,
         "Topic": TopicDetailsTypeDef,
     },
@@ -16210,14 +16197,36 @@
 )
 
 class BodySectionConfigurationTypeDef(
     _RequiredBodySectionConfigurationTypeDef, _OptionalBodySectionConfigurationTypeDef
 ):
     pass
 
+_RequiredVisualCustomActionTypeDef = TypedDict(
+    "_RequiredVisualCustomActionTypeDef",
+    {
+        "CustomActionId": str,
+        "Name": str,
+        "Trigger": VisualCustomActionTriggerType,
+        "ActionOperations": Sequence[VisualCustomActionOperationTypeDef],
+    },
+)
+_OptionalVisualCustomActionTypeDef = TypedDict(
+    "_OptionalVisualCustomActionTypeDef",
+    {
+        "Status": WidgetStatusType,
+    },
+    total=False,
+)
+
+class VisualCustomActionTypeDef(
+    _RequiredVisualCustomActionTypeDef, _OptionalVisualCustomActionTypeDef
+):
+    pass
+
 _RequiredCustomContentVisualOutputTypeDef = TypedDict(
     "_RequiredCustomContentVisualOutputTypeDef",
     {
         "VisualId": str,
         "DataSetIdentifier": str,
     },
 )
@@ -16253,55 +16262,14 @@
 )
 
 class EmptyVisualOutputTypeDef(
     _RequiredEmptyVisualOutputTypeDef, _OptionalEmptyVisualOutputTypeDef
 ):
     pass
 
-_RequiredCustomContentVisualTypeDef = TypedDict(
-    "_RequiredCustomContentVisualTypeDef",
-    {
-        "VisualId": str,
-        "DataSetIdentifier": str,
-    },
-)
-_OptionalCustomContentVisualTypeDef = TypedDict(
-    "_OptionalCustomContentVisualTypeDef",
-    {
-        "Title": VisualTitleLabelOptionsTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": CustomContentConfigurationTypeDef,
-        "Actions": Sequence[VisualCustomActionTypeDef],
-    },
-    total=False,
-)
-
-class CustomContentVisualTypeDef(
-    _RequiredCustomContentVisualTypeDef, _OptionalCustomContentVisualTypeDef
-):
-    pass
-
-_RequiredEmptyVisualTypeDef = TypedDict(
-    "_RequiredEmptyVisualTypeDef",
-    {
-        "VisualId": str,
-        "DataSetIdentifier": str,
-    },
-)
-_OptionalEmptyVisualTypeDef = TypedDict(
-    "_OptionalEmptyVisualTypeDef",
-    {
-        "Actions": Sequence[VisualCustomActionTypeDef],
-    },
-    total=False,
-)
-
-class EmptyVisualTypeDef(_RequiredEmptyVisualTypeDef, _OptionalEmptyVisualTypeDef):
-    pass
-
 TableFieldOptionsOutputTypeDef = TypedDict(
     "TableFieldOptionsOutputTypeDef",
     {
         "SelectedFieldOptions": List[TableFieldOptionTypeDef],
         "Order": List[str],
     },
     total=False,
@@ -17037,14 +17005,55 @@
         "HeaderSections": Sequence[HeaderFooterSectionConfigurationTypeDef],
         "BodySections": Sequence[BodySectionConfigurationTypeDef],
         "FooterSections": Sequence[HeaderFooterSectionConfigurationTypeDef],
         "CanvasSizeOptions": SectionBasedLayoutCanvasSizeOptionsTypeDef,
     },
 )
 
+_RequiredCustomContentVisualTypeDef = TypedDict(
+    "_RequiredCustomContentVisualTypeDef",
+    {
+        "VisualId": str,
+        "DataSetIdentifier": str,
+    },
+)
+_OptionalCustomContentVisualTypeDef = TypedDict(
+    "_OptionalCustomContentVisualTypeDef",
+    {
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": CustomContentConfigurationTypeDef,
+        "Actions": Sequence[VisualCustomActionTypeDef],
+    },
+    total=False,
+)
+
+class CustomContentVisualTypeDef(
+    _RequiredCustomContentVisualTypeDef, _OptionalCustomContentVisualTypeDef
+):
+    pass
+
+_RequiredEmptyVisualTypeDef = TypedDict(
+    "_RequiredEmptyVisualTypeDef",
+    {
+        "VisualId": str,
+        "DataSetIdentifier": str,
+    },
+)
+_OptionalEmptyVisualTypeDef = TypedDict(
+    "_OptionalEmptyVisualTypeDef",
+    {
+        "Actions": Sequence[VisualCustomActionTypeDef],
+    },
+    total=False,
+)
+
+class EmptyVisualTypeDef(_RequiredEmptyVisualTypeDef, _OptionalEmptyVisualTypeDef):
+    pass
+
 BarChartFieldWellsOutputTypeDef = TypedDict(
     "BarChartFieldWellsOutputTypeDef",
     {
         "BarChartAggregatedFieldWells": BarChartAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
@@ -19277,27 +19286,28 @@
         "Definition": TemplateVersionDefinitionOutputTypeDef,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AnalysisDefinitionUnionTypeDef = Union[AnalysisDefinitionTypeDef, AnalysisDefinitionOutputTypeDef]
 _RequiredCreateAnalysisRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnalysisRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
         "Name": str,
     },
 )
 _OptionalCreateAnalysisRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAnalysisRequestRequestTypeDef",
     {
         "Parameters": ParametersTypeDef,
-        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
+        "Permissions": Sequence[ResourcePermissionUnionTypeDef],
         "SourceEntity": AnalysisSourceEntityTypeDef,
         "ThemeArn": str,
         "Tags": Sequence[TagTypeDef],
         "Definition": AnalysisDefinitionTypeDef,
     },
     total=False,
 )
@@ -19339,15 +19349,15 @@
         "Name": str,
     },
 )
 _OptionalCreateDashboardRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDashboardRequestRequestTypeDef",
     {
         "Parameters": ParametersTypeDef,
-        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
+        "Permissions": Sequence[ResourcePermissionUnionTypeDef],
         "SourceEntity": DashboardSourceEntityTypeDef,
         "Tags": Sequence[TagTypeDef],
         "VersionDescription": str,
         "DashboardPublishOptions": DashboardPublishOptionsTypeDef,
         "ThemeArn": str,
         "Definition": DashboardVersionDefinitionTypeDef,
     },
@@ -19355,14 +19365,17 @@
 )
 
 class CreateDashboardRequestRequestTypeDef(
     _RequiredCreateDashboardRequestRequestTypeDef, _OptionalCreateDashboardRequestRequestTypeDef
 ):
     pass
 
+DashboardVersionDefinitionUnionTypeDef = Union[
+    DashboardVersionDefinitionTypeDef, DashboardVersionDefinitionOutputTypeDef
+]
 _RequiredUpdateDashboardRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDashboardRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "DashboardId": str,
         "Name": str,
     },
@@ -19392,28 +19405,31 @@
         "TemplateId": str,
     },
 )
 _OptionalCreateTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTemplateRequestRequestTypeDef",
     {
         "Name": str,
-        "Permissions": Sequence[Union[ResourcePermissionTypeDef, ResourcePermissionOutputTypeDef]],
+        "Permissions": Sequence[ResourcePermissionUnionTypeDef],
         "SourceEntity": TemplateSourceEntityTypeDef,
         "Tags": Sequence[TagTypeDef],
         "VersionDescription": str,
         "Definition": TemplateVersionDefinitionTypeDef,
     },
     total=False,
 )
 
 class CreateTemplateRequestRequestTypeDef(
     _RequiredCreateTemplateRequestRequestTypeDef, _OptionalCreateTemplateRequestRequestTypeDef
 ):
     pass
 
+TemplateVersionDefinitionUnionTypeDef = Union[
+    TemplateVersionDefinitionTypeDef, TemplateVersionDefinitionOutputTypeDef
+]
 _RequiredUpdateTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTemplateRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "TemplateId": str,
     },
 )
```

### Comparing `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight.egg-info/PKG-INFO` & `mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-quicksight
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.QuickSight 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.QuickSight 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 quicksight type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 quicksight type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-quicksight.svg?color=blue)](https://pypi.org/project/mypy-boto3-quicksight)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-quicksight)](https://pepy.tech/project/mypy-boto3-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QuickSight 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[boto3.QuickSight 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
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
 [mypy-boto3-quicksight docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/).
 
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
@@ -594,20 +594,20 @@
 )
 
 
 def check_value(value: AnalysisErrorTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_quicksight.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_quicksight.type_defs import (
     AccountCustomizationTypeDef,
     AccountInfoTypeDef,
     AccountSettingsTypeDef,
     ActiveIAMPolicyAssignmentTypeDef,
@@ -654,19 +654,19 @@
     SslPropertiesTypeDef,
     VpcConnectionPropertiesTypeDef,
     AssetBundleImportJobErrorTypeDef,
     AssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef,
     AssetBundleImportJobResourceIdOverrideConfigurationTypeDef,
     AssetBundleImportJobThemeOverrideParametersTypeDef,
     AssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef,
-    AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef,
     AssetBundleImportJobVPCConnectionOverrideParametersTypeDef,
+    TimestampTypeDef,
     AssetBundleImportJobSummaryTypeDef,
     AssetBundleImportSourceDescriptionTypeDef,
-    AssetBundleImportSourceTypeDef,
+    BlobTypeDef,
     AthenaParametersTypeDef,
     AuroraParametersTypeDef,
     AuroraPostgreSqlParametersTypeDef,
     AwsIotAnalyticsParametersTypeDef,
     DateAxisOptionsTypeDef,
     AxisDisplayMinMaxRangeTypeDef,
     AxisLinearScaleTypeDef,
@@ -707,42 +707,36 @@
     ConditionalFormattingSolidColorTypeDef,
     ConditionalFormattingCustomIconOptionsTypeDef,
     ConditionalFormattingIconDisplayConfigurationTypeDef,
     ConditionalFormattingIconSetTypeDef,
     TagTypeDef,
     CreateAccountSubscriptionRequestRequestTypeDef,
     SignupResponseTypeDef,
-    ResourcePermissionOutputTypeDef,
-    ResourcePermissionTypeDef,
     DataSetUsageConfigurationTypeDef,
-    FieldFolderOutputTypeDef,
-    FieldFolderTypeDef,
     RowLevelPermissionDataSetTypeDef,
     CreateFolderMembershipRequestRequestTypeDef,
     FolderMemberTypeDef,
     CreateGroupMembershipRequestRequestTypeDef,
     GroupMemberTypeDef,
     CreateGroupRequestRequestTypeDef,
     GroupTypeDef,
     CreateIAMPolicyAssignmentRequestRequestTypeDef,
     CreateIngestionRequestRequestTypeDef,
     CreateTemplateAliasRequestRequestTypeDef,
     TemplateAliasTypeDef,
     CreateThemeAliasRequestRequestTypeDef,
     ThemeAliasTypeDef,
-    TopicRefreshScheduleTypeDef,
     DecimalPlacesConfigurationTypeDef,
     NegativeValueConfigurationTypeDef,
     NullValueFormatConfigurationTypeDef,
     LocalNavigationConfigurationTypeDef,
     CustomActionURLOperationTypeDef,
     CustomContentConfigurationTypeDef,
     CustomNarrativeOptionsTypeDef,
     CustomParameterValuesOutputTypeDef,
-    CustomParameterValuesTypeDef,
     InputColumnTypeDef,
     DataPointDrillUpDownOptionTypeDef,
     DataPointMenuLabelOptionTypeDef,
     DataPointTooltipOptionTypeDef,
     ExportToCSVOptionTypeDef,
     ExportWithHiddenFieldsOptionTypeDef,
     SheetControlsOptionTypeDef,
@@ -760,14 +754,15 @@
     DataPathLabelTypeTypeDef,
     FieldLabelTypeTypeDef,
     MaximumLabelTypeTypeDef,
     MinimumLabelTypeTypeDef,
     RangeEndsLabelTypeTypeDef,
     DataPathValueTypeDef,
     DataSetSearchFilterTypeDef,
+    FieldFolderOutputTypeDef,
     OutputColumnTypeDef,
     DataSourceErrorInfoTypeDef,
     DatabricksParametersTypeDef,
     ExasolParametersTypeDef,
     JiraParametersTypeDef,
     MariaDbParametersTypeDef,
     MySqlParametersTypeDef,
@@ -781,21 +776,18 @@
     SparkParametersTypeDef,
     SqlServerParametersTypeDef,
     TeradataParametersTypeDef,
     TwitterParametersTypeDef,
     DataSourceSearchFilterTypeDef,
     DataSourceSummaryTypeDef,
     DateTimeDatasetParameterDefaultValuesOutputTypeDef,
-    DateTimeDatasetParameterDefaultValuesTypeDef,
     RollingDateConfigurationTypeDef,
     DateTimeValueWhenUnsetConfigurationOutputTypeDef,
     MappedDataSetParameterTypeDef,
-    DateTimeValueWhenUnsetConfigurationTypeDef,
     DateTimeParameterOutputTypeDef,
-    DateTimeParameterTypeDef,
     SheetControlInfoIconLabelOptionsTypeDef,
     DecimalDatasetParameterDefaultValuesOutputTypeDef,
     DecimalDatasetParameterDefaultValuesTypeDef,
     DecimalValueWhenUnsetConfigurationTypeDef,
     DecimalParameterOutputTypeDef,
     DecimalParameterTypeDef,
     DeleteAccountCustomizationRequestRequestTypeDef,
@@ -822,14 +814,15 @@
     DeleteUserRequestRequestTypeDef,
     DeleteVPCConnectionRequestRequestTypeDef,
     DescribeAccountCustomizationRequestRequestTypeDef,
     DescribeAccountSettingsRequestRequestTypeDef,
     DescribeAccountSubscriptionRequestRequestTypeDef,
     DescribeAnalysisDefinitionRequestRequestTypeDef,
     DescribeAnalysisPermissionsRequestRequestTypeDef,
+    ResourcePermissionOutputTypeDef,
     DescribeAnalysisRequestRequestTypeDef,
     DescribeAssetBundleExportJobRequestRequestTypeDef,
     DescribeAssetBundleImportJobRequestRequestTypeDef,
     DescribeDashboardDefinitionRequestRequestTypeDef,
     DescribeDashboardPermissionsRequestRequestTypeDef,
     DescribeDashboardRequestRequestTypeDef,
     DescribeDashboardSnapshotJobRequestRequestTypeDef,
@@ -869,14 +862,15 @@
     UserTypeDef,
     DescribeVPCConnectionRequestRequestTypeDef,
     NegativeFormatTypeDef,
     DonutCenterOptionsTypeDef,
     ListControlSelectAllOptionsTypeDef,
     ErrorInfoTypeDef,
     ExcludePeriodConfigurationTypeDef,
+    FieldFolderTypeDef,
     FieldSortTypeDef,
     FieldTooltipItemTypeDef,
     GeospatialMapStyleOptionsTypeDef,
     FilterSelectableValuesOutputTypeDef,
     FilterSelectableValuesTypeDef,
     SameSheetTargetVisualConfigurationOutputTypeDef,
     SameSheetTargetVisualConfigurationTypeDef,
@@ -885,16 +879,14 @@
     FolderSummaryTypeDef,
     FontSizeTypeDef,
     FontWeightTypeDef,
     FontTypeDef,
     TimeBasedForecastPropertiesTypeDef,
     WhatIfPointScenarioOutputTypeDef,
     WhatIfRangeScenarioOutputTypeDef,
-    WhatIfPointScenarioTypeDef,
-    WhatIfRangeScenarioTypeDef,
     FreeFormLayoutScreenCanvasSizeOptionsTypeDef,
     FreeFormLayoutElementBackgroundStyleTypeDef,
     FreeFormLayoutElementBorderStyleTypeDef,
     LoadingAnimationTypeDef,
     SessionTagTypeDef,
     GeospatialCoordinateBoundsTypeDef,
     GeospatialHeatmapDataColorTypeDef,
@@ -962,15 +954,14 @@
     ManifestFileLocationTypeDef,
     MarginStyleTypeDef,
     NamedEntityDefinitionMetricOutputTypeDef,
     NamedEntityDefinitionMetricTypeDef,
     NamespaceErrorTypeDef,
     NetworkInterfaceTypeDef,
     NewDefaultValuesOutputTypeDef,
-    NewDefaultValuesTypeDef,
     NumericRangeFilterValueTypeDef,
     ThousandSeparatorOptionsTypeDef,
     PercentileAggregationTypeDef,
     StringParameterOutputTypeDef,
     StringParameterTypeDef,
     PercentVisibleRangeTypeDef,
     PivotTableConditionalFormattingScopeTypeDef,
@@ -987,14 +978,15 @@
     ReferenceLineStaticDataConfigurationTypeDef,
     ReferenceLineStyleConfigurationTypeDef,
     ScheduleRefreshOnEntityTypeDef,
     RegisterUserRequestRequestTypeDef,
     StatePersistenceConfigurationsTypeDef,
     RegisteredUserQSearchBarEmbeddingConfigurationTypeDef,
     RenameColumnOperationTypeDef,
+    ResourcePermissionTypeDef,
     RestoreAnalysisRequestRequestTypeDef,
     RowLevelPermissionTagRuleTypeDef,
     S3BucketConfigurationTypeDef,
     UploadSettingsTypeDef,
     SectionAfterPageBreakTypeDef,
     SpacingTypeDef,
     SheetVisualScopingConfigurationOutputTypeDef,
@@ -1048,30 +1040,40 @@
     DynamicDefaultValueTypeDef,
     FilterOperationSelectedFieldsConfigurationOutputTypeDef,
     FilterOperationSelectedFieldsConfigurationTypeDef,
     NumericEqualityDrillDownFilterTypeDef,
     ParameterSelectableValuesOutputTypeDef,
     ParameterSelectableValuesTypeDef,
     TimeEqualityFilterOutputTypeDef,
-    TimeEqualityFilterTypeDef,
     TimeRangeDrillDownFilterOutputTypeDef,
-    TimeRangeDrillDownFilterTypeDef,
     AnalysisErrorTypeDef,
     DashboardErrorTypeDef,
     TemplateErrorTypeDef,
     SearchAnalysesRequestRequestTypeDef,
     AnalysisSourceTemplateTypeDef,
     DashboardSourceTemplateTypeDef,
     TemplateSourceAnalysisTypeDef,
     AnonymousUserDashboardVisualEmbeddingConfigurationTypeDef,
     RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef,
     ArcAxisConfigurationTypeDef,
     AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef,
     AssetBundleCloudFormationOverridePropertyConfigurationTypeDef,
     AssetBundleImportJobDataSourceCredentialsTypeDef,
+    AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef,
+    CustomParameterValuesTypeDef,
+    DateTimeDatasetParameterDefaultValuesTypeDef,
+    DateTimeParameterTypeDef,
+    DateTimeValueWhenUnsetConfigurationTypeDef,
+    NewDefaultValuesTypeDef,
+    TimeEqualityFilterTypeDef,
+    TimeRangeDrillDownFilterTypeDef,
+    TopicRefreshScheduleTypeDef,
+    WhatIfPointScenarioTypeDef,
+    WhatIfRangeScenarioTypeDef,
+    AssetBundleImportSourceTypeDef,
     AxisDisplayRangeOutputTypeDef,
     AxisDisplayRangeTypeDef,
     AxisScaleTypeDef,
     HistogramBinOptionsTypeDef,
     TileStyleTypeDef,
     BoxPlotOptionsTypeDef,
     CreateColumnsOperationOutputTypeDef,
@@ -1164,46 +1166,24 @@
     ColorsConfigurationOutputTypeDef,
     ColorsConfigurationTypeDef,
     ColumnTagTypeDef,
     ColumnGroupSchemaOutputTypeDef,
     ColumnGroupSchemaTypeDef,
     ColumnGroupOutputTypeDef,
     ColumnGroupTypeDef,
+    ColumnLevelPermissionRuleUnionTypeDef,
     DataSetSchemaOutputTypeDef,
     DataSetSchemaTypeDef,
     ConditionalFormattingCustomIconConditionTypeDef,
     CreateAccountCustomizationRequestRequestTypeDef,
     CreateNamespaceRequestRequestTypeDef,
     CreateVPCConnectionRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateAccountSubscriptionResponseTypeDef,
-    DescribeAnalysisPermissionsResponseTypeDef,
-    DescribeDataSetPermissionsResponseTypeDef,
-    DescribeDataSourcePermissionsResponseTypeDef,
-    DescribeFolderPermissionsResponseTypeDef,
-    DescribeFolderResolvedPermissionsResponseTypeDef,
-    DescribeTemplatePermissionsResponseTypeDef,
-    DescribeThemePermissionsResponseTypeDef,
-    DescribeTopicPermissionsResponseTypeDef,
-    LinkSharingConfigurationTypeDef,
-    UpdateAnalysisPermissionsResponseTypeDef,
-    UpdateFolderPermissionsResponseTypeDef,
-    UpdateTemplatePermissionsResponseTypeDef,
-    UpdateThemePermissionsResponseTypeDef,
-    UpdateTopicPermissionsResponseTypeDef,
-    CreateFolderRequestRequestTypeDef,
-    UpdateAnalysisPermissionsRequestRequestTypeDef,
-    UpdateDashboardPermissionsRequestRequestTypeDef,
-    UpdateDataSetPermissionsRequestRequestTypeDef,
-    UpdateDataSourcePermissionsRequestRequestTypeDef,
-    UpdateFolderPermissionsRequestRequestTypeDef,
-    UpdateTemplatePermissionsRequestRequestTypeDef,
-    UpdateThemePermissionsRequestRequestTypeDef,
-    UpdateTopicPermissionsRequestRequestTypeDef,
     DataSetSummaryTypeDef,
     CreateFolderMembershipResponseTypeDef,
     CreateGroupMembershipResponseTypeDef,
     DescribeGroupMembershipResponseTypeDef,
     ListGroupMembershipsResponseTypeDef,
     CreateGroupResponseTypeDef,
     DescribeGroupResponseTypeDef,
@@ -1215,19 +1195,16 @@
     DescribeTemplateAliasResponseTypeDef,
     ListTemplateAliasesResponseTypeDef,
     UpdateTemplateAliasResponseTypeDef,
     CreateThemeAliasResponseTypeDef,
     DescribeThemeAliasResponseTypeDef,
     ListThemeAliasesResponseTypeDef,
     UpdateThemeAliasResponseTypeDef,
-    CreateTopicRefreshScheduleRequestRequestTypeDef,
-    UpdateTopicRefreshScheduleRequestRequestTypeDef,
     CustomActionNavigationOperationTypeDef,
     CustomValuesConfigurationOutputTypeDef,
-    CustomValuesConfigurationTypeDef,
     CustomSqlOutputTypeDef,
     CustomSqlTypeDef,
     RelationalTableOutputTypeDef,
     RelationalTableTypeDef,
     SearchDashboardsRequestRequestTypeDef,
     ListDashboardsResponseTypeDef,
     SearchDashboardsResponseTypeDef,
@@ -1242,41 +1219,54 @@
     PivotTableDataPathOptionTypeDef,
     PivotTableFieldCollapseStateTargetOutputTypeDef,
     PivotTableFieldCollapseStateTargetTypeDef,
     SearchDataSetsRequestRequestTypeDef,
     SearchDataSourcesRequestRequestTypeDef,
     SearchDataSourcesResponseTypeDef,
     DateTimeDatasetParameterOutputTypeDef,
-    DateTimeDatasetParameterTypeDef,
     TimeRangeFilterValueOutputTypeDef,
     TimeRangeFilterValueTypeDef,
     DecimalDatasetParameterOutputTypeDef,
     DecimalDatasetParameterTypeDef,
+    DescribeAnalysisPermissionsResponseTypeDef,
+    DescribeDataSetPermissionsResponseTypeDef,
+    DescribeDataSourcePermissionsResponseTypeDef,
+    DescribeFolderPermissionsResponseTypeDef,
+    DescribeFolderResolvedPermissionsResponseTypeDef,
+    DescribeTemplatePermissionsResponseTypeDef,
+    DescribeThemePermissionsResponseTypeDef,
+    DescribeTopicPermissionsResponseTypeDef,
+    LinkSharingConfigurationTypeDef,
+    UpdateAnalysisPermissionsResponseTypeDef,
+    UpdateFolderPermissionsResponseTypeDef,
+    UpdateTemplatePermissionsResponseTypeDef,
+    UpdateThemePermissionsResponseTypeDef,
+    UpdateTopicPermissionsResponseTypeDef,
     DescribeFolderResponseTypeDef,
     DescribeIAMPolicyAssignmentResponseTypeDef,
     DescribeTopicRefreshResponseTypeDef,
     DescribeTopicRefreshScheduleResponseTypeDef,
     TopicRefreshScheduleSummaryTypeDef,
     DescribeUserResponseTypeDef,
     ListUsersResponseTypeDef,
     RegisterUserResponseTypeDef,
     UpdateUserResponseTypeDef,
     DisplayFormatOptionsTypeDef,
     DonutOptionsTypeDef,
     RelativeDatesFilterTypeDef,
+    FieldFolderUnionTypeDef,
     FilterOperationTargetVisualsConfigurationOutputTypeDef,
     FilterOperationTargetVisualsConfigurationTypeDef,
     SearchFoldersRequestRequestTypeDef,
     ListFoldersResponseTypeDef,
     SearchFoldersResponseTypeDef,
     FontConfigurationTypeDef,
     TypographyOutputTypeDef,
     TypographyTypeDef,
     ForecastScenarioOutputTypeDef,
-    ForecastScenarioTypeDef,
     FreeFormLayoutCanvasSizeOptionsTypeDef,
     SnapshotAnonymousUserTypeDef,
     GeospatialWindowOptionsTypeDef,
     GeospatialHeatmapColorScaleOutputTypeDef,
     GeospatialHeatmapColorScaleTypeDef,
     TableSideBorderOptionsTypeDef,
     GradientColorOutputTypeDef,
@@ -1327,25 +1317,24 @@
     TileLayoutStyleTypeDef,
     NamedEntityDefinitionOutputTypeDef,
     NamedEntityDefinitionTypeDef,
     NamespaceInfoV2TypeDef,
     VPCConnectionSummaryTypeDef,
     VPCConnectionTypeDef,
     OverrideDatasetParameterOperationOutputTypeDef,
-    OverrideDatasetParameterOperationTypeDef,
     NumericSeparatorConfigurationTypeDef,
     NumericalAggregationFunctionTypeDef,
     ParametersOutputTypeDef,
-    ParametersTypeDef,
     VisibleRangeOptionsTypeDef,
     RadarChartSeriesSettingsTypeDef,
     TopicRangeFilterConstantTypeDef,
     RefreshFrequencyTypeDef,
     RegisteredUserConsoleFeatureConfigurationsTypeDef,
     RegisteredUserDashboardFeatureConfigurationsTypeDef,
+    ResourcePermissionUnionTypeDef,
     RowLevelPermissionTagConfigurationOutputTypeDef,
     RowLevelPermissionTagConfigurationTypeDef,
     SnapshotS3DestinationConfigurationTypeDef,
     S3SourceOutputTypeDef,
     S3SourceTypeDef,
     SectionPageBreakConfigurationTypeDef,
     SectionBasedLayoutPaperCanvasSizeOptionsTypeDef,
@@ -1369,61 +1358,69 @@
     DecimalDefaultValuesOutputTypeDef,
     DecimalDefaultValuesTypeDef,
     IntegerDefaultValuesOutputTypeDef,
     IntegerDefaultValuesTypeDef,
     StringDefaultValuesOutputTypeDef,
     StringDefaultValuesTypeDef,
     DrillDownFilterOutputTypeDef,
-    DrillDownFilterTypeDef,
     AnalysisTypeDef,
     DashboardVersionTypeDef,
     AnalysisSourceEntityTypeDef,
     DashboardSourceEntityTypeDef,
     TemplateSourceEntityTypeDef,
     AnonymousUserEmbeddingExperienceConfigurationTypeDef,
     DescribeAssetBundleExportJobResponseTypeDef,
+    AssetBundleCloudFormationOverridePropertyConfigurationUnionTypeDef,
     StartAssetBundleExportJobRequestRequestTypeDef,
+    CustomValuesConfigurationTypeDef,
+    DateTimeDatasetParameterTypeDef,
+    ParametersTypeDef,
+    OverrideDatasetParameterOperationTypeDef,
+    DrillDownFilterTypeDef,
+    CreateTopicRefreshScheduleRequestRequestTypeDef,
+    TopicRefreshScheduleUnionTypeDef,
+    UpdateTopicRefreshScheduleRequestRequestTypeDef,
+    ForecastScenarioTypeDef,
     NumericAxisOptionsOutputTypeDef,
     NumericAxisOptionsTypeDef,
     CategoryFilterOutputTypeDef,
     CategoryFilterTypeDef,
     ClusterMarkerConfigurationTypeDef,
     TopicCategoryFilterOutputTypeDef,
     TopicCategoryFilterTypeDef,
     TagColumnOperationOutputTypeDef,
     TagColumnOperationTypeDef,
+    ColumnGroupUnionTypeDef,
     DataSetConfigurationOutputTypeDef,
     DataSetConfigurationTypeDef,
     ConditionalFormattingIconTypeDef,
-    DescribeDashboardPermissionsResponseTypeDef,
-    UpdateDashboardPermissionsResponseTypeDef,
     ListDataSetsResponseTypeDef,
     SearchDataSetsResponseTypeDef,
     DestinationParameterValueConfigurationOutputTypeDef,
-    DestinationParameterValueConfigurationTypeDef,
     DashboardPublishOptionsTypeDef,
     VisualPaletteOutputTypeDef,
     VisualPaletteTypeDef,
     PivotTableFieldCollapseStateOptionOutputTypeDef,
     PivotTableFieldCollapseStateOptionTypeDef,
     TimeRangeFilterOutputTypeDef,
     TimeRangeFilterTypeDef,
+    DescribeDashboardPermissionsResponseTypeDef,
+    UpdateDashboardPermissionsResponseTypeDef,
     ListTopicRefreshSchedulesResponseTypeDef,
     DefaultFormattingTypeDef,
     CustomActionFilterOperationOutputTypeDef,
     CustomActionFilterOperationTypeDef,
     AxisLabelOptionsTypeDef,
     DataLabelOptionsOutputTypeDef,
     DataLabelOptionsTypeDef,
     FunnelChartDataLabelOptionsTypeDef,
     LabelOptionsTypeDef,
     PanelTitleOptionsTypeDef,
     TableFieldCustomTextContentTypeDef,
     ForecastConfigurationOutputTypeDef,
-    ForecastConfigurationTypeDef,
     DefaultFreeFormLayoutConfigurationTypeDef,
     SnapshotUserConfigurationTypeDef,
     GeospatialHeatmapConfigurationOutputTypeDef,
     GeospatialHeatmapConfigurationTypeDef,
     GlobalTableBorderOptionsTypeDef,
     ConditionalFormattingGradientColorOutputTypeDef,
     ConditionalFormattingGradientColorTypeDef,
@@ -1451,52 +1448,64 @@
     ScrollBarOptionsTypeDef,
     TopicDateRangeFilterTypeDef,
     TopicNumericRangeFilterTypeDef,
     RefreshScheduleOutputTypeDef,
     RefreshScheduleTypeDef,
     RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef,
     RegisteredUserDashboardEmbeddingConfigurationTypeDef,
+    CreateFolderRequestRequestTypeDef,
+    UpdateAnalysisPermissionsRequestRequestTypeDef,
+    UpdateDashboardPermissionsRequestRequestTypeDef,
+    UpdateDataSetPermissionsRequestRequestTypeDef,
+    UpdateDataSourcePermissionsRequestRequestTypeDef,
+    UpdateFolderPermissionsRequestRequestTypeDef,
+    UpdateTemplatePermissionsRequestRequestTypeDef,
+    UpdateThemePermissionsRequestRequestTypeDef,
+    UpdateTopicPermissionsRequestRequestTypeDef,
+    RowLevelPermissionTagConfigurationUnionTypeDef,
     SnapshotDestinationConfigurationOutputTypeDef,
     SnapshotDestinationConfigurationTypeDef,
     SnapshotJobS3ResultTypeDef,
     PhysicalTableOutputTypeDef,
     PhysicalTableTypeDef,
     SectionBasedLayoutCanvasSizeOptionsTypeDef,
     FilterScopeConfigurationOutputTypeDef,
     FilterScopeConfigurationTypeDef,
     FreeFormLayoutElementOutputTypeDef,
     FreeFormLayoutElementTypeDef,
     SnapshotFileGroupOutputTypeDef,
     SnapshotFileGroupTypeDef,
     DatasetParameterOutputTypeDef,
-    DatasetParameterTypeDef,
     DateTimeParameterDeclarationOutputTypeDef,
     DateTimeParameterDeclarationTypeDef,
     DecimalParameterDeclarationOutputTypeDef,
     DecimalParameterDeclarationTypeDef,
     IntegerParameterDeclarationOutputTypeDef,
     IntegerParameterDeclarationTypeDef,
     StringParameterDeclarationOutputTypeDef,
     StringParameterDeclarationTypeDef,
     DateTimeHierarchyOutputTypeDef,
     ExplicitHierarchyOutputTypeDef,
     PredefinedHierarchyOutputTypeDef,
-    DateTimeHierarchyTypeDef,
-    ExplicitHierarchyTypeDef,
-    PredefinedHierarchyTypeDef,
     DescribeAnalysisResponseTypeDef,
     DashboardTypeDef,
     GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef,
+    DestinationParameterValueConfigurationTypeDef,
+    DatasetParameterTypeDef,
+    ParametersUnionTypeDef,
+    DateTimeHierarchyTypeDef,
+    ExplicitHierarchyTypeDef,
+    PredefinedHierarchyTypeDef,
+    ForecastConfigurationTypeDef,
     AxisDataOptionsOutputTypeDef,
     AxisDataOptionsTypeDef,
     TransformOperationOutputTypeDef,
     TransformOperationTypeDef,
     TemplateVersionTypeDef,
     SetParameterValueConfigurationOutputTypeDef,
-    SetParameterValueConfigurationTypeDef,
     PivotTableFieldOptionsOutputTypeDef,
     PivotTableFieldOptionsTypeDef,
     TopicCalculatedFieldOutputTypeDef,
     TopicCalculatedFieldTypeDef,
     TopicColumnOutputTypeDef,
     TopicColumnTypeDef,
     ChartAxisLabelOptionsOutputTypeDef,
@@ -1536,34 +1545,37 @@
     NumericRangeFilterTypeDef,
     ReferenceLineDynamicDataConfigurationTypeDef,
     TopicFilterOutputTypeDef,
     TopicFilterTypeDef,
     DescribeRefreshScheduleResponseTypeDef,
     ListRefreshSchedulesResponseTypeDef,
     CreateRefreshScheduleRequestRequestTypeDef,
+    RefreshScheduleUnionTypeDef,
     UpdateRefreshScheduleRequestRequestTypeDef,
     RegisteredUserEmbeddingExperienceConfigurationTypeDef,
     SnapshotJobResultFileGroupTypeDef,
+    PhysicalTableUnionTypeDef,
     DefaultSectionBasedLayoutConfigurationTypeDef,
     FreeFormLayoutConfigurationOutputTypeDef,
     FreeFormSectionLayoutConfigurationOutputTypeDef,
     FreeFormLayoutConfigurationTypeDef,
     FreeFormSectionLayoutConfigurationTypeDef,
     SnapshotConfigurationOutputTypeDef,
     SnapshotConfigurationTypeDef,
     ParameterDeclarationOutputTypeDef,
     ParameterDeclarationTypeDef,
     ColumnHierarchyOutputTypeDef,
-    ColumnHierarchyTypeDef,
     DescribeDashboardResponseTypeDef,
+    SetParameterValueConfigurationTypeDef,
+    DatasetParameterUnionTypeDef,
+    ColumnHierarchyTypeDef,
     LogicalTableOutputTypeDef,
     LogicalTableTypeDef,
     TemplateTypeDef,
     CustomActionSetParametersOperationOutputTypeDef,
-    CustomActionSetParametersOperationTypeDef,
     AxisDisplayOptionsOutputTypeDef,
     AxisDisplayOptionsTypeDef,
     FilterDateTimePickerControlTypeDef,
     ParameterDateTimePickerControlTypeDef,
     FilterDropDownControlOutputTypeDef,
     FilterDropDownControlTypeDef,
     ParameterDropDownControlOutputTypeDef,
@@ -1610,14 +1622,15 @@
     AssetBundleImportJobOverrideParametersOutputTypeDef,
     AssetBundleImportJobOverrideParametersTypeDef,
     DataSourceCredentialsTypeDef,
     DescribeDataSourceResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     ThemeVersionTypeDef,
     CreateThemeRequestRequestTypeDef,
+    ThemeConfigurationUnionTypeDef,
     UpdateThemeRequestRequestTypeDef,
     ComparisonConfigurationTypeDef,
     DateTimeFormatConfigurationTypeDef,
     NumberFormatConfigurationTypeDef,
     ReferenceLineValueLabelConfigurationTypeDef,
     StringFormatConfigurationTypeDef,
     TopBottomFilterOutputTypeDef,
@@ -1631,21 +1644,21 @@
     DatasetMetadataTypeDef,
     GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef,
     AnonymousUserSnapshotJobResultTypeDef,
     DefaultPaginatedLayoutConfigurationTypeDef,
     SectionLayoutConfigurationOutputTypeDef,
     SectionLayoutConfigurationTypeDef,
     DescribeDashboardSnapshotJobResponseTypeDef,
+    SnapshotConfigurationUnionTypeDef,
     StartDashboardSnapshotJobRequestRequestTypeDef,
+    CustomActionSetParametersOperationTypeDef,
     DataSetTypeDef,
-    CreateDataSetRequestRequestTypeDef,
-    UpdateDataSetRequestRequestTypeDef,
+    LogicalTableUnionTypeDef,
     DescribeTemplateResponseTypeDef,
     VisualCustomActionOperationOutputTypeDef,
-    VisualCustomActionOperationTypeDef,
     LineSeriesAxisDisplayOptionsOutputTypeDef,
     LineSeriesAxisDisplayOptionsTypeDef,
     FilterControlOutputTypeDef,
     FilterControlTypeDef,
     ParameterControlOutputTypeDef,
     ParameterControlTypeDef,
     TableFieldURLConfigurationTypeDef,
@@ -1658,14 +1671,15 @@
     TableCellConditionalFormattingOutputTypeDef,
     GaugeChartConditionalFormattingOptionTypeDef,
     KPIConditionalFormattingOptionTypeDef,
     FilledMapShapeConditionalFormattingTypeDef,
     PivotTableCellConditionalFormattingTypeDef,
     TableCellConditionalFormattingTypeDef,
     DescribeAssetBundleImportJobResponseTypeDef,
+    AssetBundleImportJobOverrideParametersUnionTypeDef,
     StartAssetBundleImportJobRequestRequestTypeDef,
     CreateDataSourceRequestRequestTypeDef,
     UpdateDataSourceRequestRequestTypeDef,
     ThemeTypeDef,
     GaugeChartOptionsTypeDef,
     KPIOptionsTypeDef,
     DateDimensionFieldTypeDef,
@@ -1716,17 +1730,19 @@
     TopicDetailsTypeDef,
     SnapshotJobResultTypeDef,
     DefaultNewSheetConfigurationTypeDef,
     BodySectionContentOutputTypeDef,
     HeaderFooterSectionConfigurationOutputTypeDef,
     BodySectionContentTypeDef,
     HeaderFooterSectionConfigurationTypeDef,
+    VisualCustomActionOperationTypeDef,
     DescribeDataSetResponseTypeDef,
+    CreateDataSetRequestRequestTypeDef,
+    UpdateDataSetRequestRequestTypeDef,
     VisualCustomActionOutputTypeDef,
-    VisualCustomActionTypeDef,
     TableFieldOptionTypeDef,
     GaugeChartConditionalFormattingOutputTypeDef,
     KPIConditionalFormattingOutputTypeDef,
     FilledMapConditionalFormattingOptionOutputTypeDef,
     PivotTableConditionalFormattingOptionOutputTypeDef,
     TableConditionalFormattingOptionOutputTypeDef,
     GaugeChartConditionalFormattingTypeDef,
@@ -1745,23 +1761,23 @@
     FilterGroupTypeDef,
     PivotTableSortConfigurationOutputTypeDef,
     PivotTableSortConfigurationTypeDef,
     TooltipOptionsOutputTypeDef,
     TooltipOptionsTypeDef,
     DescribeTopicResponseTypeDef,
     CreateTopicRequestRequestTypeDef,
+    TopicDetailsUnionTypeDef,
     UpdateTopicRequestRequestTypeDef,
     DescribeDashboardSnapshotJobResultResponseTypeDef,
     AnalysisDefaultsTypeDef,
     BodySectionConfigurationOutputTypeDef,
     BodySectionConfigurationTypeDef,
+    VisualCustomActionTypeDef,
     CustomContentVisualOutputTypeDef,
     EmptyVisualOutputTypeDef,
-    CustomContentVisualTypeDef,
-    EmptyVisualTypeDef,
     TableFieldOptionsOutputTypeDef,
     TableFieldOptionsTypeDef,
     FilledMapConditionalFormattingOutputTypeDef,
     PivotTableConditionalFormattingOutputTypeDef,
     TableConditionalFormattingOutputTypeDef,
     FilledMapConditionalFormattingTypeDef,
     PivotTableConditionalFormattingTypeDef,
@@ -1818,14 +1834,16 @@
     WaterfallChartAggregatedFieldWellsTypeDef,
     WordCloudAggregatedFieldWellsOutputTypeDef,
     WordCloudAggregatedFieldWellsTypeDef,
     TableUnaggregatedFieldWellsOutputTypeDef,
     TableUnaggregatedFieldWellsTypeDef,
     SectionBasedLayoutConfigurationOutputTypeDef,
     SectionBasedLayoutConfigurationTypeDef,
+    CustomContentVisualTypeDef,
+    EmptyVisualTypeDef,
     BarChartFieldWellsOutputTypeDef,
     BarChartFieldWellsTypeDef,
     BoxPlotFieldWellsOutputTypeDef,
     BoxPlotFieldWellsTypeDef,
     ComboChartFieldWellsOutputTypeDef,
     ComboChartFieldWellsTypeDef,
     FilledMapFieldWellsOutputTypeDef,
@@ -1956,24 +1974,27 @@
     TemplateVersionDefinitionOutputTypeDef,
     AnalysisDefinitionTypeDef,
     DashboardVersionDefinitionTypeDef,
     TemplateVersionDefinitionTypeDef,
     DescribeAnalysisDefinitionResponseTypeDef,
     DescribeDashboardDefinitionResponseTypeDef,
     DescribeTemplateDefinitionResponseTypeDef,
+    AnalysisDefinitionUnionTypeDef,
     CreateAnalysisRequestRequestTypeDef,
     UpdateAnalysisRequestRequestTypeDef,
     CreateDashboardRequestRequestTypeDef,
+    DashboardVersionDefinitionUnionTypeDef,
     UpdateDashboardRequestRequestTypeDef,
     CreateTemplateRequestRequestTypeDef,
+    TemplateVersionDefinitionUnionTypeDef,
     UpdateTemplateRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccountCustomizationTypeDef:
+def get_value() -> AccountCustomizationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-quicksight-1.28.15.post1/mypy_boto3_quicksight.egg-info/SOURCES.txt` & `mypy-boto3-quicksight-1.28.16/mypy_boto3_quicksight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.15.post1/setup.py` & `mypy-boto3-quicksight-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-quicksight",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_quicksight"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.QuickSight 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.QuickSight 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 quicksight type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 quicksight type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_quicksight": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

