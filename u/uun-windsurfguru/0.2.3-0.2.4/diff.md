# Comparing `tmp/uun-windsurfguru-0.2.3.tar.gz` & `tmp/uun-windsurfguru-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uun-windsurfguru-0.2.3.tar", last modified: Thu Jan 26 12:09:27 2023, max compression
+gzip compressed data, was "uun-windsurfguru-0.2.4.tar", last modified: Tue Aug  1 11:28:46 2023, max compression
```

## Comparing `uun-windsurfguru-0.2.3.tar` & `uun-windsurfguru-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 12:09:27.006176 uun-windsurfguru-0.2.3/
--rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:44:55.000000 uun-windsurfguru-0.2.3/LICENSE.md
--rw-------   0 hello     (1000) hello     (1000)      541 2023-01-26 12:09:27.006176 uun-windsurfguru-0.2.3/PKG-INFO
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 12:09:27.006176 uun-windsurfguru-0.2.3/bin/
--rwx------   0 hello     (1000) hello     (1000)     2525 2023-01-26 12:08:08.000000 uun-windsurfguru-0.2.3/bin/uun-windsurfguru
--rwx------   0 hello     (1000) hello     (1000)      504 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.3/bin/uun-windsurfguru-install
--rwx------   0 hello     (1000) hello     (1000)     1920 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.3/bin/uun-windsurfguru-setup
--rw-------   0 hello     (1000) hello     (1000)       38 2023-01-26 12:09:27.006176 uun-windsurfguru-0.2.3/setup.cfg
--rw-------   0 hello     (1000) hello     (1000)     1391 2023-01-26 12:07:43.000000 uun-windsurfguru-0.2.3/setup.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 12:09:27.006176 uun-windsurfguru-0.2.3/uun_windsurfguru/
--rw-------   0 hello     (1000) hello     (1000)        0 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.3/uun_windsurfguru/__init__.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 12:09:27.006176 uun-windsurfguru-0.2.3/uun_windsurfguru/data/
--rw-------   0 hello     (1000) hello     (1000)     3830 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.3/uun_windsurfguru/data/sample-config.json
--rwx------   0 hello     (1000) hello     (1000)       68 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.3/uun_windsurfguru/data/start.sh
--rw-------   0 hello     (1000) hello     (1000)      291 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.3/uun_windsurfguru/data/systemd.service
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 12:09:27.006176 uun-windsurfguru-0.2.3/uun_windsurfguru/modules/
--rw-------   0 hello     (1000) hello     (1000)    24695 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.3/uun_windsurfguru/modules/WindSurfGuru.py
--rw-------   0 hello     (1000) hello     (1000)      408 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.3/uun_windsurfguru/modules/__init__.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 12:09:27.006176 uun-windsurfguru-0.2.3/uun_windsurfguru.egg-info/
--rw-------   0 hello     (1000) hello     (1000)      541 2023-01-26 12:09:26.000000 uun-windsurfguru-0.2.3/uun_windsurfguru.egg-info/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)      512 2023-01-26 12:09:27.000000 uun-windsurfguru-0.2.3/uun_windsurfguru.egg-info/SOURCES.txt
--rw-------   0 hello     (1000) hello     (1000)        1 2023-01-26 12:09:26.000000 uun-windsurfguru-0.2.3/uun_windsurfguru.egg-info/dependency_links.txt
--rw-------   0 hello     (1000) hello     (1000)      171 2023-01-26 12:09:26.000000 uun-windsurfguru-0.2.3/uun_windsurfguru.egg-info/requires.txt
--rw-------   0 hello     (1000) hello     (1000)       17 2023-01-26 12:09:26.000000 uun-windsurfguru-0.2.3/uun_windsurfguru.egg-info/top_level.txt
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:46.731943 uun-windsurfguru-0.2.4/
+-rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:44:55.000000 uun-windsurfguru-0.2.4/LICENSE.md
+-rw-------   0 hello     (1000) hello     (1000)      541 2023-08-01 11:28:46.731943 uun-windsurfguru-0.2.4/PKG-INFO
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:46.728609 uun-windsurfguru-0.2.4/bin/
+-rwx------   0 hello     (1000) hello     (1000)     2950 2023-08-01 11:12:29.000000 uun-windsurfguru-0.2.4/bin/uun-windsurfguru
+-rwx------   0 hello     (1000) hello     (1000)      504 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.4/bin/uun-windsurfguru-install
+-rwx------   0 hello     (1000) hello     (1000)     1920 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.4/bin/uun-windsurfguru-setup
+-rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 11:28:46.731943 uun-windsurfguru-0.2.4/setup.cfg
+-rw-------   0 hello     (1000) hello     (1000)     1391 2023-08-01 11:09:19.000000 uun-windsurfguru-0.2.4/setup.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:46.731943 uun-windsurfguru-0.2.4/tests/
+-rw-------   0 hello     (1000) hello     (1000)     5545 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.4/tests/test_main.py
+-rw-------   0 hello     (1000) hello     (1000)      167 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.4/tests/test_run.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:46.731943 uun-windsurfguru-0.2.4/uun_windsurfguru/
+-rw-------   0 hello     (1000) hello     (1000)        0 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.4/uun_windsurfguru/__init__.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:46.731943 uun-windsurfguru-0.2.4/uun_windsurfguru/data/
+-rw-------   0 hello     (1000) hello     (1000)     3830 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.4/uun_windsurfguru/data/sample-config.json
+-rwx------   0 hello     (1000) hello     (1000)       68 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.4/uun_windsurfguru/data/start.sh
+-rw-------   0 hello     (1000) hello     (1000)      304 2023-08-01 11:06:10.000000 uun-windsurfguru-0.2.4/uun_windsurfguru/data/systemd.service
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:46.731943 uun-windsurfguru-0.2.4/uun_windsurfguru/modules/
+-rw-------   0 hello     (1000) hello     (1000)    24695 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.4/uun_windsurfguru/modules/WindSurfGuru.py
+-rw-------   0 hello     (1000) hello     (1000)      408 2022-10-16 10:03:01.000000 uun-windsurfguru-0.2.4/uun_windsurfguru/modules/__init__.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:46.731943 uun-windsurfguru-0.2.4/uun_windsurfguru.egg-info/
+-rw-------   0 hello     (1000) hello     (1000)      541 2023-08-01 11:28:46.000000 uun-windsurfguru-0.2.4/uun_windsurfguru.egg-info/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)      549 2023-08-01 11:28:46.000000 uun-windsurfguru-0.2.4/uun_windsurfguru.egg-info/SOURCES.txt
+-rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 11:28:46.000000 uun-windsurfguru-0.2.4/uun_windsurfguru.egg-info/dependency_links.txt
+-rw-------   0 hello     (1000) hello     (1000)      171 2023-08-01 11:28:46.000000 uun-windsurfguru-0.2.4/uun_windsurfguru.egg-info/requires.txt
+-rw-------   0 hello     (1000) hello     (1000)       17 2023-08-01 11:28:46.000000 uun-windsurfguru-0.2.4/uun_windsurfguru.egg-info/top_level.txt
```

### Comparing `uun-windsurfguru-0.2.3/LICENSE.md` & `uun-windsurfguru-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uun-windsurfguru-0.2.3/PKG-INFO` & `uun-windsurfguru-0.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uun-windsurfguru
-Version: 0.2.3
+Version: 0.2.4
 Summary: Display wind surf conditions on a colorful LED strip.
 Home-page: https://uuapp.plus4u.net/uu-bookkit-maing01/c145b7fe6d754775b71e196b3fbb9a6a/book/page?code=64720442
 Author: (UUN) Tomáš Faikl & Marek Beránek
 Author-email: tomas.faikl@unicornuniversity.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `uun-windsurfguru-0.2.3/bin/uun-windsurfguru` & `uun-windsurfguru-0.2.4/bin/uun-windsurfguru`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,99 @@
 #!/usr/bin/env python3
