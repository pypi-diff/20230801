# Comparing `tmp/mypy-boto3-healthlake-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-healthlake-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-healthlake-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:15 2023, max compression
+gzip compressed data, was "mypy-boto3-healthlake-1.28.16.tar", last modified: Tue Aug  1 11:36:55 2023, max compression
```

## Comparing `mypy-boto3-healthlake-1.28.15.post1.tar` & `mypy-boto3-healthlake-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:14.977172 mypy-boto3-healthlake-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:46:52.000000 mypy-boto3-healthlake-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13510 2023-07-29 10:03:14.977172 mypy-boto3-healthlake-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-29 09:46:52.000000 mypy-boto3-healthlake-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:14.977172 mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-29 09:46:52.000000 mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-29 09:46:52.000000 mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:46:52.000000 mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-07-29 09:46:53.000000 mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-07-29 09:46:53.000000 mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-29 09:46:53.000000 mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-07-29 09:46:53.000000 mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:46:52.000000 mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14183 2023-07-29 09:46:53.000000 mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14162 2023-07-29 09:46:53.000000 mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:46:52.000000 mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:14.977172 mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13510 2023-07-29 10:03:14.000000 mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-29 10:03:14.000000 mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:14.000000 mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:14.000000 mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:14.000000 mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:03:14.000000 mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:14.997172 mypy-boto3-healthlake-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 09:46:52.000000 mypy-boto3-healthlake-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:55.448875 mypy-boto3-healthlake-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:19:31.000000 mypy-boto3-healthlake-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13522 2023-08-01 11:36:55.444875 mypy-boto3-healthlake-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-08-01 11:19:31.000000 mypy-boto3-healthlake-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:55.444875 mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-01 11:19:31.000000 mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-01 11:19:31.000000 mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 11:19:31.000000 mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-08-01 11:19:31.000000 mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-08-01 11:19:31.000000 mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-08-01 11:19:31.000000 mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-08-01 11:19:31.000000 mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:19:31.000000 mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14221 2023-08-01 11:19:32.000000 mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-08-01 11:19:32.000000 mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:19:31.000000 mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:55.444875 mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13522 2023-08-01 11:36:55.000000 mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-01 11:36:55.000000 mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:55.000000 mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:55.000000 mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:55.000000 mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 11:36:55.000000 mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:55.448875 mypy-boto3-healthlake-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-01 11:19:31.000000 mypy-boto3-healthlake-1.28.16/setup.py
```

### Comparing `mypy-boto3-healthlake-1.28.15.post1/LICENSE` & `mypy-boto3-healthlake-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-healthlake-1.28.15.post1/PKG-INFO` & `mypy-boto3-healthlake-1.28.16/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-healthlake
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.HealthLake 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.HealthLake 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 healthlake type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 healthlake type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-healthlake)](https://pepy.tech/project/mypy-boto3-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthLake 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[boto3.HealthLake 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
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
 [mypy-boto3-healthlake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/).
 
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
@@ -292,48 +292,49 @@
 )
 
 
 def check_value(value: AuthorizationStrategyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_healthlake.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_healthlake.type_defs import (
     IdentityProviderConfigurationTypeDef,
     PreloadDataConfigTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
-    DatastoreFilterTypeDef,
+    TimestampTypeDef,
     DeleteFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRExportJobRequestRequestTypeDef,
     DescribeFHIRImportJobRequestRequestTypeDef,
     InputDataConfigTypeDef,
     KmsEncryptionConfigTypeDef,
-    ListFHIRExportJobsRequestRequestTypeDef,
-    ListFHIRImportJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     S3ConfigurationTypeDef,
     UntagResourceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateFHIRDatastoreResponseTypeDef,
     DeleteFHIRDatastoreResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartFHIRExportJobResponseTypeDef,
     StartFHIRImportJobResponseTypeDef,
-    ListFHIRDatastoresRequestRequestTypeDef,
+    DatastoreFilterTypeDef,
+    ListFHIRExportJobsRequestRequestTypeDef,
+    ListFHIRImportJobsRequestRequestTypeDef,
     SseConfigurationTypeDef,
     OutputDataConfigTypeDef,
+    ListFHIRDatastoresRequestRequestTypeDef,
     CreateFHIRDatastoreRequestRequestTypeDef,
     DatastorePropertiesTypeDef,
     ExportJobPropertiesTypeDef,
     ImportJobPropertiesTypeDef,
     StartFHIRExportJobRequestRequestTypeDef,
     StartFHIRImportJobRequestRequestTypeDef,
     DescribeFHIRDatastoreResponseTypeDef,
@@ -341,15 +342,15 @@
     DescribeFHIRExportJobResponseTypeDef,
     ListFHIRExportJobsResponseTypeDef,
     DescribeFHIRImportJobResponseTypeDef,
     ListFHIRImportJobsResponseTypeDef,
 )
 
 
-def get_structure() -> IdentityProviderConfigurationTypeDef:
+def get_value() -> IdentityProviderConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-healthlake-1.28.15.post1/README.md` & `mypy-boto3-healthlake-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-healthlake)](https://pepy.tech/project/mypy-boto3-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthLake 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[boto3.HealthLake 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
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
 [mypy-boto3-healthlake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/).
 
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
@@ -260,48 +260,49 @@
 )
 
 
 def check_value(value: AuthorizationStrategyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_healthlake.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_healthlake.type_defs import (
     IdentityProviderConfigurationTypeDef,
     PreloadDataConfigTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
-    DatastoreFilterTypeDef,
+    TimestampTypeDef,
     DeleteFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRExportJobRequestRequestTypeDef,
     DescribeFHIRImportJobRequestRequestTypeDef,
     InputDataConfigTypeDef,
     KmsEncryptionConfigTypeDef,
-    ListFHIRExportJobsRequestRequestTypeDef,
-    ListFHIRImportJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     S3ConfigurationTypeDef,
     UntagResourceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateFHIRDatastoreResponseTypeDef,
     DeleteFHIRDatastoreResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartFHIRExportJobResponseTypeDef,
     StartFHIRImportJobResponseTypeDef,
-    ListFHIRDatastoresRequestRequestTypeDef,
+    DatastoreFilterTypeDef,
+    ListFHIRExportJobsRequestRequestTypeDef,
+    ListFHIRImportJobsRequestRequestTypeDef,
     SseConfigurationTypeDef,
     OutputDataConfigTypeDef,
+    ListFHIRDatastoresRequestRequestTypeDef,
     CreateFHIRDatastoreRequestRequestTypeDef,
     DatastorePropertiesTypeDef,
     ExportJobPropertiesTypeDef,
     ImportJobPropertiesTypeDef,
     StartFHIRExportJobRequestRequestTypeDef,
     StartFHIRImportJobRequestRequestTypeDef,
     DescribeFHIRDatastoreResponseTypeDef,
@@ -309,15 +310,15 @@
     DescribeFHIRExportJobResponseTypeDef,
     ListFHIRExportJobsResponseTypeDef,
     DescribeFHIRImportJobResponseTypeDef,
     ListFHIRImportJobsResponseTypeDef,
 )
 
 
-def get_structure() -> IdentityProviderConfigurationTypeDef:
+def get_value() -> IdentityProviderConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake/__main__.py` & `mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.HealthLake 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.HealthLake 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake\nOther"
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

### Comparing `mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake/client.py` & `mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_healthlake.client import HealthLakeClient
 
     session = Session()
     client: HealthLakeClient = session.client("healthlake")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import JobStatusType
 from .type_defs import (
     CreateFHIRDatastoreResponseTypeDef,
     DatastoreFilterTypeDef,
@@ -35,14 +34,15 @@
     ListTagsForResourceResponseTypeDef,
     OutputDataConfigTypeDef,
     PreloadDataConfigTypeDef,
     SseConfigurationTypeDef,
     StartFHIRExportJobResponseTypeDef,
     StartFHIRImportJobResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -188,16 +188,16 @@
         self,
         *,
         DatastoreId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         JobName: str = ...,
         JobStatus: JobStatusType = ...,
-        SubmittedBefore: Union[datetime, str] = ...,
-        SubmittedAfter: Union[datetime, str] = ...
+        SubmittedBefore: TimestampTypeDef = ...,
+        SubmittedAfter: TimestampTypeDef = ...
     ) -> ListFHIRExportJobsResponseTypeDef:
         """
         Lists all FHIR export jobs associated with an account and their statuses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_fhir_export_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#list_fhir_export_jobs)
         """
@@ -206,16 +206,16 @@
         self,
         *,
         DatastoreId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         JobName: str = ...,
         JobStatus: JobStatusType = ...,
-        SubmittedBefore: Union[datetime, str] = ...,
-        SubmittedAfter: Union[datetime, str] = ...
+        SubmittedBefore: TimestampTypeDef = ...,
+        SubmittedAfter: TimestampTypeDef = ...
     ) -> ListFHIRImportJobsResponseTypeDef:
         """
         Lists all FHIR import jobs associated with an account and their statuses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_fhir_import_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#list_fhir_import_jobs)
         """
