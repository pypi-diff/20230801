# Comparing `tmp/uun-windsurfguru-0.2.4.tar.gz` & `tmp/uun-windsurfguru-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uun-windsurfguru-0.2.4.tar", last modified: Tue Aug  1 11:28:46 2023, max compression
+gzip compressed data, was "uun-windsurfguru-0.2.5.tar", last modified: Tue Aug  1 14:54:52 2023, max compression
```

## Comparing `uun-windsurfguru-0.2.4.tar` & `uun-windsurfguru-0.2.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:46.731943 uun-windsurfguru-0.2.4/
--rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:44:55.000000 uun-windsurfguru-0.2.4/LICENSE.md
--rw-------   0 hello     (1000) hello     (1000)      541 2023-08-01 11:28:46.731943 uun-windsurfguru-0.2.4/PKG-INFO
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:46.728609 uun-windsurfguru-0.2.4/bin/
--rwx------   0 hello     (1000) hello     (1000)     2950 2023-08-01 11:12:29.000000 uun-windsurfguru-0.2.4/bin/uun-windsurfguru
--rwx------   0 hello     (1000) hello     (1000)      504 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.4/bin/uun-windsurfguru-install
--rwx------   0 hello     (1000) hello     (1000)     1920 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.4/bin/uun-windsurfguru-setup
--rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 11:28:46.731943 uun-windsurfguru-0.2.4/setup.cfg
--rw-------   0 hello     (1000) hello     (1000)     1391 2023-08-01 11:09:19.000000 uun-windsurfguru-0.2.4/setup.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:46.731943 uun-windsurfguru-0.2.4/tests/
--rw-------   0 hello     (1000) hello     (1000)     5545 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.4/tests/test_main.py
--rw-------   0 hello     (1000) hello     (1000)      167 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.4/tests/test_run.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:46.731943 uun-windsurfguru-0.2.4/uun_windsurfguru/
--rw-------   0 hello     (1000) hello     (1000)        0 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.4/uun_windsurfguru/__init__.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:46.731943 uun-windsurfguru-0.2.4/uun_windsurfguru/data/
--rw-------   0 hello     (1000) hello     (1000)     3830 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.4/uun_windsurfguru/data/sample-config.json
--rwx------   0 hello     (1000) hello     (1000)       68 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.4/uun_windsurfguru/data/start.sh
--rw-------   0 hello     (1000) hello     (1000)      304 2023-08-01 11:06:10.000000 uun-windsurfguru-0.2.4/uun_windsurfguru/data/systemd.service
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:46.731943 uun-windsurfguru-0.2.4/uun_windsurfguru/modules/
--rw-------   0 hello     (1000) hello     (1000)    24695 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.4/uun_windsurfguru/modules/WindSurfGuru.py
--rw-------   0 hello     (1000) hello     (1000)      408 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.4/uun_windsurfguru/modules/__init__.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:46.731943 uun-windsurfguru-0.2.4/uun_windsurfguru.egg-info/
--rw-------   0 hello     (1000) hello     (1000)      541 2023-08-01 11:28:46.000000 uun-windsurfguru-0.2.4/uun_windsurfguru.egg-info/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)      549 2023-08-01 11:28:46.000000 uun-windsurfguru-0.2.4/uun_windsurfguru.egg-info/SOURCES.txt
--rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 11:28:46.000000 uun-windsurfguru-0.2.4/uun_windsurfguru.egg-info/dependency_links.txt
--rw-------   0 hello     (1000) hello     (1000)      171 2023-08-01 11:28:46.000000 uun-windsurfguru-0.2.4/uun_windsurfguru.egg-info/requires.txt
--rw-------   0 hello     (1000) hello     (1000)       17 2023-08-01 11:28:46.000000 uun-windsurfguru-0.2.4/uun_windsurfguru.egg-info/top_level.txt
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:54:52.321706 uun-windsurfguru-0.2.5/
+-rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:44:55.000000 uun-windsurfguru-0.2.5/LICENSE.md
+-rw-------   0 hello     (1000) hello     (1000)      541 2023-08-01 14:54:52.321706 uun-windsurfguru-0.2.5/PKG-INFO
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:54:52.318373 uun-windsurfguru-0.2.5/bin/
+-rwx------   0 hello     (1000) hello     (1000)     2950 2023-08-01 14:53:26.000000 uun-windsurfguru-0.2.5/bin/uun-windsurfguru
+-rwx------   0 hello     (1000) hello     (1000)      504 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.5/bin/uun-windsurfguru-install
+-rwx------   0 hello     (1000) hello     (1000)     1920 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.5/bin/uun-windsurfguru-setup
+-rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 14:54:52.321706 uun-windsurfguru-0.2.5/setup.cfg
+-rw-------   0 hello     (1000) hello     (1000)     1389 2023-08-01 14:49:12.000000 uun-windsurfguru-0.2.5/setup.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:54:52.318373 uun-windsurfguru-0.2.5/tests/
+-rw-------   0 hello     (1000) hello     (1000)     5545 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.5/tests/test_main.py
+-rw-------   0 hello     (1000) hello     (1000)      167 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.5/tests/test_run.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:54:52.318373 uun-windsurfguru-0.2.5/uun_windsurfguru/
+-rw-------   0 hello     (1000) hello     (1000)        0 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.5/uun_windsurfguru/__init__.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:54:52.318373 uun-windsurfguru-0.2.5/uun_windsurfguru/data/
+-rw-------   0 hello     (1000) hello     (1000)     3830 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.5/uun_windsurfguru/data/sample-config.json
+-rwx------   0 hello     (1000) hello     (1000)       68 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.5/uun_windsurfguru/data/start.sh
+-rw-------   0 hello     (1000) hello     (1000)      304 2023-08-01 11:06:10.000000 uun-windsurfguru-0.2.5/uun_windsurfguru/data/systemd.service
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:54:52.321706 uun-windsurfguru-0.2.5/uun_windsurfguru/modules/
+-rw-------   0 hello     (1000) hello     (1000)    24695 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.5/uun_windsurfguru/modules/WindSurfGuru.py
+-rw-------   0 hello     (1000) hello     (1000)      408 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.5/uun_windsurfguru/modules/__init__.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:54:52.318373 uun-windsurfguru-0.2.5/uun_windsurfguru.egg-info/
+-rw-------   0 hello     (1000) hello     (1000)      541 2023-08-01 14:54:52.000000 uun-windsurfguru-0.2.5/uun_windsurfguru.egg-info/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)      549 2023-08-01 14:54:52.000000 uun-windsurfguru-0.2.5/uun_windsurfguru.egg-info/SOURCES.txt
+-rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 14:54:52.000000 uun-windsurfguru-0.2.5/uun_windsurfguru.egg-info/dependency_links.txt
+-rw-------   0 hello     (1000) hello     (1000)      171 2023-08-01 14:54:52.000000 uun-windsurfguru-0.2.5/uun_windsurfguru.egg-info/requires.txt
+-rw-------   0 hello     (1000) hello     (1000)       17 2023-08-01 14:54:52.000000 uun-windsurfguru-0.2.5/uun_windsurfguru.egg-info/top_level.txt
```

### Comparing `uun-windsurfguru-0.2.4/LICENSE.md` & `uun-windsurfguru-0.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uun-windsurfguru-0.2.4/PKG-INFO` & `uun-windsurfguru-0.2.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uun-windsurfguru
-Version: 0.2.4
+Version: 0.2.5
 Summary: Display wind surf conditions on a colorful LED strip.
 Home-page: https://uuapp.plus4u.net/uu-bookkit-maing01/c145b7fe6d754775b71e196b3fbb9a6a/book/page?code=64720442
 Author: (UUN) Tomáš Faikl & Marek Beránek
 Author-email: tomas.faikl@unicornuniversity.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `uun-windsurfguru-0.2.4/bin/uun-windsurfguru` & `uun-windsurfguru-0.2.5/bin/uun-windsurfguru`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import signal
 import sys
 
 from uun_iot import Gateway
 from uun_iot.utils import LoggingSystemdHandler
 from uun_windsurfguru.modules import init
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 __package__ = "uun_windsurfguru"
 
 
 def main():
     argp = argparse.ArgumentParser(
         prog=__package__,
         description="Display wind surf conditions on a colorful LED strip.",
```

### Comparing `uun-windsurfguru-0.2.4/bin/uun-windsurfguru-setup` & `uun-windsurfguru-0.2.5/bin/uun-windsurfguru-setup`

 * *Files identical despite different names*

### Comparing `uun-windsurfguru-0.2.4/setup.py` & `uun-windsurfguru-0.2.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License"
     ],
     python_requires='>=3.6',
     install_requires=[
-        "uun-iot >= 0.9.1",
+        "uun-iot>=0.9.3",
         "uun-iot-libledstrip >= 0.2.3"
     ],
     extras_require={
         "neopixel": [
             "uun-iot-libledstrip[neopixel] >= 0.2.3",
         ],
         "gpio": [
```

### Comparing `uun-windsurfguru-0.2.4/tests/test_main.py` & `uun-windsurfguru-0.2.5/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `uun-windsurfguru-0.2.4/uun_windsurfguru/data/sample-config.json` & `uun-windsurfguru-0.2.5/uun_windsurfguru/data/sample-config.json`

 * *Files identical despite different names*

### Comparing `uun-windsurfguru-0.2.4/uun_windsurfguru/modules/WindSurfGuru.py` & `uun-windsurfguru-0.2.5/uun_windsurfguru/modules/WindSurfGuru.py`

 * *Files identical despite different names*

### Comparing `uun-windsurfguru-0.2.4/uun_windsurfguru.egg-info/PKG-INFO` & `uun-windsurfguru-0.2.5/uun_windsurfguru.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uun-windsurfguru
-Version: 0.2.4
+Version: 0.2.5
 Summary: Display wind surf conditions on a colorful LED strip.
 Home-page: https://uuapp.plus4u.net/uu-bookkit-maing01/c145b7fe6d754775b71e196b3fbb9a6a/book/page?code=64720442
 Author: (UUN) Tomáš Faikl & Marek Beránek
 Author-email: tomas.faikl@unicornuniversity.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `uun-windsurfguru-0.2.4/uun_windsurfguru.egg-info/SOURCES.txt` & `uun-windsurfguru-0.2.5/uun_windsurfguru.egg-info/SOURCES.txt`

 * *Files identical despite different names*

