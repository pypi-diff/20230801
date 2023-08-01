# Comparing `tmp/zerocap_api_new_test-0.1.7.tar.gz` & `tmp/zerocap_api_new_test-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zerocap_api_new_test-0.1.7.tar", last modified: Mon Jul 31 07:11:03 2023, max compression
+gzip compressed data, was "dist\zerocap_api_new_test-0.1.8.tar", last modified: Tue Aug  1 03:43:52 2023, max compression
```

## Comparing `zerocap_api_new_test-0.1.7.tar` & `zerocap_api_new_test-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 07:11:03.000000 zerocap_api_new_test-0.1.7/
--rw-rw-rw-   0        0        0    11523 2023-07-26 06:34:57.000000 zerocap_api_new_test-0.1.7/LICENSE.txt
--rw-rw-rw-   0        0        0    19586 2023-07-31 07:11:03.000000 zerocap_api_new_test-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0    15434 2023-07-31 02:13:00.000000 zerocap_api_new_test-0.1.7/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-31 07:11:03.000000 zerocap_api_new_test-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     2133 2023-07-31 07:11:00.000000 zerocap_api_new_test-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:11:03.000000 zerocap_api_new_test-0.1.7/zerocap_api_new_test/
--rw-rw-rw-   0        0        0      126 2023-07-29 09:52:06.000000 zerocap_api_new_test-0.1.7/zerocap_api_new_test/__init__.py
--rw-rw-rw-   0        0        0     8154 2023-07-29 09:52:06.000000 zerocap_api_new_test-0.1.7/zerocap_api_new_test/main.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:11:03.000000 zerocap_api_new_test-0.1.7/zerocap_api_new_test.egg-info/
--rw-rw-rw-   0        0        0    19586 2023-07-31 07:11:03.000000 zerocap_api_new_test-0.1.7/zerocap_api_new_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-31 07:11:03.000000 zerocap_api_new_test-0.1.7/zerocap_api_new_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 07:11:03.000000 zerocap_api_new_test-0.1.7/zerocap_api_new_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-31 07:11:03.000000 zerocap_api_new_test-0.1.7/zerocap_api_new_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-31 07:11:03.000000 zerocap_api_new_test-0.1.7/zerocap_api_new_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 03:43:52.000000 zerocap_api_new_test-0.1.8/
+-rw-rw-rw-   0        0        0    11523 2023-07-26 06:34:57.000000 zerocap_api_new_test-0.1.8/LICENSE.txt
+-rw-rw-rw-   0        0        0    19690 2023-08-01 03:43:52.000000 zerocap_api_new_test-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0    15434 2023-07-31 02:13:00.000000 zerocap_api_new_test-0.1.8/README.rst
+-rw-rw-rw-   0        0        0       42 2023-08-01 03:43:52.000000 zerocap_api_new_test-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     2133 2023-08-01 03:43:02.000000 zerocap_api_new_test-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:43:52.000000 zerocap_api_new_test-0.1.8/zerocap_api_new_test/
+-rw-rw-rw-   0        0        0      126 2023-07-29 09:52:06.000000 zerocap_api_new_test-0.1.8/zerocap_api_new_test/__init__.py
+-rw-rw-rw-   0        0        0     8141 2023-08-01 03:35:19.000000 zerocap_api_new_test-0.1.8/zerocap_api_new_test/main.py
+drwxrwxrwx   0        0        0        0 2023-08-01 03:43:52.000000 zerocap_api_new_test-0.1.8/zerocap_api_new_test.egg-info/
+-rw-rw-rw-   0        0        0    19690 2023-08-01 03:43:52.000000 zerocap_api_new_test-0.1.8/zerocap_api_new_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-08-01 03:43:52.000000 zerocap_api_new_test-0.1.8/zerocap_api_new_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 03:43:52.000000 zerocap_api_new_test-0.1.8/zerocap_api_new_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-08-01 03:43:52.000000 zerocap_api_new_test-0.1.8/zerocap_api_new_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-08-01 03:43:52.000000 zerocap_api_new_test-0.1.8/zerocap_api_new_test.egg-info/top_level.txt
```

### Comparing `zerocap_api_new_test-0.1.7/LICENSE.txt` & `zerocap_api_new_test-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zerocap_api_new_test-0.1.7/PKG-INFO` & `zerocap_api_new_test-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerocap_api_new_test
-Version: 0.1.7
+Version: 0.1.8
 Summary: zerocap_api
 Home-page: https://zerocap.com/
 Author: zerocap
 Author-email: jiayu.gao@eigen.capital
 License: MIT
 Platform: all
 Classifier: Programming Language :: Python :: 3
@@ -245,16 +245,17 @@
 ```
 
 
 #### 3. Batch fetch order
 <!--post https://dma-api.defi.wiki/orders/fetch_orders-->
 
 ```
