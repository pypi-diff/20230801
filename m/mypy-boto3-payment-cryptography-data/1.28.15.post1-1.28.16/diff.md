# Comparing `tmp/mypy-boto3-payment-cryptography-data-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-payment-cryptography-data-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-payment-cryptography-data-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:51 2023, max compression
+gzip compressed data, was "mypy-boto3-payment-cryptography-data-1.28.16.tar", last modified: Tue Aug  1 11:37:30 2023, max compression
```

## Comparing `mypy-boto3-payment-cryptography-data-1.28.15.post1.tar` & `mypy-boto3-payment-cryptography-data-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:51.113329 mypy-boto3-payment-cryptography-data-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:52:53.000000 mypy-boto3-payment-cryptography-data-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-07-29 10:03:51.113329 mypy-boto3-payment-cryptography-data-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-07-29 09:52:53.000000 mypy-boto3-payment-cryptography-data-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:51.093329 mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-29 09:52:53.000000 mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-29 09:52:53.000000 mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-29 09:52:53.000000 mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-07-29 09:52:53.000000 mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-07-29 09:52:53.000000 mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-07-29 09:52:53.000000 mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-07-29 09:52:53.000000 mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:52:53.000000 mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24000 2023-07-29 09:52:57.000000 mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23976 2023-07-29 09:52:53.000000 mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:52:53.000000 mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:51.113329 mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-07-29 10:03:50.000000 mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-29 10:03:50.000000 mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:50.000000 mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:50.000000 mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:50.000000 mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-29 10:03:50.000000 mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:51.113329 mypy-boto3-payment-cryptography-data-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-29 09:52:53.000000 mypy-boto3-payment-cryptography-data-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:30.912795 mypy-boto3-payment-cryptography-data-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:25:54.000000 mypy-boto3-payment-cryptography-data-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-08-01 11:37:30.912795 mypy-boto3-payment-cryptography-data-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-08-01 11:25:54.000000 mypy-boto3-payment-cryptography-data-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:30.892795 mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-01 11:25:54.000000 mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-01 11:25:54.000000 mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-01 11:25:54.000000 mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-08-01 11:25:54.000000 mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-08-01 11:25:54.000000 mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-08-01 11:25:55.000000 mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-08-01 11:25:55.000000 mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:25:54.000000 mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-08-01 11:25:55.000000 mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23974 2023-08-01 11:25:55.000000 mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:25:54.000000 mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:30.912795 mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-08-01 11:37:30.000000 mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-01 11:37:30.000000 mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:30.000000 mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:30.000000 mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:30.000000 mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-01 11:37:30.000000 mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:30.912795 mypy-boto3-payment-cryptography-data-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-08-01 11:25:54.000000 mypy-boto3-payment-cryptography-data-1.28.16/setup.py
```

### Comparing `mypy-boto3-payment-cryptography-data-1.28.15.post1/LICENSE` & `mypy-boto3-payment-cryptography-data-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-data-1.28.15.post1/PKG-INFO` & `mypy-boto3-payment-cryptography-data-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-payment-cryptography-data
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.PaymentCryptographyDataPlane 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.PaymentCryptographyDataPlane 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 payment-cryptography-data type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 payment-cryptography-data type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-payment-cryptography-data)](https://pepy.tech/project/mypy-boto3-payment-cryptography-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PaymentCryptographyDataPlane 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
+[boto3.PaymentCryptographyDataPlane 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
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
 [mypy-boto3-payment-cryptography-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/).
 
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
@@ -296,20 +296,20 @@
 )
 
 
 def check_value(value: DukptDerivationTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_payment_cryptography_data.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_payment_cryptography_data.type_defs import (
     AmexCardSecurityCodeVersion1TypeDef,
     AmexCardSecurityCodeVersion2TypeDef,
     AsymmetricEncryptionAttributesTypeDef,
     CardHolderVerificationValueTypeDef,
@@ -374,15 +374,15 @@
     VerifyAuthRequestCryptogramInputRequestTypeDef,
     TranslatePinDataInputRequestTypeDef,
     GenerateMacInputRequestTypeDef,
     VerifyMacInputRequestTypeDef,
 )
 
 
-def get_structure() -> AmexCardSecurityCodeVersion1TypeDef:
+def get_value() -> AmexCardSecurityCodeVersion1TypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-payment-cryptography-data-1.28.15.post1/README.md` & `mypy-boto3-payment-cryptography-data-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-payment-cryptography-data)](https://pepy.tech/project/mypy-boto3-payment-cryptography-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PaymentCryptographyDataPlane 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
+[boto3.PaymentCryptographyDataPlane 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
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
 [mypy-boto3-payment-cryptography-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/).
 
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
@@ -264,20 +264,20 @@
 )
 
 
 def check_value(value: DukptDerivationTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_payment_cryptography_data.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_payment_cryptography_data.type_defs import (
     AmexCardSecurityCodeVersion1TypeDef,
     AmexCardSecurityCodeVersion2TypeDef,
     AsymmetricEncryptionAttributesTypeDef,
     CardHolderVerificationValueTypeDef,
@@ -342,15 +342,15 @@
     VerifyAuthRequestCryptogramInputRequestTypeDef,
     TranslatePinDataInputRequestTypeDef,
     GenerateMacInputRequestTypeDef,
     VerifyMacInputRequestTypeDef,
 )
 
 
-def get_structure() -> AmexCardSecurityCodeVersion1TypeDef:
+def get_value() -> AmexCardSecurityCodeVersion1TypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data/__init__.py` & `mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data/__init__.pyi` & `mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data/__main__.py` & `mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PaymentCryptographyDataPlane 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.PaymentCryptographyDataPlane 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane\nOther"
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

### Comparing `mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data/client.py` & `mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data/client.pyi` & `mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data/literals.py` & `mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data/literals.pyi` & `mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data/type_defs.py` & `mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_payment_cryptography_data.type_defs import AmexCardSecurityCodeVersion1TypeDef
 
-    data: AmexCardSecurityCodeVersion1TypeDef = {...}
+    data: AmexCardSecurityCodeVersion1TypeDef = ...
     ```
 """
 import sys
 from typing import Any, Dict, Mapping
 
 from .literals import (
     DukptDerivationTypeType,
```

### Comparing `mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data/type_defs.pyi` & `mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_payment_cryptography_data.type_defs import AmexCardSecurityCodeVersion1TypeDef
 
-    data: AmexCardSecurityCodeVersion1TypeDef = {...}
+    data: AmexCardSecurityCodeVersion1TypeDef = ...
     ```
 """
 import sys
 from typing import Any, Dict, Mapping
 
 from .literals import (
     DukptDerivationTypeType,
```

### Comparing `mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data.egg-info/PKG-INFO` & `mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-payment-cryptography-data
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.PaymentCryptographyDataPlane 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.PaymentCryptographyDataPlane 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 payment-cryptography-data type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 payment-cryptography-data type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-payment-cryptography-data)](https://pepy.tech/project/mypy-boto3-payment-cryptography-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PaymentCryptographyDataPlane 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
+[boto3.PaymentCryptographyDataPlane 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
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
 [mypy-boto3-payment-cryptography-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/).
 
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
@@ -296,20 +296,20 @@
 )
 
 
 def check_value(value: DukptDerivationTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_payment_cryptography_data.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_payment_cryptography_data.type_defs import (
     AmexCardSecurityCodeVersion1TypeDef,
     AmexCardSecurityCodeVersion2TypeDef,
     AsymmetricEncryptionAttributesTypeDef,
     CardHolderVerificationValueTypeDef,
@@ -374,15 +374,15 @@
     VerifyAuthRequestCryptogramInputRequestTypeDef,
     TranslatePinDataInputRequestTypeDef,
     GenerateMacInputRequestTypeDef,
     VerifyMacInputRequestTypeDef,
 )
 
 
-def get_structure() -> AmexCardSecurityCodeVersion1TypeDef:
+def get_value() -> AmexCardSecurityCodeVersion1TypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-payment-cryptography-data-1.28.15.post1/mypy_boto3_payment_cryptography_data.egg-info/SOURCES.txt` & `mypy-boto3-payment-cryptography-data-1.28.16/mypy_boto3_payment_cryptography_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-data-1.28.15.post1/setup.py` & `mypy-boto3-payment-cryptography-data-1.28.16/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-payment-cryptography-data",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_payment_cryptography_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PaymentCryptographyDataPlane 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.PaymentCryptographyDataPlane 1.28.16 service generated with"
+        " mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -34,17 +34,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
-    keywords=(
-        "boto3 payment-cryptography-data type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="boto3 payment-cryptography-data type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_payment_cryptography_data": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/"
```

