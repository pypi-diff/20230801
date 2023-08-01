# Comparing `tmp/uun-iot-libledstrip-0.2.3.tar.gz` & `tmp/uun-iot-libledstrip-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uun-iot-libledstrip-0.2.3.tar", last modified: Thu Jan 26 11:24:53 2023, max compression
+gzip compressed data, was "uun-iot-libledstrip-0.2.4.tar", last modified: Tue Aug  1 11:29:18 2023, max compression
```

## Comparing `uun-iot-libledstrip-0.2.3.tar` & `uun-iot-libledstrip-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:24:53.908441 uun-iot-libledstrip-0.2.3/
--rw-------   0 hello     (1000) hello     (1000)     1075 2022-10-16 10:02:57.000000 uun-iot-libledstrip-0.2.3/LICENSE.md
--rw-------   0 hello     (1000) hello     (1000)      451 2023-01-26 11:24:53.908441 uun-iot-libledstrip-0.2.3/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)       38 2023-01-26 11:24:53.908441 uun-iot-libledstrip-0.2.3/setup.cfg
--rw-------   0 hello     (1000) hello     (1000)     1000 2023-01-22 14:50:38.000000 uun-iot-libledstrip-0.2.3/setup.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:24:53.905108 uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/
--rw-------   0 hello     (1000) hello     (1000)    12902 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/LedStrip.py
--rw-------   0 hello     (1000) hello     (1000)     9223 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/MeterStrip.py
--rw-------   0 hello     (1000) hello     (1000)      847 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/__init__.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:24:53.905108 uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/data/
--rw-------   0 hello     (1000) hello     (1000)     2956 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/data/sample_config.json
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:24:53.908441 uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/devices/
--rw-------   0 hello     (1000) hello     (1000)     2076 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/devices/DebugLedDev.py
--rw-------   0 hello     (1000) hello     (1000)     1917 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/devices/GPIODev.py
--rw-------   0 hello     (1000) hello     (1000)    10046 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/devices/I2CPixelDev.py
--rw-------   0 hello     (1000) hello     (1000)     1072 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/devices/LedDev.py
--rw-------   0 hello     (1000) hello     (1000)      672 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/devices/NeopixelDev.py
--rw-------   0 hello     (1000) hello     (1000)      237 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/devices/__init__.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:24:53.905108 uun-iot-libledstrip-0.2.3/uun_iot_libledstrip.egg-info/
--rw-------   0 hello     (1000) hello     (1000)      451 2023-01-26 11:24:53.000000 uun-iot-libledstrip-0.2.3/uun_iot_libledstrip.egg-info/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)      621 2023-01-26 11:24:53.000000 uun-iot-libledstrip-0.2.3/uun_iot_libledstrip.egg-info/SOURCES.txt
--rw-------   0 hello     (1000) hello     (1000)        1 2023-01-26 11:24:53.000000 uun-iot-libledstrip-0.2.3/uun_iot_libledstrip.egg-info/dependency_links.txt
--rw-------   0 hello     (1000) hello     (1000)      117 2023-01-26 11:24:53.000000 uun-iot-libledstrip-0.2.3/uun_iot_libledstrip.egg-info/requires.txt
--rw-------   0 hello     (1000) hello     (1000)       20 2023-01-26 11:24:53.000000 uun-iot-libledstrip-0.2.3/uun_iot_libledstrip.egg-info/top_level.txt
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:29:18.542059 uun-iot-libledstrip-0.2.4/
+-rw-------   0 hello     (1000) hello     (1000)     1075 2022-10-16 10:02:57.000000 uun-iot-libledstrip-0.2.4/LICENSE.md
+-rw-------   0 hello     (1000) hello     (1000)      451 2023-08-01 11:29:18.542059 uun-iot-libledstrip-0.2.4/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 11:29:18.542059 uun-iot-libledstrip-0.2.4/setup.cfg
+-rw-------   0 hello     (1000) hello     (1000)     1069 2023-06-24 10:45:48.000000 uun-iot-libledstrip-0.2.4/setup.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:29:18.538725 uun-iot-libledstrip-0.2.4/tests/
+-rw-------   0 hello     (1000) hello     (1000)     1531 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.4/tests/test_meter.py
+-rw-------   0 hello     (1000) hello     (1000)     2629 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.4/tests/test_strip_bundle.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:29:18.538725 uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/
+-rw-------   0 hello     (1000) hello     (1000)    12902 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/LedStrip.py
+-rw-------   0 hello     (1000) hello     (1000)     9223 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/MeterStrip.py
+-rw-------   0 hello     (1000) hello     (1000)      847 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/__init__.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:29:18.538725 uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/data/
+-rw-------   0 hello     (1000) hello     (1000)     2956 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/data/sample_config.json
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:29:18.542059 uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/devices/
+-rw-------   0 hello     (1000) hello     (1000)     2076 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/devices/DebugLedDev.py
+-rw-------   0 hello     (1000) hello     (1000)     1917 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/devices/GPIODev.py
+-rw-------   0 hello     (1000) hello     (1000)    10046 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/devices/I2CPixelDev.py
+-rw-------   0 hello     (1000) hello     (1000)     1072 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/devices/LedDev.py
+-rw-------   0 hello     (1000) hello     (1000)      672 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/devices/NeopixelDev.py
+-rw-------   0 hello     (1000) hello     (1000)      237 2022-10-16 10:02:58.000000 uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/devices/__init__.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:29:18.538725 uun-iot-libledstrip-0.2.4/uun_iot_libledstrip.egg-info/
+-rw-------   0 hello     (1000) hello     (1000)      451 2023-08-01 11:29:18.000000 uun-iot-libledstrip-0.2.4/uun_iot_libledstrip.egg-info/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)      668 2023-08-01 11:29:18.000000 uun-iot-libledstrip-0.2.4/uun_iot_libledstrip.egg-info/SOURCES.txt
+-rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 11:29:18.000000 uun-iot-libledstrip-0.2.4/uun_iot_libledstrip.egg-info/dependency_links.txt
+-rw-------   0 hello     (1000) hello     (1000)      124 2023-08-01 11:29:18.000000 uun-iot-libledstrip-0.2.4/uun_iot_libledstrip.egg-info/requires.txt
+-rw-------   0 hello     (1000) hello     (1000)       20 2023-08-01 11:29:18.000000 uun-iot-libledstrip-0.2.4/uun_iot_libledstrip.egg-info/top_level.txt
```

### Comparing `uun-iot-libledstrip-0.2.3/LICENSE.md` & `uun-iot-libledstrip-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uun-iot-libledstrip-0.2.3/setup.py` & `uun-iot-libledstrip-0.2.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import shutil
 import os
 import re
 
