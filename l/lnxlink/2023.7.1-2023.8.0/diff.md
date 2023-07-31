# Comparing `tmp/lnxlink-2023.7.1.tar.gz` & `tmp/lnxlink-2023.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnxlink-2023.7.1.tar", last modified: Thu Jul  6 19:18:09 2023, max compression
+gzip compressed data, was "lnxlink-2023.8.0.tar", last modified: Mon Jul 31 23:26:17 2023, max compression
```

## Comparing `lnxlink-2023.7.1.tar` & `lnxlink-2023.8.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:18:09.200178 lnxlink-2023.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-06 19:18:09.200178 lnxlink-2023.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:18:09.196179 lnxlink-2023.7.1/lnxlink/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15333 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5692 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:18:09.200178 lnxlink-2023.7.1/lnxlink/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/boot_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/camera_used.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/disk_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/idle.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/keep_alive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/microphone_used.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/notify.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/required_restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/screen_onoff.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/send_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/shutdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/suspend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/sys_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/webcam.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/modules/xdg_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/lnxlink/system_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:18:09.196179 lnxlink-2023.7.1/lnxlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-06 19:18:08.000000 lnxlink-2023.7.1/lnxlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-06 19:18:09.000000 lnxlink-2023.7.1/lnxlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:18:08.000000 lnxlink-2023.7.1/lnxlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-06 19:18:08.000000 lnxlink-2023.7.1/lnxlink.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-06 19:18:08.000000 lnxlink-2023.7.1/lnxlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 19:18:09.000000 lnxlink-2023.7.1/lnxlink.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1219 2023-07-06 19:17:57.000000 lnxlink-2023.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-06 19:18:09.200178 lnxlink-2023.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:26:17.295610 lnxlink-2023.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-31 23:26:17.295610 lnxlink-2023.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:26:17.291610 lnxlink-2023.8.0/lnxlink/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16247 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5824 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:26:17.295610 lnxlink-2023.8.0/lnxlink/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/boot_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/camera_used.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/disk_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/fullscreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/keep_alive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/microphone_used.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/notify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/required_restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/screen_onoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/send_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/suspend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/sys_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/webcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/modules/xdg_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/lnxlink/system_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:26:17.291610 lnxlink-2023.8.0/lnxlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-31 23:26:16.000000 lnxlink-2023.8.0/lnxlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-31 23:26:17.000000 lnxlink-2023.8.0/lnxlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 23:26:16.000000 lnxlink-2023.8.0/lnxlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-31 23:26:16.000000 lnxlink-2023.8.0/lnxlink.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-31 23:26:17.000000 lnxlink-2023.8.0/lnxlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 23:26:17.000000 lnxlink-2023.8.0/lnxlink.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1219 2023-07-31 23:26:02.000000 lnxlink-2023.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-31 23:26:17.295610 lnxlink-2023.8.0/setup.cfg
```

### Comparing `lnxlink-2023.7.1/LICENSE.md` & `lnxlink-2023.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.7.1/PKG-INFO` & `lnxlink-2023.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnxlink
-Version: 2023.7.1
+Version: 2023.8.0
 Summary: Internet Of Things (IOT) integration with Linux using MQTT
 Home-page: https://bkbilly.github.io/lnxlink
 Author-email: bkbilly <bkbilly@hotmail.com>
 Project-URL: Source Code, https://github.com/bkbilly/lnxlink
 Project-URL: Home Page, https://bkbilly.github.io/lnxlink
 Keywords: lnxlink
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lnxlink-2023.7.1/README.md` & `lnxlink-2023.8.0/README.md`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.7.1/lnxlink/__main__.py` & `lnxlink-2023.8.0/lnxlink/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 
 import os
 import yaml
 import time
 import json
 import distro
 import threading
-import traceback
+import logging
 import importlib.metadata
 import platform
 import argparse
 import paho.mqtt.client as mqtt
 from . import modules
 from . import config
 from .system_monitor import MonitorSuspend, GracefulKiller
 
 version = importlib.metadata.version(__package__ or __name__)
+logger = logging.getLogger('lnxlink')
 
 
 class LNXlink():
 
     def __init__(self, config_path):
-        print(f"LNXlink {version} started: {platform.python_version()}")
+
+        logger.info(f"LNXlink {version} started: {platform.python_version()}")
         self.kill = False
 
         # Read configuration from yaml file
         self.pref_topic = 'lnxlink'
         self.config = self.read_config(config_path)
 
         # Run each addon included in the modules folder
@@ -35,23 +37,22 @@
         conf_exclude = [] if conf_exclude is None else conf_exclude
         loaded_modules = modules.parse_modules(conf_modules, conf_exclude)
         for service, addon in loaded_modules.items():
             try:
                 tmp_addon = addon(self)
                 self.Addons[addon.service] = tmp_addon
             except Exception as e:
-                print(f"Error with addon {addon.service}, please remove it from your config")
-                traceback.print_exc()
+                logger.info(f"Error with addon {addon.service}, please remove it from your config: {e}")
 
         # Setup MQTT
         self.client = mqtt.Client()
         self.setup_mqtt()
 
     def publish_monitor_data(self, topic, pub_data):
-        # print(topic, pub_data, type(pub_data))
+        # logger.info(topic, pub_data, type(pub_data))
         if pub_data is None:
             return
         if isinstance(pub_data, bool):
             if pub_data is True:
                 pub_data = 'ON'
             if pub_data is False:
                 pub_data = 'OFF'
@@ -82,16 +83,15 @@
                         pub_data = addon.getInfo()
                         self.publish_monitor_data(topic, pub_data)
                     if hasattr(addon, 'getControlInfo'):
                         topic = f"{self.pref_topic}/monitor_controls/{subtopic}"
                         pub_data = addon.getControlInfo()
                         self.publish_monitor_data(topic, pub_data)
                 except Exception as e:
-                    print(f"Can't load addon: {service}")
-                    traceback.print_exc()
+                    logger.error(f"Error with addon {service}: {e}")
 
     def monitor_run_thread(self):
         '''Runs method to get sensor information every prespecified interval'''
         self.monitor_run()
 
         interval = self.config.get('update_interval', 1)
         if not self.kill:
@@ -122,15 +122,15 @@
             modules = [x.lower().replace('-', '_') for x in config['modules']]
         config['modules'] = modules
         return config
 
     def on_connect(self, client, userdata, flags, rc):
         '''Callback for MQTT connect which reports the connection status
         back to MQTT server'''
-        print(f"Connected to MQTT with code {rc}")
+        logger.info(f"Connected to MQTT with code {rc}")
         client.subscribe(f"{self.pref_topic}/commands/#")
         if self.config['mqtt']['lwt']['enabled']:
             self.client.publish(
                 f"{self.pref_topic}/lwt",
                 payload=self.config['mqtt']['lwt']['connectMsg'],
                 qos=self.config['mqtt']['lwt']['qos'],
                 retain=self.config['mqtt']['lwt']['retain']
@@ -138,74 +138,80 @@
         if self.config['mqtt']['discovery']['enabled']:
             self.setup_discovery()
         self.kill = False
         self.monitor_run_thread()
 
     def disconnect(self, *args):
         '''Reports to MQTT server that the service has stopped'''
-        print("Disconnected from MQTT.")
+        logger.info("Disconnected from MQTT.")
         if self.config['mqtt']['lwt']['enabled']:
             self.client.publish(
                 f"{self.pref_topic}/lwt",
                 payload=self.config['mqtt']['lwt']['disconnectMsg'],
                 qos=self.config['mqtt']['lwt']['qos'],
                 retain=self.config['mqtt']['lwt']['retain']
             )
         self.kill = True
         try:
             self.monitor.cancel()
         except Exception as e:
-            pass
+            logger.debug(e)
         self.client.disconnect()
 
     def temp_connection_callback(self, status):
         '''Report the connection status to MQTT server'''
         self.kill = True
         if self.config['mqtt']['lwt']['enabled']:
             if status:
-                print("Power Down detected.")
+                logger.info("Power Down detected.")
                 self.client.publish(
                     f"{self.pref_topic}/lwt",
                     payload=self.config['mqtt']['lwt']['disconnectMsg'],
                     qos=self.config['mqtt']['lwt']['qos'],
                     retain=self.config['mqtt']['lwt']['retain']
                 )
             else:
-                print("Power Up detected.")
+                logger.info("Power Up detected.")
                 if self.kill:
                     self.kill = False
                     self.monitor_run_thread()
                 self.client.publish(
                     f"{self.pref_topic}/lwt",
                     payload=self.config['mqtt']['lwt']['connectMsg'],
                     qos=self.config['mqtt']['lwt']['qos'],
                     retain=self.config['mqtt']['lwt']['retain']
                 )
 
     def on_message(self, client, userdata, msg):
         '''MQTT message is received with a module command to excecute'''
         topic = msg.topic.replace(f"{self.pref_topic}/commands/", "")
         message = msg.payload
-        print(f"Message received {topic}: {message}")
+        logger.info(f"Message received {topic}: {message}")
         try:
             message = json.loads(message)
         except Exception as e:
             message = message.decode()
-            # print("String could not be converted to JSON")
-            # traceback.print_exc()
+            logger.debug(f"String could not be converted to JSON: {e}")
 
         select_service = topic.split('/')
         addon = self.Addons.get(select_service[0])
         if addon is not None:
             if hasattr(addon, 'startControl'):
                 try:
-                    addon.startControl(select_service, message)
+                    result = addon.startControl(select_service, message)
+                    if result is not None:
+                        result_topic = f"{self.pref_topic}/command_result/{topic.strip('/')}"
+                        self.client.publish(
+                            result_topic,
+                            payload=result,
+                            retain=False
+                        )
                     self.monitor_run()
                 except Exception as e:
-                    traceback.print_exc()
+                    logger.error(e)
 
     def setup_discovery_monitoring(self, discovery_template, addon, service):
         '''Send discovery information on Home Assistant for sensors'''
         subtopic = addon.name.lower().replace(' ', '/')
         state_topic = f"{self.pref_topic}/{self.config['mqtt']['statsPrefix']}/{subtopic}"
 
         discovery = discovery_template.copy()
@@ -291,15 +297,15 @@
             discovery["max"] = options.get('max', 100)
             discovery["step"] = options.get('step', 1)
         elif options['type'] == 'select':
             discovery["command_topic"] = command_topic
             discovery["state_topic"] = state_topic
             discovery["options"] = addon.options
         else:
-            print("Not supported:", options['type'])
+            logger.info("Not supported:", options['type'])
             return
         self.client.publish(
             f"homeassistant/{options['type']}/lnxlink/{discovery['unique_id']}/config",
             payload=json.dumps(discovery),
             retain=self.config['mqtt']['lwt']['retain'])
 
     def setup_discovery(self):
@@ -320,35 +326,49 @@
         }
         for service, addon in self.Addons.items():
             addon = self.Addons[service]
             if hasattr(addon, 'getInfo'):
                 try:
                     self.setup_discovery_monitoring(discovery_template, addon, service)
                 except Exception as e:
-                    traceback.print_exc()
+                    logger.error(e)
             if hasattr(addon, 'exposedControls'):
                 for control_name, options in addon.exposedControls().items():
                     try:
                         self.setup_discovery_control(discovery_template, addon, service, control_name, options)
                     except Exception as e:
-                        traceback.print_exc()
+                        logger.error(e)
+
+
+def setup_logger(config_path):
+    config_dir = os.path.dirname(os.path.realpath(config_path))
+    print(config_dir)
+    logging.basicConfig(level=logging.INFO)
+    start_sec = str(int(time.time()))[-4:]
+    logFormatter = logging.Formatter("%(asctime)s [" + start_sec + ":%(threadName)s.%(module)s.%(funcName)s.%(lineno)d] [%(levelname)s]  %(message)s")
+    logger = logging.getLogger('lnxlink')
+
+    fileHandler = logging.FileHandler(f"{config_dir}/lnxlink.log")
+    fileHandler.setFormatter(logFormatter)
+    logger.addHandler(fileHandler)
 
 
 def main():
     parser = argparse.ArgumentParser(
         prog="LNXlink",
         description="Send system information to MQTT broker")
     parser.add_argument(
         "-c", "--config",
         help="Configuration file",
         default="/etc/config.yaml",
         required=True)
     args = parser.parse_args()
 
     config_file = os.path.abspath(args.config)
+    setup_logger(config_file)
     config.setup_config(config_file)
     config.setup_systemd(config_file)
     lnxlink = LNXlink(config_file)
 
     # Monitor for system changes (Shutdown/Suspend/Sleep)
     monitor_suspend = MonitorSuspend(lnxlink.temp_connection_callback)
     monitor_suspend.start()
```

