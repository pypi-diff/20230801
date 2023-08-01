# Comparing `tmp/AnimazePy-0.0.3.tar.gz` & `tmp/AnimazePy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AnimazePy-0.0.3.tar", last modified: Tue Aug  1 16:30:58 2023, max compression
+gzip compressed data, was "AnimazePy-1.0.1.tar", last modified: Thu Jul 13 19:26:34 2023, max compression
```

## Comparing `AnimazePy-0.0.3.tar` & `AnimazePy-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:30:58.631374 AnimazePy-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:30:58.631374 AnimazePy-0.0.3/AnimazePy/
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-08-01 16:30:48.000000 AnimazePy-0.0.3/AnimazePy/AnimazeWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-08-01 16:30:48.000000 AnimazePy-0.0.3/AnimazePy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:30:58.631374 AnimazePy-0.0.3/AnimazePy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-01 16:30:58.000000 AnimazePy-0.0.3/AnimazePy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-01 16:30:58.000000 AnimazePy-0.0.3/AnimazePy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 16:30:58.000000 AnimazePy-0.0.3/AnimazePy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 16:30:58.000000 AnimazePy-0.0.3/AnimazePy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 16:30:58.000000 AnimazePy-0.0.3/AnimazePy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-01 16:30:48.000000 AnimazePy-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-01 16:30:58.631374 AnimazePy-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-08-01 16:30:48.000000 AnimazePy-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 16:30:58.631374 AnimazePy-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-08-01 16:30:48.000000 AnimazePy-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:26:34.651905 AnimazePy-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:26:34.651905 AnimazePy-1.0.1/AnimazePy/
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-07-13 19:26:25.000000 AnimazePy-1.0.1/AnimazePy/AnimazeWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-13 19:26:25.000000 AnimazePy-1.0.1/AnimazePy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:26:34.651905 AnimazePy-1.0.1/AnimazePy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-13 19:26:34.000000 AnimazePy-1.0.1/AnimazePy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-13 19:26:34.000000 AnimazePy-1.0.1/AnimazePy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:26:34.000000 AnimazePy-1.0.1/AnimazePy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 19:26:34.000000 AnimazePy-1.0.1/AnimazePy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 19:26:34.000000 AnimazePy-1.0.1/AnimazePy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 19:26:25.000000 AnimazePy-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-13 19:26:34.651905 AnimazePy-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-13 19:26:25.000000 AnimazePy-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:26:34.651905 AnimazePy-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-13 19:26:25.000000 AnimazePy-1.0.1/setup.py
```

### Comparing `AnimazePy-0.0.3/AnimazePy/AnimazeWrapper.py` & `AnimazePy-1.0.1/AnimazePy/AnimazeWrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,52 +51,38 @@
             self.logger.error("Is Animaze running?")
             return "Connection was actively refused by the target machine. Is Animaze running?"
         except Exception as e:
             self.logger.error(f"Failed to open WebSocket due to: {str(e)}")
             return
  
 
+
     def disconnect(self):
         if self.ws is not None:
             self.ws.close()
             self.ws = None
             self.logger.info("WebSocket connection closed successfully.")
             return "WebSocket connection closed successfully."
         else:
             self.logger.error("No WebSocket connection to close.")
             return "No WebSocket connection to close."
 
-
     def send_command(self, command):
         try:
             if self.ws is None:
-                self.logger.error("WebSocket connection is not open. Must connect first.")
-                self.connect()
+                self.logger.error("WebSocket connection is not open. Call 'open_websocket' first.")
                 return
 
             self.ws.send(json.dumps(command))
             response = self.ws.recv()
             return json.loads(response)
         except Exception as e:
             self.logger.error('Failed to send command due to: ' + str(e))
-            self.ws = None
-    
 
 
-    def send_chatpal_message(self, message:str):
-        """
-        Send a prompt to Animaze ChatPal, and receive the conversational AI response, while the avatar starts speaking. 
-        
-        """
-        command = {
-            "action": "ChatbotSendMessage",
-            "id": self.dev_name,                 
-            "message": message
-        }
-        return self.send_command(command)
     
     def get_item_icon(self, avatar_name:str):
         command = {
             "action": "GetItemIcon",
             "id": self.dev_name,
             "name": avatar_name
         }
@@ -152,49 +138,35 @@
         command = {
             "action": "SetCameraFOV",
             "id": self.dev_name,
             "fov": fov
         }
         return self.send_command(command)
 
