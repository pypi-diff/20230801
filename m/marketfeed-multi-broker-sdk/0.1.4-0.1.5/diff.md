# Comparing `tmp/marketfeed_multi_broker_sdk-0.1.4.tar.gz` & `tmp/marketfeed_multi_broker_sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marketfeed_multi_broker_sdk-0.1.4.tar", last modified: Tue Aug  1 07:19:01 2023, max compression
+gzip compressed data, was "marketfeed_multi_broker_sdk-0.1.5.tar", last modified: Tue Aug  1 07:22:15 2023, max compression
```

## Comparing `marketfeed_multi_broker_sdk-0.1.4.tar` & `marketfeed_multi_broker_sdk-0.1.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-01 07:19:01.319085 marketfeed_multi_broker_sdk-0.1.4/
--rw-r--r--   0 farazs     (501) staff       (20)     2538 2023-08-01 07:19:01.318837 marketfeed_multi_broker_sdk-0.1.4/PKG-INFO
--rw-r--r--   0 farazs     (501) staff       (20)     2291 2023-08-01 07:17:38.000000 marketfeed_multi_broker_sdk-0.1.4/README.md
-drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-01 07:19:01.311898 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/
--rw-r--r--   0 farazs     (501) staff       (20)      382 2023-08-01 07:00:16.000000 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/__init__.py
--rw-r--r--   0 farazs     (501) staff       (20)      698 2023-08-01 06:57:44.000000 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/broker_interface.py
--rw-r--r--   0 farazs     (501) staff       (20)     1481 2023-08-01 06:57:31.000000 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/broker_sdk.py
-drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-01 07:19:01.315004 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/brokers/
--rw-r--r--   0 farazs     (501) staff       (20)        0 2023-07-22 19:58:31.000000 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/brokers/__init__.py
--rw-r--r--   0 farazs     (501) staff       (20)     1431 2023-08-01 07:01:22.000000 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/brokers/fyers.py
--rw-r--r--   0 farazs     (501) staff       (20)     1306 2023-07-26 20:52:11.000000 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/brokers/iifl.py
--rw-r--r--   0 farazs     (501) staff       (20)     1516 2023-07-28 07:03:20.000000 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/brokers/kotak.py
--rw-r--r--   0 farazs     (501) staff       (20)     1678 2023-07-31 11:01:09.000000 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/brokers/shoonya.py
--rw-r--r--   0 farazs     (501) staff       (20)     1508 2023-07-27 09:50:19.000000 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/brokers/xts.py
--rw-r--r--   0 farazs     (501) staff       (20)     1383 2023-08-01 06:52:06.000000 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/enums.py
--rw-r--r--   0 farazs     (501) staff       (20)     1535 2023-08-01 06:08:20.000000 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/models.py
-drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-01 07:19:01.316469 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/services/
--rw-r--r--   0 farazs     (501) staff       (20)        0 2023-07-27 05:40:23.000000 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/services/__init__.py
--rw-r--r--   0 farazs     (501) staff       (20)     6024 2023-07-31 11:33:15.000000 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/services/fyers_services.py
--rw-r--r--   0 farazs     (501) staff       (20)     4769 2023-07-30 08:32:51.000000 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/services/kotak_services.py
--rw-r--r--   0 farazs     (501) staff       (20)     6347 2023-08-01 06:54:49.000000 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/services/shoonya_services.py
--rw-r--r--   0 farazs     (501) staff       (20)     2650 2023-07-26 22:37:48.000000 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/services/xts_services.py
-drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-01 07:19:01.312829 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk.egg-info/
--rw-r--r--   0 farazs     (501) staff       (20)     2538 2023-08-01 07:19:01.000000 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk.egg-info/PKG-INFO
--rw-r--r--   0 farazs     (501) staff       (20)     1121 2023-08-01 07:19:01.000000 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 farazs     (501) staff       (20)        1 2023-08-01 07:19:01.000000 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 farazs     (501) staff       (20)       18 2023-08-01 07:19:01.000000 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk.egg-info/requires.txt
--rw-r--r--   0 farazs     (501) staff       (20)       34 2023-08-01 07:19:01.000000 marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk.egg-info/top_level.txt
--rw-r--r--   0 farazs     (501) staff       (20)       38 2023-08-01 07:19:01.319183 marketfeed_multi_broker_sdk-0.1.4/setup.cfg
--rw-r--r--   0 farazs     (501) staff       (20)      663 2023-08-01 07:18:40.000000 marketfeed_multi_broker_sdk-0.1.4/setup.py
-drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-01 07:19:01.318371 marketfeed_multi_broker_sdk-0.1.4/tests/
--rw-r--r--   0 farazs     (501) staff       (20)        0 2023-07-04 08:53:00.000000 marketfeed_multi_broker_sdk-0.1.4/tests/__init__.py
--rw-r--r--   0 farazs     (501) staff       (20)     1483 2023-07-31 09:13:09.000000 marketfeed_multi_broker_sdk-0.1.4/tests/test_fyers.py
--rw-r--r--   0 farazs     (501) staff       (20)     1156 2023-07-22 20:22:12.000000 marketfeed_multi_broker_sdk-0.1.4/tests/test_fyers_mock.py
--rw-r--r--   0 farazs     (501) staff       (20)     1622 2023-07-27 09:53:30.000000 marketfeed_multi_broker_sdk-0.1.4/tests/test_shoonya.py
--rw-r--r--   0 farazs     (501) staff       (20)     1480 2023-07-26 22:47:12.000000 marketfeed_multi_broker_sdk-0.1.4/tests/test_xts.py
+drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-01 07:22:15.376624 marketfeed_multi_broker_sdk-0.1.5/
+-rw-r--r--   0 farazs     (501) staff       (20)     2556 2023-08-01 07:22:15.376453 marketfeed_multi_broker_sdk-0.1.5/PKG-INFO
+-rw-r--r--   0 farazs     (501) staff       (20)     2309 2023-08-01 07:21:55.000000 marketfeed_multi_broker_sdk-0.1.5/README.md
+drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-01 07:22:15.368419 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/
+-rw-r--r--   0 farazs     (501) staff       (20)      382 2023-08-01 07:00:16.000000 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/__init__.py
+-rw-r--r--   0 farazs     (501) staff       (20)      698 2023-08-01 06:57:44.000000 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/broker_interface.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1481 2023-08-01 06:57:31.000000 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/broker_sdk.py
+drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-01 07:22:15.372043 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/brokers/
+-rw-r--r--   0 farazs     (501) staff       (20)        0 2023-07-22 19:58:31.000000 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/brokers/__init__.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1431 2023-08-01 07:01:22.000000 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/brokers/fyers.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1306 2023-07-26 20:52:11.000000 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/brokers/iifl.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1516 2023-07-28 07:03:20.000000 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/brokers/kotak.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1678 2023-07-31 11:01:09.000000 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/brokers/shoonya.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1508 2023-07-27 09:50:19.000000 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/brokers/xts.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1383 2023-08-01 06:52:06.000000 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/enums.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1535 2023-08-01 06:08:20.000000 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/models.py
+drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-01 07:22:15.373651 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/services/
+-rw-r--r--   0 farazs     (501) staff       (20)        0 2023-07-27 05:40:23.000000 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/services/__init__.py
+-rw-r--r--   0 farazs     (501) staff       (20)     6024 2023-07-31 11:33:15.000000 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/services/fyers_services.py
+-rw-r--r--   0 farazs     (501) staff       (20)     4769 2023-07-30 08:32:51.000000 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/services/kotak_services.py
+-rw-r--r--   0 farazs     (501) staff       (20)     6347 2023-08-01 06:54:49.000000 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/services/shoonya_services.py
+-rw-r--r--   0 farazs     (501) staff       (20)     2650 2023-07-26 22:37:48.000000 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/services/xts_services.py
+drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-01 07:22:15.369633 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk.egg-info/
+-rw-r--r--   0 farazs     (501) staff       (20)     2556 2023-08-01 07:22:15.000000 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 farazs     (501) staff       (20)     1121 2023-08-01 07:22:15.000000 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 farazs     (501) staff       (20)        1 2023-08-01 07:22:15.000000 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 farazs     (501) staff       (20)       18 2023-08-01 07:22:15.000000 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk.egg-info/requires.txt
+-rw-r--r--   0 farazs     (501) staff       (20)       34 2023-08-01 07:22:15.000000 marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk.egg-info/top_level.txt
+-rw-r--r--   0 farazs     (501) staff       (20)       38 2023-08-01 07:22:15.376690 marketfeed_multi_broker_sdk-0.1.5/setup.cfg
+-rw-r--r--   0 farazs     (501) staff       (20)      663 2023-08-01 07:22:12.000000 marketfeed_multi_broker_sdk-0.1.5/setup.py
+drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-01 07:22:15.375930 marketfeed_multi_broker_sdk-0.1.5/tests/
+-rw-r--r--   0 farazs     (501) staff       (20)        0 2023-07-04 08:53:00.000000 marketfeed_multi_broker_sdk-0.1.5/tests/__init__.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1483 2023-07-31 09:13:09.000000 marketfeed_multi_broker_sdk-0.1.5/tests/test_fyers.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1156 2023-07-22 20:22:12.000000 marketfeed_multi_broker_sdk-0.1.5/tests/test_fyers_mock.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1622 2023-07-27 09:53:30.000000 marketfeed_multi_broker_sdk-0.1.5/tests/test_shoonya.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1480 2023-07-26 22:47:12.000000 marketfeed_multi_broker_sdk-0.1.5/tests/test_xts.py
```

### Comparing `marketfeed_multi_broker_sdk-0.1.4/PKG-INFO` & `marketfeed_multi_broker_sdk-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marketfeed_multi_broker_sdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: Multi Broker SDK
 Home-page: https://github.com/tradeclone/multi-broker-sdk
 Author: Faraz
 Author-email: faraz.s@marketfeed.com
 Description-Content-Type: text/markdown
 
 # Multi-Broker SDK
