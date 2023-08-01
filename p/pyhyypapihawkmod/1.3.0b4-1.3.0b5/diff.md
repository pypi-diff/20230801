# Comparing `tmp/pyhyypapihawkmod-1.3.0b4.tar.gz` & `tmp/pyhyypapihawkmod-1.3.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.3.0b4.tar", last modified: Mon Jul 31 07:33:04 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.3.0b5.tar", last modified: Tue Aug  1 14:43:44 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.3.0b4.tar` & `pyhyypapihawkmod-1.3.0b5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 07:33:04.959539 pyhyypapihawkmod-1.3.0b4/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b4/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b4/MANIFEST.in
--rw-rw-rw-   0        0        0      519 2023-07-31 07:33:04.958027 pyhyypapihawkmod-1.3.0b4/PKG-INFO
--rw-rw-rw-   0        0        0     3250 2023-07-31 07:29:05.000000 pyhyypapihawkmod-1.3.0b4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 07:33:04.941525 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      410 2023-07-30 15:49:06.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      162 2023-07-30 07:50:36.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0    12324 2023-07-30 07:42:04.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    32743 2023-07-31 07:26:33.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4114 2023-07-30 16:00:32.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     1999 2023-07-30 15:55:41.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/imei.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    17749 2023-07-30 16:15:07.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:33:04.955531 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      519 2023-07-31 07:33:04.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      576 2023-07-31 07:33:04.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 07:33:04.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-31 07:33:04.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-31 07:33:04.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 07:33:04.960037 pyhyypapihawkmod-1.3.0b4/setup.cfg
--rw-rw-rw-   0        0        0      923 2023-07-31 07:26:36.000000 pyhyypapihawkmod-1.3.0b4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:43:44.618865 pyhyypapihawkmod-1.3.0b5/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b5/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b5/MANIFEST.in
+-rw-rw-rw-   0        0        0      519 2023-08-01 14:43:44.617852 pyhyypapihawkmod-1.3.0b5/PKG-INFO
+-rw-rw-rw-   0        0        0     3293 2023-08-01 14:39:14.000000 pyhyypapihawkmod-1.3.0b5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 14:43:44.603356 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      410 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      162 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0    12602 2023-08-01 13:37:39.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    32743 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4114 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     1999 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/imei.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    18507 2023-08-01 14:37:39.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:43:44.615855 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-08-01 14:43:44.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      576 2023-08-01 14:43:44.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 14:43:44.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-08-01 14:43:44.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-01 14:43:44.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 14:43:44.618865 pyhyypapihawkmod-1.3.0b5/setup.cfg
+-rw-rw-rw-   0        0        0      923 2023-08-01 14:39:23.000000 pyhyypapihawkmod-1.3.0b5/setup.py
```

### Comparing `pyhyypapihawkmod-1.3.0b4/LICENSE.md` & `pyhyypapihawkmod-1.3.0b5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b4/PKG-INFO` & `pyhyypapihawkmod-1.3.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.3.0b4
+Version: 1.3.0b5
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.3.0b4/README.md` & `pyhyypapihawkmod-1.3.0b5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,17 @@
 
 ```
 print(json.dumps(client.get_sync_info(),indent=2))
 
 ```
 
 Changelog 
+1.3.0b5
+- Added reconnect for timeouts
+
 1.3.0b4
 - Minor Refactoring
 
 1.3.0b3
 - Hotfix, notifications appear to go to random people. Implemented random IMEI
 
 1.3.0b2
```

### Comparing `pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/alarm_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -268,19 +268,25 @@
         
             _LOGGER.setLevel(logging.DEBUG)
             time.sleep(1.5)
             syncinfo = self._client.get_sync_info()
             time.sleep(1)
             stateinfo = self._client.get_state_info()
             time.sleep(2)
-            site = syncinfo["sites"][0]["id"]
-            time.sleep(2)
-            notificationinfo = self._client.site_notifications(site_id=site)
-            time.sleep(2)
-            zoneinfo = self._client.get_zone_state_info(site_id=site)
+            notificationinfo = {}
+            zoneinfo = {}
+            for site in syncinfo["sites"]:  
+                siteid = site["id"]
+                time.sleep(2)
+                cur_site_notificationinfo = self._client.site_notifications(site_id=siteid)
+                notificationinfo[siteid] = cur_site_notificationinfo
+                time.sleep(2)
+                cur_site_zoneinfo = self._client.get_zone_state_info(site_id=siteid)
+                zoneinfo[siteid] = cur_site_zoneinfo
+                
             
             message = {"client_string" : DEBUG_CLIENT_STRING["client_string"],
                        "syncinfo" : syncinfo,
                        "Stateinfo" : stateinfo,
                        "notifications" : notificationinfo,
                        "zoneinfo" : zoneinfo,
                        }
