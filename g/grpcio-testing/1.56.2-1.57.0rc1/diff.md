# Comparing `tmp/grpcio-testing-1.56.2.tar.gz` & `tmp/grpcio-testing-1.57.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-testing-1.56.2.tar", last modified: Fri Jul 14 18:03:43 2023, max compression
+gzip compressed data, was "grpcio-testing-1.57.0rc1.tar", last modified: Mon Jul 24 22:25:51 2023, max compression
```

## Comparing `grpcio-testing-1.56.2.tar` & `grpcio-testing-1.57.0rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:03:43.610055 grpcio-testing-1.56.2/
--rw-r--r--   0 root         (0) root         (0)    29687 2023-07-14 18:03:43.000000 grpcio-testing-1.56.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       97 2023-07-14 17:34:13.000000 grpcio-testing-1.56.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      488 2023-07-14 18:03:43.606054 grpcio-testing-1.56.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      266 2023-07-14 17:34:13.000000 grpcio-testing-1.56.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:03:43.586052 grpcio-testing-1.56.2/grpc_testing/
--rw-r--r--   0 root         (0) root         (0)    22851 2023-07-14 17:34:13.000000 grpcio-testing-1.56.2/grpc_testing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:03:43.594053 grpcio-testing-1.56.2/grpc_testing/_channel/
--rw-r--r--   0 root         (0) root         (0)      887 2023-07-14 17:34:13.000000 grpcio-testing-1.56.2/grpc_testing/_channel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2868 2023-07-14 17:34:13.000000 grpcio-testing-1.56.2/grpc_testing/_channel/_channel.py
--rw-r--r--   0 root         (0) root         (0)     3948 2023-07-14 17:34:13.000000 grpcio-testing-1.56.2/grpc_testing/_channel/_channel_rpc.py
--rw-r--r--   0 root         (0) root         (0)     1752 2023-07-14 17:34:13.000000 grpcio-testing-1.56.2/grpc_testing/_channel/_channel_state.py
--rw-r--r--   0 root         (0) root         (0)     8042 2023-07-14 17:34:13.000000 grpcio-testing-1.56.2/grpc_testing/_channel/_invocation.py
--rw-r--r--   0 root         (0) root         (0)     4781 2023-07-14 17:34:13.000000 grpcio-testing-1.56.2/grpc_testing/_channel/_multi_callable.py
--rw-r--r--   0 root         (0) root         (0)     7232 2023-07-14 17:34:13.000000 grpcio-testing-1.56.2/grpc_testing/_channel/_rpc_state.py
--rw-r--r--   0 root         (0) root         (0)     4373 2023-07-14 17:34:13.000000 grpcio-testing-1.56.2/grpc_testing/_common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:03:43.602054 grpcio-testing-1.56.2/grpc_testing/_server/
--rw-r--r--   0 root         (0) root         (0)      823 2023-07-14 17:34:13.000000 grpcio-testing-1.56.2/grpc_testing/_server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7405 2023-07-14 17:34:13.000000 grpcio-testing-1.56.2/grpc_testing/_server/_handler.py
--rw-r--r--   0 root         (0) root         (0)     5233 2023-07-14 17:34:13.000000 grpcio-testing-1.56.2/grpc_testing/_server/_rpc.py
--rw-r--r--   0 root         (0) root         (0)     6302 2023-07-14 17:34:13.000000 grpcio-testing-1.56.2/grpc_testing/_server/_server.py
--rw-r--r--   0 root         (0) root         (0)     2464 2023-07-14 17:34:13.000000 grpcio-testing-1.56.2/grpc_testing/_server/_server_rpc.py
--rw-r--r--   0 root         (0) root         (0)     2860 2023-07-14 17:34:13.000000 grpcio-testing-1.56.2/grpc_testing/_server/_service.py
--rw-r--r--   0 root         (0) root         (0)     2601 2023-07-14 17:34:13.000000 grpcio-testing-1.56.2/grpc_testing/_server/_servicer_context.py
--rw-r--r--   0 root         (0) root         (0)     7209 2023-07-14 17:34:13.000000 grpcio-testing-1.56.2/grpc_testing/_time.py
--rw-r--r--   0 root         (0) root         (0)      697 2023-07-14 17:34:13.000000 grpcio-testing-1.56.2/grpc_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:03:43.606054 grpcio-testing-1.56.2/grpcio_testing.egg-info/
--rw-r--r--   0 root         (0) root         (0)      488 2023-07-14 18:03:43.000000 grpcio-testing-1.56.2/grpcio_testing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1416 2023-07-14 18:03:43.000000 grpcio-testing-1.56.2/grpcio_testing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 18:03:43.000000 grpcio-testing-1.56.2/grpcio_testing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-14 18:03:43.000000 grpcio-testing-1.56.2/grpcio_testing.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 18:03:43.000000 grpcio-testing-1.56.2/grpcio_testing.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 18:03:43.610055 grpcio-testing-1.56.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2456 2023-07-14 17:34:13.000000 grpcio-testing-1.56.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:25:51.392839 grpcio-testing-1.57.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    29687 2023-07-24 22:25:51.000000 grpcio-testing-1.57.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       97 2023-07-24 21:57:15.000000 grpcio-testing-1.57.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      491 2023-07-24 22:25:51.392839 grpcio-testing-1.57.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-24 21:57:15.000000 grpcio-testing-1.57.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:25:51.384838 grpcio-testing-1.57.0rc1/grpc_testing/
+-rw-r--r--   0 root         (0) root         (0)    22799 2023-07-24 21:57:15.000000 grpcio-testing-1.57.0rc1/grpc_testing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:25:51.388838 grpcio-testing-1.57.0rc1/grpc_testing/_channel/
+-rw-r--r--   0 root         (0) root         (0)      887 2023-07-24 21:57:15.000000 grpcio-testing-1.57.0rc1/grpc_testing/_channel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2671 2023-07-24 21:57:15.000000 grpcio-testing-1.57.0rc1/grpc_testing/_channel/_channel.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2023-07-24 21:57:15.000000 grpcio-testing-1.57.0rc1/grpc_testing/_channel/_channel_rpc.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-07-24 21:57:15.000000 grpcio-testing-1.57.0rc1/grpc_testing/_channel/_channel_state.py
+-rw-r--r--   0 root         (0) root         (0)     8036 2023-07-24 21:57:15.000000 grpcio-testing-1.57.0rc1/grpc_testing/_channel/_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     4933 2023-07-24 21:57:15.000000 grpcio-testing-1.57.0rc1/grpc_testing/_channel/_multi_callable.py
+-rw-r--r--   0 root         (0) root         (0)     7246 2023-07-24 21:57:15.000000 grpcio-testing-1.57.0rc1/grpc_testing/_channel/_rpc_state.py
+-rw-r--r--   0 root         (0) root         (0)     4406 2023-07-24 21:57:15.000000 grpcio-testing-1.57.0rc1/grpc_testing/_common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:25:51.392839 grpcio-testing-1.57.0rc1/grpc_testing/_server/
+-rw-r--r--   0 root         (0) root         (0)      782 2023-07-24 21:57:15.000000 grpcio-testing-1.57.0rc1/grpc_testing/_server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7428 2023-07-24 21:57:15.000000 grpcio-testing-1.57.0rc1/grpc_testing/_server/_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5273 2023-07-24 21:57:15.000000 grpcio-testing-1.57.0rc1/grpc_testing/_server/_rpc.py
+-rw-r--r--   0 root         (0) root         (0)     6096 2023-07-24 21:57:15.000000 grpcio-testing-1.57.0rc1/grpc_testing/_server/_server.py
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-07-24 21:57:15.000000 grpcio-testing-1.57.0rc1/grpc_testing/_server/_server_rpc.py
+-rw-r--r--   0 root         (0) root         (0)     2846 2023-07-24 21:57:15.000000 grpcio-testing-1.57.0rc1/grpc_testing/_server/_service.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2023-07-24 21:57:15.000000 grpcio-testing-1.57.0rc1/grpc_testing/_server/_servicer_context.py
+-rw-r--r--   0 root         (0) root         (0)     7256 2023-07-24 21:57:15.000000 grpcio-testing-1.57.0rc1/grpc_testing/_time.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-07-24 21:57:15.000000 grpcio-testing-1.57.0rc1/grpc_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:25:51.392839 grpcio-testing-1.57.0rc1/grpcio_testing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      491 2023-07-24 22:25:51.000000 grpcio-testing-1.57.0rc1/grpcio_testing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-07-24 22:25:51.000000 grpcio-testing-1.57.0rc1/grpcio_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 22:25:51.000000 grpcio-testing-1.57.0rc1/grpcio_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-07-24 22:25:51.000000 grpcio-testing-1.57.0rc1/grpcio_testing.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 22:25:51.000000 grpcio-testing-1.57.0rc1/grpcio_testing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 22:25:51.392839 grpcio-testing-1.57.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2320 2023-07-24 21:57:15.000000 grpcio-testing-1.57.0rc1/setup.py
```

### Comparing `grpcio-testing-1.56.2/LICENSE` & `grpcio-testing-1.57.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.2/grpc_testing/__init__.py` & `grpcio-testing-1.57.0rc1/grpc_testing/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -489,16 +489,17 @@
         raise NotImplementedError()
 
 
 class Server(abc.ABC):
     """A server with which to test a system that services RPCs."""
 
     @abc.abstractmethod
