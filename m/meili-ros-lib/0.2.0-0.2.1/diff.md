# Comparing `tmp/meili_ros_lib-0.2.0.tar.gz` & `tmp/meili_ros_lib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meili_ros_lib-0.2.0.tar", last modified: Mon Jul 24 12:41:25 2023, max compression
+gzip compressed data, was "meili_ros_lib-0.2.1.tar", last modified: Tue Aug  1 13:09:42 2023, max compression
```

## Comparing `meili_ros_lib-0.2.0.tar` & `meili_ros_lib-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 12:41:25.973608 meili_ros_lib-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      297 2023-07-24 12:41:25.973608 meili_ros_lib-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 12:41:25.972608 meili_ros_lib-0.2.0/meili_ros_lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22757 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/agent.py
--rw-rw-rw-   0 root         (0) root         (0)     2208 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/agent_setup.py
--rw-rw-rw-   0 root         (0) root         (0)     4521 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/config_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     3284 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/connection.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/docking.py
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/maths.py
--rw-rw-rw-   0 root         (0) root         (0)    11990 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/offline.py
--rw-rw-rw-   0 root         (0) root         (0)     3213 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/parse_data.py
--rw-rw-rw-   0 root         (0) root         (0)    12925 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/sdk_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/sentry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 12:41:25.973608 meili_ros_lib-0.2.0/meili_ros_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      297 2023-07-24 12:41:25.000000 meili_ros_lib-0.2.0/meili_ros_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      479 2023-07-24 12:41:25.000000 meili_ros_lib-0.2.0/meili_ros_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 12:41:25.000000 meili_ros_lib-0.2.0/meili_ros_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-24 12:41:25.000000 meili_ros_lib-0.2.0/meili_ros_lib.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      353 2023-07-24 12:41:25.973608 meili_ros_lib-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:09:42.222515 meili_ros_lib-0.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-08-01 13:09:32.000000 meili_ros_lib-0.2.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      297 2023-08-01 13:09:42.222515 meili_ros_lib-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 13:09:32.000000 meili_ros_lib-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:09:42.221515 meili_ros_lib-0.2.1/meili_ros_lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 13:09:32.000000 meili_ros_lib-0.2.1/meili_ros_lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23867 2023-08-01 13:09:32.000000 meili_ros_lib-0.2.1/meili_ros_lib/agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2208 2023-08-01 13:09:32.000000 meili_ros_lib-0.2.1/meili_ros_lib/agent_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     4521 2023-08-01 13:09:32.000000 meili_ros_lib-0.2.1/meili_ros_lib/config_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     3284 2023-08-01 13:09:32.000000 meili_ros_lib-0.2.1/meili_ros_lib/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-08-01 13:09:32.000000 meili_ros_lib-0.2.1/meili_ros_lib/docking.py
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-08-01 13:09:32.000000 meili_ros_lib-0.2.1/meili_ros_lib/maths.py
+-rw-rw-rw-   0 root         (0) root         (0)    11990 2023-08-01 13:09:32.000000 meili_ros_lib-0.2.1/meili_ros_lib/offline.py
+-rw-rw-rw-   0 root         (0) root         (0)     3213 2023-08-01 13:09:32.000000 meili_ros_lib-0.2.1/meili_ros_lib/parse_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    12925 2023-08-01 13:09:32.000000 meili_ros_lib-0.2.1/meili_ros_lib/sdk_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-08-01 13:09:32.000000 meili_ros_lib-0.2.1/meili_ros_lib/sentry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 13:09:42.222515 meili_ros_lib-0.2.1/meili_ros_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-08-01 13:09:42.000000 meili_ros_lib-0.2.1/meili_ros_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      479 2023-08-01 13:09:42.000000 meili_ros_lib-0.2.1/meili_ros_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 13:09:42.000000 meili_ros_lib-0.2.1/meili_ros_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-08-01 13:09:42.000000 meili_ros_lib-0.2.1/meili_ros_lib.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      353 2023-08-01 13:09:42.222515 meili_ros_lib-0.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-08-01 13:09:32.000000 meili_ros_lib-0.2.1/setup.py
```

### Comparing `meili_ros_lib-0.2.0/LICENSE.txt` & `meili_ros_lib-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.2.0/meili_ros_lib/agent.py` & `meili_ros_lib-0.2.1/meili_ros_lib/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from meili_ros_lib.config_agent import ConfigAgent
 from meili_ros_lib.maths import quaternion_to_euler
 from meili_ros_lib.parse_data import parse_battery_data
 from meili_ros_lib.sentry import initialize_sentry, agent_sentry
 
 from sentry_sdk import capture_exception, capture_message
 
-
 initialize_sentry()
 
 
 def update_capacity_lipo(voltage):
     # Calculate current capacity of lipo batteries taking into account voltage/capacity estimation using regression
     capacity = 47.6 * voltage - 500
     return capacity
