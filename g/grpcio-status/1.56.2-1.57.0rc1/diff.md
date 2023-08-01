# Comparing `tmp/grpcio-status-1.56.2.tar.gz` & `tmp/grpcio-status-1.57.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-status-1.56.2.tar", last modified: Fri Jul 14 18:03:47 2023, max compression
+gzip compressed data, was "grpcio-status-1.57.0rc1.tar", last modified: Mon Jul 24 22:25:53 2023, max compression
```

## Comparing `grpcio-status-1.56.2.tar` & `grpcio-status-1.57.0rc1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:03:47.178397 grpcio-status-1.56.2/
--rw-r--r--   0 root         (0) root         (0)    29687 2023-07-14 18:03:47.000000 grpcio-status-1.56.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-14 17:34:13.000000 grpcio-status-1.56.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1136 2023-07-14 18:03:47.174396 grpcio-status-1.56.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      284 2023-07-14 17:34:13.000000 grpcio-status-1.56.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:03:47.174396 grpcio-status-1.56.2/grpc_status/
--rw-r--r--   0 root         (0) root         (0)      580 2023-07-14 17:34:13.000000 grpcio-status-1.56.2/grpc_status/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1969 2023-07-14 17:34:13.000000 grpcio-status-1.56.2/grpc_status/_async.py
--rw-r--r--   0 root         (0) root         (0)      959 2023-07-14 17:34:13.000000 grpcio-status-1.56.2/grpc_status/_common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:03:47.166396 grpcio-status-1.56.2/grpc_status/google/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:03:47.174396 grpcio-status-1.56.2/grpc_status/google/rpc/
--rw-r--r--   0 root         (0) root         (0)     1924 2023-07-14 18:03:47.000000 grpcio-status-1.56.2/grpc_status/google/rpc/status.proto
--rw-r--r--   0 root         (0) root         (0)     3017 2023-07-14 17:34:13.000000 grpcio-status-1.56.2/grpc_status/rpc_status.py
--rw-r--r--   0 root         (0) root         (0)      699 2023-07-14 17:34:13.000000 grpcio-status-1.56.2/grpc_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:03:47.174396 grpcio-status-1.56.2/grpcio_status.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1136 2023-07-14 18:03:47.000000 grpcio-status-1.56.2/grpcio_status.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      473 2023-07-14 18:03:47.000000 grpcio-status-1.56.2/grpcio_status.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 18:03:47.000000 grpcio-status-1.56.2/grpcio_status.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-07-14 18:03:47.000000 grpcio-status-1.56.2/grpcio_status.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-14 18:03:47.000000 grpcio-status-1.56.2/grpcio_status.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 18:03:47.178397 grpcio-status-1.56.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3236 2023-07-14 17:34:13.000000 grpcio-status-1.56.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:25:53.620835 grpcio-status-1.57.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    29687 2023-07-24 22:25:53.000000 grpcio-status-1.57.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-24 21:57:15.000000 grpcio-status-1.57.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-07-24 22:25:53.620835 grpcio-status-1.57.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      284 2023-07-24 21:57:15.000000 grpcio-status-1.57.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:25:53.620835 grpcio-status-1.57.0rc1/grpc_status/
+-rw-r--r--   0 root         (0) root         (0)      580 2023-07-24 21:57:15.000000 grpcio-status-1.57.0rc1/grpc_status/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-07-24 21:57:15.000000 grpcio-status-1.57.0rc1/grpc_status/_async.py
+-rw-r--r--   0 root         (0) root         (0)      959 2023-07-24 21:57:15.000000 grpcio-status-1.57.0rc1/grpc_status/_common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:25:53.616834 grpcio-status-1.57.0rc1/grpc_status/google/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:25:53.620835 grpcio-status-1.57.0rc1/grpc_status/google/rpc/
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-07-24 22:25:53.000000 grpcio-status-1.57.0rc1/grpc_status/google/rpc/status.proto
+-rw-r--r--   0 root         (0) root         (0)     2992 2023-07-24 21:57:15.000000 grpcio-status-1.57.0rc1/grpc_status/rpc_status.py
+-rw-r--r--   0 root         (0) root         (0)      702 2023-07-24 21:57:15.000000 grpcio-status-1.57.0rc1/grpc_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:25:53.620835 grpcio-status-1.57.0rc1/grpcio_status.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-07-24 22:25:53.000000 grpcio-status-1.57.0rc1/grpcio_status.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      473 2023-07-24 22:25:53.000000 grpcio-status-1.57.0rc1/grpcio_status.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 22:25:53.000000 grpcio-status-1.57.0rc1/grpcio_status.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-07-24 22:25:53.000000 grpcio-status-1.57.0rc1/grpcio_status.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-24 22:25:53.000000 grpcio-status-1.57.0rc1/grpcio_status.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 22:25:53.620835 grpcio-status-1.57.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-07-24 21:57:15.000000 grpcio-status-1.57.0rc1/setup.py
```

### Comparing `grpcio-status-1.56.2/LICENSE` & `grpcio-status-1.57.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `grpcio-status-1.56.2/PKG-INFO` & `grpcio-status-1.57.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-status
-Version: 1.56.2
+Version: 1.57.0rc1
 Summary: Status proto mapping for gRPC
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `grpcio-status-1.56.2/grpc_status/__init__.py` & `grpcio-status-1.57.0rc1/grpc_status/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-status-1.56.2/grpc_status/_async.py` & `grpcio-status-1.57.0rc1/grpc_status/_async.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,20 +37,22 @@
     if trailing_metadata is None:
         return None
     for key, value in trailing_metadata:
         if key == GRPC_DETAILS_METADATA_KEY:
             rich_status = status_pb2.Status.FromString(value)
             if code.value[0] != rich_status.code:
                 raise ValueError(
-                    'Code in Status proto (%s) doesn\'t match status code (%s)'
-                    % (code_to_grpc_status_code(rich_status.code), code))
+                    "Code in Status proto (%s) doesn't match status code (%s)"
+                    % (code_to_grpc_status_code(rich_status.code), code)
+                )
             if details != rich_status.message:
                 raise ValueError(
-                    'Message in Status proto (%s) doesn\'t match status details (%s)'
-                    % (rich_status.message, details))
+                    "Message in Status proto (%s) doesn't match status details"
+                    " (%s)" % (rich_status.message, details)
+                )
             return rich_status
     return None
 
 
 __all__ = [
-    'from_call',
+    "from_call",
 ]