-from uun_iot import Gateway
-from uun_windsurfguru.modules import init
-
-import logging
-import time
 import argparse
-import sys
+import logging
+import os
 import signal
+import sys
 
-__version__ = "0.2.3"
+from uun_iot import Gateway
+from uun_iot.utils import LoggingSystemdHandler
+from uun_windsurfguru.modules import init
+
+__version__ = "0.2.4"
 __package__ = "uun_windsurfguru"
 
 
 def main():
     argp = argparse.ArgumentParser(
-        prog=__package__, description='Display wind surf conditions on a colorful LED strip.')
-    argp.add_argument('-v', '--version', action='version',
-                      version='%(prog) ' + __version__)
-    argp.add_argument('-l', '--log', metavar='loglevel', dest='loglevel', type=str,
-                      help='level of logging: [DEBUG, INFO, WARNING, ERROR, CRITICAL]', default='WARNING')
-    argp.add_argument('-c', '--config', metavar='config', dest='config',
-                      type=str, help='configuration JSON file', default='config.json')
+        prog=__package__,
+        description="Display wind surf conditions on a colorful LED strip.",
+    )
+    argp.add_argument(
+        "-v", "--version", action="version", version="%(prog) " + __version__
+    )
+    argp.add_argument(
+        "-l",
+        "--log",
+        metavar="loglevel",
+        dest="loglevel",
+        type=str,
+        help="level of logging: [DEBUG, INFO, WARNING, ERROR, CRITICAL]",
+        default="WARNING",
+    )
+    argp.add_argument(
+        "-c",
+        "--config",
+        metavar="config",
+        dest="config",
+        type=str,
+        help="configuration JSON file",
+        default="config.json",
+    )
+    argp.add_argument(
+        "--systemd",
+        help="enable output in systemd-friendly format",
+        action="store_true",
+    )
+
+    sys.excepthook = lambda exctype, value, tb: logging.getLogger(
+        __package__
+    ).exception("Exception: ", exc_info=(exctype, value, tb))
+
     args = argp.parse_args()
