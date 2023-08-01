# Comparing `tmp/aiocomfoconnect-0.1.7.tar.gz` & `tmp/aiocomfoconnect-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocomfoconnect-0.1.7.tar", max compression
+gzip compressed data, was "aiocomfoconnect-0.1.8.tar", max compression
```

## Comparing `aiocomfoconnect-0.1.7.tar` & `aiocomfoconnect-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1133 2022-11-14 19:35:15.185394 aiocomfoconnect-0.1.7/LICENSE
--rw-r--r--   0        0        0     5973 2023-07-31 14:37:20.656155 aiocomfoconnect-0.1.7/README.md
--rw-r--r--   0        0        0      263 2022-12-16 20:50:33.736818 aiocomfoconnect-0.1.7/aiocomfoconnect/__init__.py
--rw-r--r--   0        0        0    10734 2023-07-31 14:37:20.656155 aiocomfoconnect-0.1.7/aiocomfoconnect/__main__.py
--rw-r--r--   0        0        0    20942 2023-07-31 13:34:19.888514 aiocomfoconnect-0.1.7/aiocomfoconnect/bridge.py
--rw-r--r--   0        0        0    19319 2023-04-06 04:27:11.595081 aiocomfoconnect-0.1.7/aiocomfoconnect/comfoconnect.py
--rw-r--r--   0        0        0     9341 2022-12-16 20:52:49.305149 aiocomfoconnect-0.1.7/aiocomfoconnect/const.py
--rw-r--r--   0        0        0     2796 2022-12-16 20:52:49.294316 aiocomfoconnect-0.1.7/aiocomfoconnect/discovery.py
--rw-r--r--   0        0        0     1297 2023-04-11 07:07:54.292758 aiocomfoconnect-0.1.7/aiocomfoconnect/exceptions.py
--rw-r--r--   0        0        0     1193 2023-07-31 14:37:20.656155 aiocomfoconnect-0.1.7/aiocomfoconnect/properties.py
--rw-r--r--   0        0        0     2776 2022-12-16 19:59:11.317713 aiocomfoconnect-0.1.7/aiocomfoconnect/protobuf/nanopb_pb2.py
--rw-r--r--   0        0        0    29853 2022-11-08 09:06:10.920864 aiocomfoconnect-0.1.7/aiocomfoconnect/protobuf/zehnder_pb2.py
--rw-r--r--   0        0        0     9977 2023-04-06 04:55:14.628771 aiocomfoconnect-0.1.7/aiocomfoconnect/sensors.py
--rw-r--r--   0        0        0     1203 2022-12-16 19:25:07.186887 aiocomfoconnect-0.1.7/aiocomfoconnect/util.py
--rw-r--r--   0        0        0     2395 2023-07-31 14:37:34.414486 aiocomfoconnect-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     6729 1970-01-01 00:00:00.000000 aiocomfoconnect-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1133 2022-11-14 19:35:15.185394 aiocomfoconnect-0.1.8/LICENSE
+-rw-r--r--   0        0        0     6041 2023-08-01 09:43:05.497255 aiocomfoconnect-0.1.8/README.md
+-rw-r--r--   0        0        0      263 2022-12-16 20:50:33.736818 aiocomfoconnect-0.1.8/aiocomfoconnect/__init__.py
+-rw-r--r--   0        0        0    11086 2023-08-01 09:43:05.497255 aiocomfoconnect-0.1.8/aiocomfoconnect/__main__.py
+-rw-r--r--   0        0        0    20942 2023-07-31 13:34:19.888514 aiocomfoconnect-0.1.8/aiocomfoconnect/bridge.py
+-rw-r--r--   0        0        0    19319 2023-04-06 04:27:11.595081 aiocomfoconnect-0.1.8/aiocomfoconnect/comfoconnect.py
+-rw-r--r--   0        0        0     9341 2022-12-16 20:52:49.305149 aiocomfoconnect-0.1.8/aiocomfoconnect/const.py
+-rw-r--r--   0        0        0     2796 2022-12-16 20:52:49.294316 aiocomfoconnect-0.1.8/aiocomfoconnect/discovery.py
+-rw-r--r--   0        0        0     1297 2023-04-11 07:07:54.292758 aiocomfoconnect-0.1.8/aiocomfoconnect/exceptions.py
+-rw-r--r--   0        0        0     1193 2023-07-31 14:37:20.656155 aiocomfoconnect-0.1.8/aiocomfoconnect/properties.py
+-rw-r--r--   0        0        0     2776 2022-12-16 19:59:11.317713 aiocomfoconnect-0.1.8/aiocomfoconnect/protobuf/nanopb_pb2.py
+-rw-r--r--   0        0        0    29853 2022-11-08 09:06:10.920864 aiocomfoconnect-0.1.8/aiocomfoconnect/protobuf/zehnder_pb2.py
+-rw-r--r--   0        0        0    10197 2023-08-01 09:43:05.497255 aiocomfoconnect-0.1.8/aiocomfoconnect/sensors.py
+-rw-r--r--   0        0        0     3375 2023-08-01 09:43:05.497255 aiocomfoconnect-0.1.8/aiocomfoconnect/util.py
+-rw-r--r--   0        0        0     2395 2023-08-01 09:43:28.998138 aiocomfoconnect-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     6797 1970-01-01 00:00:00.000000 aiocomfoconnect-0.1.8/PKG-INFO
```

### Comparing `aiocomfoconnect-0.1.7/LICENSE` & `aiocomfoconnect-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.7/README.md` & `aiocomfoconnect-0.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 $ python -m aiocomfoconnect set-speed low --host 192.168.1.213
 $ python -m aiocomfoconnect set-mode auto --host 192.168.1.213
 $ python -m aiocomfoconnect set-speed medium --host 192.168.1.213
 $ python -m aiocomfoconnect set-speed high --host 192.168.1.213
 
 $ python -m aiocomfoconnect show-sensors --host 192.168.1.213
 $ python -m aiocomfoconnect show-sensor 276 --host 192.168.1.213
