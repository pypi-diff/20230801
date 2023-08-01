# Comparing `tmp/mpscenes-0.4.3.tar.gz` & `tmp/mpscenes-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpscenes-0.4.3.tar", max compression
+gzip compressed data, was "mpscenes-0.4.4.tar", max compression
```

## Comparing `mpscenes-0.4.3.tar` & `mpscenes-0.4.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       71 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/.__init__.py
--rw-r--r--   0        0        0       71 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/__init__.py
--rw-r--r--   0        0        0     1161 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/common/analytic_trajectory.py
--rw-r--r--   0        0        0     1684 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/common/component.py
--rw-r--r--   0        0        0      500 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/common/errors.py
--rw-r--r--   0        0        0      755 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/common/reference_trajectory.py
--rw-r--r--   0        0        0     3271 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/common/spline_trajectory.py
--rw-r--r--   0        0        0     3314 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/goals/dynamic_sub_goal.py
--rw-r--r--   0        0        0     2513 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/goals/goal_composition.py
--rw-r--r--   0        0        0     1961 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/goals/static_joint_space_sub_goal.py
--rw-r--r--   0        0        0     2642 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/goals/static_sub_goal.py
--rw-r--r--   0        0        0     1958 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/goals/sub_goal.py
--rw-r--r--   0        0        0      905 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/goals/sub_goal_creator.py
--rw-r--r--   0        0        0     4071 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/obstacles/box_obstacle.py
--rw-r--r--   0        0        0       14 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/obstacles/box_smooth.mtl
--rw-r--r--   0        0        0      836 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/obstacles/box_smooth.obj
--rw-r--r--   0        0        0     4216 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/obstacles/collision_obstacle.py
--rw-r--r--   0        0        0     4186 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/obstacles/cylinder_obstacle.py
--rw-r--r--   0        0        0     1227 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/obstacles/dynamic_box_obstacle.py
--rw-r--r--   0        0        0     1312 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/obstacles/dynamic_cylinder_obstacle.py
--rw-r--r--   0        0        0     2901 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/obstacles/dynamic_obstacle.py
--rw-r--r--   0        0        0     1278 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/obstacles/dynamic_sphere_obstacle.py
--rw-r--r--   0        0        0     1244 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/obstacles/dynamic_urdf_obstacle.py
--rw-r--r--   0        0        0      817 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/obstacles/obstacleCreator.py
--rw-r--r--   0        0        0     3106 2023-07-26 19:16:24.795068 mpscenes-0.4.3/mpscenes/obstacles/sphere_obstacle.py
--rw-r--r--   0        0        0      136 2023-07-26 19:16:24.799068 mpscenes-0.4.3/mpscenes/obstacles/sphere_smooth.mtl
--rw-r--r--   0        0        0   111602 2023-07-26 19:16:24.799068 mpscenes-0.4.3/mpscenes/obstacles/sphere_smooth.obj
--rw-r--r--   0        0        0     1833 2023-07-26 19:16:24.799068 mpscenes-0.4.3/mpscenes/obstacles/urdf_obstacle.py
--rw-r--r--   0        0        0      551 2023-07-26 19:16:24.799068 mpscenes-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 mpscenes-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0       71 2023-08-01 08:41:06.246054 mpscenes-0.4.4/mpscenes/.__init__.py
+-rw-r--r--   0        0        0       71 2023-08-01 08:41:06.246054 mpscenes-0.4.4/mpscenes/__init__.py
+-rw-r--r--   0        0        0     1161 2023-08-01 08:41:06.246054 mpscenes-0.4.4/mpscenes/common/analytic_trajectory.py
+-rw-r--r--   0        0        0     1684 2023-08-01 08:41:06.246054 mpscenes-0.4.4/mpscenes/common/component.py
+-rw-r--r--   0        0        0      500 2023-08-01 08:41:06.246054 mpscenes-0.4.4/mpscenes/common/errors.py
+-rw-r--r--   0        0        0      755 2023-08-01 08:41:06.246054 mpscenes-0.4.4/mpscenes/common/reference_trajectory.py
+-rw-r--r--   0        0        0     3271 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/common/spline_trajectory.py
+-rw-r--r--   0        0        0     3314 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/goals/dynamic_sub_goal.py
+-rw-r--r--   0        0        0     2513 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/goals/goal_composition.py
+-rw-r--r--   0        0        0     1961 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/goals/static_joint_space_sub_goal.py
+-rw-r--r--   0        0        0     2642 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/goals/static_sub_goal.py
+-rw-r--r--   0        0        0     1958 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/goals/sub_goal.py
+-rw-r--r--   0        0        0      905 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/goals/sub_goal_creator.py
+-rw-r--r--   0        0        0     4091 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/obstacles/box_obstacle.py
+-rw-r--r--   0        0        0       14 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/obstacles/box_smooth.mtl
+-rw-r--r--   0        0        0      836 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/obstacles/box_smooth.obj
+-rw-r--r--   0        0        0     4319 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/obstacles/collision_obstacle.py
+-rw-r--r--   0        0        0     4218 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/obstacles/cylinder_obstacle.py
+-rw-r--r--   0        0        0     1227 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/obstacles/dynamic_box_obstacle.py
+-rw-r--r--   0        0        0     1312 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/obstacles/dynamic_cylinder_obstacle.py
+-rw-r--r--   0        0        0     2901 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/obstacles/dynamic_obstacle.py
+-rw-r--r--   0        0        0     1278 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/obstacles/dynamic_sphere_obstacle.py
+-rw-r--r--   0        0        0     1244 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/obstacles/dynamic_urdf_obstacle.py
+-rw-r--r--   0        0        0      817 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/obstacles/obstacleCreator.py
+-rw-r--r--   0        0        0     3126 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/obstacles/sphere_obstacle.py
+-rw-r--r--   0        0        0      136 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/obstacles/sphere_smooth.mtl
+-rw-r--r--   0        0        0   111602 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/obstacles/sphere_smooth.obj
+-rw-r--r--   0        0        0     1833 2023-08-01 08:41:06.250054 mpscenes-0.4.4/mpscenes/obstacles/urdf_obstacle.py
+-rw-r--r--   0        0        0      551 2023-08-01 08:41:06.250054 mpscenes-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 mpscenes-0.4.4/PKG-INFO
```

### Comparing `mpscenes-0.4.3/mpscenes/common/analytic_trajectory.py` & `mpscenes-0.4.4/mpscenes/common/analytic_trajectory.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.3/mpscenes/common/component.py` & `mpscenes-0.4.4/mpscenes/common/component.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.3/mpscenes/common/reference_trajectory.py` & `mpscenes-0.4.4/mpscenes/common/reference_trajectory.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.3/mpscenes/common/spline_trajectory.py` & `mpscenes-0.4.4/mpscenes/common/spline_trajectory.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.3/mpscenes/goals/dynamic_sub_goal.py` & `mpscenes-0.4.4/mpscenes/goals/dynamic_sub_goal.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.3/mpscenes/goals/goal_composition.py` & `mpscenes-0.4.4/mpscenes/goals/goal_composition.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.3/mpscenes/goals/static_joint_space_sub_goal.py` & `mpscenes-0.4.4/mpscenes/goals/static_joint_space_sub_goal.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.3/mpscenes/goals/static_sub_goal.py` & `mpscenes-0.4.4/mpscenes/goals/static_sub_goal.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.3/mpscenes/goals/sub_goal.py` & `mpscenes-0.4.4/mpscenes/goals/sub_goal.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.3/mpscenes/goals/sub_goal_creator.py` & `mpscenes-0.4.4/mpscenes/goals/sub_goal_creator.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.3/mpscenes/obstacles/box_obstacle.py` & `mpscenes-0.4.4/mpscenes/obstacles/box_obstacle.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,12 +124,12 @@
 
     def movable(self):
         return self._config.movable
 
     def csv(self, file_name, samples=100):
         pass
 
