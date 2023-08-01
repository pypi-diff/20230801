# Comparing `tmp/grpcio-channelz-1.56.2.tar.gz` & `tmp/grpcio-channelz-1.57.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-channelz-1.56.2.tar", last modified: Fri Jul 14 18:03:44 2023, max compression
+gzip compressed data, was "grpcio-channelz-1.57.0rc1.tar", last modified: Mon Jul 24 22:25:51 2023, max compression
```

## Comparing `grpcio-channelz-1.56.2.tar` & `grpcio-channelz-1.57.0rc1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:03:44.590148 grpcio-channelz-1.56.2/
--rw-r--r--   0 root         (0) root         (0)    29687 2023-07-14 18:03:44.000000 grpcio-channelz-1.56.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-14 17:34:13.000000 grpcio-channelz-1.56.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1159 2023-07-14 18:03:44.590148 grpcio-channelz-1.56.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      281 2023-07-14 17:34:13.000000 grpcio-channelz-1.56.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:03:44.582147 grpcio-channelz-1.56.2/grpc_channelz/
--rw-r--r--   0 root         (0) root         (0)      580 2023-07-14 17:34:13.000000 grpcio-channelz-1.56.2/grpc_channelz/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:03:44.590148 grpcio-channelz-1.56.2/grpc_channelz/v1/
--rw-r--r--   0 root         (0) root         (0)      580 2023-07-14 17:34:13.000000 grpcio-channelz-1.56.2/grpc_channelz/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2761 2023-07-14 17:34:13.000000 grpcio-channelz-1.56.2/grpc_channelz/v1/_async.py
--rw-r--r--   0 root         (0) root         (0)     4469 2023-07-14 17:34:13.000000 grpcio-channelz-1.56.2/grpc_channelz/v1/_servicer.py
--rw-r--r--   0 root         (0) root         (0)     2419 2023-07-14 17:34:13.000000 grpcio-channelz-1.56.2/grpc_channelz/v1/channelz.py
--rw-r--r--   0 root         (0) root         (0)    16425 2023-07-14 18:03:44.000000 grpcio-channelz-1.56.2/grpc_channelz/v1/channelz_pb2.py
--rw-r--r--   0 root         (0) root         (0)    24126 2023-07-14 18:03:44.000000 grpcio-channelz-1.56.2/grpc_channelz/v1/channelz_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    13199 2023-07-14 18:03:44.000000 grpcio-channelz-1.56.2/grpc_channelz/v1/channelz_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-07-14 17:34:13.000000 grpcio-channelz-1.56.2/grpc_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:03:44.590148 grpcio-channelz-1.56.2/grpcio_channelz.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1159 2023-07-14 18:03:44.000000 grpcio-channelz-1.56.2/grpcio_channelz.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      721 2023-07-14 18:03:44.000000 grpcio-channelz-1.56.2/grpcio_channelz.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 18:03:44.000000 grpcio-channelz-1.56.2/grpcio_channelz.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-14 18:03:44.000000 grpcio-channelz-1.56.2/grpcio_channelz.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-14 18:03:44.000000 grpcio-channelz-1.56.2/grpcio_channelz.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 18:03:44.590148 grpcio-channelz-1.56.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3250 2023-07-14 17:34:13.000000 grpcio-channelz-1.56.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:25:51.960837 grpcio-channelz-1.57.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    29687 2023-07-24 22:25:51.000000 grpcio-channelz-1.57.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-24 21:57:15.000000 grpcio-channelz-1.57.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1162 2023-07-24 22:25:51.960837 grpcio-channelz-1.57.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      281 2023-07-24 21:57:15.000000 grpcio-channelz-1.57.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:25:51.956838 grpcio-channelz-1.57.0rc1/grpc_channelz/
+-rw-r--r--   0 root         (0) root         (0)      580 2023-07-24 21:57:15.000000 grpcio-channelz-1.57.0rc1/grpc_channelz/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:25:51.960837 grpcio-channelz-1.57.0rc1/grpc_channelz/v1/
+-rw-r--r--   0 root         (0) root         (0)      580 2023-07-24 21:57:15.000000 grpcio-channelz-1.57.0rc1/grpc_channelz/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2690 2023-07-24 21:57:15.000000 grpcio-channelz-1.57.0rc1/grpc_channelz/v1/_async.py
+-rw-r--r--   0 root         (0) root         (0)     4446 2023-07-24 21:57:15.000000 grpcio-channelz-1.57.0rc1/grpc_channelz/v1/_servicer.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-07-24 21:57:15.000000 grpcio-channelz-1.57.0rc1/grpc_channelz/v1/channelz.py
+-rw-r--r--   0 root         (0) root         (0)    16425 2023-07-24 22:25:51.000000 grpcio-channelz-1.57.0rc1/grpc_channelz/v1/channelz_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    24126 2023-07-24 22:25:51.000000 grpcio-channelz-1.57.0rc1/grpc_channelz/v1/channelz_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    13199 2023-07-24 22:25:51.000000 grpcio-channelz-1.57.0rc1/grpc_channelz/v1/channelz_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-07-24 21:57:15.000000 grpcio-channelz-1.57.0rc1/grpc_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:25:51.960837 grpcio-channelz-1.57.0rc1/grpcio_channelz.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1162 2023-07-24 22:25:51.000000 grpcio-channelz-1.57.0rc1/grpcio_channelz.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      721 2023-07-24 22:25:51.000000 grpcio-channelz-1.57.0rc1/grpcio_channelz.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 22:25:51.000000 grpcio-channelz-1.57.0rc1/grpcio_channelz.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-07-24 22:25:51.000000 grpcio-channelz-1.57.0rc1/grpcio_channelz.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-24 22:25:51.000000 grpcio-channelz-1.57.0rc1/grpcio_channelz.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 22:25:51.960837 grpcio-channelz-1.57.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3257 2023-07-24 21:57:15.000000 grpcio-channelz-1.57.0rc1/setup.py
```

### Comparing `grpcio-channelz-1.56.2/LICENSE` & `grpcio-channelz-1.57.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.56.2/PKG-INFO` & `grpcio-channelz-1.57.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-channelz
-Version: 1.56.2
+Version: 1.57.0rc1
 Summary: Channel Level Live Debug Information Service for gRPC
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `grpcio-channelz-1.56.2/grpc_channelz/__init__.py` & `grpcio-channelz-1.57.0rc1/grpc_channelz/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.56.2/grpc_channelz/v1/__init__.py` & `grpcio-channelz-1.57.0rc1/grpc_channelz/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.56.2/grpc_channelz/v1/_async.py` & `grpcio-channelz-1.57.0rc1/grpc_channelz/v1/_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,60 +10,59 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """AsyncIO version of Channelz servicer."""
 
 from grpc.experimental import aio
-from grpc_channelz.v1._servicer import \
-    ChannelzServicer as _SyncChannelzServicer
+from grpc_channelz.v1._servicer import ChannelzServicer as _SyncChannelzServicer
 import grpc_channelz.v1.channelz_pb2 as _channelz_pb2
 import grpc_channelz.v1.channelz_pb2_grpc as _channelz_pb2_grpc
 
 
 class ChannelzServicer(_channelz_pb2_grpc.ChannelzServicer):
     """AsyncIO servicer for handling RPCs for service statuses."""
 
     @staticmethod
     async def GetTopChannels(
-            request: _channelz_pb2.GetTopChannelsRequest,
-            context: aio.ServicerContext
+        request: _channelz_pb2.GetTopChannelsRequest,
+        context: aio.ServicerContext,
     ) -> _channelz_pb2.GetTopChannelsResponse:
         return _SyncChannelzServicer.GetTopChannels(request, context)
 
     @staticmethod
     async def GetServers(
-            request: _channelz_pb2.GetServersRequest,
-            context: aio.ServicerContext) -> _channelz_pb2.GetServersResponse:
+        request: _channelz_pb2.GetServersRequest, context: aio.ServicerContext
+    ) -> _channelz_pb2.GetServersResponse:
         return _SyncChannelzServicer.GetServers(request, context)
 
     @staticmethod
     async def GetServer(
-            request: _channelz_pb2.GetServerRequest,
-            context: aio.ServicerContext) -> _channelz_pb2.GetServerResponse:
+        request: _channelz_pb2.GetServerRequest, context: aio.ServicerContext
+    ) -> _channelz_pb2.GetServerResponse:
         return _SyncChannelzServicer.GetServer(request, context)
 
     @staticmethod
     async def GetServerSockets(
-            request: _channelz_pb2.GetServerSocketsRequest,
-            context: aio.ServicerContext
+        request: _channelz_pb2.GetServerSocketsRequest,
+        context: aio.ServicerContext,
     ) -> _channelz_pb2.GetServerSocketsResponse:
         return _SyncChannelzServicer.GetServerSockets(request, context)
 
     @staticmethod
     async def GetChannel(
-            request: _channelz_pb2.GetChannelRequest,
-            context: aio.ServicerContext) -> _channelz_pb2.GetChannelResponse:
+        request: _channelz_pb2.GetChannelRequest, context: aio.ServicerContext
+    ) -> _channelz_pb2.GetChannelResponse:
         return _SyncChannelzServicer.GetChannel(request, context)
 
     @staticmethod
     async def GetSubchannel(
-            request: _channelz_pb2.GetSubchannelRequest,
-            context: aio.ServicerContext
+        request: _channelz_pb2.GetSubchannelRequest,
+        context: aio.ServicerContext,
     ) -> _channelz_pb2.GetSubchannelResponse:
         return _SyncChannelzServicer.GetSubchannel(request, context)
 
     @staticmethod
     async def GetSocket(
-            request: _channelz_pb2.GetSocketRequest,
-            context: aio.ServicerContext) -> _channelz_pb2.GetSocketResponse:
+        request: _channelz_pb2.GetSocketRequest, context: aio.ServicerContext
+    ) -> _channelz_pb2.GetSocketResponse:
         return _SyncChannelzServicer.GetSocket(request, context)
```

