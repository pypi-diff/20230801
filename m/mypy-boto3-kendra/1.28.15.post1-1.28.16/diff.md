# Comparing `tmp/mypy-boto3-kendra-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-kendra-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kendra-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:26 2023, max compression
+gzip compressed data, was "mypy-boto3-kendra-1.28.16.tar", last modified: Tue Aug  1 11:37:06 2023, max compression
```

## Comparing `mypy-boto3-kendra-1.28.15.post1.tar` & `mypy-boto3-kendra-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:26.297213 mypy-boto3-kendra-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:38.000000 mypy-boto3-kendra-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25922 2023-07-29 10:03:26.293213 mypy-boto3-kendra-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24433 2023-07-29 09:48:38.000000 mypy-boto3-kendra-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:26.289213 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-29 09:48:38.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-29 09:48:38.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-29 09:48:38.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49177 2023-07-29 09:48:39.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49105 2023-07-29 09:48:38.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-29 09:48:39.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-07-29 09:48:39.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:38.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   144427 2023-07-29 09:48:43.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   144216 2023-07-29 09:48:41.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:38.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:26.293213 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25922 2023-07-29 10:03:26.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-29 10:03:26.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:26.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:26.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:26.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:03:26.000000 mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:26.309213 mypy-boto3-kendra-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-29 09:48:38.000000 mypy-boto3-kendra-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:06.468852 mypy-boto3-kendra-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:21:24.000000 mypy-boto3-kendra-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26245 2023-08-01 11:37:06.456852 mypy-boto3-kendra-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24765 2023-08-01 11:21:24.000000 mypy-boto3-kendra-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:06.456852 mypy-boto3-kendra-1.28.16/mypy_boto3_kendra/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-01 11:21:24.000000 mypy-boto3-kendra-1.28.16/mypy_boto3_kendra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-01 11:21:24.000000 mypy-boto3-kendra-1.28.16/mypy_boto3_kendra/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-01 11:21:24.000000 mypy-boto3-kendra-1.28.16/mypy_boto3_kendra/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48067 2023-08-01 11:21:25.000000 mypy-boto3-kendra-1.28.16/mypy_boto3_kendra/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47995 2023-08-01 11:21:25.000000 mypy-boto3-kendra-1.28.16/mypy_boto3_kendra/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-08-01 11:21:25.000000 mypy-boto3-kendra-1.28.16/mypy_boto3_kendra/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-08-01 11:21:25.000000 mypy-boto3-kendra-1.28.16/mypy_boto3_kendra/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:21:24.000000 mypy-boto3-kendra-1.28.16/mypy_boto3_kendra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   145493 2023-08-01 11:21:31.000000 mypy-boto3-kendra-1.28.16/mypy_boto3_kendra/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   145282 2023-08-01 11:21:27.000000 mypy-boto3-kendra-1.28.16/mypy_boto3_kendra/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:21:24.000000 mypy-boto3-kendra-1.28.16/mypy_boto3_kendra/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:06.456852 mypy-boto3-kendra-1.28.16/mypy_boto3_kendra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26245 2023-08-01 11:37:06.000000 mypy-boto3-kendra-1.28.16/mypy_boto3_kendra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-01 11:37:06.000000 mypy-boto3-kendra-1.28.16/mypy_boto3_kendra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:06.000000 mypy-boto3-kendra-1.28.16/mypy_boto3_kendra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:06.000000 mypy-boto3-kendra-1.28.16/mypy_boto3_kendra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:06.000000 mypy-boto3-kendra-1.28.16/mypy_boto3_kendra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 11:37:06.000000 mypy-boto3-kendra-1.28.16/mypy_boto3_kendra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:06.468852 mypy-boto3-kendra-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-01 11:21:24.000000 mypy-boto3-kendra-1.28.16/setup.py
```

### Comparing `mypy-boto3-kendra-1.28.15.post1/LICENSE` & `mypy-boto3-kendra-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.28.15.post1/PKG-INFO` & `mypy-boto3-kendra-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kendra
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.kendra 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.kendra 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kendra type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 kendra type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kendra.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kendra)](https://pepy.tech/project/mypy-boto3-kendra)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.kendra 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
+[boto3.kendra 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
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
 [mypy-boto3-kendra docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/).
 
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
@@ -347,20 +347,20 @@
 )
 
 
 def check_value(value: AdditionalResultAttributeValueTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kendra.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kendra.type_defs import (
     AccessControlConfigurationSummaryTypeDef,
     AccessControlListConfigurationTypeDef,
     AclConfigurationTypeDef,
     DataSourceToIndexFieldMappingTypeDef,
@@ -376,17 +376,18 @@
     DataSourceSyncJobMetricTargetTypeDef,
     BatchDeleteDocumentResponseFailedDocumentTypeDef,
     BatchDeleteFeaturedResultsSetErrorTypeDef,
     BatchDeleteFeaturedResultsSetRequestRequestTypeDef,
     BatchGetDocumentStatusResponseErrorTypeDef,
     StatusTypeDef,
     BatchPutDocumentResponseFailedDocumentTypeDef,
+    BlobTypeDef,
     CapacityUnitsConfigurationTypeDef,
     ClearQuerySuggestionsRequestRequestTypeDef,
-    ClickFeedbackTypeDef,
+    TimestampTypeDef,
     ConfluenceAttachmentToIndexFieldMappingTypeDef,
     ConfluenceBlogToIndexFieldMappingTypeDef,
     ProxyConfigurationTypeDef,
     ConfluencePageToIndexFieldMappingTypeDef,
     ConfluenceSpaceToIndexFieldMappingTypeDef,
     ConnectionConfigurationTypeDef,
     ContentSourceConfigurationOutputTypeDef,
@@ -423,15 +424,14 @@
     DescribePrincipalMappingRequestRequestTypeDef,
     GroupOrderingIdSummaryTypeDef,
     DescribeQuerySuggestionsBlockListRequestRequestTypeDef,
     DescribeQuerySuggestionsConfigRequestRequestTypeDef,
     DescribeThesaurusRequestRequestTypeDef,
     DisassociatePersonasFromEntitiesRequestRequestTypeDef,
     DocumentAttributeValueOutputTypeDef,
-    DocumentAttributeValueTypeDef,
     RelevanceOutputTypeDef,
     SearchTypeDef,
     RelevanceTypeDef,
     DocumentsMetadataConfigurationTypeDef,
     EntityDisplayDataTypeDef,
     UserIdentityConfigurationTypeDef,
     FacetResultTypeDef,
@@ -448,15 +448,14 @@
     GroupSummaryTypeDef,
     HighlightTypeDef,
     IndexConfigurationSummaryTypeDef,
     TextDocumentStatisticsTypeDef,
     JsonTokenTypeConfigurationTypeDef,
     JwtTokenTypeConfigurationTypeDef,
     ListAccessControlConfigurationsRequestRequestTypeDef,
-    TimeRangeTypeDef,
     ListDataSourcesRequestRequestTypeDef,
     ListEntityPersonasRequestRequestTypeDef,
     PersonasSummaryTypeDef,
     ListExperienceEntitiesRequestRequestTypeDef,
     ListExperiencesRequestRequestTypeDef,
     ListFaqsRequestRequestTypeDef,
     ListFeaturedResultsSetsRequestRequestTypeDef,
@@ -510,14 +509,15 @@
     OnPremiseConfigurationTypeDef,
     OneDriveUsersOutputTypeDef,
     OneDriveUsersTypeDef,
     UpdateQuerySuggestionsBlockListRequestRequestTypeDef,
     UpdateThesaurusRequestRequestTypeDef,
     AlfrescoConfigurationTypeDef,
     BoxConfigurationTypeDef,
+    DataSourceVpcConfigurationUnionTypeDef,
     FsxConfigurationTypeDef,
     JiraConfigurationTypeDef,
     QuipConfigurationTypeDef,
     SlackConfigurationTypeDef,
     AssociateEntitiesToExperienceRequestRequestTypeDef,
     DisassociateEntitiesFromExperienceRequestRequestTypeDef,
     AssociateEntitiesToExperienceResponseTypeDef,
@@ -543,14 +543,17 @@
     AuthenticationConfigurationOutputTypeDef,
     AuthenticationConfigurationTypeDef,
     BatchDeleteDocumentRequestRequestTypeDef,
     BatchDeleteDocumentResponseTypeDef,
     BatchDeleteFeaturedResultsSetResponseTypeDef,
     BatchGetDocumentStatusResponseTypeDef,
     BatchPutDocumentResponseTypeDef,
+    ClickFeedbackTypeDef,
+    DocumentAttributeValueTypeDef,
+    TimeRangeTypeDef,
     ConfluenceAttachmentConfigurationOutputTypeDef,
     ConfluenceAttachmentConfigurationTypeDef,
     ConfluenceBlogConfigurationOutputTypeDef,
     ConfluenceBlogConfigurationTypeDef,
     SharePointConfigurationOutputTypeDef,
     SharePointConfigurationTypeDef,
     ConfluencePageConfigurationOutputTypeDef,
@@ -574,17 +577,14 @@
     ExperiencesSummaryTypeDef,
     DescribeFeaturedResultsSetResponseTypeDef,
     DescribePrincipalMappingResponseTypeDef,
     DocumentAttributeConditionOutputTypeDef,
     DocumentAttributeOutputTypeDef,
     DocumentAttributeTargetOutputTypeDef,
     DocumentAttributeValueCountPairTypeDef,
-    DocumentAttributeConditionTypeDef,
-    DocumentAttributeTargetTypeDef,
-    DocumentAttributeTypeDef,
     DocumentMetadataConfigurationOutputTypeDef,
     DocumentMetadataConfigurationTypeDef,
     DocumentRelevanceConfigurationTypeDef,
     S3DataSourceConfigurationOutputTypeDef,
     S3DataSourceConfigurationTypeDef,
     ExperienceEntitiesSummaryTypeDef,
     ExperienceConfigurationOutputTypeDef,
@@ -594,19 +594,17 @@
     GetSnapshotsResponseTypeDef,
     GroupMembersTypeDef,
     ListGroupsOlderThanOrderingIdResponseTypeDef,
     TextWithHighlightsTypeDef,
     ListIndicesResponseTypeDef,
     IndexStatisticsTypeDef,
     UserTokenConfigurationTypeDef,
-    ListDataSourceSyncJobsRequestRequestTypeDef,
     ListEntityPersonasResponseTypeDef,
     ListQuerySuggestionsBlockListsResponseTypeDef,
     ListThesauriResponseTypeDef,
-    SubmitFeedbackRequestRequestTypeDef,
     UrlsOutputTypeDef,
     UrlsTypeDef,
     SuggestionTextWithHighlightsTypeDef,
     TableRowTypeDef,
     DatabaseConfigurationOutputTypeDef,
     DatabaseConfigurationTypeDef,
     SalesforceKnowledgeArticleConfigurationOutputTypeDef,
@@ -615,71 +613,82 @@
     ServiceNowConfigurationTypeDef,
     GitHubConfigurationOutputTypeDef,
     GitHubConfigurationTypeDef,
     OneDriveConfigurationOutputTypeDef,
     OneDriveConfigurationTypeDef,
     DescribeQuerySuggestionsConfigResponseTypeDef,
     UpdateQuerySuggestionsConfigRequestRequestTypeDef,
+    SubmitFeedbackRequestRequestTypeDef,
+    DocumentAttributeConditionTypeDef,
+    DocumentAttributeTargetTypeDef,
+    DocumentAttributeTypeDef,
+    ListDataSourceSyncJobsRequestRequestTypeDef,
+    TimeRangeUnionTypeDef,
     ConfluenceConfigurationOutputTypeDef,
     ConfluenceConfigurationTypeDef,
     DescribeAccessControlConfigurationResponseTypeDef,
-    CreateAccessControlConfigurationRequestRequestTypeDef,
-    UpdateAccessControlConfigurationRequestRequestTypeDef,
+    HierarchicalPrincipalUnionTypeDef,
     CreateFeaturedResultsSetResponseTypeDef,
     UpdateFeaturedResultsSetResponseTypeDef,
     AttributeSuggestionsGetConfigTypeDef,
     ListDataSourceSyncJobsResponseTypeDef,
     ListExperiencesResponseTypeDef,
     HookConfigurationOutputTypeDef,
     RetrieveResultItemTypeDef,
     SourceDocumentTypeDef,
     InlineCustomDocumentEnrichmentConfigurationOutputTypeDef,
-    HookConfigurationTypeDef,
-    InlineCustomDocumentEnrichmentConfigurationTypeDef,
-    AttributeFilterTypeDef,
-    DocumentInfoTypeDef,
-    DocumentTypeDef,
+    DocumentMetadataConfigurationUnionTypeDef,
     QueryRequestRequestTypeDef,
     RetrieveRequestRequestTypeDef,
     ListExperienceEntitiesResponseTypeDef,
     DescribeExperienceResponseTypeDef,
     CreateExperienceRequestRequestTypeDef,
+    ExperienceConfigurationUnionTypeDef,
     UpdateExperienceRequestRequestTypeDef,
     PutPrincipalMappingRequestRequestTypeDef,
     AdditionalResultAttributeValueTypeDef,
     CreateIndexRequestRequestTypeDef,
     DescribeIndexResponseTypeDef,
-    UpdateIndexRequestRequestTypeDef,
     WebCrawlerConfigurationOutputTypeDef,
     WebCrawlerConfigurationTypeDef,
     SuggestionValueTypeDef,
     TableExcerptTypeDef,
     SalesforceConfigurationOutputTypeDef,
     SalesforceConfigurationTypeDef,
+    HookConfigurationTypeDef,
+    InlineCustomDocumentEnrichmentConfigurationTypeDef,
+    AttributeFilterTypeDef,
+    DocumentInfoTypeDef,
+    DocumentTypeDef,
+    CreateAccessControlConfigurationRequestRequestTypeDef,
+    UpdateAccessControlConfigurationRequestRequestTypeDef,
     GetQuerySuggestionsRequestRequestTypeDef,
     RetrieveResultTypeDef,
     CustomDocumentEnrichmentConfigurationOutputTypeDef,
-    CustomDocumentEnrichmentConfigurationTypeDef,
-    BatchGetDocumentStatusRequestRequestTypeDef,
+    UpdateIndexRequestRequestTypeDef,
     AdditionalResultAttributeTypeDef,
     SuggestionTypeDef,
     DataSourceConfigurationOutputTypeDef,
     DataSourceConfigurationTypeDef,
-    BatchPutDocumentRequestRequestTypeDef,
+    CustomDocumentEnrichmentConfigurationTypeDef,
+    BatchGetDocumentStatusRequestRequestTypeDef,
     FeaturedResultsItemTypeDef,
     QueryResultItemTypeDef,
     GetQuerySuggestionsResponseTypeDef,
     DescribeDataSourceResponseTypeDef,
+    DataSourceConfigurationUnionTypeDef,
+    BatchPutDocumentRequestRequestTypeDef,
     CreateDataSourceRequestRequestTypeDef,
+    CustomDocumentEnrichmentConfigurationUnionTypeDef,
     UpdateDataSourceRequestRequestTypeDef,
     QueryResultTypeDef,
 )
 
 
-def get_structure() -> AccessControlConfigurationSummaryTypeDef:
+def get_value() -> AccessControlConfigurationSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kendra-1.28.15.post1/README.md` & `mypy-boto3-kendra-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kendra.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kendra)](https://pepy.tech/project/mypy-boto3-kendra)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.kendra 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
+[boto3.kendra 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
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
 [mypy-boto3-kendra docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/).
 
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
@@ -315,20 +315,20 @@
 )
 
 
 def check_value(value: AdditionalResultAttributeValueTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kendra.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kendra.type_defs import (
     AccessControlConfigurationSummaryTypeDef,
     AccessControlListConfigurationTypeDef,
     AclConfigurationTypeDef,
     DataSourceToIndexFieldMappingTypeDef,
@@ -344,17 +344,18 @@
     DataSourceSyncJobMetricTargetTypeDef,
     BatchDeleteDocumentResponseFailedDocumentTypeDef,
     BatchDeleteFeaturedResultsSetErrorTypeDef,
     BatchDeleteFeaturedResultsSetRequestRequestTypeDef,
     BatchGetDocumentStatusResponseErrorTypeDef,
     StatusTypeDef,
     BatchPutDocumentResponseFailedDocumentTypeDef,
+    BlobTypeDef,
     CapacityUnitsConfigurationTypeDef,
     ClearQuerySuggestionsRequestRequestTypeDef,
-    ClickFeedbackTypeDef,
+    TimestampTypeDef,
     ConfluenceAttachmentToIndexFieldMappingTypeDef,
     ConfluenceBlogToIndexFieldMappingTypeDef,
     ProxyConfigurationTypeDef,
     ConfluencePageToIndexFieldMappingTypeDef,
     ConfluenceSpaceToIndexFieldMappingTypeDef,
     ConnectionConfigurationTypeDef,
     ContentSourceConfigurationOutputTypeDef,
@@ -391,15 +392,14 @@
     DescribePrincipalMappingRequestRequestTypeDef,
     GroupOrderingIdSummaryTypeDef,
     DescribeQuerySuggestionsBlockListRequestRequestTypeDef,
     DescribeQuerySuggestionsConfigRequestRequestTypeDef,
     DescribeThesaurusRequestRequestTypeDef,
     DisassociatePersonasFromEntitiesRequestRequestTypeDef,
     DocumentAttributeValueOutputTypeDef,
-    DocumentAttributeValueTypeDef,
     RelevanceOutputTypeDef,
     SearchTypeDef,
     RelevanceTypeDef,
     DocumentsMetadataConfigurationTypeDef,
     EntityDisplayDataTypeDef,
     UserIdentityConfigurationTypeDef,
     FacetResultTypeDef,
@@ -416,15 +416,14 @@
     GroupSummaryTypeDef,
     HighlightTypeDef,
     IndexConfigurationSummaryTypeDef,
     TextDocumentStatisticsTypeDef,
     JsonTokenTypeConfigurationTypeDef,
     JwtTokenTypeConfigurationTypeDef,
     ListAccessControlConfigurationsRequestRequestTypeDef,
-    TimeRangeTypeDef,
     ListDataSourcesRequestRequestTypeDef,
     ListEntityPersonasRequestRequestTypeDef,
     PersonasSummaryTypeDef,
     ListExperienceEntitiesRequestRequestTypeDef,
     ListExperiencesRequestRequestTypeDef,
     ListFaqsRequestRequestTypeDef,
     ListFeaturedResultsSetsRequestRequestTypeDef,
@@ -478,14 +477,15 @@
     OnPremiseConfigurationTypeDef,
     OneDriveUsersOutputTypeDef,
     OneDriveUsersTypeDef,
     UpdateQuerySuggestionsBlockListRequestRequestTypeDef,
     UpdateThesaurusRequestRequestTypeDef,
     AlfrescoConfigurationTypeDef,
     BoxConfigurationTypeDef,
+    DataSourceVpcConfigurationUnionTypeDef,
     FsxConfigurationTypeDef,
     JiraConfigurationTypeDef,
     QuipConfigurationTypeDef,
     SlackConfigurationTypeDef,
     AssociateEntitiesToExperienceRequestRequestTypeDef,
     DisassociateEntitiesFromExperienceRequestRequestTypeDef,
     AssociateEntitiesToExperienceResponseTypeDef,
@@ -511,14 +511,17 @@
     AuthenticationConfigurationOutputTypeDef,
     AuthenticationConfigurationTypeDef,
     BatchDeleteDocumentRequestRequestTypeDef,
     BatchDeleteDocumentResponseTypeDef,
     BatchDeleteFeaturedResultsSetResponseTypeDef,
     BatchGetDocumentStatusResponseTypeDef,
     BatchPutDocumentResponseTypeDef,
+    ClickFeedbackTypeDef,
+    DocumentAttributeValueTypeDef,
+    TimeRangeTypeDef,
     ConfluenceAttachmentConfigurationOutputTypeDef,
     ConfluenceAttachmentConfigurationTypeDef,
     ConfluenceBlogConfigurationOutputTypeDef,
     ConfluenceBlogConfigurationTypeDef,
     SharePointConfigurationOutputTypeDef,
     SharePointConfigurationTypeDef,
     ConfluencePageConfigurationOutputTypeDef,
@@ -542,17 +545,14 @@
     ExperiencesSummaryTypeDef,
     DescribeFeaturedResultsSetResponseTypeDef,
     DescribePrincipalMappingResponseTypeDef,
     DocumentAttributeConditionOutputTypeDef,
     DocumentAttributeOutputTypeDef,
     DocumentAttributeTargetOutputTypeDef,
     DocumentAttributeValueCountPairTypeDef,
-    DocumentAttributeConditionTypeDef,
-    DocumentAttributeTargetTypeDef,
-    DocumentAttributeTypeDef,
     DocumentMetadataConfigurationOutputTypeDef,
     DocumentMetadataConfigurationTypeDef,
     DocumentRelevanceConfigurationTypeDef,
     S3DataSourceConfigurationOutputTypeDef,
     S3DataSourceConfigurationTypeDef,
     ExperienceEntitiesSummaryTypeDef,
     ExperienceConfigurationOutputTypeDef,
@@ -562,19 +562,17 @@
     GetSnapshotsResponseTypeDef,
     GroupMembersTypeDef,
     ListGroupsOlderThanOrderingIdResponseTypeDef,
     TextWithHighlightsTypeDef,
     ListIndicesResponseTypeDef,
     IndexStatisticsTypeDef,
     UserTokenConfigurationTypeDef,
-    ListDataSourceSyncJobsRequestRequestTypeDef,
     ListEntityPersonasResponseTypeDef,
     ListQuerySuggestionsBlockListsResponseTypeDef,
     ListThesauriResponseTypeDef,
-    SubmitFeedbackRequestRequestTypeDef,
     UrlsOutputTypeDef,
     UrlsTypeDef,
     SuggestionTextWithHighlightsTypeDef,
     TableRowTypeDef,
     DatabaseConfigurationOutputTypeDef,
     DatabaseConfigurationTypeDef,
     SalesforceKnowledgeArticleConfigurationOutputTypeDef,
@@ -583,71 +581,82 @@
     ServiceNowConfigurationTypeDef,
     GitHubConfigurationOutputTypeDef,
     GitHubConfigurationTypeDef,
     OneDriveConfigurationOutputTypeDef,
     OneDriveConfigurationTypeDef,
     DescribeQuerySuggestionsConfigResponseTypeDef,
     UpdateQuerySuggestionsConfigRequestRequestTypeDef,
+    SubmitFeedbackRequestRequestTypeDef,
+    DocumentAttributeConditionTypeDef,
+    DocumentAttributeTargetTypeDef,
+    DocumentAttributeTypeDef,
+    ListDataSourceSyncJobsRequestRequestTypeDef,
+    TimeRangeUnionTypeDef,
     ConfluenceConfigurationOutputTypeDef,
     ConfluenceConfigurationTypeDef,
     DescribeAccessControlConfigurationResponseTypeDef,
-    CreateAccessControlConfigurationRequestRequestTypeDef,
-    UpdateAccessControlConfigurationRequestRequestTypeDef,
+    HierarchicalPrincipalUnionTypeDef,
     CreateFeaturedResultsSetResponseTypeDef,
     UpdateFeaturedResultsSetResponseTypeDef,
     AttributeSuggestionsGetConfigTypeDef,
     ListDataSourceSyncJobsResponseTypeDef,
     ListExperiencesResponseTypeDef,
     HookConfigurationOutputTypeDef,
     RetrieveResultItemTypeDef,
     SourceDocumentTypeDef,
     InlineCustomDocumentEnrichmentConfigurationOutputTypeDef,
-    HookConfigurationTypeDef,
-    InlineCustomDocumentEnrichmentConfigurationTypeDef,
-    AttributeFilterTypeDef,
-    DocumentInfoTypeDef,
-    DocumentTypeDef,
+    DocumentMetadataConfigurationUnionTypeDef,
     QueryRequestRequestTypeDef,
     RetrieveRequestRequestTypeDef,
     ListExperienceEntitiesResponseTypeDef,
     DescribeExperienceResponseTypeDef,
     CreateExperienceRequestRequestTypeDef,
+    ExperienceConfigurationUnionTypeDef,
     UpdateExperienceRequestRequestTypeDef,
     PutPrincipalMappingRequestRequestTypeDef,
     AdditionalResultAttributeValueTypeDef,
     CreateIndexRequestRequestTypeDef,
     DescribeIndexResponseTypeDef,
-    UpdateIndexRequestRequestTypeDef,
     WebCrawlerConfigurationOutputTypeDef,
     WebCrawlerConfigurationTypeDef,
     SuggestionValueTypeDef,
     TableExcerptTypeDef,
     SalesforceConfigurationOutputTypeDef,
     SalesforceConfigurationTypeDef,
+    HookConfigurationTypeDef,
+    InlineCustomDocumentEnrichmentConfigurationTypeDef,
+    AttributeFilterTypeDef,
+    DocumentInfoTypeDef,
+    DocumentTypeDef,
+    CreateAccessControlConfigurationRequestRequestTypeDef,
+    UpdateAccessControlConfigurationRequestRequestTypeDef,
     GetQuerySuggestionsRequestRequestTypeDef,
     RetrieveResultTypeDef,
     CustomDocumentEnrichmentConfigurationOutputTypeDef,
-    CustomDocumentEnrichmentConfigurationTypeDef,
-    BatchGetDocumentStatusRequestRequestTypeDef,
+    UpdateIndexRequestRequestTypeDef,
     AdditionalResultAttributeTypeDef,
     SuggestionTypeDef,
     DataSourceConfigurationOutputTypeDef,
     DataSourceConfigurationTypeDef,
-    BatchPutDocumentRequestRequestTypeDef,
+    CustomDocumentEnrichmentConfigurationTypeDef,
+    BatchGetDocumentStatusRequestRequestTypeDef,
     FeaturedResultsItemTypeDef,
     QueryResultItemTypeDef,
     GetQuerySuggestionsResponseTypeDef,
     DescribeDataSourceResponseTypeDef,
+    DataSourceConfigurationUnionTypeDef,
+    BatchPutDocumentRequestRequestTypeDef,
     CreateDataSourceRequestRequestTypeDef,
+    CustomDocumentEnrichmentConfigurationUnionTypeDef,
     UpdateDataSourceRequestRequestTypeDef,
     QueryResultTypeDef,
 )
 
 
-def get_structure() -> AccessControlConfigurationSummaryTypeDef:
+def get_value() -> AccessControlConfigurationSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/__main__.py` & `mypy-boto3-kendra-1.28.16/mypy_boto3_kendra/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.kendra 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.kendra 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra\nOther"
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

### Comparing `mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/client.py` & `mypy-boto3-kendra-1.28.16/mypy_boto3_kendra/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_kendra.client import kendraClient
 
     session = Session()
     client: kendraClient = session.client("kendra")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DataSourceSyncJobStatusType,
     DataSourceTypeType,
     FaqFileFormatType,
@@ -46,50 +46,44 @@
     CreateDataSourceResponseTypeDef,
     CreateExperienceResponseTypeDef,
     CreateFaqResponseTypeDef,
     CreateFeaturedResultsSetResponseTypeDef,
     CreateIndexResponseTypeDef,
     CreateQuerySuggestionsBlockListResponseTypeDef,
     CreateThesaurusResponseTypeDef,
-    CustomDocumentEnrichmentConfigurationOutputTypeDef,
-    CustomDocumentEnrichmentConfigurationTypeDef,
-    DataSourceConfigurationOutputTypeDef,
-    DataSourceConfigurationTypeDef,
+    CustomDocumentEnrichmentConfigurationUnionTypeDef,
+    DataSourceConfigurationUnionTypeDef,
     DataSourceSyncJobMetricTargetTypeDef,
-    DataSourceVpcConfigurationOutputTypeDef,
-    DataSourceVpcConfigurationTypeDef,
+    DataSourceVpcConfigurationUnionTypeDef,
     DescribeAccessControlConfigurationResponseTypeDef,
     DescribeDataSourceResponseTypeDef,
     DescribeExperienceResponseTypeDef,
     DescribeFaqResponseTypeDef,
     DescribeFeaturedResultsSetResponseTypeDef,
     DescribeIndexResponseTypeDef,
     DescribePrincipalMappingResponseTypeDef,
     DescribeQuerySuggestionsBlockListResponseTypeDef,
     DescribeQuerySuggestionsConfigResponseTypeDef,
     DescribeThesaurusResponseTypeDef,
     DisassociateEntitiesFromExperienceResponseTypeDef,
     DisassociatePersonasFromEntitiesResponseTypeDef,
     DocumentInfoTypeDef,
-    DocumentMetadataConfigurationOutputTypeDef,
-    DocumentMetadataConfigurationTypeDef,
+    DocumentMetadataConfigurationUnionTypeDef,
     DocumentRelevanceConfigurationTypeDef,
     DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
     EntityConfigurationTypeDef,
     EntityPersonaConfigurationTypeDef,
-    ExperienceConfigurationOutputTypeDef,
-    ExperienceConfigurationTypeDef,
+    ExperienceConfigurationUnionTypeDef,
     FacetTypeDef,
     FeaturedDocumentTypeDef,
     GetQuerySuggestionsResponseTypeDef,
     GetSnapshotsResponseTypeDef,
     GroupMembersTypeDef,
-    HierarchicalPrincipalOutputTypeDef,
-    HierarchicalPrincipalTypeDef,
+    HierarchicalPrincipalUnionTypeDef,
     ListAccessControlConfigurationsResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     ListDataSourceSyncJobsResponseTypeDef,
     ListEntityPersonasResponseTypeDef,
     ListExperienceEntitiesResponseTypeDef,
     ListExperiencesResponseTypeDef,
     ListFaqsResponseTypeDef,
@@ -105,16 +99,15 @@
     RetrieveResultTypeDef,
     S3PathTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     SortingConfigurationTypeDef,
     SpellCorrectionConfigurationTypeDef,
     StartDataSourceSyncJobResponseTypeDef,
     TagTypeDef,
-    TimeRangeOutputTypeDef,
-    TimeRangeTypeDef,
+    TimeRangeUnionTypeDef,
     UpdateFeaturedResultsSetResponseTypeDef,
     UserContextTypeDef,
     UserGroupResolutionConfigurationTypeDef,
     UserTokenConfigurationTypeDef,
 )
 
 __all__ = ("kendraClient",)
@@ -221,18 +214,15 @@
 
     def batch_put_document(
         self,
         *,
         IndexId: str,
         Documents: Sequence[DocumentTypeDef],
         RoleArn: str = ...,
-        CustomDocumentEnrichmentConfiguration: Union[
-            CustomDocumentEnrichmentConfigurationTypeDef,
-            CustomDocumentEnrichmentConfigurationOutputTypeDef,
-        ] = ...
+        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationUnionTypeDef = ...
     ) -> BatchPutDocumentResponseTypeDef:
         """
         Adds one or more documents to an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.batch_put_document)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#batch_put_document)
         """
@@ -264,17 +254,15 @@
     def create_access_control_configuration(
         self,
         *,
         IndexId: str,
         Name: str,
         Description: str = ...,
         AccessControlList: Sequence[PrincipalTypeDef] = ...,
-        HierarchicalAccessControlList: Sequence[
-            Union[HierarchicalPrincipalTypeDef, HierarchicalPrincipalOutputTypeDef]
-        ] = ...,
+        HierarchicalAccessControlList: Sequence[HierarchicalPrincipalUnionTypeDef] = ...,
         ClientToken: str = ...
     ) -> CreateAccessControlConfigurationResponseTypeDef:
         """
         Creates an access configuration for your documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_access_control_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_access_control_configuration)
@@ -282,30 +270,23 @@
 
     def create_data_source(
         self,
         *,
         Name: str,
         IndexId: str,
         Type: DataSourceTypeType,
-        Configuration: Union[
-            DataSourceConfigurationTypeDef, DataSourceConfigurationOutputTypeDef
-        ] = ...,
-        VpcConfiguration: Union[
-            DataSourceVpcConfigurationTypeDef, DataSourceVpcConfigurationOutputTypeDef
-        ] = ...,
+        Configuration: DataSourceConfigurationUnionTypeDef = ...,
+        VpcConfiguration: DataSourceVpcConfigurationUnionTypeDef = ...,
         Description: str = ...,
         Schedule: str = ...,
         RoleArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientToken: str = ...,
         LanguageCode: str = ...,
-        CustomDocumentEnrichmentConfiguration: Union[
-            CustomDocumentEnrichmentConfigurationTypeDef,
-            CustomDocumentEnrichmentConfigurationOutputTypeDef,
-        ] = ...
+        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationUnionTypeDef = ...
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a data source connector that you want to use with an Amazon Kendra
         index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_data_source)
@@ -313,17 +294,15 @@
 
     def create_experience(
         self,
         *,
         Name: str,
         IndexId: str,
         RoleArn: str = ...,
-        Configuration: Union[
-            ExperienceConfigurationTypeDef, ExperienceConfigurationOutputTypeDef
-        ] = ...,
+        Configuration: ExperienceConfigurationUnionTypeDef = ...,
         Description: str = ...,
         ClientToken: str = ...
     ) -> CreateExperienceResponseTypeDef:
         """
         Creates an Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_experience)