+    if not os.path.exists(args.config):
+        sys.exit(f"Could not find configuration file '{args.config}'")
 
-    ## = SETTING LOGGING = ##
-    # set log level from option
     loglevel = args.loglevel
     llevel = getattr(logging, loglevel.upper(), None)
     if not isinstance(llevel, int):
-        raise ValueError('Invalid log level: %s' % loglevel)
+        raise ValueError(f"Invalid log level: {loglevel}")
 
-    # set formatting and levels for this package and library (uuniot)
     loggerw = logging.getLogger(__package__)  # application specific logger
     loggerw.setLevel(llevel)
     loggeru = logging.getLogger("uun_iot")  # library logger
     loggeru.setLevel(llevel)
     loggeru2 = logging.getLogger("uun_iot_libledstrip")
     loggeru2.setLevel(llevel)
 
-    # console handler (output text to console), here can be added file handlers, server handlers, ...
-    ch = logging.StreamHandler()
-    ch.setLevel(llevel)
-    # set log format
-    formatter = logging.Formatter(
-        '%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-    ch.setFormatter(formatter)
-
-    # asssign the same handler to loggers
-    loggerw.addHandler(ch)
-    loggeru.addHandler(ch)
-    loggeru2.addHandler(ch)
+    handler = LoggingSystemdHandler() if args.systemd else logging.StreamHandler()
+    handler.setLevel(llevel)
+    handler.setFormatter(logging.Formatter("%(name)s - %(levelname)s - %(message)s"))
+
+    loggerw.addHandler(handler)
+    loggeru.addHandler(handler)
+    loggeru2.addHandler(handler)
 
     # try to add colors to Windows (colored LED strip)
     try:
         from colorama import init as init_c
+
         init_c()
     except ImportError:
         pass
 
     # start module system
     print("=== " + __package__ + " ===")
     with Gateway(args.config, init) as g:
         # Register a SIGTERM signal, as it is issued by systemd on stop/restart.
         #   Because by default, it does not run destructors.
         # Ctrl-C (SINGINT) correctly runs destructors, so no need to register.
+        # SIGUSR1 is used internally by HealthCheck to restart the gateway
         signal.signal(signal.SIGTERM, g.signal_handler)
-        while True:
-            time.sleep(1)
+        signal.signal(signal.SIGINT, g.signal_handler)
+        signal.signal(signal.SIGUSR1, g.signal_handler)
+
+        g.stopev.wait()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `uun-windsurfguru-0.2.3/bin/uun-windsurfguru-setup` & `uun-windsurfguru-0.2.4/bin/uun-windsurfguru-setup`

 * *Files identical despite different names*

### Comparing `uun-windsurfguru-0.2.3/setup.py` & `uun-windsurfguru-0.2.4/setup.py`

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
-        "uun-iot >= 0.8.2",
+        "uun-iot >= 0.9.1",
         "uun-iot-libledstrip >= 0.2.3"
     ],
     extras_require={
         "neopixel": [
             "uun-iot-libledstrip[neopixel] >= 0.2.3",
         ],
         "gpio": [
```

### Comparing `uun-windsurfguru-0.2.3/uun_windsurfguru/data/sample-config.json` & `uun-windsurfguru-0.2.4/uun_windsurfguru/data/sample-config.json`

 * *Files identical despite different names*

### Comparing `uun-windsurfguru-0.2.3/uun_windsurfguru/modules/WindSurfGuru.py` & `uun-windsurfguru-0.2.4/uun_windsurfguru/modules/WindSurfGuru.py`

 * *Files identical despite different names*

### Comparing `uun-windsurfguru-0.2.3/uun_windsurfguru.egg-info/PKG-INFO` & `uun-windsurfguru-0.2.4/uun_windsurfguru.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uun-windsurfguru
-Version: 0.2.3
+Version: 0.2.4
 Summary: Display wind surf conditions on a colorful LED strip.
 Home-page: https://uuapp.plus4u.net/uu-bookkit-maing01/c145b7fe6d754775b71e196b3fbb9a6a/book/page?code=64720442
 Author: (UUN) Tomáš Faikl & Marek Beránek
 Author-email: tomas.faikl@unicornuniversity.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