+$ python -m aiocomfoconnect show-sensor 276 --host 192.168.1.213 -f
 
 $ python -m aiocomfoconnect get-property --host 192.168.1.213 1 1 8 9  # Unit 0x01, SubUnit 0x01, Property 0x08, Type STRING. See PROTOCOL-RMI.md
 ```
 
 ## Available methods
 
 - `async connect()`: Connect to the bridge.
```

### Comparing `aiocomfoconnect-0.1.7/aiocomfoconnect/__main__.py` & `aiocomfoconnect-0.1.8/aiocomfoconnect/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     elif args.action == "set-mode":
         await run_set_mode(args.host, args.uuid, args.mode)
 
     elif args.action == "show-sensors":
         await run_show_sensors(args.host, args.uuid)
 
     elif args.action == "show-sensor":
-        await run_show_sensor(args.host, args.uuid, args.sensor)
+        await run_show_sensor(args.host, args.uuid, args.sensor, args.follow)
 
     elif args.action == "get-property":
         await run_get_property(args.host, args.uuid, args.node_id, args.unit, args.subunit, args.property_id, args.property_type)
 
     else:
         raise Exception("Unknown action: " + args.action)
 
@@ -186,26 +186,28 @@
     except KeyboardInterrupt:
         pass
 
     print("Disconnecting...")
     await comfoconnect.disconnect()
 
 
-async def run_show_sensor(host: str, uuid: str, sensor: int):
+async def run_show_sensor(host: str, uuid: str, sensor: int, follow=False):
     """Connect to a bridge."""
     result = Future()
 
     # Discover bridge so we know the UUID
     bridges = await discover_bridges(host)
     if not bridges:
         raise Exception("No bridge found")
 
     def sensor_callback(sensor_, value):
         """Print sensor update."""
-        result.set_result(value)
+        print(value)
+        if not result.done():
+            result.set_result(value)
 
     # Connect to the bridge
     comfoconnect = ComfoConnect(bridges[0].host, bridges[0].uuid, sensor_callback=sensor_callback)
     try:
         await comfoconnect.connect(uuid)
     except ComfoConnectNotAllowed:
         print("Could not connect to bridge. Please register first.")
@@ -215,15 +217,24 @@
         print(f"Unknown sensor with ID {sensor}")
         sys.exit(1)
 
     # Register sensors
     await comfoconnect.register_sensor(SENSORS[sensor])
 
     # Wait for value