```

### Comparing `mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake/client.pyi` & `mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_healthlake.client import HealthLakeClient
 
     session = Session()
     client: HealthLakeClient = session.client("healthlake")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import JobStatusType
 from .type_defs import (
     CreateFHIRDatastoreResponseTypeDef,
     DatastoreFilterTypeDef,
@@ -35,14 +34,15 @@
     ListTagsForResourceResponseTypeDef,
     OutputDataConfigTypeDef,
     PreloadDataConfigTypeDef,
     SseConfigurationTypeDef,
     StartFHIRExportJobResponseTypeDef,
     StartFHIRImportJobResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -174,16 +174,16 @@
         self,
         *,
         DatastoreId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         JobName: str = ...,
         JobStatus: JobStatusType = ...,
-        SubmittedBefore: Union[datetime, str] = ...,
-        SubmittedAfter: Union[datetime, str] = ...
+        SubmittedBefore: TimestampTypeDef = ...,
+        SubmittedAfter: TimestampTypeDef = ...
     ) -> ListFHIRExportJobsResponseTypeDef:
         """
         Lists all FHIR export jobs associated with an account and their statuses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_fhir_export_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#list_fhir_export_jobs)
         """
@@ -191,16 +191,16 @@
         self,
         *,
         DatastoreId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         JobName: str = ...,
         JobStatus: JobStatusType = ...,