-    def invoke_unary_unary(self, method_descriptor, invocation_metadata,
-                           request, timeout):
+    def invoke_unary_unary(
+        self, method_descriptor, invocation_metadata, request, timeout
+    ):
         """Invokes an RPC to be serviced by the system under test.
 
         Args:
           method_descriptor: A descriptor.MethodDescriptor describing a unary-unary
             RPC method.
           invocation_metadata: The RPC's invocation metadata.
           request: The RPC's request.
@@ -507,16 +508,17 @@
 
         Returns:
           A UnaryUnaryServerRpc with which to "play client" for the RPC.
         """
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def invoke_unary_stream(self, method_descriptor, invocation_metadata,
-                            request, timeout):
+    def invoke_unary_stream(
+        self, method_descriptor, invocation_metadata, request, timeout
+    ):
         """Invokes an RPC to be serviced by the system under test.
 
         Args:
           method_descriptor: A descriptor.MethodDescriptor describing a unary-stream
             RPC method.
           invocation_metadata: The RPC's invocation metadata.
           request: The RPC's request.
@@ -525,16 +527,17 @@
 
         Returns:
           A UnaryStreamServerRpc with which to "play client" for the RPC.
         """
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def invoke_stream_unary(self, method_descriptor, invocation_metadata,
-                            timeout):
+    def invoke_stream_unary(
+        self, method_descriptor, invocation_metadata, timeout
+    ):
         """Invokes an RPC to be serviced by the system under test.
 
         Args:
           method_descriptor: A descriptor.MethodDescriptor describing a stream-unary
             RPC method.
           invocation_metadata: The RPC's invocation metadata.
           timeout: A duration of time in seconds for the RPC or None to
@@ -542,16 +545,17 @@
 
         Returns:
           A StreamUnaryServerRpc with which to "play client" for the RPC.
         """
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def invoke_stream_stream(self, method_descriptor, invocation_metadata,
-                             timeout):
+    def invoke_stream_stream(
+        self, method_descriptor, invocation_metadata, timeout
+    ):
         """Invokes an RPC to be serviced by the system under test.
 
         Args:
           method_descriptor: A descriptor.MethodDescriptor describing a stream-stream
             RPC method.
           invocation_metadata: The RPC's invocation metadata.
           timeout: A duration of time in seconds for the RPC or None to
@@ -636,14 +640,15 @@
     be called at time t have been called before it describes the time
     as having advanced beyond t.
 
     Returns:
       A Time backed by the "system" (Python interpreter's) time.
     """
     from grpc_testing import _time
+
     return _time.StrictRealTime()
 
 
 def strict_fake_time(now):
     """Creates a Time that can be manipulated by test code.
 
     The returned instance maintains an internal representation of time
@@ -655,14 +660,15 @@
     be called at time t have been called before it describes the time
     as having advanced beyond t.
 
     Returns:
       A Time that simulates the passage of time.
     """
     from grpc_testing import _time
+
     return _time.StrictFakeTime(now)
 
 
 def channel(service_descriptors, time):
     """Creates a Channel for use in tests of a gRPC Python-using system.
 
     Args:
@@ -671,14 +677,15 @@
         system under test.
       time: A Time to be used for tests.
 
     Returns:
       A Channel for use in tests.
     """
     from grpc_testing import _channel
+
     return _channel.testing_channel(service_descriptors, time)
 
 
 def server_from_dictionary(descriptors_to_servicers, time):
     """Creates a Server for use in tests of a gRPC Python-using system.
 
     Args:
@@ -688,8 +695,9 @@
         modules) implementing those services.
       time: A Time to be used for tests.
 
     Returns:
       A Server for use in tests.
     """
     from grpc_testing import _server
+
     return _server.server_from_dictionary(descriptors_to_servicers, time)
```

### Comparing `grpcio-testing-1.56.2/grpc_testing/_channel/__init__.py` & `grpcio-testing-1.57.0rc1/grpc_testing/_channel/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.2/grpc_testing/_channel/_channel.py` & `grpcio-testing-1.57.0rc1/grpc_testing/_channel/_channel.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,47 +17,42 @@
 from grpc_testing._channel import _multi_callable
 
 
 # All serializer and deserializer parameters are not (yet) used by this
 # test infrastructure.
 # pylint: disable=unused-argument
 class TestingChannel(grpc_testing.Channel):
-
     def __init__(self, time, state):
         self._time = time
         self._state = state
 
     def subscribe(self, callback, try_to_connect=False):
         raise NotImplementedError()
 
     def unsubscribe(self, callback):
         raise NotImplementedError()
 
-    def unary_unary(self,
-                    method,
-                    request_serializer=None,
-                    response_deserializer=None):
+    def unary_unary(
+        self, method, request_serializer=None, response_deserializer=None
+    ):
         return _multi_callable.UnaryUnary(method, self._state)
 
-    def unary_stream(self,
-                     method,
-                     request_serializer=None,
-                     response_deserializer=None):
+    def unary_stream(
+        self, method, request_serializer=None, response_deserializer=None
+    ):
         return _multi_callable.UnaryStream(method, self._state)
 
-    def stream_unary(self,
-                     method,
-                     request_serializer=None,
-                     response_deserializer=None):
+    def stream_unary(
+        self, method, request_serializer=None, response_deserializer=None
+    ):
         return _multi_callable.StreamUnary(method, self._state)
 
-    def stream_stream(self,
-                      method,
-                      request_serializer=None,
-                      response_deserializer=None):
+    def stream_stream(
+        self, method, request_serializer=None, response_deserializer=None
+    ):
         return _multi_callable.StreamStream(method, self._state)
 
     def _close(self):
         # TODO(https://github.com/grpc/grpc/issues/12531): Decide what
         # action to take here, if any?
         pass
```

### Comparing `grpcio-testing-1.56.2/grpc_testing/_channel/_channel_rpc.py` & `grpcio-testing-1.57.0rc1/grpc_testing/_channel/_channel_rpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,31 +12,30 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import grpc_testing
 
 
 class _UnaryUnary(grpc_testing.UnaryUnaryChannelRpc):
-
     def __init__(self, rpc_state):
         self._rpc_state = rpc_state
 
     def send_initial_metadata(self, initial_metadata):
         self._rpc_state.send_initial_metadata(initial_metadata)
 
     def cancelled(self):
         self._rpc_state.cancelled()
 
     def terminate(self, response, trailing_metadata, code, details):
-        self._rpc_state.terminate_with_response(response, trailing_metadata,
-                                                code, details)
+        self._rpc_state.terminate_with_response(
+            response, trailing_metadata, code, details
+        )
 
 
 class _UnaryStream(grpc_testing.UnaryStreamChannelRpc):
-
     def __init__(self, rpc_state):
         self._rpc_state = rpc_state
 
     def send_initial_metadata(self, initial_metadata):
         self._rpc_state.send_initial_metadata(initial_metadata)
 
     def send_response(self, response):
