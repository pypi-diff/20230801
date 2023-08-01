# Comparing `tmp/rria_api-1.0.4.tar.gz` & `tmp/rria_api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rria_api-1.0.4.tar", max compression
+gzip compressed data, was "rria_api-1.0.5.tar", max compression
```

## Comparing `rria_api-1.0.4.tar` & `rria_api-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1449 2023-01-05 17:07:24.285582 rria_api-1.0.4/README.md
--rw-r--r--   0        0        0      346 2023-01-05 17:07:39.149907 rria_api-1.0.4/pyproject.toml
--rw-r--r--   0        0        0       28 2023-01-04 12:13:33.103134 rria_api-1.0.4/rria_api/__init__.py
--rw-r--r--   0        0        0     1277 2023-01-03 16:51:38.580736 rria_api-1.0.4/rria_api/gen3/action_gen3.py
--rw-r--r--   0        0        0     1516 2023-01-03 16:51:38.580736 rria_api-1.0.4/rria_api/gen3/api_gen3/device_connection.py
--rw-r--r--   0        0        0     7670 2023-01-03 16:51:38.580736 rria_api-1.0.4/rria_api/gen3/api_gen3/gen3_api.py
--rw-r--r--   0        0        0      617 2023-01-03 16:51:38.580736 rria_api-1.0.4/rria_api/gen3/connect_gen3.py
--rw-r--r--   0        0        0     1299 2023-01-03 16:51:38.580736 rria_api-1.0.4/rria_api/ned/action_ned.py
--rw-r--r--   0        0        0      346 2023-01-03 16:51:38.580736 rria_api-1.0.4/rria_api/ned/connect_ned.py
--rw-r--r--   0        0        0    21787 2023-01-03 16:51:38.580736 rria_api-1.0.4/rria_api/poetry.lock
--rw-r--r--   0        0        0    10467 2023-01-04 17:17:53.023216 rria_api-1.0.4/rria_api/robot_facade.py
--rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 rria_api-1.0.4/setup.py
--rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 rria_api-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      848 2023-08-01 19:29:35.064063 rria_api-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1509 2023-04-10 17:18:59.252547 rria_api-1.0.5/README.md
+-rw-r--r--   0        0        0       29 2023-04-10 17:18:59.257980 rria_api-1.0.5/rria_api/__init__.py
+-rw-r--r--   0        0        0     1321 2023-03-24 11:48:25.776937 rria_api-1.0.5/rria_api/gen3/action_gen3.py
+-rw-r--r--   0        0        0     1559 2023-03-24 11:48:25.778442 rria_api-1.0.5/rria_api/gen3/api_gen3/device_connection.py
+-rw-r--r--   0        0        0     7947 2023-08-01 19:28:24.939682 rria_api-1.0.5/rria_api/gen3/api_gen3/gen3_api.py
+-rw-r--r--   0        0        0      637 2023-03-24 11:48:25.778442 rria_api-1.0.5/rria_api/gen3/connect_gen3.py
+-rw-r--r--   0        0        0     1342 2023-03-24 11:48:25.779454 rria_api-1.0.5/rria_api/ned/action_ned.py
+-rw-r--r--   0        0        0      360 2023-03-24 11:48:25.779454 rria_api-1.0.5/rria_api/ned/connect_ned.py
+-rw-r--r--   0        0        0    22047 2023-04-10 17:18:59.258978 rria_api-1.0.5/rria_api/poetry.lock
+-rw-r--r--   0        0        0    10829 2023-04-10 17:18:59.258978 rria_api-1.0.5/rria_api/robot_facade.py
+-rw-r--r--   0        0        0     2016 1970-01-01 00:00:00.000000 rria_api-1.0.5/PKG-INFO
```

### Comparing `rria_api-1.0.4/README.md` & `rria_api-1.0.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: rria-api
+Version: 1.0.5
+Summary: 
+Author: felipeadsm
+Author-email: 97059009+felipeadsm@users.noreply.github.com
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: kortex_api @ file:///C:/Users/fasm/Documents/GitHub/rria_api/kortex_api-2.3.0.post34-py3-none-any.whl
+Requires-Dist: pyniryo (>=1.1.2,<2.0.0)
+Description-Content-Type: text/markdown
+
 # RRIA-API
 
 The `rria-api` is an easy-to-use package that provides a common interface to control robots used by the Residence in Robotics
 and AI at the UFPE's informatics center. The API currently supports the use of Kinova Gen3 lite and Niryo NED, with
 plans to support a Denso robot.
 
 ### **Requirements**
@@ -54,8 +69,8 @@
 
 gen3_lite.move_to_home()
 ned.move_to_home()
 
 gen3_lite.safe_disconnect()
 ned.safe_disconnect()
 
