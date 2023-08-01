# Comparing `tmp/datamarket-0.3.8.tar.gz` & `tmp/datamarket-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamarket-0.3.8.tar", last modified: Wed Jul 26 10:35:36 2023, max compression
+gzip compressed data, was "datamarket-0.3.9.tar", last modified: Tue Aug  1 06:37:04 2023, max compression
```

## Comparing `datamarket-0.3.8.tar` & `datamarket-0.3.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 10:35:36.013301 datamarket-0.3.8/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35149 2021-10-07 14:37:41.000000 datamarket-0.3.8/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1486 2023-07-26 10:35:36.013301 datamarket-0.3.8/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      934 2023-05-25 14:26:25.000000 datamarket-0.3.8/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-26 10:35:36.013301 datamarket-0.3.8/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1050 2023-07-26 10:34:42.000000 datamarket-0.3.8/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 10:35:36.009301 datamarket-0.3.8/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 10:35:36.009301 datamarket-0.3.8/src/datamarket/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2021-11-03 08:15:04.000000 datamarket-0.3.8/src/datamarket/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 10:35:36.013301 datamarket-0.3.8/src/datamarket/interfaces/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-03 09:55:33.000000 datamarket-0.3.8/src/datamarket/interfaces/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3104 2023-02-16 08:03:41.000000 datamarket-0.3.8/src/datamarket/interfaces/alchemy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2022-08-08 10:00:49.000000 datamarket-0.3.8/src/datamarket/interfaces/drive.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1344 2023-02-17 11:31:46.000000 datamarket-0.3.8/src/datamarket/interfaces/ftp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2023-04-14 11:21:25.000000 datamarket-0.3.8/src/datamarket/interfaces/proxy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2565 2023-03-14 07:00:34.000000 datamarket-0.3.8/src/datamarket/interfaces/tinybird.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 10:35:36.013301 datamarket-0.3.8/src/datamarket/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-05-26 09:46:08.000000 datamarket-0.3.8/src/datamarket/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1738 2023-05-25 14:18:08.000000 datamarket-0.3.8/src/datamarket/utils/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2488 2023-07-26 10:34:42.000000 datamarket-0.3.8/src/datamarket/utils/selenium.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 10:35:36.009301 datamarket-0.3.8/src/datamarket.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1486 2023-07-26 10:35:36.000000 datamarket-0.3.8/src/datamarket.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      553 2023-07-26 10:35:36.000000 datamarket-0.3.8/src/datamarket.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-26 10:35:36.000000 datamarket-0.3.8/src/datamarket.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       70 2023-07-26 10:35:36.000000 datamarket-0.3.8/src/datamarket.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-07-26 10:35:36.000000 datamarket-0.3.8/src/datamarket.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 06:37:04.123386 datamarket-0.3.9/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35149 2021-10-07 14:37:41.000000 datamarket-0.3.9/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1486 2023-08-01 06:37:04.119386 datamarket-0.3.9/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      934 2023-05-25 14:26:25.000000 datamarket-0.3.9/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-08-01 06:37:04.123386 datamarket-0.3.9/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1066 2023-08-01 06:31:50.000000 datamarket-0.3.9/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 06:37:04.107386 datamarket-0.3.9/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 06:37:04.115386 datamarket-0.3.9/src/datamarket/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2021-11-03 08:15:04.000000 datamarket-0.3.9/src/datamarket/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 06:37:04.119386 datamarket-0.3.9/src/datamarket/interfaces/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-03 09:55:33.000000 datamarket-0.3.9/src/datamarket/interfaces/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3104 2023-02-16 08:03:41.000000 datamarket-0.3.9/src/datamarket/interfaces/alchemy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2022-08-08 10:00:49.000000 datamarket-0.3.9/src/datamarket/interfaces/drive.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1344 2023-02-17 11:31:46.000000 datamarket-0.3.9/src/datamarket/interfaces/ftp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2023-04-14 11:21:25.000000 datamarket-0.3.9/src/datamarket/interfaces/proxy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2565 2023-03-14 07:00:34.000000 datamarket-0.3.9/src/datamarket/interfaces/tinybird.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 06:37:04.119386 datamarket-0.3.9/src/datamarket/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-05-26 09:46:08.000000 datamarket-0.3.9/src/datamarket/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2017 2023-08-01 06:34:26.000000 datamarket-0.3.9/src/datamarket/utils/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2488 2023-07-26 10:34:42.000000 datamarket-0.3.9/src/datamarket/utils/selenium.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 06:37:04.115386 datamarket-0.3.9/src/datamarket.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1486 2023-08-01 06:37:04.000000 datamarket-0.3.9/src/datamarket.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      553 2023-08-01 06:37:04.000000 datamarket-0.3.9/src/datamarket.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-08-01 06:37:04.000000 datamarket-0.3.9/src/datamarket.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-08-01 06:37:04.000000 datamarket-0.3.9/src/datamarket.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-08-01 06:37:04.000000 datamarket-0.3.9/src/datamarket.egg-info/top_level.txt
```

### Comparing `datamarket-0.3.8/LICENSE` & `datamarket-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.8/PKG-INFO` & `datamarket-0.3.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.3.8
+Version: 0.3.9
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `datamarket-0.3.8/README.md` & `datamarket-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.8/setup.py` & `datamarket-0.3.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 requirements = [
     "sqlalchemy",
     "requests[socks]",
     "retry",
     "stem",
     "pydrive",
     "undetected_chromedriver",
+    "pendulum",
 ]
 
 setuptools.setup(
     name="datamarket",
-    version="0.3.8",
+    version="0.3.9",
     author="DataMarket",
     author_email="techsupport@datamarket.es",
     description="Utilities that integrate advance scraping knowledge into just one library.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Data-Market/datamarket",
     project_urls={
```

