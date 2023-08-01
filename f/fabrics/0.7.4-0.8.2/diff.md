# Comparing `tmp/fabrics-0.7.4.tar.gz` & `tmp/fabrics-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrics-0.7.4.tar", max compression
+gzip compressed data, was "fabrics-0.8.2.tar", max compression
```

## Comparing `fabrics-0.7.4.tar` & `fabrics-0.8.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0    35306 2023-07-01 00:59:42.639427 fabrics-0.7.4/LICENSE
--rw-r--r--   0        0        0     4831 2023-07-01 00:59:42.639427 fabrics-0.7.4/README.md
--rw-r--r--   0        0        0       40 2023-07-01 00:59:42.795428 fabrics-0.7.4/fabrics/.gitignore
--rw-r--r--   0        0        0       71 2023-07-01 00:59:42.795428 fabrics-0.7.4/fabrics/__init__.py
--rw-r--r--   0        0        0      249 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/components/energies/execution_energies.py
--rw-r--r--   0        0        0     3048 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/components/leaves/attractor.py
--rw-r--r--   0        0        0     2453 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/components/leaves/dynamic_attractor.py
--rw-r--r--   0        0        0     4365 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/components/leaves/dynamic_geometry.py
--rw-r--r--   0        0        0     2915 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/components/leaves/dynamic_leaf.py
--rw-r--r--   0        0        0    10097 2023-07-01 01:00:11.675667 fabrics-0.7.4/fabrics/components/leaves/geometry.py
--rw-r--r--   0        0        0     2307 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/components/leaves/leaf.py
--rw-r--r--   0        0        0     1369 2023-07-01 01:00:11.675667 fabrics-0.7.4/fabrics/components/maps/parameterized_maps.py
--rw-r--r--   0        0        0     1319 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/defaults/default_energies.py
--rw-r--r--   0        0        0     1609 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/defaults/default_geometries.py
--rw-r--r--   0        0        0      918 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/defaults/default_leaves.py
--rw-r--r--   0        0        0     1852 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/defaults/default_maps.py
--rw-r--r--   0        0        0      260 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/diffGeometry/casadi_helpers.py
--rw-r--r--   0        0        0     3605 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/diffGeometry/diffMap.py
--rw-r--r--   0        0        0     4016 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/diffGeometry/energized_geometry.py
--rw-r--r--   0        0        0     6868 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/diffGeometry/energy.py
--rw-r--r--   0        0        0     3364 2023-07-01 01:00:11.675667 fabrics-0.7.4/fabrics/diffGeometry/geometry.py
--rw-r--r--   0        0        0     6934 2023-07-01 01:00:11.675667 fabrics-0.7.4/fabrics/diffGeometry/spec.py
--rw-r--r--   0        0        0     2818 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/diffGeometry/speedControl.py
--rw-r--r--   0        0        0     6194 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/helpers/casadiFunctionWrapper.py
--rw-r--r--   0        0        0       75 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/helpers/constants.py
--rw-r--r--   0        0        0      273 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/helpers/exceptions.py
--rw-r--r--   0        0        0     2068 2023-07-01 01:00:11.675667 fabrics-0.7.4/fabrics/helpers/functions.py
--rw-r--r--   0        0        0     3940 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/helpers/variables.py
--rw-r--r--   0        0        0     6592 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/planner/non_holonomic_parameterized_planner.py
--rw-r--r--   0        0        0    22532 2023-07-01 01:00:11.675667 fabrics-0.7.4/fabrics/planner/parameterized_planner.py
--rw-r--r--   0        0        0     1548 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/planner/serialized_planner.py
--rw-r--r--   0        0        0     1074 2023-07-01 01:00:11.679667 fabrics-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     5844 1970-01-01 00:00:00.000000 fabrics-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0    35306 2023-08-01 00:50:06.699440 fabrics-0.8.2/LICENSE
+-rw-r--r--   0        0        0     4831 2023-08-01 00:50:06.699440 fabrics-0.8.2/README.md
+-rw-r--r--   0        0        0       40 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/.gitignore
+-rw-r--r--   0        0        0       71 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/__init__.py
+-rw-r--r--   0        0        0      249 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/components/energies/execution_energies.py
+-rw-r--r--   0        0        0     3048 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/components/leaves/attractor.py
+-rw-r--r--   0        0        0     2453 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/components/leaves/dynamic_attractor.py
+-rw-r--r--   0        0        0     4354 2023-08-01 00:50:35.179296 fabrics-0.8.2/fabrics/components/leaves/dynamic_geometry.py
+-rw-r--r--   0        0        0     2915 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/components/leaves/dynamic_leaf.py
+-rw-r--r--   0        0        0    12171 2023-08-01 00:50:35.179296 fabrics-0.8.2/fabrics/components/leaves/geometry.py
+-rw-r--r--   0        0        0     2307 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/components/leaves/leaf.py
+-rw-r--r--   0        0        0     1988 2023-08-01 00:50:35.179296 fabrics-0.8.2/fabrics/components/maps/parameterized_maps.py
+-rw-r--r--   0        0        0     1319 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/defaults/default_energies.py
+-rw-r--r--   0        0        0     1609 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/defaults/default_geometries.py
+-rw-r--r--   0        0        0      918 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/defaults/default_leaves.py
+-rw-r--r--   0        0        0     1852 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/defaults/default_maps.py
+-rw-r--r--   0        0        0      260 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/diffGeometry/casadi_helpers.py
+-rw-r--r--   0        0        0     3605 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/diffGeometry/diffMap.py
+-rw-r--r--   0        0        0     4016 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/diffGeometry/energized_geometry.py
+-rw-r--r--   0        0        0     6868 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/diffGeometry/energy.py
+-rw-r--r--   0        0        0     3364 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/diffGeometry/geometry.py
+-rw-r--r--   0        0        0     6934 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/diffGeometry/spec.py
+-rw-r--r--   0        0        0     2818 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/diffGeometry/speedControl.py
+-rw-r--r--   0        0        0     6194 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/helpers/casadiFunctionWrapper.py
+-rw-r--r--   0        0        0       75 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/helpers/constants.py
+-rw-r--r--   0        0        0     2824 2023-08-01 00:50:35.179296 fabrics-0.8.2/fabrics/helpers/distances.py
+-rw-r--r--   0        0        0      273 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/helpers/exceptions.py
+-rw-r--r--   0        0        0     2068 2023-08-01 00:50:06.843439 fabrics-0.8.2/fabrics/helpers/functions.py
+-rw-r--r--   0        0        0     3940 2023-08-01 00:50:06.847439 fabrics-0.8.2/fabrics/helpers/variables.py
+-rw-r--r--   0        0        0     6252 2023-08-01 00:50:35.179296 fabrics-0.8.2/fabrics/planner/non_holonomic_parameterized_planner.py
+-rw-r--r--   0        0        0    26554 2023-08-01 00:50:35.179296 fabrics-0.8.2/fabrics/planner/parameterized_planner.py
+-rw-r--r--   0        0        0     1548 2023-08-01 00:50:06.847439 fabrics-0.8.2/fabrics/planner/serialized_planner.py
+-rw-r--r--   0        0        0     1114 2023-08-01 00:50:35.183296 fabrics-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     5801 1970-01-01 00:00:00.000000 fabrics-0.8.2/PKG-INFO
```

### Comparing `fabrics-0.7.4/LICENSE` & `fabrics-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.4/README.md` & `fabrics-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.4/fabrics/components/leaves/attractor.py` & `fabrics-0.8.2/fabrics/components/leaves/attractor.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.4/fabrics/components/leaves/dynamic_attractor.py` & `fabrics-0.8.2/fabrics/components/leaves/dynamic_attractor.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.4/fabrics/components/leaves/dynamic_geometry.py` & `fabrics-0.8.2/fabrics/components/leaves/dynamic_geometry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import casadi as ca
 import numpy as np
 
 from fabrics.diffGeometry.diffMap import DifferentialMap
 from fabrics.components.maps.parameterized_maps import (
-    ParameterizedObstacleMap,
+    SphereSphereMap,
 )
 from fabrics.diffGeometry.geometry import Geometry
 from fabrics.diffGeometry.energy import Lagrangian
 from fabrics.components.leaves.dynamic_leaf import DynamicLeaf
 from fabrics.helpers.variables import Variables
 from fabrics.helpers.functions import parse_symbolic_input
 
