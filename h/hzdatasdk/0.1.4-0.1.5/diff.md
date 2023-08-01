# Comparing `tmp/hzdatasdk-0.1.4.tar.gz` & `tmp/hzdatasdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hzdatasdk-0.1.4.tar", last modified: Mon Jul 31 09:56:42 2023, max compression
+gzip compressed data, was "hzdatasdk-0.1.5.tar", last modified: Tue Aug  1 05:21:59 2023, max compression
```

## Comparing `hzdatasdk-0.1.4.tar` & `hzdatasdk-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 09:56:42.855260 hzdatasdk-0.1.4/
--rw-rw-rw-   0        0        0     1091 2022-06-09 02:32:27.000000 hzdatasdk-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1304 2023-07-31 09:56:42.856260 hzdatasdk-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      802 2023-01-18 01:06:13.000000 hzdatasdk-0.1.4/README.md
--rw-rw-rw-   0        0        0      109 2022-06-09 02:32:27.000000 hzdatasdk-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0      714 2023-07-31 09:56:42.859262 hzdatasdk-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-31 09:56:42.600259 hzdatasdk-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-31 09:56:42.760261 hzdatasdk-0.1.4/src/hzdatasdk/
--rw-rw-rw-   0        0        0      346 2022-06-09 02:32:27.000000 hzdatasdk-0.1.4/src/hzdatasdk/__init__.py
--rw-rw-rw-   0        0        0     6186 2023-07-31 08:05:22.000000 hzdatasdk-0.1.4/src/hzdatasdk/api.py
--rw-rw-rw-   0        0        0    71706 2022-06-09 02:32:27.000000 hzdatasdk-0.1.4/src/hzdatasdk/choice.py
--rw-rw-rw-   0        0        0     8695 2022-06-09 02:32:27.000000 hzdatasdk-0.1.4/src/hzdatasdk/choiceinfo.py
--rw-rw-rw-   0        0        0     3171 2023-07-31 09:47:07.000000 hzdatasdk-0.1.4/src/hzdatasdk/client.py
--rw-rw-rw-   0        0        0     3484 2022-06-09 02:32:27.000000 hzdatasdk-0.1.4/src/hzdatasdk/hz_finance_service.py
--rw-rw-rw-   0        0        0     5371 2022-06-09 02:32:27.000000 hzdatasdk-0.1.4/src/hzdatasdk/hzdata_pb2.py
--rw-rw-rw-   0        0        0     2413 2022-06-09 02:32:27.000000 hzdatasdk-0.1.4/src/hzdatasdk/hzdata_pb2_grpc.py
--rw-rw-rw-   0        0        0    10697 2022-06-09 02:32:27.000000 hzdatasdk-0.1.4/src/hzdatasdk/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:56:42.845260 hzdatasdk-0.1.4/src/hzdatasdk.egg-info/
--rw-rw-rw-   0        0        0     1304 2023-07-31 09:56:42.000000 hzdatasdk-0.1.4/src/hzdatasdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      469 2023-07-31 09:56:42.000000 hzdatasdk-0.1.4/src/hzdatasdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 09:56:42.000000 hzdatasdk-0.1.4/src/hzdatasdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-07-31 09:56:42.000000 hzdatasdk-0.1.4/src/hzdatasdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-31 09:56:42.000000 hzdatasdk-0.1.4/src/hzdatasdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 05:21:59.858952 hzdatasdk-0.1.5/
+-rw-rw-rw-   0        0        0     1091 2022-06-09 02:32:27.000000 hzdatasdk-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1304 2023-08-01 05:21:59.860952 hzdatasdk-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      802 2023-01-18 01:06:13.000000 hzdatasdk-0.1.5/README.md
+-rw-rw-rw-   0        0        0      109 2022-06-09 02:32:27.000000 hzdatasdk-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0      714 2023-08-01 05:21:59.864951 hzdatasdk-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 05:21:59.557953 hzdatasdk-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 05:21:59.774952 hzdatasdk-0.1.5/src/hzdatasdk/
+-rw-rw-rw-   0        0        0      346 2022-06-09 02:32:27.000000 hzdatasdk-0.1.5/src/hzdatasdk/__init__.py
+-rw-rw-rw-   0        0        0     6180 2023-08-01 05:19:41.000000 hzdatasdk-0.1.5/src/hzdatasdk/api.py
+-rw-rw-rw-   0        0        0    71706 2022-06-09 02:32:27.000000 hzdatasdk-0.1.5/src/hzdatasdk/choice.py
+-rw-rw-rw-   0        0        0     8695 2022-06-09 02:32:27.000000 hzdatasdk-0.1.5/src/hzdatasdk/choiceinfo.py
+-rw-rw-rw-   0        0        0     3171 2023-07-31 09:47:07.000000 hzdatasdk-0.1.5/src/hzdatasdk/client.py
+-rw-rw-rw-   0        0        0     3484 2022-06-09 02:32:27.000000 hzdatasdk-0.1.5/src/hzdatasdk/hz_finance_service.py
+-rw-rw-rw-   0        0        0     5371 2022-06-09 02:32:27.000000 hzdatasdk-0.1.5/src/hzdatasdk/hzdata_pb2.py
+-rw-rw-rw-   0        0        0     2413 2022-06-09 02:32:27.000000 hzdatasdk-0.1.5/src/hzdatasdk/hzdata_pb2_grpc.py
+-rw-rw-rw-   0        0        0    10697 2022-06-09 02:32:27.000000 hzdatasdk-0.1.5/src/hzdatasdk/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-01 05:21:59.846951 hzdatasdk-0.1.5/src/hzdatasdk.egg-info/
+-rw-rw-rw-   0        0        0     1304 2023-08-01 05:21:59.000000 hzdatasdk-0.1.5/src/hzdatasdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2023-08-01 05:21:59.000000 hzdatasdk-0.1.5/src/hzdatasdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 05:21:59.000000 hzdatasdk-0.1.5/src/hzdatasdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-08-01 05:21:59.000000 hzdatasdk-0.1.5/src/hzdatasdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-01 05:21:59.000000 hzdatasdk-0.1.5/src/hzdatasdk.egg-info/top_level.txt
```

### Comparing `hzdatasdk-0.1.4/LICENSE` & `hzdatasdk-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hzdatasdk-0.1.4/PKG-INFO` & `hzdatasdk-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hzdatasdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: shanghai hz finance data sdk
 Home-page: https://github.com/pypa/hzdatasdk
 Author: hz finance
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pypa/hzdatasdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hzdatasdk-0.1.4/README.md` & `hzdatasdk-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `hzdatasdk-0.1.4/setup.cfg` & `hzdatasdk-0.1.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2068 7a64 6174 6173 646b 0d0a 7665   = hzdatasdk..ve
-00000020: 7273 696f 6e20 3d20 302e 312e 340d 0a61  rsion = 0.1.4..a
+00000020: 7273 696f 6e20 3d20 302e 312e 350d 0a61  rsion = 0.1.5..a
 00000030: 7574 686f 7220 3d20 687a 2066 696e 616e  uthor = hz finan
 00000040: 6365 0d0a 6175 7468 6f72 5f65 6d61 696c  ce..author_email
 00000050: 203d 2061 7574 686f 7240 6578 616d 706c   = author@exampl
 00000060: 652e 636f 6d0d 0a64 6573 6372 6970 7469  e.com..descripti
 00000070: 6f6e 203d 2073 6861 6e67 6861 6920 687a  on = shanghai hz
 00000080: 2066 696e 616e 6365 2064 6174 6120 7364   finance data sd
 00000090: 6b0d 0a6c 6f6e 675f 6465 7363 7269 7074  k..long_descript
```

