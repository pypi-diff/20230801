# Comparing `tmp/sd_clients-2.4.0-py3-none-any.whl.zip` & `tmp/sd_clients-2.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6997 bytes, number of entries: 10
--rw-r--r--  2.0 unx      408 b- defN 23-Feb-16 16:12 sd_clients/__init__.py
--rw-r--r--  2.0 unx     4974 b- defN 23-Feb-16 14:07 sd_clients/api_gateway_client.py
+Zip file size: 7060 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      408 b- defN 23-Aug-01 14:51 sd_clients/__init__.py
+-rw-r--r--  2.0 unx     5968 b- defN 23-Aug-01 14:51 sd_clients/api_gateway_client.py
 -rw-r--r--  2.0 unx     9586 b- defN 23-Feb-16 16:07 sd_clients/client_store.py
--rw-r--r--  2.0 unx     1350 b- defN 23-Feb-16 14:07 sd_clients/service_directory_client.py
--rw-r--r--  2.0 unx     2144 b- defN 23-Feb-16 14:07 sd_clients/settings.py
--rw-rw-rw-  2.0 unx      575 b- defN 23-Mar-03 15:53 sd_clients-2.4.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      894 b- defN 23-Mar-03 15:53 sd_clients-2.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-03 15:53 sd_clients-2.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Mar-03 15:53 sd_clients-2.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      827 b- defN 23-Mar-03 15:53 sd_clients-2.4.0.dist-info/RECORD
-10 files, 20861 bytes uncompressed, 5579 bytes compressed:  73.3%
+-rw-r--r--  2.0 unx     1350 b- defN 22-Oct-13 15:17 sd_clients/service_directory_client.py
+-rw-r--r--  2.0 unx     2144 b- defN 22-Oct-13 15:17 sd_clients/settings.py
+-rw-rw-rw-  2.0 unx      575 b- defN 23-Aug-01 14:56 sd_clients-2.5.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      894 b- defN 23-Aug-01 14:56 sd_clients-2.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-01 14:56 sd_clients-2.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Aug-01 14:56 sd_clients-2.5.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      827 b- defN 23-Aug-01 14:56 sd_clients-2.5.0.dist-info/RECORD
+10 files, 21855 bytes uncompressed, 5642 bytes compressed:  74.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: sd_clients/service_directory_client.py
 Comment: 
 
 Filename: sd_clients/settings.py
 Comment: 
 
-Filename: sd_clients-2.4.0.dist-info/LICENSE.txt
+Filename: sd_clients-2.5.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: sd_clients-2.4.0.dist-info/METADATA
+Filename: sd_clients-2.5.0.dist-info/METADATA
 Comment: 
 
-Filename: sd_clients-2.4.0.dist-info/WHEEL
+Filename: sd_clients-2.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: sd_clients-2.4.0.dist-info/top_level.txt
+Filename: sd_clients-2.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sd_clients-2.4.0.dist-info/RECORD
+Filename: sd_clients-2.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sd_clients/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.4.0"
+__version__ = "2.5.0"
 
 __all__ = [
     "ServiceDirectoryClient",
     "ApiGatewayProvider",
     "BaseClientStore",
     "ClientStore",
     "OIDCConnector",
```

## sd_clients/api_gateway_client.py

```diff
@@ -12,14 +12,28 @@
                     "name": "AnalyticDataset",
                     "properties": {"uri": urljoin(base, "analytic-dataset-service")},
                     "version": {"major": 1, "minor": 0, "patch": 0},
                 }
             ],
         }
     )