-result = client.fetch_orders(symbol='USDT/AUD', start_datetime=int(time.time() * 1000 - 86400), limit=10)
-
+result = client.fetch_orders(symbol='USDT/AUD', end_datetime=int(time.time() * 1000),
+                             start_datetime=int(time.time() * 1000 - 10*86400*1000),
+                             limit=10)
 ```
 
 
 
 请求参数:
 
 | Parameter      | required | data type | describe        | Value range |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerocap_api_new_test Version: 0.1.7 Summary:
+Metadata-Version: 2.1 Name: zerocap_api_new_test Version: 0.1.8 Summary:
 zerocap_api Home-page: https://zerocap.com/ Author: zerocap Author-email:
 jiayu.gao@eigen.capital License: MIT Platform: all Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE.txt # zerocap-
 api-new-test # Jump_restapi # Jump_websocket ``` æè¿°ä»ç» sdk install pip
 install zerocap-api-new-test ã ã ã ``` # restapi #### æ¥å£ææ¡£ ```
@@ -61,24 +61,24 @@
 4bc4-b5ff-380bb4ccc5e1", "client_order_id": "e7f80d34-0d80-4256-9de3-
 cd37310a55da", "datatime": "2023-07-31 02:12:23", "timestamp": "1690516007000",
 "last_trade_timestamp": "1690516007000", "status": "rejected", "symbol": "USDT/
 AUD", "type": "market", "time_in_force": "FOK", "side": "buy", "price": "1000",
 "average": "", "amount": "1000", "filled": "", "remaining": "", "cost": "",
 "transfer_id": "", "fee": "", "trades": [] } ], "status": "success", "total":
 3864, "page": "1" } ``` #### 3. Batch fetch order  ``` result =
-client.fetch_orders(symbol='USDT/AUD', start_datetime=int(time.time() * 1000 -
-86400), limit=10) ``` è¯·æ±åæ°: | Parameter | required | data type |
-describe | Value range | |----------------|----------|-----------|-------------
-----|-------------| | symbol | true | string | symbol | | | start_datetime |
-true | string | start_datetime | | | end_datetime | true | string |
-end_datetime | | | page | true | string | page | | | limit | true | string |
-limit | | | ids | true | string | Transaction ids(null character string or
-id1,id2...) | | | status | true | string | status | | | sort_order | true |
-string | sort_order | | | order_type | true | string | order_type | | | side |
-true | string | side | |
+client.fetch_orders(symbol='USDT/AUD', end_datetime=int(time.time() * 1000),
+start_datetime=int(time.time() * 1000 - 10*86400*1000), limit=10) ```
+è¯·æ±åæ°: | Parameter | required | data type | describe | Value range | |--
+--------------|----------|-----------|-----------------|-------------| | symbol
+| true | string | symbol | | | start_datetime | true | string | start_datetime
+| | | end_datetime | true | string | end_datetime | | | page | true | string |
+page | | | limit | true | string | limit | | | ids | true | string |
+Transaction ids(null character string or id1,id2...) | | | status | true |
+string | status | | | sort_order | true | string | sort_order | | | order_type
+| true | string | order_type | | | side | true | string | side | |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
 { "symbol": "", "start_datetime": 0, "end_datetime": 0, "page": 0, "limit": 0,
 "ids": "", "status": "", "sort_order": "", "order_type": "", "side": "",
 "account_vault": { "third_identity_id": "918d7125916c13191f3674e", "api_key":
 "***", "signature": "***", "note": "" } } ``` ååºæ°æ® æ¥å£æ¥é å¾å®:
 | Parameter | required | data type | describe | Value range | |---------------
 |----------|-----------|----------------|-------------| | id | true | string |
```