@@ -672,15 +651,15 @@
     def list_data_source_sync_jobs(
         self,
         *,
         Id: str,
         IndexId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        StartTimeFilter: Union[TimeRangeTypeDef, TimeRangeOutputTypeDef] = ...,
+        StartTimeFilter: TimeRangeUnionTypeDef = ...,
         StatusFilter: DataSourceSyncJobStatusType = ...
     ) -> ListDataSourceSyncJobsResponseTypeDef:
         """
         Gets statistics about synchronizing a data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_data_source_sync_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_data_source_sync_jobs)
@@ -922,45 +901,36 @@
         self,
         *,
         IndexId: str,
         Id: str,
         Name: str = ...,
         Description: str = ...,
         AccessControlList: Sequence[PrincipalTypeDef] = ...,
-        HierarchicalAccessControlList: Sequence[
-            Union[HierarchicalPrincipalTypeDef, HierarchicalPrincipalOutputTypeDef]
-        ] = ...
+        HierarchicalAccessControlList: Sequence[HierarchicalPrincipalUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Updates an access control configuration for your documents in an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_access_control_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_access_control_configuration)
         """
 
     def update_data_source(
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
-        Configuration: Union[
-            DataSourceConfigurationTypeDef, DataSourceConfigurationOutputTypeDef
-        ] = ...,
-        VpcConfiguration: Union[
-            DataSourceVpcConfigurationTypeDef, DataSourceVpcConfigurationOutputTypeDef
-        ] = ...,
+        Configuration: DataSourceConfigurationUnionTypeDef = ...,
+        VpcConfiguration: DataSourceVpcConfigurationUnionTypeDef = ...,
         Description: str = ...,
         Schedule: str = ...,
         RoleArn: str = ...,
         LanguageCode: str = ...,
-        CustomDocumentEnrichmentConfiguration: Union[
-            CustomDocumentEnrichmentConfigurationTypeDef,
-            CustomDocumentEnrichmentConfigurationOutputTypeDef,
-        ] = ...
+        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an existing Amazon Kendra data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_data_source)
         """
@@ -968,17 +938,15 @@
     def update_experience(
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
         RoleArn: str = ...,
-        Configuration: Union[
-            ExperienceConfigurationTypeDef, ExperienceConfigurationOutputTypeDef
-        ] = ...,
+        Configuration: ExperienceConfigurationUnionTypeDef = ...,
         Description: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates your Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_experience)
@@ -1006,15 +974,15 @@
         self,
         *,
         Id: str,
         Name: str = ...,
         RoleArn: str = ...,
         Description: str = ...,
         DocumentMetadataConfigurationUpdates: Sequence[
-            Union[DocumentMetadataConfigurationTypeDef, DocumentMetadataConfigurationOutputTypeDef]
+            DocumentMetadataConfigurationUnionTypeDef
         ] = ...,
         CapacityUnits: CapacityUnitsConfigurationTypeDef = ...,
         UserTokenConfigurations: Sequence[UserTokenConfigurationTypeDef] = ...,
         UserContextPolicy: UserContextPolicyType = ...,
         UserGroupResolutionConfiguration: UserGroupResolutionConfigurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
```

### Comparing `mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/client.pyi` & `mypy-boto3-kendra-1.28.16/mypy_boto3_kendra/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_kendra.client import kendraClient
 
     session = Session()
     client: kendraClient = session.client("kendra")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DataSourceSyncJobStatusType,
     DataSourceTypeType,
     FaqFileFormatType,
@@ -46,50 +46,44 @@
     CreateDataSourceResponseTypeDef,
     CreateExperienceResponseTypeDef,
     CreateFaqResponseTypeDef,
     CreateFeaturedResultsSetResponseTypeDef,
     CreateIndexResponseTypeDef,
     CreateQuerySuggestionsBlockListResponseTypeDef,
     CreateThesaurusResponseTypeDef,
-    CustomDocumentEnrichmentConfigurationOutputTypeDef,
-    CustomDocumentEnrichmentConfigurationTypeDef,
-    DataSourceConfigurationOutputTypeDef,
-    DataSourceConfigurationTypeDef,
+    CustomDocumentEnrichmentConfigurationUnionTypeDef,
+    DataSourceConfigurationUnionTypeDef,
     DataSourceSyncJobMetricTargetTypeDef,
-    DataSourceVpcConfigurationOutputTypeDef,
-    DataSourceVpcConfigurationTypeDef,
+    DataSourceVpcConfigurationUnionTypeDef,
     DescribeAccessControlConfigurationResponseTypeDef,
     DescribeDataSourceResponseTypeDef,
     DescribeExperienceResponseTypeDef,
     DescribeFaqResponseTypeDef,
     DescribeFeaturedResultsSetResponseTypeDef,
     DescribeIndexResponseTypeDef,
     DescribePrincipalMappingResponseTypeDef,
     DescribeQuerySuggestionsBlockListResponseTypeDef,
     DescribeQuerySuggestionsConfigResponseTypeDef,
     DescribeThesaurusResponseTypeDef,
     DisassociateEntitiesFromExperienceResponseTypeDef,
     DisassociatePersonasFromEntitiesResponseTypeDef,
     DocumentInfoTypeDef,
-    DocumentMetadataConfigurationOutputTypeDef,
-    DocumentMetadataConfigurationTypeDef,
+    DocumentMetadataConfigurationUnionTypeDef,
     DocumentRelevanceConfigurationTypeDef,
     DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
     EntityConfigurationTypeDef,
     EntityPersonaConfigurationTypeDef,
-    ExperienceConfigurationOutputTypeDef,
-    ExperienceConfigurationTypeDef,
+    ExperienceConfigurationUnionTypeDef,
     FacetTypeDef,
     FeaturedDocumentTypeDef,
     GetQuerySuggestionsResponseTypeDef,
     GetSnapshotsResponseTypeDef,
     GroupMembersTypeDef,
-    HierarchicalPrincipalOutputTypeDef,
-    HierarchicalPrincipalTypeDef,
+    HierarchicalPrincipalUnionTypeDef,
     ListAccessControlConfigurationsResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     ListDataSourceSyncJobsResponseTypeDef,
     ListEntityPersonasResponseTypeDef,
     ListExperienceEntitiesResponseTypeDef,
     ListExperiencesResponseTypeDef,
     ListFaqsResponseTypeDef,
@@ -105,16 +99,15 @@
     RetrieveResultTypeDef,
     S3PathTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     SortingConfigurationTypeDef,
     SpellCorrectionConfigurationTypeDef,
     StartDataSourceSyncJobResponseTypeDef,
     TagTypeDef,
-    TimeRangeOutputTypeDef,
-    TimeRangeTypeDef,
+    TimeRangeUnionTypeDef,
     UpdateFeaturedResultsSetResponseTypeDef,
     UserContextTypeDef,
     UserGroupResolutionConfigurationTypeDef,
     UserTokenConfigurationTypeDef,
 )
 
 __all__ = ("kendraClient",)
@@ -212,18 +205,15 @@
         """
     def batch_put_document(
         self,
         *,
         IndexId: str,
         Documents: Sequence[DocumentTypeDef],
         RoleArn: str = ...,
-        CustomDocumentEnrichmentConfiguration: Union[
-            CustomDocumentEnrichmentConfigurationTypeDef,
-            CustomDocumentEnrichmentConfigurationOutputTypeDef,
-        ] = ...
+        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationUnionTypeDef = ...
     ) -> BatchPutDocumentResponseTypeDef:
         """
         Adds one or more documents to an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.batch_put_document)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#batch_put_document)
         """