+    adtd = Service.from_service(
+        {
+            "name": "E360-AnalyticDatasetTools-Service",
+            "endpoints": [
+                {
+                    "name": "AnalyticDatasetDefinition",
+                    "properties": {
+                        "uri": urljoin(base, "analytic-dataset-definition-service")
+                    },
+                    "version": {"major": 1, "minor": 0, "patch": 0},
+                }
+            ],
+        }
+    )
     fs = Service.from_service(
         {
             "name": "E360-File-Service",
             "endpoints": [
                 {
                     "name": "Files",
                     "properties": {"uri": urljoin(base, "file-service")},
@@ -86,20 +100,36 @@
                     "version": {"major": 1, "minor": 0, "patch": 0},
                 }
             ],
         }
     )
     card = Service.from_service(
         {
-            "name": "E360-Card-Service",
+            "name": "E360-CohortDefinition-Service",
             "endpoints": [
                 {
-                    "name": "PatientCard",
-                    "properties": {"uri": urljoin(base, "card-service")},
-                    "version": {"major": 1, "minor": 1, "patch": 0},
+                    "name": "Cards",
+                    "properties": {
+                        "uri": urljoin(base, "cohort-definition-service-card")
+                    },
+                    "version": {"major": 1, "minor": 0, "patch": 0},
+                }
+            ],
+        }
+    )
+    patient = Service.from_service(
+        {
+            "name": "E360-CohortDefinition-Service",
+            "endpoints": [
+                {
+                    "name": "Patients",
+                    "properties": {
+                        "uri": urljoin(base, "cohort-definition-service-patient-v2")
+                    },
+                    "version": {"major": 2, "minor": 0, "patch": 0},
                 }
             ],
         }
     )
     chart = Service.from_service(
         {
             "name": "E360-ChartImage-Service",
@@ -132,15 +162,15 @@
                     "name": "Dashboards",
                     "properties": {"uri": urljoin(base, "dashboard-service-v2")},
                     "version": {"major": 2, "minor": 0, "patch": 0},
                 }
             ],
         }
     )
-    return [adt, fs, fss, ws, perm, td_import, card, chart, vis, dash]
+    return [adt, adtd, fs, fss, ws, perm, td_import, card, patient, chart, vis, dash]
 
 
 class ApiGatewayProvider(ServiceListProvider):
     service_url: str
 
     def __init__(self, service_url: str):
         self.service_url = service_url.rstrip("/")
```

## Comparing `sd_clients-2.4.0.dist-info/LICENSE.txt` & `sd_clients-2.5.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `sd_clients-2.4.0.dist-info/METADATA` & `sd_clients-2.5.0.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-clients
-Version: 2.4.0
+Version: 2.5.0
 Summary: Clients for communication with e360 Service Directory and Api Gateway
 Author: IQVIA
 Author-email: e360pypi@iqvia.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `sd_clients-2.4.0.dist-info/RECORD` & `sd_clients-2.5.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-sd_clients/__init__.py,sha256=GVJQNocLmXOvxU-mw-GRM5bJtwwxYTYBuPSciYA2xMA,408
-sd_clients/api_gateway_client.py,sha256=0YZzqGaknlQE40Lmsni0cWV1S3PNY9RQte52PxrnUlc,4974
+sd_clients/__init__.py,sha256=Xql4hqClgUsH_Pmv4AbzD4TdY2Lh4zFsLYjNgAkKkjU,408
+sd_clients/api_gateway_client.py,sha256=ZlZb0xh7uHOXhT6TfOsQjRVeNKwQ9z7wCGrR7hLA-kE,5968
 sd_clients/client_store.py,sha256=u4Hb4DOn7jERJgXTSDumXimQHSpsjrMtUU5oH0ux-18,9586
 sd_clients/service_directory_client.py,sha256=HmanI5ORsT0bhZZRxykr45HTyBWvkCVbLrxEnu6Miks,1350
 sd_clients/settings.py,sha256=4rEMJOlUjVSotESD_R5nCS_OUyeMzItMyaZeFEuLdI4,2144
-sd_clients-2.4.0.dist-info/LICENSE.txt,sha256=uoI1G5lxk8h5Ua5OqmR7137DhTctSXGt9z7EBa1yclI,575
-sd_clients-2.4.0.dist-info/METADATA,sha256=uznQ50_2vREa1Rh-el5XjPlOmT0jNL6maAEpRWKPrvw,894
-sd_clients-2.4.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-sd_clients-2.4.0.dist-info/top_level.txt,sha256=l-mSItKwzL0S3kdRGj1R1VC9lPO0JfRY0P5cHC2qKzI,11
-sd_clients-2.4.0.dist-info/RECORD,,
+sd_clients-2.5.0.dist-info/LICENSE.txt,sha256=uoI1G5lxk8h5Ua5OqmR7137DhTctSXGt9z7EBa1yclI,575
+sd_clients-2.5.0.dist-info/METADATA,sha256=JNyKv1ZlRkeAbw_MzTBzjmEFSAE69gWUDKLcrgZF2eQ,894
+sd_clients-2.5.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+sd_clients-2.5.0.dist-info/top_level.txt,sha256=l-mSItKwzL0S3kdRGj1R1VC9lPO0JfRY0P5cHC2qKzI,11
+sd_clients-2.5.0.dist-info/RECORD,,
```

