# Comparing `tmp/uun-qrdoorlock-0.5.1.tar.gz` & `tmp/uun-qrdoorlock-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uun-qrdoorlock-0.5.1.tar", last modified: Thu Jan 26 11:50:08 2023, max compression
+gzip compressed data, was "uun-qrdoorlock-0.5.3.tar", last modified: Tue Aug  1 11:29:04 2023, max compression
```

## Comparing `uun-qrdoorlock-0.5.1.tar` & `uun-qrdoorlock-0.5.3.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:50:07.997583 uun-qrdoorlock-0.5.1/
--rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:44:22.000000 uun-qrdoorlock-0.5.1/LICENSE.md
--rw-------   0 hello     (1000) hello     (1000)      453 2023-01-26 11:50:07.997583 uun-qrdoorlock-0.5.1/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)     3102 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.1/README.md
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:50:07.994249 uun-qrdoorlock-0.5.1/bin/
--rwx------   0 hello     (1000) hello     (1000)     2044 2023-01-26 11:48:52.000000 uun-qrdoorlock-0.5.1/bin/uun-qrdoorlock
--rwx------   0 hello     (1000) hello     (1000)      562 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.1/bin/uun-qrdoorlock-install
--rw-------   0 hello     (1000) hello     (1000)       38 2023-01-26 11:50:07.997583 uun-qrdoorlock-0.5.1/setup.cfg
--rw-------   0 hello     (1000) hello     (1000)     1189 2023-01-26 11:46:24.000000 uun-qrdoorlock-0.5.1/setup.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:50:07.994249 uun-qrdoorlock-0.5.1/uun_qrdoorlock/
--rw-------   0 hello     (1000) hello     (1000)        0 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.1/uun_qrdoorlock/__init__.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:50:07.997583 uun-qrdoorlock-0.5.1/uun_qrdoorlock/data/
--rw-------   0 hello     (1000) hello     (1000)     1266 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.1/uun_qrdoorlock/data/sample-config.json
--rwx------   0 hello     (1000) hello     (1000)       56 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.1/uun_qrdoorlock/data/start.sh
--rw-------   0 hello     (1000) hello     (1000)      289 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.1/uun_qrdoorlock/data/systemd.service
--rw-------   0 hello     (1000) hello     (1000)     6522 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.1/uun_qrdoorlock/hw.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:50:07.997583 uun-qrdoorlock-0.5.1/uun_qrdoorlock/modules/
--rw-------   0 hello     (1000) hello     (1000)     3689 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.1/uun_qrdoorlock/modules/DoorMonitor.py
--rw-------   0 hello     (1000) hello     (1000)     6886 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.1/uun_qrdoorlock/modules/QrLock.py
--rw-------   0 hello     (1000) hello     (1000)     1363 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.1/uun_qrdoorlock/modules/__init__.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:50:07.994249 uun-qrdoorlock-0.5.1/uun_qrdoorlock.egg-info/
--rw-------   0 hello     (1000) hello     (1000)      453 2023-01-26 11:50:07.000000 uun-qrdoorlock-0.5.1/uun_qrdoorlock.egg-info/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)      522 2023-01-26 11:50:07.000000 uun-qrdoorlock-0.5.1/uun_qrdoorlock.egg-info/SOURCES.txt
--rw-------   0 hello     (1000) hello     (1000)        1 2023-01-26 11:50:07.000000 uun-qrdoorlock-0.5.1/uun_qrdoorlock.egg-info/dependency_links.txt
--rw-------   0 hello     (1000) hello     (1000)       52 2023-01-26 11:50:07.000000 uun-qrdoorlock-0.5.1/uun_qrdoorlock.egg-info/requires.txt
--rw-------   0 hello     (1000) hello     (1000)       15 2023-01-26 11:50:07.000000 uun-qrdoorlock-0.5.1/uun_qrdoorlock.egg-info/top_level.txt
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:29:04.268674 uun-qrdoorlock-0.5.3/
+-rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:44:22.000000 uun-qrdoorlock-0.5.3/LICENSE.md
+-rw-------   0 hello     (1000) hello     (1000)      453 2023-08-01 11:29:04.268674 uun-qrdoorlock-0.5.3/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)     3102 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.3/README.md
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:29:04.265340 uun-qrdoorlock-0.5.3/bin/
+-rwx------   0 hello     (1000) hello     (1000)     2746 2023-08-01 10:49:28.000000 uun-qrdoorlock-0.5.3/bin/uun-qrdoorlock
+-rwx------   0 hello     (1000) hello     (1000)      562 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.3/bin/uun-qrdoorlock-install
+-rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 11:29:04.268674 uun-qrdoorlock-0.5.3/setup.cfg
+-rw-------   0 hello     (1000) hello     (1000)     1189 2023-06-24 10:48:51.000000 uun-qrdoorlock-0.5.3/setup.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:29:04.265340 uun-qrdoorlock-0.5.3/tests/
+-rw-------   0 hello     (1000) hello     (1000)     2286 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.3/tests/test_qr.py
+-rw-------   0 hello     (1000) hello     (1000)     1067 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.3/tests/test_run.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:29:04.268674 uun-qrdoorlock-0.5.3/uun_qrdoorlock/
+-rw-------   0 hello     (1000) hello     (1000)        0 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock/__init__.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:29:04.268674 uun-qrdoorlock-0.5.3/uun_qrdoorlock/data/
+-rw-------   0 hello     (1000) hello     (1000)     1266 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock/data/sample-config.json
+-rwx------   0 hello     (1000) hello     (1000)       56 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock/data/start.sh
+-rw-------   0 hello     (1000) hello     (1000)      302 2023-08-01 10:49:46.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock/data/systemd.service
+-rw-------   0 hello     (1000) hello     (1000)     6522 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock/hw.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:29:04.268674 uun-qrdoorlock-0.5.3/uun_qrdoorlock/modules/
+-rw-------   0 hello     (1000) hello     (1000)     3689 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock/modules/DoorMonitor.py
+-rw-------   0 hello     (1000) hello     (1000)     6884 2023-06-24 10:30:54.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock/modules/QrLock.py
+-rw-------   0 hello     (1000) hello     (1000)     1363 2022-10-16 10:03:00.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock/modules/__init__.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:29:04.268674 uun-qrdoorlock-0.5.3/uun_qrdoorlock.egg-info/
+-rw-------   0 hello     (1000) hello     (1000)      453 2023-08-01 11:29:04.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock.egg-info/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)      557 2023-08-01 11:29:04.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock.egg-info/SOURCES.txt
+-rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 11:29:04.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock.egg-info/dependency_links.txt
+-rw-------   0 hello     (1000) hello     (1000)       52 2023-08-01 11:29:04.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock.egg-info/requires.txt
+-rw-------   0 hello     (1000) hello     (1000)       15 2023-08-01 11:29:04.000000 uun-qrdoorlock-0.5.3/uun_qrdoorlock.egg-info/top_level.txt
```

### Comparing `uun-qrdoorlock-0.5.1/LICENSE.md` & `uun-qrdoorlock-0.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uun-qrdoorlock-0.5.1/README.md` & `uun-qrdoorlock-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `uun-qrdoorlock-0.5.1/bin/uun-qrdoorlock` & `uun-qrdoorlock-0.5.3/bin/uun-qrdoorlock`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,86 @@
 #!/usr/bin/env python3