@@ -175,73 +174,116 @@
             message.validate()
             self.client.send(message)
         except Exception as e:
             self.log_info(f"SEND MESSAGE ERROR{e} {event} {vehicle}")
 
     def ping_filtering_mode(self):
 
-        self.ping_speed()
+        self.ping_status()
 
         if self.node.outdoor:
             self.ping_gps()
-        else:
-            self.ping_location()
+        #else:
+        #    self.ping_location()
 
-        if self.node.battery_present:
-            self.ping_battery()
+        #if self.node.battery_present:
+        #    self.ping_battery()
+        #self.ping_speed()
 
         if self.node.traffic_control and not self.node.v2:
             self.ping_trajectory()
 
+    def get_location(self, msg, index):
+        if isinstance(msg, PoseWithCovarianceStamped):
+            x = round(msg.pose.pose.position.x, 3)
+            y = round(msg.pose.pose.position.y, 3)
+            orientation = msg.pose.pose.orientation
+        elif isinstance(msg, Pose):
+            x = round(msg.position.x, 3)
+            y = round(msg.position.y, 3)
+            orientation = msg.orientation
+        else:
+            self.log_error(
+                f"[ROSAgent] Robot {index}-{self.vehicle_names[index]} pose is not available. Message >> {msg}"
+            )
+            capture_message("[ROSAgent] Robot pose is not available")
+            return 0
+
+        yaw = round(quaternion_to_euler(
+            orientation.x, orientation.y, orientation.z, orientation.w
+        ),
+            3)
+        return { "xm": x, "ym": y, "rotation": yaw}
+
+    def get_battery(self, msg, index):
+        if self.node.lipo_battery:
+            msg.capacity = update_capacity_lipo(msg.voltage)
+        battery_data = parse_battery_data(msg)
+
+        return battery_data
+
+    def get_speed(self, msg, index):
+        if isinstance(msg, Odometry):
+            speed = msg.twist.twist.linear.x
+            speed = round(speed, 3)
+        return {"speed":speed}
+
+    def ping_status(self):
+        value = {}
+        for index in range(len(self.vehicle_list)):
+            value["timestamp"] = time.time()
+
+            location_msg = self.msg_pose[index]
+            value["location"] = self.get_location(location_msg, index)
+
+            if self.node.battery_present:
+                battery_msg = self.msg_battery[index]
+                value["battery"] = self.get_battery(battery_msg, index)
+
+            speed_msg = self.msg_speed[index]
+            value["speed"] = self.get_speed(speed_msg,index)
+
+            self.send_message_client(
+                constants.EVENT_STATUS,
+                value,
+                self.vehicle_list[index],
+            )
+
     def ping_location(self):
         """Ping Location """
         try:
             for index, msg in enumerate(self.msg_pose):
-                if isinstance(msg, PoseWithCovarianceStamped):
-                    x = round(msg.pose.pose.position.x, 3)
-                    y = round(msg.pose.pose.position.y, 3)
-                    orientation = msg.pose.pose.orientation
-                elif isinstance(msg, Pose):
-                    x = round(msg.position.x, 3)
-                    y = round(msg.position.y, 3)
-                    orientation = msg.orientation
-                else:
-                    self.log_error(
-                        f"[ROSAgent] Robot {index}-{self.vehicle_names[index]} pose is not available. Message >> {msg}"
-                    )
-                    capture_message("[ROSAgent] Robot pose is not available")
-                    continue
+                value = self.get_location(msg, index)
+                value["timestamp"] = time.time()
 
-                yaw = round(quaternion_to_euler(
-                    orientation.x, orientation.y, orientation.z, orientation.w
-                ),
-                    3)
-                self.send_message_client(
-                    constants.EVENT_LOCATION,
-                    {"timestamp": time.time(), "xm": x, "ym": y, "rotation": yaw},
-                    self.vehicle_list[index],
-                )
+                if value != 0:
+                    self.send_message_client(
+                        constants.EVENT_LOCATION,
+                        value,
+                        self.vehicle_list[index],
+                    )
 
         except Exception as error:
             self.log_info(f"[ROSAgent] Ping location error: {error}")
             capture_exception(error)
 
     def ping_battery(self):
         """Sending Battery message via websocket"""
         try:
             for index, msg in enumerate(self.msg_battery):
-                if self.node.lipo_battery:
-                    msg.capacity = update_capacity_lipo(msg.voltage)
-                battery_data = parse_battery_data(msg)
-                battery_data["timestamp"] = time.time()
-                self.send_message_client(
-                    constants.EVENT_BATTERY,
-                    {**battery_data},
-                    self.vehicle_list[index],
-                )
+                value = self.get_battery(msg, index)
+                if value is not None:
+                    value["timestamp"] = time.time()
+                    self.log_info(f"{value}")
+                    self.send_message_client(
+                        constants.EVENT_BATTERY,
+                        {**value},
+                        self.vehicle_list[index],
+                    )
+
         except Exception as error:
             capture_exception(error)
             self.log_info(f"[ROSAgent] Ping Battery Error: {error}")
 
     def ping_trajectory(self):
         """Send the trajectory as an array of poses"""
 