@@ -46,15 +45,14 @@
         self._rpc_state.cancelled()
 
     def terminate(self, trailing_metadata, code, details):
         self._rpc_state.terminate(trailing_metadata, code, details)
 
 
 class _StreamUnary(grpc_testing.StreamUnaryChannelRpc):
-
     def __init__(self, rpc_state):
         self._rpc_state = rpc_state
 
     def send_initial_metadata(self, initial_metadata):
         self._rpc_state.send_initial_metadata(initial_metadata)
 
     def take_request(self):
@@ -63,20 +61,20 @@
     def requests_closed(self):
         return self._rpc_state.requests_closed()
 
     def cancelled(self):
         self._rpc_state.cancelled()
 
     def terminate(self, response, trailing_metadata, code, details):
-        self._rpc_state.terminate_with_response(response, trailing_metadata,
-                                                code, details)
+        self._rpc_state.terminate_with_response(
+            response, trailing_metadata, code, details
+        )
 
 
 class _StreamStream(grpc_testing.StreamStreamChannelRpc):
-
     def __init__(self, rpc_state):
         self._rpc_state = rpc_state
 
     def send_initial_metadata(self, initial_metadata):
         self._rpc_state.send_initial_metadata(initial_metadata)
 
     def take_request(self):
@@ -93,23 +91,27 @@
 
     def terminate(self, trailing_metadata, code, details):
         self._rpc_state.terminate(trailing_metadata, code, details)
 
 
 def unary_unary(channel_state, method_descriptor):
     rpc_state = channel_state.take_rpc_state(method_descriptor)
-    invocation_metadata, request = (
-        rpc_state.take_invocation_metadata_and_request())
+    (
+        invocation_metadata,
+        request,
+    ) = rpc_state.take_invocation_metadata_and_request()
     return invocation_metadata, request, _UnaryUnary(rpc_state)
 
 
 def unary_stream(channel_state, method_descriptor):
     rpc_state = channel_state.take_rpc_state(method_descriptor)
-    invocation_metadata, request = (
-        rpc_state.take_invocation_metadata_and_request())
+    (
+        invocation_metadata,
+        request,
+    ) = rpc_state.take_invocation_metadata_and_request()
     return invocation_metadata, request, _UnaryStream(rpc_state)
 
 
 def stream_unary(channel_state, method_descriptor):
     rpc_state = channel_state.take_rpc_state(method_descriptor)
     return rpc_state.take_invocation_metadata(), _StreamUnary(rpc_state)
```

### Comparing `grpcio-testing-1.56.2/grpc_testing/_channel/_channel_state.py` & `grpcio-testing-1.57.0rc1/grpc_testing/_channel/_channel_state.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,32 +16,39 @@
 import threading
 
 from grpc_testing import _common
 from grpc_testing._channel import _rpc_state
 
 
 class State(_common.ChannelHandler):
-
     def __init__(self):
         self._condition = threading.Condition()
         self._rpc_states = collections.defaultdict(list)
 
-    def invoke_rpc(self, method_full_rpc_name, invocation_metadata, requests,
-                   requests_closed, timeout):
-        rpc_state = _rpc_state.State(invocation_metadata, requests,
-                                     requests_closed)
+    def invoke_rpc(
+        self,
+        method_full_rpc_name,
+        invocation_metadata,
+        requests,
+        requests_closed,
+        timeout,
+    ):
+        rpc_state = _rpc_state.State(
+            invocation_metadata, requests, requests_closed
+        )
         with self._condition:
             self._rpc_states[method_full_rpc_name].append(rpc_state)
             self._condition.notify_all()
         return rpc_state
 
     def take_rpc_state(self, method_descriptor):
-        method_full_rpc_name = '/{}/{}'.format(
+        method_full_rpc_name = "/{}/{}".format(
             method_descriptor.containing_service.full_name,
-            method_descriptor.name)
+            method_descriptor.name,
+        )
         with self._condition:
             while True:
                 method_rpc_states = self._rpc_states[method_full_rpc_name]
                 if method_rpc_states:
                     return method_rpc_states.pop(0)
                 else:
                     self._condition.wait()
```

### Comparing `grpcio-testing-1.56.2/grpc_testing/_channel/_invocation.py` & `grpcio-testing-1.57.0rc1/grpc_testing/_channel/_invocation.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 _NOT_YET_OBSERVED = object()
 logging.basicConfig()
 _LOGGER = logging.getLogger(__name__)
 
 
 def _cancel(handler):
-    return handler.cancel(grpc.StatusCode.CANCELLED, 'Locally cancelled!')
+    return handler.cancel(grpc.StatusCode.CANCELLED, "Locally cancelled!")
 
 
 def _is_active(handler):
     return handler.is_active()
 
 
 def _time_remaining(unused_handler):
@@ -54,15 +54,14 @@
 
 def _details(handler):
     unused_trailing_metadata, unused_code, details = handler.termination()
     return details
 
 
 class _Call(grpc.Call):
-
     def __init__(self, handler):
         self._handler = handler
 
     def cancel(self):
         _cancel(self._handler)
 
     def is_active(self):
@@ -84,15 +83,14 @@
         return _code(self._handler)
 
     def details(self):
         return _details(self._handler)
 
 
 class _RpcErrorCall(grpc.RpcError, grpc.Call):
-
     def __init__(self, handler):
         self._handler = handler
 
     def cancel(self):
         _cancel(self._handler)
 
     def is_active(self):
@@ -124,24 +122,23 @@
     elif read.code is grpc.StatusCode.OK:
         raise StopIteration()
     else:
         raise _RpcErrorCall(handler)
 
 
 class _HandlerExtras(object):
-
     def __init__(self):
         self.condition = threading.Condition()
         self.unary_response = _NOT_YET_OBSERVED
         self.cancelled = False
 
 
 def _with_extras_cancel(handler, extras):
     with extras.condition:
-        if handler.cancel(grpc.StatusCode.CANCELLED, 'Locally cancelled!'):
+        if handler.cancel(grpc.StatusCode.CANCELLED, "Locally cancelled!"):
             extras.cancelled = True
             return True
         else:
             return False
 
 
 def _extras_without_cancelled(extras):
@@ -167,29 +164,28 @@
             else:
                 raise _RpcErrorCall(handler)
         else:
             return extras.unary_response
 
 
 def _exception(unused_handler):
-    raise NotImplementedError('TODO!')
+    raise NotImplementedError("TODO!")
 
 
 def _traceback(unused_handler):
-    raise NotImplementedError('TODO!')
+    raise NotImplementedError("TODO!")
 
 
 def _add_done_callback(handler, callback, future):
     adapted_callback = lambda: callback(future)
     if not handler.add_callback(adapted_callback):
         callback(future)
 
 
 class _FutureCall(grpc.Future, grpc.Call):
-
     def __init__(self, handler, extras):
         self._handler = handler
         self._extras = extras
 
     def cancel(self):
         return _with_extras_cancel(self._handler, self._extras)
 
@@ -233,27 +229,26 @@
         return _code(self._handler)
 
     def details(self):
         return _details(self._handler)
 
 
 def consume_requests(request_iterator, handler):
-
     def _consume():
         while True:
             try:
                 request = next(request_iterator)
                 added = handler.add_request(request)
                 if not added:
                     break
             except StopIteration:
                 handler.close_requests()
                 break
             except Exception:  # pylint: disable=broad-except
-                details = 'Exception iterating requests!'
+                details = "Exception iterating requests!"
                 _LOGGER.exception(details)
                 handler.cancel(grpc.StatusCode.UNKNOWN, details)
 
     consumption = threading.Thread(target=_consume)
     consumption.start()
 
 
@@ -282,15 +277,14 @@
 
 
 def future_call(handler):
     return _FutureCall(handler, _HandlerExtras())
 
 
 class ResponseIteratorCall(grpc.Call):
-
     def __init__(self, handler):
         self._handler = handler
 
     def __iter__(self):
         return self
 
     def __next__(self):
