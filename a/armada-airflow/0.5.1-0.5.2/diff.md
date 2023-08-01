# Comparing `tmp/armada_airflow-0.5.1-py3-none-any.whl.zip` & `tmp/armada_airflow-0.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 20377 bytes, number of entries: 16
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-25 14:59 armada/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-25 15:05 armada/jobservice/__init__.py
--rw-r--r--  2.0 unx     2891 b- defN 23-Jul-25 15:05 armada/jobservice/jobservice_pb2.py
--rw-r--r--  2.0 unx     4122 b- defN 23-Jul-25 15:05 armada/jobservice/jobservice_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-25 14:59 armada/operators/__init__.py
--rw-r--r--  2.0 unx     6170 b- defN 23-Jul-25 14:59 armada/operators/armada.py
--rw-r--r--  2.0 unx     9671 b- defN 23-Jul-25 14:59 armada/operators/armada_deferrable.py
--rw-r--r--  2.0 unx     3080 b- defN 23-Jul-25 14:59 armada/operators/grpc.py
--rw-r--r--  2.0 unx     3044 b- defN 23-Jul-25 14:59 armada/operators/jobservice.py
--rw-r--r--  2.0 unx     2613 b- defN 23-Jul-25 14:59 armada/operators/jobservice_asyncio.py
--rw-r--r--  2.0 unx    10090 b- defN 23-Jul-25 14:59 armada/operators/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-25 15:13 armada_airflow-0.5.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3916 b- defN 23-Jul-25 15:13 armada_airflow-0.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 15:13 armada_airflow-0.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-25 15:13 armada_airflow-0.5.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1370 b- defN 23-Jul-25 15:13 armada_airflow-0.5.1.dist-info/RECORD
-16 files, 58423 bytes uncompressed, 18091 bytes compressed:  69.0%
+Zip file size: 20706 bytes, number of entries: 16
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 17:41 armada/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 17:44 armada/jobservice/__init__.py
+-rw-r--r--  2.0 unx     2891 b- defN 23-Aug-01 17:44 armada/jobservice/jobservice_pb2.py
+-rw-r--r--  2.0 unx     4122 b- defN 23-Aug-01 17:44 armada/jobservice/jobservice_pb2_grpc.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 17:41 armada/operators/__init__.py
+-rw-r--r--  2.0 unx     6170 b- defN 23-Aug-01 17:41 armada/operators/armada.py
+-rw-r--r--  2.0 unx     9671 b- defN 23-Aug-01 17:41 armada/operators/armada_deferrable.py
+-rw-r--r--  2.0 unx     4418 b- defN 23-Aug-01 17:41 armada/operators/grpc.py
+-rw-r--r--  2.0 unx     3044 b- defN 23-Aug-01 17:41 armada/operators/jobservice.py
+-rw-r--r--  2.0 unx     2613 b- defN 23-Aug-01 17:41 armada/operators/jobservice_asyncio.py
+-rw-r--r--  2.0 unx    10090 b- defN 23-Aug-01 17:41 armada/operators/utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Aug-01 17:51 armada_airflow-0.5.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3916 b- defN 23-Aug-01 17:51 armada_airflow-0.5.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-01 17:51 armada_airflow-0.5.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Aug-01 17:51 armada_airflow-0.5.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1370 b- defN 23-Aug-01 17:51 armada_airflow-0.5.2.dist-info/RECORD
+16 files, 59761 bytes uncompressed, 18420 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: armada/operators/jobservice_asyncio.py
 Comment: 
 
 Filename: armada/operators/utils.py
 Comment: 
 
-Filename: armada_airflow-0.5.1.dist-info/LICENSE
+Filename: armada_airflow-0.5.2.dist-info/LICENSE
 Comment: 
 
-Filename: armada_airflow-0.5.1.dist-info/METADATA
+Filename: armada_airflow-0.5.2.dist-info/METADATA
 Comment: 
 
