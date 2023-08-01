# Comparing `tmp/uun-weatherstation-0.6.4.tar.gz` & `tmp/uun-weatherstation-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uun-weatherstation-0.6.4.tar", last modified: Tue Aug  1 10:13:10 2023, max compression
+gzip compressed data, was "uun-weatherstation-0.6.5.tar", last modified: Tue Aug  1 11:28:19 2023, max compression
```

## Comparing `uun-weatherstation-0.6.4.tar` & `uun-weatherstation-0.6.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:13:10.380829 uun-weatherstation-0.6.4/
--rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:44:43.000000 uun-weatherstation-0.6.4/LICENSE.md
--rw-------   0 hello     (1000) hello     (1000)      466 2023-08-01 10:13:10.380829 uun-weatherstation-0.6.4/PKG-INFO
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:13:10.380829 uun-weatherstation-0.6.4/bin/
--rwx------   0 hello     (1000) hello     (1000)     2499 2023-08-01 10:06:59.000000 uun-weatherstation-0.6.4/bin/uun-weatherstation
--rwx------   0 hello     (1000) hello     (1000)      505 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/bin/uun-weatherstation-install
--rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 10:13:10.380829 uun-weatherstation-0.6.4/setup.cfg
--rw-------   0 hello     (1000) hello     (1000)     1065 2023-08-01 10:11:04.000000 uun-weatherstation-0.6.4/setup.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:13:10.380829 uun-weatherstation-0.6.4/tests/
--rw-------   0 hello     (1000) hello     (1000)     5995 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/tests/test_data_processing.py
--rw-------   0 hello     (1000) hello     (1000)      139 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/tests/test_run_5s.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:13:10.380829 uun-weatherstation-0.6.4/uun_weatherstation/
--rw-------   0 hello     (1000) hello     (1000)        1 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/uun_weatherstation/__init__.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:13:10.380829 uun-weatherstation-0.6.4/uun_weatherstation/data/
--rw-------   0 hello     (1000) hello     (1000)     1657 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/uun_weatherstation/data/sample-config.json
--rwx------   0 hello     (1000) hello     (1000)       70 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/uun_weatherstation/data/start.sh
--rw-------   0 hello     (1000) hello     (1000)      292 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/uun_weatherstation/data/systemd.service
--rw-------   0 hello     (1000) hello     (1000)      194 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/uun_weatherstation/diagnostic.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:13:10.380829 uun-weatherstation-0.6.4/uun_weatherstation/modules/
--rw-------   0 hello     (1000) hello     (1000)      416 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/uun_weatherstation/modules/HealthCheck.py
--rw-------   0 hello     (1000) hello     (1000)     8536 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/uun_weatherstation/modules/WeatherConditions.py
--rw-------   0 hello     (1000) hello     (1000)     2555 2023-08-01 07:46:32.000000 uun-weatherstation-0.6.4/uun_weatherstation/modules/__init__.py
--rw-------   0 hello     (1000) hello     (1000)      326 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.4/uun_weatherstation/utils.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 10:13:10.380829 uun-weatherstation-0.6.4/uun_weatherstation.egg-info/
--rw-------   0 hello     (1000) hello     (1000)      466 2023-08-01 10:13:10.000000 uun-weatherstation-0.6.4/uun_weatherstation.egg-info/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)      670 2023-08-01 10:13:10.000000 uun-weatherstation-0.6.4/uun_weatherstation.egg-info/SOURCES.txt
--rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 10:13:10.000000 uun-weatherstation-0.6.4/uun_weatherstation.egg-info/dependency_links.txt
--rw-------   0 hello     (1000) hello     (1000)       32 2023-08-01 10:13:10.000000 uun-weatherstation-0.6.4/uun_weatherstation.egg-info/requires.txt
--rw-------   0 hello     (1000) hello     (1000)       19 2023-08-01 10:13:10.000000 uun-weatherstation-0.6.4/uun_weatherstation.egg-info/top_level.txt
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:19.695177 uun-weatherstation-0.6.5/
+-rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:44:43.000000 uun-weatherstation-0.6.5/LICENSE.md
+-rw-------   0 hello     (1000) hello     (1000)      466 2023-08-01 11:28:19.695177 uun-weatherstation-0.6.5/PKG-INFO
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:19.691843 uun-weatherstation-0.6.5/bin/
+-rwx------   0 hello     (1000) hello     (1000)     2717 2023-08-01 10:46:25.000000 uun-weatherstation-0.6.5/bin/uun-weatherstation
+-rwx------   0 hello     (1000) hello     (1000)      505 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.5/bin/uun-weatherstation-install
+-rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 11:28:19.695177 uun-weatherstation-0.6.5/setup.cfg
+-rw-------   0 hello     (1000) hello     (1000)     1065 2023-08-01 10:11:04.000000 uun-weatherstation-0.6.5/setup.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:19.691843 uun-weatherstation-0.6.5/tests/
+-rw-------   0 hello     (1000) hello     (1000)     5995 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.5/tests/test_data_processing.py
+-rw-------   0 hello     (1000) hello     (1000)      139 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.5/tests/test_run_5s.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:19.691843 uun-weatherstation-0.6.5/uun_weatherstation/
+-rw-------   0 hello     (1000) hello     (1000)        1 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.5/uun_weatherstation/__init__.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:19.695177 uun-weatherstation-0.6.5/uun_weatherstation/data/
+-rw-------   0 hello     (1000) hello     (1000)     1657 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.5/uun_weatherstation/data/sample-config.json
+-rwx------   0 hello     (1000) hello     (1000)       70 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.5/uun_weatherstation/data/start.sh
+-rw-------   0 hello     (1000) hello     (1000)      305 2023-08-01 10:42:32.000000 uun-weatherstation-0.6.5/uun_weatherstation/data/systemd.service
+-rw-------   0 hello     (1000) hello     (1000)      194 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.5/uun_weatherstation/diagnostic.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:19.695177 uun-weatherstation-0.6.5/uun_weatherstation/modules/
+-rw-------   0 hello     (1000) hello     (1000)      416 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.5/uun_weatherstation/modules/HealthCheck.py
+-rw-------   0 hello     (1000) hello     (1000)     8536 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.5/uun_weatherstation/modules/WeatherConditions.py
+-rw-------   0 hello     (1000) hello     (1000)     2555 2023-08-01 07:46:32.000000 uun-weatherstation-0.6.5/uun_weatherstation/modules/__init__.py
+-rw-------   0 hello     (1000) hello     (1000)      326 2022-10-16 10:03:01.000000 uun-weatherstation-0.6.5/uun_weatherstation/utils.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:19.695177 uun-weatherstation-0.6.5/uun_weatherstation.egg-info/
+-rw-------   0 hello     (1000) hello     (1000)      466 2023-08-01 11:28:19.000000 uun-weatherstation-0.6.5/uun_weatherstation.egg-info/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)      670 2023-08-01 11:28:19.000000 uun-weatherstation-0.6.5/uun_weatherstation.egg-info/SOURCES.txt
+-rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 11:28:19.000000 uun-weatherstation-0.6.5/uun_weatherstation.egg-info/dependency_links.txt
+-rw-------   0 hello     (1000) hello     (1000)       32 2023-08-01 11:28:19.000000 uun-weatherstation-0.6.5/uun_weatherstation.egg-info/requires.txt
+-rw-------   0 hello     (1000) hello     (1000)       19 2023-08-01 11:28:19.000000 uun-weatherstation-0.6.5/uun_weatherstation.egg-info/top_level.txt
```

### Comparing `uun-weatherstation-0.6.4/LICENSE.md` & `uun-weatherstation-0.6.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uun-weatherstation-0.6.4/bin/uun-weatherstation` & `uun-weatherstation-0.6.5/bin/uun-weatherstation`

 * *Files 20% similar despite different names*

```diff
@@ -6,31 +6,54 @@
 import signal
 import sys
 
 from uun_iot.Gateway import Gateway
 from uun_iot.utils import LoggingSystemdHandler
 from uun_weatherstation.modules import init
 