@@ -98,18 +98,18 @@
             radius_body_variable = ca.SX.sym(radius_body_name, 1)
         geo_parameters = {
             radius_name: radius_variable,
             radius_body_name: radius_body_variable,
         }
         self._parent_variables.add_parameters(geo_parameters)
         self._forward_map = DifferentialMap(self._forward_kinematics, self._parent_variables)
-        self._geometry_map = ParameterizedObstacleMap(
+        self._geometry_map = SphereSphereMap(
             self._relative_variables,
             self._relative_variables.position_variable(),
-            np.zeros(self._dim_ref),
+            ca.SX(np.zeros(self._dim_ref)),
             radius_variable,
             radius_body_variable,
         )
 
     def geometry_map(self):
         return self._geometry_map
```

### Comparing `fabrics-0.7.4/fabrics/components/leaves/dynamic_leaf.py` & `fabrics-0.8.2/fabrics/components/leaves/dynamic_leaf.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.4/fabrics/components/leaves/geometry.py` & `fabrics-0.8.2/fabrics/components/leaves/geometry.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 import casadi as ca
-import numpy as np
 
 from fabrics.components.maps.parameterized_maps import (
-    ParameterizedObstacleMap,
+    CapsuleSphereMap,
     ParameterizedPlaneConstraintMap,
+    SphereSphereMap,
 )
 from fabrics.diffGeometry.diffMap import DifferentialMap, ExplicitDifferentialMap
 from fabrics.diffGeometry.geometry import Geometry
 from fabrics.diffGeometry.energy import Lagrangian
 from fabrics.components.leaves.leaf import Leaf
 from fabrics.helpers.variables import Variables
 from fabrics.helpers.functions import parse_symbolic_input
 
 
 class GenericGeometryLeaf(Leaf):
+
+    def extract_or_create_variable(self, variable_name: str, variable_dimension: int) -> ca.SX:
+        if variable_name in self._parent_variables.parameters():
+            return self._parent_variables.parameters()[variable_name]
+        else:
+            return ca.SX.sym(variable_name, variable_dimension)
+
     def set_geometry(self, geometry: str) -> None:
         """
         Sets the geometry from a string.
 
         Params
         ---------
         geometry: str
@@ -145,24 +152,32 @@
             radius_body_variable = ca.SX.sym(radius_body_name, 1)
         geo_parameters = {
             reference_name: reference_variable,
             radius_name: radius_variable,
             radius_body_name: radius_body_variable,
         }
         self._parent_variables.add_parameters(geo_parameters)
-        self._map = ParameterizedObstacleMap(
+#        self._map_old = ParameterizedObstacleMap(
+#            self._parent_variables,
+#            self._forward_kinematics,
+#            reference_variable,
+#            radius_variable,
+#            radius_body_variable,
+#        )
+        self._map = SphereSphereMap(
             self._parent_variables,
-            self._forward_kinematics,
             reference_variable,
-            radius_variable,
+            self._forward_kinematics,
             radius_body_variable,
+            radius_variable,
         )
 
 
 
+
 class ESDFGeometryLeaf(GenericGeometryLeaf):
     """ESDFGeometryLeaf is a leaf with explicit gradients that can be set
     at runtime.
 
     Euclidean Signed Distance Fields (ESDF) can be exploited to avoid explicit
     geometry representations. As automated differentiation does not work on ESDFs, 
     this GeometryLeaf adds parameters for J and Jdot that can be computed at
@@ -264,8 +279,54 @@
         self._map = ParameterizedPlaneConstraintMap(
             self._parent_variables,
             self._forward_kinematics,
             constraint_variable,
             radius_body_variable
         )
 
+class CapsuleSphereLeaf(GenericGeometryLeaf):
+    def __init__(
+        self,
+        parent_variables: Variables,
+        capsule_name: str,
+        sphere_name: str,
+        capsule_center_1: ca.SX,
+        capsule_center_2: ca.SX,
+    ):
+        super().__init__(
+            parent_variables, f"{capsule_name}_{sphere_name}_leaf", None
+        )
+        self._capsule_centers = [
+            capsule_center_1,
+            capsule_center_2,
+        ]
+        self._capsule_name = capsule_name
+        self._sphere_name = sphere_name
+        self.set_forward_map()
+
+
+    def set_forward_map(self):
+        sphere_radius_name = f"radius_{self._sphere_name}"
+        sphere_center_name = f"x_{self._sphere_name}"
+        capsule_radius_name = f"radius_{self._capsule_name}"
+        obstacle_dimension = self._capsule_centers[0].size()[0]
+        sphere_radius = self.extract_or_create_variable(sphere_radius_name, 1)
+        capsule_radius = self.extract_or_create_variable(capsule_radius_name, 1)
+        sphere_center = self.extract_or_create_variable(sphere_center_name, obstacle_dimension)
+        geo_parameters = {
+            sphere_radius_name: sphere_radius,
+            capsule_radius_name: capsule_radius,
+            sphere_center_name: sphere_center,
+        }
+        self._parent_variables.add_parameters(geo_parameters)
+        self._map = CapsuleSphereMap(
+            self._parent_variables,
+            self._capsule_centers,
+            sphere_center,
+            capsule_radius,
+            sphere_radius,
+        )
+
+
+
+
```

### Comparing `fabrics-0.7.4/fabrics/components/leaves/leaf.py` & `fabrics-0.8.2/fabrics/components/leaves/leaf.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.4/fabrics/defaults/default_energies.py` & `fabrics-0.8.2/fabrics/defaults/default_energies.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.4/fabrics/defaults/default_geometries.py` & `fabrics-0.8.2/fabrics/defaults/default_geometries.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.4/fabrics/defaults/default_leaves.py` & `fabrics-0.8.2/fabrics/defaults/default_leaves.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.4/fabrics/defaults/default_maps.py` & `fabrics-0.8.2/fabrics/defaults/default_maps.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.4/fabrics/diffGeometry/diffMap.py` & `fabrics-0.8.2/fabrics/diffGeometry/diffMap.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.4/fabrics/diffGeometry/energized_geometry.py` & `fabrics-0.8.2/fabrics/diffGeometry/energized_geometry.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.4/fabrics/diffGeometry/energy.py` & `fabrics-0.8.2/fabrics/diffGeometry/energy.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.4/fabrics/diffGeometry/geometry.py` & `fabrics-0.8.2/fabrics/diffGeometry/geometry.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.4/fabrics/diffGeometry/spec.py` & `fabrics-0.8.2/fabrics/diffGeometry/spec.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.4/fabrics/diffGeometry/speedControl.py` & `fabrics-0.8.2/fabrics/diffGeometry/speedControl.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.4/fabrics/helpers/casadiFunctionWrapper.py` & `fabrics-0.8.2/fabrics/helpers/casadiFunctionWrapper.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.4/fabrics/helpers/functions.py` & `fabrics-0.8.2/fabrics/helpers/functions.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.4/fabrics/helpers/variables.py` & `fabrics-0.8.2/fabrics/helpers/variables.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.4/fabrics/planner/non_holonomic_parameterized_planner.py` & `fabrics-0.8.2/fabrics/planner/non_holonomic_parameterized_planner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from dataclasses import dataclass
 import casadi as ca
+from forwardkinematics.fksCommon.fk import ForwardKinematics
 import numpy as np
 import logging
 
-from forwardkinematics.fksCommon.fk_creator import FkCreator
-from forwardkinematics.urdfFks.generic_urdf_fk import GenericURDFFk
 
 from fabrics.planner.parameterized_planner import ParameterizedFabricPlanner, FabricPlannerConfig
 from fabrics.diffGeometry.energy import Lagrangian
 from fabrics.diffGeometry.geometry import Geometry
 from fabrics.diffGeometry.energized_geometry import WeightedGeometry
 from fabrics.helpers.casadiFunctionWrapper import CasadiFunctionWrapper
 from fabrics.helpers.functions import parse_symbolic_input
@@ -24,30 +23,22 @@
         "sym('m_arm') * np.identity(x.size()[0] - 3)"
     )
 
 class NonHolonomicParameterizedFabricPlanner(ParameterizedFabricPlanner):
     def __init__(
         self,
         dof: int,
-        robot_type: str,
+        forward_kinematics: ForwardKinematics,
         facing_direction: str = '-y',
         **kwargs
     ):
         self.leaves = {}
         self._dof = dof
         self._config = NonHolonomicFabricPlannerConfig(**kwargs)