### Comparing `zerocap_api_new_test-0.1.7/README.rst` & `zerocap_api_new_test-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `zerocap_api_new_test-0.1.7/setup.py` & `zerocap_api_new_test-0.1.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         os.system('git tag v{0}'.format(about['__version__']))
         os.system('git push --tags')
 
         sys.exit()
 
 setup(
     name='zerocap_api_new_test',  # 包名
-    version='0.1.7',  # 版本号
+    version='0.1.8',  # 版本号
     description='zerocap_api',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='zerocap',
     author_email='jiayu.gao@eigen.capital',
     url='https://zerocap.com/',
     install_requires=REQUIRED,
```

### Comparing `zerocap_api_new_test-0.1.7/zerocap_api_new_test/main.py` & `zerocap_api_new_test-0.1.8/zerocap_api_new_test/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,18 +192,18 @@
         if response.status_code == 200:
             res = response.json()
             return res
         else:
             raise Exception(response.text)
 
     def fetch_orders(
-        self, 
-        symbol: str = '', 
-        start_datetime: int = '', 
-        end_datetime: int = 0, 
+        self,
+        start_datetime: int,
+        end_datetime: int,
+        symbol: str = '',
         page: int = 0,
         limit: int = 500, 
         ids: str = "", 
         status: str = "", 
         sort_order: str = "", 
         order_type: str = "",
         side: str = "",
```

### Comparing `zerocap_api_new_test-0.1.7/zerocap_api_new_test.egg-info/PKG-INFO` & `zerocap_api_new_test-0.1.8/zerocap_api_new_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerocap-api-new-test
-Version: 0.1.7
+Version: 0.1.8
 Summary: zerocap_api
 Home-page: https://zerocap.com/
 Author: zerocap
 Author-email: jiayu.gao@eigen.capital
 License: MIT
 Platform: all
 Classifier: Programming Language :: Python :: 3
@@ -245,16 +245,17 @@
 ```
 
 
 #### 3. Batch fetch order
 <!--post https://dma-api.defi.wiki/orders/fetch_orders-->
 
 ```
-result = client.fetch_orders(symbol='USDT/AUD', start_datetime=int(time.time() * 1000 - 86400), limit=10)
-
+result = client.fetch_orders(symbol='USDT/AUD', end_datetime=int(time.time() * 1000),
+                             start_datetime=int(time.time() * 1000 - 10*86400*1000),
+                             limit=10)
 ```
 
 
 
 请求参数:
 
 | Parameter      | required | data type | describe        | Value range |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerocap-api-new-test Version: 0.1.7 Summary:
+Metadata-Version: 2.1 Name: zerocap-api-new-test Version: 0.1.8 Summary:
 zerocap_api Home-page: https://zerocap.com/ Author: zerocap Author-email:
 jiayu.gao@eigen.capital License: MIT Platform: all Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE.txt # zerocap-
 api-new-test # Jump_restapi # Jump_websocket ``` æè¿°ä»ç» sdk install pip
 install zerocap-api-new-test ã ã ã ``` # restapi #### æ¥å£ææ¡£ ```
@@ -61,24 +61,24 @@
 4bc4-b5ff-380bb4ccc5e1", "client_order_id": "e7f80d34-0d80-4256-9de3-
 cd37310a55da", "datatime": "2023-07-31 02:12:23", "timestamp": "1690516007000",
 "last_trade_timestamp": "1690516007000", "status": "rejected", "symbol": "USDT/
 AUD", "type": "market", "time_in_force": "FOK", "side": "buy", "price": "1000",
 "average": "", "amount": "1000", "filled": "", "remaining": "", "cost": "",
 "transfer_id": "", "fee": "", "trades": [] } ], "status": "success", "total":
 3864, "page": "1" } ``` #### 3. Batch fetch order  ``` result =
-client.fetch_orders(symbol='USDT/AUD', start_datetime=int(time.time() * 1000 -
-86400), limit=10) ``` è¯·æ±åæ°: | Parameter | required | data type |
-describe | Value range | |----------------|----------|-----------|-------------
-----|-------------| | symbol | true | string | symbol | | | start_datetime |
-true | string | start_datetime | | | end_datetime | true | string |
-end_datetime | | | page | true | string | page | | | limit | true | string |
-limit | | | ids | true | string | Transaction ids(null character string or
-id1,id2...) | | | status | true | string | status | | | sort_order | true |
-string | sort_order | | | order_type | true | string | order_type | | | side |
-true | string | side | |
+client.fetch_orders(symbol='USDT/AUD', end_datetime=int(time.time() * 1000),
+start_datetime=int(time.time() * 1000 - 10*86400*1000), limit=10) ```
+è¯·æ±åæ°: | Parameter | required | data type | describe | Value range | |--
+--------------|----------|-----------|-----------------|-------------| | symbol
+| true | string | symbol | | | start_datetime | true | string | start_datetime
+| | | end_datetime | true | string | end_datetime | | | page | true | string |
+page | | | limit | true | string | limit | | | ids | true | string |
+Transaction ids(null character string or id1,id2...) | | | status | true |
+string | status | | | sort_order | true | string | sort_order | | | order_type
+| true | string | order_type | | | side | true | string | side | |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
 { "symbol": "", "start_datetime": 0, "end_datetime": 0, "page": 0, "limit": 0,
 "ids": "", "status": "", "sort_order": "", "order_type": "", "side": "",
 "account_vault": { "third_identity_id": "918d7125916c13191f3674e", "api_key":
 "***", "signature": "***", "note": "" } } ``` ååºæ°æ® æ¥å£æ¥é å¾å®:
 | Parameter | required | data type | describe | Value range | |---------------
 |----------|-----------|----------------|-------------| | id | true | string |
```