-        SubmittedBefore: Union[datetime, str] = ...,
-        SubmittedAfter: Union[datetime, str] = ...
+        SubmittedBefore: TimestampTypeDef = ...,
+        SubmittedAfter: TimestampTypeDef = ...
     ) -> ListFHIRImportJobsResponseTypeDef:
         """
         Lists all FHIR import jobs associated with an account and their statuses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_fhir_import_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#list_fhir_import_jobs)
         """
```

### Comparing `mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake/literals.py` & `mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake/literals.pyi` & `mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake/type_defs.py` & `mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_healthlake.type_defs import IdentityProviderConfigurationTypeDef
 
-    data: IdentityProviderConfigurationTypeDef = {...}
+    data: IdentityProviderConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import AuthorizationStrategyType, CmkTypeType, DatastoreStatusType, JobStatusType
@@ -28,35 +28,36 @@
 
 
 __all__ = (
     "IdentityProviderConfigurationTypeDef",
     "PreloadDataConfigTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
-    "DatastoreFilterTypeDef",
+    "TimestampTypeDef",
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     "DescribeFHIRExportJobRequestRequestTypeDef",
     "DescribeFHIRImportJobRequestRequestTypeDef",
     "InputDataConfigTypeDef",
     "KmsEncryptionConfigTypeDef",
-    "ListFHIRExportJobsRequestRequestTypeDef",
-    "ListFHIRImportJobsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "S3ConfigurationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateFHIRDatastoreResponseTypeDef",
     "DeleteFHIRDatastoreResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartFHIRExportJobResponseTypeDef",
     "StartFHIRImportJobResponseTypeDef",
-    "ListFHIRDatastoresRequestRequestTypeDef",
+    "DatastoreFilterTypeDef",
+    "ListFHIRExportJobsRequestRequestTypeDef",
+    "ListFHIRImportJobsRequestRequestTypeDef",
     "SseConfigurationTypeDef",
     "OutputDataConfigTypeDef",
+    "ListFHIRDatastoresRequestRequestTypeDef",
     "CreateFHIRDatastoreRequestRequestTypeDef",
     "DatastorePropertiesTypeDef",
     "ExportJobPropertiesTypeDef",
     "ImportJobPropertiesTypeDef",
     "StartFHIRExportJobRequestRequestTypeDef",
     "StartFHIRImportJobRequestRequestTypeDef",
     "DescribeFHIRDatastoreResponseTypeDef",
@@ -112,25 +113,15 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-DatastoreFilterTypeDef = TypedDict(
-    "DatastoreFilterTypeDef",
-    {
-        "DatastoreName": str,
-        "DatastoreStatus": DatastoreStatusType,
-        "CreatedBefore": Union[datetime, str],
-        "CreatedAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 DeleteFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 
@@ -182,68 +173,14 @@
 
 class KmsEncryptionConfigTypeDef(
     _RequiredKmsEncryptionConfigTypeDef, _OptionalKmsEncryptionConfigTypeDef
 ):
     pass
 
 
-_RequiredListFHIRExportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFHIRExportJobsRequestRequestTypeDef",
-    {
-        "DatastoreId": str,
-    },
-)
-_OptionalListFHIRExportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFHIRExportJobsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmittedBefore": Union[datetime, str],
-        "SubmittedAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class ListFHIRExportJobsRequestRequestTypeDef(
-    _RequiredListFHIRExportJobsRequestRequestTypeDef,
-    _OptionalListFHIRExportJobsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredListFHIRImportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFHIRImportJobsRequestRequestTypeDef",
-    {
-        "DatastoreId": str,
-    },
-)
-_OptionalListFHIRImportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFHIRImportJobsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmittedBefore": Union[datetime, str],
-        "SubmittedAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class ListFHIRImportJobsRequestRequestTypeDef(
-    _RequiredListFHIRImportJobsRequestRequestTypeDef,
-    _OptionalListFHIRImportJobsRequestRequestTypeDef,
-):
-    pass
-
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
@@ -317,24 +254,79 @@
         "JobId": str,
         "JobStatus": JobStatusType,
         "DatastoreId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListFHIRDatastoresRequestRequestTypeDef = TypedDict(
