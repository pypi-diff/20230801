# Comparing `tmp/cirq-1.3.0.dev20230731224617-py3-none-any.whl.zip` & `tmp/cirq-1.3.0.dev20230801170401-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 8403 bytes, number of entries: 6
--rw-r--r--  2.0 unx      292 b- defN 23-Jul-31 22:46 cirq-1.3.0.dev20230731224617.dist-info/AUTHORS
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-31 22:46 cirq-1.3.0.dev20230731224617.dist-info/LICENSE
--rw-r--r--  2.0 unx     7932 b- defN 23-Jul-31 22:46 cirq-1.3.0.dev20230731224617.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-31 22:46 cirq-1.3.0.dev20230731224617.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-31 22:46 cirq-1.3.0.dev20230731224617.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      563 b- defN 23-Jul-31 22:46 cirq-1.3.0.dev20230731224617.dist-info/RECORD
+-rw-r--r--  2.0 unx      292 b- defN 23-Aug-01 17:04 cirq-1.3.0.dev20230801170401.dist-info/AUTHORS
+-rw-r--r--  2.0 unx    11357 b- defN 23-Aug-01 17:04 cirq-1.3.0.dev20230801170401.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7932 b- defN 23-Aug-01 17:04 cirq-1.3.0.dev20230801170401.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-01 17:04 cirq-1.3.0.dev20230801170401.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-01 17:04 cirq-1.3.0.dev20230801170401.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      563 b- defN 23-Aug-01 17:04 cirq-1.3.0.dev20230801170401.dist-info/RECORD
 6 files, 20237 bytes uncompressed, 7365 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: cirq-1.3.0.dev20230731224617.dist-info/AUTHORS
+Filename: cirq-1.3.0.dev20230801170401.dist-info/AUTHORS
 Comment: 
 
-Filename: cirq-1.3.0.dev20230731224617.dist-info/LICENSE
+Filename: cirq-1.3.0.dev20230801170401.dist-info/LICENSE
 Comment: 
 
-Filename: cirq-1.3.0.dev20230731224617.dist-info/METADATA
+Filename: cirq-1.3.0.dev20230801170401.dist-info/METADATA
 Comment: 
 
-Filename: cirq-1.3.0.dev20230731224617.dist-info/WHEEL
+Filename: cirq-1.3.0.dev20230801170401.dist-info/WHEEL
 Comment: 
 
-Filename: cirq-1.3.0.dev20230731224617.dist-info/top_level.txt
+Filename: cirq-1.3.0.dev20230801170401.dist-info/top_level.txt
 Comment: 
 
-Filename: cirq-1.3.0.dev20230731224617.dist-info/RECORD
+Filename: cirq-1.3.0.dev20230801170401.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cirq-1.3.0.dev20230731224617.dist-info/LICENSE` & `cirq-1.3.0.dev20230801170401.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cirq-1.3.0.dev20230731224617.dist-info/METADATA` & `cirq-1.3.0.dev20230801170401.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: cirq
-Version: 1.3.0.dev20230731224617
+Version: 1.3.0.dev20230801170401
 Summary: A framework for creating, editing, and invoking Noisy Intermediate Scale Quantum (NISQ) circuits.
 Home-page: http://github.com/quantumlib/cirq
 Author: The Cirq Developers
 Author-email: cirq-dev@googlegroups.com
 License: Apache 2
 Platform: UNKNOWN
 Requires-Python: >=3.9.0
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: cirq-aqt (==1.3.0.dev20230731224617)
-Requires-Dist: cirq-core (==1.3.0.dev20230731224617)
-Requires-Dist: cirq-ft (==1.3.0.dev20230731224617)
-Requires-Dist: cirq-google (==1.3.0.dev20230731224617)
-Requires-Dist: cirq-ionq (==1.3.0.dev20230731224617)
-Requires-Dist: cirq-pasqal (==1.3.0.dev20230731224617)
-Requires-Dist: cirq-rigetti (==1.3.0.dev20230731224617)
-Requires-Dist: cirq-web (==1.3.0.dev20230731224617)
+Requires-Dist: cirq-aqt (==1.3.0.dev20230801170401)
+Requires-Dist: cirq-core (==1.3.0.dev20230801170401)
+Requires-Dist: cirq-ft (==1.3.0.dev20230801170401)
+Requires-Dist: cirq-google (==1.3.0.dev20230801170401)
+Requires-Dist: cirq-ionq (==1.3.0.dev20230801170401)
+Requires-Dist: cirq-pasqal (==1.3.0.dev20230801170401)
+Requires-Dist: cirq-rigetti (==1.3.0.dev20230801170401)
+Requires-Dist: cirq-web (==1.3.0.dev20230801170401)
 Provides-Extra: dev_env
 Requires-Dist: mypy (==1.2.0) ; extra == 'dev_env'
 Requires-Dist: types-backports (==0.1.3) ; extra == 'dev_env'
 Requires-Dist: types-cachetools ; extra == 'dev_env'
 Requires-Dist: types-protobuf (~=3.20) ; extra == 'dev_env'
 Requires-Dist: types-requests (==2.28.1) ; extra == 'dev_env'
 Requires-Dist: types-setuptools (==62.6.1) ; extra == 'dev_env'
```