@@ -298,26 +340,25 @@
             self.log_info(f"[ROSAgent] Ping Docking Routine Error: {e} ")
             capture_exception(e)
 
     def ping_speed(self):
         """Ping Speed"""
         try:
             for index, msg in enumerate(self.msg_speed):
-                if isinstance(msg, Odometry):
-                    speed = msg.twist.twist.linear.x
-                    speed = round(speed, 3)
+                try:
+                    value = self.get_speed(msg, index)
+                    value["timestamp"] = time.time()
                     self.send_message_client(
                         constants.EVENT_SPEED,
-                        {"timestamp": time.time(), "speed": speed},
+                        value,
                         self.vehicle_list[index]
                     )
-
-                else:
-                    #self.log_info(f"[ROSAgent] Robot {self.vehicle_names[index]} speed is not available")
-                    #capture_message("[ROSAgent] Robot speed is not available")
+                except:
+                    # self.log_info(f"[ROSAgent] Robot {self.vehicle_names[index]} speed is not available")
+                    # capture_message("[ROSAgent] Robot speed is not available")
                     break
 
         except Exception as e:
             self.log_info(f"[ROSAgent] Ping speed Error: {e} ")
             capture_exception(e)
 
     ################################################
@@ -386,15 +427,15 @@
 
             self.goal_id[vehicle_position] = goal_id
             self.send_message_client(
                 constants.EVENT_GOAL_STATUS,
                 {"goal_id": goal_id, "status_id": status_id},
                 vehicle_uuid,
             )
-            #self.log_info(
+            # self.log_info(
             #    f"[ROSAgent] Sending {goal_id} in progress<<{status_id}>> of vehicle {vehicle_position} ")
 
         else:
             now = datetime.datetime.now()
             dt_string = now.strftime("%d/%m/%Y %H:%M:%S")
             self.start_time = dt_string
         return 1
@@ -462,16 +503,16 @@
 
         return 0
 
     def task_finished(self, goal_id, status_id, vehicle_uuid):
         vehicle_position = self.return_vehicle_position(vehicle_uuid)
         # TASK ONLINE
         if self.ws_open:
-           # self.log_info(
-           #     f"[ROSAgent] Task {goal_id} finished<<{status_id}>> of vehicle {vehicle_position} ")
+            # self.log_info(
+            #     f"[ROSAgent] Task {goal_id} finished<<{status_id}>> of vehicle {vehicle_position} ")
             if not self.waypoints[vehicle_position]:
 
                 if self.waypoints_goal_id[vehicle_position] is not None:
                     goal_id = self.waypoints_goal_id[vehicle_position]
                     self.waypoints_goal_id[vehicle_position] = None
                     if self.goal_id_rerouted[vehicle_position] is not None:
                         goal_id = self.goal_id_rerouted[vehicle_position]
@@ -480,16 +521,16 @@
                 self.goal_id[vehicle_position] = goal_id
                 self.send_message_client(
                     constants.EVENT_GOAL_STATUS,
                     {"goal_id": goal_id, "status_id": status_id},
                     vehicle_uuid,
                 )
 
-              #  self.log_info(
-              #      f"[ROSAgent] Sending {goal_id} finished<<{status_id}>> of vehicle {vehicle_position} ")
+            #  self.log_info(
+            #      f"[ROSAgent] Sending {goal_id} finished<<{status_id}>> of vehicle {vehicle_position} ")
 
         # OFFLINE TASK
         if self.connection.offline_agent.offline:
             success = True
 
             for task in self.connection.offline_agent.offline_tasks:
                 if self.connection.offline_agent.current_task_uuid == task[0]:
```

### Comparing `meili_ros_lib-0.2.0/meili_ros_lib/agent_setup.py` & `meili_ros_lib-0.2.1/meili_ros_lib/agent_setup.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.2.0/meili_ros_lib/config_agent.py` & `meili_ros_lib-0.2.1/meili_ros_lib/config_agent.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.2.0/meili_ros_lib/connection.py` & `meili_ros_lib-0.2.1/meili_ros_lib/connection.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.2.0/meili_ros_lib/docking.py` & `meili_ros_lib-0.2.1/meili_ros_lib/docking.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.2.0/meili_ros_lib/maths.py` & `meili_ros_lib-0.2.1/meili_ros_lib/maths.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.2.0/meili_ros_lib/offline.py` & `meili_ros_lib-0.2.1/meili_ros_lib/offline.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.2.0/meili_ros_lib/parse_data.py` & `meili_ros_lib-0.2.1/meili_ros_lib/parse_data.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.2.0/meili_ros_lib/sdk_handlers.py` & `meili_ros_lib-0.2.1/meili_ros_lib/sdk_handlers.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.2.0/meili_ros_lib/sentry.py` & `meili_ros_lib-0.2.1/meili_ros_lib/sentry.py`

 * *Files identical despite different names*