-Filename: armada_airflow-0.5.1.dist-info/WHEEL
+Filename: armada_airflow-0.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: armada_airflow-0.5.1.dist-info/top_level.txt
+Filename: armada_airflow-0.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: armada_airflow-0.5.1.dist-info/RECORD
+Filename: armada_airflow-0.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## armada/operators/grpc.py

```diff
@@ -1,99 +1,138 @@
+import importlib
 from typing import Optional, Sequence, Tuple, Any, TypedDict
 
 import grpc
 
 
+class CredentialsCallbackDict(TypedDict):
+    """
+    Helper class to provide stronger type checking on Credential callback args.
+    """
+
+    module_name: str
+    function_name: str
+    function_kwargs: dict
+
+
 class GrpcChannelArgsDict(TypedDict):
     """
     Helper class to provide stronger type checking on Grpc channel arugments.
     """
 
     target: str
-    credentials: Optional[grpc.ChannelCredentials]
     options: Optional[Sequence[Tuple[str, Any]]]
     compression: Optional[grpc.Compression]
+    credentials_callback_args: Optional[CredentialsCallbackDict]
+
+
+class CredentialsCallback(object):
+    """
+    Allows the use of an arbitrary callback function to get grpc credentials.
+
+    :param module_name: The fully qualified python module name where the
+        function is located.
+    :param function_name: The name of the function to be called.
+    :param function_kwargs: Keyword arguments to function_name in a dictionary.
+    """
+
+    def __init__(
+        self,
+        module_name: str,
+        function_name: str,
+        function_kwargs: dict,
+    ) -> None:
+        self.module_name = module_name
+        self.function_name = function_name
+        self.function_kwargs = function_kwargs
+
+    def call(self):
+        """Do the callback to get grpc credentials."""
+        module = importlib.import_module(self.module_name)
+        func = getattr(module, self.function_name)
+        return func(**self.function_kwargs)
 
 
 class GrpcChannelArguments(object):
     """
     A Serializable GRPC Arguments Object.
 
     :param target: Target keyword argument used
         when instantiating a grpc channel.
-    :param credentials: credentials keyword argument used
-        when instantiating a grpc channel.
+    :param credentials_callback_args: Arguments to CredentialsCallback to use
+        when instantiating a grpc channel that takes credentials.
     :param options: options keyword argument used
         when instantiating a grpc channel.
     :param compression: compression keyword argument used
         when instantiating a grpc channel.
     :return: a GrpcChannelArguments instance
     """
 
     def __init__(
         self,
         target: str,
-        credentials: Optional[grpc.ChannelCredentials] = None,
         options: Optional[Sequence[Tuple[str, Any]]] = None,
         compression: Optional[grpc.Compression] = None,
+        credentials_callback_args: CredentialsCallbackDict = None,
     ) -> None:
         self.target = target
-        self.credentials = credentials
         self.options = options
         self.compression = compression
+        if credentials_callback_args is not None:
+            self.credentials_callback = CredentialsCallback(**credentials_callback_args)
 
     def channel(self) -> grpc.Channel:
         """
         Create a grpc.Channel based on arguments supplied to this object.
 
         :return: Return grpc.insecure_channel if credentials is None. Otherwise
             returns grpc.secure_channel.
         """
 
-        if self.credentials is None:
+        if self.credentials_callback is None:
             return grpc.insecure_channel(
                 target=self.target,
                 options=self.options,
                 compression=self.compression,
             )
         return grpc.secure_channel(
             target=self.target,
-            credentials=self.credentials,
+            credentials=self.credentials_callback.call(),
             options=self.options,
             compression=self.compression,
         )
 
     def aio_channel(self) -> grpc.aio.Channel:
         """
         Create a grpc.aio.Channel (asyncio) based on arguments supplied to this object.
 
         :return: Return grpc.aio.insecure_channel if credentials is None. Otherwise
             returns grpc.aio.secure_channel.
         """
 
-        if self.credentials is None:
+        if self.credentials_callback is None:
             return grpc.aio.insecure_channel(
                 target=self.target,
                 options=self.options,
                 compression=self.compression,
             )
         return grpc.aio.secure_channel(
             target=self.target,
-            credentials=self.credentials,
+            credentials=self.credentials_callback.call(),
             options=self.options,
             compression=self.compression,
         )
 
     def serialize(self) -> dict:
         """
         Get a serialized version of this object.
 
         :return: A dict of keyword arguments used when calling
             a grpc channel or instantiating this object.
         """
 
         return {
             "target": self.target,
-            "credentials": self.credentials,
+            "credentials_callback_args": self.credentials_callback_args,
             "options": self.options,
             "compression": self.compression,
         }
```