### Comparing `hzdatasdk-0.1.4/src/hzdatasdk/api.py` & `hzdatasdk-0.1.5/src/hzdatasdk/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,29 +107,29 @@
     end_date = to_datetime_str(end_date)
     if (not count) and (not start_date):
         start_date = "2015-01-01"
     if count and start_date:
         raise ParamsError("(start_date, count) only one param is required")
     return HZDataClient.instance().get_industry(**locals())
 
-def query_minute_trade(security=None, date=None):
+def get_minute_trade(security=None, date=None):
     if security is None:
         raise ParamsError("security is required")
     if date is None:
         raise ParamsError("date is required")
     return HZDataClient.instance().get_minute_trade(**locals())
 
-def query_minute_buy_sell1(security=None, date=None):
+def get_minute_buy_sell1(security=None, date=None):
     if security is None:
         raise ParamsError("security is required")
     if date is None:
         raise ParamsError("date is required")
     return HZDataClient.instance().get_minute_buy_sell1(**locals())
 
-def query_minute_kline(security=None, date=None):
+def get_minute_kline(security=None, date=None):
     if security is None:
         raise ParamsError("security is required")
     if date is None:
         raise ParamsError("date is required")
     return HZDataClient.instance().get_minute_kline(**locals())
```

### Comparing `hzdatasdk-0.1.4/src/hzdatasdk/choice.py` & `hzdatasdk-0.1.5/src/hzdatasdk/choice.py`

 * *Files identical despite different names*

### Comparing `hzdatasdk-0.1.4/src/hzdatasdk/choiceinfo.py` & `hzdatasdk-0.1.5/src/hzdatasdk/choiceinfo.py`

 * *Files identical despite different names*

### Comparing `hzdatasdk-0.1.4/src/hzdatasdk/client.py` & `hzdatasdk-0.1.5/src/hzdatasdk/client.py`

 * *Files identical despite different names*

### Comparing `hzdatasdk-0.1.4/src/hzdatasdk/hz_finance_service.py` & `hzdatasdk-0.1.5/src/hzdatasdk/hz_finance_service.py`

 * *Files identical despite different names*

### Comparing `hzdatasdk-0.1.4/src/hzdatasdk/hzdata_pb2.py` & `hzdatasdk-0.1.5/src/hzdatasdk/hzdata_pb2.py`

 * *Files identical despite different names*

### Comparing `hzdatasdk-0.1.4/src/hzdatasdk/hzdata_pb2_grpc.py` & `hzdatasdk-0.1.5/src/hzdatasdk/hzdata_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hzdatasdk-0.1.4/src/hzdatasdk/utils.py` & `hzdatasdk-0.1.5/src/hzdatasdk/utils.py`

 * *Files identical despite different names*

### Comparing `hzdatasdk-0.1.4/src/hzdatasdk.egg-info/PKG-INFO` & `hzdatasdk-0.1.5/src/hzdatasdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hzdatasdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: shanghai hz finance data sdk
 Home-page: https://github.com/pypa/hzdatasdk
 Author: hz finance
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pypa/hzdatasdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