-from uun_iot.Gateway import Gateway
-from uun_qrdoorlock.modules import init
-
-import logging
-import time
 import argparse
+import logging
+import os
 import signal
 import sys
 
-__version__ = "0.5.1"
+from uun_iot.Gateway import Gateway
+from uun_iot.utils import LoggingSystemdHandler
+from uun_qrdoorlock.modules import init
+
+__version__ = "0.5.3"
 __package__ = "uun_qrdoorlock"
+library = "uun_iot"
+
 
 def main():
-    argp = argparse.ArgumentParser(prog=__package__, description='Retrieve QR data from QR reader, verify that it was signed by an authority and correspondingly gain access to electronically locked door.')
-    argp.add_argument('-v', '--version', action='version', version='%(prog) ' + __version__)
-    argp.add_argument('-l', '--log', metavar='loglevel', dest='loglevel', type=str, help='level of logging: [DEBUG, INFO, WARNING, ERROR, CRITICAL]', default='WARNING')
-    argp.add_argument('-c', '--config', metavar='config', dest='config', type=str, help='location of configuration JSON file', default='config.json')
+    argp = argparse.ArgumentParser(
+        prog=__package__,
+        description="Retrieve QR data from QR reader, verify that it was signed by an authority and correspondingly gain access to electronically locked door.",
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
+        help="location of configuration JSON file",
+        default="config.json",
+    )
+    argp.add_argument(
+        "--systemd",
+        help="enable output in systemd-friendly format",
+        action="store_true",
+    )
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
+        sys.exit(f"Invalid log level: {loglevel}")
 