```

### Comparing `grpcio-status-1.56.2/grpc_status/google/rpc/status.proto` & `grpcio-status-1.57.0rc1/grpc_status/google/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `grpcio-status-1.56.2/grpc_status/rpc_status.py` & `grpcio-status-1.57.0rc1/grpc_status/rpc_status.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 import grpc
 
 from ._common import GRPC_DETAILS_METADATA_KEY
 from ._common import code_to_grpc_status_code
 
 
 class _Status(
-        collections.namedtuple('_Status',
-                               ('code', 'details', 'trailing_metadata')),
-        grpc.Status):
+    collections.namedtuple("_Status", ("code", "details", "trailing_metadata")),
+    grpc.Status,
+):
     pass
 
 
 def from_call(call):
     """Returns a google.rpc.status.Status message corresponding to a given grpc.Call.
 
     This is an EXPERIMENTAL API.
@@ -48,20 +48,22 @@
     if call.trailing_metadata() is None:
         return None
     for key, value in call.trailing_metadata():
         if key == GRPC_DETAILS_METADATA_KEY:
             rich_status = status_pb2.Status.FromString(value)
             if call.code().value[0] != rich_status.code:
                 raise ValueError(
-                    'Code in Status proto (%s) doesn\'t match status code (%s)'
-                    % (code_to_grpc_status_code(rich_status.code), call.code()))
+                    "Code in Status proto (%s) doesn't match status code (%s)"
+                    % (code_to_grpc_status_code(rich_status.code), call.code())
+                )
             if call.details() != rich_status.message:
                 raise ValueError(
-                    'Message in Status proto (%s) doesn\'t match status details (%s)'
-                    % (rich_status.message, call.details()))
+                    "Message in Status proto (%s) doesn't match status details"
+                    " (%s)" % (rich_status.message, call.details())
+                )
             return rich_status
     return None
 
 
 def to_status(status):
     """Convert a google.rpc.status.Status message to grpc.Status.
 
@@ -70,21 +72,25 @@
     Args:
       status: a google.rpc.status.Status message representing the non-OK status
         to terminate the RPC with and communicate it to the client.
 
     Returns:
       A grpc.Status instance representing the input google.rpc.status.Status message.
     """
-    return _Status(code=code_to_grpc_status_code(status.code),
-                   details=status.message,
-                   trailing_metadata=((GRPC_DETAILS_METADATA_KEY,
-                                       status.SerializeToString()),))
+    return _Status(
+        code=code_to_grpc_status_code(status.code),
+        details=status.message,
+        trailing_metadata=(
+            (GRPC_DETAILS_METADATA_KEY, status.SerializeToString()),
+        ),
+    )
 
 
 __all__ = [
-    'from_call',
-    'to_status',
+    "from_call",
+    "to_status",
 ]
 
 if sys.version_info[0] >= 3 and sys.version_info[1] >= 6:
     from . import _async as aio  # pylint: disable=unused-import
-    __all__.append('aio')
+
+    __all__.append("aio")
```

