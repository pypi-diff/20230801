# Comparing `tmp/uun-weatherstation-0.6.5.tar.gz` & `tmp/uun-weatherstation-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uun-weatherstation-0.6.5.tar", last modified: Tue Aug  1 11:28:19 2023, max compression
+gzip compressed data, was "uun-weatherstation-0.6.6.tar", last modified: Tue Aug  1 14:54:20 2023, max compression
```

## Comparing `uun-weatherstation-0.6.5.tar` & `uun-weatherstation-0.6.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:19.695177 uun-weatherstation-0.6.5/
--rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:44:43.000000 uun-weatherstation-0.6.5/LICENSE.md
--rw-------   0 hello     (1000) hello     (1000)      466 2023-08-01 11:28:19.695177 uun-weatherstation-0.6.5/PKG-INFO
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:19.691843 uun-weatherstation-0.6.5/bin/
--rwx------   0 hello     (1000) hello     (1000)     2717 2023-08-01 10:46:25.000000 uun-weatherstation-0.6.5/bin/uun-weatherstation
--rwx------   0 hello     (1000) hello     (1000)      505 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.5/bin/uun-weatherstation-install
--rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 11:28:19.695177 uun-weatherstation-0.6.5/setup.cfg
--rw-------   0 hello     (1000) hello     (1000)     1065 2023-08-01 10:11:04.000000 uun-weatherstation-0.6.5/setup.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:19.691843 uun-weatherstation-0.6.5/tests/
--rw-------   0 hello     (1000) hello     (1000)     5995 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.5/tests/test_data_processing.py
--rw-------   0 hello     (1000) hello     (1000)      139 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.5/tests/test_run_5s.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:19.691843 uun-weatherstation-0.6.5/uun_weatherstation/
--rw-------   0 hello     (1000) hello     (1000)        1 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.5/uun_weatherstation/__init__.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:19.695177 uun-weatherstation-0.6.5/uun_weatherstation/data/
--rw-------   0 hello     (1000) hello     (1000)     1657 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.5/uun_weatherstation/data/sample-config.json
--rwx------   0 hello     (1000) hello     (1000)       70 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.5/uun_weatherstation/data/start.sh
--rw-------   0 hello     (1000) hello     (1000)      305 2023-08-01 10:42:32.000000 uun-weatherstation-0.6.5/uun_weatherstation/data/systemd.service
--rw-------   0 hello     (1000) hello     (1000)      194 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.5/uun_weatherstation/diagnostic.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:19.695177 uun-weatherstation-0.6.5/uun_weatherstation/modules/
--rw-------   0 hello     (1000) hello     (1000)      416 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.5/uun_weatherstation/modules/HealthCheck.py
--rw-------   0 hello     (1000) hello     (1000)     8536 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.5/uun_weatherstation/modules/WeatherConditions.py
--rw-------   0 hello     (1000) hello     (1000)     2555 2023-08-01 07:46:32.000000 uun-weatherstation-0.6.5/uun_weatherstation/modules/__init__.py
--rw-------   0 hello     (1000) hello     (1000)      326 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.5/uun_weatherstation/utils.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:19.695177 uun-weatherstation-0.6.5/uun_weatherstation.egg-info/
--rw-------   0 hello     (1000) hello     (1000)      466 2023-08-01 11:28:19.000000 uun-weatherstation-0.6.5/uun_weatherstation.egg-info/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)      670 2023-08-01 11:28:19.000000 uun-weatherstation-0.6.5/uun_weatherstation.egg-info/SOURCES.txt
--rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 11:28:19.000000 uun-weatherstation-0.6.5/uun_weatherstation.egg-info/dependency_links.txt
--rw-------   0 hello     (1000) hello     (1000)       32 2023-08-01 11:28:19.000000 uun-weatherstation-0.6.5/uun_weatherstation.egg-info/requires.txt
--rw-------   0 hello     (1000) hello     (1000)       19 2023-08-01 11:28:19.000000 uun-weatherstation-0.6.5/uun_weatherstation.egg-info/top_level.txt
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:54:20.911700 uun-weatherstation-0.6.6/
+-rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:44:43.000000 uun-weatherstation-0.6.6/LICENSE.md
+-rw-------   0 hello     (1000) hello     (1000)      466 2023-08-01 14:54:20.911700 uun-weatherstation-0.6.6/PKG-INFO
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:54:20.911700 uun-weatherstation-0.6.6/bin/
+-rwx------   0 hello     (1000) hello     (1000)     2717 2023-08-01 14:53:02.000000 uun-weatherstation-0.6.6/bin/uun-weatherstation
+-rwx------   0 hello     (1000) hello     (1000)      505 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.6/bin/uun-weatherstation-install
+-rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 14:54:20.911700 uun-weatherstation-0.6.6/setup.cfg
+-rw-------   0 hello     (1000) hello     (1000)     1063 2023-08-01 14:49:12.000000 uun-weatherstation-0.6.6/setup.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:54:20.911700 uun-weatherstation-0.6.6/tests/
+-rw-------   0 hello     (1000) hello     (1000)     5995 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.6/tests/test_data_processing.py
+-rw-------   0 hello     (1000) hello     (1000)      139 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.6/tests/test_run_5s.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:54:20.911700 uun-weatherstation-0.6.6/uun_weatherstation/
+-rw-------   0 hello     (1000) hello     (1000)        1 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.6/uun_weatherstation/__init__.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:54:20.911700 uun-weatherstation-0.6.6/uun_weatherstation/data/
+-rw-------   0 hello     (1000) hello     (1000)     1657 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.6/uun_weatherstation/data/sample-config.json
+-rwx------   0 hello     (1000) hello     (1000)       70 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.6/uun_weatherstation/data/start.sh
+-rw-------   0 hello     (1000) hello     (1000)      305 2023-08-01 10:42:32.000000 uun-weatherstation-0.6.6/uun_weatherstation/data/systemd.service
+-rw-------   0 hello     (1000) hello     (1000)      194 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.6/uun_weatherstation/diagnostic.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:54:20.911700 uun-weatherstation-0.6.6/uun_weatherstation/modules/
+-rw-------   0 hello     (1000) hello     (1000)      416 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.6/uun_weatherstation/modules/HealthCheck.py
+-rw-------   0 hello     (1000) hello     (1000)     8536 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.6/uun_weatherstation/modules/WeatherConditions.py
+-rw-------   0 hello     (1000) hello     (1000)     2555 2023-08-01 07:46:32.000000 uun-weatherstation-0.6.6/uun_weatherstation/modules/__init__.py
+-rw-------   0 hello     (1000) hello     (1000)      326 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.6/uun_weatherstation/utils.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:54:20.911700 uun-weatherstation-0.6.6/uun_weatherstation.egg-info/
+-rw-------   0 hello     (1000) hello     (1000)      466 2023-08-01 14:54:20.000000 uun-weatherstation-0.6.6/uun_weatherstation.egg-info/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)      670 2023-08-01 14:54:20.000000 uun-weatherstation-0.6.6/uun_weatherstation.egg-info/SOURCES.txt
+-rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 14:54:20.000000 uun-weatherstation-0.6.6/uun_weatherstation.egg-info/dependency_links.txt
+-rw-------   0 hello     (1000) hello     (1000)       32 2023-08-01 14:54:20.000000 uun-weatherstation-0.6.6/uun_weatherstation.egg-info/requires.txt
+-rw-------   0 hello     (1000) hello     (1000)       19 2023-08-01 14:54:20.000000 uun-weatherstation-0.6.6/uun_weatherstation.egg-info/top_level.txt
```

### Comparing `uun-weatherstation-0.6.5/LICENSE.md` & `uun-weatherstation-0.6.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uun-weatherstation-0.6.5/bin/uun-weatherstation` & `uun-weatherstation-0.6.6/bin/uun-weatherstation`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import signal
 import sys
 
 from uun_iot.Gateway import Gateway
 from uun_iot.utils import LoggingSystemdHandler
 from uun_weatherstation.modules import init
 
-__version__ = "0.6.5"
+__version__ = "0.6.6"
 __package__ = "uun_weatherstation"
 library = "uun_iot"
 
 
 def main():
     argp = argparse.ArgumentParser(
         prog=__package__,
```

