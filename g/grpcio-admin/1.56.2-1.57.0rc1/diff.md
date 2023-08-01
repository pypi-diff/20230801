# Comparing `tmp/grpcio-admin-1.56.2.tar.gz` & `tmp/grpcio-admin-1.57.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-admin-1.56.2.tar", last modified: Fri Jul 14 18:03:57 2023, max compression
+gzip compressed data, was "grpcio-admin-1.57.0rc1.tar", last modified: Mon Jul 24 22:25:59 2023, max compression
```

## Comparing `grpcio-admin-1.56.2.tar` & `grpcio-admin-1.57.0rc1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:03:57.399382 grpcio-admin-1.56.2/
--rw-r--r--   0 root         (0) root         (0)       95 2023-07-14 17:34:13.000000 grpcio-admin-1.56.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1315 2023-07-14 18:03:57.399382 grpcio-admin-1.56.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      865 2023-07-14 17:34:13.000000 grpcio-admin-1.56.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:03:57.395382 grpcio-admin-1.56.2/grpc_admin/
--rw-r--r--   0 root         (0) root         (0)     1621 2023-07-14 17:34:13.000000 grpcio-admin-1.56.2/grpc_admin/__init__.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-07-14 17:34:13.000000 grpcio-admin-1.56.2/grpc_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:03:57.399382 grpcio-admin-1.56.2/grpcio_admin.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1315 2023-07-14 18:03:57.000000 grpcio-admin-1.56.2/grpcio_admin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      274 2023-07-14 18:03:57.000000 grpcio-admin-1.56.2/grpcio_admin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 18:03:57.000000 grpcio-admin-1.56.2/grpcio_admin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-14 18:03:57.000000 grpcio-admin-1.56.2/grpcio_admin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-14 18:03:57.000000 grpcio-admin-1.56.2/grpcio_admin.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 18:03:57.399382 grpcio-admin-1.56.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2159 2023-07-14 17:34:13.000000 grpcio-admin-1.56.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:25:59.916823 grpcio-admin-1.57.0rc1/
+-rw-r--r--   0 root         (0) root         (0)       95 2023-07-24 21:57:15.000000 grpcio-admin-1.57.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-07-24 22:25:59.912824 grpcio-admin-1.57.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      865 2023-07-24 21:57:15.000000 grpcio-admin-1.57.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:25:59.912824 grpcio-admin-1.57.0rc1/grpc_admin/
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-07-24 21:57:15.000000 grpcio-admin-1.57.0rc1/grpc_admin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-07-24 21:57:15.000000 grpcio-admin-1.57.0rc1/grpc_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 22:25:59.912824 grpcio-admin-1.57.0rc1/grpcio_admin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-07-24 22:25:59.000000 grpcio-admin-1.57.0rc1/grpcio_admin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      274 2023-07-24 22:25:59.000000 grpcio-admin-1.57.0rc1/grpcio_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 22:25:59.000000 grpcio-admin-1.57.0rc1/grpcio_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-24 22:25:59.000000 grpcio-admin-1.57.0rc1/grpcio_admin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-24 22:25:59.000000 grpcio-admin-1.57.0rc1/grpcio_admin.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 22:25:59.916823 grpcio-admin-1.57.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1997 2023-07-24 21:57:15.000000 grpcio-admin-1.57.0rc1/setup.py
```

### Comparing `grpcio-admin-1.56.2/PKG-INFO` & `grpcio-admin-1.57.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-admin
-Version: 1.56.2
+Version: 1.57.0rc1
 Summary: a collection of admin services
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `grpcio-admin-1.56.2/README.rst` & `grpcio-admin-1.57.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `grpcio-admin-1.56.2/grpc_admin/__init__.py` & `grpcio-admin-1.57.0rc1/grpc_admin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,22 +21,22 @@
     """Register admin servicers to a server.
 
     gRPC provides some predefined admin services to make debugging easier by
     exposing gRPC's internal states. Each existing admin service is packaged as
     a separate library, and the documentation of the predefined admin services
     is usually scattered. It can be time consuming to get the dependency
     management, module initialization, and library import right for each one of
-    them. 
+    them.
 
     This API provides a convenient way to create a gRPC server to expose admin
     services. With this, any new admin services that you may add in the future
     are automatically available via the admin interface just by upgrading your
     gRPC version.
 
     Args:
         server: A gRPC server to which all admin services will be added.
     """
     channelz.add_channelz_servicer(server)
     grpc_csds.add_csds_servicer(server)
 
 
-__all__ = ['add_admin_servicers']
+__all__ = ["add_admin_servicers"]
```

### Comparing `grpcio-admin-1.56.2/grpc_version.py` & `grpcio-admin-1.57.0rc1/grpc_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # AUTO-GENERATED FROM `$REPO_ROOT/templates/src/python/grpcio_admin/grpc_version.py.template`!!!
 
-VERSION = '1.56.2'
+VERSION = '1.57.0rc1'
```

### Comparing `grpcio-admin-1.56.2/grpcio_admin.egg-info/PKG-INFO` & `grpcio-admin-1.57.0rc1/grpcio_admin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-admin
-Version: 1.56.2
+Version: 1.57.0rc1
 Summary: a collection of admin services
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `grpcio-admin-1.56.2/setup.py` & `grpcio-admin-1.57.0rc1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,46 +15,48 @@
 
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
-    'grpcio-channelz>={version}'.format(version=grpc_version.VERSION),
-    'grpcio-csds>={version}'.format(version=grpc_version.VERSION),
+    "grpcio-channelz>={version}".format(version=grpc_version.VERSION),
+    "grpcio-csds>={version}".format(version=grpc_version.VERSION),
 )
 SETUP_REQUIRES = INSTALL_REQUIRES
 
-setuptools.setup(name='grpcio-admin',
-                 version=grpc_version.VERSION,
-                 license='Apache License 2.0',
-                 description='a collection of admin services',
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
+    name="grpcio-admin",
+    version=grpc_version.VERSION,
+    license="Apache License 2.0",
+    description="a collection of admin services",
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

