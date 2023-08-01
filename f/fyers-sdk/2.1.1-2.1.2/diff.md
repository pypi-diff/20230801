# Comparing `tmp/fyers_sdk-2.1.1.tar.gz` & `tmp/fyers_sdk-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_sdk-2.1.1.tar", last modified: Tue Aug  1 07:13:56 2023, max compression
+gzip compressed data, was "fyers_sdk-2.1.2.tar", last modified: Tue Aug  1 07:48:06 2023, max compression
```

## Comparing `fyers_sdk-2.1.1.tar` & `fyers_sdk-2.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:13:56.565583 fyers_sdk-2.1.1/
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-31 10:25:54.000000 fyers_sdk-2.1.1/LICENSE.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-01 07:13:56.565583 fyers_sdk-2.1.1/PKG-INFO
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-2.1.1/README.md
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:13:56.541584 fyers_sdk-2.1.1/fyers_sdk/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:13:56.565583 fyers_sdk-2.1.1/fyers_sdk/FyersWebsocket/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-2.1.1/fyers_sdk/FyersWebsocket/__init__.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    59613 2023-08-01 06:57:51.000000 fyers_sdk-2.1.1/fyers_sdk/FyersWebsocket/data_ws.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     1140 2023-08-01 06:21:10.000000 fyers_sdk-2.1.1/fyers_sdk/FyersWebsocket/defines.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     7508 2023-08-01 07:05:48.000000 fyers_sdk-2.1.1/fyers_sdk/FyersWebsocket/map.json
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    15427 2023-07-31 06:13:16.000000 fyers_sdk-2.1.1/fyers_sdk/FyersWebsocket/order_ws.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-2.1.1/fyers_sdk/__init__.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27819 2023-07-31 09:12:31.000000 fyers_sdk-2.1.1/fyers_sdk/fyersModel.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-2.1.1/fyers_sdk/fyers_logger.py
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:13:56.561583 fyers_sdk-2.1.1/fyers_sdk.egg-info/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-01 07:13:56.000000 fyers_sdk-2.1.1/fyers_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      446 2023-08-01 07:13:56.000000 fyers_sdk-2.1.1/fyers_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-08-01 07:13:56.000000 fyers_sdk-2.1.1/fyers_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      115 2023-08-01 07:13:56.000000 fyers_sdk-2.1.1/fyers_sdk.egg-info/requires.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-08-01 07:13:56.000000 fyers_sdk-2.1.1/fyers_sdk.egg-info/top_level.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-08-01 07:13:56.569584 fyers_sdk-2.1.1/setup.cfg
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-08-01 07:13:43.000000 fyers_sdk-2.1.1/setup.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:48:06.793663 fyers_sdk-2.1.2/
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-31 10:25:54.000000 fyers_sdk-2.1.2/LICENSE.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-01 07:48:06.793663 fyers_sdk-2.1.2/PKG-INFO
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-2.1.2/README.md
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:48:06.773664 fyers_sdk-2.1.2/fyers_sdk/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:48:06.793663 fyers_sdk-2.1.2/fyers_sdk/FyersWebsocket/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-2.1.2/fyers_sdk/FyersWebsocket/__init__.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    59911 2023-08-01 07:45:38.000000 fyers_sdk-2.1.2/fyers_sdk/FyersWebsocket/data_ws.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     1140 2023-08-01 06:21:10.000000 fyers_sdk-2.1.2/fyers_sdk/FyersWebsocket/defines.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     7541 2023-08-01 07:28:21.000000 fyers_sdk-2.1.2/fyers_sdk/FyersWebsocket/map.json
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    15427 2023-07-31 06:13:16.000000 fyers_sdk-2.1.2/fyers_sdk/FyersWebsocket/order_ws.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-2.1.2/fyers_sdk/__init__.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27819 2023-07-31 09:12:31.000000 fyers_sdk-2.1.2/fyers_sdk/fyersModel.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-2.1.2/fyers_sdk/fyers_logger.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:48:06.789663 fyers_sdk-2.1.2/fyers_sdk.egg-info/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-01 07:48:06.000000 fyers_sdk-2.1.2/fyers_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      446 2023-08-01 07:48:06.000000 fyers_sdk-2.1.2/fyers_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-08-01 07:48:06.000000 fyers_sdk-2.1.2/fyers_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      115 2023-08-01 07:48:06.000000 fyers_sdk-2.1.2/fyers_sdk.egg-info/requires.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-08-01 07:48:06.000000 fyers_sdk-2.1.2/fyers_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-08-01 07:48:06.793663 fyers_sdk-2.1.2/setup.cfg
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-08-01 07:47:37.000000 fyers_sdk-2.1.2/setup.py
```

### Comparing `fyers_sdk-2.1.1/LICENSE.txt` & `fyers_sdk-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.1/PKG-INFO` & `fyers_sdk-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers_sdk
-Version: 2.1.1
+Version: 2.1.2
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-2.1.1/README.md` & `fyers_sdk-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.1/fyers_sdk/FyersWebsocket/data_ws.py` & `fyers_sdk-2.1.2/fyers_sdk/FyersWebsocket/data_ws.py`

 * *Files 2% similar despite different names*

```diff
@@ -950,14 +950,17 @@
                     for i, val in enumerate(self.index_val):
                         if val in data_resp and i in [0, 1, 3, 4, 5]:
                             response[val] = data_resp[val] / (
                                 10 ** data_resp["precision"]
                             )
                         elif val in data_resp:
                             response[val] = data_resp[val]
