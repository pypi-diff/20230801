# Comparing `tmp/lite_fastapi_local-0.0.46.tar.gz` & `tmp/lite_fastapi_local-0.0.50.tar.gz`

## Comparing `lite_fastapi_local-0.0.46.tar` & `lite_fastapi_local-0.0.50.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/readme.md
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/QR_CHK_dep.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/QR_END_dep.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/QR_READ_dep.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/__init__.py
--rw-r--r--   0        0        0     9263 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/main.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/requirements.txt
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/common/__init__.py
--rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/common/function.py
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/common/variable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/__init__.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/boxDoorModel.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/drimmLedModel.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/innerLedModel.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/motorModel.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/registrationModel.py
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/setupModel.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/solModel.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/sprayModel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/router/__init__.py
--rw-r--r--   0        0        0     6769 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/router/motorRouter.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/router/sensorRouter.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/router/setupRouter.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/schema/qrSchema.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/src/lite_fastapi_local/schema/setupSchema.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/README.md
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/pyproject.toml
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.46/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/readme.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/QR_CHK_dep.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/QR_END_dep.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/QR_READ_dep.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/__init__.py
+-rw-r--r--   0        0        0     9237 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/main.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/requirements.txt
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/common/__init__.py
+-rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/common/function.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/common/variable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/model/__init__.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/model/boxDoorModel.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/model/drimmLedModel.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/model/innerLedModel.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/model/motorModel.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/model/registrationModel.py
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/model/setupModel.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/model/solModel.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/model/sprayModel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/router/__init__.py
+-rw-r--r--   0        0        0     6769 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/router/motorRouter.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/router/sensorRouter.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/router/setupRouter.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/schema/qrSchema.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/src/lite_fastapi_local/schema/setupSchema.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/README.md
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/pyproject.toml
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.50/PKG-INFO
```

### Comparing `lite_fastapi_local-0.0.46/src/lite_fastapi_local/QR_CHK_dep.py` & `lite_fastapi_local-0.0.50/src/lite_fastapi_local/QR_CHK_dep.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.46/src/lite_fastapi_local/QR_READ_dep.py` & `lite_fastapi_local-0.0.50/src/lite_fastapi_local/QR_READ_dep.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.46/src/lite_fastapi_local/main.py` & `lite_fastapi_local-0.0.50/src/lite_fastapi_local/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -227,27 +227,31 @@
     json_response = response.json()
     RESP = json_response['RESP_DATA'][0]['ACCT_NM']
     return RESP
     #return response.text
     
     
 @app.get('/transfer')
-async def send_post_request(RCV_ACCT_NO: str, RCV_BNK_CD: str, TRSC_AMT: str, customer_phone_number: str, returned_qr_code_list: list):
+async def send_post_request(RCV_ACCT_NO: str, RCV_BNK_CD: str, TRSC_AMT: str):
     mac_address = common.get_MACHINE_MAC()
     # returned_qr_code_list = common.get_returned_qr_code_list()
-    url = 'http://54.180.21.162/coocon/transfer'
+    url = 'http://54.180.21.162/coocon/transfer_v1'
     data = {
         'RCV_BNK_CD': RCV_BNK_CD,
         'RCV_ACCT_NO': RCV_ACCT_NO,
         'TRSC_AMT': TRSC_AMT,
         'accountName': '',
-        'classQr': returned_qr_code_list,
-        'return_ECIS': mac_address,
-        'customer_Id': customer_phone_number,
-        'dbType': 'op01'
+         "classQr": [
+            "KRAS1020122010100001",
+            "KRAS1020122010100002"
+        ],
+        "classNum": [
+            "050",
+            "051"
+        ]
     }
     response = requests.post(url, json=data)
     return response.json()
 
 
 def start_server():
     uvicorn.run(app, host="127.0.0.1", port=8000)
```

### Comparing `lite_fastapi_local-0.0.46/src/lite_fastapi_local/requirements.txt` & `lite_fastapi_local-0.0.50/src/lite_fastapi_local/requirements.txt`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.46/src/lite_fastapi_local/settings.py` & `lite_fastapi_local-0.0.50/src/lite_fastapi_local/settings.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.46/src/lite_fastapi_local/common/function.py` & `lite_fastapi_local-0.0.50/src/lite_fastapi_local/common/function.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.46/src/lite_fastapi_local/common/variable.py` & `lite_fastapi_local-0.0.50/src/lite_fastapi_local/common/variable.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/motorModel.py` & `lite_fastapi_local-0.0.50/src/lite_fastapi_local/model/motorModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/setupModel.py` & `lite_fastapi_local-0.0.50/src/lite_fastapi_local/model/setupModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.46/src/lite_fastapi_local/model/solModel.py` & `lite_fastapi_local-0.0.50/src/lite_fastapi_local/model/solModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.46/src/lite_fastapi_local/router/motorRouter.py` & `lite_fastapi_local-0.0.50/src/lite_fastapi_local/router/motorRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.46/src/lite_fastapi_local/router/sensorRouter.py` & `lite_fastapi_local-0.0.50/src/lite_fastapi_local/router/sensorRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.46/src/lite_fastapi_local/router/setupRouter.py` & `lite_fastapi_local-0.0.50/src/lite_fastapi_local/router/setupRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.46/LICENSE` & `lite_fastapi_local-0.0.50/LICENSE`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.46/pyproject.toml` & `lite_fastapi_local-0.0.50/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lite_fastapi_local"
-version = "0.0.46"
+version = "0.0.50"
 authors = [
   { name="dohyung102", email="dohyung102@thegreet.co.kr" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `lite_fastapi_local-0.0.46/PKG-INFO` & `lite_fastapi_local-0.0.50/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lite_fastapi_local
-Version: 0.0.46
+Version: 0.0.50
 Summary: A small example package
 Author-email: dohyung102 <dohyung102@thegreet.co.kr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