-    print(await result)
+    await result
+
+    # Follow for updates if requested
+    if follow:
+        try:
+            while True:
+                await asyncio.sleep(1)
+
+        except KeyboardInterrupt:
+            pass
 
     # Disconnect
     await comfoconnect.disconnect()
 
 
 async def run_get_property(host: str, uuid: str, node_id: int, unit: int, subunit: int, property_id: int, property_type: int):
     """Connect to a bridge."""
@@ -273,14 +284,15 @@
     p_sensors.add_argument("--host", help="Host address of the bridge")
     p_sensors.add_argument("--uuid", help="UUID of this app", default=DEFAULT_UUID)
 
     p_sensor = subparsers.add_parser("show-sensor", help="show a single sensor value")
     p_sensor.add_argument("sensor", help="The ID of the sensor", type=int)
     p_sensor.add_argument("--host", help="Host address of the bridge")
     p_sensor.add_argument("--uuid", help="UUID of this app", default=DEFAULT_UUID)
+    p_sensor.add_argument("--follow", "-f", help="Follow", default=False, action="store_true")
 
     p_sensor = subparsers.add_parser("get-property", help="show a property value")
     p_sensor.add_argument("unit", help="The Unit of the property", type=int)
     p_sensor.add_argument("subunit", help="The Subunit of the property", type=int)
     p_sensor.add_argument("property_id", help="The id of the property", type=int)
     p_sensor.add_argument("property_type", help="The type of the property", type=int, default=0x09)
```

### Comparing `aiocomfoconnect-0.1.7/aiocomfoconnect/bridge.py` & `aiocomfoconnect-0.1.8/aiocomfoconnect/bridge.py`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.7/aiocomfoconnect/comfoconnect.py` & `aiocomfoconnect-0.1.8/aiocomfoconnect/comfoconnect.py`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.7/aiocomfoconnect/const.py` & `aiocomfoconnect-0.1.8/aiocomfoconnect/const.py`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.7/aiocomfoconnect/discovery.py` & `aiocomfoconnect-0.1.8/aiocomfoconnect/discovery.py`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.7/aiocomfoconnect/exceptions.py` & `aiocomfoconnect-0.1.8/aiocomfoconnect/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.7/aiocomfoconnect/properties.py` & `aiocomfoconnect-0.1.8/aiocomfoconnect/properties.py`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.7/aiocomfoconnect/protobuf/nanopb_pb2.py` & `aiocomfoconnect-0.1.8/aiocomfoconnect/protobuf/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.7/aiocomfoconnect/protobuf/zehnder_pb2.py` & `aiocomfoconnect-0.1.8/aiocomfoconnect/protobuf/zehnder_pb2.py`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.7/aiocomfoconnect/sensors.py` & `aiocomfoconnect-0.1.8/aiocomfoconnect/sensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """ Sensor definitions. """
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Callable, Dict
 
+from .util import calculate_airflow_constraints
 from .const import (
     TYPE_CN_BOOL,
     TYPE_CN_INT16,
     TYPE_CN_UINT8,
     TYPE_CN_UINT16,
     TYPE_CN_UINT32,
+    TYPE_CN_INT64,
 )
 
 # Sensors
 SENSOR_ANALOG_INPUT_1 = 369
 SENSOR_ANALOG_INPUT_2 = 370
 SENSOR_ANALOG_INPUT_3 = 371
 SENSOR_ANALOG_INPUT_4 = 372
@@ -70,14 +72,15 @@
 SENSOR_TARGET_TEMPERATURE = 212
 SENSOR_TEMPERATURE_EXHAUST = 275
 SENSOR_TEMPERATURE_EXTRACT = 274
 SENSOR_TEMPERATURE_OUTDOOR = 276
 SENSOR_TEMPERATURE_SUPPLY = 221
 SENSOR_UNIT_AIRFLOW = 224
 SENSOR_UNIT_TEMPERATURE = 208
+SENSOR_AIRFLOW_CONSTRAINTS = 230
 
 UNIT_WATT = "W"
 UNIT_KWH = "kWh"
 UNIT_CELCIUS = "°C"
 UNIT_PERCENT = "%"
 UNIT_RPM = "rpm"
 UNIT_M3H = "m³/h"