### Comparing `grpcio-channelz-1.56.2/grpc_channelz/v1/_servicer.py` & `grpcio-channelz-1.57.0rc1/grpc_channelz/v1/_servicer.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,17 +59,19 @@
             context.set_code(grpc.StatusCode.INTERNAL)
             context.set_details(str(e))
 
     @staticmethod
     def GetServerSockets(request, context):
         try:
             return json_format.Parse(
-                cygrpc.channelz_get_server_sockets(request.server_id,
-                                                   request.start_socket_id,
-                                                   request.max_results),
+                cygrpc.channelz_get_server_sockets(
+                    request.server_id,
+                    request.start_socket_id,
+                    request.max_results,
+                ),
                 _channelz_pb2.GetServerSocketsResponse(),
             )
         except ValueError as e:
             context.set_code(grpc.StatusCode.NOT_FOUND)
             context.set_details(str(e))
         except json_format.ParseError as e:
             context.set_code(grpc.StatusCode.INTERNAL)
```

### Comparing `grpcio-channelz-1.56.2/grpc_channelz/v1/channelz.py` & `grpcio-channelz-1.57.0rc1/grpc_channelz/v1/channelz.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,35 +39,37 @@
     server: A gRPC server to which Channelz service will be added.
 """
 
 if sys.version_info[0] >= 3 and sys.version_info[1] >= 6:
     from grpc_channelz.v1 import _async as aio
 
     def add_channelz_servicer(server):
-
         if isinstance(server, grpc.experimental.aio.Server):
             _channelz_pb2_grpc.add_ChannelzServicer_to_server(
-                aio.ChannelzServicer(), server)
+                aio.ChannelzServicer(), server
+            )
         else:
             _channelz_pb2_grpc.add_ChannelzServicer_to_server(
-                ChannelzServicer(), server)
+                ChannelzServicer(), server
+            )
 
     add_channelz_servicer.__doc__ = _add_channelz_servicer_doc
 
     __all__ = [
         "aio",
         "add_channelz_servicer",
         "ChannelzServicer",
     ]
 
 else:
 
     def add_channelz_servicer(server):
         _channelz_pb2_grpc.add_ChannelzServicer_to_server(
-            ChannelzServicer(), server)
+            ChannelzServicer(), server
+        )
 
     add_channelz_servicer.__doc__ = _add_channelz_servicer_doc
 
     __all__ = [
         "add_channelz_servicer",
         "ChannelzServicer",
     ]
```

### Comparing `grpcio-channelz-1.56.2/grpc_channelz/v1/channelz_pb2.py` & `grpcio-channelz-1.57.0rc1/grpc_channelz/v1/channelz_pb2.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.56.2/grpc_channelz/v1/channelz_pb2.pyi` & `grpcio-channelz-1.57.0rc1/grpc_channelz/v1/channelz_pb2.pyi`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.56.2/grpc_channelz/v1/channelz_pb2_grpc.py` & `grpcio-channelz-1.57.0rc1/grpc_channelz/v1/channelz_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.56.2/grpc_version.py` & `grpcio-channelz-1.57.0rc1/grpc_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # AUTO-GENERATED FROM `$REPO_ROOT/templates/src/python/grpcio_channelz/grpc_version.py.template`!!!
 
-VERSION = '1.56.2'
+VERSION = '1.57.0rc1'
```

### Comparing `grpcio-channelz-1.56.2/grpcio_channelz.egg-info/PKG-INFO` & `grpcio-channelz-1.57.0rc1/grpcio_channelz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-channelz
-Version: 1.56.2
+Version: 1.57.0rc1
 Summary: Channel Level Live Debug Information Service for gRPC
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `grpcio-channelz-1.56.2/grpcio_channelz.egg-info/SOURCES.txt` & `grpcio-channelz-1.57.0rc1/grpcio_channelz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.56.2/setup.py` & `grpcio-channelz-1.57.0rc1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,91 +15,93 @@
 
 import os
 import sys
 
 import setuptools
 
 _PACKAGE_PATH = os.path.realpath(os.path.dirname(__file__))
-_README_PATH = os.path.join(_PACKAGE_PATH, 'README.rst')
+_README_PATH = os.path.join(_PACKAGE_PATH, "README.rst")
 
 # Ensure we're in the proper directory whether or not we're being used by pip.
 os.chdir(os.path.dirname(os.path.abspath(__file__)))
 
 # Break import-style to ensure we can actually find our local modules.
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
 
 
 CLASSIFIERS = [
-    'Development Status :: 5 - Production/Stable',
-    'Programming Language :: Python',
-    'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.4',
-    'Programming Language :: Python :: 3.5',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
-    'Programming Language :: Python :: 3.11',
-    'License :: OSI Approved :: Apache Software License',
+    "Development Status :: 5 - Production/Stable",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.4",
+    "Programming Language :: Python :: 3.5",
+    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "License :: OSI Approved :: Apache Software License",
 ]
 
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
     import channelz_commands as _channelz_commands
 
     # we are in the build environment, otherwise the above import fails
-    SETUP_REQUIRES = ('grpcio-tools=={version}'.format(
-        version=grpc_version.VERSION),)
+    SETUP_REQUIRES = (
+        "grpcio-tools=={version}".format(version=grpc_version.VERSION),
+    )
     COMMAND_CLASS = {
         # Run preprocess from the repository *before* doing any packaging!
-        'preprocess': _channelz_commands.Preprocess,
-        'build_package_protos': _channelz_commands.BuildPackageProtos,
+        "preprocess": _channelz_commands.Preprocess,
+        "build_package_protos": _channelz_commands.BuildPackageProtos,
     }
 except ImportError:
     SETUP_REQUIRES = ()
     COMMAND_CLASS = {
         # wire up commands to no-op not to break the external dependencies
-        'preprocess': _NoOpCommand,
-        'build_package_protos': _NoOpCommand,
+        "preprocess": _NoOpCommand,
+        "build_package_protos": _NoOpCommand,
     }
 
 setuptools.setup(
-    name='grpcio-channelz',
+    name="grpcio-channelz",
     version=grpc_version.VERSION,
-    license='Apache License 2.0',
-    description='Channel Level Live Debug Information Service for gRPC',
-    long_description=open(_README_PATH, 'r').read(),
-    author='The gRPC Authors',
-    author_email='grpc-io@googlegroups.com',
+    license="Apache License 2.0",
+    description="Channel Level Live Debug Information Service for gRPC",
+    long_description=open(_README_PATH, "r").read(),
+    author="The gRPC Authors",
+    author_email="grpc-io@googlegroups.com",
     classifiers=CLASSIFIERS,
-    url='https://grpc.io',
+    url="https://grpc.io",
     package_dir=PACKAGE_DIRECTORIES,
-    packages=setuptools.find_packages('.'),
-    python_requires='>=3.6',
+    packages=setuptools.find_packages("."),
+    python_requires=">=3.6",
     install_requires=INSTALL_REQUIRES,
     setup_requires=SETUP_REQUIRES,
-    cmdclass=COMMAND_CLASS)
+    cmdclass=COMMAND_CLASS,
+)
```