-__version__ = "0.6.4"
+__version__ = "0.6.5"
 __package__ = "uun_weatherstation"
 library = "uun_iot"
 
 
 def main():
-    argp = argparse.ArgumentParser(prog=__package__, description='Connect to weatherlink'
-                                   'weatherstation and process informations and send to server.')
-    argp.add_argument('-v', '--version', action='version',
-                      version='%(prog) ' + __version__)
-    argp.add_argument('-l', '--log', metavar='loglevel', dest='loglevel', type=str,
-                      help='level of logging: [DEBUG, INFO, WARNING, ERROR, CRITICAL]', default='WARNING')
-    argp.add_argument('-c', '--config', metavar='configfile', dest='config', type=str,
-                      help="config file location, defaults to 'config.json'", default='config.json')
-
-    sys.excepthook = lambda exctype, value, tb: logging.getLogger(__package__).exception(
-        "Exception: ", exc_info=(exctype, value, tb))
+    argp = argparse.ArgumentParser(
+        prog=__package__,
+        description="Connect to weatherlink weatherstation and process informations and send to server.",
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
+        metavar="configfile",
+        dest="config",
+        type=str,
+        help="config file location, defaults to 'config.json'",
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
 
     args = argp.parse_args()
 
     if not os.path.exists(args.config):
         sys.exit(f"Could not find configuration file '{args.config}'")
 
     loglevel = args.loglevel
@@ -38,17 +61,16 @@
     if not isinstance(llevel, int):
         sys.exit(f"Invalid log level: {loglevel}")
 
     loggerw = logging.getLogger(__package__)  # application specific logger
     loggeru = logging.getLogger(library)  # library logger
     loggerw.setLevel(llevel)
     loggeru.setLevel(llevel)
-    handler = LoggingSystemdHandler()  # StreamHandler()
-    handler.setFormatter(logging.Formatter(
-        '%(name)s - %(levelname)s - %(message)s'))
+    handler = LoggingSystemdHandler() if args.systemd else logging.StreamHandler()
+    handler.setFormatter(logging.Formatter("%(name)s - %(levelname)s - %(message)s"))
     loggerw.addHandler(handler)
     loggeru.addHandler(handler)
 
     # start module system
     print("=== " + __package__ + " ===")
     with Gateway(args.config, init) as g:
         # Register a SIGTERM signal, as it is issued by systemd on stop/restart.
@@ -58,9 +80,9 @@
         signal.signal(signal.SIGTERM, g.signal_handler)
         signal.signal(signal.SIGINT, g.signal_handler)
         signal.signal(signal.SIGUSR1, g.signal_handler)
 
         g.stopev.wait()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `uun-weatherstation-0.6.4/setup.py` & `uun-weatherstation-0.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `uun-weatherstation-0.6.4/tests/test_data_processing.py` & `uun-weatherstation-0.6.5/tests/test_data_processing.py`

 * *Files identical despite different names*

### Comparing `uun-weatherstation-0.6.4/uun_weatherstation/data/sample-config.json` & `uun-weatherstation-0.6.5/uun_weatherstation/data/sample-config.json`

 * *Files identical despite different names*

### Comparing `uun-weatherstation-0.6.4/uun_weatherstation/modules/WeatherConditions.py` & `uun-weatherstation-0.6.5/uun_weatherstation/modules/WeatherConditions.py`

 * *Files identical despite different names*

### Comparing `uun-weatherstation-0.6.4/uun_weatherstation/modules/__init__.py` & `uun-weatherstation-0.6.5/uun_weatherstation/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `uun-weatherstation-0.6.4/uun_weatherstation.egg-info/SOURCES.txt` & `uun-weatherstation-0.6.5/uun_weatherstation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

