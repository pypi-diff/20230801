# Comparing `tmp/mypy-boto3-drs-1.28.16.tar.gz` & `tmp/mypy-boto3-drs-1.28.16.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-drs-1.28.16.tar", last modified: Mon Jul 31 19:32:46 2023, max compression
+gzip compressed data, was "mypy-boto3-drs-1.28.16.post1.tar", last modified: Tue Aug  1 11:36:39 2023, max compression
```

## Comparing `mypy-boto3-drs-1.28.16.tar` & `mypy-boto3-drs-1.28.16.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.270206 mypy-boto3-drs-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 19:32:11.000000 mypy-boto3-drs-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21758 2023-07-31 19:32:46.270206 mypy-boto3-drs-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20287 2023-07-31 19:32:11.000000 mypy-boto3-drs-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.266206 mypy-boto3-drs-1.28.16/mypy_boto3_drs/
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-31 19:32:11.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-31 19:32:11.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-31 19:32:11.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39632 2023-07-31 19:32:12.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39568 2023-07-31 19:32:12.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17226 2023-07-31 19:32:12.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17224 2023-07-31 19:32:12.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-07-31 19:32:12.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12966 2023-07-31 19:32:12.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:11.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    56826 2023-07-31 19:32:13.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    56779 2023-07-31 19:32:13.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 19:32:11.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.270206 mypy-boto3-drs-1.28.16/mypy_boto3_drs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21758 2023-07-31 19:32:46.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-31 19:32:46.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:46.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:46.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 19:32:46.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 19:32:46.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:32:46.270206 mypy-boto3-drs-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-31 19:32:11.000000 mypy-boto3-drs-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:39.108907 mypy-boto3-drs-1.28.16.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:15:19.000000 mypy-boto3-drs-1.28.16.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21760 2023-08-01 11:36:39.108907 mypy-boto3-drs-1.28.16.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20286 2023-08-01 11:15:19.000000 mypy-boto3-drs-1.28.16.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:39.108907 mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-08-01 11:15:19.000000 mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-08-01 11:15:19.000000 mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-01 11:15:19.000000 mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39632 2023-08-01 11:15:20.000000 mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39568 2023-08-01 11:15:19.000000 mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17226 2023-08-01 11:15:20.000000 mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17224 2023-08-01 11:15:20.000000 mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-08-01 11:15:20.000000 mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12966 2023-08-01 11:15:20.000000 mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:15:19.000000 mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    56824 2023-08-01 11:15:22.000000 mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56777 2023-08-01 11:15:21.000000 mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 11:15:19.000000 mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:39.108907 mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21760 2023-08-01 11:36:38.000000 mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 11:36:38.000000 mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:38.000000 mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:38.000000 mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:38.000000 mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:36:38.000000 mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:39.108907 mypy-boto3-drs-1.28.16.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-08-01 11:15:19.000000 mypy-boto3-drs-1.28.16.post1/setup.py
```

### Comparing `mypy-boto3-drs-1.28.16/LICENSE` & `mypy-boto3-drs-1.28.16.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.16/PKG-INFO` & `mypy-boto3-drs-1.28.16.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-drs
-Version: 1.28.16
-Summary: Type annotations for boto3.drs 1.28.16 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16.post1
+Summary: Type annotations for boto3.drs 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 drs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 drs type-annotations botocore mypy typeshed autocomplete
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
 [mypy-boto3-drs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/).
 
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
@@ -386,20 +386,20 @@
 )
 
 
 def check_value(value: DataReplicationErrorStringType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_drs.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_drs.type_defs import (
     AccountTypeDef,
     AssociateSourceNetworkStackRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CPUTypeDef,
@@ -540,15 +540,15 @@
     DescribeSourceServersResponseTypeDef,
     StartReplicationResponseTypeDef,
     StopReplicationResponseTypeDef,
     DescribeRecoveryInstancesResponseTypeDef,
 )
 
 
-def get_structure() -> AccountTypeDef:
+def get_value() -> AccountTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-drs-1.28.16/README.md` & `mypy-boto3-drs-1.28.16.post1/README.md`

 * *Files 0% similar despite different names*

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
 [mypy-boto3-drs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/).
 
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
@@ -354,20 +354,20 @@
 )
 
 
 def check_value(value: DataReplicationErrorStringType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_drs.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_drs.type_defs import (
     AccountTypeDef,
     AssociateSourceNetworkStackRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CPUTypeDef,
@@ -508,15 +508,15 @@
     DescribeSourceServersResponseTypeDef,
     StartReplicationResponseTypeDef,
     StopReplicationResponseTypeDef,
     DescribeRecoveryInstancesResponseTypeDef,
 )
 
 
-def get_structure() -> AccountTypeDef:
+def get_value() -> AccountTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-drs-1.28.16/mypy_boto3_drs/__init__.py` & `mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.16/mypy_boto3_drs/__init__.pyi` & `mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.16/mypy_boto3_drs/__main__.py` & `mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.drs 1.28.16\nVersion:         1.28.16\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.drs 1.28.16\nVersion:         1.28.16.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs\nOther"
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

### Comparing `mypy-boto3-drs-1.28.16/mypy_boto3_drs/client.py` & `mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.16/mypy_boto3_drs/client.pyi` & `mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.16/mypy_boto3_drs/literals.py` & `mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.16/mypy_boto3_drs/literals.pyi` & `mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.16/mypy_boto3_drs/paginator.py` & `mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.16/mypy_boto3_drs/paginator.pyi` & `mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.16/mypy_boto3_drs/type_defs.py` & `mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_drs.type_defs import AccountTypeDef
 
-    data: AccountTypeDef = {...}
+    data: AccountTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
```

### Comparing `mypy-boto3-drs-1.28.16/mypy_boto3_drs/type_defs.pyi` & `mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_drs.type_defs import AccountTypeDef
 
-    data: AccountTypeDef = {...}
+    data: AccountTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
```

### Comparing `mypy-boto3-drs-1.28.16/mypy_boto3_drs.egg-info/PKG-INFO` & `mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-drs
-Version: 1.28.16
-Summary: Type annotations for boto3.drs 1.28.16 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16.post1
+Summary: Type annotations for boto3.drs 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 drs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 drs type-annotations botocore mypy typeshed autocomplete
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
 [mypy-boto3-drs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/).
 
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
@@ -386,20 +386,20 @@
 )
 
 
 def check_value(value: DataReplicationErrorStringType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_drs.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_drs.type_defs import (
     AccountTypeDef,
     AssociateSourceNetworkStackRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CPUTypeDef,
@@ -540,15 +540,15 @@
     DescribeSourceServersResponseTypeDef,
     StartReplicationResponseTypeDef,
     StopReplicationResponseTypeDef,
     DescribeRecoveryInstancesResponseTypeDef,
 )
 
 
-def get_structure() -> AccountTypeDef:
+def get_value() -> AccountTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-drs-1.28.16/mypy_boto3_drs.egg-info/SOURCES.txt` & `mypy-boto3-drs-1.28.16.post1/mypy_boto3_drs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.16/setup.py` & `mypy-boto3-drs-1.28.16.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-drs",
-    version="1.28.16",
+    version="1.28.16.post1",
     packages=["mypy_boto3_drs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.drs 1.28.16 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.drs 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 drs type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 drs type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_drs": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

