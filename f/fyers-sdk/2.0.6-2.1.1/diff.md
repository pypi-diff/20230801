# Comparing `tmp/fyers_sdk-2.0.6.tar.gz` & `tmp/fyers_sdk-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_sdk-2.0.6.tar", last modified: Tue Aug  1 07:08:10 2023, max compression
+gzip compressed data, was "fyers_sdk-2.1.1.tar", last modified: Tue Aug  1 07:13:56 2023, max compression
```

## Comparing `fyers_sdk-2.0.6.tar` & `fyers_sdk-2.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:08:10.207900 fyers_sdk-2.0.6/
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-31 10:25:54.000000 fyers_sdk-2.0.6/LICENSE.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-01 07:08:10.203900 fyers_sdk-2.0.6/PKG-INFO
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-2.0.6/README.md
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:08:10.179900 fyers_sdk-2.0.6/fyers_sdk/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:08:10.203900 fyers_sdk-2.0.6/fyers_sdk/FyersWebsocket/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-2.0.6/fyers_sdk/FyersWebsocket/__init__.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    59613 2023-08-01 06:57:51.000000 fyers_sdk-2.0.6/fyers_sdk/FyersWebsocket/data_ws.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     1140 2023-08-01 06:21:10.000000 fyers_sdk-2.0.6/fyers_sdk/FyersWebsocket/defines.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     7508 2023-08-01 07:05:48.000000 fyers_sdk-2.0.6/fyers_sdk/FyersWebsocket/map.json
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    15427 2023-07-31 06:13:16.000000 fyers_sdk-2.0.6/fyers_sdk/FyersWebsocket/order_ws.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-2.0.6/fyers_sdk/__init__.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27819 2023-07-31 09:12:31.000000 fyers_sdk-2.0.6/fyers_sdk/fyersModel.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-2.0.6/fyers_sdk/fyers_logger.py
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:08:10.203900 fyers_sdk-2.0.6/fyers_sdk.egg-info/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-01 07:08:10.000000 fyers_sdk-2.0.6/fyers_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      446 2023-08-01 07:08:10.000000 fyers_sdk-2.0.6/fyers_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-08-01 07:08:10.000000 fyers_sdk-2.0.6/fyers_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      115 2023-08-01 07:08:10.000000 fyers_sdk-2.0.6/fyers_sdk.egg-info/requires.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-08-01 07:08:10.000000 fyers_sdk-2.0.6/fyers_sdk.egg-info/top_level.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-08-01 07:08:10.207900 fyers_sdk-2.0.6/setup.cfg
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-08-01 07:08:05.000000 fyers_sdk-2.0.6/setup.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:13:56.565583 fyers_sdk-2.1.1/
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-31 10:25:54.000000 fyers_sdk-2.1.1/LICENSE.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-01 07:13:56.565583 fyers_sdk-2.1.1/PKG-INFO
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-2.1.1/README.md
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:13:56.541584 fyers_sdk-2.1.1/fyers_sdk/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:13:56.565583 fyers_sdk-2.1.1/fyers_sdk/FyersWebsocket/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-2.1.1/fyers_sdk/FyersWebsocket/__init__.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    59613 2023-08-01 06:57:51.000000 fyers_sdk-2.1.1/fyers_sdk/FyersWebsocket/data_ws.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     1140 2023-08-01 06:21:10.000000 fyers_sdk-2.1.1/fyers_sdk/FyersWebsocket/defines.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     7508 2023-08-01 07:05:48.000000 fyers_sdk-2.1.1/fyers_sdk/FyersWebsocket/map.json
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    15427 2023-07-31 06:13:16.000000 fyers_sdk-2.1.1/fyers_sdk/FyersWebsocket/order_ws.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-2.1.1/fyers_sdk/__init__.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27819 2023-07-31 09:12:31.000000 fyers_sdk-2.1.1/fyers_sdk/fyersModel.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-2.1.1/fyers_sdk/fyers_logger.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:13:56.561583 fyers_sdk-2.1.1/fyers_sdk.egg-info/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-01 07:13:56.000000 fyers_sdk-2.1.1/fyers_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      446 2023-08-01 07:13:56.000000 fyers_sdk-2.1.1/fyers_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-08-01 07:13:56.000000 fyers_sdk-2.1.1/fyers_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      115 2023-08-01 07:13:56.000000 fyers_sdk-2.1.1/fyers_sdk.egg-info/requires.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-08-01 07:13:56.000000 fyers_sdk-2.1.1/fyers_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-08-01 07:13:56.569584 fyers_sdk-2.1.1/setup.cfg
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-08-01 07:13:43.000000 fyers_sdk-2.1.1/setup.py
```

### Comparing `fyers_sdk-2.0.6/LICENSE.txt` & `fyers_sdk-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.0.6/PKG-INFO` & `fyers_sdk-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers_sdk
-Version: 2.0.6
+Version: 2.1.1
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-2.0.6/README.md` & `fyers_sdk-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.0.6/fyers_sdk/FyersWebsocket/data_ws.py` & `fyers_sdk-2.1.1/fyers_sdk/FyersWebsocket/data_ws.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.0.6/fyers_sdk/FyersWebsocket/defines.py` & `fyers_sdk-2.1.1/fyers_sdk/FyersWebsocket/defines.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.0.6/fyers_sdk/FyersWebsocket/map.json` & `fyers_sdk-2.1.1/fyers_sdk/FyersWebsocket/map.json`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.0.6/fyers_sdk/FyersWebsocket/order_ws.py` & `fyers_sdk-2.1.1/fyers_sdk/FyersWebsocket/order_ws.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.0.6/fyers_sdk/fyersModel.py` & `fyers_sdk-2.1.1/fyers_sdk/fyersModel.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.0.6/fyers_sdk/fyers_logger.py` & `fyers_sdk-2.1.1/fyers_sdk/fyers_logger.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.0.6/fyers_sdk.egg-info/PKG-INFO` & `fyers_sdk-2.1.1/fyers_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-sdk
-Version: 2.0.6
+Version: 2.1.1
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-2.0.6/setup.py` & `fyers_sdk-2.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='fyers_sdk',  
-     version='2.0.6',
+     version='2.1.1',
      author="Fyers-Tech",
      author_email="support@fyers.in",
      description="Fyers trading APIs.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/FyersDev/fyers-api-py",
      packages=setuptools.find_packages(),
```

