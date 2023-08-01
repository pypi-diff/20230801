# Comparing `tmp/myqlm_contrib-1.7.1-py3-none-any.whl.zip` & `tmp/myqlm_contrib-1.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 13382 bytes, number of entries: 8
--rw-r--r--  2.0 unx     1092 b- defN 22-Nov-04 02:28 qat/plugins/hook_sabre.py
--rw-r--r--  2.0 unx     1038 b- defN 22-Nov-04 02:28 qat/sabre/__init__.py
--rw-r--r--  2.0 unx    22523 b- defN 22-Nov-04 02:28 qat/sabre/sabre.py
--rw-r--r--  2.0 unx    11340 b- defN 22-Nov-04 02:28 myqlm_contrib-1.7.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      949 b- defN 22-Nov-04 02:28 myqlm_contrib-1.7.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-04 02:28 myqlm_contrib-1.7.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 22-Nov-04 02:28 myqlm_contrib-1.7.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      651 b- defN 22-Nov-04 02:28 myqlm_contrib-1.7.1.dist-info/RECORD
-8 files, 37689 bytes uncompressed, 12246 bytes compressed:  67.5%
+Zip file size: 13380 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     1092 b- defN 23-Jul-31 22:54 qat/plugins/hook_sabre.py
+-rw-r--r--  2.0 unx     1038 b- defN 23-Jul-31 22:54 qat/sabre/__init__.py
+-rw-r--r--  2.0 unx    22523 b- defN 23-Jul-31 22:54 qat/sabre/sabre.py
+-rw-r--r--  2.0 unx    11340 b- defN 23-Jul-31 22:55 myqlm_contrib-1.9.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      949 b- defN 23-Jul-31 22:55 myqlm_contrib-1.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-31 22:55 myqlm_contrib-1.9.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-31 22:55 myqlm_contrib-1.9.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      651 b- defN 23-Jul-31 22:55 myqlm_contrib-1.9.1.dist-info/RECORD
+8 files, 37689 bytes uncompressed, 12244 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: qat/sabre/__init__.py
 Comment: 
 
 Filename: qat/sabre/sabre.py
 Comment: 
 
-Filename: myqlm_contrib-1.7.1.dist-info/LICENSE
+Filename: myqlm_contrib-1.9.1.dist-info/LICENSE
 Comment: 
 
-Filename: myqlm_contrib-1.7.1.dist-info/METADATA
+Filename: myqlm_contrib-1.9.1.dist-info/METADATA
 Comment: 
 
-Filename: myqlm_contrib-1.7.1.dist-info/WHEEL
+Filename: myqlm_contrib-1.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: myqlm_contrib-1.7.1.dist-info/top_level.txt
+Filename: myqlm_contrib-1.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: myqlm_contrib-1.7.1.dist-info/RECORD
+Filename: myqlm_contrib-1.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `myqlm_contrib-1.7.1.dist-info/LICENSE` & `myqlm_contrib-1.9.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `myqlm_contrib-1.7.1.dist-info/METADATA` & `myqlm_contrib-1.9.1.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myqlm-contrib
-Version: 1.7.1
+Version: 1.9.1
 Summary: Modules developed by the myQLM community
 Home-page: https://atos.net/en/lp/myqlm
 Author: Atos Quantum Lab
 Author-email: myqlm@atos.net
 License: Atos myQLM EULA
 Project-URL: Documentation, https://myqlm.github.io
 Project-URL: Source Code, https://github.com/myQLM/myqlm-contrib
```