-```
+```
```

### Comparing `rria_api-1.0.4/rria_api/gen3/api_gen3/device_connection.py` & `rria_api-1.0.5/rria_api/gen3/api_gen3/device_connection.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from kortex_api.RouterClient import RouterClient, RouterClientSendOptions
-from kortex_api.SessionManager import SessionManager
-from kortex_api.autogen.messages import Session_pb2
-from kortex_api.TCPTransport import TCPTransport
-
-
-class DeviceConnection:
-    TCP_PORT = 10000
-
-    def __init__(self, ip_address, port=TCP_PORT, credentials=("", "")):
-        self.ip_address = ip_address
-        self.port = port
-        self.credentials = credentials
-
-        self.sessionManager = None
-
-        # Setup API
-        self.transport = TCPTransport()
-        self.router = RouterClient(self.transport, RouterClient.basicErrorCallback)
-
-    def connect(self):
-        self.transport.connect(self.ip_address, self.port)
-
-        session_info = Session_pb2.CreateSessionInfo()
-        session_info.username = self.credentials[0]
-        session_info.password = self.credentials[1]
-        session_info.session_inactivity_timeout = 10000  # (milliseconds)
-        session_info.connection_inactivity_timeout = 2000  # (milliseconds)
-
-        self.sessionManager = SessionManager(self.router)
-        print("Logging as", self.credentials[0], "on device", self.ip_address)
-        self.sessionManager.CreateSession(session_info)
-
-        return self.router
-
-    def disconnect(self):
-        if self.sessionManager is not None:
-            router_options = RouterClientSendOptions()
-            router_options.timeout_ms = 1000
-
-            self.sessionManager.CloseSession(router_options)
-
-        self.transport.disconnect()
+from kortex_api.RouterClient import RouterClient, RouterClientSendOptions
+from kortex_api.SessionManager import SessionManager
+from kortex_api.autogen.messages import Session_pb2
+from kortex_api.TCPTransport import TCPTransport
+
+
+class DeviceConnection:
+    TCP_PORT = 10000
+
+    def __init__(self, ip_address, port=TCP_PORT, credentials=("", "")):
+        self.ip_address = ip_address
+        self.port = port
+        self.credentials = credentials
+
+        self.sessionManager = None
+
+        # Setup API
+        self.transport = TCPTransport()
+        self.router = RouterClient(self.transport, RouterClient.basicErrorCallback)
+
+    def connect(self):
+        self.transport.connect(self.ip_address, self.port)
+
+        session_info = Session_pb2.CreateSessionInfo()
+        session_info.username = self.credentials[0]
+        session_info.password = self.credentials[1]
+        session_info.session_inactivity_timeout = 10000  # (milliseconds)
+        session_info.connection_inactivity_timeout = 2000  # (milliseconds)
+
+        self.sessionManager = SessionManager(self.router)
+        print("Logging as", self.credentials[0], "on device", self.ip_address)
+        self.sessionManager.CreateSession(session_info)
+
+        return self.router
+
+    def disconnect(self):
+        if self.sessionManager is not None:
+            router_options = RouterClientSendOptions()
+            router_options.timeout_ms = 1000
+
+            self.sessionManager.CloseSession(router_options)
+
+        self.transport.disconnect()
```

### Comparing `rria_api-1.0.4/rria_api/gen3/connect_gen3.py` & `rria_api-1.0.5/rria_api/gen3/connect_gen3.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from rria_api.gen3.api_gen3.device_connection import DeviceConnection
-
-
-class ConnectGen3:
-    route = None
-
-    def __init__(self, ip_address, credentials):
-        self.ip_address = ip_address
-        self.credentials = credentials
-
-        self.connect_instance = DeviceConnection(ip_address=self.ip_address,
-                                                 credentials=(credentials[0], credentials[1]))
-
-    def connect_robot(self):
-        self.route = self.connect_instance.connect()
-
-        return self.route
-
-    def disconnect_robot(self):
-        self.connect_instance = self.connect_instance.disconnect()
+from rria_api.gen3.api_gen3.device_connection import DeviceConnection
+
+
+class ConnectGen3:
+    route = None
+
+    def __init__(self, ip_address, credentials):
+        self.ip_address = ip_address
+        self.credentials = credentials
+
+        self.connect_instance = DeviceConnection(ip_address=self.ip_address,
+                                                 credentials=(credentials[0], credentials[1]))
+
+    def connect_robot(self):
+        self.route = self.connect_instance.connect()
+
+        return self.route
+
+    def disconnect_robot(self):
+        self.connect_instance = self.connect_instance.disconnect()
```

### Comparing `rria_api-1.0.4/rria_api/ned/action_ned.py` & `rria_api-1.0.5/rria_api/ned/action_ned.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import math
-
-
-class ActionNed:
-    def __init__(self, robot_object):
-        self.robot_object = robot_object
-
-    def move_joints(self, j1, j2, j3, j4, j5, j6):
-        trans = math.pi / 180
-        self.robot_object.move_joints(j1 * trans, j2 * trans, j3 * trans, j4 * trans, j5 * trans, j6 * trans)
-
-    def get_joints(self):
-        joints_rad = self.robot_object.get_joints()
-        joints_degrees = [round(joint * 180 / math.pi, 3) for joint in joints_rad]
-        return joints_degrees
-
-    def move_cartesian(self, x, y, z, roll, pitch, yaw):
-        trans = math.pi / 180
-        self.robot_object.move_pose(x, y, z, roll * trans, pitch * trans, yaw * trans)
-
-    def get_cartesian(self):
-        return self.robot_object.get_pose()
-
-    def move_to_home(self):
-        self.robot_object.move_to_home_pose()
-
-    def move_to_zero(self):
-        self.robot_object.move_joints([0.0, 0.0, 0.0, 0.0, 0.0, 0.0])
-
-    def open_gripper(self):
-        self.robot_object.release_with_tool()
-
-    def close_gripper(self):
-        self.robot_object.grasp_with_tool()
-
-    def set_velocity(self, velocity):
-        self.robot_object.set_arm_max_velocity(velocity)
-
-    def calibrate(self):
-        self.robot_object.calibrate_auto()
-
-    def go_to_sleep(self):
-        self.robot_object.go_to_sleep()
+import math
+
+
+class ActionNed:
+    def __init__(self, robot_object):
+        self.robot_object = robot_object
+
+    def move_joints(self, j1, j2, j3, j4, j5, j6):
+        trans = math.pi / 180
+        self.robot_object.move_joints(j1 * trans, j2 * trans, j3 * trans, j4 * trans, j5 * trans, j6 * trans)
+
+    def get_joints(self):
+        joints_rad = self.robot_object.get_joints()
+        joints_degrees = [round(joint * 180 / math.pi, 3) for joint in joints_rad]
+        return joints_degrees
+
+    def move_cartesian(self, x, y, z, roll, pitch, yaw):
+        trans = math.pi / 180
+        self.robot_object.move_pose(x, y, z, roll * trans, pitch * trans, yaw * trans)
+
+    def get_cartesian(self):
+        return self.robot_object.get_pose()
+
+    def move_to_home(self):
+        self.robot_object.move_to_home_pose()
+
+    def move_to_zero(self):
+        self.robot_object.move_joints([0.0, 0.0, 0.0, 0.0, 0.0, 0.0])
+
+    def open_gripper(self):
+        self.robot_object.release_with_tool()
+
+    def close_gripper(self):
+        self.robot_object.grasp_with_tool()
+
+    def set_velocity(self, velocity):
+        self.robot_object.set_arm_max_velocity(velocity)
+
+    def calibrate(self):
+        self.robot_object.calibrate_auto()
+
+    def go_to_sleep(self):
+        self.robot_object.go_to_sleep()
```

### Comparing `rria_api-1.0.4/rria_api/poetry.lock` & `rria_api-1.0.5/rria_api/poetry.lock`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,260 +1,260 @@
-# This file is automatically @generated by Poetry and should not be changed by hand.
-
-[[package]]
-name = "deprecated"
-version = "1.2.7"
-description = "Python @deprecated decorator to deprecate old python classes, functions or methods."
-category = "main"
-optional = false
-python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
-files = [
-    {file = "Deprecated-1.2.7-py2.py3-none-any.whl", hash = "sha256:8b6a5aa50e482d8244a62e5582b96c372e87e3a28e8b49c316e46b95c76a611d"},
-    {file = "Deprecated-1.2.7.tar.gz", hash = "sha256:408038ab5fdeca67554e8f6742d1521cd3cd0ee0ff9d47f29318a4f4da31c308"},
-]
-
-[package.dependencies]
-wrapt = ">=1.10,<2"
-
-[package.extras]
-dev = ["PyTest", "PyTest (<5)", "PyTest-Cov", "PyTest-Cov (<2.6)", "bumpversion (<1)", "sphinx (<2)", "tox"]
-
-[[package]]
-name = "enum34"
-version = "1.1.10"
-description = "Python 3.4 Enum backported to 3.3, 3.2, 3.1, 2.7, 2.6, 2.5, and 2.4"
-category = "main"
-optional = false
-python-versions = "*"
-files = [
-    {file = "enum34-1.1.10-py2-none-any.whl", hash = "sha256:a98a201d6de3f2ab3db284e70a33b0f896fbf35f8086594e8c9e74b909058d53"},
-    {file = "enum34-1.1.10-py3-none-any.whl", hash = "sha256:c3858660960c984d6ab0ebad691265180da2b43f07e061c0f8dca9ef3cffd328"},
-    {file = "enum34-1.1.10.tar.gz", hash = "sha256:cce6a7477ed816bd2542d03d53db9f0db935dd013b70f336a95c73979289f248"},
-]
-
-[[package]]
-name = "kortex-api"
-version = "2.3.0.post34"
-description = "Kinova kortex_api"
-category = "main"
-optional = false
-python-versions = "*"
-files = [
-    {file = "kortex_api-2.3.0.post34-py3-none-any.whl", hash = "sha256:1cffd7ca2afe4dfbe71bc9c22379c69a8d04ff197676a6902aee06a191868805"},
-]
-
-[package.dependencies]
-deprecated = "1.2.7"
-protobuf = "3.5.1"
-
-[package.source]
-type = "file"
-url = "dependencies/kortex_api-2.3.0.post34-py3-none-any.whl"
-
-[[package]]
-name = "numpy"
-version = "1.24.0"
-description = "Fundamental package for array computing in Python"
-category = "main"
-optional = false
-python-versions = ">=3.8"
-files = [
-    {file = "numpy-1.24.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:6e73a1f4f5b74a42abb55bc2b3d869f1b38cbc8776da5f8b66bf110284f7a437"},
-    {file = "numpy-1.24.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:9387c7d6d50e8f8c31e7bfc034241e9c6f4b3eb5db8d118d6487047b922f82af"},
-    {file = "numpy-1.24.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7ad6a024a32ee61d18f5b402cd02e9c0e22c0fb9dc23751991b3a16d209d972e"},
-    {file = "numpy-1.24.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:73cf2c5b5a07450f20a0c8e04d9955491970177dce8df8d6903bf253e53268e0"},
-    {file = "numpy-1.24.0-cp310-cp310-win32.whl", hash = "sha256:cec79ff3984b2d1d103183fc4a3361f5b55bbb66cb395cbf5a920a4bb1fd588d"},
-    {file = "numpy-1.24.0-cp310-cp310-win_amd64.whl", hash = "sha256:4f5e78b8b710cd7cd1a8145994cfffc6ddd5911669a437777d8cedfce6c83a98"},
-    {file = "numpy-1.24.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:4445f472b246cad6514cc09fbb5ecb7aab09ca2acc3c16f29f8dca6c468af501"},
-    {file = "numpy-1.24.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:ec3e5e8172a0a6a4f3c2e7423d4a8434c41349141b04744b11a90e017a95bad5"},
-    {file = "numpy-1.24.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f9168790149f917ad8e3cf5047b353fefef753bd50b07c547da0bdf30bc15d91"},
-    {file = "numpy-1.24.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ada6c1e9608ceadaf7020e1deea508b73ace85560a16f51bef26aecb93626a72"},
-    {file = "numpy-1.24.0-cp311-cp311-win32.whl", hash = "sha256:f3c4a9a9f92734a4728ddbd331e0124eabbc968a0359a506e8e74a9b0d2d419b"},
-    {file = "numpy-1.24.0-cp311-cp311-win_amd64.whl", hash = "sha256:90075ef2c6ac6397d0035bcd8b298b26e481a7035f7a3f382c047eb9c3414db0"},
-    {file = "numpy-1.24.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:0885d9a7666cafe5f9876c57bfee34226e2b2847bfb94c9505e18d81011e5401"},
-    {file = "numpy-1.24.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:e63d2157f9fc98cc178870db83b0e0c85acdadd598b134b00ebec9e0db57a01f"},
-    {file = "numpy-1.24.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cf8960f72997e56781eb1c2ea256a70124f92a543b384f89e5fb3503a308b1d3"},
-    {file = "numpy-1.24.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2f8e0df2ecc1928ef7256f18e309c9d6229b08b5be859163f5caa59c93d53646"},
-    {file = "numpy-1.24.0-cp38-cp38-win32.whl", hash = "sha256:fe44e925c68fb5e8db1334bf30ac1a1b6b963b932a19cf41d2e899cf02f36aab"},
-    {file = "numpy-1.24.0-cp38-cp38-win_amd64.whl", hash = "sha256:d7f223554aba7280e6057727333ed357b71b7da7422d02ff5e91b857888c25d1"},
-    {file = "numpy-1.24.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:ab11f6a7602cf8ea4c093e091938207de3068c5693a0520168ecf4395750f7ea"},
-    {file = "numpy-1.24.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:12bba5561d8118981f2f1ff069ecae200c05d7b6c78a5cdac0911f74bc71cbd1"},
-    {file = "numpy-1.24.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9af91f794d2d3007d91d749ebc955302889261db514eb24caef30e03e8ec1e41"},
-    {file = "numpy-1.24.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8b1ddfac6a82d4f3c8e99436c90b9c2c68c0bb14658d1684cdd00f05fab241f5"},
-    {file = "numpy-1.24.0-cp39-cp39-win32.whl", hash = "sha256:ac4fe68f1a5a18136acebd4eff91aab8bed00d1ef2fdb34b5d9192297ffbbdfc"},
-    {file = "numpy-1.24.0-cp39-cp39-win_amd64.whl", hash = "sha256:667b5b1f6a352419e340f6475ef9930348ae5cb7fca15f2cc3afcb530823715e"},
-    {file = "numpy-1.24.0-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:4d01f7832fa319a36fd75ba10ea4027c9338ede875792f7bf617f4b45056fc3a"},
-    {file = "numpy-1.24.0-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dbb0490f0a880700a6cc4d000384baf19c1f4df59fff158d9482d4dbbca2b239"},
-    {file = "numpy-1.24.0-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:0104d8adaa3a4cc60c2777cab5196593bf8a7f416eda133be1f3803dd0838886"},
-    {file = "numpy-1.24.0.tar.gz", hash = "sha256:c4ab7c9711fe6b235e86487ca74c1b092a6dd59a3cb45b63241ea0a148501853"},
-]
-
-[[package]]
-name = "opencv-python"
-version = "4.6.0.66"
-description = "Wrapper package for OpenCV python bindings."
-category = "main"
-optional = false
-python-versions = ">=3.6"
-files = [
-    {file = "opencv-python-4.6.0.66.tar.gz", hash = "sha256:c5bfae41ad4031e66bb10ec4a0a2ffd3e514d092652781e8b1ac98d1b59f1158"},
-    {file = "opencv_python-4.6.0.66-cp36-abi3-macosx_10_15_x86_64.whl", hash = "sha256:e6e448b62afc95c5b58f97e87ef84699e6607fe5c58730a03301c52496005cae"},
-    {file = "opencv_python-4.6.0.66-cp36-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5af8ba35a4fcb8913ffb86e92403e9a656a4bff4a645d196987468f0f8947875"},
-    {file = "opencv_python-4.6.0.66-cp36-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dbdc84a9b4ea2cbae33861652d25093944b9959279200b7ae0badd32439f74de"},
-    {file = "opencv_python-4.6.0.66-cp36-abi3-win32.whl", hash = "sha256:f482e78de6e7b0b060ff994ffd859bddc3f7f382bb2019ef157b0ea8ca8712f5"},
-    {file = "opencv_python-4.6.0.66-cp36-abi3-win_amd64.whl", hash = "sha256:0dc82a3d8630c099d2f3ac1b1aabee164e8188db54a786abb7a4e27eba309440"},
-    {file = "opencv_python-4.6.0.66-cp37-abi3-macosx_11_0_arm64.whl", hash = "sha256:6e32af22e3202748bd233ed8f538741876191863882eba44e332d1a34993165b"},
-]
-
-[package.dependencies]
-numpy = [
-    {version = ">=1.21.2", markers = "python_version >= \"3.10\" or python_version >= \"3.6\" and platform_system == \"Darwin\" and platform_machine == \"arm64\""},
-    {version = ">=1.19.3", markers = "python_version >= \"3.6\" and platform_system == \"Linux\" and platform_machine == \"aarch64\" or python_version >= \"3.9\""},
-    {version = ">=1.14.5", markers = "python_version >= \"3.7\""},
-    {version = ">=1.17.3", markers = "python_version >= \"3.8\""},
-]
-
-[[package]]
-name = "protobuf"
-version = "3.5.1"
-description = "Protocol Buffers"
-category = "main"
-optional = false
-python-versions = "*"
-files = [
-    {file = "protobuf-3.5.1-cp27-cp27mu-manylinux1_x86_64.whl", hash = "sha256:11788df3e176f44e0375fe6361342d7258a457b346504ea259a21b77ffc18a90"},
-    {file = "protobuf-3.5.1-cp33-cp33m-manylinux1_x86_64.whl", hash = "sha256:50c24f0d00b7efb3a72ae638ddc118e713cfe8cef40527afe24f7ebcb878e46d"},
-    {file = "protobuf-3.5.1-cp34-cp34m-manylinux1_x86_64.whl", hash = "sha256:41661f9a442eba2f1967f15333ebe9ecc7e7c51bcbaa2972303ad33a4ca0168e"},
-    {file = "protobuf-3.5.1-cp35-cp35m-manylinux1_x86_64.whl", hash = "sha256:06ec363b74bceb7d018f2171e0892f03ab6816530e2b0f77d725a58264551e48"},
-    {file = "protobuf-3.5.1-cp36-cp36m-manylinux1_x86_64.whl", hash = "sha256:b20f861b55efd8206428c13e017cc8e2c34b40b2a714446eb202bbf0ff7597a6"},
-    {file = "protobuf-3.5.1-py2.py3-none-any.whl", hash = "sha256:4d2e665410b0a278d2eb2c0a529ca2366bb325eb2ae34e189a826b71fb1b28cd"},
-    {file = "protobuf-3.5.1.tar.gz", hash = "sha256:95b78959572de7d7fafa3acb718ed71f482932ddddddbd29ba8319c10639d863"},
-]
-
-[package.dependencies]
-setuptools = "*"
-six = ">=1.9"
-
-[[package]]
-name = "pyniryo"
-version = "1.1.2"
-description = "Package to control Niryo Robot \"Ned\" through TCP"
-category = "main"
-optional = false
-python-versions = "*"
-files = [
-    {file = "pyniryo-1.1.2-py3-none-any.whl", hash = "sha256:6b286dd9499e9afe89d106951e4edefbda0863b87939cc7413628f979112660b"},
-    {file = "pyniryo-1.1.2.tar.gz", hash = "sha256:ae31741dfe5e3a997cb26644545626558d3dc25081de9ad8caa5706cd2be138c"},
-]
-
-[package.dependencies]
-enum34 = "*"
-numpy = "*"
-opencv-python = {version = ">=4.3.0.38", markers = "python_version > \"2.7\""}
-
-[[package]]
-name = "setuptools"
-version = "65.6.3"
-description = "Easily download, build, install, upgrade, and uninstall Python packages"
-category = "main"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "setuptools-65.6.3-py3-none-any.whl", hash = "sha256:57f6f22bde4e042978bcd50176fdb381d7c21a9efa4041202288d3737a0c6a54"},
-    {file = "setuptools-65.6.3.tar.gz", hash = "sha256:a7620757bf984b58deaf32fc8a4577a9bbc0850cf92c20e1ce41c38c19e5fb75"},
-]
-
-[package.extras]
-docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "pygments-github-lexers (==0.0.5)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-favicon", "sphinx-hoverxref (<2)", "sphinx-inline-tabs", "sphinx-notfound-page (==0.8.3)", "sphinx-reredirects", "sphinxcontrib-towncrier"]
-testing = ["build[virtualenv]", "filelock (>=3.4.0)", "flake8 (<5)", "flake8-2020", "ini2toml[lite] (>=0.9)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pip (>=19.1)", "pip-run (>=8.8)", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)", "pytest-perf", "pytest-timeout", "pytest-xdist", "tomli-w (>=1.0.0)", "virtualenv (>=13.0.0)", "wheel"]
-testing-integration = ["build[virtualenv]", "filelock (>=3.4.0)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pytest", "pytest-enabler", "pytest-xdist", "tomli", "virtualenv (>=13.0.0)", "wheel"]
-
-[[package]]
-name = "six"
-version = "1.16.0"
-description = "Python 2 and 3 compatibility utilities"
-category = "main"
-optional = false
-python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*"
-files = [
-    {file = "six-1.16.0-py2.py3-none-any.whl", hash = "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"},
-    {file = "six-1.16.0.tar.gz", hash = "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926"},
-]
-
-[[package]]
-name = "wrapt"
-version = "1.14.1"
-description = "Module for decorators, wrappers and monkey patching."
-category = "main"
-optional = false
-python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,>=2.7"
-files = [
-    {file = "wrapt-1.14.1-cp27-cp27m-macosx_10_9_x86_64.whl", hash = "sha256:1b376b3f4896e7930f1f772ac4b064ac12598d1c38d04907e696cc4d794b43d3"},
-    {file = "wrapt-1.14.1-cp27-cp27m-manylinux1_i686.whl", hash = "sha256:903500616422a40a98a5a3c4ff4ed9d0066f3b4c951fa286018ecdf0750194ef"},
-    {file = "wrapt-1.14.1-cp27-cp27m-manylinux1_x86_64.whl", hash = "sha256:5a9a0d155deafd9448baff28c08e150d9b24ff010e899311ddd63c45c2445e28"},
-    {file = "wrapt-1.14.1-cp27-cp27m-manylinux2010_i686.whl", hash = "sha256:ddaea91abf8b0d13443f6dac52e89051a5063c7d014710dcb4d4abb2ff811a59"},
-    {file = "wrapt-1.14.1-cp27-cp27m-manylinux2010_x86_64.whl", hash = "sha256:36f582d0c6bc99d5f39cd3ac2a9062e57f3cf606ade29a0a0d6b323462f4dd87"},
-    {file = "wrapt-1.14.1-cp27-cp27mu-manylinux1_i686.whl", hash = "sha256:7ef58fb89674095bfc57c4069e95d7a31cfdc0939e2a579882ac7d55aadfd2a1"},
-    {file = "wrapt-1.14.1-cp27-cp27mu-manylinux1_x86_64.whl", hash = "sha256:e2f83e18fe2f4c9e7db597e988f72712c0c3676d337d8b101f6758107c42425b"},
-    {file = "wrapt-1.14.1-cp27-cp27mu-manylinux2010_i686.whl", hash = "sha256:ee2b1b1769f6707a8a445162ea16dddf74285c3964f605877a20e38545c3c462"},
-    {file = "wrapt-1.14.1-cp27-cp27mu-manylinux2010_x86_64.whl", hash = "sha256:833b58d5d0b7e5b9832869f039203389ac7cbf01765639c7309fd50ef619e0b1"},
-    {file = "wrapt-1.14.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:80bb5c256f1415f747011dc3604b59bc1f91c6e7150bd7db03b19170ee06b320"},
-    {file = "wrapt-1.14.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:07f7a7d0f388028b2df1d916e94bbb40624c59b48ecc6cbc232546706fac74c2"},
-    {file = "wrapt-1.14.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:02b41b633c6261feff8ddd8d11c711df6842aba629fdd3da10249a53211a72c4"},
-    {file = "wrapt-1.14.1-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:2fe803deacd09a233e4762a1adcea5db5d31e6be577a43352936179d14d90069"},
-    {file = "wrapt-1.14.1-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:257fd78c513e0fb5cdbe058c27a0624c9884e735bbd131935fd49e9fe719d310"},
-    {file = "wrapt-1.14.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:4fcc4649dc762cddacd193e6b55bc02edca674067f5f98166d7713b193932b7f"},
-    {file = "wrapt-1.14.1-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:11871514607b15cfeb87c547a49bca19fde402f32e2b1c24a632506c0a756656"},
-    {file = "wrapt-1.14.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:8ad85f7f4e20964db4daadcab70b47ab05c7c1cf2a7c1e51087bfaa83831854c"},
-    {file = "wrapt-1.14.1-cp310-cp310-win32.whl", hash = "sha256:a9a52172be0b5aae932bef82a79ec0a0ce87288c7d132946d645eba03f0ad8a8"},
-    {file = "wrapt-1.14.1-cp310-cp310-win_amd64.whl", hash = "sha256:6d323e1554b3d22cfc03cd3243b5bb815a51f5249fdcbb86fda4bf62bab9e164"},
-    {file = "wrapt-1.14.1-cp35-cp35m-manylinux1_i686.whl", hash = "sha256:43ca3bbbe97af00f49efb06e352eae40434ca9d915906f77def219b88e85d907"},
-    {file = "wrapt-1.14.1-cp35-cp35m-manylinux1_x86_64.whl", hash = "sha256:6b1a564e6cb69922c7fe3a678b9f9a3c54e72b469875aa8018f18b4d1dd1adf3"},
-    {file = "wrapt-1.14.1-cp35-cp35m-manylinux2010_i686.whl", hash = "sha256:00b6d4ea20a906c0ca56d84f93065b398ab74b927a7a3dbd470f6fc503f95dc3"},
-    {file = "wrapt-1.14.1-cp35-cp35m-manylinux2010_x86_64.whl", hash = "sha256:a85d2b46be66a71bedde836d9e41859879cc54a2a04fad1191eb50c2066f6e9d"},
-    {file = "wrapt-1.14.1-cp35-cp35m-win32.whl", hash = "sha256:dbcda74c67263139358f4d188ae5faae95c30929281bc6866d00573783c422b7"},
-    {file = "wrapt-1.14.1-cp35-cp35m-win_amd64.whl", hash = "sha256:b21bb4c09ffabfa0e85e3a6b623e19b80e7acd709b9f91452b8297ace2a8ab00"},
-    {file = "wrapt-1.14.1-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:9e0fd32e0148dd5dea6af5fee42beb949098564cc23211a88d799e434255a1f4"},
-    {file = "wrapt-1.14.1-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9736af4641846491aedb3c3f56b9bc5568d92b0692303b5a305301a95dfd38b1"},
-    {file = "wrapt-1.14.1-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:5b02d65b9ccf0ef6c34cba6cf5bf2aab1bb2f49c6090bafeecc9cd81ad4ea1c1"},
-    {file = "wrapt-1.14.1-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:21ac0156c4b089b330b7666db40feee30a5d52634cc4560e1905d6529a3897ff"},
-    {file = "wrapt-1.14.1-cp36-cp36m-musllinux_1_1_aarch64.whl", hash = "sha256:9f3e6f9e05148ff90002b884fbc2a86bd303ae847e472f44ecc06c2cd2fcdb2d"},
-    {file = "wrapt-1.14.1-cp36-cp36m-musllinux_1_1_i686.whl", hash = "sha256:6e743de5e9c3d1b7185870f480587b75b1cb604832e380d64f9504a0535912d1"},
-    {file = "wrapt-1.14.1-cp36-cp36m-musllinux_1_1_x86_64.whl", hash = "sha256:d79d7d5dc8a32b7093e81e97dad755127ff77bcc899e845f41bf71747af0c569"},
-    {file = "wrapt-1.14.1-cp36-cp36m-win32.whl", hash = "sha256:81b19725065dcb43df02b37e03278c011a09e49757287dca60c5aecdd5a0b8ed"},
-    {file = "wrapt-1.14.1-cp36-cp36m-win_amd64.whl", hash = "sha256:b014c23646a467558be7da3d6b9fa409b2c567d2110599b7cf9a0c5992b3b471"},
-    {file = "wrapt-1.14.1-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:88bd7b6bd70a5b6803c1abf6bca012f7ed963e58c68d76ee20b9d751c74a3248"},
-    {file = "wrapt-1.14.1-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b5901a312f4d14c59918c221323068fad0540e34324925c8475263841dbdfe68"},
-    {file = "wrapt-1.14.1-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d77c85fedff92cf788face9bfa3ebaa364448ebb1d765302e9af11bf449ca36d"},
-    {file = "wrapt-1.14.1-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8d649d616e5c6a678b26d15ece345354f7c2286acd6db868e65fcc5ff7c24a77"},
-    {file = "wrapt-1.14.1-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:7d2872609603cb35ca513d7404a94d6d608fc13211563571117046c9d2bcc3d7"},
-    {file = "wrapt-1.14.1-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:ee6acae74a2b91865910eef5e7de37dc6895ad96fa23603d1d27ea69df545015"},
-    {file = "wrapt-1.14.1-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:2b39d38039a1fdad98c87279b48bc5dce2c0ca0d73483b12cb72aa9609278e8a"},
-    {file = "wrapt-1.14.1-cp37-cp37m-win32.whl", hash = "sha256:60db23fa423575eeb65ea430cee741acb7c26a1365d103f7b0f6ec412b893853"},
-    {file = "wrapt-1.14.1-cp37-cp37m-win_amd64.whl", hash = "sha256:709fe01086a55cf79d20f741f39325018f4df051ef39fe921b1ebe780a66184c"},
-    {file = "wrapt-1.14.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:8c0ce1e99116d5ab21355d8ebe53d9460366704ea38ae4d9f6933188f327b456"},
-    {file = "wrapt-1.14.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:e3fb1677c720409d5f671e39bac6c9e0e422584e5f518bfd50aa4cbbea02433f"},
-    {file = "wrapt-1.14.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:642c2e7a804fcf18c222e1060df25fc210b9c58db7c91416fb055897fc27e8cc"},
-    {file = "wrapt-1.14.1-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7b7c050ae976e286906dd3f26009e117eb000fb2cf3533398c5ad9ccc86867b1"},
-    {file = "wrapt-1.14.1-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ef3f72c9666bba2bab70d2a8b79f2c6d2c1a42a7f7e2b0ec83bb2f9e383950af"},
-    {file = "wrapt-1.14.1-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:01c205616a89d09827986bc4e859bcabd64f5a0662a7fe95e0d359424e0e071b"},
-    {file = "wrapt-1.14.1-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:5a0f54ce2c092aaf439813735584b9537cad479575a09892b8352fea5e988dc0"},
-    {file = "wrapt-1.14.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:2cf71233a0ed05ccdabe209c606fe0bac7379fdcf687f39b944420d2a09fdb57"},
-    {file = "wrapt-1.14.1-cp38-cp38-win32.whl", hash = "sha256:aa31fdcc33fef9eb2552cbcbfee7773d5a6792c137b359e82879c101e98584c5"},
-    {file = "wrapt-1.14.1-cp38-cp38-win_amd64.whl", hash = "sha256:d1967f46ea8f2db647c786e78d8cc7e4313dbd1b0aca360592d8027b8508e24d"},
-    {file = "wrapt-1.14.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:3232822c7d98d23895ccc443bbdf57c7412c5a65996c30442ebe6ed3df335383"},
-    {file = "wrapt-1.14.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:988635d122aaf2bdcef9e795435662bcd65b02f4f4c1ae37fbee7401c440b3a7"},
-    {file = "wrapt-1.14.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9cca3c2cdadb362116235fdbd411735de4328c61425b0aa9f872fd76d02c4e86"},
-    {file = "wrapt-1.14.1-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d52a25136894c63de15a35bc0bdc5adb4b0e173b9c0d07a2be9d3ca64a332735"},
-    {file = "wrapt-1.14.1-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:40e7bc81c9e2b2734ea4bc1aceb8a8f0ceaac7c5299bc5d69e37c44d9081d43b"},
-    {file = "wrapt-1.14.1-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:b9b7a708dd92306328117d8c4b62e2194d00c365f18eff11a9b53c6f923b01e3"},
-    {file = "wrapt-1.14.1-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:6a9a25751acb379b466ff6be78a315e2b439d4c94c1e99cb7266d40a537995d3"},
-    {file = "wrapt-1.14.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:34aa51c45f28ba7f12accd624225e2b1e5a3a45206aa191f6f9aac931d9d56fe"},
-    {file = "wrapt-1.14.1-cp39-cp39-win32.whl", hash = "sha256:dee0ce50c6a2dd9056c20db781e9c1cfd33e77d2d569f5d1d9321c641bb903d5"},
-    {file = "wrapt-1.14.1-cp39-cp39-win_amd64.whl", hash = "sha256:dee60e1de1898bde3b238f18340eec6148986da0455d8ba7848d50470a7a32fb"},
-    {file = "wrapt-1.14.1.tar.gz", hash = "sha256:380a85cf89e0e69b7cfbe2ea9f765f004ff419f34194018a6827ac0e3edfed4d"},
-]
-
-[metadata]
-lock-version = "2.0"
-python-versions = "^3.9"
-content-hash = "278e48d2cdab1ba02761ea5a02353669f4da478af506599c48d62a8f0f4c1353"
+# This file is automatically @generated by Poetry and should not be changed by hand.
+
+[[package]]
+name = "deprecated"
+version = "1.2.7"
+description = "Python @deprecated decorator to deprecate old python classes, functions or methods."
+category = "main"
+optional = false
+python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
+files = [
+    {file = "Deprecated-1.2.7-py2.py3-none-any.whl", hash = "sha256:8b6a5aa50e482d8244a62e5582b96c372e87e3a28e8b49c316e46b95c76a611d"},
+    {file = "Deprecated-1.2.7.tar.gz", hash = "sha256:408038ab5fdeca67554e8f6742d1521cd3cd0ee0ff9d47f29318a4f4da31c308"},
+]
+
+[package.dependencies]
+wrapt = ">=1.10,<2"
+
+[package.extras]
+dev = ["PyTest", "PyTest (<5)", "PyTest-Cov", "PyTest-Cov (<2.6)", "bumpversion (<1)", "sphinx (<2)", "tox"]
+
+[[package]]
+name = "enum34"
+version = "1.1.10"
+description = "Python 3.4 Enum backported to 3.3, 3.2, 3.1, 2.7, 2.6, 2.5, and 2.4"
+category = "main"
+optional = false
+python-versions = "*"
+files = [
+    {file = "enum34-1.1.10-py2-none-any.whl", hash = "sha256:a98a201d6de3f2ab3db284e70a33b0f896fbf35f8086594e8c9e74b909058d53"},
+    {file = "enum34-1.1.10-py3-none-any.whl", hash = "sha256:c3858660960c984d6ab0ebad691265180da2b43f07e061c0f8dca9ef3cffd328"},
+    {file = "enum34-1.1.10.tar.gz", hash = "sha256:cce6a7477ed816bd2542d03d53db9f0db935dd013b70f336a95c73979289f248"},
+]
+
+[[package]]
+name = "kortex-api"
+version = "2.3.0.post34"
+description = "Kinova kortex_api"
+category = "main"
+optional = false
+python-versions = "*"
+files = [
+    {file = "kortex_api-2.3.0.post34-py3-none-any.whl", hash = "sha256:1cffd7ca2afe4dfbe71bc9c22379c69a8d04ff197676a6902aee06a191868805"},
+]
+
+[package.dependencies]
+deprecated = "1.2.7"
+protobuf = "3.5.1"
+
+[package.source]
+type = "file"
+url = "dependencies/kortex_api-2.3.0.post34-py3-none-any.whl"
+
+[[package]]
+name = "numpy"
+version = "1.24.0"
+description = "Fundamental package for array computing in Python"
+category = "main"
+optional = false
+python-versions = ">=3.8"
+files = [
+    {file = "numpy-1.24.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:6e73a1f4f5b74a42abb55bc2b3d869f1b38cbc8776da5f8b66bf110284f7a437"},
+    {file = "numpy-1.24.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:9387c7d6d50e8f8c31e7bfc034241e9c6f4b3eb5db8d118d6487047b922f82af"},
+    {file = "numpy-1.24.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7ad6a024a32ee61d18f5b402cd02e9c0e22c0fb9dc23751991b3a16d209d972e"},
+    {file = "numpy-1.24.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:73cf2c5b5a07450f20a0c8e04d9955491970177dce8df8d6903bf253e53268e0"},
+    {file = "numpy-1.24.0-cp310-cp310-win32.whl", hash = "sha256:cec79ff3984b2d1d103183fc4a3361f5b55bbb66cb395cbf5a920a4bb1fd588d"},
+    {file = "numpy-1.24.0-cp310-cp310-win_amd64.whl", hash = "sha256:4f5e78b8b710cd7cd1a8145994cfffc6ddd5911669a437777d8cedfce6c83a98"},
+    {file = "numpy-1.24.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:4445f472b246cad6514cc09fbb5ecb7aab09ca2acc3c16f29f8dca6c468af501"},
+    {file = "numpy-1.24.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:ec3e5e8172a0a6a4f3c2e7423d4a8434c41349141b04744b11a90e017a95bad5"},
+    {file = "numpy-1.24.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f9168790149f917ad8e3cf5047b353fefef753bd50b07c547da0bdf30bc15d91"},
+    {file = "numpy-1.24.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ada6c1e9608ceadaf7020e1deea508b73ace85560a16f51bef26aecb93626a72"},
+    {file = "numpy-1.24.0-cp311-cp311-win32.whl", hash = "sha256:f3c4a9a9f92734a4728ddbd331e0124eabbc968a0359a506e8e74a9b0d2d419b"},
+    {file = "numpy-1.24.0-cp311-cp311-win_amd64.whl", hash = "sha256:90075ef2c6ac6397d0035bcd8b298b26e481a7035f7a3f382c047eb9c3414db0"},
+    {file = "numpy-1.24.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:0885d9a7666cafe5f9876c57bfee34226e2b2847bfb94c9505e18d81011e5401"},
+    {file = "numpy-1.24.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:e63d2157f9fc98cc178870db83b0e0c85acdadd598b134b00ebec9e0db57a01f"},
+    {file = "numpy-1.24.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cf8960f72997e56781eb1c2ea256a70124f92a543b384f89e5fb3503a308b1d3"},
+    {file = "numpy-1.24.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2f8e0df2ecc1928ef7256f18e309c9d6229b08b5be859163f5caa59c93d53646"},
+    {file = "numpy-1.24.0-cp38-cp38-win32.whl", hash = "sha256:fe44e925c68fb5e8db1334bf30ac1a1b6b963b932a19cf41d2e899cf02f36aab"},
+    {file = "numpy-1.24.0-cp38-cp38-win_amd64.whl", hash = "sha256:d7f223554aba7280e6057727333ed357b71b7da7422d02ff5e91b857888c25d1"},
+    {file = "numpy-1.24.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:ab11f6a7602cf8ea4c093e091938207de3068c5693a0520168ecf4395750f7ea"},
+    {file = "numpy-1.24.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:12bba5561d8118981f2f1ff069ecae200c05d7b6c78a5cdac0911f74bc71cbd1"},
+    {file = "numpy-1.24.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9af91f794d2d3007d91d749ebc955302889261db514eb24caef30e03e8ec1e41"},
+    {file = "numpy-1.24.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8b1ddfac6a82d4f3c8e99436c90b9c2c68c0bb14658d1684cdd00f05fab241f5"},
+    {file = "numpy-1.24.0-cp39-cp39-win32.whl", hash = "sha256:ac4fe68f1a5a18136acebd4eff91aab8bed00d1ef2fdb34b5d9192297ffbbdfc"},
+    {file = "numpy-1.24.0-cp39-cp39-win_amd64.whl", hash = "sha256:667b5b1f6a352419e340f6475ef9930348ae5cb7fca15f2cc3afcb530823715e"},
+    {file = "numpy-1.24.0-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:4d01f7832fa319a36fd75ba10ea4027c9338ede875792f7bf617f4b45056fc3a"},
+    {file = "numpy-1.24.0-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dbb0490f0a880700a6cc4d000384baf19c1f4df59fff158d9482d4dbbca2b239"},
+    {file = "numpy-1.24.0-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:0104d8adaa3a4cc60c2777cab5196593bf8a7f416eda133be1f3803dd0838886"},
+    {file = "numpy-1.24.0.tar.gz", hash = "sha256:c4ab7c9711fe6b235e86487ca74c1b092a6dd59a3cb45b63241ea0a148501853"},
+]
+
+[[package]]
+name = "opencv-python"
+version = "4.6.0.66"
+description = "Wrapper package for OpenCV python bindings."
+category = "main"
+optional = false
+python-versions = ">=3.6"
+files = [
+    {file = "opencv-python-4.6.0.66.tar.gz", hash = "sha256:c5bfae41ad4031e66bb10ec4a0a2ffd3e514d092652781e8b1ac98d1b59f1158"},
+    {file = "opencv_python-4.6.0.66-cp36-abi3-macosx_10_15_x86_64.whl", hash = "sha256:e6e448b62afc95c5b58f97e87ef84699e6607fe5c58730a03301c52496005cae"},
+    {file = "opencv_python-4.6.0.66-cp36-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5af8ba35a4fcb8913ffb86e92403e9a656a4bff4a645d196987468f0f8947875"},
+    {file = "opencv_python-4.6.0.66-cp36-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dbdc84a9b4ea2cbae33861652d25093944b9959279200b7ae0badd32439f74de"},
+    {file = "opencv_python-4.6.0.66-cp36-abi3-win32.whl", hash = "sha256:f482e78de6e7b0b060ff994ffd859bddc3f7f382bb2019ef157b0ea8ca8712f5"},
+    {file = "opencv_python-4.6.0.66-cp36-abi3-win_amd64.whl", hash = "sha256:0dc82a3d8630c099d2f3ac1b1aabee164e8188db54a786abb7a4e27eba309440"},
+    {file = "opencv_python-4.6.0.66-cp37-abi3-macosx_11_0_arm64.whl", hash = "sha256:6e32af22e3202748bd233ed8f538741876191863882eba44e332d1a34993165b"},
+]
+
+[package.dependencies]
+numpy = [
+    {version = ">=1.21.2", markers = "python_version >= \"3.10\" or python_version >= \"3.6\" and platform_system == \"Darwin\" and platform_machine == \"arm64\""},
+    {version = ">=1.19.3", markers = "python_version >= \"3.6\" and platform_system == \"Linux\" and platform_machine == \"aarch64\" or python_version >= \"3.9\""},
+    {version = ">=1.14.5", markers = "python_version >= \"3.7\""},
+    {version = ">=1.17.3", markers = "python_version >= \"3.8\""},
+]
+
+[[package]]
+name = "protobuf"
+version = "3.5.1"
+description = "Protocol Buffers"
+category = "main"
+optional = false
+python-versions = "*"
+files = [
+    {file = "protobuf-3.5.1-cp27-cp27mu-manylinux1_x86_64.whl", hash = "sha256:11788df3e176f44e0375fe6361342d7258a457b346504ea259a21b77ffc18a90"},
+    {file = "protobuf-3.5.1-cp33-cp33m-manylinux1_x86_64.whl", hash = "sha256:50c24f0d00b7efb3a72ae638ddc118e713cfe8cef40527afe24f7ebcb878e46d"},
+    {file = "protobuf-3.5.1-cp34-cp34m-manylinux1_x86_64.whl", hash = "sha256:41661f9a442eba2f1967f15333ebe9ecc7e7c51bcbaa2972303ad33a4ca0168e"},
+    {file = "protobuf-3.5.1-cp35-cp35m-manylinux1_x86_64.whl", hash = "sha256:06ec363b74bceb7d018f2171e0892f03ab6816530e2b0f77d725a58264551e48"},
+    {file = "protobuf-3.5.1-cp36-cp36m-manylinux1_x86_64.whl", hash = "sha256:b20f861b55efd8206428c13e017cc8e2c34b40b2a714446eb202bbf0ff7597a6"},
+    {file = "protobuf-3.5.1-py2.py3-none-any.whl", hash = "sha256:4d2e665410b0a278d2eb2c0a529ca2366bb325eb2ae34e189a826b71fb1b28cd"},
+    {file = "protobuf-3.5.1.tar.gz", hash = "sha256:95b78959572de7d7fafa3acb718ed71f482932ddddddbd29ba8319c10639d863"},
+]
+
+[package.dependencies]
+setuptools = "*"
+six = ">=1.9"
+
+[[package]]
+name = "pyniryo"
+version = "1.1.2"
+description = "Package to control Niryo Robot \"Ned\" through TCP"
+category = "main"
+optional = false
+python-versions = "*"
+files = [
+    {file = "pyniryo-1.1.2-py3-none-any.whl", hash = "sha256:6b286dd9499e9afe89d106951e4edefbda0863b87939cc7413628f979112660b"},
+    {file = "pyniryo-1.1.2.tar.gz", hash = "sha256:ae31741dfe5e3a997cb26644545626558d3dc25081de9ad8caa5706cd2be138c"},
+]
+
+[package.dependencies]
+enum34 = "*"
+numpy = "*"
+opencv-python = {version = ">=4.3.0.38", markers = "python_version > \"2.7\""}
+
+[[package]]
+name = "setuptools"
+version = "65.6.3"
+description = "Easily download, build, install, upgrade, and uninstall Python packages"
+category = "main"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "setuptools-65.6.3-py3-none-any.whl", hash = "sha256:57f6f22bde4e042978bcd50176fdb381d7c21a9efa4041202288d3737a0c6a54"},
+    {file = "setuptools-65.6.3.tar.gz", hash = "sha256:a7620757bf984b58deaf32fc8a4577a9bbc0850cf92c20e1ce41c38c19e5fb75"},
+]
+
+[package.extras]
+docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "pygments-github-lexers (==0.0.5)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-favicon", "sphinx-hoverxref (<2)", "sphinx-inline-tabs", "sphinx-notfound-page (==0.8.3)", "sphinx-reredirects", "sphinxcontrib-towncrier"]
+testing = ["build[virtualenv]", "filelock (>=3.4.0)", "flake8 (<5)", "flake8-2020", "ini2toml[lite] (>=0.9)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pip (>=19.1)", "pip-run (>=8.8)", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)", "pytest-perf", "pytest-timeout", "pytest-xdist", "tomli-w (>=1.0.0)", "virtualenv (>=13.0.0)", "wheel"]
+testing-integration = ["build[virtualenv]", "filelock (>=3.4.0)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pytest", "pytest-enabler", "pytest-xdist", "tomli", "virtualenv (>=13.0.0)", "wheel"]
+
+[[package]]
+name = "six"
+version = "1.16.0"
+description = "Python 2 and 3 compatibility utilities"
+category = "main"
+optional = false
+python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*"
+files = [
+    {file = "six-1.16.0-py2.py3-none-any.whl", hash = "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"},
+    {file = "six-1.16.0.tar.gz", hash = "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926"},
+]
+
+[[package]]
+name = "wrapt"
+version = "1.14.1"
+description = "Module for decorators, wrappers and monkey patching."
+category = "main"
+optional = false
+python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,>=2.7"
+files = [
+    {file = "wrapt-1.14.1-cp27-cp27m-macosx_10_9_x86_64.whl", hash = "sha256:1b376b3f4896e7930f1f772ac4b064ac12598d1c38d04907e696cc4d794b43d3"},
+    {file = "wrapt-1.14.1-cp27-cp27m-manylinux1_i686.whl", hash = "sha256:903500616422a40a98a5a3c4ff4ed9d0066f3b4c951fa286018ecdf0750194ef"},
+    {file = "wrapt-1.14.1-cp27-cp27m-manylinux1_x86_64.whl", hash = "sha256:5a9a0d155deafd9448baff28c08e150d9b24ff010e899311ddd63c45c2445e28"},
+    {file = "wrapt-1.14.1-cp27-cp27m-manylinux2010_i686.whl", hash = "sha256:ddaea91abf8b0d13443f6dac52e89051a5063c7d014710dcb4d4abb2ff811a59"},
+    {file = "wrapt-1.14.1-cp27-cp27m-manylinux2010_x86_64.whl", hash = "sha256:36f582d0c6bc99d5f39cd3ac2a9062e57f3cf606ade29a0a0d6b323462f4dd87"},
+    {file = "wrapt-1.14.1-cp27-cp27mu-manylinux1_i686.whl", hash = "sha256:7ef58fb89674095bfc57c4069e95d7a31cfdc0939e2a579882ac7d55aadfd2a1"},
+    {file = "wrapt-1.14.1-cp27-cp27mu-manylinux1_x86_64.whl", hash = "sha256:e2f83e18fe2f4c9e7db597e988f72712c0c3676d337d8b101f6758107c42425b"},
+    {file = "wrapt-1.14.1-cp27-cp27mu-manylinux2010_i686.whl", hash = "sha256:ee2b1b1769f6707a8a445162ea16dddf74285c3964f605877a20e38545c3c462"},
+    {file = "wrapt-1.14.1-cp27-cp27mu-manylinux2010_x86_64.whl", hash = "sha256:833b58d5d0b7e5b9832869f039203389ac7cbf01765639c7309fd50ef619e0b1"},
+    {file = "wrapt-1.14.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:80bb5c256f1415f747011dc3604b59bc1f91c6e7150bd7db03b19170ee06b320"},
+    {file = "wrapt-1.14.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:07f7a7d0f388028b2df1d916e94bbb40624c59b48ecc6cbc232546706fac74c2"},
+    {file = "wrapt-1.14.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:02b41b633c6261feff8ddd8d11c711df6842aba629fdd3da10249a53211a72c4"},
+    {file = "wrapt-1.14.1-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:2fe803deacd09a233e4762a1adcea5db5d31e6be577a43352936179d14d90069"},
+    {file = "wrapt-1.14.1-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:257fd78c513e0fb5cdbe058c27a0624c9884e735bbd131935fd49e9fe719d310"},
+    {file = "wrapt-1.14.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:4fcc4649dc762cddacd193e6b55bc02edca674067f5f98166d7713b193932b7f"},
+    {file = "wrapt-1.14.1-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:11871514607b15cfeb87c547a49bca19fde402f32e2b1c24a632506c0a756656"},
+    {file = "wrapt-1.14.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:8ad85f7f4e20964db4daadcab70b47ab05c7c1cf2a7c1e51087bfaa83831854c"},
+    {file = "wrapt-1.14.1-cp310-cp310-win32.whl", hash = "sha256:a9a52172be0b5aae932bef82a79ec0a0ce87288c7d132946d645eba03f0ad8a8"},
+    {file = "wrapt-1.14.1-cp310-cp310-win_amd64.whl", hash = "sha256:6d323e1554b3d22cfc03cd3243b5bb815a51f5249fdcbb86fda4bf62bab9e164"},
+    {file = "wrapt-1.14.1-cp35-cp35m-manylinux1_i686.whl", hash = "sha256:43ca3bbbe97af00f49efb06e352eae40434ca9d915906f77def219b88e85d907"},
+    {file = "wrapt-1.14.1-cp35-cp35m-manylinux1_x86_64.whl", hash = "sha256:6b1a564e6cb69922c7fe3a678b9f9a3c54e72b469875aa8018f18b4d1dd1adf3"},
+    {file = "wrapt-1.14.1-cp35-cp35m-manylinux2010_i686.whl", hash = "sha256:00b6d4ea20a906c0ca56d84f93065b398ab74b927a7a3dbd470f6fc503f95dc3"},
+    {file = "wrapt-1.14.1-cp35-cp35m-manylinux2010_x86_64.whl", hash = "sha256:a85d2b46be66a71bedde836d9e41859879cc54a2a04fad1191eb50c2066f6e9d"},
+    {file = "wrapt-1.14.1-cp35-cp35m-win32.whl", hash = "sha256:dbcda74c67263139358f4d188ae5faae95c30929281bc6866d00573783c422b7"},
+    {file = "wrapt-1.14.1-cp35-cp35m-win_amd64.whl", hash = "sha256:b21bb4c09ffabfa0e85e3a6b623e19b80e7acd709b9f91452b8297ace2a8ab00"},
+    {file = "wrapt-1.14.1-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:9e0fd32e0148dd5dea6af5fee42beb949098564cc23211a88d799e434255a1f4"},
+    {file = "wrapt-1.14.1-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9736af4641846491aedb3c3f56b9bc5568d92b0692303b5a305301a95dfd38b1"},
+    {file = "wrapt-1.14.1-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:5b02d65b9ccf0ef6c34cba6cf5bf2aab1bb2f49c6090bafeecc9cd81ad4ea1c1"},
+    {file = "wrapt-1.14.1-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:21ac0156c4b089b330b7666db40feee30a5d52634cc4560e1905d6529a3897ff"},
+    {file = "wrapt-1.14.1-cp36-cp36m-musllinux_1_1_aarch64.whl", hash = "sha256:9f3e6f9e05148ff90002b884fbc2a86bd303ae847e472f44ecc06c2cd2fcdb2d"},
+    {file = "wrapt-1.14.1-cp36-cp36m-musllinux_1_1_i686.whl", hash = "sha256:6e743de5e9c3d1b7185870f480587b75b1cb604832e380d64f9504a0535912d1"},
+    {file = "wrapt-1.14.1-cp36-cp36m-musllinux_1_1_x86_64.whl", hash = "sha256:d79d7d5dc8a32b7093e81e97dad755127ff77bcc899e845f41bf71747af0c569"},
+    {file = "wrapt-1.14.1-cp36-cp36m-win32.whl", hash = "sha256:81b19725065dcb43df02b37e03278c011a09e49757287dca60c5aecdd5a0b8ed"},
+    {file = "wrapt-1.14.1-cp36-cp36m-win_amd64.whl", hash = "sha256:b014c23646a467558be7da3d6b9fa409b2c567d2110599b7cf9a0c5992b3b471"},
+    {file = "wrapt-1.14.1-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:88bd7b6bd70a5b6803c1abf6bca012f7ed963e58c68d76ee20b9d751c74a3248"},
+    {file = "wrapt-1.14.1-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b5901a312f4d14c59918c221323068fad0540e34324925c8475263841dbdfe68"},
+    {file = "wrapt-1.14.1-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d77c85fedff92cf788face9bfa3ebaa364448ebb1d765302e9af11bf449ca36d"},
+    {file = "wrapt-1.14.1-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8d649d616e5c6a678b26d15ece345354f7c2286acd6db868e65fcc5ff7c24a77"},
+    {file = "wrapt-1.14.1-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:7d2872609603cb35ca513d7404a94d6d608fc13211563571117046c9d2bcc3d7"},
+    {file = "wrapt-1.14.1-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:ee6acae74a2b91865910eef5e7de37dc6895ad96fa23603d1d27ea69df545015"},
+    {file = "wrapt-1.14.1-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:2b39d38039a1fdad98c87279b48bc5dce2c0ca0d73483b12cb72aa9609278e8a"},
+    {file = "wrapt-1.14.1-cp37-cp37m-win32.whl", hash = "sha256:60db23fa423575eeb65ea430cee741acb7c26a1365d103f7b0f6ec412b893853"},
+    {file = "wrapt-1.14.1-cp37-cp37m-win_amd64.whl", hash = "sha256:709fe01086a55cf79d20f741f39325018f4df051ef39fe921b1ebe780a66184c"},
+    {file = "wrapt-1.14.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:8c0ce1e99116d5ab21355d8ebe53d9460366704ea38ae4d9f6933188f327b456"},
+    {file = "wrapt-1.14.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:e3fb1677c720409d5f671e39bac6c9e0e422584e5f518bfd50aa4cbbea02433f"},
+    {file = "wrapt-1.14.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:642c2e7a804fcf18c222e1060df25fc210b9c58db7c91416fb055897fc27e8cc"},
+    {file = "wrapt-1.14.1-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7b7c050ae976e286906dd3f26009e117eb000fb2cf3533398c5ad9ccc86867b1"},
+    {file = "wrapt-1.14.1-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ef3f72c9666bba2bab70d2a8b79f2c6d2c1a42a7f7e2b0ec83bb2f9e383950af"},
+    {file = "wrapt-1.14.1-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:01c205616a89d09827986bc4e859bcabd64f5a0662a7fe95e0d359424e0e071b"},
+    {file = "wrapt-1.14.1-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:5a0f54ce2c092aaf439813735584b9537cad479575a09892b8352fea5e988dc0"},
+    {file = "wrapt-1.14.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:2cf71233a0ed05ccdabe209c606fe0bac7379fdcf687f39b944420d2a09fdb57"},
+    {file = "wrapt-1.14.1-cp38-cp38-win32.whl", hash = "sha256:aa31fdcc33fef9eb2552cbcbfee7773d5a6792c137b359e82879c101e98584c5"},
+    {file = "wrapt-1.14.1-cp38-cp38-win_amd64.whl", hash = "sha256:d1967f46ea8f2db647c786e78d8cc7e4313dbd1b0aca360592d8027b8508e24d"},
+    {file = "wrapt-1.14.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:3232822c7d98d23895ccc443bbdf57c7412c5a65996c30442ebe6ed3df335383"},
+    {file = "wrapt-1.14.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:988635d122aaf2bdcef9e795435662bcd65b02f4f4c1ae37fbee7401c440b3a7"},
+    {file = "wrapt-1.14.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9cca3c2cdadb362116235fdbd411735de4328c61425b0aa9f872fd76d02c4e86"},
+    {file = "wrapt-1.14.1-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d52a25136894c63de15a35bc0bdc5adb4b0e173b9c0d07a2be9d3ca64a332735"},
+    {file = "wrapt-1.14.1-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:40e7bc81c9e2b2734ea4bc1aceb8a8f0ceaac7c5299bc5d69e37c44d9081d43b"},
+    {file = "wrapt-1.14.1-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:b9b7a708dd92306328117d8c4b62e2194d00c365f18eff11a9b53c6f923b01e3"},
+    {file = "wrapt-1.14.1-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:6a9a25751acb379b466ff6be78a315e2b439d4c94c1e99cb7266d40a537995d3"},
+    {file = "wrapt-1.14.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:34aa51c45f28ba7f12accd624225e2b1e5a3a45206aa191f6f9aac931d9d56fe"},
+    {file = "wrapt-1.14.1-cp39-cp39-win32.whl", hash = "sha256:dee0ce50c6a2dd9056c20db781e9c1cfd33e77d2d569f5d1d9321c641bb903d5"},
+    {file = "wrapt-1.14.1-cp39-cp39-win_amd64.whl", hash = "sha256:dee60e1de1898bde3b238f18340eec6148986da0455d8ba7848d50470a7a32fb"},
+    {file = "wrapt-1.14.1.tar.gz", hash = "sha256:380a85cf89e0e69b7cfbe2ea9f765f004ff419f34194018a6827ac0e3edfed4d"},
+]
+
+[metadata]
+lock-version = "2.0"
+python-versions = "^3.9"
+content-hash = "278e48d2cdab1ba02761ea5a02353669f4da478af506599c48d62a8f0f4c1353"
```

