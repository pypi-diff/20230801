# Comparing `tmp/grpcio-csds-1.56.2.tar.gz` & `tmp/grpcio-csds-1.57.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-csds-1.56.2.tar", last modified: Fri Jul 14 18:03:49 2023, max compression
+gzip compressed data, was "grpcio-csds-1.57.0rc1.tar", last modified: Mon Jul 24 22:25:55 2023, max compression
```

## Comparing `grpcio-csds-1.56.2.tar` & `grpcio-csds-1.57.0rc1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:03:49.382609 grpcio-csds-1.56.2/
--rw-r--r--   0 root         (0) root         (0)       94 2023-07-14 17:34:13.000000 grpcio-csds-1.56.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      960 2023-07-14 18:03:49.382609 grpcio-csds-1.56.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      511 2023-07-14 17:34:13.000000 grpcio-csds-1.56.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:03:49.378609 grpcio-csds-1.56.2/grpc_csds/
--rw-r--r--   0 root         (0) root         (0)     2149 2023-07-14 17:34:13.000000 grpcio-csds-1.56.2/grpc_csds/__init__.py
--rw-r--r--   0 root         (0) root         (0)      697 2023-07-14 17:34:13.000000 grpcio-csds-1.56.2/grpc_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:03:49.382609 grpcio-csds-1.56.2/grpcio_csds.egg-info/
--rw-r--r--   0 root         (0) root         (0)      960 2023-07-14 18:03:49.000000 grpcio-csds-1.56.2/grpcio_csds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      267 2023-07-14 18:03:49.000000 grpcio-csds-1.56.2/grpcio_csds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 18:03:49.000000 grpcio-csds-1.56.2/grpcio_csds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-07-14 18:03:49.000000 grpcio-csds-1.56.2/grpcio_csds.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-14 18:03:49.000000 grpcio-csds-1.56.2/grpcio_csds.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 18:03:49.382609 grpcio-csds-1.56.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2120 2023-07-14 17:34:13.000000 grpcio-csds-1.56.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:25:55.244832 grpcio-csds-1.57.0rc1/
+-rw-r--r--   0 root         (0) root         (0)       94 2023-07-24 21:57:15.000000 grpcio-csds-1.57.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      963 2023-07-24 22:25:55.244832 grpcio-csds-1.57.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      511 2023-07-24 21:57:15.000000 grpcio-csds-1.57.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:25:55.244832 grpcio-csds-1.57.0rc1/grpc_csds/
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-07-24 21:57:15.000000 grpcio-csds-1.57.0rc1/grpc_csds/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-07-24 21:57:15.000000 grpcio-csds-1.57.0rc1/grpc_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:25:55.244832 grpcio-csds-1.57.0rc1/grpcio_csds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      963 2023-07-24 22:25:55.000000 grpcio-csds-1.57.0rc1/grpcio_csds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      267 2023-07-24 22:25:55.000000 grpcio-csds-1.57.0rc1/grpcio_csds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 22:25:55.000000 grpcio-csds-1.57.0rc1/grpcio_csds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-24 22:25:55.000000 grpcio-csds-1.57.0rc1/grpcio_csds.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-24 22:25:55.000000 grpcio-csds-1.57.0rc1/grpcio_csds.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 22:25:55.248832 grpcio-csds-1.57.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-07-24 21:57:15.000000 grpcio-csds-1.57.0rc1/setup.py
```

### Comparing `grpcio-csds-1.56.2/PKG-INFO` & `grpcio-csds-1.57.0rc1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-csds
-Version: 1.56.2
+Version: 1.57.0rc1
 Summary: xDS configuration dump library
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `grpcio-csds-1.56.2/grpc_csds/__init__.py` & `grpcio-csds-1.57.0rc1/grpc_csds/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,41 +16,45 @@
 from envoy.service.status.v3 import csds_pb2
 from envoy.service.status.v3 import csds_pb2_grpc
 from google.protobuf import json_format
 from grpc._cython import cygrpc
 
 
 class ClientStatusDiscoveryServiceServicer(
-        csds_pb2_grpc.ClientStatusDiscoveryServiceServicer):
+    csds_pb2_grpc.ClientStatusDiscoveryServiceServicer
+):
     """CSDS Servicer works for both the sync API and asyncio API."""
 
     @staticmethod
     def FetchClientStatus(request, unused_context):
         client_config = csds_pb2.ClientConfig.FromString(
-            cygrpc.dump_xds_configs())
+            cygrpc.dump_xds_configs()
+        )
         response = csds_pb2.ClientStatusResponse()
         response.config.append(client_config)
         return response
 
     @staticmethod
     def StreamClientStatus(request_iterator, context):
         for request in request_iterator:
             yield ClientStatusDiscoveryServiceServicer.FetchClientStatus(
-                request, context)
+                request, context
+            )
 
 
 def add_csds_servicer(server):
     """Register CSDS servicer to a server.
 
     CSDS is part of xDS protocol used to expose in-effective traffic
     configuration (or xDS resources). It focuses on simplify the debugging of
     unexpected routing behaviors, which could be due to a misconfiguration,
     unhealthy backends or issues in the control or data plane.
 
     Args:
         server: A gRPC server to which the CSDS service will be added.
     """
     csds_pb2_grpc.add_ClientStatusDiscoveryServiceServicer_to_server(
-        ClientStatusDiscoveryServiceServicer(), server)
+        ClientStatusDiscoveryServiceServicer(), server
+    )
 
 
-__all__ = ['ClientStatusDiscoveryServiceServicer', 'add_csds_servicer']
+__all__ = ["ClientStatusDiscoveryServiceServicer", "add_csds_servicer"]
```