### Comparing `datamarket-0.3.8/src/datamarket/interfaces/alchemy.py` & `datamarket-0.3.9/src/datamarket/interfaces/alchemy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.8/src/datamarket/interfaces/drive.py` & `datamarket-0.3.9/src/datamarket/interfaces/drive.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.8/src/datamarket/interfaces/ftp.py` & `datamarket-0.3.9/src/datamarket/interfaces/ftp.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.8/src/datamarket/interfaces/proxy.py` & `datamarket-0.3.9/src/datamarket/interfaces/proxy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.8/src/datamarket/interfaces/tinybird.py` & `datamarket-0.3.9/src/datamarket/interfaces/tinybird.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.8/src/datamarket/utils/main.py` & `datamarket-0.3.9/src/datamarket/utils/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import logging
 import random
 import re
 import shlex
 import subprocess
 import time
 
+import pendulum
+
 ########################################################################################################################
 # FUNCTIONS
 
 logger = logging.getLogger(__name__)
 
 
 def get_config(config_path):
@@ -58,12 +60,20 @@
 
 
 def text_to_int(text):
     max_int32 = 2147483647
     try:
         num = int(re.sub(r"[^\d-]", "", text))
 
-        if -max_int32 < num < max_int32:  # max integer value (in order to avoid problems on database insertion)
+        if (
+            -max_int32 < num < max_int32
+        ):  # max integer value (in order to avoid problems on database insertion)
             return num
 
     except ValueError:
         logger.warning(f"unable to parse {text} as integer")
+
+
+def sleep_out_interval(from_h, to_h, tz="Europe/Madrid"):
+    while pendulum.now(tz=tz).hour >= to_h or pendulum.now(tz=tz).hour < from_h:
+        logger.warning("time to sleep and not scrape anything...")
+        ban_sleep(1800, 1800)
```

### Comparing `datamarket-0.3.8/src/datamarket/utils/selenium.py` & `datamarket-0.3.9/src/datamarket/utils/selenium.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.8/src/datamarket.egg-info/PKG-INFO` & `datamarket-0.3.9/src/datamarket.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.3.8
+Version: 0.3.9
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `datamarket-0.3.8/src/datamarket.egg-info/SOURCES.txt` & `datamarket-0.3.9/src/datamarket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