-    def get_camera_transform(self):
-        command = {
-            "action": "GetCameraTransform",
-        }
-        return self.send_command(command)
-    
-    def set_camera_transform(self, pos_x:float, pos_y:float, pos_z:float, rot_x:float, rot_y:float, rot_z:float, rot_w:float):
-        command = {
-            "action": "SetCameraTransform",
-            "position":[pos_x, pos_y, pos_z],
-            "rotation":[rot_x, rot_y, rot_z, rot_w]
-        }
-        return self.send_command(command)
-
     def broadcast(self, choice:bool):
         command = {
             "action": "Broadcast",
             "id": self.dev_name,
             "toggle": choice
         }
         return self.send_command(command)
 
     def trigger_special_action(self, index:int):
         command = {
             "action": "TriggerSpecialAction",
             "id": self.dev_name,
-            "index": index
+             "index": index
            }
         return self.send_command(command)
     
     def trigger_idle_anim(self, index:int):
         command = {
-            "action": "TriggerIdle",
+            "action": "SelectIdleAnim",
             "id": self.dev_name,
-            "index": index
+            "animName": index
         }
         return self.send_command(command)
     
 
     def trigger_emote(self, anim_name:str):
         command = {
             "action": "TriggerEmote",
@@ -211,22 +183,22 @@
             "index": pose_index
         }
         return self.send_command(command)
 
     def get_scenes(self):
         command = { 
             "action": "GetScenes",
-            "id": self.dev_name
+            "id": "MyDevName" 
         }
         return self.send_command(command)
     
     def get_quickscenes(self):
         command = { 
             "action": "GetQuickscenes",
-            "id": self.dev_name
+            "id": "MyDevName" 
         }
         return self.send_command(command)
 
     def load_scene(self, scene_name:str):
         command = {
             "action": "LoadScene",
             "id": self.dev_name,
@@ -234,14 +206,15 @@
         }
         return self.send_command(command)
     
 
     def load_quick_scene(self, scene_index:int):
         command = {
             "action": "LoadQuickscene",
+            "id": self.dev_name,
             "index": scene_index
         }
         return self.send_command(command)
     
 
     def get_avatars(self):
         command = {
@@ -277,76 +250,64 @@
         return self.send_command(command)
     
     def look_at_camera(self, choice:bool):
         command = {
             "action": "SetOverride",           
             "behavior": "Look At Camera",            
             "value": choice
+            ## "range": 0.5
         }
         return self.send_command(command)
     
 
-    def look_at_camera_head(self, choice:bool):
-        command = {
-            "action": "SetOverride",           
-            "behavior": "Look At Camera Head",            
-            "value": choice
-        }
-        return self.send_command(command)
-
-    
+    def mousekeyboard_behavior(self, choice:bool, keyboardScale, handToKeyboardDist, xOffset, yOffset, zOffset):
+        """ NO idea what this does or how to use it """
 
-    def mousekeyboard_behavior(self, choice:bool, keyboardScale:float, handToKeyboardDist:float, xOffset:float, yOffset:float, zOffset:float):
         command = {
-            "action": "SetOverride",                   
-            "behavior": "Mouse Keyboard Behavior",     
-            "value": choice,                           
-            "keyboardScale": keyboardScale,            
-            "handToKeyboardDist": handToKeyboardDist,  
-            "xAxisOffset": xOffset,                    
-            "yAxisOffset": yOffset,                    
-            "zAxisOffset ": zOffset                    
+            "action": "SetOverride",                    # required (string) 
+            "behavior": "Mouse Keyboard Behavior",      # required (string)
+            "value": choice,                            # required (bool)
+            "keyboardScale": keyboardScale,             # optional (float)
+            "handToKeyboardDist": handToKeyboardDist,   # optional (float)
+            "xAxisOffset": xOffset,                     # optional (float)
+            "yAxisOffset": yOffset,                     # optional (float)
+            "zAxisOffset ": zOffset                     # optional (float)
         }
         return self.send_command(command)
 
 
     def follow_mouse(self, choice:bool):
+        """ NO idea what this does or how to use it """
         command ={
-            "action": "SetOverride",            
-            "behavior": "Follow Mouse Cursor", 
-            "value": choice                  
+            "action": "SetOverride",            # required (string) 
+            "behavior": "Follow Mouse Cursor",  # required (string)
+            "value": choice                     # required (bool)
         }
         return self.send_command(command)
     
-    def pupil_behavoior(self, value:bool, frequency:float=None):
-        """ 
-        Adjust how often the pupils move 
+    def pupil_behavoior(self, value, frequency:float=None):
+        """ Adjust how often the pupils move 
             - value: True or False
-            - frequency (optional): 0.0 - 1.0
-        """
+            - frequency: 0.0 - 1.0
+            """
         command = {
-            "action": "SetOverride",          
-            "behavior": "Pupil Behavior",    
-            "value": value,                
-            "frequency": frequency        
+            "action": "SetOverride",          # required (string) 
+            "behavior": "Pupil Behavior",     # required (string)
+            "value": value,                   # required (bool)
+            "frequency": frequency            # optional required (float)
         }
         return self.send_command(command)
     
 
-    def breathing_behavior(self, value:bool, amplitude:float, frequency:float):
-        """ 
-        Adjust how often the pupils move
-            - value: True or False
-            - amplitude(optional): 0.0 - 1.0
-            - frequency(optional): 0.0 - 1.0
-        """
-        command = {
-            "action": "SetOverride",          
-            "behavior": "Breathing Behavior", 
-            "value": value,                  
-            "amplitude": amplitude,           
-            "frequency": frequency            
+    def breathing_behavior(self, value, amplitude:float, frequency:float):
+        """ Doesnt appear to do much, but does work """
+        command = {
+            "action": "SetOverride",          # required (string) 
+            "behavior": "Breathing Behavior", # required (string)
+            "value": value,                   # required (bool)
+            "amplitude": amplitude,           # optional required (float)
+            "frequency": frequency            # optional required (float)
         }
         return self.send_command(command)
```

### Comparing `AnimazePy-0.0.3/AnimazePy/__init__.py` & `AnimazePy-1.0.1/AnimazePy/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,10 +12,10 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-__version__ = "0.0.3"
+__version__ = "1.0.1"
 
 from .AnimazeWrapper import AnimazeWrapper
```

### Comparing `AnimazePy-0.0.3/AnimazePy.egg-info/PKG-INFO` & `AnimazePy-1.0.1/AnimazePy.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AnimazePy
-Version: 0.0.3
+Version: 1.0.1
 Summary: A Python Wrapper for the Animaze API
 Home-page: https://github.com/gitagogaming/AnimazePy
 Author: Gitago
 Author-email: gitproductions.814@gmail.com
 License: GPLv3+
 Project-URL: Documentation, https://github.com/gitagogaming/AnimazePy
 Project-URL: Source, https://github.com/gitagogaming/AnimazePy
@@ -27,19 +27,10 @@
 - Establish a WebSocket connection to the Animaze API
 - Send commands to control avatars, behaviors, and animations
 - Retrieve avatar information and icons
 - Set camera field of view (fov) and start a broadcast
 - Select idle animations, scenes, emotes, and special actions
 - and more!
 
-# How to enable the Websocket API in Animaze
-![animaze_enable_api](https://github.com/gitagogaming/AnimazePy/assets/76603653/3696017d-2d71-4a32-9f19-fada92ab87e9)
 
 
-
-For more information, documentation, and usage examples, visit the GitHub repository: https://github.com/gitagogaming/AnimazePy/
-
-<br>
-<br>
-<br>
-
-<i> Special Thanks to [@Killerboss2019](https://github.com/Killerboss2019) for helping me get this published to Pypi and for all the help and guidance throughtout my Python journey. </i>
+For more information, documentation, and usage examples, visit the GitHub repository: https://github.com/gitagogaming/AnimazePy/)https://github.com/gitagogaming/AnimazePy/
```

### Comparing `AnimazePy-0.0.3/LICENSE` & `AnimazePy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AnimazePy-0.0.3/PKG-INFO` & `AnimazePy-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AnimazePy
-Version: 0.0.3
+Version: 1.0.1
 Summary: A Python Wrapper for the Animaze API
 Home-page: https://github.com/gitagogaming/AnimazePy
 Author: Gitago
 Author-email: gitproductions.814@gmail.com
 License: GPLv3+
 Project-URL: Documentation, https://github.com/gitagogaming/AnimazePy
 Project-URL: Source, https://github.com/gitagogaming/AnimazePy
@@ -27,19 +27,10 @@
 - Establish a WebSocket connection to the Animaze API
 - Send commands to control avatars, behaviors, and animations
 - Retrieve avatar information and icons
 - Set camera field of view (fov) and start a broadcast
 - Select idle animations, scenes, emotes, and special actions
 - and more!
 
-# How to enable the Websocket API in Animaze
-![animaze_enable_api](https://github.com/gitagogaming/AnimazePy/assets/76603653/3696017d-2d71-4a32-9f19-fada92ab87e9)
 
 
-
-For more information, documentation, and usage examples, visit the GitHub repository: https://github.com/gitagogaming/AnimazePy/
-
-<br>
-<br>
-<br>
-
-<i> Special Thanks to [@Killerboss2019](https://github.com/Killerboss2019) for helping me get this published to Pypi and for all the help and guidance throughtout my Python journey. </i>
+For more information, documentation, and usage examples, visit the GitHub repository: https://github.com/gitagogaming/AnimazePy/)https://github.com/gitagogaming/AnimazePy/
```

### Comparing `AnimazePy-0.0.3/README.md` & `AnimazePy-1.0.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -6,19 +6,10 @@
 - Establish a WebSocket connection to the Animaze API
 - Send commands to control avatars, behaviors, and animations
 - Retrieve avatar information and icons
 - Set camera field of view (fov) and start a broadcast
 - Select idle animations, scenes, emotes, and special actions
 - and more!
 
-# How to enable the Websocket API in Animaze
-![animaze_enable_api](https://github.com/gitagogaming/AnimazePy/assets/76603653/3696017d-2d71-4a32-9f19-fada92ab87e9)
 
 
-
-For more information, documentation, and usage examples, visit the GitHub repository: https://github.com/gitagogaming/AnimazePy/
-
-<br>
-<br>
-<br>
-
-<i> Special Thanks to [@Killerboss2019](https://github.com/Killerboss2019) for helping me get this published to Pypi and for all the help and guidance throughtout my Python journey. </i>
+For more information, documentation, and usage examples, visit the GitHub repository: https://github.com/gitagogaming/AnimazePy/)https://github.com/gitagogaming/AnimazePy/
```

### Comparing `AnimazePy-0.0.3/setup.py` & `AnimazePy-1.0.1/setup.py`

 * *Files identical despite different names*