-        if self._config.urdf:
-            self._forward_kinematics = GenericURDFFk(
-                self._config.urdf,
-                rootLink=self._config.root_link,
-                end_link=self._config.end_link,
-                base_type='diffdrive',
-            )
-        else:
-            self._forward_kinematics = FkCreator(robot_type).fk()
+        self._forward_kinematics  = forward_kinematics
         self.initialize_joint_variables()
         self.set_base_geometry()
         self._target_velocity = np.zeros(self._geometry.x().size()[0])
         self._ref_sign = 1
         self.set_non_holonomic_constraints(facing_direction=facing_direction)
```

### Comparing `fabrics-0.7.4/fabrics/planner/parameterized_planner.py` & `fabrics-0.8.2/fabrics/planner/parameterized_planner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass, field
-from typing import Dict
+from typing import Dict, Optional
 import logging
 import casadi as ca
+from forwardkinematics.fksCommon.fk import ForwardKinematics
 from forwardkinematics.urdfFks.urdfFk import LinkNotInURDFError
 import numpy as np
 from copy import deepcopy
 from fabrics.helpers.exceptions import ExpressionSparseError
 from typing import List
 
 from fabrics.helpers.variables import Variables
@@ -21,15 +22,15 @@
 from fabrics.helpers.casadiFunctionWrapper import CasadiFunctionWrapper
 
 from fabrics.components.energies.execution_energies import ExecutionLagrangian
 from fabrics.components.leaves.leaf import Leaf
 from fabrics.components.leaves.attractor import GenericAttractor
 from fabrics.components.leaves.dynamic_attractor import GenericDynamicAttractor
 from fabrics.components.leaves.dynamic_geometry import DynamicObstacleLeaf, GenericDynamicGeometryLeaf
