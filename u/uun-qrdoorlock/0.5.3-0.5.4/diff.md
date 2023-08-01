# Comparing `tmp/uun-qrdoorlock-0.5.3.tar.gz` & `tmp/uun-qrdoorlock-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uun-qrdoorlock-0.5.3.tar", last modified: Tue Aug  1 11:29:04 2023, max compression
+gzip compressed data, was "uun-qrdoorlock-0.5.4.tar", last modified: Tue Aug  1 14:55:09 2023, max compression
```

## Comparing `uun-qrdoorlock-0.5.3.tar` & `uun-qrdoorlock-0.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:29:04.268674 uun-qrdoorlock-0.5.3/
--rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:44:22.000000 uun-qrdoorlock-0.5.3/LICENSE.md
--rw-------   0 hello     (1000) hello     (1000)      453 2023-08-01 11:29:04.268674 uun-qrdoorlock-0.5.3/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)     3102 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.3/README.md
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:29:04.265340 uun-qrdoorlock-0.5.3/bin/
--rwx------   0 hello     (1000) hello     (1000)     2746 2023-08-01 10:49:28.000000 uun-qrdoorlock-0.5.3/bin/uun-qrdoorlock
--rwx------   0 hello     (1000) hello     (1000)      562 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.3/bin/uun-qrdoorlock-install
--rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 11:29:04.268674 uun-qrdoorlock-0.5.3/setup.cfg
--rw-------   0 hello     (1000) hello     (1000)     1189 2023-06-24 10:48:51.000000 uun-qrdoorlock-0.5.3/setup.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:29:04.265340 uun-qrdoorlock-0.5.3/tests/
--rw-------   0 hello     (1000) hello     (1000)     2286 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.3/tests/test_qr.py
--rw-------   0 hello     (1000) hello     (1000)     1067 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.3/tests/test_run.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:29:04.268674 uun-qrdoorlock-0.5.3/uun_qrdoorlock/
--rw-------   0 hello     (1000) hello     (1000)        0 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock/__init__.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:29:04.268674 uun-qrdoorlock-0.5.3/uun_qrdoorlock/data/
--rw-------   0 hello     (1000) hello     (1000)     1266 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock/data/sample-config.json
--rwx------   0 hello     (1000) hello     (1000)       56 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock/data/start.sh
--rw-------   0 hello     (1000) hello     (1000)      302 2023-08-01 10:49:46.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock/data/systemd.service
--rw-------   0 hello     (1000) hello     (1000)     6522 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock/hw.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:29:04.268674 uun-qrdoorlock-0.5.3/uun_qrdoorlock/modules/
--rw-------   0 hello     (1000) hello     (1000)     3689 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock/modules/DoorMonitor.py
--rw-------   0 hello     (1000) hello     (1000)     6884 2023-06-24 10:30:54.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock/modules/QrLock.py
--rw-------   0 hello     (1000) hello     (1000)     1363 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock/modules/__init__.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:29:04.268674 uun-qrdoorlock-0.5.3/uun_qrdoorlock.egg-info/
--rw-------   0 hello     (1000) hello     (1000)      453 2023-08-01 11:29:04.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock.egg-info/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)      557 2023-08-01 11:29:04.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock.egg-info/SOURCES.txt
--rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 11:29:04.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock.egg-info/dependency_links.txt
--rw-------   0 hello     (1000) hello     (1000)       52 2023-08-01 11:29:04.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock.egg-info/requires.txt
--rw-------   0 hello     (1000) hello     (1000)       15 2023-08-01 11:29:04.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock.egg-info/top_level.txt
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:55:09.421710 uun-qrdoorlock-0.5.4/
+-rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:44:22.000000 uun-qrdoorlock-0.5.4/LICENSE.md
+-rw-------   0 hello     (1000) hello     (1000)      453 2023-08-01 14:55:09.421710 uun-qrdoorlock-0.5.4/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)     3102 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.4/README.md
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:55:09.418377 uun-qrdoorlock-0.5.4/bin/
+-rwx------   0 hello     (1000) hello     (1000)     2746 2023-08-01 14:52:39.000000 uun-qrdoorlock-0.5.4/bin/uun-qrdoorlock
+-rwx------   0 hello     (1000) hello     (1000)      562 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.4/bin/uun-qrdoorlock-install
+-rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 14:55:09.421710 uun-qrdoorlock-0.5.4/setup.cfg
+-rw-------   0 hello     (1000) hello     (1000)     1187 2023-08-01 14:49:12.000000 uun-qrdoorlock-0.5.4/setup.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:55:09.418377 uun-qrdoorlock-0.5.4/tests/
+-rw-------   0 hello     (1000) hello     (1000)     2286 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.4/tests/test_qr.py
+-rw-------   0 hello     (1000) hello     (1000)     1067 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.4/tests/test_run.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:55:09.418377 uun-qrdoorlock-0.5.4/uun_qrdoorlock/
+-rw-------   0 hello     (1000) hello     (1000)        0 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.4/uun_qrdoorlock/__init__.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:55:09.421710 uun-qrdoorlock-0.5.4/uun_qrdoorlock/data/
+-rw-------   0 hello     (1000) hello     (1000)     1266 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.4/uun_qrdoorlock/data/sample-config.json
+-rwx------   0 hello     (1000) hello     (1000)       56 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.4/uun_qrdoorlock/data/start.sh
+-rw-------   0 hello     (1000) hello     (1000)      302 2023-08-01 10:49:46.000000 uun-qrdoorlock-0.5.4/uun_qrdoorlock/data/systemd.service
+-rw-------   0 hello     (1000) hello     (1000)     6522 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.4/uun_qrdoorlock/hw.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:55:09.421710 uun-qrdoorlock-0.5.4/uun_qrdoorlock/modules/
+-rw-------   0 hello     (1000) hello     (1000)     3689 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.4/uun_qrdoorlock/modules/DoorMonitor.py
+-rw-------   0 hello     (1000) hello     (1000)     6884 2023-06-24 10:30:54.000000 uun-qrdoorlock-0.5.4/uun_qrdoorlock/modules/QrLock.py
+-rw-------   0 hello     (1000) hello     (1000)     1363 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.4/uun_qrdoorlock/modules/__init__.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:55:09.421710 uun-qrdoorlock-0.5.4/uun_qrdoorlock.egg-info/
+-rw-------   0 hello     (1000) hello     (1000)      453 2023-08-01 14:55:09.000000 uun-qrdoorlock-0.5.4/uun_qrdoorlock.egg-info/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)      557 2023-08-01 14:55:09.000000 uun-qrdoorlock-0.5.4/uun_qrdoorlock.egg-info/SOURCES.txt
+-rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 14:55:09.000000 uun-qrdoorlock-0.5.4/uun_qrdoorlock.egg-info/dependency_links.txt
+-rw-------   0 hello     (1000) hello     (1000)       52 2023-08-01 14:55:09.000000 uun-qrdoorlock-0.5.4/uun_qrdoorlock.egg-info/requires.txt
+-rw-------   0 hello     (1000) hello     (1000)       15 2023-08-01 14:55:09.000000 uun-qrdoorlock-0.5.4/uun_qrdoorlock.egg-info/top_level.txt
```

### Comparing `uun-qrdoorlock-0.5.3/LICENSE.md` & `uun-qrdoorlock-0.5.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uun-qrdoorlock-0.5.3/README.md` & `uun-qrdoorlock-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `uun-qrdoorlock-0.5.3/bin/uun-qrdoorlock` & `uun-qrdoorlock-0.5.4/bin/uun-qrdoorlock`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import signal
 import sys
 
 from uun_iot.Gateway import Gateway
 from uun_iot.utils import LoggingSystemdHandler
 from uun_qrdoorlock.modules import init
 