### Comparing `grpcio-status-1.56.2/grpc_version.py` & `grpcio-status-1.57.0rc1/grpc_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # AUTO-GENERATED FROM `$REPO_ROOT/templates/src/python/grpcio_status/grpc_version.py.template`!!!
 
-VERSION = '1.56.2'
+VERSION = '1.57.0rc1'
```

### Comparing `grpcio-status-1.56.2/grpcio_status.egg-info/PKG-INFO` & `grpcio-status-1.57.0rc1/grpcio_status.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-status
-Version: 1.56.2
+Version: 1.57.0rc1
 Summary: Status proto mapping for gRPC
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `grpcio-status-1.56.2/setup.py` & `grpcio-status-1.57.0rc1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,87 +14,89 @@
 """Setup module for the GRPC Python package's status mapping."""
 
 import os
 
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
-    'googleapis-common-protos>=1.5.5',
+    "protobuf>=4.21.6",
+    "grpcio>={version}".format(version=grpc_version.VERSION),
+    "googleapis-common-protos>=1.5.5",
 )
 
 try:
     import status_commands as _status_commands
 
     # we are in the build environment, otherwise the above import fails
     COMMAND_CLASS = {
         # Run preprocess from the repository *before* doing any packaging!
-        'preprocess': _status_commands.Preprocess,
-        'build_package_protos': _NoOpCommand,
+        "preprocess": _status_commands.Preprocess,
+        "build_package_protos": _NoOpCommand,
     }
 except ImportError:
     COMMAND_CLASS = {
         # wire up commands to no-op not to break the external dependencies
-        'preprocess': _NoOpCommand,
-        'build_package_protos': _NoOpCommand,
+        "preprocess": _NoOpCommand,
+        "build_package_protos": _NoOpCommand,
     }
 
-setuptools.setup(name='grpcio-status',
-                 version=grpc_version.VERSION,
-                 description='Status proto mapping for gRPC',
-                 long_description=open(_README_PATH, 'r').read(),
-                 author='The gRPC Authors',
-                 author_email='grpc-io@googlegroups.com',
-                 url='https://grpc.io',
-                 license='Apache License 2.0',
-                 classifiers=CLASSIFIERS,
-                 package_dir=PACKAGE_DIRECTORIES,
-                 packages=setuptools.find_packages('.'),
-                 python_requires='>=3.6',
-                 install_requires=INSTALL_REQUIRES,
-                 cmdclass=COMMAND_CLASS)
+setuptools.setup(
+    name="grpcio-status",
+    version=grpc_version.VERSION,
+    description="Status proto mapping for gRPC",
+    long_description=open(_README_PATH, "r").read(),
+    author="The gRPC Authors",
+    author_email="grpc-io@googlegroups.com",
+    url="https://grpc.io",
+    license="Apache License 2.0",
+    classifiers=CLASSIFIERS,
+    package_dir=PACKAGE_DIRECTORIES,
+    packages=setuptools.find_packages("."),
+    python_requires=">=3.6",
+    install_requires=INSTALL_REQUIRES,
+    cmdclass=COMMAND_CLASS,
+)
```