### Comparing `lnxlink-2023.7.1/lnxlink/config.py` & `lnxlink-2023.8.0/lnxlink/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 #!/usr/bin/env python3
 
 import yaml
 import os
 import subprocess
+import logging
 import shutil
 from pathlib import Path
 from .consts import service_headless, service_user, config_temp
 
+logger = logging.getLogger('lnxlink')
+
 
 def setup_config(config_path):
     if not os.path.exists(config_path):
-        print("Config file not found.")
+        logger.info("Config file not found.")
 
         try:
             Path(config_path).parent.mkdir(parents=True, exist_ok=True)
             with open(config_path, 'wb') as config:
                 config.write(config_temp.encode())
-            print(f"Created new template: {config_path}")
+            logger.info(f"Created new template: {config_path}")
         except IOError:
-            print("Permision denied")
+            logger.info("Permision denied")
             return False
         userprompt_config(config_path)
     return True
 
 
 def query_true_false(question, default="false"):
     valid = {"true": True, "t": True, "yes": True, True: True, "false": False, "f": False, "no": False, False:False}
@@ -37,34 +40,34 @@
     while True:
         choice = input(f" {question} {prompt}: ").lower()
         if default is not None and choice == "":
             return valid[default]
         elif choice in valid:
             return valid[choice]
         else:
-            print("Please respond with 'true' or 'false' (or 't' or 'f').")
+            logger.info("Please respond with 'true' or 'false' (or 't' or 'f').")
 
 
 def userprompt_config(config_path):
     with open(config_path) as f:
         y = yaml.safe_load(f)
 
-        # Print config
-        print('This will update the MQTT credentials and topics, these are the default topics:')
-        print(" MQTT Topic prefix for for monitoring: {}/{}/{}/...".format(
+        # logger.info config
+        logger.info('This will update the MQTT credentials and topics, these are the default topics:')
+        logger.info(" MQTT Topic prefix for for monitoring: {}/{}/{}/...".format(
             y['mqtt']['prefix'],
             y['mqtt']['clientId'],
             y['mqtt']['statsPrefix']
         ))
-        print(" MQTT Topic prefix for for commands: {}/{}/commands/...".format(
+        logger.info(" MQTT Topic prefix for for commands: {}/{}/commands/...".format(
             y['mqtt']['prefix'],
             y['mqtt']['clientId']
         ))
 
-        print("\nLeave empty for default")
+        logger.info("\nLeave empty for default")
 
         # Change default values
         y['mqtt']['discovery']['enabled'] = query_true_false("Enable MQTT automatic discovery", y['mqtt']['discovery']['enabled'])
         y['mqtt']['server'] = input(f" MQTT server [{y['mqtt']['server']}]: ") or y['mqtt']['server']
         y['mqtt']['port'] = input(f" MQTT port [{y['mqtt']['port']}]: ") or y['mqtt']['port']
         y['mqtt']['port'] = int(y['mqtt']['port'])
         y['mqtt']['auth']['user'] = input(f" MQTT username [{y['mqtt']['auth']['user']}]: ") or y['mqtt']['auth']['user']
@@ -74,21 +77,21 @@
         y['mqtt']['clientId'] = input(f" Change clientId [{y['mqtt']['clientId']}]: ") or y['mqtt']['clientId']
         y['mqtt']['statsPrefix'] = input(f" Change statsPrefix [{y['mqtt']['statsPrefix']}]: ") or y['mqtt']['statsPrefix']
 
 
     with open(config_path, 'w') as fw:
         fw.write(yaml.dump(y, default_flow_style=False, sort_keys=False))
 
-    print('\nAll changes have been saved.')
-    print(" MQTT Topic prefix for for monitoring: {}/{}/{}/...".format(
+    logger.info('\nAll changes have been saved.')
+    logger.info(" MQTT Topic prefix for for monitoring: {}/{}/{}/...".format(
         y['mqtt']['prefix'],
         y['mqtt']['clientId'],
         y['mqtt']['statsPrefix']
     ))
-    print(" MQTT Topic prefix for for commands: {}/{}/commands/...".format(
+    logger.info(" MQTT Topic prefix for for commands: {}/{}/commands/...".format(
         y['mqtt']['prefix'],
         y['mqtt']['clientId']
     ))
 
 
 def get_service_user():
     installed_as = 0
@@ -123,15 +126,15 @@
 
 def setup_systemd(config_path):
     # Check how systemd is installed
     installed_as = get_service_user()
 
     if installed_as == 0:
         # Service not found or not running
-        print("SystemD service not found or it's not running...")
+        logger.info("SystemD service not found or it's not running...")
         user_service = query_true_false("Install as a user service?", True)
         sudo, cmd_user, systemd_service, service_location = get_service_vars(user_service)
 
         # Install on SystemD
         Path(service_location).mkdir(parents=True, exist_ok=True)
         exec_cmd = f"{shutil.which('lnxlink')} -c {config_path}"
         with open(f"{service_location}/lnxlink.service", 'wb') as config:
```

### Comparing `lnxlink-2023.7.1/lnxlink/consts.py` & `lnxlink-2023.8.0/lnxlink/consts.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.7.1/lnxlink/modules/__init__.py` & `lnxlink-2023.8.0/lnxlink/modules/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from importlib import import_module
 import time
-import traceback
+import logging
 import glob
 import os
 import sys
 
+logger = logging.getLogger('lnxlink')
+
 
 def autoload_modules(auto_exclude):
     modules = []
     modules_path = f"{os.path.dirname(__file__)}/*.py"
     for module_path in glob.glob(modules_path):
         module = os.path.basename(module_path)
         if '__' not in module and '.py' in module:
@@ -16,14 +18,15 @@
             if module not in auto_exclude:
                 modules.append(module)
 
     return modules
 
 
 def parse_modules(list_modules=None, auto_exclude=[]):
+    os.environ["DISPLAY"] = ':0'
     if list_modules is None:
         list_modules = autoload_modules(auto_exclude)
     modules = {}
     for module_name in list_modules:
         retries = 10
         while retries >= 0:
             try:
@@ -34,19 +37,16 @@
                     sys.path.append(module_path)
                     addon = getattr(import_module(f"{module_name}"), 'Addon')
                 else:
                     addon = getattr(import_module(f"{__name__}.{module_name}"), 'Addon')
                 addon.service = module_name
                 modules[module_name] = addon
                 retries = -1
-                print(f"Loaded addon: {module_name}")
             except ModuleNotFoundError as e:
-                print(f"Addon {module_name} is not supported, please remove it from your config")
-                print(e)
+                logger.error(f"Addon {module_name} is not supported, please remove it from your config: {e}")
                 retries = -1
             except Exception as e:
-                print("----------------")
-                print(f"Error with module: {module_name}")
-                traceback.print_exc()
+                logger.error(f"Error with module {module_name}: {e}")
                 time.sleep(2)
                 retries -= 1
+    logger.info(f"Loaded addons: {', '.join(modules)}")
     return modules
```

### Comparing `lnxlink-2023.7.1/lnxlink/modules/battery.py` & `lnxlink-2023.8.0/lnxlink/modules/battery.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.7.1/lnxlink/modules/boot_select.py` & `lnxlink-2023.8.0/lnxlink/modules/boot_select.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.7.1/lnxlink/modules/brightness.py` & `lnxlink-2023.8.0/lnxlink/modules/brightness.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import subprocess
 import re
+import logging
+
+logger = logging.getLogger('lnxlink')
 
 
 class Addon():
 
     def __init__(self, lnxlink=None):
         self.name = 'Brightness'
 
@@ -37,15 +40,15 @@
                     "min": 0.1,
                     "max": 1,
                     "step": 0.1,
                     "value_template": "{{ value_json." + json_display + " }}",
                     "enabled": False,
                 }
         except Exception as e:
-            print(e)
+            logger.error(e)
         return controls
 
     def startControl(self, topic, data):
         if topic[1] == 'Brightness':
             for display in self._get_displays().keys():
                 subprocess.call(f"xrandr --output {display} --brightness {data}", shell=True)
         else:
```

### Comparing `lnxlink-2023.7.1/lnxlink/modules/camera_used.py` & `lnxlink-2023.8.0/lnxlink/modules/camera_used.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.7.1/lnxlink/modules/disk_usage.py` & `lnxlink-2023.8.0/lnxlink/modules/disk_usage.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.7.1/lnxlink/modules/gpu.py` & `lnxlink-2023.8.0/lnxlink/modules/gpu.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import pyamdgpuinfo
 import nvsmi
+from shutil import which
 
 
 class Addon():
 
     def __init__(self, lnxlink):
         self.name = 'GPU'
         self.gpu_ids = {
-            "nvidia": len(list(nvsmi.get_gpus())),
-            "amd": pyamdgpuinfo.detect_gpus(),
+            "amd": pyamdgpuinfo.detect_gpus()
         }
+        if which("nvidia-smi") is not None:
+            self.gpu_ids["nvidia"] = len(list(nvsmi.get_gpus()))
+        else:
+            self.gpu_ids["nvidia"] = 0
 
     def getControlInfo(self):
         gpus = {}
         for gpu_id in range(self.gpu_ids['amd']):
             amd_gpu = pyamdgpuinfo.get_gpu(gpu_id)
             gpus[f"amd_{gpu_id}"] = {
                 "name": amd_gpu.name,
```

### Comparing `lnxlink-2023.7.1/lnxlink/modules/idle.py` & `lnxlink-2023.8.0/lnxlink/modules/idle.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.7.1/lnxlink/modules/media.py` & `lnxlink-2023.8.0/lnxlink/modules/media.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.7.1/lnxlink/modules/memory.py` & `lnxlink-2023.8.0/lnxlink/modules/memory.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.7.1/lnxlink/modules/microphone_used.py` & `lnxlink-2023.8.0/lnxlink/modules/microphone_used.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.7.1/lnxlink/modules/network.py` & `lnxlink-2023.8.0/lnxlink/modules/network.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.7.1/lnxlink/modules/notify.py` & `lnxlink-2023.8.0/lnxlink/modules/notify.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.7.1/lnxlink/modules/screen_onoff.py` & `lnxlink-2023.8.0/lnxlink/modules/screen_onoff.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.7.1/lnxlink/modules/screenshot.py` & `lnxlink-2023.8.0/lnxlink/modules/screenshot.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.7.1/lnxlink/modules/sys_updates.py` & `lnxlink-2023.8.0/lnxlink/modules/sys_updates.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.7.1/lnxlink/modules/update.py` & `lnxlink-2023.8.0/lnxlink/modules/update.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import importlib.metadata
 import time
 import requests
-import traceback
+import logging
+
+logger = logging.getLogger('lnxlink')
 
 
 class Addon():
 
     def __init__(self, lnxlink):
         self.name = 'LNXlink'
         self.last_time = 0
@@ -41,9 +43,9 @@
     def _latest_version(self):
         url = "https://api.github.com/repos/bkbilly/lnxlink/releases/latest"
         try:
             resp = requests.get(url=url).json()
             self.message['latest_version'] = resp['tag_name']
             self.message['release_summary'] = resp['body']
             self.message['release_url'] = resp['html_url']
-        except:
-            traceback.print_exc()
+        except Exception as e:
+            logger.error(e)
```

### Comparing `lnxlink-2023.7.1/lnxlink/modules/webcam.py` & `lnxlink-2023.8.0/lnxlink/modules/webcam.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.7.1/lnxlink/system_monitor.py` & `lnxlink-2023.8.0/lnxlink/system_monitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 #!/usr/bin/env python3
 
 import threading
 import signal
 import dbus
+import logging
 from dbus.mainloop.glib import DBusGMainLoop
 import pgi
 pgi.install_as_gi()
 from gi.repository import GLib
 
+logger = logging.getLogger('lnxlink')
+
 
 class MonitorSuspend():
     """Monitor DBUS for Suspend and Shutdown events"""
 
     def __init__(self, callback):
         dbus_loop = DBusGMainLoop(set_as_default=True)  # integrate into main loob
         bus = dbus.SystemBus(mainloop=dbus_loop)        # connect to dbus system wide
@@ -44,10 +47,10 @@
     def __init__(self, callback):
         self.kill_now = False
         self.callback = callback
         signal.signal(signal.SIGINT, self.exit_gracefully)
         signal.signal(signal.SIGTERM, self.exit_gracefully)
 
     def exit_gracefully(self, signum, frame):
-        print("stopped gracefully")
+        logger.info("stopped gracefully")
         self.callback(1)
         self.kill_now = True
```

### Comparing `lnxlink-2023.7.1/lnxlink.egg-info/PKG-INFO` & `lnxlink-2023.8.0/lnxlink.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnxlink
-Version: 2023.7.1
+Version: 2023.8.0
 Summary: Internet Of Things (IOT) integration with Linux using MQTT
 Home-page: https://bkbilly.github.io/lnxlink
 Author-email: bkbilly <bkbilly@hotmail.com>
 Project-URL: Source Code, https://github.com/bkbilly/lnxlink
 Project-URL: Home Page, https://bkbilly.github.io/lnxlink
 Keywords: lnxlink
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lnxlink-2023.7.1/lnxlink.egg-info/SOURCES.txt` & `lnxlink-2023.8.0/lnxlink.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 lnxlink/modules/bash.py
 lnxlink/modules/battery.py
 lnxlink/modules/boot_select.py
 lnxlink/modules/brightness.py
 lnxlink/modules/camera_used.py
 lnxlink/modules/cpu.py
 lnxlink/modules/disk_usage.py
+lnxlink/modules/fullscreen.py
 lnxlink/modules/gpu.py
 lnxlink/modules/idle.py
 lnxlink/modules/keep_alive.py
 lnxlink/modules/media.py
 lnxlink/modules/memory.py
 lnxlink/modules/microphone_used.py
 lnxlink/modules/network.py
```

### Comparing `lnxlink-2023.7.1/pyproject.toml` & `lnxlink-2023.8.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name              = "lnxlink"
-version           = "2023.7.1"
+version           = "2023.8.0"
 description       = "Internet Of Things (IOT) integration with Linux using MQTT"
 readme            = "README.md"
 keywords          = ["lnxlink"]
 requires-python   = ">=3.7.0"
 authors     = [
     {name="bkbilly", email="bkbilly@hotmail.com"}
 ]
```

