# Comparing `tmp/qat_hardware-1.3.0-cp39-cp39-win_amd64.whl.zip` & `tmp/qat_hardware-1.3.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 427423 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 22-Nov-04 21:52 qat/__init__.py
--rwxr-xr-x  2.0 unx   119200 b- defN 22-Nov-04 21:52 qat/hardware/__init__.pyd
--rwxr-xr-x  2.0 unx   443749 b- defN 22-Nov-04 21:52 qat/hardware/default.pyd
--rwxr-xr-x  2.0 unx   178975 b- defN 22-Nov-04 21:52 qat/hardware/models.pyd
--rwxr-xr-x  2.0 unx   169421 b- defN 22-Nov-04 21:52 qat/hardware/tomography.pyd
--rwxr-xr-x  2.0 unx   109645 b- defN 22-Nov-04 21:52 qat/hardware/version.pyd
--rwxr-xr-x  2.0 unx   318977 b- defN 22-Nov-04 21:52 qat/hardware/ions/gates_specification.pyd
--rw-r--r--  2.0 unx     4752 b- defN 22-Nov-04 21:52 qat_hardware-1.3.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1591 b- defN 22-Nov-04 21:52 qat_hardware-1.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 22-Nov-04 21:52 qat_hardware-1.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 22-Nov-04 21:52 qat_hardware-1.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1001 b- defN 22-Nov-04 21:52 qat_hardware-1.3.0.dist-info/RECORD
-12 files, 1347414 bytes uncompressed, 425755 bytes compressed:  68.4%
+Zip file size: 352686 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       75 b- defN 23-Jul-31 23:02 qat/__init__.py
+-rwxr-xr-x  2.0 unx    82703 b- defN 23-Jul-31 23:02 qat/hardware/__init__.pyd
+-rwxr-xr-x  2.0 unx   414393 b- defN 23-Jul-31 23:02 qat/hardware/default.pyd
+-rwxr-xr-x  2.0 unx   144795 b- defN 23-Jul-31 23:02 qat/hardware/models.pyd
+-rwxr-xr-x  2.0 unx   133705 b- defN 23-Jul-31 23:02 qat/hardware/tomography.pyd
+-rwxr-xr-x  2.0 unx    73125 b- defN 23-Jul-31 23:02 qat/hardware/version.pyd
+-rwxr-xr-x  2.0 unx   283216 b- defN 23-Jul-31 23:02 qat/hardware/ions/gates_specification.pyd
+-rw-r--r--  2.0 unx     4752 b- defN 23-Jul-31 23:02 qat_hardware-1.3.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1589 b- defN 23-Jul-31 23:02 qat_hardware-1.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-31 23:02 qat_hardware-1.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-31 23:02 qat_hardware-1.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1000 b- defN 23-Jul-31 23:02 qat_hardware-1.3.1.dist-info/RECORD
+12 files, 1139456 bytes uncompressed, 351018 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: qat/hardware/version.pyd
 Comment: 
 
 Filename: qat/hardware/ions/gates_specification.pyd
 Comment: 
 
-Filename: qat_hardware-1.3.0.dist-info/LICENSE.txt
+Filename: qat_hardware-1.3.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: qat_hardware-1.3.0.dist-info/METADATA
+Filename: qat_hardware-1.3.1.dist-info/METADATA
 Comment: 
 
-Filename: qat_hardware-1.3.0.dist-info/WHEEL
+Filename: qat_hardware-1.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: qat_hardware-1.3.0.dist-info/top_level.txt
+Filename: qat_hardware-1.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: qat_hardware-1.3.0.dist-info/RECORD
+Filename: qat_hardware-1.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qat/__init__.py

```diff
@@ -0,0 +1,5 @@
+00000000: 6672 6f6d 2070 6b67 7574 696c 2069 6d70  from pkgutil imp
+00000010: 6f72 7420 6578 7465 6e64 5f70 6174 680a  ort extend_path.
+00000020: 5f5f 7061 7468 5f5f 203d 2065 7874 656e  __path__ = exten
+00000030: 645f 7061 7468 285f 5f70 6174 685f 5f2c  d_path(__path__,
+00000040: 205f 5f6e 616d 655f 5f29 0a               __name__).
```

## Comparing `qat_hardware-1.3.0.dist-info/LICENSE.txt` & `qat_hardware-1.3.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `qat_hardware-1.3.0.dist-info/METADATA` & `qat_hardware-1.3.1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: qat-hardware
-Version: 1.3.0
-Summary: Module qat-hardware [899a55f] - Compiled by Atos
+Version: 1.3.1
+Summary: Module qat-hardware [2eb55a8] - Compiled by Atos
 Home-page: https://atos.net/en/lp/myqlm
 Author: Atos Quantum Lab
 Author-email: myqlm@atos.net
 License: Atos myQLM EULA
 Project-URL: Documentation, https://myqlm.github.io
 Project-URL: Bug Tracker, https://github.com/myQLM/myqlm-issues/issues
 Project-URL: Community, https://myqlmworkspace.slack.com
@@ -35,9 +35,7 @@
 
 ```
 pip install qlmaas
 ```
 
 ## License
 [Atos myQLM EULA](https://myqlm.github.io/myqlm_specific/license.html#proprietary-part)
-
-
```

