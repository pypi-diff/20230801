# Comparing `tmp/uun-weatherstation-0.6.2.tar.gz` & `tmp/uun-weatherstation-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uun-weatherstation-0.6.2.tar", last modified: Sun Jun 11 19:52:55 2023, max compression
+gzip compressed data, was "uun-weatherstation-0.6.4.tar", last modified: Tue Aug  1 10:13:10 2023, max compression
```

## Comparing `uun-weatherstation-0.6.2.tar` & `uun-weatherstation-0.6.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwx------   0 hello     (1000) hello     (1000)        0 2023-06-11 19:52:55.088652 uun-weatherstation-0.6.2/
--rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:44:43.000000 uun-weatherstation-0.6.2/LICENSE.md
--rw-------   0 hello     (1000) hello     (1000)      466 2023-06-11 19:52:55.088652 uun-weatherstation-0.6.2/PKG-INFO
-drwx------   0 hello     (1000) hello     (1000)        0 2023-06-11 19:52:55.085318 uun-weatherstation-0.6.2/bin/
--rwx------   0 hello     (1000) hello     (1000)     2332 2023-06-11 19:49:30.000000 uun-weatherstation-0.6.2/bin/uun-weatherstation
--rwx------   0 hello     (1000) hello     (1000)      505 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/bin/uun-weatherstation-install
--rw-------   0 hello     (1000) hello     (1000)       38 2023-06-11 19:52:55.088652 uun-weatherstation-0.6.2/setup.cfg
--rw-------   0 hello     (1000) hello     (1000)     1065 2023-01-26 11:51:01.000000 uun-weatherstation-0.6.2/setup.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-06-11 19:52:55.085318 uun-weatherstation-0.6.2/tests/
--rw-------   0 hello     (1000) hello     (1000)     5995 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/tests/test_data_processing.py
--rw-------   0 hello     (1000) hello     (1000)      139 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/tests/test_run_5s.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-06-11 19:52:55.085318 uun-weatherstation-0.6.2/uun_weatherstation/
--rw-------   0 hello     (1000) hello     (1000)        1 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/uun_weatherstation/__init__.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-06-11 19:52:55.088652 uun-weatherstation-0.6.2/uun_weatherstation/data/
--rw-------   0 hello     (1000) hello     (1000)     1657 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/uun_weatherstation/data/sample-config.json
--rwx------   0 hello     (1000) hello     (1000)       70 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/uun_weatherstation/data/start.sh
--rw-------   0 hello     (1000) hello     (1000)      292 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/uun_weatherstation/data/systemd.service
--rw-------   0 hello     (1000) hello     (1000)      194 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/uun_weatherstation/diagnostic.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-06-11 19:52:55.088652 uun-weatherstation-0.6.2/uun_weatherstation/modules/
--rw-------   0 hello     (1000) hello     (1000)      416 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/uun_weatherstation/modules/HealthCheck.py
--rw-------   0 hello     (1000) hello     (1000)     8536 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/uun_weatherstation/modules/WeatherConditions.py
--rw-------   0 hello     (1000) hello     (1000)     2639 2023-06-11 19:34:00.000000 uun-weatherstation-0.6.2/uun_weatherstation/modules/__init__.py
--rw-------   0 hello     (1000) hello     (1000)      326 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.2/uun_weatherstation/utils.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-06-11 19:52:55.088652 uun-weatherstation-0.6.2/uun_weatherstation.egg-info/
--rw-------   0 hello     (1000) hello     (1000)      466 2023-06-11 19:52:55.000000 uun-weatherstation-0.6.2/uun_weatherstation.egg-info/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)      670 2023-06-11 19:52:55.000000 uun-weatherstation-0.6.2/uun_weatherstation.egg-info/SOURCES.txt
--rw-------   0 hello     (1000) hello     (1000)        1 2023-06-11 19:52:55.000000 uun-weatherstation-0.6.2/uun_weatherstation.egg-info/dependency_links.txt
--rw-------   0 hello     (1000) hello     (1000)       32 2023-06-11 19:52:55.000000 uun-weatherstation-0.6.2/uun_weatherstation.egg-info/requires.txt
--rw-------   0 hello     (1000) hello     (1000)       19 2023-06-11 19:52:55.000000 uun-weatherstation-0.6.2/uun_weatherstation.egg-info/top_level.txt
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:13:10.380829 uun-weatherstation-0.6.4/
+-rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:44:43.000000 uun-weatherstation-0.6.4/LICENSE.md
+-rw-------   0 hello     (1000) hello     (1000)      466 2023-08-01 10:13:10.380829 uun-weatherstation-0.6.4/PKG-INFO
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:13:10.380829 uun-weatherstation-0.6.4/bin/
+-rwx------   0 hello     (1000) hello     (1000)     2499 2023-08-01 10:06:59.000000 uun-weatherstation-0.6.4/bin/uun-weatherstation
+-rwx------   0 hello     (1000) hello     (1000)      505 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/bin/uun-weatherstation-install
+-rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 10:13:10.380829 uun-weatherstation-0.6.4/setup.cfg
+-rw-------   0 hello     (1000) hello     (1000)     1065 2023-08-01 10:11:04.000000 uun-weatherstation-0.6.4/setup.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:13:10.380829 uun-weatherstation-0.6.4/tests/
+-rw-------   0 hello     (1000) hello     (1000)     5995 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/tests/test_data_processing.py
+-rw-------   0 hello     (1000) hello     (1000)      139 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/tests/test_run_5s.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:13:10.380829 uun-weatherstation-0.6.4/uun_weatherstation/
+-rw-------   0 hello     (1000) hello     (1000)        1 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/uun_weatherstation/__init__.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:13:10.380829 uun-weatherstation-0.6.4/uun_weatherstation/data/
+-rw-------   0 hello     (1000) hello     (1000)     1657 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/uun_weatherstation/data/sample-config.json
+-rwx------   0 hello     (1000) hello     (1000)       70 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/uun_weatherstation/data/start.sh
+-rw-------   0 hello     (1000) hello     (1000)      292 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/uun_weatherstation/data/systemd.service
+-rw-------   0 hello     (1000) hello     (1000)      194 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/uun_weatherstation/diagnostic.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:13:10.380829 uun-weatherstation-0.6.4/uun_weatherstation/modules/
+-rw-------   0 hello     (1000) hello     (1000)      416 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/uun_weatherstation/modules/HealthCheck.py
+-rw-------   0 hello     (1000) hello     (1000)     8536 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/uun_weatherstation/modules/WeatherConditions.py
+-rw-------   0 hello     (1000) hello     (1000)     2555 2023-08-01 07:46:32.000000 uun-weatherstation-0.6.4/uun_weatherstation/modules/__init__.py
+-rw-------   0 hello     (1000) hello     (1000)      326 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/uun_weatherstation/utils.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:13:10.380829 uun-weatherstation-0.6.4/uun_weatherstation.egg-info/
+-rw-------   0 hello     (1000) hello     (1000)      466 2023-08-01 10:13:10.000000 uun-weatherstation-0.6.4/uun_weatherstation.egg-info/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)      670 2023-08-01 10:13:10.000000 uun-weatherstation-0.6.4/uun_weatherstation.egg-info/SOURCES.txt
+-rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 10:13:10.000000 uun-weatherstation-0.6.4/uun_weatherstation.egg-info/dependency_links.txt
+-rw-------   0 hello     (1000) hello     (1000)       32 2023-08-01 10:13:10.000000 uun-weatherstation-0.6.4/uun_weatherstation.egg-info/requires.txt
+-rw-------   0 hello     (1000) hello     (1000)       19 2023-08-01 10:13:10.000000 uun-weatherstation-0.6.4/uun_weatherstation.egg-info/top_level.txt
```

### Comparing `uun-weatherstation-0.6.2/LICENSE.md` & `uun-weatherstation-0.6.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uun-weatherstation-0.6.2/bin/uun-weatherstation` & `uun-weatherstation-0.6.4/bin/uun-weatherstation`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,66 @@
 #!/usr/bin/env python3
-from uun_iot.Gateway import Gateway
-from uun_weatherstation.modules import init
 
-import logging
-import time
 import argparse
-import sys
+import logging
+import os
 import signal
+import sys
 
-__version__ = "0.6.2"
+from uun_iot.Gateway import Gateway
+from uun_iot.utils import LoggingSystemdHandler
+from uun_weatherstation.modules import init
+
+__version__ = "0.6.4"
 __package__ = "uun_weatherstation"
 library = "uun_iot"
 
+
 def main():
-    argp = argparse.ArgumentParser(prog=__package__, description='Connect to weatherlink weatherstation and process informations and send to server.')
-    argp.add_argument('-v', '--version', action='version', version='%(prog) ' + __version__)
-    argp.add_argument('-l', '--log', metavar='loglevel', dest='loglevel', type=str, help='level of logging: [DEBUG, INFO, WARNING, ERROR, CRITICAL]', default='WARNING')
+    argp = argparse.ArgumentParser(prog=__package__, description='Connect to weatherlink'
+                                   'weatherstation and process informations and send to server.')
+    argp.add_argument('-v', '--version', action='version',
+                      version='%(prog) ' + __version__)
+    argp.add_argument('-l', '--log', metavar='loglevel', dest='loglevel', type=str,
+                      help='level of logging: [DEBUG, INFO, WARNING, ERROR, CRITICAL]', default='WARNING')
+    argp.add_argument('-c', '--config', metavar='configfile', dest='config', type=str,
+                      help="config file location, defaults to 'config.json'", default='config.json')
+
+    sys.excepthook = lambda exctype, value, tb: logging.getLogger(__package__).exception(
+        "Exception: ", exc_info=(exctype, value, tb))
+
     args = argp.parse_args()
- 
-    ## = SETTING LOGGING = ##
-    # set log level from option
+
+    if not os.path.exists(args.config):
+        sys.exit(f"Could not find configuration file '{args.config}'")
+
     loglevel = args.loglevel
     llevel = getattr(logging, loglevel.upper(), None)
     if not isinstance(llevel, int):
-        raise ValueError('Invalid log level: %s' % loglevel)
+        sys.exit(f"Invalid log level: {loglevel}")
 
-    # set formatting and levels for this package and library (uuniot)
-    loggerw = logging.getLogger(__package__) # application specific logger
+    loggerw = logging.getLogger(__package__)  # application specific logger
+    loggeru = logging.getLogger(library)  # library logger
     loggerw.setLevel(llevel)
-    loggeru = logging.getLogger(library) # library logger
     loggeru.setLevel(llevel)
-    
-    # console handler (output text to console), here can be added file handlers, server handlers, ...
-    ch = logging.StreamHandler()
-    ch.setLevel(llevel)
-    # set log format
-    formatter = logging.Formatter('%(name)s - %(levelname)s - %(message)s')
-    # formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-
-    ch.setFormatter(formatter)
-
-    # asssign the same handler to loggers
-    loggerw.addHandler(ch)
-    loggeru.addHandler(ch)
+    handler = LoggingSystemdHandler()  # StreamHandler()
+    handler.setFormatter(logging.Formatter(
+        '%(name)s - %(levelname)s - %(message)s'))
+    loggerw.addHandler(handler)
+    loggeru.addHandler(handler)
 
     # start module system
     print("=== " + __package__ + " ===")
-    with Gateway('config.json', init) as g:
+    with Gateway(args.config, init) as g:
         # Register a SIGTERM signal, as it is issued by systemd on stop/restart.
         #   Because by default, it does not run destructors.
         # Ctrl-C (SINGINT) correctly runs destructors, so no need to register.
         # SIGUSR1 is used internally by HealthCheck to restart the gateway
         signal.signal(signal.SIGTERM, g.signal_handler)
         signal.signal(signal.SIGINT, g.signal_handler)
         signal.signal(signal.SIGUSR1, g.signal_handler)
 
         g.stopev.wait()
 
+
 if __name__ == '__main__':
     main()
```

