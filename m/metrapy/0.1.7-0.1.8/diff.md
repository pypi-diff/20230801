# Comparing `tmp/metrapy-0.1.7.tar.gz` & `tmp/metrapy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metrapy-0.1.7.tar", last modified: Thu Jul 27 17:25:07 2023, max compression
+gzip compressed data, was "metrapy-0.1.8.tar", last modified: Tue Aug  1 16:37:27 2023, max compression
```

## Comparing `metrapy-0.1.7.tar` & `metrapy-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 17:25:07.306763 metrapy-0.1.7/
--rw-rw-rw-   0        0        0     2670 2023-07-27 17:25:07.306763 metrapy-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2347 2023-07-19 20:01:09.000000 metrapy-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 17:25:07.274757 metrapy-0.1.7/metrapy/
--rw-rw-rw-   0        0        0        0 2023-07-25 03:44:41.000000 metrapy-0.1.7/metrapy/__init__.py
--rw-rw-rw-   0        0        0    13885 2023-07-27 16:52:55.000000 metrapy-0.1.7/metrapy/connector.py
--rw-rw-rw-   0        0        0      205 2023-07-19 19:33:58.000000 metrapy-0.1.7/metrapy/defaults.py
--rw-rw-rw-   0        0        0     2414 2023-07-19 19:32:18.000000 metrapy-0.1.7/metrapy/maps.py
--rw-rw-rw-   0        0        0     1877 2023-07-19 19:33:47.000000 metrapy-0.1.7/metrapy/sync.py
--rw-rw-rw-   0        0        0      616 2023-07-27 17:24:52.000000 metrapy-0.1.7/metrapy/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-27 17:25:07.306763 metrapy-0.1.7/metrapy.egg-info/
--rw-rw-rw-   0        0        0     2670 2023-07-27 17:25:06.000000 metrapy-0.1.7/metrapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-07-27 17:25:07.000000 metrapy-0.1.7/metrapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 17:25:06.000000 metrapy-0.1.7/metrapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-27 17:25:06.000000 metrapy-0.1.7/metrapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-27 17:25:06.000000 metrapy-0.1.7/metrapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 17:25:07.306763 metrapy-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1081 2023-07-27 17:25:01.000000 metrapy-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 16:37:27.340265 metrapy-0.1.8/
+-rw-rw-rw-   0        0        0     2670 2023-08-01 16:37:27.340265 metrapy-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2347 2023-07-19 20:01:09.000000 metrapy-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 16:37:27.292478 metrapy-0.1.8/metrapy/
+-rw-rw-rw-   0        0        0        0 2023-07-25 03:44:41.000000 metrapy-0.1.8/metrapy/__init__.py
+-rw-rw-rw-   0        0        0    13920 2023-08-01 16:36:39.000000 metrapy-0.1.8/metrapy/connector.py
+-rw-rw-rw-   0        0        0      205 2023-07-19 19:33:58.000000 metrapy-0.1.8/metrapy/defaults.py
+-rw-rw-rw-   0        0        0     2414 2023-07-19 19:32:18.000000 metrapy-0.1.8/metrapy/maps.py
+-rw-rw-rw-   0        0        0     1877 2023-07-19 19:33:47.000000 metrapy-0.1.8/metrapy/sync.py
+-rw-rw-rw-   0        0        0      616 2023-07-27 17:24:52.000000 metrapy-0.1.8/metrapy/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-01 16:37:27.337238 metrapy-0.1.8/metrapy.egg-info/
+-rw-rw-rw-   0        0        0     2670 2023-08-01 16:37:26.000000 metrapy-0.1.8/metrapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-08-01 16:37:27.000000 metrapy-0.1.8/metrapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 16:37:26.000000 metrapy-0.1.8/metrapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-01 16:37:26.000000 metrapy-0.1.8/metrapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-08-01 16:37:26.000000 metrapy-0.1.8/metrapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 16:37:27.340265 metrapy-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2023-08-01 16:37:21.000000 metrapy-0.1.8/setup.py
```

### Comparing `metrapy-0.1.7/PKG-INFO` & `metrapy-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metrapy
-Version: 0.1.7
+Version: 0.1.8
 Summary: batteries included wrapper utility for MetaTrader5's python integration
 Author: pavittarx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `metrapy-0.1.7/README.md` & `metrapy-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `metrapy-0.1.7/metrapy/connector.py` & `metrapy-0.1.8/metrapy/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         if self.debug:
             print(
                 "Candles Fetched: ",
                 params["ticker"],
                 get_current_time().strftime("%m/%d/%Y, %H:%M:%S", len(candles)),
             )
 
-        candles_df = get_candles_df(candles, timezone= params['timezone'] if "timezone" in params else None)
+        candles_df = get_candles_df(candles, timezone= params['timezone'] if "timezone" in params else self.timezone or None)
 
         return {"candles": candles, "last_error": None, "params": params, 'candles_df': candles_df}
 
     def get_last_candle(self, params):
         if "ticker" not in params:
                 raise Exception("Please provide ticker information")
         
@@ -162,15 +162,15 @@
         if self.debug:
                 print(
                     "Candles Fetched: ",
                     params["ticker"],
                     get_current_time().strftime("%m/%d/%Y, %H:%M:%S", len(candle_raw)),
                 )
         
-        candle = get_candles_df(candle_raw, timezone= params['timezone'] if "timezone" in params else None)
+        candle = get_candles_df(candle_raw, timezone=  params['timezone'] if "timezone" in params else self.timezone or None)
         
         return {"candle_raw": candle[0] if len(candle) > 0 else None, "last_error": None, "params": params, 'candles_df': candle.iloc[0] if candle else None}
 
     def get_orders(self, params):
         request = {}
 
         if "ticker" in params:
```

### Comparing `metrapy-0.1.7/metrapy/maps.py` & `metrapy-0.1.8/metrapy/maps.py`

 * *Files identical despite different names*

### Comparing `metrapy-0.1.7/metrapy/sync.py` & `metrapy-0.1.8/metrapy/sync.py`

 * *Files identical despite different names*

### Comparing `metrapy-0.1.7/metrapy/utils.py` & `metrapy-0.1.8/metrapy/utils.py`

 * *Files identical despite different names*

### Comparing `metrapy-0.1.7/metrapy.egg-info/PKG-INFO` & `metrapy-0.1.8/metrapy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metrapy
-Version: 0.1.7
+Version: 0.1.8
 Summary: batteries included wrapper utility for MetaTrader5's python integration
 Author: pavittarx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `metrapy-0.1.7/setup.py` & `metrapy-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="metrapy",  # This is the name of the package
-    version="0.1.7",  # The initial release version
+    version="0.1.8",  # The initial release version
     author="pavittarx",  # Full name of the author
     description="batteries included wrapper utility for MetaTrader5's python integration",
     long_description=long_description,  # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),  # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

