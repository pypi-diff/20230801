# Comparing `tmp/mypy-boto3-codeartifact-1.28.16.tar.gz` & `tmp/mypy-boto3-codeartifact-1.28.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codeartifact-1.28.16.tar", last modified: Tue Aug  1 11:36:25 2023, max compression
+gzip compressed data, was "mypy-boto3-codeartifact-1.28.4.tar", last modified: Tue Jul 18 01:01:41 2023, max compression
```

## Comparing `mypy-boto3-codeartifact-1.28.16.tar` & `mypy-boto3-codeartifact-1.28.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.644928 mypy-boto3-codeartifact-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:12:55.000000 mypy-boto3-codeartifact-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-08-01 11:36:25.636928 mypy-boto3-codeartifact-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16833 2023-08-01 11:12:55.000000 mypy-boto3-codeartifact-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.632928 mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-01 11:12:55.000000 mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-08-01 11:12:55.000000 mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 11:12:55.000000 mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34315 2023-08-01 11:12:56.000000 mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34264 2023-08-01 11:12:55.000000 mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-08-01 11:12:56.000000 mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-08-01 11:12:56.000000 mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-08-01 11:12:56.000000 mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8638 2023-08-01 11:12:56.000000 mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:12:55.000000 mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46891 2023-08-01 11:12:58.000000 mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46812 2023-08-01 11:12:58.000000 mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:12:55.000000 mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.636928 mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-08-01 11:36:25.000000 mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 11:36:25.000000 mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:25.000000 mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:25.000000 mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:25.000000 mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 11:36:25.000000 mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:25.644928 mypy-boto3-codeartifact-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 11:12:55.000000 mypy-boto3-codeartifact-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-codeartifact-1.28.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18403 2023-07-18 01:01:41.969310 mypy-boto3-codeartifact-1.28.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16898 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34383 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34332 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8638 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46438 2023-07-18 01:00:27.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46363 2023-07-18 01:00:26.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18403 2023-07-18 01:01:41.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-18 01:01:41.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 01:01:41.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-18 01:01:41.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:01:41.969310 mypy-boto3-codeartifact-1.28.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/setup.py
```

### Comparing `mypy-boto3-codeartifact-1.28.16/LICENSE` & `mypy-boto3-codeartifact-1.28.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.16/PKG-INFO` & `mypy-boto3-codeartifact-1.28.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeartifact
-Version: 1.28.16
-Summary: Type annotations for boto3.CodeArtifact 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.4
+Summary: Type annotations for boto3.CodeArtifact 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 codeartifact type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 codeartifact type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codeartifact"></a>
 
 # mypy-boto3-codeartifact
 
 [![PyPI - mypy-boto3-codeartifact](https://img.shields.io/pypi/v/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeartifact)](https://pepy.tech/project/mypy-boto3-codeartifact)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeartifact?color=blue)](https://pypistats.org/packages/mypy-boto3-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeArtifact 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
+[boto3.CodeArtifact 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeartifact docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +74,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -343,27 +343,26 @@
 )
 
 
 def check_value(value: AllowPublishType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_codeartifact.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeartifact.type_defs import (
     AssetSummaryTypeDef,
     AssociateExternalConnectionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    BlobTypeDef,
     CopyPackageVersionsRequestRequestTypeDef,
     PackageVersionErrorTypeDef,
     SuccessfulPackageVersionInfoTypeDef,
     TagTypeDef,
     DomainDescriptionTypeDef,
     UpstreamRepositoryTypeDef,
     DeleteDomainPermissionsPolicyRequestRequestTypeDef,
@@ -395,34 +394,35 @@
     PackageDependencyTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
     ListPackagesRequestRequestTypeDef,
     ListRepositoriesInDomainRequestRequestTypeDef,
     RepositorySummaryTypeDef,
     ListRepositoriesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    PackageOriginRestrictionsOutputTypeDef,
     PackageOriginRestrictionsTypeDef,
+    PublishPackageVersionRequestRequestTypeDef,
     PutDomainPermissionsPolicyRequestRequestTypeDef,
     PutRepositoryPermissionsPolicyRequestRequestTypeDef,
     RepositoryExternalConnectionInfoTypeDef,
     UpstreamRepositoryInfoTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePackageVersionsStatusRequestRequestTypeDef,
     GetAuthorizationTokenResultTypeDef,
     GetPackageVersionAssetResultTypeDef,
     GetPackageVersionReadmeResultTypeDef,
     GetRepositoryEndpointResultTypeDef,
     ListPackageVersionAssetsResultTypeDef,
     PublishPackageVersionResultTypeDef,
-    PublishPackageVersionRequestRequestTypeDef,
     CopyPackageVersionsResultTypeDef,
     DeletePackageVersionsResultTypeDef,
     DisposePackageVersionsResultTypeDef,
     UpdatePackageVersionsStatusResultTypeDef,
     CreateDomainRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDomainResultTypeDef,
     DeleteDomainResultTypeDef,
     DescribeDomainResultTypeDef,
     CreateRepositoryRequestRequestTypeDef,
     UpdateRepositoryRequestRequestTypeDef,
     DeleteDomainPermissionsPolicyResultTypeDef,
@@ -438,14 +438,15 @@
     ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
     ListPackagesRequestListPackagesPaginateTypeDef,
     ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
     ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListPackageVersionDependenciesResultTypeDef,
     ListRepositoriesInDomainResultTypeDef,
     ListRepositoriesResultTypeDef,
+    ListTagsForResourceResultTypeDef,
     PackageOriginConfigurationTypeDef,
     PutPackageOriginConfigurationRequestRequestTypeDef,
     RepositoryDescriptionTypeDef,
     PackageVersionDescriptionTypeDef,
     PackageVersionSummaryTypeDef,
     PackageDescriptionTypeDef,
     PackageSummaryTypeDef,
@@ -460,15 +461,15 @@
     ListPackageVersionsResultTypeDef,
     DescribePackageResultTypeDef,
     DeletePackageResultTypeDef,
     ListPackagesResultTypeDef,
 )
 
 
-def get_value() -> AssetSummaryTypeDef:
+def get_structure() -> AssetSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codeartifact-1.28.16/README.md` & `mypy-boto3-codeartifact-1.28.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codeartifact"></a>
 
 # mypy-boto3-codeartifact
 
 [![PyPI - mypy-boto3-codeartifact](https://img.shields.io/pypi/v/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeartifact)](https://pepy.tech/project/mypy-boto3-codeartifact)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeartifact?color=blue)](https://pypistats.org/packages/mypy-boto3-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeArtifact 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
+[boto3.CodeArtifact 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeartifact docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +42,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -311,27 +311,26 @@
 )
 
 
 def check_value(value: AllowPublishType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_codeartifact.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeartifact.type_defs import (
     AssetSummaryTypeDef,
     AssociateExternalConnectionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    BlobTypeDef,
     CopyPackageVersionsRequestRequestTypeDef,
     PackageVersionErrorTypeDef,
     SuccessfulPackageVersionInfoTypeDef,
     TagTypeDef,
     DomainDescriptionTypeDef,
     UpstreamRepositoryTypeDef,
     DeleteDomainPermissionsPolicyRequestRequestTypeDef,
@@ -363,34 +362,35 @@
     PackageDependencyTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
     ListPackagesRequestRequestTypeDef,
     ListRepositoriesInDomainRequestRequestTypeDef,
     RepositorySummaryTypeDef,
     ListRepositoriesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    PackageOriginRestrictionsOutputTypeDef,
     PackageOriginRestrictionsTypeDef,
+    PublishPackageVersionRequestRequestTypeDef,
     PutDomainPermissionsPolicyRequestRequestTypeDef,
     PutRepositoryPermissionsPolicyRequestRequestTypeDef,
     RepositoryExternalConnectionInfoTypeDef,
     UpstreamRepositoryInfoTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePackageVersionsStatusRequestRequestTypeDef,
     GetAuthorizationTokenResultTypeDef,
     GetPackageVersionAssetResultTypeDef,
     GetPackageVersionReadmeResultTypeDef,
     GetRepositoryEndpointResultTypeDef,
     ListPackageVersionAssetsResultTypeDef,
     PublishPackageVersionResultTypeDef,
-    PublishPackageVersionRequestRequestTypeDef,
     CopyPackageVersionsResultTypeDef,
     DeletePackageVersionsResultTypeDef,
     DisposePackageVersionsResultTypeDef,
     UpdatePackageVersionsStatusResultTypeDef,
     CreateDomainRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDomainResultTypeDef,
     DeleteDomainResultTypeDef,
     DescribeDomainResultTypeDef,
     CreateRepositoryRequestRequestTypeDef,
     UpdateRepositoryRequestRequestTypeDef,
     DeleteDomainPermissionsPolicyResultTypeDef,
@@ -406,14 +406,15 @@
     ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
     ListPackagesRequestListPackagesPaginateTypeDef,
     ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
     ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListPackageVersionDependenciesResultTypeDef,
     ListRepositoriesInDomainResultTypeDef,
     ListRepositoriesResultTypeDef,
+    ListTagsForResourceResultTypeDef,
     PackageOriginConfigurationTypeDef,
     PutPackageOriginConfigurationRequestRequestTypeDef,
     RepositoryDescriptionTypeDef,
     PackageVersionDescriptionTypeDef,
     PackageVersionSummaryTypeDef,
     PackageDescriptionTypeDef,
     PackageSummaryTypeDef,
@@ -428,15 +429,15 @@
     ListPackageVersionsResultTypeDef,
     DescribePackageResultTypeDef,
     DeletePackageResultTypeDef,
     ListPackagesResultTypeDef,
 )
 
 
-def get_value() -> AssetSummaryTypeDef:
+def get_structure() -> AssetSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/__init__.py` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/__init__.pyi` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/__main__.py` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeArtifact 1.28.16\nVersion:         1.28.16\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for boto3.CodeArtifact 1.28.4\nVersion:         1.28.4\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/client.py` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,18 @@
     from mypy_boto3_codeartifact.client import CodeArtifactClient
 
     session = Session()
     client: CodeArtifactClient = session.client("codeartifact")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
+from botocore.response import StreamingBody
 
 from .literals import (
     AllowPublishType,
     AllowUpstreamType,
     PackageFormatType,
     PackageVersionOriginTypeType,
     PackageVersionStatusType,
@@ -31,15 +32,14 @@
     ListPackageVersionAssetsPaginator,
     ListPackageVersionsPaginator,
     ListRepositoriesInDomainPaginator,
     ListRepositoriesPaginator,
 )
 from .type_defs import (
     AssociateExternalConnectionResultTypeDef,
-    BlobTypeDef,
     CopyPackageVersionsResultTypeDef,
     CreateDomainResultTypeDef,
     CreateRepositoryResultTypeDef,
     DeleteDomainPermissionsPolicyResultTypeDef,
     DeleteDomainResultTypeDef,
     DeletePackageResultTypeDef,
     DeletePackageVersionsResultTypeDef,
@@ -602,15 +602,15 @@
         self,
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
-        assetContent: BlobTypeDef,
+        assetContent: Union[str, bytes, IO[Any], StreamingBody],
         assetName: str,
         assetSHA256: str,
         domainOwner: str = ...,
         namespace: str = ...,
         unfinished: bool = ...
     ) -> PublishPackageVersionResultTypeDef:
         """
```

### Comparing `mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/client.pyi` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,18 @@
     from mypy_boto3_codeartifact.client import CodeArtifactClient
 
     session = Session()
     client: CodeArtifactClient = session.client("codeartifact")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
+from botocore.response import StreamingBody
 
 from .literals import (
     AllowPublishType,
     AllowUpstreamType,
     PackageFormatType,
     PackageVersionOriginTypeType,
     PackageVersionStatusType,
@@ -31,15 +32,14 @@
     ListPackageVersionAssetsPaginator,
     ListPackageVersionsPaginator,
     ListRepositoriesInDomainPaginator,
     ListRepositoriesPaginator,
 )
 from .type_defs import (
     AssociateExternalConnectionResultTypeDef,
-    BlobTypeDef,
     CopyPackageVersionsResultTypeDef,
     CreateDomainResultTypeDef,
     CreateRepositoryResultTypeDef,
     DeleteDomainPermissionsPolicyResultTypeDef,
     DeleteDomainResultTypeDef,
     DeletePackageResultTypeDef,
     DeletePackageVersionsResultTypeDef,
@@ -564,15 +564,15 @@
         self,
         *,
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
-        assetContent: BlobTypeDef,
+        assetContent: Union[str, bytes, IO[Any], StreamingBody],
         assetName: str,
         assetSHA256: str,
         domainOwner: str = ...,
         namespace: str = ...,
         unfinished: bool = ...
     ) -> PublishPackageVersionResultTypeDef:
         """
```

### Comparing `mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/literals.py` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -272,28 +271,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/literals.pyi` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -270,28 +269,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/paginator.py` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/paginator.pyi` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/type_defs.py` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_codeartifact.type_defs import AssetSummaryTypeDef
 
-    data: AssetSummaryTypeDef = ...
+    data: AssetSummaryTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -38,15 +38,14 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssetSummaryTypeDef",
     "AssociateExternalConnectionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "BlobTypeDef",
     "CopyPackageVersionsRequestRequestTypeDef",
     "PackageVersionErrorTypeDef",
     "SuccessfulPackageVersionInfoTypeDef",
     "TagTypeDef",
     "DomainDescriptionTypeDef",
     "UpstreamRepositoryTypeDef",
     "DeleteDomainPermissionsPolicyRequestRequestTypeDef",
@@ -78,34 +77,35 @@
     "PackageDependencyTypeDef",
     "ListPackageVersionsRequestRequestTypeDef",
     "ListPackagesRequestRequestTypeDef",
     "ListRepositoriesInDomainRequestRequestTypeDef",
     "RepositorySummaryTypeDef",
     "ListRepositoriesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "PackageOriginRestrictionsOutputTypeDef",
     "PackageOriginRestrictionsTypeDef",
+    "PublishPackageVersionRequestRequestTypeDef",
     "PutDomainPermissionsPolicyRequestRequestTypeDef",
     "PutRepositoryPermissionsPolicyRequestRequestTypeDef",
     "RepositoryExternalConnectionInfoTypeDef",
     "UpstreamRepositoryInfoTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePackageVersionsStatusRequestRequestTypeDef",
     "GetAuthorizationTokenResultTypeDef",
     "GetPackageVersionAssetResultTypeDef",
     "GetPackageVersionReadmeResultTypeDef",
     "GetRepositoryEndpointResultTypeDef",
     "ListPackageVersionAssetsResultTypeDef",
     "PublishPackageVersionResultTypeDef",
-    "PublishPackageVersionRequestRequestTypeDef",
     "CopyPackageVersionsResultTypeDef",
     "DeletePackageVersionsResultTypeDef",
     "DisposePackageVersionsResultTypeDef",
     "UpdatePackageVersionsStatusResultTypeDef",
     "CreateDomainRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDomainResultTypeDef",
     "DeleteDomainResultTypeDef",
     "DescribeDomainResultTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
     "UpdateRepositoryRequestRequestTypeDef",
     "DeleteDomainPermissionsPolicyResultTypeDef",
@@ -121,14 +121,15 @@
     "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
     "ListPackagesRequestListPackagesPaginateTypeDef",
     "ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
     "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
     "ListPackageVersionDependenciesResultTypeDef",
     "ListRepositoriesInDomainResultTypeDef",
     "ListRepositoriesResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "PackageOriginConfigurationTypeDef",
     "PutPackageOriginConfigurationRequestRequestTypeDef",
     "RepositoryDescriptionTypeDef",
     "PackageVersionDescriptionTypeDef",
     "PackageVersionSummaryTypeDef",
     "PackageDescriptionTypeDef",
     "PackageSummaryTypeDef",
@@ -142,34 +143,23 @@
     "DescribePackageVersionResultTypeDef",
     "ListPackageVersionsResultTypeDef",
     "DescribePackageResultTypeDef",
     "DeletePackageResultTypeDef",
     "ListPackagesResultTypeDef",
 )
 
-_RequiredAssetSummaryTypeDef = TypedDict(
-    "_RequiredAssetSummaryTypeDef",
+AssetSummaryTypeDef = TypedDict(
+    "AssetSummaryTypeDef",
     {
         "name": str,
-    },
-)
-_OptionalAssetSummaryTypeDef = TypedDict(
-    "_OptionalAssetSummaryTypeDef",
-    {
         "size": int,
         "hashes": Dict[HashAlgorithmType, str],
     },
-    total=False,
 )
 
-
-class AssetSummaryTypeDef(_RequiredAssetSummaryTypeDef, _OptionalAssetSummaryTypeDef):
-    pass
-
-
 _RequiredAssociateExternalConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateExternalConnectionRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "externalConnection": str,
     },
@@ -197,15 +187,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredCopyPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredCopyPackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "sourceRepository": str,
         "destinationRepository": str,
         "format": PackageFormatType,
@@ -235,24 +224,22 @@
 
 PackageVersionErrorTypeDef = TypedDict(
     "PackageVersionErrorTypeDef",
     {
         "errorCode": PackageVersionErrorCodeType,
         "errorMessage": str,
     },
-    total=False,
 )
 
 SuccessfulPackageVersionInfoTypeDef = TypedDict(
     "SuccessfulPackageVersionInfoTypeDef",
     {
         "revision": str,
         "status": PackageVersionStatusType,
     },
-    total=False,
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
@@ -268,15 +255,14 @@
         "status": DomainStatusType,
         "createdTime": datetime,
         "encryptionKey": str,
         "repositoryCount": int,
         "assetSizeBytes": int,
         "s3BucketArn": str,
     },
-    total=False,
 )
 
 UpstreamRepositoryTypeDef = TypedDict(
     "UpstreamRepositoryTypeDef",
     {
         "repositoryName": str,
     },
@@ -308,15 +294,14 @@
 ResourcePolicyTypeDef = TypedDict(
     "ResourcePolicyTypeDef",
     {
         "resourceArn": str,
         "revision": str,
         "document": str,
     },
-    total=False,
 )
 
 _RequiredDeleteDomainRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDomainRequestRequestTypeDef",
     {
         "domain": str,
     },
@@ -586,28 +571,26 @@
 
 DomainEntryPointTypeDef = TypedDict(
     "DomainEntryPointTypeDef",
     {
         "repositoryName": str,
         "externalConnectionName": str,
     },
-    total=False,
 )
 
 DomainSummaryTypeDef = TypedDict(
     "DomainSummaryTypeDef",
     {
         "name": str,
         "owner": str,
         "arn": str,
         "status": DomainStatusType,
         "createdTime": datetime,
         "encryptionKey": str,
     },
-    total=False,
 )
 
 _RequiredGetAuthorizationTokenRequestRequestTypeDef = TypedDict(
     "_RequiredGetAuthorizationTokenRequestRequestTypeDef",
     {
         "domain": str,
     },
@@ -756,15 +739,14 @@
 
 LicenseInfoTypeDef = TypedDict(
     "LicenseInfoTypeDef",
     {
         "name": str,
         "url": str,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -843,15 +825,14 @@
     "PackageDependencyTypeDef",
     {
         "namespace": str,
         "package": str,
         "dependencyType": str,
         "versionRequirement": str,
     },
-    total=False,
 )
 
 _RequiredListPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
@@ -943,15 +924,14 @@
         "administratorAccount": str,
         "domainName": str,
         "domainOwner": str,
         "arn": str,
         "description": str,
         "createdTime": datetime,
     },
-    total=False,
 )
 
 ListRepositoriesRequestRequestTypeDef = TypedDict(
     "ListRepositoriesRequestRequestTypeDef",
     {
         "repositoryPrefix": str,
         "maxResults": int,
@@ -963,22 +943,69 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
+PackageOriginRestrictionsOutputTypeDef = TypedDict(
+    "PackageOriginRestrictionsOutputTypeDef",
+    {
+        "publish": AllowPublishType,
+        "upstream": AllowUpstreamType,
+    },
+)
+
 PackageOriginRestrictionsTypeDef = TypedDict(
     "PackageOriginRestrictionsTypeDef",
     {
         "publish": AllowPublishType,
         "upstream": AllowUpstreamType,
     },
 )
 
+_RequiredPublishPackageVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredPublishPackageVersionRequestRequestTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+        "format": PackageFormatType,
+        "package": str,
+        "packageVersion": str,
+        "assetContent": Union[str, bytes, IO[Any], StreamingBody],
+        "assetName": str,
+        "assetSHA256": str,
+    },
+)
+_OptionalPublishPackageVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalPublishPackageVersionRequestRequestTypeDef",
+    {
+        "domainOwner": str,
+        "namespace": str,
+        "unfinished": bool,
+    },
+    total=False,
+)
+
+
+class PublishPackageVersionRequestRequestTypeDef(
+    _RequiredPublishPackageVersionRequestRequestTypeDef,
+    _OptionalPublishPackageVersionRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredPutDomainPermissionsPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutDomainPermissionsPolicyRequestRequestTypeDef",
     {
         "domain": str,
         "policyDocument": str,
     },
 )
@@ -1027,23 +1054,21 @@
 RepositoryExternalConnectionInfoTypeDef = TypedDict(
     "RepositoryExternalConnectionInfoTypeDef",
     {
         "externalConnectionName": str,
         "packageFormat": PackageFormatType,
         "status": Literal["Available"],
     },
-    total=False,
 )
 
 UpstreamRepositoryInfoTypeDef = TypedDict(
     "UpstreamRepositoryInfoTypeDef",
     {
         "repositoryName": str,
     },
-    total=False,
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
@@ -1145,45 +1170,14 @@
         "versionRevision": str,
         "status": PackageVersionStatusType,
         "asset": AssetSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPublishPackageVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredPublishPackageVersionRequestRequestTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-        "format": PackageFormatType,
-        "package": str,
-        "packageVersion": str,
-        "assetContent": BlobTypeDef,
-        "assetName": str,
-        "assetSHA256": str,
-    },
-)
-_OptionalPublishPackageVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalPublishPackageVersionRequestRequestTypeDef",
-    {
-        "domainOwner": str,
-        "namespace": str,
-        "unfinished": bool,
-    },
-    total=False,
-)
-
-
-class PublishPackageVersionRequestRequestTypeDef(
-    _RequiredPublishPackageVersionRequestRequestTypeDef,
-    _OptionalPublishPackageVersionRequestRequestTypeDef,
-):
-    pass
-
-
 CopyPackageVersionsResultTypeDef = TypedDict(
     "CopyPackageVersionsResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1234,22 +1228,14 @@
 
 class CreateDomainRequestRequestTypeDef(
     _RequiredCreateDomainRequestRequestTypeDef, _OptionalCreateDomainRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1377,15 +1363,14 @@
 
 PackageVersionOriginTypeDef = TypedDict(
     "PackageVersionOriginTypeDef",
     {
         "domainEntryPoint": DomainEntryPointTypeDef,
         "originType": PackageVersionOriginTypeType,
     },
-    total=False,
 )
 
 ListDomainsResultTypeDef = TypedDict(
     "ListDomainsResultTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
@@ -1550,20 +1535,27 @@
     {
         "repositories": List[RepositorySummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PackageOriginConfigurationTypeDef = TypedDict(
     "PackageOriginConfigurationTypeDef",
     {
-        "restrictions": PackageOriginRestrictionsTypeDef,
+        "restrictions": PackageOriginRestrictionsOutputTypeDef,
     },
-    total=False,
 )
 
 _RequiredPutPackageOriginConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutPackageOriginConfigurationRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
@@ -1598,15 +1590,14 @@
         "domainOwner": str,
         "arn": str,
         "description": str,
         "upstreams": List[UpstreamRepositoryInfoTypeDef],
         "externalConnections": List[RepositoryExternalConnectionInfoTypeDef],
         "createdTime": datetime,
     },
-    total=False,
 )
 
 PackageVersionDescriptionTypeDef = TypedDict(
     "PackageVersionDescriptionTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
@@ -1618,60 +1609,44 @@
         "sourceCodeRepository": str,
         "publishedTime": datetime,
         "licenses": List[LicenseInfoTypeDef],
         "revision": str,
         "status": PackageVersionStatusType,
         "origin": PackageVersionOriginTypeDef,
     },
-    total=False,
 )
 
-_RequiredPackageVersionSummaryTypeDef = TypedDict(
-    "_RequiredPackageVersionSummaryTypeDef",
+PackageVersionSummaryTypeDef = TypedDict(
+    "PackageVersionSummaryTypeDef",
     {
         "version": str,
-        "status": PackageVersionStatusType,
-    },
-)
-_OptionalPackageVersionSummaryTypeDef = TypedDict(
-    "_OptionalPackageVersionSummaryTypeDef",
-    {
         "revision": str,
+        "status": PackageVersionStatusType,
         "origin": PackageVersionOriginTypeDef,
     },
-    total=False,
 )
 
-
-class PackageVersionSummaryTypeDef(
-    _RequiredPackageVersionSummaryTypeDef, _OptionalPackageVersionSummaryTypeDef
-):
-    pass
-
-
 PackageDescriptionTypeDef = TypedDict(
     "PackageDescriptionTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "name": str,
         "originConfiguration": PackageOriginConfigurationTypeDef,
     },
-    total=False,
 )
 
 PackageSummaryTypeDef = TypedDict(
     "PackageSummaryTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "originConfiguration": PackageOriginConfigurationTypeDef,
     },
-    total=False,
 )
 
 PutPackageOriginConfigurationResultTypeDef = TypedDict(
     "PutPackageOriginConfigurationResultTypeDef",
     {
         "originConfiguration": PackageOriginConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact/type_defs.pyi` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_codeartifact.type_defs import AssetSummaryTypeDef
 
-    data: AssetSummaryTypeDef = ...
+    data: AssetSummaryTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -37,15 +37,14 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssetSummaryTypeDef",
     "AssociateExternalConnectionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "BlobTypeDef",
     "CopyPackageVersionsRequestRequestTypeDef",
     "PackageVersionErrorTypeDef",
     "SuccessfulPackageVersionInfoTypeDef",
     "TagTypeDef",
     "DomainDescriptionTypeDef",
     "UpstreamRepositoryTypeDef",
     "DeleteDomainPermissionsPolicyRequestRequestTypeDef",
@@ -77,34 +76,35 @@
     "PackageDependencyTypeDef",
     "ListPackageVersionsRequestRequestTypeDef",
     "ListPackagesRequestRequestTypeDef",
     "ListRepositoriesInDomainRequestRequestTypeDef",
     "RepositorySummaryTypeDef",
     "ListRepositoriesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "PackageOriginRestrictionsOutputTypeDef",
     "PackageOriginRestrictionsTypeDef",
+    "PublishPackageVersionRequestRequestTypeDef",
     "PutDomainPermissionsPolicyRequestRequestTypeDef",
     "PutRepositoryPermissionsPolicyRequestRequestTypeDef",
     "RepositoryExternalConnectionInfoTypeDef",
     "UpstreamRepositoryInfoTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePackageVersionsStatusRequestRequestTypeDef",
     "GetAuthorizationTokenResultTypeDef",
     "GetPackageVersionAssetResultTypeDef",
     "GetPackageVersionReadmeResultTypeDef",
     "GetRepositoryEndpointResultTypeDef",
     "ListPackageVersionAssetsResultTypeDef",
     "PublishPackageVersionResultTypeDef",
-    "PublishPackageVersionRequestRequestTypeDef",
     "CopyPackageVersionsResultTypeDef",
     "DeletePackageVersionsResultTypeDef",
     "DisposePackageVersionsResultTypeDef",
     "UpdatePackageVersionsStatusResultTypeDef",
     "CreateDomainRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDomainResultTypeDef",
     "DeleteDomainResultTypeDef",
     "DescribeDomainResultTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
     "UpdateRepositoryRequestRequestTypeDef",
     "DeleteDomainPermissionsPolicyResultTypeDef",
@@ -120,14 +120,15 @@
     "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
     "ListPackagesRequestListPackagesPaginateTypeDef",
     "ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
     "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
     "ListPackageVersionDependenciesResultTypeDef",
     "ListRepositoriesInDomainResultTypeDef",
     "ListRepositoriesResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "PackageOriginConfigurationTypeDef",
     "PutPackageOriginConfigurationRequestRequestTypeDef",
     "RepositoryDescriptionTypeDef",
     "PackageVersionDescriptionTypeDef",
     "PackageVersionSummaryTypeDef",
     "PackageDescriptionTypeDef",
     "PackageSummaryTypeDef",
@@ -141,32 +142,23 @@
     "DescribePackageVersionResultTypeDef",
     "ListPackageVersionsResultTypeDef",
     "DescribePackageResultTypeDef",
     "DeletePackageResultTypeDef",
     "ListPackagesResultTypeDef",
 )
 
-_RequiredAssetSummaryTypeDef = TypedDict(
-    "_RequiredAssetSummaryTypeDef",
+AssetSummaryTypeDef = TypedDict(
+    "AssetSummaryTypeDef",
     {
         "name": str,
-    },
-)
-_OptionalAssetSummaryTypeDef = TypedDict(
-    "_OptionalAssetSummaryTypeDef",
-    {
         "size": int,
         "hashes": Dict[HashAlgorithmType, str],
     },
-    total=False,
 )
 
-class AssetSummaryTypeDef(_RequiredAssetSummaryTypeDef, _OptionalAssetSummaryTypeDef):
-    pass
-
 _RequiredAssociateExternalConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateExternalConnectionRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "externalConnection": str,
     },
@@ -192,15 +184,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredCopyPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredCopyPackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "sourceRepository": str,
         "destinationRepository": str,
         "format": PackageFormatType,
@@ -228,24 +219,22 @@
 
 PackageVersionErrorTypeDef = TypedDict(
     "PackageVersionErrorTypeDef",
     {
         "errorCode": PackageVersionErrorCodeType,
         "errorMessage": str,
     },
-    total=False,
 )
 
 SuccessfulPackageVersionInfoTypeDef = TypedDict(
     "SuccessfulPackageVersionInfoTypeDef",
     {
         "revision": str,
         "status": PackageVersionStatusType,
     },
-    total=False,
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
@@ -261,15 +250,14 @@
         "status": DomainStatusType,
         "createdTime": datetime,
         "encryptionKey": str,
         "repositoryCount": int,
         "assetSizeBytes": int,
         "s3BucketArn": str,
     },
-    total=False,
 )
 
 UpstreamRepositoryTypeDef = TypedDict(
     "UpstreamRepositoryTypeDef",
     {
         "repositoryName": str,
     },
@@ -299,15 +287,14 @@
 ResourcePolicyTypeDef = TypedDict(
     "ResourcePolicyTypeDef",
     {
         "resourceArn": str,
         "revision": str,
         "document": str,
     },
-    total=False,
 )
 
 _RequiredDeleteDomainRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDomainRequestRequestTypeDef",
     {
         "domain": str,
     },
@@ -555,28 +542,26 @@
 
 DomainEntryPointTypeDef = TypedDict(
     "DomainEntryPointTypeDef",
     {
         "repositoryName": str,
         "externalConnectionName": str,
     },
-    total=False,
 )
 
 DomainSummaryTypeDef = TypedDict(
     "DomainSummaryTypeDef",
     {
         "name": str,
         "owner": str,
         "arn": str,
         "status": DomainStatusType,
         "createdTime": datetime,
         "encryptionKey": str,
     },
-    total=False,
 )
 
 _RequiredGetAuthorizationTokenRequestRequestTypeDef = TypedDict(
     "_RequiredGetAuthorizationTokenRequestRequestTypeDef",
     {
         "domain": str,
     },
@@ -713,15 +698,14 @@
 
 LicenseInfoTypeDef = TypedDict(
     "LicenseInfoTypeDef",
     {
         "name": str,
         "url": str,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -796,15 +780,14 @@
     "PackageDependencyTypeDef",
     {
         "namespace": str,
         "package": str,
         "dependencyType": str,
         "versionRequirement": str,
     },
-    total=False,
 )
 
 _RequiredListPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
@@ -890,15 +873,14 @@
         "administratorAccount": str,
         "domainName": str,
         "domainOwner": str,
         "arn": str,
         "description": str,
         "createdTime": datetime,
     },
-    total=False,
 )
 
 ListRepositoriesRequestRequestTypeDef = TypedDict(
     "ListRepositoriesRequestRequestTypeDef",
     {
         "repositoryPrefix": str,
         "maxResults": int,
@@ -910,22 +892,67 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
+PackageOriginRestrictionsOutputTypeDef = TypedDict(
+    "PackageOriginRestrictionsOutputTypeDef",
+    {
+        "publish": AllowPublishType,
+        "upstream": AllowUpstreamType,
+    },
+)
+
 PackageOriginRestrictionsTypeDef = TypedDict(
     "PackageOriginRestrictionsTypeDef",
     {
         "publish": AllowPublishType,
         "upstream": AllowUpstreamType,
     },
 )
 
+_RequiredPublishPackageVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredPublishPackageVersionRequestRequestTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+        "format": PackageFormatType,
+        "package": str,
+        "packageVersion": str,
+        "assetContent": Union[str, bytes, IO[Any], StreamingBody],
+        "assetName": str,
+        "assetSHA256": str,
+    },
+)
+_OptionalPublishPackageVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalPublishPackageVersionRequestRequestTypeDef",
+    {
+        "domainOwner": str,
+        "namespace": str,
+        "unfinished": bool,
+    },
+    total=False,
+)
+
+class PublishPackageVersionRequestRequestTypeDef(
+    _RequiredPublishPackageVersionRequestRequestTypeDef,
+    _OptionalPublishPackageVersionRequestRequestTypeDef,
+):
+    pass
+
 _RequiredPutDomainPermissionsPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutDomainPermissionsPolicyRequestRequestTypeDef",
     {
         "domain": str,
         "policyDocument": str,
     },
 )
@@ -970,23 +997,21 @@
 RepositoryExternalConnectionInfoTypeDef = TypedDict(
     "RepositoryExternalConnectionInfoTypeDef",
     {
         "externalConnectionName": str,
         "packageFormat": PackageFormatType,
         "status": Literal["Available"],
     },
-    total=False,
 )
 
 UpstreamRepositoryInfoTypeDef = TypedDict(
     "UpstreamRepositoryInfoTypeDef",
     {
         "repositoryName": str,
     },
-    total=False,
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
@@ -1086,43 +1111,14 @@
         "versionRevision": str,
         "status": PackageVersionStatusType,
         "asset": AssetSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPublishPackageVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredPublishPackageVersionRequestRequestTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-        "format": PackageFormatType,
-        "package": str,
-        "packageVersion": str,
-        "assetContent": BlobTypeDef,
-        "assetName": str,
-        "assetSHA256": str,
-    },
-)
-_OptionalPublishPackageVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalPublishPackageVersionRequestRequestTypeDef",
-    {
-        "domainOwner": str,
-        "namespace": str,
-        "unfinished": bool,
-    },
-    total=False,
-)
-
-class PublishPackageVersionRequestRequestTypeDef(
-    _RequiredPublishPackageVersionRequestRequestTypeDef,
-    _OptionalPublishPackageVersionRequestRequestTypeDef,
-):
-    pass
-
 CopyPackageVersionsResultTypeDef = TypedDict(
     "CopyPackageVersionsResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1171,22 +1167,14 @@
 )
 
 class CreateDomainRequestRequestTypeDef(
     _RequiredCreateDomainRequestRequestTypeDef, _OptionalCreateDomainRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1310,15 +1298,14 @@
 
 PackageVersionOriginTypeDef = TypedDict(
     "PackageVersionOriginTypeDef",
     {
         "domainEntryPoint": DomainEntryPointTypeDef,
         "originType": PackageVersionOriginTypeType,
     },
-    total=False,
 )
 
 ListDomainsResultTypeDef = TypedDict(
     "ListDomainsResultTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
@@ -1475,20 +1462,27 @@
     {
         "repositories": List[RepositorySummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PackageOriginConfigurationTypeDef = TypedDict(
     "PackageOriginConfigurationTypeDef",
     {
-        "restrictions": PackageOriginRestrictionsTypeDef,
+        "restrictions": PackageOriginRestrictionsOutputTypeDef,
     },
-    total=False,
 )
 
 _RequiredPutPackageOriginConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutPackageOriginConfigurationRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
@@ -1521,15 +1515,14 @@
         "domainOwner": str,
         "arn": str,
         "description": str,
         "upstreams": List[UpstreamRepositoryInfoTypeDef],
         "externalConnections": List[RepositoryExternalConnectionInfoTypeDef],
         "createdTime": datetime,
     },
-    total=False,
 )
 
 PackageVersionDescriptionTypeDef = TypedDict(
     "PackageVersionDescriptionTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
@@ -1541,58 +1534,44 @@
         "sourceCodeRepository": str,
         "publishedTime": datetime,
         "licenses": List[LicenseInfoTypeDef],
         "revision": str,
         "status": PackageVersionStatusType,
         "origin": PackageVersionOriginTypeDef,
     },
-    total=False,
 )
 
-_RequiredPackageVersionSummaryTypeDef = TypedDict(
-    "_RequiredPackageVersionSummaryTypeDef",
+PackageVersionSummaryTypeDef = TypedDict(
+    "PackageVersionSummaryTypeDef",
     {
         "version": str,
-        "status": PackageVersionStatusType,
-    },
-)
-_OptionalPackageVersionSummaryTypeDef = TypedDict(
-    "_OptionalPackageVersionSummaryTypeDef",
-    {
         "revision": str,
+        "status": PackageVersionStatusType,
         "origin": PackageVersionOriginTypeDef,
     },
-    total=False,
 )
 
-class PackageVersionSummaryTypeDef(
-    _RequiredPackageVersionSummaryTypeDef, _OptionalPackageVersionSummaryTypeDef
-):
-    pass
-
 PackageDescriptionTypeDef = TypedDict(
     "PackageDescriptionTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "name": str,
         "originConfiguration": PackageOriginConfigurationTypeDef,
     },
-    total=False,
 )
 
 PackageSummaryTypeDef = TypedDict(
     "PackageSummaryTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "originConfiguration": PackageOriginConfigurationTypeDef,
     },
-    total=False,
 )
 
 PutPackageOriginConfigurationResultTypeDef = TypedDict(
     "PutPackageOriginConfigurationResultTypeDef",
     {
         "originConfiguration": PackageOriginConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact.egg-info/PKG-INFO` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeartifact
-Version: 1.28.16
-Summary: Type annotations for boto3.CodeArtifact 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.4
+Summary: Type annotations for boto3.CodeArtifact 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 codeartifact type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 codeartifact type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codeartifact"></a>
 
 # mypy-boto3-codeartifact
 
 [![PyPI - mypy-boto3-codeartifact](https://img.shields.io/pypi/v/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeartifact)](https://pepy.tech/project/mypy-boto3-codeartifact)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeartifact?color=blue)](https://pypistats.org/packages/mypy-boto3-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeArtifact 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
+[boto3.CodeArtifact 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeartifact docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +74,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -343,27 +343,26 @@
 )
 
 
 def check_value(value: AllowPublishType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_codeartifact.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeartifact.type_defs import (
     AssetSummaryTypeDef,
     AssociateExternalConnectionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    BlobTypeDef,
     CopyPackageVersionsRequestRequestTypeDef,
     PackageVersionErrorTypeDef,
     SuccessfulPackageVersionInfoTypeDef,
     TagTypeDef,
     DomainDescriptionTypeDef,
     UpstreamRepositoryTypeDef,
     DeleteDomainPermissionsPolicyRequestRequestTypeDef,
@@ -395,34 +394,35 @@
     PackageDependencyTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
     ListPackagesRequestRequestTypeDef,
     ListRepositoriesInDomainRequestRequestTypeDef,
     RepositorySummaryTypeDef,
     ListRepositoriesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    PackageOriginRestrictionsOutputTypeDef,
     PackageOriginRestrictionsTypeDef,
+    PublishPackageVersionRequestRequestTypeDef,
     PutDomainPermissionsPolicyRequestRequestTypeDef,
     PutRepositoryPermissionsPolicyRequestRequestTypeDef,
     RepositoryExternalConnectionInfoTypeDef,
     UpstreamRepositoryInfoTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePackageVersionsStatusRequestRequestTypeDef,
     GetAuthorizationTokenResultTypeDef,
     GetPackageVersionAssetResultTypeDef,
     GetPackageVersionReadmeResultTypeDef,
     GetRepositoryEndpointResultTypeDef,
     ListPackageVersionAssetsResultTypeDef,
     PublishPackageVersionResultTypeDef,
-    PublishPackageVersionRequestRequestTypeDef,
     CopyPackageVersionsResultTypeDef,
     DeletePackageVersionsResultTypeDef,
     DisposePackageVersionsResultTypeDef,
     UpdatePackageVersionsStatusResultTypeDef,
     CreateDomainRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDomainResultTypeDef,
     DeleteDomainResultTypeDef,
     DescribeDomainResultTypeDef,
     CreateRepositoryRequestRequestTypeDef,
     UpdateRepositoryRequestRequestTypeDef,
     DeleteDomainPermissionsPolicyResultTypeDef,
@@ -438,14 +438,15 @@
     ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
     ListPackagesRequestListPackagesPaginateTypeDef,
     ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
     ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListPackageVersionDependenciesResultTypeDef,
     ListRepositoriesInDomainResultTypeDef,
     ListRepositoriesResultTypeDef,
+    ListTagsForResourceResultTypeDef,
     PackageOriginConfigurationTypeDef,
     PutPackageOriginConfigurationRequestRequestTypeDef,
     RepositoryDescriptionTypeDef,
     PackageVersionDescriptionTypeDef,
     PackageVersionSummaryTypeDef,
     PackageDescriptionTypeDef,
     PackageSummaryTypeDef,
@@ -460,15 +461,15 @@
     ListPackageVersionsResultTypeDef,
     DescribePackageResultTypeDef,
     DeletePackageResultTypeDef,
     ListPackagesResultTypeDef,
 )
 
 
-def get_value() -> AssetSummaryTypeDef:
+def get_structure() -> AssetSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codeartifact-1.28.16/mypy_boto3_codeartifact.egg-info/SOURCES.txt` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.16/setup.py` & `mypy-boto3-codeartifact-1.28.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codeartifact",
-    version="1.28.16",
+    version="1.28.4",
     packages=["mypy_boto3_codeartifact"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeArtifact 1.28.16 service generated with mypy-boto3-builder"
-        " 7.17.1"
+        "Type annotations for boto3.CodeArtifact 1.28.4 service generated with mypy-boto3-builder"
+        " 7.15.1"
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
-    keywords="boto3 codeartifact type-annotations botocore mypy typeshed autocomplete",
+    keywords="boto3 codeartifact type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_codeartifact": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

