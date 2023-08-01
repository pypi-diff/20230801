# Comparing `tmp/bvhio-1.3.4.tar.gz` & `tmp/bvhio-1.3.6.tar.gz`

## Comparing `bvhio-1.3.4.tar` & `bvhio-1.3.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bvhio-1.3.4/.flake8
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 bvhio-1.3.4/CITATION.cff
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bvhio-1.3.4/changelog.txt
--rw-r--r--   0        0        0    16571 2020-02-02 00:00:00.000000 bvhio-1.3.4/test.ipynb
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 bvhio-1.3.4/.github/workflows/build_main.yml
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 bvhio-1.3.4/.github/workflows/build_preview.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/__init__.py
--rw-r--r--   0        0        0    13640 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/lib/Parser.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/lib/bvh/BvhContainer.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/lib/bvh/BvhJoint.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/lib/bvh/__init__.py
--rw-r--r--   0        0        0    17687 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/lib/hierarchy/Joint.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/lib/hierarchy/__init__.py
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/tests/example.bvh
--rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/tests/test_bvh.py
--rw-r--r--   0        0        0    22186 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/tests/test_hierarchy.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/tests/test_io.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 bvhio-1.3.4/bvhio/tests/utils.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bvhio-1.3.4/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 bvhio-1.3.4/LICENSE
--rw-r--r--   0        0        0    18002 2020-02-02 00:00:00.000000 bvhio-1.3.4/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 bvhio-1.3.4/pyproject.toml
--rw-r--r--   0        0        0    18635 2020-02-02 00:00:00.000000 bvhio-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bvhio-1.3.6/.flake8
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 bvhio-1.3.6/CITATION.cff
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bvhio-1.3.6/changelog.txt
+-rw-r--r--   0        0        0    16571 2020-02-02 00:00:00.000000 bvhio-1.3.6/test.ipynb
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 bvhio-1.3.6/.github/workflows/build_main.yml
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 bvhio-1.3.6/.github/workflows/build_preview.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 bvhio-1.3.6/bvhio/__init__.py
+-rw-r--r--   0        0        0    13640 2020-02-02 00:00:00.000000 bvhio-1.3.6/bvhio/lib/Parser.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 bvhio-1.3.6/bvhio/lib/bvh/BvhContainer.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 bvhio-1.3.6/bvhio/lib/bvh/BvhJoint.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 bvhio-1.3.6/bvhio/lib/bvh/__init__.py
+-rw-r--r--   0        0        0    17687 2020-02-02 00:00:00.000000 bvhio-1.3.6/bvhio/lib/hierarchy/Joint.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bvhio-1.3.6/bvhio/lib/hierarchy/__init__.py
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 bvhio-1.3.6/bvhio/tests/example.bvh
+-rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 bvhio-1.3.6/bvhio/tests/test_bvh.py
+-rw-r--r--   0        0        0    22186 2020-02-02 00:00:00.000000 bvhio-1.3.6/bvhio/tests/test_hierarchy.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 bvhio-1.3.6/bvhio/tests/test_io.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 bvhio-1.3.6/bvhio/tests/utils.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bvhio-1.3.6/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 bvhio-1.3.6/LICENSE
+-rw-r--r--   0        0        0    18069 2020-02-02 00:00:00.000000 bvhio-1.3.6/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 bvhio-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0    18702 2020-02-02 00:00:00.000000 bvhio-1.3.6/PKG-INFO
```

### Comparing `bvhio-1.3.4/test.ipynb` & `bvhio-1.3.6/test.ipynb`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.4/.github/workflows/build_main.yml` & `bvhio-1.3.6/.github/workflows/build_main.yml`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.4/.github/workflows/build_preview.yml` & `bvhio-1.3.6/.github/workflows/build_preview.yml`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.4/bvhio/lib/Parser.py` & `bvhio-1.3.6/bvhio/lib/Parser.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.4/bvhio/lib/bvh/BvhContainer.py` & `bvhio-1.3.6/bvhio/lib/bvh/BvhContainer.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.4/bvhio/lib/bvh/BvhJoint.py` & `bvhio-1.3.6/bvhio/lib/bvh/BvhJoint.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.4/bvhio/lib/hierarchy/Joint.py` & `bvhio-1.3.6/bvhio/lib/hierarchy/Joint.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.4/bvhio/tests/example.bvh` & `bvhio-1.3.6/bvhio/tests/example.bvh`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.4/bvhio/tests/test_bvh.py` & `bvhio-1.3.6/bvhio/tests/test_bvh.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.4/bvhio/tests/test_hierarchy.py` & `bvhio-1.3.6/bvhio/tests/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.4/bvhio/tests/test_io.py` & `bvhio-1.3.6/bvhio/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.4/bvhio/tests/utils.py` & `bvhio-1.3.6/bvhio/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.4/LICENSE` & `bvhio-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.4/README.md` & `bvhio-1.3.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 
 ## Why and intention
 This libary is a side product of my master thesis, in order to extract conveniently local and world data features from a humanoid skeleton hierarchy. I could not find any libary that could do that, without bloat or the features I required for extraction or modification.
 
 ## Notes
 - The package [spatial-transform](https://github.com/Wasserwecken/spatial-transform) is used as base object for joints and provides the most properties and methods.
 - The package [PyGLM](https://github.com/Zuzu-Typ/PyGLM) is used for matrix, quaternion and vector calculations.
-- Same coordination space as [openGL and GLM](https://www.evl.uic.edu/ralph/508S98/coordinates.html) is used. Which is: Right-Handed, - Y+ is up, Z- is forward and positive rotations are counter clockwise.
+- Same coordination space as [openGL and GLM](https://www.evl.uic.edu/ralph/508S98/coordinates.html) is used, which is right-handed, where Y+ is up and Z- is forward.
+- Positive rotations are counter clockwise when viewed from the origin looking in the positive direction.
 
 ## Features
 - Read/Write/Edit
     - Read and write .bvh files as simplified structure (`BvhJoint`).
     - Read and write .bvh files as transform hierarchy (`Joint`).
     - Animation data can be modified with both methods.
     - The transform hierarchy allows for easy modifications of rest and motion data.
```

#### html2text {}

```diff
@@ -20,69 +20,69 @@
 features from a humanoid skeleton hierarchy. I could not find any libary that
 could do that, without bloat or the features I required for extraction or
 modification. ## Notes - The package [spatial-transform](https://github.com/
 Wasserwecken/spatial-transform) is used as base object for joints and provides
 the most properties and methods. - The package [PyGLM](https://github.com/Zuzu-
 Typ/PyGLM) is used for matrix, quaternion and vector calculations. - Same
 coordination space as [openGL and GLM](https://www.evl.uic.edu/ralph/508S98/
-coordinates.html) is used. Which is: Right-Handed, - Y+ is up, Z- is forward
-and positive rotations are counter clockwise. ## Features - Read/Write/Edit -
-Read and write .bvh files as simplified structure (`BvhJoint`). - Read and
-write .bvh files as transform hierarchy (`Joint`). - Animation data can be
-modified with both methods. - The transform hierarchy allows for easy
-modifications of rest and motion data. - Animation - Supports modifing
-keyframe, rest positon and final pose data. - Supports joint special
-modifications, like changing the joint-roll - Keyframes are stored in local
-space and as difference to the rest pose. - Keyframes support Position,
-Rotation and Scale. - Python - Every method is documented in code with
-docstrings. - Every method has type hinting. - ([Fluent Interface](https://
-de.wikipedia.org/wiki/Fluent_Interface)) design. ## Examples ### Read bvh as
-transform hierarchy ```python import bvhio # Reads the file into a transform
-tree structure and converts all data to build proper local and world spaces. #
-This structure allows for extensive read of properties and spaces and does also
-support modifications of the animation. root = bvhio.readAsHierarchy('bvhio/
-tests/example.bvh') root.printTree() # load rest pose and print data
-root.loadRestPose(recursive=True) print('\nRest pose position and Y-direction
-of each joint in world space ') for joint, index, depth in root.layout(): print
-(f'{joint.PositionWorld} {joint.UpWorld} {joint.Name}') # ---------------------
------- OUTPUT --------------------------- # Hips # +- Chest # | +- Neck # | |
-+- Head # | +- LeftCollar # | | +- LeftUpArm # | | +- LeftLowArm # | | +-
-LeftHand # | +- RightCollar # | +- RightUpArm # | +- RightLowArm # | +-
-RightHand # +- LeftUpLeg # | +- LeftLowLeg # | +- LeftFoot # +- RightUpLeg # +-
-RightLowLeg # +- RightFoot # Rest pose position and Y-direction of each joint
-in world space # vec3( 0, 0, 0 ) vec3( 0, 1, 0 ) Hips # vec3( 0, 5.21, 0 ) vec3
-( 0, 0.997333, 0.0729792 ) Chest # vec3( 0, 23.86, 1.19209e-07 ) vec3( 0, 1, 0
-) Neck # vec3( 0, 29.31, 1.19209e-07 ) vec3( 0, 1, 0 ) Head # vec3( 1.12,
-21.44, 1.87 ) vec3( 1, 5.96046e-08, 0 ) LeftCollar # vec3( 6.66, 21.44, 1.87 )
-vec3( 0, -1, 0 ) LeftUpArm # vec3( 6.66, 9.48, 1.87 ) vec3( 0, -1, 0 )
-LeftLowArm # vec3( 6.66, -0.450002, 1.87 ) vec3( 0, -1, 0 ) LeftHand # vec3( -
-1.12, 21.44, 1.87 ) vec3( -1, 5.96046e-08, 0 ) RightCollar # vec3( -7.19,
-21.44, 1.87 ) vec3( 0, -1, 0 ) RightUpArm # vec3( -7.19, 9.62, 1.87 ) vec3( 0,
--1, 0 ) RightLowArm # vec3( -7.19, -1.03, 1.87 ) vec3( 0, -1, 0 ) RightHand #
-vec3( 3.91, 0, 0 ) vec3( 0, -1, 0 ) LeftUpLeg # vec3( 3.91, -18.34, 0 ) vec3
-( 0, -1, 0 ) LeftLowLeg # vec3( 3.91, -35.71, 0 ) vec3( 0, -1, 0 ) LeftFoot #
-vec3( -3.91, 0, 0 ) vec3( 0, -1, 0 ) RightUpLeg # vec3( -3.91, -17.63, 0 ) vec3
-( 0, -1, 0 ) RightLowLeg # vec3( -3.91, -34.77, 0 ) vec3( 0, -1, 0 ) RightFoot
-``` ### Read bvh as simple structure ```python import bvhio # Reads the file
-into a deserialized tree structure. bvh = bvhio.readAsBvh('bvhio/tests/
-example.bvh') print(f'Root: {bvh.Root}') print(f'Frames: {bvh.FrameCount}')
-print(f'Frame time: {bvh.FrameTime}') # Properties of joints in the bvh tree
-structure. bvh.Root.Name bvh.Root.Offset bvh.Root.Channels bvh.Root.EndSite
-bvh.Root.Keyframes bvh.Root.Children # Calculated properties that depend on the
-hierarchy. bvh.Root.getRotation() bvh.Root.getLength() bvh.Root.getTip() # ----
------------------------ OUTPUT --------------------------- # Root: Hips #
-Frames: 2 # Frame time: 0.033333 ``` ### bvhio joint properties and methods
-```python import bvhio # The 'Joint' object allows for reading and modifing
-animations. # Most of the functionality is based on the package 'spatial-
-transform'. hierarchy = bvhio.readAsHierarchy('bvhio/tests/example.bvh') #
-joints from the hierarchy can be selected by their name joint =
-hierarchy.filter('Head')[0] # Some methods and properties have been added to
-work with keyframe and joint data joint.Keyframes # list of local animation
-data joint.loadPose(0) # sets the transform data to a specific keyframe
-joint.writePose(0) # writes the current transform data into a keyframe
+coordinates.html) is used, which is right-handed, where Y+ is up and Z- is
+forward. - Positive rotations are counter clockwise when viewed from the origin
+looking in the positive direction. ## Features - Read/Write/Edit - Read and
+write .bvh files as simplified structure (`BvhJoint`). - Read and write .bvh
+files as transform hierarchy (`Joint`). - Animation data can be modified with
+both methods. - The transform hierarchy allows for easy modifications of rest
+and motion data. - Animation - Supports modifing keyframe, rest positon and
+final pose data. - Supports joint special modifications, like changing the
+joint-roll - Keyframes are stored in local space and as difference to the rest
+pose. - Keyframes support Position, Rotation and Scale. - Python - Every method
+is documented in code with docstrings. - Every method has type hinting. - (
+[Fluent Interface](https://de.wikipedia.org/wiki/Fluent_Interface)) design. ##
+Examples ### Read bvh as transform hierarchy ```python import bvhio # Reads the
+file into a transform tree structure and converts all data to build proper
+local and world spaces. # This structure allows for extensive read of
+properties and spaces and does also support modifications of the animation.
+root = bvhio.readAsHierarchy('bvhio/tests/example.bvh') root.printTree() # load
+rest pose and print data root.loadRestPose(recursive=True) print('\nRest pose
+position and Y-direction of each joint in world space ') for joint, index,
+depth in root.layout(): print(f'{joint.PositionWorld} {joint.UpWorld}
+{joint.Name}') # --------------------------- OUTPUT --------------------------
+- # Hips # +- Chest # | +- Neck # | | +- Head # | +- LeftCollar # | | +-
+LeftUpArm # | | +- LeftLowArm # | | +- LeftHand # | +- RightCollar # | +-
+RightUpArm # | +- RightLowArm # | +- RightHand # +- LeftUpLeg # | +- LeftLowLeg
+# | +- LeftFoot # +- RightUpLeg # +- RightLowLeg # +- RightFoot # Rest pose
+position and Y-direction of each joint in world space # vec3( 0, 0, 0 ) vec3
+( 0, 1, 0 ) Hips # vec3( 0, 5.21, 0 ) vec3( 0, 0.997333, 0.0729792 ) Chest #
+vec3( 0, 23.86, 1.19209e-07 ) vec3( 0, 1, 0 ) Neck # vec3( 0, 29.31, 1.19209e-
+07 ) vec3( 0, 1, 0 ) Head # vec3( 1.12, 21.44, 1.87 ) vec3( 1, 5.96046e-08, 0 )
+LeftCollar # vec3( 6.66, 21.44, 1.87 ) vec3( 0, -1, 0 ) LeftUpArm # vec3( 6.66,
+9.48, 1.87 ) vec3( 0, -1, 0 ) LeftLowArm # vec3( 6.66, -0.450002, 1.87 ) vec3
+( 0, -1, 0 ) LeftHand # vec3( -1.12, 21.44, 1.87 ) vec3( -1, 5.96046e-08, 0 )
+RightCollar # vec3( -7.19, 21.44, 1.87 ) vec3( 0, -1, 0 ) RightUpArm # vec3( -
+7.19, 9.62, 1.87 ) vec3( 0, -1, 0 ) RightLowArm # vec3( -7.19, -1.03, 1.87 )
+vec3( 0, -1, 0 ) RightHand # vec3( 3.91, 0, 0 ) vec3( 0, -1, 0 ) LeftUpLeg #
+vec3( 3.91, -18.34, 0 ) vec3( 0, -1, 0 ) LeftLowLeg # vec3( 3.91, -35.71, 0 )
+vec3( 0, -1, 0 ) LeftFoot # vec3( -3.91, 0, 0 ) vec3( 0, -1, 0 ) RightUpLeg #
+vec3( -3.91, -17.63, 0 ) vec3( 0, -1, 0 ) RightLowLeg # vec3( -3.91, -34.77, 0
+) vec3( 0, -1, 0 ) RightFoot ``` ### Read bvh as simple structure ```python
+import bvhio # Reads the file into a deserialized tree structure. bvh =
+bvhio.readAsBvh('bvhio/tests/example.bvh') print(f'Root: {bvh.Root}') print
+(f'Frames: {bvh.FrameCount}') print(f'Frame time: {bvh.FrameTime}') #
+Properties of joints in the bvh tree structure. bvh.Root.Name bvh.Root.Offset
+bvh.Root.Channels bvh.Root.EndSite bvh.Root.Keyframes bvh.Root.Children #
+Calculated properties that depend on the hierarchy. bvh.Root.getRotation()
+bvh.Root.getLength() bvh.Root.getTip() # --------------------------- OUTPUT ---
+------------------------ # Root: Hips # Frames: 2 # Frame time: 0.033333 ```
+### bvhio joint properties and methods ```python import bvhio # The 'Joint'
+object allows for reading and modifing animations. # Most of the functionality
+is based on the package 'spatial-transform'. hierarchy = bvhio.readAsHierarchy
+('bvhio/tests/example.bvh') # joints from the hierarchy can be selected by
+their name joint = hierarchy.filter('Head')[0] # Some methods and properties
+have been added to work with keyframe and joint data joint.Keyframes # list of
+local animation data joint.loadPose(0) # sets the transform data to a specific
+keyframe joint.writePose(0) # writes the current transform data into a keyframe
 joint.roll(0) # changes the rotation of a bone around its own axis without
 affcting the children # Some methods do also update the keyframes to no destroy
 the animation data # Please refer to the package 'spatial-transform' for their
 behaviour joint.clearParent() joint.clearChildren() joint.attach() joint.detach
 () joint.applyPosition() joint.applyRotation() joint.applyScale() ``` ###
 Interacting with joints and animation ```python import bvhio # The package
 allows to make modifcation on the animation data very conviniently. root =
```

### Comparing `bvhio-1.3.4/pyproject.toml` & `bvhio-1.3.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bvhio"
-version = "1.3.4"
+version = "1.3.6"
 authors = [ { name="Wasserwecken", email="author@example.com" }, ]
 description = "Read, write, edit and create .bvh files with hierarchical 3D transforms."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `bvhio-1.3.4/PKG-INFO` & `bvhio-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bvhio
-Version: 1.3.4
+Version: 1.3.6
 Summary: Read, write, edit and create .bvh files with hierarchical 3D transforms.
 Project-URL: Homepage, https://github.com/Wasserwecken/bvhio
 Project-URL: Bug Tracker, https://github.com/Wasserwecken/bvhio/issues
 Author-email: Wasserwecken <author@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,15 +35,16 @@
 
 ## Why and intention
 This libary is a side product of my master thesis, in order to extract conveniently local and world data features from a humanoid skeleton hierarchy. I could not find any libary that could do that, without bloat or the features I required for extraction or modification.
 
 ## Notes
 - The package [spatial-transform](https://github.com/Wasserwecken/spatial-transform) is used as base object for joints and provides the most properties and methods.
 - The package [PyGLM](https://github.com/Zuzu-Typ/PyGLM) is used for matrix, quaternion and vector calculations.
-- Same coordination space as [openGL and GLM](https://www.evl.uic.edu/ralph/508S98/coordinates.html) is used. Which is: Right-Handed, - Y+ is up, Z- is forward and positive rotations are counter clockwise.
+- Same coordination space as [openGL and GLM](https://www.evl.uic.edu/ralph/508S98/coordinates.html) is used, which is right-handed, where Y+ is up and Z- is forward.
+- Positive rotations are counter clockwise when viewed from the origin looking in the positive direction.
 
 ## Features
 - Read/Write/Edit
     - Read and write .bvh files as simplified structure (`BvhJoint`).
     - Read and write .bvh files as transform hierarchy (`Joint`).
     - Animation data can be modified with both methods.
     - The transform hierarchy allows for easy modifications of rest and motion data.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bvhio Version: 1.3.4 Summary: Read, write, edit and
+Metadata-Version: 2.1 Name: bvhio Version: 1.3.6 Summary: Read, write, edit and
 create .bvh files with hierarchical 3D transforms. Project-URL: Homepage,
 https://github.com/Wasserwecken/bvhio Project-URL: Bug Tracker, https://
 github.com/Wasserwecken/bvhio/issues Author-email: Wasserwecken
 example.com> License-File: LICENSE Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.7 Requires-Dist: numpy Requires-
 Dist: pyglm==2.7.0 Requires-Dist: spatial-transform==1.2.13 Description-
@@ -29,69 +29,69 @@
 features from a humanoid skeleton hierarchy. I could not find any libary that
 could do that, without bloat or the features I required for extraction or
 modification. ## Notes - The package [spatial-transform](https://github.com/
 Wasserwecken/spatial-transform) is used as base object for joints and provides
 the most properties and methods. - The package [PyGLM](https://github.com/Zuzu-
 Typ/PyGLM) is used for matrix, quaternion and vector calculations. - Same
 coordination space as [openGL and GLM](https://www.evl.uic.edu/ralph/508S98/
-coordinates.html) is used. Which is: Right-Handed, - Y+ is up, Z- is forward
-and positive rotations are counter clockwise. ## Features - Read/Write/Edit -
-Read and write .bvh files as simplified structure (`BvhJoint`). - Read and
-write .bvh files as transform hierarchy (`Joint`). - Animation data can be
-modified with both methods. - The transform hierarchy allows for easy
-modifications of rest and motion data. - Animation - Supports modifing
-keyframe, rest positon and final pose data. - Supports joint special
-modifications, like changing the joint-roll - Keyframes are stored in local
-space and as difference to the rest pose. - Keyframes support Position,
-Rotation and Scale. - Python - Every method is documented in code with
-docstrings. - Every method has type hinting. - ([Fluent Interface](https://
-de.wikipedia.org/wiki/Fluent_Interface)) design. ## Examples ### Read bvh as
-transform hierarchy ```python import bvhio # Reads the file into a transform
-tree structure and converts all data to build proper local and world spaces. #
-This structure allows for extensive read of properties and spaces and does also
-support modifications of the animation. root = bvhio.readAsHierarchy('bvhio/
-tests/example.bvh') root.printTree() # load rest pose and print data
-root.loadRestPose(recursive=True) print('\nRest pose position and Y-direction
-of each joint in world space ') for joint, index, depth in root.layout(): print
-(f'{joint.PositionWorld} {joint.UpWorld} {joint.Name}') # ---------------------
------- OUTPUT --------------------------- # Hips # +- Chest # | +- Neck # | |
-+- Head # | +- LeftCollar # | | +- LeftUpArm # | | +- LeftLowArm # | | +-
-LeftHand # | +- RightCollar # | +- RightUpArm # | +- RightLowArm # | +-
-RightHand # +- LeftUpLeg # | +- LeftLowLeg # | +- LeftFoot # +- RightUpLeg # +-
-RightLowLeg # +- RightFoot # Rest pose position and Y-direction of each joint
-in world space # vec3( 0, 0, 0 ) vec3( 0, 1, 0 ) Hips # vec3( 0, 5.21, 0 ) vec3
-( 0, 0.997333, 0.0729792 ) Chest # vec3( 0, 23.86, 1.19209e-07 ) vec3( 0, 1, 0
-) Neck # vec3( 0, 29.31, 1.19209e-07 ) vec3( 0, 1, 0 ) Head # vec3( 1.12,
-21.44, 1.87 ) vec3( 1, 5.96046e-08, 0 ) LeftCollar # vec3( 6.66, 21.44, 1.87 )
-vec3( 0, -1, 0 ) LeftUpArm # vec3( 6.66, 9.48, 1.87 ) vec3( 0, -1, 0 )
-LeftLowArm # vec3( 6.66, -0.450002, 1.87 ) vec3( 0, -1, 0 ) LeftHand # vec3( -
-1.12, 21.44, 1.87 ) vec3( -1, 5.96046e-08, 0 ) RightCollar # vec3( -7.19,
-21.44, 1.87 ) vec3( 0, -1, 0 ) RightUpArm # vec3( -7.19, 9.62, 1.87 ) vec3( 0,
--1, 0 ) RightLowArm # vec3( -7.19, -1.03, 1.87 ) vec3( 0, -1, 0 ) RightHand #
-vec3( 3.91, 0, 0 ) vec3( 0, -1, 0 ) LeftUpLeg # vec3( 3.91, -18.34, 0 ) vec3
-( 0, -1, 0 ) LeftLowLeg # vec3( 3.91, -35.71, 0 ) vec3( 0, -1, 0 ) LeftFoot #
-vec3( -3.91, 0, 0 ) vec3( 0, -1, 0 ) RightUpLeg # vec3( -3.91, -17.63, 0 ) vec3
-( 0, -1, 0 ) RightLowLeg # vec3( -3.91, -34.77, 0 ) vec3( 0, -1, 0 ) RightFoot
-``` ### Read bvh as simple structure ```python import bvhio # Reads the file
-into a deserialized tree structure. bvh = bvhio.readAsBvh('bvhio/tests/
-example.bvh') print(f'Root: {bvh.Root}') print(f'Frames: {bvh.FrameCount}')
-print(f'Frame time: {bvh.FrameTime}') # Properties of joints in the bvh tree
-structure. bvh.Root.Name bvh.Root.Offset bvh.Root.Channels bvh.Root.EndSite
-bvh.Root.Keyframes bvh.Root.Children # Calculated properties that depend on the
-hierarchy. bvh.Root.getRotation() bvh.Root.getLength() bvh.Root.getTip() # ----
------------------------ OUTPUT --------------------------- # Root: Hips #
-Frames: 2 # Frame time: 0.033333 ``` ### bvhio joint properties and methods
-```python import bvhio # The 'Joint' object allows for reading and modifing
-animations. # Most of the functionality is based on the package 'spatial-
-transform'. hierarchy = bvhio.readAsHierarchy('bvhio/tests/example.bvh') #
-joints from the hierarchy can be selected by their name joint =
-hierarchy.filter('Head')[0] # Some methods and properties have been added to
-work with keyframe and joint data joint.Keyframes # list of local animation
-data joint.loadPose(0) # sets the transform data to a specific keyframe
-joint.writePose(0) # writes the current transform data into a keyframe
+coordinates.html) is used, which is right-handed, where Y+ is up and Z- is
+forward. - Positive rotations are counter clockwise when viewed from the origin
+looking in the positive direction. ## Features - Read/Write/Edit - Read and
+write .bvh files as simplified structure (`BvhJoint`). - Read and write .bvh
+files as transform hierarchy (`Joint`). - Animation data can be modified with
+both methods. - The transform hierarchy allows for easy modifications of rest
+and motion data. - Animation - Supports modifing keyframe, rest positon and
+final pose data. - Supports joint special modifications, like changing the
+joint-roll - Keyframes are stored in local space and as difference to the rest
+pose. - Keyframes support Position, Rotation and Scale. - Python - Every method
+is documented in code with docstrings. - Every method has type hinting. - (
+[Fluent Interface](https://de.wikipedia.org/wiki/Fluent_Interface)) design. ##
+Examples ### Read bvh as transform hierarchy ```python import bvhio # Reads the
+file into a transform tree structure and converts all data to build proper
+local and world spaces. # This structure allows for extensive read of
+properties and spaces and does also support modifications of the animation.
+root = bvhio.readAsHierarchy('bvhio/tests/example.bvh') root.printTree() # load
+rest pose and print data root.loadRestPose(recursive=True) print('\nRest pose
+position and Y-direction of each joint in world space ') for joint, index,
+depth in root.layout(): print(f'{joint.PositionWorld} {joint.UpWorld}
+{joint.Name}') # --------------------------- OUTPUT --------------------------
+- # Hips # +- Chest # | +- Neck # | | +- Head # | +- LeftCollar # | | +-
+LeftUpArm # | | +- LeftLowArm # | | +- LeftHand # | +- RightCollar # | +-
+RightUpArm # | +- RightLowArm # | +- RightHand # +- LeftUpLeg # | +- LeftLowLeg
+# | +- LeftFoot # +- RightUpLeg # +- RightLowLeg # +- RightFoot # Rest pose
+position and Y-direction of each joint in world space # vec3( 0, 0, 0 ) vec3
+( 0, 1, 0 ) Hips # vec3( 0, 5.21, 0 ) vec3( 0, 0.997333, 0.0729792 ) Chest #
+vec3( 0, 23.86, 1.19209e-07 ) vec3( 0, 1, 0 ) Neck # vec3( 0, 29.31, 1.19209e-
+07 ) vec3( 0, 1, 0 ) Head # vec3( 1.12, 21.44, 1.87 ) vec3( 1, 5.96046e-08, 0 )
+LeftCollar # vec3( 6.66, 21.44, 1.87 ) vec3( 0, -1, 0 ) LeftUpArm # vec3( 6.66,
+9.48, 1.87 ) vec3( 0, -1, 0 ) LeftLowArm # vec3( 6.66, -0.450002, 1.87 ) vec3
+( 0, -1, 0 ) LeftHand # vec3( -1.12, 21.44, 1.87 ) vec3( -1, 5.96046e-08, 0 )
+RightCollar # vec3( -7.19, 21.44, 1.87 ) vec3( 0, -1, 0 ) RightUpArm # vec3( -
+7.19, 9.62, 1.87 ) vec3( 0, -1, 0 ) RightLowArm # vec3( -7.19, -1.03, 1.87 )
+vec3( 0, -1, 0 ) RightHand # vec3( 3.91, 0, 0 ) vec3( 0, -1, 0 ) LeftUpLeg #
+vec3( 3.91, -18.34, 0 ) vec3( 0, -1, 0 ) LeftLowLeg # vec3( 3.91, -35.71, 0 )
+vec3( 0, -1, 0 ) LeftFoot # vec3( -3.91, 0, 0 ) vec3( 0, -1, 0 ) RightUpLeg #
+vec3( -3.91, -17.63, 0 ) vec3( 0, -1, 0 ) RightLowLeg # vec3( -3.91, -34.77, 0
+) vec3( 0, -1, 0 ) RightFoot ``` ### Read bvh as simple structure ```python
+import bvhio # Reads the file into a deserialized tree structure. bvh =
+bvhio.readAsBvh('bvhio/tests/example.bvh') print(f'Root: {bvh.Root}') print
+(f'Frames: {bvh.FrameCount}') print(f'Frame time: {bvh.FrameTime}') #
+Properties of joints in the bvh tree structure. bvh.Root.Name bvh.Root.Offset
+bvh.Root.Channels bvh.Root.EndSite bvh.Root.Keyframes bvh.Root.Children #
+Calculated properties that depend on the hierarchy. bvh.Root.getRotation()
+bvh.Root.getLength() bvh.Root.getTip() # --------------------------- OUTPUT ---
+------------------------ # Root: Hips # Frames: 2 # Frame time: 0.033333 ```
+### bvhio joint properties and methods ```python import bvhio # The 'Joint'
+object allows for reading and modifing animations. # Most of the functionality
+is based on the package 'spatial-transform'. hierarchy = bvhio.readAsHierarchy
+('bvhio/tests/example.bvh') # joints from the hierarchy can be selected by
+their name joint = hierarchy.filter('Head')[0] # Some methods and properties
+have been added to work with keyframe and joint data joint.Keyframes # list of
+local animation data joint.loadPose(0) # sets the transform data to a specific
+keyframe joint.writePose(0) # writes the current transform data into a keyframe
 joint.roll(0) # changes the rotation of a bone around its own axis without
 affcting the children # Some methods do also update the keyframes to no destroy
 the animation data # Please refer to the package 'spatial-transform' for their
 behaviour joint.clearParent() joint.clearChildren() joint.attach() joint.detach
 () joint.applyPosition() joint.applyRotation() joint.applyScale() ``` ###
 Interacting with joints and animation ```python import bvhio # The package
 allows to make modifcation on the animation data very conviniently. root =
```