@@ -21,22 +21,22 @@
 
 ## Usage
 
 To utilize the functionality of BrokerSDK, import it into your Python script:
 
 ```
 from marketfeed_multi_broker_sdk import BrokerSDK
-from marketfeed_multi_broker_sdk import Login, LoginResponse
+from marketfeed_multi_broker_sdk import Broker, Login, LoginResponse
 ```
 
 Initialize the SDK with the specific broker's name and user details:
 
 ```
-sdk_xts = BrokerSDK('xts', client_code='6881359')
-sdk_fyers = BrokerSDK('fyers', client_code='XM10188')
+sdk_xts = BrokerSDK(Broker.XTS, client_code='6881359')
+sdk_fyers = BrokerSDK(Broker.FYERS, client_code='XM10188')
 
 ```
 
 Use the BrokerSDK to log in. The BrokerSDK handles communication with the specific broker based on the provided broker name.
 
 For FYERS:
```

### Comparing `marketfeed_multi_broker_sdk-0.1.4/README.md` & `marketfeed_multi_broker_sdk-0.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 
 ## Usage
 
 To utilize the functionality of BrokerSDK, import it into your Python script:
 
 ```
 from marketfeed_multi_broker_sdk import BrokerSDK
-from marketfeed_multi_broker_sdk import Login, LoginResponse
+from marketfeed_multi_broker_sdk import Broker, Login, LoginResponse
 ```
 
 Initialize the SDK with the specific broker's name and user details:
 
 ```
-sdk_xts = BrokerSDK('xts', client_code='6881359')
-sdk_fyers = BrokerSDK('fyers', client_code='XM10188')
+sdk_xts = BrokerSDK(Broker.XTS, client_code='6881359')
+sdk_fyers = BrokerSDK(Broker.FYERS, client_code='XM10188')
 
 ```
 
 Use the BrokerSDK to log in. The BrokerSDK handles communication with the specific broker based on the provided broker name.
 
 For FYERS:
```

### Comparing `marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/broker_interface.py` & `marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/broker_interface.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/broker_sdk.py` & `marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/broker_sdk.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/brokers/fyers.py` & `marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/brokers/fyers.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/brokers/iifl.py` & `marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/brokers/iifl.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/brokers/kotak.py` & `marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/brokers/kotak.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/brokers/shoonya.py` & `marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/brokers/shoonya.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/brokers/xts.py` & `marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/brokers/xts.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/enums.py` & `marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/enums.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/models.py` & `marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/models.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/services/fyers_services.py` & `marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/services/fyers_services.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/services/kotak_services.py` & `marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/services/kotak_services.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/services/shoonya_services.py` & `marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/services/shoonya_services.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk/services/xts_services.py` & `marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk/services/xts_services.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk.egg-info/PKG-INFO` & `marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marketfeed-multi-broker-sdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: Multi Broker SDK
 Home-page: https://github.com/tradeclone/multi-broker-sdk
 Author: Faraz
 Author-email: faraz.s@marketfeed.com
 Description-Content-Type: text/markdown
 
 # Multi-Broker SDK
@@ -21,22 +21,22 @@
 
 ## Usage
 
 To utilize the functionality of BrokerSDK, import it into your Python script:
 
 ```
 from marketfeed_multi_broker_sdk import BrokerSDK
-from marketfeed_multi_broker_sdk import Login, LoginResponse
+from marketfeed_multi_broker_sdk import Broker, Login, LoginResponse
 ```
 
 Initialize the SDK with the specific broker's name and user details:
 
 ```
-sdk_xts = BrokerSDK('xts', client_code='6881359')
-sdk_fyers = BrokerSDK('fyers', client_code='XM10188')
+sdk_xts = BrokerSDK(Broker.XTS, client_code='6881359')
+sdk_fyers = BrokerSDK(Broker.FYERS, client_code='XM10188')
 
 ```
 
 Use the BrokerSDK to log in. The BrokerSDK handles communication with the specific broker based on the provided broker name.
 
 For FYERS:
```

### Comparing `marketfeed_multi_broker_sdk-0.1.4/marketfeed_multi_broker_sdk.egg-info/SOURCES.txt` & `marketfeed_multi_broker_sdk-0.1.5/marketfeed_multi_broker_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.4/setup.py` & `marketfeed_multi_broker_sdk-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Get the long description from the README file
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='marketfeed_multi_broker_sdk',
-    version='0.1.4',
+    version='0.1.5',
     url='https://github.com/tradeclone/multi-broker-sdk',
     author='Faraz',
     author_email='faraz.s@marketfeed.com',
     description='Multi Broker SDK',
     long_description=long_description,
     long_description_content_type='text/markdown',  # This is important!
     packages=find_packages(),
```

### Comparing `marketfeed_multi_broker_sdk-0.1.4/tests/test_fyers.py` & `marketfeed_multi_broker_sdk-0.1.5/tests/test_fyers.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.4/tests/test_fyers_mock.py` & `marketfeed_multi_broker_sdk-0.1.5/tests/test_fyers_mock.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.4/tests/test_shoonya.py` & `marketfeed_multi_broker_sdk-0.1.5/tests/test_shoonya.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.4/tests/test_xts.py` & `marketfeed_multi_broker_sdk-0.1.5/tests/test_xts.py`

 * *Files identical despite different names*