-    "ListFHIRDatastoresRequestRequestTypeDef",
+DatastoreFilterTypeDef = TypedDict(
+    "DatastoreFilterTypeDef",
+    {
+        "DatastoreName": str,
+        "DatastoreStatus": DatastoreStatusType,
+        "CreatedBefore": TimestampTypeDef,
+        "CreatedAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFHIRExportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFHIRExportJobsRequestRequestTypeDef",
+    {
+        "DatastoreId": str,
+    },
+)
+_OptionalListFHIRExportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFHIRExportJobsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmittedBefore": TimestampTypeDef,
+        "SubmittedAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFHIRExportJobsRequestRequestTypeDef(
+    _RequiredListFHIRExportJobsRequestRequestTypeDef,
+    _OptionalListFHIRExportJobsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListFHIRImportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFHIRImportJobsRequestRequestTypeDef",
+    {
+        "DatastoreId": str,
+    },
+)
+_OptionalListFHIRImportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFHIRImportJobsRequestRequestTypeDef",
     {
-        "Filter": DatastoreFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmittedBefore": TimestampTypeDef,
+        "SubmittedAfter": TimestampTypeDef,
     },
     total=False,
 )
 
+
+class ListFHIRImportJobsRequestRequestTypeDef(
+    _RequiredListFHIRImportJobsRequestRequestTypeDef,
+    _OptionalListFHIRImportJobsRequestRequestTypeDef,
+):
+    pass
+
+
 SseConfigurationTypeDef = TypedDict(
     "SseConfigurationTypeDef",
     {
         "KmsEncryptionConfig": KmsEncryptionConfigTypeDef,
     },
 )
 
@@ -342,14 +334,24 @@
     "OutputDataConfigTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
     },
     total=False,
 )
 
+ListFHIRDatastoresRequestRequestTypeDef = TypedDict(
+    "ListFHIRDatastoresRequestRequestTypeDef",
+    {
+        "Filter": DatastoreFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 _RequiredCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreTypeVersion": Literal["R4"],
     },
 )
 _OptionalCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake/type_defs.pyi` & `mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_healthlake.type_defs import IdentityProviderConfigurationTypeDef
 