@@ -144,14 +147,15 @@
     220: Sensor("Outdoor Air Temperature (?)", None, 220, TYPE_CN_INT16, lambda x: x / 10),
     SENSOR_TEMPERATURE_SUPPLY: Sensor("Supply Air Temperature", UNIT_CELCIUS, 221, TYPE_CN_INT16, lambda x: x / 10),
     SENSOR_UNIT_AIRFLOW: Sensor("Device Airflow Unit", None, 224, TYPE_CN_UINT8, lambda x: "m3ph" if x == 3 else "lps"),
     SENSOR_COMFORTCONTROL_MODE: Sensor("Sensor based ventilation mode", None, 225, TYPE_CN_UINT8),
     SENSOR_FAN_SPEED_MODE_MODULATED: Sensor("Fan Speed (modulated)", None, 226, TYPE_CN_UINT16),
     SENSOR_BYPASS_STATE: Sensor("Bypass State", UNIT_PERCENT, 227, TYPE_CN_UINT8),
     SENSOR_FROSTPROTECTION_UNBALANCE: Sensor("frostprotection_unbalance", None, 228, TYPE_CN_UINT8),
+    SENSOR_AIRFLOW_CONSTRAINTS: Sensor("Airflow constraints", None, 230, TYPE_CN_INT64, calculate_airflow_constraints),
     SENSOR_TEMPERATURE_EXTRACT: Sensor("Extract Air Temperature", UNIT_CELCIUS, 274, TYPE_CN_INT16, lambda x: x / 10),
     SENSOR_TEMPERATURE_EXHAUST: Sensor("Exhaust Air Temperature", UNIT_CELCIUS, 275, TYPE_CN_INT16, lambda x: x / 10),
     SENSOR_TEMPERATURE_OUTDOOR: Sensor("Outdoor Air Temperature", UNIT_CELCIUS, 276, TYPE_CN_INT16, lambda x: x / 10),
     277: Sensor("Outdoor Air Temperature (?)", UNIT_CELCIUS, 277, TYPE_CN_INT16, lambda x: x / 10),
     278: Sensor("Supply Air Temperature (?)", UNIT_CELCIUS, 278, TYPE_CN_INT16, lambda x: x / 10),
     SENSOR_HUMIDITY_EXTRACT: Sensor("Extract Air Humidity", UNIT_PERCENT, 290, TYPE_CN_UINT8),
     SENSOR_HUMIDITY_EXHAUST: Sensor("Exhaust Air Humidity", UNIT_PERCENT, 291, TYPE_CN_UINT8),
```

### Comparing `aiocomfoconnect-0.1.7/pyproject.toml` & `aiocomfoconnect-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiocomfoconnect"
-version = "0.1.7"
+version = "0.1.8"
 description = "aiocomfoconnect is an asyncio Python 3 library for communicating with a Zehnder ComfoAir Q350/450/600 ventilation system"
 authors = ["Michaël Arnauts <michael.arnauts@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/michaelarnauts/aiocomfoconnect"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `aiocomfoconnect-0.1.7/PKG-INFO` & `aiocomfoconnect-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocomfoconnect
-Version: 0.1.7
+Version: 0.1.8
 Summary: aiocomfoconnect is an asyncio Python 3 library for communicating with a Zehnder ComfoAir Q350/450/600 ventilation system
 Home-page: https://github.com/michaelarnauts/aiocomfoconnect
 Author: Michaël Arnauts
 Author-email: michael.arnauts@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -42,14 +42,15 @@
 $ python -m aiocomfoconnect set-speed low --host 192.168.1.213
 $ python -m aiocomfoconnect set-mode auto --host 192.168.1.213
 $ python -m aiocomfoconnect set-speed medium --host 192.168.1.213
 $ python -m aiocomfoconnect set-speed high --host 192.168.1.213
 
 $ python -m aiocomfoconnect show-sensors --host 192.168.1.213
 $ python -m aiocomfoconnect show-sensor 276 --host 192.168.1.213
+$ python -m aiocomfoconnect show-sensor 276 --host 192.168.1.213 -f
 
 $ python -m aiocomfoconnect get-property --host 192.168.1.213 1 1 8 9  # Unit 0x01, SubUnit 0x01, Property 0x08, Type STRING. See PROTOCOL-RMI.md
 ```
 
 ## Available methods
 
 - `async connect()`: Connect to the bridge.
```