### Comparing `grpcio-csds-1.56.2/grpc_version.py` & `grpcio-csds-1.57.0rc1/grpc_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # AUTO-GENERATED FROM `$REPO_ROOT/templates/src/python/grpcio_csds/grpc_version.py.template`!!!
 
-VERSION = '1.56.2'
+VERSION = '1.57.0rc1'
```

### Comparing `grpcio-csds-1.56.2/grpcio_csds.egg-info/PKG-INFO` & `grpcio-csds-1.57.0rc1/grpcio_csds.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-csds
-Version: 1.56.2
+Version: 1.57.0rc1
 Summary: xDS configuration dump library
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `grpcio-csds-1.56.2/setup.py` & `grpcio-csds-1.57.0rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,47 +15,49 @@
 
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
 
 CLASSIFIERS = [
-    'Development Status :: 5 - Production/Stable',
-    'Programming Language :: Python',
-    'Programming Language :: Python :: 3',
-    'License :: OSI Approved :: Apache Software License',
+    "Development Status :: 5 - Production/Stable",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: Apache Software License",
 ]
 
 PACKAGE_DIRECTORIES = {
-    '': '.',
+    "": ".",
 }
 
 INSTALL_REQUIRES = (
-    'protobuf>=4.21.6',
-    'xds-protos>=0.0.7',
-    'grpcio>={version}'.format(version=grpc_version.VERSION),
+    "protobuf>=4.21.6",
+    "xds-protos>=0.0.7",
+    "grpcio>={version}".format(version=grpc_version.VERSION),
 )
 SETUP_REQUIRES = INSTALL_REQUIRES
 
-setuptools.setup(name='grpcio-csds',
-                 version=grpc_version.VERSION,
-                 license='Apache License 2.0',
-                 description='xDS configuration dump library',
-                 long_description=open(_README_PATH, 'r').read(),
-                 author='The gRPC Authors',
-                 author_email='grpc-io@googlegroups.com',
-                 classifiers=CLASSIFIERS,
-                 url='https://grpc.io',
-                 package_dir=PACKAGE_DIRECTORIES,
-                 packages=setuptools.find_packages('.'),
-                 python_requires='>=3.6',
-                 install_requires=INSTALL_REQUIRES,
-                 setup_requires=SETUP_REQUIRES)
+setuptools.setup(
+    name="grpcio-csds",
+    version=grpc_version.VERSION,
+    license="Apache License 2.0",
+    description="xDS configuration dump library",
+    long_description=open(_README_PATH, "r").read(),
+    author="The gRPC Authors",
+    author_email="grpc-io@googlegroups.com",
+    classifiers=CLASSIFIERS,
+    url="https://grpc.io",
+    package_dir=PACKAGE_DIRECTORIES,
+    packages=setuptools.find_packages("."),
+    python_requires=">=3.6",
+    install_requires=INSTALL_REQUIRES,
+    setup_requires=SETUP_REQUIRES,
+)
```