## Comparing `armada_airflow-0.5.1.dist-info/LICENSE` & `armada_airflow-0.5.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `armada_airflow-0.5.1.dist-info/METADATA` & `armada_airflow-0.5.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armada-airflow
-Version: 0.5.1
+Version: 0.5.2
 Summary: Armada Airflow Operator
 Author-email: Armada-GROSS <armada@armadaproject.io>
 License: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: armada-client
```

## Comparing `armada_airflow-0.5.1.dist-info/RECORD` & `armada_airflow-0.5.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 armada/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 armada/jobservice/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 armada/jobservice/jobservice_pb2.py,sha256=idcVXwvH0EeYCcyBcloshRhh_JQhCpLn5a2-LPqkxIU,2891
 armada/jobservice/jobservice_pb2_grpc.py,sha256=ApiwP6_oYV8oHFlRC7oFum3I0aeEFQ9RE-7cNuaUmOk,4122
 armada/operators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 armada/operators/armada.py,sha256=U5VzsgXre5drhjU7Zzsd-p1liM6S2BlNUSKI1Jf481I,6170
 armada/operators/armada_deferrable.py,sha256=ggadgIswvrd2tA0D3aT86_jSEPvnRxRfDyg_fSppYtI,9671
-armada/operators/grpc.py,sha256=o9X4HhUdjVJIjhsLZNtjLRGubr7bYQRFCkUH7LD2lXw,3080
+armada/operators/grpc.py,sha256=N29zt4zNT8eKvsfLPHgO4HabGtMA9uY_kHazmYskLaI,4418
 armada/operators/jobservice.py,sha256=_Rrrmz6NqbEeATWegdabjMv7y7dEGUzWy5hgKS23-8o,3044
 armada/operators/jobservice_asyncio.py,sha256=DmtzNfSroAheBj-pAOeUZ6lZcx4UItUNt08DFvH3cIA,2613
 armada/operators/utils.py,sha256=ZKgFazRLXNp__htb-ZqLkWW95rm6Z5VNvtNmxCzkyQw,10090
-armada_airflow-0.5.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-armada_airflow-0.5.1.dist-info/METADATA,sha256=OvMtR60m1Gv3XRYliBz9azQZzwlAqnRXjF-dr1ir2nA,3916
-armada_airflow-0.5.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-armada_airflow-0.5.1.dist-info/top_level.txt,sha256=SaKoRDJJ1bkA2Lly_EYCX5D9VxncOV0eEI5NYBHU-bs,7
-armada_airflow-0.5.1.dist-info/RECORD,,
+armada_airflow-0.5.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+armada_airflow-0.5.2.dist-info/METADATA,sha256=aF1NTAuFLs1JeqQ2_v0X8NghE7UwYWT5ZjwsVOrtI_c,3916
+armada_airflow-0.5.2.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+armada_airflow-0.5.2.dist-info/top_level.txt,sha256=SaKoRDJJ1bkA2Lly_EYCX5D9VxncOV0eEI5NYBHU-bs,7
+armada_airflow-0.5.2.dist-info/RECORD,,
```