-    # set formatting and levels for this package and library (uuniot)
-    loggerw = logging.getLogger(__package__) # application specific logger
+    loggerw = logging.getLogger(__package__)  # application specific logger
+    loggeru = logging.getLogger(library)  # library logger
     loggerw.setLevel(llevel)
-    loggeru = logging.getLogger("uun_iot") # library logger
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
+    handler = LoggingSystemdHandler() if args.systemd else logging.StreamHandler()
+    handler.setFormatter(logging.Formatter("%(name)s - %(levelname)s - %(message)s"))
+    loggerw.addHandler(handler)
+    loggeru.addHandler(handler)
 
     # start module system
     print("=== " + __package__ + " ===")
     with Gateway(args.config, init) as g:
+        # Register a SIGTERM signal, as it is issued by systemd on stop/restart.
+        #   Because by default, it does not run destructors.
+        # Ctrl-C (SINGINT) correctly runs destructors, so no need to register.
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

### Comparing `uun-qrdoorlock-0.5.1/bin/uun-qrdoorlock-install` & `uun-qrdoorlock-0.5.3/bin/uun-qrdoorlock-install`

 * *Files identical despite different names*

### Comparing `uun-qrdoorlock-0.5.1/setup.py` & `uun-qrdoorlock-0.5.3/setup.py`

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
+        "uun-iot >= 0.9.0",
         "pyserial",
         "pynacl",
         "validators",
         "termcolor"
     ],
     #extras_require = {
     #   "dev": [
```

### Comparing `uun-qrdoorlock-0.5.1/uun_qrdoorlock/data/sample-config.json` & `uun-qrdoorlock-0.5.3/uun_qrdoorlock/data/sample-config.json`

 * *Files identical despite different names*

### Comparing `uun-qrdoorlock-0.5.1/uun_qrdoorlock/hw.py` & `uun-qrdoorlock-0.5.3/uun_qrdoorlock/hw.py`

 * *Files identical despite different names*

### Comparing `uun-qrdoorlock-0.5.1/uun_qrdoorlock/modules/DoorMonitor.py` & `uun-qrdoorlock-0.5.3/uun_qrdoorlock/modules/DoorMonitor.py`

 * *Files identical despite different names*

### Comparing `uun-qrdoorlock-0.5.1/uun_qrdoorlock/modules/QrLock.py` & `uun-qrdoorlock-0.5.3/uun_qrdoorlock/modules/QrLock.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                 bytesize=serial.EIGHTBITS,
                 timeout=1
                 )
         self._qrreader = QrReader(so, self._c("lockOpenInterval"))
 
     def _init_lock(self):
         """ Initialize lock control. """
-        if not self._c("virtualMode", module=ConfigScopeEnum.GATEWAY):
+        if not self._c("virtualMode", scope=ConfigScopeEnum.GATEWAY):
             from RPi import GPIO
             self._pin = self._c("relayPin")
             GPIO.setmode(GPIO.BCM)
             GPIO.setup(self._pin, GPIO.OUT, initial=GPIO.HIGH)
             def on():
                 GPIO.output(self._pin, GPIO.LOW)
             def off():
@@ -184,11 +184,11 @@
                         )
                 self._config[self.id]["publicKey"] = pubkey
 
             self._init_reader()
             self._init_lock()
 
     def __del__(self):
-        if not self._c("virtualMode", module=ConfigScopeEnum.GATEWAY):
+        if not self._c("virtualMode", scope=ConfigScopeEnum.GATEWAY):
             from RPi import GPIO
             GPIO.cleanup(self._pin)
```

### Comparing `uun-qrdoorlock-0.5.1/uun_qrdoorlock/modules/__init__.py` & `uun-qrdoorlock-0.5.3/uun_qrdoorlock/modules/__init__.py`

 * *Files identical despite different names*