```

### Comparing `grpcio-testing-1.56.2/grpc_testing/_channel/_multi_callable.py` & `grpcio-testing-1.57.0rc1/grpc_testing/_channel/_multi_callable.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,103 +16,123 @@
 from grpc_testing import _common
 from grpc_testing._channel import _invocation
 
 
 # All per-call credentials parameters are unused by this test infrastructure.
 # pylint: disable=unused-argument
 class UnaryUnary(grpc.UnaryUnaryMultiCallable):
-
     def __init__(self, method_full_rpc_name, channel_handler):
         self._method_full_rpc_name = method_full_rpc_name
         self._channel_handler = channel_handler
 
     def __call__(self, request, timeout=None, metadata=None, credentials=None):
         rpc_handler = self._channel_handler.invoke_rpc(
-            self._method_full_rpc_name, _common.fuss_with_metadata(metadata),
-            [request], True, timeout)
+            self._method_full_rpc_name,
+            _common.fuss_with_metadata(metadata),
+            [request],
+            True,
+            timeout,
+        )
         return _invocation.blocking_unary_response(rpc_handler)
 
     def with_call(self, request, timeout=None, metadata=None, credentials=None):
         rpc_handler = self._channel_handler.invoke_rpc(
-            self._method_full_rpc_name, _common.fuss_with_metadata(metadata),
-            [request], True, timeout)
+            self._method_full_rpc_name,
+            _common.fuss_with_metadata(metadata),
+            [request],
+            True,
+            timeout,
+        )
         return _invocation.blocking_unary_response_with_call(rpc_handler)
 
     def future(self, request, timeout=None, metadata=None, credentials=None):
         rpc_handler = self._channel_handler.invoke_rpc(
-            self._method_full_rpc_name, _common.fuss_with_metadata(metadata),
-            [request], True, timeout)
+            self._method_full_rpc_name,
+            _common.fuss_with_metadata(metadata),
+            [request],
+            True,
+            timeout,
+        )
         return _invocation.future_call(rpc_handler)
 
 
 class UnaryStream(grpc.StreamStreamMultiCallable):
-
     def __init__(self, method_full_rpc_name, channel_handler):
         self._method_full_rpc_name = method_full_rpc_name
         self._channel_handler = channel_handler
 
     def __call__(self, request, timeout=None, metadata=None, credentials=None):
         rpc_handler = self._channel_handler.invoke_rpc(
-            self._method_full_rpc_name, _common.fuss_with_metadata(metadata),
-            [request], True, timeout)
+            self._method_full_rpc_name,
+            _common.fuss_with_metadata(metadata),
+            [request],
+            True,
+            timeout,
+        )
         return _invocation.ResponseIteratorCall(rpc_handler)
 
 
 class StreamUnary(grpc.StreamUnaryMultiCallable):
-
     def __init__(self, method_full_rpc_name, channel_handler):
         self._method_full_rpc_name = method_full_rpc_name
         self._channel_handler = channel_handler
 
-    def __call__(self,
-                 request_iterator,
-                 timeout=None,
-                 metadata=None,
-                 credentials=None):
-        rpc_handler = self._channel_handler.invoke_rpc(
-            self._method_full_rpc_name, _common.fuss_with_metadata(metadata),
-            [], False, timeout)
+    def __call__(
+        self, request_iterator, timeout=None, metadata=None, credentials=None
+    ):
+        rpc_handler = self._channel_handler.invoke_rpc(
+            self._method_full_rpc_name,
+            _common.fuss_with_metadata(metadata),
+            [],
+            False,
+            timeout,
+        )
         _invocation.consume_requests(request_iterator, rpc_handler)
         return _invocation.blocking_unary_response(rpc_handler)
 
-    def with_call(self,
-                  request_iterator,
-                  timeout=None,
-                  metadata=None,
-                  credentials=None):
-        rpc_handler = self._channel_handler.invoke_rpc(
-            self._method_full_rpc_name, _common.fuss_with_metadata(metadata),
-            [], False, timeout)
+    def with_call(
+        self, request_iterator, timeout=None, metadata=None, credentials=None
+    ):
+        rpc_handler = self._channel_handler.invoke_rpc(
+            self._method_full_rpc_name,
+            _common.fuss_with_metadata(metadata),
+            [],
+            False,
+            timeout,
+        )
         _invocation.consume_requests(request_iterator, rpc_handler)
         return _invocation.blocking_unary_response_with_call(rpc_handler)
 
-    def future(self,
-               request_iterator,
-               timeout=None,
-               metadata=None,
-               credentials=None):
-        rpc_handler = self._channel_handler.invoke_rpc(
-            self._method_full_rpc_name, _common.fuss_with_metadata(metadata),
-            [], False, timeout)
+    def future(
+        self, request_iterator, timeout=None, metadata=None, credentials=None
+    ):
+        rpc_handler = self._channel_handler.invoke_rpc(
+            self._method_full_rpc_name,
+            _common.fuss_with_metadata(metadata),
+            [],
+            False,
+            timeout,
+        )
         _invocation.consume_requests(request_iterator, rpc_handler)
         return _invocation.future_call(rpc_handler)
 
 
 class StreamStream(grpc.StreamStreamMultiCallable):
-
     def __init__(self, method_full_rpc_name, channel_handler):
         self._method_full_rpc_name = method_full_rpc_name
         self._channel_handler = channel_handler
 
-    def __call__(self,
-                 request_iterator,
-                 timeout=None,
-                 metadata=None,
-                 credentials=None):
-        rpc_handler = self._channel_handler.invoke_rpc(
-            self._method_full_rpc_name, _common.fuss_with_metadata(metadata),
-            [], False, timeout)
+    def __call__(
+        self, request_iterator, timeout=None, metadata=None, credentials=None
+    ):
+        rpc_handler = self._channel_handler.invoke_rpc(
+            self._method_full_rpc_name,
+            _common.fuss_with_metadata(metadata),
+            [],
+            False,
+            timeout,
+        )
         _invocation.consume_requests(request_iterator, rpc_handler)
         return _invocation.ResponseIteratorCall(rpc_handler)
 
 
 # pylint: enable=unused-argument
```

### Comparing `grpcio-testing-1.56.2/grpc_testing/_channel/_rpc_state.py` & `grpcio-testing-1.57.0rc1/grpc_testing/_channel/_rpc_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import threading
 
 import grpc
 from grpc_testing import _common
 
 
 class State(_common.ChannelRpcHandler):
-
     def __init__(self, invocation_metadata, requests, requests_closed):
         self._condition = threading.Condition()
         self._invocation_metadata = invocation_metadata
         self._requests = requests
         self._requests_closed = requests_closed
         self._initial_metadata = None
         self._responses = []
@@ -59,31 +58,36 @@
 
     def take_response(self):
         with self._condition:
             while True:
                 if self._code is grpc.StatusCode.OK:
                     if self._responses:
                         response = self._responses.pop(0)
-                        return _common.ChannelRpcRead(response, None, None,
-                                                      None)
+                        return _common.ChannelRpcRead(
+                            response, None, None, None
+                        )
                     else:
-                        return _common.ChannelRpcRead(None,
-                                                      self._trailing_metadata,
-                                                      grpc.StatusCode.OK,
-                                                      self._details)
+                        return _common.ChannelRpcRead(
+                            None,
+                            self._trailing_metadata,
+                            grpc.StatusCode.OK,
+                            self._details,
+                        )
                 elif self._code is None:
                     if self._responses:
                         response = self._responses.pop(0)
-                        return _common.ChannelRpcRead(response, None, None,
-                                                      None)
+                        return _common.ChannelRpcRead(
+                            response, None, None, None
+                        )
                     else:
                         self._condition.wait()
                 else:
-                    return _common.ChannelRpcRead(None, self._trailing_metadata,
-                                                  self._code, self._details)
+                    return _common.ChannelRpcRead(
+                        None, self._trailing_metadata, self._code, self._details
+                    )
 
     def termination(self):
         with self._condition:
             while True:
                 if self._code is None:
                     self._condition.wait()
                 else:
@@ -101,35 +105,36 @@
                 return True
             else:
                 return False
 
     def take_invocation_metadata(self):
         with self._condition:
             if self._invocation_metadata is None:
-                raise ValueError('Expected invocation metadata!')
+                raise ValueError("Expected invocation metadata!")
             else:
                 invocation_metadata = self._invocation_metadata
                 self._invocation_metadata = None
                 return invocation_metadata
 
     def take_invocation_metadata_and_request(self):
         with self._condition:
             if self._invocation_metadata is None:
-                raise ValueError('Expected invocation metadata!')
+                raise ValueError("Expected invocation metadata!")
             elif not self._requests:
-                raise ValueError('Expected at least one request!')
+                raise ValueError("Expected at least one request!")
             else:
                 invocation_metadata = self._invocation_metadata
                 self._invocation_metadata = None
                 return invocation_metadata, self._requests.pop(0)
 
     def send_initial_metadata(self, initial_metadata):
         with self._condition:
             self._initial_metadata = _common.fuss_with_metadata(
-                initial_metadata)
+                initial_metadata
+            )
             self._condition.notify_all()
 
     def take_request(self):
         with self._condition:
             while True:
                 if self._requests:
                     return self._requests.pop(0)
@@ -146,46 +151,50 @@
 
     def send_response(self, response):
         with self._condition:
             if self._code is None:
                 self._responses.append(response)
                 self._condition.notify_all()
 
-    def terminate_with_response(self, response, trailing_metadata, code,
-                                details):
+    def terminate_with_response(
+        self, response, trailing_metadata, code, details
+    ):
         with self._condition:
             if self._initial_metadata is None:
                 self._initial_metadata = _common.FUSSED_EMPTY_METADATA
             self._responses.append(response)
             self._trailing_metadata = _common.fuss_with_metadata(
-                trailing_metadata)
+                trailing_metadata
+            )
             self._code = code
             self._details = details
             self._condition.notify_all()
 
     def terminate(self, trailing_metadata, code, details):
         with self._condition:
             if self._initial_metadata is None:
                 self._initial_metadata = _common.FUSSED_EMPTY_METADATA
             self._trailing_metadata = _common.fuss_with_metadata(
-                trailing_metadata)
+                trailing_metadata
+            )
             self._code = code
             self._details = details
             self._condition.notify_all()
 
     def cancelled(self):
         with self._condition:
             while True:
                 if self._code is grpc.StatusCode.CANCELLED:
                     return
                 elif self._code is None:
                     self._condition.wait()
                 else:
-                    raise ValueError('Status code unexpectedly {}!'.format(
-                        self._code))
+                    raise ValueError(
+                        "Status code unexpectedly {}!".format(self._code)
+                    )
 
     def is_active(self):
         raise NotImplementedError()
 
     def time_remaining(self):
         raise NotImplementedError()
```

### Comparing `grpcio-testing-1.56.2/grpc_testing/_common.py` & `grpcio-testing-1.57.0rc1/grpc_testing/_common.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 """Common interfaces and implementation."""
 
 import abc
 import collections
 
 
 def _fuss(tuplified_metadata):
-    return tuplified_metadata + ((
-        'grpc.metadata_added_by_runtime',
-        'gRPC is allowed to add metadata in transmission and does so.',
-    ),)
+    return tuplified_metadata + (
+        (
+            "grpc.metadata_added_by_runtime",
+            "gRPC is allowed to add metadata in transmission and does so.",
+        ),
+    )
 
 
 FUSSED_EMPTY_METADATA = _fuss(())
 
 
 def fuss_with_metadata(metadata):
     if metadata is None:
@@ -34,32 +36,36 @@
         return _fuss(tuple(metadata))
 
 
 def rpc_names(service_descriptors):
     rpc_names_to_descriptors = {}
     for service_descriptor in service_descriptors:
         for method_descriptor in service_descriptor.methods_by_name.values():
-            rpc_name = '/{}/{}'.format(service_descriptor.full_name,
-                                       method_descriptor.name)
+            rpc_name = "/{}/{}".format(
+                service_descriptor.full_name, method_descriptor.name
+            )
             rpc_names_to_descriptors[rpc_name] = method_descriptor
     return rpc_names_to_descriptors
 
 
 class ChannelRpcRead(
-        collections.namedtuple('ChannelRpcRead', (
-            'response',
-            'trailing_metadata',
-            'code',
-            'details',
-        ))):
+    collections.namedtuple(
+        "ChannelRpcRead",
+        (
+            "response",
+            "trailing_metadata",
+            "code",
+            "details",
+        ),
+    )
+):
     pass
 
 
 class ChannelRpcHandler(abc.ABC):
-
     @abc.abstractmethod
     def initial_metadata(self):
         raise NotImplementedError()
 
     @abc.abstractmethod
     def add_request(self, request):
         raise NotImplementedError()
@@ -90,36 +96,44 @@
 
     @abc.abstractmethod
     def add_callback(self, callback):
         raise NotImplementedError()
 
 
 class ChannelHandler(abc.ABC):
-
     @abc.abstractmethod
-    def invoke_rpc(self, method_full_rpc_name, invocation_metadata, requests,
-                   requests_closed, timeout):
+    def invoke_rpc(
+        self,
+        method_full_rpc_name,
+        invocation_metadata,
+        requests,
+        requests_closed,
+        timeout,
+    ):
         raise NotImplementedError()
 
 
 class ServerRpcRead(
-        collections.namedtuple('ServerRpcRead', (
-            'request',
-            'requests_closed',
-            'terminated',
-        ))):
+    collections.namedtuple(
+        "ServerRpcRead",
+        (
+            "request",
+            "requests_closed",
+            "terminated",
+        ),
+    )
+):
     pass
 
 
 REQUESTS_CLOSED = ServerRpcRead(None, True, False)
 TERMINATED = ServerRpcRead(None, False, True)
 
 
 class ServerRpcHandler(abc.ABC):
-
     @abc.abstractmethod
     def send_initial_metadata(self, initial_metadata):
         raise NotImplementedError()
 
     @abc.abstractmethod
     def take_request(self):
         raise NotImplementedError()
@@ -134,27 +148,30 @@
 
     @abc.abstractmethod
     def add_termination_callback(self, callback):
         raise NotImplementedError()
 
 
 class Serverish(abc.ABC):
-
     @abc.abstractmethod
-    def invoke_unary_unary(self, method_descriptor, handler,
-                           invocation_metadata, request, deadline):
+    def invoke_unary_unary(
+        self, method_descriptor, handler, invocation_metadata, request, deadline
+    ):
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def invoke_unary_stream(self, method_descriptor, handler,
-                            invocation_metadata, request, deadline):
+    def invoke_unary_stream(
+        self, method_descriptor, handler, invocation_metadata, request, deadline
+    ):
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def invoke_stream_unary(self, method_descriptor, handler,
-                            invocation_metadata, deadline):
+    def invoke_stream_unary(
+        self, method_descriptor, handler, invocation_metadata, deadline
+    ):
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def invoke_stream_stream(self, method_descriptor, handler,
-                             invocation_metadata, deadline):
+    def invoke_stream_stream(
+        self, method_descriptor, handler, invocation_metadata, deadline
+    ):
         raise NotImplementedError()
```

### Comparing `grpcio-testing-1.56.2/grpc_testing/_server/__init__.py` & `grpcio-testing-1.57.0rc1/grpc_testing/_server/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,9 +12,10 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from grpc_testing._server import _server
 
 
 def server_from_dictionary(descriptors_to_servicers, time):
-    return _server.server_from_descriptor_to_servicers(descriptors_to_servicers,
-                                                       time)
+    return _server.server_from_descriptor_to_servicers(
+        descriptors_to_servicers, time
+    )
```

### Comparing `grpcio-testing-1.56.2/grpc_testing/_server/_handler.py` & `grpcio-testing-1.57.0rc1/grpc_testing/_server/_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 import grpc
 from grpc_testing import _common
 
 _CLIENT_INACTIVE = object()
 
 
 class Handler(_common.ServerRpcHandler):
-
     @abc.abstractmethod
     def initial_metadata(self):
         raise NotImplementedError()
 
     @abc.abstractmethod
     def add_request(self, request):
         raise NotImplementedError()