-from fabrics.components.leaves.geometry import ObstacleLeaf, LimitLeaf, PlaneConstraintGeometryLeaf, SelfCollisionLeaf, GenericGeometryLeaf, ESDFGeometryLeaf
+from fabrics.components.leaves.geometry import CapsuleSphereLeaf, ObstacleLeaf, LimitLeaf, PlaneConstraintGeometryLeaf, SelfCollisionLeaf, GenericGeometryLeaf, ESDFGeometryLeaf
 
 from mpscenes.goals.goal_composition import GoalComposition
 from mpscenes.goals.sub_goal import SubGoal
 
 from forwardkinematics.fksCommon.fk_creator import FkCreator
 from forwardkinematics.urdfFks.generic_urdf_fk import GenericURDFFk
 
@@ -100,31 +101,21 @@
     damper_beta: str = (
         "0.5 * (ca.tanh(-sym('alpha_b') * (ca.norm_2(x) - sym('radius_shift'))) + 1) * sym('beta_close') + sym('beta_distant') + ca.fmax(0, sym('a_ex') - sym('a_le'))"
     )
     damper_eta: str = (
         "0.5 * (ca.tanh(-sym('alpha_eta') * sym('ex_lag') * (1 - sym('ex_factor')) - 0.5) + 1)"
     )
     """
-    urdf: str = None
-    root_link: str = 'base_link'
-    end_link: str = 'ee_link'
 
 
 class ParameterizedFabricPlanner(object):
-    def __init__(self, dof: int, robot_type: str, **kwargs):
+    def __init__(self, dof: int, forward_kinematics: ForwardKinematics, **kwargs):
         self._dof = dof
         self._config = FabricPlannerConfig(**kwargs)
-        if self._config.urdf:
-            self._forward_kinematics = GenericURDFFk(
-                self._config.urdf,
-                rootLink=self._config.root_link,
-                end_link=self._config.end_link,
-            )
-        else:
-            self._forward_kinematics = FkCreator(robot_type).fk()
+        self._forward_kinematics = forward_kinematics
         self.initialize_joint_variables()
         self.set_base_geometry()
         self._target_velocity = np.zeros(self._geometry.x().size()[0])
         self._ref_sign = 1
         self.leaves = {}
 
     """ INITIALIZING """
@@ -288,113 +279,255 @@
         eta_expression = self.config.damper_eta
         self._damper = Damper(beta_expression, eta_expression, x_psi, dm_psi, exLag._l)
         self._variables.add_parameters(self._damper.symbolic_parameters())
 
     def get_forward_kinematics(self, link_name) -> ca.SX:
         if isinstance(link_name, ca.SX):
             return link_name
-        if self._config.urdf:
+        if isinstance(self._forward_kinematics, GenericURDFFk):
             fk = self._forward_kinematics.fk(
                 self._variables.position_variable(),
-                self._config.root_link,
+                self._forward_kinematics._rootLink,
                 link_name,
                 positionOnly=True
             )
         else:
             fk = self._forward_kinematics.fk(
                 self._variables.position_variable(),
                 link_name,
                 positionOnly=True
             )
         return fk
 
+    def add_capsule_sphere_geometry(
+            self,
+            obstacle_name: str,
+            capsule_name: str,
+            tf_capsule_origin: ca.SX,
+            capsule_length: float
+            ) -> None:
+        tf_origin_center_0 = np.identity(4)
+        tf_origin_center_0[2][3] = capsule_length / 2
+        tf_center_0 = ca.mtimes(tf_capsule_origin, tf_origin_center_0)
+        tf_origin_center_1 = np.identity(4)
+        tf_origin_center_1[2][3] = - capsule_length / 2
+        tf_center_1 = ca.mtimes(tf_capsule_origin, tf_origin_center_1)
+        capsule_sphere_leaf = CapsuleSphereLeaf(
+            self._variables,
+            capsule_name,
+            obstacle_name,
+            tf_center_0[0:3,3],
+            tf_center_1[0:3,3],
+        )
+        capsule_sphere_leaf.set_geometry(self.config.collision_geometry)
+        capsule_sphere_leaf.set_finsler_structure(self.config.collision_finsler)
+        self.add_leaf(capsule_sphere_leaf)
+
+
+
+
+    def add_spherical_obstacle_geometry(
+            self,
+            obstacle_name: str,
+            collision_link_name: str,
+            forward_kinematics: ca.SX,
+            ) -> None:
+        """
+        Add a spherical obstacle geometry to the fabrics planner.
+
+        Parameters
+        ----------
+        obstacle_name : str
+            The name of the obstacle to be added.
+        collision_link_name : str
+            The name of the robot's collision link that the obstacle is associated with.
+        forward_kinematics : ca.SX
+            The forward kinematics expression representing the obstacle's position.
+
+        Returns
+        -------
+        None
+
+        Notes
+        -----
+        - The `forward_kinematics` should be a symbolic
+            expression using CasADi SX for the obstacle's position.
+        - The `collision_geometry` and `collision_finsler` configurations
+            must be set before adding the obstacle.
+        - After adding the obstacle, it will be included in the robot's
+            configuration and affect its motion planning.
+
+        Example
+        -------
+        obstacle_name = "Sphere_Obstacle"
+        collision_link_name = "Link1"
+        forward_kinematics = ca.SX([fk_x, fk_y, fk_z])
+        robot.add_spherical_obstacle_geometry(
+            obstacle_name,
+            collision_link_name,
+            forward_kinematics
+        )
+        """
+        geometry = ObstacleLeaf(
+            self._variables,
+            forward_kinematics,
+            obstacle_name,
+            collision_link_name,
+        )
+        geometry.set_geometry(self.config.collision_geometry)
+        geometry.set_finsler_structure(self.config.collision_finsler)
+        self.add_leaf(geometry)
+
+    def add_dynamic_spherical_obstacle_geometry(
+            self,
+            obstacle_name: str,
+            collision_link_name: str,
+            forward_kinematics: ca.SX,
+            reference_parameters: dict,
+            dynamic_obstacle_dimension: int = 3,
+            ) -> None:
+        geometry = DynamicObstacleLeaf(
+            self._variables,
+            forward_kinematics[0:dynamic_obstacle_dimension],
+            obstacle_name,
+            collision_link_name,
+            reference_parameters=reference_parameters
+        )
+        geometry.set_geometry(self.config.collision_geometry)
+        geometry.set_finsler_structure(self.config.collision_finsler)
+        self.add_leaf(geometry)
+
+    def add_plane_constraint(
+            self,
+            constraint_name: str,
+            collision_link_name: str,
+            forward_kinematics: ca.SX,
+            ) -> None:
+
+        geometry = PlaneConstraintGeometryLeaf(
+            self._variables,
+            constraint_name,
+            collision_link_name,
+            forward_kinematics,
+        )
+        geometry.set_geometry(self.config.geometry_plane_constraint)
+        geometry.set_finsler_structure(self.config.finsler_plane_constraint)
+        self.add_leaf(geometry)
+    
+    def add_esdf_geometry(
+            self,
+            collision_link_name: str,
+            ) -> None:
+        fk = self.get_forward_kinematics(collision_link_name)
+        geometry = ESDFGeometryLeaf(self._variables, collision_link_name, fk)
+        geometry.set_geometry(self.config.collision_geometry)
+        geometry.set_finsler_structure(self.config.collision_finsler)
+        self.add_leaf(geometry)
+
+    def add_spherical_self_collision_geometry(
+            self,
+            collision_link_1: str,
+            collision_link_2: str,
+            ) -> None:
+        fk_1 = self.get_forward_kinematics(collision_link_1)
+        fk_2 = self.get_forward_kinematics(collision_link_2)
+        fk = fk_2 - fk_1
+        if is_sparse(fk):
+            message = (
+                    f"Expression {fk} for links {collision_link_1} "
+                    "and {collision_link_2} is sparse and thus skipped."
+            )
+            logging.warning(message.format_map(locals()))
+        self_collision_name = (
+                f"self_collision_{collision_link_1}_"
+                "{collision_link_2}"
+        )
+        geometry = SelfCollisionLeaf(self._variables, fk, self_collision_name)
+        geometry.set_geometry(self.config.self_collision_geometry)
+        geometry.set_finsler_structure(self.config.self_collision_finsler)
+        self.add_leaf(geometry)
+
+    def add_limit_geometry(
+            self,
+            joint_index: int,
+            limits: list,
+            ) -> None:
+        lower_limit_geometry = LimitLeaf(self._variables, joint_index, limits[0], 0)
+        lower_limit_geometry.set_geometry(self.config.limit_geometry)
+        lower_limit_geometry.set_finsler_structure(self.config.limit_finsler)
+        upper_limit_geometry = LimitLeaf(self._variables, joint_index, limits[1], 1)
+        upper_limit_geometry.set_geometry(self.config.limit_geometry)
+        upper_limit_geometry.set_finsler_structure(self.config.limit_finsler)
+        self.add_leaf(lower_limit_geometry)
+        self.add_leaf(upper_limit_geometry)
+
 
-    """ DEFAULT COMPOSITION """
     def set_components(
         self,
-        collision_links: list = None,
-        self_collision_pairs: dict = None,
-        collision_links_esdf: list = None,
-        goal: GoalComposition = None,
-        limits: list = None,
+        collision_links: Optional[list] = None,
+        self_collision_pairs: Optional[dict] = None,
+        collision_links_esdf: Optional[list] = None,
+        goal: Optional[GoalComposition] = None,
+        limits: Optional[list] = None,
         number_obstacles: int = 1,
         number_dynamic_obstacles: int = 0,
         number_plane_constraints: int = 0,
         dynamic_obstacle_dimension: int = 3,
     ):
-        if collision_links is None:
-            collision_links = []
-        if collision_links_esdf is None:
-            collision_links_esdf = []
-        if self_collision_pairs is None:
-            self_collision_pairs = {}
+        collision_links = collision_links or []
+        collision_links_esdf = collision_links_esdf or []
+        self_collision_pairs = self_collision_pairs or {}
+
         reference_parameter_list = []
         for i in range(number_dynamic_obstacles):
             reference_parameters = {
                 f"x_obst_dynamic_{i}": ca.SX.sym(f"x_obst_dynamic_{i}", dynamic_obstacle_dimension),
                 f"xdot_obst_dynamic_{i}": ca.SX.sym(f"xdot_obst_dynamic_{i}", dynamic_obstacle_dimension),
                 f"xddot_obst_dynamic_{i}": ca.SX.sym(f"xddot_obst_dynamic_{i}", dynamic_obstacle_dimension),
             }
             reference_parameter_list.append(reference_parameters)
         for collision_link in collision_links:
             fk = self.get_forward_kinematics(collision_link)
             if is_sparse(fk):
-                logging.warning(f"Expression {fk} for link {collision_link} is sparse and thus skipped.")
+                message = (
+                        f"Expression {fk} for link {collision_link} "
+                        "is sparse and thus skipped."
+                )
+                logging.warning(message.format_map(locals()))
                 continue
             for i in range(number_obstacles):
                 obstacle_name = f"obst_{i}"
-                geometry = ObstacleLeaf(self._variables, fk, obstacle_name, collision_link)
-                geometry.set_geometry(self.config.collision_geometry)
-                geometry.set_finsler_structure(self.config.collision_finsler)
-                self.add_leaf(geometry)
+                self.add_spherical_obstacle_geometry(obstacle_name, collision_link, fk)
             for i in range(number_dynamic_obstacles):
                 obstacle_name = f"obst_dynamic_{i}"
-                geometry = DynamicObstacleLeaf(self._variables, fk, obstacle_name, collision_link, reference_parameters=reference_parameter_list[i])
-                geometry.set_geometry(self.config.collision_geometry)
-                geometry.set_finsler_structure(self.config.collision_finsler)
-                self.add_leaf(geometry)
+                self.add_dynamic_spherical_obstacle_geometry(
+                        obstacle_name,
+                        collision_link,
+                        fk,
+                        reference_parameter_list[i],
+                        dynamic_obstacle_dimension=dynamic_obstacle_dimension,
+                )
             for i in range(number_plane_constraints):
                 constraint_name = f"constraint_{i}"
-                geometry = PlaneConstraintGeometryLeaf(self._variables, constraint_name, collision_link, fk)
-                geometry.set_geometry(self.config.geometry_plane_constraint)
-                geometry.set_finsler_structure(self.config.finsler_plane_constraint)
-                self.add_leaf(geometry)
+                self.add_plane_constraint(constraint_name, collision_link, fk)
 
 
         for collision_link in collision_links_esdf:
-            fk = self.get_forward_kinematics(collision_link)
-            geometry = ESDFGeometryLeaf(self._variables, collision_link, fk)
-            geometry.set_geometry(self.config.collision_geometry)
-            geometry.set_finsler_structure(self.config.collision_finsler)
-            self.add_leaf(geometry)
+            self.add_esdf_geometry(collision_link)
 
         for self_collision_key, self_collision_list in self_collision_pairs.items():
-            fk_key = self.get_forward_kinematics(self_collision_key)
             for self_collision_link in self_collision_list:
-                fk_link = self.get_forward_kinematics(self_collision_link)
-                fk = fk_link - fk_key
-                if is_sparse(fk):
-                    logging.warning(f"Expression {fk} for links {self_collision_key} and {self_collision_link} is sparse and thus skipped.")
-                    continue
-                self_collision_name = f"self_collision_{self_collision_key}_{self_collision_link}"
-                geometry = SelfCollisionLeaf(self._variables, fk, self_collision_name)
-                geometry.set_geometry(self.config.self_collision_geometry)
-                geometry.set_finsler_structure(self.config.self_collision_finsler)
-                self.add_leaf(geometry)
+                self.add_spherical_self_collision_geometry(
+                        self_collision_key,
+                        self_collision_link
+                )
 
         if limits:
             for joint_index in range(len(limits)):
-                lower_limit_geometry = LimitLeaf(self._variables, joint_index, limits[joint_index][0], 0)
-                lower_limit_geometry.set_geometry(self.config.limit_geometry)
-                lower_limit_geometry.set_finsler_structure(self.config.limit_finsler)
-                upper_limit_geometry = LimitLeaf(self._variables, joint_index, limits[joint_index][1], 1)
-                upper_limit_geometry.set_geometry(self.config.limit_geometry)
-                upper_limit_geometry.set_finsler_structure(self.config.limit_finsler)
-                self.add_leaf(lower_limit_geometry)
-                self.add_leaf(upper_limit_geometry)
+                self.add_limit_geometry(joint_index, limits[joint_index])
 
         execution_energy = ExecutionLagrangian(self._variables)
         self.set_execution_energy(execution_energy)
         if goal:
             self.set_goal_component(goal)
             # Adds default execution energy
             execution_energy = ExecutionLagrangian(self._variables)
```

### Comparing `fabrics-0.7.4/fabrics/planner/serialized_planner.py` & `fabrics-0.8.2/fabrics/planner/serialized_planner.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.4/pyproject.toml` & `fabrics-0.8.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 [tool.poetry]
 name = "fabrics"
-version = "0.7.4"
+version = "0.8.2"
 description = "Optimization fabrics in python."
 authors = ["Max Spahn <m.spahn@tudelft.nl>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://tud-amr/fabrics"
 keywords = ["robotics", "motion-planning", "geometry"]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.10"
-casadi = "^3.5.4,!=3.5.5.post1,!=3.5.5.post1,<3.6.0"
+casadi = "^3.6"
 numpy = "^1.15.3"
 geomdl = "^5.3.1"
 pyquaternion = "^0.9.9"
 pickle-mixin = "^1.0.2"
 quaternionic = "^1.0.0"
-forwardkinematics = "^1.0"
-mpscenes = "^0.3"
+forwardkinematics = "^1"
+mpscenes = "^0.4"
 pynput = "^1.7.6"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.13.4"
 pytest = "^6.2.5"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.tutorials]
 optional = true
 
 [tool.poetry.group.tutorials.dependencies]
-planarenvs = "^1.3.2"
+planarenvs = "^1.4"
 matplotlib = "^3.7.0"
 jupyterlab = "^3.6.1"
 
 [tool.poetry.group.agents]
 optional = true
 
 [tool.poetry.group.agents.dependencies]
-urdfenvs = "^0.7.6"
-planarenvs = "^1.3.3"
+#urdfenvs = "^0.8"
+planarenvs = "^1.4"
+urdfenvs = {git = "https://github.com/maxspahn/gym_envs_urdf.git", rev = "develop"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fabrics-0.7.4/PKG-INFO` & `fabrics-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: fabrics
-Version: 0.7.4
+Version: 0.8.2
 Summary: Optimization fabrics in python.
 Home-page: https://tud-amr/fabrics
 License: GPL-3.0-or-later
 Keywords: robotics,motion-planning,geometry
 Author: Max Spahn
 Author-email: m.spahn@tudelft.nl
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: casadi (>=3.5.4,<4.0.0,!=3.5.5.post1,!=3.5.5.post1,<3.6.0)
-Requires-Dist: forwardkinematics (>=1.0,<2.0)
+Requires-Dist: casadi (>=3.6,<4.0)
+Requires-Dist: forwardkinematics (>=1,<2)
 Requires-Dist: geomdl (>=5.3.1,<6.0.0)
-Requires-Dist: mpscenes (>=0.3,<0.4)
+Requires-Dist: mpscenes (>=0.4,<0.5)
 Requires-Dist: numpy (>=1.15.3,<2.0.0)
 Requires-Dist: pickle-mixin (>=1.0.2,<2.0.0)
 Requires-Dist: pynput (>=1.7.6,<2.0.0)
 Requires-Dist: pyquaternion (>=0.9.9,<0.10.0)
 Requires-Dist: quaternionic (>=1.0.0,<2.0.0)
 Project-URL: Repository, https://tud-amr/fabrics
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: fabrics Version: 0.7.4 Summary: Optimization
+Metadata-Version: 2.1 Name: fabrics Version: 0.8.2 Summary: Optimization
 fabrics in python. Home-page: https://tud-amr/fabrics License: GPL-3.0-or-later
 Keywords: robotics,motion-planning,geometry Author: Max Spahn Author-email:
 m.spahn@tudelft.nl Requires-Python: >=3.8,<3.10 Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Requires-Dist: casadi
-(>=3.5.4,<4.0.0,!=3.5.5.post1,!=3.5.5.post1,<3.6.0) Requires-Dist:
-forwardkinematics (>=1.0,<2.0) Requires-Dist: geomdl (>=5.3.1,<6.0.0) Requires-
-Dist: mpscenes (>=0.3,<0.4) Requires-Dist: numpy (>=1.15.3,<2.0.0) Requires-
-Dist: pickle-mixin (>=1.0.2,<2.0.0) Requires-Dist: pynput (>=1.7.6,<2.0.0)
-Requires-Dist: pyquaternion (>=0.9.9,<0.10.0) Requires-Dist: quaternionic
-(>=1.0.0,<2.0.0) Project-URL: Repository, https://tud-amr/fabrics Description-
-Content-Type: text/markdown # (Geometric) Fabrics [![Build and Agents](https://
-github.com/maxspahn/fabrics/actions/workflows/diffGeo_agents.yml/badge.svg)]
-(https://github.com/maxspahn/fabrics/actions/workflows/diffGeo_agents.yml) [!
-[Build and Unittest](https://github.com/maxspahn/fabrics/actions/workflows/
-unitTest.yml/badge.svg)](https://github.com/maxspahn/fabrics/actions/workflows/
-unitTest.yml) **Note on development** > This project is still under heavy
-development and there is a lack of > documentation. I, @maxspahn, am committed
-to improve and maintain that package. > However, I rely on people like you to
-point me to issues and unclear sections of > the code. So feel free to leave
-issues whenever something bugs you. **Fabrics ros-wrapper** > The fabrics-ros
-wrapper will be released very shortly when compatibility is > verified.
-Geometric Fabrics represent a geometric approach to motion generation for
-various robot structures. The idea is a next development step after Riemannian
-Motion Policies and offers increased stability and accessibility.
+(>=3.6,<4.0) Requires-Dist: forwardkinematics (>=1,<2) Requires-Dist: geomdl
+(>=5.3.1,<6.0.0) Requires-Dist: mpscenes (>=0.4,<0.5) Requires-Dist: numpy
+(>=1.15.3,<2.0.0) Requires-Dist: pickle-mixin (>=1.0.2,<2.0.0) Requires-Dist:
+pynput (>=1.7.6,<2.0.0) Requires-Dist: pyquaternion (>=0.9.9,<0.10.0) Requires-
+Dist: quaternionic (>=1.0.0,<2.0.0) Project-URL: Repository, https://tud-amr/
+fabrics Description-Content-Type: text/markdown # (Geometric) Fabrics [![Build
+and Agents](https://github.com/maxspahn/fabrics/actions/workflows/
+diffGeo_agents.yml/badge.svg)](https://github.com/maxspahn/fabrics/actions/
+workflows/diffGeo_agents.yml) [![Build and Unittest](https://github.com/
+maxspahn/fabrics/actions/workflows/unitTest.yml/badge.svg)](https://github.com/
+maxspahn/fabrics/actions/workflows/unitTest.yml) **Note on development** > This
+project is still under heavy development and there is a lack of >
+documentation. I, @maxspahn, am committed to improve and maintain that package.
+> However, I rely on people like you to point me to issues and unclear sections
+of > the code. So feel free to leave issues whenever something bugs you.
+**Fabrics ros-wrapper** > The fabrics-ros wrapper will be released very shortly
+when compatibility is > verified. Geometric Fabrics represent a geometric
+approach to motion generation for various robot structures. The idea is a next
+development step after Riemannian Motion Policies and offers increased
+stability and accessibility.
 Holonomic robots Non-Holonomic robots
 [1]              [1]
 [1]              [1]
 [1]
 ## Installation Install the package through pip, using ```bash pip3 install "."
 ``` or from PyPI using ```bash pip3 install fabrics ``` Options are [agents]
 and [tutorials]. Those can be installed using ``` pip3 install ".[agents]" pip3
```

