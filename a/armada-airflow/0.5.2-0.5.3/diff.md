# Comparing `tmp/armada_airflow-0.5.2-py3-none-any.whl.zip` & `tmp/armada_airflow-0.5.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 20706 bytes, number of entries: 16
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 17:41 armada/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 17:44 armada/jobservice/__init__.py
--rw-r--r--  2.0 unx     2891 b- defN 23-Aug-01 17:44 armada/jobservice/jobservice_pb2.py
--rw-r--r--  2.0 unx     4122 b- defN 23-Aug-01 17:44 armada/jobservice/jobservice_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 17:41 armada/operators/__init__.py
--rw-r--r--  2.0 unx     6170 b- defN 23-Aug-01 17:41 armada/operators/armada.py
--rw-r--r--  2.0 unx     9671 b- defN 23-Aug-01 17:41 armada/operators/armada_deferrable.py
--rw-r--r--  2.0 unx     4418 b- defN 23-Aug-01 17:41 armada/operators/grpc.py
--rw-r--r--  2.0 unx     3044 b- defN 23-Aug-01 17:41 armada/operators/jobservice.py
--rw-r--r--  2.0 unx     2613 b- defN 23-Aug-01 17:41 armada/operators/jobservice_asyncio.py
--rw-r--r--  2.0 unx    10090 b- defN 23-Aug-01 17:41 armada/operators/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Aug-01 17:51 armada_airflow-0.5.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3916 b- defN 23-Aug-01 17:51 armada_airflow-0.5.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-01 17:51 armada_airflow-0.5.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Aug-01 17:51 armada_airflow-0.5.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1370 b- defN 23-Aug-01 17:51 armada_airflow-0.5.2.dist-info/RECORD
-16 files, 59761 bytes uncompressed, 18420 bytes compressed:  69.2%
+Zip file size: 20708 bytes, number of entries: 16
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 20:15 armada/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 20:21 armada/jobservice/__init__.py
+-rw-r--r--  2.0 unx     2891 b- defN 23-Aug-01 20:21 armada/jobservice/jobservice_pb2.py
+-rw-r--r--  2.0 unx     4122 b- defN 23-Aug-01 20:21 armada/jobservice/jobservice_pb2_grpc.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 20:15 armada/operators/__init__.py
+-rw-r--r--  2.0 unx     6170 b- defN 23-Aug-01 20:15 armada/operators/armada.py
+-rw-r--r--  2.0 unx     9671 b- defN 23-Aug-01 20:15 armada/operators/armada_deferrable.py
+-rw-r--r--  2.0 unx     4460 b- defN 23-Aug-01 20:15 armada/operators/grpc.py
+-rw-r--r--  2.0 unx     3044 b- defN 23-Aug-01 20:15 armada/operators/jobservice.py
+-rw-r--r--  2.0 unx     2613 b- defN 23-Aug-01 20:15 armada/operators/jobservice_asyncio.py
+-rw-r--r--  2.0 unx    10090 b- defN 23-Aug-01 20:15 armada/operators/utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Aug-01 20:29 armada_airflow-0.5.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3916 b- defN 23-Aug-01 20:29 armada_airflow-0.5.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-01 20:29 armada_airflow-0.5.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Aug-01 20:29 armada_airflow-0.5.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1370 b- defN 23-Aug-01 20:29 armada_airflow-0.5.3.dist-info/RECORD
+16 files, 59803 bytes uncompressed, 18422 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: armada/operators/jobservice_asyncio.py
 Comment: 
 
 Filename: armada/operators/utils.py
 Comment: 
 
-Filename: armada_airflow-0.5.2.dist-info/LICENSE
+Filename: armada_airflow-0.5.3.dist-info/LICENSE
 Comment: 
 
-Filename: armada_airflow-0.5.2.dist-info/METADATA
+Filename: armada_airflow-0.5.3.dist-info/METADATA
 Comment: 
 
-Filename: armada_airflow-0.5.2.dist-info/WHEEL
+Filename: armada_airflow-0.5.3.dist-info/WHEEL
 Comment: 
 