@@ -251,64 +241,53 @@
     def create_access_control_configuration(
         self,
         *,
         IndexId: str,
         Name: str,
         Description: str = ...,
         AccessControlList: Sequence[PrincipalTypeDef] = ...,
-        HierarchicalAccessControlList: Sequence[
-            Union[HierarchicalPrincipalTypeDef, HierarchicalPrincipalOutputTypeDef]
-        ] = ...,
+        HierarchicalAccessControlList: Sequence[HierarchicalPrincipalUnionTypeDef] = ...,
         ClientToken: str = ...
     ) -> CreateAccessControlConfigurationResponseTypeDef:
         """
         Creates an access configuration for your documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_access_control_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_access_control_configuration)
         """
     def create_data_source(
         self,
         *,
         Name: str,
         IndexId: str,
         Type: DataSourceTypeType,
-        Configuration: Union[
-            DataSourceConfigurationTypeDef, DataSourceConfigurationOutputTypeDef
-        ] = ...,
-        VpcConfiguration: Union[
-            DataSourceVpcConfigurationTypeDef, DataSourceVpcConfigurationOutputTypeDef
-        ] = ...,
+        Configuration: DataSourceConfigurationUnionTypeDef = ...,
+        VpcConfiguration: DataSourceVpcConfigurationUnionTypeDef = ...,
         Description: str = ...,
         Schedule: str = ...,
         RoleArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientToken: str = ...,
         LanguageCode: str = ...,
-        CustomDocumentEnrichmentConfiguration: Union[
-            CustomDocumentEnrichmentConfigurationTypeDef,
-            CustomDocumentEnrichmentConfigurationOutputTypeDef,
-        ] = ...
+        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationUnionTypeDef = ...
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a data source connector that you want to use with an Amazon Kendra
         index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_data_source)
         """
     def create_experience(
         self,
         *,
         Name: str,
         IndexId: str,
         RoleArn: str = ...,
-        Configuration: Union[
-            ExperienceConfigurationTypeDef, ExperienceConfigurationOutputTypeDef
-        ] = ...,
+        Configuration: ExperienceConfigurationUnionTypeDef = ...,
         Description: str = ...,
         ClientToken: str = ...
     ) -> CreateExperienceResponseTypeDef:
         """
         Creates an Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_experience)