### Comparing `uun-weatherstation-0.6.5/setup.py` & `uun-weatherstation-0.6.6/setup.py`

 * *Files 2% similar despite different names*

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
         "requests>=2.24.0"
     ],
     scripts=[
         "bin/" + name,
         "bin/" + name + "-install"
     ],
     package_data={
```

### Comparing `uun-weatherstation-0.6.5/tests/test_data_processing.py` & `uun-weatherstation-0.6.6/tests/test_data_processing.py`

 * *Files identical despite different names*

### Comparing `uun-weatherstation-0.6.5/uun_weatherstation/data/sample-config.json` & `uun-weatherstation-0.6.6/uun_weatherstation/data/sample-config.json`

 * *Files identical despite different names*

### Comparing `uun-weatherstation-0.6.5/uun_weatherstation/modules/WeatherConditions.py` & `uun-weatherstation-0.6.6/uun_weatherstation/modules/WeatherConditions.py`

 * *Files identical despite different names*

### Comparing `uun-weatherstation-0.6.5/uun_weatherstation/modules/__init__.py` & `uun-weatherstation-0.6.6/uun_weatherstation/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `uun-weatherstation-0.6.5/uun_weatherstation.egg-info/SOURCES.txt` & `uun-weatherstation-0.6.6/uun_weatherstation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