### Comparing `uun-weatherstation-0.6.2/setup.py` & `uun-weatherstation-0.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License"
     ],
     python_requires='>=3.6',
     install_requires=[
-        "uun-iot >= 0.7.3",
+        "uun-iot >= 0.9.1",
         "requests>=2.24.0"
     ],
     scripts=[
         "bin/" + name,
         "bin/" + name + "-install"
     ],
     package_data={
```

### Comparing `uun-weatherstation-0.6.2/tests/test_data_processing.py` & `uun-weatherstation-0.6.4/tests/test_data_processing.py`

 * *Files identical despite different names*

### Comparing `uun-weatherstation-0.6.2/uun_weatherstation/data/sample-config.json` & `uun-weatherstation-0.6.4/uun_weatherstation/data/sample-config.json`

 * *Files identical despite different names*

### Comparing `uun-weatherstation-0.6.2/uun_weatherstation/modules/WeatherConditions.py` & `uun-weatherstation-0.6.4/uun_weatherstation/modules/WeatherConditions.py`

 * *Files identical despite different names*

### Comparing `uun-weatherstation-0.6.2/uun_weatherstation/modules/__init__.py` & `uun-weatherstation-0.6.4/uun_weatherstation/modules/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 """Initialize additional modules."""
 import logging
 import requests
+from uun_iot import UuAppClient
 
 from .WeatherConditions import WeatherConditions
 from .HealthCheck import HealthCheck
-from uun_iot.UuAppClient import UuCmdSession
+from uun_iot.UuAppClient import UuAppClient, UuCmdSession
 from uun_iot.diagnostic import DiagnosticEvent
 
 # module list in format { module_id: [module_instance, None], ... }
-def init(config, uuclient):
+def init(config: dict, uuclient: UuAppClient):
 
     gconfig = config["gateway"]
 
     if "healthCheck" not in gconfig:
         def cmd_weatherconditions(storage):
             """ Send weather to uuApp and return entries that failed to be sent. Each entry is sent separately. """
             uucmd = config["uuApp"]['uuCmdList']['weatherConditionsAdd']
             s = UuCmdSession(uuclient, uucmd)
             failed = []
             len_storage = 0
             len_failed = 0
             for dto_in in storage:
                 len_storage += 1
-                try:
-                    r, ok = s.post(dto_in)
-                    r.raise_for_status()
-                except requests.exceptions.RequestException as e:
-                    loggerwc.info("Error in server communication: %s", e)
+                r, (ok, exc) = s.post(dto_in)
+                if not ok:
                     len_failed += 1
                     failed.append(dto_in)
             return failed
 
         return [
             WeatherConditions(config=gconfig, uucmd=cmd_weatherconditions),
         ]
 
     healthcheck = HealthCheck(gconfig)
     notify = healthcheck.notifier("weatherConditions")
 
     loggerwc = logging.getLogger(__name__+".WeatherCondtionsUuCmd")
-    def cmd_weatherconditions(storage):
+    def cmd_weatherconditions_healthcheck(storage):
         """ Send weather to uuApp and return entries that failed to be sent. Each entry is sent separately. """
         uucmd = config["uuApp"]['uuCmdList']['weatherConditionsAdd']
         s = UuCmdSession(uuclient, uucmd)
         failed = []
         len_storage = 0
         len_failed = 0
         for dto_in in storage:
@@ -63,11 +61,11 @@
             notify(DiagnosticEvent.DATA_SEND_OK)
         else:
             notify(DiagnosticEvent.DATA_SEND_PARTIAL, failed=len_failed, successful=len_storage-len_failed)
 
         return failed
 
     return [
-        WeatherConditions(config=gconfig, uucmd=cmd_weatherconditions, notify=notify),
+        WeatherConditions(config=gconfig, uucmd=cmd_weatherconditions_healthcheck, notify=notify),
         healthcheck
     ]
```

### Comparing `uun-weatherstation-0.6.2/uun_weatherstation.egg-info/SOURCES.txt` & `uun-weatherstation-0.6.4/uun_weatherstation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