-    data: IdentityProviderConfigurationTypeDef = {...}
+    data: IdentityProviderConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import AuthorizationStrategyType, CmkTypeType, DatastoreStatusType, JobStatusType
@@ -27,35 +27,36 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "IdentityProviderConfigurationTypeDef",
     "PreloadDataConfigTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
-    "DatastoreFilterTypeDef",
+    "TimestampTypeDef",
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     "DescribeFHIRExportJobRequestRequestTypeDef",
     "DescribeFHIRImportJobRequestRequestTypeDef",
     "InputDataConfigTypeDef",
     "KmsEncryptionConfigTypeDef",
-    "ListFHIRExportJobsRequestRequestTypeDef",
-    "ListFHIRImportJobsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "S3ConfigurationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateFHIRDatastoreResponseTypeDef",
     "DeleteFHIRDatastoreResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartFHIRExportJobResponseTypeDef",
     "StartFHIRImportJobResponseTypeDef",
-    "ListFHIRDatastoresRequestRequestTypeDef",
+    "DatastoreFilterTypeDef",
+    "ListFHIRExportJobsRequestRequestTypeDef",
+    "ListFHIRImportJobsRequestRequestTypeDef",
     "SseConfigurationTypeDef",
     "OutputDataConfigTypeDef",
+    "ListFHIRDatastoresRequestRequestTypeDef",
     "CreateFHIRDatastoreRequestRequestTypeDef",
     "DatastorePropertiesTypeDef",
     "ExportJobPropertiesTypeDef",
     "ImportJobPropertiesTypeDef",
     "StartFHIRExportJobRequestRequestTypeDef",
     "StartFHIRImportJobRequestRequestTypeDef",
     "DescribeFHIRDatastoreResponseTypeDef",
@@ -109,25 +110,15 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-DatastoreFilterTypeDef = TypedDict(
-    "DatastoreFilterTypeDef",
-    {
-        "DatastoreName": str,
-        "DatastoreStatus": DatastoreStatusType,
-        "CreatedBefore": Union[datetime, str],
-        "CreatedAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 DeleteFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 
@@ -177,64 +168,14 @@
 )
 
 class KmsEncryptionConfigTypeDef(
     _RequiredKmsEncryptionConfigTypeDef, _OptionalKmsEncryptionConfigTypeDef
 ):
     pass
 
-_RequiredListFHIRExportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFHIRExportJobsRequestRequestTypeDef",
-    {
-        "DatastoreId": str,
-    },
-)
-_OptionalListFHIRExportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFHIRExportJobsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmittedBefore": Union[datetime, str],
-        "SubmittedAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-class ListFHIRExportJobsRequestRequestTypeDef(
-    _RequiredListFHIRExportJobsRequestRequestTypeDef,
-    _OptionalListFHIRExportJobsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredListFHIRImportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFHIRImportJobsRequestRequestTypeDef",
-    {
-        "DatastoreId": str,
-    },
-)
-_OptionalListFHIRImportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFHIRImportJobsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmittedBefore": Union[datetime, str],
-        "SubmittedAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-class ListFHIRImportJobsRequestRequestTypeDef(
-    _RequiredListFHIRImportJobsRequestRequestTypeDef,
-    _OptionalListFHIRImportJobsRequestRequestTypeDef,
-):
-    pass
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
@@ -308,24 +249,75 @@
         "JobId": str,
         "JobStatus": JobStatusType,
         "DatastoreId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListFHIRDatastoresRequestRequestTypeDef = TypedDict(
-    "ListFHIRDatastoresRequestRequestTypeDef",
+DatastoreFilterTypeDef = TypedDict(
+    "DatastoreFilterTypeDef",
+    {
+        "DatastoreName": str,
+        "DatastoreStatus": DatastoreStatusType,
+        "CreatedBefore": TimestampTypeDef,
+        "CreatedAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFHIRExportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFHIRExportJobsRequestRequestTypeDef",
+    {
+        "DatastoreId": str,
+    },
+)
+_OptionalListFHIRExportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFHIRExportJobsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmittedBefore": TimestampTypeDef,
+        "SubmittedAfter": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class ListFHIRExportJobsRequestRequestTypeDef(
+    _RequiredListFHIRExportJobsRequestRequestTypeDef,
+    _OptionalListFHIRExportJobsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListFHIRImportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFHIRImportJobsRequestRequestTypeDef",
+    {
+        "DatastoreId": str,
+    },
+)
+_OptionalListFHIRImportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFHIRImportJobsRequestRequestTypeDef",
     {
-        "Filter": DatastoreFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmittedBefore": TimestampTypeDef,
+        "SubmittedAfter": TimestampTypeDef,
     },
     total=False,
 )
 