+                        if "prev_close_price" in response and "ltp" in response:
+                            response["ch"] = round((response['ltp']  - response['prev_close_price']),2) 
+                            response["chp"] = round((response["ch"]  / response['prev_close_price'] * 100) , 2)
 
             self.On_message(response)
 
         except Exception as e:
             self.data_logger.exception(e)
 
     def __datafeed_resp(self, data: bytearray):
```

### Comparing `fyers_sdk-2.1.1/fyers_sdk/FyersWebsocket/defines.py` & `fyers_sdk-2.1.2/fyers_sdk/FyersWebsocket/defines.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.1/fyers_sdk/FyersWebsocket/map.json` & `fyers_sdk-2.1.2/fyers_sdk/FyersWebsocket/map.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8848720800889879%*

 * *Differences: {"'data_val'": "{insert: [(4, 'bid_size'), (5, 'ask_size'), (6, 'bid_price'), (7, 'ask_price'), "*

 * *               "(17, 'lower_ckt'), (18, 'upper_ckt')], delete: [18, 17, 7, 6, 5, 4]}",*

 * * "'depthvalue'": "{insert: [(0, 'bid_price1'), (1, 'bid_price2'), (2, 'bid_price3'), (3, "*

 * *                 "'bid_price4'), (4, 'bid_price5'), (5, 'ask_price1'), (6, 'ask_price2'), (7, "*

 * *                 "'ask_price3'), (8, 'ask_price4'), (9, 'ask_price5'), (10, 'bid_size1'), (11, "*

 * *                 "'bid_size2'), (12, 'bid_s […]*

```diff
@@ -1,64 +1,64 @@
 {
     "data_val": [
         "ltp",
         "vol_traded_today",
         "last_traded_time",
         "exch_feed_time",
-        "bidSize",
-        "askSize",
-        "bidPrice",
-        "askPrice",
+        "bid_size",
+        "ask_size",
+        "bid_price",
+        "ask_price",
         "last_traded_qty",
         "tot_buy_qty",
         "tot_sell_qty",
         "avg_trade_price",
         "OI",
         "low_price",
         "high_price",
         "Yhigh",
         "Ylow",
-        "lowCircuit",
-        "upCircuit",
+        "lower_ckt",
+        "upper_ckt",
         "open_price",
         "prev_close_price",
         "type",
         "symbol"
     ],
     "depthvalue": [
-        "bidPrice1",
-        "bidPrice2",
-        "bidPrice3",
-        "bidPrice4",
-        "bidPrice5",
-        "askPrice1",
-        "askPrice2",
-        "askPrice3",
-        "askPrice4",
-        "askPrice5",
-        "bidsize1",
-        "bidsize2",
-        "bidsize3",
-        "bidsize4",
-        "bidsize5",
-        "askSize1",
-        "askSize2",
-        "askSize3",
-        "askSize4",
-        "askSize5",
-        "bidorder1",
-        "bidorder2",
-        "bidorder3",
-        "bidorder4",
-        "bidorder5",
-        "askorder1",
-        "askorder2",
-        "askorder3",
-        "askorder4",
-        "askorder5",
+        "bid_price1",
+        "bid_price2",
+        "bid_price3",
+        "bid_price4",
+        "bid_price5",
+        "ask_price1",
+        "ask_price2",
+        "ask_price3",
+        "ask_price4",
+        "ask_price5",
+        "bid_size1",
+        "bid_size2",
+        "bid_size3",
+        "bid_size4",
+        "bid_size5",
+        "ask_size1",
+        "ask_size2",
+        "ask_size3",
+        "ask_size4",
+        "ask_size5",
+        "bid_order1",
+        "bid_order2",
+        "bid_order3",
+        "bid_order4",
+        "bid_order5",
+        "ask_order1",
+        "ask_order2",
+        "ask_order3",
+        "ask_order4",
+        "ask_order5",
         "type",
         "symbol"
     ],
     "exch_seg_dict": {
         "1010": "nse_cm",
         "1011": "nse_fo",
         "1012": "cde_fo",
```

### Comparing `fyers_sdk-2.1.1/fyers_sdk/FyersWebsocket/order_ws.py` & `fyers_sdk-2.1.2/fyers_sdk/FyersWebsocket/order_ws.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.1/fyers_sdk/fyersModel.py` & `fyers_sdk-2.1.2/fyers_sdk/fyersModel.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.1/fyers_sdk/fyers_logger.py` & `fyers_sdk-2.1.2/fyers_sdk/fyers_logger.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.1/fyers_sdk.egg-info/PKG-INFO` & `fyers_sdk-2.1.2/fyers_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-sdk
-Version: 2.1.1
+Version: 2.1.2
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-2.1.1/setup.py` & `fyers_sdk-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='fyers_sdk',  
-     version='2.1.1',
+     version='2.1.2',
      author="Fyers-Tech",
      author_email="support@fyers.in",
      description="Fyers trading APIs.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/FyersDev/fyers-api-py",
      packages=setuptools.find_packages(),
```