@@ -49,15 +48,14 @@
 
     @abc.abstractmethod
     def stream_response_termination(self):
         raise NotImplementedError()
 
 
 class _Handler(Handler):
-
     def __init__(self, requests_closed):
         self._condition = threading.Condition()
         self._requests = []
         self._requests_closed = requests_closed
         self._initial_metadata = None
         self._responses = []
         self._trailing_metadata = None
@@ -117,15 +115,16 @@
         with self._condition:
             while True:
                 if self._initial_metadata is None:
                     if self._code is None:
                         self._condition.wait()
                     else:
                         raise ValueError(
-                            'No initial metadata despite status code!')
+                            "No initial metadata despite status code!"
+                        )
                 else:
                     return self._initial_metadata
 
     def add_request(self, request):
         with self._condition:
             self._requests.append(request)
             self._condition.notify_all()
@@ -136,15 +135,15 @@
                 if self._responses:
                     response = self._responses.pop(0)
                     self._condition.notify_all()
                     return response
                 elif self._code is None:
                     self._condition.wait()
                 else:
-                    raise ValueError('No more responses!')
+                    raise ValueError("No more responses!")
 
     def requests_closed(self):
         with self._condition:
             self._requests_closed = True
             self._condition.notify_all()
 
     def cancel(self):
@@ -159,15 +158,15 @@
         for termination_callback in termination_callbacks:
             termination_callback()
 
     def unary_response_termination(self):
         with self._condition:
             while True:
                 if self._code is _CLIENT_INACTIVE:
-                    raise ValueError('Huh? Cancelled but wanting status?')
+                    raise ValueError("Huh? Cancelled but wanting status?")
                 elif self._code is None:
                     self._condition.wait()
                 else:
                     if self._unary_response is None:
                         if self._responses:
                             self._unary_response = self._responses.pop(0)
                     return (
@@ -177,28 +176,28 @@
                         self._details,
                     )
 
     def stream_response_termination(self):
         with self._condition:
             while True:
                 if self._code is _CLIENT_INACTIVE:
-                    raise ValueError('Huh? Cancelled but wanting status?')
+                    raise ValueError("Huh? Cancelled but wanting status?")
                 elif self._code is None:
                     self._condition.wait()
                 else:
                     return self._trailing_metadata, self._code, self._details
 
     def expire(self):
         with self._condition:
             if self._code is None:
                 if self._initial_metadata is None:
                     self._initial_metadata = _common.FUSSED_EMPTY_METADATA
                 self._trailing_metadata = _common.FUSSED_EMPTY_METADATA
                 self._code = grpc.StatusCode.DEADLINE_EXCEEDED
-                self._details = 'Took too much time!'
+                self._details = "Took too much time!"
                 termination_callbacks = self._termination_callbacks
                 self._termination_callbacks = None
                 self._condition.notify_all()
         for termination_callback in termination_callbacks:
             termination_callback()
 
     def set_expiration_future(self, expiration_future):
```

### Comparing `grpcio-testing-1.56.2/grpc_testing/_server/_rpc.py` & `grpcio-testing-1.57.0rc1/grpc_testing/_server/_rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from grpc_testing import _common
 
 logging.basicConfig()
 _LOGGER = logging.getLogger(__name__)
 
 
 class Rpc(object):
-
     def __init__(self, handler, invocation_metadata):
         self._condition = threading.Condition()
         self._handler = handler
         self._invocation_metadata = invocation_metadata
         self._initial_metadata_sent = False
         self._pending_trailing_metadata = None
         self._pending_code = None
@@ -46,15 +45,15 @@
         self._callbacks = None
 
         def call_back():
             for callback in callbacks:
                 try:
                     callback()
                 except Exception:  # pylint: disable=broad-except
-                    _LOGGER.exception('Exception calling server-side callback!')
+                    _LOGGER.exception("Exception calling server-side callback!")
 
         callback_calling_thread = threading.Thread(target=call_back)
         callback_calling_thread.start()
 
     def _terminate(self, trailing_metadata, code, details):
         if self._active:
             self._active = False
@@ -67,36 +66,39 @@
             trailing_metadata = _common.FUSSED_EMPTY_METADATA
         else:
             trailing_metadata = self._pending_trailing_metadata
         if self._pending_code is None:
             code = grpc.StatusCode.OK
         else:
             code = self._pending_code
-        details = '' if self._pending_details is None else self._pending_details
+        details = "" if self._pending_details is None else self._pending_details
         self._terminate(trailing_metadata, code, details)
 
     def _abort(self, code, details):
         self._terminate(_common.FUSSED_EMPTY_METADATA, code, details)
 
     def add_rpc_error(self, rpc_error):
         with self._condition:
             self._rpc_errors.append(rpc_error)
 
     def application_cancel(self):
         with self._condition:
-            self._abort(grpc.StatusCode.CANCELLED,
-                        'Cancelled by server-side application!')
+            self._abort(
+                grpc.StatusCode.CANCELLED,
+                "Cancelled by server-side application!",
+            )
 
     def application_exception_abort(self, exception):
         with self._condition:
             if exception not in self._rpc_errors:
-                _LOGGER.exception('Exception calling application!')
+                _LOGGER.exception("Exception calling application!")
                 self._abort(
                     grpc.StatusCode.UNKNOWN,
-                    'Exception calling application: {}'.format(exception))
+                    "Exception calling application: {}".format(exception),
+                )
 
     def extrinsic_abort(self):
         with self._condition:
             if self._active:
                 self._active = False
                 self._call_back()
                 self._condition.notify_all()
```

### Comparing `grpcio-testing-1.56.2/grpc_testing/_server/_server.py` & `grpcio-testing-1.57.0rc1/grpc_testing/_server/_server.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,130 +25,165 @@
 
 def _implementation(descriptors_to_servicers, method_descriptor):
     servicer = descriptors_to_servicers[method_descriptor.containing_service]
     return getattr(servicer, method_descriptor.name)
 
 
 def _unary_unary_service(request):
-
     def service(implementation, rpc, servicer_context):
         _service.unary_unary(implementation, rpc, request, servicer_context)
 
     return service
 
 
 def _unary_stream_service(request):
-
     def service(implementation, rpc, servicer_context):
         _service.unary_stream(implementation, rpc, request, servicer_context)
 
     return service
 
 
 def _stream_unary_service(handler):
-
     def service(implementation, rpc, servicer_context):
         _service.stream_unary(implementation, rpc, handler, servicer_context)
 
     return service
 
 
 def _stream_stream_service(handler):
-
     def service(implementation, rpc, servicer_context):
         _service.stream_stream(implementation, rpc, handler, servicer_context)
 
     return service
 
 
 class _Serverish(_common.Serverish):
-
     def __init__(self, descriptors_to_servicers, time):
         self._descriptors_to_servicers = descriptors_to_servicers
         self._time = time
 
-    def _invoke(self, service_behavior, method_descriptor, handler,
-                invocation_metadata, deadline):
-        implementation = _implementation(self._descriptors_to_servicers,
-                                         method_descriptor)
+    def _invoke(
+        self,
+        service_behavior,
+        method_descriptor,
+        handler,
+        invocation_metadata,
+        deadline,
+    ):
+        implementation = _implementation(
+            self._descriptors_to_servicers, method_descriptor
+        )
         rpc = _rpc.Rpc(handler, invocation_metadata)
         if handler.add_termination_callback(rpc.extrinsic_abort):
             servicer_context = _servicer_context.ServicerContext(
-                rpc, self._time, deadline)
-            service_thread = threading.Thread(target=service_behavior,
-                                              args=(
-                                                  implementation,
-                                                  rpc,
-                                                  servicer_context,
-                                              ))
+                rpc, self._time, deadline
+            )
+            service_thread = threading.Thread(
+                target=service_behavior,
+                args=(
+                    implementation,
+                    rpc,
+                    servicer_context,
+                ),
+            )
             service_thread.start()
 
