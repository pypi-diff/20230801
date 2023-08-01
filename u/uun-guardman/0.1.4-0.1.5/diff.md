# Comparing `tmp/uun-guardman-0.1.4.tar.gz` & `tmp/uun-guardman-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uun-guardman-0.1.4.tar", last modified: Tue Aug  1 11:24:33 2023, max compression
+gzip compressed data, was "uun-guardman-0.1.5.tar", last modified: Tue Aug  1 14:54:36 2023, max compression
```

## Comparing `uun-guardman-0.1.4.tar` & `uun-guardman-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:24:33.257641 uun-guardman-0.1.4/
--rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:40:40.000000 uun-guardman-0.1.4/LICENSE.md
--rw-------   0 hello     (1000) hello     (1000)      386 2023-08-01 11:24:33.257641 uun-guardman-0.1.4/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)      392 2022-10-16 10:02:57.000000 uun-guardman-0.1.4/README.md
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:24:33.254307 uun-guardman-0.1.4/bin/
--rwx------   0 hello     (1000) hello     (1000)     3021 2023-08-01 11:17:43.000000 uun-guardman-0.1.4/bin/uun-guardman
--rwx------   0 hello     (1000) hello     (1000)      500 2022-10-16 10:02:57.000000 uun-guardman-0.1.4/bin/uun-guardman-install
--rwx------   0 hello     (1000) hello     (1000)     1891 2022-10-16 10:02:57.000000 uun-guardman-0.1.4/bin/uun-guardman-setup
--rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 11:24:33.257641 uun-guardman-0.1.4/setup.cfg
--rw-------   0 hello     (1000) hello     (1000)     1200 2023-08-01 11:19:00.000000 uun-guardman-0.1.4/setup.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:24:33.254307 uun-guardman-0.1.4/tests/
--rw-------   0 hello     (1000) hello     (1000)    10304 2022-10-16 10:02:57.000000 uun-guardman-0.1.4/tests/test_main.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:24:33.254307 uun-guardman-0.1.4/uun_guardman/
--rw-------   0 hello     (1000) hello     (1000)        0 2022-10-16 10:02:57.000000 uun-guardman-0.1.4/uun_guardman/__init__.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:24:33.257641 uun-guardman-0.1.4/uun_guardman/data/
--rw-------   0 hello     (1000) hello     (1000)     4005 2022-10-16 10:02:57.000000 uun-guardman-0.1.4/uun_guardman/data/sample-config.json
--rwx------   0 hello     (1000) hello     (1000)       64 2022-10-16 10:02:57.000000 uun-guardman-0.1.4/uun_guardman/data/start.sh
--rw-------   0 hello     (1000) hello     (1000)      300 2023-08-01 11:17:55.000000 uun-guardman-0.1.4/uun_guardman/data/systemd.service
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:24:33.257641 uun-guardman-0.1.4/uun_guardman/modules/
--rw-------   0 hello     (1000) hello     (1000)     8981 2022-10-16 10:02:57.000000 uun-guardman-0.1.4/uun_guardman/modules/GuardMan.py
--rw-------   0 hello     (1000) hello     (1000)      426 2022-10-16 10:02:57.000000 uun-guardman-0.1.4/uun_guardman/modules/__init__.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:24:33.257641 uun-guardman-0.1.4/uun_guardman.egg-info/
--rw-------   0 hello     (1000) hello     (1000)      386 2023-08-01 11:24:33.000000 uun-guardman-0.1.4/uun_guardman.egg-info/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)      481 2023-08-01 11:24:33.000000 uun-guardman-0.1.4/uun_guardman.egg-info/SOURCES.txt
--rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 11:24:33.000000 uun-guardman-0.1.4/uun_guardman.egg-info/dependency_links.txt
--rw-------   0 hello     (1000) hello     (1000)      130 2023-08-01 11:24:33.000000 uun-guardman-0.1.4/uun_guardman.egg-info/requires.txt
--rw-------   0 hello     (1000) hello     (1000)       13 2023-08-01 11:24:33.000000 uun-guardman-0.1.4/uun_guardman.egg-info/top_level.txt
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:54:36.678369 uun-guardman-0.1.5/
+-rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:40:40.000000 uun-guardman-0.1.5/LICENSE.md
+-rw-------   0 hello     (1000) hello     (1000)      386 2023-08-01 14:54:36.675036 uun-guardman-0.1.5/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)      392 2022-10-16 10:02:57.000000 uun-guardman-0.1.5/README.md
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:54:36.675036 uun-guardman-0.1.5/bin/
+-rwx------   0 hello     (1000) hello     (1000)     3021 2023-08-01 14:51:20.000000 uun-guardman-0.1.5/bin/uun-guardman
+-rwx------   0 hello     (1000) hello     (1000)      500 2022-10-16 10:02:57.000000 uun-guardman-0.1.5/bin/uun-guardman-install
+-rwx------   0 hello     (1000) hello     (1000)     1891 2022-10-16 10:02:57.000000 uun-guardman-0.1.5/bin/uun-guardman-setup
+-rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 14:54:36.678369 uun-guardman-0.1.5/setup.cfg
+-rw-------   0 hello     (1000) hello     (1000)     1198 2023-08-01 14:49:12.000000 uun-guardman-0.1.5/setup.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:54:36.675036 uun-guardman-0.1.5/tests/
+-rw-------   0 hello     (1000) hello     (1000)    10304 2022-10-16 10:02:57.000000 uun-guardman-0.1.5/tests/test_main.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:54:36.675036 uun-guardman-0.1.5/uun_guardman/
+-rw-------   0 hello     (1000) hello     (1000)        0 2022-10-16 10:02:57.000000 uun-guardman-0.1.5/uun_guardman/__init__.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:54:36.675036 uun-guardman-0.1.5/uun_guardman/data/
+-rw-------   0 hello     (1000) hello     (1000)     4005 2022-10-16 10:02:57.000000 uun-guardman-0.1.5/uun_guardman/data/sample-config.json
+-rwx------   0 hello     (1000) hello     (1000)       64 2022-10-16 10:02:57.000000 uun-guardman-0.1.5/uun_guardman/data/start.sh
+-rw-------   0 hello     (1000) hello     (1000)      300 2023-08-01 11:17:55.000000 uun-guardman-0.1.5/uun_guardman/data/systemd.service
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:54:36.675036 uun-guardman-0.1.5/uun_guardman/modules/
+-rw-------   0 hello     (1000) hello     (1000)     8981 2022-10-16 10:02:57.000000 uun-guardman-0.1.5/uun_guardman/modules/GuardMan.py
+-rw-------   0 hello     (1000) hello     (1000)      426 2022-10-16 10:02:57.000000 uun-guardman-0.1.5/uun_guardman/modules/__init__.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:54:36.675036 uun-guardman-0.1.5/uun_guardman.egg-info/
+-rw-------   0 hello     (1000) hello     (1000)      386 2023-08-01 14:54:36.000000 uun-guardman-0.1.5/uun_guardman.egg-info/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)      481 2023-08-01 14:54:36.000000 uun-guardman-0.1.5/uun_guardman.egg-info/SOURCES.txt
+-rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 14:54:36.000000 uun-guardman-0.1.5/uun_guardman.egg-info/dependency_links.txt
+-rw-------   0 hello     (1000) hello     (1000)      130 2023-08-01 14:54:36.000000 uun-guardman-0.1.5/uun_guardman.egg-info/requires.txt
+-rw-------   0 hello     (1000) hello     (1000)       13 2023-08-01 14:54:36.000000 uun-guardman-0.1.5/uun_guardman.egg-info/top_level.txt
```

### Comparing `uun-guardman-0.1.4/LICENSE.md` & `uun-guardman-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uun-guardman-0.1.4/bin/uun-guardman` & `uun-guardman-0.1.5/bin/uun-guardman`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys
 import time
 
 from uun_guardman.modules import init
 from uun_iot import Gateway
 from uun_iot.utils import LoggingSystemdHandler
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 __package__ = "uun_guardman"
 
 
 def main():
     argp = argparse.ArgumentParser(
         prog=__package__,
         description="Connect to uuConsole server application, get status codes of specified processes and display them using color-coding and blinkg on a LED strip.",
```

### Comparing `uun-guardman-0.1.4/bin/uun-guardman-setup` & `uun-guardman-0.1.5/bin/uun-guardman-setup`

 * *Files identical despite different names*

### Comparing `uun-guardman-0.1.4/setup.py` & `uun-guardman-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License"
     ],
     python_requires='>=3.6',
     install_requires=[
-        "uun-iot >= 0.9.1",
+        "uun-iot>=0.9.3",
         "uun-iot-libledstrip >= 0.2.4" 
     ],
     extras_require={
         # uun-iot-libledstrip >= 0.2
         "neopixel": [
             "uun-iot-libledstrip[neopixel] >= 0.2.4",
         ],
```

### Comparing `uun-guardman-0.1.4/tests/test_main.py` & `uun-guardman-0.1.5/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `uun-guardman-0.1.4/uun_guardman/data/sample-config.json` & `uun-guardman-0.1.5/uun_guardman/data/sample-config.json`

 * *Files identical despite different names*

### Comparing `uun-guardman-0.1.4/uun_guardman/modules/GuardMan.py` & `uun-guardman-0.1.5/uun_guardman/modules/GuardMan.py`

 * *Files identical despite different names*