-__version__ = "0.5.3"
+__version__ = "0.5.4"
 __package__ = "uun_qrdoorlock"
 library = "uun_iot"
 
 
 def main():
     argp = argparse.ArgumentParser(
         prog=__package__,
```

### Comparing `uun-qrdoorlock-0.5.3/bin/uun-qrdoorlock-install` & `uun-qrdoorlock-0.5.4/bin/uun-qrdoorlock-install`

 * *Files identical despite different names*

### Comparing `uun-qrdoorlock-0.5.3/setup.py` & `uun-qrdoorlock-0.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License"
     ],
     python_requires='>=3.6',
     install_requires=[
-        "uun-iot >= 0.9.0",
+        "uun-iot>=0.9.3",
         "pyserial",
         "pynacl",
         "validators",
         "termcolor"
     ],
     #extras_require = {
     #   "dev": [
```

### Comparing `uun-qrdoorlock-0.5.3/tests/test_qr.py` & `uun-qrdoorlock-0.5.4/tests/test_qr.py`

 * *Files identical despite different names*

### Comparing `uun-qrdoorlock-0.5.3/tests/test_run.py` & `uun-qrdoorlock-0.5.4/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `uun-qrdoorlock-0.5.3/uun_qrdoorlock/data/sample-config.json` & `uun-qrdoorlock-0.5.4/uun_qrdoorlock/data/sample-config.json`

 * *Files identical despite different names*

### Comparing `uun-qrdoorlock-0.5.3/uun_qrdoorlock/hw.py` & `uun-qrdoorlock-0.5.4/uun_qrdoorlock/hw.py`

 * *Files identical despite different names*

### Comparing `uun-qrdoorlock-0.5.3/uun_qrdoorlock/modules/DoorMonitor.py` & `uun-qrdoorlock-0.5.4/uun_qrdoorlock/modules/DoorMonitor.py`

 * *Files identical despite different names*

### Comparing `uun-qrdoorlock-0.5.3/uun_qrdoorlock/modules/QrLock.py` & `uun-qrdoorlock-0.5.4/uun_qrdoorlock/modules/QrLock.py`

 * *Files identical despite different names*

### Comparing `uun-qrdoorlock-0.5.3/uun_qrdoorlock/modules/__init__.py` & `uun-qrdoorlock-0.5.4/uun_qrdoorlock/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `uun-qrdoorlock-0.5.3/uun_qrdoorlock.egg-info/SOURCES.txt` & `uun-qrdoorlock-0.5.4/uun_qrdoorlock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