### Comparing `rria_api-1.0.4/rria_api/robot_facade.py` & `rria_api-1.0.5/rria_api/robot_facade.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,362 +1,362 @@
-from rria_api.ned.connect_ned import ConnectNed
-from rria_api.ned.action_ned import ActionNed
-from rria_api.gen3.connect_gen3 import ConnectGen3
-from rria_api.gen3.action_gen3 import ActionGen3
-from time import sleep
-
-
-class RobotObject:
-    def __init__(self, ip_address, robot_type):
-        self.ip_address = ip_address
-        self.robot_type = robot_type
-
-        # This atribute is used to store the general robot instance
-        self.robot_instance = None
-
-        # This atribute is used to store the general connection instance
-        self.connection_instance = None
-
-    def connect_robot(self):
-        """
-        Connect robot depends on the robot type
-        :rtype: bool
-
-        """
-
-        if self.robot_type == 'gen3':
-            try:
-                self.connection_instance = ConnectGen3(self.ip_address, ["admin", "admin"])
-                self.robot_instance = self.connection_instance.connect_robot()
-
-                return True
-
-            except(Exception,):
-                print('The connection attempt failed. Check the physical connection to the robot and try again later.')
-
-                return False
-
-        if self.robot_type == 'ned':
-            try:
-                self.connection_instance = ConnectNed()
-                self.robot_instance = self.connection_instance.connect_robot(self.ip_address)
-
-                return True
-
-            except(Exception,):
-                print('The connection attempt failed. Check the physical connection to the robot and try again later.')
-
-                return False
-
-        if self.robot_type == 'denso':
-            pass
-
-        if self.robot_type == 'test':
-            sleep(1)
-            return True
-
-    def disconnect_robot(self):
-        """
-        Close connection with robot
-        :rtype: None
-
-        """
-        if self.robot_type == 'gen3':
-            self.connection_instance.disconnect_robot()
-
-        if self.robot_type == 'ned':
-            self.connection_instance.disconnect_robot()
-
-        if self.robot_type == 'denso':
-            pass
-
-        if self.robot_type == 'test':
-            sleep(1)
-            return True
-
-    def safe_disconnect(self):
-        """
-        Move robot for home position and close connection with robot. Home position dependes on robot type. For Gen3 is
-        [0.0, 0.0, 0.0, 0.0, 0.0, 0.0]  degrees and for Ned is [0.0, 0.3, -1.3, 0.0, 0.0, 0.0] radians.
-        :rtype: None
-
-        """
-        if self.robot_type == 'gen3':
-            ActionGen3(self.robot_instance).move_to_zero()
-            self.connection_instance.disconnect_robot()
-
-        if self.robot_type == 'ned':
-            ActionNed(self.robot_instance).move_to_home()
-            self.connection_instance.disconnect_robot()
-
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
-            sleep(1)
-            return True
-
-    # Move Joints/Cartesian methods
-    def joints(self):
-        return self.get_joints()
-
-    def get_joints(self):
-        """
-        Get joints value in radians
-        You can also use a getter ::
-
-            joints = robot.get_joints()
-            joints = robot.joints
-
-        :return: List of joints value
-        :rtype: list[float]
-        """
-        if self.robot_type == 'gen3':
-            return ActionGen3(self.robot_instance).get_joints()
-
-        if self.robot_type == 'ned':
-            return ActionNed(self.robot_instance).get_joints()
-
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
-            sleep(0.5)
-            return ['J1', 'J2', 'J3', 'J4', 'J5', 'J6']
-
-    def move_joints(self, j1, j2, j3, j4, j5, j6):
-        """
-        Move robot joints. Joints are expressed in degrees.
-
-        All lines of the next example realize the same operation: ::
-
-            robot.move_joints(0.2, 0.1, 0.3, 0.0, 0.5, 0.0)
-
-        :param j1: joint 1,
-        :type j1: float
-        :param j2: joint 2,
-        :type j2: float
-        :param j3: joint 3,
-        :type j3: float
-        :param j4: joint 4,
-        :type j4: float
-        :param j5: joint 5,
-        :type j5: float
-        :param j6: joint 6,
-        :type j6: float
-        :rtype: None
-        """
-        if self.robot_type == 'gen3':
-            ActionGen3(self.robot_instance).move_joints([j1, j2, j3, j4, j5, j6])
-
-        if self.robot_type == 'ned':
-            ActionNed(self.robot_instance).move_joints(j1, j2, j3, j4, j5, j6)
-
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
-            sleep(1)
-            return True
-
-    def cartesian(self):
-        return self.get_cartesian()
-
-    def get_cartesian(self):
-        """
-        Get end effector link pose as [x, y, z, roll, pitch, yaw].
-        x, y & z are expressed in meters / roll, pitch & yaw are expressed in radians
-        You can also use a getter ::
-
-            pose = robot.get_pose()
-            pose = robot.pose
-
-        :rtype: PoseObject
-        """
-        if self.robot_type == 'gen3':
-            return ActionGen3(self.robot_instance).get_cartesian()
-
-        if self.robot_type == 'ned':
-            return ActionNed(self.robot_instance).get_cartesian()
-
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
-            sleep(1)
-            return True
-
-    def move_cartesian(self, x, y, z, roll, pitch, yaw):
-        """
-        Move robot end effector pose to a (x, y, z, roll, pitch, yaw, frame_name) pose
-        in a particular frame (frame_name) if defined.
-        x, y & z are expressed in meters / roll, pitch & yaw are expressed in radians
-
-        All lines of the next example realize the same operation: ::
-
-            robot.move_cartesian(0.2, 0.1, 0.3, 0.0, 0.5, 0.0)
-
-        :param x: coordinate x,
-        :type x: float
-        :param y: coordinate y,
-        :type y: float
-        :param z: coordinate z,
-        :type z: float
-        :param roll: rotation on x-axis,
-        :type roll: float
-        :param pitch: rotation on y-axis,
-        :type pitch: float
-        :param yaw: rotation on z-axis,
-        :type yaw: float
-        :rtype: None
-        """
-        if self.robot_type == 'gen3':
-            return ActionGen3(self.robot_instance).move_cartesian([x, y, z, roll, pitch, yaw])
-
-        if self.robot_type == 'ned':
-            return ActionNed(self.robot_instance).move_cartesian(x, y, z, roll, pitch, yaw)
-
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
-            sleep(1)
-            return True
-
-    # TODO: Pegar os valores de home do robot
-    def move_to_home(self):
-        """
-        Move robot for home position. Home position dependes on robot type. For Gen3 is [0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
-        degrees and for Ned is [0.0, 0.3, -1.3, 0.0, 0.0, 0.0] radians.
-
-        :rtype: None
-        """
-        if self.robot_type == 'gen3':
-            ActionGen3(self.robot_instance).move_to_home()
-
-        if self.robot_type == 'ned':
-            ActionNed(self.robot_instance).move_to_home()
-
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
-            sleep(1)
-            return True
-
-    def move_to_zero(self):
-        """
-        Move robot for zero position. Home position dependes on robot type. For Gen3 is [0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
-        degrees and for Ned is [0.0, 0.0, 0.0, 0.0, 0.0, 0.0] radians.
-
-        :rtype: None
-        """
-        if self.robot_type == 'gen3':
-            ActionGen3(self.robot_instance).move_to_zero()
-
-        if self.robot_type == 'ned':
-            ActionNed(self.robot_instance).move_to_zero()
-
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
-            sleep(1)
-            return True
-
-    def open_gripper(self):
-        """
-        Open gripper.
-        :rtype: None
-        """
-        if self.robot_type == 'gen3':
-            ActionGen3(self.robot_instance).open_gripper()
-
-        if self.robot_type == 'ned':
-            ActionNed(self.robot_instance).open_gripper()
-
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
-            sleep(1)
-            return True
-
-    def close_gripper(self):
-        """
-        Close gripper
-        :rtype: None
-        """
-        if self.robot_type == 'gen3':
-            ActionGen3(self.robot_instance).close_gripper()
-
-        if self.robot_type == 'ned':
-            ActionNed(self.robot_instance).close_gripper()
-
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
-            sleep(1)
-            return True
-
-    # TODO: Ver a função de aumento de velocidade para o Gen3
-    def set_velocity(self, velocity):
-        """
-        Limit arm max velocity to a percentage of its maximum velocity. For niryo one, velocity is a percentage of 100.
-        For gen3, there are two types of velocities, an angular and a cartesian. The speed used in this method is
-        angular.
-
-        :param velocity: Should be between 1 & 100 for niryo
-        :type velocity: int
-        :rtype: None
-        """
-        if self.robot_type == 'gen3':
-            ActionGen3(self.robot_instance).set_velocity(velocity)
-
-        if self.robot_type == 'ned':
-            ActionNed(self.robot_instance).set_velocity(velocity)
-
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
-            sleep(1)
-            return True
-
-    def calibrate(self):
-        """
-        Start an automatic motors calibration if motors are not calibrated yet
-
-        :rtype: None
-        """
-        if self.robot_type == 'gen3':
-            print('Gen3 NÃO necessita de calibração')
-
-        if self.robot_type == 'ned':
-            ActionNed(self.robot_instance).calibrate()
-
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
-            sleep(1)
-            return True
-
-    def go_to_sleep(self):
-        """
-        Go home pose and activate learning mode. The function is avaliable only for Ned robot.
-
-        :rtype: None
-        """
-        if self.robot_type == 'gen3':
-            ...
-
-        if self.robot_type == 'ned':
-            ActionNed(self.robot_instance).go_to_sleep()
-
-        if self.robot_type == 'denso':
-            ...
-
-        if self.robot_type == 'test':
-            sleep(1)
-            return True
+from rria_api.ned.connect_ned import ConnectNed
+from rria_api.ned.action_ned import ActionNed
+from rria_api.gen3.connect_gen3 import ConnectGen3
+from rria_api.gen3.action_gen3 import ActionGen3
+from time import sleep
+
+
+class RobotObject:
+    def __init__(self, ip_address, robot_type):
+        self.ip_address = ip_address
+        self.robot_type = robot_type
+
+        # This atribute is used to store the general robot instance
+        self.robot_instance = None
+
+        # This atribute is used to store the general connection instance
+        self.connection_instance = None
+
+    def connect_robot(self):
+        """
+        Connect robot depends on the robot type
+        :rtype: bool
+
+        """
+
+        if self.robot_type == 'gen3':
+            try:
+                self.connection_instance = ConnectGen3(self.ip_address, ["admin", "admin"])
+                self.robot_instance = self.connection_instance.connect_robot()
+
+                return True
+
+            except(Exception,):
+                print('The connection attempt failed. Check the physical connection to the robot and try again later.')
+
+                return False
+
+        if self.robot_type == 'ned':
+            try:
+                self.connection_instance = ConnectNed()
+                self.robot_instance = self.connection_instance.connect_robot(self.ip_address)
+
+                return True
+
+            except(Exception,):
+                print('The connection attempt failed. Check the physical connection to the robot and try again later.')
+
+                return False
+
+        if self.robot_type == 'denso':
+            pass
+
+        if self.robot_type == 'test':
+            sleep(1)
+            return True
+
+    def disconnect_robot(self):
+        """
+        Close connection with robot
+        :rtype: None
+
+        """
+        if self.robot_type == 'gen3':
+            self.connection_instance.disconnect_robot()
+
+        if self.robot_type == 'ned':
+            self.connection_instance.disconnect_robot()
+
+        if self.robot_type == 'denso':
+            pass
+
+        if self.robot_type == 'test':
+            sleep(1)
+            return True
+
+    def safe_disconnect(self):
+        """
+        Move robot for home position and close connection with robot. Home position dependes on robot type. For Gen3 is
+        [0.0, 0.0, 0.0, 0.0, 0.0, 0.0]  degrees and for Ned is [0.0, 0.3, -1.3, 0.0, 0.0, 0.0] radians.
+        :rtype: None
+
+        """
+        if self.robot_type == 'gen3':
+            ActionGen3(self.robot_instance).move_to_zero()
+            self.connection_instance.disconnect_robot()
+
+        if self.robot_type == 'ned':
+            ActionNed(self.robot_instance).move_to_home()
+            self.connection_instance.disconnect_robot()
+
+        if self.robot_type == 'denso':
+            ...
+
+        if self.robot_type == 'test':
+            sleep(1)
+            return True
+
+    # Move Joints/Cartesian methods
+    def joints(self):
+        return self.get_joints()
+
+    def get_joints(self):
+        """
+        Get joints value in radians
+        You can also use a getter ::
+
+            joints = robot.get_joints()
+            joints = robot.joints
+
+        :return: List of joints value
+        :rtype: list[float]
+        """
+        if self.robot_type == 'gen3':
+            return ActionGen3(self.robot_instance).get_joints()
+
+        if self.robot_type == 'ned':
+            return ActionNed(self.robot_instance).get_joints()
+
+        if self.robot_type == 'denso':
+            ...
+
+        if self.robot_type == 'test':
+            sleep(0.5)
+            return ['J1', 'J2', 'J3', 'J4', 'J5', 'J6']
+
+    def move_joints(self, j1, j2, j3, j4, j5, j6):
+        """
+        Move robot joints. Joints are expressed in degrees.
+
+        All lines of the next example realize the same operation: ::
+
+            robot.move_joints(0.2, 0.1, 0.3, 0.0, 0.5, 0.0)
+
+        :param j1: joint 1,
+        :type j1: float
+        :param j2: joint 2,
+        :type j2: float
+        :param j3: joint 3,
+        :type j3: float
+        :param j4: joint 4,
+        :type j4: float
+        :param j5: joint 5,
+        :type j5: float
+        :param j6: joint 6,
+        :type j6: float
+        :rtype: None
+        """
+        if self.robot_type == 'gen3':
+            ActionGen3(self.robot_instance).move_joints([j1, j2, j3, j4, j5, j6])
+
+        if self.robot_type == 'ned':
+            ActionNed(self.robot_instance).move_joints(j1, j2, j3, j4, j5, j6)
+
+        if self.robot_type == 'denso':
+            ...
+
+        if self.robot_type == 'test':
+            sleep(1)
+            return True
+
+    def cartesian(self):
+        return self.get_cartesian()
+
+    def get_cartesian(self):
+        """
+        Get end effector link pose as [x, y, z, roll, pitch, yaw].
+        x, y & z are expressed in meters / roll, pitch & yaw are expressed in radians
+        You can also use a getter ::
+
+            pose = robot.get_pose()
+            pose = robot.pose
+
+        :rtype: PoseObject
+        """
+        if self.robot_type == 'gen3':
+            return ActionGen3(self.robot_instance).get_cartesian()
+
+        if self.robot_type == 'ned':
+            return ActionNed(self.robot_instance).get_cartesian()
+
+        if self.robot_type == 'denso':
+            ...
+
+        if self.robot_type == 'test':
+            sleep(1)
+            return True
+
+    def move_cartesian(self, x, y, z, roll, pitch, yaw):
+        """
+        Move robot end effector pose to a (x, y, z, roll, pitch, yaw, frame_name) pose
+        in a particular frame (frame_name) if defined.
+        x, y & z are expressed in meters / roll, pitch & yaw are expressed in radians
+
+        All lines of the next example realize the same operation: ::
+
+            robot.move_cartesian(0.2, 0.1, 0.3, 0.0, 0.5, 0.0)
+
+        :param x: coordinate x,
+        :type x: float
+        :param y: coordinate y,
+        :type y: float
+        :param z: coordinate z,
+        :type z: float
+        :param roll: rotation on x-axis,
+        :type roll: float
+        :param pitch: rotation on y-axis,
+        :type pitch: float
+        :param yaw: rotation on z-axis,
+        :type yaw: float
+        :rtype: None
+        """
+        if self.robot_type == 'gen3':
+            return ActionGen3(self.robot_instance).move_cartesian([x, y, z, roll, pitch, yaw])
+
+        if self.robot_type == 'ned':
+            return ActionNed(self.robot_instance).move_cartesian(x, y, z, roll, pitch, yaw)
+
+        if self.robot_type == 'denso':
+            ...
+
+        if self.robot_type == 'test':
+            sleep(1)
+            return True
+
+    # TODO: Pegar os valores de home do robot
+    def move_to_home(self):
+        """
+        Move robot for home position. Home position dependes on robot type. For Gen3 is [0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
+        degrees and for Ned is [0.0, 0.3, -1.3, 0.0, 0.0, 0.0] radians.
+
+        :rtype: None
+        """
+        if self.robot_type == 'gen3':
+            ActionGen3(self.robot_instance).move_to_home()
+
+        if self.robot_type == 'ned':
+            ActionNed(self.robot_instance).move_to_home()
+
+        if self.robot_type == 'denso':
+            ...
+
+        if self.robot_type == 'test':
+            sleep(1)
+            return True
+
+    def move_to_zero(self):
+        """
+        Move robot for zero position. Home position dependes on robot type. For Gen3 is [0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
+        degrees and for Ned is [0.0, 0.0, 0.0, 0.0, 0.0, 0.0] radians.
+
+        :rtype: None
+        """
+        if self.robot_type == 'gen3':
+            ActionGen3(self.robot_instance).move_to_zero()
+
+        if self.robot_type == 'ned':
+            ActionNed(self.robot_instance).move_to_zero()
+
+        if self.robot_type == 'denso':
+            ...
+
+        if self.robot_type == 'test':
+            sleep(1)
+            return True
+
+    def open_gripper(self):
+        """
+        Open gripper.
+        :rtype: None
+        """
+        if self.robot_type == 'gen3':
+            ActionGen3(self.robot_instance).open_gripper()
+
+        if self.robot_type == 'ned':
+            ActionNed(self.robot_instance).open_gripper()
+
+        if self.robot_type == 'denso':
+            ...
+
+        if self.robot_type == 'test':
+            sleep(1)
+            return True
+
+    def close_gripper(self):
+        """
+        Close gripper
+        :rtype: None
+        """
+        if self.robot_type == 'gen3':
+            ActionGen3(self.robot_instance).close_gripper()
+
+        if self.robot_type == 'ned':
+            ActionNed(self.robot_instance).close_gripper()
+
+        if self.robot_type == 'denso':
+            ...
+
+        if self.robot_type == 'test':
+            sleep(1)
+            return True
+
+    # TODO: Ver a função de aumento de velocidade para o Gen3
+    def set_velocity(self, velocity):
+        """
+        Limit arm max velocity to a percentage of its maximum velocity. For niryo one, velocity is a percentage of 100.
+        For gen3, there are two types of velocities, an angular and a cartesian. The speed used in this method is
+        angular.
+
+        :param velocity: Should be between 1 & 100 for niryo
+        :type velocity: int
+        :rtype: None
+        """
+        if self.robot_type == 'gen3':
+            ActionGen3(self.robot_instance).set_velocity(velocity)
+
+        if self.robot_type == 'ned':
+            ActionNed(self.robot_instance).set_velocity(velocity)
+
+        if self.robot_type == 'denso':
+            ...
+
+        if self.robot_type == 'test':
+            sleep(1)
+            return True
+
+    def calibrate(self):
+        """
+        Start an automatic motors calibration if motors are not calibrated yet
+
+        :rtype: None
+        """
+        if self.robot_type == 'gen3':
+            print('Gen3 NÃO necessita de calibração')
+
+        if self.robot_type == 'ned':
+            ActionNed(self.robot_instance).calibrate()
+
+        if self.robot_type == 'denso':
+            ...
+
+        if self.robot_type == 'test':
+            sleep(1)
+            return True
+
+    def go_to_sleep(self):
+        """
+        Go home pose and activate learning mode. The function is avaliable only for Ned robot.
+
+        :rtype: None
+        """
+        if self.robot_type == 'gen3':
+            ...
+
+        if self.robot_type == 'ned':
+            ActionNed(self.robot_instance).go_to_sleep()
+
+        if self.robot_type == 'denso':
+            ...
+
+        if self.robot_type == 'test':
+            sleep(1)
+            return True
```

