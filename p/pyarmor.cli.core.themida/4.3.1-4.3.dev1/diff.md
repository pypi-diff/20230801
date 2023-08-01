# Comparing `tmp/pyarmor.cli.core.themida-4.3.1-cp38-none-any.whl.zip` & `tmp/pyarmor.cli.core.themida-4.3.dev1-cp39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 8098652 bytes, number of entries: 7
--rw-r--r--  2.0 unx       22 b- defN 23-Aug-01 01:20 pyarmor/cli/core/themida/__init__.py
--rwxr-xr-x  2.0 unx  4074526 b- defN 23-Aug-01 01:20 pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd
--rwxr-xr-x  2.0 unx  4975632 b- defN 23-Aug-01 01:20 pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd
--rw-r--r--  2.0 unx      809 b- defN 23-Aug-01 01:20 pyarmor.cli.core.themida-4.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 23-Aug-01 01:20 pyarmor.cli.core.themida-4.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Aug-01 01:20 pyarmor.cli.core.themida-4.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      690 b- defN 23-Aug-01 01:20 pyarmor.cli.core.themida-4.3.1.dist-info/RECORD
-7 files, 9051780 bytes uncompressed, 8097404 bytes compressed:  10.5%
+Zip file size: 7722018 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       25 b- defN 23-Jul-23 12:59 pyarmor/cli/core/themida/__init__.py
+-rwxr-xr-x  2.0 unx  3787806 b- defN 23-Jul-23 12:59 pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd
+-rwxr-xr-x  2.0 unx  4879888 b- defN 23-Jul-23 12:59 pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd
+-rw-r--r--  2.0 unx      812 b- defN 23-Jul-23 12:59 pyarmor.cli.core.themida-4.3.dev1.dist-info/METADATA
+-rw-r--r--  2.0 unx       93 b- defN 23-Jul-23 12:59 pyarmor.cli.core.themida-4.3.dev1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-23 12:59 pyarmor.cli.core.themida-4.3.dev1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      702 b- defN 23-Jul-23 12:59 pyarmor.cli.core.themida-4.3.dev1.dist-info/RECORD
+7 files, 8669334 bytes uncompressed, 7720746 bytes compressed:  10.9%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd
 Comment: 
 
 Filename: pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd
 Comment: 
 
-Filename: pyarmor.cli.core.themida-4.3.1.dist-info/METADATA
+Filename: pyarmor.cli.core.themida-4.3.dev1.dist-info/METADATA
 Comment: 
 
-Filename: pyarmor.cli.core.themida-4.3.1.dist-info/WHEEL
+Filename: pyarmor.cli.core.themida-4.3.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: pyarmor.cli.core.themida-4.3.1.dist-info/top_level.txt
+Filename: pyarmor.cli.core.themida-4.3.dev1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyarmor.cli.core.themida-4.3.1.dist-info/RECORD
+Filename: pyarmor.cli.core.themida-4.3.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyarmor/cli/core/themida/__init__.py

```diff
@@ -1 +1 @@
-__VERSION__ = '4.3.1'
+__VERSION__ = '4.3.dev1'
```

## Comparing `pyarmor.cli.core.themida-4.3.1.dist-info/METADATA` & `pyarmor.cli.core.themida-4.3.dev1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarmor.cli.core.themida
-Version: 4.3.1
+Version: 4.3.dev1
 Summary: Provide pre-built extension module `pyarmor_runtime` protected by Themida for Pyarmor
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