-    def invoke_unary_unary(self, method_descriptor, handler,
-                           invocation_metadata, request, deadline):
-        self._invoke(_unary_unary_service(request), method_descriptor, handler,
-                     invocation_metadata, deadline)
-
-    def invoke_unary_stream(self, method_descriptor, handler,
-                            invocation_metadata, request, deadline):
-        self._invoke(_unary_stream_service(request), method_descriptor, handler,
-                     invocation_metadata, deadline)
-
-    def invoke_stream_unary(self, method_descriptor, handler,
-                            invocation_metadata, deadline):
-        self._invoke(_stream_unary_service(handler), method_descriptor, handler,
-                     invocation_metadata, deadline)
-
-    def invoke_stream_stream(self, method_descriptor, handler,
-                             invocation_metadata, deadline):
-        self._invoke(_stream_stream_service(handler), method_descriptor,
-                     handler, invocation_metadata, deadline)
+    def invoke_unary_unary(
+        self, method_descriptor, handler, invocation_metadata, request, deadline
+    ):
+        self._invoke(
+            _unary_unary_service(request),
+            method_descriptor,
+            handler,
+            invocation_metadata,
+            deadline,
+        )
+
+    def invoke_unary_stream(
+        self, method_descriptor, handler, invocation_metadata, request, deadline
+    ):
+        self._invoke(
+            _unary_stream_service(request),
+            method_descriptor,
+            handler,
+            invocation_metadata,
+            deadline,
+        )
+
+    def invoke_stream_unary(
+        self, method_descriptor, handler, invocation_metadata, deadline
+    ):
+        self._invoke(
+            _stream_unary_service(handler),
+            method_descriptor,
+            handler,
+            invocation_metadata,
+            deadline,
+        )
+
+    def invoke_stream_stream(
+        self, method_descriptor, handler, invocation_metadata, deadline
+    ):
+        self._invoke(
+            _stream_stream_service(handler),
+            method_descriptor,
+            handler,
+            invocation_metadata,
+            deadline,
+        )
 
 
 def _deadline_and_handler(requests_closed, time, timeout):
     if timeout is None:
         return None, _handler.handler_without_deadline(requests_closed)
     else:
         deadline = time.time() + timeout
-        handler = _handler.handler_with_deadline(requests_closed, time,
-                                                 deadline)
+        handler = _handler.handler_with_deadline(
+            requests_closed, time, deadline
+        )
         return deadline, handler
 
 
 class _Server(grpc_testing.Server):
-
     def __init__(self, serverish, time):
         self._serverish = serverish
         self._time = time
 
-    def invoke_unary_unary(self, method_descriptor, invocation_metadata,
-                           request, timeout):
+    def invoke_unary_unary(
+        self, method_descriptor, invocation_metadata, request, timeout
+    ):
         deadline, handler = _deadline_and_handler(True, self._time, timeout)
-        self._serverish.invoke_unary_unary(method_descriptor, handler,
-                                           invocation_metadata, request,
-                                           deadline)
+        self._serverish.invoke_unary_unary(
+            method_descriptor, handler, invocation_metadata, request, deadline
+        )
         return _server_rpc.UnaryUnaryServerRpc(handler)
 
-    def invoke_unary_stream(self, method_descriptor, invocation_metadata,
-                            request, timeout):
+    def invoke_unary_stream(
+        self, method_descriptor, invocation_metadata, request, timeout
+    ):
         deadline, handler = _deadline_and_handler(True, self._time, timeout)
-        self._serverish.invoke_unary_stream(method_descriptor, handler,
-                                            invocation_metadata, request,
-                                            deadline)
+        self._serverish.invoke_unary_stream(
+            method_descriptor, handler, invocation_metadata, request, deadline
+        )
         return _server_rpc.UnaryStreamServerRpc(handler)
 
-    def invoke_stream_unary(self, method_descriptor, invocation_metadata,
-                            timeout):
+    def invoke_stream_unary(
+        self, method_descriptor, invocation_metadata, timeout
+    ):
         deadline, handler = _deadline_and_handler(False, self._time, timeout)
-        self._serverish.invoke_stream_unary(method_descriptor, handler,
-                                            invocation_metadata, deadline)
+        self._serverish.invoke_stream_unary(
+            method_descriptor, handler, invocation_metadata, deadline
+        )
         return _server_rpc.StreamUnaryServerRpc(handler)
 
-    def invoke_stream_stream(self, method_descriptor, invocation_metadata,
-                             timeout):
+    def invoke_stream_stream(
+        self, method_descriptor, invocation_metadata, timeout
+    ):
         deadline, handler = _deadline_and_handler(False, self._time, timeout)
-        self._serverish.invoke_stream_stream(method_descriptor, handler,
-                                             invocation_metadata, deadline)
+        self._serverish.invoke_stream_stream(
+            method_descriptor, handler, invocation_metadata, deadline
+        )
         return _server_rpc.StreamStreamServerRpc(handler)
 
 
 def server_from_descriptor_to_servicers(descriptors_to_servicers, time):
     return _Server(_Serverish(descriptors_to_servicers, time), time)
```

### Comparing `grpcio-testing-1.56.2/grpc_testing/_server/_server_rpc.py` & `grpcio-testing-1.57.0rc1/grpc_testing/_server/_server_rpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,28 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import grpc_testing
 
 
 class UnaryUnaryServerRpc(grpc_testing.UnaryUnaryServerRpc):
-
     def __init__(self, handler):
         self._handler = handler
 
     def initial_metadata(self):
         return self._handler.initial_metadata()
 
     def cancel(self):
         self._handler.cancel()
 
     def termination(self):
         return self._handler.unary_response_termination()
 
 
 class UnaryStreamServerRpc(grpc_testing.UnaryStreamServerRpc):
-
     def __init__(self, handler):
         self._handler = handler
 
     def initial_metadata(self):
         return self._handler.initial_metadata()
 
     def take_response(self):
@@ -45,15 +43,14 @@
         self._handler.cancel()
 
     def termination(self):
         return self._handler.stream_response_termination()
 
 
 class StreamUnaryServerRpc(grpc_testing.StreamUnaryServerRpc):
-
     def __init__(self, handler):
         self._handler = handler
 
     def initial_metadata(self):
         return self._handler.initial_metadata()
 
     def send_request(self, request):
@@ -66,15 +63,14 @@
         self._handler.cancel()
 
     def termination(self):
         return self._handler.unary_response_termination()
 
 
 class StreamStreamServerRpc(grpc_testing.StreamStreamServerRpc):
-
     def __init__(self, handler):
         self._handler = handler
 
     def initial_metadata(self):
         return self._handler.initial_metadata()
 
     def send_request(self, request):
```

### Comparing `grpcio-testing-1.56.2/grpc_testing/_server/_service.py` & `grpcio-testing-1.57.0rc1/grpc_testing/_server/_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 import copy
 
 import grpc
 
 
 class _RequestIterator(object):
-
     def __init__(self, rpc, handler):
         self._rpc = rpc
         self._handler = handler
 
     def _next(self):
         read = self._handler.take_request()
         if read.requests_closed:
@@ -77,14 +76,16 @@
 
 
 def unary_stream(implementation, rpc, request, servicer_context):
     _stream_response(request, implementation, rpc, servicer_context)
 
 
 def stream_unary(implementation, rpc, handler, servicer_context):
-    _unary_response(_RequestIterator(rpc, handler), implementation, rpc,
-                    servicer_context)
+    _unary_response(
+        _RequestIterator(rpc, handler), implementation, rpc, servicer_context
+    )
 
 
 def stream_stream(implementation, rpc, handler, servicer_context):
-    _stream_response(_RequestIterator(rpc, handler), implementation, rpc,
-                     servicer_context)
+    _stream_response(
+        _RequestIterator(rpc, handler), implementation, rpc, servicer_context
+    )
```

### Comparing `grpcio-testing-1.56.2/grpc_testing/_server/_servicer_context.py` & `grpcio-testing-1.57.0rc1/grpc_testing/_server/_servicer_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 
 import grpc
 from grpc_testing import _common
 
 
 class ServicerContext(grpc.ServicerContext):
-
     def __init__(self, rpc, time, deadline):
         self._rpc = rpc
         self._time = time
         self._deadline = deadline
 
     def is_active(self):
         return self._rpc.is_active()
