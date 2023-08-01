# Comparing `tmp/uun-guardman-0.1.2.tar.gz` & `tmp/uun-guardman-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uun-guardman-0.1.2.tar", last modified: Thu Jan 26 11:37:28 2023, max compression
+gzip compressed data, was "uun-guardman-0.1.4.tar", last modified: Tue Aug  1 11:24:33 2023, max compression
```

## Comparing `uun-guardman-0.1.2.tar` & `uun-guardman-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:37:28.135824 uun-guardman-0.1.2/
--rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:40:40.000000 uun-guardman-0.1.2/LICENSE.md
--rw-------   0 hello     (1000) hello     (1000)      386 2023-01-26 11:37:28.135824 uun-guardman-0.1.2/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)      392 2022-10-16 10:02:57.000000 uun-guardman-0.1.2/README.md
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:37:28.135824 uun-guardman-0.1.2/bin/
--rwx------   0 hello     (1000) hello     (1000)     2411 2023-01-26 11:36:50.000000 uun-guardman-0.1.2/bin/uun-guardman
--rwx------   0 hello     (1000) hello     (1000)      500 2022-10-16 10:02:57.000000 uun-guardman-0.1.2/bin/uun-guardman-install
--rwx------   0 hello     (1000) hello     (1000)     1891 2022-10-16 10:02:57.000000 uun-guardman-0.1.2/bin/uun-guardman-setup
--rw-------   0 hello     (1000) hello     (1000)       38 2023-01-26 11:37:28.135824 uun-guardman-0.1.2/setup.cfg
--rw-------   0 hello     (1000) hello     (1000)     1214 2023-01-26 11:35:39.000000 uun-guardman-0.1.2/setup.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:37:28.135824 uun-guardman-0.1.2/uun_guardman/
--rw-------   0 hello     (1000) hello     (1000)        0 2022-10-16 10:02:57.000000 uun-guardman-0.1.2/uun_guardman/__init__.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:37:28.135824 uun-guardman-0.1.2/uun_guardman/data/
--rw-------   0 hello     (1000) hello     (1000)     4005 2022-10-16 10:02:57.000000 uun-guardman-0.1.2/uun_guardman/data/sample-config.json
--rwx------   0 hello     (1000) hello     (1000)       64 2022-10-16 10:02:57.000000 uun-guardman-0.1.2/uun_guardman/data/start.sh
--rw-------   0 hello     (1000) hello     (1000)      287 2022-10-16 10:02:57.000000 uun-guardman-0.1.2/uun_guardman/data/systemd.service
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:37:28.135824 uun-guardman-0.1.2/uun_guardman/modules/
--rw-------   0 hello     (1000) hello     (1000)     8981 2022-10-16 10:02:57.000000 uun-guardman-0.1.2/uun_guardman/modules/GuardMan.py
--rw-------   0 hello     (1000) hello     (1000)      426 2022-10-16 10:02:57.000000 uun-guardman-0.1.2/uun_guardman/modules/__init__.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:37:28.135824 uun-guardman-0.1.2/uun_guardman.egg-info/
--rw-------   0 hello     (1000) hello     (1000)      386 2023-01-26 11:37:28.000000 uun-guardman-0.1.2/uun_guardman.egg-info/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)      462 2023-01-26 11:37:28.000000 uun-guardman-0.1.2/uun_guardman.egg-info/SOURCES.txt
--rw-------   0 hello     (1000) hello     (1000)        1 2023-01-26 11:37:28.000000 uun-guardman-0.1.2/uun_guardman.egg-info/dependency_links.txt
--rw-------   0 hello     (1000) hello     (1000)      130 2023-01-26 11:37:28.000000 uun-guardman-0.1.2/uun_guardman.egg-info/requires.txt
--rw-------   0 hello     (1000) hello     (1000)       13 2023-01-26 11:37:28.000000 uun-guardman-0.1.2/uun_guardman.egg-info/top_level.txt
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:24:33.257641 uun-guardman-0.1.4/
+-rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:40:40.000000 uun-guardman-0.1.4/LICENSE.md
+-rw-------   0 hello     (1000) hello     (1000)      386 2023-08-01 11:24:33.257641 uun-guardman-0.1.4/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)      392 2022-10-16 10:02:57.000000 uun-guardman-0.1.4/README.md
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:24:33.254307 uun-guardman-0.1.4/bin/
+-rwx------   0 hello     (1000) hello     (1000)     3021 2023-08-01 11:17:43.000000 uun-guardman-0.1.4/bin/uun-guardman
+-rwx------   0 hello     (1000) hello     (1000)      500 2022-10-16 10:02:57.000000 uun-guardman-0.1.4/bin/uun-guardman-install
+-rwx------   0 hello     (1000) hello     (1000)     1891 2022-10-16 10:02:57.000000 uun-guardman-0.1.4/bin/uun-guardman-setup
+-rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 11:24:33.257641 uun-guardman-0.1.4/setup.cfg
+-rw-------   0 hello     (1000) hello     (1000)     1200 2023-08-01 11:19:00.000000 uun-guardman-0.1.4/setup.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:24:33.254307 uun-guardman-0.1.4/tests/
+-rw-------   0 hello     (1000) hello     (1000)    10304 2022-10-16 10:02:57.000000 uun-guardman-0.1.4/tests/test_main.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:24:33.254307 uun-guardman-0.1.4/uun_guardman/
+-rw-------   0 hello     (1000) hello     (1000)        0 2022-10-16 10:02:57.000000 uun-guardman-0.1.4/uun_guardman/__init__.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:24:33.257641 uun-guardman-0.1.4/uun_guardman/data/
+-rw-------   0 hello     (1000) hello     (1000)     4005 2022-10-16 10:02:57.000000 uun-guardman-0.1.4/uun_guardman/data/sample-config.json
+-rwx------   0 hello     (1000) hello     (1000)       64 2022-10-16 10:02:57.000000 uun-guardman-0.1.4/uun_guardman/data/start.sh
+-rw-------   0 hello     (1000) hello     (1000)      300 2023-08-01 11:17:55.000000 uun-guardman-0.1.4/uun_guardman/data/systemd.service
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:24:33.257641 uun-guardman-0.1.4/uun_guardman/modules/
+-rw-------   0 hello     (1000) hello     (1000)     8981 2022-10-16 10:02:57.000000 uun-guardman-0.1.4/uun_guardman/modules/GuardMan.py
+-rw-------   0 hello     (1000) hello     (1000)      426 2022-10-16 10:02:57.000000 uun-guardman-0.1.4/uun_guardman/modules/__init__.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:24:33.257641 uun-guardman-0.1.4/uun_guardman.egg-info/
+-rw-------   0 hello     (1000) hello     (1000)      386 2023-08-01 11:24:33.000000 uun-guardman-0.1.4/uun_guardman.egg-info/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)      481 2023-08-01 11:24:33.000000 uun-guardman-0.1.4/uun_guardman.egg-info/SOURCES.txt
+-rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 11:24:33.000000 uun-guardman-0.1.4/uun_guardman.egg-info/dependency_links.txt
+-rw-------   0 hello     (1000) hello     (1000)      130 2023-08-01 11:24:33.000000 uun-guardman-0.1.4/uun_guardman.egg-info/requires.txt
+-rw-------   0 hello     (1000) hello     (1000)       13 2023-08-01 11:24:33.000000 uun-guardman-0.1.4/uun_guardman.egg-info/top_level.txt
```

### Comparing `uun-guardman-0.1.2/LICENSE.md` & `uun-guardman-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uun-guardman-0.1.2/bin/uun-guardman` & `uun-guardman-0.1.4/bin/uun-guardman`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,100 @@
 #!/usr/bin/env python3
-from uun_iot import Gateway
-from uun_guardman.modules import init
-
-import logging
-import time
 import argparse
-import sys
+import logging
+import os
 import signal
+import sys
+import time
 
-__version__ = "0.1.2"
+from uun_guardman.modules import init
+from uun_iot import Gateway
+from uun_iot.utils import LoggingSystemdHandler
+
+__version__ = "0.1.4"
 __package__ = "uun_guardman"
 
+
 def main():
-    argp = argparse.ArgumentParser(prog=__package__, description='Connect to uuConsole server application, get status codes of specified processes and display them using color-coding and blinkg on a LED strip.')
-    argp.add_argument('-v', '--version', action='version', version='%(prog) ' + __version__)
-    argp.add_argument('-l', '--log', metavar='loglevel', dest='loglevel', type=str, help='level of logging: [DEBUG, INFO, WARNING, ERROR, CRITICAL]', default='WARNING')
-    argp.add_argument('-c', '--config', metavar='config', dest='config', type=str, help='configuration JSON file', default='config.json')
+    argp = argparse.ArgumentParser(
+        prog=__package__,
+        description="Connect to uuConsole server application, get status codes of specified processes and display them using color-coding and blinkg on a LED strip.",
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
+        raise ValueError("Invalid log level: %s" % loglevel)
 
-    # set formatting and levels for this package and library (uuniot)
-    loggerw = logging.getLogger(__package__) # application specific logger
+    loggerw = logging.getLogger(__package__)  # application specific logger
     loggerw.setLevel(llevel)
-    loggeru = logging.getLogger("uun_iot") # library logger
+    loggeru = logging.getLogger("uun_iot")  # library logger
     loggeru.setLevel(llevel)
-    
-    # console handler (output text to console), here can be added file handlers, server handlers, ...
-    ch = logging.StreamHandler()
-    ch.setLevel(llevel)
-    # set log format
-    formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-    ch.setFormatter(formatter)
-
-    # asssign the same handler to loggers
-    loggerw.addHandler(ch)
-    loggeru.addHandler(ch)
+    loggeru2 = logging.getLogger("uun_iot_libledstrip")
+    loggeru2.setLevel(llevel)
+
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
 
-    # start module system
     print("=== " + __package__ + " ===")
     with Gateway(args.config, init) as g:
         # Register a SIGTERM signal, as it is issued by systemd on stop/restart.
         #   Because by default, it does not run destructors.
         # Ctrl-C (SINGINT) correctly runs destructors, so no need to register.
-
+        # SIGUSR1 is used internally by HealthCheck to restart the gateway
         signal.signal(signal.SIGTERM, g.signal_handler)
-        while True:
-            time.sleep(1)
+        signal.signal(signal.SIGINT, g.signal_handler)
+        signal.signal(signal.SIGUSR1, g.signal_handler)
+
+        g.stopev.wait()
+
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `uun-guardman-0.1.2/bin/uun-guardman-setup` & `uun-guardman-0.1.4/bin/uun-guardman-setup`

 * *Files identical despite different names*

### Comparing `uun-guardman-0.1.2/setup.py` & `uun-guardman-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 import setuptools
-import shutil
 import os
 import re
 
 name="uun-guardman"
 name_=name.replace('-', '_')
 
 # version from exported binary
 pkg_path = os.path.abspath(os.path.dirname(__file__))
 with open(f"{pkg_path}/bin/{name}", encoding="utf8") as f:
     version = re.search(r'__version__ = "(.*?)"', f.read()).group(1)
 
 setuptools.setup(
     name=name,
     version=version,
-    author="(UUN) - Marek Beránek, Tomáš Faikl",
+    author="(UUN) - Tomáš Faikl, Marek Beránek",
     author_email="",
     description="Display status of remote uuApp on a colorful LED strip.",
     url="",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License"
     ],
     python_requires='>=3.6',
     install_requires=[
-        "uun-iot >= 0.8.2",
-        "uun-iot-libledstrip >= 0.2.3" 
+        "uun-iot >= 0.9.1",
+        "uun-iot-libledstrip >= 0.2.4" 
     ],
     extras_require={
         # uun-iot-libledstrip >= 0.2
         "neopixel": [
-            "uun-iot-libledstrip[neopixel] >= 0.2.3",
+            "uun-iot-libledstrip[neopixel] >= 0.2.4",
         ],
         "dev": [
-            "uun-iot-libledstrip[dev] >= 0.2.3",
+            "uun-iot-libledstrip[dev] >= 0.2.4",
         ]
     },
     scripts=[
         "bin/" + name,
         "bin/" + name + "-install",
         "bin/" + name + "-setup"
     ],
```

### Comparing `uun-guardman-0.1.2/uun_guardman/data/sample-config.json` & `uun-guardman-0.1.4/uun_guardman/data/sample-config.json`

 * *Files identical despite different names*

### Comparing `uun-guardman-0.1.2/uun_guardman/modules/GuardMan.py` & `uun-guardman-0.1.4/uun_guardman/modules/GuardMan.py`

 * *Files identical despite different names*