-Filename: armada_airflow-0.5.2.dist-info/top_level.txt
+Filename: armada_airflow-0.5.3.dist-info/top_level.txt
 Comment: 
 
-Filename: armada_airflow-0.5.2.dist-info/RECORD
+Filename: armada_airflow-0.5.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## armada/operators/grpc.py

```diff
@@ -73,14 +73,16 @@
         options: Optional[Sequence[Tuple[str, Any]]] = None,
         compression: Optional[grpc.Compression] = None,
         credentials_callback_args: CredentialsCallbackDict = None,
     ) -> None:
         self.target = target
         self.options = options
         self.compression = compression
+        self.credentials_callback = None
+
         if credentials_callback_args is not None:
             self.credentials_callback = CredentialsCallback(**credentials_callback_args)
 
     def channel(self) -> grpc.Channel:
         """
         Create a grpc.Channel based on arguments supplied to this object.
```

## Comparing `armada_airflow-0.5.2.dist-info/LICENSE` & `armada_airflow-0.5.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `armada_airflow-0.5.2.dist-info/METADATA` & `armada_airflow-0.5.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armada-airflow
-Version: 0.5.2
+Version: 0.5.3
 Summary: Armada Airflow Operator
 Author-email: Armada-GROSS <armada@armadaproject.io>
 License: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: armada-client
```

## Comparing `armada_airflow-0.5.2.dist-info/RECORD` & `armada_airflow-0.5.3.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 armada/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 armada/jobservice/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 armada/jobservice/jobservice_pb2.py,sha256=idcVXwvH0EeYCcyBcloshRhh_JQhCpLn5a2-LPqkxIU,2891
 armada/jobservice/jobservice_pb2_grpc.py,sha256=ApiwP6_oYV8oHFlRC7oFum3I0aeEFQ9RE-7cNuaUmOk,4122
 armada/operators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 armada/operators/armada.py,sha256=U5VzsgXre5drhjU7Zzsd-p1liM6S2BlNUSKI1Jf481I,6170
 armada/operators/armada_deferrable.py,sha256=ggadgIswvrd2tA0D3aT86_jSEPvnRxRfDyg_fSppYtI,9671
-armada/operators/grpc.py,sha256=N29zt4zNT8eKvsfLPHgO4HabGtMA9uY_kHazmYskLaI,4418
+armada/operators/grpc.py,sha256=nHfn_fsakXhma-JbQWXH6A4BkTJj2e06uccWhj0n1yc,4460
 armada/operators/jobservice.py,sha256=_Rrrmz6NqbEeATWegdabjMv7y7dEGUzWy5hgKS23-8o,3044
 armada/operators/jobservice_asyncio.py,sha256=DmtzNfSroAheBj-pAOeUZ6lZcx4UItUNt08DFvH3cIA,2613
 armada/operators/utils.py,sha256=ZKgFazRLXNp__htb-ZqLkWW95rm6Z5VNvtNmxCzkyQw,10090
-armada_airflow-0.5.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-armada_airflow-0.5.2.dist-info/METADATA,sha256=aF1NTAuFLs1JeqQ2_v0X8NghE7UwYWT5ZjwsVOrtI_c,3916
-armada_airflow-0.5.2.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-armada_airflow-0.5.2.dist-info/top_level.txt,sha256=SaKoRDJJ1bkA2Lly_EYCX5D9VxncOV0eEI5NYBHU-bs,7
-armada_airflow-0.5.2.dist-info/RECORD,,
+armada_airflow-0.5.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+armada_airflow-0.5.3.dist-info/METADATA,sha256=3k2Z-gMHyZp1_4GUyhUgjYxeS3C2T685HABG9l_nW-Y,3916
+armada_airflow-0.5.3.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+armada_airflow-0.5.3.dist-info/top_level.txt,sha256=SaKoRDJJ1bkA2Lly_EYCX5D9VxncOV0eEI5NYBHU-bs,7
+armada_airflow-0.5.3.dist-info/RECORD,,
```