@@ -627,15 +606,15 @@
     def list_data_source_sync_jobs(
         self,
         *,
         Id: str,
         IndexId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        StartTimeFilter: Union[TimeRangeTypeDef, TimeRangeOutputTypeDef] = ...,
+        StartTimeFilter: TimeRangeUnionTypeDef = ...,
         StatusFilter: DataSourceSyncJobStatusType = ...
     ) -> ListDataSourceSyncJobsResponseTypeDef:
         """
         Gets statistics about synchronizing a data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_data_source_sync_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_data_source_sync_jobs)
@@ -857,61 +836,50 @@
         self,
         *,
         IndexId: str,
         Id: str,
         Name: str = ...,
         Description: str = ...,
         AccessControlList: Sequence[PrincipalTypeDef] = ...,
-        HierarchicalAccessControlList: Sequence[
-            Union[HierarchicalPrincipalTypeDef, HierarchicalPrincipalOutputTypeDef]
-        ] = ...
+        HierarchicalAccessControlList: Sequence[HierarchicalPrincipalUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Updates an access control configuration for your documents in an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_access_control_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_access_control_configuration)
         """
     def update_data_source(
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
-        Configuration: Union[
-            DataSourceConfigurationTypeDef, DataSourceConfigurationOutputTypeDef
-        ] = ...,
-        VpcConfiguration: Union[
-            DataSourceVpcConfigurationTypeDef, DataSourceVpcConfigurationOutputTypeDef
-        ] = ...,
+        Configuration: DataSourceConfigurationUnionTypeDef = ...,
+        VpcConfiguration: DataSourceVpcConfigurationUnionTypeDef = ...,
         Description: str = ...,
         Schedule: str = ...,
         RoleArn: str = ...,
         LanguageCode: str = ...,
-        CustomDocumentEnrichmentConfiguration: Union[
-            CustomDocumentEnrichmentConfigurationTypeDef,
-            CustomDocumentEnrichmentConfigurationOutputTypeDef,
-        ] = ...
+        CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an existing Amazon Kendra data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_data_source)
         """
     def update_experience(
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
         RoleArn: str = ...,
-        Configuration: Union[
-            ExperienceConfigurationTypeDef, ExperienceConfigurationOutputTypeDef
-        ] = ...,
+        Configuration: ExperienceConfigurationUnionTypeDef = ...,
         Description: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates your Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_experience)
@@ -937,15 +905,15 @@
         self,
         *,
         Id: str,
         Name: str = ...,
         RoleArn: str = ...,
         Description: str = ...,
         DocumentMetadataConfigurationUpdates: Sequence[
-            Union[DocumentMetadataConfigurationTypeDef, DocumentMetadataConfigurationOutputTypeDef]
+            DocumentMetadataConfigurationUnionTypeDef
         ] = ...,
         CapacityUnits: CapacityUnitsConfigurationTypeDef = ...,
         UserTokenConfigurations: Sequence[UserTokenConfigurationTypeDef] = ...,
         UserContextPolicy: UserContextPolicyType = ...,
         UserGroupResolutionConfiguration: UserGroupResolutionConfigurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
```

### Comparing `mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/literals.py` & `mypy-boto3-kendra-1.28.16/mypy_boto3_kendra/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/literals.pyi` & `mypy-boto3-kendra-1.28.16/mypy_boto3_kendra/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/type_defs.py` & `mypy-boto3-kendra-1.28.16/mypy_boto3_kendra/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_kendra.type_defs import AccessControlConfigurationSummaryTypeDef
 
-    data: AccessControlConfigurationSummaryTypeDef = {...}
+    data: AccessControlConfigurationSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -104,17 +104,18 @@
     "DataSourceSyncJobMetricTargetTypeDef",
     "BatchDeleteDocumentResponseFailedDocumentTypeDef",
     "BatchDeleteFeaturedResultsSetErrorTypeDef",
     "BatchDeleteFeaturedResultsSetRequestRequestTypeDef",
     "BatchGetDocumentStatusResponseErrorTypeDef",
     "StatusTypeDef",
     "BatchPutDocumentResponseFailedDocumentTypeDef",
+    "BlobTypeDef",
     "CapacityUnitsConfigurationTypeDef",
     "ClearQuerySuggestionsRequestRequestTypeDef",
-    "ClickFeedbackTypeDef",
+    "TimestampTypeDef",
     "ConfluenceAttachmentToIndexFieldMappingTypeDef",
     "ConfluenceBlogToIndexFieldMappingTypeDef",
     "ProxyConfigurationTypeDef",
     "ConfluencePageToIndexFieldMappingTypeDef",
     "ConfluenceSpaceToIndexFieldMappingTypeDef",
     "ConnectionConfigurationTypeDef",
     "ContentSourceConfigurationOutputTypeDef",
@@ -151,15 +152,14 @@
     "DescribePrincipalMappingRequestRequestTypeDef",
     "GroupOrderingIdSummaryTypeDef",
     "DescribeQuerySuggestionsBlockListRequestRequestTypeDef",
     "DescribeQuerySuggestionsConfigRequestRequestTypeDef",
     "DescribeThesaurusRequestRequestTypeDef",
     "DisassociatePersonasFromEntitiesRequestRequestTypeDef",
     "DocumentAttributeValueOutputTypeDef",
-    "DocumentAttributeValueTypeDef",
     "RelevanceOutputTypeDef",
     "SearchTypeDef",
     "RelevanceTypeDef",
     "DocumentsMetadataConfigurationTypeDef",
     "EntityDisplayDataTypeDef",
     "UserIdentityConfigurationTypeDef",
     "FacetResultTypeDef",
@@ -176,15 +176,14 @@
     "GroupSummaryTypeDef",
     "HighlightTypeDef",
     "IndexConfigurationSummaryTypeDef",
     "TextDocumentStatisticsTypeDef",
     "JsonTokenTypeConfigurationTypeDef",
     "JwtTokenTypeConfigurationTypeDef",
     "ListAccessControlConfigurationsRequestRequestTypeDef",
-    "TimeRangeTypeDef",
     "ListDataSourcesRequestRequestTypeDef",
     "ListEntityPersonasRequestRequestTypeDef",
     "PersonasSummaryTypeDef",
     "ListExperienceEntitiesRequestRequestTypeDef",
     "ListExperiencesRequestRequestTypeDef",
     "ListFaqsRequestRequestTypeDef",
     "ListFeaturedResultsSetsRequestRequestTypeDef",
@@ -238,14 +237,15 @@
     "OnPremiseConfigurationTypeDef",
     "OneDriveUsersOutputTypeDef",
     "OneDriveUsersTypeDef",
     "UpdateQuerySuggestionsBlockListRequestRequestTypeDef",
     "UpdateThesaurusRequestRequestTypeDef",
     "AlfrescoConfigurationTypeDef",
     "BoxConfigurationTypeDef",
+    "DataSourceVpcConfigurationUnionTypeDef",
     "FsxConfigurationTypeDef",
     "JiraConfigurationTypeDef",
     "QuipConfigurationTypeDef",
     "SlackConfigurationTypeDef",
     "AssociateEntitiesToExperienceRequestRequestTypeDef",
     "DisassociateEntitiesFromExperienceRequestRequestTypeDef",
     "AssociateEntitiesToExperienceResponseTypeDef",
@@ -271,14 +271,17 @@
     "AuthenticationConfigurationOutputTypeDef",
     "AuthenticationConfigurationTypeDef",
     "BatchDeleteDocumentRequestRequestTypeDef",
     "BatchDeleteDocumentResponseTypeDef",
     "BatchDeleteFeaturedResultsSetResponseTypeDef",
     "BatchGetDocumentStatusResponseTypeDef",
     "BatchPutDocumentResponseTypeDef",
+    "ClickFeedbackTypeDef",
+    "DocumentAttributeValueTypeDef",
+    "TimeRangeTypeDef",
     "ConfluenceAttachmentConfigurationOutputTypeDef",
     "ConfluenceAttachmentConfigurationTypeDef",
     "ConfluenceBlogConfigurationOutputTypeDef",
     "ConfluenceBlogConfigurationTypeDef",
     "SharePointConfigurationOutputTypeDef",
     "SharePointConfigurationTypeDef",
     "ConfluencePageConfigurationOutputTypeDef",
@@ -302,17 +305,14 @@
     "ExperiencesSummaryTypeDef",
     "DescribeFeaturedResultsSetResponseTypeDef",
     "DescribePrincipalMappingResponseTypeDef",
     "DocumentAttributeConditionOutputTypeDef",
     "DocumentAttributeOutputTypeDef",
     "DocumentAttributeTargetOutputTypeDef",
     "DocumentAttributeValueCountPairTypeDef",
-    "DocumentAttributeConditionTypeDef",
-    "DocumentAttributeTargetTypeDef",
-    "DocumentAttributeTypeDef",
     "DocumentMetadataConfigurationOutputTypeDef",
     "DocumentMetadataConfigurationTypeDef",
     "DocumentRelevanceConfigurationTypeDef",
     "S3DataSourceConfigurationOutputTypeDef",
     "S3DataSourceConfigurationTypeDef",
     "ExperienceEntitiesSummaryTypeDef",
     "ExperienceConfigurationOutputTypeDef",
@@ -322,19 +322,17 @@
     "GetSnapshotsResponseTypeDef",
     "GroupMembersTypeDef",
     "ListGroupsOlderThanOrderingIdResponseTypeDef",
     "TextWithHighlightsTypeDef",
     "ListIndicesResponseTypeDef",
     "IndexStatisticsTypeDef",
     "UserTokenConfigurationTypeDef",
-    "ListDataSourceSyncJobsRequestRequestTypeDef",
     "ListEntityPersonasResponseTypeDef",
     "ListQuerySuggestionsBlockListsResponseTypeDef",
     "ListThesauriResponseTypeDef",
-    "SubmitFeedbackRequestRequestTypeDef",
     "UrlsOutputTypeDef",
     "UrlsTypeDef",
     "SuggestionTextWithHighlightsTypeDef",
     "TableRowTypeDef",
     "DatabaseConfigurationOutputTypeDef",
     "DatabaseConfigurationTypeDef",
     "SalesforceKnowledgeArticleConfigurationOutputTypeDef",
@@ -343,65 +341,76 @@
     "ServiceNowConfigurationTypeDef",
     "GitHubConfigurationOutputTypeDef",
     "GitHubConfigurationTypeDef",
     "OneDriveConfigurationOutputTypeDef",
     "OneDriveConfigurationTypeDef",
     "DescribeQuerySuggestionsConfigResponseTypeDef",
     "UpdateQuerySuggestionsConfigRequestRequestTypeDef",
+    "SubmitFeedbackRequestRequestTypeDef",
+    "DocumentAttributeConditionTypeDef",
+    "DocumentAttributeTargetTypeDef",
+    "DocumentAttributeTypeDef",
+    "ListDataSourceSyncJobsRequestRequestTypeDef",
+    "TimeRangeUnionTypeDef",
     "ConfluenceConfigurationOutputTypeDef",
     "ConfluenceConfigurationTypeDef",
     "DescribeAccessControlConfigurationResponseTypeDef",
-    "CreateAccessControlConfigurationRequestRequestTypeDef",
-    "UpdateAccessControlConfigurationRequestRequestTypeDef",
+    "HierarchicalPrincipalUnionTypeDef",
     "CreateFeaturedResultsSetResponseTypeDef",
     "UpdateFeaturedResultsSetResponseTypeDef",
     "AttributeSuggestionsGetConfigTypeDef",
     "ListDataSourceSyncJobsResponseTypeDef",
     "ListExperiencesResponseTypeDef",
     "HookConfigurationOutputTypeDef",
     "RetrieveResultItemTypeDef",
     "SourceDocumentTypeDef",
     "InlineCustomDocumentEnrichmentConfigurationOutputTypeDef",
-    "HookConfigurationTypeDef",
-    "InlineCustomDocumentEnrichmentConfigurationTypeDef",
-    "AttributeFilterTypeDef",
-    "DocumentInfoTypeDef",
-    "DocumentTypeDef",
+    "DocumentMetadataConfigurationUnionTypeDef",
     "QueryRequestRequestTypeDef",
     "RetrieveRequestRequestTypeDef",
     "ListExperienceEntitiesResponseTypeDef",
     "DescribeExperienceResponseTypeDef",
     "CreateExperienceRequestRequestTypeDef",
+    "ExperienceConfigurationUnionTypeDef",
     "UpdateExperienceRequestRequestTypeDef",
     "PutPrincipalMappingRequestRequestTypeDef",
     "AdditionalResultAttributeValueTypeDef",
     "CreateIndexRequestRequestTypeDef",
     "DescribeIndexResponseTypeDef",
-    "UpdateIndexRequestRequestTypeDef",
     "WebCrawlerConfigurationOutputTypeDef",
     "WebCrawlerConfigurationTypeDef",
     "SuggestionValueTypeDef",
     "TableExcerptTypeDef",
     "SalesforceConfigurationOutputTypeDef",
     "SalesforceConfigurationTypeDef",
+    "HookConfigurationTypeDef",
+    "InlineCustomDocumentEnrichmentConfigurationTypeDef",
+    "AttributeFilterTypeDef",
+    "DocumentInfoTypeDef",
+    "DocumentTypeDef",
+    "CreateAccessControlConfigurationRequestRequestTypeDef",
+    "UpdateAccessControlConfigurationRequestRequestTypeDef",
     "GetQuerySuggestionsRequestRequestTypeDef",
     "RetrieveResultTypeDef",
     "CustomDocumentEnrichmentConfigurationOutputTypeDef",
-    "CustomDocumentEnrichmentConfigurationTypeDef",
-    "BatchGetDocumentStatusRequestRequestTypeDef",
+    "UpdateIndexRequestRequestTypeDef",
     "AdditionalResultAttributeTypeDef",
     "SuggestionTypeDef",
     "DataSourceConfigurationOutputTypeDef",
     "DataSourceConfigurationTypeDef",
-    "BatchPutDocumentRequestRequestTypeDef",
+    "CustomDocumentEnrichmentConfigurationTypeDef",
+    "BatchGetDocumentStatusRequestRequestTypeDef",
     "FeaturedResultsItemTypeDef",
     "QueryResultItemTypeDef",
     "GetQuerySuggestionsResponseTypeDef",
     "DescribeDataSourceResponseTypeDef",
+    "DataSourceConfigurationUnionTypeDef",
+    "BatchPutDocumentRequestRequestTypeDef",
     "CreateDataSourceRequestRequestTypeDef",
+    "CustomDocumentEnrichmentConfigurationUnionTypeDef",
     "UpdateDataSourceRequestRequestTypeDef",
     "QueryResultTypeDef",
 )
 
 AccessControlConfigurationSummaryTypeDef = TypedDict(
     "AccessControlConfigurationSummaryTypeDef",
     {
@@ -599,14 +608,15 @@
         "Id": str,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CapacityUnitsConfigurationTypeDef = TypedDict(
     "CapacityUnitsConfigurationTypeDef",
     {
         "StorageCapacityUnits": int,
         "QueryCapacityUnits": int,
     },
 )
@@ -614,22 +624,15 @@
 ClearQuerySuggestionsRequestRequestTypeDef = TypedDict(
     "ClearQuerySuggestionsRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 
-ClickFeedbackTypeDef = TypedDict(
-    "ClickFeedbackTypeDef",
-    {
-        "ResultId": str,
-        "ClickTime": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 ConfluenceAttachmentToIndexFieldMappingTypeDef = TypedDict(
     "ConfluenceAttachmentToIndexFieldMappingTypeDef",
     {
         "DataSourceFieldName": ConfluenceAttachmentFieldNameType,
         "DateFieldFormat": str,
         "IndexFieldName": str,
     },
@@ -1067,25 +1070,14 @@
         "StringListValue": List[str],
         "LongValue": int,
         "DateValue": datetime,
     },
     total=False,
 )
 
-DocumentAttributeValueTypeDef = TypedDict(
-    "DocumentAttributeValueTypeDef",
-    {
-        "StringValue": str,
-        "StringListValue": Sequence[str],
-        "LongValue": int,
-        "DateValue": Union[datetime, str],
-    },
-    total=False,
-)
-
 RelevanceOutputTypeDef = TypedDict(
     "RelevanceOutputTypeDef",
     {
         "Freshness": bool,
         "Importance": int,
         "Duration": str,
         "RankOrder": OrderType,
@@ -1395,23 +1387,14 @@
 class ListAccessControlConfigurationsRequestRequestTypeDef(
     _RequiredListAccessControlConfigurationsRequestRequestTypeDef,
     _OptionalListAccessControlConfigurationsRequestRequestTypeDef,
 ):
     pass
 
 
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredListDataSourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSourcesRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalListDataSourcesRequestRequestTypeDef = TypedDict(
@@ -2594,14 +2577,17 @@
 )
 
 
 class BoxConfigurationTypeDef(_RequiredBoxConfigurationTypeDef, _OptionalBoxConfigurationTypeDef):
     pass
 
 
+DataSourceVpcConfigurationUnionTypeDef = Union[
+    DataSourceVpcConfigurationTypeDef, DataSourceVpcConfigurationOutputTypeDef
+]
 _RequiredFsxConfigurationTypeDef = TypedDict(
     "_RequiredFsxConfigurationTypeDef",
     {
         "FileSystemId": str,
         "FileSystemType": Literal["WINDOWS"],
         "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
@@ -3003,14 +2989,42 @@
     "BatchPutDocumentResponseTypeDef",
     {
         "FailedDocuments": List[BatchPutDocumentResponseFailedDocumentTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ClickFeedbackTypeDef = TypedDict(
+    "ClickFeedbackTypeDef",
+    {
+        "ResultId": str,
+        "ClickTime": TimestampTypeDef,
+    },
+)
+
+DocumentAttributeValueTypeDef = TypedDict(
+    "DocumentAttributeValueTypeDef",
+    {
+        "StringValue": str,
+        "StringListValue": Sequence[str],
+        "LongValue": int,
+        "DateValue": TimestampTypeDef,
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
 ConfluenceAttachmentConfigurationOutputTypeDef = TypedDict(
     "ConfluenceAttachmentConfigurationOutputTypeDef",
     {
         "CrawlAttachments": bool,
         "AttachmentFieldMappings": List[ConfluenceAttachmentToIndexFieldMappingTypeDef],
     },
     total=False,
@@ -3458,54 +3472,14 @@
         "DocumentAttributeValue": DocumentAttributeValueOutputTypeDef,
         "Count": int,
         "FacetResults": List[Dict[str, Any]],
     },
     total=False,
 )
 
-_RequiredDocumentAttributeConditionTypeDef = TypedDict(
-    "_RequiredDocumentAttributeConditionTypeDef",
-    {
-        "ConditionDocumentAttributeKey": str,
-        "Operator": ConditionOperatorType,
-    },
-)
-_OptionalDocumentAttributeConditionTypeDef = TypedDict(
-    "_OptionalDocumentAttributeConditionTypeDef",
-    {
-        "ConditionOnValue": DocumentAttributeValueTypeDef,
-    },
-    total=False,
-)
-
-
-class DocumentAttributeConditionTypeDef(
-    _RequiredDocumentAttributeConditionTypeDef, _OptionalDocumentAttributeConditionTypeDef
-):
-    pass
-
-
-DocumentAttributeTargetTypeDef = TypedDict(
-    "DocumentAttributeTargetTypeDef",
-    {
-        "TargetDocumentAttributeKey": str,
-        "TargetDocumentAttributeValueDeletion": bool,
-        "TargetDocumentAttributeValue": DocumentAttributeValueTypeDef,
-    },
-    total=False,
-)
-
-DocumentAttributeTypeDef = TypedDict(
-    "DocumentAttributeTypeDef",
-    {
-        "Key": str,
-        "Value": DocumentAttributeValueTypeDef,
-    },
-)
-
 _RequiredDocumentMetadataConfigurationOutputTypeDef = TypedDict(
     "_RequiredDocumentMetadataConfigurationOutputTypeDef",
     {
         "Name": str,
         "Type": DocumentAttributeValueTypeType,
     },
 )
@@ -3714,40 +3688,14 @@
     {
         "JwtTokenTypeConfiguration": JwtTokenTypeConfigurationTypeDef,
         "JsonTokenTypeConfiguration": JsonTokenTypeConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDataSourceSyncJobsRequestRequestTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-    },
-)
-_OptionalListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDataSourceSyncJobsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "StartTimeFilter": TimeRangeTypeDef,
-        "StatusFilter": DataSourceSyncJobStatusType,
-    },
-    total=False,
-)
-
-
-class ListDataSourceSyncJobsRequestRequestTypeDef(
-    _RequiredListDataSourceSyncJobsRequestRequestTypeDef,
-    _OptionalListDataSourceSyncJobsRequestRequestTypeDef,
-):
-    pass
-
-
 ListEntityPersonasResponseTypeDef = TypedDict(
     "ListEntityPersonasResponseTypeDef",
     {
         "SummaryItems": List[PersonasSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3767,37 +3715,14 @@
     {
         "NextToken": str,
         "ThesaurusSummaryItems": List[ThesaurusSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSubmitFeedbackRequestRequestTypeDef = TypedDict(
-    "_RequiredSubmitFeedbackRequestRequestTypeDef",
-    {
-        "IndexId": str,
-        "QueryId": str,
-    },
-)
-_OptionalSubmitFeedbackRequestRequestTypeDef = TypedDict(
-    "_OptionalSubmitFeedbackRequestRequestTypeDef",
-    {
-        "ClickFeedbackItems": Sequence[ClickFeedbackTypeDef],
-        "RelevanceFeedbackItems": Sequence[RelevanceFeedbackTypeDef],
-    },
-    total=False,
-)
-
-
-class SubmitFeedbackRequestRequestTypeDef(
-    _RequiredSubmitFeedbackRequestRequestTypeDef, _OptionalSubmitFeedbackRequestRequestTypeDef
-):
-    pass
-
-
 UrlsOutputTypeDef = TypedDict(
     "UrlsOutputTypeDef",
     {
         "SeedUrlConfiguration": SeedUrlConfigurationOutputTypeDef,
         "SiteMapsConfiguration": SiteMapsConfigurationOutputTypeDef,
     },
     total=False,
@@ -4179,14 +4104,104 @@
 class UpdateQuerySuggestionsConfigRequestRequestTypeDef(
     _RequiredUpdateQuerySuggestionsConfigRequestRequestTypeDef,
     _OptionalUpdateQuerySuggestionsConfigRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredSubmitFeedbackRequestRequestTypeDef = TypedDict(
+    "_RequiredSubmitFeedbackRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "QueryId": str,
+    },
+)
+_OptionalSubmitFeedbackRequestRequestTypeDef = TypedDict(
+    "_OptionalSubmitFeedbackRequestRequestTypeDef",
+    {
+        "ClickFeedbackItems": Sequence[ClickFeedbackTypeDef],
+        "RelevanceFeedbackItems": Sequence[RelevanceFeedbackTypeDef],
+    },
+    total=False,
+)
+
+
+class SubmitFeedbackRequestRequestTypeDef(
+    _RequiredSubmitFeedbackRequestRequestTypeDef, _OptionalSubmitFeedbackRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredDocumentAttributeConditionTypeDef = TypedDict(
+    "_RequiredDocumentAttributeConditionTypeDef",
+    {
+        "ConditionDocumentAttributeKey": str,
+        "Operator": ConditionOperatorType,
+    },
+)
+_OptionalDocumentAttributeConditionTypeDef = TypedDict(
+    "_OptionalDocumentAttributeConditionTypeDef",
+    {
+        "ConditionOnValue": DocumentAttributeValueTypeDef,
+    },
+    total=False,
+)
+
+
+class DocumentAttributeConditionTypeDef(
+    _RequiredDocumentAttributeConditionTypeDef, _OptionalDocumentAttributeConditionTypeDef
+):
+    pass
+
+
+DocumentAttributeTargetTypeDef = TypedDict(
+    "DocumentAttributeTargetTypeDef",
+    {
+        "TargetDocumentAttributeKey": str,
+        "TargetDocumentAttributeValueDeletion": bool,
+        "TargetDocumentAttributeValue": DocumentAttributeValueTypeDef,
+    },
+    total=False,
+)
+
+DocumentAttributeTypeDef = TypedDict(
+    "DocumentAttributeTypeDef",
+    {
+        "Key": str,
+        "Value": DocumentAttributeValueTypeDef,
+    },
+)
+
+_RequiredListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDataSourceSyncJobsRequestRequestTypeDef",
+    {
+        "Id": str,
+        "IndexId": str,
+    },
+)
+_OptionalListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDataSourceSyncJobsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "StartTimeFilter": TimeRangeTypeDef,
+        "StatusFilter": DataSourceSyncJobStatusType,
+    },
+    total=False,
+)
+
+
+class ListDataSourceSyncJobsRequestRequestTypeDef(
+    _RequiredListDataSourceSyncJobsRequestRequestTypeDef,
+    _OptionalListDataSourceSyncJobsRequestRequestTypeDef,
+):
+    pass
+
+
+TimeRangeUnionTypeDef = Union[TimeRangeTypeDef, TimeRangeOutputTypeDef]
 _RequiredConfluenceConfigurationOutputTypeDef = TypedDict(
     "_RequiredConfluenceConfigurationOutputTypeDef",
     {
         "ServerUrl": str,
         "SecretArn": str,
         "Version": ConfluenceVersionType,
     },
@@ -4253,70 +4268,17 @@
         "ErrorMessage": str,
         "AccessControlList": List[PrincipalTypeDef],
         "HierarchicalAccessControlList": List[HierarchicalPrincipalOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAccessControlConfigurationRequestRequestTypeDef",
-    {
-        "IndexId": str,
-        "Name": str,
-    },
-)
-_OptionalCreateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAccessControlConfigurationRequestRequestTypeDef",
-    {
-        "Description": str,
-        "AccessControlList": Sequence[PrincipalTypeDef],
-        "HierarchicalAccessControlList": Sequence[
-            Union[HierarchicalPrincipalTypeDef, HierarchicalPrincipalOutputTypeDef]
-        ],
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-
-class CreateAccessControlConfigurationRequestRequestTypeDef(
-    _RequiredCreateAccessControlConfigurationRequestRequestTypeDef,
-    _OptionalCreateAccessControlConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAccessControlConfigurationRequestRequestTypeDef",
-    {
-        "IndexId": str,
-        "Id": str,
-    },
-)
-_OptionalUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAccessControlConfigurationRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "AccessControlList": Sequence[PrincipalTypeDef],
-        "HierarchicalAccessControlList": Sequence[
-            Union[HierarchicalPrincipalTypeDef, HierarchicalPrincipalOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-
-class UpdateAccessControlConfigurationRequestRequestTypeDef(
-    _RequiredUpdateAccessControlConfigurationRequestRequestTypeDef,
-    _OptionalUpdateAccessControlConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
+HierarchicalPrincipalUnionTypeDef = Union[
+    HierarchicalPrincipalTypeDef, HierarchicalPrincipalOutputTypeDef
+]
 CreateFeaturedResultsSetResponseTypeDef = TypedDict(
     "CreateFeaturedResultsSetResponseTypeDef",
     {
         "FeaturedResultsSet": FeaturedResultsSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4409,108 +4371,17 @@
         "Condition": DocumentAttributeConditionOutputTypeDef,
         "Target": DocumentAttributeTargetOutputTypeDef,
         "DocumentContentDeletion": bool,
     },
     total=False,
 )
 
-_RequiredHookConfigurationTypeDef = TypedDict(
-    "_RequiredHookConfigurationTypeDef",
-    {
-        "LambdaArn": str,
-        "S3Bucket": str,
-    },
-)
-_OptionalHookConfigurationTypeDef = TypedDict(
-    "_OptionalHookConfigurationTypeDef",
-    {
-        "InvocationCondition": DocumentAttributeConditionTypeDef,
-    },
-    total=False,
-)
-
-
-class HookConfigurationTypeDef(
-    _RequiredHookConfigurationTypeDef, _OptionalHookConfigurationTypeDef
-):
-    pass
-
-
-InlineCustomDocumentEnrichmentConfigurationTypeDef = TypedDict(
-    "InlineCustomDocumentEnrichmentConfigurationTypeDef",
-    {
-        "Condition": DocumentAttributeConditionTypeDef,
-        "Target": DocumentAttributeTargetTypeDef,
-        "DocumentContentDeletion": bool,
-    },
-    total=False,
-)
-
-AttributeFilterTypeDef = TypedDict(
-    "AttributeFilterTypeDef",
-    {
-        "AndAllFilters": Sequence[Dict[str, Any]],
-        "OrAllFilters": Sequence[Dict[str, Any]],
-        "NotFilter": Dict[str, Any],
-        "EqualsTo": DocumentAttributeTypeDef,
-        "ContainsAll": DocumentAttributeTypeDef,
-        "ContainsAny": DocumentAttributeTypeDef,
-        "GreaterThan": DocumentAttributeTypeDef,
-        "GreaterThanOrEquals": DocumentAttributeTypeDef,
-        "LessThan": DocumentAttributeTypeDef,
-        "LessThanOrEquals": DocumentAttributeTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDocumentInfoTypeDef = TypedDict(
-    "_RequiredDocumentInfoTypeDef",
-    {
-        "DocumentId": str,
-    },
-)
-_OptionalDocumentInfoTypeDef = TypedDict(
-    "_OptionalDocumentInfoTypeDef",
-    {
-        "Attributes": Sequence[DocumentAttributeTypeDef],
-    },
-    total=False,
-)
-
-
-class DocumentInfoTypeDef(_RequiredDocumentInfoTypeDef, _OptionalDocumentInfoTypeDef):
-    pass
-
-
-_RequiredDocumentTypeDef = TypedDict(
-    "_RequiredDocumentTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalDocumentTypeDef = TypedDict(
-    "_OptionalDocumentTypeDef",
-    {
-        "Title": str,
-        "Blob": Union[str, bytes, IO[Any], StreamingBody],
-        "S3Path": S3PathTypeDef,
-        "Attributes": Sequence[DocumentAttributeTypeDef],
-        "AccessControlList": Sequence[PrincipalTypeDef],
-        "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalTypeDef],
-        "ContentType": ContentTypeType,
-        "AccessControlConfigurationId": str,
-    },
-    total=False,
-)
-
-
-class DocumentTypeDef(_RequiredDocumentTypeDef, _OptionalDocumentTypeDef):
-    pass
-
-
+DocumentMetadataConfigurationUnionTypeDef = Union[
+    DocumentMetadataConfigurationTypeDef, DocumentMetadataConfigurationOutputTypeDef
+]
 _RequiredQueryRequestRequestTypeDef = TypedDict(
     "_RequiredQueryRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalQueryRequestRequestTypeDef = TypedDict(
@@ -4614,14 +4485,17 @@
 
 class CreateExperienceRequestRequestTypeDef(
     _RequiredCreateExperienceRequestRequestTypeDef, _OptionalCreateExperienceRequestRequestTypeDef
 ):
     pass
 
 
+ExperienceConfigurationUnionTypeDef = Union[
+    ExperienceConfigurationTypeDef, ExperienceConfigurationOutputTypeDef
+]
 _RequiredUpdateExperienceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateExperienceRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -4725,44 +4599,14 @@
         "UserTokenConfigurations": List[UserTokenConfigurationTypeDef],
         "UserContextPolicy": UserContextPolicyType,
         "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateIndexRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateIndexRequestRequestTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalUpdateIndexRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateIndexRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RoleArn": str,
-        "Description": str,
-        "DocumentMetadataConfigurationUpdates": Sequence[
-            Union[DocumentMetadataConfigurationTypeDef, DocumentMetadataConfigurationOutputTypeDef]
-        ],
-        "CapacityUnits": CapacityUnitsConfigurationTypeDef,
-        "UserTokenConfigurations": Sequence[UserTokenConfigurationTypeDef],
-        "UserContextPolicy": UserContextPolicyType,
-        "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateIndexRequestRequestTypeDef(
-    _RequiredUpdateIndexRequestRequestTypeDef, _OptionalUpdateIndexRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredWebCrawlerConfigurationOutputTypeDef = TypedDict(
     "_RequiredWebCrawlerConfigurationOutputTypeDef",
     {
         "Urls": UrlsOutputTypeDef,
     },
 )
 _OptionalWebCrawlerConfigurationOutputTypeDef = TypedDict(
@@ -4888,14 +4732,160 @@
 
 class SalesforceConfigurationTypeDef(
     _RequiredSalesforceConfigurationTypeDef, _OptionalSalesforceConfigurationTypeDef
 ):
     pass
 
 
+_RequiredHookConfigurationTypeDef = TypedDict(
+    "_RequiredHookConfigurationTypeDef",
+    {
+        "LambdaArn": str,
+        "S3Bucket": str,
+    },
+)
+_OptionalHookConfigurationTypeDef = TypedDict(
+    "_OptionalHookConfigurationTypeDef",
+    {
+        "InvocationCondition": DocumentAttributeConditionTypeDef,
+    },
+    total=False,
+)
+
+
+class HookConfigurationTypeDef(
+    _RequiredHookConfigurationTypeDef, _OptionalHookConfigurationTypeDef
+):
+    pass
+
+
+InlineCustomDocumentEnrichmentConfigurationTypeDef = TypedDict(
+    "InlineCustomDocumentEnrichmentConfigurationTypeDef",
+    {
+        "Condition": DocumentAttributeConditionTypeDef,
+        "Target": DocumentAttributeTargetTypeDef,
+        "DocumentContentDeletion": bool,
+    },
+    total=False,
+)
+
+AttributeFilterTypeDef = TypedDict(
+    "AttributeFilterTypeDef",
+    {
+        "AndAllFilters": Sequence[Dict[str, Any]],
+        "OrAllFilters": Sequence[Dict[str, Any]],
+        "NotFilter": Dict[str, Any],
+        "EqualsTo": DocumentAttributeTypeDef,
+        "ContainsAll": DocumentAttributeTypeDef,
+        "ContainsAny": DocumentAttributeTypeDef,
+        "GreaterThan": DocumentAttributeTypeDef,
+        "GreaterThanOrEquals": DocumentAttributeTypeDef,
+        "LessThan": DocumentAttributeTypeDef,
+        "LessThanOrEquals": DocumentAttributeTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDocumentInfoTypeDef = TypedDict(
+    "_RequiredDocumentInfoTypeDef",
+    {
+        "DocumentId": str,
+    },
+)
+_OptionalDocumentInfoTypeDef = TypedDict(
+    "_OptionalDocumentInfoTypeDef",
+    {
+        "Attributes": Sequence[DocumentAttributeTypeDef],
+    },
+    total=False,
+)
+
+
+class DocumentInfoTypeDef(_RequiredDocumentInfoTypeDef, _OptionalDocumentInfoTypeDef):
+    pass
+
+
+_RequiredDocumentTypeDef = TypedDict(
+    "_RequiredDocumentTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalDocumentTypeDef = TypedDict(
+    "_OptionalDocumentTypeDef",
+    {
+        "Title": str,
+        "Blob": BlobTypeDef,
+        "S3Path": S3PathTypeDef,
+        "Attributes": Sequence[DocumentAttributeTypeDef],
+        "AccessControlList": Sequence[PrincipalTypeDef],
+        "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalTypeDef],
+        "ContentType": ContentTypeType,
+        "AccessControlConfigurationId": str,
+    },
+    total=False,
+)
+
+
+class DocumentTypeDef(_RequiredDocumentTypeDef, _OptionalDocumentTypeDef):
+    pass
+
+
+_RequiredCreateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAccessControlConfigurationRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "Name": str,
+    },
+)
+_OptionalCreateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAccessControlConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+        "AccessControlList": Sequence[PrincipalTypeDef],
+        "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalUnionTypeDef],
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class CreateAccessControlConfigurationRequestRequestTypeDef(
+    _RequiredCreateAccessControlConfigurationRequestRequestTypeDef,
+    _OptionalCreateAccessControlConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAccessControlConfigurationRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "Id": str,
+    },
+)
+_OptionalUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAccessControlConfigurationRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "AccessControlList": Sequence[PrincipalTypeDef],
+        "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateAccessControlConfigurationRequestRequestTypeDef(
+    _RequiredUpdateAccessControlConfigurationRequestRequestTypeDef,
+    _OptionalUpdateAccessControlConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredGetQuerySuggestionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetQuerySuggestionsRequestRequestTypeDef",
     {
         "IndexId": str,
         "QueryText": str,
     },
 )
@@ -4933,33 +4923,42 @@
         "PreExtractionHookConfiguration": HookConfigurationOutputTypeDef,
         "PostExtractionHookConfiguration": HookConfigurationOutputTypeDef,
         "RoleArn": str,
     },
     total=False,
 )
 
-CustomDocumentEnrichmentConfigurationTypeDef = TypedDict(
-    "CustomDocumentEnrichmentConfigurationTypeDef",
+_RequiredUpdateIndexRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateIndexRequestRequestTypeDef",
     {
-        "InlineConfigurations": Sequence[InlineCustomDocumentEnrichmentConfigurationTypeDef],
-        "PreExtractionHookConfiguration": HookConfigurationTypeDef,
-        "PostExtractionHookConfiguration": HookConfigurationTypeDef,
-        "RoleArn": str,
+        "Id": str,
     },
-    total=False,
 )
-
-BatchGetDocumentStatusRequestRequestTypeDef = TypedDict(
-    "BatchGetDocumentStatusRequestRequestTypeDef",
+_OptionalUpdateIndexRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateIndexRequestRequestTypeDef",
     {
-        "IndexId": str,
-        "DocumentInfoList": Sequence[DocumentInfoTypeDef],
+        "Name": str,
+        "RoleArn": str,
+        "Description": str,
+        "DocumentMetadataConfigurationUpdates": Sequence[DocumentMetadataConfigurationUnionTypeDef],
+        "CapacityUnits": CapacityUnitsConfigurationTypeDef,
+        "UserTokenConfigurations": Sequence[UserTokenConfigurationTypeDef],
+        "UserContextPolicy": UserContextPolicyType,
+        "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
     },
+    total=False,
 )
 
+
+class UpdateIndexRequestRequestTypeDef(
+    _RequiredUpdateIndexRequestRequestTypeDef, _OptionalUpdateIndexRequestRequestTypeDef
+):
+    pass
+
+
 AdditionalResultAttributeTypeDef = TypedDict(
     "AdditionalResultAttributeTypeDef",
     {
         "Key": str,
         "ValueType": Literal["TEXT_WITH_HIGHLIGHTS_VALUE"],
         "Value": AdditionalResultAttributeValueTypeDef,
     },
@@ -5021,36 +5020,32 @@
         "GitHubConfiguration": GitHubConfigurationTypeDef,
         "AlfrescoConfiguration": AlfrescoConfigurationTypeDef,
         "TemplateConfiguration": TemplateConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredBatchPutDocumentRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchPutDocumentRequestRequestTypeDef",
-    {
-        "IndexId": str,
-        "Documents": Sequence[DocumentTypeDef],
-    },
-)
-_OptionalBatchPutDocumentRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchPutDocumentRequestRequestTypeDef",
+CustomDocumentEnrichmentConfigurationTypeDef = TypedDict(
+    "CustomDocumentEnrichmentConfigurationTypeDef",
     {
+        "InlineConfigurations": Sequence[InlineCustomDocumentEnrichmentConfigurationTypeDef],
+        "PreExtractionHookConfiguration": HookConfigurationTypeDef,
+        "PostExtractionHookConfiguration": HookConfigurationTypeDef,
         "RoleArn": str,
-        "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationTypeDef,
     },
     total=False,
 )
 
-
-class BatchPutDocumentRequestRequestTypeDef(
-    _RequiredBatchPutDocumentRequestRequestTypeDef, _OptionalBatchPutDocumentRequestRequestTypeDef
-):
-    pass
-
+BatchGetDocumentStatusRequestRequestTypeDef = TypedDict(
+    "BatchGetDocumentStatusRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "DocumentInfoList": Sequence[DocumentInfoTypeDef],
+    },
+)
 
 FeaturedResultsItemTypeDef = TypedDict(
     "FeaturedResultsItemTypeDef",
     {
         "Id": str,
         "Type": QueryResultTypeType,
         "AdditionalAttributes": List[AdditionalResultAttributeTypeDef],
@@ -5110,14 +5105,40 @@
         "ErrorMessage": str,
         "LanguageCode": str,
         "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DataSourceConfigurationUnionTypeDef = Union[
+    DataSourceConfigurationTypeDef, DataSourceConfigurationOutputTypeDef
+]
+_RequiredBatchPutDocumentRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchPutDocumentRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "Documents": Sequence[DocumentTypeDef],
+    },
+)
+_OptionalBatchPutDocumentRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchPutDocumentRequestRequestTypeDef",
+    {
+        "RoleArn": str,
+        "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class BatchPutDocumentRequestRequestTypeDef(
+    _RequiredBatchPutDocumentRequestRequestTypeDef, _OptionalBatchPutDocumentRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredCreateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceRequestRequestTypeDef",
     {
         "Name": str,
         "IndexId": str,
         "Type": DataSourceTypeType,
     },
@@ -5141,14 +5162,17 @@
 
 class CreateDataSourceRequestRequestTypeDef(
     _RequiredCreateDataSourceRequestRequestTypeDef, _OptionalCreateDataSourceRequestRequestTypeDef
 ):
     pass
 
 
+CustomDocumentEnrichmentConfigurationUnionTypeDef = Union[
+    CustomDocumentEnrichmentConfigurationTypeDef, CustomDocumentEnrichmentConfigurationOutputTypeDef
+]
 _RequiredUpdateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataSourceRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
```

### Comparing `mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra/type_defs.pyi` & `mypy-boto3-kendra-1.28.16/mypy_boto3_kendra/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_kendra.type_defs import AccessControlConfigurationSummaryTypeDef
 
-    data: AccessControlConfigurationSummaryTypeDef = {...}
+    data: AccessControlConfigurationSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -103,17 +103,18 @@
     "DataSourceSyncJobMetricTargetTypeDef",
     "BatchDeleteDocumentResponseFailedDocumentTypeDef",
     "BatchDeleteFeaturedResultsSetErrorTypeDef",
     "BatchDeleteFeaturedResultsSetRequestRequestTypeDef",
     "BatchGetDocumentStatusResponseErrorTypeDef",
     "StatusTypeDef",
     "BatchPutDocumentResponseFailedDocumentTypeDef",
+    "BlobTypeDef",
     "CapacityUnitsConfigurationTypeDef",
     "ClearQuerySuggestionsRequestRequestTypeDef",
-    "ClickFeedbackTypeDef",
+    "TimestampTypeDef",
     "ConfluenceAttachmentToIndexFieldMappingTypeDef",
     "ConfluenceBlogToIndexFieldMappingTypeDef",
     "ProxyConfigurationTypeDef",
     "ConfluencePageToIndexFieldMappingTypeDef",
     "ConfluenceSpaceToIndexFieldMappingTypeDef",
     "ConnectionConfigurationTypeDef",
     "ContentSourceConfigurationOutputTypeDef",
@@ -150,15 +151,14 @@
     "DescribePrincipalMappingRequestRequestTypeDef",
     "GroupOrderingIdSummaryTypeDef",
     "DescribeQuerySuggestionsBlockListRequestRequestTypeDef",
     "DescribeQuerySuggestionsConfigRequestRequestTypeDef",
     "DescribeThesaurusRequestRequestTypeDef",
     "DisassociatePersonasFromEntitiesRequestRequestTypeDef",
     "DocumentAttributeValueOutputTypeDef",
-    "DocumentAttributeValueTypeDef",
     "RelevanceOutputTypeDef",
     "SearchTypeDef",
     "RelevanceTypeDef",
     "DocumentsMetadataConfigurationTypeDef",
     "EntityDisplayDataTypeDef",
     "UserIdentityConfigurationTypeDef",
     "FacetResultTypeDef",
@@ -175,15 +175,14 @@
     "GroupSummaryTypeDef",
     "HighlightTypeDef",
     "IndexConfigurationSummaryTypeDef",
     "TextDocumentStatisticsTypeDef",
     "JsonTokenTypeConfigurationTypeDef",
     "JwtTokenTypeConfigurationTypeDef",
     "ListAccessControlConfigurationsRequestRequestTypeDef",
-    "TimeRangeTypeDef",
     "ListDataSourcesRequestRequestTypeDef",
     "ListEntityPersonasRequestRequestTypeDef",
     "PersonasSummaryTypeDef",
     "ListExperienceEntitiesRequestRequestTypeDef",
     "ListExperiencesRequestRequestTypeDef",
     "ListFaqsRequestRequestTypeDef",
     "ListFeaturedResultsSetsRequestRequestTypeDef",
@@ -237,14 +236,15 @@
     "OnPremiseConfigurationTypeDef",
     "OneDriveUsersOutputTypeDef",
     "OneDriveUsersTypeDef",
     "UpdateQuerySuggestionsBlockListRequestRequestTypeDef",
     "UpdateThesaurusRequestRequestTypeDef",
     "AlfrescoConfigurationTypeDef",
     "BoxConfigurationTypeDef",
+    "DataSourceVpcConfigurationUnionTypeDef",
     "FsxConfigurationTypeDef",
     "JiraConfigurationTypeDef",
     "QuipConfigurationTypeDef",
     "SlackConfigurationTypeDef",
     "AssociateEntitiesToExperienceRequestRequestTypeDef",
     "DisassociateEntitiesFromExperienceRequestRequestTypeDef",
     "AssociateEntitiesToExperienceResponseTypeDef",
@@ -270,14 +270,17 @@
     "AuthenticationConfigurationOutputTypeDef",
     "AuthenticationConfigurationTypeDef",
     "BatchDeleteDocumentRequestRequestTypeDef",
     "BatchDeleteDocumentResponseTypeDef",
     "BatchDeleteFeaturedResultsSetResponseTypeDef",
     "BatchGetDocumentStatusResponseTypeDef",
     "BatchPutDocumentResponseTypeDef",
+    "ClickFeedbackTypeDef",
+    "DocumentAttributeValueTypeDef",
+    "TimeRangeTypeDef",
     "ConfluenceAttachmentConfigurationOutputTypeDef",
     "ConfluenceAttachmentConfigurationTypeDef",
     "ConfluenceBlogConfigurationOutputTypeDef",
     "ConfluenceBlogConfigurationTypeDef",
     "SharePointConfigurationOutputTypeDef",
     "SharePointConfigurationTypeDef",
     "ConfluencePageConfigurationOutputTypeDef",
@@ -301,17 +304,14 @@
     "ExperiencesSummaryTypeDef",
     "DescribeFeaturedResultsSetResponseTypeDef",
     "DescribePrincipalMappingResponseTypeDef",
     "DocumentAttributeConditionOutputTypeDef",
     "DocumentAttributeOutputTypeDef",
     "DocumentAttributeTargetOutputTypeDef",
     "DocumentAttributeValueCountPairTypeDef",
-    "DocumentAttributeConditionTypeDef",
-    "DocumentAttributeTargetTypeDef",
-    "DocumentAttributeTypeDef",
     "DocumentMetadataConfigurationOutputTypeDef",
     "DocumentMetadataConfigurationTypeDef",
     "DocumentRelevanceConfigurationTypeDef",
     "S3DataSourceConfigurationOutputTypeDef",
     "S3DataSourceConfigurationTypeDef",
     "ExperienceEntitiesSummaryTypeDef",
     "ExperienceConfigurationOutputTypeDef",
@@ -321,19 +321,17 @@
     "GetSnapshotsResponseTypeDef",
     "GroupMembersTypeDef",
     "ListGroupsOlderThanOrderingIdResponseTypeDef",
     "TextWithHighlightsTypeDef",
     "ListIndicesResponseTypeDef",
     "IndexStatisticsTypeDef",
     "UserTokenConfigurationTypeDef",
-    "ListDataSourceSyncJobsRequestRequestTypeDef",
     "ListEntityPersonasResponseTypeDef",
     "ListQuerySuggestionsBlockListsResponseTypeDef",
     "ListThesauriResponseTypeDef",
-    "SubmitFeedbackRequestRequestTypeDef",
     "UrlsOutputTypeDef",
     "UrlsTypeDef",
     "SuggestionTextWithHighlightsTypeDef",
     "TableRowTypeDef",
     "DatabaseConfigurationOutputTypeDef",
     "DatabaseConfigurationTypeDef",
     "SalesforceKnowledgeArticleConfigurationOutputTypeDef",
@@ -342,65 +340,76 @@
     "ServiceNowConfigurationTypeDef",
     "GitHubConfigurationOutputTypeDef",
     "GitHubConfigurationTypeDef",
     "OneDriveConfigurationOutputTypeDef",
     "OneDriveConfigurationTypeDef",
     "DescribeQuerySuggestionsConfigResponseTypeDef",
     "UpdateQuerySuggestionsConfigRequestRequestTypeDef",
+    "SubmitFeedbackRequestRequestTypeDef",
+    "DocumentAttributeConditionTypeDef",
+    "DocumentAttributeTargetTypeDef",
+    "DocumentAttributeTypeDef",
+    "ListDataSourceSyncJobsRequestRequestTypeDef",
+    "TimeRangeUnionTypeDef",
     "ConfluenceConfigurationOutputTypeDef",
     "ConfluenceConfigurationTypeDef",
     "DescribeAccessControlConfigurationResponseTypeDef",
-    "CreateAccessControlConfigurationRequestRequestTypeDef",
-    "UpdateAccessControlConfigurationRequestRequestTypeDef",
+    "HierarchicalPrincipalUnionTypeDef",
     "CreateFeaturedResultsSetResponseTypeDef",
     "UpdateFeaturedResultsSetResponseTypeDef",
     "AttributeSuggestionsGetConfigTypeDef",
     "ListDataSourceSyncJobsResponseTypeDef",
     "ListExperiencesResponseTypeDef",
     "HookConfigurationOutputTypeDef",
     "RetrieveResultItemTypeDef",
     "SourceDocumentTypeDef",
     "InlineCustomDocumentEnrichmentConfigurationOutputTypeDef",
-    "HookConfigurationTypeDef",
-    "InlineCustomDocumentEnrichmentConfigurationTypeDef",
-    "AttributeFilterTypeDef",
-    "DocumentInfoTypeDef",
-    "DocumentTypeDef",
+    "DocumentMetadataConfigurationUnionTypeDef",
     "QueryRequestRequestTypeDef",
     "RetrieveRequestRequestTypeDef",
     "ListExperienceEntitiesResponseTypeDef",
     "DescribeExperienceResponseTypeDef",
     "CreateExperienceRequestRequestTypeDef",
+    "ExperienceConfigurationUnionTypeDef",
     "UpdateExperienceRequestRequestTypeDef",
     "PutPrincipalMappingRequestRequestTypeDef",
     "AdditionalResultAttributeValueTypeDef",
     "CreateIndexRequestRequestTypeDef",
     "DescribeIndexResponseTypeDef",
-    "UpdateIndexRequestRequestTypeDef",
     "WebCrawlerConfigurationOutputTypeDef",
     "WebCrawlerConfigurationTypeDef",
     "SuggestionValueTypeDef",
     "TableExcerptTypeDef",
     "SalesforceConfigurationOutputTypeDef",
     "SalesforceConfigurationTypeDef",
+    "HookConfigurationTypeDef",
+    "InlineCustomDocumentEnrichmentConfigurationTypeDef",
+    "AttributeFilterTypeDef",
+    "DocumentInfoTypeDef",
+    "DocumentTypeDef",
+    "CreateAccessControlConfigurationRequestRequestTypeDef",
+    "UpdateAccessControlConfigurationRequestRequestTypeDef",
     "GetQuerySuggestionsRequestRequestTypeDef",
     "RetrieveResultTypeDef",
     "CustomDocumentEnrichmentConfigurationOutputTypeDef",
-    "CustomDocumentEnrichmentConfigurationTypeDef",
-    "BatchGetDocumentStatusRequestRequestTypeDef",
+    "UpdateIndexRequestRequestTypeDef",
     "AdditionalResultAttributeTypeDef",
     "SuggestionTypeDef",
     "DataSourceConfigurationOutputTypeDef",
     "DataSourceConfigurationTypeDef",
-    "BatchPutDocumentRequestRequestTypeDef",
+    "CustomDocumentEnrichmentConfigurationTypeDef",
+    "BatchGetDocumentStatusRequestRequestTypeDef",
     "FeaturedResultsItemTypeDef",
     "QueryResultItemTypeDef",
     "GetQuerySuggestionsResponseTypeDef",
     "DescribeDataSourceResponseTypeDef",
+    "DataSourceConfigurationUnionTypeDef",
+    "BatchPutDocumentRequestRequestTypeDef",
     "CreateDataSourceRequestRequestTypeDef",
+    "CustomDocumentEnrichmentConfigurationUnionTypeDef",
     "UpdateDataSourceRequestRequestTypeDef",
     "QueryResultTypeDef",
 )
 
 AccessControlConfigurationSummaryTypeDef = TypedDict(
     "AccessControlConfigurationSummaryTypeDef",
     {
@@ -594,14 +603,15 @@
         "Id": str,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CapacityUnitsConfigurationTypeDef = TypedDict(
     "CapacityUnitsConfigurationTypeDef",
     {
         "StorageCapacityUnits": int,
         "QueryCapacityUnits": int,
     },
 )
@@ -609,22 +619,15 @@
 ClearQuerySuggestionsRequestRequestTypeDef = TypedDict(
     "ClearQuerySuggestionsRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 
-ClickFeedbackTypeDef = TypedDict(
-    "ClickFeedbackTypeDef",
-    {
-        "ResultId": str,
-        "ClickTime": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 ConfluenceAttachmentToIndexFieldMappingTypeDef = TypedDict(
     "ConfluenceAttachmentToIndexFieldMappingTypeDef",
     {
         "DataSourceFieldName": ConfluenceAttachmentFieldNameType,
         "DateFieldFormat": str,
         "IndexFieldName": str,
     },
@@ -1054,25 +1057,14 @@
         "StringListValue": List[str],
         "LongValue": int,
         "DateValue": datetime,
     },
     total=False,
 )
 
-DocumentAttributeValueTypeDef = TypedDict(
-    "DocumentAttributeValueTypeDef",
-    {
-        "StringValue": str,
-        "StringListValue": Sequence[str],
-        "LongValue": int,
-        "DateValue": Union[datetime, str],
-    },
-    total=False,
-)
-
 RelevanceOutputTypeDef = TypedDict(
     "RelevanceOutputTypeDef",
     {
         "Freshness": bool,
         "Importance": int,
         "Duration": str,
         "RankOrder": OrderType,
@@ -1370,23 +1362,14 @@
 
 class ListAccessControlConfigurationsRequestRequestTypeDef(
     _RequiredListAccessControlConfigurationsRequestRequestTypeDef,
     _OptionalListAccessControlConfigurationsRequestRequestTypeDef,
 ):
     pass
 
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredListDataSourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSourcesRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalListDataSourcesRequestRequestTypeDef = TypedDict(
@@ -2491,14 +2474,17 @@
     },
     total=False,
 )
 
 class BoxConfigurationTypeDef(_RequiredBoxConfigurationTypeDef, _OptionalBoxConfigurationTypeDef):
     pass
 
+DataSourceVpcConfigurationUnionTypeDef = Union[
+    DataSourceVpcConfigurationTypeDef, DataSourceVpcConfigurationOutputTypeDef
+]
 _RequiredFsxConfigurationTypeDef = TypedDict(
     "_RequiredFsxConfigurationTypeDef",
     {
         "FileSystemId": str,
         "FileSystemType": Literal["WINDOWS"],
         "VpcConfiguration": DataSourceVpcConfigurationTypeDef,
     },
@@ -2890,14 +2876,42 @@
     "BatchPutDocumentResponseTypeDef",
     {
         "FailedDocuments": List[BatchPutDocumentResponseFailedDocumentTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ClickFeedbackTypeDef = TypedDict(
+    "ClickFeedbackTypeDef",
+    {
+        "ResultId": str,
+        "ClickTime": TimestampTypeDef,
+    },
+)
+
+DocumentAttributeValueTypeDef = TypedDict(
+    "DocumentAttributeValueTypeDef",
+    {
+        "StringValue": str,
+        "StringListValue": Sequence[str],
+        "LongValue": int,
+        "DateValue": TimestampTypeDef,
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
 ConfluenceAttachmentConfigurationOutputTypeDef = TypedDict(
     "ConfluenceAttachmentConfigurationOutputTypeDef",
     {
         "CrawlAttachments": bool,
         "AttachmentFieldMappings": List[ConfluenceAttachmentToIndexFieldMappingTypeDef],
     },
     total=False,
@@ -3329,52 +3343,14 @@
         "DocumentAttributeValue": DocumentAttributeValueOutputTypeDef,
         "Count": int,
         "FacetResults": List[Dict[str, Any]],
     },
     total=False,
 )
 
-_RequiredDocumentAttributeConditionTypeDef = TypedDict(
-    "_RequiredDocumentAttributeConditionTypeDef",
-    {
-        "ConditionDocumentAttributeKey": str,
-        "Operator": ConditionOperatorType,
-    },
-)
-_OptionalDocumentAttributeConditionTypeDef = TypedDict(
-    "_OptionalDocumentAttributeConditionTypeDef",
-    {
-        "ConditionOnValue": DocumentAttributeValueTypeDef,
-    },
-    total=False,
-)
-
-class DocumentAttributeConditionTypeDef(
-    _RequiredDocumentAttributeConditionTypeDef, _OptionalDocumentAttributeConditionTypeDef
-):
-    pass
-
-DocumentAttributeTargetTypeDef = TypedDict(
-    "DocumentAttributeTargetTypeDef",
-    {
-        "TargetDocumentAttributeKey": str,
-        "TargetDocumentAttributeValueDeletion": bool,
-        "TargetDocumentAttributeValue": DocumentAttributeValueTypeDef,
-    },
-    total=False,
-)
-
-DocumentAttributeTypeDef = TypedDict(
-    "DocumentAttributeTypeDef",
-    {
-        "Key": str,
-        "Value": DocumentAttributeValueTypeDef,
-    },
-)
-
 _RequiredDocumentMetadataConfigurationOutputTypeDef = TypedDict(
     "_RequiredDocumentMetadataConfigurationOutputTypeDef",
     {
         "Name": str,
         "Type": DocumentAttributeValueTypeType,
     },
 )
@@ -3575,38 +3551,14 @@
     {
         "JwtTokenTypeConfiguration": JwtTokenTypeConfigurationTypeDef,
         "JsonTokenTypeConfiguration": JsonTokenTypeConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDataSourceSyncJobsRequestRequestTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-    },
-)
-_OptionalListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDataSourceSyncJobsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "StartTimeFilter": TimeRangeTypeDef,
-        "StatusFilter": DataSourceSyncJobStatusType,
-    },
-    total=False,
-)
-
-class ListDataSourceSyncJobsRequestRequestTypeDef(
-    _RequiredListDataSourceSyncJobsRequestRequestTypeDef,
-    _OptionalListDataSourceSyncJobsRequestRequestTypeDef,
-):
-    pass
-
 ListEntityPersonasResponseTypeDef = TypedDict(
     "ListEntityPersonasResponseTypeDef",
     {
         "SummaryItems": List[PersonasSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3626,35 +3578,14 @@
     {
         "NextToken": str,
         "ThesaurusSummaryItems": List[ThesaurusSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSubmitFeedbackRequestRequestTypeDef = TypedDict(
-    "_RequiredSubmitFeedbackRequestRequestTypeDef",
-    {
-        "IndexId": str,
-        "QueryId": str,
-    },
-)
-_OptionalSubmitFeedbackRequestRequestTypeDef = TypedDict(
-    "_OptionalSubmitFeedbackRequestRequestTypeDef",
-    {
-        "ClickFeedbackItems": Sequence[ClickFeedbackTypeDef],
-        "RelevanceFeedbackItems": Sequence[RelevanceFeedbackTypeDef],
-    },
-    total=False,
-)
-
-class SubmitFeedbackRequestRequestTypeDef(
-    _RequiredSubmitFeedbackRequestRequestTypeDef, _OptionalSubmitFeedbackRequestRequestTypeDef
-):
-    pass
-
 UrlsOutputTypeDef = TypedDict(
     "UrlsOutputTypeDef",
     {
         "SeedUrlConfiguration": SeedUrlConfigurationOutputTypeDef,
         "SiteMapsConfiguration": SiteMapsConfigurationOutputTypeDef,
     },
     total=False,
@@ -4014,14 +3945,98 @@
 
 class UpdateQuerySuggestionsConfigRequestRequestTypeDef(
     _RequiredUpdateQuerySuggestionsConfigRequestRequestTypeDef,
     _OptionalUpdateQuerySuggestionsConfigRequestRequestTypeDef,
 ):
     pass
 
+_RequiredSubmitFeedbackRequestRequestTypeDef = TypedDict(
+    "_RequiredSubmitFeedbackRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "QueryId": str,
+    },
+)
+_OptionalSubmitFeedbackRequestRequestTypeDef = TypedDict(
+    "_OptionalSubmitFeedbackRequestRequestTypeDef",
+    {
+        "ClickFeedbackItems": Sequence[ClickFeedbackTypeDef],
+        "RelevanceFeedbackItems": Sequence[RelevanceFeedbackTypeDef],
+    },
+    total=False,
+)
+
+class SubmitFeedbackRequestRequestTypeDef(
+    _RequiredSubmitFeedbackRequestRequestTypeDef, _OptionalSubmitFeedbackRequestRequestTypeDef
+):
+    pass
+
+_RequiredDocumentAttributeConditionTypeDef = TypedDict(
+    "_RequiredDocumentAttributeConditionTypeDef",
+    {
+        "ConditionDocumentAttributeKey": str,
+        "Operator": ConditionOperatorType,
+    },
+)
+_OptionalDocumentAttributeConditionTypeDef = TypedDict(
+    "_OptionalDocumentAttributeConditionTypeDef",
+    {
+        "ConditionOnValue": DocumentAttributeValueTypeDef,
+    },
+    total=False,
+)
+
+class DocumentAttributeConditionTypeDef(
+    _RequiredDocumentAttributeConditionTypeDef, _OptionalDocumentAttributeConditionTypeDef
+):
+    pass
+
+DocumentAttributeTargetTypeDef = TypedDict(
+    "DocumentAttributeTargetTypeDef",
+    {
+        "TargetDocumentAttributeKey": str,
+        "TargetDocumentAttributeValueDeletion": bool,
+        "TargetDocumentAttributeValue": DocumentAttributeValueTypeDef,
+    },
+    total=False,
+)
+
+DocumentAttributeTypeDef = TypedDict(
+    "DocumentAttributeTypeDef",
+    {
+        "Key": str,
+        "Value": DocumentAttributeValueTypeDef,
+    },
+)
+
+_RequiredListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDataSourceSyncJobsRequestRequestTypeDef",
+    {
+        "Id": str,
+        "IndexId": str,
+    },
+)
+_OptionalListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDataSourceSyncJobsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "StartTimeFilter": TimeRangeTypeDef,
+        "StatusFilter": DataSourceSyncJobStatusType,
+    },
+    total=False,
+)
+
+class ListDataSourceSyncJobsRequestRequestTypeDef(
+    _RequiredListDataSourceSyncJobsRequestRequestTypeDef,
+    _OptionalListDataSourceSyncJobsRequestRequestTypeDef,
+):
+    pass
+
+TimeRangeUnionTypeDef = Union[TimeRangeTypeDef, TimeRangeOutputTypeDef]
 _RequiredConfluenceConfigurationOutputTypeDef = TypedDict(
     "_RequiredConfluenceConfigurationOutputTypeDef",
     {
         "ServerUrl": str,
         "SecretArn": str,
         "Version": ConfluenceVersionType,
     },
@@ -4084,66 +4099,17 @@
         "ErrorMessage": str,
         "AccessControlList": List[PrincipalTypeDef],
         "HierarchicalAccessControlList": List[HierarchicalPrincipalOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAccessControlConfigurationRequestRequestTypeDef",
-    {
-        "IndexId": str,
-        "Name": str,
-    },
-)
-_OptionalCreateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAccessControlConfigurationRequestRequestTypeDef",
-    {
-        "Description": str,
-        "AccessControlList": Sequence[PrincipalTypeDef],
-        "HierarchicalAccessControlList": Sequence[
-            Union[HierarchicalPrincipalTypeDef, HierarchicalPrincipalOutputTypeDef]
-        ],
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-class CreateAccessControlConfigurationRequestRequestTypeDef(
-    _RequiredCreateAccessControlConfigurationRequestRequestTypeDef,
-    _OptionalCreateAccessControlConfigurationRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAccessControlConfigurationRequestRequestTypeDef",
-    {
-        "IndexId": str,
-        "Id": str,
-    },
-)
-_OptionalUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAccessControlConfigurationRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "AccessControlList": Sequence[PrincipalTypeDef],
-        "HierarchicalAccessControlList": Sequence[
-            Union[HierarchicalPrincipalTypeDef, HierarchicalPrincipalOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-class UpdateAccessControlConfigurationRequestRequestTypeDef(
-    _RequiredUpdateAccessControlConfigurationRequestRequestTypeDef,
-    _OptionalUpdateAccessControlConfigurationRequestRequestTypeDef,
-):
-    pass
-
+HierarchicalPrincipalUnionTypeDef = Union[
+    HierarchicalPrincipalTypeDef, HierarchicalPrincipalOutputTypeDef
+]
 CreateFeaturedResultsSetResponseTypeDef = TypedDict(
     "CreateFeaturedResultsSetResponseTypeDef",
     {
         "FeaturedResultsSet": FeaturedResultsSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4234,102 +4200,17 @@
         "Condition": DocumentAttributeConditionOutputTypeDef,
         "Target": DocumentAttributeTargetOutputTypeDef,
         "DocumentContentDeletion": bool,
     },
     total=False,
 )
 
-_RequiredHookConfigurationTypeDef = TypedDict(
-    "_RequiredHookConfigurationTypeDef",
-    {
-        "LambdaArn": str,
-        "S3Bucket": str,
-    },
-)
-_OptionalHookConfigurationTypeDef = TypedDict(
-    "_OptionalHookConfigurationTypeDef",
-    {
-        "InvocationCondition": DocumentAttributeConditionTypeDef,
-    },
-    total=False,
-)
-
-class HookConfigurationTypeDef(
-    _RequiredHookConfigurationTypeDef, _OptionalHookConfigurationTypeDef
-):
-    pass
-
-InlineCustomDocumentEnrichmentConfigurationTypeDef = TypedDict(
-    "InlineCustomDocumentEnrichmentConfigurationTypeDef",
-    {
-        "Condition": DocumentAttributeConditionTypeDef,
-        "Target": DocumentAttributeTargetTypeDef,
-        "DocumentContentDeletion": bool,
-    },
-    total=False,
-)
-
-AttributeFilterTypeDef = TypedDict(
-    "AttributeFilterTypeDef",
-    {
-        "AndAllFilters": Sequence[Dict[str, Any]],
-        "OrAllFilters": Sequence[Dict[str, Any]],
-        "NotFilter": Dict[str, Any],
-        "EqualsTo": DocumentAttributeTypeDef,
-        "ContainsAll": DocumentAttributeTypeDef,
-        "ContainsAny": DocumentAttributeTypeDef,
-        "GreaterThan": DocumentAttributeTypeDef,
-        "GreaterThanOrEquals": DocumentAttributeTypeDef,
-        "LessThan": DocumentAttributeTypeDef,
-        "LessThanOrEquals": DocumentAttributeTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDocumentInfoTypeDef = TypedDict(
-    "_RequiredDocumentInfoTypeDef",
-    {
-        "DocumentId": str,
-    },
-)
-_OptionalDocumentInfoTypeDef = TypedDict(
-    "_OptionalDocumentInfoTypeDef",
-    {
-        "Attributes": Sequence[DocumentAttributeTypeDef],
-    },
-    total=False,
-)
-
-class DocumentInfoTypeDef(_RequiredDocumentInfoTypeDef, _OptionalDocumentInfoTypeDef):
-    pass
-
-_RequiredDocumentTypeDef = TypedDict(
-    "_RequiredDocumentTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalDocumentTypeDef = TypedDict(
-    "_OptionalDocumentTypeDef",
-    {
-        "Title": str,
-        "Blob": Union[str, bytes, IO[Any], StreamingBody],
-        "S3Path": S3PathTypeDef,
-        "Attributes": Sequence[DocumentAttributeTypeDef],
-        "AccessControlList": Sequence[PrincipalTypeDef],
-        "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalTypeDef],
-        "ContentType": ContentTypeType,
-        "AccessControlConfigurationId": str,
-    },
-    total=False,
-)
-
-class DocumentTypeDef(_RequiredDocumentTypeDef, _OptionalDocumentTypeDef):
-    pass
-
+DocumentMetadataConfigurationUnionTypeDef = Union[
+    DocumentMetadataConfigurationTypeDef, DocumentMetadataConfigurationOutputTypeDef
+]
 _RequiredQueryRequestRequestTypeDef = TypedDict(
     "_RequiredQueryRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalQueryRequestRequestTypeDef = TypedDict(
@@ -4427,14 +4308,17 @@
 )
 
 class CreateExperienceRequestRequestTypeDef(
     _RequiredCreateExperienceRequestRequestTypeDef, _OptionalCreateExperienceRequestRequestTypeDef
 ):
     pass
 
+ExperienceConfigurationUnionTypeDef = Union[
+    ExperienceConfigurationTypeDef, ExperienceConfigurationOutputTypeDef
+]
 _RequiredUpdateExperienceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateExperienceRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -4532,42 +4416,14 @@
         "UserTokenConfigurations": List[UserTokenConfigurationTypeDef],
         "UserContextPolicy": UserContextPolicyType,
         "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateIndexRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateIndexRequestRequestTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalUpdateIndexRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateIndexRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RoleArn": str,
-        "Description": str,
-        "DocumentMetadataConfigurationUpdates": Sequence[
-            Union[DocumentMetadataConfigurationTypeDef, DocumentMetadataConfigurationOutputTypeDef]
-        ],
-        "CapacityUnits": CapacityUnitsConfigurationTypeDef,
-        "UserTokenConfigurations": Sequence[UserTokenConfigurationTypeDef],
-        "UserContextPolicy": UserContextPolicyType,
-        "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class UpdateIndexRequestRequestTypeDef(
-    _RequiredUpdateIndexRequestRequestTypeDef, _OptionalUpdateIndexRequestRequestTypeDef
-):
-    pass
-
 _RequiredWebCrawlerConfigurationOutputTypeDef = TypedDict(
     "_RequiredWebCrawlerConfigurationOutputTypeDef",
     {
         "Urls": UrlsOutputTypeDef,
     },
 )
 _OptionalWebCrawlerConfigurationOutputTypeDef = TypedDict(
@@ -4685,14 +4541,150 @@
 )
 
 class SalesforceConfigurationTypeDef(
     _RequiredSalesforceConfigurationTypeDef, _OptionalSalesforceConfigurationTypeDef
 ):
     pass
 
+_RequiredHookConfigurationTypeDef = TypedDict(
+    "_RequiredHookConfigurationTypeDef",
+    {
+        "LambdaArn": str,
+        "S3Bucket": str,
+    },
+)
+_OptionalHookConfigurationTypeDef = TypedDict(
+    "_OptionalHookConfigurationTypeDef",
+    {
+        "InvocationCondition": DocumentAttributeConditionTypeDef,
+    },
+    total=False,
+)
+
+class HookConfigurationTypeDef(
+    _RequiredHookConfigurationTypeDef, _OptionalHookConfigurationTypeDef
+):
+    pass
+
+InlineCustomDocumentEnrichmentConfigurationTypeDef = TypedDict(
+    "InlineCustomDocumentEnrichmentConfigurationTypeDef",
+    {
+        "Condition": DocumentAttributeConditionTypeDef,
+        "Target": DocumentAttributeTargetTypeDef,
+        "DocumentContentDeletion": bool,
+    },
+    total=False,
+)
+
+AttributeFilterTypeDef = TypedDict(
+    "AttributeFilterTypeDef",
+    {
+        "AndAllFilters": Sequence[Dict[str, Any]],
+        "OrAllFilters": Sequence[Dict[str, Any]],
+        "NotFilter": Dict[str, Any],
+        "EqualsTo": DocumentAttributeTypeDef,
+        "ContainsAll": DocumentAttributeTypeDef,
+        "ContainsAny": DocumentAttributeTypeDef,
+        "GreaterThan": DocumentAttributeTypeDef,
+        "GreaterThanOrEquals": DocumentAttributeTypeDef,
+        "LessThan": DocumentAttributeTypeDef,
+        "LessThanOrEquals": DocumentAttributeTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDocumentInfoTypeDef = TypedDict(
+    "_RequiredDocumentInfoTypeDef",
+    {
+        "DocumentId": str,
+    },
+)
+_OptionalDocumentInfoTypeDef = TypedDict(
+    "_OptionalDocumentInfoTypeDef",
+    {
+        "Attributes": Sequence[DocumentAttributeTypeDef],
+    },
+    total=False,
+)
+
+class DocumentInfoTypeDef(_RequiredDocumentInfoTypeDef, _OptionalDocumentInfoTypeDef):
+    pass
+
+_RequiredDocumentTypeDef = TypedDict(
+    "_RequiredDocumentTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalDocumentTypeDef = TypedDict(
+    "_OptionalDocumentTypeDef",
+    {
+        "Title": str,
+        "Blob": BlobTypeDef,
+        "S3Path": S3PathTypeDef,
+        "Attributes": Sequence[DocumentAttributeTypeDef],
+        "AccessControlList": Sequence[PrincipalTypeDef],
+        "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalTypeDef],
+        "ContentType": ContentTypeType,
+        "AccessControlConfigurationId": str,
+    },
+    total=False,
+)
+
+class DocumentTypeDef(_RequiredDocumentTypeDef, _OptionalDocumentTypeDef):
+    pass
+
+_RequiredCreateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAccessControlConfigurationRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "Name": str,
+    },
+)
+_OptionalCreateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAccessControlConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+        "AccessControlList": Sequence[PrincipalTypeDef],
+        "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalUnionTypeDef],
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+class CreateAccessControlConfigurationRequestRequestTypeDef(
+    _RequiredCreateAccessControlConfigurationRequestRequestTypeDef,
+    _OptionalCreateAccessControlConfigurationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAccessControlConfigurationRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "Id": str,
+    },
+)
+_OptionalUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAccessControlConfigurationRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "AccessControlList": Sequence[PrincipalTypeDef],
+        "HierarchicalAccessControlList": Sequence[HierarchicalPrincipalUnionTypeDef],
+    },
+    total=False,
+)
+
+class UpdateAccessControlConfigurationRequestRequestTypeDef(
+    _RequiredUpdateAccessControlConfigurationRequestRequestTypeDef,
+    _OptionalUpdateAccessControlConfigurationRequestRequestTypeDef,
+):
+    pass
+
 _RequiredGetQuerySuggestionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetQuerySuggestionsRequestRequestTypeDef",
     {
         "IndexId": str,
         "QueryText": str,
     },
 )
@@ -4728,33 +4720,40 @@
         "PreExtractionHookConfiguration": HookConfigurationOutputTypeDef,
         "PostExtractionHookConfiguration": HookConfigurationOutputTypeDef,
         "RoleArn": str,
     },
     total=False,
 )
 
-CustomDocumentEnrichmentConfigurationTypeDef = TypedDict(
-    "CustomDocumentEnrichmentConfigurationTypeDef",
+_RequiredUpdateIndexRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateIndexRequestRequestTypeDef",
     {
-        "InlineConfigurations": Sequence[InlineCustomDocumentEnrichmentConfigurationTypeDef],
-        "PreExtractionHookConfiguration": HookConfigurationTypeDef,
-        "PostExtractionHookConfiguration": HookConfigurationTypeDef,
-        "RoleArn": str,
+        "Id": str,
     },
-    total=False,
 )
-
-BatchGetDocumentStatusRequestRequestTypeDef = TypedDict(
-    "BatchGetDocumentStatusRequestRequestTypeDef",
+_OptionalUpdateIndexRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateIndexRequestRequestTypeDef",
     {
-        "IndexId": str,
-        "DocumentInfoList": Sequence[DocumentInfoTypeDef],
+        "Name": str,
+        "RoleArn": str,
+        "Description": str,
+        "DocumentMetadataConfigurationUpdates": Sequence[DocumentMetadataConfigurationUnionTypeDef],
+        "CapacityUnits": CapacityUnitsConfigurationTypeDef,
+        "UserTokenConfigurations": Sequence[UserTokenConfigurationTypeDef],
+        "UserContextPolicy": UserContextPolicyType,
+        "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
     },
+    total=False,
 )
 
+class UpdateIndexRequestRequestTypeDef(
+    _RequiredUpdateIndexRequestRequestTypeDef, _OptionalUpdateIndexRequestRequestTypeDef
+):
+    pass
+
 AdditionalResultAttributeTypeDef = TypedDict(
     "AdditionalResultAttributeTypeDef",
     {
         "Key": str,
         "ValueType": Literal["TEXT_WITH_HIGHLIGHTS_VALUE"],
         "Value": AdditionalResultAttributeValueTypeDef,
     },
@@ -4816,34 +4815,32 @@
         "GitHubConfiguration": GitHubConfigurationTypeDef,
         "AlfrescoConfiguration": AlfrescoConfigurationTypeDef,
         "TemplateConfiguration": TemplateConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredBatchPutDocumentRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchPutDocumentRequestRequestTypeDef",
-    {
-        "IndexId": str,
-        "Documents": Sequence[DocumentTypeDef],
-    },
-)
-_OptionalBatchPutDocumentRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchPutDocumentRequestRequestTypeDef",
+CustomDocumentEnrichmentConfigurationTypeDef = TypedDict(
+    "CustomDocumentEnrichmentConfigurationTypeDef",
     {
+        "InlineConfigurations": Sequence[InlineCustomDocumentEnrichmentConfigurationTypeDef],
+        "PreExtractionHookConfiguration": HookConfigurationTypeDef,
+        "PostExtractionHookConfiguration": HookConfigurationTypeDef,
         "RoleArn": str,
-        "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationTypeDef,
     },
     total=False,
 )
 
-class BatchPutDocumentRequestRequestTypeDef(
-    _RequiredBatchPutDocumentRequestRequestTypeDef, _OptionalBatchPutDocumentRequestRequestTypeDef
-):
-    pass
+BatchGetDocumentStatusRequestRequestTypeDef = TypedDict(
+    "BatchGetDocumentStatusRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "DocumentInfoList": Sequence[DocumentInfoTypeDef],
+    },
+)
 
 FeaturedResultsItemTypeDef = TypedDict(
     "FeaturedResultsItemTypeDef",
     {
         "Id": str,
         "Type": QueryResultTypeType,
         "AdditionalAttributes": List[AdditionalResultAttributeTypeDef],
@@ -4903,14 +4900,38 @@
         "ErrorMessage": str,
         "LanguageCode": str,
         "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DataSourceConfigurationUnionTypeDef = Union[
+    DataSourceConfigurationTypeDef, DataSourceConfigurationOutputTypeDef
+]
+_RequiredBatchPutDocumentRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchPutDocumentRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "Documents": Sequence[DocumentTypeDef],
+    },
+)
+_OptionalBatchPutDocumentRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchPutDocumentRequestRequestTypeDef",
+    {
+        "RoleArn": str,
+        "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class BatchPutDocumentRequestRequestTypeDef(
+    _RequiredBatchPutDocumentRequestRequestTypeDef, _OptionalBatchPutDocumentRequestRequestTypeDef
+):
+    pass
+
 _RequiredCreateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceRequestRequestTypeDef",
     {
         "Name": str,
         "IndexId": str,
         "Type": DataSourceTypeType,
     },
@@ -4932,14 +4953,17 @@
 )
 
 class CreateDataSourceRequestRequestTypeDef(
     _RequiredCreateDataSourceRequestRequestTypeDef, _OptionalCreateDataSourceRequestRequestTypeDef
 ):
     pass
 
+CustomDocumentEnrichmentConfigurationUnionTypeDef = Union[
+    CustomDocumentEnrichmentConfigurationTypeDef, CustomDocumentEnrichmentConfigurationOutputTypeDef
+]
 _RequiredUpdateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataSourceRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
```

### Comparing `mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra.egg-info/PKG-INFO` & `mypy-boto3-kendra-1.28.16/mypy_boto3_kendra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kendra
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.kendra 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.kendra 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kendra type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 kendra type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kendra.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kendra)](https://pepy.tech/project/mypy-boto3-kendra)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.kendra 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
+[boto3.kendra 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
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
 [mypy-boto3-kendra docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/).
 
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
@@ -347,20 +347,20 @@
 )
 
 
 def check_value(value: AdditionalResultAttributeValueTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kendra.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kendra.type_defs import (
     AccessControlConfigurationSummaryTypeDef,
     AccessControlListConfigurationTypeDef,
     AclConfigurationTypeDef,
     DataSourceToIndexFieldMappingTypeDef,
@@ -376,17 +376,18 @@
     DataSourceSyncJobMetricTargetTypeDef,
     BatchDeleteDocumentResponseFailedDocumentTypeDef,
     BatchDeleteFeaturedResultsSetErrorTypeDef,
     BatchDeleteFeaturedResultsSetRequestRequestTypeDef,
     BatchGetDocumentStatusResponseErrorTypeDef,
     StatusTypeDef,
     BatchPutDocumentResponseFailedDocumentTypeDef,
+    BlobTypeDef,
     CapacityUnitsConfigurationTypeDef,
     ClearQuerySuggestionsRequestRequestTypeDef,
-    ClickFeedbackTypeDef,
+    TimestampTypeDef,
     ConfluenceAttachmentToIndexFieldMappingTypeDef,
     ConfluenceBlogToIndexFieldMappingTypeDef,
     ProxyConfigurationTypeDef,
     ConfluencePageToIndexFieldMappingTypeDef,
     ConfluenceSpaceToIndexFieldMappingTypeDef,
     ConnectionConfigurationTypeDef,
     ContentSourceConfigurationOutputTypeDef,
@@ -423,15 +424,14 @@
     DescribePrincipalMappingRequestRequestTypeDef,
     GroupOrderingIdSummaryTypeDef,
     DescribeQuerySuggestionsBlockListRequestRequestTypeDef,
     DescribeQuerySuggestionsConfigRequestRequestTypeDef,
     DescribeThesaurusRequestRequestTypeDef,
     DisassociatePersonasFromEntitiesRequestRequestTypeDef,
     DocumentAttributeValueOutputTypeDef,
-    DocumentAttributeValueTypeDef,
     RelevanceOutputTypeDef,
     SearchTypeDef,
     RelevanceTypeDef,
     DocumentsMetadataConfigurationTypeDef,
     EntityDisplayDataTypeDef,
     UserIdentityConfigurationTypeDef,
     FacetResultTypeDef,
@@ -448,15 +448,14 @@
     GroupSummaryTypeDef,
     HighlightTypeDef,
     IndexConfigurationSummaryTypeDef,
     TextDocumentStatisticsTypeDef,
     JsonTokenTypeConfigurationTypeDef,
     JwtTokenTypeConfigurationTypeDef,
     ListAccessControlConfigurationsRequestRequestTypeDef,
-    TimeRangeTypeDef,
     ListDataSourcesRequestRequestTypeDef,
     ListEntityPersonasRequestRequestTypeDef,
     PersonasSummaryTypeDef,
     ListExperienceEntitiesRequestRequestTypeDef,
     ListExperiencesRequestRequestTypeDef,
     ListFaqsRequestRequestTypeDef,
     ListFeaturedResultsSetsRequestRequestTypeDef,
@@ -510,14 +509,15 @@
     OnPremiseConfigurationTypeDef,
     OneDriveUsersOutputTypeDef,
     OneDriveUsersTypeDef,
     UpdateQuerySuggestionsBlockListRequestRequestTypeDef,
     UpdateThesaurusRequestRequestTypeDef,
     AlfrescoConfigurationTypeDef,
     BoxConfigurationTypeDef,
+    DataSourceVpcConfigurationUnionTypeDef,
     FsxConfigurationTypeDef,
     JiraConfigurationTypeDef,
     QuipConfigurationTypeDef,
     SlackConfigurationTypeDef,
     AssociateEntitiesToExperienceRequestRequestTypeDef,
     DisassociateEntitiesFromExperienceRequestRequestTypeDef,
     AssociateEntitiesToExperienceResponseTypeDef,
@@ -543,14 +543,17 @@
     AuthenticationConfigurationOutputTypeDef,
     AuthenticationConfigurationTypeDef,
     BatchDeleteDocumentRequestRequestTypeDef,
     BatchDeleteDocumentResponseTypeDef,
     BatchDeleteFeaturedResultsSetResponseTypeDef,
     BatchGetDocumentStatusResponseTypeDef,
     BatchPutDocumentResponseTypeDef,
+    ClickFeedbackTypeDef,
+    DocumentAttributeValueTypeDef,
+    TimeRangeTypeDef,
     ConfluenceAttachmentConfigurationOutputTypeDef,
     ConfluenceAttachmentConfigurationTypeDef,
     ConfluenceBlogConfigurationOutputTypeDef,
     ConfluenceBlogConfigurationTypeDef,
     SharePointConfigurationOutputTypeDef,
     SharePointConfigurationTypeDef,
     ConfluencePageConfigurationOutputTypeDef,
@@ -574,17 +577,14 @@
     ExperiencesSummaryTypeDef,
     DescribeFeaturedResultsSetResponseTypeDef,
     DescribePrincipalMappingResponseTypeDef,
     DocumentAttributeConditionOutputTypeDef,
     DocumentAttributeOutputTypeDef,
     DocumentAttributeTargetOutputTypeDef,
     DocumentAttributeValueCountPairTypeDef,
-    DocumentAttributeConditionTypeDef,
-    DocumentAttributeTargetTypeDef,
-    DocumentAttributeTypeDef,
     DocumentMetadataConfigurationOutputTypeDef,
     DocumentMetadataConfigurationTypeDef,
     DocumentRelevanceConfigurationTypeDef,
     S3DataSourceConfigurationOutputTypeDef,
     S3DataSourceConfigurationTypeDef,
     ExperienceEntitiesSummaryTypeDef,
     ExperienceConfigurationOutputTypeDef,
@@ -594,19 +594,17 @@
     GetSnapshotsResponseTypeDef,
     GroupMembersTypeDef,
     ListGroupsOlderThanOrderingIdResponseTypeDef,
     TextWithHighlightsTypeDef,
     ListIndicesResponseTypeDef,
     IndexStatisticsTypeDef,
     UserTokenConfigurationTypeDef,
-    ListDataSourceSyncJobsRequestRequestTypeDef,
     ListEntityPersonasResponseTypeDef,
     ListQuerySuggestionsBlockListsResponseTypeDef,
     ListThesauriResponseTypeDef,
-    SubmitFeedbackRequestRequestTypeDef,
     UrlsOutputTypeDef,
     UrlsTypeDef,
     SuggestionTextWithHighlightsTypeDef,
     TableRowTypeDef,
     DatabaseConfigurationOutputTypeDef,
     DatabaseConfigurationTypeDef,
     SalesforceKnowledgeArticleConfigurationOutputTypeDef,
@@ -615,71 +613,82 @@
     ServiceNowConfigurationTypeDef,
     GitHubConfigurationOutputTypeDef,
     GitHubConfigurationTypeDef,
     OneDriveConfigurationOutputTypeDef,
     OneDriveConfigurationTypeDef,
     DescribeQuerySuggestionsConfigResponseTypeDef,
     UpdateQuerySuggestionsConfigRequestRequestTypeDef,
+    SubmitFeedbackRequestRequestTypeDef,
+    DocumentAttributeConditionTypeDef,
+    DocumentAttributeTargetTypeDef,
+    DocumentAttributeTypeDef,
+    ListDataSourceSyncJobsRequestRequestTypeDef,
+    TimeRangeUnionTypeDef,
     ConfluenceConfigurationOutputTypeDef,
     ConfluenceConfigurationTypeDef,
     DescribeAccessControlConfigurationResponseTypeDef,
-    CreateAccessControlConfigurationRequestRequestTypeDef,
-    UpdateAccessControlConfigurationRequestRequestTypeDef,
+    HierarchicalPrincipalUnionTypeDef,
     CreateFeaturedResultsSetResponseTypeDef,
     UpdateFeaturedResultsSetResponseTypeDef,
     AttributeSuggestionsGetConfigTypeDef,
     ListDataSourceSyncJobsResponseTypeDef,
     ListExperiencesResponseTypeDef,
     HookConfigurationOutputTypeDef,
     RetrieveResultItemTypeDef,
     SourceDocumentTypeDef,
     InlineCustomDocumentEnrichmentConfigurationOutputTypeDef,
-    HookConfigurationTypeDef,
-    InlineCustomDocumentEnrichmentConfigurationTypeDef,
-    AttributeFilterTypeDef,
-    DocumentInfoTypeDef,
-    DocumentTypeDef,
+    DocumentMetadataConfigurationUnionTypeDef,
     QueryRequestRequestTypeDef,
     RetrieveRequestRequestTypeDef,
     ListExperienceEntitiesResponseTypeDef,
     DescribeExperienceResponseTypeDef,
     CreateExperienceRequestRequestTypeDef,
+    ExperienceConfigurationUnionTypeDef,
     UpdateExperienceRequestRequestTypeDef,
     PutPrincipalMappingRequestRequestTypeDef,
     AdditionalResultAttributeValueTypeDef,
     CreateIndexRequestRequestTypeDef,
     DescribeIndexResponseTypeDef,
-    UpdateIndexRequestRequestTypeDef,
     WebCrawlerConfigurationOutputTypeDef,
     WebCrawlerConfigurationTypeDef,
     SuggestionValueTypeDef,
     TableExcerptTypeDef,
     SalesforceConfigurationOutputTypeDef,
     SalesforceConfigurationTypeDef,
+    HookConfigurationTypeDef,
+    InlineCustomDocumentEnrichmentConfigurationTypeDef,
+    AttributeFilterTypeDef,
+    DocumentInfoTypeDef,
+    DocumentTypeDef,
+    CreateAccessControlConfigurationRequestRequestTypeDef,
+    UpdateAccessControlConfigurationRequestRequestTypeDef,
     GetQuerySuggestionsRequestRequestTypeDef,
     RetrieveResultTypeDef,
     CustomDocumentEnrichmentConfigurationOutputTypeDef,
-    CustomDocumentEnrichmentConfigurationTypeDef,
-    BatchGetDocumentStatusRequestRequestTypeDef,
+    UpdateIndexRequestRequestTypeDef,
     AdditionalResultAttributeTypeDef,
     SuggestionTypeDef,
     DataSourceConfigurationOutputTypeDef,
     DataSourceConfigurationTypeDef,
-    BatchPutDocumentRequestRequestTypeDef,
+    CustomDocumentEnrichmentConfigurationTypeDef,
+    BatchGetDocumentStatusRequestRequestTypeDef,
     FeaturedResultsItemTypeDef,
     QueryResultItemTypeDef,
     GetQuerySuggestionsResponseTypeDef,
     DescribeDataSourceResponseTypeDef,
+    DataSourceConfigurationUnionTypeDef,
+    BatchPutDocumentRequestRequestTypeDef,
     CreateDataSourceRequestRequestTypeDef,
+    CustomDocumentEnrichmentConfigurationUnionTypeDef,
     UpdateDataSourceRequestRequestTypeDef,
     QueryResultTypeDef,
 )
 
 
-def get_structure() -> AccessControlConfigurationSummaryTypeDef:
+def get_value() -> AccessControlConfigurationSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kendra-1.28.15.post1/mypy_boto3_kendra.egg-info/SOURCES.txt` & `mypy-boto3-kendra-1.28.16/mypy_boto3_kendra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.28.15.post1/setup.py` & `mypy-boto3-kendra-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kendra",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_kendra"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.kendra 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.kendra 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 kendra type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 kendra type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_kendra": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