-    def distance(self, position: np.ndarray) -> float:
-        pos = self.position_into_obstacle_frame(position)
+    def distance(self, position: np.ndarray, **kwargs) -> float:
+        pos = self.position_into_obstacle_frame(position, **kwargs)
         q = np.transpose(np.subtract(np.transpose(np.absolute(pos)),
                                      np.array(self.size())/2.0)) 
         return np.linalg.norm(np.maximum(q, 0), axis=0) + np.minimum(np.maximum(q[0], np.maximum(q[1], q[2])), 0.0)
```

### Comparing `mpscenes-0.4.3/mpscenes/obstacles/box_smooth.obj` & `mpscenes-0.4.4/mpscenes/obstacles/box_smooth.obj`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.3/mpscenes/obstacles/collision_obstacle.py` & `mpscenes-0.4.4/mpscenes/obstacles/collision_obstacle.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,17 +118,21 @@
 
     def acceleration(self, **kwargs) -> np.ndarray:
         return np.zeros(self.dimension())
 
     def movable(self) -> bool:
         return self._config.movable
 
-    def position_into_obstacle_frame(self, positions: np.ndarray) -> np.ndarray:
+    def position_into_obstacle_frame(self, positions: np.ndarray, **kwargs) -> np.ndarray:
+        if 't' in kwargs:
+            t = kwargs.get('t')
+        else:
+            t = 0
         transformation_matrix = quaternion_to_homogeneous_matrix(
-            self.position(), self.orientation()
+            self.position(t=t), self.orientation()
         )
         if len(positions.shape) > 1:
             nb_points = positions.shape[0]
             positions_homo = np.transpose(np.append(positions, np.ones((nb_points, 1)), axis=1))
             return np.dot(np.linalg.inv(transformation_matrix), positions_homo)[0:3,:]
         else:
             positions_homo = np.transpose(np.append(positions, 1))
```

