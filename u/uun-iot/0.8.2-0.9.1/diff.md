# Comparing `tmp/uun-iot-0.8.2.tar.gz` & `tmp/uun-iot-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uun-iot-0.8.2.tar", last modified: Thu Jan 26 11:23:57 2023, max compression
+gzip compressed data, was "uun-iot-0.9.1.tar", last modified: Tue Aug  1 11:28:04 2023, max compression
```

## Comparing `uun-iot-0.8.2.tar` & `uun-iot-0.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:23:57.255040 uun-iot-0.8.2/
--rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:43:51.000000 uun-iot-0.8.2/LICENSE.md
--rw-------   0 hello     (1000) hello     (1000)      468 2023-01-26 11:23:57.255040 uun-iot-0.8.2/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)     1965 2022-10-16 10:02:57.000000 uun-iot-0.8.2/README.md
--rw-------   0 hello     (1000) hello     (1000)       38 2023-01-26 11:23:57.255040 uun-iot-0.8.2/setup.cfg
--rw-------   0 hello     (1000) hello     (1000)      892 2023-01-22 14:43:43.000000 uun-iot-0.8.2/setup.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:23:57.251706 uun-iot-0.8.2/uun_iot/
--rw-------   0 hello     (1000) hello     (1000)    25084 2022-10-30 12:40:32.000000 uun-iot-0.8.2/uun_iot/Gateway.py
--rw-------   0 hello     (1000) hello     (1000)    12024 2022-10-16 10:02:57.000000 uun-iot-0.8.2/uun_iot/UuAppClient.py
--rw-------   0 hello     (1000) hello     (1000)      224 2023-01-22 14:49:07.000000 uun-iot-0.8.2/uun_iot/__init__.py
--rw-------   0 hello     (1000) hello     (1000)     9179 2022-10-16 10:02:57.000000 uun-iot-0.8.2/uun_iot/decorators.py
--rw-------   0 hello     (1000) hello     (1000)     1916 2022-10-16 10:02:57.000000 uun-iot-0.8.2/uun_iot/diagnostic.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:23:57.255040 uun-iot-0.8.2/uun_iot/modules/
--rw-------   0 hello     (1000) hello     (1000)    14058 2022-10-23 08:04:43.000000 uun-iot-0.8.2/uun_iot/modules/BaseHealthCheck.py
--rw-------   0 hello     (1000) hello     (1000)     2018 2022-10-16 10:02:57.000000 uun-iot-0.8.2/uun_iot/modules/Heartbeat.py
--rw-------   0 hello     (1000) hello     (1000)    10128 2022-10-31 07:37:38.000000 uun-iot-0.8.2/uun_iot/modules/Module.py
--rw-------   0 hello     (1000) hello     (1000)      362 2022-10-16 10:02:57.000000 uun-iot-0.8.2/uun_iot/modules/__init__.py
--rw-------   0 hello     (1000) hello     (1000)      367 2022-10-16 10:02:57.000000 uun-iot-0.8.2/uun_iot/typing.py
--rw-------   0 hello     (1000) hello     (1000)    12191 2022-10-30 22:10:23.000000 uun-iot-0.8.2/uun_iot/utils.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-01-26 11:23:57.251706 uun-iot-0.8.2/uun_iot.egg-info/
--rw-------   0 hello     (1000) hello     (1000)      468 2023-01-26 11:23:57.000000 uun-iot-0.8.2/uun_iot.egg-info/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)      442 2023-01-26 11:23:57.000000 uun-iot-0.8.2/uun_iot.egg-info/SOURCES.txt
--rw-------   0 hello     (1000) hello     (1000)        1 2023-01-26 11:23:57.000000 uun-iot-0.8.2/uun_iot.egg-info/dependency_links.txt
--rw-------   0 hello     (1000) hello     (1000)       56 2023-01-26 11:23:57.000000 uun-iot-0.8.2/uun_iot.egg-info/requires.txt
--rw-------   0 hello     (1000) hello     (1000)        8 2023-01-26 11:23:57.000000 uun-iot-0.8.2/uun_iot.egg-info/top_level.txt
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:04.861788 uun-iot-0.9.1/
+-rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:43:51.000000 uun-iot-0.9.1/LICENSE.md
+-rw-------   0 hello     (1000) hello     (1000)      468 2023-08-01 11:28:04.861788 uun-iot-0.9.1/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)     1965 2022-10-16 10:02:57.000000 uun-iot-0.9.1/README.md
+-rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 11:28:04.861788 uun-iot-0.9.1/setup.cfg
+-rw-------   0 hello     (1000) hello     (1000)      892 2023-01-22 14:43:43.000000 uun-iot-0.9.1/setup.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:04.861788 uun-iot-0.9.1/uun_iot/
+-rw-------   0 hello     (1000) hello     (1000)    25084 2022-10-30 12:40:32.000000 uun-iot-0.9.1/uun_iot/Gateway.py
+-rw-------   0 hello     (1000) hello     (1000)    20253 2023-06-24 09:53:33.000000 uun-iot-0.9.1/uun_iot/UuAppClient.py
+-rw-------   0 hello     (1000) hello     (1000)      224 2023-08-01 10:00:52.000000 uun-iot-0.9.1/uun_iot/__init__.py
+-rw-------   0 hello     (1000) hello     (1000)     9179 2023-08-01 07:17:17.000000 uun-iot-0.9.1/uun_iot/decorators.py
+-rw-------   0 hello     (1000) hello     (1000)     1916 2022-10-16 10:02:57.000000 uun-iot-0.9.1/uun_iot/diagnostic.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:04.861788 uun-iot-0.9.1/uun_iot/modules/
+-rw-------   0 hello     (1000) hello     (1000)    14058 2022-10-23 08:04:43.000000 uun-iot-0.9.1/uun_iot/modules/BaseHealthCheck.py
+-rw-------   0 hello     (1000) hello     (1000)     2018 2022-10-16 10:02:57.000000 uun-iot-0.9.1/uun_iot/modules/Heartbeat.py
+-rw-------   0 hello     (1000) hello     (1000)    10128 2022-10-31 07:37:38.000000 uun-iot-0.9.1/uun_iot/modules/Module.py
+-rw-------   0 hello     (1000) hello     (1000)      362 2022-10-16 10:02:57.000000 uun-iot-0.9.1/uun_iot/modules/__init__.py
+-rw-------   0 hello     (1000) hello     (1000)      367 2022-10-16 10:02:57.000000 uun-iot-0.9.1/uun_iot/typing.py
+-rw-------   0 hello     (1000) hello     (1000)    12903 2023-08-01 09:53:25.000000 uun-iot-0.9.1/uun_iot/utils.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 11:28:04.861788 uun-iot-0.9.1/uun_iot.egg-info/
+-rw-------   0 hello     (1000) hello     (1000)      468 2023-08-01 11:28:04.000000 uun-iot-0.9.1/uun_iot.egg-info/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)      442 2023-08-01 11:28:04.000000 uun-iot-0.9.1/uun_iot.egg-info/SOURCES.txt
+-rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 11:28:04.000000 uun-iot-0.9.1/uun_iot.egg-info/dependency_links.txt
+-rw-------   0 hello     (1000) hello     (1000)       56 2023-08-01 11:28:04.000000 uun-iot-0.9.1/uun_iot.egg-info/requires.txt
+-rw-------   0 hello     (1000) hello     (1000)        8 2023-08-01 11:28:04.000000 uun-iot-0.9.1/uun_iot.egg-info/top_level.txt
```

### Comparing `uun-iot-0.8.2/LICENSE.md` & `uun-iot-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uun-iot-0.8.2/README.md` & `uun-iot-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `uun-iot-0.8.2/setup.py` & `uun-iot-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.8.2/uun_iot/Gateway.py` & `uun-iot-0.9.1/uun_iot/Gateway.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.8.2/uun_iot/decorators.py` & `uun-iot-0.9.1/uun_iot/decorators.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.8.2/uun_iot/diagnostic.py` & `uun-iot-0.9.1/uun_iot/diagnostic.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.8.2/uun_iot/modules/BaseHealthCheck.py` & `uun-iot-0.9.1/uun_iot/modules/BaseHealthCheck.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.8.2/uun_iot/modules/Heartbeat.py` & `uun-iot-0.9.1/uun_iot/modules/Heartbeat.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.8.2/uun_iot/modules/Module.py` & `uun-iot-0.9.1/uun_iot/modules/Module.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.8.2/uun_iot/utils.py` & `uun-iot-0.9.1/uun_iot/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,14 +80,35 @@
         iso_timestamp: ISO timestamp
 
     Returns:
         datetime: corresponding :class:`datetime.datetime` object
     """
     return datetime.strptime(iso_timestamp, '%a, %d %b %Y %H:%M:%S %Z')
 
+class LoggingSystemdHandler(logging.StreamHandler):
+    """ Severity information for stdout&stderr logging. See SD-DAEMON(3) """
+    PREFIX = {
+        # EMERG <0>
+        # ALERT <1>
+        logging.CRITICAL: "<2>",
+        logging.ERROR: "<3>",
+        logging.WARNING: "<4>",
+        # NOTICE <5>
+        logging.INFO: "<6>",
+        logging.DEBUG: "<7>",
+        logging.NOTSET: "<7>"
+    }
+    def emit(self, record):
+        try:
+            msg = self.PREFIX[record.levelno] + self.format(record)
+            msg = msg.replace("\n", "\\n") # Tracebacks on single line
+            self.stream.write(msg + "\n")
+            self.stream.flush()
+        except Exception:
+            self.handleError(record)
 
 logger_rt = logging.getLogger(__name__ + ".RepeatTimer")
 class RepeatTimer:
     """ Periodically run function with unlimited repetition.
 
     Start the timer by executing :meth:`.start`. The timer can be interrupted
     at any time by issuing :meth:`.stop`.
```

