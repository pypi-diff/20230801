# Comparing `tmp/uun-iot-0.9.2.tar.gz` & `tmp/uun-iot-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uun-iot-0.9.2.tar", last modified: Tue Aug  1 12:01:08 2023, max compression
+gzip compressed data, was "uun-iot-0.9.3.tar", last modified: Tue Aug  1 14:30:03 2023, max compression
```

## Comparing `uun-iot-0.9.2.tar` & `uun-iot-0.9.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 12:01:08.193438 uun-iot-0.9.2/
--rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:43:51.000000 uun-iot-0.9.2/LICENSE.md
--rw-------   0 hello     (1000) hello     (1000)      468 2023-08-01 12:01:08.193438 uun-iot-0.9.2/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)     1965 2022-10-16 10:02:57.000000 uun-iot-0.9.2/README.md
--rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 12:01:08.193438 uun-iot-0.9.2/setup.cfg
--rw-------   0 hello     (1000) hello     (1000)      892 2023-01-22 14:43:43.000000 uun-iot-0.9.2/setup.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 12:01:08.193438 uun-iot-0.9.2/uun_iot/
--rw-------   0 hello     (1000) hello     (1000)    25084 2022-10-30 12:40:32.000000 uun-iot-0.9.2/uun_iot/Gateway.py
--rw-------   0 hello     (1000) hello     (1000)    20292 2023-08-01 11:59:34.000000 uun-iot-0.9.2/uun_iot/UuAppClient.py
--rw-------   0 hello     (1000) hello     (1000)      224 2023-08-01 12:00:39.000000 uun-iot-0.9.2/uun_iot/__init__.py
--rw-------   0 hello     (1000) hello     (1000)     9179 2023-08-01 07:17:17.000000 uun-iot-0.9.2/uun_iot/decorators.py
--rw-------   0 hello     (1000) hello     (1000)     1916 2022-10-16 10:02:57.000000 uun-iot-0.9.2/uun_iot/diagnostic.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 12:01:08.193438 uun-iot-0.9.2/uun_iot/modules/
--rw-------   0 hello     (1000) hello     (1000)    14058 2022-10-23 08:04:43.000000 uun-iot-0.9.2/uun_iot/modules/BaseHealthCheck.py
--rw-------   0 hello     (1000) hello     (1000)     2018 2022-10-16 10:02:57.000000 uun-iot-0.9.2/uun_iot/modules/Heartbeat.py
--rw-------   0 hello     (1000) hello     (1000)    10128 2022-10-31 07:37:38.000000 uun-iot-0.9.2/uun_iot/modules/Module.py
--rw-------   0 hello     (1000) hello     (1000)      362 2022-10-16 10:02:57.000000 uun-iot-0.9.2/uun_iot/modules/__init__.py
--rw-------   0 hello     (1000) hello     (1000)      367 2022-10-16 10:02:57.000000 uun-iot-0.9.2/uun_iot/typing.py
--rw-------   0 hello     (1000) hello     (1000)    12903 2023-08-01 09:53:25.000000 uun-iot-0.9.2/uun_iot/utils.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 12:01:08.193438 uun-iot-0.9.2/uun_iot.egg-info/
--rw-------   0 hello     (1000) hello     (1000)      468 2023-08-01 12:01:08.000000 uun-iot-0.9.2/uun_iot.egg-info/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)      442 2023-08-01 12:01:08.000000 uun-iot-0.9.2/uun_iot.egg-info/SOURCES.txt
--rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 12:01:08.000000 uun-iot-0.9.2/uun_iot.egg-info/dependency_links.txt
--rw-------   0 hello     (1000) hello     (1000)       56 2023-08-01 12:01:08.000000 uun-iot-0.9.2/uun_iot.egg-info/requires.txt
--rw-------   0 hello     (1000) hello     (1000)        8 2023-08-01 12:01:08.000000 uun-iot-0.9.2/uun_iot.egg-info/top_level.txt
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:30:03.936435 uun-iot-0.9.3/
+-rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:43:51.000000 uun-iot-0.9.3/LICENSE.md
+-rw-------   0 hello     (1000) hello     (1000)      468 2023-08-01 14:30:03.936435 uun-iot-0.9.3/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)     1965 2022-10-16 10:02:57.000000 uun-iot-0.9.3/README.md
+-rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 14:30:03.936435 uun-iot-0.9.3/setup.cfg
+-rw-------   0 hello     (1000) hello     (1000)      892 2023-01-22 14:43:43.000000 uun-iot-0.9.3/setup.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:30:03.936435 uun-iot-0.9.3/uun_iot/
+-rw-------   0 hello     (1000) hello     (1000)    25084 2022-10-30 12:40:32.000000 uun-iot-0.9.3/uun_iot/Gateway.py
+-rw-------   0 hello     (1000) hello     (1000)    20292 2023-08-01 11:59:34.000000 uun-iot-0.9.3/uun_iot/UuAppClient.py
+-rw-------   0 hello     (1000) hello     (1000)      224 2023-08-01 14:27:58.000000 uun-iot-0.9.3/uun_iot/__init__.py
+-rw-------   0 hello     (1000) hello     (1000)     9179 2023-08-01 07:17:17.000000 uun-iot-0.9.3/uun_iot/decorators.py
+-rw-------   0 hello     (1000) hello     (1000)     1916 2022-10-16 10:02:57.000000 uun-iot-0.9.3/uun_iot/diagnostic.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:30:03.936435 uun-iot-0.9.3/uun_iot/modules/
+-rw-------   0 hello     (1000) hello     (1000)    14058 2022-10-23 08:04:43.000000 uun-iot-0.9.3/uun_iot/modules/BaseHealthCheck.py
+-rw-------   0 hello     (1000) hello     (1000)     2018 2022-10-16 10:02:57.000000 uun-iot-0.9.3/uun_iot/modules/Heartbeat.py
+-rw-------   0 hello     (1000) hello     (1000)    10181 2023-08-01 14:03:32.000000 uun-iot-0.9.3/uun_iot/modules/Module.py
+-rw-------   0 hello     (1000) hello     (1000)      362 2022-10-16 10:02:57.000000 uun-iot-0.9.3/uun_iot/modules/__init__.py
+-rw-------   0 hello     (1000) hello     (1000)      367 2022-10-16 10:02:57.000000 uun-iot-0.9.3/uun_iot/typing.py
+-rw-------   0 hello     (1000) hello     (1000)    12903 2023-08-01 09:53:25.000000 uun-iot-0.9.3/uun_iot/utils.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:30:03.936435 uun-iot-0.9.3/uun_iot.egg-info/
+-rw-------   0 hello     (1000) hello     (1000)      468 2023-08-01 14:30:03.000000 uun-iot-0.9.3/uun_iot.egg-info/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)      442 2023-08-01 14:30:03.000000 uun-iot-0.9.3/uun_iot.egg-info/SOURCES.txt
+-rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 14:30:03.000000 uun-iot-0.9.3/uun_iot.egg-info/dependency_links.txt
+-rw-------   0 hello     (1000) hello     (1000)       56 2023-08-01 14:30:03.000000 uun-iot-0.9.3/uun_iot.egg-info/requires.txt
+-rw-------   0 hello     (1000) hello     (1000)        8 2023-08-01 14:30:03.000000 uun-iot-0.9.3/uun_iot.egg-info/top_level.txt
```

### Comparing `uun-iot-0.9.2/LICENSE.md` & `uun-iot-0.9.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.2/README.md` & `uun-iot-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.2/setup.py` & `uun-iot-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.2/uun_iot/Gateway.py` & `uun-iot-0.9.3/uun_iot/Gateway.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.2/uun_iot/UuAppClient.py` & `uun-iot-0.9.3/uun_iot/UuAppClient.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.2/uun_iot/decorators.py` & `uun-iot-0.9.3/uun_iot/decorators.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.2/uun_iot/diagnostic.py` & `uun-iot-0.9.3/uun_iot/diagnostic.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.2/uun_iot/modules/BaseHealthCheck.py` & `uun-iot-0.9.3/uun_iot/modules/BaseHealthCheck.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.2/uun_iot/modules/Heartbeat.py` & `uun-iot-0.9.3/uun_iot/modules/Heartbeat.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.2/uun_iot/modules/Module.py` & `uun-iot-0.9.3/uun_iot/modules/Module.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         Raises:
             KeyError: when a given key does not exist inside the configuration
         """
 
         mconf = self._config
 
         if key is None:
-            return mconf
+            return mconf[self.id] if scope == ConfigScopeEnum.SELF else mconf
 
         if scope == ConfigScopeEnum.SELF:
             key = self.id + "/" + key
 
         key_parts = key.split("/")
         for k in key_parts:
             try:
```

### Comparing `uun-iot-0.9.2/uun_iot/utils.py` & `uun-iot-0.9.3/uun_iot/utils.py`

 * *Files identical despite different names*