-version = "0.2.3"
+version = "0.2.4"
 name = "uun-iot-libledstrip"
 name_=name.replace('-', '_')
 
 setuptools.setup(
     name=name,
     version=version,
     author="(UUN) Tomáš Faikl",
@@ -33,14 +33,15 @@
         "gpio": [
             "RPi.GPIO"
         ],
         "i2c": [
             "smbus2"
         ],
         "dev": [
-            "colored",
+            # deprecated rounding of colors in newer versions
+            "colored==1.4.4",
         ]
     },
     package_data={
         name_: ["data/*"]
     }
 )
```

### Comparing `uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/LedStrip.py` & `uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/LedStrip.py`

 * *Files identical despite different names*

### Comparing `uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/MeterStrip.py` & `uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/MeterStrip.py`

 * *Files identical despite different names*

### Comparing `uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/__init__.py` & `uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/__init__.py`

 * *Files identical despite different names*

### Comparing `uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/data/sample_config.json` & `uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/data/sample_config.json`

 * *Files identical despite different names*

### Comparing `uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/devices/DebugLedDev.py` & `uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/devices/DebugLedDev.py`

 * *Files identical despite different names*

### Comparing `uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/devices/GPIODev.py` & `uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/devices/GPIODev.py`

 * *Files identical despite different names*

### Comparing `uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/devices/I2CPixelDev.py` & `uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/devices/I2CPixelDev.py`

 * *Files identical despite different names*

### Comparing `uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/devices/LedDev.py` & `uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/devices/LedDev.py`

 * *Files identical despite different names*

### Comparing `uun-iot-libledstrip-0.2.3/uun_iot_libledstrip/devices/NeopixelDev.py` & `uun-iot-libledstrip-0.2.4/uun_iot_libledstrip/devices/NeopixelDev.py`

 * *Files identical despite different names*

### Comparing `uun-iot-libledstrip-0.2.3/uun_iot_libledstrip.egg-info/SOURCES.txt` & `uun-iot-libledstrip-0.2.4/uun_iot_libledstrip.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 LICENSE.md
 setup.py
+tests/test_meter.py
+tests/test_strip_bundle.py
 uun_iot_libledstrip/LedStrip.py
 uun_iot_libledstrip/MeterStrip.py
 uun_iot_libledstrip/__init__.py
 uun_iot_libledstrip.egg-info/PKG-INFO
 uun_iot_libledstrip.egg-info/SOURCES.txt
 uun_iot_libledstrip.egg-info/dependency_links.txt
 uun_iot_libledstrip.egg-info/requires.txt
```