### Comparing `mpscenes-0.4.3/mpscenes/obstacles/cylinder_obstacle.py` & `mpscenes-0.4.4/mpscenes/obstacles/cylinder_obstacle.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,16 +114,16 @@
 
     def movable(self):
         return self._config.movable
 
     def csv(self, file_name, samples=100):
         pass
 
-    def distance(self, position) -> float:
-        pos = self.position_into_obstacle_frame(position)
+    def distance(self, position: np.ndarray, **kwargs) -> float:
+        pos = self.position_into_obstacle_frame(position, **kwargs)
         if len(pos.shape) > 1:
             pos[2, :] += self.size()[1]/2
             norm_pos_2 = np.linalg.norm(pos[0:2, :], axis=0)
             abs_val = np.absolute(np.stack((norm_pos_2, pos[2, :])))
             d = np.transpose(np.subtract(np.transpose(abs_val), np.array(self.size())))
             return np.minimum(np.maximum(d[0, :], d[1, :]), 0.0) + np.linalg.norm(np.maximum(d, 0.0), axis=0)
         else:
```

### Comparing `mpscenes-0.4.3/mpscenes/obstacles/dynamic_box_obstacle.py` & `mpscenes-0.4.4/mpscenes/obstacles/dynamic_box_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.3/mpscenes/obstacles/dynamic_cylinder_obstacle.py` & `mpscenes-0.4.4/mpscenes/obstacles/dynamic_cylinder_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.3/mpscenes/obstacles/dynamic_obstacle.py` & `mpscenes-0.4.4/mpscenes/obstacles/dynamic_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.3/mpscenes/obstacles/dynamic_sphere_obstacle.py` & `mpscenes-0.4.4/mpscenes/obstacles/dynamic_sphere_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.3/mpscenes/obstacles/dynamic_urdf_obstacle.py` & `mpscenes-0.4.4/mpscenes/obstacles/dynamic_urdf_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.3/mpscenes/obstacles/obstacleCreator.py` & `mpscenes-0.4.4/mpscenes/obstacles/obstacleCreator.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.3/mpscenes/obstacles/sphere_obstacle.py` & `mpscenes-0.4.4/mpscenes/obstacles/sphere_obstacle.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,10 +94,10 @@
         x = self.position()[0] + (self.radius() - 0.1) * np.cos(theta)
         y = self.position()[1] + (self.radius() - 0.1) * np.sin(theta)
         with open(file_name, "w", encoding="utf8") as file:
             csv_writer = csv.writer(file, delimiter=",")
             for i in range(2 * samples):
                 csv_writer.writerow([x[i], y[i]])
 
-    def distance(self, position: np.ndarray) -> float:
-        pos = self.position_into_obstacle_frame(position)
+    def distance(self, position: np.ndarray, **kwargs) -> float:
+        pos = self.position_into_obstacle_frame(position, **kwargs)
         return np.linalg.norm(pos, axis=0) - self.radius()
```

### Comparing `mpscenes-0.4.3/mpscenes/obstacles/sphere_smooth.obj` & `mpscenes-0.4.4/mpscenes/obstacles/sphere_smooth.obj`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.3/mpscenes/obstacles/urdf_obstacle.py` & `mpscenes-0.4.4/mpscenes/obstacles/urdf_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.4.3/pyproject.toml` & `mpscenes-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpscenes"
-version = "0.4.3"
+version = "0.4.4"
 description = "Generic motion planning scenes, including goals and obstacles."
 authors = ["Max <m.spahn@tudelft.nl>"]
   
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.22.0"
```

### Comparing `mpscenes-0.4.3/PKG-INFO` & `mpscenes-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpscenes
-Version: 0.4.3
+Version: 0.4.4
 Summary: Generic motion planning scenes, including goals and obstacles.
 Author: Max
 Author-email: m.spahn@tudelft.nl
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