```

### Comparing `pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/imei.py` & `pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/imei.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/push_receiver.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import socket
 import ssl
 import struct
 import time
 from urllib.parse import urlencode
 from urllib.request import Request, urlopen
 import uuid
+import threading as thread
 
 import appdirs
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from google.protobuf.json_format import MessageToDict
 import http_ece
 from oscrypto.asymmetric import generate_pair
@@ -48,14 +49,16 @@
 REGISTER_URL = "https://android.clients.google.com/c2dm/register3"
 CHECKIN_URL = "https://android.clients.google.com/checkin"
 FCM_SUBSCRIBE = "https://fcm.googleapis.com/fcm/connect/subscribe"
 FCM_ENDPOINT = "https://fcm.googleapis.com/fcm/send"
 GOOGLE_MTALK_ENDPOINT = "mtalk.google.com"
 READ_TIMEOUT_SECS = 60 * 60
 MIN_RESET_INTERVAL_SECS = 60 * 5
+MAX_SILENT_INTERVAL_SECS = 60 * 60
+STATUS_TIMEOUT = 1
 
 MCS_VERSION = 41
 PACKET_BY_TAG = [
     HeartbeatPing,
     HeartbeatAck,
     LoginRequest,
     LoginResponse,
@@ -246,14 +249,16 @@
 
     
     def __init__(
         self,
     ) -> None:
         self.fcm_registration = FCMRegistration()
         self.received_persistent_ids = []
+        self.time_last_message_received = time.time()
+        self.time_of_last_reset = 0
 
 
     def __read(self, sock, size):
         buf = b""
         while len(buf) < size:
             buf += sock.recv(size - len(buf))
         return buf
@@ -328,14 +333,15 @@
             if version < MCS_VERSION and version != 38:
                 raise RuntimeError("protocol version {} unsupported".format(version))
         else:
             (tag,) = struct.unpack("B", self.__read(data, 1))
         _LOGGER.debug("tag %s (%s)", tag, PACKET_BY_TAG[tag])
         size = self.__read_varint32(data)
         _LOGGER.debug("size %s", size)
+        self.time_last_message_received = time.time()
         if size >= 0:
             buf = self.__read(data, size)
             _LOGGER.debug(hexlify(buf))
             packet = PACKET_BY_TAG[tag]
             payload = packet()
             payload.ParseFromString(buf)
             _LOGGER.debug(payload)
@@ -383,31 +389,37 @@
         self.__send(google_socket, req)
         login_response = self.__recv(google_socket, first=True)
         _LOGGER.debug("Received login response: %s", login_response)
         return google_socket
 
 
     def __reset(self, google_socket, credentials, persistent_ids):
-        last_reset = 0
         now = time.time()
-        if now - last_reset < MIN_RESET_INTERVAL_SECS:
+        if now - self.time_of_last_reset < MIN_RESET_INTERVAL_SECS:
             raise Exception("Too many connection reset attempts.")
-        last_reset = now
+        self.time_of_last_reset = now
         _LOGGER.debug("Reestablishing connection")
         try:
             google_socket.shutdown(2)
             google_socket.close()
         except OSError as err:
             _LOGGER.debug("Unable to close connection %f", err)
         return self.__login(credentials, persistent_ids)
 
+    def __status_check(self):
+        time_since_last_message = time.time() - self.time_last_message_received
+        if (time_since_last_message > MAX_SILENT_INTERVAL_SECS):
+            _LOGGER.info(f'No communications received in {time_since_last_message}s.  Resetting connection.')
+            return STATUS_TIMEOUT
+        return None
+
+
 
     def __listen(self, credentials, callback, persistent_ids, obj):
         google_socket = self.__login(credentials, persistent_ids)
-
         while True:
             try:
                 data = self.__recv(google_socket)
                 if isinstance(data, DataMessageStanza):
                     msg_id = self.__handle_data_message(data, credentials, callback, obj)
                     persistent_ids.append(msg_id)
                 elif isinstance(data, HeartbeatPing):
@@ -415,14 +427,18 @@
                 elif data is None or isinstance(data, Close):
                     google_socket = self.__reset(google_socket, credentials, persistent_ids)
                 else:
                     _LOGGER.debug("Unexpected message type %s", type(data))
             except ConnectionResetError:
                 _LOGGER.debug("Connection Reset: Reconnecting")
                 google_socket = self.__login(credentials, persistent_ids)
+            if self.__status_check() == STATUS_TIMEOUT:
+                google_socket = self.__reset(google_socket, credentials, persistent_ids)
+           
+                
 
 
     def __handle_data_message(self, data, credentials, callback, obj):
         load_der_private_key = serialization.load_der_private_key
 
         crypto_key = self.__app_data_by_key(
             data, "crypto-key", blow_shit_up=False
```

### Comparing `pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.3.0b4
+Version: 1.3.0b5
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b4/setup.py` & `pyhyypapihawkmod-1.3.0b5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.3.0b4",
+    version="1.3.0b5",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