@@ -57,25 +56,28 @@
         raise NotImplementedError()
 
     def set_compression(self):
         raise NotImplementedError()
 
     def send_initial_metadata(self, initial_metadata):
         initial_metadata_sent = self._rpc.send_initial_metadata(
-            _common.fuss_with_metadata(initial_metadata))
+            _common.fuss_with_metadata(initial_metadata)
+        )
         if not initial_metadata_sent:
             raise ValueError(
-                'ServicerContext.send_initial_metadata called too late!')
+                "ServicerContext.send_initial_metadata called too late!"
+            )
 
     def disable_next_message_compression(self):
         raise NotImplementedError()
 
     def set_trailing_metadata(self, trailing_metadata):
         self._rpc.set_trailing_metadata(
-            _common.fuss_with_metadata(trailing_metadata))
+            _common.fuss_with_metadata(trailing_metadata)
+        )
 
     def abort(self, code, details):
         with self._rpc._condition:
             self._rpc._abort(code, details)
         raise Exception()
 
     def abort_with_status(self, status):
```

### Comparing `grpcio-testing-1.56.2/grpc_testing/_time.py` & `grpcio-testing-1.57.0rc1/grpc_testing/_time.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,64 +38,69 @@
     calling.start()
     # NOTE(nathaniel): Because this function is called from "strict" Time
     # implementations, it blocks until after all behaviors have terminated.
     calling.join()
 
 
 class _State(object):
-
     def __init__(self):
         self.condition = threading.Condition()
         self.times_to_behaviors = collections.defaultdict(list)
 
 
 class _Delta(
-        collections.namedtuple('_Delta', (
-            'mature_behaviors',
-            'earliest_mature_time',
-            'earliest_immature_time',
-        ))):
+    collections.namedtuple(
+        "_Delta",
+        (
+            "mature_behaviors",
+            "earliest_mature_time",
+            "earliest_immature_time",
+        ),
+    )
+):
     pass
 
 
 def _process(state, now):
     mature_behaviors = []
     earliest_mature_time = None
     while state.times_to_behaviors:
         earliest_time = min(state.times_to_behaviors)
         if earliest_time <= now:
             if earliest_mature_time is None:
                 earliest_mature_time = earliest_time
             earliest_mature_behaviors = state.times_to_behaviors.pop(
-                earliest_time)
+                earliest_time
+            )
             mature_behaviors.extend(earliest_mature_behaviors)
         else:
             earliest_immature_time = earliest_time
             break
     else:
         earliest_immature_time = None
-    return _Delta(mature_behaviors, earliest_mature_time,
-                  earliest_immature_time)
+    return _Delta(
+        mature_behaviors, earliest_mature_time, earliest_immature_time
+    )
 
 
 class _Future(grpc.Future):
-
     def __init__(self, state, behavior, time):
         self._state = state
         self._behavior = behavior
         self._time = time
         self._cancelled = False
 
     def cancel(self):
         with self._state.condition:
             if self._cancelled:
                 return True
             else:
                 behaviors_at_time = self._state.times_to_behaviors.get(
-                    self._time)
+                    self._time
+                )
                 if behaviors_at_time is None:
                     return False
                 else:
                     behaviors_at_time.remove(self._behavior)
                     if not behaviors_at_time:
                         self._state.times_to_behaviors.pop(self._time)
                         self._state.condition.notify_all()
@@ -122,15 +127,14 @@
         raise NotImplementedError()
 
     def add_done_callback(self, fn):
         raise NotImplementedError()
 
 
 class StrictRealTime(grpc_testing.Time):
-
     def __init__(self):
         self._state = _State()
         self._active = False
         self._calling = None
 
     def _activity(self):
         while True:
@@ -149,17 +153,18 @@
                     else:
                         timeout = max(0, delta.earliest_immature_time - now)
                         self._state.condition.wait(timeout=timeout)
             _call(delta.mature_behaviors)
 
     def _ensure_called_through(self, time):
         with self._state.condition:
-            while ((self._state.times_to_behaviors and
-                    min(self._state.times_to_behaviors) < time) or
-                   (self._calling is not None and self._calling < time)):
+            while (
+                self._state.times_to_behaviors
+                and min(self._state.times_to_behaviors) < time
+            ) or (self._calling is not None and self._calling < time):
                 self._state.condition.wait()
 
     def _call_at(self, behavior, time):
         with self._state.condition:
             self._state.times_to_behaviors[time].append(behavior)
             if self._active:
                 self._state.condition.notify_all()
@@ -185,15 +190,14 @@
 
     def sleep_until(self, time):
         _time.sleep(max(0, time - _time.time()))
         self._ensure_called_through(time)
 
 
 class StrictFakeTime(grpc_testing.Time):
-
     def __init__(self, time):
         self._state = _State()
         self._time = time
 
     def time(self):
         return self._time
```

### Comparing `grpcio-testing-1.56.2/grpc_version.py` & `grpcio-testing-1.57.0rc1/grpc_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # AUTO-GENERATED FROM `$REPO_ROOT/templates/src/python/grpcio_testing/grpc_version.py.template`!!!
 
-VERSION = '1.56.2'
+VERSION = '1.57.0rc1'
```

### Comparing `grpcio-testing-1.56.2/grpcio_testing.egg-info/SOURCES.txt` & `grpcio-testing-1.57.0rc1/grpcio_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.2/setup.py` & `grpcio-testing-1.57.0rc1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,67 +15,69 @@
 
 import os
 import sys
 
 import setuptools
 
 _PACKAGE_PATH = os.path.realpath(os.path.dirname(__file__))
-_README_PATH = os.path.join(_PACKAGE_PATH, 'README.rst')
+_README_PATH = os.path.join(_PACKAGE_PATH, "README.rst")
 
 # Ensure we're in the proper directory whether or not we're being used by pip.
 os.chdir(os.path.dirname(os.path.abspath(__file__)))
 
 # Break import style to ensure that we can find same-directory modules.
 import grpc_version
 
 
 class _NoOpCommand(setuptools.Command):
     """No-op command."""
 
-    description = ''
+    description = ""
     user_options = []
 
     def initialize_options(self):
         pass
 
     def finalize_options(self):
         pass
 
     def run(self):
         pass
 
 
 PACKAGE_DIRECTORIES = {
-    '': '.',
+    "": ".",
 }
 
 INSTALL_REQUIRES = (
-    'protobuf>=4.21.6',
-    'grpcio>={version}'.format(version=grpc_version.VERSION),
+    "protobuf>=4.21.6",
+    "grpcio>={version}".format(version=grpc_version.VERSION),
 )
 
 try:
     import testing_commands as _testing_commands
 
     # we are in the build environment, otherwise the above import fails
     COMMAND_CLASS = {
         # Run preprocess from the repository *before* doing any packaging!
-        'preprocess': _testing_commands.Preprocess,
+        "preprocess": _testing_commands.Preprocess,
     }
 except ImportError:
     COMMAND_CLASS = {
         # wire up commands to no-op not to break the external dependencies
-        'preprocess': _NoOpCommand,
+        "preprocess": _NoOpCommand,
     }
 
-setuptools.setup(name='grpcio-testing',
-                 version=grpc_version.VERSION,
-                 license='Apache License 2.0',
-                 description='Testing utilities for gRPC Python',
-                 long_description=open(_README_PATH, 'r').read(),
-                 author='The gRPC Authors',
-                 author_email='grpc-io@googlegroups.com',
-                 url='https://grpc.io',
-                 package_dir=PACKAGE_DIRECTORIES,
-                 packages=setuptools.find_packages('.'),
-                 install_requires=INSTALL_REQUIRES,
-                 cmdclass=COMMAND_CLASS)
+setuptools.setup(
+    name="grpcio-testing",
+    version=grpc_version.VERSION,
+    license="Apache License 2.0",
+    description="Testing utilities for gRPC Python",
+    long_description=open(_README_PATH, "r").read(),
+    author="The gRPC Authors",
+    author_email="grpc-io@googlegroups.com",
+    url="https://grpc.io",
+    package_dir=PACKAGE_DIRECTORIES,
+    packages=setuptools.find_packages("."),
+    install_requires=INSTALL_REQUIRES,
+    cmdclass=COMMAND_CLASS,
+)
```