+class ListFHIRImportJobsRequestRequestTypeDef(
+    _RequiredListFHIRImportJobsRequestRequestTypeDef,
+    _OptionalListFHIRImportJobsRequestRequestTypeDef,
+):
+    pass
+
 SseConfigurationTypeDef = TypedDict(
     "SseConfigurationTypeDef",
     {
         "KmsEncryptionConfig": KmsEncryptionConfigTypeDef,
     },
 )
 
@@ -333,14 +325,24 @@
     "OutputDataConfigTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
     },
     total=False,
 )
 
+ListFHIRDatastoresRequestRequestTypeDef = TypedDict(
+    "ListFHIRDatastoresRequestRequestTypeDef",
+    {
+        "Filter": DatastoreFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 _RequiredCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreTypeVersion": Literal["R4"],
     },
 )
 _OptionalCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake.egg-info/PKG-INFO` & `mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-healthlake
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.HealthLake 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.HealthLake 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 healthlake type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 healthlake type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-healthlake)](https://pepy.tech/project/mypy-boto3-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthLake 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[boto3.HealthLake 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
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
 [mypy-boto3-healthlake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/).
 
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
@@ -292,48 +292,49 @@
 )
 
 
 def check_value(value: AuthorizationStrategyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_healthlake.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_healthlake.type_defs import (
     IdentityProviderConfigurationTypeDef,
     PreloadDataConfigTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
-    DatastoreFilterTypeDef,
+    TimestampTypeDef,
     DeleteFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRExportJobRequestRequestTypeDef,
     DescribeFHIRImportJobRequestRequestTypeDef,
     InputDataConfigTypeDef,
     KmsEncryptionConfigTypeDef,
-    ListFHIRExportJobsRequestRequestTypeDef,
-    ListFHIRImportJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     S3ConfigurationTypeDef,
     UntagResourceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateFHIRDatastoreResponseTypeDef,
     DeleteFHIRDatastoreResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartFHIRExportJobResponseTypeDef,
     StartFHIRImportJobResponseTypeDef,
-    ListFHIRDatastoresRequestRequestTypeDef,
+    DatastoreFilterTypeDef,
+    ListFHIRExportJobsRequestRequestTypeDef,
+    ListFHIRImportJobsRequestRequestTypeDef,
     SseConfigurationTypeDef,
     OutputDataConfigTypeDef,
+    ListFHIRDatastoresRequestRequestTypeDef,
     CreateFHIRDatastoreRequestRequestTypeDef,
     DatastorePropertiesTypeDef,
     ExportJobPropertiesTypeDef,
     ImportJobPropertiesTypeDef,
     StartFHIRExportJobRequestRequestTypeDef,
     StartFHIRImportJobRequestRequestTypeDef,
     DescribeFHIRDatastoreResponseTypeDef,
@@ -341,15 +342,15 @@
     DescribeFHIRExportJobResponseTypeDef,
     ListFHIRExportJobsResponseTypeDef,
     DescribeFHIRImportJobResponseTypeDef,
     ListFHIRImportJobsResponseTypeDef,
 )
 
 
-def get_structure() -> IdentityProviderConfigurationTypeDef:
+def get_value() -> IdentityProviderConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-healthlake-1.28.15.post1/mypy_boto3_healthlake.egg-info/SOURCES.txt` & `mypy-boto3-healthlake-1.28.16/mypy_boto3_healthlake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-healthlake-1.28.15.post1/setup.py` & `mypy-boto3-healthlake-1.28.16/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-healthlake",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_healthlake"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.HealthLake 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.HealthLake 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 healthlake type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 healthlake type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_healthlake": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

